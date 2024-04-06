# Comparing `tmp/offat-0.8.1.tar.gz` & `tmp/offat-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "offat-0.8.1.tar", max compression
+gzip compressed data, was "offat-0.9.0.tar", max compression
```

## Comparing `offat-0.8.1.tar` & `offat-0.9.0.tar`

### file list

```diff
@@ -1,20 +1,26 @@
--rw-r--r--   0        0        0     1071 2023-09-22 05:42:08.060221 offat-0.8.1/LICENSE
--rw-r--r--   0        0        0     7732 2023-09-22 05:42:08.060221 offat-0.8.1/README.md
--rw-r--r--   0        0        0        0 2023-09-22 05:42:08.060221 offat-0.8.1/offat/__init__.py
--rw-r--r--   0        0        0     3044 2023-09-22 05:42:08.060221 offat-0.8.1/offat/__main__.py
--rw-r--r--   0        0        0     1812 2023-09-22 05:42:08.060221 offat-0.8.1/offat/config_data_handler.py
--rw-r--r--   0        0        0     4355 2023-09-22 05:42:08.060221 offat-0.8.1/offat/http.py
--rw-r--r--   0        0        0     1122 2023-09-22 05:42:08.064221 offat-0.8.1/offat/logger.py
--rw-r--r--   0        0        0     3767 2023-09-22 05:42:08.064221 offat-0.8.1/offat/openapi.py
--rw-r--r--   0        0        0        0 2023-09-22 05:42:08.064221 offat-0.8.1/offat/tester/__init__.py
--rw-r--r--   0        0        0     1567 2023-09-22 05:42:08.064221 offat-0.8.1/offat/tester/data_exposure.py
--rw-r--r--   0        0        0     3730 2023-09-22 05:42:08.064221 offat-0.8.1/offat/tester/fuzzer.py
--rw-r--r--   0        0        0     4738 2023-09-22 05:42:08.064221 offat-0.8.1/offat/tester/post_test_processor.py
--rw-r--r--   0        0        0     1617 2023-09-22 05:42:08.064221 offat-0.8.1/offat/tester/regexs.py
--rw-r--r--   0        0        0    29165 2023-09-22 05:42:08.064221 offat-0.8.1/offat/tester/test_generator.py
--rw-r--r--   0        0        0     2280 2023-09-22 05:42:08.064221 offat-0.8.1/offat/tester/test_results.py
--rw-r--r--   0        0        0     5150 2023-09-22 05:42:08.064221 offat-0.8.1/offat/tester/test_runner.py
--rw-r--r--   0        0        0     6959 2023-09-22 05:42:08.064221 offat-0.8.1/offat/tester/tester_utils.py
--rw-r--r--   0        0        0     4783 2023-09-22 05:42:08.064221 offat-0.8.1/offat/utils.py
--rw-r--r--   0        0        0      873 2023-09-22 05:42:08.064221 offat-0.8.1/pyproject.toml
--rw-r--r--   0        0        0     8700 1970-01-01 00:00:00.000000 offat-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-09-23 18:59:05.616972 offat-0.9.0/LICENSE
+-rw-r--r--   0        0        0     8466 2023-09-23 18:59:05.616972 offat-0.9.0/README.md
+-rw-r--r--   0        0        0        0 2023-09-23 18:59:05.616972 offat-0.9.0/offat/__init__.py
+-rw-r--r--   0        0        0     3044 2023-09-23 18:59:05.616972 offat-0.9.0/offat/__main__.py
+-rw-r--r--   0        0        0        0 2023-09-23 18:59:05.616972 offat-0.9.0/offat/api/__init__.py
+-rw-r--r--   0        0        0      182 2023-09-23 18:59:05.616972 offat-0.9.0/offat/api/__main__.py
+-rw-r--r--   0        0        0     2143 2023-09-23 18:59:05.616972 offat-0.9.0/offat/api/app.py
+-rw-r--r--   0        0        0      395 2023-09-23 18:59:05.616972 offat-0.9.0/offat/api/config.py
+-rw-r--r--   0        0        0      613 2023-09-23 18:59:05.616972 offat-0.9.0/offat/api/jobs.py
+-rw-r--r--   0        0        0       98 2023-09-23 18:59:05.616972 offat-0.9.0/offat/api/models.py
+-rw-r--r--   0        0        0     1812 2023-09-23 18:59:05.616972 offat-0.9.0/offat/config_data_handler.py
+-rw-r--r--   0        0        0     4355 2023-09-23 18:59:05.616972 offat-0.9.0/offat/http.py
+-rw-r--r--   0        0        0     1122 2023-09-23 18:59:05.616972 offat-0.9.0/offat/logger.py
+-rw-r--r--   0        0        0     3881 2023-09-23 18:59:05.616972 offat-0.9.0/offat/openapi.py
+-rw-r--r--   0        0        0        0 2023-09-23 18:59:05.616972 offat-0.9.0/offat/tester/__init__.py
+-rw-r--r--   0        0        0     1567 2023-09-23 18:59:05.616972 offat-0.9.0/offat/tester/data_exposure.py
+-rw-r--r--   0        0        0     3730 2023-09-23 18:59:05.616972 offat-0.9.0/offat/tester/fuzzer.py
+-rw-r--r--   0        0        0     4738 2023-09-23 18:59:05.616972 offat-0.9.0/offat/tester/post_test_processor.py
+-rw-r--r--   0        0        0     1617 2023-09-23 18:59:05.616972 offat-0.9.0/offat/tester/regexs.py
+-rw-r--r--   0        0        0    29165 2023-09-23 18:59:05.616972 offat-0.9.0/offat/tester/test_generator.py
+-rw-r--r--   0        0        0     2280 2023-09-23 18:59:05.616972 offat-0.9.0/offat/tester/test_results.py
+-rw-r--r--   0        0        0     5150 2023-09-23 18:59:05.616972 offat-0.9.0/offat/tester/test_runner.py
+-rw-r--r--   0        0        0     6973 2023-09-23 18:59:05.616972 offat-0.9.0/offat/tester/tester_utils.py
+-rw-r--r--   0        0        0     4783 2023-09-23 18:59:05.616972 offat-0.9.0/offat/utils.py
+-rw-r--r--   0        0        0     1221 2023-09-23 18:59:05.620972 offat-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     9755 1970-01-01 00:00:00.000000 offat-0.9.0/PKG-INFO
```

### Comparing `offat-0.8.1/LICENSE` & `offat-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `offat-0.8.1/README.md` & `offat-0.9.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -2,26 +2,36 @@
 
 ![OffAT Logo](./.images/logos/offat.png)
 
 Automatically Tests for vulnerabilities after generating tests from openapi specification file. Project is in Beta stage, so sometimes it might crash while running.
 
 ![UnDocumented petstore API endpoint HTTP method results](./.images/tests/offat-v0.5.0.png)
 
-## Features
+## Security Checks
 
 - [X] Restricted HTTP Methods
 - [X] SQLi
 - [X] BOLA (Might need few bug fixes)
 - [X] Data Exposure (Detects Common Data Exposures)
 - [X] BOPLA / Mass Assignment
 - [X] Broken Access Control
 - [X] Basic Command Injection
 - [X] Basic XSS/HTML Injection test
 - [ ] Broken Authentication
 
+## Features
+
+- Few Security Checks from OWASP API Top 10
+- Automated Testing
+- User Config
+- API for Automating tests and Integrating Tool with other platforms/tools
+- CLI tool
+- Dockerized Project for Easy Usage
+- Open Source Tool with MIT License
+
 ## Demo
 
 [![asciicast](https://asciinema.org/a/9MSwl7UafIVT3iJn13OcvWXeF.svg)](https://asciinema.org/a/9MSwl7UafIVT3iJn13OcvWXeF)
 
 ## PyPi Downloads
 
 [![Upload offat Python Package to PyPi](https://github.com/dmdhrumilmistry/offat/actions/workflows/pypi-publish.yml/badge.svg)](https://github.com/dmdhrumilmistry/offat/actions/workflows/pypi-publish.yml)
@@ -51,27 +61,42 @@
   ```bash
   python3 -m pip install git+https://github.com/dmdhrumilmistry/offat.git
   ```
 
 - Install Release from PyPi
 
   ```bash
