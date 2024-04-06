# Comparing `tmp/yolink-api-0.4.1.tar.gz` & `tmp/yolink-api-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yolink-api-0.4.1.tar", last modified: Fri Mar 22 11:12:50 2024, max compression
+gzip compressed data, was "yolink-api-0.4.2.tar", last modified: Sat Apr  6 13:22:21 2024, max compression
```

## Comparing `yolink-api-0.4.1.tar` & `yolink-api-0.4.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 11:12:50.614553 yolink-api-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-03-22 11:12:45.000000 yolink-api-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-03-22 11:12:50.614553 yolink-api-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-03-22 11:12:45.000000 yolink-api-0.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-03-22 11:12:45.000000 yolink-api-0.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-22 11:12:50.614553 yolink-api-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      874 2024-03-22 11:12:45.000000 yolink-api-0.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 11:12:50.614553 yolink-api-0.4.1/yolink/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 11:12:45.000000 yolink-api-0.4.1/yolink/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-03-22 11:12:45.000000 yolink-api-0.4.1/yolink/auth_mgr.py
--rw-r--r--   0 runner    (1001) docker     (127)     2841 2024-03-22 11:12:45.000000 yolink-api-0.4.1/yolink/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-03-22 11:12:45.000000 yolink-api-0.4.1/yolink/client_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-03-22 11:12:45.000000 yolink-api-0.4.1/yolink/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-03-22 11:12:45.000000 yolink-api-0.4.1/yolink/device.py
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-03-22 11:12:45.000000 yolink-api-0.4.1/yolink/endpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-03-22 11:12:45.000000 yolink-api-0.4.1/yolink/exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     4218 2024-03-22 11:12:45.000000 yolink-api-0.4.1/yolink/home_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-03-22 11:12:45.000000 yolink-api-0.4.1/yolink/message_listener.py
--rw-r--r--   0 runner    (1001) docker     (127)     2650 2024-03-22 11:12:45.000000 yolink-api-0.4.1/yolink/message_resolver.py
--rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-03-22 11:12:45.000000 yolink-api-0.4.1/yolink/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5654 2024-03-22 11:12:45.000000 yolink-api-0.4.1/yolink/mqtt_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      528 2024-03-22 11:12:45.000000 yolink-api-0.4.1/yolink/outlet_request_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)      949 2024-03-22 11:12:45.000000 yolink-api-0.4.1/yolink/thermostat_request_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3501 2024-03-22 11:12:45.000000 yolink-api-0.4.1/yolink/unit_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 11:12:50.614553 yolink-api-0.4.1/yolink_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-03-22 11:12:50.000000 yolink-api-0.4.1/yolink_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-03-22 11:12:50.000000 yolink-api-0.4.1/yolink_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-22 11:12:50.000000 yolink-api-0.4.1/yolink_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-22 11:12:50.000000 yolink-api-0.4.1/yolink_api.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-03-22 11:12:50.000000 yolink-api-0.4.1/yolink_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-22 11:12:50.000000 yolink-api-0.4.1/yolink_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:22:21.328843 yolink-api-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-06 13:22:18.000000 yolink-api-0.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2440 2024-04-06 13:22:21.328843 yolink-api-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1902 2024-04-06 13:22:18.000000 yolink-api-0.4.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-06 13:22:18.000000 yolink-api-0.4.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 13:22:21.328843 yolink-api-0.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-04-06 13:22:18.000000 yolink-api-0.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:22:21.328843 yolink-api-0.4.2/yolink/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 13:22:18.000000 yolink-api-0.4.2/yolink/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-04-06 13:22:18.000000 yolink-api-0.4.2/yolink/auth_mgr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2841 2024-04-06 13:22:18.000000 yolink-api-0.4.2/yolink/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-06 13:22:18.000000 yolink-api-0.4.2/yolink/client_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-04-06 13:22:18.000000 yolink-api-0.4.2/yolink/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-04-06 13:22:18.000000 yolink-api-0.4.2/yolink/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-06 13:22:18.000000 yolink-api-0.4.2/yolink/endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-06 13:22:18.000000 yolink-api-0.4.2/yolink/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4451 2024-04-06 13:22:18.000000 yolink-api-0.4.2/yolink/home_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-06 13:22:18.000000 yolink-api-0.4.2/yolink/message_listener.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2650 2024-04-06 13:22:18.000000 yolink-api-0.4.2/yolink/message_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-04-06 13:22:18.000000 yolink-api-0.4.2/yolink/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5654 2024-04-06 13:22:18.000000 yolink-api-0.4.2/yolink/mqtt_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-04-06 13:22:18.000000 yolink-api-0.4.2/yolink/outlet_request_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2024-04-06 13:22:18.000000 yolink-api-0.4.2/yolink/thermostat_request_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3501 2024-04-06 13:22:18.000000 yolink-api-0.4.2/yolink/unit_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:22:21.328843 yolink-api-0.4.2/yolink_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2440 2024-04-06 13:22:21.000000 yolink-api-0.4.2/yolink_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-06 13:22:21.000000 yolink-api-0.4.2/yolink_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 13:22:21.000000 yolink-api-0.4.2/yolink_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 13:22:21.000000 yolink-api-0.4.2/yolink_api.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-06 13:22:21.000000 yolink-api-0.4.2/yolink_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-06 13:22:21.000000 yolink-api-0.4.2/yolink_api.egg-info/top_level.txt
```

### Comparing `yolink-api-0.4.1/LICENSE` & `yolink-api-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `yolink-api-0.4.1/setup.py` & `yolink-api-0.4.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name="yolink-api",
-    version="0.4.1",
+    version="0.4.2",
     author="YoSmart",
     description="A library to authenticate with yolink device",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/YoSmart-Inc/yolink-api",
     project_urls={
         "Bug Tracker": "https://github.com/YoSmart-Inc/yolink-api/issues",
```

