# Comparing `tmp/outside-framework-1.3.3.tar.gz` & `tmp/outside-framework-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "outside-framework-1.3.3.tar", last modified: Mon Feb 26 12:54:37 2024, max compression
+gzip compressed data, was "outside-framework-1.4.0.tar", last modified: Sat Apr  6 14:52:27 2024, max compression
```

## Comparing `outside-framework-1.3.3.tar` & `outside-framework-1.4.0.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxrwxr-x   0 toni      (1000) toni      (1000)        0 2024-02-26 12:54:37.517699 outside-framework-1.3.3/
--rw-rw-r--   0 toni      (1000) toni      (1000)     1071 2024-02-14 10:41:30.000000 outside-framework-1.3.3/LICENSE
--rw-r--r--   0 toni      (1000) toni      (1000)     3728 2024-02-26 12:54:37.517699 outside-framework-1.3.3/PKG-INFO
--rw-rw-r--   0 toni      (1000) toni      (1000)     3176 2024-02-14 10:41:30.000000 outside-framework-1.3.3/README.md
--rw-rw-r--   0 toni      (1000) toni      (1000)      539 2024-02-26 12:54:03.000000 outside-framework-1.3.3/pyproject.toml
--rw-rw-r--   0 toni      (1000) toni      (1000)       38 2024-02-26 12:54:37.517699 outside-framework-1.3.3/setup.cfg
-drwxrwxr-x   0 toni      (1000) toni      (1000)        0 2024-02-26 12:54:37.513699 outside-framework-1.3.3/src/
-drwxrwxr-x   0 toni      (1000) toni      (1000)        0 2024-02-26 12:54:37.513699 outside-framework-1.3.3/src/outside/
--rw-rw-r--   0 toni      (1000) toni      (1000)     9242 2024-02-26 12:52:26.000000 outside-framework-1.3.3/src/outside/__init__.py
--rw-rw-r--   0 toni      (1000) toni      (1000)     1113 2024-02-26 12:52:48.000000 outside-framework-1.3.3/src/outside/__main__.py
--rw-rw-r--   0 toni      (1000) toni      (1000)     1823 2024-02-14 10:41:30.000000 outside-framework-1.3.3/src/outside/code_description.py
--rw-rw-r--   0 toni      (1000) toni      (1000)    17554 2024-02-14 10:41:30.000000 outside-framework-1.3.3/src/outside/protocol_http.py
-drwxrwxr-x   0 toni      (1000) toni      (1000)        0 2024-02-26 12:54:37.517699 outside-framework-1.3.3/src/outside_framework.egg-info/
--rw-r--r--   0 toni      (1000) toni      (1000)     3728 2024-02-26 12:54:37.000000 outside-framework-1.3.3/src/outside_framework.egg-info/PKG-INFO
--rw-rw-r--   0 toni      (1000) toni      (1000)      321 2024-02-26 12:54:37.000000 outside-framework-1.3.3/src/outside_framework.egg-info/SOURCES.txt
--rw-rw-r--   0 toni      (1000) toni      (1000)        1 2024-02-26 12:54:37.000000 outside-framework-1.3.3/src/outside_framework.egg-info/dependency_links.txt
--rw-rw-r--   0 toni      (1000) toni      (1000)        8 2024-02-26 12:54:37.000000 outside-framework-1.3.3/src/outside_framework.egg-info/top_level.txt
+drwxrwxr-x   0 bill      (1000) bill      (1000)        0 2024-04-06 14:52:27.195631 outside-framework-1.4.0/
+-rw-rw-r--   0 bill      (1000) bill      (1000)     1071 2024-04-06 14:52:06.000000 outside-framework-1.4.0/LICENSE
+-rw-r--r--   0 bill      (1000) bill      (1000)     3728 2024-04-06 14:52:27.195631 outside-framework-1.4.0/PKG-INFO
+-rw-rw-r--   0 bill      (1000) bill      (1000)     3176 2024-04-06 14:52:06.000000 outside-framework-1.4.0/README.md
+-rw-rw-r--   0 bill      (1000) bill      (1000)      539 2024-04-06 14:52:06.000000 outside-framework-1.4.0/pyproject.toml
+-rw-rw-r--   0 bill      (1000) bill      (1000)       38 2024-04-06 14:52:27.195631 outside-framework-1.4.0/setup.cfg
+drwxrwxr-x   0 bill      (1000) bill      (1000)        0 2024-04-06 14:52:27.195631 outside-framework-1.4.0/src/
+drwxrwxr-x   0 bill      (1000) bill      (1000)        0 2024-04-06 14:52:27.195631 outside-framework-1.4.0/src/outside/
+-rw-rw-r--   0 bill      (1000) bill      (1000)     9182 2024-04-06 14:52:06.000000 outside-framework-1.4.0/src/outside/__init__.py
+-rw-rw-r--   0 bill      (1000) bill      (1000)     1926 2024-04-06 14:52:06.000000 outside-framework-1.4.0/src/outside/__main__.py
+-rw-rw-r--   0 bill      (1000) bill      (1000)     1823 2024-04-06 14:52:06.000000 outside-framework-1.4.0/src/outside/code_description.py
+-rw-rw-r--   0 bill      (1000) bill      (1000)    19053 2024-04-06 14:52:06.000000 outside-framework-1.4.0/src/outside/protocol_http.py
+-rw-rw-r--   0 bill      (1000) bill      (1000)     4596 2024-04-06 14:52:06.000000 outside-framework-1.4.0/src/outside/protocol_websocket.py
+-rw-rw-r--   0 bill      (1000) bill      (1000)      202 2024-04-06 14:52:06.000000 outside-framework-1.4.0/src/outside/utility.py
+drwxrwxr-x   0 bill      (1000) bill      (1000)        0 2024-04-06 14:52:27.195631 outside-framework-1.4.0/src/outside_framework.egg-info/
+-rw-r--r--   0 bill      (1000) bill      (1000)     3728 2024-04-06 14:52:27.000000 outside-framework-1.4.0/src/outside_framework.egg-info/PKG-INFO
+-rw-rw-r--   0 bill      (1000) bill      (1000)      378 2024-04-06 14:52:27.000000 outside-framework-1.4.0/src/outside_framework.egg-info/SOURCES.txt
+-rw-rw-r--   0 bill      (1000) bill      (1000)        1 2024-04-06 14:52:27.000000 outside-framework-1.4.0/src/outside_framework.egg-info/dependency_links.txt
+-rw-rw-r--   0 bill      (1000) bill      (1000)        8 2024-04-06 14:52:27.000000 outside-framework-1.4.0/src/outside_framework.egg-info/top_level.txt
```

### Comparing `outside-framework-1.3.3/LICENSE` & `outside-framework-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `outside-framework-1.3.3/PKG-INFO` & `outside-framework-1.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: outside-framework
-Version: 1.3.3
+Version: 1.4.0
 Summary: An easy-to-use python web framework. Inspired by Flask.
 Author-email: BillPlayzToday <hello1502.channel@gmail.com>
 Project-URL: Homepage, https://github.com/BillPlayzToday/outside
 Project-URL: Issues, https://github.com/BillPlayzToday/outside/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `outside-framework-1.3.3/README.md` & `outside-framework-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `outside-framework-1.3.3/pyproject.toml` & `outside-framework-1.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "outside-framework"
-version = "1.3.3"
+version = "1.4.0"
 authors = [
     { name = "BillPlayzToday", email = "hello1502.channel@gmail.com" }
 ]
 description = "An easy-to-use python web framework. Inspired by Flask."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `outside-framework-1.3.3/src/outside/__init__.py` & `outside-framework-1.4.0/src/outside/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 import time
