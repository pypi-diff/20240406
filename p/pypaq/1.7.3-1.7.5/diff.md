# Comparing `tmp/pypaq-1.7.3.tar.gz` & `tmp/pypaq-1.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypaq-1.7.3.tar", last modified: Mon Mar 11 21:22:12 2024, max compression
+gzip compressed data, was "pypaq-1.7.5.tar", last modified: Sat Apr  6 18:28:17 2024, max compression
```

## Comparing `pypaq-1.7.3.tar` & `pypaq-1.7.5.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxr-x   0 pniewinski  (1000) pniewinski  (1000)        0 2024-03-11 21:22:12.597342 pypaq-1.7.3/
--rw-r--r--   0 pniewinski  (1000) pniewinski  (1000)      383 2024-03-11 21:22:12.597342 pypaq-1.7.3/PKG-INFO
--rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)      445 2023-10-10 21:57:36.000000 pypaq-1.7.3/README.md
-drwxrwxr-x   0 pniewinski  (1000) pniewinski  (1000)        0 2024-03-11 21:22:12.593342 pypaq-1.7.3/pypaq/
--rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)        0 2023-02-27 23:13:46.000000 pypaq-1.7.3/pypaq/__init__.py
--rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)       41 2023-03-09 20:19:41.000000 pypaq-1.7.3/pypaq/exception.py
-drwxrwxr-x   0 pniewinski  (1000) pniewinski  (1000)        0 2024-03-11 21:22:12.593342 pypaq-1.7.3/pypaq/lipytools/
--rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)        0 2023-02-27 23:13:46.000000 pypaq-1.7.3/pypaq/lipytools/__init__.py
--rwxrwxr-x   0 pniewinski  (1000) pniewinski  (1000)     4111 2023-03-10 11:50:02.000000 pypaq-1.7.3/pypaq/lipytools/decorators.py
--rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)      826 2023-03-24 23:09:04.000000 pypaq-1.7.3/pypaq/lipytools/double_hinge.py
--rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)     3442 2024-03-11 21:16:06.000000 pypaq-1.7.3/pypaq/lipytools/files.py
--rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)     1297 2023-11-02 21:40:01.000000 pypaq-1.7.3/pypaq/lipytools/moving_average.py
--rwxrwxr-x   0 pniewinski  (1000) pniewinski  (1000)     4908 2024-02-19 12:35:41.000000 pypaq-1.7.3/pypaq/lipytools/plots.py
--rwxrwxr-x   0 pniewinski  (1000) pniewinski  (1000)     3780 2023-11-10 11:27:16.000000 pypaq-1.7.3/pypaq/lipytools/printout.py
--rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)     2361 2024-02-06 21:33:57.000000 pypaq-1.7.3/pypaq/lipytools/pylogger.py
--rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)       73 2023-02-27 23:13:46.000000 pypaq-1.7.3/pypaq/lipytools/softmax.py
--rwxrwxr-x   0 pniewinski  (1000) pniewinski  (1000)      977 2023-03-26 08:26:06.000000 pypaq-1.7.3/pypaq/lipytools/stats.py
--rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)     1941 2024-02-13 14:18:37.000000 pypaq-1.7.3/pypaq/lipytools/time_reporter.py
-drwxrwxr-x   0 pniewinski  (1000) pniewinski  (1000)        0 2024-03-11 21:22:12.593342 pypaq-1.7.3/pypaq/mpython/
--rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)        0 2023-02-27 23:13:46.000000 pypaq-1.7.3/pypaq/mpython/__init__.py
--rwxrwxr-x   0 pniewinski  (1000) pniewinski  (1000)     1570 2023-12-02 23:28:46.000000 pypaq-1.7.3/pypaq/mpython/mpdecor.py
--rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)     5528 2024-02-24 11:44:59.000000 pypaq-1.7.3/pypaq/mpython/mptools.py
-drwxrwxr-x   0 pniewinski  (1000) pniewinski  (1000)        0 2024-03-11 21:22:12.597342 pypaq-1.7.3/pypaq/pms/
--rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)        0 2023-02-27 23:13:46.000000 pypaq-1.7.3/pypaq/pms/__init__.py
--rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)     4582 2024-02-03 12:35:45.000000 pypaq-1.7.3/pypaq/pms/base.py
--rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)     3651 2023-05-16 14:09:15.000000 pypaq-1.7.3/pypaq/pms/config_manager.py
--rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)     8354 2023-11-14 12:14:14.000000 pypaq-1.7.3/pypaq/pms/para.py
--rwxrwxr-x   0 pniewinski  (1000) pniewinski  (1000)    13853 2024-02-24 11:44:59.000000 pypaq-1.7.3/pypaq/pms/parasave.py
--rwxrwxr-x   0 pniewinski  (1000) pniewinski  (1000)    18707 2023-12-07 22:58:02.000000 pypaq-1.7.3/pypaq/pms/paspa.py
--rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)     6863 2023-12-08 19:16:36.000000 pypaq-1.7.3/pypaq/pms/points_cloud.py
--rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)      211 2024-02-10 12:18:01.000000 pypaq-1.7.3/pypaq/pytypes.py
-drwxrwxr-x   0 pniewinski  (1000) pniewinski  (1000)        0 2024-03-11 21:22:12.597342 pypaq-1.7.3/pypaq/textools/
--rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)        0 2023-02-27 23:13:46.000000 pypaq-1.7.3/pypaq/textools/__init__.py
--rwxrwxr-x   0 pniewinski  (1000) pniewinski  (1000)     1210 2023-02-27 23:13:46.000000 pypaq-1.7.3/pypaq/textools/text_metrics.py
--rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)      668 2023-12-29 14:42:47.000000 pypaq-1.7.3/pypaq/textools/text_processing.py
-drwxrwxr-x   0 pniewinski  (1000) pniewinski  (1000)        0 2024-03-11 21:22:12.593342 pypaq-1.7.3/pypaq.egg-info/
--rw-r--r--   0 pniewinski  (1000) pniewinski  (1000)      383 2024-03-11 21:22:12.000000 pypaq-1.7.3/pypaq.egg-info/PKG-INFO
--rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)      852 2024-03-11 21:22:12.000000 pypaq-1.7.3/pypaq.egg-info/SOURCES.txt
--rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)        1 2024-03-11 21:22:12.000000 pypaq-1.7.3/pypaq.egg-info/dependency_links.txt
--rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)       63 2024-03-11 21:22:12.000000 pypaq-1.7.3/pypaq.egg-info/requires.txt
--rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)        6 2024-03-11 21:22:12.000000 pypaq-1.7.3/pypaq.egg-info/top_level.txt
--rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)       38 2024-03-11 21:22:12.597342 pypaq-1.7.3/setup.cfg
--rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)      491 2024-03-11 21:22:11.000000 pypaq-1.7.3/setup.py
+drwxrwxr-x   0 ppp       (1000) ppp       (1000)        0 2024-04-06 18:28:17.451240 pypaq-1.7.5/
+-rw-r--r--   0 ppp       (1000) ppp       (1000)      383 2024-04-06 18:28:17.451240 pypaq-1.7.5/PKG-INFO
+-rw-rw-r--   0 ppp       (1000) ppp       (1000)      470 2024-04-06 17:44:30.000000 pypaq-1.7.5/README.md
+drwxrwxr-x   0 ppp       (1000) ppp       (1000)        0 2024-04-06 18:28:17.447240 pypaq-1.7.5/pypaq/
+-rw-rw-r--   0 ppp       (1000) ppp       (1000)        0 2024-04-06 17:44:30.000000 pypaq-1.7.5/pypaq/__init__.py
+-rw-rw-r--   0 ppp       (1000) ppp       (1000)       41 2024-04-06 17:44:30.000000 pypaq-1.7.5/pypaq/exception.py
+drwxrwxr-x   0 ppp       (1000) ppp       (1000)        0 2024-04-06 18:28:17.447240 pypaq-1.7.5/pypaq/lipytools/
+-rw-rw-r--   0 ppp       (1000) ppp       (1000)        0 2024-04-06 17:44:30.000000 pypaq-1.7.5/pypaq/lipytools/__init__.py
+-rwxrwxr-x   0 ppp       (1000) ppp       (1000)     4111 2024-04-06 17:44:30.000000 pypaq-1.7.5/pypaq/lipytools/decorators.py
+-rw-rw-r--   0 ppp       (1000) ppp       (1000)      826 2024-04-06 17:44:30.000000 pypaq-1.7.5/pypaq/lipytools/double_hinge.py
+-rw-rw-r--   0 ppp       (1000) ppp       (1000)     3934 2024-04-06 17:44:30.000000 pypaq-1.7.5/pypaq/lipytools/files.py
+-rw-rw-r--   0 ppp       (1000) ppp       (1000)     1297 2024-04-06 17:44:30.000000 pypaq-1.7.5/pypaq/lipytools/moving_average.py
+-rwxrwxr-x   0 ppp       (1000) ppp       (1000)     4908 2024-04-06 17:44:30.000000 pypaq-1.7.5/pypaq/lipytools/plots.py
+-rwxrwxr-x   0 ppp       (1000) ppp       (1000)     5783 2024-04-06 17:44:30.000000 pypaq-1.7.5/pypaq/lipytools/printout.py
+-rw-rw-r--   0 ppp       (1000) ppp       (1000)     2361 2024-04-06 17:44:30.000000 pypaq-1.7.5/pypaq/lipytools/pylogger.py
+-rw-rw-r--   0 ppp       (1000) ppp       (1000)       73 2024-04-06 17:44:30.000000 pypaq-1.7.5/pypaq/lipytools/softmax.py
+-rwxrwxr-x   0 ppp       (1000) ppp       (1000)      977 2024-04-06 17:44:30.000000 pypaq-1.7.5/pypaq/lipytools/stats.py
+-rw-rw-r--   0 ppp       (1000) ppp       (1000)     1941 2024-04-06 17:44:30.000000 pypaq-1.7.5/pypaq/lipytools/time_reporter.py
+drwxrwxr-x   0 ppp       (1000) ppp       (1000)        0 2024-04-06 18:28:17.447240 pypaq-1.7.5/pypaq/mpython/
+-rw-rw-r--   0 ppp       (1000) ppp       (1000)        0 2024-04-06 17:44:30.000000 pypaq-1.7.5/pypaq/mpython/__init__.py
+-rwxrwxr-x   0 ppp       (1000) ppp       (1000)     1570 2024-04-06 17:44:30.000000 pypaq-1.7.5/pypaq/mpython/mpdecor.py
+-rw-rw-r--   0 ppp       (1000) ppp       (1000)     5528 2024-04-06 17:44:30.000000 pypaq-1.7.5/pypaq/mpython/mptools.py
+drwxrwxr-x   0 ppp       (1000) ppp       (1000)        0 2024-04-06 18:28:17.447240 pypaq-1.7.5/pypaq/pms/
+-rw-rw-r--   0 ppp       (1000) ppp       (1000)        0 2024-04-06 17:44:30.000000 pypaq-1.7.5/pypaq/pms/__init__.py
+-rw-rw-r--   0 ppp       (1000) ppp       (1000)     4582 2024-04-06 17:44:30.000000 pypaq-1.7.5/pypaq/pms/base.py
+-rw-rw-r--   0 ppp       (1000) ppp       (1000)     3651 2024-04-06 17:44:30.000000 pypaq-1.7.5/pypaq/pms/config_manager.py
+-rw-rw-r--   0 ppp       (1000) ppp       (1000)     8354 2024-04-06 17:44:30.000000 pypaq-1.7.5/pypaq/pms/para.py
+-rwxrwxr-x   0 ppp       (1000) ppp       (1000)    13853 2024-04-06 17:44:30.000000 pypaq-1.7.5/pypaq/pms/parasave.py
+-rwxrwxr-x   0 ppp       (1000) ppp       (1000)    18707 2024-04-06 17:44:30.000000 pypaq-1.7.5/pypaq/pms/paspa.py
+-rw-rw-r--   0 ppp       (1000) ppp       (1000)     6863 2024-04-06 17:44:30.000000 pypaq-1.7.5/pypaq/pms/points_cloud.py
+-rw-rw-r--   0 ppp       (1000) ppp       (1000)      211 2024-04-06 17:44:30.000000 pypaq-1.7.5/pypaq/pytypes.py
+drwxrwxr-x   0 ppp       (1000) ppp       (1000)        0 2024-04-06 18:28:17.451240 pypaq-1.7.5/pypaq/textools/
+-rw-rw-r--   0 ppp       (1000) ppp       (1000)        0 2024-04-06 17:44:30.000000 pypaq-1.7.5/pypaq/textools/__init__.py
+-rwxrwxr-x   0 ppp       (1000) ppp       (1000)     1210 2024-04-06 17:44:30.000000 pypaq-1.7.5/pypaq/textools/text_metrics.py
+-rw-rw-r--   0 ppp       (1000) ppp       (1000)      668 2024-04-06 17:44:30.000000 pypaq-1.7.5/pypaq/textools/text_processing.py
+drwxrwxr-x   0 ppp       (1000) ppp       (1000)        0 2024-04-06 18:28:17.451240 pypaq-1.7.5/pypaq.egg-info/
+-rw-r--r--   0 ppp       (1000) ppp       (1000)      383 2024-04-06 18:28:17.000000 pypaq-1.7.5/pypaq.egg-info/PKG-INFO
+-rw-rw-r--   0 ppp       (1000) ppp       (1000)      852 2024-04-06 18:28:17.000000 pypaq-1.7.5/pypaq.egg-info/SOURCES.txt
+-rw-rw-r--   0 ppp       (1000) ppp       (1000)        1 2024-04-06 18:28:17.000000 pypaq-1.7.5/pypaq.egg-info/dependency_links.txt
+-rw-rw-r--   0 ppp       (1000) ppp       (1000)       63 2024-04-06 18:28:17.000000 pypaq-1.7.5/pypaq.egg-info/requires.txt
+-rw-rw-r--   0 ppp       (1000) ppp       (1000)        6 2024-04-06 18:28:17.000000 pypaq-1.7.5/pypaq.egg-info/top_level.txt
+-rw-rw-r--   0 ppp       (1000) ppp       (1000)       38 2024-04-06 18:28:17.451240 pypaq-1.7.5/setup.cfg
+-rw-rw-r--   0 ppp       (1000) ppp       (1000)      491 2024-04-06 18:22:30.000000 pypaq-1.7.5/setup.py
```

### Comparing `pypaq-1.7.3/pypaq/lipytools/decorators.py` & `pypaq-1.7.5/pypaq/lipytools/decorators.py`

 * *Files identical despite different names*

### Comparing `pypaq-1.7.3/pypaq/lipytools/double_hinge.py` & `pypaq-1.7.5/pypaq/lipytools/double_hinge.py`

 * *Files identical despite different names*

### Comparing `pypaq-1.7.3/pypaq/lipytools/files.py` & `pypaq-1.7.5/pypaq/lipytools/files.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,76 +7,95 @@
 from pathlib import Path
 import sys
 from typing import Union, Dict, List, Optional
 
 from pypaq.exception import PyPaqException
 
 
