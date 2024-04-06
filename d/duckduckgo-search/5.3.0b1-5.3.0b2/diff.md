# Comparing `tmp/duckduckgo_search-5.3.0b1.tar.gz` & `tmp/duckduckgo_search-5.3.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "duckduckgo_search-5.3.0b1.tar", last modified: Wed Apr  3 23:37:51 2024, max compression
+gzip compressed data, was "duckduckgo_search-5.3.0b2.tar", last modified: Fri Apr  5 18:41:04 2024, max compression
```

## Comparing `duckduckgo_search-5.3.0b1.tar` & `duckduckgo_search-5.3.0b2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:37:51.195926 duckduckgo_search-5.3.0b1/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1063 2024-04-03 23:37:41.000000 duckduckgo_search-5.3.0b1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)    18186 2024-04-03 23:37:51.195926 duckduckgo_search-5.3.0b1/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (127)    16745 2024-04-03 23:37:41.000000 duckduckgo_search-5.3.0b1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:37:51.195926 duckduckgo_search-5.3.0b1/duckduckgo_search/
--rwxr-xr-x   0 runner    (1001) docker     (127)      797 2024-04-03 23:37:41.000000 duckduckgo_search-5.3.0b1/duckduckgo_search/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      140 2024-04-03 23:37:41.000000 duckduckgo_search-5.3.0b1/duckduckgo_search/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16612 2024-04-03 23:37:41.000000 duckduckgo_search-5.3.0b1/duckduckgo_search/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     3025 2024-04-03 23:37:41.000000 duckduckgo_search-5.3.0b1/duckduckgo_search/duckduckgo_search.py
--rw-r--r--   0 runner    (1001) docker     (127)    40880 2024-04-03 23:37:41.000000 duckduckgo_search-5.3.0b1/duckduckgo_search/duckduckgo_search_async.py
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-03 23:37:41.000000 duckduckgo_search-5.3.0b1/duckduckgo_search/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-03 23:37:41.000000 duckduckgo_search-5.3.0b1/duckduckgo_search/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    15875 2024-04-03 23:37:41.000000 duckduckgo_search-5.3.0b1/duckduckgo_search/utils.py
--rwxr-xr-x   0 runner    (1001) docker     (127)       24 2024-04-03 23:37:41.000000 duckduckgo_search-5.3.0b1/duckduckgo_search/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:37:51.195926 duckduckgo_search-5.3.0b1/duckduckgo_search.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    18186 2024-04-03 23:37:51.000000 duckduckgo_search-5.3.0b1/duckduckgo_search.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-03 23:37:51.000000 duckduckgo_search-5.3.0b1/duckduckgo_search.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 23:37:51.000000 duckduckgo_search-5.3.0b1/duckduckgo_search.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-03 23:37:51.000000 duckduckgo_search-5.3.0b1/duckduckgo_search.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-03 23:37:51.000000 duckduckgo_search-5.3.0b1/duckduckgo_search.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-03 23:37:51.000000 duckduckgo_search-5.3.0b1/duckduckgo_search.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-04-03 23:37:41.000000 duckduckgo_search-5.3.0b1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 23:37:51.195926 duckduckgo_search-5.3.0b1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:37:51.195926 duckduckgo_search-5.3.0b1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3675 2024-04-03 23:37:41.000000 duckduckgo_search-5.3.0b1/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1860 2024-04-03 23:37:41.000000 duckduckgo_search-5.3.0b1/tests/test_duckduckgo_search.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:41:04.777678 duckduckgo_search-5.3.0b2/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1063 2024-04-05 18:40:45.000000 duckduckgo_search-5.3.0b2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)    18228 2024-04-05 18:41:04.777678 duckduckgo_search-5.3.0b2/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)    16745 2024-04-05 18:40:45.000000 duckduckgo_search-5.3.0b2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:41:04.773678 duckduckgo_search-5.3.0b2/duckduckgo_search/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      797 2024-04-05 18:40:45.000000 duckduckgo_search-5.3.0b2/duckduckgo_search/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      140 2024-04-05 18:40:45.000000 duckduckgo_search-5.3.0b2/duckduckgo_search/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16612 2024-04-05 18:40:45.000000 duckduckgo_search-5.3.0b2/duckduckgo_search/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3025 2024-04-05 18:40:45.000000 duckduckgo_search-5.3.0b2/duckduckgo_search/duckduckgo_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40880 2024-04-05 18:40:45.000000 duckduckgo_search-5.3.0b2/duckduckgo_search/duckduckgo_search_async.py
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-05 18:40:45.000000 duckduckgo_search-5.3.0b2/duckduckgo_search/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-05 18:40:45.000000 duckduckgo_search-5.3.0b2/duckduckgo_search/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    16130 2024-04-05 18:40:45.000000 duckduckgo_search-5.3.0b2/duckduckgo_search/utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)       24 2024-04-05 18:40:45.000000 duckduckgo_search-5.3.0b2/duckduckgo_search/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:41:04.777678 duckduckgo_search-5.3.0b2/duckduckgo_search.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    18228 2024-04-05 18:41:04.000000 duckduckgo_search-5.3.0b2/duckduckgo_search.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-05 18:41:04.000000 duckduckgo_search-5.3.0b2/duckduckgo_search.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 18:41:04.000000 duckduckgo_search-5.3.0b2/duckduckgo_search.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-05 18:41:04.000000 duckduckgo_search-5.3.0b2/duckduckgo_search.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-05 18:41:04.000000 duckduckgo_search-5.3.0b2/duckduckgo_search.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-05 18:41:04.000000 duckduckgo_search-5.3.0b2/duckduckgo_search.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-04-05 18:40:45.000000 duckduckgo_search-5.3.0b2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 18:41:04.777678 duckduckgo_search-5.3.0b2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:41:04.777678 duckduckgo_search-5.3.0b2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3675 2024-04-05 18:40:45.000000 duckduckgo_search-5.3.0b2/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1860 2024-04-05 18:40:45.000000 duckduckgo_search-5.3.0b2/tests/test_duckduckgo_search.py
```

### Comparing `duckduckgo_search-5.3.0b1/LICENSE.md` & `duckduckgo_search-5.3.0b2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-5.3.0b1/PKG-INFO` & `duckduckgo_search-5.3.0b2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duckduckgo_search
-Version: 5.3.0b1
+Version: 5.3.0b2
 Summary: Search for words, documents, images, news, maps and text translation using the DuckDuckGo.com search engine.
 Author: deedy5
 License: MIT License
 Project-URL: Homepage, https://github.com/deedy5/duckduckgo_search
 Keywords: python,duckduckgo
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
@@ -20,17 +20,18 @@
 Classifier: Topic :: Internet :: WWW/HTTP :: Indexing/Search
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: click>=8.1.7
 Requires-Dist: httpx[brotli,http2,socks]>=0.27.0
