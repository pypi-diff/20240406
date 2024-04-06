# Comparing `tmp/pysma-plus-0.1.3.tar.gz` & `tmp/pysma-plus-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysma-plus-0.1.3.tar", last modified: Tue Apr  2 18:39:10 2024, max compression
+gzip compressed data, was "pysma-plus-0.1.4.tar", last modified: Sat Apr  6 09:25:57 2024, max compression
```

## Comparing `pysma-plus-0.1.3.tar` & `pysma-plus-0.1.4.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxr-x   0 sven      (1001) sven      (1001)        0 2024-04-02 18:39:10.097640 pysma-plus-0.1.3/
--rw-rw-r--   0 sven      (1001) sven      (1001)     1075 2024-03-27 10:30:58.000000 pysma-plus-0.1.3/LICENSE
--rw-rw-r--   0 sven      (1001) sven      (1001)       80 2024-03-30 19:14:11.000000 pysma-plus-0.1.3/MANIFEST.in
--rw-r--r--   0 sven      (1001) sven      (1001)     2669 2024-04-02 18:39:10.097640 pysma-plus-0.1.3/PKG-INFO
--rw-rw-r--   0 sven      (1001) sven      (1001)      642 2024-03-30 18:43:59.000000 pysma-plus-0.1.3/README.md
--rw-rw-r--   0 sven      (1001) sven      (1001)      895 2024-04-02 18:39:05.000000 pysma-plus-0.1.3/pyproject.toml
-drwxrwxr-x   0 sven      (1001) sven      (1001)        0 2024-04-02 18:39:10.097640 pysma-plus-0.1.3/pysma_plus.egg-info/
--rw-r--r--   0 sven      (1001) sven      (1001)     2669 2024-04-02 18:39:10.000000 pysma-plus-0.1.3/pysma_plus.egg-info/PKG-INFO
--rw-rw-r--   0 sven      (1001) sven      (1001)      597 2024-04-02 18:39:10.000000 pysma-plus-0.1.3/pysma_plus.egg-info/SOURCES.txt
--rw-rw-r--   0 sven      (1001) sven      (1001)        1 2024-04-02 18:39:10.000000 pysma-plus-0.1.3/pysma_plus.egg-info/dependency_links.txt
--rw-rw-r--   0 sven      (1001) sven      (1001)       35 2024-04-02 18:39:10.000000 pysma-plus-0.1.3/pysma_plus.egg-info/requires.txt
--rw-rw-r--   0 sven      (1001) sven      (1001)       10 2024-04-02 18:39:10.000000 pysma-plus-0.1.3/pysma_plus.egg-info/top_level.txt
--rw-rw-r--   0 sven      (1001) sven      (1001)        1 2024-03-30 19:16:34.000000 pysma-plus-0.1.3/pysma_plus.egg-info/zip-safe
-drwxrwxr-x   0 sven      (1001) sven      (1001)        0 2024-04-02 18:39:10.097640 pysma-plus-0.1.3/pysmaplus/
--rw-rw-r--   0 sven      (1001) sven      (1001)     1920 2024-03-29 07:19:41.000000 pysma-plus-0.1.3/pysmaplus/__init__.py
--rw-rw-r--   0 sven      (1001) sven      (1001)     6668 2024-03-31 12:59:54.000000 pysma-plus-0.1.3/pysmaplus/const.py
--rw-rw-r--   0 sven      (1001) sven      (1001)    21131 2024-03-28 08:57:32.000000 pysma-plus-0.1.3/pysmaplus/definitions.py
--rw-rw-r--   0 sven      (1001) sven      (1001)      507 2024-03-27 12:21:42.000000 pysma-plus-0.1.3/pysmaplus/device.py
--rw-rw-r--   0 sven      (1001) sven      (1001)      426 2024-03-27 10:31:31.000000 pysma-plus-0.1.3/pysmaplus/exceptions.py
--rw-rw-r--   0 sven      (1001) sven      (1001)      695 2024-03-27 10:31:31.000000 pysma-plus-0.1.3/pysmaplus/helpers.py
--rw-rw-r--   0 sven      (1001) sven      (1001)     6237 2024-03-31 12:44:16.000000 pysma-plus-0.1.3/pysmaplus/sensor.py
--rw-rw-r--   0 sven      (1001) sven      (1001)    13923 2024-04-02 12:33:41.000000 pysma-plus-0.1.3/pysmaplus/smaennexos.py
--rw-rw-r--   0 sven      (1001) sven      (1001)     9564 2024-04-02 18:32:46.000000 pysma-plus-0.1.3/pysmaplus/smaspeedwireem.py
--rw-rw-r--   0 sven      (1001) sven      (1001)    16136 2024-03-27 12:04:04.000000 pysma-plus-0.1.3/pysmaplus/smawebconnect.py
--rw-rw-r--   0 sven      (1001) sven      (1001)      229 2024-04-02 18:39:10.098640 pysma-plus-0.1.3/setup.cfg
--rw-rw-r--   0 sven      (1001) sven      (1001)      758 2024-04-02 18:39:05.000000 pysma-plus-0.1.3/setup.py
-drwxrwxr-x   0 sven      (1001) sven      (1001)        0 2024-04-02 18:39:10.097640 pysma-plus-0.1.3/tests/
--rw-rw-r--   0 sven      (1001) sven      (1001)   315314 2024-03-27 10:30:58.000000 pysma-plus-0.1.3/tests/__init__.py
--rw-rw-r--   0 sven      (1001) sven      (1001)      883 2024-03-27 10:30:58.000000 pysma-plus-0.1.3/tests/test_definitions.py
--rw-rw-r--   0 sven      (1001) sven      (1001)      433 2024-03-27 10:30:58.000000 pysma-plus-0.1.3/tests/test_helpers.py
--rw-rw-r--   0 sven      (1001) sven      (1001)    17280 2024-03-27 10:30:58.000000 pysma-plus-0.1.3/tests/test_init.py
--rw-rw-r--   0 sven      (1001) sven      (1001)     4785 2024-03-27 10:30:58.000000 pysma-plus-0.1.3/tests/test_sensor.py
+drwxrwxr-x   0 sven      (1001) sven      (1001)        0 2024-04-06 09:25:57.315550 pysma-plus-0.1.4/
+-rw-rw-r--   0 sven      (1001) sven      (1001)     1075 2024-03-27 10:30:58.000000 pysma-plus-0.1.4/LICENSE
+-rw-rw-r--   0 sven      (1001) sven      (1001)       80 2024-03-30 19:14:11.000000 pysma-plus-0.1.4/MANIFEST.in
+-rw-r--r--   0 sven      (1001) sven      (1001)     3112 2024-04-06 09:25:57.315550 pysma-plus-0.1.4/PKG-INFO
+-rw-rw-r--   0 sven      (1001) sven      (1001)     1085 2024-04-04 19:52:13.000000 pysma-plus-0.1.4/README.md
+-rw-rw-r--   0 sven      (1001) sven      (1001)      895 2024-04-06 09:25:53.000000 pysma-plus-0.1.4/pyproject.toml
+drwxrwxr-x   0 sven      (1001) sven      (1001)        0 2024-04-06 09:25:57.315550 pysma-plus-0.1.4/pysma_plus.egg-info/
+-rw-r--r--   0 sven      (1001) sven      (1001)     3112 2024-04-06 09:25:57.000000 pysma-plus-0.1.4/pysma_plus.egg-info/PKG-INFO
+-rw-rw-r--   0 sven      (1001) sven      (1001)      597 2024-04-06 09:25:57.000000 pysma-plus-0.1.4/pysma_plus.egg-info/SOURCES.txt
+-rw-rw-r--   0 sven      (1001) sven      (1001)        1 2024-04-06 09:25:57.000000 pysma-plus-0.1.4/pysma_plus.egg-info/dependency_links.txt
+-rw-rw-r--   0 sven      (1001) sven      (1001)       35 2024-04-06 09:25:57.000000 pysma-plus-0.1.4/pysma_plus.egg-info/requires.txt
+-rw-rw-r--   0 sven      (1001) sven      (1001)       10 2024-04-06 09:25:57.000000 pysma-plus-0.1.4/pysma_plus.egg-info/top_level.txt
+-rw-rw-r--   0 sven      (1001) sven      (1001)        1 2024-03-30 19:16:34.000000 pysma-plus-0.1.4/pysma_plus.egg-info/zip-safe
+drwxrwxr-x   0 sven      (1001) sven      (1001)        0 2024-04-06 09:25:57.314550 pysma-plus-0.1.4/pysmaplus/
+-rw-rw-r--   0 sven      (1001) sven      (1001)     1920 2024-03-29 07:19:41.000000 pysma-plus-0.1.4/pysmaplus/__init__.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)     6668 2024-04-05 16:45:56.000000 pysma-plus-0.1.4/pysmaplus/const.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)    21131 2024-03-28 08:57:32.000000 pysma-plus-0.1.4/pysmaplus/definitions.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)      603 2024-04-05 19:39:26.000000 pysma-plus-0.1.4/pysmaplus/device.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)      426 2024-03-27 10:31:31.000000 pysma-plus-0.1.4/pysmaplus/exceptions.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)      695 2024-03-27 10:31:31.000000 pysma-plus-0.1.4/pysmaplus/helpers.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)     6237 2024-04-05 16:46:03.000000 pysma-plus-0.1.4/pysmaplus/sensor.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)    15781 2024-04-05 19:32:42.000000 pysma-plus-0.1.4/pysmaplus/smaennexos.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)     9809 2024-04-05 19:23:38.000000 pysma-plus-0.1.4/pysmaplus/smaspeedwireem.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)    16194 2024-04-05 16:40:53.000000 pysma-plus-0.1.4/pysmaplus/smawebconnect.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)      229 2024-04-06 09:25:57.316550 pysma-plus-0.1.4/setup.cfg
+-rw-rw-r--   0 sven      (1001) sven      (1001)      758 2024-04-06 09:25:53.000000 pysma-plus-0.1.4/setup.py
+drwxrwxr-x   0 sven      (1001) sven      (1001)        0 2024-04-06 09:25:57.315550 pysma-plus-0.1.4/tests/
+-rw-rw-r--   0 sven      (1001) sven      (1001)   315314 2024-03-27 10:30:58.000000 pysma-plus-0.1.4/tests/__init__.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)      883 2024-03-27 10:30:58.000000 pysma-plus-0.1.4/tests/test_definitions.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)      433 2024-03-27 10:30:58.000000 pysma-plus-0.1.4/tests/test_helpers.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)    17280 2024-03-27 10:30:58.000000 pysma-plus-0.1.4/tests/test_init.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)     4785 2024-03-27 10:30:58.000000 pysma-plus-0.1.4/tests/test_sensor.py
```

### Comparing `pysma-plus-0.1.3/LICENSE` & `pysma-plus-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pysma-plus-0.1.3/PKG-INFO` & `pysma-plus-0.1.4/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pysma-plus
-Version: 0.1.3
+Version: 0.1.4
 Summary: Library to interface SMA Devices via WebConnect, EnnexOS and Energy Meter Devices
 Home-page: https://github.com/littleyoda/pysma
