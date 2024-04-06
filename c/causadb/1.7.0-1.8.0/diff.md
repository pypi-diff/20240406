# Comparing `tmp/causadb-1.7.0.tar.gz` & `tmp/causadb-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "causadb-1.7.0.tar", max compression
+gzip compressed data, was "causadb-1.8.0.tar", max compression
```

## Comparing `causadb-1.7.0.tar` & `causadb-1.8.0.tar`

### file list

```diff
@@ -1,16 +1,17 @@
--rw-r--r--   0        0        0      642 2024-04-04 19:10:01.661629 causadb-1.7.0/README.md
--rw-r--r--   0        0        0      115 2024-04-04 19:10:01.661629 causadb-1.7.0/causadb/__init__.py
--rw-r--r--   0        0        0       22 2024-04-04 19:10:21.978006 causadb-1.7.0/causadb/__version__.py
--rw-r--r--   0        0        0     5338 2024-04-04 19:10:01.661629 causadb-1.7.0/causadb/causadb.py
--rw-r--r--   0        0        0     2855 2024-04-04 19:10:01.661629 causadb-1.7.0/causadb/cli/account.py
--rw-r--r--   0        0        0     3116 2024-04-04 19:10:01.661629 causadb-1.7.0/causadb/cli/data.py
--rwxr-xr-x   0        0        0      962 2024-04-04 19:10:01.661629 causadb-1.7.0/causadb/cli/main.py
--rw-r--r--   0        0        0     7085 2024-04-04 19:10:01.661629 causadb-1.7.0/causadb/cli/models.py
--rw-r--r--   0        0        0      891 2024-04-04 19:10:01.661629 causadb-1.7.0/causadb/cli/utils.py
--rw-r--r--   0        0        0     2646 2024-04-04 19:10:01.661629 causadb-1.7.0/causadb/data.py
--rw-r--r--   0        0        0        0 2024-04-04 19:10:01.661629 causadb-1.7.0/causadb/examples/__init__.py
--rw-r--r--   0        0        0     1876 2024-04-04 19:10:01.661629 causadb-1.7.0/causadb/examples/heating.py
--rw-r--r--   0        0        0    15066 2024-04-04 19:10:01.661629 causadb-1.7.0/causadb/model.py
--rw-r--r--   0        0        0      215 2024-04-04 19:10:01.661629 causadb-1.7.0/causadb/utils.py
--rw-r--r--   0        0        0      715 2024-04-04 19:10:21.145991 causadb-1.7.0/pyproject.toml
--rw-r--r--   0        0        0     1529 1970-01-01 00:00:00.000000 causadb-1.7.0/PKG-INFO
+-rw-r--r--   0        0        0      642 2024-04-05 11:48:58.012021 causadb-1.8.0/README.md
+-rw-r--r--   0        0        0      115 2024-04-05 11:48:58.012021 causadb-1.8.0/causadb/__init__.py
+-rw-r--r--   0        0        0       22 2024-04-05 11:49:26.215869 causadb-1.8.0/causadb/__version__.py
+-rw-r--r--   0        0        0     5338 2024-04-05 11:48:58.012021 causadb-1.8.0/causadb/causadb.py
+-rw-r--r--   0        0        0     2855 2024-04-05 11:48:58.012021 causadb-1.8.0/causadb/cli/account.py
+-rw-r--r--   0        0        0     3116 2024-04-05 11:48:58.012021 causadb-1.8.0/causadb/cli/data.py
+-rwxr-xr-x   0        0        0      962 2024-04-05 11:48:58.012021 causadb-1.8.0/causadb/cli/main.py
+-rw-r--r--   0        0        0     7085 2024-04-05 11:48:58.012021 causadb-1.8.0/causadb/cli/models.py
+-rw-r--r--   0        0        0      891 2024-04-05 11:48:58.012021 causadb-1.8.0/causadb/cli/utils.py
+-rw-r--r--   0        0        0     2646 2024-04-05 11:48:58.012021 causadb-1.8.0/causadb/data.py
+-rw-r--r--   0        0        0        0 2024-04-05 11:48:58.012021 causadb-1.8.0/causadb/examples/__init__.py
+-rw-r--r--   0        0        0     1876 2024-04-05 11:48:58.012021 causadb-1.8.0/causadb/examples/heating.py
+-rw-r--r--   0        0        0    15066 2024-04-05 11:48:58.012021 causadb-1.8.0/causadb/model.py
+-rw-r--r--   0        0        0     2555 2024-04-05 11:48:58.012021 causadb-1.8.0/causadb/plotting.py
+-rw-r--r--   0        0        0      215 2024-04-05 11:48:58.012021 causadb-1.8.0/causadb/utils.py
+-rw-r--r--   0        0        0      796 2024-04-05 11:49:25.435874 causadb-1.8.0/pyproject.toml
+-rw-r--r--   0        0        0     1655 1970-01-01 00:00:00.000000 causadb-1.8.0/PKG-INFO
```

### Comparing `causadb-1.7.0/README.md` & `causadb-1.8.0/README.md`

 * *Files identical despite different names*

### Comparing `causadb-1.7.0/causadb/causadb.py` & `causadb-1.8.0/causadb/causadb.py`

 * *Files identical despite different names*

### Comparing `causadb-1.7.0/causadb/cli/account.py` & `causadb-1.8.0/causadb/cli/account.py`

 * *Files identical despite different names*

### Comparing `causadb-1.7.0/causadb/cli/data.py` & `causadb-1.8.0/causadb/cli/data.py`

 * *Files identical despite different names*

### Comparing `causadb-1.7.0/causadb/cli/main.py` & `causadb-1.8.0/causadb/cli/main.py`

 * *Files identical despite different names*

### Comparing `causadb-1.7.0/causadb/cli/models.py` & `causadb-1.8.0/causadb/cli/models.py`

 * *Files identical despite different names*

### Comparing `causadb-1.7.0/causadb/cli/utils.py` & `causadb-1.8.0/causadb/cli/utils.py`

 * *Files identical despite different names*

### Comparing `causadb-1.7.0/causadb/data.py` & `causadb-1.8.0/causadb/data.py`

 * *Files identical despite different names*

### Comparing `causadb-1.7.0/causadb/examples/heating.py` & `causadb-1.8.0/causadb/examples/heating.py`

 * *Files identical despite different names*

### Comparing `causadb-1.7.0/causadb/model.py` & `causadb-1.8.0/causadb/model.py`

 * *Files identical despite different names*

### Comparing `causadb-1.7.0/pyproject.toml` & `causadb-1.8.0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "causadb"
-version = "1.7.0"
+version = "1.8.0"
 description = ""
 authors = ["Jordan hart <jordan@causa.tech>"]
 readme = "README.md"
 packages = [
     { include = "causadb", from = "." }
 ]
 
