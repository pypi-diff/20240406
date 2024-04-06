# Comparing `tmp/ynca-5.8.0.tar.gz` & `tmp/ynca-5.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ynca-5.8.0.tar", last modified: Thu Jun  8 19:43:19 2023, max compression
+gzip compressed data, was "ynca-5.9.0.tar", last modified: Sat Oct  7 18:39:57 2023, max compression
```

## Comparing `ynca-5.8.0.tar` & `ynca-5.9.0.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:43:19.105356 ynca-5.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-06-08 19:43:09.000000 ynca-5.8.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-08 19:43:09.000000 ynca-5.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5421 2023-06-08 19:43:19.105356 ynca-5.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4719 2023-06-08 19:43:09.000000 ynca-5.8.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-08 19:43:19.105356 ynca-5.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4041 2023-06-08 19:43:09.000000 ynca-5.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:43:19.101356 ynca-5.8.0/ynca/
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-06-08 19:43:09.000000 ynca-5.8.0/ynca/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12068 2023-06-08 19:43:09.000000 ynca-5.8.0/ynca/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     9003 2023-06-08 19:43:09.000000 ynca-5.8.0/ynca/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-06-08 19:43:09.000000 ynca-5.8.0/ynca/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3479 2023-06-08 19:43:09.000000 ynca-5.8.0/ynca/converters.py
--rw-r--r--   0 runner    (1001) docker     (123)    10241 2023-06-08 19:43:09.000000 ynca-5.8.0/ynca/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-06-08 19:43:09.000000 ynca-5.8.0/ynca/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     4585 2023-06-08 19:43:09.000000 ynca-5.8.0/ynca/function.py
--rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-06-08 19:43:09.000000 ynca-5.8.0/ynca/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3356 2023-06-08 19:43:09.000000 ynca-5.8.0/ynca/modelinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 19:43:09.000000 ynca-5.8.0/ynca/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    14889 2023-06-08 19:43:09.000000 ynca-5.8.0/ynca/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     5868 2023-06-08 19:43:09.000000 ynca-5.8.0/ynca/subunit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:43:19.105356 ynca-5.8.0/ynca/subunits/
--rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-06-08 19:43:09.000000 ynca-5.8.0/ynca/subunits/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-08 19:43:09.000000 ynca-5.8.0/ynca/subunits/airplay.py
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-08 19:43:09.000000 ynca-5.8.0/ynca/subunits/bt.py
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-06-08 19:43:09.000000 ynca-5.8.0/ynca/subunits/dab.py
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-08 19:43:09.000000 ynca-5.8.0/ynca/subunits/ipod.py
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-08 19:43:09.000000 ynca-5.8.0/ynca/subunits/ipodusb.py
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-08 19:43:09.000000 ynca-5.8.0/ynca/subunits/napster.py
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-06-08 19:43:09.000000 ynca-5.8.0/ynca/subunits/netradio.py
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-06-08 19:43:09.000000 ynca-5.8.0/ynca/subunits/pandora.py
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-08 19:43:09.000000 ynca-5.8.0/ynca/subunits/pc.py
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-08 19:43:09.000000 ynca-5.8.0/ynca/subunits/rhap.py
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-08 19:43:09.000000 ynca-5.8.0/ynca/subunits/server.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-08 19:43:09.000000 ynca-5.8.0/ynca/subunits/sirius.py
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-06-08 19:43:09.000000 ynca-5.8.0/ynca/subunits/spotify.py
--rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-06-08 19:43:09.000000 ynca-5.8.0/ynca/subunits/system.py
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-06-08 19:43:09.000000 ynca-5.8.0/ynca/subunits/tun.py
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-06-08 19:43:09.000000 ynca-5.8.0/ynca/subunits/uaw.py
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-08 19:43:09.000000 ynca-5.8.0/ynca/subunits/usb.py
--rw-r--r--   0 runner    (1001) docker     (123)     5370 2023-06-08 19:43:09.000000 ynca-5.8.0/ynca/subunits/zone.py
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-06-08 19:43:09.000000 ynca-5.8.0/ynca/terminal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:43:19.101356 ynca-5.8.0/ynca.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5421 2023-06-08 19:43:19.000000 ynca-5.8.0/ynca.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-06-08 19:43:19.000000 ynca-5.8.0/ynca.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 19:43:19.000000 ynca-5.8.0/ynca.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-08 19:43:19.000000 ynca-5.8.0/ynca.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-08 19:43:19.000000 ynca-5.8.0/ynca.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-07 18:39:57.342256 ynca-5.9.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2023-10-07 18:39:43.000000 ynca-5.9.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2023-10-07 18:39:43.000000 ynca-5.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5474 2023-10-07 18:39:57.342256 ynca-5.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4772 2023-10-07 18:39:43.000000 ynca-5.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2023-10-07 18:39:57.342256 ynca-5.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4041 2023-10-07 18:39:43.000000 ynca-5.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-07 18:39:57.342256 ynca-5.9.0/ynca/
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2023-10-07 18:39:43.000000 ynca-5.9.0/ynca/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12144 2023-10-07 18:39:43.000000 ynca-5.9.0/ynca/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9227 2023-10-07 18:39:43.000000 ynca-5.9.0/ynca/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2023-10-07 18:39:43.000000 ynca-5.9.0/ynca/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3479 2023-10-07 18:39:43.000000 ynca-5.9.0/ynca/converters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10603 2023-10-07 18:39:43.000000 ynca-5.9.0/ynca/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2023-10-07 18:39:43.000000 ynca-5.9.0/ynca/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5166 2023-10-07 18:39:43.000000 ynca-5.9.0/ynca/function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1285 2023-10-07 18:39:43.000000 ynca-5.9.0/ynca/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3356 2023-10-07 18:39:43.000000 ynca-5.9.0/ynca/modelinfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-07 18:39:43.000000 ynca-5.9.0/ynca/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    15159 2023-10-07 18:39:43.000000 ynca-5.9.0/ynca/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5932 2023-10-07 18:39:43.000000 ynca-5.9.0/ynca/subunit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-07 18:39:57.342256 ynca-5.9.0/ynca/subunits/
+-rw-r--r--   0 runner    (1001) docker     (127)     1694 2023-10-07 18:39:43.000000 ynca-5.9.0/ynca/subunits/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2023-10-07 18:39:43.000000 ynca-5.9.0/ynca/subunits/airplay.py
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2023-10-07 18:39:43.000000 ynca-5.9.0/ynca/subunits/bt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2023-10-07 18:39:43.000000 ynca-5.9.0/ynca/subunits/dab.py
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2023-10-07 18:39:43.000000 ynca-5.9.0/ynca/subunits/ipod.py
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2023-10-07 18:39:43.000000 ynca-5.9.0/ynca/subunits/ipodusb.py
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2023-10-07 18:39:43.000000 ynca-5.9.0/ynca/subunits/napster.py
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2023-10-07 18:39:43.000000 ynca-5.9.0/ynca/subunits/netradio.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2023-10-07 18:39:43.000000 ynca-5.9.0/ynca/subunits/pandora.py
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2023-10-07 18:39:43.000000 ynca-5.9.0/ynca/subunits/pc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2023-10-07 18:39:43.000000 ynca-5.9.0/ynca/subunits/rhap.py
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2023-10-07 18:39:43.000000 ynca-5.9.0/ynca/subunits/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2023-10-07 18:39:43.000000 ynca-5.9.0/ynca/subunits/sirius.py
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2023-10-07 18:39:43.000000 ynca-5.9.0/ynca/subunits/spotify.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2717 2023-10-07 18:39:43.000000 ynca-5.9.0/ynca/subunits/system.py
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2023-10-07 18:39:43.000000 ynca-5.9.0/ynca/subunits/tun.py
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2023-10-07 18:39:43.000000 ynca-5.9.0/ynca/subunits/uaw.py
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2023-10-07 18:39:43.000000 ynca-5.9.0/ynca/subunits/usb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4975 2023-10-07 18:39:43.000000 ynca-5.9.0/ynca/subunits/zone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2487 2023-10-07 18:39:43.000000 ynca-5.9.0/ynca/terminal.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-07 18:39:57.342256 ynca-5.9.0/ynca.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5474 2023-10-07 18:39:57.000000 ynca-5.9.0/ynca.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2023-10-07 18:39:57.000000 ynca-5.9.0/ynca.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-07 18:39:57.000000 ynca-5.9.0/ynca.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2023-10-07 18:39:57.000000 ynca-5.9.0/ynca.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2023-10-07 18:39:57.000000 ynca-5.9.0/ynca.egg-info/top_level.txt
```

### Comparing `ynca-5.8.0/LICENSE.txt` & `ynca-5.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ynca-5.8.0/PKG-INFO` & `ynca-5.9.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ynca
-Version: 5.8.0
+Version: 5.9.0
 Summary: Package to control Yamaha receivers that support the YNCA protocol.
 Home-page: https://github.com/mvdwetering/ynca
 Author: Michel van de Wetering
 Author-email: michel.van.de.wetering+ynca@gmail.com
 License: MIT
 Keywords: automation
 Classifier: Development Status :: 5 - Production/Stable
