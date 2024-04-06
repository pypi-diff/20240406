# Comparing `tmp/mocker_db-0.0.8.tar.gz` & `tmp/mocker_db-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mocker_db-0.0.8.tar", last modified: Sat Apr  6 02:24:32 2024, max compression
+gzip compressed data, was "mocker_db-0.0.9.tar", last modified: Sat Apr  6 02:37:32 2024, max compression
```

## Comparing `mocker_db-0.0.8.tar` & `mocker_db-0.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 02:24:32.682547 mocker_db-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-06 02:14:17.000000 mocker_db-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8086 2024-04-06 02:24:32.682547 mocker_db-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4534 2024-04-06 02:14:17.000000 mocker_db-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 02:24:32.682547 mocker_db-0.0.8/mocker_db/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-06 02:24:05.000000 mocker_db-0.0.8/mocker_db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26611 2024-04-06 02:24:05.000000 mocker_db-0.0.8/mocker_db/mocker_db.py
--rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-04-06 02:24:32.000000 mocker_db-0.0.8/mocker_db/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 02:24:32.682547 mocker_db-0.0.8/mocker_db.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8086 2024-04-06 02:24:32.000000 mocker_db-0.0.8/mocker_db.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-06 02:24:32.000000 mocker_db-0.0.8/mocker_db.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 02:24:32.000000 mocker_db-0.0.8/mocker_db.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-06 02:24:32.000000 mocker_db-0.0.8/mocker_db.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-06 02:24:32.000000 mocker_db-0.0.8/mocker_db.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 02:24:32.682547 mocker_db-0.0.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 02:37:32.953832 mocker_db-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-06 02:34:22.000000 mocker_db-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8086 2024-04-06 02:37:32.953832 mocker_db-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4534 2024-04-06 02:34:22.000000 mocker_db-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 02:37:32.953832 mocker_db-0.0.9/mocker_db/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-06 02:37:13.000000 mocker_db-0.0.9/mocker_db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26611 2024-04-06 02:37:13.000000 mocker_db-0.0.9/mocker_db/mocker_db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-04-06 02:37:32.000000 mocker_db-0.0.9/mocker_db/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 02:37:32.953832 mocker_db-0.0.9/mocker_db.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8086 2024-04-06 02:37:32.000000 mocker_db-0.0.9/mocker_db.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-06 02:37:32.000000 mocker_db-0.0.9/mocker_db.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 02:37:32.000000 mocker_db-0.0.9/mocker_db.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-06 02:37:32.000000 mocker_db-0.0.9/mocker_db.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-06 02:37:32.000000 mocker_db-0.0.9/mocker_db.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 02:37:32.953832 mocker_db-0.0.9/setup.cfg
```

### Comparing `mocker_db-0.0.8/LICENSE` & `mocker_db-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mocker_db-0.0.8/PKG-INFO` & `mocker_db-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mocker_db
-Version: 0.0.8
+Version: 0.0.9
 Summary: A mock handler for simulating a vector database.
 Author: Kyrylo Mordan
 Author-email: parachute.repo@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
```

### Comparing `mocker_db-0.0.8/README.md` & `mocker_db-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `mocker_db-0.0.8/mocker_db/mocker_db.py` & `mocker_db-0.0.9/mocker_db/mocker_db.py`

 * *Files identical despite different names*

### Comparing `mocker_db-0.0.8/mocker_db/setup.py` & `mocker_db-0.0.9/mocker_db/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,14 @@
       long_description = fh.read()
 else:
   long_description = ''
 
 setup(
     name="mocker_db",
     packages=["mocker_db"],
-    install_requires=['### mocker_db.py', 'dill==0.3.7', 'attrs>=22.2.0', 'numpy', 'sentence-transformers==2.2.2', 'hnswlib==0.8.0'],
+    install_requires=['### mocker_db.py', 'numpy', 'attrs>=22.2.0', 'dill==0.3.7', 'sentence-transformers==2.2.2', 'hnswlib==0.8.0'],
     classifiers=['Development Status :: 3 - Alpha', 'Intended Audience :: Developers', 'Intended Audience :: Science/Research', 'Programming Language :: Python :: 3', 'Programming Language :: Python :: 3.9', 'Programming Language :: Python :: 3.10', 'Programming Language :: Python :: 3.11', 'License :: OSI Approved :: MIT License', 'Topic :: Scientific/Engineering'],
     long_description=long_description,
     long_description_content_type='text/markdown',
-    author="Kyrylo Mordan", author_email="parachute.repo@gmail.com", description="A mock handler for simulating a vector database.", version="0.0.8"
+    author="Kyrylo Mordan", author_email="parachute.repo@gmail.com", description="A mock handler for simulating a vector database.", version="0.0.9"
 )
```

### Comparing `mocker_db-0.0.8/mocker_db.egg-info/PKG-INFO` & `mocker_db-0.0.9/mocker_db.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mocker-db
-Version: 0.0.8
+Version: 0.0.9
 Summary: A mock handler for simulating a vector database.
 Author: Kyrylo Mordan
 Author-email: parachute.repo@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
```

