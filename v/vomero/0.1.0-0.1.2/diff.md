# Comparing `tmp/vomero-0.1.0.tar.gz` & `tmp/vomero-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vomero-0.1.0.tar", max compression
+gzip compressed data, was "vomero-0.1.2.tar", max compression
```

## Comparing `vomero-0.1.0.tar` & `vomero-0.1.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1071 2024-04-05 21:18:06.619800 vomero-0.1.0/LICENSE
--rw-r--r--   0        0        0     2605 2024-04-05 21:18:06.619800 vomero-0.1.0/README.md
--rw-r--r--   0        0        0      488 2024-04-05 21:18:06.619800 vomero-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       88 2024-04-05 21:18:06.619800 vomero-0.1.0/src/vomero/__init__.py
--rw-r--r--   0        0        0     5645 2024-04-05 21:18:06.619800 vomero-0.1.0/src/vomero/streams.py
--rw-r--r--   0        0        0      357 2024-04-05 21:18:06.619800 vomero-0.1.0/src/vomero/types.py
--rw-r--r--   0        0        0     1000 2024-04-05 21:18:06.619800 vomero-0.1.0/src/vomero/worker.py
--rw-r--r--   0        0        0     3108 1970-01-01 00:00:00.000000 vomero-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-04-05 21:27:31.364110 vomero-0.1.2/LICENSE
+-rw-r--r--   0        0        0     2605 2024-04-05 21:27:31.364110 vomero-0.1.2/README.md
+-rw-r--r--   0        0        0      537 2024-04-05 21:27:31.364110 vomero-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0       88 2024-04-05 21:27:31.364110 vomero-0.1.2/src/vomero/__init__.py
+-rw-r--r--   0        0        0     5645 2024-04-05 21:27:31.364110 vomero-0.1.2/src/vomero/streams.py
+-rw-r--r--   0        0        0      357 2024-04-05 21:27:31.364110 vomero-0.1.2/src/vomero/types.py
+-rw-r--r--   0        0        0     1000 2024-04-05 21:27:31.364110 vomero-0.1.2/src/vomero/worker.py
+-rw-r--r--   0        0        0     3155 1970-01-01 00:00:00.000000 vomero-0.1.2/PKG-INFO
```

### Comparing `vomero-0.1.0/LICENSE` & `vomero-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `vomero-0.1.0/README.md` & `vomero-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `vomero-0.1.0/src/vomero/streams.py` & `vomero-0.1.2/src/vomero/streams.py`

 * *Files identical despite different names*

### Comparing `vomero-0.1.0/src/vomero/worker.py` & `vomero-0.1.2/src/vomero/worker.py`

 * *Files identical despite different names*

### Comparing `vomero-0.1.0/PKG-INFO` & `vomero-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: vomero
-Version: 0.1.0
+Version: 0.1.2
 Summary: Event processing library for Python based on Redis Streams
+Home-page: https://github.com/mzsawicki/vomero
 License: MIT
 Author: Marcin Sawicki
 Author-email: marcin.z.sawicki@protonmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

