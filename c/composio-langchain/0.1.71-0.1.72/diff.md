# Comparing `tmp/composio_langchain-0.1.71.tar.gz` & `tmp/composio_langchain-0.1.72.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "composio_langchain-0.1.71.tar", last modified: Sat Apr  6 13:21:14 2024, max compression
+gzip compressed data, was "composio_langchain-0.1.72.tar", last modified: Sat Apr  6 13:56:37 2024, max compression
```

## Comparing `composio_langchain-0.1.71.tar` & `composio_langchain-0.1.72.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-06 13:21:14.382871 composio_langchain-0.1.71/
--rw-r--r--   0 utkarsh    (501) staff       (20)        0 2024-03-16 10:20:25.000000 composio_langchain-0.1.71/MANIFEST.in
--rw-r--r--   0 utkarsh    (501) staff       (20)     3337 2024-04-06 13:21:14.382611 composio_langchain-0.1.71/PKG-INFO
--rw-r--r--   0 utkarsh    (501) staff       (20)     2591 2024-04-02 17:07:00.000000 composio_langchain-0.1.71/README.md
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-06 13:21:14.381180 composio_langchain-0.1.71/composio_langchain/
--rw-r--r--   0 utkarsh    (501) staff       (20)       88 2024-03-24 04:08:45.000000 composio_langchain-0.1.71/composio_langchain/__init__.py
--rw-r--r--   0 utkarsh    (501) staff       (20)     5257 2024-04-06 13:18:09.000000 composio_langchain-0.1.71/composio_langchain/composio_tool_spec.py
--rw-r--r--   0 utkarsh    (501) staff       (20)     2804 2024-03-18 18:14:40.000000 composio_langchain-0.1.71/composio_langchain/pydantic_utils.py
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-06 13:21:14.382340 composio_langchain-0.1.71/composio_langchain.egg-info/
--rw-r--r--   0 utkarsh    (501) staff       (20)     3337 2024-04-06 13:21:14.000000 composio_langchain-0.1.71/composio_langchain.egg-info/PKG-INFO
--rw-r--r--   0 utkarsh    (501) staff       (20)      363 2024-04-06 13:21:14.000000 composio_langchain-0.1.71/composio_langchain.egg-info/SOURCES.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)        1 2024-04-06 13:21:14.000000 composio_langchain-0.1.71/composio_langchain.egg-info/dependency_links.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)      152 2024-04-06 13:21:14.000000 composio_langchain-0.1.71/composio_langchain.egg-info/requires.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)       19 2024-04-06 13:21:14.000000 composio_langchain-0.1.71/composio_langchain.egg-info/top_level.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)      458 2024-04-06 13:20:53.000000 composio_langchain-0.1.71/pyproject.toml
--rw-r--r--   0 utkarsh    (501) staff       (20)       38 2024-04-06 13:21:14.382918 composio_langchain-0.1.71/setup.cfg
--rw-r--r--   0 utkarsh    (501) staff       (20)      839 2024-04-06 13:20:53.000000 composio_langchain-0.1.71/setup.py
+drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-06 13:56:37.961677 composio_langchain-0.1.72/
+-rw-r--r--   0 karanvaidya   (501) staff       (20)        0 2024-04-02 18:29:17.000000 composio_langchain-0.1.72/MANIFEST.in
+-rw-r--r--   0 karanvaidya   (501) staff       (20)     3334 2024-04-06 13:56:37.961440 composio_langchain-0.1.72/PKG-INFO
+-rw-r--r--   0 karanvaidya   (501) staff       (20)     2591 2024-04-02 18:29:17.000000 composio_langchain-0.1.72/README.md
+drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-06 13:56:37.960348 composio_langchain-0.1.72/composio_langchain/
+-rw-r--r--   0 karanvaidya   (501) staff       (20)       88 2024-04-02 18:29:17.000000 composio_langchain-0.1.72/composio_langchain/__init__.py
+-rw-r--r--   0 karanvaidya   (501) staff       (20)     5257 2024-04-06 13:52:08.000000 composio_langchain-0.1.72/composio_langchain/composio_tool_spec.py
+-rw-r--r--   0 karanvaidya   (501) staff       (20)     2804 2024-04-02 18:29:17.000000 composio_langchain-0.1.72/composio_langchain/pydantic_utils.py
+drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-06 13:56:37.961206 composio_langchain-0.1.72/composio_langchain.egg-info/
+-rw-r--r--   0 karanvaidya   (501) staff       (20)     3334 2024-04-06 13:56:37.000000 composio_langchain-0.1.72/composio_langchain.egg-info/PKG-INFO
+-rw-r--r--   0 karanvaidya   (501) staff       (20)      363 2024-04-06 13:56:37.000000 composio_langchain-0.1.72/composio_langchain.egg-info/SOURCES.txt
+-rw-r--r--   0 karanvaidya   (501) staff       (20)        1 2024-04-06 13:56:37.000000 composio_langchain-0.1.72/composio_langchain.egg-info/dependency_links.txt
+-rw-r--r--   0 karanvaidya   (501) staff       (20)      149 2024-04-06 13:56:37.000000 composio_langchain-0.1.72/composio_langchain.egg-info/requires.txt
+-rw-r--r--   0 karanvaidya   (501) staff       (20)       19 2024-04-06 13:56:37.000000 composio_langchain-0.1.72/composio_langchain.egg-info/top_level.txt
+-rw-r--r--   0 karanvaidya   (501) staff       (20)      455 2024-04-06 13:56:16.000000 composio_langchain-0.1.72/pyproject.toml
+-rw-r--r--   0 karanvaidya   (501) staff       (20)       38 2024-04-06 13:56:37.961726 composio_langchain-0.1.72/setup.cfg
+-rw-r--r--   0 karanvaidya   (501) staff       (20)      839 2024-04-06 13:56:16.000000 composio_langchain-0.1.72/setup.py
```

### Comparing `composio_langchain-0.1.71/PKG-INFO` & `composio_langchain-0.1.72/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: composio_langchain
-Version: 0.1.71
+Version: 0.1.72
 Summary: Use Composio to get an array of tools with your LangChain agent.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Karan
 Author-email: karan@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: requests
 Requires-Dist: jsonschema
 Requires-Dist: argparse
 Requires-Dist: nest_asyncio
