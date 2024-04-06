# Comparing `tmp/open_aoi-0.0.5.tar.gz` & `tmp/open_aoi-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open_aoi-0.0.5.tar", last modified: Sun Feb 11 14:59:23 2024, max compression
+gzip compressed data, was "open_aoi-0.0.6.tar", last modified: Sat Apr  6 14:23:23 2024, max compression
```

## Comparing `open_aoi-0.0.5.tar` & `open_aoi-0.0.6.tar`

### file list

```diff
@@ -1,36 +1,40 @@
-drwxrwxrwx   0 egor      (1000) egor      (1000)        0 2024-02-11 14:59:23.496696 open_aoi-0.0.5/
--rwxrwxrwx   0 egor      (1000) egor      (1000)     1073 2024-02-10 14:28:46.000000 open_aoi-0.0.5/LICENSE
--rwxrwxrwx   0 egor      (1000) egor      (1000)     1531 2024-02-11 14:59:23.495766 open_aoi-0.0.5/PKG-INFO
--rwxrwxrwx   0 egor      (1000) egor      (1000)      742 2024-02-11 14:58:43.000000 open_aoi-0.0.5/README.md
--rwxrwxrwx   0 egor      (1000) egor      (1000)      785 2024-02-11 14:58:55.000000 open_aoi-0.0.5/pyproject.toml
--rwxrwxrwx   0 egor      (1000) egor      (1000)       38 2024-02-11 14:59:23.498665 open_aoi-0.0.5/setup.cfg
-drwxrwxrwx   0 egor      (1000) egor      (1000)        0 2024-02-11 14:59:23.420257 open_aoi-0.0.5/src/
-drwxrwxrwx   0 egor      (1000) egor      (1000)        0 2024-02-11 14:59:23.441876 open_aoi-0.0.5/src/open_aoi/
--rwxrwxrwx   0 egor      (1000) egor      (1000)      412 2024-01-30 20:20:48.000000 open_aoi-0.0.5/src/open_aoi/enums.py
--rwxrwxrwx   0 egor      (1000) egor      (1000)      248 2024-01-31 16:55:04.000000 open_aoi-0.0.5/src/open_aoi/exceptions.py
-drwxrwxrwx   0 egor      (1000) egor      (1000)        0 2024-02-11 14:59:23.476556 open_aoi-0.0.5/src/open_aoi/mixins/
--rwxrwxrwx   0 egor      (1000) egor      (1000)     1487 2024-02-11 14:56:07.000000 open_aoi-0.0.5/src/open_aoi/mixins/accessor.py
--rwxrwxrwx   0 egor      (1000) egor      (1000)      283 2024-01-29 20:43:20.000000 open_aoi-0.0.5/src/open_aoi/mixins/camera.py
--rwxrwxrwx   0 egor      (1000) egor      (1000)      332 2024-01-25 20:15:36.000000 open_aoi-0.0.5/src/open_aoi/mixins/control_zone.py
--rwxrwxrwx   0 egor      (1000) egor      (1000)      178 2024-01-29 20:51:45.000000 open_aoi-0.0.5/src/open_aoi/mixins/inspection_profile.py
--rwxrwxrwx   0 egor      (1000) egor      (1000)       88 2024-01-29 20:03:42.000000 open_aoi-0.0.5/src/open_aoi/mixins/inspection_record.py
--rwxrwxrwx   0 egor      (1000) egor      (1000)      405 2024-02-11 14:57:45.000000 open_aoi-0.0.5/src/open_aoi/mixins/template.py
--rwxrwxrwx   0 egor      (1000) egor      (1000)     9604 2024-02-11 14:55:46.000000 open_aoi-0.0.5/src/open_aoi/models.py
-drwxrwxrwx   0 egor      (1000) egor      (1000)        0 2024-02-11 14:59:23.481407 open_aoi-0.0.5/src/open_aoi/scripts/
--rwxrwxrwx   0 egor      (1000) egor      (1000)      126 2024-02-11 14:55:57.000000 open_aoi-0.0.5/src/open_aoi/scripts/db_create_all.py
--rwxrwxrwx   0 egor      (1000) egor      (1000)     3077 2024-02-11 14:56:03.000000 open_aoi-0.0.5/src/open_aoi/scripts/db_create_assets.py
--rwxrwxrwx   0 egor      (1000) egor      (1000)     1056 2024-02-11 14:13:27.000000 open_aoi-0.0.5/src/open_aoi/settings.py
-drwxrwxrwx   0 egor      (1000) egor      (1000)        0 2024-02-11 14:59:23.494786 open_aoi-0.0.5/src/open_aoi.egg-info/
--rwxrwxrwx   0 egor      (1000) egor      (1000)     1531 2024-02-11 14:59:23.000000 open_aoi-0.0.5/src/open_aoi.egg-info/PKG-INFO
--rwxrwxrwx   0 egor      (1000) egor      (1000)      859 2024-02-11 14:59:23.000000 open_aoi-0.0.5/src/open_aoi.egg-info/SOURCES.txt
--rwxrwxrwx   0 egor      (1000) egor      (1000)        1 2024-02-11 14:59:23.000000 open_aoi-0.0.5/src/open_aoi.egg-info/dependency_links.txt
--rwxrwxrwx   0 egor      (1000) egor      (1000)       84 2024-02-11 14:59:23.000000 open_aoi-0.0.5/src/open_aoi.egg-info/requires.txt
--rwxrwxrwx   0 egor      (1000) egor      (1000)       32 2024-02-11 14:59:23.000000 open_aoi-0.0.5/src/open_aoi.egg-info/top_level.txt
-drwxrwxrwx   0 egor      (1000) egor      (1000)        0 2024-02-11 14:59:23.483438 open_aoi-0.0.5/src/open_aoi_web_interface/
--rwxrwxrwx   0 egor      (1000) egor      (1000)      408 2024-02-11 14:54:33.000000 open_aoi-0.0.5/src/open_aoi_web_interface/main.py
-drwxrwxrwx   0 egor      (1000) egor      (1000)        0 2024-02-11 14:59:23.492331 open_aoi-0.0.5/src/open_aoi_web_interface/views/
--rwxrwxrwx   0 egor      (1000) egor      (1000)        0 2024-01-31 18:46:16.000000 open_aoi-0.0.5/src/open_aoi_web_interface/views/__init__.py
--rwxrwxrwx   0 egor      (1000) egor      (1000)     2777 2024-02-11 14:54:48.000000 open_aoi-0.0.5/src/open_aoi_web_interface/views/common.py
--rwxrwxrwx   0 egor      (1000) egor      (1000)      730 2024-02-11 14:55:02.000000 open_aoi-0.0.5/src/open_aoi_web_interface/views/utils.py
--rwxrwxrwx   0 egor      (1000) egor      (1000)     2873 2024-02-11 14:55:09.000000 open_aoi-0.0.5/src/open_aoi_web_interface/views/view_access.py
--rwxrwxrwx   0 egor      (1000) egor      (1000)      574 2024-02-11 14:55:13.000000 open_aoi-0.0.5/src/open_aoi_web_interface/views/view_home.py
+drwxrwxrwx   0 egor      (1000) egor      (1000)        0 2024-04-06 14:23:23.355785 open_aoi-0.0.6/
+-rwxrwxrwx   0 egor      (1000) egor      (1000)     1073 2024-02-13 20:04:15.000000 open_aoi-0.0.6/LICENSE
+-rwxrwxrwx   0 egor      (1000) egor      (1000)     1571 2024-04-06 14:23:23.352948 open_aoi-0.0.6/PKG-INFO
+-rwxrwxrwx   0 egor      (1000) egor      (1000)      739 2024-03-17 13:58:48.000000 open_aoi-0.0.6/README.md
+-rwxrwxrwx   0 egor      (1000) egor      (1000)      804 2024-04-06 14:22:09.000000 open_aoi-0.0.6/pyproject.toml
+-rwxrwxrwx   0 egor      (1000) egor      (1000)       38 2024-04-06 14:23:23.356003 open_aoi-0.0.6/setup.cfg
+drwxrwxrwx   0 egor      (1000) egor      (1000)        0 2024-04-06 14:23:23.275804 open_aoi-0.0.6/src/
+drwxrwxrwx   0 egor      (1000) egor      (1000)        0 2024-04-06 14:23:23.295027 open_aoi-0.0.6/src/open_aoi/
+drwxrwxrwx   0 egor      (1000) egor      (1000)        0 2024-04-06 14:23:23.320807 open_aoi-0.0.6/src/open_aoi/controllers/
+-rwxrwxrwx   0 egor      (1000) egor      (1000)     1948 2024-04-05 15:36:57.000000 open_aoi-0.0.6/src/open_aoi/controllers/__init__.py
+-rwxrwxrwx   0 egor      (1000) egor      (1000)      818 2024-04-04 17:14:57.000000 open_aoi-0.0.6/src/open_aoi/controllers/accessor.py
+-rwxrwxrwx   0 egor      (1000) egor      (1000)      741 2024-04-04 16:54:52.000000 open_aoi-0.0.6/src/open_aoi/controllers/camera.py
+-rwxrwxrwx   0 egor      (1000) egor      (1000)     2052 2024-04-05 15:34:51.000000 open_aoi-0.0.6/src/open_aoi/controllers/control_handler.py
+-rwxrwxrwx   0 egor      (1000) egor      (1000)      821 2024-04-04 19:19:04.000000 open_aoi-0.0.6/src/open_aoi/controllers/defect_type.py
+-rwxrwxrwx   0 egor      (1000) egor      (1000)      180 2024-04-04 17:00:36.000000 open_aoi-0.0.6/src/open_aoi/controllers/inspection.py
+drwxrwxrwx   0 egor      (1000) egor      (1000)        0 2024-04-06 14:23:23.325125 open_aoi-0.0.6/src/open_aoi/controllers/ros_services/
+-rwxrwxrwx   0 egor      (1000) egor      (1000)      985 2024-04-05 20:11:53.000000 open_aoi-0.0.6/src/open_aoi/controllers/ros_services/__init__.py
+-rwxrwxrwx   0 egor      (1000) egor      (1000)     1524 2024-04-05 19:35:47.000000 open_aoi-0.0.6/src/open_aoi/controllers/ros_services/image_acquisition.py
+-rwxrwxrwx   0 egor      (1000) egor      (1000)      690 2024-04-04 17:00:39.000000 open_aoi-0.0.6/src/open_aoi/controllers/template.py
+-rwxrwxrwx   0 egor      (1000) egor      (1000)      251 2024-04-04 18:39:54.000000 open_aoi-0.0.6/src/open_aoi/enums.py
+-rwxrwxrwx   0 egor      (1000) egor      (1000)      489 2024-04-05 18:36:15.000000 open_aoi-0.0.6/src/open_aoi/exceptions.py
+drwxrwxrwx   0 egor      (1000) egor      (1000)        0 2024-04-06 14:23:23.346962 open_aoi-0.0.6/src/open_aoi/mixins/
+-rwxrwxrwx   0 egor      (1000) egor      (1000)       25 2024-04-04 17:11:38.000000 open_aoi-0.0.6/src/open_aoi/mixins/__init__.py
+-rwxrwxrwx   0 egor      (1000) egor      (1000)     2072 2024-04-04 16:41:47.000000 open_aoi-0.0.6/src/open_aoi/mixins/accessor.py
+-rwxrwxrwx   0 egor      (1000) egor      (1000)      337 2024-04-04 16:41:27.000000 open_aoi-0.0.6/src/open_aoi/mixins/camera.py
+-rwxrwxrwx   0 egor      (1000) egor      (1000)     4096 2024-04-05 15:32:22.000000 open_aoi-0.0.6/src/open_aoi/mixins/control_handler.py
+-rwxrwxrwx   0 egor      (1000) egor      (1000)      223 2024-04-04 16:58:21.000000 open_aoi-0.0.6/src/open_aoi/mixins/control_zone.py
+-rwxrwxrwx   0 egor      (1000) egor      (1000)      151 2024-04-04 17:02:30.000000 open_aoi-0.0.6/src/open_aoi/mixins/inspection.py
+-rwxrwxrwx   0 egor      (1000) egor      (1000)      341 2024-04-04 17:04:08.000000 open_aoi-0.0.6/src/open_aoi/mixins/template.py
+-rwxrwxrwx   0 egor      (1000) egor      (1000)    11567 2024-04-04 20:39:34.000000 open_aoi-0.0.6/src/open_aoi/models.py
+drwxrwxrwx   0 egor      (1000) egor      (1000)        0 2024-04-06 14:23:23.349757 open_aoi-0.0.6/src/open_aoi/scripts/
+-rwxrwxrwx   0 egor      (1000) egor      (1000)      160 2024-04-01 17:53:57.000000 open_aoi-0.0.6/src/open_aoi/scripts/db_create_all.py
+-rwxrwxrwx   0 egor      (1000) egor      (1000)     3046 2024-04-04 20:16:21.000000 open_aoi-0.0.6/src/open_aoi/scripts/db_create_assets.py
+-rwxrwxrwx   0 egor      (1000) egor      (1000)     1449 2024-04-05 18:21:36.000000 open_aoi-0.0.6/src/open_aoi/settings.py
+drwxrwxrwx   0 egor      (1000) egor      (1000)        0 2024-04-06 14:23:23.351305 open_aoi-0.0.6/src/open_aoi.egg-info/
+-rwxrwxrwx   0 egor      (1000) egor      (1000)     1571 2024-04-06 14:23:23.000000 open_aoi-0.0.6/src/open_aoi.egg-info/PKG-INFO
+-rwxrwxrwx   0 egor      (1000) egor      (1000)     1000 2024-04-06 14:23:23.000000 open_aoi-0.0.6/src/open_aoi.egg-info/SOURCES.txt
+-rwxrwxrwx   0 egor      (1000) egor      (1000)        1 2024-04-06 14:23:23.000000 open_aoi-0.0.6/src/open_aoi.egg-info/dependency_links.txt
+-rwxrwxrwx   0 egor      (1000) egor      (1000)       97 2024-04-06 14:23:23.000000 open_aoi-0.0.6/src/open_aoi.egg-info/requires.txt
+-rwxrwxrwx   0 egor      (1000) egor      (1000)        9 2024-04-06 14:23:23.000000 open_aoi-0.0.6/src/open_aoi.egg-info/top_level.txt
```

### Comparing `open_aoi-0.0.5/LICENSE` & `open_aoi-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `open_aoi-0.0.5/PKG-INFO` & `open_aoi-0.0.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open_aoi
-Version: 0.0.5
+Version: 0.0.6
 Summary: Support python package for Open AOI system project.
 Author-email: Cherniaev Egor <chrnyaevek@gmail.com>
 Project-URL: Homepage, https://github.com/ChrnyaevEK/open-aoi
 Project-URL: Issues, https://github.com/ChrnyaevEK/open-aoi/issues
 Keywords: automated optical inspection,pcb,computer vision
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -16,14 +16,16 @@
 Requires-Dist: opencv-python
 Requires-Dist: nicegui
 Requires-Dist: roslibpy
 Requires-Dist: sqlalchemy
 Requires-Dist: pymysql
 Requires-Dist: cryptography
 Requires-Dist: bcrypt
+Requires-Dist: pillow
+Requires-Dist: minio
 
 # Welcome to Open AOI!
 This is a support package for [Open AOI project](https://github.com/ChrnyaevEK/open-aoi-system).
 
 Open AOI is ROS2 powered Automated Optical Inspection framework, developed as part of my master thesis at **BUT Brno** university. Project aims to provide development environment for PCB optical inspection tasks in production. Project targets **Raspberry Pi** platform yet it is possible to use any other general purpose computer. Project use **docker** and **Nice GUI** for frontend.
 
 
@@ -33,9 +35,9 @@
 Start web server with the following command.
 ```
 python -m open_aoi_web_interface.main
 ```
 
 ## Run GPIO service
 ```
