# Comparing `tmp/multion-0.5.0.tar.gz` & `tmp/multion-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multion-0.5.0.tar", max compression
+gzip compressed data, was "multion-1.0.0.tar", max compression
```

## Comparing `multion-0.5.0.tar` & `multion-1.0.0.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0     3937 2024-04-05 19:55:43.250646 multion-0.5.0/README.md
--rw-r--r--   0        0        0      592 2024-04-05 19:55:43.250646 multion-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     1417 2024-04-05 19:55:43.250646 multion-0.5.0/src/multion/__init__.py
--rw-r--r--   0        0        0    15613 2024-04-05 19:55:43.250646 multion-0.5.0/src/multion/client.py
--rw-r--r--   0        0        0      853 2024-04-05 19:55:43.250646 multion-0.5.0/src/multion/core/__init__.py
--rw-r--r--   0        0        0      426 2024-04-05 19:55:43.250646 multion-0.5.0/src/multion/core/api_error.py
--rw-r--r--   0        0        0     1490 2024-04-05 19:55:43.250646 multion-0.5.0/src/multion/core/client_wrapper.py
--rw-r--r--   0        0        0     1047 2024-04-05 19:55:43.250646 multion-0.5.0/src/multion/core/datetime_utils.py
--rw-r--r--   0        0        0     1480 2024-04-05 19:55:43.250646 multion-0.5.0/src/multion/core/file.py
--rw-r--r--   0        0        0     5059 2024-04-05 19:55:43.250646 multion-0.5.0/src/multion/core/http_client.py
--rw-r--r--   0        0        0     3742 2024-04-05 19:55:43.250646 multion-0.5.0/src/multion/core/jsonable_encoder.py
--rw-r--r--   0        0        0      329 2024-04-05 19:55:43.250646 multion-0.5.0/src/multion/core/pydantic_utilities.py
--rw-r--r--   0        0        0      330 2024-04-05 19:55:43.254646 multion-0.5.0/src/multion/core/remove_none_from_dict.py
--rw-r--r--   0        0        0     1420 2024-04-05 19:55:43.254646 multion-0.5.0/src/multion/core/request_options.py
--rw-r--r--   0        0        0      162 2024-04-05 19:55:43.254646 multion-0.5.0/src/multion/environment.py
--rw-r--r--   0        0        0      385 2024-04-05 19:55:43.254646 multion-0.5.0/src/multion/errors/__init__.py
--rw-r--r--   0        0        0      301 2024-04-05 19:55:43.254646 multion-0.5.0/src/multion/errors/bad_request_error.py
--rw-r--r--   0        0        0      333 2024-04-05 19:55:43.254646 multion-0.5.0/src/multion/errors/internal_server_error.py
--rw-r--r--   0        0        0      308 2024-04-05 19:55:43.254646 multion-0.5.0/src/multion/errors/unauthorized_error.py
--rw-r--r--   0        0        0      313 2024-04-05 19:55:43.254646 multion-0.5.0/src/multion/errors/unprocessable_entity_error.py
--rw-r--r--   0        0        0        0 2024-04-05 19:55:43.254646 multion-0.5.0/src/multion/py.typed
--rw-r--r--   0        0        0      427 2024-04-05 19:55:43.254646 multion-0.5.0/src/multion/sessions/__init__.py
--rw-r--r--   0        0        0    28787 2024-04-05 19:55:43.254646 multion-0.5.0/src/multion/sessions/client.py
--rw-r--r--   0        0        0      590 2024-04-05 19:55:43.254646 multion-0.5.0/src/multion/sessions/types/__init__.py
--rw-r--r--   0        0        0     1024 2024-04-05 19:55:43.254646 multion-0.5.0/src/multion/sessions/types/create_session_input_browser_params.py
--rw-r--r--   0        0        0     1048 2024-04-05 19:55:43.254646 multion-0.5.0/src/multion/sessions/types/sessions_close_response.py
--rw-r--r--   0        0        0      953 2024-04-05 19:55:43.254646 multion-0.5.0/src/multion/sessions/types/sessions_list_response.py
--rw-r--r--   0        0        0      967 2024-04-05 19:55:43.254646 multion-0.5.0/src/multion/sessions/types/sessions_screenshot_response.py
--rw-r--r--   0        0        0     1022 2024-04-05 19:55:43.254646 multion-0.5.0/src/multion/sessions/types/step_session_input_browser_params.py
--rw-r--r--   0        0        0     1015 2024-04-05 19:55:43.254646 multion-0.5.0/src/multion/types/__init__.py
--rw-r--r--   0        0        0     1091 2024-04-05 19:55:43.254646 multion-0.5.0/src/multion/types/bad_request_response.py
--rw-r--r--   0        0        0     1355 2024-04-05 19:55:43.254646 multion-0.5.0/src/multion/types/browse_output.py
--rw-r--r--   0        0        0      953 2024-04-05 19:55:43.254646 multion-0.5.0/src/multion/types/http_validation_error.py
--rw-r--r--   0        0        0     1100 2024-04-05 19:55:43.254646 multion-0.5.0/src/multion/types/internal_server_error_response.py
--rw-r--r--   0        0        0     1096 2024-04-05 19:55:43.254646 multion-0.5.0/src/multion/types/payment_required_response.py
--rw-r--r--   0        0        0      850 2024-04-05 19:55:43.254646 multion-0.5.0/src/multion/types/remote_value.py
--rw-r--r--   0        0        0     1312 2024-04-05 19:55:43.254646 multion-0.5.0/src/multion/types/retrieve_output.py
--rw-r--r--   0        0        0     1361 2024-04-05 19:55:43.254646 multion-0.5.0/src/multion/types/session_created.py
--rw-r--r--   0        0        0     1365 2024-04-05 19:55:43.254646 multion-0.5.0/src/multion/types/session_step_success.py
--rw-r--r--   0        0        0     1093 2024-04-05 19:55:43.254646 multion-0.5.0/src/multion/types/unauthorized_response.py
--rw-r--r--   0        0        0      972 2024-04-05 19:55:43.254646 multion-0.5.0/src/multion/types/validation_error.py
--rw-r--r--   0        0        0      128 2024-04-05 19:55:43.254646 multion-0.5.0/src/multion/types/validation_error_loc_item.py
--rw-r--r--   0        0        0       75 2024-04-05 19:55:43.254646 multion-0.5.0/src/multion/version.py
--rw-r--r--   0        0        0     4427 1970-01-01 00:00:00.000000 multion-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     3937 2024-04-06 20:26:20.192376 multion-1.0.0/README.md
+-rw-r--r--   0        0        0      592 2024-04-06 20:26:20.192376 multion-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1417 2024-04-06 20:26:20.192376 multion-1.0.0/src/multion/__init__.py
+-rw-r--r--   0        0        0    15767 2024-04-06 20:26:20.192376 multion-1.0.0/src/multion/client.py
+-rw-r--r--   0        0        0      853 2024-04-06 20:26:20.192376 multion-1.0.0/src/multion/core/__init__.py
+-rw-r--r--   0        0        0      426 2024-04-06 20:26:20.192376 multion-1.0.0/src/multion/core/api_error.py
+-rw-r--r--   0        0        0     1490 2024-04-06 20:26:20.192376 multion-1.0.0/src/multion/core/client_wrapper.py
+-rw-r--r--   0        0        0     1047 2024-04-06 20:26:20.192376 multion-1.0.0/src/multion/core/datetime_utils.py
+-rw-r--r--   0        0        0     1480 2024-04-06 20:26:20.192376 multion-1.0.0/src/multion/core/file.py
+-rw-r--r--   0        0        0     5059 2024-04-06 20:26:20.192376 multion-1.0.0/src/multion/core/http_client.py
+-rw-r--r--   0        0        0     3742 2024-04-06 20:26:20.192376 multion-1.0.0/src/multion/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      329 2024-04-06 20:26:20.192376 multion-1.0.0/src/multion/core/pydantic_utilities.py
+-rw-r--r--   0        0        0      330 2024-04-06 20:26:20.192376 multion-1.0.0/src/multion/core/remove_none_from_dict.py
+-rw-r--r--   0        0        0     1420 2024-04-06 20:26:20.192376 multion-1.0.0/src/multion/core/request_options.py
+-rw-r--r--   0        0        0      162 2024-04-06 20:26:20.192376 multion-1.0.0/src/multion/environment.py
+-rw-r--r--   0        0        0      385 2024-04-06 20:26:20.192376 multion-1.0.0/src/multion/errors/__init__.py
+-rw-r--r--   0        0        0      301 2024-04-06 20:26:20.192376 multion-1.0.0/src/multion/errors/bad_request_error.py
+-rw-r--r--   0        0        0      333 2024-04-06 20:26:20.192376 multion-1.0.0/src/multion/errors/internal_server_error.py
+-rw-r--r--   0        0        0      308 2024-04-06 20:26:20.192376 multion-1.0.0/src/multion/errors/unauthorized_error.py
+-rw-r--r--   0        0        0      313 2024-04-06 20:26:20.192376 multion-1.0.0/src/multion/errors/unprocessable_entity_error.py
+-rw-r--r--   0        0        0        0 2024-04-06 20:26:20.192376 multion-1.0.0/src/multion/py.typed
+-rw-r--r--   0        0        0      427 2024-04-06 20:26:20.192376 multion-1.0.0/src/multion/sessions/__init__.py
+-rw-r--r--   0        0        0    28787 2024-04-06 20:26:20.192376 multion-1.0.0/src/multion/sessions/client.py
+-rw-r--r--   0        0        0      590 2024-04-06 20:26:20.192376 multion-1.0.0/src/multion/sessions/types/__init__.py
+-rw-r--r--   0        0        0     1024 2024-04-06 20:26:20.192376 multion-1.0.0/src/multion/sessions/types/create_session_input_browser_params.py
+-rw-r--r--   0        0        0     1048 2024-04-06 20:26:20.192376 multion-1.0.0/src/multion/sessions/types/sessions_close_response.py
+-rw-r--r--   0        0        0      953 2024-04-06 20:26:20.192376 multion-1.0.0/src/multion/sessions/types/sessions_list_response.py
+-rw-r--r--   0        0        0      967 2024-04-06 20:26:20.192376 multion-1.0.0/src/multion/sessions/types/sessions_screenshot_response.py
+-rw-r--r--   0        0        0     1022 2024-04-06 20:26:20.192376 multion-1.0.0/src/multion/sessions/types/step_session_input_browser_params.py
+-rw-r--r--   0        0        0     1015 2024-04-06 20:26:20.192376 multion-1.0.0/src/multion/types/__init__.py
+-rw-r--r--   0        0        0     1091 2024-04-06 20:26:20.192376 multion-1.0.0/src/multion/types/bad_request_response.py
+-rw-r--r--   0        0        0     1355 2024-04-06 20:26:20.192376 multion-1.0.0/src/multion/types/browse_output.py
+-rw-r--r--   0        0        0      953 2024-04-06 20:26:20.192376 multion-1.0.0/src/multion/types/http_validation_error.py
+-rw-r--r--   0        0        0     1100 2024-04-06 20:26:20.192376 multion-1.0.0/src/multion/types/internal_server_error_response.py
+-rw-r--r--   0        0        0     1096 2024-04-06 20:26:20.192376 multion-1.0.0/src/multion/types/payment_required_response.py
+-rw-r--r--   0        0        0      850 2024-04-06 20:26:20.192376 multion-1.0.0/src/multion/types/remote_value.py
+-rw-r--r--   0        0        0     1312 2024-04-06 20:26:20.192376 multion-1.0.0/src/multion/types/retrieve_output.py
+-rw-r--r--   0        0        0     1361 2024-04-06 20:26:20.192376 multion-1.0.0/src/multion/types/session_created.py
+-rw-r--r--   0        0        0     1365 2024-04-06 20:26:20.192376 multion-1.0.0/src/multion/types/session_step_success.py
+-rw-r--r--   0        0        0     1093 2024-04-06 20:26:20.192376 multion-1.0.0/src/multion/types/unauthorized_response.py
+-rw-r--r--   0        0        0      972 2024-04-06 20:26:20.192376 multion-1.0.0/src/multion/types/validation_error.py
+-rw-r--r--   0        0        0      128 2024-04-06 20:26:20.192376 multion-1.0.0/src/multion/types/validation_error_loc_item.py
+-rw-r--r--   0        0        0       75 2024-04-06 20:26:20.192376 multion-1.0.0/src/multion/version.py
+-rw-r--r--   0        0        0     4427 1970-01-01 00:00:00.000000 multion-1.0.0/PKG-INFO
```

### Comparing `multion-0.5.0/README.md` & `multion-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `multion-0.5.0/pyproject.toml` & `multion-1.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "multion"
-version = "0.5.0"
+version = "1.0.0"
 description = ""
 readme = "README.md"
 authors = []
 packages = [
     { include = "multion", from = "src"}
 ]
```

