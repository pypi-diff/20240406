# Comparing `tmp/fal_client-0.2.0.tar.gz` & `tmp/fal_client-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fal_client-0.2.0.tar", last modified: Fri Apr  5 20:28:00 2024, max compression
+gzip compressed data, was "fal_client-0.2.1.tar", last modified: Sat Apr  6 05:47:12 2024, max compression
```

## Comparing `fal_client-0.2.0.tar` & `fal_client-0.2.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 isidentical   (501) staff       (20)        0 2024-04-05 20:28:00.009906 fal_client-0.2.0/
--rw-r--r--   0 isidentical   (501) staff       (20)      469 2024-04-05 20:28:00.009638 fal_client-0.2.0/PKG-INFO
--rw-r--r--   0 isidentical   (501) staff       (20)      128 2024-04-05 17:23:39.000000 fal_client-0.2.0/README.md
--rw-r--r--   0 isidentical   (501) staff       (20)      634 2024-04-05 20:27:13.000000 fal_client-0.2.0/pyproject.toml
--rw-r--r--   0 isidentical   (501) staff       (20)       38 2024-04-05 20:28:00.009972 fal_client-0.2.0/setup.cfg
-drwxr-xr-x   0 isidentical   (501) staff       (20)        0 2024-04-05 20:28:00.006750 fal_client-0.2.0/src/
-drwxr-xr-x   0 isidentical   (501) staff       (20)        0 2024-04-05 20:28:00.007953 fal_client-0.2.0/src/fal_client/
--rw-r--r--   0 isidentical   (501) staff       (20)      666 2024-04-05 17:23:39.000000 fal_client-0.2.0/src/fal_client/__init__.py
--rw-r--r--   0 isidentical   (501) staff       (20)      565 2024-04-05 17:23:39.000000 fal_client-0.2.0/src/fal_client/auth.py
--rw-r--r--   0 isidentical   (501) staff       (20)     9580 2024-04-05 20:26:54.000000 fal_client-0.2.0/src/fal_client/client.py
--rw-r--r--   0 isidentical   (501) staff       (20)        0 2024-04-05 17:23:39.000000 fal_client-0.2.0/src/fal_client/py.typed
-drwxr-xr-x   0 isidentical   (501) staff       (20)        0 2024-04-05 20:28:00.009338 fal_client-0.2.0/src/fal_client.egg-info/
--rw-r--r--   0 isidentical   (501) staff       (20)      469 2024-04-05 20:28:00.000000 fal_client-0.2.0/src/fal_client.egg-info/PKG-INFO
--rw-r--r--   0 isidentical   (501) staff       (20)      365 2024-04-05 20:28:00.000000 fal_client-0.2.0/src/fal_client.egg-info/SOURCES.txt
--rw-r--r--   0 isidentical   (501) staff       (20)        1 2024-04-05 20:28:00.000000 fal_client-0.2.0/src/fal_client.egg-info/dependency_links.txt
--rw-r--r--   0 isidentical   (501) staff       (20)       39 2024-04-05 20:28:00.000000 fal_client-0.2.0/src/fal_client.egg-info/requires.txt
--rw-r--r--   0 isidentical   (501) staff       (20)       11 2024-04-05 20:28:00.000000 fal_client-0.2.0/src/fal_client.egg-info/top_level.txt
-drwxr-xr-x   0 isidentical   (501) staff       (20)        0 2024-04-05 20:28:00.009115 fal_client-0.2.0/tests/
--rw-r--r--   0 isidentical   (501) staff       (20)     2465 2024-04-05 20:26:54.000000 fal_client-0.2.0/tests/test_async_client.py
--rw-r--r--   0 isidentical   (501) staff       (20)     2219 2024-04-05 20:26:54.000000 fal_client-0.2.0/tests/test_sync_client.py
+drwxr-xr-x   0 isidentical   (501) staff       (20)        0 2024-04-06 05:47:12.664370 fal_client-0.2.1/
+-rw-r--r--   0 isidentical   (501) staff       (20)     2584 2024-04-06 05:47:12.664056 fal_client-0.2.1/PKG-INFO
+-rw-r--r--   0 isidentical   (501) staff       (20)     2243 2024-04-06 05:45:54.000000 fal_client-0.2.1/README.md
+-rw-r--r--   0 isidentical   (501) staff       (20)      634 2024-04-06 05:46:53.000000 fal_client-0.2.1/pyproject.toml
+-rw-r--r--   0 isidentical   (501) staff       (20)       38 2024-04-06 05:47:12.664429 fal_client-0.2.1/setup.cfg
+drwxr-xr-x   0 isidentical   (501) staff       (20)        0 2024-04-06 05:47:12.660633 fal_client-0.2.1/src/
+drwxr-xr-x   0 isidentical   (501) staff       (20)        0 2024-04-06 05:47:12.662080 fal_client-0.2.1/src/fal_client/
+-rw-r--r--   0 isidentical   (501) staff       (20)      899 2024-04-06 05:04:12.000000 fal_client-0.2.1/src/fal_client/__init__.py
+-rw-r--r--   0 isidentical   (501) staff       (20)      565 2024-04-05 17:23:39.000000 fal_client-0.2.1/src/fal_client/auth.py
+-rw-r--r--   0 isidentical   (501) staff       (20)    13637 2024-04-06 05:39:01.000000 fal_client-0.2.1/src/fal_client/client.py
+-rw-r--r--   0 isidentical   (501) staff       (20)        0 2024-04-05 17:23:39.000000 fal_client-0.2.1/src/fal_client/py.typed
+drwxr-xr-x   0 isidentical   (501) staff       (20)        0 2024-04-06 05:47:12.663731 fal_client-0.2.1/src/fal_client.egg-info/
+-rw-r--r--   0 isidentical   (501) staff       (20)     2584 2024-04-06 05:47:12.000000 fal_client-0.2.1/src/fal_client.egg-info/PKG-INFO
+-rw-r--r--   0 isidentical   (501) staff       (20)      365 2024-04-06 05:47:12.000000 fal_client-0.2.1/src/fal_client.egg-info/SOURCES.txt
+-rw-r--r--   0 isidentical   (501) staff       (20)        1 2024-04-06 05:47:12.000000 fal_client-0.2.1/src/fal_client.egg-info/dependency_links.txt
+-rw-r--r--   0 isidentical   (501) staff       (20)       39 2024-04-06 05:47:12.000000 fal_client-0.2.1/src/fal_client.egg-info/requires.txt
+-rw-r--r--   0 isidentical   (501) staff       (20)       11 2024-04-06 05:47:12.000000 fal_client-0.2.1/src/fal_client.egg-info/top_level.txt
+drwxr-xr-x   0 isidentical   (501) staff       (20)        0 2024-04-06 05:47:12.663299 fal_client-0.2.1/tests/
+-rw-r--r--   0 isidentical   (501) staff       (20)     2465 2024-04-05 20:26:54.000000 fal_client-0.2.1/tests/test_async_client.py
+-rw-r--r--   0 isidentical   (501) staff       (20)     2219 2024-04-05 20:26:54.000000 fal_client-0.2.1/tests/test_sync_client.py
```

### Comparing `fal_client-0.2.0/pyproject.toml` & `fal_client-0.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fal_client"
-version = "0.2.0"
+version = "0.2.1"
 description = "Python client for fal.ai"
 readme = "README.md"
 authors = [{ name = "fal <hello@fal.ai>" }]
 requires-python = ">=3.8"
 dependencies = [
     "httpx>=0.21.0,<1",
     "httpx-sse>=0.4.0,<0.5",
```

### Comparing `fal_client-0.2.0/src/fal_client/__init__.py` & `fal_client-0.2.1/src/fal_client/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -26,12 +26,18 @@
     "stream_async",
 ]
 
 sync_client = SyncClient()
 run = sync_client.run
 submit = sync_client.submit
 stream = sync_client.stream
+upload = sync_client.upload
+upload_file = sync_client.upload_file
+upload_image = sync_client.upload_image
 
 async_client = AsyncClient()
 run_async = async_client.run
 submit_async = async_client.submit
 stream_async = async_client.stream
+upload_async = async_client.upload
+upload_file_async = async_client.upload_file
+upload_image_async = async_client.upload_image
```

### Comparing `fal_client-0.2.0/src/fal_client/auth.py` & `fal_client-0.2.1/src/fal_client/auth.py`

 * *Files identical despite different names*

### Comparing `fal_client-0.2.0/tests/test_async_client.py` & `fal_client-0.2.1/tests/test_async_client.py`

 * *Files identical despite different names*

### Comparing `fal_client-0.2.0/tests/test_sync_client.py` & `fal_client-0.2.1/tests/test_sync_client.py`

 * *Files identical despite different names*

