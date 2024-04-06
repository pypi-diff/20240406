# Comparing `tmp/composio_langchain-0.1.68.tar.gz` & `tmp/composio_langchain-0.1.69.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "composio_langchain-0.1.68.tar", last modified: Thu Apr  4 17:51:13 2024, max compression
+gzip compressed data, was "composio_langchain-0.1.69.tar", last modified: Sat Apr  6 12:53:57 2024, max compression
```

## Comparing `composio_langchain-0.1.68.tar` & `composio_langchain-0.1.69.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-04 17:51:13.016629 composio_langchain-0.1.68/
--rw-r--r--   0 utkarsh    (501) staff       (20)        0 2024-03-16 10:20:25.000000 composio_langchain-0.1.68/MANIFEST.in
--rw-r--r--   0 utkarsh    (501) staff       (20)     3337 2024-04-04 17:51:13.016399 composio_langchain-0.1.68/PKG-INFO
--rw-r--r--   0 utkarsh    (501) staff       (20)     2591 2024-04-02 17:07:00.000000 composio_langchain-0.1.68/README.md
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-04 17:51:13.015102 composio_langchain-0.1.68/composio_langchain/
--rw-r--r--   0 utkarsh    (501) staff       (20)       88 2024-03-24 04:08:45.000000 composio_langchain-0.1.68/composio_langchain/__init__.py
--rw-r--r--   0 utkarsh    (501) staff       (20)     4943 2024-03-27 14:52:24.000000 composio_langchain-0.1.68/composio_langchain/composio_tool_spec.py
--rw-r--r--   0 utkarsh    (501) staff       (20)     2804 2024-03-18 18:14:40.000000 composio_langchain-0.1.68/composio_langchain/pydantic_utils.py
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-04 17:51:13.016137 composio_langchain-0.1.68/composio_langchain.egg-info/
--rw-r--r--   0 utkarsh    (501) staff       (20)     3337 2024-04-04 17:51:13.000000 composio_langchain-0.1.68/composio_langchain.egg-info/PKG-INFO
--rw-r--r--   0 utkarsh    (501) staff       (20)      363 2024-04-04 17:51:13.000000 composio_langchain-0.1.68/composio_langchain.egg-info/SOURCES.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)        1 2024-04-04 17:51:13.000000 composio_langchain-0.1.68/composio_langchain.egg-info/dependency_links.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)      152 2024-04-04 17:51:13.000000 composio_langchain-0.1.68/composio_langchain.egg-info/requires.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)       19 2024-04-04 17:51:13.000000 composio_langchain-0.1.68/composio_langchain.egg-info/top_level.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)      458 2024-04-04 17:50:54.000000 composio_langchain-0.1.68/pyproject.toml
--rw-r--r--   0 utkarsh    (501) staff       (20)       38 2024-04-04 17:51:13.016678 composio_langchain-0.1.68/setup.cfg
--rw-r--r--   0 utkarsh    (501) staff       (20)      839 2024-04-04 17:50:54.000000 composio_langchain-0.1.68/setup.py
+drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-06 12:53:57.139848 composio_langchain-0.1.69/
+-rw-r--r--   0 utkarsh    (501) staff       (20)        0 2024-03-16 10:20:25.000000 composio_langchain-0.1.69/MANIFEST.in
+-rw-r--r--   0 utkarsh    (501) staff       (20)     3337 2024-04-06 12:53:57.138653 composio_langchain-0.1.69/PKG-INFO
+-rw-r--r--   0 utkarsh    (501) staff       (20)     2591 2024-04-02 17:07:00.000000 composio_langchain-0.1.69/README.md
+drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-06 12:53:57.122993 composio_langchain-0.1.69/composio_langchain/
+-rw-r--r--   0 utkarsh    (501) staff       (20)       88 2024-03-24 04:08:45.000000 composio_langchain-0.1.69/composio_langchain/__init__.py
+-rw-r--r--   0 utkarsh    (501) staff       (20)     4943 2024-03-27 14:52:24.000000 composio_langchain-0.1.69/composio_langchain/composio_tool_spec.py
+-rw-r--r--   0 utkarsh    (501) staff       (20)     2804 2024-03-18 18:14:40.000000 composio_langchain-0.1.69/composio_langchain/pydantic_utils.py
+drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-06 12:53:57.129112 composio_langchain-0.1.69/composio_langchain.egg-info/
+-rw-r--r--   0 utkarsh    (501) staff       (20)     3337 2024-04-06 12:53:57.000000 composio_langchain-0.1.69/composio_langchain.egg-info/PKG-INFO
+-rw-r--r--   0 utkarsh    (501) staff       (20)      363 2024-04-06 12:53:57.000000 composio_langchain-0.1.69/composio_langchain.egg-info/SOURCES.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)        1 2024-04-06 12:53:57.000000 composio_langchain-0.1.69/composio_langchain.egg-info/dependency_links.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)      152 2024-04-06 12:53:57.000000 composio_langchain-0.1.69/composio_langchain.egg-info/requires.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)       19 2024-04-06 12:53:57.000000 composio_langchain-0.1.69/composio_langchain.egg-info/top_level.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)      458 2024-04-06 12:53:03.000000 composio_langchain-0.1.69/pyproject.toml
+-rw-r--r--   0 utkarsh    (501) staff       (20)       38 2024-04-06 12:53:57.139973 composio_langchain-0.1.69/setup.cfg
+-rw-r--r--   0 utkarsh    (501) staff       (20)      839 2024-04-06 12:53:03.000000 composio_langchain-0.1.69/setup.py
```

### Comparing `composio_langchain-0.1.68/PKG-INFO` & `composio_langchain-0.1.69/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: composio_langchain
-Version: 0.1.68
+Version: 0.1.69
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
-Requires-Dist: composio_core===0.1.68
+Requires-Dist: composio_core===0.1.69
 
 ## 🦜🔗 Using Composio With LangChain
 
 Integrate Composio with LangChain agents to allow them to interact seamlessly with external apps, enhancing their functionality and reach.
 
 ### Goal