@@ -20,29 +20,29 @@
 # YNCA
 
 Package to control Yamaha receivers that support the YNCA protocol.
 
 According to reports of users and info found on the internet the following receivers should work.
 There might be more receivers that support this protocol. If you find some let met know so the list can be updated.
 
-> HTR-4071, RX-A700, RX-A710, RX-A720, RX-A740, RX-A800, RX-A810, RX-A820, RX-A840, RX-A850, RX-A1000, RX-A1010, RX-A1020, RX-A1030, RX-A1040, RX-A2000, RX-A2010, RX-A2020, RX-A2070, RX-A3000, RX-A3010, RX-A3020, RX-V475, RX-V477, RX-V483, RX-V671, RX-V673, RX-V675, RX-V677, RX-V771, RX-V773, RX-V777, RX-V867, RX-V871, RX-V1067, RX-V2067, RX-V3067, TSR-700, TSR-7850
+> HTR-4065, HTR-4071, HTR-6064, RX-A660, RX-A700, RX-A710, RX-A720, RX-A740, RX-A750, RX-A800, RX-A810, RX-A820, RX-A840, RX-A850, RX-A1000, RX-A1010, RX-A1020, RX-A1030, RX-A1040, RX-A2000, RX-A2010, RX-A2020, RX-A2070, RX-A3000, RX-A3010, RX-A3020, RX-A3030, RX-A3070, RX-V475, RX-V477, RX-V481D, RX-V483, RX-V671, RX-V673, RX-V675, RX-V677, RX-V771, RX-V773, RX-V775, RX-V777, RX-V867, RX-V871, RX-V1067, RX-V1071, RX-V2067, RX-V2071, RX-V3067, RX-V3071, TSR-700, TSR-7850
 
-Note that there is a restriction that only 1 YNCA connection to a receiver can be made at the time (restriction on the receiver side, not this library).
+Note that only 1 YNCA connection to a receiver can be made at the time (restriction on the receiver side, not this library).
 Usually not a problem as the Yamaha AV Control App uses a different protocol which can be used at the same time, but something to be aware of when testing the library.
 
 
 ## Installation
 
 ```bash
 python3 -m pip install ynca
 ```
 
 ## Contents
 
-Note that the intended API to use is exposed from the toplevel package.
+The intended API to use is exposed from the toplevel package.
 
 ### Classes
 
 #### YncaApi
 
 This is the main class to interact with. The YncaApi class is exposing YNCA subunits and their functions as Python classes/datatypes and allows to connect to devices supporting that API. It keeps a cache which gets updated when values are received from the device so reading attributes is instant as it does not need to query the receiver.
 
@@ -69,15 +69,15 @@
 python3 -m ynca.terminal socket://192.168.178.21:50000
 ```
 
 #### YNCA Server
 
 This is a very basic YNCA server intended to be just enough for debugging and testing without connecting to a real device.
 
-Note that the server needs to be filled with data from an actual device and it will basically just repeat the same answers as the real device gave (with a few exceptions).
+The server needs to be filled with data from an actual device and it will basically just repeat the same answers as the real device gave (with a few exceptions).
 Filling the server can be done by providing it with YNCA logging of a real device, like the ones in the YCNA package repository or a log from your own device e.g. by running `example.py` with loglevel DEBUG (uncomment the line in the example code).
 
 It has some additional commandline options for using different ports, binding to a specific host or testing disconnects
 
 ```
 python3 -m ynca.server <ynca_repo>/logs/RX-A810.txt
 python3 -m ynca.server --host localhost --port 12345 <ynca_repo>/logs/RX-A810.txt
@@ -92,15 +92,15 @@
 # Port could also be e.g. COM3 on Windows or any `serial_url` as supported by PySerial
 # Like for example `socket://192.168.178.21:50000` for IP connection
 receiver = YncaApi("/dev/tty1")
 
 # Initializing takes a while (~10 seconds for a 2 zone receiver) since it communicates
 # quite a lot with the actual device to determine its capabilities.
 # Later calls to the subunits are fast.
-# Note that attributes that are still None after initialization are not supported by the subunits
+# The attributes that are still None after initialization are not supported by the subunits
 receiver.initialize()
 
 # Every subunit has a dedicated attribute on the `YncaApi` class.
 # The name of the attribute is the subunit id as used in YNCA.
 # The returned subunit class can be used to communicate with the subunit
 sys = receiver.sys
 main = receiver.main
```

### Comparing `ynca-5.8.0/README.md` & `ynca-5.9.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 # YNCA
 
 Package to control Yamaha receivers that support the YNCA protocol.
 
 According to reports of users and info found on the internet the following receivers should work.
 There might be more receivers that support this protocol. If you find some let met know so the list can be updated.
 
-> HTR-4071, RX-A700, RX-A710, RX-A720, RX-A740, RX-A800, RX-A810, RX-A820, RX-A840, RX-A850, RX-A1000, RX-A1010, RX-A1020, RX-A1030, RX-A1040, RX-A2000, RX-A2010, RX-A2020, RX-A2070, RX-A3000, RX-A3010, RX-A3020, RX-V475, RX-V477, RX-V483, RX-V671, RX-V673, RX-V675, RX-V677, RX-V771, RX-V773, RX-V777, RX-V867, RX-V871, RX-V1067, RX-V2067, RX-V3067, TSR-700, TSR-7850
+> HTR-4065, HTR-4071, HTR-6064, RX-A660, RX-A700, RX-A710, RX-A720, RX-A740, RX-A750, RX-A800, RX-A810, RX-A820, RX-A840, RX-A850, RX-A1000, RX-A1010, RX-A1020, RX-A1030, RX-A1040, RX-A2000, RX-A2010, RX-A2020, RX-A2070, RX-A3000, RX-A3010, RX-A3020, RX-A3030, RX-A3070, RX-V475, RX-V477, RX-V481D, RX-V483, RX-V671, RX-V673, RX-V675, RX-V677, RX-V771, RX-V773, RX-V775, RX-V777, RX-V867, RX-V871, RX-V1067, RX-V1071, RX-V2067, RX-V2071, RX-V3067, RX-V3071, TSR-700, TSR-7850
 
-Note that there is a restriction that only 1 YNCA connection to a receiver can be made at the time (restriction on the receiver side, not this library).
+Note that only 1 YNCA connection to a receiver can be made at the time (restriction on the receiver side, not this library).
 Usually not a problem as the Yamaha AV Control App uses a different protocol which can be used at the same time, but something to be aware of when testing the library.
 
 
 ## Installation
 
 ```bash
 python3 -m pip install ynca
 ```
 
 ## Contents
 
-Note that the intended API to use is exposed from the toplevel package.
+The intended API to use is exposed from the toplevel package.
 
 ### Classes
 
 #### YncaApi
 
 This is the main class to interact with. The YncaApi class is exposing YNCA subunits and their functions as Python classes/datatypes and allows to connect to devices supporting that API. It keeps a cache which gets updated when values are received from the device so reading attributes is instant as it does not need to query the receiver.
 
@@ -50,15 +50,15 @@
 python3 -m ynca.terminal socket://192.168.178.21:50000
 ```
 
 #### YNCA Server
 
 This is a very basic YNCA server intended to be just enough for debugging and testing without connecting to a real device.
 
-Note that the server needs to be filled with data from an actual device and it will basically just repeat the same answers as the real device gave (with a few exceptions).
+The server needs to be filled with data from an actual device and it will basically just repeat the same answers as the real device gave (with a few exceptions).
 Filling the server can be done by providing it with YNCA logging of a real device, like the ones in the YCNA package repository or a log from your own device e.g. by running `example.py` with loglevel DEBUG (uncomment the line in the example code).
 
 It has some additional commandline options for using different ports, binding to a specific host or testing disconnects
 
 ```
 python3 -m ynca.server <ynca_repo>/logs/RX-A810.txt
 python3 -m ynca.server --host localhost --port 12345 <ynca_repo>/logs/RX-A810.txt
@@ -73,15 +73,15 @@
 # Port could also be e.g. COM3 on Windows or any `serial_url` as supported by PySerial
 # Like for example `socket://192.168.178.21:50000` for IP connection
 receiver = YncaApi("/dev/tty1")
 
 # Initializing takes a while (~10 seconds for a 2 zone receiver) since it communicates
 # quite a lot with the actual device to determine its capabilities.
 # Later calls to the subunits are fast.
-# Note that attributes that are still None after initialization are not supported by the subunits
+# The attributes that are still None after initialization are not supported by the subunits
 receiver.initialize()
 
 # Every subunit has a dedicated attribute on the `YncaApi` class.
 # The name of the attribute is the subunit id as used in YNCA.
 # The returned subunit class can be used to communicate with the subunit
 sys = receiver.sys
 main = receiver.main
