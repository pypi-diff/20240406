# Comparing `tmp/composio_autogen-0.1.70.tar.gz` & `tmp/composio_autogen-0.1.71.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "composio_autogen-0.1.70.tar", last modified: Sat Apr  6 12:55:59 2024, max compression
+gzip compressed data, was "composio_autogen-0.1.71.tar", last modified: Sat Apr  6 13:21:33 2024, max compression
```

## Comparing `composio_autogen-0.1.70.tar` & `composio_autogen-0.1.71.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-06 12:55:59.902163 composio_autogen-0.1.70/
--rw-r--r--   0 utkarsh    (501) staff       (20)     3309 2024-04-06 12:55:59.901958 composio_autogen-0.1.70/PKG-INFO
--rw-r--r--   0 utkarsh    (501) staff       (20)     2776 2024-04-02 16:44:24.000000 composio_autogen-0.1.70/README.md
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-06 12:55:59.900685 composio_autogen-0.1.70/composio_autogen/
--rw-r--r--   0 utkarsh    (501) staff       (20)       79 2024-03-21 07:30:14.000000 composio_autogen-0.1.70/composio_autogen/__init__.py
--rw-r--r--   0 utkarsh    (501) staff       (20)     6977 2024-04-04 17:45:13.000000 composio_autogen-0.1.70/composio_autogen/autogen_toolspec.py
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-06 12:55:59.901701 composio_autogen-0.1.70/composio_autogen.egg-info/
--rw-r--r--   0 utkarsh    (501) staff       (20)     3309 2024-04-06 12:55:59.000000 composio_autogen-0.1.70/composio_autogen.egg-info/PKG-INFO
--rw-r--r--   0 utkarsh    (501) staff       (20)      298 2024-04-06 12:55:59.000000 composio_autogen-0.1.70/composio_autogen.egg-info/SOURCES.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)        1 2024-04-06 12:55:59.000000 composio_autogen-0.1.70/composio_autogen.egg-info/dependency_links.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)       42 2024-04-06 12:55:59.000000 composio_autogen-0.1.70/composio_autogen.egg-info/requires.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)       17 2024-04-06 12:55:59.000000 composio_autogen-0.1.70/composio_autogen.egg-info/top_level.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)      297 2024-04-06 12:55:25.000000 composio_autogen-0.1.70/pyproject.toml
--rw-r--r--   0 utkarsh    (501) staff       (20)       38 2024-04-06 12:55:59.902212 composio_autogen-0.1.70/setup.cfg
--rw-r--r--   0 utkarsh    (501) staff       (20)      841 2024-04-06 12:55:25.000000 composio_autogen-0.1.70/setup.py
+drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-06 13:21:33.817324 composio_autogen-0.1.71/
+-rw-r--r--   0 utkarsh    (501) staff       (20)     3309 2024-04-06 13:21:33.817078 composio_autogen-0.1.71/PKG-INFO
+-rw-r--r--   0 utkarsh    (501) staff       (20)     2776 2024-04-02 16:44:24.000000 composio_autogen-0.1.71/README.md
+drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-06 13:21:33.816001 composio_autogen-0.1.71/composio_autogen/
+-rw-r--r--   0 utkarsh    (501) staff       (20)       79 2024-03-21 07:30:14.000000 composio_autogen-0.1.71/composio_autogen/__init__.py
+-rw-r--r--   0 utkarsh    (501) staff       (20)     7299 2024-04-06 13:20:20.000000 composio_autogen-0.1.71/composio_autogen/autogen_toolspec.py
+drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-06 13:21:33.816821 composio_autogen-0.1.71/composio_autogen.egg-info/
+-rw-r--r--   0 utkarsh    (501) staff       (20)     3309 2024-04-06 13:21:33.000000 composio_autogen-0.1.71/composio_autogen.egg-info/PKG-INFO
+-rw-r--r--   0 utkarsh    (501) staff       (20)      298 2024-04-06 13:21:33.000000 composio_autogen-0.1.71/composio_autogen.egg-info/SOURCES.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)        1 2024-04-06 13:21:33.000000 composio_autogen-0.1.71/composio_autogen.egg-info/dependency_links.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)       42 2024-04-06 13:21:33.000000 composio_autogen-0.1.71/composio_autogen.egg-info/requires.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)       17 2024-04-06 13:21:33.000000 composio_autogen-0.1.71/composio_autogen.egg-info/top_level.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)      297 2024-04-06 13:20:53.000000 composio_autogen-0.1.71/pyproject.toml
+-rw-r--r--   0 utkarsh    (501) staff       (20)       38 2024-04-06 13:21:33.817371 composio_autogen-0.1.71/setup.cfg
+-rw-r--r--   0 utkarsh    (501) staff       (20)      841 2024-04-06 13:20:53.000000 composio_autogen-0.1.71/setup.py
```

### Comparing `composio_autogen-0.1.70/PKG-INFO` & `composio_autogen-0.1.71/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: composio_autogen
-Version: 0.1.70
+Version: 0.1.71
 Summary: Use Composio to get an array of tools with your Autogen agent.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Sawradip
 Author-email: sawradip@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-Requires-Dist: composio_core===0.1.70