### Comparing `multion-0.5.0/src/multion/__init__.py` & `multion-1.0.0/src/multion/__init__.py`

 * *Files identical despite different names*

### Comparing `multion-0.5.0/src/multion/client.py` & `multion-1.0.0/src/multion/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,15 +113,16 @@
         ---
         from multion.client import MultiOn
 
         client = MultiOn(
             api_key="YOUR_API_KEY",
         )
         client.browse(
-            cmd="cmd",
+            cmd="find the top post on hackernews",
+            url="https://news.ycombinator.com/",
         )
         """
         _request: typing.Dict[str, typing.Any] = {"cmd": cmd}
         if url is not OMIT:
             _request["url"] = url
         if local is not OMIT:
             _request["local"] = local
@@ -262,15 +263,16 @@
         ---
         from multion.client import AsyncMultiOn
 
         client = AsyncMultiOn(
             api_key="YOUR_API_KEY",
         )
         await client.browse(
-            cmd="cmd",
+            cmd="find the top post on hackernews",
+            url="https://news.ycombinator.com/",
         )
         """
         _request: typing.Dict[str, typing.Any] = {"cmd": cmd}
         if url is not OMIT:
             _request["url"] = url
         if local is not OMIT:
             _request["local"] = local
```

### Comparing `multion-0.5.0/src/multion/core/__init__.py` & `multion-1.0.0/src/multion/core/__init__.py`

 * *Files identical despite different names*

### Comparing `multion-0.5.0/src/multion/core/client_wrapper.py` & `multion-1.0.0/src/multion/core/client_wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         self._base_url = base_url
         self._timeout = timeout
 
     def get_headers(self) -> typing.Dict[str, str]:
         headers: typing.Dict[str, str] = {
             "X-Fern-Language": "Python",
             "X-Fern-SDK-Name": "multion",
-            "X-Fern-SDK-Version": "0.5.0",
+            "X-Fern-SDK-Version": "1.0.0",
         }
         headers["X_MULTION_API_KEY"] = self.api_key
         return headers
 
     def get_base_url(self) -> str:
         return self._base_url
