# Comparing `tmp/ntscraper-0.3.8.tar.gz` & `tmp/ntscraper-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ntscraper-0.3.8.tar", last modified: Sun Dec 17 10:37:24 2023, max compression
+gzip compressed data, was "ntscraper-0.3.9.tar", last modified: Tue Dec 26 09:22:19 2023, max compression
```

## Comparing `ntscraper-0.3.8.tar` & `ntscraper-0.3.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-12-17 10:37:24.625296 ntscraper-0.3.8/
--rw-rw-rw-   0        0        0     1091 2023-01-15 20:51:11.000000 ntscraper-0.3.8/LICENSE.txt
--rw-rw-rw-   0        0        0     5390 2023-12-17 10:37:24.625296 ntscraper-0.3.8/PKG-INFO
--rw-rw-rw-   0        0        0     4464 2023-12-09 19:03:06.000000 ntscraper-0.3.8/README.md
-drwxrwxrwx   0        0        0        0 2023-12-17 10:37:24.588264 ntscraper-0.3.8/ntscraper/
--rw-rw-rw-   0        0        0       26 2023-10-24 12:37:04.000000 ntscraper-0.3.8/ntscraper/__init__.py
--rw-rw-rw-   0        0        0    39318 2023-12-17 10:37:05.000000 ntscraper-0.3.8/ntscraper/nitter.py
-drwxrwxrwx   0        0        0        0 2023-12-17 10:37:24.622727 ntscraper-0.3.8/ntscraper.egg-info/
--rw-rw-rw-   0        0        0     5390 2023-12-17 10:37:24.000000 ntscraper-0.3.8/ntscraper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      236 2023-12-17 10:37:24.000000 ntscraper-0.3.8/ntscraper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-12-17 10:37:24.000000 ntscraper-0.3.8/ntscraper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2023-12-17 10:37:24.000000 ntscraper-0.3.8/ntscraper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-12-17 10:37:24.000000 ntscraper-0.3.8/ntscraper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-12-17 10:37:24.625296 ntscraper-0.3.8/setup.cfg
--rw-rw-rw-   0        0        0     1356 2023-12-17 10:37:15.000000 ntscraper-0.3.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-12-26 09:22:19.977232 ntscraper-0.3.9/
+-rw-rw-rw-   0        0        0     1091 2023-01-15 20:51:11.000000 ntscraper-0.3.9/LICENSE.txt
+-rw-rw-rw-   0        0        0     5390 2023-12-26 09:22:19.977232 ntscraper-0.3.9/PKG-INFO
+-rw-rw-rw-   0        0        0     4464 2023-12-09 19:03:06.000000 ntscraper-0.3.9/README.md
+drwxrwxrwx   0        0        0        0 2023-12-26 09:22:19.920184 ntscraper-0.3.9/ntscraper/
+-rw-rw-rw-   0        0        0       26 2023-10-24 12:37:04.000000 ntscraper-0.3.9/ntscraper/__init__.py
+-rw-rw-rw-   0        0        0    39332 2023-12-26 09:22:06.000000 ntscraper-0.3.9/ntscraper/nitter.py
+drwxrwxrwx   0        0        0        0 2023-12-26 09:22:19.977232 ntscraper-0.3.9/ntscraper.egg-info/
+-rw-rw-rw-   0        0        0     5390 2023-12-26 09:22:19.000000 ntscraper-0.3.9/ntscraper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      236 2023-12-26 09:22:19.000000 ntscraper-0.3.9/ntscraper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-12-26 09:22:19.000000 ntscraper-0.3.9/ntscraper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2023-12-26 09:22:19.000000 ntscraper-0.3.9/ntscraper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-12-26 09:22:19.000000 ntscraper-0.3.9/ntscraper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-12-26 09:22:19.977232 ntscraper-0.3.9/setup.cfg
+-rw-rw-rw-   0        0        0     1356 2023-12-26 09:21:01.000000 ntscraper-0.3.9/setup.py
```

### Comparing `ntscraper-0.3.8/LICENSE.txt` & `ntscraper-0.3.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ntscraper-0.3.8/PKG-INFO` & `ntscraper-0.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ntscraper
-Version: 0.3.8
+Version: 0.3.9
 Summary: Unofficial library to scrape Twitter profiles and posts from Nitter instances
 Author: Lorenzo Bocchi
 Author-email: lorenzobocchi99@yahoo.com
 License: MIT
 Project-URL: Homepage, https://github.com/bocchilorenzo/ntscraper
 Project-URL: Source, https://github.com/bocchilorenzo/ntscraper
 Project-URL: Documentation, https://github.com/bocchilorenzo/ntscraper
