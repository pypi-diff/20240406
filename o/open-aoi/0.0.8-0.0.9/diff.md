# Comparing `tmp/open_aoi-0.0.8.tar.gz` & `tmp/open_aoi-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open_aoi-0.0.8.tar", last modified: Sat Apr  6 15:47:44 2024, max compression
+gzip compressed data, was "open_aoi-0.0.9.tar", last modified: Sat Apr  6 15:52:10 2024, max compression
```

## Comparing `open_aoi-0.0.8.tar` & `open_aoi-0.0.9.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxrwx   0 egor      (1000) egor      (1000)        0 2024-04-06 15:47:44.162140 open_aoi-0.0.8/
--rwxrwxrwx   0 egor      (1000) egor      (1000)     1073 2024-02-13 20:04:15.000000 open_aoi-0.0.8/LICENSE
--rwxrwxrwx   0 egor      (1000) egor      (1000)     1518 2024-04-06 15:47:44.158921 open_aoi-0.0.8/PKG-INFO
--rwxrwxrwx   0 egor      (1000) egor      (1000)      739 2024-03-17 13:58:48.000000 open_aoi-0.0.8/README.md
--rwxrwxrwx   0 egor      (1000) egor      (1000)      775 2024-04-06 15:47:35.000000 open_aoi-0.0.8/pyproject.toml
--rwxrwxrwx   0 egor      (1000) egor      (1000)       38 2024-04-06 15:47:44.163109 open_aoi-0.0.8/setup.cfg
-drwxrwxrwx   0 egor      (1000) egor      (1000)        0 2024-04-06 15:47:44.034299 open_aoi-0.0.8/src/
-drwxrwxrwx   0 egor      (1000) egor      (1000)        0 2024-04-06 15:47:44.073152 open_aoi-0.0.8/src/open_aoi/
-drwxrwxrwx   0 egor      (1000) egor      (1000)        0 2024-04-06 15:47:44.126485 open_aoi-0.0.8/src/open_aoi/controllers/
--rwxrwxrwx   0 egor      (1000) egor      (1000)     1948 2024-04-05 15:36:57.000000 open_aoi-0.0.8/src/open_aoi/controllers/__init__.py
--rwxrwxrwx   0 egor      (1000) egor      (1000)      818 2024-04-04 17:14:57.000000 open_aoi-0.0.8/src/open_aoi/controllers/accessor.py
--rwxrwxrwx   0 egor      (1000) egor      (1000)      741 2024-04-04 16:54:52.000000 open_aoi-0.0.8/src/open_aoi/controllers/camera.py
--rwxrwxrwx   0 egor      (1000) egor      (1000)     2052 2024-04-05 15:34:51.000000 open_aoi-0.0.8/src/open_aoi/controllers/control_handler.py
--rwxrwxrwx   0 egor      (1000) egor      (1000)      821 2024-04-04 19:19:04.000000 open_aoi-0.0.8/src/open_aoi/controllers/defect_type.py
--rwxrwxrwx   0 egor      (1000) egor      (1000)      180 2024-04-04 17:00:36.000000 open_aoi-0.0.8/src/open_aoi/controllers/inspection.py
--rwxrwxrwx   0 egor      (1000) egor      (1000)      690 2024-04-04 17:00:39.000000 open_aoi-0.0.8/src/open_aoi/controllers/template.py
--rwxrwxrwx   0 egor      (1000) egor      (1000)      251 2024-04-04 18:39:54.000000 open_aoi-0.0.8/src/open_aoi/enums.py
--rwxrwxrwx   0 egor      (1000) egor      (1000)      489 2024-04-05 18:36:15.000000 open_aoi-0.0.8/src/open_aoi/exceptions.py
-drwxrwxrwx   0 egor      (1000) egor      (1000)        0 2024-04-06 15:47:44.145332 open_aoi-0.0.8/src/open_aoi/mixins/
--rwxrwxrwx   0 egor      (1000) egor      (1000)       25 2024-04-04 17:11:38.000000 open_aoi-0.0.8/src/open_aoi/mixins/__init__.py
--rwxrwxrwx   0 egor      (1000) egor      (1000)     2072 2024-04-04 16:41:47.000000 open_aoi-0.0.8/src/open_aoi/mixins/accessor.py
--rwxrwxrwx   0 egor      (1000) egor      (1000)      337 2024-04-04 16:41:27.000000 open_aoi-0.0.8/src/open_aoi/mixins/camera.py
--rwxrwxrwx   0 egor      (1000) egor      (1000)     4096 2024-04-05 15:32:22.000000 open_aoi-0.0.8/src/open_aoi/mixins/control_handler.py
--rwxrwxrwx   0 egor      (1000) egor      (1000)      223 2024-04-04 16:58:21.000000 open_aoi-0.0.8/src/open_aoi/mixins/control_zone.py
--rwxrwxrwx   0 egor      (1000) egor      (1000)      151 2024-04-04 17:02:30.000000 open_aoi-0.0.8/src/open_aoi/mixins/inspection.py
--rwxrwxrwx   0 egor      (1000) egor      (1000)      341 2024-04-04 17:04:08.000000 open_aoi-0.0.8/src/open_aoi/mixins/template.py
--rwxrwxrwx   0 egor      (1000) egor      (1000)    11567 2024-04-04 20:39:34.000000 open_aoi-0.0.8/src/open_aoi/models.py
-drwxrwxrwx   0 egor      (1000) egor      (1000)        0 2024-04-06 15:47:44.152584 open_aoi-0.0.8/src/open_aoi/scripts/
--rwxrwxrwx   0 egor      (1000) egor      (1000)      160 2024-04-01 17:53:57.000000 open_aoi-0.0.8/src/open_aoi/scripts/db_create_all.py
--rwxrwxrwx   0 egor      (1000) egor      (1000)     3046 2024-04-04 20:16:21.000000 open_aoi-0.0.8/src/open_aoi/scripts/db_create_assets.py
--rwxrwxrwx   0 egor      (1000) egor      (1000)     1388 2024-04-06 15:30:31.000000 open_aoi-0.0.8/src/open_aoi/settings.py
-drwxrwxrwx   0 egor      (1000) egor      (1000)        0 2024-04-06 15:47:44.155512 open_aoi-0.0.8/src/open_aoi.egg-info/
--rwxrwxrwx   0 egor      (1000) egor      (1000)     1518 2024-04-06 15:47:43.000000 open_aoi-0.0.8/src/open_aoi.egg-info/PKG-INFO
--rwxrwxrwx   0 egor      (1000) egor      (1000)      891 2024-04-06 15:47:44.000000 open_aoi-0.0.8/src/open_aoi.egg-info/SOURCES.txt
--rwxrwxrwx   0 egor      (1000) egor      (1000)        1 2024-04-06 15:47:43.000000 open_aoi-0.0.8/src/open_aoi.egg-info/dependency_links.txt
--rwxrwxrwx   0 egor      (1000) egor      (1000)       74 2024-04-06 15:47:43.000000 open_aoi-0.0.8/src/open_aoi.egg-info/requires.txt
--rwxrwxrwx   0 egor      (1000) egor      (1000)        9 2024-04-06 15:47:43.000000 open_aoi-0.0.8/src/open_aoi.egg-info/top_level.txt
+drwxrwxrwx   0 egor      (1000) egor      (1000)        0 2024-04-06 15:52:10.226600 open_aoi-0.0.9/
+-rwxrwxrwx   0 egor      (1000) egor      (1000)     1073 2024-02-13 20:04:15.000000 open_aoi-0.0.9/LICENSE
+-rwxrwxrwx   0 egor      (1000) egor      (1000)     1518 2024-04-06 15:52:10.221815 open_aoi-0.0.9/PKG-INFO
+-rwxrwxrwx   0 egor      (1000) egor      (1000)      739 2024-03-17 13:58:48.000000 open_aoi-0.0.9/README.md
+-rwxrwxrwx   0 egor      (1000) egor      (1000)      775 2024-04-06 15:51:58.000000 open_aoi-0.0.9/pyproject.toml
+-rwxrwxrwx   0 egor      (1000) egor      (1000)       38 2024-04-06 15:52:10.227290 open_aoi-0.0.9/setup.cfg
+drwxrwxrwx   0 egor      (1000) egor      (1000)        0 2024-04-06 15:52:10.162419 open_aoi-0.0.9/src/
+drwxrwxrwx   0 egor      (1000) egor      (1000)        0 2024-04-06 15:52:10.176992 open_aoi-0.0.9/src/open_aoi/
+drwxrwxrwx   0 egor      (1000) egor      (1000)        0 2024-04-06 15:52:10.201585 open_aoi-0.0.9/src/open_aoi/controllers/
+-rwxrwxrwx   0 egor      (1000) egor      (1000)     1948 2024-04-05 15:36:57.000000 open_aoi-0.0.9/src/open_aoi/controllers/__init__.py
+-rwxrwxrwx   0 egor      (1000) egor      (1000)      818 2024-04-04 17:14:57.000000 open_aoi-0.0.9/src/open_aoi/controllers/accessor.py
+-rwxrwxrwx   0 egor      (1000) egor      (1000)      741 2024-04-04 16:54:52.000000 open_aoi-0.0.9/src/open_aoi/controllers/camera.py
+-rwxrwxrwx   0 egor      (1000) egor      (1000)     2052 2024-04-05 15:34:51.000000 open_aoi-0.0.9/src/open_aoi/controllers/control_handler.py
+-rwxrwxrwx   0 egor      (1000) egor      (1000)      821 2024-04-04 19:19:04.000000 open_aoi-0.0.9/src/open_aoi/controllers/defect_type.py
+-rwxrwxrwx   0 egor      (1000) egor      (1000)      180 2024-04-04 17:00:36.000000 open_aoi-0.0.9/src/open_aoi/controllers/inspection.py
+-rwxrwxrwx   0 egor      (1000) egor      (1000)      690 2024-04-04 17:00:39.000000 open_aoi-0.0.9/src/open_aoi/controllers/template.py
+-rwxrwxrwx   0 egor      (1000) egor      (1000)      251 2024-04-04 18:39:54.000000 open_aoi-0.0.9/src/open_aoi/enums.py
+-rwxrwxrwx   0 egor      (1000) egor      (1000)      489 2024-04-05 18:36:15.000000 open_aoi-0.0.9/src/open_aoi/exceptions.py
+drwxrwxrwx   0 egor      (1000) egor      (1000)        0 2024-04-06 15:52:10.213141 open_aoi-0.0.9/src/open_aoi/mixins/
+-rwxrwxrwx   0 egor      (1000) egor      (1000)       25 2024-04-04 17:11:38.000000 open_aoi-0.0.9/src/open_aoi/mixins/__init__.py
+-rwxrwxrwx   0 egor      (1000) egor      (1000)     2072 2024-04-04 16:41:47.000000 open_aoi-0.0.9/src/open_aoi/mixins/accessor.py
+-rwxrwxrwx   0 egor      (1000) egor      (1000)      337 2024-04-04 16:41:27.000000 open_aoi-0.0.9/src/open_aoi/mixins/camera.py
+-rwxrwxrwx   0 egor      (1000) egor      (1000)     4096 2024-04-05 15:32:22.000000 open_aoi-0.0.9/src/open_aoi/mixins/control_handler.py
+-rwxrwxrwx   0 egor      (1000) egor      (1000)      223 2024-04-04 16:58:21.000000 open_aoi-0.0.9/src/open_aoi/mixins/control_zone.py
+-rwxrwxrwx   0 egor      (1000) egor      (1000)      151 2024-04-04 17:02:30.000000 open_aoi-0.0.9/src/open_aoi/mixins/inspection.py
+-rwxrwxrwx   0 egor      (1000) egor      (1000)      341 2024-04-04 17:04:08.000000 open_aoi-0.0.9/src/open_aoi/mixins/template.py
+-rwxrwxrwx   0 egor      (1000) egor      (1000)    11567 2024-04-04 20:39:34.000000 open_aoi-0.0.9/src/open_aoi/models.py
+drwxrwxrwx   0 egor      (1000) egor      (1000)        0 2024-04-06 15:52:10.215727 open_aoi-0.0.9/src/open_aoi/scripts/
+-rwxrwxrwx   0 egor      (1000) egor      (1000)      160 2024-04-01 17:53:57.000000 open_aoi-0.0.9/src/open_aoi/scripts/db_create_all.py
+-rwxrwxrwx   0 egor      (1000) egor      (1000)     3046 2024-04-04 20:16:21.000000 open_aoi-0.0.9/src/open_aoi/scripts/db_create_assets.py
+-rwxrwxrwx   0 egor      (1000) egor      (1000)      937 2024-04-06 15:51:35.000000 open_aoi-0.0.9/src/open_aoi/settings.py
+drwxrwxrwx   0 egor      (1000) egor      (1000)        0 2024-04-06 15:52:10.217677 open_aoi-0.0.9/src/open_aoi.egg-info/
+-rwxrwxrwx   0 egor      (1000) egor      (1000)     1518 2024-04-06 15:52:10.000000 open_aoi-0.0.9/src/open_aoi.egg-info/PKG-INFO
+-rwxrwxrwx   0 egor      (1000) egor      (1000)      891 2024-04-06 15:52:10.000000 open_aoi-0.0.9/src/open_aoi.egg-info/SOURCES.txt
+-rwxrwxrwx   0 egor      (1000) egor      (1000)        1 2024-04-06 15:52:10.000000 open_aoi-0.0.9/src/open_aoi.egg-info/dependency_links.txt
+-rwxrwxrwx   0 egor      (1000) egor      (1000)       74 2024-04-06 15:52:10.000000 open_aoi-0.0.9/src/open_aoi.egg-info/requires.txt
+-rwxrwxrwx   0 egor      (1000) egor      (1000)        9 2024-04-06 15:52:10.000000 open_aoi-0.0.9/src/open_aoi.egg-info/top_level.txt
```

### Comparing `open_aoi-0.0.8/LICENSE` & `open_aoi-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `open_aoi-0.0.8/PKG-INFO` & `open_aoi-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open_aoi
-Version: 0.0.8
+Version: 0.0.9
 Summary: Support python package for Open AOI system project.
 Author-email: Cherniaev Egor <chrnyaevek@gmail.com>
 Project-URL: Homepage, https://github.com/ChrnyaevEK/open-aoi
 Project-URL: Issues, https://github.com/ChrnyaevEK/open-aoi/issues
 Keywords: automated optical inspection,pcb,computer vision
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `open_aoi-0.0.8/README.md` & `open_aoi-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `open_aoi-0.0.8/pyproject.toml` & `open_aoi-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "open_aoi"
-version="0.0.8"
+version="0.0.9"
 authors = [
   { name="Cherniaev Egor", email="chrnyaevek@gmail.com" },
 ]
 description = "Support python package for Open AOI system project."
 keywords=["automated optical inspection", "pcb", "computer vision"]
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `open_aoi-0.0.8/src/open_aoi/controllers/__init__.py` & `open_aoi-0.0.9/src/open_aoi/controllers/__init__.py`

 * *Files identical despite different names*

### Comparing `open_aoi-0.0.8/src/open_aoi/controllers/accessor.py` & `open_aoi-0.0.9/src/open_aoi/controllers/accessor.py`

 * *Files identical despite different names*

### Comparing `open_aoi-0.0.8/src/open_aoi/controllers/camera.py` & `open_aoi-0.0.9/src/open_aoi/controllers/camera.py`

 * *Files identical despite different names*

### Comparing `open_aoi-0.0.8/src/open_aoi/controllers/control_handler.py` & `open_aoi-0.0.9/src/open_aoi/controllers/control_handler.py`

 * *Files identical despite different names*

### Comparing `open_aoi-0.0.8/src/open_aoi/controllers/defect_type.py` & `open_aoi-0.0.9/src/open_aoi/controllers/defect_type.py`

 * *Files identical despite different names*

### Comparing `open_aoi-0.0.8/src/open_aoi/controllers/template.py` & `open_aoi-0.0.9/src/open_aoi/controllers/template.py`

 * *Files identical despite different names*

### Comparing `open_aoi-0.0.8/src/open_aoi/mixins/accessor.py` & `open_aoi-0.0.9/src/open_aoi/mixins/accessor.py`

 * *Files identical despite different names*

### Comparing `open_aoi-0.0.8/src/open_aoi/mixins/control_handler.py` & `open_aoi-0.0.9/src/open_aoi/mixins/control_handler.py`

 * *Files identical despite different names*

### Comparing `open_aoi-0.0.8/src/open_aoi/models.py` & `open_aoi-0.0.9/src/open_aoi/models.py`

 * *Files identical despite different names*

### Comparing `open_aoi-0.0.8/src/open_aoi/scripts/db_create_assets.py` & `open_aoi-0.0.9/src/open_aoi/scripts/db_create_assets.py`

 * *Files identical despite different names*

### Comparing `open_aoi-0.0.8/src/open_aoi/settings.py` & `open_aoi-0.0.9/src/open_aoi/settings.py`

 * *Files 25% similar despite different names*

```diff
@@ -12,30 +12,14 @@
 MYSQL_PORT = os.environ["MYSQL_PORT"]
 assert MYSQL_PORT
 try:
     MYSQL_PORT = int(MYSQL_PORT)
 except ValueError:
     raise RuntimeError("Failed to parse mysql port from environment")
 
