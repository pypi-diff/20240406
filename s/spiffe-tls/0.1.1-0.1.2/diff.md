# Comparing `tmp/spiffe_tls-0.1.1.tar.gz` & `tmp/spiffe_tls-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spiffe_tls-0.1.1.tar", max compression
+gzip compressed data, was "spiffe_tls-0.1.2.tar", max compression
```

## Comparing `spiffe_tls-0.1.1.tar` & `spiffe_tls-0.1.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    11357 2024-04-01 01:23:32.314701 spiffe_tls-0.1.1/LICENSE
--rw-r--r--   0        0        0     2429 2024-04-01 01:23:32.314701 spiffe_tls-0.1.1/README.md
--rw-r--r--   0        0        0      903 2024-04-01 01:23:32.314701 spiffe_tls-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      208 2024-04-01 01:23:32.314701 spiffe_tls-0.1.1/src/spiffetls/__init__.py
--rw-r--r--   0        0        0     5398 2024-04-01 01:23:32.314701 spiffe_tls-0.1.1/src/spiffetls/context.py
--rw-r--r--   0        0        0     3011 2024-04-01 01:23:32.314701 spiffe_tls-0.1.1/src/spiffetls/dial.py
--rw-r--r--   0        0        0     1816 2024-04-01 01:23:32.314701 spiffe_tls-0.1.1/src/spiffetls/errors.py
--rw-r--r--   0        0        0     4463 2024-04-01 01:23:32.314701 spiffe_tls-0.1.1/src/spiffetls/listen.py
--rw-r--r--   0        0        0     2621 2024-04-01 01:23:32.314701 spiffe_tls-0.1.1/src/spiffetls/mode.py
--rw-r--r--   0        0        0        0 2024-04-01 01:23:32.314701 spiffe_tls-0.1.1/src/spiffetls/tlsconfig/__init__.py
--rw-r--r--   0        0        0     3756 2024-04-01 01:23:32.314701 spiffe_tls-0.1.1/src/spiffetls/tlsconfig/authorize.py
--rw-r--r--   0        0        0     3059 1970-01-01 00:00:00.000000 spiffe_tls-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-06 18:01:55.477739 spiffe_tls-0.1.2/LICENSE
+-rw-r--r--   0        0        0     2386 2024-04-06 18:01:55.477739 spiffe_tls-0.1.2/README.md
+-rw-r--r--   0        0        0      962 2024-04-06 18:01:55.477739 spiffe_tls-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      208 2024-04-06 18:01:55.477739 spiffe_tls-0.1.2/src/spiffetls/__init__.py
+-rw-r--r--   0        0        0     5398 2024-04-06 18:01:55.477739 spiffe_tls-0.1.2/src/spiffetls/context.py
+-rw-r--r--   0        0        0     3011 2024-04-06 18:01:55.477739 spiffe_tls-0.1.2/src/spiffetls/dial.py
+-rw-r--r--   0        0        0     1816 2024-04-06 18:01:55.477739 spiffe_tls-0.1.2/src/spiffetls/errors.py
+-rw-r--r--   0        0        0     4463 2024-04-06 18:01:55.477739 spiffe_tls-0.1.2/src/spiffetls/listen.py
+-rw-r--r--   0        0        0     2621 2024-04-06 18:01:55.477739 spiffe_tls-0.1.2/src/spiffetls/mode.py
+-rw-r--r--   0        0        0        0 2024-04-06 18:01:55.477739 spiffe_tls-0.1.2/src/spiffetls/tlsconfig/__init__.py
+-rw-r--r--   0        0        0     3756 2024-04-06 18:01:55.477739 spiffe_tls-0.1.2/src/spiffetls/tlsconfig/authorize.py
+-rw-r--r--   0        0        0     3140 1970-01-01 00:00:00.000000 spiffe_tls-0.1.2/PKG-INFO
```

### Comparing `spiffe_tls-0.1.1/LICENSE` & `spiffe_tls-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `spiffe_tls-0.1.1/README.md` & `spiffe_tls-0.1.2/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 # `spiffe-tls` package (experimental)
 
 ## Overview
 
-The `spiffe-tls` package, part of the `py-spiffe` library, is designed to simplify the creation of secure TLS
-connections by leveraging SPIFFE IDs for authentication. Utilizing the capabilities
-of [pyOpenSSL](https://pypi.org/project/pyOpenSSL/), this package offers
-straightforward utilities for both TLS client and server configurations. Currently in its experimental phase,
-`spiffe-tls`enables integration of [SPIFFE](https://spiffe.io)-based authentication, facilitating automatic management
-of X.509 certificates and CA trusted bundles through an `X509Source` from the [spiffe](https://pypi.org/project/spiffe/)
-package.
+The `spiffe-tls` package, part of the [py-spiffe library](https://github.com/HewlettPackard/py-spiffe), streamlines the
+establishment of secure TLS connections using [SPIFFE](https://spiffe.io) certificates. Powered
+by  [pyOpenSSL](https://pypi.org/project/pyOpenSSL/), it provides straightforward utilities for configuring TLS clients
+and servers. Currently experimental, `spiffe-tls` facilitates the seamless integration of SPIFFE for the automatic
+management of X.509 certificates and CA trust bundles via `X509Source` from
+the [spiffe](https://pypi.org/project/spiffe/) package.
 
 ## Key Features
 
 - TLS connections with SPIFFE ID validation.
 - Mutual TLS (MTLS) support for authenticated client-server communication.
 - Customizable server and client TLS configurations.
```