```

### Comparing `multion-0.5.0/src/multion/core/datetime_utils.py` & `multion-1.0.0/src/multion/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `multion-0.5.0/src/multion/core/file.py` & `multion-1.0.0/src/multion/core/file.py`

 * *Files identical despite different names*

### Comparing `multion-0.5.0/src/multion/core/http_client.py` & `multion-1.0.0/src/multion/core/http_client.py`

 * *Files identical despite different names*

### Comparing `multion-0.5.0/src/multion/core/jsonable_encoder.py` & `multion-1.0.0/src/multion/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `multion-0.5.0/src/multion/core/request_options.py` & `multion-1.0.0/src/multion/core/request_options.py`

 * *Files identical despite different names*

### Comparing `multion-0.5.0/src/multion/sessions/client.py` & `multion-1.0.0/src/multion/sessions/client.py`

 * *Files identical despite different names*

### Comparing `multion-0.5.0/src/multion/sessions/types/__init__.py` & `multion-1.0.0/src/multion/sessions/types/__init__.py`

 * *Files identical despite different names*

### Comparing `multion-0.5.0/src/multion/sessions/types/create_session_input_browser_params.py` & `multion-1.0.0/src/multion/sessions/types/create_session_input_browser_params.py`

 * *Files identical despite different names*

