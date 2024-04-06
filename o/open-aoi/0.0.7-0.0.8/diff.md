# Comparing `tmp/open_aoi-0.0.7.tar.gz` & `tmp/open_aoi-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open_aoi-0.0.7.tar", last modified: Sat Apr  6 15:31:28 2024, max compression
+gzip compressed data, was "open_aoi-0.0.8.tar", last modified: Sat Apr  6 15:47:44 2024, max compression
```

## Comparing `open_aoi-0.0.7.tar` & `open_aoi-0.0.8.tar`

### file list

```diff
@@ -1,40 +1,37 @@
-drwxrwxrwx   0 egor      (1000) egor      (1000)        0 2024-04-06 15:31:28.282726 open_aoi-0.0.7/
--rwxrwxrwx   0 egor      (1000) egor      (1000)     1073 2024-02-13 20:04:15.000000 open_aoi-0.0.7/LICENSE
--rwxrwxrwx   0 egor      (1000) egor      (1000)     1542 2024-04-06 15:31:28.281057 open_aoi-0.0.7/PKG-INFO
--rwxrwxrwx   0 egor      (1000) egor      (1000)      739 2024-03-17 13:58:48.000000 open_aoi-0.0.7/README.md
--rwxrwxrwx   0 egor      (1000) egor      (1000)      787 2024-04-06 15:31:17.000000 open_aoi-0.0.7/pyproject.toml
--rwxrwxrwx   0 egor      (1000) egor      (1000)       38 2024-04-06 15:31:28.283159 open_aoi-0.0.7/setup.cfg
-drwxrwxrwx   0 egor      (1000) egor      (1000)        0 2024-04-06 15:31:28.207294 open_aoi-0.0.7/src/
-drwxrwxrwx   0 egor      (1000) egor      (1000)        0 2024-04-06 15:31:28.226917 open_aoi-0.0.7/src/open_aoi/
-drwxrwxrwx   0 egor      (1000) egor      (1000)        0 2024-04-06 15:31:28.251322 open_aoi-0.0.7/src/open_aoi/controllers/
--rwxrwxrwx   0 egor      (1000) egor      (1000)     1948 2024-04-05 15:36:57.000000 open_aoi-0.0.7/src/open_aoi/controllers/__init__.py
--rwxrwxrwx   0 egor      (1000) egor      (1000)      818 2024-04-04 17:14:57.000000 open_aoi-0.0.7/src/open_aoi/controllers/accessor.py
--rwxrwxrwx   0 egor      (1000) egor      (1000)      741 2024-04-04 16:54:52.000000 open_aoi-0.0.7/src/open_aoi/controllers/camera.py
--rwxrwxrwx   0 egor      (1000) egor      (1000)     2052 2024-04-05 15:34:51.000000 open_aoi-0.0.7/src/open_aoi/controllers/control_handler.py
--rwxrwxrwx   0 egor      (1000) egor      (1000)      821 2024-04-04 19:19:04.000000 open_aoi-0.0.7/src/open_aoi/controllers/defect_type.py
--rwxrwxrwx   0 egor      (1000) egor      (1000)      180 2024-04-04 17:00:36.000000 open_aoi-0.0.7/src/open_aoi/controllers/inspection.py
-drwxrwxrwx   0 egor      (1000) egor      (1000)        0 2024-04-06 15:31:28.259120 open_aoi-0.0.7/src/open_aoi/controllers/ros_services/
--rwxrwxrwx   0 egor      (1000) egor      (1000)      985 2024-04-05 20:11:53.000000 open_aoi-0.0.7/src/open_aoi/controllers/ros_services/__init__.py
--rwxrwxrwx   0 egor      (1000) egor      (1000)     1524 2024-04-05 19:35:47.000000 open_aoi-0.0.7/src/open_aoi/controllers/ros_services/image_acquisition.py
--rwxrwxrwx   0 egor      (1000) egor      (1000)      690 2024-04-04 17:00:39.000000 open_aoi-0.0.7/src/open_aoi/controllers/template.py
--rwxrwxrwx   0 egor      (1000) egor      (1000)      251 2024-04-04 18:39:54.000000 open_aoi-0.0.7/src/open_aoi/enums.py
--rwxrwxrwx   0 egor      (1000) egor      (1000)      489 2024-04-05 18:36:15.000000 open_aoi-0.0.7/src/open_aoi/exceptions.py
-drwxrwxrwx   0 egor      (1000) egor      (1000)        0 2024-04-06 15:31:28.274489 open_aoi-0.0.7/src/open_aoi/mixins/
--rwxrwxrwx   0 egor      (1000) egor      (1000)       25 2024-04-04 17:11:38.000000 open_aoi-0.0.7/src/open_aoi/mixins/__init__.py
--rwxrwxrwx   0 egor      (1000) egor      (1000)     2072 2024-04-04 16:41:47.000000 open_aoi-0.0.7/src/open_aoi/mixins/accessor.py
--rwxrwxrwx   0 egor      (1000) egor      (1000)      337 2024-04-04 16:41:27.000000 open_aoi-0.0.7/src/open_aoi/mixins/camera.py
--rwxrwxrwx   0 egor      (1000) egor      (1000)     4096 2024-04-05 15:32:22.000000 open_aoi-0.0.7/src/open_aoi/mixins/control_handler.py
--rwxrwxrwx   0 egor      (1000) egor      (1000)      223 2024-04-04 16:58:21.000000 open_aoi-0.0.7/src/open_aoi/mixins/control_zone.py
--rwxrwxrwx   0 egor      (1000) egor      (1000)      151 2024-04-04 17:02:30.000000 open_aoi-0.0.7/src/open_aoi/mixins/inspection.py
--rwxrwxrwx   0 egor      (1000) egor      (1000)      341 2024-04-04 17:04:08.000000 open_aoi-0.0.7/src/open_aoi/mixins/template.py
--rwxrwxrwx   0 egor      (1000) egor      (1000)    11567 2024-04-04 20:39:34.000000 open_aoi-0.0.7/src/open_aoi/models.py
-drwxrwxrwx   0 egor      (1000) egor      (1000)        0 2024-04-06 15:31:28.276815 open_aoi-0.0.7/src/open_aoi/scripts/
--rwxrwxrwx   0 egor      (1000) egor      (1000)      160 2024-04-01 17:53:57.000000 open_aoi-0.0.7/src/open_aoi/scripts/db_create_all.py
--rwxrwxrwx   0 egor      (1000) egor      (1000)     3046 2024-04-04 20:16:21.000000 open_aoi-0.0.7/src/open_aoi/scripts/db_create_assets.py
--rwxrwxrwx   0 egor      (1000) egor      (1000)     1388 2024-04-06 15:30:31.000000 open_aoi-0.0.7/src/open_aoi/settings.py
-drwxrwxrwx   0 egor      (1000) egor      (1000)        0 2024-04-06 15:31:28.279644 open_aoi-0.0.7/src/open_aoi.egg-info/
--rwxrwxrwx   0 egor      (1000) egor      (1000)     1542 2024-04-06 15:31:28.000000 open_aoi-0.0.7/src/open_aoi.egg-info/PKG-INFO
--rwxrwxrwx   0 egor      (1000) egor      (1000)     1000 2024-04-06 15:31:28.000000 open_aoi-0.0.7/src/open_aoi.egg-info/SOURCES.txt
--rwxrwxrwx   0 egor      (1000) egor      (1000)        1 2024-04-06 15:31:28.000000 open_aoi-0.0.7/src/open_aoi.egg-info/dependency_links.txt
--rwxrwxrwx   0 egor      (1000) egor      (1000)       83 2024-04-06 15:31:28.000000 open_aoi-0.0.7/src/open_aoi.egg-info/requires.txt
--rwxrwxrwx   0 egor      (1000) egor      (1000)        9 2024-04-06 15:31:28.000000 open_aoi-0.0.7/src/open_aoi.egg-info/top_level.txt
+drwxrwxrwx   0 egor      (1000) egor      (1000)        0 2024-04-06 15:47:44.162140 open_aoi-0.0.8/
+-rwxrwxrwx   0 egor      (1000) egor      (1000)     1073 2024-02-13 20:04:15.000000 open_aoi-0.0.8/LICENSE
+-rwxrwxrwx   0 egor      (1000) egor      (1000)     1518 2024-04-06 15:47:44.158921 open_aoi-0.0.8/PKG-INFO
+-rwxrwxrwx   0 egor      (1000) egor      (1000)      739 2024-03-17 13:58:48.000000 open_aoi-0.0.8/README.md
+-rwxrwxrwx   0 egor      (1000) egor      (1000)      775 2024-04-06 15:47:35.000000 open_aoi-0.0.8/pyproject.toml
+-rwxrwxrwx   0 egor      (1000) egor      (1000)       38 2024-04-06 15:47:44.163109 open_aoi-0.0.8/setup.cfg
+drwxrwxrwx   0 egor      (1000) egor      (1000)        0 2024-04-06 15:47:44.034299 open_aoi-0.0.8/src/
+drwxrwxrwx   0 egor      (1000) egor      (1000)        0 2024-04-06 15:47:44.073152 open_aoi-0.0.8/src/open_aoi/
+drwxrwxrwx   0 egor      (1000) egor      (1000)        0 2024-04-06 15:47:44.126485 open_aoi-0.0.8/src/open_aoi/controllers/
+-rwxrwxrwx   0 egor      (1000) egor      (1000)     1948 2024-04-05 15:36:57.000000 open_aoi-0.0.8/src/open_aoi/controllers/__init__.py
+-rwxrwxrwx   0 egor      (1000) egor      (1000)      818 2024-04-04 17:14:57.000000 open_aoi-0.0.8/src/open_aoi/controllers/accessor.py
+-rwxrwxrwx   0 egor      (1000) egor      (1000)      741 2024-04-04 16:54:52.000000 open_aoi-0.0.8/src/open_aoi/controllers/camera.py
+-rwxrwxrwx   0 egor      (1000) egor      (1000)     2052 2024-04-05 15:34:51.000000 open_aoi-0.0.8/src/open_aoi/controllers/control_handler.py
+-rwxrwxrwx   0 egor      (1000) egor      (1000)      821 2024-04-04 19:19:04.000000 open_aoi-0.0.8/src/open_aoi/controllers/defect_type.py
+-rwxrwxrwx   0 egor      (1000) egor      (1000)      180 2024-04-04 17:00:36.000000 open_aoi-0.0.8/src/open_aoi/controllers/inspection.py
+-rwxrwxrwx   0 egor      (1000) egor      (1000)      690 2024-04-04 17:00:39.000000 open_aoi-0.0.8/src/open_aoi/controllers/template.py
+-rwxrwxrwx   0 egor      (1000) egor      (1000)      251 2024-04-04 18:39:54.000000 open_aoi-0.0.8/src/open_aoi/enums.py
+-rwxrwxrwx   0 egor      (1000) egor      (1000)      489 2024-04-05 18:36:15.000000 open_aoi-0.0.8/src/open_aoi/exceptions.py
+drwxrwxrwx   0 egor      (1000) egor      (1000)        0 2024-04-06 15:47:44.145332 open_aoi-0.0.8/src/open_aoi/mixins/
+-rwxrwxrwx   0 egor      (1000) egor      (1000)       25 2024-04-04 17:11:38.000000 open_aoi-0.0.8/src/open_aoi/mixins/__init__.py
+-rwxrwxrwx   0 egor      (1000) egor      (1000)     2072 2024-04-04 16:41:47.000000 open_aoi-0.0.8/src/open_aoi/mixins/accessor.py
+-rwxrwxrwx   0 egor      (1000) egor      (1000)      337 2024-04-04 16:41:27.000000 open_aoi-0.0.8/src/open_aoi/mixins/camera.py
+-rwxrwxrwx   0 egor      (1000) egor      (1000)     4096 2024-04-05 15:32:22.000000 open_aoi-0.0.8/src/open_aoi/mixins/control_handler.py
+-rwxrwxrwx   0 egor      (1000) egor      (1000)      223 2024-04-04 16:58:21.000000 open_aoi-0.0.8/src/open_aoi/mixins/control_zone.py
+-rwxrwxrwx   0 egor      (1000) egor      (1000)      151 2024-04-04 17:02:30.000000 open_aoi-0.0.8/src/open_aoi/mixins/inspection.py
+-rwxrwxrwx   0 egor      (1000) egor      (1000)      341 2024-04-04 17:04:08.000000 open_aoi-0.0.8/src/open_aoi/mixins/template.py
+-rwxrwxrwx   0 egor      (1000) egor      (1000)    11567 2024-04-04 20:39:34.000000 open_aoi-0.0.8/src/open_aoi/models.py
+drwxrwxrwx   0 egor      (1000) egor      (1000)        0 2024-04-06 15:47:44.152584 open_aoi-0.0.8/src/open_aoi/scripts/
+-rwxrwxrwx   0 egor      (1000) egor      (1000)      160 2024-04-01 17:53:57.000000 open_aoi-0.0.8/src/open_aoi/scripts/db_create_all.py
+-rwxrwxrwx   0 egor      (1000) egor      (1000)     3046 2024-04-04 20:16:21.000000 open_aoi-0.0.8/src/open_aoi/scripts/db_create_assets.py
+-rwxrwxrwx   0 egor      (1000) egor      (1000)     1388 2024-04-06 15:30:31.000000 open_aoi-0.0.8/src/open_aoi/settings.py
+drwxrwxrwx   0 egor      (1000) egor      (1000)        0 2024-04-06 15:47:44.155512 open_aoi-0.0.8/src/open_aoi.egg-info/
+-rwxrwxrwx   0 egor      (1000) egor      (1000)     1518 2024-04-06 15:47:43.000000 open_aoi-0.0.8/src/open_aoi.egg-info/PKG-INFO
+-rwxrwxrwx   0 egor      (1000) egor      (1000)      891 2024-04-06 15:47:44.000000 open_aoi-0.0.8/src/open_aoi.egg-info/SOURCES.txt
+-rwxrwxrwx   0 egor      (1000) egor      (1000)        1 2024-04-06 15:47:43.000000 open_aoi-0.0.8/src/open_aoi.egg-info/dependency_links.txt
+-rwxrwxrwx   0 egor      (1000) egor      (1000)       74 2024-04-06 15:47:43.000000 open_aoi-0.0.8/src/open_aoi.egg-info/requires.txt
+-rwxrwxrwx   0 egor      (1000) egor      (1000)        9 2024-04-06 15:47:43.000000 open_aoi-0.0.8/src/open_aoi.egg-info/top_level.txt
```

### Comparing `open_aoi-0.0.7/LICENSE` & `open_aoi-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `open_aoi-0.0.7/PKG-INFO` & `open_aoi-0.0.8/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: open_aoi
-Version: 0.0.7
+Version: 0.0.8
 Summary: Support python package for Open AOI system project.
 Author-email: Cherniaev Egor <chrnyaevek@gmail.com>
 Project-URL: Homepage, https://github.com/ChrnyaevEK/open-aoi
 Project-URL: Issues, https://github.com/ChrnyaevEK/open-aoi/issues
 Keywords: automated optical inspection,pcb,computer vision
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: opencv-python
 Requires-Dist: nicegui
-Requires-Dist: roslibpy
 Requires-Dist: sqlalchemy
 Requires-Dist: pymysql
 Requires-Dist: cryptography
 Requires-Dist: bcrypt
 Requires-Dist: pillow
 Requires-Dist: minio
```

