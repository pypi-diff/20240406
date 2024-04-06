# Comparing `tmp/yaml-to-markdown-0.1.1712381225.tar.gz` & `tmp/yaml-to-markdown-0.1.1712382686.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yaml-to-markdown-0.1.1712381225.tar", last modified: Sat Apr  6 05:27:06 2024, max compression
+gzip compressed data, was "yaml-to-markdown-0.1.1712382686.tar", last modified: Sat Apr  6 05:51:27 2024, max compression
```

## Comparing `yaml-to-markdown-0.1.1712381225.tar` & `yaml-to-markdown-0.1.1712382686.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 05:27:06.179115 yaml-to-markdown-0.1.1712381225/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-06 05:26:08.000000 yaml-to-markdown-0.1.1712381225/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-04-06 05:27:06.179115 yaml-to-markdown-0.1.1712381225/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-04-06 05:26:08.000000 yaml-to-markdown-0.1.1712381225/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-06 05:27:06.179115 yaml-to-markdown-0.1.1712381225/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      751 2024-04-06 05:26:08.000000 yaml-to-markdown-0.1.1712381225/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 05:27:06.175115 yaml-to-markdown-0.1.1712381225/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 05:27:06.179115 yaml-to-markdown-0.1.1712381225/src/yaml_to_markdown/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 05:26:08.000000 yaml-to-markdown-0.1.1712381225/src/yaml_to_markdown/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-04-06 05:26:08.000000 yaml-to-markdown-0.1.1712381225/src/yaml_to_markdown/convert.py
--rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-04-06 05:26:08.000000 yaml-to-markdown-0.1.1712381225/src/yaml_to_markdown/convert_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5578 2024-04-06 05:26:08.000000 yaml-to-markdown-0.1.1712381225/src/yaml_to_markdown/md_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     7294 2024-04-06 05:26:08.000000 yaml-to-markdown-0.1.1712381225/src/yaml_to_markdown/md_converter_test.py
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-06 05:26:08.000000 yaml-to-markdown-0.1.1712381225/src/yaml_to_markdown/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-06 05:26:08.000000 yaml-to-markdown-0.1.1712381225/src/yaml_to_markdown/utils_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 05:27:06.179115 yaml-to-markdown-0.1.1712381225/src/yaml_to_markdown.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-04-06 05:27:06.000000 yaml-to-markdown-0.1.1712381225/src/yaml_to_markdown.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-06 05:27:06.000000 yaml-to-markdown-0.1.1712381225/src/yaml_to_markdown.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 05:27:06.000000 yaml-to-markdown-0.1.1712381225/src/yaml_to_markdown.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-06 05:27:06.000000 yaml-to-markdown-0.1.1712381225/src/yaml_to_markdown.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-06 05:27:06.000000 yaml-to-markdown-0.1.1712381225/src/yaml_to_markdown.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-06 05:27:06.000000 yaml-to-markdown-0.1.1712381225/src/yaml_to_markdown.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 05:51:27.089375 yaml-to-markdown-0.1.1712382686/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-06 05:50:32.000000 yaml-to-markdown-0.1.1712382686/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-04-06 05:51:27.089375 yaml-to-markdown-0.1.1712382686/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-04-06 05:50:32.000000 yaml-to-markdown-0.1.1712382686/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-06 05:51:27.089375 yaml-to-markdown-0.1.1712382686/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-06 05:50:32.000000 yaml-to-markdown-0.1.1712382686/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 05:51:27.085375 yaml-to-markdown-0.1.1712382686/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 05:51:27.085375 yaml-to-markdown-0.1.1712382686/src/yaml_to_markdown/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 05:50:32.000000 yaml-to-markdown-0.1.1712382686/src/yaml_to_markdown/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-04-06 05:50:32.000000 yaml-to-markdown-0.1.1712382686/src/yaml_to_markdown/convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-04-06 05:50:32.000000 yaml-to-markdown-0.1.1712382686/src/yaml_to_markdown/convert_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5986 2024-04-06 05:50:32.000000 yaml-to-markdown-0.1.1712382686/src/yaml_to_markdown/md_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7644 2024-04-06 05:50:32.000000 yaml-to-markdown-0.1.1712382686/src/yaml_to_markdown/md_converter_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-06 05:50:32.000000 yaml-to-markdown-0.1.1712382686/src/yaml_to_markdown/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-06 05:50:32.000000 yaml-to-markdown-0.1.1712382686/src/yaml_to_markdown/utils_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 05:51:27.089375 yaml-to-markdown-0.1.1712382686/src/yaml_to_markdown.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-04-06 05:51:26.000000 yaml-to-markdown-0.1.1712382686/src/yaml_to_markdown.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-06 05:51:27.000000 yaml-to-markdown-0.1.1712382686/src/yaml_to_markdown.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 05:51:26.000000 yaml-to-markdown-0.1.1712382686/src/yaml_to_markdown.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-06 05:51:26.000000 yaml-to-markdown-0.1.1712382686/src/yaml_to_markdown.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-06 05:51:26.000000 yaml-to-markdown-0.1.1712382686/src/yaml_to_markdown.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-06 05:51:26.000000 yaml-to-markdown-0.1.1712382686/src/yaml_to_markdown.egg-info/top_level.txt
```

### Comparing `yaml-to-markdown-0.1.1712381225/LICENSE` & `yaml-to-markdown-0.1.1712382686/LICENSE`

 * *Files identical despite different names*

### Comparing `yaml-to-markdown-0.1.1712381225/PKG-INFO` & `yaml-to-markdown-0.1.1712382686/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 Metadata-Version: 2.1
 Name: yaml-to-markdown