-  python3 -m pip install offat
+  python3 -m pip install offat        # only cli tool
+  python3 -m pip install offat[api]   # cli + api
   ```
 
 ### Using Containers
 
 ### Docker
 
 - Build Image
 
   ```bash
-  docker build -t offat .
+  make build-local-images
+  ```
+
+- CLI Tool
+
+  ```bash
+  docker run --rm dmdhrumilmistry/offat
+  ```
+
+- API
+
+  ```bash
+  docker compose up -d
   ```
 
+  > POST `openapi` documentation to `/api/v1/scan/` endpoint with its valid `type` (json/yaml); `job_id` will be returned, `job_id` should
+
 ### Manual Method
 
 - Open terminal
 
 - Install git package
 
   ```bash
@@ -97,14 +122,26 @@
   ```bash
   # without options
   poetry install
   ```
 
 ## Start OffAT
 
+### API
+
+- Start API Server
+
+  ```bash
+  python -m offat.api
+  ```
+
+- API Documentation can be found at <http://localhost:8000/docs>
+
+### CLI Tool
+
 - Run offat
 
   ```bash
   offat -f swagger_file.json
   ```
 
 - To get all the commands use `help`
```

### Comparing `offat-0.8.1/offat/__main__.py` & `offat-0.9.0/offat/__main__.py`

 * *Files identical despite different names*

### Comparing `offat-0.8.1/offat/config_data_handler.py` & `offat-0.9.0/offat/config_data_handler.py`

 * *Files identical despite different names*

### Comparing `offat-0.8.1/offat/http.py` & `offat-0.9.0/offat/http.py`

 * *Files identical despite different names*

### Comparing `offat-0.8.1/offat/logger.py` & `offat-0.9.0/offat/logger.py`

 * *Files identical despite different names*

### Comparing `offat-0.8.1/offat/openapi.py` & `offat-0.9.0/offat/openapi.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,22 +3,25 @@
 
 
 logger = create_logger(__name__)
 
 
 class OpenAPIParser:
     ''''''
