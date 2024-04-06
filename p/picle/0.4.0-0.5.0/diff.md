# Comparing `tmp/picle-0.4.0.tar.gz` & `tmp/picle-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "picle-0.4.0.tar", max compression
+gzip compressed data, was "picle-0.5.0.tar", max compression
```

## Comparing `picle-0.4.0.tar` & `picle-0.5.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1071 2023-01-01 02:30:45.840067 picle-0.4.0/LICENSE
--rw-r--r--   0        0        0       80 2024-04-05 01:13:50.673276 picle-0.4.0/picle/__init__.py
--rw-r--r--   0        0        0     4531 2024-03-16 10:14:19.744008 picle-0.4.0/picle/cache.py
--rw-r--r--   0        0        0     3193 2024-04-05 08:48:59.627598 picle-0.4.0/picle/models.py
--rw-r--r--   0        0        0    28317 2024-04-05 08:48:59.808228 picle-0.4.0/picle/picle.py
--rw-r--r--   0        0        0      354 2024-04-05 03:31:06.926191 picle-0.4.0/picle/utils.py
--rw-r--r--   0        0        0     1529 2024-04-05 08:48:38.046270 picle-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     1329 2024-03-19 10:44:18.402593 picle-0.4.0/README.md
--rw-r--r--   0        0        0     2737 1970-01-01 00:00:00.000000 picle-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-01-01 02:30:45.840067 picle-0.5.0/LICENSE
+-rw-r--r--   0        0        0       80 2024-04-05 01:13:50.673276 picle-0.5.0/picle/__init__.py
+-rw-r--r--   0        0        0     4531 2024-03-16 10:14:19.744008 picle-0.5.0/picle/cache.py
+-rw-r--r--   0        0        0     4823 2024-04-06 11:10:27.404727 picle-0.5.0/picle/models.py
+-rw-r--r--   0        0        0    30639 2024-04-06 11:04:50.221061 picle-0.5.0/picle/picle.py
+-rw-r--r--   0        0        0      354 2024-04-05 03:31:06.926191 picle-0.5.0/picle/utils.py
+-rw-r--r--   0        0        0     1659 2024-04-06 11:25:19.042963 picle-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     1329 2024-03-19 10:44:18.402593 picle-0.5.0/README.md
+-rw-r--r--   0        0        0     2816 1970-01-01 00:00:00.000000 picle-0.5.0/PKG-INFO
```

### Comparing `picle-0.4.0/LICENSE` & `picle-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `picle-0.4.0/picle/cache.py` & `picle-0.5.0/picle/cache.py`

 * *Files identical despite different names*

### Comparing `picle-0.4.0/picle/models.py` & `picle-0.5.0/picle/models.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,30 @@
-from pprint import pformat
-from json import dumps as json_dumps
+import json
+import pprint
+
 from typing import List, Union, Optional, Callable, Any
 from pydantic import ValidationError, BaseModel, StrictStr, Field, StrictBool, StrictInt
 
 try:
     from yaml import dump as yaml_dump
 
     HAS_YAML = True
 except ImportError:
     HAS_YAML = False
 
+try:
+    from rich.console import Console as rich_console
+    from rich.table import Table as rich_table
+    from rich.pretty import pprint as rich_pprint
+
+    RICHCONSOLE = rich_console()
+    HAS_RICH = True
+except ImportError:
+    HAS_RICH = False
+
 
 class Filters(BaseModel):
     include: Any = Field(
         None,
         description="Filter output by pattern inclusion",
         json_schema_extra={"function": "filter_include"},
     )
@@ -71,38 +82,85 @@
     @staticmethod
     def formatter_pprint(data: Any) -> str:
         """
         Function to pretty print results using python ``pprint`` module
 
         :param data: any data to pretty print
         """
-        return pformat(data, indent=4)
+        return pprint.pformat(data, indent=4)
 
     @staticmethod
     def formatter_json(data: Any) -> str:
         """
         Function to transform results into JSON string
 
         :param data: any data to convert
         """
-        return json_dumps(data, indent=4, sort_keys=True)
+        return json.dumps(data, indent=4, sort_keys=True)
 
     @staticmethod
     def formatter_yaml(data: Any) -> str:
         """
         Function to transform results into YAML string
 
         :param data: any data to convert
         """
         if HAS_YAML:
             return yaml_dump(data, default_flow_style=False)
         else:
             return data
 
 