```

### Comparing `ynca-5.8.0/setup.py` & `ynca-5.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     long_description = f.read()
 
 setup(
     name="ynca",
     # Versions should comply with PEP440.  For a discussion on single-sourcing
     # the version across setup.py and the project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version="5.8.0",
+    version="5.9.0",
     description="Package to control Yamaha receivers that support the YNCA protocol.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     # The project's main homepage.
     url="https://github.com/mvdwetering/ynca",
     # Author details
     author="Michel van de Wetering",
```

### Comparing `ynca-5.8.0/ynca/__init__.py` & `ynca-5.9.0/ynca/__init__.py`

 * *Files identical despite different names*

### Comparing `ynca-5.8.0/ynca/api.py` & `ynca-5.9.0/ynca/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,15 +104,15 @@
 
     def _get_subunit_class(self, subunit_id):
         subunit_classes = all_subclasses(SubunitBase)
         for subunit_class in subunit_classes:
             try:
                 if subunit_class.id == subunit_id:
                     return subunit_class
-            except AttributeError:   # pragma: no cover
+            except AttributeError:  # pragma: no cover
                 # Intermediate Subunit classes like ZoneBase don't have an ID
                 pass
 
     def _initialize_available_subunits(self, connection: YncaConnection):
         # Every receiver has a System subunit
         # It also does not respond to AVAIL=? so it will not end up in _available_subunits
         system = System(connection)
@@ -135,20 +135,20 @@
         without executing the timeconsuming `initialize()` method.
         """
         result: YncaConnectionCheckResult = YncaConnectionCheckResult()
         connection = None
         connection_check_event = threading.Event()
 
         def _connection_check_message_received(
-            status: YncaProtocolStatus, subunit: str, function_: str, value: str
+            status: YncaProtocolStatus, subunit: str|None, function_: str|None, value: str|None
         ):
-            if subunit == Subunit.SYS and function_ == "MODELNAME":
-                result.modelname = value
+            if subunit == Subunit.SYS and function_ == "MODELNAME" and value is not None:
+                result.modelname = value 
                 connection_check_event.set()
-            if function_ == "AVAIL":
+            if function_ == "AVAIL" and subunit is not None:
                 result.zones.append(subunit)
 
         try:
             connection = YncaConnection.create_from_serial_url(self._serial_url)
             connection.connect(self._disconnect_callback, self._communication_log_size)
             connection.register_message_callback(_connection_check_message_received)
             connection.get(Subunit.MAIN, "AVAIL")
@@ -192,15 +192,15 @@
             self._initialize_available_subunits(connection)
             is_initialized = True
         finally:
             if not is_initialized:
                 self.close()
 
     def _protocol_message_received(
-        self, status: YncaProtocolStatus, subunit: str, function_: str, value: str
+        self, status: YncaProtocolStatus, subunit: str|None, function_: str|None, value: str|None
     ):
         if function_ == "AVAIL":
             self._available_subunits.add(subunit)
 
         if subunit == Subunit.SYS and function_ == "VERSION":
             self._initialized_event.set()
```

### Comparing `ynca-5.8.0/ynca/connection.py` & `ynca-5.9.0/ynca/connection.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import logging
 import queue
 import re
 import threading
 import time
 from enum import Enum
-from typing import Callable, List, Optional, Set
+from typing import Callable, List, Optional, Set, cast
 
 import serial  # type: ignore
 import serial.threaded  # type: ignore
 
 from .errors import YncaConnectionError, YncaConnectionFailed
 from .helpers import RingBuffer
 
@@ -33,16 +33,16 @@
     COMMAND_SPACING = 0.1
 
     # YNCA spec says standby timeout is 40 seconds, so use a shorter period to be on the safe side
     KEEP_ALIVE_INTERVAL = 30
 
     def __init__(self):
         super().__init__()
-        self.message_callback = None
-        self.disconnect_callback = None
+        self.message_callback:Callable[[YncaProtocolStatus, str|None, str|None, str|None], None]
+        self.disconnect_callback:Callable[[], None] | None
         self._send_queue = None
         self._send_thread = None
         self._last_sent_command = None
         self.connected = False
         self._keep_alive_pending = False
         self._communication_log_buffer: LogBuffer = LogBuffer(0)
         self.num_commands_sent = 0
@@ -83,17 +83,17 @@
 
         if self.disconnect_callback:
             self.disconnect_callback()
 
     def handle_line(self, line):
         ignore = False
         status = YncaProtocolStatus.OK
-        subunit = None
-        function = None
-        value = None
+        subunit:str|None = None
+        function:str|None = None
+        value:str|None = None
 
         logger.debug("Recv - %s", line)
         self._communication_log_buffer.add(f"Received: {line}")
 
         if line == "@UNDEFINED":
             status = YncaProtocolStatus.UNDEFINED
         elif line == "@RESTRICTED":
@@ -191,29 +191,29 @@
         """
         self._port = serial_url
         self._serial = None
         self._readerthread: Optional[serial.threaded.ReaderThread] = None
         self._protocol: Optional[YncaProtocol] = None
 
         self._message_callbacks: Set[
-            Callable[[YncaProtocolStatus, str, str, str], None]
+            Callable[[YncaProtocolStatus, str|None, str|None, str|None], None]
         ] = set()
 
     def register_message_callback(
-        self, callback: Callable[[YncaProtocolStatus, str, str, str], None]
+        self, callback: Callable[[YncaProtocolStatus, str|None, str|None, str|None], None]
     ):
         self._message_callbacks.add(callback)
 
     def unregister_message_callback(
-        self, callback: Callable[[YncaProtocolStatus, str, str, str], None]
+        self, callback: Callable[[YncaProtocolStatus, str|None, str|None, str|None], None]
     ):
         self._message_callbacks.discard(callback)
 
     def _call_registered_message_callbacks(
-        self, status: YncaProtocolStatus, subunit: str, function_: str, value: str
+        self, status: YncaProtocolStatus, subunit: str|None, function_: str|None, value: str|None
     ):
         for callback in self._message_callbacks:
             callback(status, subunit, function_, value)
 
     def connect(
         self,
         disconnect_callback: Callable[[], None] | None = None,
@@ -221,15 +221,16 @@
     ):
         try:
             self._serial = serial.serial_for_url(self._port)
             self._readerthread = serial.threaded.ReaderThread(
                 self._serial, YncaProtocol
             )
             self._readerthread.start()
-            _, self._protocol = self._readerthread.connect()
+            _, protocol = self._readerthread.connect()
+            self._protocol = cast(YncaProtocol, protocol)
         except serial.SerialException as e:
             raise YncaConnectionError(e)
         except RuntimeError as e:
             raise YncaConnectionFailed(e)
 
         if self._protocol:
             self._protocol.message_callback = self._call_registered_message_callbacks
```

### Comparing `ynca-5.8.0/ynca/constants.py` & `ynca-5.9.0/ynca/constants.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Misc constants"""
 import logging
-from enum import Enum
+from enum import Enum, unique
 
 logger = logging.getLogger(__name__)
 
 MIN_VOLUME = -80.5  # Minimum volume value for receivers
 
-
+@unique
 class Subunit(str, Enum):
     """Known Subunits in YNCA"""
 
     SYS = "SYS"
     MAIN = "MAIN"
     ZONE2 = "ZONE2"
     ZONE3 = "ZONE3"
@@ -31,8 +31,8 @@
     SERVER = "SERVER"
     SPOTIFY = "SPOTIFY"
     TUN = "TUN"
     UAW = "UAW"
     USB = "USB"
 
     def __format__(self, spec) -> str:
-        return self.value
+        return self.value
```

### Comparing `ynca-5.8.0/ynca/converters.py` & `ynca-5.9.0/ynca/converters.py`

 * *Files identical despite different names*

### Comparing `ynca-5.8.0/ynca/enums.py` & `ynca-5.9.0/ynca/enums.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,137 +1,147 @@
 """Enums used for mapping YNCA values"""
 
 import logging
-from enum import Enum
+from enum import Enum, unique
 
 logger = logging.getLogger(__name__)
 
 UNKNOWN_STRING = "< UNKNOWN >"
 
-
+@unique
 class AdaptiveDrc(str, Enum):
     OFF = "Off"
     AUTO = "Auto"
 
     @classmethod
     def _missing_(cls, value):
         logger.warning("Unknown value '%s' in %s", value, cls.__name__)
         return cls.UNKNOWN
 
     UNKNOWN = UNKNOWN_STRING
     """Unknown values in the enum are mapped to UNKNOWN"""
 
 
+@unique
 class Avail(str, Enum):
     NOT_CONNECTED = "Not Connected"
     NOT_READY = "Not Ready"
     READY = "Ready"
 
     @classmethod
     def _missing_(cls, value):
         logger.warning("Unknown value '%s' in %s", value, cls.__name__)
         return cls.UNKNOWN
 
     UNKNOWN = UNKNOWN_STRING
     """Unknown values in the enum are mapped to UNKNOWN"""
 
 
+@unique
 class BandDab(str, Enum):
     DAB = "DAB"
     FM = "FM"
 
     @classmethod
     def _missing_(cls, value):
         logger.warning("Unknown value '%s' in %s", value, cls.__name__)
         return cls.UNKNOWN
 
     UNKNOWN = UNKNOWN_STRING
     """Unknown values in the enum are mapped to UNKNOWN"""
 
 
+@unique
 class BandTun(str, Enum):
     AM = "AM"
     FM = "FM"
 
     @classmethod
     def _missing_(cls, value):
         logger.warning("Unknown value '%s' in %s", value, cls.__name__)
         return cls.UNKNOWN
 
     UNKNOWN = UNKNOWN_STRING
     """Unknown values in the enum are mapped to UNKNOWN"""
 
 
+@unique
 class Enhancer(str, Enum):
     ON = "On"
     OFF = "Off"
 
     @classmethod
     def _missing_(cls, value):
         logger.warning("Unknown value '%s' in %s", value, cls.__name__)
         return cls.UNKNOWN
 
     UNKNOWN = UNKNOWN_STRING
     """Unknown values in the enum are mapped to UNKNOWN"""
 
 
+@unique
 class HdmiOut(str, Enum):
     OFF = "Off"
     OUT1 = "OUT1"
     OUT2 = "OUT2"
     OUT1_PLUS_2 = "OUT1 + 2"
 
     @classmethod
     def _missing_(cls, value):
         logger.warning("Unknown value '%s' in %s", value, cls.__name__)
         return cls.UNKNOWN
 
     UNKNOWN = UNKNOWN_STRING
     """Unknown values in the enum are mapped to UNKNOWN"""
 
+
+@unique
 class HdmiOutOnOff(Enum):
     ON = "On"
     OFF = "Off"
 
     @classmethod
     def _missing_(cls, value):
         logger.warning("Unknown value '%s' in %s", value, cls.__name__)
         return cls.UNKNOWN
 
     UNKNOWN = UNKNOWN_STRING
     """Unknown values in the enum are mapped to UNKNOWN"""
 
 
+@unique
 class InitVolLvl(str, Enum):
     MUTE = "Mute"
     OFF = "Off"
     """Only some receivers report Off, most seem to use InitVolMode to indicate On/Off"""
 
     @classmethod
     def _missing_(cls, value):
         logger.warning("Unknown value '%s' in %s", value, cls.__name__)
         return cls.UNKNOWN
 
     UNKNOWN = UNKNOWN_STRING
     """Unknown values in the enum are mapped to UNKNOWN"""
 
 
+@unique
 class InitVolMode(str, Enum):
     ON = "On"
     OFF = "Off"
 
     @classmethod
     def _missing_(cls, value):
         logger.warning("Unknown value '%s' in %s", value, cls.__name__)
         return cls.UNKNOWN
 
     UNKNOWN = UNKNOWN_STRING
     """Unknown values in the enum are mapped to UNKNOWN"""
 
 
+@unique
 class Input(Enum):
     # Inputs with connectors on the receiver
     AUDIO1 = "AUDIO1"
     AUDIO2 = "AUDIO2"
     AUDIO3 = "AUDIO3"
     AUDIO4 = "AUDIO4"
     AV1 = "AV1"
@@ -177,55 +187,58 @@
         logger.warning("Unknown value '%s' in %s", value, cls.__name__)
         return cls.UNKNOWN
 
     UNKNOWN = UNKNOWN_STRING
     """Unknown values in the enum are mapped to UNKNOWN"""
 
 
+@unique
 class Mute(str, Enum):
     ON = "On"
     ATT_MINUS_20 = "Att -20 dB"
     ATT_MINUS_40 = "Att -40 dB"
     OFF = "Off"
 
     @classmethod
     def _missing_(cls, value):
         logger.warning("Unknown value '%s' in %s", value, cls.__name__)
         return cls.UNKNOWN
 
     UNKNOWN = UNKNOWN_STRING
     """Unknown values in the enum are mapped to UNKNOWN"""
 
-
+@unique
 class Party(Enum):
     ON = "On"
     OFF = "Off"
 
     @classmethod
     def _missing_(cls, value):
         logger.warning("Unknown value '%s' in %s", value, cls.__name__)
         return cls.UNKNOWN
 
     UNKNOWN = UNKNOWN_STRING
     """Unknown values in the enum are mapped to UNKNOWN"""
 
 
+@unique
 class PartyMute(Enum):
     ON = "On"
     OFF = "Off"
 
     @classmethod
     def _missing_(cls, value):
         logger.warning("Unknown value '%s' in %s", value, cls.__name__)
         return cls.UNKNOWN
 
     UNKNOWN = UNKNOWN_STRING
     """Unknown values in the enum are mapped to UNKNOWN"""
 
 
+@unique
 class Playback(str, Enum):
     STOP = "Stop"
     PAUSE = "Pause"
     PLAY = "Play"
     SKIP_REV = "Skip Rev"
     SKIP_FWD = "Skip Fwd"
 
@@ -234,81 +247,87 @@
         logger.warning("Unknown value '%s' in %s", value, cls.__name__)
         return cls.UNKNOWN
 
     UNKNOWN = UNKNOWN_STRING
     """Unknown values in the enum are mapped to UNKNOWN"""
 
 
+@unique
 class PlaybackInfo(str, Enum):
     STOP = "Stop"
     PAUSE = "Pause"
     PLAY = "Play"
 
     @classmethod
     def _missing_(cls, value):
         logger.warning("Unknown value '%s' in %s", value, cls.__name__)
         return cls.UNKNOWN
 
     UNKNOWN = UNKNOWN_STRING
     """Unknown values in the enum are mapped to UNKNOWN"""
 
 
+@unique
 class PureDirMode(Enum):
     ON = "On"
     OFF = "Off"
 
     @classmethod
     def _missing_(cls, value):
         logger.warning("Unknown value '%s' in %s", value, cls.__name__)
         return cls.UNKNOWN
 
     UNKNOWN = UNKNOWN_STRING
     """Unknown values in the enum are mapped to UNKNOWN"""
 
 
+@unique
 class Pwr(Enum):
     ON = "On"
     STANDBY = "Standby"
 
     @classmethod
     def _missing_(cls, value):
         logger.warning("Unknown value '%s' in %s", value, cls.__name__)
         return cls.UNKNOWN
 
     UNKNOWN = UNKNOWN_STRING
     """Unknown values in the enum are mapped to UNKNOWN"""
 
 
+@unique
 class Repeat(str, Enum):
     OFF = "Off"
     SINGLE = "Single"
     ALL = "All"
 
     @classmethod
     def _missing_(cls, value):
         logger.warning("Unknown value '%s' in %s", value, cls.__name__)
         return cls.UNKNOWN
 
     UNKNOWN = UNKNOWN_STRING
     """Unknown values in the enum are mapped to UNKNOWN"""
 
 
+@unique
 class Shuffle(str, Enum):
     ON = "On"
     OFF = "Off"
 
     @classmethod
     def _missing_(cls, value):
         logger.warning("Unknown value '%s' in %s", value, cls.__name__)
         return cls.UNKNOWN
 
     UNKNOWN = UNKNOWN_STRING
     """Unknown values in the enum are mapped to UNKNOWN"""
 
 
+@unique
 class Sleep(str, Enum):
     OFF = "Off"
     THIRTY_MIN = "30 min"
     SIXTY_MIN = "60 min"
     NINETY_MIN = "90 min"
     ONEHUNDREDTWENTY_MIN = "120 min"
 
@@ -317,14 +336,15 @@
         logger.warning("Unknown value '%s' in %s", value, cls.__name__)
         return cls.UNKNOWN
 
     UNKNOWN = UNKNOWN_STRING
     """Unknown values in the enum are mapped to UNKNOWN"""
 
 
+@unique
 class SoundPrg(str, Enum):
     HALL_IN_MUNICH = "Hall in Munich"
     HALL_IN_VIENNA = "Hall in Vienna"
     HALL_IN_AMSTERDAM = "Hall in Amsterdam"
     CHURCH_IN_FREIBURG = "Church in Freiburg"
     CHURCH_IN_ROYAUMONT = "Church in Royaumont"
     CHAMBER = "Chamber"
@@ -357,56 +377,61 @@
         logger.warning("Unknown value '%s' in %s", value, cls.__name__)
         return cls.UNKNOWN
 
     UNKNOWN = UNKNOWN_STRING
     """Unknown values in the enum are mapped to UNKNOWN"""
 
 
+@unique
 class Straight(Enum):
     ON = "On"
     OFF = "Off"
 
     @classmethod
     def _missing_(cls, value):
         logger.warning("Unknown value '%s' in %s", value, cls.__name__)
         return cls.UNKNOWN
 
     UNKNOWN = UNKNOWN_STRING
     """Unknown values in the enum are mapped to UNKNOWN"""
 
 
+@unique
 class ThreeDeeCinema(str, Enum):
     OFF = "Off"
     AUTO = "Auto"
 
     @classmethod
     def _missing_(cls, value):
         logger.warning("Unknown value '%s' in %s", value, cls.__name__)
         return cls.UNKNOWN
 
     UNKNOWN = UNKNOWN_STRING
     """Unknown values in the enum are mapped to UNKNOWN"""
 
 
+@unique
 class TwoChDecoder(str, Enum):
     # Older models support Dolby Prologic and DTS:Neo settings
     DolbyPl = "Dolby PL"
     DolbyPl2Movie = "Dolby PLII Movie"
     DolbyPl2Music = "Dolby PLII Music"
     DolbyPl2Game = "Dolby PLII Game"
     DolbyPl2xMovie = "Dolby PLIIx Movie"
     DolbyPl2xMusic = "Dolby PLIIx Music"
     DolbyPl2xGame = "Dolby PLIIx Game"
     DtsNeo6Cinema = "DTS NEO:6 Cinema"
     DtsNeo6Music = "DTS NEO:6 Music"
 
     # Newer models seem to have diffent values
-    # These have been seen
+    # These have been seen (Note that RX-A3070 also supports the DTS NEO presets)
     Auro3d = "AURO-3D"  # Seen on RX-A6A
-    DtsNeuralX = "DTS Neural:X"  # Seen on RX-A1060
+    Auto = "Auto"  # SEen on RX-A3070
+    DolbySurround = "Dolby Surround"  # Seen on RX-A3070
+    DtsNeuralX = "DTS Neural:X"  # Seen on RX-A1060 and RX-A3070
 
     @classmethod
     def _missing_(cls, value):
         logger.warning("Unknown value '%s' in %s", value, cls.__name__)
         return cls.UNKNOWN
 
     UNKNOWN = UNKNOWN_STRING
```

### Comparing `ynca-5.8.0/ynca/errors.py` & `ynca-5.9.0/ynca/errors.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,10 +11,10 @@
 
 class YncaConnectionFailed(YncaException):
     """Connection made, but broke. Most likely connecting to a device that already has the YNCA port occupied."""
 
 
 class YncaInitializationFailedException(YncaException):
     """Initialization of Zone failed.
-Several possible causes, for example:
-* connecting to a device that already has the YNCA port occupied
-* bug in the ynca component > enable debug logging for more info"""
+    Several possible causes, for example:
+    * connecting to a device that already has the YNCA port occupied
+    * bug in the ynca component > enable debug logging for more info"""
```

### Comparing `ynca-5.8.0/ynca/function.py` & `ynca-5.9.0/ynca/function.py`

 * *Files 24% similar despite different names*

```diff
@@ -34,37 +34,40 @@
     Provides an easy way to specify all properties needed to handle a YNCA function.
     The resulting descriptor makes it easy to just read/write to the attributes and
     values will be read from cache or converted and sent to the device.
     """
 
     def __init__(
         self,
-        name: str,
         converter: ConverterBase,
         cmd: Cmd = Cmd.GET | Cmd.PUT,
+        name_override: str | None = None,
         init: str | None = None,
         no_initialize: bool = False,
     ) -> None:
         """
-        name:
-            Name of the function
         converter:
             Converter to use for value to/from str conversions
         cmd:
             Operations the command supports. PUT and/or GET
+        name_override:
+            Optional name_override useful in case where function name can not be a valid Python attribute name e.g. 2CHDECODER
         init:
             Name of function to use for initialize. Only needed if the function name to initialize is different from the function name itself. E.g. METAINFO for ARTIST, ALBUM and SONG to reduce amount of commands needed
         no_initialize:
             Do not initialize this function, very specific usecase, do _not_ use unless you know what you are doing!
         """
-        self.name = name
-        self.cmd = cmd
         self.converter = converter
-        self.no_initialize = no_initialize
+        self.cmd = cmd
         self.initializer = init
+        self.no_initialize = no_initialize
+
+        # Name will be set in __set_name__, provide typehint to help the linter
+        self.name: str
+        self._name_override = name_override
 
     @overload
     def __get__(self, instance: None, owner) -> FunctionBase[T]:  # pragma: no cover
         ...
 
     @overload
     def __get__(self, instance: SubunitBase, owner) -> T | None:  # pragma: no cover
@@ -82,92 +85,94 @@
         return instance.function_handlers[self.name].value
 
     def __set__(self, instance, value: T):
         if Cmd.PUT not in self.cmd:
             raise AttributeError(f"Function {self.name} does not support PUT command")
         instance._put(self.name, self.converter.to_str(value))
 
-    def __delete__(self, instance: SubunitBase):  # pragma: no cover
-        # Don't think I have use for this
-        pass
+    def __delete__(self, instance: SubunitBase):
+        del instance.function_handlers[self.name]
+
+    def __set_name__(self, owner, name):
+        self.name = name.upper() if not self._name_override else self._name_override
 
 
 class EnumFunction(FunctionBase[E], Generic[E]):
     def __init__(
         self,
-        name: str,
         datatype: Type[E],
         cmd: Cmd = Cmd.GET | Cmd.PUT,
+        name_override: str | None = None,
         init=None,
     ) -> None:
         super().__init__(
-            name,
+            name_override=name_override,
             cmd=cmd,
             converter=EnumConverter[E](datatype),
             init=init,
         )
 
 
 class StrFunction(FunctionBase[str]):
     def __init__(
         self,
-        name: str,
         cmd: Cmd = Cmd.GET | Cmd.PUT,
         converter: ConverterBase = StrConverter(),
+        name_override: str | None = None,
         init=None,
     ) -> None:
         super().__init__(
-            name,
+            name_override=name_override,
             cmd=cmd,
             converter=converter,
             init=init,
         )
 
 
 class IntFunction(FunctionBase[int]):
     def __init__(
         self,
-        name: str,
         command_type: Cmd = Cmd.GET | Cmd.PUT,
         converter: ConverterBase = IntConverter(),
+        name_override: str | None = None,
         init=None,
     ) -> None:
         super().__init__(
-            name,
+            name_override=name_override,
             cmd=command_type,
             converter=converter,
             init=init,
         )
 
 
 class FloatFunction(FunctionBase[float]):
     def __init__(
         self,
-        name: str,
         cmd: Cmd = Cmd.GET | Cmd.PUT,
         converter: ConverterBase = FloatConverter(),
+        name_override: str | None = None,
         init=None,
     ) -> None:
         super().__init__(
-            name,
+            name_override=name_override,
             cmd=cmd,
             converter=converter,
             init=init,
         )
 
 
 class EnumOrFloatFunction(FunctionBase, Generic[E]):
     def __init__(
         self,
-        name: str,
         datatype: Type[E],
         converter: MultiConverter | None = None,
         cmd: Cmd = Cmd.GET | Cmd.PUT,
+        name_override: str | None = None,
         init=None,
     ) -> None:
         super().__init__(
-            name,
+            name_override=name_override,
             cmd=cmd,
             converter=converter
             or MultiConverter([EnumConverter[E](datatype), FloatConverter()]),
             init=init,
         )
```

### Comparing `ynca-5.8.0/ynca/helpers.py` & `ynca-5.9.0/ynca/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     negative = value < 0
 
     steps = round(value / stepsize)
     stepped_value = steps * stepsize
     after_the_point, before_the_point = modf(stepped_value)
 
     before_the_point = abs(before_the_point)
-    after_the_point = int(abs(after_the_point * (10**decimals)))
+    after_the_point = int(abs(after_the_point * (10 ** decimals)))
 
     output = "-" if negative and (before_the_point > 0 or after_the_point > 0) else ""
     output += str(int(before_the_point))
     if decimals > 0:
         output += f".{str(after_the_point).rjust(decimals, '0')}"
 
     return output
```

### Comparing `ynca-5.8.0/ynca/modelinfo.py` & `ynca-5.9.0/ynca/modelinfo.py`

 * *Files identical despite different names*

### Comparing `ynca-5.8.0/ynca/server.py` & `ynca-5.9.0/ynca/server.py`

 * *Files 1% similar despite different names*

```diff
@@ -202,14 +202,22 @@
         if value.startswith("@"):
             if not skip_error_response:
                 self.write_line(value)
         else:
             self.write_line(f"@{subunit}:{function}={value}")
 
     def handle_put(self, subunit, function, value):
+
+        # Just eat remote codes as they don't give responses
+        # unless not supported, but can not really check
+        if subunit == "SYS" and function == "REMOTECODE":
+            if len(value) != 8:
+                self.write_line(UNDEFINED)
+            return
+
         if function == "VOL" and value.startswith("Up") or value.startswith("Down"):
             # Need to handle Up/Down as it would otherwise overwrite the VOL value wtih text Up/Down
             up = value.startswith("Up")
 
             parts = value.split(" ")
             amount = 0.5 if len(parts) == 1 else (int(parts[1]))
 
@@ -255,16 +263,14 @@
                         if zone_is_on != UNDEFINED:
                             sys_is_on |= zone_is_on == "On"
                     sys_on_value = "On" if sys_is_on else "Standby"
                     result = self.store.put_data("SYS", function, sys_on_value)
                     if result[1]:
                         self.write_line(f"@SYS:{function}={sys_on_value}")
 
-
-
     def handle(self):
         # self.rfile is a file-like object created by the handler;
         # we can now use e.g. readline() instead of raw recv() calls
         #
         # Note that the connection is closed when this handler returns!
 
         commands_received = 0
```

### Comparing `ynca-5.8.0/ynca/subunit.py` & `ynca-5.9.0/ynca/subunit.py`

 * *Files 7% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 class SubunitBase(ABC):
     """
     Baseclass for Subunits, should be subclassed do not instantiate manually.
     """
 
     id: Subunit  # Just typed, needs to be set in subclasses
 
-    avail = EnumFunction[Avail]("AVAIL", Avail, Cmd.GET)
+    avail = EnumFunction[Avail](Avail, Cmd.GET)
 
     def __init__(self, connection: YncaConnection) -> None:
         self._update_callbacks: Set[Callable[[str, Any], None]] = set()
 
         self.function_handlers: Dict[str, YncaFunctionHandler] = {}
 
         # Note that we need to iterate over the _class_
@@ -120,17 +120,17 @@
             )
             self._connection = None
             self._update_callbacks = set()
 
     def _protocol_message_received(
         self,
         status: YncaProtocolStatus,
-        subunit: str,
-        function_name: str,
-        value_str: str,
+        subunit: str|None,
+        function_name: str|None,
+        value_str: str|None,
     ):
         if status is not YncaProtocolStatus.OK:
             # Can't really handle errors since at this point we can't see to what command it belonged
             return
 
         # During initialization SYS:VERSION is used to signal that initialization is done
         if (
@@ -139,15 +139,15 @@
             and function_name == "VERSION"
         ):
             self._initialized_event.set()
 
         if self.id != subunit:
             return
 
-        if handler := self.function_handlers.get(function_name, None):
+        if function_name is not None and value_str is not None and (handler := self.function_handlers.get(function_name, None)):
             handler.update(value_str)
             self._call_registered_update_callbacks(function_name, handler.value)
 
     def _put(self, function_name: str, value: str):
         if self._connection:
             self._connection.put(self.id, function_name, value)
```

### Comparing `ynca-5.8.0/ynca/subunits/__init__.py` & `ynca-5.9.0/ynca/subunits/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,53 +4,53 @@
 from ..function import Cmd, EnumFunction, FloatFunction, StrFunction
 from ..enums import Playback, PlaybackInfo, Repeat, Shuffle
 from ..helpers import number_to_string_with_stepsize
 from ..subunit import SubunitBase
 
 
 class AlbumFunction:
-    album = StrFunction("ALBUM", Cmd.GET, init="METAINFO")
+    album = StrFunction(Cmd.GET, init="METAINFO")
 
 
 class ArtistFunction:
-    artist = StrFunction("ARTIST", Cmd.GET, init="METAINFO")
+    artist = StrFunction(Cmd.GET, init="METAINFO")
 
 
 class ChNameFunction:
-    chname = StrFunction("CHNAME", Cmd.GET, init="METAINFO")
+    chname = StrFunction(Cmd.GET, init="METAINFO")
 
 
 class PlaybackFunction:
     def playback(self, parameter: Playback):
         """Change playback state"""
         self._put("PLAYBACK", parameter)  # type: ignore
 
 
 class PlaybackInfoFunction:
-    playbackinfo = EnumFunction[PlaybackInfo]("PLAYBACKINFO", PlaybackInfo, Cmd.GET)
+    playbackinfo = EnumFunction[PlaybackInfo](PlaybackInfo, Cmd.GET)
 
 
 class RepeatFunction:
-    repeat = EnumFunction[Repeat]("REPEAT", Repeat)
+    repeat = EnumFunction[Repeat](Repeat)
 
 
 class ShuffleFunction:
-    shuffle = EnumFunction[Shuffle]("SHUFFLE", Shuffle)
+    shuffle = EnumFunction[Shuffle](Shuffle)
 
 
 class SongFunction:
-    song = StrFunction("SONG", Cmd.GET, init="METAINFO")
+    song = StrFunction(Cmd.GET, init="METAINFO")
 
 
 class StationFunction:
-    station = StrFunction("STATION", Cmd.GET)
+    station = StrFunction(Cmd.GET)
 
 
 class TrackFunction:
-    track = StrFunction("TRACK", Cmd.GET, init="METAINFO")
+    track = StrFunction(Cmd.GET, init="METAINFO")
 
 
 # A number of subunits have the same/similar featureset
 # so make a common base that only needs to be tested once
 class MediaPlaybackSubunitBase(
     PlaybackFunction,
     PlaybackInfoFunction,
@@ -62,13 +62,12 @@
     SubunitBase,
 ):
     pass
 
 
 class FmFreqFunction:
     fmfreq = FloatFunction(
-        "FMFREQ",
         converter=FloatConverter(
             to_str=lambda v: number_to_string_with_stepsize(v, 2, 0.2)
         ),
     )
     """Read/write FM frequency. Values will be aligned to a valid stepsize."""
```

### Comparing `ynca-5.8.0/ynca/subunits/dab.py` & `ynca-5.9.0/ynca/subunits/tun.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 from __future__ import annotations
 
 from ..constants import Subunit
-from ..function import Cmd, EnumFunction, StrFunction
-from ..enums import (
-    BandDab,
-)
+from ..converters import IntConverter
+from ..function import Cmd, EnumFunction, IntFunction, StrFunction
+from ..enums import BandTun
+from ..helpers import number_to_string_with_stepsize
 from ..subunit import SubunitBase
 from . import FmFreqFunction
 
 
-class Dab(SubunitBase, FmFreqFunction):
-    id = Subunit.DAB
+class Tun(SubunitBase, FmFreqFunction):
+    id = Subunit.TUN
 
-    band = EnumFunction[BandDab]("BAND", BandDab)
+    band = EnumFunction[BandTun](BandTun)
 
-    dabchlabel = StrFunction("DABCHLABEL", Cmd.GET)
-    dabdlslabel = StrFunction("DABDLSLABEL", Cmd.GET)
-    dabensemblelabel = StrFunction("DABENSEMBLELABEL", Cmd.GET)
-    dabservicelabel = StrFunction("DABSERVICELABEL", Cmd.GET)
-    dabprgtype = StrFunction("DABPRGTYPE", Cmd.GET)
-
-    fmrdsprgservice = StrFunction("FMRDSPRGSERVICE", Cmd.GET, init="FMRDSINFO")
-    fmrdsprgtype = StrFunction("FMRDSPRGTYPE", Cmd.GET, init="FMRDSINFO")
-    fmrdstxt = StrFunction("FMRDSTXT", Cmd.GET, init="FMRDSINFO")
+    amfreq = IntFunction(
+        converter=IntConverter(
+            to_str=lambda v: number_to_string_with_stepsize(v, 0, 10)
+        ),
+    )
+    """Read/write AM frequency. Values will be aligned to a valid stepsize."""
+
+    rdsprgservice = StrFunction(Cmd.GET, init="RDSINFO")
+    rdsprgtype = StrFunction(Cmd.GET, init="RDSINFO")
+    rdstxta = StrFunction(Cmd.GET, init="RDSINFO")
+    rdstxtb = StrFunction(Cmd.GET, init="RDSINFO")
```

### Comparing `ynca-5.8.0/ynca/subunits/pandora.py` & `ynca-5.9.0/ynca/subunits/pandora.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,12 +15,12 @@
 
 class Pandora(
     PlaybackFunction,
     PlaybackInfoFunction,
     ArtistFunction,
     AlbumFunction,
     SongFunction,
-    TrackFunction,    # Pandora seems to use TRACK or SONG for title based on logs. Maybe depends on firmware version?
+    TrackFunction,  # Pandora seems to use TRACK or SONG for title based on logs. Maybe depends on firmware version?
     StationFunction,
     SubunitBase,
 ):
     id = Subunit.PANDORA
```

### Comparing `ynca-5.8.0/ynca/subunits/sirius.py` & `ynca-5.9.0/ynca/subunits/sirius.py`

 * *Files identical despite different names*

### Comparing `ynca-5.8.0/ynca/subunits/system.py` & `ynca-5.9.0/ynca/subunits/system.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,49 +8,49 @@
 
 logger = logging.getLogger(__name__)
 
 
 class System(SubunitBase):
     id = Subunit.SYS
 
-    hdmiout1 = EnumFunction[HdmiOutOnOff]("HDMIOUT1", HdmiOutOnOff)
-    hdmiout2 = EnumFunction[HdmiOutOnOff]("HDMIOUT2", HdmiOutOnOff)
-    hdmiout3 = EnumFunction[HdmiOutOnOff]("HDMIOUT3", HdmiOutOnOff)
-    inpnameaudio1 = StrFunction("INPNAMEAUDIO1", Cmd.GET, init="INPNAME")
-    inpnameaudio2 = StrFunction("INPNAMEAUDIO2", Cmd.GET, init="INPNAME")
-    inpnameaudio3 = StrFunction("INPNAMEAUDIO3", Cmd.GET, init="INPNAME")
-    inpnameaudio4 = StrFunction("INPNAMEAUDIO4", Cmd.GET, init="INPNAME")
-    inpnameav1 = StrFunction("INPNAMEAV1", Cmd.GET, init="INPNAME")
-    inpnameav2 = StrFunction("INPNAMEAV2", Cmd.GET, init="INPNAME")
-    inpnameav3 = StrFunction("INPNAMEAV3", Cmd.GET, init="INPNAME")
-    inpnameav4 = StrFunction("INPNAMEAV4", Cmd.GET, init="INPNAME")
-    inpnameav5 = StrFunction("INPNAMEAV5", Cmd.GET, init="INPNAME")
-    inpnameav6 = StrFunction("INPNAMEAV6", Cmd.GET, init="INPNAME")
-    inpnameav7 = StrFunction("INPNAMEAV7", Cmd.GET, init="INPNAME")
-    inpnamedock = StrFunction("INPNAMEDOCK", Cmd.GET, init="INPNAME")
-    inpnamehdmi1 = StrFunction("INPNAMEHDMI1", Cmd.GET, init="INPNAME")
-    inpnamehdmi2 = StrFunction("INPNAMEHDMI2", Cmd.GET, init="INPNAME")
-    inpnamehdmi3 = StrFunction("INPNAMEHDMI3", Cmd.GET, init="INPNAME")
-    inpnamehdmi4 = StrFunction("INPNAMEHDMI4", Cmd.GET, init="INPNAME")
-    inpnamehdmi5 = StrFunction("INPNAMEHDMI5", Cmd.GET, init="INPNAME")
-    inpnamehdmi6 = StrFunction("INPNAMEHDMI6", Cmd.GET, init="INPNAME")
-    inpnamehdmi7 = StrFunction("INPNAMEHDMI7", Cmd.GET, init="INPNAME")
-    inpnamemultich = StrFunction("INPNAMEMULTICH", Cmd.GET, init="INPNAME")
-    inpnamephono = StrFunction("INPNAMEPHONO", Cmd.GET, init="INPNAME")
-    inpnameusb = StrFunction("INPNAMEUSB", Cmd.GET, init="INPNAME")
-    inpnamevaux = StrFunction("INPNAMEVAUX", Cmd.GET, init="INPNAME")
-    modelname = StrFunction("MODELNAME", Cmd.GET)
-    party = EnumFunction[Party]("PARTY", Party)
-    partymute = EnumFunction[PartyMute]("PARTYMUTE", PartyMute, Cmd.PUT)
-    pwr = EnumFunction[Pwr]("PWR", Pwr)
+    hdmiout1 = EnumFunction[HdmiOutOnOff](HdmiOutOnOff)
+    hdmiout2 = EnumFunction[HdmiOutOnOff](HdmiOutOnOff)
+    hdmiout3 = EnumFunction[HdmiOutOnOff](HdmiOutOnOff)
+    inpnameaudio1 = StrFunction(Cmd.GET, init="INPNAME")
+    inpnameaudio2 = StrFunction(Cmd.GET, init="INPNAME")
+    inpnameaudio3 = StrFunction(Cmd.GET, init="INPNAME")
+    inpnameaudio4 = StrFunction(Cmd.GET, init="INPNAME")
+    inpnameav1 = StrFunction(Cmd.GET, init="INPNAME")
+    inpnameav2 = StrFunction(Cmd.GET, init="INPNAME")
+    inpnameav3 = StrFunction(Cmd.GET, init="INPNAME")
+    inpnameav4 = StrFunction(Cmd.GET, init="INPNAME")
+    inpnameav5 = StrFunction(Cmd.GET, init="INPNAME")
+    inpnameav6 = StrFunction(Cmd.GET, init="INPNAME")
+    inpnameav7 = StrFunction(Cmd.GET, init="INPNAME")
+    inpnamedock = StrFunction(Cmd.GET, init="INPNAME")
+    inpnamehdmi1 = StrFunction(Cmd.GET, init="INPNAME")
+    inpnamehdmi2 = StrFunction(Cmd.GET, init="INPNAME")
+    inpnamehdmi3 = StrFunction(Cmd.GET, init="INPNAME")
+    inpnamehdmi4 = StrFunction(Cmd.GET, init="INPNAME")
+    inpnamehdmi5 = StrFunction(Cmd.GET, init="INPNAME")
+    inpnamehdmi6 = StrFunction(Cmd.GET, init="INPNAME")
+    inpnamehdmi7 = StrFunction(Cmd.GET, init="INPNAME")
+    inpnamemultich = StrFunction(Cmd.GET, init="INPNAME")
+    inpnamephono = StrFunction(Cmd.GET, init="INPNAME")
+    inpnameusb = StrFunction(Cmd.GET, init="INPNAME")
+    inpnamevaux = StrFunction(Cmd.GET, init="INPNAME")
+    modelname = StrFunction(Cmd.GET)
+    party = EnumFunction[Party](Party)
+    partymute = EnumFunction[PartyMute](PartyMute, Cmd.PUT)
+    pwr = EnumFunction[Pwr](Pwr)
 
     # No_initialize VERSION to avoid it being sent during initialization
     # It is also used behind the scenes for syncing and would interfere
     version = FunctionBase[str](
-        "VERSION", converter=StrConverter(), cmd=Cmd.GET, no_initialize=True
+        converter=StrConverter(), cmd=Cmd.GET, no_initialize=True
     )
 
     def partyvol_up(self):
         """
         Increase the party volume with one step.
         """
         self._put("PARTYVOL", "Up")
```

### Comparing `ynca-5.8.0/ynca/subunits/zone.py` & `ynca-5.9.0/ynca/subunits/zone.py`

 * *Files 24% similar despite different names*

```diff
@@ -40,97 +40,92 @@
 
 
 class ZoneBase(PlaybackFunction, SubunitBase):
 
     # BASIC gets a lot of attribute like PWR, SLEEP, VOL, MUTE, INP, STRAIGHT, ENHANCER, SOUNDPRG and more
     # Use it to significantly reduce the amount of commands to send
 
-    adaptivedrc = EnumFunction[AdaptiveDrc]("ADAPTIVEDRC", AdaptiveDrc)
-    enhancer = EnumFunction[Enhancer]("ENHANCER", Enhancer)
-    hdmiout = EnumFunction[HdmiOut]("HDMIOUT", HdmiOut)
+    adaptivedrc = EnumFunction[AdaptiveDrc](AdaptiveDrc)
+    enhancer = EnumFunction[Enhancer](Enhancer)
+    hdmiout = EnumFunction[HdmiOut](HdmiOut)
     hpbass = FloatFunction(
-        "HPBASS",
         converter=FloatConverter(
             to_str=lambda v: number_to_string_with_stepsize(v, 1, 0.5)
         ),
     )
     hptreble = FloatFunction(
-        "HPTREBLE",
         converter=FloatConverter(
             to_str=lambda v: number_to_string_with_stepsize(v, 1, 0.5)
         ),
     )
     initvollvl = EnumOrFloatFunction[InitVolLvl](
-        "INITVOLLVL",
         InitVolLvl,
         MultiConverter(
             [
                 FloatConverter(
                     to_str=lambda v: number_to_string_with_stepsize(v, 1, 0.5)
                 ),
                 EnumConverter[InitVolLvl](InitVolLvl),
             ]
         ),
     )
-    initvolmode = EnumFunction[InitVolMode]("INITVOLMODE", InitVolMode)
-    inp = EnumFunction[Input]("INP", Input, init="BASIC")
+    initvolmode = EnumFunction[InitVolMode](InitVolMode)
+    inp = EnumFunction[Input](Input, init="BASIC")
     maxvol = FloatFunction(
-        "MAXVOL",
         converter=MultiConverter(
             [
                 # Special handling for 16.5 which is valid, but does not fit stepsize of 5
                 FloatConverter(
                     to_str=lambda v: "16.5" if v == 16.5 else raiser(ValueError)
                 ),
                 FloatConverter(
                     to_str=lambda v: number_to_string_with_stepsize(v, 1, 5)
                 ),
             ]
         ),
     )
-    mute = EnumFunction[Mute]("MUTE", Mute, init="BASIC")
-    puredirmode = EnumFunction[PureDirMode]("PUREDIRMODE", PureDirMode, init="BASIC")
-    pwr = EnumFunction[Pwr]("PWR", Pwr, init="BASIC")
-    scene1name = StrFunction("SCENE1NAME", Cmd.GET, init="SCENENAME")
-    scene2name = StrFunction("SCENE2NAME", Cmd.GET, init="SCENENAME")
-    scene3name = StrFunction("SCENE3NAME", Cmd.GET, init="SCENENAME")
-    scene4name = StrFunction("SCENE4NAME", Cmd.GET, init="SCENENAME")
-    scene5name = StrFunction("SCENE5NAME", Cmd.GET, init="SCENENAME")
-    scene6name = StrFunction("SCENE6NAME", Cmd.GET, init="SCENENAME")
-    scene7name = StrFunction("SCENE7NAME", Cmd.GET, init="SCENENAME")
-    scene8name = StrFunction("SCENE8NAME", Cmd.GET, init="SCENENAME")
-    scene9name = StrFunction("SCENE9NAME", Cmd.GET, init="SCENENAME")
-    scene10name = StrFunction("SCENE10NAME", Cmd.GET, init="SCENENAME")
-    scene11name = StrFunction("SCENE11NAME", Cmd.GET, init="SCENENAME")
-    scene12name = StrFunction("SCENE12NAME", Cmd.GET, init="SCENENAME")
-    sleep = EnumFunction[Sleep]("SLEEP", Sleep)
-    soundprg = EnumFunction[SoundPrg]("SOUNDPRG", SoundPrg, init="BASIC")
+    mute = EnumFunction[Mute](Mute, init="BASIC")
+    puredirmode = EnumFunction[PureDirMode](PureDirMode, init="BASIC")
+    pwr = EnumFunction[Pwr](Pwr, init="BASIC")
+    scene1name = StrFunction(Cmd.GET, init="SCENENAME")
+    scene2name = StrFunction(Cmd.GET, init="SCENENAME")
+    scene3name = StrFunction(Cmd.GET, init="SCENENAME")
+    scene4name = StrFunction(Cmd.GET, init="SCENENAME")
+    scene5name = StrFunction(Cmd.GET, init="SCENENAME")
+    scene6name = StrFunction(Cmd.GET, init="SCENENAME")
+    scene7name = StrFunction(Cmd.GET, init="SCENENAME")
+    scene8name = StrFunction(Cmd.GET, init="SCENENAME")
+    scene9name = StrFunction(Cmd.GET, init="SCENENAME")
+    scene10name = StrFunction(Cmd.GET, init="SCENENAME")
+    scene11name = StrFunction(Cmd.GET, init="SCENENAME")
+    scene12name = StrFunction(Cmd.GET, init="SCENENAME")
+    sleep = EnumFunction[Sleep](Sleep)
+    soundprg = EnumFunction[SoundPrg](SoundPrg, init="BASIC")
     spbass = FloatFunction(
-        "SPBASS",
         converter=FloatConverter(
             to_str=lambda v: number_to_string_with_stepsize(v, 1, 0.5)
         ),
     )
     sptreble = FloatFunction(
-        "SPTREBLE",
         converter=FloatConverter(
             to_str=lambda v: number_to_string_with_stepsize(v, 1, 0.5)
         ),
     )
-    straight = EnumFunction[Straight]("STRAIGHT", Straight, init="BASIC")
-    threedcinema = EnumFunction[ThreeDeeCinema]("3DCINEMA", ThreeDeeCinema)
-    twochdecoder = EnumFunction[TwoChDecoder]("2CHDECODER", TwoChDecoder)
+    straight = EnumFunction[Straight](Straight, init="BASIC")
+    threedcinema = EnumFunction[ThreeDeeCinema](
+        ThreeDeeCinema, name_override="3DCINEMA"
+    )
+    twochdecoder = EnumFunction[TwoChDecoder](TwoChDecoder, name_override="2CHDECODER")
     vol = FloatFunction(
-        "VOL",
         converter=FloatConverter(
             to_str=lambda v: number_to_string_with_stepsize(v, 1, 0.5)
         ),
         init="BASIC",
     )
-    zonename = StrFunction("ZONENAME", converter=StrConverter(min_len=0, max_len=9))
+    zonename = StrFunction(converter=StrConverter(min_len=0, max_len=9))
 
     def scene(self, scene_id: int | str):
         """Recall a scene"""
         self._put("SCENE", f"Scene {scene_id}")
 
     def vol_up(self, step_size: float = 0.5):
         """
```

### Comparing `ynca-5.8.0/ynca/terminal.py` & `ynca-5.9.0/ynca/terminal.py`

 * *Files identical despite different names*

### Comparing `ynca-5.8.0/ynca.egg-info/PKG-INFO` & `ynca-5.9.0/ynca.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ynca
-Version: 5.8.0
+Version: 5.9.0
 Summary: Package to control Yamaha receivers that support the YNCA protocol.
 Home-page: https://github.com/mvdwetering/ynca
 Author: Michel van de Wetering
 Author-email: michel.van.de.wetering+ynca@gmail.com
 License: MIT
 Keywords: automation
 Classifier: Development Status :: 5 - Production/Stable
@@ -20,29 +20,29 @@
 # YNCA
 
 Package to control Yamaha receivers that support the YNCA protocol.
 
 According to reports of users and info found on the internet the following receivers should work.
 There might be more receivers that support this protocol. If you find some let met know so the list can be updated.
 
-> HTR-4071, RX-A700, RX-A710, RX-A720, RX-A740, RX-A800, RX-A810, RX-A820, RX-A840, RX-A850, RX-A1000, RX-A1010, RX-A1020, RX-A1030, RX-A1040, RX-A2000, RX-A2010, RX-A2020, RX-A2070, RX-A3000, RX-A3010, RX-A3020, RX-V475, RX-V477, RX-V483, RX-V671, RX-V673, RX-V675, RX-V677, RX-V771, RX-V773, RX-V777, RX-V867, RX-V871, RX-V1067, RX-V2067, RX-V3067, TSR-700, TSR-7850
+> HTR-4065, HTR-4071, HTR-6064, RX-A660, RX-A700, RX-A710, RX-A720, RX-A740, RX-A750, RX-A800, RX-A810, RX-A820, RX-A840, RX-A850, RX-A1000, RX-A1010, RX-A1020, RX-A1030, RX-A1040, RX-A2000, RX-A2010, RX-A2020, RX-A2070, RX-A3000, RX-A3010, RX-A3020, RX-A3030, RX-A3070, RX-V475, RX-V477, RX-V481D, RX-V483, RX-V671, RX-V673, RX-V675, RX-V677, RX-V771, RX-V773, RX-V775, RX-V777, RX-V867, RX-V871, RX-V1067, RX-V1071, RX-V2067, RX-V2071, RX-V3067, RX-V3071, TSR-700, TSR-7850
 
-Note that there is a restriction that only 1 YNCA connection to a receiver can be made at the time (restriction on the receiver side, not this library).
+Note that only 1 YNCA connection to a receiver can be made at the time (restriction on the receiver side, not this library).
 Usually not a problem as the Yamaha AV Control App uses a different protocol which can be used at the same time, but something to be aware of when testing the library.
 
 
 ## Installation
 
 ```bash
 python3 -m pip install ynca
 ```
 
 ## Contents
 
-Note that the intended API to use is exposed from the toplevel package.
+The intended API to use is exposed from the toplevel package.
 
 ### Classes
 
 #### YncaApi
 
 This is the main class to interact with. The YncaApi class is exposing YNCA subunits and their functions as Python classes/datatypes and allows to connect to devices supporting that API. It keeps a cache which gets updated when values are received from the device so reading attributes is instant as it does not need to query the receiver.
 
@@ -69,15 +69,15 @@
 python3 -m ynca.terminal socket://192.168.178.21:50000
 ```
 
 #### YNCA Server
 
 This is a very basic YNCA server intended to be just enough for debugging and testing without connecting to a real device.
 
-Note that the server needs to be filled with data from an actual device and it will basically just repeat the same answers as the real device gave (with a few exceptions).
+The server needs to be filled with data from an actual device and it will basically just repeat the same answers as the real device gave (with a few exceptions).
 Filling the server can be done by providing it with YNCA logging of a real device, like the ones in the YCNA package repository or a log from your own device e.g. by running `example.py` with loglevel DEBUG (uncomment the line in the example code).
 
 It has some additional commandline options for using different ports, binding to a specific host or testing disconnects
 
 ```
 python3 -m ynca.server <ynca_repo>/logs/RX-A810.txt
 python3 -m ynca.server --host localhost --port 12345 <ynca_repo>/logs/RX-A810.txt
@@ -92,15 +92,15 @@
 # Port could also be e.g. COM3 on Windows or any `serial_url` as supported by PySerial
 # Like for example `socket://192.168.178.21:50000` for IP connection
 receiver = YncaApi("/dev/tty1")
 
 # Initializing takes a while (~10 seconds for a 2 zone receiver) since it communicates
 # quite a lot with the actual device to determine its capabilities.
 # Later calls to the subunits are fast.
-# Note that attributes that are still None after initialization are not supported by the subunits
+# The attributes that are still None after initialization are not supported by the subunits
 receiver.initialize()
 
 # Every subunit has a dedicated attribute on the `YncaApi` class.
 # The name of the attribute is the subunit id as used in YNCA.
 # The returned subunit class can be used to communicate with the subunit
 sys = receiver.sys
 main = receiver.main
```

### Comparing `ynca-5.8.0/ynca.egg-info/SOURCES.txt` & `ynca-5.9.0/ynca.egg-info/SOURCES.txt`

 * *Files identical despite different names*

