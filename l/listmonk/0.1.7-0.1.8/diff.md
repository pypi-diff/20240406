# Comparing `tmp/listmonk-0.1.7.tar.gz` & `tmp/listmonk-0.1.8.tar.gz`

## Comparing `listmonk-0.1.7.tar` & `listmonk-0.1.8.tar`

### file list

```diff
@@ -1,12 +1,15 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 listmonk-0.1.7/.DS_Store
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 listmonk-0.1.7/requirements.txt
--rw-r--r--   0        0        0     1287 2020-02-02 00:00:00.000000 listmonk-0.1.7/listmonk/__init__.py
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 listmonk-0.1.7/listmonk/urls.py
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 listmonk-0.1.7/listmonk/errors/__init__.py
--rw-r--r--   0        0        0    22036 2020-02-02 00:00:00.000000 listmonk-0.1.7/listmonk/impl/__init__.py
--rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 listmonk-0.1.7/listmonk/models/__init__.py
--rw-r--r--   0        0        0     3091 2020-02-02 00:00:00.000000 listmonk-0.1.7/.gitignore
--rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 listmonk-0.1.7/LICENSE
--rw-r--r--   0        0        0     4016 2020-02-02 00:00:00.000000 listmonk-0.1.7/README.md
--rw-r--r--   0        0        0     1343 2020-02-02 00:00:00.000000 listmonk-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     5011 2020-02-02 00:00:00.000000 listmonk-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 listmonk-0.1.8/.DS_Store
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 listmonk-0.1.8/requirements.txt
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 listmonk-0.1.8/listmonk/.DS_Store
+-rw-r--r--   0        0        0     1287 2020-02-02 00:00:00.000000 listmonk-0.1.8/listmonk/__init__.py
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 listmonk-0.1.8/listmonk/urls.py
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 listmonk-0.1.8/listmonk/errors/__init__.py
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 listmonk-0.1.8/listmonk/impl/.DS_Store
+-rw-r--r--   0        0        0    22030 2020-02-02 00:00:00.000000 listmonk-0.1.8/listmonk/impl/__init__.py
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 listmonk-0.1.8/listmonk/models/.DS_Store
+-rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 listmonk-0.1.8/listmonk/models/__init__.py
+-rw-r--r--   0        0        0     3091 2020-02-02 00:00:00.000000 listmonk-0.1.8/.gitignore
+-rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 listmonk-0.1.8/LICENSE
+-rw-r--r--   0        0        0     4016 2020-02-02 00:00:00.000000 listmonk-0.1.8/README.md
+-rw-r--r--   0        0        0     1343 2020-02-02 00:00:00.000000 listmonk-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     5011 2020-02-02 00:00:00.000000 listmonk-0.1.8/PKG-INFO
```

### Comparing `listmonk-0.1.7/.DS_Store` & `listmonk-0.1.8/listmonk/impl/.DS_Store`

 * *Files identical despite different names*

### Comparing `listmonk-0.1.7/listmonk/__init__.py` & `listmonk-0.1.8/listmonk/__init__.py`

 * *Files identical despite different names*

### Comparing `listmonk-0.1.7/listmonk/impl/__init__.py` & `listmonk-0.1.8/listmonk/impl/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from base64 import b64encode
 from typing import Optional, Tuple
 
 import httpx
 
 from listmonk import models, urls  # noqa: F401
 
-__version__ = '0.1.7'
+__version__ = '0.1.8'
 
 from listmonk.errors import ValidationError, OperationNotAllowedError, FileNotFoundError
 
 from listmonk.models import SubscriberStatuses
 
 # region global vars
 url_base: Optional[str] = None
@@ -197,15 +197,15 @@
 
     url = f'{url_base}{urls.subscribers}?page={page_num}&per_page={per_page}&order_by=updated_at&order=DESC'
 
     if list_id:
         url += f'&list_id={list_id}'
 
     if query_text:
-        url += f"&query={urllib.parse.urlencode({'query': query_text})}"
+        url += f"&{urllib.parse.urlencode({'query': query_text})}"
 
     resp = httpx.get(url, headers=core_headers, follow_redirects=True)
     resp.raise_for_status()
 
     # For paging:
     # data: {"total":55712,"per_page":10,"page":1, ...}
     raw_data = resp.json()
```

### Comparing `listmonk-0.1.7/listmonk/models/__init__.py` & `listmonk-0.1.8/listmonk/models/__init__.py`

 * *Files identical despite different names*

### Comparing `listmonk-0.1.7/.gitignore` & `listmonk-0.1.8/.gitignore`

 * *Files identical despite different names*

### Comparing `listmonk-0.1.7/LICENSE` & `listmonk-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `listmonk-0.1.7/README.md` & `listmonk-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `listmonk-0.1.7/pyproject.toml` & `listmonk-0.1.8/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     'Programming Language :: Python :: 3.11',
     'Programming Language :: Python :: 3.12',
 ]
 dependencies = [
     "httpx",
     "pydantic",
 ]
-version = "0.1.7"
+version = "0.1.8"
 
 
 [project.urls]
 Homepage = "https://github.com/mikeckennedy/listmonk"
 Tracker = "https://github.com/mikeckennedy/listmonk/issues"
 Source = "https://github.com/mikeckennedy/listmonk"
```

### Comparing `listmonk-0.1.7/PKG-INFO` & `listmonk-0.1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: listmonk
-Version: 0.1.7
+Version: 0.1.8
 Summary: Listmonk Email App API Client for Python
 Project-URL: Homepage, https://github.com/mikeckennedy/listmonk
 Project-URL: Tracker, https://github.com/mikeckennedy/listmonk/issues
 Project-URL: Source, https://github.com/mikeckennedy/listmonk
 Author-email: Michael Kennedy <michael@talkpython.fm>
 License-Expression: MIT
 License-File: LICENSE
```

