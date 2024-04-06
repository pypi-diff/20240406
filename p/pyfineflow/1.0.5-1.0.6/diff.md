# Comparing `tmp/pyfineflow-1.0.5.tar.gz` & `tmp/pyfineflow-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfineflow-1.0.5.tar", last modified: Sat Feb 10 12:05:51 2024, max compression
+gzip compressed data, was "pyfineflow-1.0.6.tar", last modified: Sat Apr  6 14:24:18 2024, max compression
```

## Comparing `pyfineflow-1.0.5.tar` & `pyfineflow-1.0.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-02-10 12:05:51.479753 pyfineflow-1.0.5/
--rw-rw-rw-   0        0        0     1086 2024-02-08 02:37:27.000000 pyfineflow-1.0.5/LICENSE
--rw-rw-rw-   0        0        0     1166 2024-02-10 12:05:51.478701 pyfineflow-1.0.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-02-10 12:05:51.470363 pyfineflow-1.0.5/pyfineflow/
--rw-rw-rw-   0        0        0        0 2024-02-08 02:37:27.000000 pyfineflow-1.0.5/pyfineflow/__init__.py
--rw-rw-rw-   0        0        0    16192 2024-02-08 15:01:43.000000 pyfineflow-1.0.5/pyfineflow/core.py
--rw-rw-rw-   0        0        0     1222 2024-02-08 02:37:27.000000 pyfineflow-1.0.5/pyfineflow/log_conf.py
--rw-rw-rw-   0        0        0     3449 2024-02-08 02:37:27.000000 pyfineflow-1.0.5/pyfineflow/schemas.py
--rw-rw-rw-   0        0        0     4111 2024-02-08 15:01:53.000000 pyfineflow-1.0.5/pyfineflow/utils.py
-drwxrwxrwx   0        0        0        0 2024-02-10 12:05:51.476209 pyfineflow-1.0.5/pyfineflow.egg-info/
--rw-rw-rw-   0        0        0     1166 2024-02-10 12:05:51.000000 pyfineflow-1.0.5/pyfineflow.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      292 2024-02-10 12:05:51.000000 pyfineflow-1.0.5/pyfineflow.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-10 12:05:51.000000 pyfineflow-1.0.5/pyfineflow.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-02-10 12:05:51.000000 pyfineflow-1.0.5/pyfineflow.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-02-10 12:05:51.000000 pyfineflow-1.0.5/pyfineflow.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-02-10 12:05:51.479753 pyfineflow-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0      540 2024-02-10 12:05:47.000000 pyfineflow-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-06 14:24:18.820325 pyfineflow-1.0.6/
+-rw-rw-rw-   0        0        0     1086 2024-02-03 16:31:19.000000 pyfineflow-1.0.6/LICENSE
+-rw-rw-rw-   0        0        0     1142 2024-04-06 14:24:18.819324 pyfineflow-1.0.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-06 14:24:18.806213 pyfineflow-1.0.6/pyfineflow/
+-rw-rw-rw-   0        0        0        0 2024-01-18 17:00:18.000000 pyfineflow-1.0.6/pyfineflow/__init__.py
+-rw-rw-rw-   0        0        0    16193 2024-04-06 14:23:18.000000 pyfineflow-1.0.6/pyfineflow/core.py
+-rw-rw-rw-   0        0        0     1222 2024-01-18 17:00:18.000000 pyfineflow-1.0.6/pyfineflow/log_conf.py
+-rw-rw-rw-   0        0        0     3449 2024-01-18 17:00:18.000000 pyfineflow-1.0.6/pyfineflow/schemas.py
+-rw-rw-rw-   0        0        0     4111 2024-02-16 03:26:57.000000 pyfineflow-1.0.6/pyfineflow/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-06 14:24:18.817325 pyfineflow-1.0.6/pyfineflow.egg-info/
+-rw-rw-rw-   0        0        0     1142 2024-04-06 14:24:18.000000 pyfineflow-1.0.6/pyfineflow.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      292 2024-04-06 14:24:18.000000 pyfineflow-1.0.6/pyfineflow.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-06 14:24:18.000000 pyfineflow-1.0.6/pyfineflow.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-04-06 14:24:18.000000 pyfineflow-1.0.6/pyfineflow.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-06 14:24:18.000000 pyfineflow-1.0.6/pyfineflow.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-06 14:24:18.820325 pyfineflow-1.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      540 2024-04-06 14:24:13.000000 pyfineflow-1.0.6/setup.py
```

### Comparing `pyfineflow-1.0.5/LICENSE` & `pyfineflow-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pyfineflow-1.0.5/PKG-INFO` & `pyfineflow-1.0.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 Metadata-Version: 2.1
 Name: pyfineflow
-Version: 1.0.5
+Version: 1.0.6
 Summary: python nodes server for fineflow
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: fastapi
 
 # pyfineflow
 
 > fineflow的python节点后端
 
 ## usage
```

### Comparing `pyfineflow-1.0.5/pyfineflow/core.py` & `pyfineflow-1.0.6/pyfineflow/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,15 +74,15 @@
         item = item.copy()
         key = item['key']
         if key not in items_dict:
             items_dict[key] = item
         else:
             item.update(items_dict[key])
             items_dict[key] = item
-    return list(items_dict.items())
+    return list(items_dict.values())
 
 
 class Fine:
     def __init__(self, mod: str, key: str = None, github_url=None, des=None, use_ws=False):
         if not key:
             if not github_url:
                 raise Exception("need key or github_url")
```

### Comparing `pyfineflow-1.0.5/pyfineflow/log_conf.py` & `pyfineflow-1.0.6/pyfineflow/log_conf.py`

 * *Files identical despite different names*

### Comparing `pyfineflow-1.0.5/pyfineflow/schemas.py` & `pyfineflow-1.0.6/pyfineflow/schemas.py`

 * *Files identical despite different names*

### Comparing `pyfineflow-1.0.5/pyfineflow/utils.py` & `pyfineflow-1.0.6/pyfineflow/utils.py`

 * *Files identical despite different names*

### Comparing `pyfineflow-1.0.5/pyfineflow.egg-info/PKG-INFO` & `pyfineflow-1.0.6/pyfineflow.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 Metadata-Version: 2.1
 Name: pyfineflow
-Version: 1.0.5
+Version: 1.0.6
 Summary: python nodes server for fineflow
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: fastapi
 
 # pyfineflow
 
 > fineflow的python节点后端
 
 ## usage
```

### Comparing `pyfineflow-1.0.5/setup.py` & `pyfineflow-1.0.6/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # --skip-existing 覆盖
 # python setup.py sdist bdist_wheel
 # twine upload dist/* --skip-existing
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 setup(
     name='pyfineflow',
-    version='1.0.5',
+    version='1.0.6',
     packages=find_packages(exclude=['__pycache__']),
     description='python nodes server for fineflow',
     long_description=long_description,
     long_description_content_type='text/markdown',
     install_requires=[
         'fastapi',
     ]
```

