# Comparing `tmp/systemslink_python-0.1.0.tar.gz` & `tmp/systemslink_python-0.1.1.tar.gz`

## Comparing `systemslink_python-0.1.0.tar` & `systemslink_python-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 systemslink_python-0.1.0/requirements.txt
--rw-r--r--   0        0        0    19507 2020-02-02 00:00:00.000000 systemslink_python-0.1.0/src/systemslink_python/__init__.py
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 systemslink_python-0.1.0/.gitignore
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 systemslink_python-0.1.0/LICENCE
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 systemslink_python-0.1.0/README.md
--rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 systemslink_python-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1315 2020-02-02 00:00:00.000000 systemslink_python-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 systemslink_python-0.1.1/.gitlab-ci.yml
+-rw-r--r--   0        0        0    19507 2020-02-02 00:00:00.000000 systemslink_python-0.1.1/src/systemslink_python/__init__.py
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 systemslink_python-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 systemslink_python-0.1.1/LICENCE
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 systemslink_python-0.1.1/README.md
+-rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 systemslink_python-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1363 2020-02-02 00:00:00.000000 systemslink_python-0.1.1/PKG-INFO
```

### Comparing `systemslink_python-0.1.0/src/systemslink_python/__init__.py` & `systemslink_python-0.1.1/src/systemslink_python/__init__.py`

 * *Files identical despite different names*

### Comparing `systemslink_python-0.1.0/LICENCE` & `systemslink_python-0.1.1/LICENCE`

 * *Files identical despite different names*

### Comparing `systemslink_python-0.1.0/README.md` & `systemslink_python-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `systemslink_python-0.1.0/PKG-INFO` & `systemslink_python-0.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Metadata-Version: 2.3
 Name: systemslink_python
-Version: 0.1.0
+Version: 0.1.1
 Summary: A small python interface for interacting with a SystemsLink energy management system.
 Project-URL: Homepage, https://gitlab.com/Lime-Parallelogram/systemslink-python
 Project-URL: Issues, https://gitlab.com/Lime-Parallelogram/systemslink-python/-/issues
 Author-email: Will Hall <public.me@limeparallelogram.uk>
 License-File: LICENCE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
+Requires-Dist: openpyxl
+Requires-Dist: requests
 Description-Content-Type: text/markdown
 
 # SystemsLink Energy Manager Data Scraper
 
 This project aims to provide a Python library capable of retrieving data from an instance of SystemsLink Energy Manager.
 
 > ⚠️ Please note: To my knowledge, the SystemsLink energy monitoring platform does not offer any public APIs from which data can be retrieved. Instead, this system will step through the standard authentication and requests procedure as would be used by a normal user accessing the webpage.
```

