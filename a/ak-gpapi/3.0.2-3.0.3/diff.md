# Comparing `tmp/ak-gpapi-3.0.2.tar.gz` & `tmp/ak-gpapi-3.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ak-gpapi-3.0.2.tar", last modified: Fri Mar 29 04:06:10 2024, max compression
+gzip compressed data, was "ak-gpapi-3.0.3.tar", last modified: Sat Apr  6 06:20:26 2024, max compression
```

## Comparing `ak-gpapi-3.0.2.tar` & `ak-gpapi-3.0.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 04:06:10.544230 ak-gpapi-3.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)    35102 2024-03-29 04:06:02.000000 ak-gpapi-3.0.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-03-29 04:06:02.000000 ak-gpapi-3.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2454 2024-03-29 04:06:10.544230 ak-gpapi-3.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-03-29 04:06:02.000000 ak-gpapi-3.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 04:06:10.544230 ak-gpapi-3.0.2/ak_gpapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2454 2024-03-29 04:06:10.000000 ak-gpapi-3.0.2/ak_gpapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-03-29 04:06:10.000000 ak-gpapi-3.0.2/ak_gpapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 04:06:10.000000 ak-gpapi-3.0.2/ak_gpapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-03-29 04:06:10.000000 ak-gpapi-3.0.2/ak_gpapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-29 04:06:10.000000 ak-gpapi-3.0.2/ak_gpapi.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 04:06:10.544230 ak-gpapi-3.0.2/gpapi/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 04:06:02.000000 ak-gpapi-3.0.2/gpapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10536 2024-03-29 04:06:02.000000 ak-gpapi-3.0.2/gpapi/config.py
--rw-r--r--   0 runner    (1001) docker     (127)   318690 2024-03-29 04:06:02.000000 ak-gpapi-3.0.2/gpapi/device.properties
--rw-r--r--   0 runner    (1001) docker     (127)    31724 2024-03-29 04:06:02.000000 ak-gpapi-3.0.2/gpapi/googleplay.py
--rw-r--r--   0 runner    (1001) docker     (127)   658644 2024-03-29 04:06:08.000000 ak-gpapi-3.0.2/gpapi/googleplay_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-03-29 04:06:02.000000 ak-gpapi-3.0.2/gpapi/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-03-29 04:06:10.548231 ak-gpapi-3.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-03-29 04:06:02.000000 ak-gpapi-3.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 04:06:10.544230 ak-gpapi-3.0.2/test/
--rw-r--r--   0 runner    (1001) docker     (127)     2895 2024-03-29 04:06:02.000000 ak-gpapi-3.0.2/test/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 06:20:26.963580 ak-gpapi-3.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    35102 2024-04-06 06:20:21.000000 ak-gpapi-3.0.3/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-06 06:20:21.000000 ak-gpapi-3.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2454 2024-04-06 06:20:26.963580 ak-gpapi-3.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-04-06 06:20:21.000000 ak-gpapi-3.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 06:20:26.963580 ak-gpapi-3.0.3/ak_gpapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2454 2024-04-06 06:20:26.000000 ak-gpapi-3.0.3/ak_gpapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-06 06:20:26.000000 ak-gpapi-3.0.3/ak_gpapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 06:20:26.000000 ak-gpapi-3.0.3/ak_gpapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-06 06:20:26.000000 ak-gpapi-3.0.3/ak_gpapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-06 06:20:26.000000 ak-gpapi-3.0.3/ak_gpapi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 06:20:26.963580 ak-gpapi-3.0.3/gpapi/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 06:20:21.000000 ak-gpapi-3.0.3/gpapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10536 2024-04-06 06:20:21.000000 ak-gpapi-3.0.3/gpapi/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)   318690 2024-04-06 06:20:21.000000 ak-gpapi-3.0.3/gpapi/device.properties
+-rw-r--r--   0 runner    (1001) docker     (127)    31896 2024-04-06 06:20:21.000000 ak-gpapi-3.0.3/gpapi/googleplay.py
+-rw-r--r--   0 runner    (1001) docker     (127)   658644 2024-04-06 06:20:25.000000 ak-gpapi-3.0.3/gpapi/googleplay_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-04-06 06:20:21.000000 ak-gpapi-3.0.3/gpapi/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-06 06:20:26.967579 ak-gpapi-3.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-04-06 06:20:21.000000 ak-gpapi-3.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 06:20:26.963580 ak-gpapi-3.0.3/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     2895 2024-04-06 06:20:21.000000 ak-gpapi-3.0.3/test/test.py
```

### Comparing `ak-gpapi-3.0.2/LICENSE.md` & `ak-gpapi-3.0.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ak-gpapi-3.0.2/PKG-INFO` & `ak-gpapi-3.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ak-gpapi
-Version: 3.0.2
+Version: 3.0.3
 Summary: Unofficial python api for google play
 Home-page: https://github.com/appknox/googleplay-api
 Author: appknox
 Author-email: engineering@appknox.com
 License: GPL3
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `ak-gpapi-3.0.2/README.md` & `ak-gpapi-3.0.3/README.md`

 * *Files identical despite different names*

