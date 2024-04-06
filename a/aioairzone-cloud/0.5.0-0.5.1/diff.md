# Comparing `tmp/aioairzone-cloud-0.5.0.tar.gz` & `tmp/aioairzone-cloud-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioairzone-cloud-0.5.0.tar", last modified: Fri Apr  5 08:22:11 2024, max compression
+gzip compressed data, was "aioairzone-cloud-0.5.1.tar", last modified: Sat Apr  6 14:32:25 2024, max compression
```

## Comparing `aioairzone-cloud-0.5.0.tar` & `aioairzone-cloud-0.5.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 noltari   (1000) noltari   (1000)        0 2024-04-05 08:22:11.442738 aioairzone-cloud-0.5.0/
--rw-r--r--   0 noltari   (1000) noltari   (1000)    11357 2024-01-05 18:10:25.000000 aioairzone-cloud-0.5.0/LICENSE
--rw-r--r--   0 noltari   (1000) noltari   (1000)       59 2024-01-05 18:10:25.000000 aioairzone-cloud-0.5.0/MANIFEST.in
--rw-r--r--   0 noltari   (1000) noltari   (1000)     1551 2024-04-05 08:22:11.442738 aioairzone-cloud-0.5.0/PKG-INFO
--rw-r--r--   0 noltari   (1000) noltari   (1000)      746 2024-01-05 18:10:25.000000 aioairzone-cloud-0.5.0/README.md
-drwxr-xr-x   0 noltari   (1000) noltari   (1000)        0 2024-04-05 08:22:11.442738 aioairzone-cloud-0.5.0/aioairzone_cloud/
--rw-r--r--   0 noltari   (1000) noltari   (1000)       33 2024-01-05 18:10:25.000000 aioairzone-cloud-0.5.0/aioairzone_cloud/__init__.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)     3530 2024-04-05 06:43:24.000000 aioairzone-cloud-0.5.0/aioairzone_cloud/aidoo.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)    32279 2024-04-05 08:04:13.000000 aioairzone-cloud-0.5.0/aioairzone_cloud/cloudapi.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)     2777 2024-04-05 06:43:24.000000 aioairzone-cloud-0.5.0/aioairzone_cloud/common.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)    10182 2024-04-05 08:15:56.000000 aioairzone-cloud-0.5.0/aioairzone_cloud/const.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)     8852 2024-04-05 08:10:42.000000 aioairzone-cloud-0.5.0/aioairzone_cloud/device.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)    11288 2024-04-05 07:36:49.000000 aioairzone-cloud-0.5.0/aioairzone_cloud/device_group.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)     3081 2024-03-10 20:15:29.000000 aioairzone-cloud-0.5.0/aioairzone_cloud/entity.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)      807 2024-02-29 06:57:16.000000 aioairzone-cloud-0.5.0/aioairzone_cloud/exceptions.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)      925 2024-04-05 06:43:19.000000 aioairzone-cloud-0.5.0/aioairzone_cloud/group.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)     5368 2024-04-05 07:45:36.000000 aioairzone-cloud-0.5.0/aioairzone_cloud/hotwater.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)    26050 2024-04-05 06:43:24.000000 aioairzone-cloud-0.5.0/aioairzone_cloud/hvac.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)     1821 2024-04-05 06:43:19.000000 aioairzone-cloud-0.5.0/aioairzone_cloud/installation.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)        0 2024-01-05 18:10:25.000000 aioairzone-cloud-0.5.0/aioairzone_cloud/py.typed
--rw-r--r--   0 noltari   (1000) noltari   (1000)     1463 2024-04-05 06:43:19.000000 aioairzone-cloud-0.5.0/aioairzone_cloud/system.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)     2495 2024-02-29 06:57:16.000000 aioairzone-cloud-0.5.0/aioairzone_cloud/token.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)     5948 2024-04-05 06:43:24.000000 aioairzone-cloud-0.5.0/aioairzone_cloud/webserver.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)     8581 2024-04-05 06:43:24.000000 aioairzone-cloud-0.5.0/aioairzone_cloud/websockets.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)     3707 2024-04-05 06:43:24.000000 aioairzone-cloud-0.5.0/aioairzone_cloud/zone.py
-drwxr-xr-x   0 noltari   (1000) noltari   (1000)        0 2024-04-05 08:22:11.442738 aioairzone-cloud-0.5.0/aioairzone_cloud.egg-info/
--rw-r--r--   0 noltari   (1000) noltari   (1000)     1551 2024-04-05 08:22:11.000000 aioairzone-cloud-0.5.0/aioairzone_cloud.egg-info/PKG-INFO
--rw-r--r--   0 noltari   (1000) noltari   (1000)      832 2024-04-05 08:22:11.000000 aioairzone-cloud-0.5.0/aioairzone_cloud.egg-info/SOURCES.txt
--rw-r--r--   0 noltari   (1000) noltari   (1000)        1 2024-04-05 08:22:11.000000 aioairzone-cloud-0.5.0/aioairzone_cloud.egg-info/dependency_links.txt
--rw-r--r--   0 noltari   (1000) noltari   (1000)        1 2024-04-05 08:22:11.000000 aioairzone-cloud-0.5.0/aioairzone_cloud.egg-info/not-zip-safe
--rw-r--r--   0 noltari   (1000) noltari   (1000)        8 2024-04-05 08:22:11.000000 aioairzone-cloud-0.5.0/aioairzone_cloud.egg-info/requires.txt
--rw-r--r--   0 noltari   (1000) noltari   (1000)       17 2024-04-05 08:22:11.000000 aioairzone-cloud-0.5.0/aioairzone_cloud.egg-info/top_level.txt
--rw-r--r--   0 noltari   (1000) noltari   (1000)     2327 2024-04-05 08:21:31.000000 aioairzone-cloud-0.5.0/pyproject.toml
--rw-r--r--   0 noltari   (1000) noltari   (1000)       77 2024-01-05 18:10:25.000000 aioairzone-cloud-0.5.0/requirements.txt
--rw-r--r--   0 noltari   (1000) noltari   (1000)       38 2024-04-05 08:22:11.442738 aioairzone-cloud-0.5.0/setup.cfg
+drwxr-xr-x   0 noltari   (1000) noltari   (1000)        0 2024-04-06 14:32:25.766481 aioairzone-cloud-0.5.1/
+-rw-r--r--   0 noltari   (1000) noltari   (1000)    11357 2023-12-27 17:30:29.000000 aioairzone-cloud-0.5.1/LICENSE
+-rw-r--r--   0 noltari   (1000) noltari   (1000)       59 2023-12-27 17:30:29.000000 aioairzone-cloud-0.5.1/MANIFEST.in
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     1551 2024-04-06 14:32:25.766481 aioairzone-cloud-0.5.1/PKG-INFO
+-rw-r--r--   0 noltari   (1000) noltari   (1000)      746 2023-12-27 17:30:29.000000 aioairzone-cloud-0.5.1/README.md
+drwxr-xr-x   0 noltari   (1000) noltari   (1000)        0 2024-04-06 14:32:25.766481 aioairzone-cloud-0.5.1/aioairzone_cloud/
+-rw-r--r--   0 noltari   (1000) noltari   (1000)       33 2023-12-27 17:30:29.000000 aioairzone-cloud-0.5.1/aioairzone_cloud/__init__.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     3530 2024-04-04 17:05:15.000000 aioairzone-cloud-0.5.1/aioairzone_cloud/aidoo.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)    32279 2024-04-06 13:58:52.000000 aioairzone-cloud-0.5.1/aioairzone_cloud/cloudapi.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     3020 2024-04-06 14:00:41.000000 aioairzone-cloud-0.5.1/aioairzone_cloud/common.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)    10264 2024-04-06 13:59:56.000000 aioairzone-cloud-0.5.1/aioairzone_cloud/const.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     8852 2024-04-06 13:58:52.000000 aioairzone-cloud-0.5.1/aioairzone_cloud/device.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)    11288 2024-04-06 13:58:52.000000 aioairzone-cloud-0.5.1/aioairzone_cloud/device_group.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     3081 2024-02-28 14:34:38.000000 aioairzone-cloud-0.5.1/aioairzone_cloud/entity.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)      807 2024-02-28 08:54:11.000000 aioairzone-cloud-0.5.1/aioairzone_cloud/exceptions.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)      925 2024-04-03 16:08:52.000000 aioairzone-cloud-0.5.1/aioairzone_cloud/group.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     6161 2024-04-06 14:25:23.000000 aioairzone-cloud-0.5.1/aioairzone_cloud/hotwater.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)    26050 2024-04-04 17:06:10.000000 aioairzone-cloud-0.5.1/aioairzone_cloud/hvac.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     1821 2024-04-03 16:08:59.000000 aioairzone-cloud-0.5.1/aioairzone_cloud/installation.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)        0 2023-12-27 17:30:29.000000 aioairzone-cloud-0.5.1/aioairzone_cloud/py.typed
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     1463 2024-04-03 16:09:19.000000 aioairzone-cloud-0.5.1/aioairzone_cloud/system.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     2495 2024-02-28 12:49:43.000000 aioairzone-cloud-0.5.1/aioairzone_cloud/token.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     5948 2024-04-03 16:34:41.000000 aioairzone-cloud-0.5.1/aioairzone_cloud/webserver.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     8581 2024-04-03 16:04:15.000000 aioairzone-cloud-0.5.1/aioairzone_cloud/websockets.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     3707 2024-04-04 17:06:28.000000 aioairzone-cloud-0.5.1/aioairzone_cloud/zone.py
+drwxr-xr-x   0 noltari   (1000) noltari   (1000)        0 2024-04-06 14:32:25.766481 aioairzone-cloud-0.5.1/aioairzone_cloud.egg-info/
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     1551 2024-04-06 14:32:25.000000 aioairzone-cloud-0.5.1/aioairzone_cloud.egg-info/PKG-INFO
+-rw-r--r--   0 noltari   (1000) noltari   (1000)      832 2024-04-06 14:32:25.000000 aioairzone-cloud-0.5.1/aioairzone_cloud.egg-info/SOURCES.txt
+-rw-r--r--   0 noltari   (1000) noltari   (1000)        1 2024-04-06 14:32:25.000000 aioairzone-cloud-0.5.1/aioairzone_cloud.egg-info/dependency_links.txt
+-rw-r--r--   0 noltari   (1000) noltari   (1000)        1 2024-04-06 14:32:25.000000 aioairzone-cloud-0.5.1/aioairzone_cloud.egg-info/not-zip-safe
+-rw-r--r--   0 noltari   (1000) noltari   (1000)        8 2024-04-06 14:32:25.000000 aioairzone-cloud-0.5.1/aioairzone_cloud.egg-info/requires.txt
+-rw-r--r--   0 noltari   (1000) noltari   (1000)       17 2024-04-06 14:32:25.000000 aioairzone-cloud-0.5.1/aioairzone_cloud.egg-info/top_level.txt
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     2327 2024-04-06 14:31:15.000000 aioairzone-cloud-0.5.1/pyproject.toml
+-rw-r--r--   0 noltari   (1000) noltari   (1000)       77 2023-12-27 17:30:29.000000 aioairzone-cloud-0.5.1/requirements.txt
+-rw-r--r--   0 noltari   (1000) noltari   (1000)       38 2024-04-06 14:32:25.766481 aioairzone-cloud-0.5.1/setup.cfg
```

### Comparing `aioairzone-cloud-0.5.0/LICENSE` & `aioairzone-cloud-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.5.0/PKG-INFO` & `aioairzone-cloud-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioairzone-cloud
-Version: 0.5.0
+Version: 0.5.1
 Summary: Library to control Airzone Cloud devices
 Author-email: Álvaro Fernández Rojas <noltari@gmail.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/Noltari/aioairzone-cloud
 Project-URL: Bug Tracker, https://github.com/Noltari/aioairzone-cloud/issues
 Keywords: airzone,cloud,hvac,home
 Platform: any
