# Comparing `tmp/service_oriented-0.0.2a9.tar.gz` & `tmp/service_oriented-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "service_oriented-0.0.2a9.tar", last modified: Sun Jan 28 14:12:50 2024, max compression
+gzip compressed data, was "service_oriented-0.0.3.tar", last modified: Sat Apr  6 21:52:17 2024, max compression
```

## Comparing `service_oriented-0.0.2a9.tar` & `service_oriented-0.0.3.tar`

### file list

```diff
@@ -1,27 +1,92 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 14:12:50.990145 service_oriented-0.0.2a9/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-01-28 14:12:12.000000 service_oriented-0.0.2a9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-01-28 14:12:12.000000 service_oriented-0.0.2a9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2995 2024-01-28 14:12:50.990145 service_oriented-0.0.2a9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-01-28 14:12:12.000000 service_oriented-0.0.2a9/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-01-28 14:12:12.000000 service_oriented-0.0.2a9/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)      891 2024-01-28 14:12:12.000000 service_oriented-0.0.2a9/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 14:12:50.982145 service_oriented-0.0.2a9/service_oriented/
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-01-28 14:12:12.000000 service_oriented-0.0.2a9/service_oriented/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 14:12:50.982145 service_oriented-0.0.2a9/service_oriented/application/
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-01-28 14:12:12.000000 service_oriented-0.0.2a9/service_oriented/application/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-01-28 14:12:12.000000 service_oriented-0.0.2a9/service_oriented/application/base_application.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 14:12:50.982145 service_oriented-0.0.2a9/service_oriented/application/config/
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-01-28 14:12:12.000000 service_oriented-0.0.2a9/service_oriented/application/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-01-28 14:12:12.000000 service_oriented-0.0.2a9/service_oriented/application/config/base_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2038 2024-01-28 14:12:12.000000 service_oriented-0.0.2a9/service_oriented/application/config/yaml_config_settings_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-01-28 14:12:12.000000 service_oriented-0.0.2a9/service_oriented/application/entry_point_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)      941 2024-01-28 14:12:12.000000 service_oriented-0.0.2a9/service_oriented/deployment_environment.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-28 14:12:12.000000 service_oriented-0.0.2a9/service_oriented/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 14:12:50.982145 service_oriented-0.0.2a9/service_oriented.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2995 2024-01-28 14:12:50.000000 service_oriented-0.0.2a9/service_oriented.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-01-28 14:12:50.000000 service_oriented-0.0.2a9/service_oriented.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-28 14:12:50.000000 service_oriented-0.0.2a9/service_oriented.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-01-28 14:12:50.000000 service_oriented-0.0.2a9/service_oriented.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-01-28 14:12:50.000000 service_oriented-0.0.2a9/service_oriented.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-01-28 14:12:50.990145 service_oriented-0.0.2a9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2609 2024-01-28 14:12:12.000000 service_oriented-0.0.2a9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 21:52:17.679363 service_oriented-0.0.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 21:52:17.663363 service_oriented-0.0.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 21:52:17.667363 service_oriented-0.0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-04-06 21:51:33.000000 service_oriented-0.0.3/.github/workflows/main-branch.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-04-06 21:51:33.000000 service_oriented-0.0.3/.github/workflows/other-branch.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2627 2024-04-06 21:51:33.000000 service_oriented-0.0.3/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3128 2024-04-06 21:51:33.000000 service_oriented-0.0.3/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 21:52:17.663363 service_oriented-0.0.3/.meta/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 21:52:17.667363 service_oriented-0.0.3/.meta/coverage/
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-04-06 21:52:14.000000 service_oriented-0.0.3/.meta/coverage/badge.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     4988 2024-04-06 21:52:14.000000 service_oriented-0.0.3/.meta/coverage/report.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1948 2024-04-06 21:51:33.000000 service_oriented-0.0.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-06 21:51:33.000000 service_oriented-0.0.3/.safety-policy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-06 21:51:33.000000 service_oriented-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-06 21:51:33.000000 service_oriented-0.0.3/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     2613 2024-04-06 21:52:17.679363 service_oriented-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-06 21:51:33.000000 service_oriented-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 21:52:17.667363 service_oriented-0.0.3/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      511 2024-04-06 21:51:33.000000 service_oriented-0.0.3/bin/run-example-application
+-rw-r--r--   0 runner    (1001) docker     (127)     2968 2024-04-06 21:51:33.000000 service_oriented-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-04-06 21:51:57.000000 service_oriented-0.0.3/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 21:52:17.667363 service_oriented-0.0.3/service_oriented/
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-06 21:51:33.000000 service_oriented-0.0.3/service_oriented/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-06 21:52:17.000000 service_oriented-0.0.3/service_oriented/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 21:52:17.667363 service_oriented-0.0.3/service_oriented/application/
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-06 21:51:33.000000 service_oriented-0.0.3/service_oriented/application/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-04-06 21:51:33.000000 service_oriented-0.0.3/service_oriented/application/abstract_composition_root.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-04-06 21:51:33.000000 service_oriented-0.0.3/service_oriented/application/base_application.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 21:52:17.671363 service_oriented-0.0.3/service_oriented/application/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-06 21:51:33.000000 service_oriented-0.0.3/service_oriented/application/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2560 2024-04-06 21:51:33.000000 service_oriented-0.0.3/service_oriented/application/config/base_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2046 2024-04-06 21:51:33.000000 service_oriented-0.0.3/service_oriented/application/config/yaml_config_settings_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-04-06 21:51:33.000000 service_oriented-0.0.3/service_oriented/application/entry_point_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-04-06 21:51:33.000000 service_oriented-0.0.3/service_oriented/application/generic_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2024-04-06 21:51:33.000000 service_oriented-0.0.3/service_oriented/deployment_environment.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 21:52:17.671363 service_oriented-0.0.3/service_oriented/logging/
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-06 21:51:33.000000 service_oriented-0.0.3/service_oriented/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-06 21:51:33.000000 service_oriented-0.0.3/service_oriented/logging/normalized_json_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 21:51:33.000000 service_oriented-0.0.3/service_oriented/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 21:52:17.671363 service_oriented-0.0.3/service_oriented/services/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 21:51:33.000000 service_oriented-0.0.3/service_oriented/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 21:52:17.671363 service_oriented-0.0.3/service_oriented/services/logger_service/
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-06 21:51:33.000000 service_oriented-0.0.3/service_oriented/services/logger_service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-06 21:51:33.000000 service_oriented-0.0.3/service_oriented/services/logger_service/logger_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-06 21:51:33.000000 service_oriented-0.0.3/service_oriented/services/logger_service/logger_service_with_yaml_logging_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 21:52:17.675363 service_oriented-0.0.3/service_oriented.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2613 2024-04-06 21:52:17.000000 service_oriented-0.0.3/service_oriented.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2880 2024-04-06 21:52:17.000000 service_oriented-0.0.3/service_oriented.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 21:52:17.000000 service_oriented-0.0.3/service_oriented.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-06 21:52:17.000000 service_oriented-0.0.3/service_oriented.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-06 21:52:17.000000 service_oriented-0.0.3/service_oriented.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 21:52:17.671363 service_oriented-0.0.3/service_oriented_test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 21:51:33.000000 service_oriented-0.0.3/service_oriented_test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 21:52:17.671363 service_oriented-0.0.3/service_oriented_test/application/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 21:51:33.000000 service_oriented-0.0.3/service_oriented_test/application/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3282 2024-04-06 21:51:33.000000 service_oriented-0.0.3/service_oriented_test/application/base_application_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 21:52:17.671363 service_oriented-0.0.3/service_oriented_test/application/config/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 21:51:33.000000 service_oriented-0.0.3/service_oriented_test/application/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6191 2024-04-06 21:51:33.000000 service_oriented-0.0.3/service_oriented_test/application/config/base_config_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2968 2024-04-06 21:51:33.000000 service_oriented-0.0.3/service_oriented_test/application/config/yaml_config_settings_source_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-04-06 21:51:33.000000 service_oriented-0.0.3/service_oriented_test/application/entry_point_spec_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3368 2024-04-06 21:51:33.000000 service_oriented-0.0.3/service_oriented_test/application/generic_main_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 21:51:33.000000 service_oriented-0.0.3/service_oriented_test/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2738 2024-04-06 21:51:33.000000 service_oriented-0.0.3/service_oriented_test/deployment_environment_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 21:52:17.671363 service_oriented-0.0.3/service_oriented_test/example_application/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 21:51:33.000000 service_oriented-0.0.3/service_oriented_test/example_application/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 21:52:17.671363 service_oriented-0.0.3/service_oriented_test/example_application/app/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 21:51:33.000000 service_oriented-0.0.3/service_oriented_test/example_application/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-06 21:51:33.000000 service_oriented-0.0.3/service_oriented_test/example_application/app/application.py
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-06 21:51:33.000000 service_oriented-0.0.3/service_oriented_test/example_application/app/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 21:52:17.675363 service_oriented-0.0.3/service_oriented_test/example_application/app/entry_points/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 21:51:33.000000 service_oriented-0.0.3/service_oriented_test/example_application/app/entry_points/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-04-06 21:51:33.000000 service_oriented-0.0.3/service_oriented_test/example_application/app/entry_points/printer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-06 21:51:33.000000 service_oriented-0.0.3/service_oriented_test/example_application/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 21:52:17.675363 service_oriented-0.0.3/service_oriented_test/example_application_test/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 21:52:17.675363 service_oriented-0.0.3/service_oriented_test/example_application_test/app/
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-06 21:51:33.000000 service_oriented-0.0.3/service_oriented_test/example_application_test/app/application_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4647 2024-04-06 21:51:33.000000 service_oriented-0.0.3/service_oriented_test/example_application_test/app/config_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 21:52:17.675363 service_oriented-0.0.3/service_oriented_test/example_application_test/app/entry_points/
+-rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-04-06 21:51:33.000000 service_oriented-0.0.3/service_oriented_test/example_application_test/app/entry_points/printer_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-06 21:51:33.000000 service_oriented-0.0.3/service_oriented_test/example_application_test/factories.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 21:52:17.675363 service_oriented-0.0.3/service_oriented_test/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-06 21:51:33.000000 service_oriented-0.0.3/service_oriented_test/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-06 21:51:33.000000 service_oriented-0.0.3/service_oriented_test/fixtures/logging_config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 21:52:17.675363 service_oriented-0.0.3/service_oriented_test/logging/
+-rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-04-06 21:51:33.000000 service_oriented-0.0.3/service_oriented_test/logging/normalized_json_formatter_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 21:51:33.000000 service_oriented-0.0.3/service_oriented_test/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 21:52:17.663363 service_oriented-0.0.3/service_oriented_test/services/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 21:52:17.675363 service_oriented-0.0.3/service_oriented_test/services/logger_service/
+-rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-04-06 21:51:33.000000 service_oriented-0.0.3/service_oriented_test/services/logger_service/logger_service_with_yaml_logging_config_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 21:52:17.679363 service_oriented-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-06 21:51:33.000000 service_oriented-0.0.3/whitelist.txt
```

### Comparing `service_oriented-0.0.2a9/LICENSE` & `service_oriented-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `service_oriented-0.0.2a9/PKG-INFO` & `service_oriented-0.0.3/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,70 +1,56 @@
 Metadata-Version: 2.1
 Name: service_oriented
-Version: 0.0.2a9
+Version: 0.0.3
 Summary: Toolkit for building service oriented applications in python
-Home-page: https://github.com/tdg5/service-oriented-py
 Author: Danny Guinther
-Author-email: dannyguinther@gmail.com
 License: MIT
-Keywords: [TODO]
+Project-URL: Homepage, https://github.com/tdg5/service-oriented-py
+Project-URL: Source, https://github.com/tdg5/service-oriented-py
+Project-URL: Tracker, https://github.com/tdg5/service-oriented-py/issues
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Python: >=3.9.0
+Classifier: Programming Language :: Python :: 3.9
+Requires-Python: >3.9.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: PyYaml~=6.0.1
-Requires-Dist: pydantic~=2.5.3
 Requires-Dist: pydantic-settings~=2.1.0
-Provides-Extra: all
-Requires-Dist: PyYaml~=6.0.1; extra == "all"
-Requires-Dist: pydantic~=2.5.3; extra == "all"
-Requires-Dist: pydantic-settings~=2.1.0; extra == "all"
-Requires-Dist: black~=23.12.1; extra == "all"
-Requires-Dist: build==1.0.3; extra == "all"
-Requires-Dist: dlint==0.14.1; extra == "all"
-Requires-Dist: flake8-comprehensions==3.14.0; extra == "all"
-Requires-Dist: flake8-eradicate==1.5.0; extra == "all"
-Requires-Dist: flake8-spellcheck==0.28.0; extra == "all"
-Requires-Dist: flake8-typing-imports==1.15.0; extra == "all"
-Requires-Dist: flake8==7.0.0; extra == "all"
-Requires-Dist: isort==5.13.2; extra == "all"
-Requires-Dist: mypy~=1.8.0; extra == "all"
-Requires-Dist: pep8-naming==0.13.3; extra == "all"
-Requires-Dist: pre-commit==3.6.0; extra == "all"
-Requires-Dist: pytest-watch~=4.2.0; extra == "all"
-Requires-Dist: pytest~=7.4.0; extra == "all"
-Requires-Dist: safety==2.3.4; extra == "all"
-Requires-Dist: twine==4.0.2; extra == "all"
-Requires-Dist: wheel>=0.42.0; extra == "all"
-Provides-Extra: deps
-Requires-Dist: PyYaml~=6.0.1; extra == "deps"
-Requires-Dist: pydantic~=2.5.3; extra == "deps"
-Requires-Dist: pydantic-settings~=2.1.0; extra == "deps"
+Requires-Dist: pydantic~=2.5.3
+Requires-Dist: python-json-logger==2.0.7
+Requires-Dist: pyyaml~=6.0.1
 Provides-Extra: dev
-Requires-Dist: black~=23.12.1; extra == "dev"
-Requires-Dist: build==1.0.3; extra == "dev"
-Requires-Dist: dlint==0.14.1; extra == "dev"
-Requires-Dist: flake8-comprehensions==3.14.0; extra == "dev"
-Requires-Dist: flake8-eradicate==1.5.0; extra == "dev"
-Requires-Dist: flake8-spellcheck==0.28.0; extra == "dev"
-Requires-Dist: flake8-typing-imports==1.15.0; extra == "dev"
-Requires-Dist: flake8==7.0.0; extra == "dev"
-Requires-Dist: isort==5.13.2; extra == "dev"
+Requires-Dist: black~=24.2.0; extra == "dev"
+Requires-Dist: build~=1.0.3; extra == "dev"
+Requires-Dist: coverage-badge~=1.1.0; extra == "dev"
+Requires-Dist: coverage~=7.4.4; extra == "dev"
+Requires-Dist: dlint~=0.14.1; extra == "dev"
+Requires-Dist: flake8-comprehensions~=3.14.0; extra == "dev"
+Requires-Dist: flake8-eradicate~=1.5.0; extra == "dev"
+Requires-Dist: flake8-pyproject~=1.2.3; extra == "dev"
+Requires-Dist: flake8-spellcheck~=0.28.0; extra == "dev"
+Requires-Dist: flake8-typing-imports~=1.15.0; extra == "dev"
+Requires-Dist: flake8~=7.0.0; extra == "dev"
+Requires-Dist: isort~=5.13.2; extra == "dev"
 Requires-Dist: mypy~=1.8.0; extra == "dev"
-Requires-Dist: pep8-naming==0.13.3; extra == "dev"
-Requires-Dist: pre-commit==3.6.0; extra == "dev"
-Requires-Dist: pytest-watch~=4.2.0; extra == "dev"
+Requires-Dist: pep8-naming~=0.13.3; extra == "dev"
+Requires-Dist: pre-commit~=3.6.0; extra == "dev"
+Requires-Dist: pytest-mock~=3.12.0; extra == "dev"
+Requires-Dist: pytest-watcher~=0.4.2; extra == "dev"
 Requires-Dist: pytest~=7.4.0; extra == "dev"
-Requires-Dist: safety==2.3.4; extra == "dev"
-Requires-Dist: twine==4.0.2; extra == "dev"
+Requires-Dist: rodi~=2.0.6; extra == "dev"
+Requires-Dist: safety~=2.3.4; extra == "dev"
+Requires-Dist: twine~=4.0.2; extra == "dev"
 Requires-Dist: wheel>=0.42.0; extra == "dev"
+Provides-Extra: all
+Requires-Dist: service-oriented[dev]; extra == "all"
+
+[![code coverage](https://github.com/tdg5/service-oriented-py/raw/main/.meta/coverage/badge.svg)](https://raw.githubusercontent.com/tdg5/service-oriented-py/main/.meta/coverage/report.txt)
+[![license](https://img.shields.io/github/license/tdg5/service-oriented-py.svg)](https://github.com/tdg5/service-oriented-py/blob/main/LICENSE)
 
 # service-oriented-py
 
 `service-oriented-py` is a toolkit for building service oriented applications in python.
```

