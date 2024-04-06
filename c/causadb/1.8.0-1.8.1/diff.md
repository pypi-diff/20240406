# Comparing `tmp/causadb-1.8.0.tar.gz` & `tmp/causadb-1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "causadb-1.8.0.tar", max compression
+gzip compressed data, was "causadb-1.8.1.tar", max compression
```

## Comparing `causadb-1.8.0.tar` & `causadb-1.8.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      642 2024-04-05 11:48:58.012021 causadb-1.8.0/README.md
--rw-r--r--   0        0        0      115 2024-04-05 11:48:58.012021 causadb-1.8.0/causadb/__init__.py
--rw-r--r--   0        0        0       22 2024-04-05 11:49:26.215869 causadb-1.8.0/causadb/__version__.py
--rw-r--r--   0        0        0     5338 2024-04-05 11:48:58.012021 causadb-1.8.0/causadb/causadb.py
--rw-r--r--   0        0        0     2855 2024-04-05 11:48:58.012021 causadb-1.8.0/causadb/cli/account.py
--rw-r--r--   0        0        0     3116 2024-04-05 11:48:58.012021 causadb-1.8.0/causadb/cli/data.py
--rwxr-xr-x   0        0        0      962 2024-04-05 11:48:58.012021 causadb-1.8.0/causadb/cli/main.py
--rw-r--r--   0        0        0     7085 2024-04-05 11:48:58.012021 causadb-1.8.0/causadb/cli/models.py
--rw-r--r--   0        0        0      891 2024-04-05 11:48:58.012021 causadb-1.8.0/causadb/cli/utils.py
--rw-r--r--   0        0        0     2646 2024-04-05 11:48:58.012021 causadb-1.8.0/causadb/data.py
--rw-r--r--   0        0        0        0 2024-04-05 11:48:58.012021 causadb-1.8.0/causadb/examples/__init__.py
--rw-r--r--   0        0        0     1876 2024-04-05 11:48:58.012021 causadb-1.8.0/causadb/examples/heating.py
--rw-r--r--   0        0        0    15066 2024-04-05 11:48:58.012021 causadb-1.8.0/causadb/model.py
--rw-r--r--   0        0        0     2555 2024-04-05 11:48:58.012021 causadb-1.8.0/causadb/plotting.py
--rw-r--r--   0        0        0      215 2024-04-05 11:48:58.012021 causadb-1.8.0/causadb/utils.py
--rw-r--r--   0        0        0      796 2024-04-05 11:49:25.435874 causadb-1.8.0/pyproject.toml
--rw-r--r--   0        0        0     1655 1970-01-01 00:00:00.000000 causadb-1.8.0/PKG-INFO
+-rw-r--r--   0        0        0      642 2024-04-06 09:23:58.565904 causadb-1.8.1/README.md
+-rw-r--r--   0        0        0      115 2024-04-06 09:23:58.565904 causadb-1.8.1/causadb/__init__.py
+-rw-r--r--   0        0        0       22 2024-04-06 09:24:25.677896 causadb-1.8.1/causadb/__version__.py
+-rw-r--r--   0        0        0     5338 2024-04-06 09:23:58.565904 causadb-1.8.1/causadb/causadb.py
+-rw-r--r--   0        0        0     2855 2024-04-06 09:23:58.565904 causadb-1.8.1/causadb/cli/account.py
+-rw-r--r--   0        0        0     3116 2024-04-06 09:23:58.565904 causadb-1.8.1/causadb/cli/data.py
+-rwxr-xr-x   0        0        0      962 2024-04-06 09:23:58.565904 causadb-1.8.1/causadb/cli/main.py
+-rw-r--r--   0        0        0     7085 2024-04-06 09:23:58.565904 causadb-1.8.1/causadb/cli/models.py
+-rw-r--r--   0        0        0      891 2024-04-06 09:23:58.565904 causadb-1.8.1/causadb/cli/utils.py
+-rw-r--r--   0        0        0     2646 2024-04-06 09:23:58.565904 causadb-1.8.1/causadb/data.py
+-rw-r--r--   0        0        0        0 2024-04-06 09:23:58.565904 causadb-1.8.1/causadb/examples/__init__.py
+-rw-r--r--   0        0        0     1876 2024-04-06 09:23:58.565904 causadb-1.8.1/causadb/examples/heating.py
+-rw-r--r--   0        0        0    15066 2024-04-06 09:23:58.565904 causadb-1.8.1/causadb/model.py
+-rw-r--r--   0        0        0     2555 2024-04-06 09:23:58.565904 causadb-1.8.1/causadb/plotting.py
+-rw-r--r--   0        0        0      215 2024-04-06 09:23:58.565904 causadb-1.8.1/causadb/utils.py
+-rw-r--r--   0        0        0      797 2024-04-06 09:24:24.633897 causadb-1.8.1/pyproject.toml
+-rw-r--r--   0        0        0     1656 1970-01-01 00:00:00.000000 causadb-1.8.1/PKG-INFO
```

### Comparing `causadb-1.8.0/README.md` & `causadb-1.8.1/README.md`

 * *Files identical despite different names*

### Comparing `causadb-1.8.0/causadb/causadb.py` & `causadb-1.8.1/causadb/causadb.py`

 * *Files identical despite different names*

### Comparing `causadb-1.8.0/causadb/cli/account.py` & `causadb-1.8.1/causadb/cli/account.py`

 * *Files identical despite different names*

### Comparing `causadb-1.8.0/causadb/cli/data.py` & `causadb-1.8.1/causadb/cli/data.py`

 * *Files identical despite different names*

### Comparing `causadb-1.8.0/causadb/cli/main.py` & `causadb-1.8.1/causadb/cli/main.py`

 * *Files identical despite different names*

### Comparing `causadb-1.8.0/causadb/cli/models.py` & `causadb-1.8.1/causadb/cli/models.py`

 * *Files identical despite different names*

### Comparing `causadb-1.8.0/causadb/cli/utils.py` & `causadb-1.8.1/causadb/cli/utils.py`

 * *Files identical despite different names*

### Comparing `causadb-1.8.0/causadb/data.py` & `causadb-1.8.1/causadb/data.py`

 * *Files identical despite different names*

### Comparing `causadb-1.8.0/causadb/examples/heating.py` & `causadb-1.8.1/causadb/examples/heating.py`

 * *Files identical despite different names*

### Comparing `causadb-1.8.0/causadb/model.py` & `causadb-1.8.1/causadb/model.py`

 * *Files identical despite different names*

### Comparing `causadb-1.8.0/causadb/plotting.py` & `causadb-1.8.1/causadb/plotting.py`

 * *Files identical despite different names*

### Comparing `causadb-1.8.0/pyproject.toml` & `causadb-1.8.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "causadb"
-version = "1.8.0"
+version = "1.8.1"
 description = ""
 authors = ["Jordan hart <jordan@causa.tech>"]
 readme = "README.md"
 packages = [
     { include = "causadb", from = "." }
 ]
 
 [tool.poetry.scripts]
 causadb = "causadb.cli.main:app"
 
 [tool.poetry.dependencies]
 python = "^3.9"
