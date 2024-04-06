# Comparing `tmp/dspin-1.0.7.tar.gz` & `tmp/dspin-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dspin-1.0.7.tar", last modified: Fri Mar 22 22:21:06 2024, max compression
+gzip compressed data, was "dspin-1.0.8.tar", last modified: Sat Apr  6 04:46:44 2024, max compression
```

## Comparing `dspin-1.0.7.tar` & `dspin-1.0.8.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2024-03-22 22:21:06.832354 dspin-1.0.7/
--rw-rw-rw-   0        0        0    11558 2023-12-28 23:40:19.000000 dspin-1.0.7/LICENSE
--rw-rw-rw-   0        0        0     2094 2024-03-22 22:21:06.829365 dspin-1.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     9808 2024-03-21 19:38:11.000000 dspin-1.0.7/README.md
-drwxrwxrwx   0        0        0        0 2024-03-22 22:21:06.771516 dspin-1.0.7/__pycache__/
--rw-rw-rw-   0        0        0      181 2023-12-28 23:40:19.000000 dspin-1.0.7/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0      133 2023-12-28 23:40:19.000000 dspin-1.0.7/__pycache__/__init__.cpython-37.pyc
--rw-rw-rw-   0        0        0    17966 2023-12-28 23:40:19.000000 dspin-1.0.7/__pycache__/compute.cpython-310.pyc
--rw-rw-rw-   0        0        0    17814 2023-12-28 23:40:19.000000 dspin-1.0.7/__pycache__/compute.cpython-37.pyc
--rw-rw-rw-   0        0        0    21671 2023-12-28 23:40:19.000000 dspin-1.0.7/__pycache__/dspin_abstract.cpython-310.pyc
--rw-rw-rw-   0        0        0    11846 2023-12-28 23:40:19.000000 dspin-1.0.7/__pycache__/plot.cpython-310.pyc
--rw-rw-rw-   0        0        0     9083 2023-12-28 23:40:19.000000 dspin-1.0.7/__pycache__/plotting.cpython-37.pyc
-drwxrwxrwx   0        0        0        0 2024-03-22 22:21:06.796452 dspin-1.0.7/dspin/
--rw-rw-rw-   0        0        0        0 2023-12-28 23:40:19.000000 dspin-1.0.7/dspin/__init__.py
--rw-rw-rw-   0        0        0    31240 2024-03-20 23:38:01.000000 dspin-1.0.7/dspin/compute.py
--rw-rw-rw-   0        0        0    31521 2024-03-22 17:23:37.000000 dspin-1.0.7/dspin/dspin.py
--rw-rw-rw-   0        0        0     3305 2024-03-20 22:26:00.000000 dspin-1.0.7/dspin/gpt.py
--rw-rw-rw-   0        0        0    19795 2024-03-22 22:19:25.000000 dspin-1.0.7/dspin/plot.py
-drwxrwxrwx   0        0        0        0 2024-03-22 22:21:06.827369 dspin-1.0.7/dspin.egg-info/
--rw-rw-rw-   0        0        0     2094 2024-03-22 22:21:06.000000 dspin-1.0.7/dspin.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      520 2024-03-22 22:21:06.000000 dspin-1.0.7/dspin.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-22 22:21:06.000000 dspin-1.0.7/dspin.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2024-03-22 22:21:06.000000 dspin-1.0.7/dspin.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-03-22 22:21:06.000000 dspin-1.0.7/dspin.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       52 2023-12-29 05:28:40.000000 dspin-1.0.7/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-03-22 22:21:06.832354 dspin-1.0.7/setup.cfg
--rw-rw-rw-   0        0        0     2237 2024-03-22 22:20:59.000000 dspin-1.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-06 04:46:44.667016 dspin-1.0.8/
+-rw-rw-rw-   0        0        0    11558 2023-12-28 23:40:19.000000 dspin-1.0.8/LICENSE
+-rw-rw-rw-   0        0        0     2094 2024-04-06 04:46:44.665022 dspin-1.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     9808 2024-03-21 19:38:11.000000 dspin-1.0.8/README.md
+drwxrwxrwx   0        0        0        0 2024-04-06 04:46:44.616151 dspin-1.0.8/__pycache__/
+-rw-rw-rw-   0        0        0      181 2023-12-28 23:40:19.000000 dspin-1.0.8/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0      133 2023-12-28 23:40:19.000000 dspin-1.0.8/__pycache__/__init__.cpython-37.pyc
+-rw-rw-rw-   0        0        0    17966 2023-12-28 23:40:19.000000 dspin-1.0.8/__pycache__/compute.cpython-310.pyc
+-rw-rw-rw-   0        0        0    17814 2023-12-28 23:40:19.000000 dspin-1.0.8/__pycache__/compute.cpython-37.pyc
+-rw-rw-rw-   0        0        0    21671 2023-12-28 23:40:19.000000 dspin-1.0.8/__pycache__/dspin_abstract.cpython-310.pyc
+-rw-rw-rw-   0        0        0    11846 2023-12-28 23:40:19.000000 dspin-1.0.8/__pycache__/plot.cpython-310.pyc
+-rw-rw-rw-   0        0        0     9083 2023-12-28 23:40:19.000000 dspin-1.0.8/__pycache__/plotting.cpython-37.pyc
+drwxrwxrwx   0        0        0        0 2024-04-06 04:46:44.622135 dspin-1.0.8/dspin/
+-rw-rw-rw-   0        0        0        0 2023-12-28 23:40:19.000000 dspin-1.0.8/dspin/__init__.py
+-rw-rw-rw-   0        0        0    18361 2024-04-06 00:50:53.000000 dspin-1.0.8/dspin/annotate.py
+-rw-rw-rw-   0        0        0    31240 2024-03-20 23:38:01.000000 dspin-1.0.8/dspin/compute.py
+-rw-rw-rw-   0        0        0    31521 2024-03-22 17:23:37.000000 dspin-1.0.8/dspin/dspin.py
+-rw-rw-rw-   0        0        0    19795 2024-03-22 22:19:25.000000 dspin-1.0.8/dspin/plot.py
+drwxrwxrwx   0        0        0        0 2024-04-06 04:46:44.664023 dspin-1.0.8/dspin.egg-info/
+-rw-rw-rw-   0        0        0     2094 2024-04-06 04:46:44.000000 dspin-1.0.8/dspin.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      525 2024-04-06 04:46:44.000000 dspin-1.0.8/dspin.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-06 04:46:44.000000 dspin-1.0.8/dspin.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2024-04-06 04:46:44.000000 dspin-1.0.8/dspin.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-04-06 04:46:44.000000 dspin-1.0.8/dspin.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       52 2023-12-29 05:28:40.000000 dspin-1.0.8/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-04-06 04:46:44.667016 dspin-1.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     2237 2024-04-06 04:46:16.000000 dspin-1.0.8/setup.py
```

### Comparing `dspin-1.0.7/LICENSE` & `dspin-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `dspin-1.0.7/PKG-INFO` & `dspin-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dspin
-Version: 1.0.7
+Version: 1.0.8
 Summary: Regulatory network models from single-cell perturbation profiling
 Home-page: https://github.com/JialongJiang/DSPIN
 Author: Jialong Jiang
 Author-email: jiangjl@caltech.edu
 License: Apache-2.0 license
 Keywords: network inference,single cell,transcriptomics
 Classifier: Development Status :: 4 - Beta
```

