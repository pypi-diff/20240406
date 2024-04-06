# Comparing `tmp/sdrf-pipelines-0.0.8.tar.gz` & `tmp/sdrf-pipelines-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sdrf-pipelines-0.0.8.tar", last modified: Thu Jul  9 21:46:43 2020, max compression
+gzip compressed data, was "dist/sdrf-pipelines-0.0.9.tar", last modified: Fri Jul 10 20:27:04 2020, max compression
```

## Comparing `sdrf-pipelines-0.0.8.tar` & `sdrf-pipelines-0.0.9.tar`

### file list

```diff
@@ -1,37 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-07-09 21:46:43.554175 sdrf-pipelines-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (116)    11357 2020-07-09 21:46:35.000000 sdrf-pipelines-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)     8519 2020-07-09 21:46:43.554175 sdrf-pipelines-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     6894 2020-07-09 21:46:35.000000 sdrf-pipelines-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-07-09 21:46:43.550175 sdrf-pipelines-0.0.8/sdrf_pipelines/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-07-09 21:46:35.000000 sdrf-pipelines-0.0.8/sdrf_pipelines/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-07-09 21:46:43.554175 sdrf-pipelines-0.0.8/sdrf_pipelines/maxquant/
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-07-09 21:46:35.000000 sdrf-pipelines-0.0.8/sdrf_pipelines/maxquant/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    83450 2020-07-09 21:46:35.000000 sdrf-pipelines-0.0.8/sdrf_pipelines/maxquant/maxquant.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-07-09 21:46:43.554175 sdrf-pipelines-0.0.8/sdrf_pipelines/openms/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-07-09 21:46:35.000000 sdrf-pipelines-0.0.8/sdrf_pipelines/openms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    15776 2020-07-09 21:46:35.000000 sdrf-pipelines-0.0.8/sdrf_pipelines/openms/openms.py
--rw-r--r--   0 runner    (1001) docker     (116)     4660 2020-07-09 21:46:35.000000 sdrf-pipelines-0.0.8/sdrf_pipelines/openms/unimod.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     4621 2020-07-09 21:46:35.000000 sdrf-pipelines-0.0.8/sdrf_pipelines/parse_sdrf.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-07-09 21:46:43.554175 sdrf-pipelines-0.0.8/sdrf_pipelines/sdrf/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-07-09 21:46:35.000000 sdrf-pipelines-0.0.8/sdrf_pipelines/sdrf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2219 2020-07-09 21:46:35.000000 sdrf-pipelines-0.0.8/sdrf_pipelines/sdrf/sdrf.py
--rw-r--r--   0 runner    (1001) docker     (116)    14632 2020-07-09 21:46:35.000000 sdrf-pipelines-0.0.8/sdrf_pipelines/sdrf/sdrf_schema.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-07-09 21:46:43.554175 sdrf-pipelines-0.0.8/sdrf_pipelines/tests/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-07-09 21:46:35.000000 sdrf-pipelines-0.0.8/sdrf_pipelines/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1379 2020-07-09 21:46:35.000000 sdrf-pipelines-0.0.8/sdrf_pipelines/tests/sdrfchecker_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-07-09 21:46:43.554175 sdrf-pipelines-0.0.8/sdrf_pipelines/utils/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-07-09 21:46:35.000000 sdrf-pipelines-0.0.8/sdrf_pipelines/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1187 2020-07-09 21:46:35.000000 sdrf-pipelines-0.0.8/sdrf_pipelines/utils/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-07-09 21:46:43.554175 sdrf-pipelines-0.0.8/sdrf_pipelines/zooma/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-07-09 21:46:35.000000 sdrf-pipelines-0.0.8/sdrf_pipelines/zooma/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     6249 2020-07-09 21:46:35.000000 sdrf-pipelines-0.0.8/sdrf_pipelines/zooma/ols.py
--rw-r--r--   0 runner    (1001) docker     (116)     4014 2020-07-09 21:46:35.000000 sdrf-pipelines-0.0.8/sdrf_pipelines/zooma/zooma.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-07-09 21:46:43.554175 sdrf-pipelines-0.0.8/sdrf_pipelines.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     8519 2020-07-09 21:46:43.000000 sdrf-pipelines-0.0.8/sdrf_pipelines.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      811 2020-07-09 21:46:43.000000 sdrf-pipelines-0.0.8/sdrf_pipelines.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-07-09 21:46:43.000000 sdrf-pipelines-0.0.8/sdrf_pipelines.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       63 2020-07-09 21:46:43.000000 sdrf-pipelines-0.0.8/sdrf_pipelines.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (116)       43 2020-07-09 21:46:43.000000 sdrf-pipelines-0.0.8/sdrf_pipelines.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       15 2020-07-09 21:46:43.000000 sdrf-pipelines-0.0.8/sdrf_pipelines.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)       38 2020-07-09 21:46:43.554175 sdrf-pipelines-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1147 2020-07-09 21:46:35.000000 sdrf-pipelines-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-07-10 20:27:04.849058 sdrf-pipelines-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (116)    11357 2020-07-10 20:26:53.000000 sdrf-pipelines-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (116)      144 2020-07-10 20:26:53.000000 sdrf-pipelines-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (116)     8519 2020-07-10 20:27:04.849058 sdrf-pipelines-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     6894 2020-07-10 20:26:53.000000 sdrf-pipelines-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-07-10 20:27:04.845057 sdrf-pipelines-0.0.9/sdrf_pipelines/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2020-07-10 20:26:53.000000 sdrf-pipelines-0.0.9/sdrf_pipelines/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-07-10 20:27:04.845057 sdrf-pipelines-0.0.9/sdrf_pipelines/maxquant/
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2020-07-10 20:26:53.000000 sdrf-pipelines-0.0.9/sdrf_pipelines/maxquant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)    83450 2020-07-10 20:26:53.000000 sdrf-pipelines-0.0.9/sdrf_pipelines/maxquant/maxquant.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-07-10 20:27:04.845057 sdrf-pipelines-0.0.9/sdrf_pipelines/openms/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2020-07-10 20:26:53.000000 sdrf-pipelines-0.0.9/sdrf_pipelines/openms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)    15776 2020-07-10 20:26:53.000000 sdrf-pipelines-0.0.9/sdrf_pipelines/openms/openms.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4660 2020-07-10 20:26:53.000000 sdrf-pipelines-0.0.9/sdrf_pipelines/openms/unimod.py
+-rw-r--r--   0 runner    (1001) docker     (116)  2386895 2020-07-10 20:26:53.000000 sdrf-pipelines-0.0.9/sdrf_pipelines/openms/unimod.xml
+-rwxr-xr-x   0 runner    (1001) docker     (116)     4621 2020-07-10 20:26:53.000000 sdrf-pipelines-0.0.9/sdrf_pipelines/parse_sdrf.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-07-10 20:27:04.849058 sdrf-pipelines-0.0.9/sdrf_pipelines/sdrf/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2020-07-10 20:26:53.000000 sdrf-pipelines-0.0.9/sdrf_pipelines/sdrf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2219 2020-07-10 20:26:53.000000 sdrf-pipelines-0.0.9/sdrf_pipelines/sdrf/sdrf.py
+-rw-r--r--   0 runner    (1001) docker     (116)    14632 2020-07-10 20:26:53.000000 sdrf-pipelines-0.0.9/sdrf_pipelines/sdrf/sdrf_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-07-10 20:27:04.849058 sdrf-pipelines-0.0.9/sdrf_pipelines/tests/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2020-07-10 20:26:53.000000 sdrf-pipelines-0.0.9/sdrf_pipelines/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1379 2020-07-10 20:26:53.000000 sdrf-pipelines-0.0.9/sdrf_pipelines/tests/sdrfchecker_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-07-10 20:27:04.849058 sdrf-pipelines-0.0.9/sdrf_pipelines/utils/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2020-07-10 20:26:53.000000 sdrf-pipelines-0.0.9/sdrf_pipelines/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1187 2020-07-10 20:26:53.000000 sdrf-pipelines-0.0.9/sdrf_pipelines/utils/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-07-10 20:27:04.849058 sdrf-pipelines-0.0.9/sdrf_pipelines/zooma/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2020-07-10 20:26:53.000000 sdrf-pipelines-0.0.9/sdrf_pipelines/zooma/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6249 2020-07-10 20:26:53.000000 sdrf-pipelines-0.0.9/sdrf_pipelines/zooma/ols.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4014 2020-07-10 20:26:53.000000 sdrf-pipelines-0.0.9/sdrf_pipelines/zooma/zooma.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-07-10 20:27:04.845057 sdrf-pipelines-0.0.9/sdrf_pipelines.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)     8519 2020-07-10 20:27:04.000000 sdrf-pipelines-0.0.9/sdrf_pipelines.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)      856 2020-07-10 20:27:04.000000 sdrf-pipelines-0.0.9/sdrf_pipelines.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2020-07-10 20:27:04.000000 sdrf-pipelines-0.0.9/sdrf_pipelines.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       63 2020-07-10 20:27:04.000000 sdrf-pipelines-0.0.9/sdrf_pipelines.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       43 2020-07-10 20:27:04.000000 sdrf-pipelines-0.0.9/sdrf_pipelines.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       15 2020-07-10 20:27:04.000000 sdrf-pipelines-0.0.9/sdrf_pipelines.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       38 2020-07-10 20:27:04.849058 sdrf-pipelines-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)     1183 2020-07-10 20:26:53.000000 sdrf-pipelines-0.0.9/setup.py
```

### Comparing `sdrf-pipelines-0.0.8/LICENSE` & `sdrf-pipelines-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `sdrf-pipelines-0.0.8/PKG-INFO` & `sdrf-pipelines-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdrf-pipelines
-Version: 0.0.8
+Version: 0.0.9
 Summary: Translate, convert SDRF to configuration pipelines
 Home-page: https://github.com/bigbio/sdrf-pipelines
 Author: BigBio Team
 Author-email: ypriverol@gmail.com
 License: 'Apache 2.0
 Description: # sdrf-pipelines
```

