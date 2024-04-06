# Comparing `tmp/tabletexifier-0.1.9.tar.gz` & `tmp/tabletexifier-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tabletexifier-0.1.9.tar", last modified: Wed May 12 14:34:12 2021, max compression
+gzip compressed data, was "tabletexifier-0.2.tar", last modified: Sat Apr  6 18:36:08 2024, max compression
```

## Comparing `tabletexifier-0.1.9.tar` & `tabletexifier-0.2.tar`

### file list

```diff
@@ -1,18 +1,21 @@
-drwxrwxr-x   0 amiguel   (1000) amiguel   (1000)        0 2021-05-12 14:34:12.000000 tabletexifier-0.1.9/
-drwxrwxr-x   0 amiguel   (1000) amiguel   (1000)        0 2021-05-12 14:34:12.000000 tabletexifier-0.1.9/tabletexifier/
--rw-rw-r--   0 amiguel   (1000) amiguel   (1000)     5885 2021-05-12 14:32:24.000000 tabletexifier-0.1.9/tabletexifier/table_styles.py
--rw-rw-r--   0 amiguel   (1000) amiguel   (1000)     9766 2021-05-12 14:32:24.000000 tabletexifier-0.1.9/tabletexifier/Table.py
--rw-r--r--   0 amiguel   (1000) amiguel   (1000)       24 2020-10-21 15:04:40.000000 tabletexifier-0.1.9/tabletexifier/__init__.py
-drwxrwxr-x   0 amiguel   (1000) amiguel   (1000)        0 2021-05-12 14:34:12.000000 tabletexifier-0.1.9/tabletexifier.egg-info/
--rw-rw-r--   0 amiguel   (1000) amiguel   (1000)        1 2021-05-12 14:34:11.000000 tabletexifier-0.1.9/tabletexifier.egg-info/dependency_links.txt
--rw-rw-r--   0 amiguel   (1000) amiguel   (1000)       19 2021-05-12 14:34:11.000000 tabletexifier-0.1.9/tabletexifier.egg-info/top_level.txt
--rw-rw-r--   0 amiguel   (1000) amiguel   (1000)      317 2021-05-12 14:34:12.000000 tabletexifier-0.1.9/tabletexifier.egg-info/SOURCES.txt
--rw-rw-r--   0 amiguel   (1000) amiguel   (1000)     5902 2021-05-12 14:34:11.000000 tabletexifier-0.1.9/tabletexifier.egg-info/PKG-INFO
--rw-rw-r--   0 amiguel   (1000) amiguel   (1000)     4098 2021-05-12 14:32:24.000000 tabletexifier-0.1.9/README.md
--rw-rw-r--   0 amiguel   (1000) amiguel   (1000)       38 2021-05-12 14:34:12.000000 tabletexifier-0.1.9/setup.cfg
--rw-rw-r--   0 amiguel   (1000) amiguel   (1000)     5902 2021-05-12 14:34:12.000000 tabletexifier-0.1.9/PKG-INFO
--rw-r--r--   0 amiguel   (1000) amiguel   (1000)      635 2021-05-12 14:31:13.000000 tabletexifier-0.1.9/setup.py
-drwxrwxr-x   0 amiguel   (1000) amiguel   (1000)        0 2021-05-12 14:34:12.000000 tabletexifier-0.1.9/test/
--rw-rw-r--   0 amiguel   (1000) amiguel   (1000)      125 2021-05-12 14:32:24.000000 tabletexifier-0.1.9/test/test_table_styles.py
--rw-rw-r--   0 amiguel   (1000) amiguel   (1000)     3901 2021-05-12 14:32:24.000000 tabletexifier-0.1.9/test/test_basic_functions.py
--rw-r--r--   0 amiguel   (1000) amiguel   (1000)        0 2020-10-21 17:44:30.000000 tabletexifier-0.1.9/test/__init__.py
+drwxrwxr-x   0 amiguel   (1000) amiguel   (1000)        0 2024-04-06 18:36:08.621325 tabletexifier-0.2/
+-rw-r--r--   0 amiguel   (1000) amiguel   (1000)    35149 2020-10-21 14:46:33.000000 tabletexifier-0.2/LICENSE
+-rw-rw-r--   0 amiguel   (1000) amiguel   (1000)     1092 2024-04-06 18:36:08.621325 tabletexifier-0.2/PKG-INFO
+-rw-rw-r--   0 amiguel   (1000) amiguel   (1000)      638 2024-04-06 18:35:40.000000 tabletexifier-0.2/README.md
+-rw-rw-r--   0 amiguel   (1000) amiguel   (1000)       38 2024-04-06 18:36:08.625325 tabletexifier-0.2/setup.cfg
+-rw-rw-r--   0 amiguel   (1000) amiguel   (1000)      633 2024-04-06 18:33:11.000000 tabletexifier-0.2/setup.py
+drwxrwxr-x   0 amiguel   (1000) amiguel   (1000)        0 2024-04-06 18:36:08.621325 tabletexifier-0.2/tabletexifier/
+-rw-rw-r--   0 amiguel   (1000) amiguel   (1000)     3258 2024-04-06 18:33:11.000000 tabletexifier-0.2/tabletexifier/Cell.py
+-rw-rw-r--   0 amiguel   (1000) amiguel   (1000)    10990 2024-04-06 18:33:11.000000 tabletexifier-0.2/tabletexifier/Table.py
+-rw-r--r--   0 amiguel   (1000) amiguel   (1000)       24 2020-10-21 15:04:40.000000 tabletexifier-0.2/tabletexifier/__init__.py
+-rw-rw-r--   0 amiguel   (1000) amiguel   (1000)      118 2024-04-06 18:33:11.000000 tabletexifier-0.2/tabletexifier/exceptions.py
+-rw-rw-r--   0 amiguel   (1000) amiguel   (1000)     4881 2024-04-06 18:33:11.000000 tabletexifier-0.2/tabletexifier/table_styles.py
+drwxrwxr-x   0 amiguel   (1000) amiguel   (1000)        0 2024-04-06 18:36:08.621325 tabletexifier-0.2/tabletexifier.egg-info/
+-rw-rw-r--   0 amiguel   (1000) amiguel   (1000)     1092 2024-04-06 18:36:07.000000 tabletexifier-0.2/tabletexifier.egg-info/PKG-INFO
+-rw-rw-r--   0 amiguel   (1000) amiguel   (1000)      375 2024-04-06 18:36:08.000000 tabletexifier-0.2/tabletexifier.egg-info/SOURCES.txt
+-rw-rw-r--   0 amiguel   (1000) amiguel   (1000)        1 2024-04-06 18:36:07.000000 tabletexifier-0.2/tabletexifier.egg-info/dependency_links.txt
+-rw-rw-r--   0 amiguel   (1000) amiguel   (1000)       19 2024-04-06 18:36:08.000000 tabletexifier-0.2/tabletexifier.egg-info/top_level.txt
+drwxrwxr-x   0 amiguel   (1000) amiguel   (1000)        0 2024-04-06 18:36:08.621325 tabletexifier-0.2/test/
+-rw-r--r--   0 amiguel   (1000) amiguel   (1000)        0 2020-10-21 17:44:30.000000 tabletexifier-0.2/test/__init__.py
+-rw-rw-r--   0 amiguel   (1000) amiguel   (1000)     3901 2021-05-12 14:32:24.000000 tabletexifier-0.2/test/test_basic_functions.py
+-rw-rw-r--   0 amiguel   (1000) amiguel   (1000)      125 2021-05-12 14:32:24.000000 tabletexifier-0.2/test/test_table_styles.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `tabletexifier-0.1.9/setup.py` & `tabletexifier-0.2/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
-    name="tabletexifier", 
-    version="0.1.9",
+    name="tabletexifier",
+    version="0.2",
     author="Kamuish",
     author_email="andremiguel952@gmail.com",
     description="Pretty formatted tables that can be exported to LaTeX",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
-    python_requires='>=3.6',
-)
+    python_requires=">=3.6",
+)
```

### Comparing `tabletexifier-0.1.9/test/test_basic_functions.py` & `tabletexifier-0.2/test/test_basic_functions.py`

 * *Files identical despite different names*