### Comparing `service_oriented-0.0.2a9/service_oriented/application/base_application.py` & `service_oriented-0.0.3/service_oriented/application/base_application.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,24 +11,24 @@
     default_entry_points: Dict[str, EntryPointSpec] = {}
 
     @classmethod
     def __init_subclass__(
         cls,
         entry_points: Optional[Dict[str, EntryPointSpec]] = None,
         **kwargs: Any,
-    ):
+    ) -> None:
         super().__init_subclass__(**kwargs)
         _entry_points = entry_points or {}
         cls.default_entry_points = _entry_points
 
     def __init__(
         self,
         config: C,
         entry_points: Optional[Dict[str, EntryPointSpec]] = None,
-    ):
+    ) -> None:
         self.config: C = config
         _entry_points = entry_points or {}
         self.entry_points = {**self.default_entry_points, **_entry_points}
 
     def run(self) -> None:
         entry_point_name = self.config.entry_point
         entry_point_spec = self.entry_points.get(entry_point_name)
```

### Comparing `service_oriented-0.0.2a9/service_oriented/application/config/base_config.py` & `service_oriented-0.0.3/service_oriented/application/config/base_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     deployment_environment: Annotated[
         DeploymentEnvironment,
         BeforeValidator(handle_alternative_deployment_environment_formats),
     ]
     entry_point: str
     yaml_config_path: Optional[str] = None
 
