# Comparing `tmp/scrapy-influxdb-exporter-1.0.5.tar.gz` & `tmp/scrapy-influxdb-exporter-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrapy-influxdb-exporter-1.0.5.tar", last modified: Tue Apr  2 21:46:40 2024, max compression
+gzip compressed data, was "scrapy-influxdb-exporter-1.0.6.tar", last modified: Sat Apr  6 15:36:26 2024, max compression
```

## Comparing `scrapy-influxdb-exporter-1.0.5.tar` & `scrapy-influxdb-exporter-1.0.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:46:40.241773 scrapy-influxdb-exporter-1.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-02 21:46:35.000000 scrapy-influxdb-exporter-1.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-04-02 21:46:40.241773 scrapy-influxdb-exporter-1.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-04-02 21:46:35.000000 scrapy-influxdb-exporter-1.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-04-02 21:46:35.000000 scrapy-influxdb-exporter-1.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 21:46:40.241773 scrapy-influxdb-exporter-1.0.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:46:40.237773 scrapy-influxdb-exporter-1.0.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:46:40.241773 scrapy-influxdb-exporter-1.0.5/src/scrapy_influxdb_exporter/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 21:46:35.000000 scrapy-influxdb-exporter-1.0.5/src/scrapy_influxdb_exporter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-02 21:46:35.000000 scrapy-influxdb-exporter-1.0.5/src/scrapy_influxdb_exporter/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-04-02 21:46:35.000000 scrapy-influxdb-exporter-1.0.5/src/scrapy_influxdb_exporter/statscollectors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:46:40.241773 scrapy-influxdb-exporter-1.0.5/src/scrapy_influxdb_exporter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-04-02 21:46:40.000000 scrapy-influxdb-exporter-1.0.5/src/scrapy_influxdb_exporter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-02 21:46:40.000000 scrapy-influxdb-exporter-1.0.5/src/scrapy_influxdb_exporter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 21:46:40.000000 scrapy-influxdb-exporter-1.0.5/src/scrapy_influxdb_exporter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-02 21:46:40.000000 scrapy-influxdb-exporter-1.0.5/src/scrapy_influxdb_exporter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-02 21:46:40.000000 scrapy-influxdb-exporter-1.0.5/src/scrapy_influxdb_exporter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:36:26.745947 scrapy-influxdb-exporter-1.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-06 15:36:22.000000 scrapy-influxdb-exporter-1.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-04-06 15:36:26.745947 scrapy-influxdb-exporter-1.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-04-06 15:36:22.000000 scrapy-influxdb-exporter-1.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-04-06 15:36:22.000000 scrapy-influxdb-exporter-1.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 15:36:26.745947 scrapy-influxdb-exporter-1.0.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:36:26.741948 scrapy-influxdb-exporter-1.0.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:36:26.745947 scrapy-influxdb-exporter-1.0.6/src/scrapy_influxdb_exporter/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 15:36:22.000000 scrapy-influxdb-exporter-1.0.6/src/scrapy_influxdb_exporter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-06 15:36:22.000000 scrapy-influxdb-exporter-1.0.6/src/scrapy_influxdb_exporter/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-04-06 15:36:22.000000 scrapy-influxdb-exporter-1.0.6/src/scrapy_influxdb_exporter/statscollectors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:36:26.745947 scrapy-influxdb-exporter-1.0.6/src/scrapy_influxdb_exporter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-04-06 15:36:26.000000 scrapy-influxdb-exporter-1.0.6/src/scrapy_influxdb_exporter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-06 15:36:26.000000 scrapy-influxdb-exporter-1.0.6/src/scrapy_influxdb_exporter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 15:36:26.000000 scrapy-influxdb-exporter-1.0.6/src/scrapy_influxdb_exporter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-06 15:36:26.000000 scrapy-influxdb-exporter-1.0.6/src/scrapy_influxdb_exporter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-06 15:36:26.000000 scrapy-influxdb-exporter-1.0.6/src/scrapy_influxdb_exporter.egg-info/top_level.txt
```

### Comparing `scrapy-influxdb-exporter-1.0.5/LICENSE` & `scrapy-influxdb-exporter-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `scrapy-influxdb-exporter-1.0.5/PKG-INFO` & `scrapy-influxdb-exporter-1.0.6/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,39 +1,47 @@
 Metadata-Version: 2.1
 Name: scrapy-influxdb-exporter
-Version: 1.0.5
+Version: 1.0.6
 Summary: A simple package to export Scrapy spider stats to InfluxDB
 Author-email: Stefano Fusai <stefanofusai@gmail.com>
 Project-URL: Homepage, https://github.com/stefanofusai/scrapy-influxdb-exporter
 Project-URL: Repository, https://github.com/stefanofusai/scrapy-influxdb-exporter
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: influxdb3-python
 Requires-Dist: scrapy
 
 # scrapy-influxdb-exporter
+
 A simple package to export Scrapy spider stats to InfluxDB.
 
 ## Installation
+
 ```bash
 pip install scrapy-influxdb-exporter
 ```
 
 ## Usage
+
 Add the following settings to your Scrapy project settings file:
+
 ```python
 INFLUXDB_DATABASE = ...
 INFLUXDB_HOST = ...