-ROS_PORT = os.environ["ROS_PORT"]
-assert ROS_PORT
-try:
-    ROS_PORT = int(ROS_PORT)
-except ValueError:
-    raise RuntimeError("Failed to parse ROS port from environment")
-
-WEB_INTERFACE_PORT = os.environ["WEB_INTERFACE_PORT"]
-assert WEB_INTERFACE_PORT
-try:
-    WEB_INTERFACE_PORT = int(WEB_INTERFACE_PORT)
-except ValueError:
-    raise RuntimeError("Failed to parse web port from environment")
-
-ALLOW_SIMULATION_NODE = os.environ["SIMULATION"] == "1"
-
 AOI_OPERATOR_INITIAL_PASSWORD = os.environ["AOI_OPERATOR_INITIAL_PASSWORD"]
 assert AOI_OPERATOR_INITIAL_PASSWORD
 
 AOI_ADMINISTRATOR_INITIAL_PASSWORD = os.environ["AOI_ADMINISTRATOR_INITIAL_PASSWORD"]
 assert AOI_ADMINISTRATOR_INITIAL_PASSWORD
 
 STORAGE_SECRET = os.environ["STORAGE_SECRET"]
```

### Comparing `open_aoi-0.0.8/src/open_aoi.egg-info/PKG-INFO` & `open_aoi-0.0.9/src/open_aoi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open_aoi
-Version: 0.0.8
+Version: 0.0.9
 Summary: Support python package for Open AOI system project.
 Author-email: Cherniaev Egor <chrnyaevek@gmail.com>
 Project-URL: Homepage, https://github.com/ChrnyaevEK/open-aoi
 Project-URL: Issues, https://github.com/ChrnyaevEK/open-aoi/issues
 Keywords: automated optical inspection,pcb,computer vision
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `open_aoi-0.0.8/src/open_aoi.egg-info/SOURCES.txt` & `open_aoi-0.0.9/src/open_aoi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