-    def __init__(self, *args: Any, **kwargs: Any):
+    def __init__(self, *args: Any, **kwargs: Any) -> None:
         if not self.model_config.get("env_nested_delimiter"):
             raise RuntimeError("env_nested_delimiter model config is required")
 
         if not self.model_config.get("env_prefix"):
             raise RuntimeError("env_prefix model config is required")
 
         super().__init__(*args, **kwargs)
```

### Comparing `service_oriented-0.0.2a9/service_oriented/application/config/yaml_config_settings_source.py` & `service_oriented-0.0.3/service_oriented/application/config/yaml_config_settings_source.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
             yaml_config_path=yaml_config_path,
         )
 
     def __init__(
         self,
         settings_cls: Type[BaseSettings],
         yaml_config_path: Optional[str] = None,
-    ):
+    ) -> None:
         super().__init__(settings_cls)
 
         self._yaml_config: Dict[str, Any] = self._load_yaml_config(yaml_config_path)
 
     def _load_yaml_config(self, yaml_config_path: Optional[str]) -> Dict[str, Any]:
         if not yaml_config_path or not os.path.exists(yaml_config_path):
             return {}
```

### Comparing `service_oriented-0.0.2a9/service_oriented/application/entry_point_spec.py` & `service_oriented-0.0.3/service_oriented/application/entry_point_spec.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,18 +12,18 @@
 
 P = ParamSpec("P")
 C = TypeVar("C", bound=BaseConfig)
 
 
 class _EntryPointClass(Protocol[P]):
     def __init__(self, config: C, *args: P.args, **kwargs: P.kwargs) -> None:
-        ...  # pragma: no cover
+        pass  # pragma: no cover
 
     def run(self) -> None:
-        ...  # pragma: no cover
+        pass  # pragma: no cover
 
 
 class EntryPointSpec:
     def __init__(
         self,
         cls: Type[_EntryPointClass[P]],
         *args: P.args,
```

### Comparing `service_oriented-0.0.2a9/service_oriented/deployment_environment.py` & `service_oriented-0.0.3/service_oriented/deployment_environment.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 class DeploymentEnvironment:
     def __init__(
         self,
         identifier: str,
         region: str,
         stage: str,
         vendor: str,
-    ):
+    ) -> None:
         self.identifier: str = identifier
         self.region: str = region
         self.stage: str = stage
         self.vendor: str = vendor
         self.stub: str = f"{self.stage}:{self.vendor}:{self.region}:{self.identifier}"
 
     @classmethod
```

### Comparing `service_oriented-0.0.2a9/service_oriented.egg-info/PKG-INFO` & `service_oriented-0.0.3/service_oriented.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,70 +1,56 @@
 Metadata-Version: 2.1
 Name: service_oriented
-Version: 0.0.2a9
+Version: 0.0.3
 Summary: Toolkit for building service oriented applications in python
-Home-page: https://github.com/tdg5/service-oriented-py
 Author: Danny Guinther
