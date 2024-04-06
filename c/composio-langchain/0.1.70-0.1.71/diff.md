# Comparing `tmp/composio_langchain-0.1.70.tar.gz` & `tmp/composio_langchain-0.1.71.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "composio_langchain-0.1.70.tar", last modified: Sat Apr  6 12:55:40 2024, max compression
+gzip compressed data, was "composio_langchain-0.1.71.tar", last modified: Sat Apr  6 13:21:14 2024, max compression
```

## Comparing `composio_langchain-0.1.70.tar` & `composio_langchain-0.1.71.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-06 12:55:40.345824 composio_langchain-0.1.70/
--rw-r--r--   0 utkarsh    (501) staff       (20)        0 2024-03-16 10:20:25.000000 composio_langchain-0.1.70/MANIFEST.in
--rw-r--r--   0 utkarsh    (501) staff       (20)     3337 2024-04-06 12:55:40.345625 composio_langchain-0.1.70/PKG-INFO
--rw-r--r--   0 utkarsh    (501) staff       (20)     2591 2024-04-02 17:07:00.000000 composio_langchain-0.1.70/README.md
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-06 12:55:40.344524 composio_langchain-0.1.70/composio_langchain/
--rw-r--r--   0 utkarsh    (501) staff       (20)       88 2024-03-24 04:08:45.000000 composio_langchain-0.1.70/composio_langchain/__init__.py
--rw-r--r--   0 utkarsh    (501) staff       (20)     4943 2024-03-27 14:52:24.000000 composio_langchain-0.1.70/composio_langchain/composio_tool_spec.py
--rw-r--r--   0 utkarsh    (501) staff       (20)     2804 2024-03-18 18:14:40.000000 composio_langchain-0.1.70/composio_langchain/pydantic_utils.py
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-06 12:55:40.345386 composio_langchain-0.1.70/composio_langchain.egg-info/
--rw-r--r--   0 utkarsh    (501) staff       (20)     3337 2024-04-06 12:55:40.000000 composio_langchain-0.1.70/composio_langchain.egg-info/PKG-INFO
--rw-r--r--   0 utkarsh    (501) staff       (20)      363 2024-04-06 12:55:40.000000 composio_langchain-0.1.70/composio_langchain.egg-info/SOURCES.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)        1 2024-04-06 12:55:40.000000 composio_langchain-0.1.70/composio_langchain.egg-info/dependency_links.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)      152 2024-04-06 12:55:40.000000 composio_langchain-0.1.70/composio_langchain.egg-info/requires.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)       19 2024-04-06 12:55:40.000000 composio_langchain-0.1.70/composio_langchain.egg-info/top_level.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)      458 2024-04-06 12:55:25.000000 composio_langchain-0.1.70/pyproject.toml
--rw-r--r--   0 utkarsh    (501) staff       (20)       38 2024-04-06 12:55:40.345872 composio_langchain-0.1.70/setup.cfg
--rw-r--r--   0 utkarsh    (501) staff       (20)      839 2024-04-06 12:55:25.000000 composio_langchain-0.1.70/setup.py
+drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-06 13:21:14.382871 composio_langchain-0.1.71/
+-rw-r--r--   0 utkarsh    (501) staff       (20)        0 2024-03-16 10:20:25.000000 composio_langchain-0.1.71/MANIFEST.in
+-rw-r--r--   0 utkarsh    (501) staff       (20)     3337 2024-04-06 13:21:14.382611 composio_langchain-0.1.71/PKG-INFO
+-rw-r--r--   0 utkarsh    (501) staff       (20)     2591 2024-04-02 17:07:00.000000 composio_langchain-0.1.71/README.md
+drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-06 13:21:14.381180 composio_langchain-0.1.71/composio_langchain/
+-rw-r--r--   0 utkarsh    (501) staff       (20)       88 2024-03-24 04:08:45.000000 composio_langchain-0.1.71/composio_langchain/__init__.py
+-rw-r--r--   0 utkarsh    (501) staff       (20)     5257 2024-04-06 13:18:09.000000 composio_langchain-0.1.71/composio_langchain/composio_tool_spec.py
+-rw-r--r--   0 utkarsh    (501) staff       (20)     2804 2024-03-18 18:14:40.000000 composio_langchain-0.1.71/composio_langchain/pydantic_utils.py
+drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-06 13:21:14.382340 composio_langchain-0.1.71/composio_langchain.egg-info/
+-rw-r--r--   0 utkarsh    (501) staff       (20)     3337 2024-04-06 13:21:14.000000 composio_langchain-0.1.71/composio_langchain.egg-info/PKG-INFO
+-rw-r--r--   0 utkarsh    (501) staff       (20)      363 2024-04-06 13:21:14.000000 composio_langchain-0.1.71/composio_langchain.egg-info/SOURCES.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)        1 2024-04-06 13:21:14.000000 composio_langchain-0.1.71/composio_langchain.egg-info/dependency_links.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)      152 2024-04-06 13:21:14.000000 composio_langchain-0.1.71/composio_langchain.egg-info/requires.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)       19 2024-04-06 13:21:14.000000 composio_langchain-0.1.71/composio_langchain.egg-info/top_level.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)      458 2024-04-06 13:20:53.000000 composio_langchain-0.1.71/pyproject.toml
+-rw-r--r--   0 utkarsh    (501) staff       (20)       38 2024-04-06 13:21:14.382918 composio_langchain-0.1.71/setup.cfg
+-rw-r--r--   0 utkarsh    (501) staff       (20)      839 2024-04-06 13:20:53.000000 composio_langchain-0.1.71/setup.py
```

### Comparing `composio_langchain-0.1.70/PKG-INFO` & `composio_langchain-0.1.71/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: composio_langchain
-Version: 0.1.70
+Version: 0.1.71
 Summary: Use Composio to get an array of tools with your LangChain agent.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Karan
 Author-email: karan@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -14,15 +14,15 @@
 Requires-Dist: jsonschema
 Requires-Dist: argparse
 Requires-Dist: nest_asyncio
 Requires-Dist: langchain===0.1.0
 Requires-Dist: langchain-openai===0.0.2.post1
 Requires-Dist: langchainhub==0.1.15
 Requires-Dist: pydantic===2.6.4