+def r_text(file_path:str, raise_exception=False) -> Optional[str]:
+    if not os.path.isfile(file_path):
+        if raise_exception:
+            raise FileNotFoundError(f'file {file_path} not exists!')
+        return None
+    with open(file_path, 'r', encoding='utf-8') as file:
+        return file.read()
+
+
+def w_text(text:str, file_path:str):
+    with open(file_path, 'w') as file:
+        return file.write(text)
+
+
 def r_pickle(file_path, obj_type=None, raise_exception=False):
     """ reads pickle
     if obj_type is given checks for compatibility with given type """
     if not os.path.isfile(file_path):
-        if raise_exception: raise FileNotFoundError(f'file {file_path} not exists!')
+        if raise_exception:
+            raise FileNotFoundError(f'file {file_path} not exists!')
         return None
 
-    # obj = pickle.load(open(file_path, 'rb')) << replaced by:
-    with open(file_path, 'rb') as file: obj = pickle.load(file)
+    with open(file_path, 'rb') as file:
+        obj = pickle.load(file)
 
     if obj_type:
         if not type(obj) is obj_type:
             raise PyPaqException(f'ERROR: obj from file is not {str(obj_type)} type')
     return obj
 
 
 def w_pickle(obj, file_path):
     with open(file_path, 'wb') as file:
         pickle.dump(obj, file)
 
 
 def r_json(file_path, raise_exception=False) -> Optional[Union[Dict,List]]:
     if not os.path.isfile(file_path):