### Comparing `sdrf-pipelines-0.0.8/README.md` & `sdrf-pipelines-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `sdrf-pipelines-0.0.8/sdrf_pipelines/maxquant/maxquant.py` & `sdrf-pipelines-0.0.9/sdrf_pipelines/maxquant/maxquant.py`

 * *Files identical despite different names*

### Comparing `sdrf-pipelines-0.0.8/sdrf_pipelines/openms/openms.py` & `sdrf-pipelines-0.0.9/sdrf_pipelines/openms/openms.py`

 * *Files identical despite different names*

### Comparing `sdrf-pipelines-0.0.8/sdrf_pipelines/openms/unimod.py` & `sdrf-pipelines-0.0.9/sdrf_pipelines/openms/unimod.py`

 * *Files identical despite different names*

### Comparing `sdrf-pipelines-0.0.8/sdrf_pipelines/parse_sdrf.py` & `sdrf-pipelines-0.0.9/sdrf_pipelines/parse_sdrf.py`

 * *Files identical despite different names*

### Comparing `sdrf-pipelines-0.0.8/sdrf_pipelines/sdrf/sdrf.py` & `sdrf-pipelines-0.0.9/sdrf_pipelines/sdrf/sdrf.py`

 * *Files identical despite different names*

### Comparing `sdrf-pipelines-0.0.8/sdrf_pipelines/sdrf/sdrf_schema.py` & `sdrf-pipelines-0.0.9/sdrf_pipelines/sdrf/sdrf_schema.py`

 * *Files identical despite different names*

