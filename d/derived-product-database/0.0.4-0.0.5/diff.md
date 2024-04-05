# Comparing `tmp/derived-product-database-0.0.4.tar.gz` & `tmp/derived-product-database-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "derived-product-database-0.0.4.tar", last modified: Fri Apr  5 23:00:33 2024, max compression
+gzip compressed data, was "derived-product-database-0.0.5.tar", last modified: Fri Apr  5 23:06:06 2024, max compression
```

## Comparing `derived-product-database-0.0.4.tar` & `derived-product-database-0.0.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 nharper  (2103922330) GS\Domain Users (346589396)        0 2024-04-05 23:00:33.832067 derived-product-database-0.0.4/
--rw-r--r--   0 nharper  (2103922330) GS\Domain Users (346589396)     7047 2024-04-05 20:17:04.000000 derived-product-database-0.0.4/LICENSE
--rw-r--r--   0 nharper  (2103922330) GS\Domain Users (346589396)    11070 2024-04-05 23:00:33.831431 derived-product-database-0.0.4/PKG-INFO
--rw-r--r--   0 nharper  (2103922330) GS\Domain Users (346589396)     2209 2024-04-02 23:13:12.000000 derived-product-database-0.0.4/README.md
-drwxr-xr-x   0 nharper  (2103922330) GS\Domain Users (346589396)        0 2024-04-05 23:00:33.830747 derived-product-database-0.0.4/derived_product_database.egg-info/
--rw-r--r--   0 nharper  (2103922330) GS\Domain Users (346589396)    11070 2024-04-05 23:00:33.000000 derived-product-database-0.0.4/derived_product_database.egg-info/PKG-INFO
--rw-r--r--   0 nharper  (2103922330) GS\Domain Users (346589396)      271 2024-04-05 23:00:33.000000 derived-product-database-0.0.4/derived_product_database.egg-info/SOURCES.txt
--rw-r--r--   0 nharper  (2103922330) GS\Domain Users (346589396)        1 2024-04-05 23:00:33.000000 derived-product-database-0.0.4/derived_product_database.egg-info/dependency_links.txt
--rw-r--r--   0 nharper  (2103922330) GS\Domain Users (346589396)      104 2024-04-05 23:00:33.000000 derived-product-database-0.0.4/derived_product_database.egg-info/requires.txt
--rw-r--r--   0 nharper  (2103922330) GS\Domain Users (346589396)        1 2024-04-05 23:00:33.000000 derived-product-database-0.0.4/derived_product_database.egg-info/top_level.txt
--rw-r--r--   0 nharper  (2103922330) GS\Domain Users (346589396)      985 2024-04-05 22:57:32.000000 derived-product-database-0.0.4/pyproject.toml
--rw-r--r--   0 nharper  (2103922330) GS\Domain Users (346589396)       38 2024-04-05 23:00:33.832153 derived-product-database-0.0.4/setup.cfg
+drwxr-xr-x   0 nharper  (2103922330) GS\Domain Users (346589396)        0 2024-04-05 23:06:06.401412 derived-product-database-0.0.5/
+-rw-r--r--   0 nharper  (2103922330) GS\Domain Users (346589396)     7047 2024-04-05 20:17:04.000000 derived-product-database-0.0.5/LICENSE
+-rw-r--r--   0 nharper  (2103922330) GS\Domain Users (346589396)    11123 2024-04-05 23:06:06.399115 derived-product-database-0.0.5/PKG-INFO
+-rw-r--r--   0 nharper  (2103922330) GS\Domain Users (346589396)     2209 2024-04-02 23:13:12.000000 derived-product-database-0.0.5/README.md
+drwxr-xr-x   0 nharper  (2103922330) GS\Domain Users (346589396)        0 2024-04-05 23:06:06.395286 derived-product-database-0.0.5/derived_product_database.egg-info/
+-rw-r--r--   0 nharper  (2103922330) GS\Domain Users (346589396)    11123 2024-04-05 23:06:06.000000 derived-product-database-0.0.5/derived_product_database.egg-info/PKG-INFO
+-rw-r--r--   0 nharper  (2103922330) GS\Domain Users (346589396)      271 2024-04-05 23:06:06.000000 derived-product-database-0.0.5/derived_product_database.egg-info/SOURCES.txt
+-rw-r--r--   0 nharper  (2103922330) GS\Domain Users (346589396)        1 2024-04-05 23:06:06.000000 derived-product-database-0.0.5/derived_product_database.egg-info/dependency_links.txt
+-rw-r--r--   0 nharper  (2103922330) GS\Domain Users (346589396)      157 2024-04-05 23:06:06.000000 derived-product-database-0.0.5/derived_product_database.egg-info/requires.txt
+-rw-r--r--   0 nharper  (2103922330) GS\Domain Users (346589396)        1 2024-04-05 23:06:06.000000 derived-product-database-0.0.5/derived_product_database.egg-info/top_level.txt
+-rw-r--r--   0 nharper  (2103922330) GS\Domain Users (346589396)     1038 2024-04-05 23:06:01.000000 derived-product-database-0.0.5/pyproject.toml
+-rw-r--r--   0 nharper  (2103922330) GS\Domain Users (346589396)       38 2024-04-05 23:06:06.401586 derived-product-database-0.0.5/setup.cfg
```

### Comparing `derived-product-database-0.0.4/LICENSE` & `derived-product-database-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `derived-product-database-0.0.4/PKG-INFO` & `derived-product-database-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: derived-product-database
-Version: 0.0.4
+Version: 0.0.5
 Summary: A package for interacting with the USGS influx db
 Author-email: Noah Harper <nharper@usgs.gov>
 License: Creative Commons Legal Code
         
         CC0 1.0 Universal
         
             CREATIVE COMMONS CORPORATION IS NOT A LAW FIRM AND DOES NOT PROVIDE
@@ -128,24 +128,24 @@
 Project-URL: Issues, https://code.usgs.gov/cvo-realtime-seismic/derived-project-database/-/issues
 Keywords: infrasound,seismic,usgs,volcanos
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: numpy
-Requires-Dist: pandas
-Requires-Dist: obspy
-Requires-Dist: influxdb-client
-Requires-Dist: fastapi
-Requires-Dist: pydantic
-Requires-Dist: pydantic_settings
-Requires-Dist: uvicorn[standard]
-Requires-Dist: datetime
-Requires-Dist: loguru
+Requires-Dist: numpy-1.26.4
+Requires-Dist: pandas-2.2.1
+Requires-Dist: obspy-1.4.0
+Requires-Dist: influxdb-client-1.41.0
+Requires-Dist: fastapi-0.110.1
+Requires-Dist: pydantic-2.6.4
+Requires-Dist: pydantic_settings-2.2.1
+Requires-Dist: uvicorn-0.29.0
+Requires-Dist: datetime-5.5
+Requires-Dist: loguru-0.7.2
 
 # Sample GitLab Project
 
 This sample project shows how a project in GitLab looks for demonstration purposes. It contains issues, merge requests and Markdown files in many branches,
 named and filled with lorem ipsum.
 
 You can look around to get an idea how to structure your project and, when done, you can safely delete this project.
```

