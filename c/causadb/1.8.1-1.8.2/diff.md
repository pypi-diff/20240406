# Comparing `tmp/causadb-1.8.1.tar.gz` & `tmp/causadb-1.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "causadb-1.8.1.tar", max compression
+gzip compressed data, was "causadb-1.8.2.tar", max compression
```

## Comparing `causadb-1.8.1.tar` & `causadb-1.8.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      642 2024-04-06 09:23:58.565904 causadb-1.8.1/README.md
--rw-r--r--   0        0        0      115 2024-04-06 09:23:58.565904 causadb-1.8.1/causadb/__init__.py
--rw-r--r--   0        0        0       22 2024-04-06 09:24:25.677896 causadb-1.8.1/causadb/__version__.py
--rw-r--r--   0        0        0     5338 2024-04-06 09:23:58.565904 causadb-1.8.1/causadb/causadb.py
--rw-r--r--   0        0        0     2855 2024-04-06 09:23:58.565904 causadb-1.8.1/causadb/cli/account.py
--rw-r--r--   0        0        0     3116 2024-04-06 09:23:58.565904 causadb-1.8.1/causadb/cli/data.py
--rwxr-xr-x   0        0        0      962 2024-04-06 09:23:58.565904 causadb-1.8.1/causadb/cli/main.py
--rw-r--r--   0        0        0     7085 2024-04-06 09:23:58.565904 causadb-1.8.1/causadb/cli/models.py
--rw-r--r--   0        0        0      891 2024-04-06 09:23:58.565904 causadb-1.8.1/causadb/cli/utils.py
--rw-r--r--   0        0        0     2646 2024-04-06 09:23:58.565904 causadb-1.8.1/causadb/data.py
--rw-r--r--   0        0        0        0 2024-04-06 09:23:58.565904 causadb-1.8.1/causadb/examples/__init__.py
--rw-r--r--   0        0        0     1876 2024-04-06 09:23:58.565904 causadb-1.8.1/causadb/examples/heating.py
--rw-r--r--   0        0        0    15066 2024-04-06 09:23:58.565904 causadb-1.8.1/causadb/model.py
--rw-r--r--   0        0        0     2555 2024-04-06 09:23:58.565904 causadb-1.8.1/causadb/plotting.py
--rw-r--r--   0        0        0      215 2024-04-06 09:23:58.565904 causadb-1.8.1/causadb/utils.py
--rw-r--r--   0        0        0      797 2024-04-06 09:24:24.633897 causadb-1.8.1/pyproject.toml
--rw-r--r--   0        0        0     1656 1970-01-01 00:00:00.000000 causadb-1.8.1/PKG-INFO
+-rw-r--r--   0        0        0      642 2024-04-06 09:26:04.140433 causadb-1.8.2/README.md
+-rw-r--r--   0        0        0      115 2024-04-06 09:26:04.140433 causadb-1.8.2/causadb/__init__.py
+-rw-r--r--   0        0        0       22 2024-04-06 09:26:36.336281 causadb-1.8.2/causadb/__version__.py
+-rw-r--r--   0        0        0     5338 2024-04-06 09:26:04.140433 causadb-1.8.2/causadb/causadb.py
+-rw-r--r--   0        0        0     2855 2024-04-06 09:26:04.140433 causadb-1.8.2/causadb/cli/account.py
+-rw-r--r--   0        0        0     3116 2024-04-06 09:26:04.140433 causadb-1.8.2/causadb/cli/data.py
+-rwxr-xr-x   0        0        0      962 2024-04-06 09:26:04.140433 causadb-1.8.2/causadb/cli/main.py
+-rw-r--r--   0        0        0     7085 2024-04-06 09:26:04.140433 causadb-1.8.2/causadb/cli/models.py
+-rw-r--r--   0        0        0      891 2024-04-06 09:26:04.140433 causadb-1.8.2/causadb/cli/utils.py
+-rw-r--r--   0        0        0     2646 2024-04-06 09:26:04.140433 causadb-1.8.2/causadb/data.py
+-rw-r--r--   0        0        0        0 2024-04-06 09:26:04.140433 causadb-1.8.2/causadb/examples/__init__.py
+-rw-r--r--   0        0        0     1876 2024-04-06 09:26:04.140433 causadb-1.8.2/causadb/examples/heating.py
+-rw-r--r--   0        0        0    15066 2024-04-06 09:26:04.140433 causadb-1.8.2/causadb/model.py
+-rw-r--r--   0        0        0     2555 2024-04-06 09:26:04.140433 causadb-1.8.2/causadb/plotting.py
+-rw-r--r--   0        0        0      215 2024-04-06 09:26:04.140433 causadb-1.8.2/causadb/utils.py
+-rw-r--r--   0        0        0      797 2024-04-06 09:26:35.452285 causadb-1.8.2/pyproject.toml
+-rw-r--r--   0        0        0     1656 1970-01-01 00:00:00.000000 causadb-1.8.2/PKG-INFO
```

### Comparing `causadb-1.8.1/README.md` & `causadb-1.8.2/README.md`

 * *Files identical despite different names*

### Comparing `causadb-1.8.1/causadb/causadb.py` & `causadb-1.8.2/causadb/causadb.py`

 * *Files identical despite different names*

### Comparing `causadb-1.8.1/causadb/cli/account.py` & `causadb-1.8.2/causadb/cli/account.py`

 * *Files identical despite different names*

### Comparing `causadb-1.8.1/causadb/cli/data.py` & `causadb-1.8.2/causadb/cli/data.py`

 * *Files identical despite different names*

### Comparing `causadb-1.8.1/causadb/cli/main.py` & `causadb-1.8.2/causadb/cli/main.py`

 * *Files identical despite different names*

### Comparing `causadb-1.8.1/causadb/cli/models.py` & `causadb-1.8.2/causadb/cli/models.py`

 * *Files identical despite different names*

### Comparing `causadb-1.8.1/causadb/cli/utils.py` & `causadb-1.8.2/causadb/cli/utils.py`

 * *Files identical despite different names*

### Comparing `causadb-1.8.1/causadb/data.py` & `causadb-1.8.2/causadb/data.py`

 * *Files identical despite different names*

### Comparing `causadb-1.8.1/causadb/examples/heating.py` & `causadb-1.8.2/causadb/examples/heating.py`

 * *Files identical despite different names*

### Comparing `causadb-1.8.1/causadb/model.py` & `causadb-1.8.2/causadb/model.py`

 * *Files identical despite different names*

### Comparing `causadb-1.8.1/causadb/plotting.py` & `causadb-1.8.2/causadb/plotting.py`

 * *Files identical despite different names*

### Comparing `causadb-1.8.1/pyproject.toml` & `causadb-1.8.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "causadb"
-version = "1.8.1"
+version = "1.8.2"
 description = ""
 authors = ["Jordan hart <jordan@causa.tech>"]
 readme = "README.md"
 packages = [
     { include = "causadb", from = "." }
 ]
```

### Comparing `causadb-1.8.1/PKG-INFO` & `causadb-1.8.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: causadb
-Version: 1.8.1
+Version: 1.8.2
 Summary: 
 Author: Jordan hart
 Author-email: jordan@causa.tech
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