```

### Comparing `ntscraper-0.3.8/README.md` & `ntscraper-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `ntscraper-0.3.8/ntscraper/nitter.py` & `ntscraper-0.3.9/ntscraper/nitter.py`

 * *Files 0% similar despite different names*

```diff
@@ -196,15 +196,18 @@
         ):
             if soup.find("div", class_="error-panel"):
                 message = (
                     f"Fetching error: "
                     + soup.find("div", class_="error-panel").find("span").text.strip()
                 )
             else:
-                message = f"Empty page on {self.instance}"
+                if soup.find("div", class_="timeline-header timeline-protected"):
+                    message = "Account is protected"
+                else:
+                    message = f"Empty page on {self.instance}"
             logging.warning(message)
             soup = None
         return soup
 
     def _get_page(self, endpoint, max_retries=5):
         """
         Download page from Nitter instance
@@ -865,15 +868,15 @@
         :param filters: list of filters to apply. Default is None
         :param exclude: list of filters to exclude. Default is None
         :param max_retries: max retries to scrape a page. Default is 5
         :param instance: Nitter instance to use. Default is None
         :return: dictionary or array with dictionaries (in case of multiple terms) of the tweets and threads for the provided terms
         """
         if type(terms) == str:
-            term = sub(r"[^A-Za-z0-9_+-:]", " ", terms).replace("  ", " ").strip()
+            term = terms.strip()
 
             return self._search(
                 term,
                 mode,
                 number,
                 since,
                 until,
@@ -882,15 +885,15 @@
                 to,
                 filters,
                 exclude,
                 max_retries,
                 instance,
             )
         elif len(terms) == 1:
-            term = sub(r"[^A-Za-z0-9_+-:]", " ", terms[0]).replace("  ", " ").strip()
+            term = terms[0].strip()
 
             return self._search(
                 term,
                 mode,
                 number,
                 since,
                 until,
@@ -906,15 +909,15 @@
             if len(terms) > cpu_count():
                 raise ValueError(
                     f"Too many terms. Maximum number of terms is {cpu_count()}"
                 )
 
             args = [
                 (
-                    sub(r"[^A-Za-z0-9_+-:]", " ", term).replace("  ", " ").strip(),
+                    term.strip(),
                     mode,
                     number,
                     since,
                     until,
                     near,
                     language,
                     to,
```

### Comparing `ntscraper-0.3.8/ntscraper.egg-info/PKG-INFO` & `ntscraper-0.3.9/ntscraper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ntscraper
-Version: 0.3.8
+Version: 0.3.9
 Summary: Unofficial library to scrape Twitter profiles and posts from Nitter instances
 Author: Lorenzo Bocchi
 Author-email: lorenzobocchi99@yahoo.com
 License: MIT
 Project-URL: Homepage, https://github.com/bocchilorenzo/ntscraper
 Project-URL: Source, https://github.com/bocchilorenzo/ntscraper
 Project-URL: Documentation, https://github.com/bocchilorenzo/ntscraper
```

### Comparing `ntscraper-0.3.8/setup.py` & `ntscraper-0.3.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 HERE = path.abspath(path.dirname(__file__))
 
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name="ntscraper",
-    version="0.3.8",
+    version="0.3.9",
     description="Unofficial library to scrape Twitter profiles and posts from Nitter instances",
     long_description=long_description,
     long_description_content_type="text/markdown",
     project_urls={
         'Homepage': 'https://github.com/bocchilorenzo/ntscraper',
         'Source': 'https://github.com/bocchilorenzo/ntscraper',
         'Documentation': 'https://github.com/bocchilorenzo/ntscraper'
```

