# Comparing `tmp/composio_autogen-0.1.71.tar.gz` & `tmp/composio_autogen-0.1.72.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "composio_autogen-0.1.71.tar", last modified: Sat Apr  6 13:21:33 2024, max compression
+gzip compressed data, was "composio_autogen-0.1.72.tar", last modified: Sat Apr  6 13:56:49 2024, max compression
```

## Comparing `composio_autogen-0.1.71.tar` & `composio_autogen-0.1.72.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-06 13:21:33.817324 composio_autogen-0.1.71/
--rw-r--r--   0 utkarsh    (501) staff       (20)     3309 2024-04-06 13:21:33.817078 composio_autogen-0.1.71/PKG-INFO
--rw-r--r--   0 utkarsh    (501) staff       (20)     2776 2024-04-02 16:44:24.000000 composio_autogen-0.1.71/README.md
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-06 13:21:33.816001 composio_autogen-0.1.71/composio_autogen/
--rw-r--r--   0 utkarsh    (501) staff       (20)       79 2024-03-21 07:30:14.000000 composio_autogen-0.1.71/composio_autogen/__init__.py
--rw-r--r--   0 utkarsh    (501) staff       (20)     7299 2024-04-06 13:20:20.000000 composio_autogen-0.1.71/composio_autogen/autogen_toolspec.py
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-06 13:21:33.816821 composio_autogen-0.1.71/composio_autogen.egg-info/
--rw-r--r--   0 utkarsh    (501) staff       (20)     3309 2024-04-06 13:21:33.000000 composio_autogen-0.1.71/composio_autogen.egg-info/PKG-INFO
--rw-r--r--   0 utkarsh    (501) staff       (20)      298 2024-04-06 13:21:33.000000 composio_autogen-0.1.71/composio_autogen.egg-info/SOURCES.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)        1 2024-04-06 13:21:33.000000 composio_autogen-0.1.71/composio_autogen.egg-info/dependency_links.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)       42 2024-04-06 13:21:33.000000 composio_autogen-0.1.71/composio_autogen.egg-info/requires.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)       17 2024-04-06 13:21:33.000000 composio_autogen-0.1.71/composio_autogen.egg-info/top_level.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)      297 2024-04-06 13:20:53.000000 composio_autogen-0.1.71/pyproject.toml
--rw-r--r--   0 utkarsh    (501) staff       (20)       38 2024-04-06 13:21:33.817371 composio_autogen-0.1.71/setup.cfg
--rw-r--r--   0 utkarsh    (501) staff       (20)      841 2024-04-06 13:20:53.000000 composio_autogen-0.1.71/setup.py
+drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-06 13:56:49.716268 composio_autogen-0.1.72/
+-rw-r--r--   0 karanvaidya   (501) staff       (20)     3308 2024-04-06 13:56:49.716050 composio_autogen-0.1.72/PKG-INFO
+-rw-r--r--   0 karanvaidya   (501) staff       (20)     2776 2024-04-02 18:29:17.000000 composio_autogen-0.1.72/README.md
+drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-06 13:56:49.714777 composio_autogen-0.1.72/composio_autogen/
+-rw-r--r--   0 karanvaidya   (501) staff       (20)       79 2024-04-02 18:29:17.000000 composio_autogen-0.1.72/composio_autogen/__init__.py
+-rw-r--r--   0 karanvaidya   (501) staff       (20)     7299 2024-04-06 13:52:08.000000 composio_autogen-0.1.72/composio_autogen/autogen_toolspec.py
+drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-06 13:56:49.715793 composio_autogen-0.1.72/composio_autogen.egg-info/
+-rw-r--r--   0 karanvaidya   (501) staff       (20)     3308 2024-04-06 13:56:49.000000 composio_autogen-0.1.72/composio_autogen.egg-info/PKG-INFO
+-rw-r--r--   0 karanvaidya   (501) staff       (20)      298 2024-04-06 13:56:49.000000 composio_autogen-0.1.72/composio_autogen.egg-info/SOURCES.txt
+-rw-r--r--   0 karanvaidya   (501) staff       (20)        1 2024-04-06 13:56:49.000000 composio_autogen-0.1.72/composio_autogen.egg-info/dependency_links.txt
+-rw-r--r--   0 karanvaidya   (501) staff       (20)       41 2024-04-06 13:56:49.000000 composio_autogen-0.1.72/composio_autogen.egg-info/requires.txt
+-rw-r--r--   0 karanvaidya   (501) staff       (20)       17 2024-04-06 13:56:49.000000 composio_autogen-0.1.72/composio_autogen.egg-info/top_level.txt
+-rw-r--r--   0 karanvaidya   (501) staff       (20)      297 2024-04-06 13:56:16.000000 composio_autogen-0.1.72/pyproject.toml
+-rw-r--r--   0 karanvaidya   (501) staff       (20)       38 2024-04-06 13:56:49.716358 composio_autogen-0.1.72/setup.cfg
+-rw-r--r--   0 karanvaidya   (501) staff       (20)      841 2024-04-06 13:56:16.000000 composio_autogen-0.1.72/setup.py
```

### Comparing `composio_autogen-0.1.71/PKG-INFO` & `composio_autogen-0.1.72/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: composio_autogen
-Version: 0.1.71
+Version: 0.1.72
 Summary: Use Composio to get an array of tools with your Autogen agent.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Sawradip
 Author-email: sawradip@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-Requires-Dist: composio_core===0.1.71
-Requires-Dist: pyautogen===0.2.19
+Requires-Dist: composio_core===0.1.72
+Requires-Dist: pyautogen>=0.2.19
 
 # Composio <> Autogen
 Use Composio to enhance your Autogen workflows with a suite of tools.
 
 ## Quick Start
 
 ### Goal
```

### Comparing `composio_autogen-0.1.71/README.md` & `composio_autogen-0.1.72/README.md`

 * *Files identical despite different names*

### Comparing `composio_autogen-0.1.71/composio_autogen/autogen_toolspec.py` & `composio_autogen-0.1.72/composio_autogen/autogen_toolspec.py`

 * *Files identical despite different names*

### Comparing `composio_autogen-0.1.71/composio_autogen.egg-info/PKG-INFO` & `composio_autogen-0.1.72/composio_autogen.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: composio_autogen
-Version: 0.1.71
+Version: 0.1.72
 Summary: Use Composio to get an array of tools with your Autogen agent.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Sawradip
 Author-email: sawradip@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-Requires-Dist: composio_core===0.1.71
-Requires-Dist: pyautogen===0.2.19
+Requires-Dist: composio_core===0.1.72
+Requires-Dist: pyautogen>=0.2.19
 
 # Composio <> Autogen
 Use Composio to enhance your Autogen workflows with a suite of tools.
 
 ## Quick Start
 
 ### Goal
```

### Comparing `composio_autogen-0.1.71/setup.py` & `composio_autogen-0.1.72/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     return os.path.join(*paths)
 
 
 readme_path = resolve_paths(get_current_dir(), "README.md")
 
 setup(
     name="composio_autogen",
-    version="0.1.71",
+    version="0.1.72",
     author="Sawradip",
     author_email="sawradip@composio.dev",
     description="Use Composio to get an array of tools with your Autogen agent.",
     long_description=open(readme_path).read(),
     long_description_content_type="text/markdown",
     url="https://github.com/SamparkAI/composio_sdk",
     classifiers=[
```

