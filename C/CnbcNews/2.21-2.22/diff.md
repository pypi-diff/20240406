# Comparing `tmp/CnbcNews-2.21.tar.gz` & `tmp/CnbcNews-2.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CnbcNews-2.21.tar", last modified: Sat Apr  6 17:57:15 2024, max compression
+gzip compressed data, was "CnbcNews-2.22.tar", last modified: Sat Apr  6 18:08:44 2024, max compression
```

## Comparing `CnbcNews-2.21.tar` & `CnbcNews-2.22.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-06 17:57:15.522486 CnbcNews-2.21/
-drwxrwxrwx   0        0        0        0 2024-04-06 17:57:15.453515 CnbcNews-2.21/CnbcNews/
--rw-rw-rw-   0        0        0       44 2024-04-06 16:37:01.000000 CnbcNews-2.21/CnbcNews/__init__.py
--rw-rw-rw-   0        0        0     4633 2024-04-06 17:57:03.000000 CnbcNews-2.21/CnbcNews/main.py
-drwxrwxrwx   0        0        0        0 2024-04-06 17:57:15.517485 CnbcNews-2.21/CnbcNews.egg-info/
--rw-rw-rw-   0        0        0     2730 2024-04-06 17:57:15.000000 CnbcNews-2.21/CnbcNews.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      250 2024-04-06 17:57:15.000000 CnbcNews-2.21/CnbcNews.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-06 17:57:15.000000 CnbcNews-2.21/CnbcNews.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2024-04-06 17:57:15.000000 CnbcNews-2.21/CnbcNews.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       22 2024-04-06 17:57:15.000000 CnbcNews-2.21/CnbcNews.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-06 17:57:15.000000 CnbcNews-2.21/CnbcNews.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2730 2024-04-06 17:57:15.521485 CnbcNews-2.21/PKG-INFO
--rw-rw-rw-   0        0        0     2631 2024-04-06 16:52:16.000000 CnbcNews-2.21/README.md
--rw-rw-rw-   0        0        0       42 2024-04-06 17:57:15.523486 CnbcNews-2.21/setup.cfg
--rw-rw-rw-   0        0        0      558 2024-04-06 17:57:11.000000 CnbcNews-2.21/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-06 18:08:44.861405 CnbcNews-2.22/
+drwxrwxrwx   0        0        0        0 2024-04-06 18:08:44.738117 CnbcNews-2.22/CnbcNews/
+-rw-rw-rw-   0        0        0       44 2024-04-06 16:37:01.000000 CnbcNews-2.22/CnbcNews/__init__.py
+-rw-rw-rw-   0        0        0     4593 2024-04-06 17:59:40.000000 CnbcNews-2.22/CnbcNews/main.py
+drwxrwxrwx   0        0        0        0 2024-04-06 18:08:44.851237 CnbcNews-2.22/CnbcNews.egg-info/
+-rw-rw-rw-   0        0        0     2730 2024-04-06 18:08:44.000000 CnbcNews-2.22/CnbcNews.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      250 2024-04-06 18:08:44.000000 CnbcNews-2.22/CnbcNews.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-06 18:08:44.000000 CnbcNews-2.22/CnbcNews.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2024-04-06 18:08:44.000000 CnbcNews-2.22/CnbcNews.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       36 2024-04-06 18:08:44.000000 CnbcNews-2.22/CnbcNews.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-06 18:08:44.000000 CnbcNews-2.22/CnbcNews.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2730 2024-04-06 18:08:44.857518 CnbcNews-2.22/PKG-INFO
+-rw-rw-rw-   0        0        0     2631 2024-04-06 16:52:16.000000 CnbcNews-2.22/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-06 18:08:44.862298 CnbcNews-2.22/setup.cfg
+-rw-rw-rw-   0        0        0      596 2024-04-06 18:08:38.000000 CnbcNews-2.22/setup.py
```

### Comparing `CnbcNews-2.21/CnbcNews/main.py` & `CnbcNews-2.22/CnbcNews/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,14 @@
         url = f"https://www.cnbc.com/{field}/?page={page_number}"
         page = requests.get(url)
         soup = BeautifulSoup(page.content, "html.parser")
         news_sections = soup.find_all("a", class_="Card-title")
         for section in news_sections:
             try:
                 article_urls.append(section['href'])
-                print(section['href'])
             except KeyError as e:
                 print(repr(e))
         page_number += 1
     return article_urls[:number]
 
 
 def getArticles(field, number=20, dropna= True | False):
```

### Comparing `CnbcNews-2.21/CnbcNews.egg-info/PKG-INFO` & `CnbcNews-2.22/CnbcNews.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CnbcNews
-Version: 2.21
+Version: 2.22
 Description-Content-Type: text/markdown
 
 # **CnbcNews** #
 
 [![PyPI version](https://img.shields.io/pypi/v/CnbcNews.svg)](https://pypi.org/project/CnbcNews/)
 <!-- [![Donate](https://img.shields.io/badge/Donate-PayPal-green.svg)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=XX272QZV9A2FN&source=url) -->
```

### Comparing `CnbcNews-2.21/PKG-INFO` & `CnbcNews-2.22/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CnbcNews
-Version: 2.21
+Version: 2.22
 Description-Content-Type: text/markdown
 
 # **CnbcNews** #
 
 [![PyPI version](https://img.shields.io/pypi/v/CnbcNews.svg)](https://pypi.org/project/CnbcNews/)
 <!-- [![Donate](https://img.shields.io/badge/Donate-PayPal-green.svg)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=XX272QZV9A2FN&source=url) -->
```

### Comparing `CnbcNews-2.21/README.md` & `CnbcNews-2.22/README.md`

 * *Files identical despite different names*

### Comparing `CnbcNews-2.21/setup.py` & `CnbcNews-2.22/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,19 +2,21 @@
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='CnbcNews',
-    version='2.21',
+    version='2.22',
     packages=find_packages(),
     install_requires=[
+        'requests',
         'beautifulsoup4',
-        'pandas'
+        'pandas',
+        'json'
     ],
     entry_points={
         "console_scripts": [
             "CnbcNews-getArticles = CnbcNews.main:main",
         ],
     },
     long_description=long_description,
```

