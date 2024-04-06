# Comparing `tmp/apsystems_ez1-1.2.0.tar.gz` & `tmp/apsystems_ez1-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apsystems_ez1-1.2.0.tar", max compression
+gzip compressed data, was "apsystems_ez1-1.3.0.tar", max compression
```

## Comparing `apsystems_ez1-1.2.0.tar` & `apsystems_ez1-1.3.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    12910 2024-03-29 19:25:22.724710 apsystems_ez1-1.2.0/APsystemsEZ1/__init__.py
--rw-r--r--   0        0        0     1073 2024-03-29 19:25:22.724710 apsystems_ez1-1.2.0/LICENSE
--rw-r--r--   0        0        0    12345 2024-03-29 19:25:22.724710 apsystems_ez1-1.2.0/README.md
--rw-r--r--   0        0        0      731 2024-03-29 19:25:22.740710 apsystems_ez1-1.2.0/pyproject.toml
--rw-r--r--   0        0        0    12858 1970-01-01 00:00:00.000000 apsystems_ez1-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0    13592 2024-04-06 15:37:54.426551 apsystems_ez1-1.3.0/APsystemsEZ1/__init__.py
+-rw-r--r--   0        0        0     1073 2024-04-06 15:37:54.426551 apsystems_ez1-1.3.0/LICENSE
+-rw-r--r--   0        0        0    12345 2024-04-06 15:37:54.426551 apsystems_ez1-1.3.0/README.md
+-rw-r--r--   0        0        0      731 2024-04-06 15:37:54.442552 apsystems_ez1-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0    12858 1970-01-01 00:00:00.000000 apsystems_ez1-1.3.0/PKG-INFO
```

### Comparing `apsystems_ez1-1.2.0/APsystemsEZ1/__init__.py` & `apsystems_ez1-1.3.0/APsystemsEZ1/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,14 +6,18 @@
 
 
 class Status(IntEnum):
     normal = 0
     alarm = 1
 
 
+class InverterReturnedError(Exception):
+    pass
+
+
 @dataclass
 class ReturnDeviceInfo:
     deviceId: str
     devVer: str
     ssid: str
     ipAddr: str
     minPower: int
@@ -40,44 +44,57 @@
 
 class APsystemsEZ1M:
     """This class represents an EZ1 Microinverter and provides methods to interact with it
     over a network. The class allows for getting and setting various device parameters like
     power status, alarm information, device information, and power limits.
     """
 
-    def __init__(self, ip_address: str, port: int = 8050, timeout: int = 10, session: ClientSession| None = None):
+    def __init__(self, ip_address: str, port: int = 8050, timeout: int = 10, session: ClientSession | None = None):
         """
         Initializes a new instance of the EZ1Microinverter class with the specified IP address
         and port.
 
         :param ip_address: The IP address of the EZ1 Microinverter.
         :param port: The port on which the microinverter's server is running. Default is 8050.
         :param timeout: The timeout for all requests. The default of 10 seconds should be plenty.
         """
         self.base_url = f"http://{ip_address}:{port}"
         self.timeout = timeout
-        if session is None:
-            session = ClientSession()
         self.session = session
 
-    async def _request(self, endpoint: str) -> dict | None:
+    async def _request(self, endpoint: str, retry: bool | None = True) -> dict | None:
         """
         A private method to send HTTP requests to the specified endpoint of the microinverter.
         This method is used internally by other class methods to perform GET or POST requests.
 
         :param endpoint: The API endpoint to make the request to.
 
         :return: The JSON response from the microinverter as a dictionary.
         :raises: Prints an error message if the HTTP request fails for any reason.
         """
         url = f"{self.base_url}/{endpoint}"
-        async with self.session.get(url, timeout=self.timeout) as resp:
-            if not resp.ok:
+        if self.session is None:
+            ses = ClientSession()
+        else:
+            ses = self.session
+        async with ses.get(url, timeout=self.timeout) as resp:
+            if resp.status != 200:
                 raise HttpBadRequest(f"HTTP Error: {resp.status}")
-            return await resp.json()
+            data = await resp.json()
+            if data["message"] == "SUCCESS":
+                # Close if session created on per-execution base
+                if self.session is None:
+                    await ses.close()
+                return data
+            # Close if session created on per-execution base
+            if self.session is None:
+                await ses.close()
+            if retry:  # Re-run request when the inverter returned failed because of unknown reason
+                return await self._request(endpoint, retry=False)
+            raise InverterReturnedError
 
     async def get_device_info(self) -> ReturnDeviceInfo | None:
         """
         Retrieves detailed information about the device. This method sends a request to the
         "getDeviceInfo" endpoint and returns a dictionary containing various details about the device.
 
         The returned data includes the device ID, device version, the SSID it is connected to, its IP
@@ -249,15 +266,15 @@
 
         :return: 0/normal when on, 1/alarm when off
         """
         response = await self._request("getOnOff")
         return Status(int(response["data"]["status"])) if response else None
 
     async def set_device_power_status(
-        self, power_status: Status | None
+            self, power_status: Status | None
     ) -> Status | None:
         """
         Sets the power status of the device to either on or off. This method sends a request to the
         "setOnOff" endpoint with a specified power status parameter. The power status accepts multiple
         string representations: '0' or 'ON' to start the inverter, and '1', 'SLEEP', or 'OFF' to stop
         the inverter.
```

### Comparing `apsystems_ez1-1.2.0/LICENSE` & `apsystems_ez1-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `apsystems_ez1-1.2.0/README.md` & `apsystems_ez1-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `apsystems_ez1-1.2.0/pyproject.toml` & `apsystems_ez1-1.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "apsystems-ez1"
-version = "1.2.0"
+version = "1.3.0"
 description = "The APsystems EZ1 Python library offers a streamlined interface for interacting with the local API of APsystems EZ1 Microinverters."
 authors = ["Sonnenladen GmbH <l.tiedt@sonnenladen.de>"]
 readme = "README.md"
 
 packages = [
     { include = "APsystemsEZ1" },
     { include = "APsystemsEZ1/**/*.py" },
```

### Comparing `apsystems_ez1-1.2.0/PKG-INFO` & `apsystems_ez1-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apsystems-ez1
-Version: 1.2.0
+Version: 1.3.0
 Summary: The APsystems EZ1 Python library offers a streamlined interface for interacting with the local API of APsystems EZ1 Microinverters.
 Author: Sonnenladen GmbH
 Author-email: l.tiedt@sonnenladen.de
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: apsystems-ez1 Version: 1.2.0 Summary: The APsystems
+Metadata-Version: 2.1 Name: apsystems-ez1 Version: 1.3.0 Summary: The APsystems
 EZ1 Python library offers a streamlined interface for interacting with the
 local API of APsystems EZ1 Microinverters. Author: Sonnenladen GmbH Author-
 email: l.tiedt@sonnenladen.de Requires-Python: >=3.11,<4.0 Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.11 Classifier: Programming Language :: Python :: 3.12 Requires-Dist:
 aiohttp (>=3,<4) Description-Content-Type: text/markdown # APsystems EZ1 -
 Python Library ## Overview The APsystems EZ1 Python library can be used to
```

