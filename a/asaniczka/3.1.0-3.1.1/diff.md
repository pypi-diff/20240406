# Comparing `tmp/asaniczka-3.1.0.tar.gz` & `tmp/asaniczka-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asaniczka-3.1.0.tar", last modified: Sat Apr  6 08:03:05 2024, max compression
+gzip compressed data, was "asaniczka-3.1.1.tar", last modified: Sat Apr  6 08:10:19 2024, max compression
```

## Comparing `asaniczka-3.1.0.tar` & `asaniczka-3.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 08:03:05.365508 asaniczka-3.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-04-06 08:03:05.365508 asaniczka-3.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-04-06 08:03:00.000000 asaniczka-3.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 08:03:05.365508 asaniczka-3.1.0/asaniczka/
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-06 08:03:00.000000 asaniczka-3.1.0/asaniczka/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24084 2024-04-06 08:03:00.000000 asaniczka-3.1.0/asaniczka/db_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)    33999 2024-04-06 08:03:00.000000 asaniczka-3.1.0/asaniczka/main.py
--rw-r--r--   0 runner    (1001) docker     (127)    14041 2024-04-06 08:03:00.000000 asaniczka-3.1.0/asaniczka/scrape_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 08:03:05.365508 asaniczka-3.1.0/asaniczka.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-04-06 08:03:05.000000 asaniczka-3.1.0/asaniczka.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-06 08:03:05.000000 asaniczka-3.1.0/asaniczka.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 08:03:05.000000 asaniczka-3.1.0/asaniczka.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-06 08:03:05.000000 asaniczka-3.1.0/asaniczka.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-06 08:03:05.000000 asaniczka-3.1.0/asaniczka.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-04-06 08:03:00.000000 asaniczka-3.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 08:03:05.365508 asaniczka-3.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 08:10:19.187154 asaniczka-3.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-04-06 08:10:19.187154 asaniczka-3.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-04-06 08:10:10.000000 asaniczka-3.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 08:10:19.187154 asaniczka-3.1.1/asaniczka/
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-06 08:10:10.000000 asaniczka-3.1.1/asaniczka/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24084 2024-04-06 08:10:10.000000 asaniczka-3.1.1/asaniczka/db_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33999 2024-04-06 08:10:10.000000 asaniczka-3.1.1/asaniczka/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14068 2024-04-06 08:10:10.000000 asaniczka-3.1.1/asaniczka/scrape_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 08:10:19.187154 asaniczka-3.1.1/asaniczka.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-04-06 08:10:19.000000 asaniczka-3.1.1/asaniczka.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-06 08:10:19.000000 asaniczka-3.1.1/asaniczka.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 08:10:19.000000 asaniczka-3.1.1/asaniczka.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-06 08:10:19.000000 asaniczka-3.1.1/asaniczka.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-06 08:10:19.000000 asaniczka-3.1.1/asaniczka.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-04-06 08:10:10.000000 asaniczka-3.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 08:10:19.187154 asaniczka-3.1.1/setup.cfg
```

### Comparing `asaniczka-3.1.0/PKG-INFO` & `asaniczka-3.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asaniczka
-Version: 3.1.0
+Version: 3.1.1
 Summary: All my commonly used fuctions
 Author-email: Asaniczka <asaniczka@gmail.com>
 Maintainer-email: Asaniczka <asaniczka@gmail.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/asaniczka/asaniczka_pip
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `asaniczka-3.1.0/README.md` & `asaniczka-3.1.1/README.md`

 * *Files identical despite different names*

### Comparing `asaniczka-3.1.0/asaniczka/db_tools.py` & `asaniczka-3.1.1/asaniczka/db_tools.py`

 * *Files identical despite different names*

### Comparing `asaniczka-3.1.0/asaniczka/main.py` & `asaniczka-3.1.1/asaniczka/main.py`

 * *Files identical despite different names*

### Comparing `asaniczka-3.1.0/asaniczka/scrape_helper.py` & `asaniczka-3.1.1/asaniczka/scrape_helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -443,7 +443,8 @@
 
     lines = response.split("\n")
     lines = [line.strip() for line in lines]
     proxies = [Proxy(line, ProxyProvider.WEBSHARE) for line in lines]
 
     working_proxies = validate_proxies(proxies)
     print("You have ", len(working_proxies), " working proxies!")
+    return working_proxies
```

### Comparing `asaniczka-3.1.0/asaniczka.egg-info/PKG-INFO` & `asaniczka-3.1.1/asaniczka.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asaniczka
-Version: 3.1.0
+Version: 3.1.1
 Summary: All my commonly used fuctions
 Author-email: Asaniczka <asaniczka@gmail.com>
 Maintainer-email: Asaniczka <asaniczka@gmail.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/asaniczka/asaniczka_pip
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `asaniczka-3.1.0/pyproject.toml` & `asaniczka-3.1.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ['setuptools >= 61.0', 'wheel']
 build-backend = 'setuptools.build_meta'
 
 [project]
 name = "asaniczka"
-version = "3.1.0"
+version = "3.1.1"
 description = "All my commonly used fuctions"
 readme = "README.md"
 dependencies = [
   "pytz>=2022.1",
   "requests>=2.0",
   "playwright>=1.0.0",
   "tqdm>=4.0.0",
```

