# Comparing `tmp/cheeseapi-0.4.8.tar.gz` & `tmp/cheeseapi-0.4.9.tar.gz`

## Comparing `cheeseapi-0.4.8.tar` & `cheeseapi-0.4.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 cheeseapi-0.4.8/CheeseAPI/__init__.py
--rw-r--r--   0        0        0     2033 2020-02-02 00:00:00.000000 cheeseapi-0.4.8/CheeseAPI/app.py
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 cheeseapi-0.4.8/CheeseAPI/cors.py
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 cheeseapi-0.4.8/CheeseAPI/exception.py
--rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 cheeseapi-0.4.8/CheeseAPI/file.py
--rw-r--r--   0        0        0    30868 2020-02-02 00:00:00.000000 cheeseapi-0.4.8/CheeseAPI/handle.py
--rw-r--r--   0        0        0     4191 2020-02-02 00:00:00.000000 cheeseapi-0.4.8/CheeseAPI/protocol.py
--rw-r--r--   0        0        0     2753 2020-02-02 00:00:00.000000 cheeseapi-0.4.8/CheeseAPI/request.py
--rw-r--r--   0        0        0    14572 2020-02-02 00:00:00.000000 cheeseapi-0.4.8/CheeseAPI/response.py
--rw-r--r--   0        0        0     6814 2020-02-02 00:00:00.000000 cheeseapi-0.4.8/CheeseAPI/route.py
--rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 cheeseapi-0.4.8/CheeseAPI/server.py
--rw-r--r--   0        0        0     2362 2020-02-02 00:00:00.000000 cheeseapi-0.4.8/CheeseAPI/signal.py
--rw-r--r--   0        0        0     7664 2020-02-02 00:00:00.000000 cheeseapi-0.4.8/CheeseAPI/text.py
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 cheeseapi-0.4.8/CheeseAPI/websocket.py
--rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 cheeseapi-0.4.8/CheeseAPI/workspace.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 cheeseapi-0.4.8/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 cheeseapi-0.4.8/LICENSE
--rw-r--r--   0        0        0     4566 2020-02-02 00:00:00.000000 cheeseapi-0.4.8/README.md
--rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 cheeseapi-0.4.8/pyproject.toml
--rw-r--r--   0        0        0     5024 2020-02-02 00:00:00.000000 cheeseapi-0.4.8/PKG-INFO
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 cheeseapi-0.4.9/CheeseAPI/__init__.py
+-rw-r--r--   0        0        0     2033 2020-02-02 00:00:00.000000 cheeseapi-0.4.9/CheeseAPI/app.py
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 cheeseapi-0.4.9/CheeseAPI/cors.py
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 cheeseapi-0.4.9/CheeseAPI/exception.py
+-rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 cheeseapi-0.4.9/CheeseAPI/file.py
+-rw-r--r--   0        0        0    30687 2020-02-02 00:00:00.000000 cheeseapi-0.4.9/CheeseAPI/handle.py
+-rw-r--r--   0        0        0     4191 2020-02-02 00:00:00.000000 cheeseapi-0.4.9/CheeseAPI/protocol.py
+-rw-r--r--   0        0        0     2753 2020-02-02 00:00:00.000000 cheeseapi-0.4.9/CheeseAPI/request.py
+-rw-r--r--   0        0        0    14572 2020-02-02 00:00:00.000000 cheeseapi-0.4.9/CheeseAPI/response.py
+-rw-r--r--   0        0        0     6814 2020-02-02 00:00:00.000000 cheeseapi-0.4.9/CheeseAPI/route.py
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 cheeseapi-0.4.9/CheeseAPI/server.py
+-rw-r--r--   0        0        0     2362 2020-02-02 00:00:00.000000 cheeseapi-0.4.9/CheeseAPI/signal.py
+-rw-r--r--   0        0        0     7664 2020-02-02 00:00:00.000000 cheeseapi-0.4.9/CheeseAPI/text.py
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 cheeseapi-0.4.9/CheeseAPI/websocket.py
+-rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 cheeseapi-0.4.9/CheeseAPI/workspace.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 cheeseapi-0.4.9/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 cheeseapi-0.4.9/LICENSE
+-rw-r--r--   0        0        0     4566 2020-02-02 00:00:00.000000 cheeseapi-0.4.9/README.md
+-rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 cheeseapi-0.4.9/pyproject.toml
+-rw-r--r--   0        0        0     5024 2020-02-02 00:00:00.000000 cheeseapi-0.4.9/PKG-INFO
```

### Comparing `cheeseapi-0.4.8/CheeseAPI/app.py` & `cheeseapi-0.4.9/CheeseAPI/app.py`

 * *Files identical despite different names*

### Comparing `cheeseapi-0.4.8/CheeseAPI/file.py` & `cheeseapi-0.4.9/CheeseAPI/file.py`

 * *Files identical despite different names*

### Comparing `cheeseapi-0.4.8/CheeseAPI/handle.py` & `cheeseapi-0.4.9/CheeseAPI/handle.py`

 * *Files 0% similar despite different names*

```diff
@@ -271,15 +271,14 @@
                             'response': protocol.response,
                             **protocol.kwargs
                         })
                     await self.http_response(protocol)
                     return
 
                 if e.args[0] == 1:
-                    await self.http_options(protocol)
                     if isinstance(protocol.response, BaseResponse):
                         if self._app.signal.http_options.receivers:
                             await self._app.signal.http_options.send_async(**{
                                 'request': protocol.request,
                                 'response': protocol.response,
                                 **protocol.kwargs
                             })
@@ -346,18 +345,39 @@
                     })
             except (FileNotFoundError, IsADirectoryError):
                 ...
 
     async def http_404(self, protocol: 'HttpProtocol'):
         protocol.response = Response(status = http.HTTPStatus.NOT_FOUND)
 
-    async def http_options(self, protocol: 'HttpProtocol'):
+    async def http_405(self, protocol: 'HttpProtocol'):
+        protocol.response = Response(status = http.HTTPStatus.METHOD_NOT_ALLOWED)
+
+    async def http_500(self, protocol: 'HttpProtocol', e: BaseException, recycled: bool = False):
+        protocol.response = Response(status = http.HTTPStatus.INTERNAL_SERVER_ERROR)
+
+        if not recycled:
+            for text in self._app._text.http_500(protocol, e):
+                logger.danger(text[0], text[1])
+
+    async def http_response(self, protocol: 'HttpProtocol', recycled: bool = False):
+        if not isinstance(protocol.response, BaseResponse):
+            await self.noResponse(protocol)
+
+        if not recycled:
+            await self.http_beforeResponse(protocol)
+            if self._app.signal.http_beforeResponse.receivers:
+                await self._app.signal.http_beforeResponse.send_async(**{
+                    'request': protocol.request,
+                    'response': protocol.response,
+                    **protocol.kwargs
+                })
+
         if (
-            protocol.request.method == http.HTTPMethod.OPTIONS
-            and (
+            (
                 protocol.request.origin not in self._app.cors.exclude_origin
                 and
                 (
                     self._app.cors.origin == '*'
                     or
                     protocol.request.origin in self._app.cors.origin
                 )
@@ -376,37 +396,14 @@
                 protocol.response.headers['Access-Control-Allow-Methods'] = ', '.join(self._app.cors.methods - self._app.cors.exclude_methods)
 
             if self._app.cors.headers == '*':
                 protocol.response.headers['Access-Control-Allow-Headers'] = self._app.cors.headers
             elif self._app.cors.headers:
                 protocol.response.headers['Access-Control-Allow-Headers'] = ', '.join(self._app.cors.headers)
 
-    async def http_405(self, protocol: 'HttpProtocol'):
-        protocol.response = Response(status = http.HTTPStatus.METHOD_NOT_ALLOWED)
-
-    async def http_500(self, protocol: 'HttpProtocol', e: BaseException, recycled: bool = False):
-        protocol.response = Response(status = http.HTTPStatus.INTERNAL_SERVER_ERROR)
-
-        if not recycled:
-            for text in self._app._text.http_500(protocol, e):
-                logger.danger(text[0], text[1])
-
-    async def http_response(self, protocol: 'HttpProtocol', recycled: bool = False):
-        if not isinstance(protocol.response, BaseResponse):
-            await self.noResponse(protocol)
-
-        if not recycled:
-            await self.http_beforeResponse(protocol)
-            if self._app.signal.http_beforeResponse.receivers:
-                await self._app.signal.http_beforeResponse.send_async(**{
-                    'request': protocol.request,
-                    'response': protocol.response,
-                    **protocol.kwargs
-                })
-
         try:
             content, streamed = await protocol.response()
             protocol.transport.write(content)
             while streamed:
                 content, streamed = await protocol.response()
                 protocol.transport.write(content)
         except RuntimeError:
```

### Comparing `cheeseapi-0.4.8/CheeseAPI/protocol.py` & `cheeseapi-0.4.9/CheeseAPI/protocol.py`

 * *Files identical despite different names*

### Comparing `cheeseapi-0.4.8/CheeseAPI/request.py` & `cheeseapi-0.4.9/CheeseAPI/request.py`

 * *Files identical despite different names*

### Comparing `cheeseapi-0.4.8/CheeseAPI/response.py` & `cheeseapi-0.4.9/CheeseAPI/response.py`

 * *Files identical despite different names*

### Comparing `cheeseapi-0.4.8/CheeseAPI/route.py` & `cheeseapi-0.4.9/CheeseAPI/route.py`

 * *Files identical despite different names*

### Comparing `cheeseapi-0.4.8/CheeseAPI/server.py` & `cheeseapi-0.4.9/CheeseAPI/server.py`

 * *Files identical despite different names*

### Comparing `cheeseapi-0.4.8/CheeseAPI/signal.py` & `cheeseapi-0.4.9/CheeseAPI/signal.py`

 * *Files identical despite different names*

### Comparing `cheeseapi-0.4.8/CheeseAPI/text.py` & `cheeseapi-0.4.9/CheeseAPI/text.py`

 * *Files identical despite different names*

### Comparing `cheeseapi-0.4.8/CheeseAPI/websocket.py` & `cheeseapi-0.4.9/CheeseAPI/websocket.py`

 * *Files identical despite different names*

### Comparing `cheeseapi-0.4.8/CheeseAPI/workspace.py` & `cheeseapi-0.4.9/CheeseAPI/workspace.py`

 * *Files identical despite different names*

### Comparing `cheeseapi-0.4.8/LICENSE` & `cheeseapi-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cheeseapi-0.4.8/README.md` & `cheeseapi-0.4.9/README.md`

 * *Files identical despite different names*

### Comparing `cheeseapi-0.4.8/pyproject.toml` & `cheeseapi-0.4.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "hatchling" ]
 build-backend = "hatchling.build"
 
 [project]
 name = "CheeseAPI"
-version = "0.4.8"
+version = "0.4.9"
 description = "一款web协程框架。"
 readme = "README.md"
 license-files = { paths = [ "LICENSE" ] }
 authors = [
     { name = "Cheese Unknown", email = "cheese@cheese.ren" }
 ]
 keywords = [ 'API', 'BackEnd' ]
```

### Comparing `cheeseapi-0.4.8/PKG-INFO` & `cheeseapi-0.4.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: CheeseAPI
-Version: 0.4.8
+Version: 0.4.9
 Summary: 一款web协程框架。
 Project-URL: Source, https://github.com/CheeseUnknown/CheeseAPI
 Author-email: Cheese Unknown <cheese@cheese.ren>
 License-File: LICENSE
 Keywords: API,BackEnd
 Requires-Dist: blinker
 Requires-Dist: cheeselog
```

