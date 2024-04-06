# Comparing `tmp/CnbcNews-1.8.tar.gz` & `tmp/CnbcNews-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CnbcNews-1.8.tar", last modified: Sat Apr  6 16:37:34 2024, max compression
+gzip compressed data, was "CnbcNews-1.9.tar", last modified: Sat Apr  6 16:52:58 2024, max compression
```

## Comparing `CnbcNews-1.8.tar` & `CnbcNews-1.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-06 16:37:34.192406 CnbcNews-1.8/
-drwxrwxrwx   0        0        0        0 2024-04-06 16:37:34.146347 CnbcNews-1.8/CnbcNews/
--rw-rw-rw-   0        0        0       44 2024-04-06 16:37:01.000000 CnbcNews-1.8/CnbcNews/__init__.py
--rw-rw-rw-   0        0        0     4540 2024-04-06 16:15:54.000000 CnbcNews-1.8/CnbcNews/main.py
-drwxrwxrwx   0        0        0        0 2024-04-06 16:37:34.187402 CnbcNews-1.8/CnbcNews.egg-info/
--rw-rw-rw-   0        0        0     2741 2024-04-06 16:37:33.000000 CnbcNews-1.8/CnbcNews.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      250 2024-04-06 16:37:34.000000 CnbcNews-1.8/CnbcNews.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-06 16:37:33.000000 CnbcNews-1.8/CnbcNews.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2024-04-06 16:37:33.000000 CnbcNews-1.8/CnbcNews.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       22 2024-04-06 16:37:33.000000 CnbcNews-1.8/CnbcNews.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-06 16:37:33.000000 CnbcNews-1.8/CnbcNews.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2741 2024-04-06 16:37:34.191406 CnbcNews-1.8/PKG-INFO
--rw-rw-rw-   0        0        0     2643 2024-04-06 16:33:07.000000 CnbcNews-1.8/README.md
--rw-rw-rw-   0        0        0       42 2024-04-06 16:37:34.193404 CnbcNews-1.8/setup.cfg
--rw-rw-rw-   0        0        0      557 2024-04-06 16:37:28.000000 CnbcNews-1.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-06 16:52:58.188248 CnbcNews-1.9/
+drwxrwxrwx   0        0        0        0 2024-04-06 16:52:58.157039 CnbcNews-1.9/CnbcNews/
+-rw-rw-rw-   0        0        0       44 2024-04-06 16:37:01.000000 CnbcNews-1.9/CnbcNews/__init__.py
+-rw-rw-rw-   0        0        0     4583 2024-04-06 16:51:11.000000 CnbcNews-1.9/CnbcNews/main.py
+drwxrwxrwx   0        0        0        0 2024-04-06 16:52:58.185249 CnbcNews-1.9/CnbcNews.egg-info/
+-rw-rw-rw-   0        0        0     2729 2024-04-06 16:52:57.000000 CnbcNews-1.9/CnbcNews.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      250 2024-04-06 16:52:58.000000 CnbcNews-1.9/CnbcNews.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-06 16:52:57.000000 CnbcNews-1.9/CnbcNews.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2024-04-06 16:52:57.000000 CnbcNews-1.9/CnbcNews.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       22 2024-04-06 16:52:57.000000 CnbcNews-1.9/CnbcNews.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-06 16:52:57.000000 CnbcNews-1.9/CnbcNews.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2729 2024-04-06 16:52:58.187288 CnbcNews-1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     2631 2024-04-06 16:52:16.000000 CnbcNews-1.9/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-06 16:52:58.189252 CnbcNews-1.9/setup.cfg
+-rw-rw-rw-   0        0        0      557 2024-04-06 16:52:55.000000 CnbcNews-1.9/setup.py
```

### Comparing `CnbcNews-1.8/CnbcNews/main.py` & `CnbcNews-1.9/CnbcNews/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import json
 import pandas as pd
 from bs4 import BeautifulSoup
 import requests
 import csv
 import os
 import time
 
@@ -84,17 +85,17 @@
         getArticles(field=field, number=number)
         time.sleep(timeout)
 
 
 def main():
     import sys
     if len(sys.argv)==4:
-        getArticles(sys.argv[1], sys.argv[2], sys.argv[3])
+        getArticles(sys.argv[1], int(sys.argv[2]), json.loads(sys.argv[3].lower()))
     elif len(sys.argv)==3:
-        getArticles(sys.argv[1], sys.argv[2])
+        getArticles(sys.argv[1], int(sys.argv[2]))
     elif len(sys.argv)==2:
         getArticles(sys.argv[1])
     else:
         print("please provide the field ! exemple : CnbcNews-getArticles technology")
 
 if __name__ == "__main__":
     main()
```

### Comparing `CnbcNews-1.8/CnbcNews.egg-info/PKG-INFO` & `CnbcNews-1.9/CnbcNews.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: CnbcNews
-Version: 1.8
+Version: 1.9
 Description-Content-Type: text/markdown
 
 # **CnbcNews** #
 
 [![PyPI version](https://img.shields.io/pypi/v/CnbcNews.svg)](https://pypi.org/project/CnbcNews/)
 <!-- [![Donate](https://img.shields.io/badge/Donate-PayPal-green.svg)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=XX272QZV9A2FN&source=url) -->
 
 <!-- <img align="right" height="128px" width="128px" src="https://raw.githubusercontent.com/fhamborg/CnbcNews/master/misc/logo/logo-256.png" /> -->
 
 CnbcNews is an open source, easy-to-use news crawler that extracts structured information from Cnbc news website for Machine learning purposes. It can recursively follow internal hyperlinks and read RSS feeds to fetch both most recent articles in any given field. You only need to provide the desired field ('technology', 'politics', 'tv', 'business', 'markets', 'investing'..) of the news website to crawl it completely. 
 
 ## Extracted information
 CnbcNews extracts the following attributes from Cnbc news articles.
-* headline
 * article headline
 * article body (main text)
 * article's author name
 * publication date
 * label
 
 ## Features
```

### Comparing `CnbcNews-1.8/PKG-INFO` & `CnbcNews-1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: CnbcNews
-Version: 1.8
+Version: 1.9
 Description-Content-Type: text/markdown
 
 # **CnbcNews** #
 
 [![PyPI version](https://img.shields.io/pypi/v/CnbcNews.svg)](https://pypi.org/project/CnbcNews/)
 <!-- [![Donate](https://img.shields.io/badge/Donate-PayPal-green.svg)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=XX272QZV9A2FN&source=url) -->
 
 <!-- <img align="right" height="128px" width="128px" src="https://raw.githubusercontent.com/fhamborg/CnbcNews/master/misc/logo/logo-256.png" /> -->
 
 CnbcNews is an open source, easy-to-use news crawler that extracts structured information from Cnbc news website for Machine learning purposes. It can recursively follow internal hyperlinks and read RSS feeds to fetch both most recent articles in any given field. You only need to provide the desired field ('technology', 'politics', 'tv', 'business', 'markets', 'investing'..) of the news website to crawl it completely. 
 
 ## Extracted information
 CnbcNews extracts the following attributes from Cnbc news articles.
-* headline
 * article headline
 * article body (main text)
 * article's author name
 * publication date
 * label
 
 ## Features
```

### Comparing `CnbcNews-1.8/README.md` & `CnbcNews-1.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 
 <!-- <img align="right" height="128px" width="128px" src="https://raw.githubusercontent.com/fhamborg/CnbcNews/master/misc/logo/logo-256.png" /> -->
 
 CnbcNews is an open source, easy-to-use news crawler that extracts structured information from Cnbc news website for Machine learning purposes. It can recursively follow internal hyperlinks and read RSS feeds to fetch both most recent articles in any given field. You only need to provide the desired field ('technology', 'politics', 'tv', 'business', 'markets', 'investing'..) of the news website to crawl it completely. 
 
 ## Extracted information
 CnbcNews extracts the following attributes from Cnbc news articles.
-* headline
 * article headline
 * article body (main text)
 * article's author name
 * publication date
 * label
 
 ## Features
```

### Comparing `CnbcNews-1.8/setup.py` & `CnbcNews-1.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='CnbcNews',
-    version='1.8',
+    version='1.9',
     packages=find_packages(),
     install_requires=[
         'beautifulsoup4',
         'pandas'
     ],
     entry_points={
         "console_scripts": [
```

