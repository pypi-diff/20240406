# Comparing `tmp/composio_core-0.1.69.tar.gz` & `tmp/composio_core-0.1.70.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "composio_core-0.1.69.tar", last modified: Sat Apr  6 12:53:46 2024, max compression
+gzip compressed data, was "composio_core-0.1.70.tar", last modified: Sat Apr  6 12:55:29 2024, max compression
```

## Comparing `composio_core-0.1.69.tar` & `composio_core-0.1.70.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-06 12:53:46.046623 composio_core-0.1.69/
--rw-r--r--   0 utkarsh    (501) staff       (20)       48 2024-03-15 13:37:31.000000 composio_core-0.1.69/MANIFEST.in
--rw-r--r--   0 utkarsh    (501) staff       (20)      771 2024-04-06 12:53:46.046283 composio_core-0.1.69/PKG-INFO
--rw-r--r--   0 utkarsh    (501) staff       (20)      102 2024-03-16 10:06:01.000000 composio_core-0.1.69/README.md
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-06 12:53:46.043448 composio_core-0.1.69/composio/
--rw-r--r--   0 utkarsh    (501) staff       (20)      176 2024-03-27 14:52:24.000000 composio_core-0.1.69/composio/__init__.py
--rwxr-xr-x   0 utkarsh    (501) staff       (20)    11902 2024-04-06 12:52:24.000000 composio_core-0.1.69/composio/composio_cli.py
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-06 12:53:46.044738 composio_core-0.1.69/composio/sdk/
--rw-r--r--   0 utkarsh    (501) staff       (20)       85 2024-03-27 14:52:24.000000 composio_core-0.1.69/composio/sdk/__init__.py
--rw-r--r--   0 utkarsh    (501) staff       (20)     5542 2024-04-06 12:52:11.000000 composio_core-0.1.69/composio/sdk/core.py
--rw-r--r--   0 utkarsh    (501) staff       (20)     7414 2024-04-04 17:45:19.000000 composio_core-0.1.69/composio/sdk/enums.py
--rw-r--r--   0 utkarsh    (501) staff       (20)    16227 2024-04-06 12:36:58.000000 composio_core-0.1.69/composio/sdk/sdk.py
--rw-r--r--   0 utkarsh    (501) staff       (20)     2210 2024-04-06 12:48:31.000000 composio_core-0.1.69/composio/sdk/storage.py
--rw-r--r--   0 utkarsh    (501) staff       (20)     2861 2024-04-06 12:48:50.000000 composio_core-0.1.69/composio/sdk/utils.py
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-06 12:53:46.045985 composio_core-0.1.69/composio_core.egg-info/
--rw-r--r--   0 utkarsh    (501) staff       (20)      771 2024-04-06 12:53:46.000000 composio_core-0.1.69/composio_core.egg-info/PKG-INFO
--rw-r--r--   0 utkarsh    (501) staff       (20)      466 2024-04-06 12:53:46.000000 composio_core-0.1.69/composio_core.egg-info/SOURCES.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)        1 2024-04-06 12:53:46.000000 composio_core-0.1.69/composio_core.egg-info/dependency_links.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)       60 2024-04-06 12:53:46.000000 composio_core-0.1.69/composio_core.egg-info/entry_points.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)       92 2024-04-06 12:53:46.000000 composio_core-0.1.69/composio_core.egg-info/requires.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)        9 2024-04-06 12:53:46.000000 composio_core-0.1.69/composio_core.egg-info/top_level.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)      510 2024-03-23 19:08:16.000000 composio_core-0.1.69/pyproject.toml
--rw-r--r--   0 utkarsh    (501) staff       (20)       90 2024-03-23 19:08:10.000000 composio_core-0.1.69/requirements.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)       38 2024-04-06 12:53:46.046695 composio_core-0.1.69/setup.cfg
--rw-r--r--   0 utkarsh    (501) staff       (20)     1134 2024-04-06 12:53:03.000000 composio_core-0.1.69/setup.py
+drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-06 12:55:29.705673 composio_core-0.1.70/
+-rw-r--r--   0 utkarsh    (501) staff       (20)       48 2024-03-15 13:37:31.000000 composio_core-0.1.70/MANIFEST.in
+-rw-r--r--   0 utkarsh    (501) staff       (20)      771 2024-04-06 12:55:29.704714 composio_core-0.1.70/PKG-INFO
+-rw-r--r--   0 utkarsh    (501) staff       (20)      102 2024-03-16 10:06:01.000000 composio_core-0.1.70/README.md
+drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-06 12:55:29.700394 composio_core-0.1.70/composio/
+-rw-r--r--   0 utkarsh    (501) staff       (20)      176 2024-03-27 14:52:24.000000 composio_core-0.1.70/composio/__init__.py
+-rwxr-xr-x   0 utkarsh    (501) staff       (20)    11895 2024-04-06 12:54:36.000000 composio_core-0.1.70/composio/composio_cli.py
+drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-06 12:55:29.701325 composio_core-0.1.70/composio/sdk/
+-rw-r--r--   0 utkarsh    (501) staff       (20)       85 2024-03-27 14:52:24.000000 composio_core-0.1.70/composio/sdk/__init__.py
+-rw-r--r--   0 utkarsh    (501) staff       (20)     5542 2024-04-06 12:52:11.000000 composio_core-0.1.70/composio/sdk/core.py
+-rw-r--r--   0 utkarsh    (501) staff       (20)     7414 2024-04-04 17:45:19.000000 composio_core-0.1.70/composio/sdk/enums.py
+-rw-r--r--   0 utkarsh    (501) staff       (20)    16227 2024-04-06 12:36:58.000000 composio_core-0.1.70/composio/sdk/sdk.py
+-rw-r--r--   0 utkarsh    (501) staff       (20)     2210 2024-04-06 12:48:31.000000 composio_core-0.1.70/composio/sdk/storage.py
+-rw-r--r--   0 utkarsh    (501) staff       (20)     2861 2024-04-06 12:48:50.000000 composio_core-0.1.70/composio/sdk/utils.py
+drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-06 12:55:29.704204 composio_core-0.1.70/composio_core.egg-info/
+-rw-r--r--   0 utkarsh    (501) staff       (20)      771 2024-04-06 12:55:29.000000 composio_core-0.1.70/composio_core.egg-info/PKG-INFO
+-rw-r--r--   0 utkarsh    (501) staff       (20)      466 2024-04-06 12:55:29.000000 composio_core-0.1.70/composio_core.egg-info/SOURCES.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)        1 2024-04-06 12:55:29.000000 composio_core-0.1.70/composio_core.egg-info/dependency_links.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)       60 2024-04-06 12:55:29.000000 composio_core-0.1.70/composio_core.egg-info/entry_points.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)       92 2024-04-06 12:55:29.000000 composio_core-0.1.70/composio_core.egg-info/requires.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)        9 2024-04-06 12:55:29.000000 composio_core-0.1.70/composio_core.egg-info/top_level.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)      510 2024-03-23 19:08:16.000000 composio_core-0.1.70/pyproject.toml
+-rw-r--r--   0 utkarsh    (501) staff       (20)       90 2024-03-23 19:08:10.000000 composio_core-0.1.70/requirements.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)       38 2024-04-06 12:55:29.705735 composio_core-0.1.70/setup.cfg
+-rw-r--r--   0 utkarsh    (501) staff       (20)     1134 2024-04-06 12:55:25.000000 composio_core-0.1.70/setup.py
```

### Comparing `composio_core-0.1.69/PKG-INFO` & `composio_core-0.1.70/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: composio_core
-Version: 0.1.69
+Version: 0.1.70
 Summary: Core package to act as a bridge between composio platform and other services.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Utkarsh
 Author-email: utkarsh@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `composio_core-0.1.69/composio/composio_cli.py` & `composio_core-0.1.70/composio/composio_cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -253,9 +253,7 @@
         console.print(f"[red]Error occurred during user identification: {e}[/red]")
         sys.exit(1)
 
     if hasattr(args, 'func'):
         args.func(args)
     else:
         console.print("[red]Error: No valid command provided. Use --help for more information.[/red]")
-
-main()
```