### Comparing `multion-0.5.0/src/multion/sessions/types/sessions_close_response.py` & `multion-1.0.0/src/multion/sessions/types/sessions_close_response.py`

 * *Files identical despite different names*

### Comparing `multion-0.5.0/src/multion/sessions/types/sessions_list_response.py` & `multion-1.0.0/src/multion/sessions/types/sessions_list_response.py`

 * *Files identical despite different names*

### Comparing `multion-0.5.0/src/multion/sessions/types/sessions_screenshot_response.py` & `multion-1.0.0/src/multion/sessions/types/sessions_screenshot_response.py`

 * *Files identical despite different names*

### Comparing `multion-0.5.0/src/multion/sessions/types/step_session_input_browser_params.py` & `multion-1.0.0/src/multion/sessions/types/step_session_input_browser_params.py`

 * *Files identical despite different names*

### Comparing `multion-0.5.0/src/multion/types/__init__.py` & `multion-1.0.0/src/multion/types/__init__.py`

 * *Files identical despite different names*

### Comparing `multion-0.5.0/src/multion/types/bad_request_response.py` & `multion-1.0.0/src/multion/types/bad_request_response.py`

 * *Files identical despite different names*

### Comparing `multion-0.5.0/src/multion/types/browse_output.py` & `multion-1.0.0/src/multion/types/browse_output.py`

 * *Files identical despite different names*