-class PipeFunctionsModel(Filters, Formatters):
+class Outputters(BaseModel):
+    rich_json: Union[dict, list] = Field(
+        None,
+        description="Pretty print JSON string using Rich",
+        json_schema_extra={"function": "outputter_rich_json"},
+    )
+    rich_print: Any = Field(
+        None,
+        description="Pretty print output using Rich",
+        json_schema_extra={"function": "outputter_rich_print"},
+    )
+
+    @staticmethod
+    def outputter_rich_json(data: Union[dict, list]) -> None:
+        """
+        Function to pretty print JSON string using Rich library
+
+        :param data: any data to print
+        """
+        if isinstance(data, bytes):
+            data = data.decode("utf-8")
+
+        if not isinstance(data, str):
+            data = json.dumps(data)
+
+        # data should be a json string
+        try:
+            if HAS_RICH:
+                RICHCONSOLE.print_json(data, sort_keys=True, indent=4)
+            else:
+                print(data)
+        except Exception as e:
+            print(f"ERROR: Data is not a valid JSON string: '{data}', error: '{e}'")
+
+    @staticmethod
+    def outputter_rich_print(data: Any) -> None:
+        """
+        Function to pretty print output using Rich library
+
+        :param data: any data to print
+        """
+        if HAS_RICH:
+            RICHCONSOLE.print(data)
+        else:
+            print(data)
+
+
+class PipeFunctionsModel(Filters, Formatters, Outputters):
     """
     Collection of common pipe functions to use in PICLE shell models
     """
 
     class PicleConfig:
         pipe = "self"
```

### Comparing `picle-0.4.0/picle/picle.py` & `picle-0.5.0/picle/picle.py`

 * *Files 4% similar despite different names*

```diff
@@ -521,14 +521,15 @@
         for shell in self.shells[1:]:
             path.append(shell.__name__)
         self.write("->".join(path))
 
     def default(self, line: str):
         """Method called if no do_xyz methods found"""
         ret = False
+        outputter = None
 
         # print help for given command or commands
         if line.strip().endswith("?"):
             try:
                 command_models = self.parse_command(line.strip().rstrip("?"))
             except FieldLooseMatchOnly as e:
                 model, parameter = e.args
@@ -595,14 +596,28 @@
                     if run_kwargs and hasattr(model, "run"):
                         # call first command using collected arguments only
                         if index == 0:
                             ret = model.run(**run_kwargs)
                         # pipe results through subsequent commands
                         else:
                             ret = model.run(ret, **run_kwargs)
+                        # run processors from PicleConfig if any for first command only
+                        if index == 0:
+                            if hasattr(model, "PicleConfig") and hasattr(
+                                model.PicleConfig, "processors"
+                            ):
+                                for processor in model.PicleConfig.processors:
+                                    if callable(processor):
+                                        ret = processor(ret)
+                        # extract outputter from PicleConfig
+                        if index == 0:
+                            if hasattr(model, "PicleConfig") and hasattr(
+                                model.PicleConfig, "outputter"
+                            ):
+                                outputter = model.PicleConfig.outputter
                     # check if model has subshell
                     elif (
                         hasattr(model, "PicleConfig")
                         and getattr(model.PicleConfig, "subshell", None) is True
                     ):
                         # collect parent shells
                         for item in command[:-1]:
@@ -613,14 +628,15 @@
                             ):
                                 if m not in self.shells:
                                     self.shells.append(m)
                         # update prompt value
                         self.prompt = getattr(model.PicleConfig, "prompt", self.prompt)
                         self.shell = model
                         self.shells.append(self.shell)
+                    # run command via reference function
                     elif command[-1]["fields"]:
                         last_field_name = command[-1]["fields"][-1]["name"]
                         last_field = model.model_fields[last_field_name]
                         json_schema_extra = (
                             getattr(last_field, "json_schema_extra") or {}
                         )
                         # check if last field refers to callable e.g. function
@@ -653,20 +669,44 @@
                                     f"Model '{model.__name__}' has no '{method_name}' "
                                     f"method defined for '{last_field_name}' function"
                                 )
                         else:
                             self.write(
                                 f"Model '{model.__name__}' has no 'run' method defined"
                             )
