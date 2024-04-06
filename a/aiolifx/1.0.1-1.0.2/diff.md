# Comparing `tmp/aiolifx-1.0.1.tar.gz` & `tmp/aiolifx-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiolifx-1.0.1.tar", last modified: Sat Jan 13 09:40:21 2024, max compression
+gzip compressed data, was "aiolifx-1.0.2.tar", last modified: Sat Apr  6 10:48:36 2024, max compression
```

## Comparing `aiolifx-1.0.1.tar` & `aiolifx-1.0.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 fw        (1000) fw        (1000)        0 2024-01-13 09:40:21.989624 aiolifx-1.0.1/
--rw-rw-r--   0 fw        (1000) fw        (1000)     1085 2021-05-03 10:41:06.000000 aiolifx-1.0.1/LICENSE.txt
--rw-rw-r--   0 fw        (1000) fw        (1000)       68 2021-05-03 10:41:06.000000 aiolifx-1.0.1/MANIFEST.in
--rw-r--r--   0 fw        (1000) fw        (1000)     4103 2024-01-13 09:40:21.989624 aiolifx-1.0.1/PKG-INFO
--rw-rw-r--   0 fw        (1000) fw        (1000)     3476 2023-04-23 10:52:10.000000 aiolifx-1.0.1/README.md
-drwxrwxr-x   0 fw        (1000) fw        (1000)        0 2024-01-13 09:40:21.985624 aiolifx-1.0.1/aiolifx/
--rw-rw-r--   0 fw        (1000) fw        (1000)      171 2022-08-04 14:39:27.000000 aiolifx-1.0.1/aiolifx/__init__.py
--rw-rw-r--   0 fw        (1000) fw        (1000)    24945 2023-04-23 15:22:45.000000 aiolifx-1.0.1/aiolifx/__main__.py
--rw-rw-r--   0 fw        (1000) fw        (1000)    85487 2024-01-13 09:26:58.000000 aiolifx-1.0.1/aiolifx/aiolifx.py
--rw-rw-r--   0 fw        (1000) fw        (1000)      757 2022-08-04 14:39:27.000000 aiolifx-1.0.1/aiolifx/connection.py
--rw-rw-r--   0 fw        (1000) fw        (1000)     6392 2023-04-13 02:19:41.000000 aiolifx-1.0.1/aiolifx/message.py
--rw-rw-r--   0 fw        (1000) fw        (1000)    66140 2023-04-23 10:52:01.000000 aiolifx-1.0.1/aiolifx/msgtypes.py
--rw-rw-r--   0 fw        (1000) fw        (1000)     3083 2023-11-21 14:04:05.000000 aiolifx-1.0.1/aiolifx/products.py
--rw-rw-r--   0 fw        (1000) fw        (1000)    31595 2023-11-25 03:05:34.000000 aiolifx-1.0.1/aiolifx/products_defs.py
--rw-rw-r--   0 fw        (1000) fw        (1000)    25789 2023-04-23 10:52:01.000000 aiolifx-1.0.1/aiolifx/unpack.py
--rwxrwxr-x   0 fw        (1000) fw        (1000)     1615 2023-11-25 03:05:33.000000 aiolifx-1.0.1/aiolifx/update_products.py
-drwxrwxr-x   0 fw        (1000) fw        (1000)        0 2024-01-13 09:40:21.989624 aiolifx-1.0.1/aiolifx.egg-info/
--rw-r--r--   0 fw        (1000) fw        (1000)     4103 2024-01-13 09:40:21.000000 aiolifx-1.0.1/aiolifx.egg-info/PKG-INFO
--rw-rw-r--   0 fw        (1000) fw        (1000)      480 2024-01-13 09:40:21.000000 aiolifx-1.0.1/aiolifx.egg-info/SOURCES.txt
--rw-rw-r--   0 fw        (1000) fw        (1000)        1 2024-01-13 09:40:21.000000 aiolifx-1.0.1/aiolifx.egg-info/dependency_links.txt
--rw-rw-r--   0 fw        (1000) fw        (1000)       49 2024-01-13 09:40:21.000000 aiolifx-1.0.1/aiolifx.egg-info/entry_points.txt
--rw-rw-r--   0 fw        (1000) fw        (1000)        1 2024-01-13 09:40:21.000000 aiolifx-1.0.1/aiolifx.egg-info/not-zip-safe
--rw-rw-r--   0 fw        (1000) fw        (1000)       83 2024-01-13 09:40:21.000000 aiolifx-1.0.1/aiolifx.egg-info/requires.txt
--rw-rw-r--   0 fw        (1000) fw        (1000)        8 2024-01-13 09:40:21.000000 aiolifx-1.0.1/aiolifx.egg-info/top_level.txt
--rw-rw-r--   0 fw        (1000) fw        (1000)       79 2024-01-13 09:40:21.989624 aiolifx-1.0.1/setup.cfg
--rw-rw-r--   0 fw        (1000) fw        (1000)     1305 2024-01-13 09:35:19.000000 aiolifx-1.0.1/setup.py
+drwxrwxr-x   0 fw        (1000) fw        (1000)        0 2024-04-06 10:48:36.288261 aiolifx-1.0.2/
+-rw-rw-r--   0 fw        (1000) fw        (1000)     1085 2021-05-03 10:41:06.000000 aiolifx-1.0.2/LICENSE.txt
+-rw-rw-r--   0 fw        (1000) fw        (1000)       68 2021-05-03 10:41:06.000000 aiolifx-1.0.2/MANIFEST.in
+-rw-r--r--   0 fw        (1000) fw        (1000)     4103 2024-04-06 10:48:36.288261 aiolifx-1.0.2/PKG-INFO
+-rw-rw-r--   0 fw        (1000) fw        (1000)     3476 2023-04-23 10:52:10.000000 aiolifx-1.0.2/README.md
+drwxrwxr-x   0 fw        (1000) fw        (1000)        0 2024-04-06 10:48:36.288261 aiolifx-1.0.2/aiolifx/
+-rw-rw-r--   0 fw        (1000) fw        (1000)      171 2022-08-04 14:39:27.000000 aiolifx-1.0.2/aiolifx/__init__.py
+-rw-rw-r--   0 fw        (1000) fw        (1000)    24945 2023-04-23 15:22:45.000000 aiolifx-1.0.2/aiolifx/__main__.py
+-rw-rw-r--   0 fw        (1000) fw        (1000)    85487 2024-01-13 09:26:58.000000 aiolifx-1.0.2/aiolifx/aiolifx.py
+-rw-rw-r--   0 fw        (1000) fw        (1000)      757 2022-08-04 14:39:27.000000 aiolifx-1.0.2/aiolifx/connection.py
+-rw-rw-r--   0 fw        (1000) fw        (1000)     6392 2023-04-13 02:19:41.000000 aiolifx-1.0.2/aiolifx/message.py
+-rw-rw-r--   0 fw        (1000) fw        (1000)    66140 2023-04-23 10:52:01.000000 aiolifx-1.0.2/aiolifx/msgtypes.py
+-rw-rw-r--   0 fw        (1000) fw        (1000)     3083 2023-11-21 14:04:05.000000 aiolifx-1.0.2/aiolifx/products.py
+-rw-rw-r--   0 fw        (1000) fw        (1000)    40436 2024-04-06 10:35:02.000000 aiolifx-1.0.2/aiolifx/products_defs.py
+-rw-rw-r--   0 fw        (1000) fw        (1000)    25789 2023-04-23 10:52:01.000000 aiolifx-1.0.2/aiolifx/unpack.py
+-rwxrwxr-x   0 fw        (1000) fw        (1000)     1615 2023-11-25 03:05:33.000000 aiolifx-1.0.2/aiolifx/update_products.py
+drwxrwxr-x   0 fw        (1000) fw        (1000)        0 2024-04-06 10:48:36.288261 aiolifx-1.0.2/aiolifx.egg-info/
+-rw-r--r--   0 fw        (1000) fw        (1000)     4103 2024-04-06 10:48:36.000000 aiolifx-1.0.2/aiolifx.egg-info/PKG-INFO
+-rw-rw-r--   0 fw        (1000) fw        (1000)      480 2024-04-06 10:48:36.000000 aiolifx-1.0.2/aiolifx.egg-info/SOURCES.txt
+-rw-rw-r--   0 fw        (1000) fw        (1000)        1 2024-04-06 10:48:36.000000 aiolifx-1.0.2/aiolifx.egg-info/dependency_links.txt
+-rw-rw-r--   0 fw        (1000) fw        (1000)       49 2024-04-06 10:48:36.000000 aiolifx-1.0.2/aiolifx.egg-info/entry_points.txt
+-rw-rw-r--   0 fw        (1000) fw        (1000)        1 2024-04-06 10:48:36.000000 aiolifx-1.0.2/aiolifx.egg-info/not-zip-safe
+-rw-rw-r--   0 fw        (1000) fw        (1000)       83 2024-04-06 10:48:36.000000 aiolifx-1.0.2/aiolifx.egg-info/requires.txt
+-rw-rw-r--   0 fw        (1000) fw        (1000)        8 2024-04-06 10:48:36.000000 aiolifx-1.0.2/aiolifx.egg-info/top_level.txt
+-rw-rw-r--   0 fw        (1000) fw        (1000)       79 2024-04-06 10:48:36.288261 aiolifx-1.0.2/setup.cfg
+-rw-rw-r--   0 fw        (1000) fw        (1000)     1305 2024-04-06 10:36:27.000000 aiolifx-1.0.2/setup.py
```

### Comparing `aiolifx-1.0.1/LICENSE.txt` & `aiolifx-1.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aiolifx-1.0.1/PKG-INFO` & `aiolifx-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiolifx
-Version: 1.0.1
+Version: 1.0.2
 Summary: API for local communication with LIFX devices over a LAN with asyncio.
 Home-page: http://github.com/frawau/aiolifx
 Author: François Wautier
 Author-email: francois@wautier.eu
 License: MIT
 Keywords: lifx,light,automation
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `aiolifx-1.0.1/README.md` & `aiolifx-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `aiolifx-1.0.1/aiolifx/__main__.py` & `aiolifx-1.0.2/aiolifx/__main__.py`

 * *Files identical despite different names*

### Comparing `aiolifx-1.0.1/aiolifx/aiolifx.py` & `aiolifx-1.0.2/aiolifx/aiolifx.py`

 * *Files identical despite different names*

### Comparing `aiolifx-1.0.1/aiolifx/connection.py` & `aiolifx-1.0.2/aiolifx/connection.py`

 * *Files identical despite different names*

### Comparing `aiolifx-1.0.1/aiolifx/message.py` & `aiolifx-1.0.2/aiolifx/message.py`

 * *Files identical despite different names*

### Comparing `aiolifx-1.0.1/aiolifx/msgtypes.py` & `aiolifx-1.0.2/aiolifx/msgtypes.py`

 * *Files identical despite different names*

### Comparing `aiolifx-1.0.1/aiolifx/products.py` & `aiolifx-1.0.2/aiolifx/products.py`

 * *Files identical despite different names*

### Comparing `aiolifx-1.0.1/aiolifx/products_defs.py` & `aiolifx-1.0.2/aiolifx/products_defs.py`

 * *Files 7% similar despite different names*

```diff
@@ -88,14 +88,40 @@
     136: "LIFX GU10 Color Intl",
     137: "LIFX Candle Color US",
     138: "LIFX Candle Color Intl",
     141: "LIFX Neon US",
     142: "LIFX Neon Intl",
     143: "LIFX String US",
     144: "LIFX String Intl",