### Comparing `yolink-api-0.4.1/yolink/auth_mgr.py` & `yolink-api-0.4.2/yolink/auth_mgr.py`

 * *Files identical despite different names*

### Comparing `yolink-api-0.4.1/yolink/client.py` & `yolink-api-0.4.2/yolink/client.py`

 * *Files identical despite different names*

### Comparing `yolink-api-0.4.1/yolink/const.py` & `yolink-api-0.4.2/yolink/const.py`

 * *Files identical despite different names*

### Comparing `yolink-api-0.4.1/yolink/device.py` & `yolink-api-0.4.2/yolink/device.py`

 * *Files identical despite different names*

### Comparing `yolink-api-0.4.1/yolink/endpoint.py` & `yolink-api-0.4.2/yolink/endpoint.py`

 * *Files identical despite different names*

### Comparing `yolink-api-0.4.1/yolink/exception.py` & `yolink-api-0.4.2/yolink/exception.py`

 * *Files identical despite different names*

### Comparing `yolink-api-0.4.1/yolink/home_manager.py` & `yolink-api-0.4.2/yolink/home_manager.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 """YoLink home manager."""
 
 from __future__ import annotations
 import logging
 from typing import Any
 from .auth_mgr import YoLinkAuthMgr
 from .client import YoLinkClient
+from .const import ATTR_DEVICE_WATER_DEPTH_SENSOR
 from .device import YoLinkDevice, YoLinkDeviceMode
 from .exception import YoLinkClientError, YoLinkUnSupportedMethodError
 from .message_listener import MessageListener
 from .model import BRDP
 from .mqtt_client import YoLinkMqttClient
 from .endpoint import Endpoint, Endpoints
 
 _LOGGER = logging.getLogger(__name__)
 
+has_external_data_devices = [ATTR_DEVICE_WATER_DEPTH_SENSOR]
+
 
 class YoLinkHome:
     """YoLink home manager."""
 
     def __init__(self) -> None:
         """Init YoLink Home Manager."""
         self._home_devices: dict[str, YoLinkDevice] = {}
@@ -85,21 +88,23 @@
             url=Endpoints.US.value.url, bsdp={"method": "Home.getDeviceList"}, **kwargs
         )
         for _device in response.data["devices"]:
             _yl_device = YoLinkDevice(YoLinkDeviceMode(**_device), self._http_client)
             self._endpoints[_yl_device.device_endpoint.name] = (
                 _yl_device.device_endpoint
             )
-            try:
-                dev_external_data_resp = await _yl_device.get_external_data()
-                _yl_device.device_attrs = dev_external_data_resp.data.get("extData")
-            except YoLinkUnSupportedMethodError:
-                _LOGGER.debug(
-                    "getExternalData is not supported for: %s", _yl_device.device_type
-                )
+            if _yl_device.device_type in has_external_data_devices:
+                try:
+                    dev_external_data_resp = await _yl_device.get_external_data()
+                    _yl_device.device_attrs = dev_external_data_resp.data.get("extData")
+                except YoLinkUnSupportedMethodError:
+                    _LOGGER.debug(
+                        "getExternalData is not supported for: %s",
+                        _yl_device.device_type,
+                    )
             self._home_devices[_device["deviceId"]] = _yl_device
 
         return self._home_devices
 
     def get_devices(self) -> list[YoLinkDevice]:
         """Get home devices."""
         return self._home_devices.values()
```

### Comparing `yolink-api-0.4.1/yolink/message_resolver.py` & `yolink-api-0.4.2/yolink/message_resolver.py`

 * *Files identical despite different names*

### Comparing `yolink-api-0.4.1/yolink/model.py` & `yolink-api-0.4.2/yolink/model.py`

 * *Files identical despite different names*

### Comparing `yolink-api-0.4.1/yolink/mqtt_client.py` & `yolink-api-0.4.2/yolink/mqtt_client.py`

 * *Files identical despite different names*

### Comparing `yolink-api-0.4.1/yolink/outlet_request_builder.py` & `yolink-api-0.4.2/yolink/outlet_request_builder.py`

 * *Files identical despite different names*

### Comparing `yolink-api-0.4.1/yolink/thermostat_request_builder.py` & `yolink-api-0.4.2/yolink/thermostat_request_builder.py`

 * *Files identical despite different names*

### Comparing `yolink-api-0.4.1/yolink/unit_helper.py` & `yolink-api-0.4.2/yolink/unit_helper.py`

 * *Files identical despite different names*

### Comparing `yolink-api-0.4.1/yolink_api.egg-info/SOURCES.txt` & `yolink-api-0.4.2/yolink_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

