# Comparing `tmp/SMsfan-1.2.2.tar.gz` & `tmp/SMsfan-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SMsfan-1.2.2.tar", last modified: Sat Apr  6 17:58:07 2024, max compression
+gzip compressed data, was "SMsfan-1.2.3.tar", last modified: Sat Apr  6 17:59:30 2024, max compression
```

## Comparing `SMsfan-1.2.2.tar` & `SMsfan-1.2.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2024-04-06 17:58:07.802981 SMsfan-1.2.2/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1086 2024-04-06 17:26:53.000000 SMsfan-1.2.2/LICENSE
--rw-r--r--   0 vlad      (1000) vlad      (1000)      844 2024-04-06 17:58:07.802981 SMsfan-1.2.2/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2761 2024-04-06 17:26:53.000000 SMsfan-1.2.2/README.md
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2024-04-06 17:58:07.802981 SMsfan-1.2.2/SMsfan/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     5211 2024-04-06 17:56:23.000000 SMsfan-1.2.2/SMsfan/__init__.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2024-04-06 17:58:07.802981 SMsfan-1.2.2/SMsfan.egg-info/
--rw-r--r--   0 vlad      (1000) vlad      (1000)      844 2024-04-06 17:58:07.000000 SMsfan-1.2.2/SMsfan.egg-info/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)      204 2024-04-06 17:58:07.000000 SMsfan-1.2.2/SMsfan.egg-info/SOURCES.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2024-04-06 17:58:07.000000 SMsfan-1.2.2/SMsfan.egg-info/dependency_links.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)       16 2024-04-06 17:58:07.000000 SMsfan-1.2.2/SMsfan.egg-info/requires.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        7 2024-04-06 17:58:07.000000 SMsfan-1.2.2/SMsfan.egg-info/top_level.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)       67 2024-04-06 17:58:07.802981 SMsfan-1.2.2/setup.cfg
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1260 2024-04-06 17:57:38.000000 SMsfan-1.2.2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2024-04-06 17:59:30.591911 SMsfan-1.2.3/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1086 2024-04-06 17:26:53.000000 SMsfan-1.2.3/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      844 2024-04-06 17:59:30.591911 SMsfan-1.2.3/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2761 2024-04-06 17:26:53.000000 SMsfan-1.2.3/README.md
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2024-04-06 17:59:30.591911 SMsfan-1.2.3/SMsfan/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     5213 2024-04-06 17:59:10.000000 SMsfan-1.2.3/SMsfan/__init__.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2024-04-06 17:59:30.591911 SMsfan-1.2.3/SMsfan.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      844 2024-04-06 17:59:30.000000 SMsfan-1.2.3/SMsfan.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      204 2024-04-06 17:59:30.000000 SMsfan-1.2.3/SMsfan.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2024-04-06 17:59:30.000000 SMsfan-1.2.3/SMsfan.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       16 2024-04-06 17:59:30.000000 SMsfan-1.2.3/SMsfan.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        7 2024-04-06 17:59:30.000000 SMsfan-1.2.3/SMsfan.egg-info/top_level.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       67 2024-04-06 17:59:30.591911 SMsfan-1.2.3/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1260 2024-04-06 17:59:29.000000 SMsfan-1.2.3/setup.py
```

### Comparing `SMsfan-1.2.2/LICENSE` & `SMsfan-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `SMsfan-1.2.2/PKG-INFO` & `SMsfan-1.2.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SMsfan
-Version: 1.2.2
+Version: 1.2.3
 Summary: Library to control Multi-IO Automation Card
 Home-page: https://sequentmicrosystems.com
 Author: Sequent Microsystems
 Author-email: olcitu@gmail.com
 License: MIT
 Keywords: industrial,raspberry,power,4-20mA,0-10V,optoisolated
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `SMsfan-1.2.2/README.md` & `SMsfan-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `SMsfan-1.2.2/SMsfan/__init__.py` & `SMsfan-1.2.3/SMsfan/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import smbus2
 import struct
-import RPi.GPIO as GPIO
+# import RPi.GPIO as GPIO
 
 # bus = smbus2.SMBus(1)    # 0 = /dev/i2c-0 (port I2C0), 1 = /dev/i2c-1 (port I2C1)
 
 DEVICE_ADDRESS = 0x03  # 7 bit address (will be left shifted to add the read write bit)
 DEVICE_ALT_ADDRESS = 0x2C
```

### Comparing `SMsfan-1.2.2/SMsfan.egg-info/PKG-INFO` & `SMsfan-1.2.3/SMsfan.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SMsfan
-Version: 1.2.2
+Version: 1.2.3
 Summary: Library to control Multi-IO Automation Card
 Home-page: https://sequentmicrosystems.com
 Author: Sequent Microsystems
 Author-email: olcitu@gmail.com
 License: MIT
 Keywords: industrial,raspberry,power,4-20mA,0-10V,optoisolated
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `SMsfan-1.2.2/setup.py` & `SMsfan-1.2.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='SMsfan',
     packages=setuptools.find_packages(),
-    version='1.2.2',
+    version='1.2.3',
     license='MIT',
     description='Library to control Multi-IO Automation Card',
     #long_description=long_description,
     #long_description_content_type="text/markdown",
     author='Sequent Microsystems',
     author_email='olcitu@gmail.com',
     url='https://sequentmicrosystems.com',
```