-                        # run result through processors if any
-                        for processor in json_schema_extra.get("processors", []):
-                            ret = processor(ret)
+                        # use processors from Field definition if any
+                        if json_schema_extra.get("processors"):
+                            for processor in json_schema_extra["processors"]:
+                                if callable(processor):
+                                    ret = processor(ret)
+                        # run processors from PicleConfig if any for first command only
+                        if index == 0:
+                            if hasattr(model, "PicleConfig") and hasattr(
+                                model.PicleConfig, "processors"
+                            ):
+                                for processor in model.PicleConfig.processors:
+                                    if callable(processor):
+                                        ret = processor(ret)
+                        # extract outputter from first command
+                        if index == 0:
+                            # use outputter from Field definition
+                            if json_schema_extra.get("outputter"):
+                                outputter = json_schema_extra["outputter"]
+                            # use PicleConfig outputter
+                            elif hasattr(model, "PicleConfig") and hasattr(
+                                model.PicleConfig, "outputter"
+                            ):
+                                outputter = model.PicleConfig.outputter
                     else:
                         self.write(f"Incorrect command")
-                        continue
+                        return
 
-        # returning True will close the shell
+        # returning True will close the shell exit
         if ret is True:
             return True
         elif ret:
-            self.write(ret)
-        return None
+            # use specified outputter to output results
+            if callable(outputter):
+                outputter(ret)
+            # write to stdout by default
+            else:
+                self.write(ret)
```

### Comparing `picle-0.4.0/pyproject.toml` & `picle-0.5.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "picle"
-version = "0.4.0"
+version = "0.5.0"
 description = "Python Interactive Command Line Shells"
 authors = ["Denis Mulyalin <d.mulyalin@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/dmulyalin/picle"
 repository = "https://github.com/dmulyalin/picle"
 documentation = "https://dmulyalin.github.io/picle/"
@@ -18,14 +18,17 @@
 mkdocs = { version = "1.2.4", optional = true, markers = "python_version >= '3.7'" }
 mkdocs-material = { version = "7.2.2", optional = true, markers = "python_version >= '3.7'" }
 mkdocs-material-extensions = { version = "1.0.1", optional = true, markers = "python_version >= '3.7'" }
 mkdocstrings = { version = "0.18.*", optional = true, markers = "python_version >= '3.7'", extras = ["python"] } 
 pygments = { version = "2.11", optional = true, markers = "python_version >= '3.7'" }
 pymdown-extensions = { version = "9.3", optional = true, markers = "python_version >= '3.7'" }
 
+# optional dependencies for extras definition
+rich = { version = ">=13.0.0,<=14.0.0", optional = true }
+
 [tool.poetry.dev-dependencies]
 black = "22.3.*"
 pytest = { version = "7.1.*", markers = "python_version >= '3.7'" }
 ipdb = ">=0.0.0, <=1.0.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
@@ -35,8 +38,11 @@
 docs = [
     "mkdocs",
     "mkdocs-material",
     "mkdocs-material-extensions",
     "mkdocstrings",
     "pygments",
     "pymdown-extensions",
+]
+full = [
+	"rich"
 ]
```

### Comparing `picle-0.4.0/README.md` & `picle-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `picle-0.4.0/PKG-INFO` & `picle-0.5.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 Metadata-Version: 2.1
 Name: picle
-Version: 0.4.0
+Version: 0.5.0
 Summary: Python Interactive Command Line Shells
 Home-page: https://github.com/dmulyalin/picle
 License: MIT
 Author: Denis Mulyalin
 Author-email: d.mulyalin@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: docs
+Provides-Extra: full
 Requires-Dist: mkdocs (==1.2.4) ; (python_version >= "3.7") and (extra == "docs")
 Requires-Dist: mkdocs-material (==7.2.2) ; (python_version >= "3.7") and (extra == "docs")
 Requires-Dist: mkdocs-material-extensions (==1.0.1) ; (python_version >= "3.7") and (extra == "docs")
 Requires-Dist: mkdocstrings[python] (>=0.18.0,<0.19.0) ; (python_version >= "3.7") and (extra == "docs")
 Requires-Dist: pydantic (>=2.0.1,<=3.0.0)
 Requires-Dist: pygments (==2.11) ; (python_version >= "3.7") and (extra == "docs")
 Requires-Dist: pymdown-extensions (==9.3) ; (python_version >= "3.7") and (extra == "docs")
 Requires-Dist: pyreadline3 (==3.4.1) ; sys_platform == "win32"
+Requires-Dist: rich (>=13.0.0,<=14.0.0) ; extra == "full"
 Project-URL: Documentation, https://dmulyalin.github.io/picle/
 Project-URL: Repository, https://github.com/dmulyalin/picle
 Description-Content-Type: text/markdown
 
 # PICLE - Python Interactive Command Line Shells
 
 PICLE is a module to construct interactive command line shell
```