### Comparing `sdrf-pipelines-0.0.8/sdrf_pipelines/tests/sdrfchecker_tests.py` & `sdrf-pipelines-0.0.9/sdrf_pipelines/tests/sdrfchecker_tests.py`

 * *Files identical despite different names*

### Comparing `sdrf-pipelines-0.0.8/sdrf_pipelines/utils/exceptions.py` & `sdrf-pipelines-0.0.9/sdrf_pipelines/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `sdrf-pipelines-0.0.8/sdrf_pipelines/zooma/ols.py` & `sdrf-pipelines-0.0.9/sdrf_pipelines/zooma/ols.py`

 * *Files identical despite different names*

### Comparing `sdrf-pipelines-0.0.8/sdrf_pipelines/zooma/zooma.py` & `sdrf-pipelines-0.0.9/sdrf_pipelines/zooma/zooma.py`

 * *Files identical despite different names*

### Comparing `sdrf-pipelines-0.0.8/sdrf_pipelines.egg-info/PKG-INFO` & `sdrf-pipelines-0.0.9/sdrf_pipelines.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdrf-pipelines
-Version: 0.0.8
+Version: 0.0.9
 Summary: Translate, convert SDRF to configuration pipelines
 Home-page: https://github.com/bigbio/sdrf-pipelines
 Author: BigBio Team
 Author-email: ypriverol@gmail.com
 License: 'Apache 2.0
 Description: # sdrf-pipelines
