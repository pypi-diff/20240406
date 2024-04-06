# Comparing `tmp/blacksmith-2.7.1.tar.gz` & `tmp/blacksmith-2.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blacksmith-2.7.1.tar", max compression
+gzip compressed data, was "blacksmith-2.7.2.tar", max compression
```

## Comparing `blacksmith-2.7.1.tar` & `blacksmith-2.7.2.tar`

### file list

```diff
@@ -1,65 +1,65 @@
--rw-r--r--   0        0        0     1528 2024-01-21 22:29:45.080413 blacksmith-2.7.1/LICENSE
--rw-r--r--   0        0        0     4069 2024-01-21 22:29:45.080413 blacksmith-2.7.1/README.rst
--rw-r--r--   0        0        0     2907 2024-02-05 17:58:24.619573 blacksmith-2.7.1/pyproject.toml
--rw-r--r--   0        0        0     4281 2024-01-21 22:29:45.093746 blacksmith-2.7.1/src/blacksmith/__init__.py
--rw-r--r--   0        0        0        0 2024-01-21 22:29:45.093746 blacksmith-2.7.1/src/blacksmith/adapters/__init__.py
--rw-r--r--   0        0        0        0 2021-10-23 20:54:22.320117 blacksmith-2.7.1/src/blacksmith/domain/__init__.py
--rw-r--r--   0        0        0      813 2024-01-21 22:29:45.093746 blacksmith-2.7.1/src/blacksmith/domain/error.py
--rw-r--r--   0        0        0     4015 2024-01-21 22:29:45.093746 blacksmith-2.7.1/src/blacksmith/domain/exceptions.py
--rw-r--r--   0        0        0     1083 2024-01-21 22:29:45.097079 blacksmith-2.7.1/src/blacksmith/domain/model/__init__.py
--rw-r--r--   0        0        0     4285 2024-01-21 22:29:45.097079 blacksmith-2.7.1/src/blacksmith/domain/model/http.py
--rw-r--r--   0        0        0        0 2024-01-21 22:29:45.097079 blacksmith-2.7.1/src/blacksmith/domain/model/middleware/__init__.py
--rw-r--r--   0        0        0     1201 2024-01-21 22:29:45.097079 blacksmith-2.7.1/src/blacksmith/domain/model/middleware/circuit_breaker.py
--rw-r--r--   0        0        0     4365 2024-01-21 22:29:45.097079 blacksmith-2.7.1/src/blacksmith/domain/model/middleware/http_cache.py
--rw-r--r--   0        0        0     2993 2024-01-21 22:29:45.097079 blacksmith-2.7.1/src/blacksmith/domain/model/middleware/prometheus.py
--rw-r--r--   0        0        0     1174 2024-01-21 22:29:45.097079 blacksmith-2.7.1/src/blacksmith/domain/model/middleware/zipkin.py
--rw-r--r--   0        0        0    12652 2024-01-21 22:29:45.097079 blacksmith-2.7.1/src/blacksmith/domain/model/params.py
--rw-r--r--   0        0        0     5156 2024-01-21 22:29:45.097079 blacksmith-2.7.1/src/blacksmith/domain/registry.py
--rw-r--r--   0        0        0      983 2024-01-21 22:29:45.097079 blacksmith-2.7.1/src/blacksmith/domain/scanner.py
--rw-r--r--   0        0        0      885 2024-01-21 22:29:45.097079 blacksmith-2.7.1/src/blacksmith/domain/typing.py
--rw-r--r--   0        0        0        0 2024-01-21 22:29:45.097079 blacksmith-2.7.1/src/blacksmith/middleware/__init__.py
--rw-r--r--   0        0        0      716 2024-01-21 22:29:45.097079 blacksmith-2.7.1/src/blacksmith/middleware/_async/__init__.py
--rw-r--r--   0        0        0      802 2024-01-21 22:29:45.097079 blacksmith-2.7.1/src/blacksmith/middleware/_async/auth.py
--rw-r--r--   0        0        0     1472 2024-01-21 22:29:45.097079 blacksmith-2.7.1/src/blacksmith/middleware/_async/base.py
--rw-r--r--   0        0        0     2330 2024-01-21 22:29:45.097079 blacksmith-2.7.1/src/blacksmith/middleware/_async/circuit_breaker.py
--rw-r--r--   0        0        0     5933 2024-01-21 22:29:45.097079 blacksmith-2.7.1/src/blacksmith/middleware/_async/http_cache.py
--rw-r--r--   0        0        0     2436 2024-01-21 22:29:45.097079 blacksmith-2.7.1/src/blacksmith/middleware/_async/prometheus.py
--rw-r--r--   0        0        0     2869 2024-01-21 22:29:45.097079 blacksmith-2.7.1/src/blacksmith/middleware/_async/zipkin.py
--rw-r--r--   0        0        0      696 2024-02-05 17:58:12.236055 blacksmith-2.7.1/src/blacksmith/middleware/_sync/__init__.py
--rw-r--r--   0        0        0      797 2024-02-05 17:58:12.236055 blacksmith-2.7.1/src/blacksmith/middleware/_sync/auth.py
--rw-r--r--   0        0        0     1434 2024-02-05 17:58:12.236055 blacksmith-2.7.1/src/blacksmith/middleware/_sync/base.py
--rw-r--r--   0        0        0     2284 2024-02-05 17:58:12.236055 blacksmith-2.7.1/src/blacksmith/middleware/_sync/circuit_breaker.py
--rw-r--r--   0        0        0     5827 2024-02-05 17:58:12.239389 blacksmith-2.7.1/src/blacksmith/middleware/_sync/http_cache.py
--rw-r--r--   0        0        0     2418 2024-02-05 17:58:12.239389 blacksmith-2.7.1/src/blacksmith/middleware/_sync/prometheus.py
--rw-r--r--   0        0        0     2851 2024-02-05 17:58:12.242722 blacksmith-2.7.1/src/blacksmith/middleware/_sync/zipkin.py
--rw-r--r--   0        0        0        0 2024-01-21 22:29:45.097079 blacksmith-2.7.1/src/blacksmith/py.typed
--rw-r--r--   0        0        0       24 2021-10-24 11:21:34.426587 blacksmith-2.7.1/src/blacksmith/sd/__init__.py
--rw-r--r--   0        0        0      334 2024-01-21 22:29:45.097079 blacksmith-2.7.1/src/blacksmith/sd/_async/__init__.py
--rw-r--r--   0        0        0        0 2024-01-21 22:29:45.097079 blacksmith-2.7.1/src/blacksmith/sd/_async/adapters/__init__.py
--rw-r--r--   0        0        0     5666 2024-01-21 22:29:45.097079 blacksmith-2.7.1/src/blacksmith/sd/_async/adapters/consul.py
--rw-r--r--   0        0        0     1693 2024-01-21 22:29:45.097079 blacksmith-2.7.1/src/blacksmith/sd/_async/adapters/router.py
--rw-r--r--   0        0        0     1010 2024-01-21 22:29:45.097079 blacksmith-2.7.1/src/blacksmith/sd/_async/adapters/static.py
--rw-r--r--   0        0        0      317 2024-01-21 22:29:45.097079 blacksmith-2.7.1/src/blacksmith/sd/_async/base.py
--rw-r--r--   0        0        0      326 2024-02-05 17:58:12.242722 blacksmith-2.7.1/src/blacksmith/sd/_sync/__init__.py
--rw-r--r--   0        0        0        0 2024-02-05 17:58:12.242722 blacksmith-2.7.1/src/blacksmith/sd/_sync/adapters/__init__.py
--rw-r--r--   0        0        0     5620 2024-02-05 17:58:12.246055 blacksmith-2.7.1/src/blacksmith/sd/_sync/adapters/consul.py
--rw-r--r--   0        0        0     1684 2024-02-05 17:58:12.246055 blacksmith-2.7.1/src/blacksmith/sd/_sync/adapters/router.py
--rw-r--r--   0        0        0     1001 2024-02-05 17:58:12.246055 blacksmith-2.7.1/src/blacksmith/sd/_sync/adapters/static.py
--rw-r--r--   0        0        0      310 2024-02-05 17:58:12.242722 blacksmith-2.7.1/src/blacksmith/sd/_sync/base.py
--rw-r--r--   0        0        0        0 2021-10-23 21:02:59.310144 blacksmith-2.7.1/src/blacksmith/service/__init__.py
--rw-r--r--   0        0        0        0 2024-01-21 22:29:45.097079 blacksmith-2.7.1/src/blacksmith/service/_async/__init__.py
--rw-r--r--   0        0        0        0 2024-01-21 22:29:45.097079 blacksmith-2.7.1/src/blacksmith/service/_async/adapters/__init__.py
--rw-r--r--   0        0        0     2146 2024-01-21 22:29:45.097079 blacksmith-2.7.1/src/blacksmith/service/_async/adapters/httpx.py
--rw-r--r--   0        0        0      420 2024-01-21 22:29:45.097079 blacksmith-2.7.1/src/blacksmith/service/_async/base.py
--rw-r--r--   0        0        0     5903 2024-01-21 22:29:45.097079 blacksmith-2.7.1/src/blacksmith/service/_async/client.py
--rw-r--r--   0        0        0    14250 2024-01-21 22:29:45.097079 blacksmith-2.7.1/src/blacksmith/service/_async/route_proxy.py
--rw-r--r--   0        0        0        0 2024-02-05 17:58:12.246055 blacksmith-2.7.1/src/blacksmith/service/_sync/__init__.py
--rw-r--r--   0        0        0        0 2024-02-05 17:58:12.256055 blacksmith-2.7.1/src/blacksmith/service/_sync/adapters/__init__.py
--rw-r--r--   0        0        0     2123 2024-02-05 17:58:12.256055 blacksmith-2.7.1/src/blacksmith/service/_sync/adapters/httpx.py
--rw-r--r--   0        0        0      417 2024-02-05 17:58:12.246055 blacksmith-2.7.1/src/blacksmith/service/_sync/base.py
--rw-r--r--   0        0        0     5837 2024-02-05 17:58:15.516104 blacksmith-2.7.1/src/blacksmith/service/_sync/client.py
--rw-r--r--   0        0        0    13869 2024-02-05 17:58:15.649439 blacksmith-2.7.1/src/blacksmith/service/_sync/route_proxy.py
--rw-r--r--   0        0        0     8388 2024-02-05 17:58:05.369286 blacksmith-2.7.1/src/blacksmith/service/http_body_serializer.py
--rw-r--r--   0        0        0      121 2024-01-21 22:29:45.097079 blacksmith-2.7.1/src/blacksmith/service/ports.py
--rw-r--r--   0        0        0      450 2024-01-21 22:29:45.097079 blacksmith-2.7.1/src/blacksmith/typing.py
--rw-r--r--   0        0        0     5577 1970-01-01 00:00:00.000000 blacksmith-2.7.1/PKG-INFO
+-rw-r--r--   0        0        0     1528 2024-01-21 22:29:45.080413 blacksmith-2.7.2/LICENSE
+-rw-r--r--   0        0        0     4069 2024-01-21 22:29:45.080413 blacksmith-2.7.2/README.rst
+-rw-r--r--   0        0        0     2907 2024-04-06 17:34:53.081347 blacksmith-2.7.2/pyproject.toml
+-rw-r--r--   0        0        0     4281 2024-01-21 22:29:45.093746 blacksmith-2.7.2/src/blacksmith/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-21 22:29:45.093746 blacksmith-2.7.2/src/blacksmith/adapters/__init__.py
+-rw-r--r--   0        0        0        0 2021-10-23 20:54:22.320117 blacksmith-2.7.2/src/blacksmith/domain/__init__.py
+-rw-r--r--   0        0        0      813 2024-01-21 22:29:45.093746 blacksmith-2.7.2/src/blacksmith/domain/error.py
+-rw-r--r--   0        0        0     4015 2024-01-21 22:29:45.093746 blacksmith-2.7.2/src/blacksmith/domain/exceptions.py
+-rw-r--r--   0        0        0     1083 2024-01-21 22:29:45.097079 blacksmith-2.7.2/src/blacksmith/domain/model/__init__.py
+-rw-r--r--   0        0        0     4285 2024-01-21 22:29:45.097079 blacksmith-2.7.2/src/blacksmith/domain/model/http.py
+-rw-r--r--   0        0        0        0 2024-01-21 22:29:45.097079 blacksmith-2.7.2/src/blacksmith/domain/model/middleware/__init__.py
+-rw-r--r--   0        0        0     1201 2024-01-21 22:29:45.097079 blacksmith-2.7.2/src/blacksmith/domain/model/middleware/circuit_breaker.py
+-rw-r--r--   0        0        0     4365 2024-01-21 22:29:45.097079 blacksmith-2.7.2/src/blacksmith/domain/model/middleware/http_cache.py
+-rw-r--r--   0        0        0     2993 2024-01-21 22:29:45.097079 blacksmith-2.7.2/src/blacksmith/domain/model/middleware/prometheus.py
+-rw-r--r--   0        0        0     1174 2024-01-21 22:29:45.097079 blacksmith-2.7.2/src/blacksmith/domain/model/middleware/zipkin.py
+-rw-r--r--   0        0        0    12672 2024-04-06 17:29:44.326493 blacksmith-2.7.2/src/blacksmith/domain/model/params.py
+-rw-r--r--   0        0        0     5156 2024-01-21 22:29:45.097079 blacksmith-2.7.2/src/blacksmith/domain/registry.py
+-rw-r--r--   0        0        0      983 2024-01-21 22:29:45.097079 blacksmith-2.7.2/src/blacksmith/domain/scanner.py
+-rw-r--r--   0        0        0      885 2024-01-21 22:29:45.097079 blacksmith-2.7.2/src/blacksmith/domain/typing.py
+-rw-r--r--   0        0        0        0 2024-01-21 22:29:45.097079 blacksmith-2.7.2/src/blacksmith/middleware/__init__.py
+-rw-r--r--   0        0        0      716 2024-01-21 22:29:45.097079 blacksmith-2.7.2/src/blacksmith/middleware/_async/__init__.py
+-rw-r--r--   0        0        0      802 2024-01-21 22:29:45.097079 blacksmith-2.7.2/src/blacksmith/middleware/_async/auth.py
+-rw-r--r--   0        0        0     1472 2024-01-21 22:29:45.097079 blacksmith-2.7.2/src/blacksmith/middleware/_async/base.py
+-rw-r--r--   0        0        0     2330 2024-01-21 22:29:45.097079 blacksmith-2.7.2/src/blacksmith/middleware/_async/circuit_breaker.py
+-rw-r--r--   0        0        0     5933 2024-01-21 22:29:45.097079 blacksmith-2.7.2/src/blacksmith/middleware/_async/http_cache.py
+-rw-r--r--   0        0        0     2436 2024-01-21 22:29:45.097079 blacksmith-2.7.2/src/blacksmith/middleware/_async/prometheus.py
+-rw-r--r--   0        0        0     2869 2024-01-21 22:29:45.097079 blacksmith-2.7.2/src/blacksmith/middleware/_async/zipkin.py
+-rw-r--r--   0        0        0      696 2024-04-06 17:34:42.031293 blacksmith-2.7.2/src/blacksmith/middleware/_sync/__init__.py
+-rw-r--r--   0        0        0      797 2024-04-06 17:34:42.031293 blacksmith-2.7.2/src/blacksmith/middleware/_sync/auth.py
+-rw-r--r--   0        0        0     1434 2024-04-06 17:34:42.031293 blacksmith-2.7.2/src/blacksmith/middleware/_sync/base.py
+-rw-r--r--   0        0        0     2284 2024-04-06 17:34:42.031293 blacksmith-2.7.2/src/blacksmith/middleware/_sync/circuit_breaker.py
+-rw-r--r--   0        0        0     5827 2024-04-06 17:34:42.034626 blacksmith-2.7.2/src/blacksmith/middleware/_sync/http_cache.py
+-rw-r--r--   0        0        0     2418 2024-04-06 17:34:42.034626 blacksmith-2.7.2/src/blacksmith/middleware/_sync/prometheus.py
+-rw-r--r--   0        0        0     2851 2024-04-06 17:34:42.037960 blacksmith-2.7.2/src/blacksmith/middleware/_sync/zipkin.py
+-rw-r--r--   0        0        0        0 2024-01-21 22:29:45.097079 blacksmith-2.7.2/src/blacksmith/py.typed
+-rw-r--r--   0        0        0       24 2021-10-24 11:21:34.426587 blacksmith-2.7.2/src/blacksmith/sd/__init__.py
+-rw-r--r--   0        0        0      334 2024-01-21 22:29:45.097079 blacksmith-2.7.2/src/blacksmith/sd/_async/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-21 22:29:45.097079 blacksmith-2.7.2/src/blacksmith/sd/_async/adapters/__init__.py
+-rw-r--r--   0        0        0     5666 2024-01-21 22:29:45.097079 blacksmith-2.7.2/src/blacksmith/sd/_async/adapters/consul.py
+-rw-r--r--   0        0        0     1693 2024-01-21 22:29:45.097079 blacksmith-2.7.2/src/blacksmith/sd/_async/adapters/router.py
+-rw-r--r--   0        0        0     1010 2024-01-21 22:29:45.097079 blacksmith-2.7.2/src/blacksmith/sd/_async/adapters/static.py
+-rw-r--r--   0        0        0      317 2024-01-21 22:29:45.097079 blacksmith-2.7.2/src/blacksmith/sd/_async/base.py
+-rw-r--r--   0        0        0      326 2024-04-06 17:34:42.037960 blacksmith-2.7.2/src/blacksmith/sd/_sync/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-06 17:34:42.037960 blacksmith-2.7.2/src/blacksmith/sd/_sync/adapters/__init__.py
+-rw-r--r--   0        0        0     5620 2024-04-06 17:34:42.041293 blacksmith-2.7.2/src/blacksmith/sd/_sync/adapters/consul.py
+-rw-r--r--   0        0        0     1684 2024-04-06 17:34:42.041293 blacksmith-2.7.2/src/blacksmith/sd/_sync/adapters/router.py
+-rw-r--r--   0        0        0     1001 2024-04-06 17:34:42.041293 blacksmith-2.7.2/src/blacksmith/sd/_sync/adapters/static.py
+-rw-r--r--   0        0        0      310 2024-04-06 17:34:42.037960 blacksmith-2.7.2/src/blacksmith/sd/_sync/base.py
+-rw-r--r--   0        0        0        0 2021-10-23 21:02:59.310144 blacksmith-2.7.2/src/blacksmith/service/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-21 22:29:45.097079 blacksmith-2.7.2/src/blacksmith/service/_async/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-21 22:29:45.097079 blacksmith-2.7.2/src/blacksmith/service/_async/adapters/__init__.py
+-rw-r--r--   0        0        0     2146 2024-01-21 22:29:45.097079 blacksmith-2.7.2/src/blacksmith/service/_async/adapters/httpx.py
+-rw-r--r--   0        0        0      420 2024-01-21 22:29:45.097079 blacksmith-2.7.2/src/blacksmith/service/_async/base.py
+-rw-r--r--   0        0        0     5903 2024-01-21 22:29:45.097079 blacksmith-2.7.2/src/blacksmith/service/_async/client.py
+-rw-r--r--   0        0        0    14250 2024-01-21 22:29:45.097079 blacksmith-2.7.2/src/blacksmith/service/_async/route_proxy.py
+-rw-r--r--   0        0        0        0 2024-04-06 17:34:42.041293 blacksmith-2.7.2/src/blacksmith/service/_sync/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-06 17:34:42.051293 blacksmith-2.7.2/src/blacksmith/service/_sync/adapters/__init__.py
+-rw-r--r--   0        0        0     2123 2024-04-06 17:34:42.051293 blacksmith-2.7.2/src/blacksmith/service/_sync/adapters/httpx.py
+-rw-r--r--   0        0        0      417 2024-04-06 17:34:42.041293 blacksmith-2.7.2/src/blacksmith/service/_sync/base.py
+-rw-r--r--   0        0        0     5837 2024-04-06 17:34:45.201309 blacksmith-2.7.2/src/blacksmith/service/_sync/client.py
+-rw-r--r--   0        0        0    13869 2024-04-06 17:34:45.387976 blacksmith-2.7.2/src/blacksmith/service/_sync/route_proxy.py
+-rw-r--r--   0        0        0     8388 2024-02-05 17:58:05.369286 blacksmith-2.7.2/src/blacksmith/service/http_body_serializer.py
+-rw-r--r--   0        0        0      121 2024-01-21 22:29:45.097079 blacksmith-2.7.2/src/blacksmith/service/ports.py
+-rw-r--r--   0        0        0      450 2024-01-21 22:29:45.097079 blacksmith-2.7.2/src/blacksmith/typing.py
+-rw-r--r--   0        0        0     5577 1970-01-01 00:00:00.000000 blacksmith-2.7.2/PKG-INFO
```

### Comparing `blacksmith-2.7.1/LICENSE` & `blacksmith-2.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `blacksmith-2.7.1/README.rst` & `blacksmith-2.7.2/README.rst`

 * *Files identical despite different names*

