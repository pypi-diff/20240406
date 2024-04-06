# Comparing `tmp/abberior-sted-0.0.1.tar.gz` & `tmp/abberior-sted-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abberior-sted-0.0.1.tar", last modified: Sat Mar 23 08:55:15 2024, max compression
+gzip compressed data, was "abberior-sted-0.0.2.tar", last modified: Sat Apr  6 11:45:58 2024, max compression
```

## Comparing `abberior-sted-0.0.1.tar` & `abberior-sted-0.0.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 Anthony    (501) staff       (20)        0 2024-03-23 08:55:15.057863 abberior-sted-0.0.1/
--rw-r--r--   0 Anthony    (501) staff       (20)    18650 2024-03-23 08:17:28.000000 abberior-sted-0.0.1/LICENSE
--rw-r--r--   0 Anthony    (501) staff       (20)       33 2024-03-21 20:25:19.000000 abberior-sted-0.0.1/MANIFEST.in
--rw-r--r--   0 Anthony    (501) staff       (20)     2065 2024-03-23 08:55:15.056659 abberior-sted-0.0.1/PKG-INFO
--rw-r--r--   0 Anthony    (501) staff       (20)     1253 2024-03-23 08:09:51.000000 abberior-sted-0.0.1/README.md
-drwxr-xr-x   0 Anthony    (501) staff       (20)        0 2024-03-23 08:55:15.043495 abberior-sted-0.0.1/abberior/
--rw-r--r--   0 Anthony    (501) staff       (20)       39 2024-03-21 20:25:19.000000 abberior-sted-0.0.1/abberior/__init__.py
-drwxr-xr-x   0 Anthony    (501) staff       (20)        0 2024-03-23 08:55:15.044499 abberior-sted-0.0.1/abberior/config/
--rw-r--r--   0 Anthony    (501) staff       (20)    52581 2024-03-21 20:25:19.000000 abberior-sted-0.0.1/abberior/config/conf.yml
-drwxr-xr-x   0 Anthony    (501) staff       (20)        0 2024-03-23 08:55:15.046719 abberior-sted-0.0.1/abberior/debug/
--rw-r--r--   0 Anthony    (501) staff       (20)    52557 2024-03-21 20:25:19.000000 abberior-sted-0.0.1/abberior/debug/conf.yml
--rw-r--r--   0 Anthony    (501) staff       (20)    25406 2024-03-23 08:09:17.000000 abberior-sted-0.0.1/abberior/microscope.py
--rw-r--r--   0 Anthony    (501) staff       (20)    24269 2024-03-21 20:25:19.000000 abberior-sted-0.0.1/abberior/user.py
--rw-r--r--   0 Anthony    (501) staff       (20)     5835 2024-03-21 20:25:19.000000 abberior-sted-0.0.1/abberior/utils.py
-drwxr-xr-x   0 Anthony    (501) staff       (20)        0 2024-03-23 08:55:15.055162 abberior-sted-0.0.1/abberior_sted.egg-info/
--rw-r--r--   0 Anthony    (501) staff       (20)     2065 2024-03-23 08:55:15.000000 abberior-sted-0.0.1/abberior_sted.egg-info/PKG-INFO
--rw-r--r--   0 Anthony    (501) staff       (20)      350 2024-03-23 08:55:15.000000 abberior-sted-0.0.1/abberior_sted.egg-info/SOURCES.txt
--rw-r--r--   0 Anthony    (501) staff       (20)        1 2024-03-23 08:55:15.000000 abberior-sted-0.0.1/abberior_sted.egg-info/dependency_links.txt
--rw-r--r--   0 Anthony    (501) staff       (20)       43 2024-03-23 08:55:15.000000 abberior-sted-0.0.1/abberior_sted.egg-info/requires.txt
--rw-r--r--   0 Anthony    (501) staff       (20)        9 2024-03-23 08:55:15.000000 abberior-sted-0.0.1/abberior_sted.egg-info/top_level.txt
--rw-r--r--   0 Anthony    (501) staff       (20)       38 2024-03-23 08:55:15.058208 abberior-sted-0.0.1/setup.cfg
--rw-r--r--   0 Anthony    (501) staff       (20)     1108 2024-03-23 08:53:52.000000 abberior-sted-0.0.1/setup.py
+drwxr-xr-x   0 Anthony    (501) staff       (20)        0 2024-04-06 11:45:58.383500 abberior-sted-0.0.2/
+-rw-r--r--   0 Anthony    (501) staff       (20)    18650 2024-03-23 08:17:28.000000 abberior-sted-0.0.2/LICENSE
+-rw-r--r--   0 Anthony    (501) staff       (20)       33 2024-03-21 20:25:19.000000 abberior-sted-0.0.2/MANIFEST.in
+-rw-r--r--   0 Anthony    (501) staff       (20)     2194 2024-04-06 11:45:58.382341 abberior-sted-0.0.2/PKG-INFO
+-rw-r--r--   0 Anthony    (501) staff       (20)     1253 2024-03-23 08:09:51.000000 abberior-sted-0.0.2/README.md
+drwxr-xr-x   0 Anthony    (501) staff       (20)        0 2024-04-06 11:45:58.372535 abberior-sted-0.0.2/abberior/
+-rw-r--r--   0 Anthony    (501) staff       (20)       39 2024-03-21 20:25:19.000000 abberior-sted-0.0.2/abberior/__init__.py
+drwxr-xr-x   0 Anthony    (501) staff       (20)        0 2024-04-06 11:45:58.373376 abberior-sted-0.0.2/abberior/config/
+-rw-r--r--   0 Anthony    (501) staff       (20)    52581 2024-03-21 20:25:19.000000 abberior-sted-0.0.2/abberior/config/conf.yml
+drwxr-xr-x   0 Anthony    (501) staff       (20)        0 2024-04-06 11:45:58.375077 abberior-sted-0.0.2/abberior/debug/
+-rw-r--r--   0 Anthony    (501) staff       (20)    52557 2024-03-21 20:25:19.000000 abberior-sted-0.0.2/abberior/debug/conf.yml
+-rw-r--r--   0 Anthony    (501) staff       (20)    25406 2024-03-23 08:09:17.000000 abberior-sted-0.0.2/abberior/microscope.py
+-rw-r--r--   0 Anthony    (501) staff       (20)    24269 2024-03-21 20:25:19.000000 abberior-sted-0.0.2/abberior/user.py
+-rw-r--r--   0 Anthony    (501) staff       (20)     5835 2024-03-21 20:25:19.000000 abberior-sted-0.0.2/abberior/utils.py
+drwxr-xr-x   0 Anthony    (501) staff       (20)        0 2024-04-06 11:45:58.381227 abberior-sted-0.0.2/abberior_sted.egg-info/
+-rw-r--r--   0 Anthony    (501) staff       (20)     2194 2024-04-06 11:45:58.000000 abberior-sted-0.0.2/abberior_sted.egg-info/PKG-INFO
+-rw-r--r--   0 Anthony    (501) staff       (20)      350 2024-04-06 11:45:58.000000 abberior-sted-0.0.2/abberior_sted.egg-info/SOURCES.txt
+-rw-r--r--   0 Anthony    (501) staff       (20)        1 2024-04-06 11:45:58.000000 abberior-sted-0.0.2/abberior_sted.egg-info/dependency_links.txt
+-rw-r--r--   0 Anthony    (501) staff       (20)       43 2024-04-06 11:45:58.000000 abberior-sted-0.0.2/abberior_sted.egg-info/requires.txt
+-rw-r--r--   0 Anthony    (501) staff       (20)        9 2024-04-06 11:45:58.000000 abberior-sted-0.0.2/abberior_sted.egg-info/top_level.txt
+-rw-r--r--   0 Anthony    (501) staff       (20)       38 2024-04-06 11:45:58.383794 abberior-sted-0.0.2/setup.cfg
+-rw-r--r--   0 Anthony    (501) staff       (20)     1286 2024-04-06 11:45:00.000000 abberior-sted-0.0.2/setup.py
```

### Comparing `abberior-sted-0.0.1/LICENSE` & `abberior-sted-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `abberior-sted-0.0.1/PKG-INFO` & `abberior-sted-0.0.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 Metadata-Version: 2.1
 Name: abberior-sted
-Version: 0.0.1
+Version: 0.0.2
 Summary: Interface to Imspector control software for Abberior STED microscopes
 License: CC-BY-4.0 license
+Project-URL: Documentation, https://github.com/FLClab/Abberior-STED
+Project-URL: Source, https://github.com/FLClab/Abberior-STED
 Keywords: abberior sted imspector specpy
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `abberior-sted-0.0.1/README.md` & `abberior-sted-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `abberior-sted-0.0.1/abberior/config/conf.yml` & `abberior-sted-0.0.2/abberior/config/conf.yml`

 * *Files identical despite different names*

