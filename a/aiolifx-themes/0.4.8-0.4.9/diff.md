# Comparing `tmp/aiolifx_themes-0.4.8.tar.gz` & `tmp/aiolifx_themes-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiolifx_themes-0.4.8.tar", max compression
+gzip compressed data, was "aiolifx_themes-0.4.9.tar", max compression
```

## Comparing `aiolifx_themes-0.4.8.tar` & `aiolifx_themes-0.4.9.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1101 2023-08-31 01:59:43.300865 aiolifx_themes-0.4.8/LICENSE
--rw-r--r--   0        0        0     4643 2023-08-31 01:59:43.300865 aiolifx_themes-0.4.8/README.md
--rw-r--r--   0        0        0     2511 2023-08-31 01:59:44.564875 aiolifx_themes-0.4.8/pyproject.toml
--rw-r--r--   0        0        0       22 2023-08-31 01:59:44.524874 aiolifx_themes-0.4.8/src/aiolifx_themes/__init__.py
--rw-r--r--   0        0        0        0 2023-08-31 01:59:43.300865 aiolifx_themes-0.4.8/src/aiolifx_themes/py.typed
--rw-r--r--   0        0        0    32941 2023-08-31 01:59:43.300865 aiolifx_themes-0.4.8/src/aiolifx_themes/themes.py
--rw-r--r--   0        0        0     1708 2023-08-31 01:59:43.300865 aiolifx_themes-0.4.8/src/aiolifx_themes/util.py
--rw-r--r--   0        0        0     6026 1970-01-01 00:00:00.000000 aiolifx_themes-0.4.8/PKG-INFO
+-rw-r--r--   0        0        0     1101 2023-09-14 00:49:33.547175 aiolifx_themes-0.4.9/LICENSE
+-rw-r--r--   0        0        0     4643 2023-09-14 00:49:33.547175 aiolifx_themes-0.4.9/README.md
+-rw-r--r--   0        0        0     2511 2023-09-14 00:49:34.339177 aiolifx_themes-0.4.9/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-09-14 00:49:34.307177 aiolifx_themes-0.4.9/src/aiolifx_themes/__init__.py
+-rw-r--r--   0        0        0        0 2023-09-14 00:49:33.547175 aiolifx_themes-0.4.9/src/aiolifx_themes/py.typed
+-rw-r--r--   0        0        0    32941 2023-09-14 00:49:33.547175 aiolifx_themes-0.4.9/src/aiolifx_themes/themes.py
+-rw-r--r--   0        0        0     1708 2023-09-14 00:49:33.547175 aiolifx_themes-0.4.9/src/aiolifx_themes/util.py
+-rw-r--r--   0        0        0     6026 1970-01-01 00:00:00.000000 aiolifx_themes-0.4.9/PKG-INFO
```

### Comparing `aiolifx_themes-0.4.8/LICENSE` & `aiolifx_themes-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `aiolifx_themes-0.4.8/README.md` & `aiolifx_themes-0.4.9/README.md`

 * *Files identical despite different names*

### Comparing `aiolifx_themes-0.4.8/pyproject.toml` & `aiolifx_themes-0.4.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aiolifx-themes"
-version = "0.4.8"
+version = "0.4.9"
 description = "Async library that applies color themes to LIFX lights"
 authors = ["Avi Miller <me@dje.li>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/Djelibeybi/aiolifx-themes"
 documentation = "https://aiolifx-themes.readthedocs.io"
 classifiers = [
```

### Comparing `aiolifx_themes-0.4.8/src/aiolifx_themes/themes.py` & `aiolifx_themes-0.4.9/src/aiolifx_themes/themes.py`

 * *Files identical despite different names*

### Comparing `aiolifx_themes-0.4.8/src/aiolifx_themes/util.py` & `aiolifx_themes-0.4.9/src/aiolifx_themes/util.py`

 * *Files identical despite different names*

### Comparing `aiolifx_themes-0.4.8/PKG-INFO` & `aiolifx_themes-0.4.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiolifx-themes
-Version: 0.4.8
+Version: 0.4.9
 Summary: Async library that applies color themes to LIFX lights
 Home-page: https://github.com/Djelibeybi/aiolifx-themes
 License: MIT
 Author: Avi Miller
 Author-email: me@dje.li
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: aiolifx-themes Version: 0.4.8 Summary: Async
+Metadata-Version: 2.1 Name: aiolifx-themes Version: 0.4.9 Summary: Async
 library that applies color themes to LIFX lights Home-page: https://github.com/
 Djelibeybi/aiolifx-themes License: MIT Author: Avi Miller Author-email:
 me@dje.li Requires-Python: >=3.9,<4.0 Classifier: Development Status :: 2 -
 Pre-Alpha Classifier: Intended Audience :: Developers Classifier: License ::
 OSI Approved :: MIT License Classifier: Natural Language :: English Classifier:
 Operating System :: OS Independent Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
```

