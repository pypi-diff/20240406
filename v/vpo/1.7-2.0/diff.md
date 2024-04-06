# Comparing `tmp/vpo-1.7.tar.gz` & `tmp/vpo-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vpo-1.7.tar", last modified: Sun Mar 17 20:09:32 2024, max compression
+gzip compressed data, was "vpo-2.0.tar", last modified: Sat Apr  6 08:47:41 2024, max compression
```

## Comparing `vpo-1.7.tar` & `vpo-2.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-03-17 20:09:32.927175 vpo-1.7/
--rw-rw-rw-   0        0        0     1090 2024-03-17 08:03:16.000000 vpo-1.7/LICENCE
--rw-rw-rw-   0        0        0      835 2024-03-17 20:09:32.925173 vpo-1.7/PKG-INFO
--rw-rw-rw-   0        0        0       47 2024-03-17 08:35:15.000000 vpo-1.7/README.md
--rw-rw-rw-   0        0        0       42 2024-03-17 20:09:32.927175 vpo-1.7/setup.cfg
--rw-rw-rw-   0        0        0      875 2024-03-17 20:09:19.000000 vpo-1.7/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-17 20:09:32.917559 vpo-1.7/vpo/
--rw-rw-rw-   0        0        0    33058 2024-03-17 20:09:03.000000 vpo-1.7/vpo/__init__.py
--rw-rw-rw-   0        0        0    43464 2024-03-17 18:08:38.000000 vpo-1.7/vpo/authkey.py
--rw-rw-rw-   0        0        0     2391 2024-03-17 18:08:40.000000 vpo-1.7/vpo/disc.py
--rw-rw-rw-   0        0        0     1531 2024-03-17 18:08:43.000000 vpo-1.7/vpo/others.py
-drwxrwxrwx   0        0        0        0 2024-03-17 20:09:32.924174 vpo-1.7/vpo.egg-info/
--rw-rw-rw-   0        0        0      835 2024-03-17 20:09:32.000000 vpo-1.7/vpo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      217 2024-03-17 20:09:32.000000 vpo-1.7/vpo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-17 20:09:32.000000 vpo-1.7/vpo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2024-03-17 20:09:32.000000 vpo-1.7/vpo.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2024-03-17 20:09:32.000000 vpo-1.7/vpo.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-06 08:47:41.793908 vpo-2.0/
+-rw-rw-rw-   0        0        0     1090 2024-03-17 08:03:16.000000 vpo-2.0/LICENCE
+-rw-rw-rw-   0        0        0      694 2024-04-06 08:47:41.792907 vpo-2.0/PKG-INFO
+-rw-rw-rw-   0        0        0       47 2024-03-17 08:35:15.000000 vpo-2.0/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-06 08:47:41.793908 vpo-2.0/setup.cfg
+-rw-rw-rw-   0        0        0      875 2024-04-06 08:47:38.000000 vpo-2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-06 08:47:41.783899 vpo-2.0/vpo/
+-rw-rw-rw-   0        0        0    33058 2024-04-06 08:46:33.000000 vpo-2.0/vpo/__init__.py
+-rw-rw-rw-   0        0        0    43465 2024-04-06 08:43:45.000000 vpo-2.0/vpo/authkey.py
+-rw-rw-rw-   0        0        0     2391 2024-03-17 20:30:42.000000 vpo-2.0/vpo/disc.py
+-rw-rw-rw-   0        0        0     1531 2024-03-17 18:08:43.000000 vpo-2.0/vpo/others.py
+drwxrwxrwx   0        0        0        0 2024-04-06 08:47:41.791906 vpo-2.0/vpo.egg-info/
+-rw-rw-rw-   0        0        0      694 2024-04-06 08:47:41.000000 vpo-2.0/vpo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      217 2024-04-06 08:47:41.000000 vpo-2.0/vpo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-06 08:47:41.000000 vpo-2.0/vpo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2024-04-06 08:47:41.000000 vpo-2.0/vpo.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2024-04-06 08:47:41.000000 vpo-2.0/vpo.egg-info/top_level.txt
```

### Comparing `vpo-1.7/LICENCE` & `vpo-2.0/LICENCE`

 * *Files identical despite different names*

### Comparing `vpo-1.7/setup.py` & `vpo-2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="vpo",
-    version="1.7",
+    version="2.0",
     author="VP_Services",
     author_email="discordyashing@gmail.com",
     url="https://github.com/hackiyui/vpimport",
     description="Un package qui vous facilitera la vie: un système de keyauth automatique par exemple",
     packages=['vpo'],
     install_requires=["win32security", "uuid", "wmi", "datetime", "uuid", "pystyle"],
     python_requires=">=3.11",
```

### Comparing `vpo-1.7/vpo/__init__.py` & `vpo-2.0/vpo/__init__.py`

 * *Files identical despite different names*

### Comparing `vpo-1.7/vpo/authkey.py` & `vpo-2.0/vpo/authkey.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,15 +83,15 @@
     import os
     import json as jsond
     import binascii
     from uuid import uuid4
     import hmac
     import hashlib
     from time import sleep
-    from authkey import others                                      
+    from .authkey import others                                      
     '''You cannot use that'''                                                 
                                                                                           
     name = ownerid = secret = version = hash_to_check = ""                                                 
                                                                                           
     def __init__(self, name, ownerid, secret, version, hash_to_check):                                                 
         if len(ownerid) != 10 and len(secret) != 64:                                                 
             print("Go to Manage Applications on dashboard, copy python code, and replace code in main.py with that")
```

### Comparing `vpo-1.7/vpo/disc.py` & `vpo-2.0/vpo/disc.py`

 * *Files identical despite different names*

### Comparing `vpo-1.7/vpo/others.py` & `vpo-2.0/vpo/others.py`

 * *Files identical despite different names*