-python -m -m open_aoi_gpio_interface.main
+python -m open_aoi_gpio_interface.main
 ```
```

### Comparing `open_aoi-0.0.5/README.md` & `open_aoi-0.0.6/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -10,9 +10,9 @@
 Start web server with the following command.
 ```
 python -m open_aoi_web_interface.main
 ```
 
 ## Run GPIO service
 ```
-python -m -m open_aoi_gpio_interface.main
+python -m open_aoi_gpio_interface.main
 ```
```

### Comparing `open_aoi-0.0.5/pyproject.toml` & `open_aoi-0.0.6/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "open_aoi"
-version="0.0.5"
+version="0.0.6"
 authors = [
   { name="Cherniaev Egor", email="chrnyaevek@gmail.com" },
 ]
 description = "Support python package for Open AOI system project."
 keywords=["automated optical inspection", "pcb", "computer vision"]
 readme = "README.md"
 requires-python = ">=3.7"
-dependencies = ["python-dotenv", "opencv-python", "nicegui", "roslibpy", "sqlalchemy", "pymysql", "cryptography", "bcrypt"]
+dependencies = ["python-dotenv", "opencv-python", "nicegui", "roslibpy", "sqlalchemy", "pymysql", "cryptography", "bcrypt", "pillow", "minio"]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
```

### Comparing `open_aoi-0.0.5/src/open_aoi/mixins/accessor.py` & `open_aoi-0.0.6/src/open_aoi/mixins/accessor.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,45 +1,61 @@
 import bcrypt
 
 from open_aoi.exceptions import AuthException
