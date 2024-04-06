# Comparing `tmp/CnbcNews-1.7.tar.gz` & `tmp/CnbcNews-1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CnbcNews-1.7.tar", last modified: Sat Apr  6 16:37:10 2024, max compression
+gzip compressed data, was "CnbcNews-1.8.tar", last modified: Sat Apr  6 16:37:34 2024, max compression
```

## Comparing `CnbcNews-1.7.tar` & `CnbcNews-1.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-06 16:37:10.446476 CnbcNews-1.7/
-drwxrwxrwx   0        0        0        0 2024-04-06 16:37:10.416617 CnbcNews-1.7/CnbcNews/
--rw-rw-rw-   0        0        0       44 2024-04-06 16:37:01.000000 CnbcNews-1.7/CnbcNews/__init__.py
--rw-rw-rw-   0        0        0     4540 2024-04-06 16:15:54.000000 CnbcNews-1.7/CnbcNews/main.py
-drwxrwxrwx   0        0        0        0 2024-04-06 16:37:10.440583 CnbcNews-1.7/CnbcNews.egg-info/
--rw-rw-rw-   0        0        0     2741 2024-04-06 16:37:10.000000 CnbcNews-1.7/CnbcNews.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      250 2024-04-06 16:37:10.000000 CnbcNews-1.7/CnbcNews.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-06 16:37:10.000000 CnbcNews-1.7/CnbcNews.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2024-04-06 16:37:10.000000 CnbcNews-1.7/CnbcNews.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       22 2024-04-06 16:37:10.000000 CnbcNews-1.7/CnbcNews.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-06 16:37:10.000000 CnbcNews-1.7/CnbcNews.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2741 2024-04-06 16:37:10.443580 CnbcNews-1.7/PKG-INFO
--rw-rw-rw-   0        0        0     2643 2024-04-06 16:33:07.000000 CnbcNews-1.7/README.md
--rw-rw-rw-   0        0        0       42 2024-04-06 16:37:10.446476 CnbcNews-1.7/setup.cfg
--rw-rw-rw-   0        0        0      557 2024-04-06 16:33:54.000000 CnbcNews-1.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-06 16:37:34.192406 CnbcNews-1.8/
+drwxrwxrwx   0        0        0        0 2024-04-06 16:37:34.146347 CnbcNews-1.8/CnbcNews/
+-rw-rw-rw-   0        0        0       44 2024-04-06 16:37:01.000000 CnbcNews-1.8/CnbcNews/__init__.py
+-rw-rw-rw-   0        0        0     4540 2024-04-06 16:15:54.000000 CnbcNews-1.8/CnbcNews/main.py
+drwxrwxrwx   0        0        0        0 2024-04-06 16:37:34.187402 CnbcNews-1.8/CnbcNews.egg-info/
+-rw-rw-rw-   0        0        0     2741 2024-04-06 16:37:33.000000 CnbcNews-1.8/CnbcNews.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      250 2024-04-06 16:37:34.000000 CnbcNews-1.8/CnbcNews.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-06 16:37:33.000000 CnbcNews-1.8/CnbcNews.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2024-04-06 16:37:33.000000 CnbcNews-1.8/CnbcNews.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       22 2024-04-06 16:37:33.000000 CnbcNews-1.8/CnbcNews.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-06 16:37:33.000000 CnbcNews-1.8/CnbcNews.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2741 2024-04-06 16:37:34.191406 CnbcNews-1.8/PKG-INFO
+-rw-rw-rw-   0        0        0     2643 2024-04-06 16:33:07.000000 CnbcNews-1.8/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-06 16:37:34.193404 CnbcNews-1.8/setup.cfg
+-rw-rw-rw-   0        0        0      557 2024-04-06 16:37:28.000000 CnbcNews-1.8/setup.py
```

### Comparing `CnbcNews-1.7/CnbcNews/main.py` & `CnbcNews-1.8/CnbcNews/main.py`

 * *Files identical despite different names*

### Comparing `CnbcNews-1.7/CnbcNews.egg-info/PKG-INFO` & `CnbcNews-1.8/CnbcNews.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CnbcNews
-Version: 1.7
+Version: 1.8
 Description-Content-Type: text/markdown
 
 # **CnbcNews** #
 
 [![PyPI version](https://img.shields.io/pypi/v/CnbcNews.svg)](https://pypi.org/project/CnbcNews/)
 <!-- [![Donate](https://img.shields.io/badge/Donate-PayPal-green.svg)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=XX272QZV9A2FN&source=url) -->
```

### Comparing `CnbcNews-1.7/PKG-INFO` & `CnbcNews-1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CnbcNews
-Version: 1.7
+Version: 1.8
 Description-Content-Type: text/markdown
 
 # **CnbcNews** #
 
 [![PyPI version](https://img.shields.io/pypi/v/CnbcNews.svg)](https://pypi.org/project/CnbcNews/)
 <!-- [![Donate](https://img.shields.io/badge/Donate-PayPal-green.svg)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=XX272QZV9A2FN&source=url) -->
```

### Comparing `CnbcNews-1.7/README.md` & `CnbcNews-1.8/README.md`

 * *Files identical despite different names*

### Comparing `CnbcNews-1.7/setup.py` & `CnbcNews-1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='CnbcNews',
-    version='1.7',
+    version='1.8',
     packages=find_packages(),
     install_requires=[
         'beautifulsoup4',
         'pandas'
     ],
     entry_points={
         "console_scripts": [
```

