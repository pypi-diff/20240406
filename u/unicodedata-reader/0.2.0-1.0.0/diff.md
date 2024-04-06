# Comparing `tmp/unicodedata_reader-0.2.0.tar.gz` & `tmp/unicodedata_reader-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unicodedata_reader-0.2.0.tar", max compression
+gzip compressed data, was "unicodedata_reader-1.0.0.tar", max compression
```

## Comparing `unicodedata_reader-0.2.0.tar` & `unicodedata_reader-1.0.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0    11357 2024-04-06 18:07:10.880042 unicodedata_reader-0.2.0/LICENSE
--rw-r--r--   0        0        0     3120 2024-04-06 18:07:10.880042 unicodedata_reader-0.2.0/README.md
--rw-r--r--   0        0        0      678 2024-04-06 18:07:10.880042 unicodedata_reader-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      107 2024-04-06 18:07:10.880042 unicodedata_reader-0.2.0/unicodedata_reader/__init__.py
--rw-r--r--   0        0        0     1101 2024-04-06 18:07:10.880042 unicodedata_reader-0.2.0/unicodedata_reader/__main__.py
--rwxr-xr-x   0        0        0     1310 2024-04-06 18:07:10.880042 unicodedata_reader-0.2.0/unicodedata_reader/bidi_brackets.py
--rw-r--r--   0        0        0     4675 2024-04-06 18:07:10.880042 unicodedata_reader-0.2.0/unicodedata_reader/cli.py
--rwxr-xr-x   0        0        0     4360 2024-04-06 18:07:10.880042 unicodedata_reader-0.2.0/unicodedata_reader/compressor.py
--rw-r--r--   0        0        0      982 2024-04-06 18:07:10.880042 unicodedata_reader-0.2.0/unicodedata_reader/east_asian_width.py
--rwxr-xr-x   0        0        0     1220 2024-04-06 18:07:10.880042 unicodedata_reader-0.2.0/unicodedata_reader/emoji.py
--rw-r--r--   0        0        0    13464 2024-04-06 18:07:10.880042 unicodedata_reader-0.2.0/unicodedata_reader/entry.py
--rwxr-xr-x   0        0        0      558 2024-04-06 18:07:10.880042 unicodedata_reader-0.2.0/unicodedata_reader/general_category.py
--rwxr-xr-x   0        0        0      671 2024-04-06 18:07:10.880042 unicodedata_reader-0.2.0/unicodedata_reader/line_break.py
--rw-r--r--   0        0        0     3806 2024-04-06 18:07:10.880042 unicodedata_reader-0.2.0/unicodedata_reader/reader.py
--rw-r--r--   0        0        0     2141 2024-04-06 18:07:10.884042 unicodedata_reader-0.2.0/unicodedata_reader/set.py
--rwxr-xr-x   0        0        0      996 2024-04-06 18:07:10.884042 unicodedata_reader-0.2.0/unicodedata_reader/vertical_orientation.py
--rw-r--r--   0        0        0     3864 1970-01-01 00:00:00.000000 unicodedata_reader-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-06 18:10:32.935142 unicodedata_reader-1.0.0/LICENSE
+-rw-r--r--   0        0        0     3120 2024-04-06 18:10:32.935142 unicodedata_reader-1.0.0/README.md
+-rw-r--r--   0        0        0      678 2024-04-06 18:10:32.935142 unicodedata_reader-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0      107 2024-04-06 18:10:32.935142 unicodedata_reader-1.0.0/unicodedata_reader/__init__.py
+-rw-r--r--   0        0        0     1101 2024-04-06 18:10:32.935142 unicodedata_reader-1.0.0/unicodedata_reader/__main__.py
+-rwxr-xr-x   0        0        0     1310 2024-04-06 18:10:32.935142 unicodedata_reader-1.0.0/unicodedata_reader/bidi_brackets.py
+-rw-r--r--   0        0        0     4675 2024-04-06 18:10:32.935142 unicodedata_reader-1.0.0/unicodedata_reader/cli.py
+-rwxr-xr-x   0        0        0     4360 2024-04-06 18:10:32.935142 unicodedata_reader-1.0.0/unicodedata_reader/compressor.py
+-rw-r--r--   0        0        0      982 2024-04-06 18:10:32.935142 unicodedata_reader-1.0.0/unicodedata_reader/east_asian_width.py
+-rwxr-xr-x   0        0        0     1220 2024-04-06 18:10:32.935142 unicodedata_reader-1.0.0/unicodedata_reader/emoji.py
+-rw-r--r--   0        0        0    13464 2024-04-06 18:10:32.935142 unicodedata_reader-1.0.0/unicodedata_reader/entry.py
+-rwxr-xr-x   0        0        0      558 2024-04-06 18:10:32.935142 unicodedata_reader-1.0.0/unicodedata_reader/general_category.py
+-rwxr-xr-x   0        0        0      671 2024-04-06 18:10:32.935142 unicodedata_reader-1.0.0/unicodedata_reader/line_break.py
+-rw-r--r--   0        0        0     3806 2024-04-06 18:10:32.935142 unicodedata_reader-1.0.0/unicodedata_reader/reader.py
+-rw-r--r--   0        0        0     2141 2024-04-06 18:10:32.935142 unicodedata_reader-1.0.0/unicodedata_reader/set.py
+-rwxr-xr-x   0        0        0      996 2024-04-06 18:10:32.935142 unicodedata_reader-1.0.0/unicodedata_reader/vertical_orientation.py
+-rw-r--r--   0        0        0     3864 1970-01-01 00:00:00.000000 unicodedata_reader-1.0.0/PKG-INFO
```

### Comparing `unicodedata_reader-0.2.0/LICENSE` & `unicodedata_reader-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `unicodedata_reader-0.2.0/README.md` & `unicodedata_reader-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `unicodedata_reader-0.2.0/pyproject.toml` & `unicodedata_reader-1.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "unicodedata-reader"
-version = "0.2.0"
+version = "1.0.0"
 description = ""
 authors = ["Koji Ishii <kojii@chromium.org>"]
 readme = "README.md"
 repository = "https://github.com/kojiishi/unicodedata-reader"
 license = "Apache-2.0"
 
 [tool.poetry.dependencies]
