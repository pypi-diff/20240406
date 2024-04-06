# Comparing `tmp/unicodedata_reader-1.0.1.tar.gz` & `tmp/unicodedata_reader-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unicodedata_reader-1.0.1.tar", max compression
+gzip compressed data, was "unicodedata_reader-1.1.0.tar", max compression
```

## Comparing `unicodedata_reader-1.0.1.tar` & `unicodedata_reader-1.1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0    11357 2024-04-06 18:26:11.817131 unicodedata_reader-1.0.1/LICENSE
--rw-r--r--   0        0        0     3120 2024-04-06 18:26:11.817131 unicodedata_reader-1.0.1/README.md
--rw-r--r--   0        0        0      678 2024-04-06 18:26:11.817131 unicodedata_reader-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      107 2024-04-06 18:26:11.821131 unicodedata_reader-1.0.1/unicodedata_reader/__init__.py
--rw-r--r--   0        0        0     1101 2024-04-06 18:26:11.821131 unicodedata_reader-1.0.1/unicodedata_reader/__main__.py
--rwxr-xr-x   0        0        0     1310 2024-04-06 18:26:11.821131 unicodedata_reader-1.0.1/unicodedata_reader/bidi_brackets.py
--rw-r--r--   0        0        0     4675 2024-04-06 18:26:11.821131 unicodedata_reader-1.0.1/unicodedata_reader/cli.py
--rwxr-xr-x   0        0        0     4360 2024-04-06 18:26:11.821131 unicodedata_reader-1.0.1/unicodedata_reader/compressor.py
--rw-r--r--   0        0        0      982 2024-04-06 18:26:11.821131 unicodedata_reader-1.0.1/unicodedata_reader/east_asian_width.py
--rwxr-xr-x   0        0        0     1220 2024-04-06 18:26:11.821131 unicodedata_reader-1.0.1/unicodedata_reader/emoji.py
--rw-r--r--   0        0        0    13464 2024-04-06 18:26:11.821131 unicodedata_reader-1.0.1/unicodedata_reader/entry.py
--rwxr-xr-x   0        0        0      558 2024-04-06 18:26:11.821131 unicodedata_reader-1.0.1/unicodedata_reader/general_category.py
--rwxr-xr-x   0        0        0      671 2024-04-06 18:26:11.821131 unicodedata_reader-1.0.1/unicodedata_reader/line_break.py
--rw-r--r--   0        0        0     3806 2024-04-06 18:26:11.821131 unicodedata_reader-1.0.1/unicodedata_reader/reader.py
--rw-r--r--   0        0        0     2204 2024-04-06 18:26:11.821131 unicodedata_reader-1.0.1/unicodedata_reader/set.py
--rwxr-xr-x   0        0        0      996 2024-04-06 18:26:11.821131 unicodedata_reader-1.0.1/unicodedata_reader/vertical_orientation.py
--rw-r--r--   0        0        0     3864 1970-01-01 00:00:00.000000 unicodedata_reader-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-06 19:55:08.599310 unicodedata_reader-1.1.0/LICENSE
+-rw-r--r--   0        0        0     3120 2024-04-06 19:55:08.599310 unicodedata_reader-1.1.0/README.md
+-rw-r--r--   0        0        0      678 2024-04-06 19:55:08.599310 unicodedata_reader-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0      107 2024-04-06 19:55:08.603310 unicodedata_reader-1.1.0/unicodedata_reader/__init__.py
+-rw-r--r--   0        0        0     1101 2024-04-06 19:55:08.603310 unicodedata_reader-1.1.0/unicodedata_reader/__main__.py
+-rwxr-xr-x   0        0        0     1310 2024-04-06 19:55:08.603310 unicodedata_reader-1.1.0/unicodedata_reader/bidi_brackets.py
+-rw-r--r--   0        0        0     4675 2024-04-06 19:55:08.603310 unicodedata_reader-1.1.0/unicodedata_reader/cli.py
+-rwxr-xr-x   0        0        0     4360 2024-04-06 19:55:08.603310 unicodedata_reader-1.1.0/unicodedata_reader/compressor.py
+-rw-r--r--   0        0        0      982 2024-04-06 19:55:08.603310 unicodedata_reader-1.1.0/unicodedata_reader/east_asian_width.py
+-rwxr-xr-x   0        0        0     1220 2024-04-06 19:55:08.603310 unicodedata_reader-1.1.0/unicodedata_reader/emoji.py
+-rw-r--r--   0        0        0    13464 2024-04-06 19:55:08.603310 unicodedata_reader-1.1.0/unicodedata_reader/entry.py
+-rwxr-xr-x   0        0        0      558 2024-04-06 19:55:08.603310 unicodedata_reader-1.1.0/unicodedata_reader/general_category.py
+-rwxr-xr-x   0        0        0      671 2024-04-06 19:55:08.603310 unicodedata_reader-1.1.0/unicodedata_reader/line_break.py
+-rw-r--r--   0        0        0     3992 2024-04-06 19:55:08.603310 unicodedata_reader-1.1.0/unicodedata_reader/reader.py
+-rw-r--r--   0        0        0     2255 2024-04-06 19:55:08.603310 unicodedata_reader-1.1.0/unicodedata_reader/set.py
+-rwxr-xr-x   0        0        0      996 2024-04-06 19:55:08.603310 unicodedata_reader-1.1.0/unicodedata_reader/vertical_orientation.py
+-rw-r--r--   0        0        0     3864 1970-01-01 00:00:00.000000 unicodedata_reader-1.1.0/PKG-INFO
```

### Comparing `unicodedata_reader-1.0.1/LICENSE` & `unicodedata_reader-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `unicodedata_reader-1.0.1/README.md` & `unicodedata_reader-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `unicodedata_reader-1.0.1/pyproject.toml` & `unicodedata_reader-1.1.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "unicodedata-reader"
-version = "1.0.1"
+version = "1.1.0"
 description = ""
 authors = ["Koji Ishii <kojii@chromium.org>"]
 readme = "README.md"
 repository = "https://github.com/kojiishi/unicodedata-reader"
 license = "Apache-2.0"
 
 [tool.poetry.dependencies]