### Comparing `open_aoi-0.0.7/README.md` & `open_aoi-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `open_aoi-0.0.7/pyproject.toml` & `open_aoi-0.0.8/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "open_aoi"
-version="0.0.7"
+version="0.0.8"
 authors = [
   { name="Cherniaev Egor", email="chrnyaevek@gmail.com" },
 ]
 description = "Support python package for Open AOI system project."
 keywords=["automated optical inspection", "pcb", "computer vision"]
 readme = "README.md"
 requires-python = ">=3.7"
-dependencies = ["opencv-python", "nicegui", "roslibpy", "sqlalchemy", "pymysql", "cryptography", "bcrypt", "pillow", "minio"]
+dependencies = ["opencv-python", "nicegui", "sqlalchemy", "pymysql", "cryptography", "bcrypt", "pillow", "minio"]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
```

### Comparing `open_aoi-0.0.7/src/open_aoi/controllers/__init__.py` & `open_aoi-0.0.8/src/open_aoi/controllers/__init__.py`

 * *Files identical despite different names*

### Comparing `open_aoi-0.0.7/src/open_aoi/controllers/accessor.py` & `open_aoi-0.0.8/src/open_aoi/controllers/accessor.py`

 * *Files identical despite different names*

### Comparing `open_aoi-0.0.7/src/open_aoi/controllers/camera.py` & `open_aoi-0.0.8/src/open_aoi/controllers/camera.py`

 * *Files identical despite different names*

### Comparing `open_aoi-0.0.7/src/open_aoi/controllers/control_handler.py` & `open_aoi-0.0.8/src/open_aoi/controllers/control_handler.py`

 * *Files identical despite different names*

### Comparing `open_aoi-0.0.7/src/open_aoi/controllers/defect_type.py` & `open_aoi-0.0.8/src/open_aoi/controllers/defect_type.py`

 * *Files identical despite different names*

### Comparing `open_aoi-0.0.7/src/open_aoi/controllers/template.py` & `open_aoi-0.0.8/src/open_aoi/controllers/template.py`

 * *Files identical despite different names*

### Comparing `open_aoi-0.0.7/src/open_aoi/mixins/accessor.py` & `open_aoi-0.0.8/src/open_aoi/mixins/accessor.py`

 * *Files identical despite different names*

### Comparing `open_aoi-0.0.7/src/open_aoi/mixins/control_handler.py` & `open_aoi-0.0.8/src/open_aoi/mixins/control_handler.py`

 * *Files identical despite different names*

### Comparing `open_aoi-0.0.7/src/open_aoi/models.py` & `open_aoi-0.0.8/src/open_aoi/models.py`

 * *Files identical despite different names*

### Comparing `open_aoi-0.0.7/src/open_aoi/scripts/db_create_assets.py` & `open_aoi-0.0.8/src/open_aoi/scripts/db_create_assets.py`

 * *Files identical despite different names*

### Comparing `open_aoi-0.0.7/src/open_aoi/settings.py` & `open_aoi-0.0.8/src/open_aoi/settings.py`

 * *Files identical despite different names*

### Comparing `open_aoi-0.0.7/src/open_aoi.egg-info/PKG-INFO` & `open_aoi-0.0.8/src/open_aoi.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: open_aoi
-Version: 0.0.7
+Version: 0.0.8
 Summary: Support python package for Open AOI system project.
 Author-email: Cherniaev Egor <chrnyaevek@gmail.com>
 Project-URL: Homepage, https://github.com/ChrnyaevEK/open-aoi
 Project-URL: Issues, https://github.com/ChrnyaevEK/open-aoi/issues
 Keywords: automated optical inspection,pcb,computer vision
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: opencv-python
 Requires-Dist: nicegui
-Requires-Dist: roslibpy
 Requires-Dist: sqlalchemy
 Requires-Dist: pymysql
 Requires-Dist: cryptography
 Requires-Dist: bcrypt
 Requires-Dist: pillow
 Requires-Dist: minio
```

### Comparing `open_aoi-0.0.7/src/open_aoi.egg-info/SOURCES.txt` & `open_aoi-0.0.8/src/open_aoi.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -13,16 +13,14 @@
 src/open_aoi/controllers/__init__.py
 src/open_aoi/controllers/accessor.py
 src/open_aoi/controllers/camera.py
 src/open_aoi/controllers/control_handler.py
 src/open_aoi/controllers/defect_type.py
 src/open_aoi/controllers/inspection.py
 src/open_aoi/controllers/template.py
-src/open_aoi/controllers/ros_services/__init__.py
-src/open_aoi/controllers/ros_services/image_acquisition.py
 src/open_aoi/mixins/__init__.py
 src/open_aoi/mixins/accessor.py
 src/open_aoi/mixins/camera.py
 src/open_aoi/mixins/control_handler.py
 src/open_aoi/mixins/control_zone.py
 src/open_aoi/mixins/inspection.py
 src/open_aoi/mixins/template.py
```