@@ -20,16 +20,20 @@
 pandas = "^2.2.0"
 marko = "^2.0.2"
 setuptools = "^69.0.3"
 python-dotenv = "^1.0.1"
 pyarrow = "^15.0.0"
 tqdm = "^4.66.2"
 pydantic = "^2.6.4"
+matplotlib = "^3.8.4"
+seaborn = "^0.13.2"
+networkx = "^3.2.1"
 
 [tool.poetry.group.dev.dependencies]
 invoke = "^2.2.0"
 pydoc-markdown = "^4.8.2"
 pytest = "^7.4.4"
+jupyter = "^1.0.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `causadb-1.7.0/PKG-INFO` & `causadb-1.8.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 Metadata-Version: 2.1
 Name: causadb
-Version: 1.7.0
+Version: 1.8.0
 Summary: 
 Author: Jordan hart
 Author-email: jordan@causa.tech
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: marko (>=2.0.2,<3.0.0)
+Requires-Dist: matplotlib (>=3.8.4,<4.0.0)
+Requires-Dist: networkx (>=3.2.1,<4.0.0)
 Requires-Dist: pandas (>=2.2.0,<3.0.0)
 Requires-Dist: pyarrow (>=15.0.0,<16.0.0)
 Requires-Dist: pydantic (>=2.6.4,<3.0.0)
 Requires-Dist: python-dotenv (>=1.0.1,<2.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: rich (>=13.7.0,<14.0.0)
+Requires-Dist: seaborn (>=0.13.2,<0.14.0)
 Requires-Dist: setuptools (>=69.0.3,<70.0.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Requires-Dist: tqdm (>=4.66.2,<5.0.0)
 Requires-Dist: typer[all] (>=0.9.0,<0.10.0)
 Description-Content-Type: text/markdown
 
 # CausaDB Command Line Interface (CLI) and Python Client
```