### Comparing `derived-product-database-0.0.4/README.md` & `derived-product-database-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `derived-product-database-0.0.4/derived_product_database.egg-info/PKG-INFO` & `derived-product-database-0.0.5/derived_product_database.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: derived-product-database
-Version: 0.0.4
+Version: 0.0.5
 Summary: A package for interacting with the USGS influx db
 Author-email: Noah Harper <nharper@usgs.gov>
 License: Creative Commons Legal Code
         
         CC0 1.0 Universal
         
             CREATIVE COMMONS CORPORATION IS NOT A LAW FIRM AND DOES NOT PROVIDE
@@ -128,24 +128,24 @@
 Project-URL: Issues, https://code.usgs.gov/cvo-realtime-seismic/derived-project-database/-/issues
 Keywords: infrasound,seismic,usgs,volcanos
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: numpy
-Requires-Dist: pandas
-Requires-Dist: obspy
-Requires-Dist: influxdb-client
-Requires-Dist: fastapi
-Requires-Dist: pydantic
-Requires-Dist: pydantic_settings
-Requires-Dist: uvicorn[standard]
-Requires-Dist: datetime
-Requires-Dist: loguru
+Requires-Dist: numpy-1.26.4
+Requires-Dist: pandas-2.2.1
+Requires-Dist: obspy-1.4.0
+Requires-Dist: influxdb-client-1.41.0
+Requires-Dist: fastapi-0.110.1
+Requires-Dist: pydantic-2.6.4
+Requires-Dist: pydantic_settings-2.2.1
+Requires-Dist: uvicorn-0.29.0
+Requires-Dist: datetime-5.5
+Requires-Dist: loguru-0.7.2
 
 # Sample GitLab Project
 
 This sample project shows how a project in GitLab looks for demonstration purposes. It contains issues, merge requests and Markdown files in many branches,
 named and filled with lorem ipsum.
 
 You can look around to get an idea how to structure your project and, when done, you can safely delete this project.
```

### Comparing `derived-product-database-0.0.4/pyproject.toml` & `derived-product-database-0.0.5/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 [build-system]
 requires = ["setuptools>=66.1.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "derived-product-database"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Noah Harper", email="nharper@usgs.gov" },
 ]
 description = "A package for interacting with the USGS influx db"
 readme = "README.md"
 requires-python = ">=3.10"
 license = {file = "LICENSE"}
 keywords = ["infrasound", "seismic", "usgs", "volcanos"]
 classifiers = [
     "Programming Language :: Python :: 3.10",
     "Operating System :: OS Independent",
 ]
 dependencies = [
-  "numpy",
-  "pandas",
-  "obspy",
-  "influxdb-client",
-  "fastapi",
-  "pydantic",
-  "pydantic_settings",
-  "uvicorn[standard]",
-  "datetime",
-  "loguru",
+  "numpy-1.26.4",
+  "pandas-2.2.1",
+  "obspy-1.4.0",
+  "influxdb-client-1.41.0",
+  "fastapi-0.110.1",
+  "pydantic-2.6.4",
+  "pydantic_settings-2.2.1",
+  "uvicorn-0.29.0",
+  "datetime-5.5",
+  "loguru-0.7.2",
 ]
 
 [tool.setuptools.packages.find]
 include = ["dpd_service*"]
 exclude = ["dpd_agent*", "docs*", "tests*"]
 
 [project.urls]
```

