# Comparing `tmp/SMsfan-1.2.0.tar.gz` & `tmp/SMsfan-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SMsfan-1.2.0.tar", last modified: Sat Apr  6 17:49:26 2024, max compression
+gzip compressed data, was "SMsfan-1.2.1.tar", last modified: Sat Apr  6 17:51:02 2024, max compression
```

## Comparing `SMsfan-1.2.0.tar` & `SMsfan-1.2.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2024-04-06 17:49:26.149729 SMsfan-1.2.0/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1086 2024-04-06 17:26:53.000000 SMsfan-1.2.0/LICENSE
--rw-r--r--   0 vlad      (1000) vlad      (1000)      843 2024-04-06 17:49:26.149729 SMsfan-1.2.0/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2761 2024-04-06 17:26:53.000000 SMsfan-1.2.0/README.md
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2024-04-06 17:49:26.149729 SMsfan-1.2.0/SMsfan/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     5166 2024-04-06 17:47:26.000000 SMsfan-1.2.0/SMsfan/__init__.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2024-04-06 17:49:26.149729 SMsfan-1.2.0/SMsfan.egg-info/
--rw-r--r--   0 vlad      (1000) vlad      (1000)      843 2024-04-06 17:49:26.000000 SMsfan-1.2.0/SMsfan.egg-info/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)      204 2024-04-06 17:49:26.000000 SMsfan-1.2.0/SMsfan.egg-info/SOURCES.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2024-04-06 17:49:26.000000 SMsfan-1.2.0/SMsfan.egg-info/dependency_links.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)       15 2024-04-06 17:49:26.000000 SMsfan-1.2.0/SMsfan.egg-info/requires.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        7 2024-04-06 17:49:26.000000 SMsfan-1.2.0/SMsfan.egg-info/top_level.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)       67 2024-04-06 17:49:26.149729 SMsfan-1.2.0/setup.cfg
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1259 2024-04-06 17:48:30.000000 SMsfan-1.2.0/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2024-04-06 17:51:02.111820 SMsfan-1.2.1/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1086 2024-04-06 17:26:53.000000 SMsfan-1.2.1/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      844 2024-04-06 17:51:02.108486 SMsfan-1.2.1/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2761 2024-04-06 17:26:53.000000 SMsfan-1.2.1/README.md
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2024-04-06 17:51:02.108486 SMsfan-1.2.1/SMsfan/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     5166 2024-04-06 17:47:26.000000 SMsfan-1.2.1/SMsfan/__init__.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2024-04-06 17:51:02.108486 SMsfan-1.2.1/SMsfan.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      844 2024-04-06 17:51:02.000000 SMsfan-1.2.1/SMsfan.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      204 2024-04-06 17:51:02.000000 SMsfan-1.2.1/SMsfan.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2024-04-06 17:51:02.000000 SMsfan-1.2.1/SMsfan.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       16 2024-04-06 17:51:02.000000 SMsfan-1.2.1/SMsfan.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        7 2024-04-06 17:51:02.000000 SMsfan-1.2.1/SMsfan.egg-info/top_level.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       67 2024-04-06 17:51:02.111820 SMsfan-1.2.1/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1260 2024-04-06 17:50:59.000000 SMsfan-1.2.1/setup.py
```

### Comparing `SMsfan-1.2.0/LICENSE` & `SMsfan-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `SMsfan-1.2.0/PKG-INFO` & `SMsfan-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SMsfan
-Version: 1.2.0
+Version: 1.2.1
 Summary: Library to control Multi-IO Automation Card
 Home-page: https://sequentmicrosystems.com
 Author: Sequent Microsystems
 Author-email: olcitu@gmail.com
 License: MIT
 Keywords: industrial,raspberry,power,4-20mA,0-10V,optoisolated
 Classifier: Development Status :: 3 - Alpha
@@ -14,9 +14,9 @@
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 License-File: LICENSE
-Requires-Dist: smbus
+Requires-Dist: smbus2
 Requires-Dist: RPi.GPIO
```

### Comparing `SMsfan-1.2.0/README.md` & `SMsfan-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `SMsfan-1.2.0/SMsfan/__init__.py` & `SMsfan-1.2.1/SMsfan/__init__.py`

 * *Files identical despite different names*

### Comparing `SMsfan-1.2.0/SMsfan.egg-info/PKG-INFO` & `SMsfan-1.2.1/SMsfan.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SMsfan
-Version: 1.2.0
+Version: 1.2.1
 Summary: Library to control Multi-IO Automation Card
 Home-page: https://sequentmicrosystems.com
 Author: Sequent Microsystems
 Author-email: olcitu@gmail.com
 License: MIT
 Keywords: industrial,raspberry,power,4-20mA,0-10V,optoisolated
 Classifier: Development Status :: 3 - Alpha
@@ -14,9 +14,9 @@
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 License-File: LICENSE
-Requires-Dist: smbus
+Requires-Dist: smbus2
 Requires-Dist: RPi.GPIO
```

### Comparing `SMsfan-1.2.0/setup.py` & `SMsfan-1.2.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,25 +2,25 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='SMsfan',
     packages=setuptools.find_packages(),
-    version='1.2.0',
+    version='1.2.1',
     license='MIT',
     description='Library to control Multi-IO Automation Card',
     #long_description=long_description,
     #long_description_content_type="text/markdown",
     author='Sequent Microsystems',
     author_email='olcitu@gmail.com',
     url='https://sequentmicrosystems.com',
     keywords=['industrial', 'raspberry', 'power', '4-20mA', '0-10V', 'optoisolated'],
     install_requires=[
-        "smbus",
+        "smbus2",
         "RPi.GPIO",
         ],
     classifiers=[
         'Development Status :: 3 - Alpha',
         # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
         'Intended Audience :: Developers',
         'Topic :: Software Development :: Build Tools',
```