```

### Comparing `sdrf-pipelines-0.0.8/sdrf_pipelines.egg-info/SOURCES.txt` & `sdrf-pipelines-0.0.9/sdrf_pipelines.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 LICENSE
+MANIFEST.in
 README.md
 setup.py
 sdrf_pipelines/__init__.py
 sdrf_pipelines/parse_sdrf.py
 sdrf_pipelines.egg-info/PKG-INFO
 sdrf_pipelines.egg-info/SOURCES.txt
 sdrf_pipelines.egg-info/dependency_links.txt
@@ -10,14 +11,15 @@
 sdrf_pipelines.egg-info/requires.txt
 sdrf_pipelines.egg-info/top_level.txt
 sdrf_pipelines/maxquant/__init__.py
 sdrf_pipelines/maxquant/maxquant.py
 sdrf_pipelines/openms/__init__.py
 sdrf_pipelines/openms/openms.py
 sdrf_pipelines/openms/unimod.py
+sdrf_pipelines/openms/unimod.xml
 sdrf_pipelines/sdrf/__init__.py
 sdrf_pipelines/sdrf/sdrf.py
 sdrf_pipelines/sdrf/sdrf_schema.py
 sdrf_pipelines/tests/__init__.py
 sdrf_pipelines/tests/sdrfchecker_tests.py
 sdrf_pipelines/utils/__init__.py
 sdrf_pipelines/utils/exceptions.py
```

### Comparing `sdrf-pipelines-0.0.8/setup.py` & `sdrf-pipelines-0.0.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding='UTF-8') as fh:
     long_description = fh.read()
 
 setup(
   name="sdrf-pipelines",
-  version="0.0.8",
+  version="0.0.9",
   author="BigBio Team",
   author_email="ypriverol@gmail.com",
   description="Translate, convert SDRF to configuration pipelines",
   long_description_content_type="text/markdown",
   long_description=long_description,
   license="'Apache 2.0",
-  data_files=[("", ["LICENSE"])],
+  data_files=[("", ["LICENSE", "sdrf_pipelines/openms/unimod.xml"])],
   package_data={'': ['*.xml'],},
   url="https://github.com/bigbio/sdrf-pipelines",
   packages=find_packages(),
   install_requires=['click', 'pandas', 'pandas_schema', 'requests', 'pytest'],
   entry_points={
     'console_scripts': [
       'parse_sdrf = sdrf_pipelines.parse_sdrf:main'
@@ -27,10 +27,10 @@
   classifiers=[
       "Programming Language :: Python :: 3",
       "License :: OSI Approved :: Apache Software License",
       "Operating System :: OS Independent",
       'Topic :: Scientific/Engineering :: Bio-Informatics'
   ],
   keywords='sdrf python multiomics proteomics',
-  python_requires='>=3.6',
   include_package_data=True,
+  python_requires='>=3.6',
 )
```