-Version: 0.1.1712381225
+Version: 0.1.1712382686
+Summary: Converts a YAML/JSON file or python Dict/List to a Markdown file
 Home-page: https://anevis.github.io/yaml-to-markdown/
 Author: anevis
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: click==8.1.7
 Requires-Dist: jsonschema[format]==4.21.1
@@ -47,20 +48,20 @@
 
 ### From the Command Line
 
 You can also use the command line interface to convert a JSON or YAML file to Markdown. Here's an example:
 
 #### Convert a JSON file to Markdown:
 ```bash
-python yaml_to_markdown/convert.py --output-file output.md --json-file test.json
+yaml-to-markdown --output-file output.md --json-file test.json
 ```
 
 #### Convert a YAML file to Markdown:
 ```bash
-python yaml_to_markdown/convert.py --output-file output.md --yaml-file test.yaml
+yaml-to-markdown --output-file output.md --yaml-file test.yaml
 ```
 
 ## Developer Guide
 Please see the [DEVELOPER.md](docs/DEVELOPER.md) file for more information on how to contribute to this project.
 
 ## License
```

### Comparing `yaml-to-markdown-0.1.1712381225/README.md` & `yaml-to-markdown-0.1.1712382686/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -35,20 +35,20 @@
 
 ### From the Command Line
 
 You can also use the command line interface to convert a JSON or YAML file to Markdown. Here's an example:
 
 #### Convert a JSON file to Markdown:
 ```bash
-python yaml_to_markdown/convert.py --output-file output.md --json-file test.json
+yaml-to-markdown --output-file output.md --json-file test.json
 ```
 
 #### Convert a YAML file to Markdown:
 ```bash
-python yaml_to_markdown/convert.py --output-file output.md --yaml-file test.yaml
+yaml-to-markdown --output-file output.md --yaml-file test.yaml
 ```
 
 ## Developer Guide
 Please see the [DEVELOPER.md](docs/DEVELOPER.md) file for more information on how to contribute to this project.
 
 ## License
```

### Comparing `yaml-to-markdown-0.1.1712381225/setup.py` & `yaml-to-markdown-0.1.1712382686/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="yaml-to-markdown",
     version=f"0.1.{ts}",
