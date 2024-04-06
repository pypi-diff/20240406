# Comparing `tmp/pypdl-1.3.1.tar.gz` & `tmp/pypdl-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypdl-1.3.1.tar", last modified: Tue Mar 12 15:16:04 2024, max compression
+gzip compressed data, was "pypdl-1.3.2.tar", last modified: Sat Apr  6 07:52:39 2024, max compression
```

## Comparing `pypdl-1.3.1.tar` & `pypdl-1.3.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 15:16:04.267289 pypdl-1.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-03-12 15:16:00.000000 pypdl-1.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12242 2024-03-12 15:16:04.267289 pypdl-1.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11604 2024-03-12 15:16:00.000000 pypdl-1.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 15:16:04.267289 pypdl-1.3.1/pypdl/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-03-12 15:16:00.000000 pypdl-1.3.1/pypdl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2876 2024-03-12 15:16:00.000000 pypdl-1.3.1/pypdl/downloader.py
--rw-r--r--   0 runner    (1001) docker     (127)    10197 2024-03-12 15:16:00.000000 pypdl-1.3.1/pypdl/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     4019 2024-03-12 15:16:00.000000 pypdl-1.3.1/pypdl/utls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 15:16:04.267289 pypdl-1.3.1/pypdl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12242 2024-03-12 15:16:04.000000 pypdl-1.3.1/pypdl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-03-12 15:16:04.000000 pypdl-1.3.1/pypdl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-12 15:16:04.000000 pypdl-1.3.1/pypdl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-12 15:16:04.000000 pypdl-1.3.1/pypdl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-12 15:16:04.000000 pypdl-1.3.1/pypdl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-12 15:16:04.267289 pypdl-1.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      982 2024-03-12 15:16:00.000000 pypdl-1.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 07:52:38.998847 pypdl-1.3.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-06 07:52:35.000000 pypdl-1.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12242 2024-04-06 07:52:38.998847 pypdl-1.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11604 2024-04-06 07:52:35.000000 pypdl-1.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 07:52:38.994847 pypdl-1.3.2/pypdl/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-06 07:52:35.000000 pypdl-1.3.2/pypdl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2876 2024-04-06 07:52:35.000000 pypdl-1.3.2/pypdl/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10358 2024-04-06 07:52:35.000000 pypdl-1.3.2/pypdl/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4019 2024-04-06 07:52:35.000000 pypdl-1.3.2/pypdl/utls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 07:52:38.994847 pypdl-1.3.2/pypdl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12242 2024-04-06 07:52:38.000000 pypdl-1.3.2/pypdl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-06 07:52:38.000000 pypdl-1.3.2/pypdl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 07:52:38.000000 pypdl-1.3.2/pypdl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-06 07:52:38.000000 pypdl-1.3.2/pypdl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-06 07:52:38.000000 pypdl-1.3.2/pypdl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 07:52:38.998847 pypdl-1.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      982 2024-04-06 07:52:35.000000 pypdl-1.3.2/setup.py
```

### Comparing `pypdl-1.3.1/LICENSE` & `pypdl-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pypdl-1.3.1/PKG-INFO` & `pypdl-1.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: pypdl
-Version: 1.3.1
+Version: 1.3.2
 Summary: A concurrent python download manager
 Home-page: https://github.com/mjishnu/pypdl
 Author: mjishnu
 Author-email: <mjishnu@skiff.com>
 License: MIT
 Keywords: python,downloader,concurrent-downloader,parrel-downloader,download manager,fast-downloader
-Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: reprint
 
 # pypdl
```

### Comparing `pypdl-1.3.1/README.md` & `pypdl-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `pypdl-1.3.1/pypdl/downloader.py` & `pypdl-1.3.2/pypdl/downloader.py`

 * *Files identical despite different names*

### Comparing `pypdl-1.3.1/pypdl/main.py` & `pypdl-1.3.2/pypdl/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,23 +108,27 @@
             )
             self._workers.append(md)
             self._pool.submit(md.worker)
 
     def _get_header(self, url):
         kwargs = self._kwargs.copy()
         kwargs.pop("params", None)
-        response = requests.head(url, **kwargs)
 
-        if response.status_code != 200:
-            self._interrupt.set()
-            raise ConnectionError(
-                f"Server Returned: {response.reason}({response.status_code}), Invalid URL"
-            )
+        with requests.head(url, **kwargs) as response:
+            if response.status_code == 200:
+                return response.headers
+
+        with requests.get(url, stream=True, **self._kwargs) as response:
+            if response.status_code == 200:
+                return response.headers
 
-        return response.headers
+        self._interrupt.set()
+        raise ConnectionError(
+            f"Server Returned: {response.reason}({response.status_code}), Invalid URL"
+        )
 
     def _get_info(self, url, file_path, multithread, etag):
         header = self._get_header(url)
         file_path = get_filepath(url, header, file_path)
 
         if size := int(header.get("content-length", 0)):
             self.size = size
```

### Comparing `pypdl-1.3.1/pypdl/utls.py` & `pypdl-1.3.2/pypdl/utls.py`

 * *Files identical despite different names*

### Comparing `pypdl-1.3.1/pypdl.egg-info/PKG-INFO` & `pypdl-1.3.2/pypdl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: pypdl
-Version: 1.3.1
+Version: 1.3.2
 Summary: A concurrent python download manager
 Home-page: https://github.com/mjishnu/pypdl
 Author: mjishnu
 Author-email: <mjishnu@skiff.com>
 License: MIT
 Keywords: python,downloader,concurrent-downloader,parrel-downloader,download manager,fast-downloader
-Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: reprint
 
 # pypdl
```

### Comparing `pypdl-1.3.1/setup.py` & `pypdl-1.3.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = "1.3.1"
+VERSION = "1.3.2"
 DESCRIPTION = "A concurrent python download manager"
 with open("README.md", "r") as f:
     LONG_DESCRIPTION = f.read()
 
 setup(
     name="pypdl",
     version=VERSION,
```