```

### Comparing `composio_langchain-0.1.68/README.md` & `composio_langchain-0.1.69/README.md`

 * *Files identical despite different names*

### Comparing `composio_langchain-0.1.68/composio_langchain/composio_tool_spec.py` & `composio_langchain-0.1.69/composio_langchain/composio_tool_spec.py`

 * *Files identical despite different names*

### Comparing `composio_langchain-0.1.68/composio_langchain/pydantic_utils.py` & `composio_langchain-0.1.69/composio_langchain/pydantic_utils.py`

 * *Files identical despite different names*

### Comparing `composio_langchain-0.1.68/composio_langchain.egg-info/PKG-INFO` & `composio_langchain-0.1.69/composio_langchain.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: composio_langchain
-Version: 0.1.68
+Version: 0.1.69
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
-Requires-Dist: composio_core===0.1.68
+Requires-Dist: composio_core===0.1.69
 
 ## 🦜🔗 Using Composio With LangChain
 
 Integrate Composio with LangChain agents to allow them to interact seamlessly with external apps, enhancing their functionality and reach.
 
 ### Goal
```

### Comparing `composio_langchain-0.1.68/setup.py` & `composio_langchain-0.1.69/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     return os.path.join(*paths)
 
 
 readme_path = resolve_paths(get_current_dir(), "README.md")
 
 setup(
     name="composio_langchain",
-    version="0.1.68",
+    version="0.1.69",
     author="Karan",
     author_email="karan@composio.dev",
     description="Use Composio to get an array of tools with your LangChain agent.",
     long_description=open(readme_path).read(),
     long_description_content_type="text/markdown",
     url="https://github.com/SamparkAI/composio_sdk",
     classifiers=[
```