### Comparing `ak-gpapi-3.0.2/ak_gpapi.egg-info/PKG-INFO` & `ak-gpapi-3.0.3/ak_gpapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ak-gpapi
-Version: 3.0.2
+Version: 3.0.3
 Summary: Unofficial python api for google play
 Home-page: https://github.com/appknox/googleplay-api
 Author: appknox
 Author-email: engineering@appknox.com
 License: GPL3
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `ak-gpapi-3.0.2/gpapi/config.py` & `ak-gpapi-3.0.3/gpapi/config.py`

 * *Files identical despite different names*

### Comparing `ak-gpapi-3.0.2/gpapi/device.properties` & `ak-gpapi-3.0.3/gpapi/device.properties`

 * *Files identical despite different names*

### Comparing `ak-gpapi-3.0.2/gpapi/googleplay.py` & `ak-gpapi-3.0.3/gpapi/googleplay.py`

 * *Files 1% similar despite different names*

```diff
@@ -222,22 +222,24 @@
         try:
             if response.payload.HasField('uploadDeviceConfigResponse'):
                 self.device_config_token = response.payload.uploadDeviceConfigResponse
                 self.device_config_token = self.device_config_token.uploadDeviceConfigToken
         except ValueError:
             pass
 
-    def login(self, email=None, password=None, gsfId=None, authSubToken=None, returnParams=False):
+    def login(self, email=None, password=None, gsfId=None, authSubToken=None, returnParams=False, verify_auth=True):
         """Login to your Google Account.
         For first time login you should provide:
             * email
             * password
         For the following logins you need to provide:
             * gsfId
-            * authSubToken"""
+            * authSubToken
+        verify_auth=True verifies auth when login with gsfId & authSubToken. checks token sanity by default.
+        """
         if email is not None and password is not None:
             # First time setup, where we obtain an ac2dm token and
             # upload device information
 
             encryptedPass = self.encryptPassword(email, password).decode('utf-8')
             # AC2DM token
             params = self.deviceBuilder.getLoginParams(email, encryptedPass)
@@ -278,16 +280,17 @@
             self.uploadDeviceConfig()
             if returnParams:
                 return self.gsfId, self.authSubToken
         elif gsfId is not None and authSubToken is not None:
             # no need to initialize API
             self.gsfId = gsfId
             self.setAuthSubToken(authSubToken)
-            # check if token is valid with a simple search
-            self.search('drv')
+            if verify_auth:
+                # check if token is valid with a simple search
+                self.search('drv')
         else:
             raise LoginError('Either (email,pass) or (gsfId, authSubToken) is needed')
 
     def getAuthSubToken(self, email, passwd):
         requestParams = self.deviceBuilder.getLoginParams(email, passwd)
         requestParams['service'] = 'androidmarket'
         requestParams['app'] = 'com.android.vending'
```

### Comparing `ak-gpapi-3.0.2/gpapi/googleplay_pb2.py` & `ak-gpapi-3.0.3/gpapi/googleplay_pb2.py`

 * *Files identical despite different names*

### Comparing `ak-gpapi-3.0.2/gpapi/utils.py` & `ak-gpapi-3.0.3/gpapi/utils.py`

 * *Files identical despite different names*

### Comparing `ak-gpapi-3.0.2/setup.py` & `ak-gpapi-3.0.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import subprocess
 import shutil
 
 PROTOC_EXEC = "protoc"
 
 CURRENT_DIR = os.path.abspath( os.path.dirname( __file__ ) )
 
-__VERSION__ = '3.0.2'
+__VERSION__ = '3.0.3'
 
 class ProtobufBuilder(_build):
 
     def run(self):
         # check if protobuf is installed
         exec_path = shutil.which(PROTOC_EXEC)
         if exec_path is None:
```

### Comparing `ak-gpapi-3.0.2/test/test.py` & `ak-gpapi-3.0.3/test/test.py`

 * *Files identical despite different names*