-typer = {extras = ["all"], version = "^0.9.0"}
+typer = {extras = ["all"], version = "^0.12.1"}
 requests = "^2.31.0"
 toml = "^0.10.2"
 rich = "^13.7.0"
 pandas = "^2.2.0"
 marko = "^2.0.2"
 setuptools = "^69.0.3"
 python-dotenv = "^1.0.1"
```

### Comparing `causadb-1.8.0/PKG-INFO` & `causadb-1.8.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: causadb
-Version: 1.8.0
+Version: 1.8.1
 Summary: 
 Author: Jordan hart
 Author-email: jordan@causa.tech
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -19,15 +19,15 @@
 Requires-Dist: python-dotenv (>=1.0.1,<2.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: rich (>=13.7.0,<14.0.0)
 Requires-Dist: seaborn (>=0.13.2,<0.14.0)
 Requires-Dist: setuptools (>=69.0.3,<70.0.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Requires-Dist: tqdm (>=4.66.2,<5.0.0)
-Requires-Dist: typer[all] (>=0.9.0,<0.10.0)
+Requires-Dist: typer[all] (>=0.12.1,<0.13.0)
 Description-Content-Type: text/markdown
 
 # CausaDB Command Line Interface (CLI) and Python Client
 
 This is the CLI and Python client for CausaDB, an easy-to-use platform for building and querying causal AI models in the cloud.
 
 ## Documentation
```