+    description="Converts a YAML/JSON file or python Dict/List to a Markdown file",
     packages=find_packages(where="src"),
     package_dir={"": "src"},
     url="https://anevis.github.io/yaml-to-markdown/",
     license="MIT",
     author="anevis",
     install_requires=[
         "click==8.1.7",
```

### Comparing `yaml-to-markdown-0.1.1712381225/src/yaml_to_markdown/convert.py` & `yaml-to-markdown-0.1.1712382686/src/yaml_to_markdown/convert.py`

 * *Files identical despite different names*

### Comparing `yaml-to-markdown-0.1.1712381225/src/yaml_to_markdown/convert_test.py` & `yaml-to-markdown-0.1.1712382686/src/yaml_to_markdown/convert_test.py`

 * *Files identical despite different names*

### Comparing `yaml-to-markdown-0.1.1712381225/src/yaml_to_markdown/md_converter.py` & `yaml-to-markdown-0.1.1712382686/src/yaml_to_markdown/md_converter.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,25 +40,36 @@
         Args:
             custom_processors ([Dict[Callable[[MDConverter, str, Any, int], str]]])
         """
         self._custom_processors = custom_processors
 
     def convert(
         self,
-        data: Dict[str, Union[List[Any], Dict[str, Any], str]],
+        data: Union[Dict[str, Union[List[Any], Dict[str, Any], str]], List[Any]],
         output_writer: IO[str],
     ) -> None:
         """
         Convert the given JSON object into Markdown.
 
         Args:
-            data (Dict[str, Union[List[Any], Dict[str, Any], str]]):
+            data (Union[Dict[str, Union[List[Any], Dict[str, Any], str]], List[Any]]):
+                The JSON object to convert, either a dictionary or a list.
             output_writer (IO[str]):
                 The output stream object to write the Markdown to.
         """
+        if isinstance(data, dict):
+            self._process_dict(data, output_writer)
+        elif isinstance(data, list):
+            self._process_dict({"": data}, output_writer)
+
+    def _process_dict(
+        self,
+        data: Dict[str, Any],
+        output_writer: IO[str],
+    ) -> None:
         for section in self._sections if self._sections is not None else data.keys():
             if section in data:
                 output_writer.write(self.process_section(section, data.get(section)))
 
     def process_section(
         self, section: str, data: Union[List[Any], Dict[str, Any], str], level: int = 2
     ) -> str:
```

### Comparing `yaml-to-markdown-0.1.1712381225/src/yaml_to_markdown/md_converter_test.py` & `yaml-to-markdown-0.1.1712382686/src/yaml_to_markdown/md_converter_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,31 @@
         "col2": "R2C2",
     },
 ]
 _LIST_ITEMS = ["data1", "data2"]
 
 
 class TestMDConverter:
+    def test_process_list(self) -> None:
+        output_writer = StringIO()
+        md_converter = MDConverter()
+        data = [{"section1": "data1"}]
+
+        md_converter.convert(data, output_writer)
+        output = output_writer.getvalue()
+
+        assert (
+            output
+            == """## 
+| Section1 |
+| --- |
+| data1 |
+"""
+        )
+
     def test_process_section_with_str(self) -> None:
         output_writer = StringIO()
         md_converter = MDConverter()
         data = {"section1": "data1"}
 
         md_converter.convert(data, output_writer)
         output = output_writer.getvalue()
```

### Comparing `yaml-to-markdown-0.1.1712381225/src/yaml_to_markdown.egg-info/PKG-INFO` & `yaml-to-markdown-0.1.1712382686/src/yaml_to_markdown.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 Metadata-Version: 2.1
 Name: yaml-to-markdown
-Version: 0.1.1712381225
+Version: 0.1.1712382686
+Summary: Converts a YAML/JSON file or python Dict/List to a Markdown file
 Home-page: https://anevis.github.io/yaml-to-markdown/
 Author: anevis
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: click==8.1.7
 Requires-Dist: jsonschema[format]==4.21.1
@@ -47,20 +48,20 @@
 
 ### From the Command Line
 
 You can also use the command line interface to convert a JSON or YAML file to Markdown. Here's an example:
 
 #### Convert a JSON file to Markdown:
 ```bash
-python yaml_to_markdown/convert.py --output-file output.md --json-file test.json
+yaml-to-markdown --output-file output.md --json-file test.json
 ```
 
 #### Convert a YAML file to Markdown:
 ```bash
-python yaml_to_markdown/convert.py --output-file output.md --yaml-file test.yaml
+yaml-to-markdown --output-file output.md --yaml-file test.yaml
 ```
 
 ## Developer Guide
 Please see the [DEVELOPER.md](docs/DEVELOPER.md) file for more information on how to contribute to this project.
 
 ## License
```

### Comparing `yaml-to-markdown-0.1.1712381225/src/yaml_to_markdown.egg-info/SOURCES.txt` & `yaml-to-markdown-0.1.1712382686/src/yaml_to_markdown.egg-info/SOURCES.txt`

 * *Files identical despite different names*