-Author-email: dannyguinther@gmail.com
 License: MIT
-Keywords: [TODO]
+Project-URL: Homepage, https://github.com/tdg5/service-oriented-py
+Project-URL: Source, https://github.com/tdg5/service-oriented-py
+Project-URL: Tracker, https://github.com/tdg5/service-oriented-py/issues
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Python: >=3.9.0
+Classifier: Programming Language :: Python :: 3.9
+Requires-Python: >3.9.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: PyYaml~=6.0.1
-Requires-Dist: pydantic~=2.5.3
 Requires-Dist: pydantic-settings~=2.1.0
-Provides-Extra: all
-Requires-Dist: PyYaml~=6.0.1; extra == "all"
-Requires-Dist: pydantic~=2.5.3; extra == "all"
-Requires-Dist: pydantic-settings~=2.1.0; extra == "all"
-Requires-Dist: black~=23.12.1; extra == "all"
-Requires-Dist: build==1.0.3; extra == "all"
-Requires-Dist: dlint==0.14.1; extra == "all"
-Requires-Dist: flake8-comprehensions==3.14.0; extra == "all"
-Requires-Dist: flake8-eradicate==1.5.0; extra == "all"
-Requires-Dist: flake8-spellcheck==0.28.0; extra == "all"
-Requires-Dist: flake8-typing-imports==1.15.0; extra == "all"
-Requires-Dist: flake8==7.0.0; extra == "all"
-Requires-Dist: isort==5.13.2; extra == "all"
-Requires-Dist: mypy~=1.8.0; extra == "all"
-Requires-Dist: pep8-naming==0.13.3; extra == "all"
-Requires-Dist: pre-commit==3.6.0; extra == "all"
-Requires-Dist: pytest-watch~=4.2.0; extra == "all"
-Requires-Dist: pytest~=7.4.0; extra == "all"
-Requires-Dist: safety==2.3.4; extra == "all"
-Requires-Dist: twine==4.0.2; extra == "all"
-Requires-Dist: wheel>=0.42.0; extra == "all"
-Provides-Extra: deps
-Requires-Dist: PyYaml~=6.0.1; extra == "deps"
-Requires-Dist: pydantic~=2.5.3; extra == "deps"
-Requires-Dist: pydantic-settings~=2.1.0; extra == "deps"
+Requires-Dist: pydantic~=2.5.3
+Requires-Dist: python-json-logger==2.0.7
+Requires-Dist: pyyaml~=6.0.1
 Provides-Extra: dev