-        if raise_exception: raise FileNotFoundError(f'file {file_path} not exists!')
+        if raise_exception:
+            raise FileNotFoundError(f'file {file_path} not exists!')
         return None
     with open(file_path, 'r', encoding='utf-8') as file:
         return json.load(file)
 
 
 def w_json(data:Union[Dict,List], file_path):
     with open(file_path, 'w', encoding='utf-8') as file:
         json.dump(data, file, indent=4, ensure_ascii=False)
 
 
 def r_jsonl(file_path, raise_exception=False) -> Optional[List]:
     if not os.path.isfile(file_path):
-        if raise_exception: raise FileNotFoundError(f'file {file_path} not exists!')
+        if raise_exception:
+            raise FileNotFoundError(f'file {file_path} not exists!')
         return None
     with open(file_path, 'r', encoding='utf-8') as file:
         return [json.loads(line) for line in file]
 
 
 def w_jsonl(data:List, file_path):
     with open(file_path, 'w', encoding='utf-8') as file:
         for d in data:
             json.dump(d, file, ensure_ascii=False)
             file.write('\n')
 
 
 def r_csv(file_path, raise_exception=False) -> Optional[List]:
     if not os.path.isfile(file_path):
-        if raise_exception: raise FileNotFoundError(f'file {file_path} not exists!')
+        if raise_exception:
+            raise FileNotFoundError(f'file {file_path} not exists!')
         return None
     csv.field_size_limit(sys.maxsize)
     with open(file_path, newline='') as f:
         reader = csv.reader(f)
         return [row for row in reader][1:]
 
 
 def r_yaml(file_path, raise_exception=False):
     if not os.path.isfile(file_path):