-Download-URL: https://github.com/littleyoda/pysma/tarball/0.1.3
+Download-URL: https://github.com/littleyoda/pysma/tarball/0.1.4
 Author: Sven Bursch-Osewold, Johann Kellerman and other
 Author-email: Sven Bursch-Osewold <sb_pysma@bursch.com>, Johann Kellerman <kellerza@gmail.com>
 License: The MIT License (MIT)
         
         Copyright (c) 2016 kellerza
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -55,9 +55,20 @@
 * SMA Energy Meter (EMETER-10, EMETER-20) und ### Sunny Home Manager 2.0 (shm2)
 
 
 ## Example usage
 
 See [example.py](./example.py) for a basic usage and tests
 
+## Successfully tested devices
 
+| Bereich | Gerät | Methode |
+|--|--|--|
+| Wechselrichter | Tripower X (STP XX-50)<br>(15,25) | ennexos |
+| Hybrid-Wechselrichter | Sunny Tripower Smart Energy<br>(10.0)  | webconnect |
+| Hybrid-Wechselrichter | Sunny Boy Storage<br>(SBS3.7-10, SBS5.0-10) | webconnect |
+| | | |
+| Energy Meter | Energy Meter 2<br>(EMTER 20) | speedwire |
+| Energy Meter | Sunny Home Manager 2<br>(SHM2) | speedwire |
+| | | |
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pysma-plus-0.1.3/pyproject.toml` & `pysma-plus-0.1.4/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pysma-plus"
-version = "0.1.3"
+version = "0.1.4"
 description = "Library to interface SMA Devices via WebConnect, EnnexOS and Energy Meter Devices"
 readme = "README.md"
 authors = [{ name = "Sven Bursch-Osewold", email = "sb_pysma@bursch.com" },{ name = "Johann Kellerman" , email ="kellerza@gmail.com"} ]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `pysma-plus-0.1.3/pysma_plus.egg-info/PKG-INFO` & `pysma-plus-0.1.4/pysma_plus.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pysma-plus
-Version: 0.1.3
+Version: 0.1.4
 Summary: Library to interface SMA Devices via WebConnect, EnnexOS and Energy Meter Devices
 Home-page: https://github.com/littleyoda/pysma
-Download-URL: https://github.com/littleyoda/pysma/tarball/0.1.3
+Download-URL: https://github.com/littleyoda/pysma/tarball/0.1.4
 Author: Sven Bursch-Osewold, Johann Kellerman and other
 Author-email: Sven Bursch-Osewold <sb_pysma@bursch.com>, Johann Kellerman <kellerza@gmail.com>
 License: The MIT License (MIT)
         
         Copyright (c) 2016 kellerza
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -55,9 +55,20 @@
 * SMA Energy Meter (EMETER-10, EMETER-20) und ### Sunny Home Manager 2.0 (shm2)
 
 
 ## Example usage
 
 See [example.py](./example.py) for a basic usage and tests
 
+## Successfully tested devices
 
+| Bereich | Gerät | Methode |
+|--|--|--|
+| Wechselrichter | Tripower X (STP XX-50)<br>(15,25) | ennexos |
+| Hybrid-Wechselrichter | Sunny Tripower Smart Energy<br>(10.0)  | webconnect |
+| Hybrid-Wechselrichter | Sunny Boy Storage<br>(SBS3.7-10, SBS5.0-10) | webconnect |
+| | | |
+| Energy Meter | Energy Meter 2<br>(EMTER 20) | speedwire |
+| Energy Meter | Sunny Home Manager 2<br>(SHM2) | speedwire |
+| | | |
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pysma-plus-0.1.3/pysma_plus.egg-info/SOURCES.txt` & `pysma-plus-0.1.4/pysma_plus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pysma-plus-0.1.3/pysmaplus/__init__.py` & `pysma-plus-0.1.4/pysmaplus/__init__.py`

 * *Files identical despite different names*

