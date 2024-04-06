# Comparing `tmp/asyncpow-0.2.3.tar.gz` & `tmp/asyncpow-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asyncpow-0.2.3.tar", max compression
+gzip compressed data, was "asyncpow-0.2.4.tar", max compression
```

## Comparing `asyncpow-0.2.3.tar` & `asyncpow-0.2.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     6694 2024-04-04 21:28:10.592738 asyncpow-0.2.3/README.md
--rw-r--r--   0        0        0     1187 2024-04-04 21:28:10.592738 asyncpow-0.2.3/asyncpow/__init__.py
--rw-r--r--   0        0        0     4916 2024-04-04 21:28:10.592738 asyncpow-0.2.3/asyncpow/apis/media.py
--rw-r--r--   0        0        0     2768 2024-04-04 21:28:10.592738 asyncpow-0.2.3/asyncpow/apis/movie.py
--rw-r--r--   0        0        0     4412 2024-04-04 21:28:10.592738 asyncpow-0.2.3/asyncpow/apis/search.py
--rw-r--r--   0        0        0     2977 2024-04-04 21:28:10.592738 asyncpow-0.2.3/asyncpow/apis/status.py
--rw-r--r--   0        0        0     2825 2024-04-04 21:28:10.592738 asyncpow-0.2.3/asyncpow/apis/tv.py
--rw-r--r--   0        0        0     1148 2024-04-04 21:28:10.592738 asyncpow-0.2.3/asyncpow/const.py
--rw-r--r--   0        0        0     1664 2024-04-04 21:28:10.592738 asyncpow-0.2.3/asyncpow/exceptions.py
--rw-r--r--   0        0        0     3895 2024-04-04 21:28:10.592738 asyncpow-0.2.3/asyncpow/models/common.py
--rw-r--r--   0        0        0     2339 2024-04-04 21:28:10.592738 asyncpow-0.2.3/asyncpow/models/media.py
--rw-r--r--   0        0        0     4032 2024-04-04 21:28:10.592738 asyncpow-0.2.3/asyncpow/models/movie.py
--rw-r--r--   0        0        0     2812 2024-04-04 21:28:10.592738 asyncpow-0.2.3/asyncpow/models/search.py
--rw-r--r--   0        0        0     1517 2024-04-04 21:28:10.592738 asyncpow-0.2.3/asyncpow/models/status.py
--rw-r--r--   0        0        0     3120 2024-04-04 21:28:10.592738 asyncpow-0.2.3/asyncpow/models/tv.py
--rw-r--r--   0        0        0     4264 2024-04-04 21:28:10.592738 asyncpow-0.2.3/asyncpow/overseerr.py
--rw-r--r--   0        0        0        0 2024-04-04 21:28:10.592738 asyncpow-0.2.3/asyncpow/py.typed
--rw-r--r--   0        0        0     4067 2024-04-04 21:28:10.592738 asyncpow-0.2.3/asyncpow/utils/http.py
--rw-r--r--   0        0        0     2919 2024-04-04 21:28:54.936685 asyncpow-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     7638 1970-01-01 00:00:00.000000 asyncpow-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     6694 2024-04-06 19:58:29.227539 asyncpow-0.2.4/README.md
+-rw-r--r--   0        0        0     1187 2024-04-06 19:58:29.227539 asyncpow-0.2.4/asyncpow/__init__.py
+-rw-r--r--   0        0        0     4916 2024-04-06 19:58:29.227539 asyncpow-0.2.4/asyncpow/apis/media.py
+-rw-r--r--   0        0        0     2768 2024-04-06 19:58:29.227539 asyncpow-0.2.4/asyncpow/apis/movie.py
+-rw-r--r--   0        0        0     4412 2024-04-06 19:58:29.227539 asyncpow-0.2.4/asyncpow/apis/search.py
+-rw-r--r--   0        0        0     2977 2024-04-06 19:58:29.227539 asyncpow-0.2.4/asyncpow/apis/status.py
+-rw-r--r--   0        0        0     2825 2024-04-06 19:58:29.227539 asyncpow-0.2.4/asyncpow/apis/tv.py
+-rw-r--r--   0        0        0     1148 2024-04-06 19:58:29.227539 asyncpow-0.2.4/asyncpow/const.py
+-rw-r--r--   0        0        0     1664 2024-04-06 19:58:29.227539 asyncpow-0.2.4/asyncpow/exceptions.py
+-rw-r--r--   0        0        0     3895 2024-04-06 19:58:29.227539 asyncpow-0.2.4/asyncpow/models/common.py
+-rw-r--r--   0        0        0     2339 2024-04-06 19:58:29.227539 asyncpow-0.2.4/asyncpow/models/media.py
+-rw-r--r--   0        0        0     4032 2024-04-06 19:58:29.227539 asyncpow-0.2.4/asyncpow/models/movie.py
+-rw-r--r--   0        0        0     2812 2024-04-06 19:58:29.227539 asyncpow-0.2.4/asyncpow/models/search.py
+-rw-r--r--   0        0        0     1517 2024-04-06 19:58:29.227539 asyncpow-0.2.4/asyncpow/models/status.py
+-rw-r--r--   0        0        0     3136 2024-04-06 19:58:29.227539 asyncpow-0.2.4/asyncpow/models/tv.py
+-rw-r--r--   0        0        0     4264 2024-04-06 19:58:29.227539 asyncpow-0.2.4/asyncpow/overseerr.py
+-rw-r--r--   0        0        0        0 2024-04-06 19:58:29.227539 asyncpow-0.2.4/asyncpow/py.typed
+-rw-r--r--   0        0        0     4067 2024-04-06 19:58:29.227539 asyncpow-0.2.4/asyncpow/utils/http.py
+-rw-r--r--   0        0        0     2919 2024-04-06 19:59:15.423982 asyncpow-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     7638 1970-01-01 00:00:00.000000 asyncpow-0.2.4/PKG-INFO
```

### Comparing `asyncpow-0.2.3/README.md` & `asyncpow-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `asyncpow-0.2.3/asyncpow/__init__.py` & `asyncpow-0.2.4/asyncpow/__init__.py`

 * *Files identical despite different names*