```

### Comparing `unicodedata_reader-1.0.1/unicodedata_reader/__main__.py` & `unicodedata_reader-1.1.0/unicodedata_reader/__main__.py`

 * *Files identical despite different names*

### Comparing `unicodedata_reader-1.0.1/unicodedata_reader/bidi_brackets.py` & `unicodedata_reader-1.1.0/unicodedata_reader/bidi_brackets.py`

 * *Files identical despite different names*

### Comparing `unicodedata_reader-1.0.1/unicodedata_reader/cli.py` & `unicodedata_reader-1.1.0/unicodedata_reader/cli.py`

 * *Files identical despite different names*

### Comparing `unicodedata_reader-1.0.1/unicodedata_reader/compressor.py` & `unicodedata_reader-1.1.0/unicodedata_reader/compressor.py`

 * *Files identical despite different names*

### Comparing `unicodedata_reader-1.0.1/unicodedata_reader/east_asian_width.py` & `unicodedata_reader-1.1.0/unicodedata_reader/east_asian_width.py`

 * *Files identical despite different names*

### Comparing `unicodedata_reader-1.0.1/unicodedata_reader/emoji.py` & `unicodedata_reader-1.1.0/unicodedata_reader/emoji.py`

 * *Files identical despite different names*

### Comparing `unicodedata_reader-1.0.1/unicodedata_reader/entry.py` & `unicodedata_reader-1.1.0/unicodedata_reader/entry.py`

 * *Files identical despite different names*

### Comparing `unicodedata_reader-1.0.1/unicodedata_reader/general_category.py` & `unicodedata_reader-1.1.0/unicodedata_reader/general_category.py`

 * *Files identical despite different names*

### Comparing `unicodedata_reader-1.0.1/unicodedata_reader/line_break.py` & `unicodedata_reader-1.1.0/unicodedata_reader/line_break.py`

 * *Files identical despite different names*

### Comparing `unicodedata_reader-1.0.1/unicodedata_reader/reader.py` & `unicodedata_reader-1.1.0/unicodedata_reader/reader.py`

 * *Files 3% similar despite different names*

```diff
@@ -50,14 +50,19 @@
         return entries
 
     def line_break(self) -> UnicodeDataEntries:
         name = 'LineBreak'
         lines = self.read_lines(name)
         return UnicodeLineBreakDataEntries(name=name, lines=lines)
 
+    def name(self) -> UnicodeDataEntries:
+        lines = self.read_lines('extracted/DerivedName')
+        entries = UnicodeDataEntries(name='Name', lines=lines)
+        return entries
+
     def scripts(self) -> UnicodeDataEntries:
         name = 'Scripts'
         lines = self.read_lines(name)
         return UnicodeDataEntries(name=name, lines=lines)
 
     def script_extensions(self) -> UnicodeDataEntries:
         name = 'ScriptExtensions'
```

### Comparing `unicodedata_reader-1.0.1/unicodedata_reader/set.py` & `unicodedata_reader-1.1.0/unicodedata_reader/set.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,10 @@
+from typing import Any
 from typing import Callable
+from typing import Iterable
 
 from unicodedata_reader.entry import *
 from unicodedata_reader.reader import *
 
 
 class Set(object):
     """A simple set of Unicode code points."""
```

### Comparing `unicodedata_reader-1.0.1/unicodedata_reader/vertical_orientation.py` & `unicodedata_reader-1.1.0/unicodedata_reader/vertical_orientation.py`

 * *Files identical despite different names*

### Comparing `unicodedata_reader-1.0.1/PKG-INFO` & `unicodedata_reader-1.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unicodedata-reader
-Version: 1.0.1
+Version: 1.1.0
 Summary: 
 Home-page: https://github.com/kojiishi/unicodedata-reader
 License: Apache-2.0
 Author: Koji Ishii
 Author-email: kojii@chromium.org
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: Apache Software License
```

