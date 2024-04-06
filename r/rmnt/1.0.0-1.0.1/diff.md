# Comparing `tmp/rmnt-1.0.0.tar.gz` & `tmp/rmnt-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rmnt-1.0.0.tar", last modified: Sat Apr  6 16:07:00 2024, max compression
+gzip compressed data, was "rmnt-1.0.1.tar", last modified: Sat Apr  6 17:00:47 2024, max compression
```

## Comparing `rmnt-1.0.0.tar` & `rmnt-1.0.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-04-06 16:07:00.728766 rmnt-1.0.0/
--rw-rw-rw-   0        0        0     1101 2024-04-05 18:06:29.000000 rmnt-1.0.0/LICENSE
--rw-rw-rw-   0        0        0       15 2024-04-05 18:02:51.000000 rmnt-1.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0     1306 2024-04-06 16:07:00.723768 rmnt-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      852 2024-04-06 14:37:51.000000 rmnt-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-06 16:07:00.576796 rmnt-1.0.0/rmnt/
--rw-rw-rw-   0        0        0        0 2024-04-05 17:49:26.000000 rmnt-1.0.0/rmnt/__init__.py
--rw-rw-rw-   0        0        0        0 2024-04-06 16:05:49.000000 rmnt-1.0.0/rmnt/__main__.py
--rw-rw-rw-   0        0        0      483 2024-04-06 11:37:28.000000 rmnt-1.0.0/rmnt/exec.py
--rw-rw-rw-   0        0        0      601 2024-04-06 11:43:12.000000 rmnt-1.0.0/rmnt/generator.py
--rw-rw-rw-   0        0        0     2318 2024-04-06 14:05:44.000000 rmnt-1.0.0/rmnt/orchestrator.py
--rw-rw-rw-   0        0        0     1668 2024-04-06 11:48:40.000000 rmnt-1.0.0/rmnt/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-06 16:07:00.714778 rmnt-1.0.0/rmnt.egg-info/
--rw-rw-rw-   0        0        0     1306 2024-04-06 16:06:59.000000 rmnt-1.0.0/rmnt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      308 2024-04-06 16:06:59.000000 rmnt-1.0.0/rmnt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-06 16:06:59.000000 rmnt-1.0.0/rmnt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2024-04-06 16:06:59.000000 rmnt-1.0.0/rmnt.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      599 2024-04-06 16:06:59.000000 rmnt-1.0.0/rmnt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-04-06 16:06:59.000000 rmnt-1.0.0/rmnt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-06 16:07:00.728766 rmnt-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      965 2024-04-06 14:30:47.000000 rmnt-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-06 17:00:46.952747 rmnt-1.0.1/
+-rw-rw-rw-   0        0        0     1101 2024-04-05 18:06:29.000000 rmnt-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0       15 2024-04-05 18:02:51.000000 rmnt-1.0.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     1306 2024-04-06 17:00:46.950749 rmnt-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      852 2024-04-06 14:37:51.000000 rmnt-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-06 17:00:46.636620 rmnt-1.0.1/rmnt/
+-rw-rw-rw-   0        0        0        0 2024-04-05 17:49:26.000000 rmnt-1.0.1/rmnt/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-04-06 16:05:49.000000 rmnt-1.0.1/rmnt/__main__.py
+-rw-rw-rw-   0        0        0      483 2024-04-06 11:37:28.000000 rmnt-1.0.1/rmnt/exec.py
+-rw-rw-rw-   0        0        0      601 2024-04-06 11:43:12.000000 rmnt-1.0.1/rmnt/generator.py
+-rw-rw-rw-   0        0        0     2318 2024-04-06 14:05:44.000000 rmnt-1.0.1/rmnt/orchestrator.py
+-rw-rw-rw-   0        0        0     1668 2024-04-06 11:48:40.000000 rmnt-1.0.1/rmnt/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-06 17:00:46.941755 rmnt-1.0.1/rmnt.egg-info/
+-rw-rw-rw-   0        0        0     1306 2024-04-06 17:00:44.000000 rmnt-1.0.1/rmnt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      308 2024-04-06 17:00:45.000000 rmnt-1.0.1/rmnt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-06 17:00:45.000000 rmnt-1.0.1/rmnt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2024-04-06 17:00:45.000000 rmnt-1.0.1/rmnt.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      599 2024-04-06 17:00:45.000000 rmnt-1.0.1/rmnt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-04-06 17:00:45.000000 rmnt-1.0.1/rmnt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-06 17:00:46.952747 rmnt-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      965 2024-04-06 16:59:05.000000 rmnt-1.0.1/setup.py
```

### Comparing `rmnt-1.0.0/LICENSE` & `rmnt-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rmnt-1.0.0/PKG-INFO` & `rmnt-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rmnt
-Version: 1.0.0
+Version: 1.0.1
 Summary: CLI Scaffolding Tool for web projects with Flask and FastAPI
 Home-page: https://github.com/raghuramjee7/rmnt
 Author: Raghu Ram Jee Janapareddy
 Author-email: ramjeeraghu@gmail.com
 License: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Operating System :: OS Independent
```

### Comparing `rmnt-1.0.0/README.md` & `rmnt-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `rmnt-1.0.0/rmnt/generator.py` & `rmnt-1.0.1/rmnt/generator.py`

 * *Files identical despite different names*

### Comparing `rmnt-1.0.0/rmnt/orchestrator.py` & `rmnt-1.0.1/rmnt/orchestrator.py`

 * *Files identical despite different names*

### Comparing `rmnt-1.0.0/rmnt/utils.py` & `rmnt-1.0.1/rmnt/utils.py`

 * *Files identical despite different names*

### Comparing `rmnt-1.0.0/rmnt.egg-info/PKG-INFO` & `rmnt-1.0.1/rmnt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rmnt
-Version: 1.0.0
+Version: 1.0.1
 Summary: CLI Scaffolding Tool for web projects with Flask and FastAPI
 Home-page: https://github.com/raghuramjee7/rmnt
 Author: Raghu Ram Jee Janapareddy
 Author-email: ramjeeraghu@gmail.com
 License: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Operating System :: OS Independent
```

### Comparing `rmnt-1.0.0/rmnt.egg-info/requires.txt` & `rmnt-1.0.1/rmnt.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `rmnt-1.0.0/setup.py` & `rmnt-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 with open("requirements.txt", "r", encoding="utf-16") as fh:
     requirements = fh.read()
 setup(
     name = 'rmnt',
-    version = '1.0.0',
+    version = '1.0.1',
     author = 'Raghu Ram Jee Janapareddy',
     author_email = 'ramjeeraghu@gmail.com',
     license = 'MIT License',
     description = 'CLI Scaffolding Tool for web projects with Flask and FastAPI',
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = 'https://github.com/raghuramjee7/rmnt',
```

