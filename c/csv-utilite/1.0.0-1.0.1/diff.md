# Comparing `tmp/csv_utilite-1.0.0.tar.gz` & `tmp/csv_utilite-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csv_utilite-1.0.0.tar", last modified: Fri Apr  5 17:40:29 2024, max compression
+gzip compressed data, was "csv_utilite-1.0.1.tar", last modified: Sat Apr  6 21:52:31 2024, max compression
```

## Comparing `csv_utilite-1.0.0.tar` & `csv_utilite-1.0.1.tar`

### file list

```diff
@@ -1,29 +1,28 @@
-drwxrwxrwx   0        0        0        0 2024-04-05 17:40:29.531529 csv_utilite-1.0.0/
--rw-rw-rw-   0        0        0    11558 2024-03-25 15:12:02.000000 csv_utilite-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     7858 2024-04-05 17:40:29.525527 csv_utilite-1.0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-05 17:40:29.459368 csv_utilite-1.0.0/csv_utilite/
--rw-rw-rw-   0        0        0      355 2024-03-31 11:21:28.000000 csv_utilite-1.0.0/csv_utilite/__init__.py
--rw-rw-rw-   0        0        0     3118 2024-03-25 13:06:43.000000 csv_utilite-1.0.0/csv_utilite/conversion.py
--rw-rw-rw-   0        0        0     2573 2024-03-24 19:51:21.000000 csv_utilite-1.0.0/csv_utilite/formating.py
--rw-rw-rw-   0        0        0     2488 2024-03-25 13:26:03.000000 csv_utilite-1.0.0/csv_utilite/generation.py
--rw-rw-rw-   0        0        0     3050 2024-03-24 17:26:03.000000 csv_utilite-1.0.0/csv_utilite/manipulation.py
--rw-rw-rw-   0        0        0     2638 2024-03-23 14:50:06.000000 csv_utilite-1.0.0/csv_utilite/reader.py
--rw-rw-rw-   0        0        0     1962 2024-03-25 12:29:30.000000 csv_utilite-1.0.0/csv_utilite/validation.py
--rw-rw-rw-   0        0        0     2338 2024-03-24 17:19:25.000000 csv_utilite-1.0.0/csv_utilite/writer.py
-drwxrwxrwx   0        0        0        0 2024-04-05 17:40:29.483366 csv_utilite-1.0.0/csv_utilite.egg-info/
--rw-rw-rw-   0        0        0     7858 2024-04-05 17:40:29.000000 csv_utilite-1.0.0/csv_utilite.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      548 2024-04-05 17:40:29.000000 csv_utilite-1.0.0/csv_utilite.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 17:40:29.000000 csv_utilite-1.0.0/csv_utilite.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-04-05 17:40:29.000000 csv_utilite-1.0.0/csv_utilite.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-04-05 17:38:18.000000 csv_utilite-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-05 17:40:29.532528 csv_utilite-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      999 2024-04-05 17:40:02.000000 csv_utilite-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-05 17:40:29.515363 csv_utilite-1.0.0/test/
--rw-rw-rw-   0        0        0        0 2024-03-23 14:34:00.000000 csv_utilite-1.0.0/test/__init__.py
--rw-rw-rw-   0        0        0     2541 2024-04-05 17:39:51.000000 csv_utilite-1.0.0/test/test_conversion.py
--rw-rw-rw-   0        0        0     1867 2024-04-05 17:39:38.000000 csv_utilite-1.0.0/test/test_formating.py
--rw-rw-rw-   0        0        0     2724 2024-04-05 17:38:21.000000 csv_utilite-1.0.0/test/test_generation.py
--rw-rw-rw-   0        0        0     2063 2024-04-05 17:38:21.000000 csv_utilite-1.0.0/test/test_manipulation.py
--rw-rw-rw-   0        0        0     4197 2024-04-05 17:38:21.000000 csv_utilite-1.0.0/test/test_reader.py
--rw-rw-rw-   0        0        0     1787 2024-04-05 17:38:21.000000 csv_utilite-1.0.0/test/test_validation.py
--rw-rw-rw-   0        0        0     3972 2024-04-05 17:38:21.000000 csv_utilite-1.0.0/test/test_writer.py
+drwxrwxrwx   0        0        0        0 2024-04-06 21:52:31.943904 csv_utilite-1.0.1/
+-rw-rw-rw-   0        0        0    11558 2024-03-25 15:12:02.000000 csv_utilite-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0     7158 2024-04-06 21:52:31.943904 csv_utilite-1.0.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-06 21:52:31.860559 csv_utilite-1.0.1/csv_utilite/
+-rw-rw-rw-   0        0        0      355 2024-03-31 11:21:28.000000 csv_utilite-1.0.1/csv_utilite/__init__.py
+-rw-rw-rw-   0        0        0     3118 2024-03-25 13:06:43.000000 csv_utilite-1.0.1/csv_utilite/conversion.py
+-rw-rw-rw-   0        0        0     2573 2024-03-24 19:51:21.000000 csv_utilite-1.0.1/csv_utilite/formating.py
+-rw-rw-rw-   0        0        0     2488 2024-03-25 13:26:03.000000 csv_utilite-1.0.1/csv_utilite/generation.py
+-rw-rw-rw-   0        0        0     3050 2024-03-24 17:26:03.000000 csv_utilite-1.0.1/csv_utilite/manipulation.py
+-rw-rw-rw-   0        0        0     2638 2024-03-23 14:50:06.000000 csv_utilite-1.0.1/csv_utilite/reader.py
+-rw-rw-rw-   0        0        0     1962 2024-03-25 12:29:30.000000 csv_utilite-1.0.1/csv_utilite/validation.py
+-rw-rw-rw-   0        0        0     2338 2024-03-24 17:19:25.000000 csv_utilite-1.0.1/csv_utilite/writer.py
+drwxrwxrwx   0        0        0        0 2024-04-06 21:52:31.877324 csv_utilite-1.0.1/csv_utilite.egg-info/
+-rw-rw-rw-   0        0        0     7158 2024-04-06 21:52:31.000000 csv_utilite-1.0.1/csv_utilite.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      533 2024-04-06 21:52:31.000000 csv_utilite-1.0.1/csv_utilite.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-06 21:52:31.000000 csv_utilite-1.0.1/csv_utilite.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-04-06 21:52:31.000000 csv_utilite-1.0.1/csv_utilite.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-06 21:52:31.943904 csv_utilite-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      999 2024-04-06 21:44:31.000000 csv_utilite-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-06 21:52:31.927375 csv_utilite-1.0.1/test/
+-rw-rw-rw-   0        0        0        0 2024-03-23 14:34:00.000000 csv_utilite-1.0.1/test/__init__.py
+-rw-rw-rw-   0        0        0     2541 2024-04-05 17:39:51.000000 csv_utilite-1.0.1/test/test_conversion.py
+-rw-rw-rw-   0        0        0     1867 2024-04-05 17:39:38.000000 csv_utilite-1.0.1/test/test_formating.py
+-rw-rw-rw-   0        0        0     2724 2024-04-05 17:38:21.000000 csv_utilite-1.0.1/test/test_generation.py
+-rw-rw-rw-   0        0        0     2063 2024-04-05 17:38:21.000000 csv_utilite-1.0.1/test/test_manipulation.py
+-rw-rw-rw-   0        0        0     4197 2024-04-05 17:38:21.000000 csv_utilite-1.0.1/test/test_reader.py
+-rw-rw-rw-   0        0        0     1787 2024-04-05 17:38:21.000000 csv_utilite-1.0.1/test/test_validation.py
+-rw-rw-rw-   0        0        0     3972 2024-04-05 17:38:21.000000 csv_utilite-1.0.1/test/test_writer.py
```

### Comparing `csv_utilite-1.0.0/LICENSE` & `csv_utilite-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `csv_utilite-1.0.0/csv_utilite/conversion.py` & `csv_utilite-1.0.1/csv_utilite/conversion.py`

 * *Files identical despite different names*