-Requires-Dist: composio_core===0.1.70
+Requires-Dist: composio_core===0.1.71
 
 ## 🦜🔗 Using Composio With LangChain
 
 Integrate Composio with LangChain agents to allow them to interact seamlessly with external apps, enhancing their functionality and reach.
 
 ### Goal
```

### Comparing `composio_langchain-0.1.70/README.md` & `composio_langchain-0.1.71/README.md`

 * *Files identical despite different names*

### Comparing `composio_langchain-0.1.70/composio_langchain/composio_tool_spec.py` & `composio_langchain-0.1.71/composio_langchain/composio_tool_spec.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,47 +22,50 @@
     'integer': 0.0,
     'boolean': False,
     'object': {},
     'array': []
 }
 
 def pydantic_model_from_param_schema(param_schema):
-    fields = {}
+    required_fields = {}
+    optional_fields = {}
     param_title = param_schema['title'].replace(" ", "")
     required_props = param_schema.get('required', [])
     schema_params_object = param_schema.get('properties', {})
-    for prop_name, prop_info in schema_params_object.items():
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
+
     required_params = schema_params.get('required', [])
     schema_params_object = schema_params.get('properties', {})
     for param_name, param_schema in schema_params_object.items():
         param_type = param_schema['type']
         param_title = param_schema['title'].replace(" ", "")
 
         if param_type in schema_type_python_type_dict:
@@ -76,16 +79,20 @@
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
+        else :
+            optional_parameters.append(param)
+    return required_parameters + optional_parameters
 
     
 def ComposioTool(client : ComposioCore, action_schema: dict[str, any]) ->  StructuredTool:
     name = action_schema["name"]
     description = action_schema["description"]
     parameters = json_schema_to_model(action_schema["parameters"])
     appName = action_schema["appName"]
```

### Comparing `composio_langchain-0.1.70/composio_langchain/pydantic_utils.py` & `composio_langchain-0.1.71/composio_langchain/pydantic_utils.py`

 * *Files identical despite different names*

### Comparing `composio_langchain-0.1.70/composio_langchain.egg-info/PKG-INFO` & `composio_langchain-0.1.71/composio_langchain.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: composio_langchain
-Version: 0.1.70
+Version: 0.1.71
 Summary: Use Composio to get an array of tools with your LangChain agent.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Karan
 Author-email: karan@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -14,15 +14,15 @@
 Requires-Dist: jsonschema
 Requires-Dist: argparse
 Requires-Dist: nest_asyncio
 Requires-Dist: langchain===0.1.0
 Requires-Dist: langchain-openai===0.0.2.post1
 Requires-Dist: langchainhub==0.1.15
 Requires-Dist: pydantic===2.6.4
-Requires-Dist: composio_core===0.1.70
+Requires-Dist: composio_core===0.1.71
 
 ## 🦜🔗 Using Composio With LangChain
 
 Integrate Composio with LangChain agents to allow them to interact seamlessly with external apps, enhancing their functionality and reach.
 
 ### Goal
```

### Comparing `composio_langchain-0.1.70/setup.py` & `composio_langchain-0.1.71/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     return os.path.join(*paths)
 
 
 readme_path = resolve_paths(get_current_dir(), "README.md")
 
 setup(
     name="composio_langchain",
-    version="0.1.70",
+    version="0.1.71",
     author="Karan",
     author_email="karan@composio.dev",
     description="Use Composio to get an array of tools with your LangChain agent.",
     long_description=open(readme_path).read(),
     long_description_content_type="text/markdown",
     url="https://github.com/SamparkAI/composio_sdk",
     classifiers=[
```

