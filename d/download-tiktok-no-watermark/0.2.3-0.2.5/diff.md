# Comparing `tmp/download_tiktok_no_watermark-0.2.3.tar.gz` & `tmp/download_tiktok_no_watermark-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "download_tiktok_no_watermark-0.2.3.tar", last modified: Sat Apr  6 19:36:37 2024, max compression
+gzip compressed data, was "download_tiktok_no_watermark-0.2.5.tar", last modified: Sat Apr  6 19:40:48 2024, max compression
```

## Comparing `download_tiktok_no_watermark-0.2.3.tar` & `download_tiktok_no_watermark-0.2.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 jacobadelman   (501) staff       (20)        0 2024-04-06 19:36:37.590633 download_tiktok_no_watermark-0.2.3/
--rw-r--r--   0 jacobadelman   (501) staff       (20)      711 2024-04-06 19:36:37.590486 download_tiktok_no_watermark-0.2.3/PKG-INFO
--rw-r--r--   0 jacobadelman   (501) staff       (20)      554 2024-04-06 19:23:19.000000 download_tiktok_no_watermark-0.2.3/README.md
-drwxr-xr-x   0 jacobadelman   (501) staff       (20)        0 2024-04-06 19:36:37.589158 download_tiktok_no_watermark-0.2.3/download_tiktok_no_watermark/
--rw-r--r--   0 jacobadelman   (501) staff       (20)     7030 2024-04-06 19:34:05.000000 download_tiktok_no_watermark-0.2.3/download_tiktok_no_watermark/download.py
-drwxr-xr-x   0 jacobadelman   (501) staff       (20)        0 2024-04-06 19:36:37.590250 download_tiktok_no_watermark-0.2.3/download_tiktok_no_watermark.egg-info/
--rw-r--r--   0 jacobadelman   (501) staff       (20)      711 2024-04-06 19:36:37.000000 download_tiktok_no_watermark-0.2.3/download_tiktok_no_watermark.egg-info/PKG-INFO
--rw-r--r--   0 jacobadelman   (501) staff       (20)      318 2024-04-06 19:36:37.000000 download_tiktok_no_watermark-0.2.3/download_tiktok_no_watermark.egg-info/SOURCES.txt
--rw-r--r--   0 jacobadelman   (501) staff       (20)        1 2024-04-06 19:36:37.000000 download_tiktok_no_watermark-0.2.3/download_tiktok_no_watermark.egg-info/dependency_links.txt
--rw-r--r--   0 jacobadelman   (501) staff       (20)       80 2024-04-06 19:36:37.000000 download_tiktok_no_watermark-0.2.3/download_tiktok_no_watermark.egg-info/requires.txt
--rw-r--r--   0 jacobadelman   (501) staff       (20)       29 2024-04-06 19:36:37.000000 download_tiktok_no_watermark-0.2.3/download_tiktok_no_watermark.egg-info/top_level.txt
--rw-r--r--   0 jacobadelman   (501) staff       (20)       38 2024-04-06 19:36:37.590680 download_tiktok_no_watermark-0.2.3/setup.cfg
--rw-r--r--   0 jacobadelman   (501) staff       (20)     1091 2024-04-06 19:35:51.000000 download_tiktok_no_watermark-0.2.3/setup.py
+drwxr-xr-x   0 jacobadelman   (501) staff       (20)        0 2024-04-06 19:40:48.569122 download_tiktok_no_watermark-0.2.5/
+-rw-r--r--   0 jacobadelman   (501) staff       (20)      711 2024-04-06 19:40:48.568985 download_tiktok_no_watermark-0.2.5/PKG-INFO
+-rw-r--r--   0 jacobadelman   (501) staff       (20)      554 2024-04-06 19:23:19.000000 download_tiktok_no_watermark-0.2.5/README.md
+drwxr-xr-x   0 jacobadelman   (501) staff       (20)        0 2024-04-06 19:40:48.568185 download_tiktok_no_watermark-0.2.5/download_tiktok_no_watermark/
+-rw-r--r--   0 jacobadelman   (501) staff       (20)     7030 2024-04-06 19:34:05.000000 download_tiktok_no_watermark-0.2.5/download_tiktok_no_watermark/download.py
+drwxr-xr-x   0 jacobadelman   (501) staff       (20)        0 2024-04-06 19:40:48.568801 download_tiktok_no_watermark-0.2.5/download_tiktok_no_watermark.egg-info/
+-rw-r--r--   0 jacobadelman   (501) staff       (20)      711 2024-04-06 19:40:48.000000 download_tiktok_no_watermark-0.2.5/download_tiktok_no_watermark.egg-info/PKG-INFO
+-rw-r--r--   0 jacobadelman   (501) staff       (20)      318 2024-04-06 19:40:48.000000 download_tiktok_no_watermark-0.2.5/download_tiktok_no_watermark.egg-info/SOURCES.txt
+-rw-r--r--   0 jacobadelman   (501) staff       (20)        1 2024-04-06 19:40:48.000000 download_tiktok_no_watermark-0.2.5/download_tiktok_no_watermark.egg-info/dependency_links.txt
+-rw-r--r--   0 jacobadelman   (501) staff       (20)       80 2024-04-06 19:40:48.000000 download_tiktok_no_watermark-0.2.5/download_tiktok_no_watermark.egg-info/requires.txt
+-rw-r--r--   0 jacobadelman   (501) staff       (20)       29 2024-04-06 19:40:48.000000 download_tiktok_no_watermark-0.2.5/download_tiktok_no_watermark.egg-info/top_level.txt
+-rw-r--r--   0 jacobadelman   (501) staff       (20)       38 2024-04-06 19:40:48.569161 download_tiktok_no_watermark-0.2.5/setup.cfg
+-rw-r--r--   0 jacobadelman   (501) staff       (20)     1091 2024-04-06 19:40:46.000000 download_tiktok_no_watermark-0.2.5/setup.py
```

### Comparing `download_tiktok_no_watermark-0.2.3/PKG-INFO` & `download_tiktok_no_watermark-0.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: download_tiktok_no_watermark
-Version: 0.2.3
+Version: 0.2.5
 Summary: Download TikTok videos no watermark
 Home-page: https://github.com/jakeadelman/download_tiktok_no_watermark
 Author: Jacob Adelman
 Author-email: jacobzadelman@gmail.com
 License: BSD 2-clause
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
```

### Comparing `download_tiktok_no_watermark-0.2.3/README.md` & `download_tiktok_no_watermark-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `download_tiktok_no_watermark-0.2.3/download_tiktok_no_watermark/download.py` & `download_tiktok_no_watermark-0.2.5/download_tiktok_no_watermark/download.py`

 * *Files identical despite different names*

### Comparing `download_tiktok_no_watermark-0.2.3/download_tiktok_no_watermark.egg-info/PKG-INFO` & `download_tiktok_no_watermark-0.2.5/download_tiktok_no_watermark.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: download-tiktok-no-watermark
-Version: 0.2.3
+Version: 0.2.5
 Summary: Download TikTok videos no watermark
 Home-page: https://github.com/jakeadelman/download_tiktok_no_watermark
 Author: Jacob Adelman
 Author-email: jacobzadelman@gmail.com
 License: BSD 2-clause
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
```

### Comparing `download_tiktok_no_watermark-0.2.3/setup.py` & `download_tiktok_no_watermark-0.2.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='download_tiktok_no_watermark',
-    version='0.2.3',    
+    version='0.2.5',    
     description='Download TikTok videos no watermark',
     url='https://github.com/jakeadelman/download_tiktok_no_watermark',
     author='Jacob Adelman',
     author_email='jacobzadelman@gmail.com',
     license='BSD 2-clause',
     packages=['download_tiktok_no_watermark'],
     install_requires=['beautifulsoup4==4.12.3'
```