### Comparing `blacksmith-2.7.1/pyproject.toml` & `blacksmith-2.7.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 description = "REST API Client designed for microservices"
 homepage = "https://github.com/mardiros/blacksmith"
 license = "BSD-derived"
 name = "blacksmith"
 
 readme = "README.rst"
 repository = "https://github.com/mardiros/blacksmith"
-version = "2.7.1"
+version = "2.7.2"
 
 [tool.poetry.dependencies]
 python = "^3.7"
 httpx = [
   {python = "3.7", version = "^0.24.1"},
   {python = ">=3.8", version = ">=0.24, <1"},
 ]
```

### Comparing `blacksmith-2.7.1/src/blacksmith/__init__.py` & `blacksmith-2.7.2/src/blacksmith/__init__.py`

 * *Files identical despite different names*

### Comparing `blacksmith-2.7.1/src/blacksmith/domain/error.py` & `blacksmith-2.7.2/src/blacksmith/domain/error.py`

 * *Files identical despite different names*

### Comparing `blacksmith-2.7.1/src/blacksmith/domain/exceptions.py` & `blacksmith-2.7.2/src/blacksmith/domain/exceptions.py`

 * *Files identical despite different names*

### Comparing `blacksmith-2.7.1/src/blacksmith/domain/model/__init__.py` & `blacksmith-2.7.2/src/blacksmith/domain/model/__init__.py`

 * *Files identical despite different names*

### Comparing `blacksmith-2.7.1/src/blacksmith/domain/model/http.py` & `blacksmith-2.7.2/src/blacksmith/domain/model/http.py`

 * *Files identical despite different names*

### Comparing `blacksmith-2.7.1/src/blacksmith/domain/model/middleware/circuit_breaker.py` & `blacksmith-2.7.2/src/blacksmith/domain/model/middleware/circuit_breaker.py`

 * *Files identical despite different names*

### Comparing `blacksmith-2.7.1/src/blacksmith/domain/model/middleware/http_cache.py` & `blacksmith-2.7.2/src/blacksmith/domain/model/middleware/http_cache.py`

 * *Files identical despite different names*

### Comparing `blacksmith-2.7.1/src/blacksmith/domain/model/middleware/prometheus.py` & `blacksmith-2.7.2/src/blacksmith/domain/model/middleware/prometheus.py`

 * *Files identical despite different names*

### Comparing `blacksmith-2.7.1/src/blacksmith/domain/model/middleware/zipkin.py` & `blacksmith-2.7.2/src/blacksmith/domain/model/middleware/zipkin.py`

 * *Files identical despite different names*

### Comparing `blacksmith-2.7.1/src/blacksmith/domain/model/params.py` & `blacksmith-2.7.2/src/blacksmith/domain/model/params.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,16 +49,16 @@
     Request Params Model.
 
     Fields must use subclass :func:`.PathInfoField`, :func:`.HeaderField`,
     :func:`.QueryStringField` or :func:`.PostBodyField` to declare each fields.
     """
 
 
-TResponse = TypeVar("TResponse", bound="Response")
-TCollectionResponse = TypeVar("TCollectionResponse", bound="Response")
+TResponse = TypeVar("TResponse", bound="Optional[Response]")
+TCollectionResponse = TypeVar("TCollectionResponse", bound="Optional[Response]")
 
 
 class Response(BaseModel):
     """Response Model."""
 
 
 @dataclass
```

### Comparing `blacksmith-2.7.1/src/blacksmith/domain/registry.py` & `blacksmith-2.7.2/src/blacksmith/domain/registry.py`

 * *Files identical despite different names*

### Comparing `blacksmith-2.7.1/src/blacksmith/domain/scanner.py` & `blacksmith-2.7.2/src/blacksmith/domain/scanner.py`

 * *Files identical despite different names*

### Comparing `blacksmith-2.7.1/src/blacksmith/domain/typing.py` & `blacksmith-2.7.2/src/blacksmith/domain/typing.py`

 * *Files identical despite different names*

### Comparing `blacksmith-2.7.1/src/blacksmith/middleware/_async/__init__.py` & `blacksmith-2.7.2/src/blacksmith/middleware/_async/__init__.py`

 * *Files identical despite different names*

### Comparing `blacksmith-2.7.1/src/blacksmith/middleware/_async/auth.py` & `blacksmith-2.7.2/src/blacksmith/middleware/_async/auth.py`

 * *Files identical despite different names*

### Comparing `blacksmith-2.7.1/src/blacksmith/middleware/_async/base.py` & `blacksmith-2.7.2/src/blacksmith/middleware/_async/base.py`

 * *Files identical despite different names*

### Comparing `blacksmith-2.7.1/src/blacksmith/middleware/_async/circuit_breaker.py` & `blacksmith-2.7.2/src/blacksmith/middleware/_async/circuit_breaker.py`

 * *Files identical despite different names*

### Comparing `blacksmith-2.7.1/src/blacksmith/middleware/_async/http_cache.py` & `blacksmith-2.7.2/src/blacksmith/middleware/_async/http_cache.py`

 * *Files identical despite different names*

### Comparing `blacksmith-2.7.1/src/blacksmith/middleware/_async/prometheus.py` & `blacksmith-2.7.2/src/blacksmith/middleware/_async/prometheus.py`

 * *Files identical despite different names*

### Comparing `blacksmith-2.7.1/src/blacksmith/middleware/_async/zipkin.py` & `blacksmith-2.7.2/src/blacksmith/middleware/_async/zipkin.py`

 * *Files identical despite different names*

### Comparing `blacksmith-2.7.1/src/blacksmith/middleware/_sync/__init__.py` & `blacksmith-2.7.2/src/blacksmith/middleware/_sync/__init__.py`

 * *Files identical despite different names*

### Comparing `blacksmith-2.7.1/src/blacksmith/middleware/_sync/auth.py` & `blacksmith-2.7.2/src/blacksmith/middleware/_sync/auth.py`

 * *Files identical despite different names*

### Comparing `blacksmith-2.7.1/src/blacksmith/middleware/_sync/base.py` & `blacksmith-2.7.2/src/blacksmith/middleware/_sync/base.py`

 * *Files identical despite different names*

### Comparing `blacksmith-2.7.1/src/blacksmith/middleware/_sync/circuit_breaker.py` & `blacksmith-2.7.2/src/blacksmith/middleware/_sync/circuit_breaker.py`

 * *Files identical despite different names*

### Comparing `blacksmith-2.7.1/src/blacksmith/middleware/_sync/http_cache.py` & `blacksmith-2.7.2/src/blacksmith/middleware/_sync/http_cache.py`

 * *Files identical despite different names*

### Comparing `blacksmith-2.7.1/src/blacksmith/middleware/_sync/prometheus.py` & `blacksmith-2.7.2/src/blacksmith/middleware/_sync/prometheus.py`

 * *Files identical despite different names*

### Comparing `blacksmith-2.7.1/src/blacksmith/middleware/_sync/zipkin.py` & `blacksmith-2.7.2/src/blacksmith/middleware/_sync/zipkin.py`

 * *Files identical despite different names*

### Comparing `blacksmith-2.7.1/src/blacksmith/sd/_async/adapters/consul.py` & `blacksmith-2.7.2/src/blacksmith/sd/_async/adapters/consul.py`

 * *Files identical despite different names*

### Comparing `blacksmith-2.7.1/src/blacksmith/sd/_async/adapters/router.py` & `blacksmith-2.7.2/src/blacksmith/sd/_async/adapters/router.py`

 * *Files identical despite different names*

### Comparing `blacksmith-2.7.1/src/blacksmith/sd/_async/adapters/static.py` & `blacksmith-2.7.2/src/blacksmith/sd/_async/adapters/static.py`

 * *Files identical despite different names*

### Comparing `blacksmith-2.7.1/src/blacksmith/sd/_sync/adapters/consul.py` & `blacksmith-2.7.2/src/blacksmith/sd/_sync/adapters/consul.py`

 * *Files identical despite different names*

### Comparing `blacksmith-2.7.1/src/blacksmith/sd/_sync/adapters/router.py` & `blacksmith-2.7.2/src/blacksmith/sd/_sync/adapters/router.py`

 * *Files identical despite different names*

### Comparing `blacksmith-2.7.1/src/blacksmith/sd/_sync/adapters/static.py` & `blacksmith-2.7.2/src/blacksmith/sd/_sync/adapters/static.py`

 * *Files identical despite different names*

### Comparing `blacksmith-2.7.1/src/blacksmith/service/_async/adapters/httpx.py` & `blacksmith-2.7.2/src/blacksmith/service/_async/adapters/httpx.py`

 * *Files identical despite different names*

### Comparing `blacksmith-2.7.1/src/blacksmith/service/_async/client.py` & `blacksmith-2.7.2/src/blacksmith/service/_async/client.py`

 * *Files identical despite different names*

### Comparing `blacksmith-2.7.1/src/blacksmith/service/_async/route_proxy.py` & `blacksmith-2.7.2/src/blacksmith/service/_async/route_proxy.py`

 * *Files identical despite different names*

### Comparing `blacksmith-2.7.1/src/blacksmith/service/_sync/adapters/httpx.py` & `blacksmith-2.7.2/src/blacksmith/service/_sync/adapters/httpx.py`

 * *Files identical despite different names*

### Comparing `blacksmith-2.7.1/src/blacksmith/service/_sync/client.py` & `blacksmith-2.7.2/src/blacksmith/service/_sync/client.py`

 * *Files identical despite different names*

### Comparing `blacksmith-2.7.1/src/blacksmith/service/_sync/route_proxy.py` & `blacksmith-2.7.2/src/blacksmith/service/_sync/route_proxy.py`

 * *Files identical despite different names*

### Comparing `blacksmith-2.7.1/src/blacksmith/service/http_body_serializer.py` & `blacksmith-2.7.2/src/blacksmith/service/http_body_serializer.py`

 * *Files identical despite different names*

### Comparing `blacksmith-2.7.1/PKG-INFO` & `blacksmith-2.7.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blacksmith
-Version: 2.7.1
+Version: 2.7.2
 Summary: REST API Client designed for microservices
 Home-page: https://github.com/mardiros/blacksmith
 License: BSD-derived
 Author: Guillaume Gauvrit
 Author-email: guillaume@gauvr.it
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 4 - Beta
```