-Requires-Dist: black~=23.12.1; extra == "dev"
-Requires-Dist: build==1.0.3; extra == "dev"
-Requires-Dist: dlint==0.14.1; extra == "dev"
-Requires-Dist: flake8-comprehensions==3.14.0; extra == "dev"
-Requires-Dist: flake8-eradicate==1.5.0; extra == "dev"
-Requires-Dist: flake8-spellcheck==0.28.0; extra == "dev"
-Requires-Dist: flake8-typing-imports==1.15.0; extra == "dev"
-Requires-Dist: flake8==7.0.0; extra == "dev"
-Requires-Dist: isort==5.13.2; extra == "dev"
+Requires-Dist: black~=24.2.0; extra == "dev"
+Requires-Dist: build~=1.0.3; extra == "dev"
+Requires-Dist: coverage-badge~=1.1.0; extra == "dev"
+Requires-Dist: coverage~=7.4.4; extra == "dev"
+Requires-Dist: dlint~=0.14.1; extra == "dev"
+Requires-Dist: flake8-comprehensions~=3.14.0; extra == "dev"
+Requires-Dist: flake8-eradicate~=1.5.0; extra == "dev"
+Requires-Dist: flake8-pyproject~=1.2.3; extra == "dev"
+Requires-Dist: flake8-spellcheck~=0.28.0; extra == "dev"
+Requires-Dist: flake8-typing-imports~=1.15.0; extra == "dev"
+Requires-Dist: flake8~=7.0.0; extra == "dev"
+Requires-Dist: isort~=5.13.2; extra == "dev"
 Requires-Dist: mypy~=1.8.0; extra == "dev"