-import os
 import sys
 import socket
 import signal
 import multiprocessing
 import queue
 
-import outside.protocol_http as protocol_http
-import outside.code_description as code_description
+from . import protocol_http
+from . import code_description
 
 
 class OutsideHTTP:
     def __init__(self,host):
         self.config = {
             "host": ("0.0.0.0",80), # The Host (IP,Port)
             "backlog_length": 25, # Amount of parallel connections allowed (active or inactive)
@@ -145,15 +144,15 @@
                             running_process._terminating_at = current_time
             except OSError:
                 continue
             else:
                 new_queue = multiprocessing.Queue()
                 new_process = multiprocessing.Process(
                     target = protocol_http.process_request,
-                    name = f"(outside subprocess) HTTP Request from {address[0]}:{address[1]}",
+                    name = f"[outside] HTTP request from {address[0]}:{address[1]}",
                     daemon = True,
                     args = [new_queue,accepted_socket,address,self.config,self._route_names,self._routes,self._error_routes]
                 )
                 new_process.start()
                 new_process._last_activity = time.time()
                 new_process._socket_address = address
                 self._active_requests.append((new_process,new_queue))
```

### Comparing `outside-framework-1.3.3/src/outside/code_description.py` & `outside-framework-1.4.0/src/outside/code_description.py`

 * *Files identical despite different names*

### Comparing `outside-framework-1.3.3/src/outside/protocol_http.py` & `outside-framework-1.4.0/src/outside/protocol_http.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,52 +6,56 @@
 import mimetypes
 import time
 import http.cookies
 import urllib.parse
 import socket
 import signal
 import ssl
+import base64
+import hashlib
 
-import outside.code_description as code_description
+from . import code_description
+from . import protocol_websocket
 
 def process_request(activity_queue,connected_socket,address,config,route_names,routes,error_routes,is_reused = False):
     start_time = time.time()
     debug_name = f"{address[0]}:{str(address[1])}"
 
+    def terminate(signum = None,stackframe = None):
+        close_socket(connected_socket)
+        sys.exit(0)
+    
     def close_socket(unknown_socket):
         try:
             unknown_socket.shutdown(socket.SHUT_RDWR)
         except OSError:
             pass
 
         try:
             unknown_socket.close()
         except OSError:
             pass
-
-    def terminate(signum = None,stackframe = None):
-        close_socket(connected_socket)
-        sys.exit(0)
-
-    def recv(recv_size = config["recv_size"]):
+    
+    def get_socket():
         if (config["ssl_enabled"]):
-            return connected_ssl_socket.recv(recv_size)
+            return connected_ssl_socket
         else:
-            return connected_socket.recv(recv_size)
+            return connected_socket
+
+    def recv(recv_size = config["recv_size"]):
+        return get_socket().recv(recv_size)
 
     def send(data,append_file = None):
         send_size = config["send_size"]
         data_length = len(data)
         if (append_file):
             data_length = (data_length + (append_file.read_end - append_file.read_start))
         if (data_length > (config["big_definition_mb"] * 1024 * 1024)):
             send_size = (config["big_send_limit_mb"] * 1024 * 1024)
-        send_socket = connected_socket
-        if (config["ssl_enabled"]):
-            send_socket = connected_ssl_socket
+        send_socket = get_socket()
 
         while (len(data) > 0):
             send_socket.send(data[:send_size])
             data = data[send_size:]
             activity_queue.put(time.time())
 
         if (append_file):
@@ -83,15 +87,15 @@
                 except ssl.SSLError as exception:
                     if (exception.reason == "HTTP_REQUEST"):
                         terminate()
                     else:
                         raise
 
         # Begin Request Flow
-        request_class = Request("NONE",{},b"","HTTP/-1","/",address)
+        request_class = Request("",{},b"","","",address)
         # Receive Request Info + Headers
         print(f"[{debug_name} - INFO] Waiting for request info.")
         header_lines = [b""]
         while True:
             recv_data = recv()
             if (len(recv_data) == 0):
                 raise BrokenPipeError
@@ -118,14 +122,16 @@
                 request_class.params[param_name] = param_values[0]
         request_class.version = split_preline[2]
 
         for header_line in header_lines[1:]:
             split_line = header_line.decode("utf-8").split(": ")
             request_class.headers[split_line[0]] = split_line[1]
 
+        request_class._extract_cookies()
+
         print(f"[{debug_name} - INFO] Flow: {request_class.headers.get('Host') or ''}{request_class.url}")
 
         # Receive Body
         if (request_class.headers.get("Content-Length")):
             request_class.headers["Content-Length"] = int(request_class.headers["Content-Length"])
             if (not request_class.content):
                 request_class.content = b""
@@ -142,23 +148,40 @@
         responding_route = None
         for route_name in route_names:
             if (request_class.url.startswith(route_name)):
                 responding_route = routes[route_name]
                 break
         if (not responding_route):
             responding_route = error_routes[404]
+        if (isinstance(responding_route,protocol_websocket.WebSocket)):
+            print(f"[{debug_name} - INFO] Initializing websocket.")
+            if ((request_class.headers.get("Connection")) and ("Upgrade" in request_class.headers["Connection"]) and (request_class.headers.get("Upgrade") == "websocket") and (request_class.headers.get("Sec-WebSocket-Key"))):
+                websocket_connection = protocol_websocket.WebSocketConnection(request_class,get_socket(),activity_queue,terminate)
+            else:
+                print(f"[{debug_name} - ERROR] Handshake not accepted.")
+                responding_route = error_routes[400]
 
         # Respond
-        print(f"[{debug_name} - INFO] Generating response.")
-        request_class._extract_cookies()
-        scheduled_response_class = ScheduledResponse(request_class,responding_route,error_routes)
-        response_class = scheduled_response_class.run()
-        if (not response_class):
-            print(f"[{debug_name} - WARN] ScheduledResponse did not return Response, releasing process.")
-            terminate()
+        if (isinstance(responding_route,protocol_websocket.WebSocket)):
+            response_class = Response(
+                status_code = 101,
+                headers = {
+                    "Upgrade": "websocket",
+                    "Connection": "Upgrade",
+                    "Sec-Websocket-Accept": base64.b64encode(hashlib.sha1(f"{request_class.headers.get('Sec-WebSocket-Key')}258EAFA5-E914-47DA-95CA-C5AB0DC85B11".encode("utf-8")).digest()).decode("utf-8")
+                },
+                content = b""
+            )
+        else:
+            print(f"[{debug_name} - INFO] Generating response.")
+            scheduled_response_class = ScheduledResponse(request_class,responding_route,error_routes)
+            response_class = scheduled_response_class.run()
+            if (not response_class):
+                print(f"[{debug_name} - WARN] ScheduledResponse did not return Response, releasing process.")
+                terminate()
 
         content_is_file = isinstance(response_class.content,FilePath)
 
         if (content_is_file):
             content_length = os.path.getsize(response_class.content.path)
             if ((config["allow_range_from_mb"] != -1) and (config["allow_range_from_mb"] < (content_length / 1024 / 1024))):
                 response_class.headers["Accept-Ranges"] = "bytes"
@@ -191,27 +214,28 @@
         content_is_file = isinstance(response_class.content,FilePath)
         if (content_is_file):
             response_class.headers["Content-Length"] = (response_class.content.read_end - response_class.content.read_start)
         else:
             response_class.headers["Content-Length"] = len(response_class.content)
         
         socket_keep_alive = False
-        if ((config["keep_alive"]) and (request_class.headers.get("Connection") == "keep-alive")):
-            response_class.headers["Connection"] = "keep-alive"
-            socket_keep_alive = True
-        else:
-            response_class.headers["Connection"] = "close"
+        if (not response_class.headers.get("Connection")):
+            if ((config["keep_alive"]) and (request_class.headers.get("Connection") == "keep-alive")):
+                response_class.headers["Connection"] = "keep-alive"
+                socket_keep_alive = True
+            else:
+                response_class.headers["Connection"] = "close"
 
-        response_data = (b"HTTP/1.1 " + str(response_class.status_code).encode("utf-8") + b" " + code_description.get_description(response_class.status_code).encode("utf-8") + b"\n")
+        response_data = (b"HTTP/1.1 " + str(response_class.status_code).encode("utf-8") + b" " + code_description.get_description(response_class.status_code).encode("utf-8") + b"\r\n")
 
         for header_name in response_class.headers:
             header_value = response_class.headers[header_name]
             if (isinstance(header_value,int)):
                 header_value = str(header_value)
-            response_data = (response_data + header_name.encode("utf-8") + b": " + header_value.encode("utf-8") + b"\n")
+            response_data = (response_data + header_name.encode("utf-8") + b": " + header_value.encode("utf-8") + b"\r\n")
 
         if (response_class.headers.get("Set-Cookie")):
             print(f"[{debug_name} - ERROR] Set-Cookie header was returned by ScheduledResponse, use add_cookie instead.")
             terminate()
         for cookie_name,cookie_value in response_class.cookies.items():
             response_data = (response_data + b"Set-Cookie: " + cookie_name.encode("utf-8") + b"=" + cookie_value.value.encode("utf-8"))
             if (cookie_value.max_age):
@@ -222,25 +246,30 @@
                 response_data = (response_data + f"; HttpOnly".encode("utf-8"))
             if (cookie_value.secure):
                 response_data = (response_data + f"; Secure".encode("utf-8"))
             if (cookie_value.path):
                 response_data = (response_data + f"; Path={cookie_value.path}".encode("utf-8"))
             if (cookie_value.same_site):
                 response_data = (response_data + f"; SameSite={cookie_value.same_site}".encode("utf-8"))
-            response_data = (response_data + b"\n")
+            response_data = (response_data + b"\r\n")
 
         print(f"[{debug_name} - INFO] Sending response.")
         if (content_is_file):
-            response_data = (response_data + b"\n")
+            response_data = (response_data + b"\r\n")
             send(response_data,response_class.content)
         else:
-            response_data = (response_data + b"\n" + response_class.content)
+            response_data = (response_data + b"\r\n" + response_class.content)
             send(response_data)
 
-        print(f"[{debug_name} - INFO] Code {str(response_class.status_code)} in {str((time.time() - start_time) / 1000)}ms.")
+        print(f"[{debug_name} - INFO] Code {str(response_class.status_code)} in {str(round((time.time() - start_time) / 1000 / 1000) * 1000)}ms.")
+        if (isinstance(responding_route,protocol_websocket.WebSocket)):
+            print(f"[{debug_name} - INFO] Handshake complete.")
+            responding_route.connection_handler(websocket_connection)
+            websocket_connection.exit()
+        
         if (config["post_callback"]):
             config["post_callback"](request_class,response_class)
         if (socket_keep_alive):
             print(f"[{debug_name} - INFO] Waiting for further requests.")
             reuse_socket = connected_socket
             if (config["ssl_enabled"]):
                 reuse_socket = connected_ssl_socket
@@ -346,18 +375,14 @@
                 print(f"[{self.request.address[0]} - ERROR] Response content type ({type(generated_response.content).__name__}) is not supported.")
                 raise NotImplementedError
         elif (not isinstance(generated_response.content,bytes)):
             generated_response.content = generated_response.content.encode("utf-8")
 
         return generated_response
 
-class Websocket:
-    def __init__(self):
-        pass # TODO
-
 class FilePath:
     def __init__(self,path):
         self.path = path
         self.read_start = 0
         self.read_end = os.path.getsize(self.path)
         self._content = None
```

### Comparing `outside-framework-1.3.3/src/outside_framework.egg-info/PKG-INFO` & `outside-framework-1.4.0/src/outside_framework.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: outside-framework
-Version: 1.3.3
+Version: 1.4.0
 Summary: An easy-to-use python web framework. Inspired by Flask.
 Author-email: BillPlayzToday <hello1502.channel@gmail.com>
 Project-URL: Homepage, https://github.com/BillPlayzToday/outside
 Project-URL: Issues, https://github.com/BillPlayzToday/outside/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