+from open_aoi.mixins import Mixin
 
 
-class Mixin:
-    id: int
-    hash: str
+class AccessorAuthMixin(Mixin):
+    """Basic authentication"""
 
-    @staticmethod
-    def _hash_password(password: str) -> str:
-        """Convert password to hash"""
-        salt = bcrypt.gensalt()
-        return bcrypt.hashpw(password.encode(), salt).decode()
+    hash: str
 
     def set_password(self, password: str) -> None:
         """Override stored hash with new one"""
         self.hash = self._hash_password(password)
 
     def test_credentials(self, password: str) -> None:
         """Test password against stored hash"""
 
         try:
             assert bcrypt.checkpw(password.encode(), self.hash.encode())
         except AssertionError as e:
             raise AuthException("Credential test failed") from e
 
-    def assert_access(self, storage: dict):
+    @staticmethod
+    def _hash_password(password: str) -> str:
+        """Convert password to hash"""
+        salt = bcrypt.gensalt()
+        return bcrypt.hashpw(password.encode(), salt).decode()
+
+
+class AccessorSessionCredentialsMixin(Mixin):
+    """Server side credentials"""
+
+    def assert_session_access(self, storage: dict):
         """Test storage record for access granted in past"""
         try:
             assert storage["access_allowed"]
             assert storage["accessor"] == self.id
         except (AssertionError, KeyError) as e:
             raise AuthException("Access assertion failed") from e
 