### Comparing `abberior-sted-0.0.1/abberior/debug/conf.yml` & `abberior-sted-0.0.2/abberior/debug/conf.yml`

 * *Files identical despite different names*

### Comparing `abberior-sted-0.0.1/abberior/microscope.py` & `abberior-sted-0.0.2/abberior/microscope.py`

 * *Files identical despite different names*

### Comparing `abberior-sted-0.0.1/abberior/user.py` & `abberior-sted-0.0.2/abberior/user.py`

 * *Files identical despite different names*

### Comparing `abberior-sted-0.0.1/abberior/utils.py` & `abberior-sted-0.0.2/abberior/utils.py`

 * *Files identical despite different names*

### Comparing `abberior-sted-0.0.1/abberior_sted.egg-info/PKG-INFO` & `abberior-sted-0.0.2/abberior_sted.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 Metadata-Version: 2.1
 Name: abberior-sted
-Version: 0.0.1
+Version: 0.0.2
 Summary: Interface to Imspector control software for Abberior STED microscopes
 License: CC-BY-4.0 license
+Project-URL: Documentation, https://github.com/FLClab/Abberior-STED
+Project-URL: Source, https://github.com/FLClab/Abberior-STED
 Keywords: abberior sted imspector specpy
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `abberior-sted-0.0.1/setup.py` & `abberior-sted-0.0.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 from setuptools import setup, find_packages
 
 setup(
     name='abberior-sted',
-    version='0.0.1',
+    version='0.0.2',
     description="Interface to Imspector control software for Abberior STED microscopes",
     long_description=open("README.md").read(),
     long_description_content_type='text/markdown',
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved",
         "Operating System :: OS Independent",
@@ -24,11 +24,15 @@
     install_requires=[
         "scikit-image",
         "numpy",
         "scipy",
         "matplotlib",
         "pyyaml"
     ],  # And any other dependencies foo needs
-    packages=["abberior"],
+    packages=find_packages(include=["abberior"]),
     include_package_data=True,
+    project_urls={
+        'Documentation': 'https://github.com/FLClab/Abberior-STED',
+        'Source': 'https://github.com/FLClab/Abberior-STED',
+    },
 )
 # I do not require specpy to be installed
```