+    161: "LIFX Outdoor Neon US",
+    162: "LIFX Outdoor Neon Intl",
+    163: "LIFX A19 US",
+    164: "LIFX BR30 US",
+    165: "LIFX A19 Intl",
+    166: "LIFX BR30 Intl",
+    167: "LIFX Downlight",
+    168: "LIFX Downlight",
+    169: "LIFX A21 1600lm US",
+    170: "LIFX A21 1600lm Intl",
+    171: "LIFX Round Spot US",
+    173: "LIFX Round Path US",
+    174: "LIFX Square Path US",
+    175: "LIFX PAR38 US",
+    176: "LIFX Ceiling US",
+    177: "LIFX Ceiling Intl",
+    181: "LIFX Color US",
+    182: "LIFX Color Intl",
+    185: "LIFX Candle Color US",
+    186: "LIFX Candle Color Intl",
+    187: "LIFX Candle Color US",
+    188: "LIFX Candle Color Intl",
+    203: "LIFX String US",
+    204: "LIFX String Intl",
+    205: "LIFX Indoor Neon US",
+    206: "LIFX Indoor Neon Intl",
 }
 
 features_map = {
     1: {
         "buttons": False,
         "chain": False,
         "color": True,
@@ -1294,13 +1320,351 @@
         "buttons": False,
         "chain": False,
         "color": True,
         "extended_multizone": True,
         "hev": False,
         "infrared": False,
         "matrix": False,
+        "max_kelvin": 9000,
+        "min_kelvin": 1500,
+        "multizone": True,
+        "relays": False,
+    },
+    161: {
+        "buttons": False,
+        "chain": False,
+        "color": True,
+        "extended_multizone": True,
+        "hev": False,
+        "infrared": False,
+        "matrix": False,
+        "max_kelvin": 9000,
+        "min_kelvin": 1500,
+        "multizone": True,
+        "relays": False,
+    },
+    162: {
+        "buttons": False,
+        "chain": False,
+        "color": True,
+        "extended_multizone": True,
+        "hev": False,
+        "infrared": False,
+        "matrix": False,
+        "max_kelvin": 9000,
+        "min_kelvin": 1500,
+        "multizone": True,
+        "relays": False,
+    },
+    163: {
+        "buttons": False,
+        "chain": False,
+        "color": True,
+        "extended_multizone": True,
+        "hev": False,
+        "infrared": False,
+        "matrix": False,
+        "max_kelvin": 9000,
+        "min_kelvin": 1500,
+        "multizone": True,
+        "relays": False,
+    },
+    164: {
+        "buttons": False,
+        "chain": False,
+        "color": True,
+        "extended_multizone": False,
+        "hev": False,
+        "infrared": False,
+        "matrix": False,
+        "max_kelvin": 9000,
+        "min_kelvin": 1500,
+        "multizone": False,
+        "relays": False,
+    },
+    165: {
+        "buttons": False,
+        "chain": False,
+        "color": True,
+        "extended_multizone": True,
+        "hev": False,
+        "infrared": False,
+        "matrix": False,
+        "max_kelvin": 9000,
+        "min_kelvin": 1500,
+        "multizone": True,
+        "relays": False,
+    },
+    166: {
+        "buttons": False,
+        "chain": False,
+        "color": True,
+        "extended_multizone": False,
+        "hev": False,
+        "infrared": False,
+        "matrix": False,
+        "max_kelvin": 9000,
+        "min_kelvin": 1500,
+        "multizone": False,
+        "relays": False,
+    },
+    167: {
+        "buttons": False,
+        "chain": False,
+        "color": True,
+        "extended_multizone": False,
+        "hev": False,
+        "infrared": False,
+        "matrix": False,
+        "max_kelvin": 9000,
+        "min_kelvin": 1500,
+        "multizone": False,
+        "relays": False,
+    },
+    168: {
+        "buttons": False,
+        "chain": False,
+        "color": True,
+        "extended_multizone": False,
+        "hev": False,
+        "infrared": False,
+        "matrix": False,
+        "max_kelvin": 9000,
+        "min_kelvin": 1500,
+        "multizone": False,
+        "relays": False,
+    },
+    169: {
+        "buttons": False,
+        "chain": False,
+        "color": True,
+        "extended_multizone": False,
+        "hev": False,
+        "infrared": False,
+        "matrix": False,
+        "max_kelvin": 9000,
+        "min_kelvin": 1500,
+        "multizone": False,
+        "relays": False,
+    },
+    170: {
+        "buttons": False,
+        "chain": False,
+        "color": True,
+        "extended_multizone": False,
+        "hev": False,
+        "infrared": False,
+        "matrix": False,
+        "max_kelvin": 9000,
+        "min_kelvin": 1500,
+        "multizone": False,
+        "relays": False,
+    },
+    171: {
+        "buttons": False,
+        "chain": False,
+        "color": True,
+        "extended_multizone": False,
+        "hev": False,
+        "infrared": False,
+        "matrix": True,
+        "max_kelvin": 9000,
+        "min_kelvin": 1500,
+        "multizone": False,
+        "relays": False,
+    },
+    173: {
+        "buttons": False,
+        "chain": False,
+        "color": True,
+        "extended_multizone": False,
+        "hev": False,
+        "infrared": False,
+        "matrix": True,
+        "max_kelvin": 9000,
+        "min_kelvin": 1500,
+        "multizone": False,
+        "relays": False,
+    },
+    174: {
+        "buttons": False,
+        "chain": False,
+        "color": True,
+        "extended_multizone": False,
+        "hev": False,
+        "infrared": False,
+        "matrix": True,
+        "max_kelvin": 9000,
+        "min_kelvin": 1500,
+        "multizone": False,
+        "relays": False,
+    },
+    175: {
+        "buttons": False,
+        "chain": False,
+        "color": True,
+        "extended_multizone": False,
+        "hev": False,
+        "infrared": False,
+        "matrix": False,
+        "max_kelvin": 9000,
+        "min_kelvin": 1500,
+        "multizone": False,
+        "relays": False,
+    },
+    176: {
+        "buttons": False,
+        "chain": False,
+        "color": True,
+        "extended_multizone": False,
+        "hev": False,
+        "infrared": False,
+        "matrix": True,
+        "max_kelvin": 9000,
+        "min_kelvin": 1500,
+        "multizone": False,
+        "relays": False,
+    },
+    177: {
+        "buttons": False,
+        "chain": False,
+        "color": True,
+        "extended_multizone": False,
+        "hev": False,
+        "infrared": False,
+        "matrix": True,
+        "max_kelvin": 9000,
+        "min_kelvin": 1500,
+        "multizone": False,
+        "relays": False,
+    },
+    181: {
+        "buttons": False,
+        "chain": False,
+        "color": True,
+        "extended_multizone": False,
+        "hev": False,
+        "infrared": False,
+        "matrix": False,
+        "max_kelvin": 9000,
+        "min_kelvin": 1500,
+        "multizone": False,
+        "relays": False,
+    },
+    182: {
+        "buttons": False,
+        "chain": False,
+        "color": True,
+        "extended_multizone": False,
+        "hev": False,
+        "infrared": False,
+        "matrix": False,
+        "max_kelvin": 9000,
+        "min_kelvin": 1500,
+        "multizone": False,
+        "relays": False,
+    },
+    185: {
+        "buttons": False,
+        "chain": False,
+        "color": True,
+        "extended_multizone": False,
+        "hev": False,
+        "infrared": False,
+        "matrix": True,
+        "max_kelvin": 9000,
+        "min_kelvin": 1500,
+        "multizone": False,
+        "relays": False,
+    },
+    186: {
+        "buttons": False,
+        "chain": False,
+        "color": True,
+        "extended_multizone": False,
+        "hev": False,
+        "infrared": False,
+        "matrix": True,
+        "max_kelvin": 9000,
+        "min_kelvin": 1500,
+        "multizone": False,
+        "relays": False,
+    },
+    187: {
+        "buttons": False,
+        "chain": False,
+        "color": True,
+        "extended_multizone": False,
+        "hev": False,
+        "infrared": False,
+        "matrix": False,
+        "max_kelvin": 9000,
+        "min_kelvin": 1500,
+        "multizone": False,
+        "relays": False,
+    },
+    188: {
+        "buttons": False,
+        "chain": False,
+        "color": True,
+        "extended_multizone": False,
+        "hev": False,
+        "infrared": False,
+        "matrix": False,
+        "max_kelvin": 9000,
+        "min_kelvin": 1500,
+        "multizone": False,
+        "relays": False,
+    },
+    203: {
+        "buttons": False,
+        "chain": False,
+        "color": True,
+        "extended_multizone": True,
+        "hev": False,
+        "infrared": False,
+        "matrix": False,
+        "max_kelvin": 9000,
+        "min_kelvin": 1500,
+        "multizone": True,
+        "relays": False,
+    },
+    204: {
+        "buttons": False,
+        "chain": False,
+        "color": True,
+        "extended_multizone": True,
+        "hev": False,
+        "infrared": False,
+        "matrix": False,
+        "max_kelvin": 9000,
+        "min_kelvin": 1500,
+        "multizone": True,
+        "relays": False,
+    },
+    205: {
+        "buttons": False,
+        "chain": False,
+        "color": True,
+        "extended_multizone": True,
+        "hev": False,
+        "infrared": False,
+        "matrix": False,
+        "max_kelvin": 9000,
+        "min_kelvin": 1500,
+        "multizone": True,
+        "relays": False,
+    },
+    206: {
+        "buttons": False,
+        "chain": False,
+        "color": True,
+        "extended_multizone": True,
+        "hev": False,
+        "infrared": False,
+        "matrix": False,
         "max_kelvin": 9000,
         "min_kelvin": 1500,
         "multizone": True,
         "relays": False,
     },
 }
```

### Comparing `aiolifx-1.0.1/aiolifx/unpack.py` & `aiolifx-1.0.2/aiolifx/unpack.py`

 * *Files identical despite different names*

### Comparing `aiolifx-1.0.1/aiolifx/update_products.py` & `aiolifx-1.0.2/aiolifx/update_products.py`

 * *Files identical despite different names*

### Comparing `aiolifx-1.0.1/aiolifx.egg-info/PKG-INFO` & `aiolifx-1.0.2/aiolifx.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiolifx
-Version: 1.0.1
+Version: 1.0.2
 Summary: API for local communication with LIFX devices over a LAN with asyncio.
 Home-page: http://github.com/frawau/aiolifx
 Author: François Wautier
 Author-email: francois@wautier.eu
 License: MIT
 Keywords: lifx,light,automation
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `aiolifx-1.0.1/setup.py` & `aiolifx-1.0.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3
 # -*- coding:utf-8 -*-
 import setuptools
 
-version = "1.0.1"
+version = "1.0.2"
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="aiolifx",
     packages=["aiolifx"],
```