-    def grant_access(self, storage: dict):
+    def grant_session_access(self, storage: dict):
         """Push flags and metadata to app store to reflect access has been granted to accessor in past"""
         storage["access_allowed"] = True
         storage["accessor"] = self.id
 
     @staticmethod
-    def revoke_access(storage: dict):
+    def identify_session_access(storage: dict) -> int:
+        """Return id of accessor if access is allowed and record exist"""
+        try:
+            assert storage["access_allowed"]
+            assert storage["accessor"] is not None
+        except (AssertionError, KeyError) as e:
+            raise AuthException("Access assertion failed") from e
+        return storage["accessor"]
+
+    @staticmethod
+    def revoke_session_access(storage: dict):
         """Remove access flags and metadata from session"""
         del storage["access_allowed"]
         del storage["accessor"]
```

### Comparing `open_aoi-0.0.5/src/open_aoi/models.py` & `open_aoi-0.0.6/src/open_aoi/models.py`

 * *Files 22% similar despite different names*

```diff
@@ -10,40 +10,40 @@
     Boolean,
     Integer,
     MetaData,
 )
 from sqlalchemy import create_engine
 from sqlalchemy.orm import Mapped, mapped_column, DeclarativeBase, relationship
 
-from open_aoi.settings import (
-    MYSQL_DATABASE,
-    MYSQL_PASSWORD,
-    MYSQL_USER,
-    MYSQL_PORT
-)
-from open_aoi.enums import DefectTypeEnum, RoleEnum, AccessorEnum
-from open_aoi.mixins.control_zone import Mixin as ControlZoneMixin
-from open_aoi.mixins.accessor import Mixin as AccessorMixin
-from open_aoi.mixins.inspection_record import Mixin as InspectionRecordMixin
-from open_aoi.mixins.template import Mixin as TemplateMixin
-from open_aoi.mixins.camera import Mixin as CameraMixin
-from open_aoi.mixins.inspection_profile import Mixin as InspectionProfileMixin
+from open_aoi.settings import MYSQL_DATABASE, MYSQL_PASSWORD, MYSQL_USER, MYSQL_PORT
+from open_aoi.enums import RoleEnum, AccessorEnum
+from open_aoi.mixins.control_zone import ImageManipulationMixin
+from open_aoi.mixins.accessor import AccessorAuthMixin, AccessorSessionCredentialsMixin
+from open_aoi.mixins.inspection import InspectionStatisticsMixin
+from open_aoi.mixins.template import ImageSourceMixin
+from open_aoi.mixins.camera import CameraControlMixin
+from open_aoi.mixins.control_handler import ModuleSourceMixin
 
 
-class Base(DeclarativeBase):
-    pass
+CODE_LIMIT = 100
+TITLE_LIMIT = 200
+DESCRIPTION_LIMIT = 500
 
 
 metadata_obj = MetaData()
 engine = create_engine(
     f"mysql+pymysql://{MYSQL_USER}:{MYSQL_PASSWORD}@localhost:{MYSQL_PORT}/{MYSQL_DATABASE}"
 )
 
 
