# Comparing `tmp/composio_autogen-0.1.69.tar.gz` & `tmp/composio_autogen-0.1.70.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "composio_autogen-0.1.69.tar", last modified: Sat Apr  6 12:54:18 2024, max compression
+gzip compressed data, was "composio_autogen-0.1.70.tar", last modified: Sat Apr  6 12:55:59 2024, max compression
```

## Comparing `composio_autogen-0.1.69.tar` & `composio_autogen-0.1.70.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-06 12:54:18.564486 composio_autogen-0.1.69/
--rw-r--r--   0 utkarsh    (501) staff       (20)     3309 2024-04-06 12:54:18.564246 composio_autogen-0.1.69/PKG-INFO
--rw-r--r--   0 utkarsh    (501) staff       (20)     2776 2024-04-02 16:44:24.000000 composio_autogen-0.1.69/README.md
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-06 12:54:18.562848 composio_autogen-0.1.69/composio_autogen/
--rw-r--r--   0 utkarsh    (501) staff       (20)       79 2024-03-21 07:30:14.000000 composio_autogen-0.1.69/composio_autogen/__init__.py
--rw-r--r--   0 utkarsh    (501) staff       (20)     6977 2024-04-04 17:45:13.000000 composio_autogen-0.1.69/composio_autogen/autogen_toolspec.py
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-06 12:54:18.563979 composio_autogen-0.1.69/composio_autogen.egg-info/
--rw-r--r--   0 utkarsh    (501) staff       (20)     3309 2024-04-06 12:54:18.000000 composio_autogen-0.1.69/composio_autogen.egg-info/PKG-INFO
--rw-r--r--   0 utkarsh    (501) staff       (20)      298 2024-04-06 12:54:18.000000 composio_autogen-0.1.69/composio_autogen.egg-info/SOURCES.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)        1 2024-04-06 12:54:18.000000 composio_autogen-0.1.69/composio_autogen.egg-info/dependency_links.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)       42 2024-04-06 12:54:18.000000 composio_autogen-0.1.69/composio_autogen.egg-info/requires.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)       17 2024-04-06 12:54:18.000000 composio_autogen-0.1.69/composio_autogen.egg-info/top_level.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)      297 2024-04-06 12:53:03.000000 composio_autogen-0.1.69/pyproject.toml
--rw-r--r--   0 utkarsh    (501) staff       (20)       38 2024-04-06 12:54:18.564541 composio_autogen-0.1.69/setup.cfg
--rw-r--r--   0 utkarsh    (501) staff       (20)      841 2024-04-06 12:53:03.000000 composio_autogen-0.1.69/setup.py
+drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-06 12:55:59.902163 composio_autogen-0.1.70/
+-rw-r--r--   0 utkarsh    (501) staff       (20)     3309 2024-04-06 12:55:59.901958 composio_autogen-0.1.70/PKG-INFO
+-rw-r--r--   0 utkarsh    (501) staff       (20)     2776 2024-04-02 16:44:24.000000 composio_autogen-0.1.70/README.md
+drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-06 12:55:59.900685 composio_autogen-0.1.70/composio_autogen/
+-rw-r--r--   0 utkarsh    (501) staff       (20)       79 2024-03-21 07:30:14.000000 composio_autogen-0.1.70/composio_autogen/__init__.py
+-rw-r--r--   0 utkarsh    (501) staff       (20)     6977 2024-04-04 17:45:13.000000 composio_autogen-0.1.70/composio_autogen/autogen_toolspec.py
+drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-06 12:55:59.901701 composio_autogen-0.1.70/composio_autogen.egg-info/
+-rw-r--r--   0 utkarsh    (501) staff       (20)     3309 2024-04-06 12:55:59.000000 composio_autogen-0.1.70/composio_autogen.egg-info/PKG-INFO
+-rw-r--r--   0 utkarsh    (501) staff       (20)      298 2024-04-06 12:55:59.000000 composio_autogen-0.1.70/composio_autogen.egg-info/SOURCES.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)        1 2024-04-06 12:55:59.000000 composio_autogen-0.1.70/composio_autogen.egg-info/dependency_links.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)       42 2024-04-06 12:55:59.000000 composio_autogen-0.1.70/composio_autogen.egg-info/requires.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)       17 2024-04-06 12:55:59.000000 composio_autogen-0.1.70/composio_autogen.egg-info/top_level.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)      297 2024-04-06 12:55:25.000000 composio_autogen-0.1.70/pyproject.toml
+-rw-r--r--   0 utkarsh    (501) staff       (20)       38 2024-04-06 12:55:59.902212 composio_autogen-0.1.70/setup.cfg
+-rw-r--r--   0 utkarsh    (501) staff       (20)      841 2024-04-06 12:55:25.000000 composio_autogen-0.1.70/setup.py
```

### Comparing `composio_autogen-0.1.69/PKG-INFO` & `composio_autogen-0.1.70/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: composio_autogen
-Version: 0.1.69
+Version: 0.1.70
 Summary: Use Composio to get an array of tools with your Autogen agent.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Sawradip
 Author-email: sawradip@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-Requires-Dist: composio_core===0.1.69
+Requires-Dist: composio_core===0.1.70
 Requires-Dist: pyautogen===0.2.19
 
 # Composio <> Autogen
 Use Composio to enhance your Autogen workflows with a suite of tools.
 
 ## Quick Start
```

### Comparing `composio_autogen-0.1.69/README.md` & `composio_autogen-0.1.70/README.md`

 * *Files identical despite different names*

### Comparing `composio_autogen-0.1.69/composio_autogen/autogen_toolspec.py` & `composio_autogen-0.1.70/composio_autogen/autogen_toolspec.py`

 * *Files identical despite different names*

### Comparing `composio_autogen-0.1.69/composio_autogen.egg-info/PKG-INFO` & `composio_autogen-0.1.70/composio_autogen.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: composio_autogen
-Version: 0.1.69
+Version: 0.1.70
 Summary: Use Composio to get an array of tools with your Autogen agent.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Sawradip
 Author-email: sawradip@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-Requires-Dist: composio_core===0.1.69
+Requires-Dist: composio_core===0.1.70
 Requires-Dist: pyautogen===0.2.19
 
 # Composio <> Autogen
 Use Composio to enhance your Autogen workflows with a suite of tools.
 
 ## Quick Start
```

### Comparing `composio_autogen-0.1.69/setup.py` & `composio_autogen-0.1.70/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     return os.path.join(*paths)
 
 
 readme_path = resolve_paths(get_current_dir(), "README.md")
 
 setup(
     name="composio_autogen",
-    version="0.1.69",
+    version="0.1.70",
     author="Sawradip",
     author_email="sawradip@composio.dev",
     description="Use Composio to get an array of tools with your Autogen agent.",
     long_description=open(readme_path).read(),
     long_description_content_type="text/markdown",
     url="https://github.com/SamparkAI/composio_sdk",
     classifiers=[
```

