# Comparing `tmp/pyrasp-0.6.0.1.tar.gz` & `tmp/pyrasp-0.6.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrasp-0.6.0.1.tar", last modified: Fri Apr  5 16:29:00 2024, max compression
+gzip compressed data, was "pyrasp-0.6.0.2.tar", last modified: Fri Apr  5 16:44:02 2024, max compression
```

## Comparing `pyrasp-0.6.0.1.tar` & `pyrasp-0.6.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-04-05 16:29:00.704992 pyrasp-0.6.0.1/
--rw-rw-rw-   0        0        0    35823 2024-04-05 16:28:55.000000 pyrasp-0.6.0.1/LICENSE
--rw-rw-rw-   0        0        0    71889 2024-04-05 16:29:00.703377 pyrasp-0.6.0.1/PKG-INFO
--rw-rw-rw-   0        0        0    29958 2024-04-05 16:28:55.000000 pyrasp-0.6.0.1/README.md
--rw-rw-rw-   0        0        0      770 2024-04-05 16:28:55.000000 pyrasp-0.6.0.1/pyproject.toml
-drwxrwxrwx   0        0        0        0 2024-04-05 16:29:00.686687 pyrasp-0.6.0.1/pyrasp/
--rw-rw-rw-   0        0        0        0 2024-04-05 16:28:55.000000 pyrasp-0.6.0.1/pyrasp/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-05 16:29:00.698126 pyrasp-0.6.0.1/pyrasp/data/
--rw-rw-rw-   0        0        0   402447 2024-04-05 16:28:55.000000 pyrasp-0.6.0.1/pyrasp/data/sqli_model-1.0.0
--rw-rw-rw-   0        0        0  1047682 2024-04-05 16:28:55.000000 pyrasp-0.6.0.1/pyrasp/data/xss_model-1.1.0
--rw-rw-rw-   0        0        0    75220 2024-04-05 16:28:55.000000 pyrasp-0.6.0.1/pyrasp/pyrasp.py
--rw-rw-rw-   0        0        0     5254 2024-04-05 16:28:55.000000 pyrasp-0.6.0.1/pyrasp/pyrasp_data.py
-drwxrwxrwx   0        0        0        0 2024-04-05 16:29:00.701273 pyrasp-0.6.0.1/pyrasp.egg-info/
--rw-rw-rw-   0        0        0    71889 2024-04-05 16:29:00.000000 pyrasp-0.6.0.1/pyrasp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      296 2024-04-05 16:29:00.000000 pyrasp-0.6.0.1/pyrasp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 16:29:00.000000 pyrasp-0.6.0.1/pyrasp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2024-04-05 16:29:00.000000 pyrasp-0.6.0.1/pyrasp.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-05 16:29:00.000000 pyrasp-0.6.0.1/pyrasp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-05 16:29:00.705526 pyrasp-0.6.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-05 16:44:02.579819 pyrasp-0.6.0.2/
+-rw-rw-rw-   0        0        0    35823 2024-04-05 16:43:57.000000 pyrasp-0.6.0.2/LICENSE
+-rw-rw-rw-   0        0        0    71889 2024-04-05 16:44:02.578817 pyrasp-0.6.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0    29958 2024-04-05 16:43:57.000000 pyrasp-0.6.0.2/README.md
+-rw-rw-rw-   0        0        0      770 2024-04-05 16:43:57.000000 pyrasp-0.6.0.2/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-04-05 16:44:02.563367 pyrasp-0.6.0.2/pyrasp/
+-rw-rw-rw-   0        0        0        0 2024-04-05 16:43:57.000000 pyrasp-0.6.0.2/pyrasp/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-05 16:44:02.573125 pyrasp-0.6.0.2/pyrasp/data/
+-rw-rw-rw-   0        0        0   402447 2024-04-05 16:43:57.000000 pyrasp-0.6.0.2/pyrasp/data/sqli_model-1.0.0
+-rw-rw-rw-   0        0        0  1047682 2024-04-05 16:43:57.000000 pyrasp-0.6.0.2/pyrasp/data/xss_model-1.1.0
+-rw-rw-rw-   0        0        0    75220 2024-04-05 16:43:57.000000 pyrasp-0.6.0.2/pyrasp/pyrasp.py
+-rw-rw-rw-   0        0        0     5254 2024-04-05 16:43:57.000000 pyrasp-0.6.0.2/pyrasp/pyrasp_data.py
+drwxrwxrwx   0        0        0        0 2024-04-05 16:44:02.576819 pyrasp-0.6.0.2/pyrasp.egg-info/
+-rw-rw-rw-   0        0        0    71889 2024-04-05 16:44:02.000000 pyrasp-0.6.0.2/pyrasp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      296 2024-04-05 16:44:02.000000 pyrasp-0.6.0.2/pyrasp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 16:44:02.000000 pyrasp-0.6.0.2/pyrasp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2024-04-05 16:44:02.000000 pyrasp-0.6.0.2/pyrasp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-05 16:44:02.000000 pyrasp-0.6.0.2/pyrasp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-05 16:44:02.579819 pyrasp-0.6.0.2/setup.cfg
```

### Comparing `pyrasp-0.6.0.1/LICENSE` & `pyrasp-0.6.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrasp-0.6.0.1/PKG-INFO` & `pyrasp-0.6.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrasp
-Version: 0.6.0.1
+Version: 0.6.0.2
 Summary: Python RASP
 Author-email: Renaud Bidou <renaud@paracyberbellum.io>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `pyrasp-0.6.0.1/README.md` & `pyrasp-0.6.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pyrasp-0.6.0.1/pyproject.toml` & `pyrasp-0.6.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pyrasp"
-version = "0.6.0.1"
+version = "0.6.0.2"
 authors = [
     { name = "Renaud Bidou", email = "renaud@paracyberbellum.io" }
 ]
 description = "Python RASP"
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.7"
```

### Comparing `pyrasp-0.6.0.1/pyrasp/data/sqli_model-1.0.0` & `pyrasp-0.6.0.2/pyrasp/data/sqli_model-1.0.0`

 * *Files identical despite different names*

### Comparing `pyrasp-0.6.0.1/pyrasp/data/xss_model-1.1.0` & `pyrasp-0.6.0.2/pyrasp/data/xss_model-1.1.0`

 * *Files identical despite different names*

### Comparing `pyrasp-0.6.0.1/pyrasp/pyrasp.py` & `pyrasp-0.6.0.2/pyrasp/pyrasp.py`

 * *Files identical despite different names*

### Comparing `pyrasp-0.6.0.1/pyrasp/pyrasp_data.py` & `pyrasp-0.6.0.2/pyrasp/pyrasp_data.py`

 * *Files identical despite different names*

### Comparing `pyrasp-0.6.0.1/pyrasp.egg-info/PKG-INFO` & `pyrasp-0.6.0.2/pyrasp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrasp
-Version: 0.6.0.1
+Version: 0.6.0.2
 Summary: Python RASP
 Author-email: Renaud Bidou <renaud@paracyberbellum.io>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