-class Role(Base):
+class Base(DeclarativeBase):
+    pass
+
+
+class RoleModel(Base):
     """Define accessor rights"""
 
     __tablename__ = "Role"
     metadata = metadata_obj
 
     id: Mapped[int] = mapped_column(
         primary_key=True, nullable=False, autoincrement=True
@@ -73,229 +73,284 @@
     allow_system_operations: Mapped[bool] = mapped_column(
         Boolean(), default=False, nullable=False
     )
     allow_statistics_view: Mapped[bool] = mapped_column(
         Boolean(), default=False, nullable=False
     )
 
-    accessor_list: Mapped[List["Accessor"]] = relationship(back_populates="role")
+    accessor_list: Mapped[List["AccessorModel"]] = relationship(back_populates="role")
     registry = RoleEnum
 
 
-class Accessor(Base, AccessorMixin):
+class AccessorModel(Base, AccessorAuthMixin, AccessorSessionCredentialsMixin):
     __tablename__ = "Accessor"
     metadata = metadata_obj
 
     id: Mapped[int] = mapped_column(
         primary_key=True, nullable=False, autoincrement=True
     )
 
+    username: Mapped[str] = mapped_column(String(50), nullable=False)
     title: Mapped[str] = mapped_column(String(50), nullable=False)
     description: Mapped[str] = mapped_column(String(200), nullable=False)
 
     role_id: Mapped[int] = mapped_column(ForeignKey("Role.id"), nullable=False)
-    role: Mapped["Role"] = relationship()
+    role: Mapped["RoleModel"] = relationship()
 
     hash: Mapped[str] = mapped_column(String(60), nullable=False)
     registry = AccessorEnum
 
 
-class DefectType(Base):
+class DefectTypeModel(Base):
     """Define system wide known error types"""
 
     __tablename__ = "DefectType"
     metadata = metadata_obj
 
     id: Mapped[int] = mapped_column(primary_key=True, autoincrement=True)
 
     title: Mapped[str] = mapped_column(String(50), nullable=False)
     description: Mapped[str] = mapped_column(String(200), nullable=False)
 
-    registry = DefectTypeEnum
+    control_handler_list: Mapped[List["ControlHandlerModel"]] = relationship(
+        back_populates="defect_type"
+    )
+
+
+class ControlHandlerModel(Base, ModuleSourceMixin):
+    """Database representation of control handler"""
+
+    __tablename__ = "ControlHandler"
+    metadata = metadata_obj
+
+    id: Mapped[int] = mapped_column(primary_key=True, autoincrement=True)
 
+    title: Mapped[str] = mapped_column(String(50), nullable=False)
+    description: Mapped[str] = mapped_column(String(200), nullable=False)
 
-class ControlTarget(Base):
+    handler_blob: Mapped[str] = mapped_column(
+        String(100), nullable=True
+    )  # If null, should not be used!
+
+    control_target_list: Mapped[List["ControlTargetModel"]] = relationship(
+        back_populates="control_handler"
+    )
+
+    defect_type_id: Mapped[int] = mapped_column(
+        ForeignKey("DefectType.id"), nullable=False
+    )
+    defect_type: Mapped["DefectTypeModel"] = relationship(
+        back_populates="control_handler_list"
+    )
+
+
+class ControlTargetModel(Base):
     """
-    Helper object to map defect type to search for in test image to the control zone.
-    Multiple control targets are allowed for single control zone (unique)
+    Helper object to map control handler to the control zone (control handler is unique).
+    Multiple control targets are allowed for single control zone.
     """
 
     __tablename__ = "ControlTarget"
     metadata = metadata_obj
 
     id: Mapped[int] = mapped_column(primary_key=True, autoincrement=True)
 
-    defect_type_id: Mapped[int] = mapped_column(
-        ForeignKey("DefectType.id"), nullable=False
+    control_handler_id: Mapped[int] = mapped_column(
+        ForeignKey("ControlHandler.id"), nullable=False
+    )
+    control_handler: Mapped["ControlHandlerModel"] = relationship(
+        back_populates="control_target_list"
     )
-    defect_type: Mapped["DefectType"] = relationship()
 
     control_zone_id: Mapped[int] = mapped_column(
         ForeignKey("ControlZone.id"), nullable=False
     )
-    control_zone: Mapped["ControlZone"] = relationship(
+    control_zone: Mapped["ControlZoneModel"] = relationship(
         back_populates="control_target_list"
     )
 
 
-class ControlZone(Base, ControlZoneMixin):
+class ConnectedComponentModel(Base):
+    """
+    Location description for control zone
+    """
+
+    __tablename__ = "ConnectedComponent"
+    metadata = metadata_obj
+
+    id: Mapped[int] = mapped_column(primary_key=True, autoincrement=True)
+
+    stat_left: Mapped[int] = mapped_column(Integer, nullable=False)
+    stat_top: Mapped[int] = mapped_column(Integer, nullable=False)
+    stat_width: Mapped[int] = mapped_column(Integer, nullable=False)
+    stat_height: Mapped[int] = mapped_column(Integer, nullable=False)
+
+    control_zone_id: Mapped[int] = mapped_column(
+        ForeignKey("ControlZone.id"), nullable=False
+    )
+    control_zone: Mapped["ControlZoneModel"] = relationship(back_populates="cc")
+
+
+class ControlZoneModel(Base, ImageManipulationMixin):
     """
-    Small zone on template where related defect type detection is conducted
+    Small zone on template where related control handler is applied in order to detect defect type
     """
 
     __tablename__ = "ControlZone"
     metadata = metadata_obj
 
     id: Mapped[int] = mapped_column(primary_key=True, autoincrement=True)
 
     template_id: Mapped[int] = mapped_column(ForeignKey("Template.id"), nullable=False)
-    template: Mapped["Template"] = relationship(back_populates="control_zone_list")
+    template: Mapped["TemplateModel"] = relationship(back_populates="control_zone_list")
 
-    top_left_x: Mapped[float] = mapped_column(Numeric(precision=10, scale=2))
-    top_left_y: Mapped[float] = mapped_column(Numeric(precision=10, scale=2))
+    cc: Mapped["ConnectedComponentModel"] = relationship(back_populates="control_zone")
 
-    bottom_right_x: Mapped[float] = mapped_column(Numeric(precision=10, scale=2))
-    bottom_right_y: Mapped[float] = mapped_column(Numeric(precision=10, scale=2))
+    rotation: Mapped[float] = mapped_column(Numeric(precision=10, scale=2))
 
-    control_target_list: Mapped[List["ControlTarget"]] = relationship(
-        back_populates="control_zone", cascade="all, delete"
+    control_target_list: Mapped[List["ControlTargetModel"]] = relationship(
+        back_populates="control_zone"
     )
 
     created_at: Mapped[datetime] = mapped_column(DateTime, server_default=func.now())
     created_by_accessor_id: Mapped[int] = mapped_column(
         ForeignKey("Accessor.id"), nullable=False
     )
-    created_by: Mapped["Accessor"] = relationship()
+    created_by: Mapped["AccessorModel"] = relationship()
 
 
-class Defect(Base):
+class ControlLogModel(Base):
     """
-    Helper to map defect type that was found to control zone. Multiple defects are allowed.
+    Helper to map defect type that was found to control zone. Multiple control logs are allowed.
     """
 
-    __tablename__ = "Defect"
+    __tablename__ = "ControlLog"
     metadata = metadata_obj
 
     id: Mapped[int] = mapped_column(primary_key=True, autoincrement=True)
 
-    defect_type_id: Mapped[int] = mapped_column(
-        ForeignKey("DefectType.id"), nullable=False
+    control_target_id: Mapped[int] = mapped_column(
+        ForeignKey("ControlTarget.id"), nullable=False
     )
-    defect_type: Mapped["DefectType"] = relationship()
-
-    inspection_record_id: Mapped[int] = mapped_column(
-        ForeignKey("InspectionRecord.id"), nullable=False
+    control_target: Mapped["ControlTargetModel"] = relationship()
+    passed: Mapped[bool] = mapped_column(Boolean(), default=False, nullable=False)
+    log: Mapped[str] = mapped_column(String(200), nullable=True)
+    inspection_id: Mapped[int] = mapped_column(
+        ForeignKey("Inspection.id"), nullable=False
     )
-    inspection_record: Mapped["InspectionRecord"] = relationship(
-        back_populates="defect_list"
+    inspection: Mapped["InspectionModel"] = relationship(
+        back_populates="control_log_list"
     )
 
 
-class InspectionRecord(Base, InspectionRecordMixin):
+class InspectionModel(Base, InspectionStatisticsMixin):
     """
     Connect defect collection with template
     """
 
-    __tablename__ = "InspectionRecord"
+    __tablename__ = "Inspection"
     metadata = metadata_obj
 
     id: Mapped[int] = mapped_column(primary_key=True, autoincrement=True)
 
-    template_id: Mapped[int] = mapped_column(ForeignKey("Template.id"), nullable=False)
-    template: Mapped["Template"] = relationship(back_populates="inspection_record_list")
+    image_blob: Mapped[str] = mapped_column(String(100), nullable=False)
 
-    defect_list: Mapped[List["Defect"]] = relationship(
-        back_populates="inspection_record", cascade="all, delete"
+    inspection_profile_id: Mapped[int] = mapped_column(
+        ForeignKey("InspectionProfile.id"), nullable=False
+    )
+    inspection_profile: Mapped["InspectionProfileModel"] = relationship(
+        back_populates="inspection_list"
+    )
+
+    control_log_list: Mapped[List["ControlLogModel"]] = relationship(
+        back_populates="inspection"
     )
 
     created_at: Mapped[datetime] = mapped_column(DateTime, server_default=func.now())
 
 
-class Template(Base, TemplateMixin):
+class TemplateModel(Base, ImageSourceMixin):
     """
     Main reference image. Aggregate control zones.
     """
 
     __tablename__ = "Template"
     metadata = metadata_obj
 
     id: Mapped[int] = mapped_column(primary_key=True, autoincrement=True)
-    is_active: Mapped[bool] = mapped_column(Boolean(), default=False, nullable=False)
+    title: Mapped[str] = mapped_column(String(TITLE_LIMIT), nullable=False)
 
-    image_uid: Mapped[str] = mapped_column(String(100), nullable=False)
+    image_blob: Mapped[str] = mapped_column(String(100), nullable=False)
 
-    control_zone_list: Mapped[List["ControlZone"]] = relationship(
-        back_populates="template", cascade="all, delete"
+    control_zone_list: Mapped[List["ControlZoneModel"]] = relationship(
+        back_populates="template"
     )
 
-    inspection_record_list: Mapped[List["InspectionRecord"]] = relationship(
-        back_populates="template", cascade="all, delete"
-    )
-
-    inspection_profile_id: Mapped[int] = mapped_column(
-        ForeignKey("InspectionProfile.id"), nullable=False
-    )
-    inspection_profile: Mapped["InspectionProfile"] = relationship(
-        back_populates="template_list"
+    inspection_profile_list: Mapped["InspectionProfileModel"] = relationship(
+        back_populates="template"
     )
 
     created_at: Mapped[datetime] = mapped_column(DateTime, server_default=func.now())
     created_by_accessor_id: Mapped[int] = mapped_column(
         ForeignKey("Accessor.id"), nullable=False
     )
-    created_by: Mapped["Accessor"] = relationship()
+    created_by: Mapped["AccessorModel"] = relationship()
 
 
-class Camera(Base, CameraMixin):
+class CameraModel(Base, CameraControlMixin):
     """
     Represent available cameras
     """
 
     __tablename__ = "Camera"
     metadata = metadata_obj
 
     id: Mapped[int] = mapped_column(primary_key=True, autoincrement=True)
 
-    title: Mapped[str] = mapped_column(String(200), nullable=False)
-    description: Mapped[str] = mapped_column(String(500), nullable=False)
+    title: Mapped[str] = mapped_column(String(TITLE_LIMIT), nullable=False)
+    description: Mapped[str] = mapped_column(String(DESCRIPTION_LIMIT), nullable=False)
 
     # TODO: insert validation ipv4
     ip_address: Mapped[str] = mapped_column(String(15), nullable=False)
-    port: Mapped[str] = mapped_column(Integer, nullable=False)
 
     created_at: Mapped[datetime] = mapped_column(DateTime, server_default=func.now())
     created_by_accessor_id: Mapped[int] = mapped_column(
         ForeignKey("Accessor.id"), nullable=False
     )
-    created_by: Mapped["Accessor"] = relationship()
+    created_by: Mapped["AccessorModel"] = relationship()
 
 
-class InspectionProfile(Base, InspectionProfileMixin):
+class InspectionProfileModel(Base):
     """
     Concrete instance of desired test configuration
     """
 
     __tablename__ = "InspectionProfile"
     metadata = metadata_obj
 
     id: Mapped[int] = mapped_column(primary_key=True, autoincrement=True)
+    is_active: Mapped[bool] = mapped_column(Boolean, nullable=False, default=False)
 
-    title: Mapped[str] = mapped_column(String(200), nullable=False)
-    description: Mapped[str] = mapped_column(String(500), nullable=False)
-
-    identification_code: Mapped[str] = mapped_column(String(100), nullable=False)
+    title: Mapped[str] = mapped_column(String(TITLE_LIMIT), nullable=False)
+    description: Mapped[str] = mapped_column(String(DESCRIPTION_LIMIT), nullable=False)
 
-    # Point to all available templates
-    template_list: Mapped[List["Template"]] = relationship(
-        back_populates="inspection_profile", cascade="all, delete"
-    )
+    identification_code: Mapped[str] = mapped_column(String(CODE_LIMIT), nullable=False)
 
     camera_id: Mapped[Optional[int]] = mapped_column(
         ForeignKey("Camera.id"), nullable=True
     )
-    camera: Mapped[Optional["Camera"]] = relationship()
+    camera: Mapped[Optional["CameraModel"]] = relationship()
+
+    template_id: Mapped[Optional[int]] = mapped_column(
+        ForeignKey("Template.id"), nullable=True
+    )
+    template: Mapped[Optional["TemplateModel"]] = relationship()
+
+    inspection_list: Mapped[List["InspectionModel"]] = relationship(
+        back_populates="inspection_profile"
+    )
 
     created_at: Mapped[datetime] = mapped_column(DateTime, server_default=func.now())
     created_by_accessor_id: Mapped[int] = mapped_column(
         ForeignKey("Accessor.id"), nullable=False
     )
-    created_by: Mapped["Accessor"] = relationship()
+    created_by: Mapped["AccessorModel"] = relationship()
```

### Comparing `open_aoi-0.0.5/src/open_aoi/scripts/db_create_assets.py` & `open_aoi-0.0.6/src/open_aoi/scripts/db_create_assets.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,73 +8,72 @@
     AOI_ADMINISTRATOR_INITIAL_PASSWORD,
     AOI_OPERATOR_INITIAL_PASSWORD,
 )
 
 if __name__ == "__main__":
     with Session(engine) as session:
         # Defect types
-        dt_missing_component = DefectType(
-            id=DefectTypeEnum.MISSING_COMPONENT.value,
+        dt_missing_component = DefectTypeModel(
             title="Missing component",
             description="Component is present on template, but is missing on tested image.",
         )
 
-        dt_wrong_component_orientation = DefectType(
-            id=DefectTypeEnum.WRONG_COMPONENT_ORIENTATION.value,
+        dt_wrong_component_orientation = DefectTypeModel(
             title="Wrong component orientation",
             description="Component orientation is different against template.",
         )
 
-        dt_typography = DefectType(
-            id=DefectTypeEnum.TYPOGRAFY.value,
+        dt_typography = DefectTypeModel(
             title="Typografy",
             description="Typografy quality issues.",
         )
 
         # Roles
-        r_operator = Role(
+        r_operator = RoleModel(
             id=RoleEnum.OPERATOR.value,
             allow_system_view=True,
             allow_inspection_log_view=True,
             allow_inspection_details_view=True,
             allow_inspection_flow_control=True,
             allow_accessor_operations=False,
             allow_device_operations=False,
             allow_inspection_profile_operations=False,
             allow_system_operations=False,
             allow_statistics_view=False,
         )
 
-        r_administrator = Role(
+        r_administrator = RoleModel(
             id=RoleEnum.ADMINISTRATOR.value,
             allow_system_view=True,
             allow_inspection_log_view=True,
             allow_inspection_details_view=True,
             allow_inspection_flow_control=True,
             allow_accessor_operations=True,
             allow_device_operations=True,
             allow_inspection_profile_operations=True,
             allow_system_operations=True,
             allow_statistics_view=True,
         )
 
         # Accessors
-        a_operator = Accessor(
+        a_operator = AccessorModel(
             id=AccessorEnum.OPERATOR.value,
-            title="Operator",
+            username="operator",
+            title="Operator (default)",
             description="Operator is capable of basic sytem control including inspection requests.",
             role_id=RoleEnum.OPERATOR.value,
-            hash=Accessor._hash_password(AOI_OPERATOR_INITIAL_PASSWORD),
+            hash=AccessorModel._hash_password(AOI_OPERATOR_INITIAL_PASSWORD),
         )
-        a_administrator = Accessor(
+        a_administrator = AccessorModel(
             id=AccessorEnum.ADMINISTRATOR.value,
-            title="Administrator",
+            username="administrator",
+            title="Administrator (default)",
             description="Administrator is granted full access to system including security section and inspection configuration.",
             role_id=RoleEnum.ADMINISTRATOR.value,
-            hash=Accessor._hash_password(AOI_ADMINISTRATOR_INITIAL_PASSWORD),
+            hash=AccessorModel._hash_password(AOI_ADMINISTRATOR_INITIAL_PASSWORD),
         )
 
         session.add_all(
             [
                 dt_missing_component,
                 dt_wrong_component_orientation,
                 dt_typography,
```

### Comparing `open_aoi-0.0.5/src/open_aoi.egg-info/PKG-INFO` & `open_aoi-0.0.6/src/open_aoi.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open_aoi
-Version: 0.0.5
+Version: 0.0.6
 Summary: Support python package for Open AOI system project.
 Author-email: Cherniaev Egor <chrnyaevek@gmail.com>
 Project-URL: Homepage, https://github.com/ChrnyaevEK/open-aoi
 Project-URL: Issues, https://github.com/ChrnyaevEK/open-aoi/issues
 Keywords: automated optical inspection,pcb,computer vision
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -16,14 +16,16 @@
 Requires-Dist: opencv-python
 Requires-Dist: nicegui
 Requires-Dist: roslibpy
 Requires-Dist: sqlalchemy
 Requires-Dist: pymysql
 Requires-Dist: cryptography
 Requires-Dist: bcrypt
+Requires-Dist: pillow
+Requires-Dist: minio
 
 # Welcome to Open AOI!
 This is a support package for [Open AOI project](https://github.com/ChrnyaevEK/open-aoi-system).
 
 Open AOI is ROS2 powered Automated Optical Inspection framework, developed as part of my master thesis at **BUT Brno** university. Project aims to provide development environment for PCB optical inspection tasks in production. Project targets **Raspberry Pi** platform yet it is possible to use any other general purpose computer. Project use **docker** and **Nice GUI** for frontend.
 
 
@@ -33,9 +35,9 @@
 Start web server with the following command.
 ```
 python -m open_aoi_web_interface.main
 ```
 
 ## Run GPIO service
 ```
-python -m -m open_aoi_gpio_interface.main
+python -m open_aoi_gpio_interface.main
 ```
```

