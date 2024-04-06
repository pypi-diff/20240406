# Comparing `tmp/reddit2text-0.0.1.tar.gz` & `tmp/reddit2text-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reddit2text-0.0.1.tar", last modified: Tue Mar  5 19:44:12 2024, max compression
+gzip compressed data, was "reddit2text-0.0.2.tar", last modified: Sat Apr  6 18:22:36 2024, max compression
```

## Comparing `reddit2text-0.0.1.tar` & `reddit2text-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-05 19:44:12.587282 reddit2text-0.0.1/
--rw-r--r--   0 root         (0) root         (0)    11357 2024-03-05 18:59:10.000000 reddit2text-0.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)      831 2024-03-05 19:44:12.587282 reddit2text-0.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      120 2024-03-05 18:59:10.000000 reddit2text-0.0.1/README.md
--rw-r--r--   0 root         (0) root         (0)      830 2024-03-05 19:43:26.000000 reddit2text-0.0.1/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-05 19:44:12.583282 reddit2text-0.0.1/reddit2text/
--rw-r--r--   0 root         (0) root         (0)       25 2024-03-05 19:26:14.000000 reddit2text-0.0.1/reddit2text/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1919 2024-03-05 19:26:00.000000 reddit2text-0.0.1/reddit2text/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-05 19:44:12.583282 reddit2text-0.0.1/reddit2text.egg-info/
--rw-r--r--   0 root         (0) root         (0)      831 2024-03-05 19:44:12.000000 reddit2text-0.0.1/reddit2text.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      225 2024-03-05 19:44:12.000000 reddit2text-0.0.1/reddit2text.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-05 19:44:12.000000 reddit2text-0.0.1/reddit2text.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       12 2024-03-05 19:44:12.000000 reddit2text-0.0.1/reddit2text.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-05 19:44:12.587282 reddit2text-0.0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1600 2024-03-05 19:27:51.000000 reddit2text-0.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 18:22:36.092851 reddit2text-0.0.2/
+-rw-r--r--   0 root         (0) root         (0)    11357 2024-03-05 18:59:10.000000 reddit2text-0.0.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      960 2024-04-06 18:22:36.092851 reddit2text-0.0.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      120 2024-03-05 18:59:10.000000 reddit2text-0.0.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 18:22:36.084851 reddit2text-0.0.2/reddit2text/
+-rw-r--r--   0 root         (0) root         (0)       25 2024-03-05 19:26:14.000000 reddit2text-0.0.2/reddit2text/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1919 2024-03-05 19:26:00.000000 reddit2text-0.0.2/reddit2text/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 18:22:36.092851 reddit2text-0.0.2/reddit2text.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      960 2024-04-06 18:22:35.000000 reddit2text-0.0.2/reddit2text.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      244 2024-04-06 18:22:36.000000 reddit2text-0.0.2/reddit2text.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-06 18:22:35.000000 reddit2text-0.0.2/reddit2text.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2024-04-06 18:22:35.000000 reddit2text-0.0.2/reddit2text.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2024-04-06 18:22:35.000000 reddit2text-0.0.2/reddit2text.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-06 18:22:36.092851 reddit2text-0.0.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1600 2024-04-06 18:18:58.000000 reddit2text-0.0.2/setup.py
```

### Comparing `reddit2text-0.0.1/LICENSE` & `reddit2text-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `reddit2text-0.0.1/PKG-INFO` & `reddit2text-0.0.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 Metadata-Version: 2.1
 Name: reddit2text
-Version: 0.0.1
+Version: 0.0.2
 Summary: Convert Reddit posts to text
 Author: Nicholas Hansen-Feruch
-Author-email: Nicholas Hansen-Feruch <nicholas.feruch@gmail.com>
-Project-URL: Homepage, https://github.com/NFeruch/reddit2text
-Project-URL: Issues, https://github.com/NFeruch/reddit2text/issues
+Author-email: nicholas.feruch@gmail.com
+Keywords: python,reddit,text conversion,reddit api,praw,reddit to text,reddit comments,social media analysis
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: praw
 
-# reddit2text
-A python library that converts a reddit post to its textual representation, usually for feeding to an LLM
+
+A Python package for converting Reddit posts into structured text representations.
+This includes the post's title, author, upvotes, and body, along with all comments
+and their hierarchical structure. Ideal for processing, analysis, or feeding into
+natural language models.
```

### Comparing `reddit2text-0.0.1/reddit2text/main.py` & `reddit2text-0.0.2/reddit2text/main.py`

 * *Files identical despite different names*

### Comparing `reddit2text-0.0.1/reddit2text.egg-info/PKG-INFO` & `reddit2text-0.0.2/reddit2text.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 Metadata-Version: 2.1
 Name: reddit2text
-Version: 0.0.1
+Version: 0.0.2
 Summary: Convert Reddit posts to text
 Author: Nicholas Hansen-Feruch
-Author-email: Nicholas Hansen-Feruch <nicholas.feruch@gmail.com>
-Project-URL: Homepage, https://github.com/NFeruch/reddit2text
-Project-URL: Issues, https://github.com/NFeruch/reddit2text/issues
+Author-email: nicholas.feruch@gmail.com
+Keywords: python,reddit,text conversion,reddit api,praw,reddit to text,reddit comments,social media analysis
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: praw
 
-# reddit2text
-A python library that converts a reddit post to its textual representation, usually for feeding to an LLM
+
+A Python package for converting Reddit posts into structured text representations.
+This includes the post's title, author, upvotes, and body, along with all comments
+and their hierarchical structure. Ideal for processing, analysis, or feeding into
+natural language models.
```

### Comparing `reddit2text-0.0.1/setup.py` & `reddit2text-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.1'  # Consider starting with a semantic versioning scheme
+VERSION = '0.0.2'  # Consider starting with a semantic versioning scheme
 DESCRIPTION = 'Convert Reddit posts to text'
 LONG_DESCRIPTION = """
 A Python package for converting Reddit posts into structured text representations.
 This includes the post's title, author, upvotes, and body, along with all comments
 and their hierarchical structure. Ideal for processing, analysis, or feeding into
 natural language models.
 """
```

