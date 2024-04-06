# Comparing `tmp/UofA_BAJA_2023-2024-0.1.5.tar.gz` & `tmp/UofA_BAJA_2023-2024-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "UofA_BAJA_2023-2024-0.1.5.tar", last modified: Sun Mar 31 16:55:43 2024, max compression
+gzip compressed data, was "UofA_BAJA_2023-2024-0.1.6.tar", last modified: Sat Apr  6 02:03:13 2024, max compression
```

## Comparing `UofA_BAJA_2023-2024-0.1.5.tar` & `UofA_BAJA_2023-2024-0.1.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-03-31 16:55:43.262802 UofA_BAJA_2023-2024-0.1.5/
--rw-rw-rw-   0        0        0     1091 2024-03-31 06:55:58.000000 UofA_BAJA_2023-2024-0.1.5/LICENSE
--rw-rw-rw-   0        0        0      979 2024-03-31 16:55:43.261802 UofA_BAJA_2023-2024-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0      508 2024-03-31 06:58:30.000000 UofA_BAJA_2023-2024-0.1.5/README.md
--rw-rw-rw-   0        0        0      463 2024-03-31 16:55:24.000000 UofA_BAJA_2023-2024-0.1.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-31 16:55:43.262802 UofA_BAJA_2023-2024-0.1.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-03-31 16:55:43.229800 UofA_BAJA_2023-2024-0.1.5/src/
-drwxrwxrwx   0        0        0        0 2024-03-31 16:55:43.259800 UofA_BAJA_2023-2024-0.1.5/src/UofA_BAJA_2023_2024.egg-info/
--rw-rw-rw-   0        0        0      979 2024-03-31 16:55:43.000000 UofA_BAJA_2023-2024-0.1.5/src/UofA_BAJA_2023_2024.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      410 2024-03-31 16:55:43.000000 UofA_BAJA_2023-2024-0.1.5/src/UofA_BAJA_2023_2024.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-31 16:55:43.000000 UofA_BAJA_2023-2024-0.1.5/src/UofA_BAJA_2023_2024.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2024-03-31 16:55:43.000000 UofA_BAJA_2023-2024-0.1.5/src/UofA_BAJA_2023_2024.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-03-31 16:55:43.257799 UofA_BAJA_2023-2024-0.1.5/src/UofA_BAJA_2023_2024_common/
--rw-rw-rw-   0        0        0      335 2024-03-31 08:16:37.000000 UofA_BAJA_2023-2024-0.1.5/src/UofA_BAJA_2023_2024_common/Messages.py
--rw-rw-rw-   0        0        0     7255 2024-03-31 16:46:32.000000 UofA_BAJA_2023-2024-0.1.5/src/UofA_BAJA_2023_2024_common/SerialDevices.py
--rw-rw-rw-   0        0        0        0 2024-03-31 07:40:48.000000 UofA_BAJA_2023-2024-0.1.5/src/UofA_BAJA_2023_2024_common/__init__.py
--rw-rw-rw-   0        0        0     1121 2024-03-31 16:55:16.000000 UofA_BAJA_2023-2024-0.1.5/src/UofA_BAJA_2023_2024_common/enums.py
--rw-rw-rw-   0        0        0        0 2024-03-31 06:52:51.000000 UofA_BAJA_2023-2024-0.1.5/src/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-06 02:03:13.692269 UofA_BAJA_2023-2024-0.1.6/
+-rw-rw-rw-   0        0        0     1091 2024-04-02 04:55:41.000000 UofA_BAJA_2023-2024-0.1.6/LICENSE
+-rw-rw-rw-   0        0        0      979 2024-04-06 02:03:13.690275 UofA_BAJA_2023-2024-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0      508 2024-04-02 04:55:41.000000 UofA_BAJA_2023-2024-0.1.6/README.md
+-rw-rw-rw-   0        0        0      463 2024-04-06 02:02:44.000000 UofA_BAJA_2023-2024-0.1.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-06 02:03:13.692269 UofA_BAJA_2023-2024-0.1.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-06 02:03:13.658270 UofA_BAJA_2023-2024-0.1.6/src/
+drwxrwxrwx   0        0        0        0 2024-04-06 02:03:13.688270 UofA_BAJA_2023-2024-0.1.6/src/UofA_BAJA_2023_2024.egg-info/
+-rw-rw-rw-   0        0        0      979 2024-04-06 02:03:13.000000 UofA_BAJA_2023-2024-0.1.6/src/UofA_BAJA_2023_2024.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      410 2024-04-06 02:03:13.000000 UofA_BAJA_2023-2024-0.1.6/src/UofA_BAJA_2023_2024.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-06 02:03:13.000000 UofA_BAJA_2023-2024-0.1.6/src/UofA_BAJA_2023_2024.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2024-04-06 02:03:13.000000 UofA_BAJA_2023-2024-0.1.6/src/UofA_BAJA_2023_2024.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-06 02:03:13.686274 UofA_BAJA_2023-2024-0.1.6/src/UofA_BAJA_2023_2024_common/
+-rw-rw-rw-   0        0        0      335 2024-04-02 04:55:41.000000 UofA_BAJA_2023-2024-0.1.6/src/UofA_BAJA_2023_2024_common/Messages.py
+-rw-rw-rw-   0        0        0     7255 2024-04-02 04:55:41.000000 UofA_BAJA_2023-2024-0.1.6/src/UofA_BAJA_2023_2024_common/SerialDevices.py
+-rw-rw-rw-   0        0        0        0 2024-04-02 04:55:41.000000 UofA_BAJA_2023-2024-0.1.6/src/UofA_BAJA_2023_2024_common/__init__.py
+-rw-rw-rw-   0        0        0     1111 2024-04-06 02:00:51.000000 UofA_BAJA_2023-2024-0.1.6/src/UofA_BAJA_2023_2024_common/enums.py
+-rw-rw-rw-   0        0        0        0 2024-04-02 04:55:41.000000 UofA_BAJA_2023-2024-0.1.6/src/__init__.py
```

### Comparing `UofA_BAJA_2023-2024-0.1.5/LICENSE` & `UofA_BAJA_2023-2024-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `UofA_BAJA_2023-2024-0.1.5/PKG-INFO` & `UofA_BAJA_2023-2024-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UofA_BAJA_2023-2024
-Version: 0.1.5
+Version: 0.1.6
 Summary: packages for the UofA Baja team
 Author-email: Alex Romero <bix.romero@gmail.com>
 Project-URL: Homepage, https://github.com/UofA-BAJA/2023-2024-Firmware
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `UofA_BAJA_2023-2024-0.1.5/src/UofA_BAJA_2023_2024.egg-info/PKG-INFO` & `UofA_BAJA_2023-2024-0.1.6/src/UofA_BAJA_2023_2024.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UofA_BAJA_2023-2024
-Version: 0.1.5
+Version: 0.1.6
 Summary: packages for the UofA Baja team
 Author-email: Alex Romero <bix.romero@gmail.com>
 Project-URL: Homepage, https://github.com/UofA-BAJA/2023-2024-Firmware
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `UofA_BAJA_2023-2024-0.1.5/src/UofA_BAJA_2023_2024_common/SerialDevices.py` & `UofA_BAJA_2023-2024-0.1.6/src/UofA_BAJA_2023_2024_common/SerialDevices.py`

 * *Files identical despite different names*

### Comparing `UofA_BAJA_2023-2024-0.1.5/src/UofA_BAJA_2023_2024_common/enums.py` & `UofA_BAJA_2023-2024-0.1.6/src/UofA_BAJA_2023_2024_common/enums.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 class ModuleTypes:
     IMU = "IMU"
     RPM_FRONT = "RPM_FRONT"
     RPM_REAR = "RPM_REAR"
     RPM_ENGINE = "RPM_ENGINE"
-    BRAK_PRESSURE = "BRK"
+    BRK = "BRK"
     STEER = "STEER"
     PEDAL_ANGLE = "PEDAL"
     LORA_PI = "LORA_PI"
     LORA_PIT = "LORA_PIT"
 
 class Commands:
     BEGIN = "BEGIN"
```