### Comparing `pysma-plus-0.1.3/pysmaplus/const.py` & `pysma-plus-0.1.4/pysmaplus/const.py`

 * *Files identical despite different names*

### Comparing `pysma-plus-0.1.3/pysmaplus/definitions.py` & `pysma-plus-0.1.4/pysmaplus/definitions.py`

 * *Files identical despite different names*

### Comparing `pysma-plus-0.1.3/pysmaplus/helpers.py` & `pysma-plus-0.1.4/pysmaplus/helpers.py`

 * *Files identical despite different names*

### Comparing `pysma-plus-0.1.3/pysmaplus/sensor.py` & `pysma-plus-0.1.4/pysmaplus/sensor.py`

 * *Files identical despite different names*

### Comparing `pysma-plus-0.1.3/pysmaplus/smaennexos.py` & `pysma-plus-0.1.4/pysmaplus/smaennexos.py`

 * *Files 6% similar despite different names*

```diff
@@ -116,15 +116,17 @@
 
     # pylint: disable=too-many-instance-attributes
     _aio_session: ClientSession
     _new_session_data: Optional[dict]
     _url: str
     _token: str
     _authorization_header: str
-
+    _last_parameters: Any
+    _last_measurements: Any
+    _last_device: Any
 
     def __init__(
         self,
         session: ClientSession,
         url: str,
         password: Optional[str],
         group: str,
@@ -209,49 +211,87 @@
                 'username': self._new_session_data["user"],
                 'password': self._new_session_data["pass"],
                 }}
         ret = await self._jsonrequest(loginurl,postdata)
         if "access_token" not in ret:
             raise SmaAuthenticationException(f"Login failed!")
         self._token = ret["access_token"]
-        self._authorization_header = { "Authorization" : "Bearer " + self._token } 
+        self._authorization_header = { "Authorization" : "Bearer " + self._token,
+                                       "Content-Type": "application/json"
+                                       }
         _LOGGER.debug("Login successfull")
         return True
 
-    async def _get_livedata(self) -> Dict:
+    async def _get_parameter(self : str) -> Dict:
+        url = self._url + '/api/v1/parameters/search'
+        postdata = {
+             'data': '{"queryItems":[{"componentId":"IGULD:SELF"}]}',
+             'headers': self._authorization_header
+        }
+        ret = await self._jsonrequest(url, postdata)
+        data = {}
+        if (len(ret) != 1):
+            _LOGGER.warning("Uncommon length of array in parameters request: %d", len(ret))
+
+        for d in ret[0]["values"]:
+            dname = d["channelId"].replace("Parameter.","").replace("[]", "")
+            if "value" in d:
+                v = d["value"]
+                data[dname] = {
+                        "name": dname,
+                        "value": v,
+                        "origname": d["channelId"]
+                    }
+            elif "values" in d:
+                # Split Value-Arrays
+                for idx in range(0, len(d["values"])):
+                    v = d["values"][idx]
+                    idxname = dname + "." + str(idx + 1)
+                    data[idxname] = {
+                            "name": idxname,
+                            "value": v,
+                            "origname": d["channelId"]
+                    }
+            else:
+                # Value current not available // night?
+                # TODO
+                pass
+        return data
+
+    async def _get_livedata(self : str) -> Dict:
         liveurl = self._url + '/api/v1/measurements/live'
         postdata = { 
              'data': '[{"componentId":"IGULD:SELF"}]',
              'headers': self._authorization_header
         }
         ret = await self._jsonrequest(liveurl,postdata)
-        device_sensors = Sensors()
+        self._last_measurements = ret
         data = {}
         for d in ret:
             dname = d["channelId"].replace("Measurement.","").replace("[]", "")
             if "value" in d["values"][0]:
                 v = d["values"][0]["value"]
                 if self._isfloat(v):
                      v = round(v,2)
                 data[dname] = {
                         "name": dname,
                         "value": v,
-                        "origname": d["channelId"] 
+                        "origname": d["channelId"]
                     }
             elif "values" in d["values"][0]:
                 # Split Value-Arrays
                 for idx in range(0, len(d["values"][0]["values"])):
                     v = d["values"][0]["values"][idx]
                     if self._isfloat(v):
                         v = round(v,2)
                     idxname = dname + "." + str(idx + 1)
                     data[idxname] = {
                             "name": idxname,
                             "value": v,
-                            "origname": d["channelId"] 
+                            "origname": d["channelId"]
                     }
             else:
                 # Value current not available // night?
                 # TODO
                 pass
         return data
     
@@ -332,16 +372,25 @@
             dict: dict containing serial, name, type, manufacturer and sw_version
         """
         url = self._url + '/api/v1/plants/Plant:1/devices/IGULD:SELF'
         requestdata = { 
              'headers': self._authorization_header
         }
         dev = await self._jsonrequest(url,requestdata, hdrs.METH_GET)
+        self._last_device = dev
+        self._last_parameters = await self._get_parameter()
         _LOGGER.debug("Found Device: %s", dev)
         device_info = {
             "serial": dev["serial"],
             "name": dev["product"],
             "type": dev["name"],
             "manufacturer": dev["vendor"],
             "sw_version": dev["firmwareVersion"],
         }
         return device_info
+
+    async def get_debug(self) -> Dict:
+        return {
+            "device": self._last_device,
+            "measurements": self._last_measurements,
+            "parameters": self._last_parameters
+        }
```