```

### Comparing `unicodedata_reader-0.2.0/unicodedata_reader/__main__.py` & `unicodedata_reader-1.0.0/unicodedata_reader/__main__.py`

 * *Files identical despite different names*

### Comparing `unicodedata_reader-0.2.0/unicodedata_reader/bidi_brackets.py` & `unicodedata_reader-1.0.0/unicodedata_reader/bidi_brackets.py`

 * *Files identical despite different names*

### Comparing `unicodedata_reader-0.2.0/unicodedata_reader/cli.py` & `unicodedata_reader-1.0.0/unicodedata_reader/cli.py`

 * *Files identical despite different names*

### Comparing `unicodedata_reader-0.2.0/unicodedata_reader/compressor.py` & `unicodedata_reader-1.0.0/unicodedata_reader/compressor.py`

 * *Files identical despite different names*

### Comparing `unicodedata_reader-0.2.0/unicodedata_reader/east_asian_width.py` & `unicodedata_reader-1.0.0/unicodedata_reader/east_asian_width.py`

 * *Files identical despite different names*

### Comparing `unicodedata_reader-0.2.0/unicodedata_reader/emoji.py` & `unicodedata_reader-1.0.0/unicodedata_reader/emoji.py`

 * *Files identical despite different names*

### Comparing `unicodedata_reader-0.2.0/unicodedata_reader/entry.py` & `unicodedata_reader-1.0.0/unicodedata_reader/entry.py`

 * *Files identical despite different names*

### Comparing `unicodedata_reader-0.2.0/unicodedata_reader/general_category.py` & `unicodedata_reader-1.0.0/unicodedata_reader/general_category.py`

 * *Files identical despite different names*

### Comparing `unicodedata_reader-0.2.0/unicodedata_reader/line_break.py` & `unicodedata_reader-1.0.0/unicodedata_reader/line_break.py`

 * *Files identical despite different names*

### Comparing `unicodedata_reader-0.2.0/unicodedata_reader/reader.py` & `unicodedata_reader-1.0.0/unicodedata_reader/reader.py`

 * *Files identical despite different names*

### Comparing `unicodedata_reader-0.2.0/unicodedata_reader/set.py` & `unicodedata_reader-1.0.0/unicodedata_reader/set.py`

 * *Files identical despite different names*

### Comparing `unicodedata_reader-0.2.0/unicodedata_reader/vertical_orientation.py` & `unicodedata_reader-1.0.0/unicodedata_reader/vertical_orientation.py`

 * *Files identical despite different names*

### Comparing `unicodedata_reader-0.2.0/PKG-INFO` & `unicodedata_reader-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unicodedata-reader
-Version: 0.2.0
+Version: 1.0.0
 Summary: 
 Home-page: https://github.com/kojiishi/unicodedata-reader
 License: Apache-2.0
 Author: Koji Ishii
 Author-email: kojii@chromium.org
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: Apache Software License
```

