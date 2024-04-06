# Comparing `tmp/twikit-1.4.3.tar.gz` & `tmp/twikit-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twikit-1.4.3.tar", last modified: Fri Apr  5 01:16:04 2024, max compression
+gzip compressed data, was "twikit-1.4.4.tar", last modified: Sat Apr  6 04:32:09 2024, max compression
```

## Comparing `twikit-1.4.3.tar` & `twikit-1.4.4.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0        0        0        0 2024-04-05 01:16:04.417485 twikit-1.4.3/
--rw-rw-rw-   0        0        0     1079 2024-03-23 06:08:25.000000 twikit-1.4.3/LICENSE
--rw-rw-rw-   0        0        0     3534 2024-04-05 01:16:04.414492 twikit-1.4.3/PKG-INFO
--rw-rw-rw-   0        0        0     3264 2024-03-23 06:08:25.000000 twikit-1.4.3/README.md
--rw-rw-rw-   0        0        0       42 2024-04-05 01:16:04.417485 twikit-1.4.3/setup.cfg
--rw-rw-rw-   0        0        0      693 2024-03-28 12:25:18.000000 twikit-1.4.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-05 01:16:04.309772 twikit-1.4.3/twikit/
--rw-rw-rw-   0        0        0      601 2024-04-05 01:12:09.000000 twikit-1.4.3/twikit/__init__.py
--rw-rw-rw-   0        0        0   107913 2024-04-05 01:08:17.000000 twikit-1.4.3/twikit/client.py
--rw-rw-rw-   0        0        0     2076 2024-03-29 07:12:11.000000 twikit-1.4.3/twikit/errors.py
--rw-rw-rw-   0        0        0     6983 2024-04-02 02:28:49.000000 twikit-1.4.3/twikit/group.py
--rw-rw-rw-   0        0        0     1887 2024-04-01 07:48:50.000000 twikit-1.4.3/twikit/http.py
--rw-rw-rw-   0        0        0     7399 2024-04-02 02:28:12.000000 twikit-1.4.3/twikit/list.py
--rw-rw-rw-   0        0        0     3800 2024-03-23 06:08:25.000000 twikit-1.4.3/twikit/message.py
--rw-rw-rw-   0        0        0     1385 2024-03-23 06:08:25.000000 twikit-1.4.3/twikit/notification.py
--rw-rw-rw-   0        0        0     1034 2024-03-23 06:08:25.000000 twikit-1.4.3/twikit/trend.py
--rw-rw-rw-   0        0        0    16644 2024-04-02 02:26:56.000000 twikit-1.4.3/twikit/tweet.py
-drwxrwxrwx   0        0        0        0 2024-04-05 01:16:04.409506 twikit-1.4.3/twikit/twikit_async/
--rw-rw-rw-   0        0        0      553 2024-03-23 06:08:25.000000 twikit-1.4.3/twikit/twikit_async/__init__.py
--rw-rw-rw-   0        0        0   111344 2024-04-05 01:04:43.000000 twikit-1.4.3/twikit/twikit_async/client.py
--rw-rw-rw-   0        0        0      875 2024-03-23 06:08:25.000000 twikit-1.4.3/twikit/twikit_async/errors.py
--rw-rw-rw-   0        0        0     7177 2024-04-02 02:30:57.000000 twikit-1.4.3/twikit/twikit_async/group.py
--rw-rw-rw-   0        0        0     1929 2024-03-23 06:08:25.000000 twikit-1.4.3/twikit/twikit_async/http.py
--rw-rw-rw-   0        0        0     7562 2024-04-02 02:30:39.000000 twikit-1.4.3/twikit/twikit_async/list.py
--rw-rw-rw-   0        0        0     3866 2024-03-23 06:08:25.000000 twikit-1.4.3/twikit/twikit_async/message.py
--rw-rw-rw-   0        0        0     1385 2024-03-23 06:08:25.000000 twikit-1.4.3/twikit/twikit_async/notification.py
--rw-rw-rw-   0        0        0     1034 2024-03-23 06:08:25.000000 twikit-1.4.3/twikit/twikit_async/trend.py
--rw-rw-rw-   0        0        0    16751 2024-04-02 02:29:48.000000 twikit-1.4.3/twikit/twikit_async/tweet.py
--rw-rw-rw-   0        0        0    14128 2024-04-02 02:29:20.000000 twikit-1.4.3/twikit/twikit_async/user.py
--rw-rw-rw-   0        0        0     3354 2024-04-02 05:30:54.000000 twikit-1.4.3/twikit/twikit_async/utils.py
--rw-rw-rw-   0        0        0    13905 2024-04-02 02:27:48.000000 twikit-1.4.3/twikit/user.py
--rw-rw-rw-   0        0        0    20911 2024-04-05 01:12:40.000000 twikit-1.4.3/twikit/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-05 01:16:04.327725 twikit-1.4.3/twikit.egg-info/
--rw-rw-rw-   0        0        0     3534 2024-04-05 01:16:04.000000 twikit-1.4.3/twikit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      737 2024-04-05 01:16:04.000000 twikit-1.4.3/twikit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 01:16:04.000000 twikit-1.4.3/twikit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2024-04-05 01:16:04.000000 twikit-1.4.3/twikit.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-05 01:16:04.000000 twikit-1.4.3/twikit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-06 04:32:09.805292 twikit-1.4.4/
+-rw-rw-rw-   0        0        0     1079 2024-03-23 06:08:25.000000 twikit-1.4.4/LICENSE
+-rw-rw-rw-   0        0        0     3534 2024-04-06 04:32:09.802303 twikit-1.4.4/PKG-INFO
+-rw-rw-rw-   0        0        0     3264 2024-03-23 06:08:25.000000 twikit-1.4.4/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-06 04:32:09.805292 twikit-1.4.4/setup.cfg
+-rw-rw-rw-   0        0        0      693 2024-03-28 12:25:18.000000 twikit-1.4.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-06 04:32:09.731489 twikit-1.4.4/twikit/
+-rw-rw-rw-   0        0        0      601 2024-04-06 04:32:07.000000 twikit-1.4.4/twikit/__init__.py
+-rw-rw-rw-   0        0        0   107913 2024-04-05 18:02:49.000000 twikit-1.4.4/twikit/client.py
+-rw-rw-rw-   0        0        0     2380 2024-04-06 04:29:07.000000 twikit-1.4.4/twikit/errors.py
+-rw-rw-rw-   0        0        0     6983 2024-04-02 02:28:49.000000 twikit-1.4.4/twikit/group.py
+-rw-rw-rw-   0        0        0     1913 2024-04-06 04:28:27.000000 twikit-1.4.4/twikit/http.py
+-rw-rw-rw-   0        0        0     7399 2024-04-02 02:28:12.000000 twikit-1.4.4/twikit/list.py
+-rw-rw-rw-   0        0        0     3800 2024-03-23 06:08:25.000000 twikit-1.4.4/twikit/message.py
+-rw-rw-rw-   0        0        0     1385 2024-03-23 06:08:25.000000 twikit-1.4.4/twikit/notification.py
+-rw-rw-rw-   0        0        0     1034 2024-03-23 06:08:25.000000 twikit-1.4.4/twikit/trend.py
+-rw-rw-rw-   0        0        0    16644 2024-04-02 02:26:56.000000 twikit-1.4.4/twikit/tweet.py
+drwxrwxrwx   0        0        0        0 2024-04-06 04:32:09.798312 twikit-1.4.4/twikit/twikit_async/
+-rw-rw-rw-   0        0        0      553 2024-03-23 06:08:25.000000 twikit-1.4.4/twikit/twikit_async/__init__.py
+-rw-rw-rw-   0        0        0   111344 2024-04-05 01:04:43.000000 twikit-1.4.4/twikit/twikit_async/client.py
+-rw-rw-rw-   0        0        0      875 2024-03-23 06:08:25.000000 twikit-1.4.4/twikit/twikit_async/errors.py
+-rw-rw-rw-   0        0        0     7177 2024-04-02 02:30:57.000000 twikit-1.4.4/twikit/twikit_async/group.py
+-rw-rw-rw-   0        0        0     1955 2024-04-06 04:28:33.000000 twikit-1.4.4/twikit/twikit_async/http.py
+-rw-rw-rw-   0        0        0     7562 2024-04-02 02:30:39.000000 twikit-1.4.4/twikit/twikit_async/list.py
+-rw-rw-rw-   0        0        0     3866 2024-03-23 06:08:25.000000 twikit-1.4.4/twikit/twikit_async/message.py
+-rw-rw-rw-   0        0        0     1385 2024-03-23 06:08:25.000000 twikit-1.4.4/twikit/twikit_async/notification.py
+-rw-rw-rw-   0        0        0     1034 2024-03-23 06:08:25.000000 twikit-1.4.4/twikit/twikit_async/trend.py
+-rw-rw-rw-   0        0        0    16751 2024-04-02 02:29:48.000000 twikit-1.4.4/twikit/twikit_async/tweet.py
+-rw-rw-rw-   0        0        0    14128 2024-04-02 02:29:20.000000 twikit-1.4.4/twikit/twikit_async/user.py
+-rw-rw-rw-   0        0        0     3354 2024-04-02 05:30:54.000000 twikit-1.4.4/twikit/twikit_async/utils.py
+-rw-rw-rw-   0        0        0    13905 2024-04-02 02:27:48.000000 twikit-1.4.4/twikit/user.py
+-rw-rw-rw-   0        0        0    20911 2024-04-05 01:12:40.000000 twikit-1.4.4/twikit/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-06 04:32:09.749442 twikit-1.4.4/twikit.egg-info/
+-rw-rw-rw-   0        0        0     3534 2024-04-06 04:32:09.000000 twikit-1.4.4/twikit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      737 2024-04-06 04:32:09.000000 twikit-1.4.4/twikit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-06 04:32:09.000000 twikit-1.4.4/twikit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2024-04-06 04:32:09.000000 twikit-1.4.4/twikit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-06 04:32:09.000000 twikit-1.4.4/twikit.egg-info/top_level.txt
```

### Comparing `twikit-1.4.3/LICENSE` & `twikit-1.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `twikit-1.4.3/PKG-INFO` & `twikit-1.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twikit
-Version: 1.4.3
+Version: 1.4.4
 Summary: Twitter API wrapper for python with **no API key required**.
 Home-page: https://github.com/d60/twikit
 License: MIT
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `twikit-1.4.3/README.md` & `twikit-1.4.4/README.md`

 * *Files identical despite different names*

### Comparing `twikit-1.4.3/setup.py` & `twikit-1.4.4/setup.py`

 * *Files identical despite different names*

### Comparing `twikit-1.4.3/twikit/__init__.py` & `twikit-1.4.4/twikit/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,8 +21,8 @@
 )
 from .message import Message
 from .trend import Trend
 from .tweet import ScheduledTweet, Tweet
 from .user import User
 from .utils import build_query
 
