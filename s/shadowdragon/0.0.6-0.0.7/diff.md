# Comparing `tmp/shadowdragon-0.0.6.tar.gz` & `tmp/shadowdragon-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shadowdragon-0.0.6.tar", last modified: Sat Apr  6 00:09:49 2024, max compression
+gzip compressed data, was "shadowdragon-0.0.7.tar", last modified: Sat Apr  6 00:10:11 2024, max compression
```

## Comparing `shadowdragon-0.0.6.tar` & `shadowdragon-0.0.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 kglick@middlebury.edu   (501) staff       (20)        0 2024-04-06 00:09:49.716896 shadowdragon-0.0.6/
--rw-r--r--   0 kglick@middlebury.edu   (501) staff       (20)     1067 2024-04-05 00:33:01.000000 shadowdragon-0.0.6/LICENSE
--rw-r--r--   0 kglick@middlebury.edu   (501) staff       (20)      609 2024-04-06 00:09:49.714521 shadowdragon-0.0.6/PKG-INFO
--rw-r--r--   0 kglick@middlebury.edu   (501) staff       (20)       49 2024-04-05 00:33:01.000000 shadowdragon-0.0.6/README.md
--rw-r--r--   0 kglick@middlebury.edu   (501) staff       (20)      549 2024-04-05 00:33:02.000000 shadowdragon-0.0.6/pyproject.toml
--rw-r--r--   0 kglick@middlebury.edu   (501) staff       (20)       38 2024-04-06 00:09:49.717063 shadowdragon-0.0.6/setup.cfg
-drwxr-xr-x   0 kglick@middlebury.edu   (501) staff       (20)        0 2024-04-06 00:09:49.673529 shadowdragon-0.0.6/src/
-drwxr-xr-x   0 kglick@middlebury.edu   (501) staff       (20)        0 2024-04-06 00:09:49.681972 shadowdragon-0.0.6/src/shadowdragon/
--rw-r--r--   0 kglick@middlebury.edu   (501) staff       (20)       61 2024-04-05 00:33:02.000000 shadowdragon-0.0.6/src/shadowdragon/__init__.py
--rw-r--r--   0 kglick@middlebury.edu   (501) staff       (20)    31247 2024-04-06 00:06:55.000000 shadowdragon-0.0.6/src/shadowdragon/shadowdragon.py
-drwxr-xr-x   0 kglick@middlebury.edu   (501) staff       (20)        0 2024-04-06 00:09:49.712813 shadowdragon-0.0.6/src/shadowdragon.egg-info/
--rw-r--r--   0 kglick@middlebury.edu   (501) staff       (20)      609 2024-04-06 00:09:49.000000 shadowdragon-0.0.6/src/shadowdragon.egg-info/PKG-INFO
--rw-r--r--   0 kglick@middlebury.edu   (501) staff       (20)      293 2024-04-06 00:09:49.000000 shadowdragon-0.0.6/src/shadowdragon.egg-info/SOURCES.txt
--rw-r--r--   0 kglick@middlebury.edu   (501) staff       (20)        1 2024-04-06 00:09:49.000000 shadowdragon-0.0.6/src/shadowdragon.egg-info/dependency_links.txt
--rw-r--r--   0 kglick@middlebury.edu   (501) staff       (20)        8 2024-04-06 00:09:49.000000 shadowdragon-0.0.6/src/shadowdragon.egg-info/requires.txt
--rw-r--r--   0 kglick@middlebury.edu   (501) staff       (20)       13 2024-04-06 00:09:49.000000 shadowdragon-0.0.6/src/shadowdragon.egg-info/top_level.txt
+drwxr-xr-x   0 kglick@middlebury.edu   (501) staff       (20)        0 2024-04-06 00:10:11.980126 shadowdragon-0.0.7/
+-rw-r--r--   0 kglick@middlebury.edu   (501) staff       (20)     1067 2024-04-05 00:33:01.000000 shadowdragon-0.0.7/LICENSE
+-rw-r--r--   0 kglick@middlebury.edu   (501) staff       (20)      609 2024-04-06 00:10:11.978693 shadowdragon-0.0.7/PKG-INFO
+-rw-r--r--   0 kglick@middlebury.edu   (501) staff       (20)       49 2024-04-05 00:33:01.000000 shadowdragon-0.0.7/README.md
+-rw-r--r--   0 kglick@middlebury.edu   (501) staff       (20)      549 2024-04-06 00:10:03.000000 shadowdragon-0.0.7/pyproject.toml
+-rw-r--r--   0 kglick@middlebury.edu   (501) staff       (20)       38 2024-04-06 00:10:11.980232 shadowdragon-0.0.7/setup.cfg
+drwxr-xr-x   0 kglick@middlebury.edu   (501) staff       (20)        0 2024-04-06 00:10:11.962758 shadowdragon-0.0.7/src/
+drwxr-xr-x   0 kglick@middlebury.edu   (501) staff       (20)        0 2024-04-06 00:10:11.968004 shadowdragon-0.0.7/src/shadowdragon/
+-rw-r--r--   0 kglick@middlebury.edu   (501) staff       (20)       61 2024-04-05 00:33:02.000000 shadowdragon-0.0.7/src/shadowdragon/__init__.py
+-rw-r--r--   0 kglick@middlebury.edu   (501) staff       (20)    31247 2024-04-06 00:06:55.000000 shadowdragon-0.0.7/src/shadowdragon/shadowdragon.py
+drwxr-xr-x   0 kglick@middlebury.edu   (501) staff       (20)        0 2024-04-06 00:10:11.977874 shadowdragon-0.0.7/src/shadowdragon.egg-info/
+-rw-r--r--   0 kglick@middlebury.edu   (501) staff       (20)      609 2024-04-06 00:10:11.000000 shadowdragon-0.0.7/src/shadowdragon.egg-info/PKG-INFO
+-rw-r--r--   0 kglick@middlebury.edu   (501) staff       (20)      293 2024-04-06 00:10:11.000000 shadowdragon-0.0.7/src/shadowdragon.egg-info/SOURCES.txt
+-rw-r--r--   0 kglick@middlebury.edu   (501) staff       (20)        1 2024-04-06 00:10:11.000000 shadowdragon-0.0.7/src/shadowdragon.egg-info/dependency_links.txt
+-rw-r--r--   0 kglick@middlebury.edu   (501) staff       (20)        8 2024-04-06 00:10:11.000000 shadowdragon-0.0.7/src/shadowdragon.egg-info/requires.txt
+-rw-r--r--   0 kglick@middlebury.edu   (501) staff       (20)       13 2024-04-06 00:10:11.000000 shadowdragon-0.0.7/src/shadowdragon.egg-info/top_level.txt
```

### Comparing `shadowdragon-0.0.6/LICENSE` & `shadowdragon-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `shadowdragon-0.0.6/PKG-INFO` & `shadowdragon-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shadowdragon
-Version: 0.0.6
+Version: 0.0.7
 Summary: An async wrapper for the ShadowDragon API
 Author-email: Kojin Glick <kglick@middlebury.edu>
 Project-URL: Homepage, https://github.com/kojinglick-ctec/shadowdragon/
 Project-URL: Issues, https://github.com/kojinglick-ctec/shadowdragon/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `shadowdragon-0.0.6/pyproject.toml` & `shadowdragon-0.0.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "shadowdragon"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="Kojin Glick", email="kglick@middlebury.edu" },
 ]
 description = "An async wrapper for the ShadowDragon API"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `shadowdragon-0.0.6/src/shadowdragon/shadowdragon.py` & `shadowdragon-0.0.7/src/shadowdragon/shadowdragon.py`

 * *Files identical despite different names*

### Comparing `shadowdragon-0.0.6/src/shadowdragon.egg-info/PKG-INFO` & `shadowdragon-0.0.7/src/shadowdragon.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shadowdragon
-Version: 0.0.6
+Version: 0.0.7
 Summary: An async wrapper for the ShadowDragon API
 Author-email: Kojin Glick <kglick@middlebury.edu>
 Project-URL: Homepage, https://github.com/kojinglick-ctec/shadowdragon/
 Project-URL: Issues, https://github.com/kojinglick-ctec/shadowdragon/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