-    def __init__(self, fpath:str) -> None:
-        self._parser = ResolvingParser(fpath, backend = 'openapi-spec-validator')
-        if self._parser.valid:
-            logger.info('Specification file is valid')
+    def __init__(self, fpath:str, spec:dict=None) -> None:
+        if fpath:
+            self._parser = ResolvingParser(fpath, backend = 'openapi-spec-validator')
+            if self._parser.valid:
+                logger.info('Specification file is valid')
+            else:
+                logger.error('Specification file is invalid!')
+            self._spec = self._parser.specification
         else:
-            logger.error('Specification file is invalid!')
-
-        self._spec = self._parser.specification
+            self._spec = spec
+            
         self.host = self._spec.get('host')
         self.base_url = f"http://{self.host}{self._spec.get('basePath','')}"
         self.request_response_params = self._get_request_response_params()
 
 
     def _get_endpoints(self):
         '''Returns list of endpoint paths along with HTTP methods allowed'''
```

### Comparing `offat-0.8.1/offat/tester/data_exposure.py` & `offat-0.9.0/offat/tester/data_exposure.py`

 * *Files identical despite different names*

### Comparing `offat-0.8.1/offat/tester/fuzzer.py` & `offat-0.9.0/offat/tester/fuzzer.py`

 * *Files identical despite different names*

### Comparing `offat-0.8.1/offat/tester/post_test_processor.py` & `offat-0.9.0/offat/tester/post_test_processor.py`

 * *Files identical despite different names*

### Comparing `offat-0.8.1/offat/tester/regexs.py` & `offat-0.9.0/offat/tester/regexs.py`

 * *Files identical despite different names*

### Comparing `offat-0.8.1/offat/tester/test_generator.py` & `offat-0.9.0/offat/tester/test_generator.py`

 * *Files identical despite different names*

### Comparing `offat-0.8.1/offat/tester/test_results.py` & `offat-0.9.0/offat/tester/test_results.py`

 * *Files identical despite different names*

### Comparing `offat-0.8.1/offat/tester/test_runner.py` & `offat-0.9.0/offat/tester/test_runner.py`

 * *Files identical despite different names*

### Comparing `offat-0.8.1/offat/tester/tester_utils.py` & `offat-0.9.0/offat/tester/tester_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -143,8 +143,8 @@
         write_json_to_file(
             json_data={
                 'results':results
             }, 
             file_path=output_file
         )
 
-    
+    return results
```

### Comparing `offat-0.8.1/offat/utils.py` & `offat-0.9.0/offat/utils.py`

 * *Files identical despite different names*

### Comparing `offat-0.8.1/pyproject.toml` & `offat-0.9.0/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,27 +1,34 @@
 [tool.poetry]
 name = "offat"