### Comparing `multion-0.5.0/src/multion/types/http_validation_error.py` & `multion-1.0.0/src/multion/types/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `multion-0.5.0/src/multion/types/internal_server_error_response.py` & `multion-1.0.0/src/multion/types/internal_server_error_response.py`

 * *Files identical despite different names*

### Comparing `multion-0.5.0/src/multion/types/payment_required_response.py` & `multion-1.0.0/src/multion/types/payment_required_response.py`

 * *Files identical despite different names*

### Comparing `multion-0.5.0/src/multion/types/remote_value.py` & `multion-1.0.0/src/multion/types/remote_value.py`

 * *Files identical despite different names*

### Comparing `multion-0.5.0/src/multion/types/retrieve_output.py` & `multion-1.0.0/src/multion/types/retrieve_output.py`

 * *Files identical despite different names*

### Comparing `multion-0.5.0/src/multion/types/session_created.py` & `multion-1.0.0/src/multion/types/session_created.py`

 * *Files identical despite different names*

### Comparing `multion-0.5.0/src/multion/types/session_step_success.py` & `multion-1.0.0/src/multion/types/session_step_success.py`

 * *Files identical despite different names*

### Comparing `multion-0.5.0/src/multion/types/unauthorized_response.py` & `multion-1.0.0/src/multion/types/unauthorized_response.py`

 * *Files identical despite different names*

### Comparing `multion-0.5.0/src/multion/types/validation_error.py` & `multion-1.0.0/src/multion/types/validation_error.py`

 * *Files identical despite different names*

### Comparing `multion-0.5.0/PKG-INFO` & `multion-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multion
-Version: 0.5.0
+Version: 1.0.0
 Summary: 
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