### Comparing `asyncpow-0.2.3/asyncpow/apis/media.py` & `asyncpow-0.2.4/asyncpow/apis/media.py`

 * *Files identical despite different names*

### Comparing `asyncpow-0.2.3/asyncpow/apis/movie.py` & `asyncpow-0.2.4/asyncpow/apis/movie.py`

 * *Files identical despite different names*

### Comparing `asyncpow-0.2.3/asyncpow/apis/search.py` & `asyncpow-0.2.4/asyncpow/apis/search.py`

 * *Files identical despite different names*

### Comparing `asyncpow-0.2.3/asyncpow/apis/status.py` & `asyncpow-0.2.4/asyncpow/apis/status.py`

 * *Files identical despite different names*

### Comparing `asyncpow-0.2.3/asyncpow/apis/tv.py` & `asyncpow-0.2.4/asyncpow/apis/tv.py`

 * *Files identical despite different names*

### Comparing `asyncpow-0.2.3/asyncpow/const.py` & `asyncpow-0.2.4/asyncpow/const.py`

 * *Files identical despite different names*

### Comparing `asyncpow-0.2.3/asyncpow/exceptions.py` & `asyncpow-0.2.4/asyncpow/exceptions.py`

 * *Files identical despite different names*

### Comparing `asyncpow-0.2.3/asyncpow/models/common.py` & `asyncpow-0.2.4/asyncpow/models/common.py`

 * *Files identical despite different names*

### Comparing `asyncpow-0.2.3/asyncpow/models/media.py` & `asyncpow-0.2.4/asyncpow/models/media.py`

 * *Files identical despite different names*

### Comparing `asyncpow-0.2.3/asyncpow/models/movie.py` & `asyncpow-0.2.4/asyncpow/models/movie.py`

 * *Files identical despite different names*

### Comparing `asyncpow-0.2.3/asyncpow/models/search.py` & `asyncpow-0.2.4/asyncpow/models/search.py`

 * *Files identical despite different names*

### Comparing `asyncpow-0.2.3/asyncpow/models/status.py` & `asyncpow-0.2.4/asyncpow/models/status.py`

 * *Files identical despite different names*

### Comparing `asyncpow-0.2.3/asyncpow/models/tv.py` & `asyncpow-0.2.4/asyncpow/models/tv.py`

 * *Files 5% similar despite different names*

```diff
@@ -43,27 +43,27 @@
     airDate: str | None
     episodeNumber: int
     overview: str
     productionCode: str
     seasonNumber: int
     showId: int
     stillPath: str | None
-    voteAverage: int
+    voteAverage: float
     voteCount: int | None = None
 
 
 class SeasonModel(BaseModel):
     """Model for TV Seasons"""
 
     id: int
     airDate: str | None = None
     episodeCount: int
     name: str
     overview: str
-    posterPath: str
+    posterPath: str | None = None
     seasonNumber: int
 
 
 class CreatedByModel(BaseModel):
     """Model for Created by"""
 
     id: int
```

### Comparing `asyncpow-0.2.3/asyncpow/overseerr.py` & `asyncpow-0.2.4/asyncpow/overseerr.py`

 * *Files identical despite different names*

### Comparing `asyncpow-0.2.3/asyncpow/utils/http.py` & `asyncpow-0.2.4/asyncpow/utils/http.py`

 * *Files identical despite different names*

### Comparing `asyncpow-0.2.3/pyproject.toml` & `asyncpow-0.2.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "asyncpow"
-version = "0.2.3"
+version = "0.2.4"
 description = "Asynchronous Python Overseerr Wrapper"
 authors = ["Steven Marks - TotalDebug"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/totaldebug/asyncpow"
 repository = "https://github.com/totaldebug/asyncpow"
 classifiers = [
```

### Comparing `asyncpow-0.2.3/PKG-INFO` & `asyncpow-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asyncpow
-Version: 0.2.3
+Version: 0.2.4
 Summary: Asynchronous Python Overseerr Wrapper
 Home-page: https://github.com/totaldebug/asyncpow
 License: MIT
 Keywords: wled,api,async,client
 Author: Steven Marks - TotalDebug
 Maintainer: Steven Marks - TotalDebug
 Requires-Python: >=3.12,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: asyncpow Version: 0.2.3 Summary: Asynchronous
+Metadata-Version: 2.1 Name: asyncpow Version: 0.2.4 Summary: Asynchronous
 Python Overseerr Wrapper Home-page: https://github.com/totaldebug/asyncpow
 License: MIT Keywords: wled,api,async,client Author: Steven Marks - TotalDebug
 Maintainer: Steven Marks - TotalDebug Requires-Python: >=3.12,<4.0 Classifier:
 Development Status :: 4 - Beta Classifier: Framework :: AsyncIO Classifier:
 Intended Audience :: Developers Classifier: License :: OSI Approved :: MIT
 License Classifier: Natural Language :: English Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.12
```

