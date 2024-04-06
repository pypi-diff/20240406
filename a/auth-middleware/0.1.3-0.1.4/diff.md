# Comparing `tmp/auth_middleware-0.1.3.tar.gz` & `tmp/auth_middleware-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auth_middleware-0.1.3.tar", max compression
+gzip compressed data, was "auth_middleware-0.1.4.tar", max compression
```

## Comparing `auth_middleware-0.1.3.tar` & `auth_middleware-0.1.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1070 2024-04-06 13:22:03.304051 auth_middleware-0.1.3/LICENSE
--rw-r--r--   0        0        0     3765 2024-04-06 13:22:03.304051 auth_middleware-0.1.3/README.md
--rw-r--r--   0        0        0      845 2024-04-06 13:22:45.472360 auth_middleware-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      536 2024-04-06 13:22:03.324051 auth_middleware-0.1.3/src/auth_middleware/__init__.py
--rw-r--r--   0        0        0       89 2024-04-06 13:22:03.324051 auth_middleware-0.1.3/src/auth_middleware/exceptions.py
--rw-r--r--   0        0        0     1085 2024-04-06 13:22:03.324051 auth_middleware-0.1.3/src/auth_middleware/functions.py
--rw-r--r--   0        0        0     1069 2024-04-06 13:22:03.324051 auth_middleware-0.1.3/src/auth_middleware/group_checker.py
--rw-r--r--   0        0        0     3949 2024-04-06 13:22:03.324051 auth_middleware-0.1.3/src/auth_middleware/jwt_auth_middleware.py
--rw-r--r--   0        0        0     1963 2024-04-06 13:22:03.324051 auth_middleware-0.1.3/src/auth_middleware/jwt_auth_provider.py
--rw-r--r--   0        0        0     2915 2024-04-06 13:22:03.324051 auth_middleware-0.1.3/src/auth_middleware/jwt_bearer_manager.py
--rw-r--r--   0        0        0      762 2024-04-06 13:22:03.324051 auth_middleware-0.1.3/src/auth_middleware/logging.py
--rw-r--r--   0        0        0        0 2024-04-06 13:22:03.324051 auth_middleware-0.1.3/src/auth_middleware/providers/__init__.py
--rw-r--r--   0        0        0      141 2024-04-06 13:22:03.324051 auth_middleware-0.1.3/src/auth_middleware/providers/cognito/__init__.py
--rw-r--r--   0        0        0     3072 2024-04-06 13:22:03.324051 auth_middleware-0.1.3/src/auth_middleware/providers/cognito/cognito_provider.py
--rw-r--r--   0        0        0      180 2024-04-06 13:22:03.324051 auth_middleware-0.1.3/src/auth_middleware/providers/cognito/exceptions.py
--rw-r--r--   0        0        0     1157 2024-04-06 13:22:03.324051 auth_middleware-0.1.3/src/auth_middleware/providers/cognito/settings.py
--rw-r--r--   0        0        0      146 2024-04-06 13:22:03.324051 auth_middleware-0.1.3/src/auth_middleware/providers/entra_id/__init__.py
--rw-r--r--   0        0        0     4176 2024-04-06 13:22:03.324051 auth_middleware-0.1.3/src/auth_middleware/providers/entra_id/entra_id_provider.py
--rw-r--r--   0        0        0      184 2024-04-06 13:22:03.324051 auth_middleware-0.1.3/src/auth_middleware/providers/entra_id/exceptions.py
--rw-r--r--   0        0        0      864 2024-04-06 13:22:03.324051 auth_middleware-0.1.3/src/auth_middleware/providers/entra_id/settings.py
--rw-r--r--   0        0        0     1007 2024-04-06 13:22:03.324051 auth_middleware-0.1.3/src/auth_middleware/settings.py
--rw-r--r--   0        0        0     1375 2024-04-06 13:22:03.324051 auth_middleware-0.1.3/src/auth_middleware/types.py
--rw-r--r--   0        0        0     4417 1970-01-01 00:00:00.000000 auth_middleware-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-04-06 13:50:09.441245 auth_middleware-0.1.4/LICENSE
+-rw-r--r--   0        0        0     3765 2024-04-06 13:50:09.441245 auth_middleware-0.1.4/README.md
+-rw-r--r--   0        0        0      845 2024-04-06 13:50:44.577745 auth_middleware-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      536 2024-04-06 13:50:09.457245 auth_middleware-0.1.4/src/auth_middleware/__init__.py
+-rw-r--r--   0        0        0       89 2024-04-06 13:50:09.457245 auth_middleware-0.1.4/src/auth_middleware/exceptions.py
+-rw-r--r--   0        0        0     1085 2024-04-06 13:50:09.457245 auth_middleware-0.1.4/src/auth_middleware/functions.py
+-rw-r--r--   0        0        0     1069 2024-04-06 13:50:09.457245 auth_middleware-0.1.4/src/auth_middleware/group_checker.py
+-rw-r--r--   0        0        0     3949 2024-04-06 13:50:09.457245 auth_middleware-0.1.4/src/auth_middleware/jwt_auth_middleware.py
+-rw-r--r--   0        0        0     1963 2024-04-06 13:50:09.457245 auth_middleware-0.1.4/src/auth_middleware/jwt_auth_provider.py
+-rw-r--r--   0        0        0     2915 2024-04-06 13:50:09.461245 auth_middleware-0.1.4/src/auth_middleware/jwt_bearer_manager.py
+-rw-r--r--   0        0        0      762 2024-04-06 13:50:09.461245 auth_middleware-0.1.4/src/auth_middleware/logging.py
+-rw-r--r--   0        0        0        0 2024-04-06 13:50:09.461245 auth_middleware-0.1.4/src/auth_middleware/providers/__init__.py
+-rw-r--r--   0        0        0      141 2024-04-06 13:50:09.461245 auth_middleware-0.1.4/src/auth_middleware/providers/cognito/__init__.py
+-rw-r--r--   0        0        0     3072 2024-04-06 13:50:09.461245 auth_middleware-0.1.4/src/auth_middleware/providers/cognito/cognito_provider.py
+-rw-r--r--   0        0        0      180 2024-04-06 13:50:09.461245 auth_middleware-0.1.4/src/auth_middleware/providers/cognito/exceptions.py
+-rw-r--r--   0        0        0     1157 2024-04-06 13:50:09.461245 auth_middleware-0.1.4/src/auth_middleware/providers/cognito/settings.py
+-rw-r--r--   0        0        0      146 2024-04-06 13:50:09.461245 auth_middleware-0.1.4/src/auth_middleware/providers/entra_id/__init__.py
+-rw-r--r--   0        0        0     4176 2024-04-06 13:50:09.461245 auth_middleware-0.1.4/src/auth_middleware/providers/entra_id/entra_id_provider.py
+-rw-r--r--   0        0        0      184 2024-04-06 13:50:09.461245 auth_middleware-0.1.4/src/auth_middleware/providers/entra_id/exceptions.py
+-rw-r--r--   0        0        0      864 2024-04-06 13:50:09.461245 auth_middleware-0.1.4/src/auth_middleware/providers/entra_id/settings.py
+-rw-r--r--   0        0        0     1007 2024-04-06 13:50:09.461245 auth_middleware-0.1.4/src/auth_middleware/settings.py
+-rw-r--r--   0        0        0     1375 2024-04-06 13:50:09.461245 auth_middleware-0.1.4/src/auth_middleware/types.py
+-rw-r--r--   0        0        0     4417 1970-01-01 00:00:00.000000 auth_middleware-0.1.4/PKG-INFO
```

### Comparing `auth_middleware-0.1.3/LICENSE` & `auth_middleware-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `auth_middleware-0.1.3/README.md` & `auth_middleware-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `auth_middleware-0.1.3/pyproject.toml` & `auth_middleware-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "auth-middleware"
-version = "0.1.3"
+version = "0.1.4"
 description = "Async Auth Middleware for FastAPI/Starlette"
 authors = ["impalah <impalah@gmail.com>"]
 readme = "README.md"
 packages = [{include = "auth_middleware", from = "src"}]
 
 [tool.poetry.dependencies]
 python = "^3.12"
