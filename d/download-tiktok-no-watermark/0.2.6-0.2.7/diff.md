# Comparing `tmp/download_tiktok_no_watermark-0.2.6.tar.gz` & `tmp/download_tiktok_no_watermark-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "download_tiktok_no_watermark-0.2.6.tar", last modified: Sat Apr  6 19:50:23 2024, max compression
+gzip compressed data, was "download_tiktok_no_watermark-0.2.7.tar", last modified: Sat Apr  6 19:55:35 2024, max compression
```

## Comparing `download_tiktok_no_watermark-0.2.6.tar` & `download_tiktok_no_watermark-0.2.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 jacobadelman   (501) staff       (20)        0 2024-04-06 19:50:23.460601 download_tiktok_no_watermark-0.2.6/
--rw-r--r--   0 jacobadelman   (501) staff       (20)      866 2024-04-06 19:50:23.460373 download_tiktok_no_watermark-0.2.6/PKG-INFO
--rw-r--r--   0 jacobadelman   (501) staff       (20)      554 2024-04-06 19:23:19.000000 download_tiktok_no_watermark-0.2.6/README.md
-drwxr-xr-x   0 jacobadelman   (501) staff       (20)        0 2024-04-06 19:50:23.459143 download_tiktok_no_watermark-0.2.6/download_tiktok_no_watermark/
--rw-r--r--   0 jacobadelman   (501) staff       (20)     7030 2024-04-06 19:34:05.000000 download_tiktok_no_watermark-0.2.6/download_tiktok_no_watermark/download.py
-drwxr-xr-x   0 jacobadelman   (501) staff       (20)        0 2024-04-06 19:50:23.460138 download_tiktok_no_watermark-0.2.6/download_tiktok_no_watermark.egg-info/
--rw-r--r--   0 jacobadelman   (501) staff       (20)      866 2024-04-06 19:50:23.000000 download_tiktok_no_watermark-0.2.6/download_tiktok_no_watermark.egg-info/PKG-INFO
--rw-r--r--   0 jacobadelman   (501) staff       (20)      318 2024-04-06 19:50:23.000000 download_tiktok_no_watermark-0.2.6/download_tiktok_no_watermark.egg-info/SOURCES.txt
--rw-r--r--   0 jacobadelman   (501) staff       (20)        1 2024-04-06 19:50:23.000000 download_tiktok_no_watermark-0.2.6/download_tiktok_no_watermark.egg-info/dependency_links.txt
--rw-r--r--   0 jacobadelman   (501) staff       (20)       80 2024-04-06 19:50:23.000000 download_tiktok_no_watermark-0.2.6/download_tiktok_no_watermark.egg-info/requires.txt
--rw-r--r--   0 jacobadelman   (501) staff       (20)       29 2024-04-06 19:50:23.000000 download_tiktok_no_watermark-0.2.6/download_tiktok_no_watermark.egg-info/top_level.txt
--rw-r--r--   0 jacobadelman   (501) staff       (20)       38 2024-04-06 19:50:23.460658 download_tiktok_no_watermark-0.2.6/setup.cfg
--rw-r--r--   0 jacobadelman   (501) staff       (20)     1091 2024-04-06 19:50:00.000000 download_tiktok_no_watermark-0.2.6/setup.py
+drwxr-xr-x   0 jacobadelman   (501) staff       (20)        0 2024-04-06 19:55:35.668034 download_tiktok_no_watermark-0.2.7/
+-rw-r--r--   0 jacobadelman   (501) staff       (20)      711 2024-04-06 19:55:35.667911 download_tiktok_no_watermark-0.2.7/PKG-INFO
+-rw-r--r--   0 jacobadelman   (501) staff       (20)      554 2024-04-06 19:23:19.000000 download_tiktok_no_watermark-0.2.7/README.md
+drwxr-xr-x   0 jacobadelman   (501) staff       (20)        0 2024-04-06 19:55:35.667028 download_tiktok_no_watermark-0.2.7/download_tiktok_no_watermark/
+-rw-r--r--   0 jacobadelman   (501) staff       (20)     7030 2024-04-06 19:52:33.000000 download_tiktok_no_watermark-0.2.7/download_tiktok_no_watermark/download.py
+drwxr-xr-x   0 jacobadelman   (501) staff       (20)        0 2024-04-06 19:55:35.667725 download_tiktok_no_watermark-0.2.7/download_tiktok_no_watermark.egg-info/
+-rw-r--r--   0 jacobadelman   (501) staff       (20)      711 2024-04-06 19:55:35.000000 download_tiktok_no_watermark-0.2.7/download_tiktok_no_watermark.egg-info/PKG-INFO
+-rw-r--r--   0 jacobadelman   (501) staff       (20)      318 2024-04-06 19:55:35.000000 download_tiktok_no_watermark-0.2.7/download_tiktok_no_watermark.egg-info/SOURCES.txt
+-rw-r--r--   0 jacobadelman   (501) staff       (20)        1 2024-04-06 19:55:35.000000 download_tiktok_no_watermark-0.2.7/download_tiktok_no_watermark.egg-info/dependency_links.txt
+-rw-r--r--   0 jacobadelman   (501) staff       (20)       80 2024-04-06 19:55:35.000000 download_tiktok_no_watermark-0.2.7/download_tiktok_no_watermark.egg-info/requires.txt
+-rw-r--r--   0 jacobadelman   (501) staff       (20)       29 2024-04-06 19:55:35.000000 download_tiktok_no_watermark-0.2.7/download_tiktok_no_watermark.egg-info/top_level.txt
+-rw-r--r--   0 jacobadelman   (501) staff       (20)       38 2024-04-06 19:55:35.668072 download_tiktok_no_watermark-0.2.7/setup.cfg
+-rw-r--r--   0 jacobadelman   (501) staff       (20)     1091 2024-04-06 19:55:13.000000 download_tiktok_no_watermark-0.2.7/setup.py
```

### Comparing `download_tiktok_no_watermark-0.2.6/PKG-INFO` & `download_tiktok_no_watermark-0.2.7/download_tiktok_no_watermark.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,17 @@
 Metadata-Version: 2.1
-Name: download_tiktok_no_watermark
-Version: 0.2.6
+Name: download-tiktok-no-watermark
+Version: 0.2.7
 Summary: Download TikTok videos no watermark
 Home-page: https://github.com/jakeadelman/download_tiktok_no_watermark
 Author: Jacob Adelman
 Author-email: jacobzadelman@gmail.com
 License: BSD 2-clause
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
-Requires-Dist: beautifulsoup4==4.12.3
-Requires-Dist: colorama==0.4.6
-Requires-Dist: Requests==2.31.0
-Requires-Dist: tls_client==1.0.1
-Requires-Dist: js2py
```

### Comparing `download_tiktok_no_watermark-0.2.6/README.md` & `download_tiktok_no_watermark-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `download_tiktok_no_watermark-0.2.6/download_tiktok_no_watermark/download.py` & `download_tiktok_no_watermark-0.2.7/download_tiktok_no_watermark/download.py`

 * *Files identical despite different names*

### Comparing `download_tiktok_no_watermark-0.2.6/setup.py` & `download_tiktok_no_watermark-0.2.7/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='download_tiktok_no_watermark',
-    version='0.2.6',    
+    version='0.2.7',    
     description='Download TikTok videos no watermark',
     url='https://github.com/jakeadelman/download_tiktok_no_watermark',
     author='Jacob Adelman',
     author_email='jacobzadelman@gmail.com',
     license='BSD 2-clause',
     packages=['download_tiktok_no_watermark'],
     install_requires=['beautifulsoup4==4.12.3'
```