-        if raise_exception: raise FileNotFoundError(f'file {file_path} not exists!')
+        if raise_exception:
+            raise FileNotFoundError(f'file {file_path} not exists!')
         return None
     with open(file_path) as file:
         return yaml.load(file, yaml.Loader)
 
 
 def get_dir(path: Union[str, Path]):
     path = str(path)
@@ -99,11 +118,12 @@
     ls = os.listdir(path)
     lsD = {'files':[], 'dirs':[]}
     for e in ls:
         lsD['files' if os.path.isfile(f'{path}/{e}') else 'dirs'].append(e)
     return lsD
 
 
-def get_requirements(fileFP:str='requirements.txt') -> List[str]:
-    with open(fileFP) as file:
-        return [l.strip() for l in file]
+def get_requirements(file_path:str='requirements.txt') -> List[str]:
+    file_text = r_text(file_path, raise_exception=True)
+    file_lines = file_text.split('\n')
+    return [l.strip() for l in file_lines]
```

### Comparing `pypaq-1.7.3/pypaq/lipytools/moving_average.py` & `pypaq-1.7.5/pypaq/lipytools/moving_average.py`

 * *Files identical despite different names*

### Comparing `pypaq-1.7.3/pypaq/lipytools/plots.py` & `pypaq-1.7.5/pypaq/lipytools/plots.py`

 * *Files identical despite different names*

### Comparing `pypaq-1.7.3/pypaq/lipytools/pylogger.py` & `pypaq-1.7.5/pypaq/lipytools/pylogger.py`

 * *Files identical despite different names*

### Comparing `pypaq-1.7.3/pypaq/lipytools/stats.py` & `pypaq-1.7.5/pypaq/lipytools/stats.py`

 * *Files identical despite different names*

### Comparing `pypaq-1.7.3/pypaq/lipytools/time_reporter.py` & `pypaq-1.7.5/pypaq/lipytools/time_reporter.py`

 * *Files identical despite different names*

### Comparing `pypaq-1.7.3/pypaq/mpython/mpdecor.py` & `pypaq-1.7.5/pypaq/mpython/mpdecor.py`

 * *Files identical despite different names*

### Comparing `pypaq-1.7.3/pypaq/mpython/mptools.py` & `pypaq-1.7.5/pypaq/mpython/mptools.py`

 * *Files identical despite different names*

### Comparing `pypaq-1.7.3/pypaq/pms/base.py` & `pypaq-1.7.5/pypaq/pms/base.py`

 * *Files identical despite different names*

### Comparing `pypaq-1.7.3/pypaq/pms/config_manager.py` & `pypaq-1.7.5/pypaq/pms/config_manager.py`

 * *Files identical despite different names*

### Comparing `pypaq-1.7.3/pypaq/pms/para.py` & `pypaq-1.7.5/pypaq/pms/para.py`

 * *Files identical despite different names*

### Comparing `pypaq-1.7.3/pypaq/pms/parasave.py` & `pypaq-1.7.5/pypaq/pms/parasave.py`

 * *Files identical despite different names*

### Comparing `pypaq-1.7.3/pypaq/pms/paspa.py` & `pypaq-1.7.5/pypaq/pms/paspa.py`

 * *Files identical despite different names*

### Comparing `pypaq-1.7.3/pypaq/pms/points_cloud.py` & `pypaq-1.7.5/pypaq/pms/points_cloud.py`

 * *Files identical despite different names*

### Comparing `pypaq-1.7.3/pypaq/textools/text_metrics.py` & `pypaq-1.7.5/pypaq/textools/text_metrics.py`

 * *Files identical despite different names*

### Comparing `pypaq-1.7.3/pypaq/textools/text_processing.py` & `pypaq-1.7.5/pypaq/textools/text_processing.py`

 * *Files identical despite different names*

### Comparing `pypaq-1.7.3/pypaq.egg-info/SOURCES.txt` & `pypaq-1.7.5/pypaq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