### Comparing `dspin-1.0.7/README.md` & `dspin-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `dspin-1.0.7/__pycache__/compute.cpython-310.pyc` & `dspin-1.0.8/__pycache__/compute.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `dspin-1.0.7/__pycache__/compute.cpython-37.pyc` & `dspin-1.0.8/__pycache__/compute.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `dspin-1.0.7/__pycache__/dspin_abstract.cpython-310.pyc` & `dspin-1.0.8/__pycache__/dspin_abstract.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `dspin-1.0.7/__pycache__/plot.cpython-310.pyc` & `dspin-1.0.8/__pycache__/plot.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `dspin-1.0.7/__pycache__/plotting.cpython-37.pyc` & `dspin-1.0.8/__pycache__/plotting.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `dspin-1.0.7/dspin/compute.py` & `dspin-1.0.8/dspin/compute.py`

 * *Files identical despite different names*

### Comparing `dspin-1.0.7/dspin/dspin.py` & `dspin-1.0.8/dspin/dspin.py`

 * *Files identical despite different names*

### Comparing `dspin-1.0.7/dspin/plot.py` & `dspin-1.0.8/dspin/plot.py`

 * *Files identical despite different names*

### Comparing `dspin-1.0.7/dspin.egg-info/PKG-INFO` & `dspin-1.0.8/dspin.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dspin
-Version: 1.0.7
+Version: 1.0.8
 Summary: Regulatory network models from single-cell perturbation profiling
 Home-page: https://github.com/JialongJiang/DSPIN
 Author: Jialong Jiang
 Author-email: jiangjl@caltech.edu
 License: Apache-2.0 license
 Keywords: network inference,single cell,transcriptomics
 Classifier: Development Status :: 4 - Beta
```

### Comparing `dspin-1.0.7/dspin.egg-info/SOURCES.txt` & `dspin-1.0.8/dspin.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 __pycache__/__init__.cpython-37.pyc
 __pycache__/compute.cpython-310.pyc
 __pycache__/compute.cpython-37.pyc
 __pycache__/dspin_abstract.cpython-310.pyc
 __pycache__/plot.cpython-310.pyc
 __pycache__/plotting.cpython-37.pyc
 dspin/__init__.py
+dspin/annotate.py
 dspin/compute.py
 dspin/dspin.py
-dspin/gpt.py
 dspin/plot.py
 dspin.egg-info/PKG-INFO
 dspin.egg-info/SOURCES.txt
 dspin.egg-info/dependency_links.txt
 dspin.egg-info/requires.txt
 dspin.egg-info/top_level.txt
```

### Comparing `dspin-1.0.7/setup.py` & `dspin-1.0.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 # # Replace with your package's documentation requirements
 # doc_requires = [
 #     # Example: "sphinx"
 # ]
 
 # Managing your version (adjust accordingly)
-version = "1.0.7"  # You can manage versioning in a more sophisticated way if needed
+version = "1.0.8"  # You can manage versioning in a more sophisticated way if needed
 
 # Long description (usually a README file)
 readme = open("README_PyPI.md").read()  # Adjust the file name if necessary
 
 setup(
     name="dspin",
     version=version,
```

