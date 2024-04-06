# Comparing `tmp/dydantic-0.0.1rc0.tar.gz` & `tmp/dydantic-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dydantic-0.0.1rc0.tar", max compression
+gzip compressed data, was "dydantic-0.0.2.tar", max compression
```

## Comparing `dydantic-0.0.1rc0.tar` & `dydantic-0.0.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1067 2024-04-06 05:52:07.999927 dydantic-0.0.1rc0/LICENSE
--rw-r--r--   0        0        0     2600 2024-04-06 06:50:17.046941 dydantic-0.0.1rc0/README.md
--rw-r--r--   0        0        0     1979 2024-04-06 06:24:35.972522 dydantic-0.0.1rc0/dydantic/__init__.py
--rw-r--r--   0        0        0     8059 2024-04-06 06:47:42.367528 dydantic-0.0.1rc0/dydantic/_utils.py
--rw-r--r--   0        0        0        0 2024-04-06 06:24:35.972780 dydantic-0.0.1rc0/dydantic/py.typed
--rw-r--r--   0        0        0      995 2024-04-06 06:50:26.346448 dydantic-0.0.1rc0/pyproject.toml
--rw-r--r--   0        0        0     3222 1970-01-01 00:00:00.000000 dydantic-0.0.1rc0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-04-06 05:52:07.999927 dydantic-0.0.2/LICENSE
+-rw-r--r--   0        0        0     2600 2024-04-06 06:50:17.046941 dydantic-0.0.2/README.md
+-rw-r--r--   0        0        0     1979 2024-04-06 06:24:35.972522 dydantic-0.0.2/dydantic/__init__.py
+-rw-r--r--   0        0        0     8059 2024-04-06 06:47:42.367528 dydantic-0.0.2/dydantic/_utils.py
+-rw-r--r--   0        0        0        0 2024-04-06 06:24:35.972780 dydantic-0.0.2/dydantic/py.typed
+-rw-r--r--   0        0        0      992 2024-04-06 06:51:05.096785 dydantic-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     3219 1970-01-01 00:00:00.000000 dydantic-0.0.2/PKG-INFO
```

### Comparing `dydantic-0.0.1rc0/LICENSE` & `dydantic-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dydantic-0.0.1rc0/README.md` & `dydantic-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `dydantic-0.0.1rc0/dydantic/__init__.py` & `dydantic-0.0.2/dydantic/__init__.py`

 * *Files identical despite different names*

### Comparing `dydantic-0.0.1rc0/dydantic/_utils.py` & `dydantic-0.0.2/dydantic/_utils.py`

 * *Files identical despite different names*

### Comparing `dydantic-0.0.1rc0/pyproject.toml` & `dydantic-0.0.2/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dydantic"
-version = "0.0.1rc0"
+version = "0.0.2"
 description = "Dynamically generate pydantic models from JSON schema."
 authors = ["William Fu-Hinthorn <13333726+hinthornw@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `dydantic-0.0.1rc0/PKG-INFO` & `dydantic-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dydantic
-Version: 0.0.1rc0
+Version: 0.0.2
 Summary: Dynamically generate pydantic models from JSON schema.
 License: MIT
 Author: William Fu-Hinthorn
 Author-email: 13333726+hinthornw@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