-Requires-Dist: pep8-naming==0.13.3; extra == "dev"
-Requires-Dist: pre-commit==3.6.0; extra == "dev"
-Requires-Dist: pytest-watch~=4.2.0; extra == "dev"
+Requires-Dist: pep8-naming~=0.13.3; extra == "dev"
+Requires-Dist: pre-commit~=3.6.0; extra == "dev"
+Requires-Dist: pytest-mock~=3.12.0; extra == "dev"
+Requires-Dist: pytest-watcher~=0.4.2; extra == "dev"
 Requires-Dist: pytest~=7.4.0; extra == "dev"
-Requires-Dist: safety==2.3.4; extra == "dev"
-Requires-Dist: twine==4.0.2; extra == "dev"
+Requires-Dist: rodi~=2.0.6; extra == "dev"
+Requires-Dist: safety~=2.3.4; extra == "dev"
+Requires-Dist: twine~=4.0.2; extra == "dev"
 Requires-Dist: wheel>=0.42.0; extra == "dev"
+Provides-Extra: all
+Requires-Dist: service-oriented[dev]; extra == "all"
+
+[![code coverage](https://github.com/tdg5/service-oriented-py/raw/main/.meta/coverage/badge.svg)](https://raw.githubusercontent.com/tdg5/service-oriented-py/main/.meta/coverage/report.txt)
+[![license](https://img.shields.io/github/license/tdg5/service-oriented-py.svg)](https://github.com/tdg5/service-oriented-py/blob/main/LICENSE)
 
 # service-oriented-py
 
 `service-oriented-py` is a toolkit for building service oriented applications in python.
```

### Comparing `service_oriented-0.0.2a9/service_oriented.egg-info/requires.txt` & `service_oriented-0.0.3/service_oriented.egg-info/requires.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,49 +1,31 @@
-PyYaml~=6.0.1
-pydantic~=2.5.3
 pydantic-settings~=2.1.0
-
-[all]
-PyYaml~=6.0.1
 pydantic~=2.5.3
-pydantic-settings~=2.1.0
-black~=23.12.1
-build==1.0.3
-dlint==0.14.1
-flake8-comprehensions==3.14.0
-flake8-eradicate==1.5.0
-flake8-spellcheck==0.28.0
-flake8-typing-imports==1.15.0
-flake8==7.0.0
-isort==5.13.2
-mypy~=1.8.0
-pep8-naming==0.13.3
-pre-commit==3.6.0
-pytest-watch~=4.2.0
-pytest~=7.4.0
-safety==2.3.4
-twine==4.0.2
-wheel>=0.42.0
+python-json-logger==2.0.7
+pyyaml~=6.0.1
 
-[deps]
-PyYaml~=6.0.1
-pydantic~=2.5.3
-pydantic-settings~=2.1.0
+[all]
+service-oriented[dev]
 
 [dev]
-black~=23.12.1
-build==1.0.3
-dlint==0.14.1
-flake8-comprehensions==3.14.0
-flake8-eradicate==1.5.0
-flake8-spellcheck==0.28.0
-flake8-typing-imports==1.15.0
-flake8==7.0.0
-isort==5.13.2
+black~=24.2.0
+build~=1.0.3
+coverage-badge~=1.1.0
+coverage~=7.4.4
+dlint~=0.14.1
+flake8-comprehensions~=3.14.0
+flake8-eradicate~=1.5.0
+flake8-pyproject~=1.2.3
+flake8-spellcheck~=0.28.0
+flake8-typing-imports~=1.15.0
+flake8~=7.0.0
+isort~=5.13.2
 mypy~=1.8.0
-pep8-naming==0.13.3
-pre-commit==3.6.0
-pytest-watch~=4.2.0
+pep8-naming~=0.13.3
+pre-commit~=3.6.0
+pytest-mock~=3.12.0
+pytest-watcher~=0.4.2
 pytest~=7.4.0
-safety==2.3.4
-twine==4.0.2
+rodi~=2.0.6
+safety~=2.3.4
+twine~=4.0.2
 wheel>=0.42.0
```