```

### Comparing `aioairzone-cloud-0.5.0/README.md` & `aioairzone-cloud-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.5.0/aioairzone_cloud/aidoo.py` & `aioairzone-cloud-0.5.1/aioairzone_cloud/aidoo.py`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.5.0/aioairzone_cloud/cloudapi.py` & `aioairzone-cloud-0.5.1/aioairzone_cloud/cloudapi.py`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.5.0/aioairzone_cloud/common.py` & `aioairzone-cloud-0.5.1/aioairzone_cloud/common.py`

 * *Files 12% similar despite different names*

```diff
@@ -26,14 +26,28 @@
     AUTO = "auto"
 
     @classmethod
     def _missing_(cls, value: Any) -> AirQualityMode:
         return cls.UNKNOWN
 
 
+class HotWaterOperation(IntEnum):
+    """Airzone Cloud Hot Water operations."""
+
+    UNKNOWN = -1
+
+    Off = 0
+    On = 1
+    Powerful = 2
+
+    @classmethod
+    def _missing_(cls, value: Any) -> HotWaterOperation:
+        return cls.UNKNOWN
+
+
 class OperationAction(IntEnum):
     """Airzone Cloud operation actions."""
 
     COOLING = 1
     DRYING = 2
     FAN = 3
     HEATING = 4