```

### Comparing `auth_middleware-0.1.3/src/auth_middleware/__init__.py` & `auth_middleware-0.1.4/src/auth_middleware/__init__.py`

 * *Files identical despite different names*

### Comparing `auth_middleware-0.1.3/src/auth_middleware/functions.py` & `auth_middleware-0.1.4/src/auth_middleware/functions.py`

 * *Files identical despite different names*

### Comparing `auth_middleware-0.1.3/src/auth_middleware/group_checker.py` & `auth_middleware-0.1.4/src/auth_middleware/group_checker.py`

 * *Files identical despite different names*

### Comparing `auth_middleware-0.1.3/src/auth_middleware/jwt_auth_middleware.py` & `auth_middleware-0.1.4/src/auth_middleware/jwt_auth_middleware.py`

 * *Files identical despite different names*

### Comparing `auth_middleware-0.1.3/src/auth_middleware/jwt_auth_provider.py` & `auth_middleware-0.1.4/src/auth_middleware/jwt_auth_provider.py`

 * *Files identical despite different names*

### Comparing `auth_middleware-0.1.3/src/auth_middleware/jwt_bearer_manager.py` & `auth_middleware-0.1.4/src/auth_middleware/jwt_bearer_manager.py`

 * *Files identical despite different names*

### Comparing `auth_middleware-0.1.3/src/auth_middleware/logging.py` & `auth_middleware-0.1.4/src/auth_middleware/logging.py`

 * *Files identical despite different names*

### Comparing `auth_middleware-0.1.3/src/auth_middleware/providers/cognito/cognito_provider.py` & `auth_middleware-0.1.4/src/auth_middleware/providers/cognito/cognito_provider.py`

 * *Files identical despite different names*

### Comparing `auth_middleware-0.1.3/src/auth_middleware/providers/cognito/settings.py` & `auth_middleware-0.1.4/src/auth_middleware/providers/cognito/settings.py`

 * *Files identical despite different names*

### Comparing `auth_middleware-0.1.3/src/auth_middleware/providers/entra_id/entra_id_provider.py` & `auth_middleware-0.1.4/src/auth_middleware/providers/entra_id/entra_id_provider.py`

 * *Files identical despite different names*

### Comparing `auth_middleware-0.1.3/src/auth_middleware/providers/entra_id/settings.py` & `auth_middleware-0.1.4/src/auth_middleware/providers/entra_id/settings.py`

 * *Files identical despite different names*

### Comparing `auth_middleware-0.1.3/src/auth_middleware/settings.py` & `auth_middleware-0.1.4/src/auth_middleware/settings.py`

 * *Files identical despite different names*

### Comparing `auth_middleware-0.1.3/src/auth_middleware/types.py` & `auth_middleware-0.1.4/src/auth_middleware/types.py`

 * *Files identical despite different names*

### Comparing `auth_middleware-0.1.3/PKG-INFO` & `auth_middleware-0.1.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auth-middleware
-Version: 0.1.3
+Version: 0.1.4
 Summary: Async Auth Middleware for FastAPI/Starlette
 Author: impalah
 Author-email: impalah@gmail.com
 Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: colorlog (>=6.8.0,<7.0.0)
```