-version = "0.8.1"
+version = "0.9.0"
 description = "Offensive API tester tool automates checks for common API vulnerabilities"
 authors = ["Dhrumil Mistry <56185972+dmdhrumilmistry@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 aiohttp = "^3.8.4"
 pyyaml = "^6.0"
 prance = "^23.6.21.0"
 openapi-spec-validator = "^0.5.7"
 colorama = "^0.4.6"
 tabulate = "^0.9.0"
+fastapi = {version = "^0.103.1", optional = true}
+uvicorn = {extras = ["standard"], version = "^0.23.2", optional = true}
+rq = {version = "^1.15.1", optional = true}
+redis = {version = "^5.0.0", optional = true}
+python-dotenv = {version = "^1.0.0", optional = true}
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.0"
 
+[tool.poetry.extras]
+api = ["fastapi", "uvicorn", "redis", "rq", "python-dotenv"]
 
 [tool.poetry.urls]
 "Home" = "https://github.com/dmdhrumilmistry/offat"
 "Bug Tracker" = "https://github.com/dmdhrumilmistry/offat/issues"
 "Support" = "https://github.com/sponsors/dmdhrumilmistry/"
 "PayPal" = "https://paypal.me/dmdhrumilmistry"
```

### Comparing `offat-0.8.1/PKG-INFO` & `offat-0.9.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,50 +1,66 @@
 Metadata-Version: 2.1
 Name: offat
-Version: 0.8.1
+Version: 0.9.0
 Summary: Offensive API tester tool automates checks for common API vulnerabilities
 License: MIT
 Author: Dhrumil Mistry
 Author-email: 56185972+dmdhrumilmistry@users.noreply.github.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: api
 Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
 Requires-Dist: colorama (>=0.4.6,<0.5.0)
+Requires-Dist: fastapi (>=0.103.1,<0.104.0) ; extra == "api"
 Requires-Dist: openapi-spec-validator (>=0.5.7,<0.6.0)
 Requires-Dist: prance (>=23.6.21.0,<24.0.0.0)
+Requires-Dist: python-dotenv (>=1.0.0,<2.0.0) ; extra == "api"
 Requires-Dist: pyyaml (>=6.0,<7.0)
+Requires-Dist: redis (>=5.0.0,<6.0.0) ; extra == "api"
+Requires-Dist: rq (>=1.15.1,<2.0.0) ; extra == "api"
 Requires-Dist: tabulate (>=0.9.0,<0.10.0)
+Requires-Dist: uvicorn[standard] (>=0.23.2,<0.24.0) ; extra == "api"
 Project-URL: Bug Tracker, https://github.com/dmdhrumilmistry/offat/issues
 Project-URL: Home, https://github.com/dmdhrumilmistry/offat
 Project-URL: PayPal, https://paypal.me/dmdhrumilmistry
 Project-URL: Support, https://github.com/sponsors/dmdhrumilmistry/
 Description-Content-Type: text/markdown
 
 # OFFAT - OFFensive Api Tester
 
 ![OffAT Logo](./.images/logos/offat.png)
 
 Automatically Tests for vulnerabilities after generating tests from openapi specification file. Project is in Beta stage, so sometimes it might crash while running.
 
 ![UnDocumented petstore API endpoint HTTP method results](./.images/tests/offat-v0.5.0.png)
 
-## Features
+## Security Checks
 
 - [X] Restricted HTTP Methods
 - [X] SQLi
 - [X] BOLA (Might need few bug fixes)
 - [X] Data Exposure (Detects Common Data Exposures)
 - [X] BOPLA / Mass Assignment
 - [X] Broken Access Control
 - [X] Basic Command Injection
 - [X] Basic XSS/HTML Injection test
 - [ ] Broken Authentication
 
+## Features
+
+- Few Security Checks from OWASP API Top 10
+- Automated Testing
+- User Config
+- API for Automating tests and Integrating Tool with other platforms/tools
+- CLI tool
+- Dockerized Project for Easy Usage
+- Open Source Tool with MIT License
+
 ## Demo
 
 [![asciicast](https://asciinema.org/a/9MSwl7UafIVT3iJn13OcvWXeF.svg)](https://asciinema.org/a/9MSwl7UafIVT3iJn13OcvWXeF)
 
 ## PyPi Downloads
 
 [![Upload offat Python Package to PyPi](https://github.com/dmdhrumilmistry/offat/actions/workflows/pypi-publish.yml/badge.svg)](https://github.com/dmdhrumilmistry/offat/actions/workflows/pypi-publish.yml)
@@ -74,27 +90,42 @@
   ```bash
   python3 -m pip install git+https://github.com/dmdhrumilmistry/offat.git
   ```
 
 - Install Release from PyPi
 
   ```bash
-  python3 -m pip install offat
+  python3 -m pip install offat        # only cli tool
+  python3 -m pip install offat[api]   # cli + api
   ```
 
 ### Using Containers
 
 ### Docker
 
 - Build Image
 
   ```bash
-  docker build -t offat .
+  make build-local-images
+  ```
+
+- CLI Tool
+
+  ```bash
+  docker run --rm dmdhrumilmistry/offat
+  ```
+
+- API
+
+  ```bash
+  docker compose up -d
   ```
 
+  > POST `openapi` documentation to `/api/v1/scan/` endpoint with its valid `type` (json/yaml); `job_id` will be returned, `job_id` should
+
 ### Manual Method
 
 - Open terminal
 
 - Install git package
 
   ```bash
@@ -120,14 +151,26 @@
   ```bash
   # without options
   poetry install
   ```
 
 ## Start OffAT
 
+### API
+
+- Start API Server
+
+  ```bash
+  python -m offat.api
+  ```
+
+- API Documentation can be found at <http://localhost:8000/docs>
+
+### CLI Tool
+
 - Run offat
 
   ```bash
   offat -f swagger_file.json
   ```
 
 - To get all the commands use `help`
```