-Requires-Dist: orjson>=3.10.0
 Provides-Extra: lxml
 Requires-Dist: lxml>=5.1.1; extra == "lxml"
+Provides-Extra: orjson
+Requires-Dist: orjson>=3.10.0; extra == "orjson"
 Provides-Extra: dev
 Requires-Dist: mypy>=1.9.0; extra == "dev"
 Requires-Dist: pytest>=8.1.1; extra == "dev"
 Requires-Dist: ruff>=0.3.5; extra == "dev"
 
 ![Python >= 3.8](https://img.shields.io/badge/python->=3.8-red.svg) [![](https://badgen.net/github/release/deedy5/duckduckgo_search)](https://github.com/deedy5/duckduckgo_search/releases) [![](https://badge.fury.io/py/duckduckgo-search.svg)](https://pypi.org/project/duckduckgo-search) [![Downloads](https://static.pepy.tech/badge/duckduckgo-search)](https://pepy.tech/project/duckduckgo-search) [![Downloads](https://static.pepy.tech/badge/duckduckgo-search/week)](https://pepy.tech/project/duckduckgo-search)
 # Duckduckgo_search<a name="TOP"></a>
```

### Comparing `duckduckgo_search-5.3.0b1/README.md` & `duckduckgo_search-5.3.0b2/README.md`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-5.3.0b1/duckduckgo_search/__init__.py` & `duckduckgo_search-5.3.0b2/duckduckgo_search/__init__.py`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-5.3.0b1/duckduckgo_search/cli.py` & `duckduckgo_search-5.3.0b2/duckduckgo_search/cli.py`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-5.3.0b1/duckduckgo_search/duckduckgo_search.py` & `duckduckgo_search-5.3.0b2/duckduckgo_search/duckduckgo_search.py`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-5.3.0b1/duckduckgo_search/duckduckgo_search_async.py` & `duckduckgo_search-5.3.0b2/duckduckgo_search/duckduckgo_search_async.py`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-5.3.0b1/duckduckgo_search/utils.py` & `duckduckgo_search-5.3.0b2/duckduckgo_search/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,24 @@
 from html import unescape
 from math import atan2, cos, radians, sin, sqrt
 from random import SystemRandom, choices
 from typing import Any, Dict, List, Union
 from urllib.parse import unquote
 
 import certifi
-import orjson
+
+try:
+    import orjson
+
+    ORJSON_AVAILABLE = True
+except ImportError:
+    import json
+
+    ORJSON_AVAILABLE = False
+
 
 from .exceptions import DuckDuckGoSearchException
 
 CRYPTORAND = SystemRandom()
 REGEX_STRIP_TAGS = re.compile("<.*?>")
 SSL_CONTEXT = ssl.create_default_context(cafile=certifi.where())
 # Include all cipher suites that Cloudflare supports today. https://developers.cloudflare.com/ssl/reference/cipher-suites/recommendations/
@@ -280,29 +289,29 @@
 def _get_headers() -> Dict[str, str]:
     """Get random headers using probability."""
     return choices(HEADERS, weights=HEADERS_PROB)[0]
 
 
 def _get_ssl_context() -> ssl.SSLContext:
     """Get SSL context with shuffled ciphers."""
-    CRYPTORAND.shuffle(DEFAULT_CIPHERS[:6])
-    SSL_CONTEXT.set_ciphers(":".join(DEFAULT_CIPHERS))
+    shuffled_ciphers = CRYPTORAND.sample(DEFAULT_CIPHERS[6:], len(DEFAULT_CIPHERS) - 6)
+    SSL_CONTEXT.set_ciphers(":".join(DEFAULT_CIPHERS[:6] + shuffled_ciphers))
     return SSL_CONTEXT
 
 
 def json_dumps(obj: Any) -> str:
     try:
-        return orjson.dumps(obj).decode("utf-8")
+        return orjson.dumps(obj).decode("utf-8") if ORJSON_AVAILABLE else json.dumps(obj)
     except Exception as ex:
         raise DuckDuckGoSearchException(f"{type(ex).__name__}: {ex}") from ex
 
 
 def json_loads(obj: Union[str, bytes]) -> Any:
     try:
-        return orjson.loads(obj)
+        return orjson.loads(obj) if ORJSON_AVAILABLE else json.loads(obj)
     except Exception as ex:
         raise DuckDuckGoSearchException(f"{type(ex).__name__}: {ex}") from ex
 
 
 def _extract_vqd(html_bytes: bytes, keywords: str) -> str:
     """Extract vqd from html bytes."""
     for c1, c1_len, c2 in (
```

### Comparing `duckduckgo_search-5.3.0b1/duckduckgo_search.egg-info/PKG-INFO` & `duckduckgo_search-5.3.0b2/duckduckgo_search.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duckduckgo_search
-Version: 5.3.0b1
+Version: 5.3.0b2
 Summary: Search for words, documents, images, news, maps and text translation using the DuckDuckGo.com search engine.
 Author: deedy5
 License: MIT License
 Project-URL: Homepage, https://github.com/deedy5/duckduckgo_search
 Keywords: python,duckduckgo
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
@@ -20,17 +20,18 @@
 Classifier: Topic :: Internet :: WWW/HTTP :: Indexing/Search
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: click>=8.1.7
 Requires-Dist: httpx[brotli,http2,socks]>=0.27.0
-Requires-Dist: orjson>=3.10.0
 Provides-Extra: lxml
 Requires-Dist: lxml>=5.1.1; extra == "lxml"
+Provides-Extra: orjson
+Requires-Dist: orjson>=3.10.0; extra == "orjson"
 Provides-Extra: dev
 Requires-Dist: mypy>=1.9.0; extra == "dev"
 Requires-Dist: pytest>=8.1.1; extra == "dev"
 Requires-Dist: ruff>=0.3.5; extra == "dev"
 
 ![Python >= 3.8](https://img.shields.io/badge/python->=3.8-red.svg) [![](https://badgen.net/github/release/deedy5/duckduckgo_search)](https://github.com/deedy5/duckduckgo_search/releases) [![](https://badge.fury.io/py/duckduckgo-search.svg)](https://pypi.org/project/duckduckgo-search) [![Downloads](https://static.pepy.tech/badge/duckduckgo-search)](https://pepy.tech/project/duckduckgo-search) [![Downloads](https://static.pepy.tech/badge/duckduckgo-search/week)](https://pepy.tech/project/duckduckgo-search)
 # Duckduckgo_search<a name="TOP"></a>
```

### Comparing `duckduckgo_search-5.3.0b1/duckduckgo_search.egg-info/SOURCES.txt` & `duckduckgo_search-5.3.0b2/duckduckgo_search.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-5.3.0b1/pyproject.toml` & `duckduckgo_search-5.3.0b2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -26,15 +26,14 @@
     "Programming Language :: Python :: Implementation :: CPython",
     "Topic :: Internet :: WWW/HTTP :: Indexing/Search",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 dependencies = [
     "click>=8.1.7",  
     "httpx[brotli, http2, socks]>=0.27.0",
-    "orjson>=3.10.0",
 ]
 dynamic = ["version"]
 
 [project.urls]  # Optional
 "Homepage" = "https://github.com/deedy5/duckduckgo_search"
 
 [project.scripts]
@@ -43,14 +42,17 @@
 [tool.setuptools.dynamic]
 version = {attr = "duckduckgo_search.version.__version__"}
 
 [project.optional-dependencies]
 lxml = [
     "lxml>=5.1.1",
 ]
+orjson = [
+    "orjson>=3.10.0",
+]
 dev = [
     "mypy>=1.9.0",
     "pytest>=8.1.1",
     "ruff>=0.3.5",
 ]
 
 [tool.ruff]
```

### Comparing `duckduckgo_search-5.3.0b1/tests/test_cli.py` & `duckduckgo_search-5.3.0b2/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-5.3.0b1/tests/test_duckduckgo_search.py` & `duckduckgo_search-5.3.0b2/tests/test_duckduckgo_search.py`

 * *Files identical despite different names*