### Comparing `pysma-plus-0.1.3/pysmaplus/smaspeedwireem.py` & `pysma-plus-0.1.4/pysmaplus/smaspeedwireem.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import base64
 import socket
 import struct
 import asyncio
 import copy
 import logging
 import binascii
 from typing import Any, Dict, Optional
@@ -94,14 +95,15 @@
 
 
 _LOGGER = logging.getLogger(__name__)
 class SMAspeedwireEM(Device):
     """Class to connect to the ennexos based SMA inverters. (e.g. Tripower X Devices)"""
     _sock: socket
     _susyid: Dict[int, Any] = {270: "Energy Meter", 349: "Energy Meter 2", 372: "Sunny Home Manager 2"}
+    _last_packet: bytes = None
 
     def __init__(self):
         """Init SMA connection.
 
         Args:
             session (ClientSession): aiohttp client session
             url (str): Url or IP address of device
@@ -179,15 +181,16 @@
 
         """
         data = None
         tries = 4
         try:
             while tries > 0:
                 a = datetime.datetime.now()
-                data=self._decode(self._sock.recv(608))
+                self._last_packet = self._sock.recv(608)
+                data=self._decode(self._last_packet)
                 b = datetime.datetime.now()
                 if data and (b-a).total_seconds() < 0.1:
                     continue
                 if data:
                     break
                 tries -= 1
         except TimeoutError as e:
@@ -286,7 +289,11 @@
                 obis= "sw_version"
                 pos += 4 + 4
             else:
                 _LOGGER.debug("Unknown packet in speedwire: " + str(mchannel) + " " + str(mvalueindex) + " " + str(mtyp) + " " + str(mtariff))
                 pos += 4 + 4
             data[obis] = value
         return data
+
+    async def get_debug(self) -> Dict:
+        encoded = base64.b64encode(self._last_packet)
+        return { "packet": encoded.decode('ascii')}
```

### Comparing `pysma-plus-0.1.3/pysmaplus/smawebconnect.py` & `pysma-plus-0.1.4/pysmaplus/smawebconnect.py`

 * *Files 1% similar despite different names*

```diff
@@ -464,7 +464,10 @@
                     ]:
                         new_sensor = copy.copy(sensor_definition)
                         new_sensor.key_idx = idx
                         new_sensor.name = f"{sensor_definition.name}_{idx}"
                         device_sensors.add(new_sensor)
 
         return device_sensors
+
+    async def get_debug(self) -> Dict:
+        return {}
```

### Comparing `pysma-plus-0.1.3/setup.py` & `pysma-plus-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 """pysma library setup."""
 from pathlib import Path
 
 from setuptools import setup
 
-VERSION = "0.1.3"
+VERSION = "0.1.4"
 URL = "https://github.com/littleyoda/pysma"
 
 setup(
     name="pysma-plus",
     version=VERSION,
     description="Library to interface SMA Devices via WebConnect, EnnexOS and Energy Meter Devices",
     long_description=Path("README.md").read_text(),
```

### Comparing `pysma-plus-0.1.3/tests/__init__.py` & `pysma-plus-0.1.4/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pysma-plus-0.1.3/tests/test_definitions.py` & `pysma-plus-0.1.4/tests/test_definitions.py`

 * *Files identical despite different names*

### Comparing `pysma-plus-0.1.3/tests/test_init.py` & `pysma-plus-0.1.4/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `pysma-plus-0.1.3/tests/test_sensor.py` & `pysma-plus-0.1.4/tests/test_sensor.py`

 * *Files identical despite different names*