+INFLUXDB_MEASUREMENT_NAME = ...
 INFLUXDB_ORG = ...
 INFLUXDB_TOKEN = ...
 STATS_CLASS = "scrapy_influxdb_exporter.statscollectors.InfluxDBStatsCollector"
 ```
 
 ## Acknowledgments
+
 This project was inspired by [scrapy-prometheus-exporter](https://github.com/rangertaha/scrapy-prometheus-exporter) by [@rangertaha](https://github.com/rangertaha) and [this article](https://mikulskibartosz.name/how-to-monitor-scrapy-spiders-using-influxdb-and-grafana) by [@mikulskibartosz](https://github.com/mikulskibartosz).
 
 ## Contributing
+
 Contributions are welcome! To get started, please refer to our [contribution guidelines](https://github.com/stefanofusai/scrapy-influxdb-exporter/blob/main/CONTRIBUTING.md).
 
 ## Issues
+
 If you encounter any problems while using this package, please open a new issue [here](https://github.com/stefanofusai/scrapy-influxdb-exporter/issues).
```

### Comparing `scrapy-influxdb-exporter-1.0.5/README.md` & `scrapy-influxdb-exporter-1.0.6/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,34 @@
 # scrapy-influxdb-exporter
+
 A simple package to export Scrapy spider stats to InfluxDB.
 
 ## Installation
+
 ```bash
 pip install scrapy-influxdb-exporter
 ```
 
 ## Usage
+
 Add the following settings to your Scrapy project settings file:
+
 ```python
 INFLUXDB_DATABASE = ...
 INFLUXDB_HOST = ...
+INFLUXDB_MEASUREMENT_NAME = ...
 INFLUXDB_ORG = ...
 INFLUXDB_TOKEN = ...
 STATS_CLASS = "scrapy_influxdb_exporter.statscollectors.InfluxDBStatsCollector"
 ```
 
 ## Acknowledgments
+
 This project was inspired by [scrapy-prometheus-exporter](https://github.com/rangertaha/scrapy-prometheus-exporter) by [@rangertaha](https://github.com/rangertaha) and [this article](https://mikulskibartosz.name/how-to-monitor-scrapy-spiders-using-influxdb-and-grafana) by [@mikulskibartosz](https://github.com/mikulskibartosz).
 
 ## Contributing
+
 Contributions are welcome! To get started, please refer to our [contribution guidelines](https://github.com/stefanofusai/scrapy-influxdb-exporter/blob/main/CONTRIBUTING.md).
 
 ## Issues
+
 If you encounter any problems while using this package, please open a new issue [here](https://github.com/stefanofusai/scrapy-influxdb-exporter/issues).
```

### Comparing `scrapy-influxdb-exporter-1.0.5/pyproject.toml` & `scrapy-influxdb-exporter-1.0.6/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "scrapy-influxdb-exporter"
-version = "1.0.5"
+version = "1.0.6"
 authors = [{ "name" = "Stefano Fusai", "email" = "stefanofusai@gmail.com" }]
 description = "A simple package to export Scrapy spider stats to InfluxDB"
 readme = "README.md"
 requires-python = ">=3.11"
 dependencies = ["influxdb3-python", "scrapy"]
 
 [project.urls]
```

### Comparing `scrapy-influxdb-exporter-1.0.5/src/scrapy_influxdb_exporter.egg-info/PKG-INFO` & `scrapy-influxdb-exporter-1.0.6/src/scrapy_influxdb_exporter.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,39 +1,47 @@
 Metadata-Version: 2.1
 Name: scrapy-influxdb-exporter
-Version: 1.0.5
+Version: 1.0.6
 Summary: A simple package to export Scrapy spider stats to InfluxDB
 Author-email: Stefano Fusai <stefanofusai@gmail.com>
 Project-URL: Homepage, https://github.com/stefanofusai/scrapy-influxdb-exporter
 Project-URL: Repository, https://github.com/stefanofusai/scrapy-influxdb-exporter
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: influxdb3-python
 Requires-Dist: scrapy
 
 # scrapy-influxdb-exporter
+
 A simple package to export Scrapy spider stats to InfluxDB.
 
 ## Installation
+
 ```bash
 pip install scrapy-influxdb-exporter
 ```
 
 ## Usage
+
 Add the following settings to your Scrapy project settings file:
+
 ```python
 INFLUXDB_DATABASE = ...
 INFLUXDB_HOST = ...
+INFLUXDB_MEASUREMENT_NAME = ...
 INFLUXDB_ORG = ...
 INFLUXDB_TOKEN = ...
 STATS_CLASS = "scrapy_influxdb_exporter.statscollectors.InfluxDBStatsCollector"
 ```
 
 ## Acknowledgments
+
 This project was inspired by [scrapy-prometheus-exporter](https://github.com/rangertaha/scrapy-prometheus-exporter) by [@rangertaha](https://github.com/rangertaha) and [this article](https://mikulskibartosz.name/how-to-monitor-scrapy-spiders-using-influxdb-and-grafana) by [@mikulskibartosz](https://github.com/mikulskibartosz).
 
 ## Contributing
+
 Contributions are welcome! To get started, please refer to our [contribution guidelines](https://github.com/stefanofusai/scrapy-influxdb-exporter/blob/main/CONTRIBUTING.md).
 
 ## Issues
+
 If you encounter any problems while using this package, please open a new issue [here](https://github.com/stefanofusai/scrapy-influxdb-exporter/issues).
```