### Comparing `spiffe_tls-0.1.1/pyproject.toml` & `spiffe_tls-0.1.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 [tool.poetry]
 name = "spiffe-tls"
-version = "0.1.1"
+version = "0.1.2"
 description = "TLS Support using SPIFFE"
 authors = ["Max Lambrecht <maxlambrecht@gmail.com>"]
 readme = "README.md"
 license = "Apache-2.0"
+repository = "https://github.com/HewlettPackard/py-spiffe"
 
 packages = [
     { include = "spiffetls", from = "src" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"  # >= 3.9, < 4.0
-spiffe = "~0.1.0"
+spiffe = "~0.1.2"
 pyOpenSSL = "^24.0"
 
 [tool.poetry.dev-dependencies]
 black = "^24.3"
 mypy = "^1.9"
-mypy-protobuf = "^3.0"
+mypy-protobuf = "^3.6"
 types-pyOpenSSL = "^24.0"
 pytest = "^8.1"
 pytest-mock = "^3.14"
 pre-commit = "^3.7"
 flake8 = "^7.0"
 testutils = { path = "../testutils" }
```

### Comparing `spiffe_tls-0.1.1/src/spiffetls/context.py` & `spiffe_tls-0.1.2/src/spiffetls/context.py`

 * *Files identical despite different names*

### Comparing `spiffe_tls-0.1.1/src/spiffetls/dial.py` & `spiffe_tls-0.1.2/src/spiffetls/dial.py`

 * *Files identical despite different names*

### Comparing `spiffe_tls-0.1.1/src/spiffetls/errors.py` & `spiffe_tls-0.1.2/src/spiffetls/errors.py`

 * *Files identical despite different names*

### Comparing `spiffe_tls-0.1.1/src/spiffetls/listen.py` & `spiffe_tls-0.1.2/src/spiffetls/listen.py`

 * *Files identical despite different names*

### Comparing `spiffe_tls-0.1.1/src/spiffetls/mode.py` & `spiffe_tls-0.1.2/src/spiffetls/mode.py`

 * *Files identical despite different names*

### Comparing `spiffe_tls-0.1.1/src/spiffetls/tlsconfig/authorize.py` & `spiffe_tls-0.1.2/src/spiffetls/tlsconfig/authorize.py`

 * *Files identical despite different names*

### Comparing `spiffe_tls-0.1.1/PKG-INFO` & `spiffe_tls-0.1.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 Metadata-Version: 2.1
 Name: spiffe-tls
-Version: 0.1.1
+Version: 0.1.2
 Summary: TLS Support using SPIFFE
+Home-page: https://github.com/HewlettPackard/py-spiffe
 License: Apache-2.0
 Author: Max Lambrecht
 Author-email: maxlambrecht@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: pyOpenSSL (>=24.0,<25.0)
-Requires-Dist: spiffe (>=0.1.0,<0.2.0)
+Requires-Dist: spiffe (>=0.1.2,<0.2.0)
+Project-URL: Repository, https://github.com/HewlettPackard/py-spiffe
 Description-Content-Type: text/markdown
 
 # `spiffe-tls` package (experimental)
 
 ## Overview
 
-The `spiffe-tls` package, part of the `py-spiffe` library, is designed to simplify the creation of secure TLS
-connections by leveraging SPIFFE IDs for authentication. Utilizing the capabilities
-of [pyOpenSSL](https://pypi.org/project/pyOpenSSL/), this package offers
-straightforward utilities for both TLS client and server configurations. Currently in its experimental phase,
-`spiffe-tls`enables integration of [SPIFFE](https://spiffe.io)-based authentication, facilitating automatic management
-of X.509 certificates and CA trusted bundles through an `X509Source` from the [spiffe](https://pypi.org/project/spiffe/)
-package.
+The `spiffe-tls` package, part of the [py-spiffe library](https://github.com/HewlettPackard/py-spiffe), streamlines the
+establishment of secure TLS connections using [SPIFFE](https://spiffe.io) certificates. Powered
+by  [pyOpenSSL](https://pypi.org/project/pyOpenSSL/), it provides straightforward utilities for configuring TLS clients
+and servers. Currently experimental, `spiffe-tls` facilitates the seamless integration of SPIFFE for the automatic
+management of X.509 certificates and CA trust bundles via `X509Source` from
+the [spiffe](https://pypi.org/project/spiffe/) package.
 
 ## Key Features
 
 - TLS connections with SPIFFE ID validation.
 - Mutual TLS (MTLS) support for authenticated client-server communication.
 - Customizable server and client TLS configurations.
```