### Comparing `composio_core-0.1.69/composio/sdk/core.py` & `composio_core-0.1.70/composio/sdk/core.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.1.69/composio/sdk/enums.py` & `composio_core-0.1.70/composio/sdk/enums.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.1.69/composio/sdk/sdk.py` & `composio_core-0.1.70/composio/sdk/sdk.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.1.69/composio/sdk/storage.py` & `composio_core-0.1.70/composio/sdk/storage.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.1.69/composio/sdk/utils.py` & `composio_core-0.1.70/composio/sdk/utils.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.1.69/composio_core.egg-info/PKG-INFO` & `composio_core-0.1.70/composio_core.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: composio_core
-Version: 0.1.69
+Version: 0.1.70
 Summary: Core package to act as a bridge between composio platform and other services.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Utkarsh
 Author-email: utkarsh@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `composio_core-0.1.69/setup.py` & `composio_core-0.1.70/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
     def run(self):
         install.run(self)
 
 
 setup(
     name="composio_core",
-    version="0.1.69",
+    version="0.1.70",
     author="Utkarsh",
     author_email="utkarsh@composio.dev",
     description="Core package to act as a bridge between composio platform and other services.",
     long_description=open(readme_path).read(),
     long_description_content_type="text/markdown",
     url="https://github.com/SamparkAI/composio_sdk",
     classifiers=[
```