-Requires-Dist: langchain===0.1.0
-Requires-Dist: langchain-openai===0.0.2.post1
-Requires-Dist: langchainhub==0.1.15
-Requires-Dist: pydantic===2.6.4
-Requires-Dist: composio_core===0.1.71
+Requires-Dist: langchain>=0.1.0
+Requires-Dist: langchain-openai>=0.0.2.post1
+Requires-Dist: langchainhub>=0.1.15
+Requires-Dist: pydantic>=2.6.4
+Requires-Dist: composio_core===0.1.72
 
 ## 🦜🔗 Using Composio With LangChain
 
 Integrate Composio with LangChain agents to allow them to interact seamlessly with external apps, enhancing their functionality and reach.
 
 ### Goal
```

### Comparing `composio_langchain-0.1.71/README.md` & `composio_langchain-0.1.72/README.md`

 * *Files identical despite different names*

### Comparing `composio_langchain-0.1.71/composio_langchain/composio_tool_spec.py` & `composio_langchain-0.1.72/composio_langchain/composio_tool_spec.py`

 * *Files identical despite different names*

### Comparing `composio_langchain-0.1.71/composio_langchain/pydantic_utils.py` & `composio_langchain-0.1.72/composio_langchain/pydantic_utils.py`

 * *Files identical despite different names*

### Comparing `composio_langchain-0.1.71/composio_langchain.egg-info/PKG-INFO` & `composio_langchain-0.1.72/composio_langchain.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: composio_langchain
-Version: 0.1.71
+Version: 0.1.72
 Summary: Use Composio to get an array of tools with your LangChain agent.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Karan
 Author-email: karan@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: requests
 Requires-Dist: jsonschema
 Requires-Dist: argparse
 Requires-Dist: nest_asyncio
-Requires-Dist: langchain===0.1.0
-Requires-Dist: langchain-openai===0.0.2.post1
-Requires-Dist: langchainhub==0.1.15
-Requires-Dist: pydantic===2.6.4
-Requires-Dist: composio_core===0.1.71
+Requires-Dist: langchain>=0.1.0
+Requires-Dist: langchain-openai>=0.0.2.post1
+Requires-Dist: langchainhub>=0.1.15
+Requires-Dist: pydantic>=2.6.4
+Requires-Dist: composio_core===0.1.72
 
 ## 🦜🔗 Using Composio With LangChain
 
 Integrate Composio with LangChain agents to allow them to interact seamlessly with external apps, enhancing their functionality and reach.
 
 ### Goal
```

### Comparing `composio_langchain-0.1.71/setup.py` & `composio_langchain-0.1.72/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     return os.path.join(*paths)
 
 
 readme_path = resolve_paths(get_current_dir(), "README.md")
 
 setup(
     name="composio_langchain",
-    version="0.1.71",
+    version="0.1.72",
     author="Karan",
     author_email="karan@composio.dev",
     description="Use Composio to get an array of tools with your LangChain agent.",
     long_description=open(readme_path).read(),
     long_description_content_type="text/markdown",
     url="https://github.com/SamparkAI/composio_sdk",
     classifiers=[
```

