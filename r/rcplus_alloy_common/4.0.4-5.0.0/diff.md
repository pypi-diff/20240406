# Comparing `tmp/rcplus_alloy_common-4.0.4.tar.gz` & `tmp/rcplus_alloy_common-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rcplus_alloy_common-4.0.4.tar", max compression
+gzip compressed data, was "rcplus_alloy_common-5.0.0.tar", max compression
```

## Comparing `rcplus_alloy_common-4.0.4.tar` & `rcplus_alloy_common-5.0.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0       77 2024-04-03 12:33:51.460947 rcplus_alloy_common-4.0.4/LICENSE
--rw-r--r--   0        0        0      571 2024-04-03 12:33:51.460947 rcplus_alloy_common-4.0.4/README.md
--rw-r--r--   0        0        0     3017 2024-04-03 12:33:51.464948 rcplus_alloy_common-4.0.4/pyproject.toml
--rw-r--r--   0        0        0     2668 2024-04-03 12:33:51.464948 rcplus_alloy_common-4.0.4/src/rcplus_alloy_common/__init__.py
--rw-r--r--   0        0        0     1072 2024-04-03 12:33:51.464948 rcplus_alloy_common-4.0.4/src/rcplus_alloy_common/airflow/__init__.py
--rw-r--r--   0        0        0     4256 2024-04-03 12:33:51.464948 rcplus_alloy_common-4.0.4/src/rcplus_alloy_common/airflow/dag.py
--rw-r--r--   0        0        0     2998 2024-04-03 12:33:51.464948 rcplus_alloy_common-4.0.4/src/rcplus_alloy_common/airflow/decorators.py
--rw-r--r--   0        0        0      703 2024-04-03 12:33:51.464948 rcplus_alloy_common-4.0.4/src/rcplus_alloy_common/airflow/hooks.py
--rw-r--r--   0        0        0     8258 2024-04-03 12:33:51.464948 rcplus_alloy_common-4.0.4/src/rcplus_alloy_common/airflow/locking.py
--rw-r--r--   0        0        0    11749 2024-04-03 12:33:51.464948 rcplus_alloy_common-4.0.4/src/rcplus_alloy_common/airflow/observability.py
--rw-r--r--   0        0        0    26534 2024-04-03 12:33:51.464948 rcplus_alloy_common-4.0.4/src/rcplus_alloy_common/airflow/operators.py
--rw-r--r--   0        0        0        0 2024-04-03 12:33:51.464948 rcplus_alloy_common-4.0.4/src/rcplus_alloy_common/airflow/py.typed
--rw-r--r--   0        0        0     2186 2024-04-03 12:33:51.464948 rcplus_alloy_common-4.0.4/src/rcplus_alloy_common/airflow/sensors.py
--rw-r--r--   0        0        0     5997 2024-04-03 12:33:51.464948 rcplus_alloy_common-4.0.4/src/rcplus_alloy_common/airflow/utils.py
--rw-r--r--   0        0        0       98 2024-04-03 12:33:51.464948 rcplus_alloy_common-4.0.4/src/rcplus_alloy_common/aws/__init__.py
--rw-r--r--   0        0        0     4051 2024-04-03 12:33:51.464948 rcplus_alloy_common-4.0.4/src/rcplus_alloy_common/aws/dynamodb.py
--rw-r--r--   0        0        0     2720 2024-04-03 12:33:51.464948 rcplus_alloy_common-4.0.4/src/rcplus_alloy_common/aws/utils.py
--rw-r--r--   0        0        0    12430 2024-04-03 12:33:51.464948 rcplus_alloy_common-4.0.4/src/rcplus_alloy_common/aws/wr.py
--rw-r--r--   0        0        0     2750 2024-04-03 12:33:51.464948 rcplus_alloy_common-4.0.4/src/rcplus_alloy_common/aws/wr_utils.py
--rw-r--r--   0        0        0     2475 2024-04-03 12:33:51.464948 rcplus_alloy_common-4.0.4/src/rcplus_alloy_common/constants.py
--rw-r--r--   0        0        0      710 2024-04-03 12:33:51.464948 rcplus_alloy_common-4.0.4/src/rcplus_alloy_common/encoder.py
--rw-r--r--   0        0        0      616 2024-04-03 12:33:51.464948 rcplus_alloy_common-4.0.4/src/rcplus_alloy_common/exceptions.py
--rw-r--r--   0        0        0        0 2024-04-03 12:33:51.464948 rcplus_alloy_common-4.0.4/src/rcplus_alloy_common/gam/__init__.py
--rw-r--r--   0        0        0     7223 2024-04-03 12:33:51.464948 rcplus_alloy_common-4.0.4/src/rcplus_alloy_common/gam/audience.py
--rw-r--r--   0        0        0       80 2024-04-03 12:33:51.464948 rcplus_alloy_common-4.0.4/src/rcplus_alloy_common/gam/constants.py
--rw-r--r--   0        0        0    10291 2024-04-03 12:33:51.464948 rcplus_alloy_common-4.0.4/src/rcplus_alloy_common/gam/keyvalues.py
--rw-r--r--   0        0        0        0 2024-04-03 12:33:51.464948 rcplus_alloy_common-4.0.4/src/rcplus_alloy_common/gam/mock/__init__.py
--rw-r--r--   0        0        0    18267 2024-04-03 12:33:51.464948 rcplus_alloy_common-4.0.4/src/rcplus_alloy_common/gam/mock/services.py
--rw-r--r--   0        0        0     2170 2024-04-03 12:33:51.464948 rcplus_alloy_common-4.0.4/src/rcplus_alloy_common/gam/network.py
--rw-r--r--   0        0        0        0 2024-04-03 12:33:51.464948 rcplus_alloy_common-4.0.4/src/rcplus_alloy_common/gam/py.typed
--rw-r--r--   0        0        0      494 2024-04-03 12:33:51.464948 rcplus_alloy_common-4.0.4/src/rcplus_alloy_common/gam/utils.py
--rw-r--r--   0        0        0     8397 2024-04-03 12:33:51.464948 rcplus_alloy_common-4.0.4/src/rcplus_alloy_common/logging.py
--rw-r--r--   0        0        0     6968 2024-04-03 12:33:51.464948 rcplus_alloy_common-4.0.4/src/rcplus_alloy_common/metrics.py
--rw-r--r--   0        0        0     1250 2024-04-03 12:33:51.464948 rcplus_alloy_common-4.0.4/src/rcplus_alloy_common/multitenancy.py
--rw-r--r--   0        0        0        0 2024-04-03 12:33:51.464948 rcplus_alloy_common-4.0.4/src/rcplus_alloy_common/py.typed
--rw-r--r--   0        0        0     3925 2024-04-03 12:33:51.464948 rcplus_alloy_common-4.0.4/src/rcplus_alloy_common/retry.py
--rw-r--r--   0        0        0       19 2024-04-03 12:33:51.464948 rcplus_alloy_common-4.0.4/src/rcplus_alloy_common/version.py
--rw-r--r--   0        0        0     2181 1970-01-01 00:00:00.000000 rcplus_alloy_common-4.0.4/PKG-INFO
+-rw-r--r--   0        0        0       77 2024-04-06 08:04:03.808445 rcplus_alloy_common-5.0.0/LICENSE
+-rw-r--r--   0        0        0      571 2024-04-06 08:04:03.808445 rcplus_alloy_common-5.0.0/README.md
+-rw-r--r--   0        0        0     3013 2024-04-06 08:04:03.808445 rcplus_alloy_common-5.0.0/pyproject.toml
+-rw-r--r--   0        0        0     2668 2024-04-06 08:04:03.808445 rcplus_alloy_common-5.0.0/src/rcplus_alloy_common/__init__.py
+-rw-r--r--   0        0        0     1072 2024-04-06 08:04:03.808445 rcplus_alloy_common-5.0.0/src/rcplus_alloy_common/airflow/__init__.py
+-rw-r--r--   0        0        0     4256 2024-04-06 08:04:03.808445 rcplus_alloy_common-5.0.0/src/rcplus_alloy_common/airflow/dag.py
+-rw-r--r--   0        0        0     2998 2024-04-06 08:04:03.808445 rcplus_alloy_common-5.0.0/src/rcplus_alloy_common/airflow/decorators.py
+-rw-r--r--   0        0        0      703 2024-04-06 08:04:03.808445 rcplus_alloy_common-5.0.0/src/rcplus_alloy_common/airflow/hooks.py
+-rw-r--r--   0        0        0     8258 2024-04-06 08:04:03.808445 rcplus_alloy_common-5.0.0/src/rcplus_alloy_common/airflow/locking.py
+-rw-r--r--   0        0        0    11749 2024-04-06 08:04:03.808445 rcplus_alloy_common-5.0.0/src/rcplus_alloy_common/airflow/observability.py
+-rw-r--r--   0        0        0    26534 2024-04-06 08:04:03.812445 rcplus_alloy_common-5.0.0/src/rcplus_alloy_common/airflow/operators.py
+-rw-r--r--   0        0        0        0 2024-04-06 08:04:03.812445 rcplus_alloy_common-5.0.0/src/rcplus_alloy_common/airflow/py.typed
+-rw-r--r--   0        0        0     2186 2024-04-06 08:04:03.812445 rcplus_alloy_common-5.0.0/src/rcplus_alloy_common/airflow/sensors.py
+-rw-r--r--   0        0        0     5997 2024-04-06 08:04:03.812445 rcplus_alloy_common-5.0.0/src/rcplus_alloy_common/airflow/utils.py
+-rw-r--r--   0        0        0       98 2024-04-06 08:04:03.812445 rcplus_alloy_common-5.0.0/src/rcplus_alloy_common/aws/__init__.py
+-rw-r--r--   0        0        0     4051 2024-04-06 08:04:03.812445 rcplus_alloy_common-5.0.0/src/rcplus_alloy_common/aws/dynamodb.py
+-rw-r--r--   0        0        0     2720 2024-04-06 08:04:03.812445 rcplus_alloy_common-5.0.0/src/rcplus_alloy_common/aws/utils.py
+-rw-r--r--   0        0        0    12430 2024-04-06 08:04:03.812445 rcplus_alloy_common-5.0.0/src/rcplus_alloy_common/aws/wr.py
+-rw-r--r--   0        0        0     2750 2024-04-06 08:04:03.812445 rcplus_alloy_common-5.0.0/src/rcplus_alloy_common/aws/wr_utils.py
+-rw-r--r--   0        0        0     2475 2024-04-06 08:04:03.812445 rcplus_alloy_common-5.0.0/src/rcplus_alloy_common/constants.py
+-rw-r--r--   0        0        0      710 2024-04-06 08:04:03.812445 rcplus_alloy_common-5.0.0/src/rcplus_alloy_common/encoder.py
+-rw-r--r--   0        0        0      616 2024-04-06 08:04:03.812445 rcplus_alloy_common-5.0.0/src/rcplus_alloy_common/exceptions.py
+-rw-r--r--   0        0        0        0 2024-04-06 08:04:03.812445 rcplus_alloy_common-5.0.0/src/rcplus_alloy_common/gam/__init__.py
+-rw-r--r--   0        0        0     7223 2024-04-06 08:04:03.812445 rcplus_alloy_common-5.0.0/src/rcplus_alloy_common/gam/audience.py
+-rw-r--r--   0        0        0       80 2024-04-06 08:04:03.812445 rcplus_alloy_common-5.0.0/src/rcplus_alloy_common/gam/constants.py
+-rw-r--r--   0        0        0    10291 2024-04-06 08:04:03.812445 rcplus_alloy_common-5.0.0/src/rcplus_alloy_common/gam/keyvalues.py
+-rw-r--r--   0        0        0        0 2024-04-06 08:04:03.812445 rcplus_alloy_common-5.0.0/src/rcplus_alloy_common/gam/mock/__init__.py
+-rw-r--r--   0        0        0    18267 2024-04-06 08:04:03.812445 rcplus_alloy_common-5.0.0/src/rcplus_alloy_common/gam/mock/services.py
+-rw-r--r--   0        0        0     2170 2024-04-06 08:04:03.812445 rcplus_alloy_common-5.0.0/src/rcplus_alloy_common/gam/network.py
+-rw-r--r--   0        0        0        0 2024-04-06 08:04:03.812445 rcplus_alloy_common-5.0.0/src/rcplus_alloy_common/gam/py.typed
+-rw-r--r--   0        0        0      494 2024-04-06 08:04:03.812445 rcplus_alloy_common-5.0.0/src/rcplus_alloy_common/gam/utils.py
+-rw-r--r--   0        0        0     8397 2024-04-06 08:04:03.812445 rcplus_alloy_common-5.0.0/src/rcplus_alloy_common/logging.py
+-rw-r--r--   0        0        0     6968 2024-04-06 08:04:03.812445 rcplus_alloy_common-5.0.0/src/rcplus_alloy_common/metrics.py
+-rw-r--r--   0        0        0     1250 2024-04-06 08:04:03.812445 rcplus_alloy_common-5.0.0/src/rcplus_alloy_common/multitenancy.py
+-rw-r--r--   0        0        0        0 2024-04-06 08:04:03.812445 rcplus_alloy_common-5.0.0/src/rcplus_alloy_common/py.typed
+-rw-r--r--   0        0        0     3925 2024-04-06 08:04:03.812445 rcplus_alloy_common-5.0.0/src/rcplus_alloy_common/retry.py
+-rw-r--r--   0        0        0       19 2024-04-06 08:04:03.812445 rcplus_alloy_common-5.0.0/src/rcplus_alloy_common/version.py
+-rw-r--r--   0        0        0     2173 1970-01-01 00:00:00.000000 rcplus_alloy_common-5.0.0/PKG-INFO
```

### Comparing `rcplus_alloy_common-4.0.4/README.md` & `rcplus_alloy_common-5.0.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # rcplus-alloy-lib-py-common
 
 ![PyPI](https://img.shields.io/pypi/v/rcplus-alloy-common)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/rcplus-alloy-common)
 ![Coverage badge](./coverage.svg)
 
-Current version: **v4.0.4**
+Current version: **v5.0.0**
 
 ---
 
 Python utilities for RC+/Alloy.
 
 _**NOTE**_: This Python package is published to PyPI.org as publicly available package.
```

### Comparing `rcplus_alloy_common-4.0.4/pyproject.toml` & `rcplus_alloy_common-5.0.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -15,22 +15,22 @@
 max-args = 11
 
 [tool.ruff.flake8-quotes]
 docstring-quotes = "double"
 
 [tool.poetry]
 name = "rcplus_alloy_common"
-version = "4.0.4"
+version = "5.0.0"
 description = "RC+/Alloy helpers functions for Python"
 readme = "README.md"
 authors = [
     "Ringier AG <info@rcplus.io>",
 ]
 license = "Proprietary"
-repository = "https://github.com/ringier-data/rcplus-alloy-lib-py-common"
+repository = "https://github.com/alloy-ch/rcplus-alloy-lib-py-common"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Natural Language :: English",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Software Development :: Libraries :: Python Modules",
```

### Comparing `rcplus_alloy_common-4.0.4/src/rcplus_alloy_common/__init__.py` & `rcplus_alloy_common-5.0.0/src/rcplus_alloy_common/__init__.py`

 * *Files identical despite different names*

### Comparing `rcplus_alloy_common-4.0.4/src/rcplus_alloy_common/airflow/__init__.py` & `rcplus_alloy_common-5.0.0/src/rcplus_alloy_common/airflow/__init__.py`

 * *Files identical despite different names*

### Comparing `rcplus_alloy_common-4.0.4/src/rcplus_alloy_common/airflow/dag.py` & `rcplus_alloy_common-5.0.0/src/rcplus_alloy_common/airflow/dag.py`

 * *Files identical despite different names*

### Comparing `rcplus_alloy_common-4.0.4/src/rcplus_alloy_common/airflow/decorators.py` & `rcplus_alloy_common-5.0.0/src/rcplus_alloy_common/airflow/decorators.py`

 * *Files identical despite different names*

### Comparing `rcplus_alloy_common-4.0.4/src/rcplus_alloy_common/airflow/hooks.py` & `rcplus_alloy_common-5.0.0/src/rcplus_alloy_common/airflow/hooks.py`

 * *Files identical despite different names*

### Comparing `rcplus_alloy_common-4.0.4/src/rcplus_alloy_common/airflow/locking.py` & `rcplus_alloy_common-5.0.0/src/rcplus_alloy_common/airflow/locking.py`

 * *Files identical despite different names*

### Comparing `rcplus_alloy_common-4.0.4/src/rcplus_alloy_common/airflow/observability.py` & `rcplus_alloy_common-5.0.0/src/rcplus_alloy_common/airflow/observability.py`

 * *Files identical despite different names*

### Comparing `rcplus_alloy_common-4.0.4/src/rcplus_alloy_common/airflow/operators.py` & `rcplus_alloy_common-5.0.0/src/rcplus_alloy_common/airflow/operators.py`

 * *Files identical despite different names*

### Comparing `rcplus_alloy_common-4.0.4/src/rcplus_alloy_common/airflow/sensors.py` & `rcplus_alloy_common-5.0.0/src/rcplus_alloy_common/airflow/sensors.py`

 * *Files identical despite different names*

### Comparing `rcplus_alloy_common-4.0.4/src/rcplus_alloy_common/airflow/utils.py` & `rcplus_alloy_common-5.0.0/src/rcplus_alloy_common/airflow/utils.py`

 * *Files identical despite different names*

### Comparing `rcplus_alloy_common-4.0.4/src/rcplus_alloy_common/aws/dynamodb.py` & `rcplus_alloy_common-5.0.0/src/rcplus_alloy_common/aws/dynamodb.py`

 * *Files identical despite different names*

### Comparing `rcplus_alloy_common-4.0.4/src/rcplus_alloy_common/aws/utils.py` & `rcplus_alloy_common-5.0.0/src/rcplus_alloy_common/aws/utils.py`

 * *Files identical despite different names*

### Comparing `rcplus_alloy_common-4.0.4/src/rcplus_alloy_common/aws/wr.py` & `rcplus_alloy_common-5.0.0/src/rcplus_alloy_common/aws/wr.py`

 * *Files identical despite different names*

### Comparing `rcplus_alloy_common-4.0.4/src/rcplus_alloy_common/aws/wr_utils.py` & `rcplus_alloy_common-5.0.0/src/rcplus_alloy_common/aws/wr_utils.py`

 * *Files identical despite different names*

### Comparing `rcplus_alloy_common-4.0.4/src/rcplus_alloy_common/constants.py` & `rcplus_alloy_common-5.0.0/src/rcplus_alloy_common/constants.py`

 * *Files identical despite different names*

### Comparing `rcplus_alloy_common-4.0.4/src/rcplus_alloy_common/encoder.py` & `rcplus_alloy_common-5.0.0/src/rcplus_alloy_common/encoder.py`

 * *Files identical despite different names*

### Comparing `rcplus_alloy_common-4.0.4/src/rcplus_alloy_common/exceptions.py` & `rcplus_alloy_common-5.0.0/src/rcplus_alloy_common/exceptions.py`

 * *Files identical despite different names*

### Comparing `rcplus_alloy_common-4.0.4/src/rcplus_alloy_common/gam/audience.py` & `rcplus_alloy_common-5.0.0/src/rcplus_alloy_common/gam/audience.py`

 * *Files identical despite different names*

### Comparing `rcplus_alloy_common-4.0.4/src/rcplus_alloy_common/gam/keyvalues.py` & `rcplus_alloy_common-5.0.0/src/rcplus_alloy_common/gam/keyvalues.py`

 * *Files identical despite different names*

### Comparing `rcplus_alloy_common-4.0.4/src/rcplus_alloy_common/gam/mock/services.py` & `rcplus_alloy_common-5.0.0/src/rcplus_alloy_common/gam/mock/services.py`

 * *Files identical despite different names*

### Comparing `rcplus_alloy_common-4.0.4/src/rcplus_alloy_common/gam/network.py` & `rcplus_alloy_common-5.0.0/src/rcplus_alloy_common/gam/network.py`

 * *Files identical despite different names*

### Comparing `rcplus_alloy_common-4.0.4/src/rcplus_alloy_common/logging.py` & `rcplus_alloy_common-5.0.0/src/rcplus_alloy_common/logging.py`

 * *Files identical despite different names*

### Comparing `rcplus_alloy_common-4.0.4/src/rcplus_alloy_common/metrics.py` & `rcplus_alloy_common-5.0.0/src/rcplus_alloy_common/metrics.py`

 * *Files identical despite different names*

### Comparing `rcplus_alloy_common-4.0.4/src/rcplus_alloy_common/multitenancy.py` & `rcplus_alloy_common-5.0.0/src/rcplus_alloy_common/multitenancy.py`

 * *Files identical despite different names*

### Comparing `rcplus_alloy_common-4.0.4/src/rcplus_alloy_common/retry.py` & `rcplus_alloy_common-5.0.0/src/rcplus_alloy_common/retry.py`

 * *Files identical despite different names*

### Comparing `rcplus_alloy_common-4.0.4/PKG-INFO` & `rcplus_alloy_common-5.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: rcplus_alloy_common
-Version: 4.0.4
+Version: 5.0.0
 Summary: RC+/Alloy helpers functions for Python
-Home-page: https://github.com/ringier-data/rcplus-alloy-lib-py-common
+Home-page: https://github.com/alloy-ch/rcplus-alloy-lib-py-common
 License: Proprietary
 Keywords: rcplus,alloy,logging,metrics,utilities
 Author: Ringier AG
 Author-email: info@rcplus.io
 Requires-Python: >=3.10,<4
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -28,24 +28,24 @@
 Requires-Dist: jsonschema (>=3.0.0)
 Requires-Dist: pandas (>=2.1,<3.0) ; extra == "aws"
 Requires-Dist: pydantic (>=1,<3)
 Requires-Dist: python-json-logger (>=2.0.4)
 Requires-Dist: pytz (>=2023.3,<2024.0) ; extra == "airflow"
 Requires-Dist: pyyaml (>=6.0,<7.0) ; extra == "airflow" or extra == "aws"
 Requires-Dist: requests (>=2.6.1)
-Project-URL: Repository, https://github.com/ringier-data/rcplus-alloy-lib-py-common
+Project-URL: Repository, https://github.com/alloy-ch/rcplus-alloy-lib-py-common
 Description-Content-Type: text/markdown
 
 # rcplus-alloy-lib-py-common
 
 ![PyPI](https://img.shields.io/pypi/v/rcplus-alloy-common)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/rcplus-alloy-common)
 ![Coverage badge](./coverage.svg)
 
-Current version: **v4.0.4**
+Current version: **v5.0.0**
 
 ---
 
 Python utilities for RC+/Alloy.
 
 _**NOTE**_: This Python package is published to PyPI.org as publicly available package.
```