-__version__ = '1.4.3'
+__version__ = '1.4.4'
```

### Comparing `twikit-1.4.3/twikit/client.py` & `twikit-1.4.4/twikit/client.py`

 * *Files identical despite different names*

### Comparing `twikit-1.4.3/twikit/errors.py` & `twikit-1.4.4/twikit/errors.py`

 * *Files 14% similar despite different names*

```diff
@@ -28,14 +28,20 @@
     Exception raised for 408 Request Timeout errors.
     """
 
 class TooManyRequests(TwitterException):
     """
     Exception raised for 429 Too Many Requests errors.
     """
+    def __init__(self, *args, headers: dict | None = None) -> None:
+        super().__init__(*args)
+        if headers is not None and 'x-rate-limit-reset' in headers:
+            self.rate_limit_reset = int(headers.get('x-rate-limit-reset'))
+        else:
+            self.rate_limit_reset = None
 
 class ServerError(TwitterException):
     """
     Exception raised for 5xx Server Error responses.
     """
 
 class CouldNotTweet(TwitterException):
```

### Comparing `twikit-1.4.3/twikit/group.py` & `twikit-1.4.4/twikit/group.py`

 * *Files identical despite different names*

### Comparing `twikit-1.4.3/twikit/http.py` & `twikit-1.4.4/twikit/http.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,15 +35,15 @@
             elif status_code == 403:
                 raise Forbidden(message)
             elif status_code == 404:
                 raise NotFound(message)
             elif status_code == 408:
                 raise RequestTimeout(message)
             elif status_code == 429:
-                raise TooManyRequests(message)
+                raise TooManyRequests(message, headers=response.headers)
             elif 500 <= status_code < 600:
                 raise ServerError(message)
             else:
                 raise TwitterException(message)
 
         return response
```

### Comparing `twikit-1.4.3/twikit/list.py` & `twikit-1.4.4/twikit/list.py`

 * *Files identical despite different names*

### Comparing `twikit-1.4.3/twikit/message.py` & `twikit-1.4.4/twikit/message.py`

 * *Files identical despite different names*

### Comparing `twikit-1.4.3/twikit/notification.py` & `twikit-1.4.4/twikit/notification.py`

 * *Files identical despite different names*

### Comparing `twikit-1.4.3/twikit/trend.py` & `twikit-1.4.4/twikit/trend.py`

 * *Files identical despite different names*

### Comparing `twikit-1.4.3/twikit/tweet.py` & `twikit-1.4.4/twikit/tweet.py`

 * *Files identical despite different names*

### Comparing `twikit-1.4.3/twikit/twikit_async/__init__.py` & `twikit-1.4.4/twikit/twikit_async/__init__.py`

 * *Files identical despite different names*

### Comparing `twikit-1.4.3/twikit/twikit_async/client.py` & `twikit-1.4.4/twikit/twikit_async/client.py`

 * *Files identical despite different names*

### Comparing `twikit-1.4.3/twikit/twikit_async/errors.py` & `twikit-1.4.4/twikit/twikit_async/errors.py`

 * *Files identical despite different names*

### Comparing `twikit-1.4.3/twikit/twikit_async/group.py` & `twikit-1.4.4/twikit/twikit_async/group.py`

 * *Files identical despite different names*

### Comparing `twikit-1.4.3/twikit/twikit_async/http.py` & `twikit-1.4.4/twikit/twikit_async/http.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,15 +35,15 @@
             elif status_code == 403:
                 raise Forbidden(message)
             elif status_code == 404:
                 raise NotFound(message)
             elif status_code == 408:
                 raise RequestTimeout(message)
             elif status_code == 429:
-                raise TooManyRequests(message)
+                raise TooManyRequests(message, headers=response.headers)
             elif 500 <= status_code < 600:
                 raise ServerError(message)
             else:
                 raise TwitterException(message)
 
         return response
```

### Comparing `twikit-1.4.3/twikit/twikit_async/list.py` & `twikit-1.4.4/twikit/twikit_async/list.py`

 * *Files identical despite different names*

### Comparing `twikit-1.4.3/twikit/twikit_async/message.py` & `twikit-1.4.4/twikit/twikit_async/message.py`

 * *Files identical despite different names*

### Comparing `twikit-1.4.3/twikit/twikit_async/notification.py` & `twikit-1.4.4/twikit/twikit_async/notification.py`

 * *Files identical despite different names*

### Comparing `twikit-1.4.3/twikit/twikit_async/trend.py` & `twikit-1.4.4/twikit/twikit_async/trend.py`

 * *Files identical despite different names*

### Comparing `twikit-1.4.3/twikit/twikit_async/tweet.py` & `twikit-1.4.4/twikit/twikit_async/tweet.py`

 * *Files identical despite different names*

### Comparing `twikit-1.4.3/twikit/twikit_async/user.py` & `twikit-1.4.4/twikit/twikit_async/user.py`

 * *Files identical despite different names*

### Comparing `twikit-1.4.3/twikit/twikit_async/utils.py` & `twikit-1.4.4/twikit/twikit_async/utils.py`

 * *Files identical despite different names*

### Comparing `twikit-1.4.3/twikit/user.py` & `twikit-1.4.4/twikit/user.py`

 * *Files identical despite different names*

### Comparing `twikit-1.4.3/twikit/utils.py` & `twikit-1.4.4/twikit/utils.py`

 * *Files identical despite different names*

### Comparing `twikit-1.4.3/twikit.egg-info/PKG-INFO` & `twikit-1.4.4/twikit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twikit
-Version: 1.4.3
+Version: 1.4.4
 Summary: Twitter API wrapper for python with **no API key required**.
 Home-page: https://github.com/d60/twikit
 License: MIT
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `twikit-1.4.3/twikit.egg-info/SOURCES.txt` & `twikit-1.4.4/twikit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