```

### Comparing `aioairzone-cloud-0.5.0/aioairzone_cloud/const.py` & `aioairzone-cloud-0.5.1/aioairzone_cloud/const.py`

 * *Files 0% similar despite different names*

```diff
@@ -156,14 +156,16 @@
 AZD_MASTER: Final[str] = "master"
 AZD_MODE: Final[str] = "mode"
 AZD_MODE_AUTO: Final[str] = "mode-auto"
 AZD_MODES: Final[str] = "modes"
 AZD_NAME: Final[str] = "name"
 AZD_NUM_DEVICES: Final[str] = "num-devices"
 AZD_NUM_GROUPS: Final[str] = "num-groups"
+AZD_OPERATION: Final[str] = "operation"
+AZD_OPERATIONS: Final[str] = "operations"
 AZD_POWER: Final[str] = "power"
 AZD_POWER_MODE: Final[str] = "power-mode"
 AZD_PROBLEMS: Final[str] = "problems"
 AZD_SPEED: Final[str] = "speed"
 AZD_SPEEDS: Final[str] = "speeds"
 AZD_SPEED_TYPE: Final[str] = "speed-type"
 AZD_SYSTEM: Final[str] = "system"
```

### Comparing `aioairzone-cloud-0.5.0/aioairzone_cloud/device.py` & `aioairzone-cloud-0.5.1/aioairzone_cloud/device.py`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.5.0/aioairzone_cloud/device_group.py` & `aioairzone-cloud-0.5.1/aioairzone_cloud/device_group.py`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.5.0/aioairzone_cloud/entity.py` & `aioairzone-cloud-0.5.1/aioairzone_cloud/entity.py`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.5.0/aioairzone_cloud/exceptions.py` & `aioairzone-cloud-0.5.1/aioairzone_cloud/exceptions.py`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.5.0/aioairzone_cloud/group.py` & `aioairzone-cloud-0.5.1/aioairzone_cloud/group.py`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.5.0/aioairzone_cloud/hotwater.py` & `aioairzone-cloud-0.5.1/aioairzone_cloud/hotwater.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 """Airzone Cloud API Domestic Hot Water."""
 
 from __future__ import annotations
 
 from typing import Any
 
-from .common import parse_bool, parse_float, parse_int
+from .common import HotWaterOperation, parse_bool, parse_float, parse_int
 from .const import (
     API_ACTIVE,
     API_CELSIUS,
     API_DEFAULT_TEMP_STEP_ACS,
     API_POWER,
     API_POWERFUL_MODE,
     API_RANGE_SP_MAX_ACS,
     API_RANGE_SP_MIN_ACS,
     API_SETPOINT,
     API_STEP,
     API_TANK_TEMP,
     API_VALUE,
     AZD_ACTIVE,
+    AZD_OPERATION,
+    AZD_OPERATIONS,
     AZD_POWER,
     AZD_POWER_MODE,
     AZD_TEMP,
     AZD_TEMP_SET,
     AZD_TEMP_SET_MAX,
     AZD_TEMP_SET_MIN,
     AZD_TEMP_STEP,
@@ -34,28 +36,30 @@
     """Airzone Cloud Domestic Hot Water device."""
 
     def __init__(self, inst_id: str, ws_id: str, device_data: dict[str, Any]):
         """Airzone Cloud DHW device init."""
         super().__init__(inst_id, ws_id, device_data)
 
         self.active: bool | None = None
-        self.name: str = "DHW"
+        self.name: str = "Airzone Cloud DHW"
         self.power: bool | None = None
         self.power_mode: bool | None = None
         self.temp_set_max: int | None = None
         self.temp_set_min: int | None = None
         self.temp_set: int | None = None
         self.temp: float | None = None
         self.temp_step: int | None = None
 
     def data(self) -> dict[str, Any]:
         """Return DHW device data."""
         data = super().data()
 
         data[AZD_ACTIVE] = self.get_active()
+        data[AZD_OPERATION] = self.get_operation()
+        data[AZD_OPERATIONS] = self.get_operations()
         data[AZD_POWER] = self.get_power()
         data[AZD_TEMP] = self.get_temperature()
         data[AZD_TEMP_SET] = self.get_temp_set()
         data[AZD_TEMP_SET_MAX] = self.get_temp_set_max()
         data[AZD_TEMP_SET_MIN] = self.get_temp_set_min()
         data[AZD_TEMP_STEP] = self.get_temp_step()
 
@@ -65,14 +69,32 @@
 
         return data
 
     def get_active(self) -> bool | None:
         """Return DHW device active status."""
         return self.active
 
+    def get_operation(self) -> HotWaterOperation:
+        """Return DHW current operation."""
+        if self.get_power():
+            if self.get_power_mode():
+                return HotWaterOperation.Powerful
+            return HotWaterOperation.On
+        return HotWaterOperation.Off
+
+    def get_operations(self) -> list[HotWaterOperation]:
+        """Return DHW operation list."""
+        operations = [
+            HotWaterOperation.Off,
+            HotWaterOperation.On,
+        ]
+        if self.get_power_mode() is not None:
+            operations += [HotWaterOperation.Powerful]
+        return operations
+
     def get_power(self) -> bool | None:
         """Return DHW device power."""
         return self.power
 
     def get_power_mode(self) -> bool | None:
         """Return DHW device power_mode."""
         return self.power_mode
```

