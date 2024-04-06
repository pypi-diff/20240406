# Comparing `tmp/composio_core-0.1.71.tar.gz` & `tmp/composio_core-0.1.72.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "composio_core-0.1.71.tar", last modified: Sat Apr  6 13:21:01 2024, max compression
+gzip compressed data, was "composio_core-0.1.72.tar", last modified: Sat Apr  6 13:56:31 2024, max compression
```

## Comparing `composio_core-0.1.71.tar` & `composio_core-0.1.72.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-06 13:21:01.936219 composio_core-0.1.71/
--rw-r--r--   0 utkarsh    (501) staff       (20)       48 2024-03-15 13:37:31.000000 composio_core-0.1.71/MANIFEST.in
--rw-r--r--   0 utkarsh    (501) staff       (20)      771 2024-04-06 13:21:01.935988 composio_core-0.1.71/PKG-INFO
--rw-r--r--   0 utkarsh    (501) staff       (20)      102 2024-03-16 10:06:01.000000 composio_core-0.1.71/README.md
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-06 13:21:01.933451 composio_core-0.1.71/composio/
--rw-r--r--   0 utkarsh    (501) staff       (20)      176 2024-03-27 14:52:24.000000 composio_core-0.1.71/composio/__init__.py
--rwxr-xr-x   0 utkarsh    (501) staff       (20)    11895 2024-04-06 12:54:36.000000 composio_core-0.1.71/composio/composio_cli.py
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-06 13:21:01.934763 composio_core-0.1.71/composio/sdk/
--rw-r--r--   0 utkarsh    (501) staff       (20)       85 2024-03-27 14:52:24.000000 composio_core-0.1.71/composio/sdk/__init__.py
--rw-r--r--   0 utkarsh    (501) staff       (20)     5542 2024-04-06 12:52:11.000000 composio_core-0.1.71/composio/sdk/core.py
--rw-r--r--   0 utkarsh    (501) staff       (20)     7414 2024-04-04 17:45:19.000000 composio_core-0.1.71/composio/sdk/enums.py
--rw-r--r--   0 utkarsh    (501) staff       (20)    16227 2024-04-06 12:36:58.000000 composio_core-0.1.71/composio/sdk/sdk.py
--rw-r--r--   0 utkarsh    (501) staff       (20)     2210 2024-04-06 12:48:31.000000 composio_core-0.1.71/composio/sdk/storage.py
--rw-r--r--   0 utkarsh    (501) staff       (20)     2861 2024-04-06 12:48:50.000000 composio_core-0.1.71/composio/sdk/utils.py
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-06 13:21:01.935706 composio_core-0.1.71/composio_core.egg-info/
--rw-r--r--   0 utkarsh    (501) staff       (20)      771 2024-04-06 13:21:01.000000 composio_core-0.1.71/composio_core.egg-info/PKG-INFO
--rw-r--r--   0 utkarsh    (501) staff       (20)      466 2024-04-06 13:21:01.000000 composio_core-0.1.71/composio_core.egg-info/SOURCES.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)        1 2024-04-06 13:21:01.000000 composio_core-0.1.71/composio_core.egg-info/dependency_links.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)       60 2024-04-06 13:21:01.000000 composio_core-0.1.71/composio_core.egg-info/entry_points.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)       92 2024-04-06 13:21:01.000000 composio_core-0.1.71/composio_core.egg-info/requires.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)        9 2024-04-06 13:21:01.000000 composio_core-0.1.71/composio_core.egg-info/top_level.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)      510 2024-03-23 19:08:16.000000 composio_core-0.1.71/pyproject.toml
--rw-r--r--   0 utkarsh    (501) staff       (20)       90 2024-03-23 19:08:10.000000 composio_core-0.1.71/requirements.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)       38 2024-04-06 13:21:01.936273 composio_core-0.1.71/setup.cfg
--rw-r--r--   0 utkarsh    (501) staff       (20)     1134 2024-04-06 13:20:53.000000 composio_core-0.1.71/setup.py
+drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-06 13:56:31.390073 composio_core-0.1.72/
+-rw-r--r--   0 karanvaidya   (501) staff       (20)       48 2024-04-02 18:29:17.000000 composio_core-0.1.72/MANIFEST.in
+-rw-r--r--   0 karanvaidya   (501) staff       (20)      770 2024-04-06 13:56:31.389857 composio_core-0.1.72/PKG-INFO
+-rw-r--r--   0 karanvaidya   (501) staff       (20)      102 2024-04-02 18:29:17.000000 composio_core-0.1.72/README.md
+drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-06 13:56:31.386410 composio_core-0.1.72/composio/
+-rw-r--r--   0 karanvaidya   (501) staff       (20)      176 2024-04-02 18:29:17.000000 composio_core-0.1.72/composio/__init__.py
+-rwxr-xr-x   0 karanvaidya   (501) staff       (20)    11895 2024-04-06 13:52:08.000000 composio_core-0.1.72/composio/composio_cli.py
+drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-06 13:56:31.388402 composio_core-0.1.72/composio/sdk/
+-rw-r--r--   0 karanvaidya   (501) staff       (20)       85 2024-04-02 18:29:17.000000 composio_core-0.1.72/composio/sdk/__init__.py
+-rw-r--r--   0 karanvaidya   (501) staff       (20)     5542 2024-04-06 13:52:08.000000 composio_core-0.1.72/composio/sdk/core.py
+-rw-r--r--   0 karanvaidya   (501) staff       (20)     7414 2024-04-04 15:13:54.000000 composio_core-0.1.72/composio/sdk/enums.py
+-rw-r--r--   0 karanvaidya   (501) staff       (20)    16227 2024-04-06 13:52:08.000000 composio_core-0.1.72/composio/sdk/sdk.py
+-rw-r--r--   0 karanvaidya   (501) staff       (20)     2210 2024-04-06 13:52:08.000000 composio_core-0.1.72/composio/sdk/storage.py
+-rw-r--r--   0 karanvaidya   (501) staff       (20)     2861 2024-04-06 13:52:08.000000 composio_core-0.1.72/composio/sdk/utils.py
+drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-06 13:56:31.389609 composio_core-0.1.72/composio_core.egg-info/
+-rw-r--r--   0 karanvaidya   (501) staff       (20)      770 2024-04-06 13:56:31.000000 composio_core-0.1.72/composio_core.egg-info/PKG-INFO
+-rw-r--r--   0 karanvaidya   (501) staff       (20)      466 2024-04-06 13:56:31.000000 composio_core-0.1.72/composio_core.egg-info/SOURCES.txt
+-rw-r--r--   0 karanvaidya   (501) staff       (20)        1 2024-04-06 13:56:31.000000 composio_core-0.1.72/composio_core.egg-info/dependency_links.txt
+-rw-r--r--   0 karanvaidya   (501) staff       (20)       60 2024-04-06 13:56:31.000000 composio_core-0.1.72/composio_core.egg-info/entry_points.txt
+-rw-r--r--   0 karanvaidya   (501) staff       (20)       91 2024-04-06 13:56:31.000000 composio_core-0.1.72/composio_core.egg-info/requires.txt
+-rw-r--r--   0 karanvaidya   (501) staff       (20)        9 2024-04-06 13:56:31.000000 composio_core-0.1.72/composio_core.egg-info/top_level.txt
+-rw-r--r--   0 karanvaidya   (501) staff       (20)      509 2024-04-06 13:53:19.000000 composio_core-0.1.72/pyproject.toml
+-rw-r--r--   0 karanvaidya   (501) staff       (20)       92 2024-04-06 13:54:53.000000 composio_core-0.1.72/requirements.txt
+-rw-r--r--   0 karanvaidya   (501) staff       (20)       38 2024-04-06 13:56:31.390114 composio_core-0.1.72/setup.cfg
+-rw-r--r--   0 karanvaidya   (501) staff       (20)     1134 2024-04-06 13:56:16.000000 composio_core-0.1.72/setup.py
```

### Comparing `composio_core-0.1.71/PKG-INFO` & `composio_core-0.1.72/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: composio_core
-Version: 0.1.71
+Version: 0.1.72
 Summary: Core package to act as a bridge between composio platform and other services.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Utkarsh
 Author-email: utkarsh@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: requests
 Requires-Dist: jsonschema
 Requires-Dist: argparse
