# Comparing `tmp/reddit2text-0.0.2.tar.gz` & `tmp/reddit2text-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reddit2text-0.0.2.tar", last modified: Sat Apr  6 18:22:36 2024, max compression
+gzip compressed data, was "reddit2text-0.0.4.tar", last modified: Sat Apr  6 18:52:20 2024, max compression
```

## Comparing `reddit2text-0.0.2.tar` & `reddit2text-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 18:22:36.092851 reddit2text-0.0.2/
--rw-r--r--   0 root         (0) root         (0)    11357 2024-03-05 18:59:10.000000 reddit2text-0.0.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)      960 2024-04-06 18:22:36.092851 reddit2text-0.0.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      120 2024-03-05 18:59:10.000000 reddit2text-0.0.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 18:22:36.084851 reddit2text-0.0.2/reddit2text/
--rw-r--r--   0 root         (0) root         (0)       25 2024-03-05 19:26:14.000000 reddit2text-0.0.2/reddit2text/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1919 2024-03-05 19:26:00.000000 reddit2text-0.0.2/reddit2text/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 18:22:36.092851 reddit2text-0.0.2/reddit2text.egg-info/
--rw-r--r--   0 root         (0) root         (0)      960 2024-04-06 18:22:35.000000 reddit2text-0.0.2/reddit2text.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      244 2024-04-06 18:22:36.000000 reddit2text-0.0.2/reddit2text.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-06 18:22:35.000000 reddit2text-0.0.2/reddit2text.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        5 2024-04-06 18:22:35.000000 reddit2text-0.0.2/reddit2text.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2024-04-06 18:22:35.000000 reddit2text-0.0.2/reddit2text.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-06 18:22:36.092851 reddit2text-0.0.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1600 2024-04-06 18:18:58.000000 reddit2text-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:52:20.273206 reddit2text-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-06 18:52:16.000000 reddit2text-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-04-06 18:52:20.273206 reddit2text-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-06 18:52:16.000000 reddit2text-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:52:20.269206 reddit2text-0.0.4/reddit2text/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-06 18:52:16.000000 reddit2text-0.0.4/reddit2text/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-04-06 18:52:16.000000 reddit2text-0.0.4/reddit2text/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:52:20.273206 reddit2text-0.0.4/reddit2text.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-04-06 18:52:20.000000 reddit2text-0.0.4/reddit2text.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-06 18:52:20.000000 reddit2text-0.0.4/reddit2text.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 18:52:20.000000 reddit2text-0.0.4/reddit2text.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-06 18:52:20.000000 reddit2text-0.0.4/reddit2text.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-06 18:52:20.000000 reddit2text-0.0.4/reddit2text.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 18:52:20.273206 reddit2text-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-04-06 18:52:16.000000 reddit2text-0.0.4/setup.py
```

### Comparing `reddit2text-0.0.2/LICENSE` & `reddit2text-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `reddit2text-0.0.2/PKG-INFO` & `reddit2text-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reddit2text
-Version: 0.0.2
+Version: 0.0.4
 Summary: Convert Reddit posts to text
 Author: Nicholas Hansen-Feruch
 Author-email: nicholas.feruch@gmail.com
 Keywords: python,reddit,text conversion,reddit api,praw,reddit to text,reddit comments,social media analysis
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `reddit2text-0.0.2/reddit2text/main.py` & `reddit2text-0.0.4/reddit2text/main.py`

 * *Files identical despite different names*

### Comparing `reddit2text-0.0.2/reddit2text.egg-info/PKG-INFO` & `reddit2text-0.0.4/reddit2text.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reddit2text
-Version: 0.0.2
+Version: 0.0.4
 Summary: Convert Reddit posts to text
 Author: Nicholas Hansen-Feruch
 Author-email: nicholas.feruch@gmail.com
 Keywords: python,reddit,text conversion,reddit api,praw,reddit to text,reddit comments,social media analysis
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `reddit2text-0.0.2/setup.py` & `reddit2text-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.2'  # Consider starting with a semantic versioning scheme
+VERSION = '0.0.4'  # Consider starting with a semantic versioning scheme
 DESCRIPTION = 'Convert Reddit posts to text'
 LONG_DESCRIPTION = """
 A Python package for converting Reddit posts into structured text representations.
 This includes the post's title, author, upvotes, and body, along with all comments
 and their hierarchical structure. Ideal for processing, analysis, or feeding into
 natural language models.
 """
```

