# Comparing `tmp/auth_middleware-0.1.1.tar.gz` & `tmp/auth_middleware-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auth_middleware-0.1.1.tar", max compression
+gzip compressed data, was "auth_middleware-0.1.2.tar", max compression
```

## Comparing `auth_middleware-0.1.1.tar` & `auth_middleware-0.1.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1070 2024-04-05 18:59:46.909155 auth_middleware-0.1.1/LICENSE
--rw-r--r--   0        0        0     1904 2024-04-05 18:59:46.909155 auth_middleware-0.1.1/README.md
--rw-r--r--   0        0        0      799 2024-04-05 18:59:46.909155 auth_middleware-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      536 2024-04-05 18:59:46.909155 auth_middleware-0.1.1/src/auth_middleware/__init__.py
--rw-r--r--   0        0        0       89 2024-04-05 18:59:46.909155 auth_middleware-0.1.1/src/auth_middleware/exceptions.py
--rw-r--r--   0        0        0      834 2024-04-05 18:59:46.913155 auth_middleware-0.1.1/src/auth_middleware/functions.py
--rw-r--r--   0        0        0     1069 2024-04-05 18:59:46.913155 auth_middleware-0.1.1/src/auth_middleware/group_checker.py
--rw-r--r--   0        0        0     3949 2024-04-05 18:59:46.913155 auth_middleware-0.1.1/src/auth_middleware/jwt_auth_middleware.py
--rw-r--r--   0        0        0     1963 2024-04-05 18:59:46.913155 auth_middleware-0.1.1/src/auth_middleware/jwt_auth_provider.py
--rw-r--r--   0        0        0     2915 2024-04-05 18:59:46.913155 auth_middleware-0.1.1/src/auth_middleware/jwt_bearer_manager.py
--rw-r--r--   0        0        0      762 2024-04-05 18:59:46.913155 auth_middleware-0.1.1/src/auth_middleware/logging.py
--rw-r--r--   0        0        0        0 2024-04-05 18:59:46.913155 auth_middleware-0.1.1/src/auth_middleware/providers/__init__.py
--rw-r--r--   0        0        0      141 2024-04-05 18:59:46.913155 auth_middleware-0.1.1/src/auth_middleware/providers/cognito/__init__.py
--rw-r--r--   0        0        0     3072 2024-04-05 18:59:46.913155 auth_middleware-0.1.1/src/auth_middleware/providers/cognito/cognito_provider.py
--rw-r--r--   0        0        0      180 2024-04-05 18:59:46.913155 auth_middleware-0.1.1/src/auth_middleware/providers/cognito/exceptions.py
--rw-r--r--   0        0        0     1157 2024-04-05 18:59:46.913155 auth_middleware-0.1.1/src/auth_middleware/providers/cognito/settings.py
--rw-r--r--   0        0        0      146 2024-04-05 18:59:46.913155 auth_middleware-0.1.1/src/auth_middleware/providers/entra_id/__init__.py
--rw-r--r--   0        0        0     4176 2024-04-05 18:59:46.913155 auth_middleware-0.1.1/src/auth_middleware/providers/entra_id/entra_id_provider.py
--rw-r--r--   0        0        0      184 2024-04-05 18:59:46.913155 auth_middleware-0.1.1/src/auth_middleware/providers/entra_id/exceptions.py
--rw-r--r--   0        0        0      864 2024-04-05 18:59:46.913155 auth_middleware-0.1.1/src/auth_middleware/providers/entra_id/settings.py
--rw-r--r--   0        0        0     1007 2024-04-05 18:59:46.913155 auth_middleware-0.1.1/src/auth_middleware/settings.py
--rw-r--r--   0        0        0     1375 2024-04-05 18:59:46.913155 auth_middleware-0.1.1/src/auth_middleware/types.py
--rw-r--r--   0        0        0     2556 1970-01-01 00:00:00.000000 auth_middleware-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-04-06 12:22:35.494559 auth_middleware-0.1.2/LICENSE
+-rw-r--r--   0        0        0     3714 2024-04-06 12:22:35.494559 auth_middleware-0.1.2/README.md
+-rw-r--r--   0        0        0      845 2024-04-06 12:23:07.554471 auth_middleware-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      536 2024-04-06 12:22:35.514559 auth_middleware-0.1.2/src/auth_middleware/__init__.py
+-rw-r--r--   0        0        0       89 2024-04-06 12:22:35.514559 auth_middleware-0.1.2/src/auth_middleware/exceptions.py
+-rw-r--r--   0        0        0     1085 2024-04-06 12:22:35.514559 auth_middleware-0.1.2/src/auth_middleware/functions.py
+-rw-r--r--   0        0        0     1069 2024-04-06 12:22:35.514559 auth_middleware-0.1.2/src/auth_middleware/group_checker.py
+-rw-r--r--   0        0        0     3949 2024-04-06 12:22:35.514559 auth_middleware-0.1.2/src/auth_middleware/jwt_auth_middleware.py
+-rw-r--r--   0        0        0     1963 2024-04-06 12:22:35.514559 auth_middleware-0.1.2/src/auth_middleware/jwt_auth_provider.py
+-rw-r--r--   0        0        0     2915 2024-04-06 12:22:35.514559 auth_middleware-0.1.2/src/auth_middleware/jwt_bearer_manager.py
+-rw-r--r--   0        0        0      762 2024-04-06 12:22:35.514559 auth_middleware-0.1.2/src/auth_middleware/logging.py
+-rw-r--r--   0        0        0        0 2024-04-06 12:22:35.514559 auth_middleware-0.1.2/src/auth_middleware/providers/__init__.py
+-rw-r--r--   0        0        0      141 2024-04-06 12:22:35.514559 auth_middleware-0.1.2/src/auth_middleware/providers/cognito/__init__.py
+-rw-r--r--   0        0        0     3072 2024-04-06 12:22:35.514559 auth_middleware-0.1.2/src/auth_middleware/providers/cognito/cognito_provider.py
+-rw-r--r--   0        0        0      180 2024-04-06 12:22:35.514559 auth_middleware-0.1.2/src/auth_middleware/providers/cognito/exceptions.py
+-rw-r--r--   0        0        0     1157 2024-04-06 12:22:35.514559 auth_middleware-0.1.2/src/auth_middleware/providers/cognito/settings.py
+-rw-r--r--   0        0        0      146 2024-04-06 12:22:35.514559 auth_middleware-0.1.2/src/auth_middleware/providers/entra_id/__init__.py
+-rw-r--r--   0        0        0     4176 2024-04-06 12:22:35.514559 auth_middleware-0.1.2/src/auth_middleware/providers/entra_id/entra_id_provider.py
+-rw-r--r--   0        0        0      184 2024-04-06 12:22:35.514559 auth_middleware-0.1.2/src/auth_middleware/providers/entra_id/exceptions.py
+-rw-r--r--   0        0        0      864 2024-04-06 12:22:35.514559 auth_middleware-0.1.2/src/auth_middleware/providers/entra_id/settings.py
+-rw-r--r--   0        0        0     1007 2024-04-06 12:22:35.514559 auth_middleware-0.1.2/src/auth_middleware/settings.py
+-rw-r--r--   0        0        0     1375 2024-04-06 12:22:35.514559 auth_middleware-0.1.2/src/auth_middleware/types.py
+-rw-r--r--   0        0        0     4366 1970-01-01 00:00:00.000000 auth_middleware-0.1.2/PKG-INFO
```

### Comparing `auth_middleware-0.1.1/LICENSE` & `auth_middleware-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `auth_middleware-0.1.1/pyproject.toml` & `auth_middleware-0.1.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "auth-middleware"
-version = "0.1.1"
+version = "0.1.2"
 description = "Async Auth Middleware for FastAPI/Starlette"
 authors = ["impalah <impalah@gmail.com>"]
 readme = "README.md"
 packages = [{include = "auth_middleware", from = "src"}]
 
 [tool.poetry.dependencies]
 python = "^3.12"
@@ -21,11 +21,13 @@
 pytest-mock = "^3.12.0"
 pytest-asyncio = "^0.23.3"
 mock = "^5.1.0"
 pytest-cov = "^4.1.0"
 black = "^23.12.1"
 pytest-env = "^1.1.3"
 mypy = "^1.8.0"
+sphinx = "^7.2.6"
+sphinx-rtd-theme = "^2.0.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `auth_middleware-0.1.1/src/auth_middleware/__init__.py` & `auth_middleware-0.1.2/src/auth_middleware/__init__.py`

 * *Files identical despite different names*

### Comparing `auth_middleware-0.1.1/src/auth_middleware/group_checker.py` & `auth_middleware-0.1.2/src/auth_middleware/group_checker.py`

 * *Files identical despite different names*

### Comparing `auth_middleware-0.1.1/src/auth_middleware/jwt_auth_middleware.py` & `auth_middleware-0.1.2/src/auth_middleware/jwt_auth_middleware.py`

 * *Files identical despite different names*

### Comparing `auth_middleware-0.1.1/src/auth_middleware/jwt_auth_provider.py` & `auth_middleware-0.1.2/src/auth_middleware/jwt_auth_provider.py`

 * *Files identical despite different names*

### Comparing `auth_middleware-0.1.1/src/auth_middleware/jwt_bearer_manager.py` & `auth_middleware-0.1.2/src/auth_middleware/jwt_bearer_manager.py`

 * *Files identical despite different names*

### Comparing `auth_middleware-0.1.1/src/auth_middleware/logging.py` & `auth_middleware-0.1.2/src/auth_middleware/logging.py`

 * *Files identical despite different names*

### Comparing `auth_middleware-0.1.1/src/auth_middleware/providers/cognito/cognito_provider.py` & `auth_middleware-0.1.2/src/auth_middleware/providers/cognito/cognito_provider.py`

 * *Files identical despite different names*

### Comparing `auth_middleware-0.1.1/src/auth_middleware/providers/cognito/settings.py` & `auth_middleware-0.1.2/src/auth_middleware/providers/cognito/settings.py`

 * *Files identical despite different names*

### Comparing `auth_middleware-0.1.1/src/auth_middleware/providers/entra_id/entra_id_provider.py` & `auth_middleware-0.1.2/src/auth_middleware/providers/entra_id/entra_id_provider.py`

 * *Files identical despite different names*

### Comparing `auth_middleware-0.1.1/src/auth_middleware/providers/entra_id/settings.py` & `auth_middleware-0.1.2/src/auth_middleware/providers/entra_id/settings.py`

 * *Files identical despite different names*

### Comparing `auth_middleware-0.1.1/src/auth_middleware/settings.py` & `auth_middleware-0.1.2/src/auth_middleware/settings.py`

 * *Files identical despite different names*

### Comparing `auth_middleware-0.1.1/src/auth_middleware/types.py` & `auth_middleware-0.1.2/src/auth_middleware/types.py`

 * *Files identical despite different names*