-Requires-Dist: beaupy===3.7.2
-Requires-Dist: termcolor==2.4.0
-Requires-Dist: pydantic==2.6.4
-Requires-Dist: openai==1.14.1
+Requires-Dist: beaupy>=3.7.2
+Requires-Dist: termcolor>=2.4.0
+Requires-Dist: pydantic>=2.6.4
+Requires-Dist: openai>=1.14.1
 
 # Composio Core Package
 
 Core package to act as a bridge between composio platform and other services.
```

### Comparing `composio_core-0.1.71/composio/composio_cli.py` & `composio_core-0.1.72/composio/composio_cli.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.1.71/composio/sdk/core.py` & `composio_core-0.1.72/composio/sdk/core.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.1.71/composio/sdk/enums.py` & `composio_core-0.1.72/composio/sdk/enums.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.1.71/composio/sdk/sdk.py` & `composio_core-0.1.72/composio/sdk/sdk.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.1.71/composio/sdk/storage.py` & `composio_core-0.1.72/composio/sdk/storage.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.1.71/composio/sdk/utils.py` & `composio_core-0.1.72/composio/sdk/utils.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.1.71/composio_core.egg-info/PKG-INFO` & `composio_core-0.1.72/composio_core.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: composio_core
-Version: 0.1.71
+Version: 0.1.72
 Summary: Core package to act as a bridge between composio platform and other services.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Utkarsh
 Author-email: utkarsh@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: requests
 Requires-Dist: jsonschema
 Requires-Dist: argparse
-Requires-Dist: beaupy===3.7.2
-Requires-Dist: termcolor==2.4.0
-Requires-Dist: pydantic==2.6.4
-Requires-Dist: openai==1.14.1
+Requires-Dist: beaupy>=3.7.2
+Requires-Dist: termcolor>=2.4.0
+Requires-Dist: pydantic>=2.6.4
+Requires-Dist: openai>=1.14.1
 
 # Composio Core Package
 
 Core package to act as a bridge between composio platform and other services.
```

### Comparing `composio_core-0.1.71/setup.py` & `composio_core-0.1.72/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
     def run(self):
         install.run(self)
 
 
 setup(
     name="composio_core",
-    version="0.1.71",
+    version="0.1.72",
     author="Utkarsh",
     author_email="utkarsh@composio.dev",
     description="Core package to act as a bridge between composio platform and other services.",
     long_description=open(readme_path).read(),
     long_description_content_type="text/markdown",
     url="https://github.com/SamparkAI/composio_sdk",
     classifiers=[
```

