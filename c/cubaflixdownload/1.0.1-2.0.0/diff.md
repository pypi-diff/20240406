# Comparing `tmp/cubaflixdownload-1.0.1.tar.gz` & `tmp/cubaflixdownload-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cubaflixdownload-1.0.1.tar", last modified: Fri Mar 29 05:05:14 2024, max compression
+gzip compressed data, was "cubaflixdownload-2.0.0.tar", last modified: Sat Apr  6 03:28:03 2024, max compression
```

## Comparing `cubaflixdownload-1.0.1.tar` & `cubaflixdownload-2.0.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-03-29 05:05:14.306874 cubaflixdownload-1.0.1/
--rw-rw-rw-   0        0        0     1235 2023-04-13 20:26:37.000000 cubaflixdownload-1.0.1/LICENSE
--rw-rw-rw-   0        0        0     1001 2024-03-29 05:05:14.303874 cubaflixdownload-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      638 2023-04-25 04:32:36.000000 cubaflixdownload-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-03-29 05:05:14.246870 cubaflixdownload-1.0.1/cubaflixdownload/
--rw-rw-rw-   0        0        0      931 2024-03-26 07:28:02.000000 cubaflixdownload-1.0.1/cubaflixdownload/__init__.py
--rw-rw-rw-   0        0        0       75 2024-03-29 05:04:37.000000 cubaflixdownload-1.0.1/cubaflixdownload/version.py
-drwxrwxrwx   0        0        0        0 2024-03-29 05:05:14.296873 cubaflixdownload-1.0.1/cubaflixdownload.egg-info/
--rw-rw-rw-   0        0        0     1001 2024-03-29 05:05:12.000000 cubaflixdownload-1.0.1/cubaflixdownload.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      317 2024-03-29 05:05:13.000000 cubaflixdownload-1.0.1/cubaflixdownload.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-29 05:05:12.000000 cubaflixdownload-1.0.1/cubaflixdownload.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-03-29 05:05:12.000000 cubaflixdownload-1.0.1/cubaflixdownload.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-03-29 05:05:12.000000 cubaflixdownload-1.0.1/cubaflixdownload.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2024-03-29 05:05:12.000000 cubaflixdownload-1.0.1/cubaflixdownload.egg-info/zip-safe
--rw-rw-rw-   0        0        0       42 2024-03-29 05:05:14.308874 cubaflixdownload-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1632 2024-03-26 07:30:21.000000 cubaflixdownload-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-06 03:28:03.866416 cubaflixdownload-2.0.0/
+-rw-rw-rw-   0        0        0     1235 2023-04-13 20:26:37.000000 cubaflixdownload-2.0.0/LICENSE
+-rw-rw-rw-   0        0        0     1001 2024-04-06 03:28:03.863416 cubaflixdownload-2.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0      638 2023-04-25 04:32:36.000000 cubaflixdownload-2.0.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-06 03:28:03.809413 cubaflixdownload-2.0.0/cubaflixdownload/
+-rw-rw-rw-   0        0        0      931 2024-03-26 07:28:02.000000 cubaflixdownload-2.0.0/cubaflixdownload/__init__.py
+-rw-rw-rw-   0        0        0       75 2024-04-06 03:27:44.000000 cubaflixdownload-2.0.0/cubaflixdownload/version.py
+drwxrwxrwx   0        0        0        0 2024-04-06 03:28:03.857416 cubaflixdownload-2.0.0/cubaflixdownload.egg-info/
+-rw-rw-rw-   0        0        0     1001 2024-04-06 03:28:02.000000 cubaflixdownload-2.0.0/cubaflixdownload.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      317 2024-04-06 03:28:02.000000 cubaflixdownload-2.0.0/cubaflixdownload.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-06 03:28:02.000000 cubaflixdownload-2.0.0/cubaflixdownload.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-04-06 03:28:02.000000 cubaflixdownload-2.0.0/cubaflixdownload.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-04-06 03:28:02.000000 cubaflixdownload-2.0.0/cubaflixdownload.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2024-04-06 03:28:02.000000 cubaflixdownload-2.0.0/cubaflixdownload.egg-info/zip-safe
+-rw-rw-rw-   0        0        0       42 2024-04-06 03:28:03.868416 cubaflixdownload-2.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1632 2024-03-26 07:30:21.000000 cubaflixdownload-2.0.0/setup.py
```

### Comparing `cubaflixdownload-1.0.1/LICENSE` & `cubaflixdownload-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cubaflixdownload-1.0.1/PKG-INFO` & `cubaflixdownload-2.0.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cubaflixdownload
-Version: 1.0.1
+Version: 2.0.0
 Summary: Python 3 library for short text
 Home-page: https://github.com/fenixinvitado2021/shorturl
 Author: RayServer
 Author-email: susej.mabel2009@gmail.com
 License: The Unlicense (Unlicense)
 Keywords: telegram,download,stream,bots
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `cubaflixdownload-1.0.1/README.md` & `cubaflixdownload-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `cubaflixdownload-1.0.1/cubaflixdownload/__init__.py` & `cubaflixdownload-2.0.0/cubaflixdownload/__init__.py`

 * *Files identical despite different names*

### Comparing `cubaflixdownload-1.0.1/cubaflixdownload.egg-info/PKG-INFO` & `cubaflixdownload-2.0.0/cubaflixdownload.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cubaflixdownload
-Version: 1.0.1
+Version: 2.0.0
 Summary: Python 3 library for short text
 Home-page: https://github.com/fenixinvitado2021/shorturl
 Author: RayServer
 Author-email: susej.mabel2009@gmail.com
 License: The Unlicense (Unlicense)
 Keywords: telegram,download,stream,bots
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `cubaflixdownload-1.0.1/setup.py` & `cubaflixdownload-2.0.0/setup.py`

 * *Files identical despite different names*