### Comparing `aioairzone-cloud-0.5.0/aioairzone_cloud/hvac.py` & `aioairzone-cloud-0.5.1/aioairzone_cloud/hvac.py`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.5.0/aioairzone_cloud/installation.py` & `aioairzone-cloud-0.5.1/aioairzone_cloud/installation.py`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.5.0/aioairzone_cloud/system.py` & `aioairzone-cloud-0.5.1/aioairzone_cloud/system.py`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.5.0/aioairzone_cloud/token.py` & `aioairzone-cloud-0.5.1/aioairzone_cloud/token.py`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.5.0/aioairzone_cloud/webserver.py` & `aioairzone-cloud-0.5.1/aioairzone_cloud/webserver.py`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.5.0/aioairzone_cloud/websockets.py` & `aioairzone-cloud-0.5.1/aioairzone_cloud/websockets.py`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.5.0/aioairzone_cloud/zone.py` & `aioairzone-cloud-0.5.1/aioairzone_cloud/zone.py`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.5.0/aioairzone_cloud.egg-info/PKG-INFO` & `aioairzone-cloud-0.5.1/aioairzone_cloud.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioairzone-cloud
-Version: 0.5.0
+Version: 0.5.1
 Summary: Library to control Airzone Cloud devices
 Author-email: Álvaro Fernández Rojas <noltari@gmail.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/Noltari/aioairzone-cloud
 Project-URL: Bug Tracker, https://github.com/Noltari/aioairzone-cloud/issues
 Keywords: airzone,cloud,hvac,home
 Platform: any
```

### Comparing `aioairzone-cloud-0.5.0/aioairzone_cloud.egg-info/SOURCES.txt` & `aioairzone-cloud-0.5.1/aioairzone_cloud.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.5.0/pyproject.toml` & `aioairzone-cloud-0.5.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "aioairzone-cloud"
-version = "0.5.0"
+version = "0.5.1"
 description = "Library to control Airzone Cloud devices"
 readme = "README.md"
 requires-python = ">=3.11"
 license = {text = "Apache-2.0"}
 keywords = ["airzone", "cloud", "hvac", "home"] 
 authors = [
   {name = "Álvaro Fernández Rojas", email = "noltari@gmail.com" }
```