### Comparing `csv_utilite-1.0.0/csv_utilite/formating.py` & `csv_utilite-1.0.1/csv_utilite/formating.py`

 * *Files identical despite different names*

### Comparing `csv_utilite-1.0.0/csv_utilite/generation.py` & `csv_utilite-1.0.1/csv_utilite/generation.py`

 * *Files identical despite different names*

### Comparing `csv_utilite-1.0.0/csv_utilite/manipulation.py` & `csv_utilite-1.0.1/csv_utilite/manipulation.py`

 * *Files identical despite different names*

### Comparing `csv_utilite-1.0.0/csv_utilite/reader.py` & `csv_utilite-1.0.1/csv_utilite/reader.py`

 * *Files identical despite different names*

### Comparing `csv_utilite-1.0.0/csv_utilite/validation.py` & `csv_utilite-1.0.1/csv_utilite/validation.py`

 * *Files identical despite different names*

### Comparing `csv_utilite-1.0.0/csv_utilite/writer.py` & `csv_utilite-1.0.1/csv_utilite/writer.py`

 * *Files identical despite different names*

### Comparing `csv_utilite-1.0.0/csv_utilite.egg-info/SOURCES.txt` & `csv_utilite-1.0.1/csv_utilite.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 LICENSE
-pyproject.toml
 setup.py
 csv_utilite/__init__.py
 csv_utilite/conversion.py
 csv_utilite/formating.py
 csv_utilite/generation.py
 csv_utilite/manipulation.py
 csv_utilite/reader.py
```

### Comparing `csv_utilite-1.0.0/setup.py` & `csv_utilite-1.0.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages 
 
 setup(
     name='csv_utilite',
-    version='1.0.0',
+    version='1.0.1',
     description='csv-util is a Python package designed to facilitate working with CSV files in a more convenient and Pythonic manner compared to the built-in csv module.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Khalil Habib Shariff',
     author_email='khaleelhabib@outlook.com',
     packages=find_packages(),
     install_requires=[
```

### Comparing `csv_utilite-1.0.0/test/test_conversion.py` & `csv_utilite-1.0.1/test/test_conversion.py`

 * *Files identical despite different names*

### Comparing `csv_utilite-1.0.0/test/test_formating.py` & `csv_utilite-1.0.1/test/test_formating.py`

 * *Files identical despite different names*

### Comparing `csv_utilite-1.0.0/test/test_generation.py` & `csv_utilite-1.0.1/test/test_generation.py`

 * *Files identical despite different names*

### Comparing `csv_utilite-1.0.0/test/test_manipulation.py` & `csv_utilite-1.0.1/test/test_manipulation.py`

 * *Files identical despite different names*

### Comparing `csv_utilite-1.0.0/test/test_reader.py` & `csv_utilite-1.0.1/test/test_reader.py`

 * *Files identical despite different names*

### Comparing `csv_utilite-1.0.0/test/test_validation.py` & `csv_utilite-1.0.1/test/test_validation.py`

 * *Files identical despite different names*

### Comparing `csv_utilite-1.0.0/test/test_writer.py` & `csv_utilite-1.0.1/test/test_writer.py`

 * *Files identical despite different names*