+Requires-Dist: composio_core===0.1.71
 Requires-Dist: pyautogen===0.2.19
 
 # Composio <> Autogen
 Use Composio to enhance your Autogen workflows with a suite of tools.
 
 ## Quick Start
```

### Comparing `composio_autogen-0.1.70/README.md` & `composio_autogen-0.1.71/README.md`

 * *Files identical despite different names*

### Comparing `composio_autogen-0.1.70/composio_autogen/autogen_toolspec.py` & `composio_autogen-0.1.71/composio_autogen/autogen_toolspec.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,52 +23,55 @@
     'integer': 0.0,
     'boolean': False,
     'object': {},
     'array': []
 }
 
 def pydantic_model_from_param_schema(param_schema):
-    fields = {}
+    required_fields = {}
+    optional_fields = {}
+
     param_title = param_schema['title'].replace(" ", "")
     required_props = param_schema.get('required', [])
-    for prop_name, prop_info in param_schema['properties'].items():
+    for prop_name, prop_info in param_schema.get('properties', {}).items():
         prop_type = prop_info["type"]
         prop_title = prop_info['title'].replace(" ", "")
         prop_default = prop_info.get('default', fallback_values[prop_type])
         if prop_type in schema_type_python_type_dict:
             signature_prop_type = schema_type_python_type_dict[prop_type]
         else:
             signature_prop_type = pydantic_model_from_param_schema(prop_info)
 
         if prop_name in required_props:
-            fields[prop_name] = (signature_prop_type, 
+            required_fields[prop_name] = (signature_prop_type, 
                                 Field(..., 
                                     title=prop_title, 
                                     description=prop_info.get('description', 
                                                               prop_info.get('desc', 
                                                                              prop_title))
                                     ))
         else:
-            fields[prop_name] = (signature_prop_type, 
+            optional_fields[prop_name] = (signature_prop_type, 
                                 Field(title=prop_title, 
                                     default=prop_default
                                     ))
-    fieldModel = create_model(param_title, **fields)
+    fieldModel = create_model(param_title, **required_fields, **optional_fields)
     return fieldModel
         
 
     
 
 def get_signature_format_from_schema_params(
         schema_params
 ):
-    parameters = []
+    required_parameters = []
+    optional_parameters = []
     required_params = schema_params.get('required', [])
 
-    for param_name, param_schema in schema_params['properties'].items():
+    for param_name, param_schema in schema_params.get('properties', {}).items():
         param_type = param_schema['type']
         param_title = param_schema['title'].replace(" ", "")
 
         if param_type in schema_type_python_type_dict:
             signature_param_type = schema_type_python_type_dict[param_type]
         else:
             signature_param_type = pydantic_model_from_param_schema(param_schema)
@@ -79,17 +82,21 @@
                                                                                              param_title))]
         param = Parameter(
             name=param_name,
             kind=Parameter.POSITIONAL_OR_KEYWORD,
             annotation=param_annotation,
             default=Parameter.empty if param_name in required_params else param_default 
         )
-        parameters.append(param)
-    return parameters
 
+        is_required = param_name in required_params
+        if is_required:
+            required_parameters.append(param)
+        else:
+            optional_parameters.append(param)
+    return required_parameters + optional_parameters
 
 class ComposioToolset:
     def __init__(self, caller = None, executor = None):
         self.caller = caller
         self.executor = executor
         self.client =  ComposioCore(framework=FrameworkEnum.AUTOGEN)
```

### Comparing `composio_autogen-0.1.70/composio_autogen.egg-info/PKG-INFO` & `composio_autogen-0.1.71/composio_autogen.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: composio_autogen
-Version: 0.1.70
+Version: 0.1.71
 Summary: Use Composio to get an array of tools with your Autogen agent.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Sawradip
 Author-email: sawradip@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-Requires-Dist: composio_core===0.1.70
+Requires-Dist: composio_core===0.1.71
 Requires-Dist: pyautogen===0.2.19
 
 # Composio <> Autogen
 Use Composio to enhance your Autogen workflows with a suite of tools.
 
 ## Quick Start
```

### Comparing `composio_autogen-0.1.70/setup.py` & `composio_autogen-0.1.71/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     return os.path.join(*paths)
 
 
 readme_path = resolve_paths(get_current_dir(), "README.md")
 
 setup(
     name="composio_autogen",
-    version="0.1.70",
+    version="0.1.71",
     author="Sawradip",
     author_email="sawradip@composio.dev",
     description="Use Composio to get an array of tools with your Autogen agent.",
     long_description=open(readme_path).read(),
     long_description_content_type="text/markdown",
     url="https://github.com/SamparkAI/composio_sdk",
     classifiers=[
```

