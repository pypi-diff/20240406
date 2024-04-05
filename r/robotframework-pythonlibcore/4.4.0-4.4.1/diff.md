# Comparing `tmp/robotframework-pythonlibcore-4.4.0.tar.gz` & `tmp/robotframework-pythonlibcore-4.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotframework-pythonlibcore-4.4.0.tar", last modified: Fri Mar 22 20:14:04 2024, max compression
+gzip compressed data, was "robotframework-pythonlibcore-4.4.1.tar", last modified: Fri Apr  5 22:26:56 2024, max compression
```

## Comparing `robotframework-pythonlibcore-4.4.0.tar` & `robotframework-pythonlibcore-4.4.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 tatuaalto   (501) staff       (20)        0 2024-03-22 20:14:04.555016 robotframework-pythonlibcore-4.4.0/
--rw-r--r--   0 tatuaalto   (501) staff       (20)      568 2022-10-15 18:35:51.000000 robotframework-pythonlibcore-4.4.0/COPYRIGHT.txt
--rw-r--r--   0 tatuaalto   (501) staff       (20)    11358 2022-10-15 18:35:51.000000 robotframework-pythonlibcore-4.4.0/LICENSE.txt
--rw-r--r--   0 tatuaalto   (501) staff       (20)       34 2022-10-15 18:35:51.000000 robotframework-pythonlibcore-4.4.0/MANIFEST.in
--rw-r--r--   0 tatuaalto   (501) staff       (20)     8972 2024-03-22 20:14:04.554866 robotframework-pythonlibcore-4.4.0/PKG-INFO
--rw-r--r--   0 tatuaalto   (501) staff       (20)     7788 2024-03-21 20:11:47.000000 robotframework-pythonlibcore-4.4.0/README.md
--rw-r--r--   0 tatuaalto   (501) staff       (20)      742 2024-03-19 19:56:19.000000 robotframework-pythonlibcore-4.4.0/pyproject.toml
--rw-r--r--   0 tatuaalto   (501) staff       (20)       38 2024-03-22 20:14:04.555058 robotframework-pythonlibcore-4.4.0/setup.cfg
--rw-r--r--   0 tatuaalto   (501) staff       (20)     1805 2024-03-22 20:13:08.000000 robotframework-pythonlibcore-4.4.0/setup.py
-drwxr-xr-x   0 tatuaalto   (501) staff       (20)        0 2024-03-22 20:14:04.554189 robotframework-pythonlibcore-4.4.0/src/
-drwxr-xr-x   0 tatuaalto   (501) staff       (20)        0 2024-03-22 20:14:04.554672 robotframework-pythonlibcore-4.4.0/src/robotframework_pythonlibcore.egg-info/
--rw-r--r--   0 tatuaalto   (501) staff       (20)     8972 2024-03-22 20:14:04.000000 robotframework-pythonlibcore-4.4.0/src/robotframework_pythonlibcore.egg-info/PKG-INFO
--rw-r--r--   0 tatuaalto   (501) staff       (20)      315 2024-03-22 20:14:04.000000 robotframework-pythonlibcore-4.4.0/src/robotframework_pythonlibcore.egg-info/SOURCES.txt
--rw-r--r--   0 tatuaalto   (501) staff       (20)        1 2024-03-22 20:14:04.000000 robotframework-pythonlibcore-4.4.0/src/robotframework_pythonlibcore.egg-info/dependency_links.txt
--rw-r--r--   0 tatuaalto   (501) staff       (20)       13 2024-03-22 20:14:04.000000 robotframework-pythonlibcore-4.4.0/src/robotframework_pythonlibcore.egg-info/top_level.txt
--rw-r--r--   0 tatuaalto   (501) staff       (20)    15356 2024-03-22 20:08:12.000000 robotframework-pythonlibcore-4.4.0/src/robotlibcore.py
+drwxr-xr-x   0 tatuaalto   (501) staff       (20)        0 2024-04-05 22:26:56.279165 robotframework-pythonlibcore-4.4.1/
+-rw-r--r--   0 tatuaalto   (501) staff       (20)      568 2022-10-15 18:35:51.000000 robotframework-pythonlibcore-4.4.1/COPYRIGHT.txt
+-rw-r--r--   0 tatuaalto   (501) staff       (20)    11358 2022-10-15 18:35:51.000000 robotframework-pythonlibcore-4.4.1/LICENSE.txt
+-rw-r--r--   0 tatuaalto   (501) staff       (20)       34 2022-10-15 18:35:51.000000 robotframework-pythonlibcore-4.4.1/MANIFEST.in
+-rw-r--r--   0 tatuaalto   (501) staff       (20)     8972 2024-04-05 22:26:56.278946 robotframework-pythonlibcore-4.4.1/PKG-INFO
+-rw-r--r--   0 tatuaalto   (501) staff       (20)     7788 2024-03-21 20:11:47.000000 robotframework-pythonlibcore-4.4.1/README.md
+-rw-r--r--   0 tatuaalto   (501) staff       (20)      742 2024-03-19 19:56:19.000000 robotframework-pythonlibcore-4.4.1/pyproject.toml
+-rw-r--r--   0 tatuaalto   (501) staff       (20)       38 2024-04-05 22:26:56.279207 robotframework-pythonlibcore-4.4.1/setup.cfg
+-rw-r--r--   0 tatuaalto   (501) staff       (20)     1805 2024-03-22 20:13:08.000000 robotframework-pythonlibcore-4.4.1/setup.py
+drwxr-xr-x   0 tatuaalto   (501) staff       (20)        0 2024-04-05 22:26:56.278146 robotframework-pythonlibcore-4.4.1/src/
+drwxr-xr-x   0 tatuaalto   (501) staff       (20)        0 2024-04-05 22:26:56.278772 robotframework-pythonlibcore-4.4.1/src/robotframework_pythonlibcore.egg-info/
+-rw-r--r--   0 tatuaalto   (501) staff       (20)     8972 2024-04-05 22:26:56.000000 robotframework-pythonlibcore-4.4.1/src/robotframework_pythonlibcore.egg-info/PKG-INFO
+-rw-r--r--   0 tatuaalto   (501) staff       (20)      315 2024-04-05 22:26:56.000000 robotframework-pythonlibcore-4.4.1/src/robotframework_pythonlibcore.egg-info/SOURCES.txt
+-rw-r--r--   0 tatuaalto   (501) staff       (20)        1 2024-04-05 22:26:56.000000 robotframework-pythonlibcore-4.4.1/src/robotframework_pythonlibcore.egg-info/dependency_links.txt
+-rw-r--r--   0 tatuaalto   (501) staff       (20)       13 2024-04-05 22:26:56.000000 robotframework-pythonlibcore-4.4.1/src/robotframework_pythonlibcore.egg-info/top_level.txt
+-rw-r--r--   0 tatuaalto   (501) staff       (20)    15868 2024-04-05 22:26:24.000000 robotframework-pythonlibcore-4.4.1/src/robotlibcore.py
```

### Comparing `robotframework-pythonlibcore-4.4.0/COPYRIGHT.txt` & `robotframework-pythonlibcore-4.4.1/COPYRIGHT.txt`

 * *Files identical despite different names*

### Comparing `robotframework-pythonlibcore-4.4.0/LICENSE.txt` & `robotframework-pythonlibcore-4.4.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `robotframework-pythonlibcore-4.4.0/PKG-INFO` & `robotframework-pythonlibcore-4.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-pythonlibcore
-Version: 4.4.0
+Version: 4.4.1
 Summary: Tools to ease creating larger test libraries for Robot Framework using Python.
 Home-page: https://github.com/robotframework/PythonLibCore
 Author: Tatu Aalto
 Author-email: aalto.tatu@gmail.com
 License: Apache License 2.0
 Keywords: robotframework testing testautomation library development
 Platform: any
```

### Comparing `robotframework-pythonlibcore-4.4.0/README.md` & `robotframework-pythonlibcore-4.4.1/README.md`

 * *Files identical despite different names*

### Comparing `robotframework-pythonlibcore-4.4.0/pyproject.toml` & `robotframework-pythonlibcore-4.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `robotframework-pythonlibcore-4.4.0/setup.py` & `robotframework-pythonlibcore-4.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `robotframework-pythonlibcore-4.4.0/src/robotframework_pythonlibcore.egg-info/PKG-INFO` & `robotframework-pythonlibcore-4.4.1/src/robotframework_pythonlibcore.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-pythonlibcore
-Version: 4.4.0
+Version: 4.4.1
 Summary: Tools to ease creating larger test libraries for Robot Framework using Python.
 Home-page: https://github.com/robotframework/PythonLibCore
 Author: Tatu Aalto
 Author-email: aalto.tatu@gmail.com
 License: Apache License 2.0
 Keywords: robotframework testing testautomation library development
 Platform: any
```

### Comparing `robotframework-pythonlibcore-4.4.0/src/robotlibcore.py` & `robotframework-pythonlibcore-4.4.1/src/robotlibcore.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 from typing import Any, Callable, List, Optional, Union, get_type_hints
 
 from robot.api import logger
 from robot.api.deco import keyword  # noqa: F401
 from robot.errors import DataError
 from robot.utils import Importer
 
-__version__ = "4.4.0"
+__version__ = "4.4.1"
 
 
 class PythonLibCoreException(Exception):  # noqa: N818
     pass
 
 
 class PluginError(PythonLibCoreException):
@@ -53,43 +53,55 @@
             except json.decoder.JSONDecodeError:
                 logger.warn(f"Could not convert json file {translation} to dictionary.")
                 return {}
     else:
         return {}
 
 
+def _translated_keywords(translation_data: dict) -> list:
+    return [item.get("name") for item in translation_data.values() if item.get("name")]
+
+
 class HybridCore:
     def __init__(self, library_components: List, translation: Optional[Path] = None) -> None:
         self.keywords = {}
         self.keywords_spec = {}
         self.attributes = {}
         translation_data = _translation(translation)
-        self.add_library_components(library_components, translation_data)
-        self.add_library_components([self], translation_data)
+        translated_kw_names = _translated_keywords(translation_data)
+        self.add_library_components(library_components, translation_data, translated_kw_names)
+        self.add_library_components([self], translation_data, translated_kw_names)
         self.__set_library_listeners(library_components)
 
-    def add_library_components(self, library_components: List, translation: Optional[dict] = None):
+    def add_library_components(
+        self,
+        library_components: List,
+        translation: Optional[dict] = None,
+        translated_kw_names: Optional[list] = None,
+    ):
         translation = translation if translation else {}
+        translated_kw_names = translated_kw_names if translated_kw_names else []
         self.keywords_spec["__init__"] = KeywordBuilder.build(self.__init__, translation)  # type: ignore
         self.__replace_intro_doc(translation)
         for component in library_components:
             for name, func in self.__get_members(component):
                 if callable(func) and hasattr(func, "robot_name"):
                     kw = getattr(component, name)
-                    kw_name = self.__get_keyword_name(func, name, translation)
+                    kw_name = self.__get_keyword_name(func, name, translation, translated_kw_names)
                     self.keywords[kw_name] = kw
                     self.keywords_spec[kw_name] = KeywordBuilder.build(kw, translation)
                     # Expose keywords as attributes both using original
                     # method names as well as possible custom names.
                     self.attributes[name] = self.attributes[kw_name] = kw
 
-    def __get_keyword_name(self, func: Callable, name: str, translation: dict):
-        if name in translation:  # noqa: SIM102
-            if new_name := translation[name].get("name"):
-                return new_name
+    def __get_keyword_name(self, func: Callable, name: str, translation: dict, translated_kw_names: list):
+        if name in translated_kw_names:
+            return name
+        if name in translation and translation[name].get("name"):
+            return translation[name].get("name")
         return func.robot_name or name
 
     def __replace_intro_doc(self, translation: dict):
         if "__intro__" in translation:
             self.__doc__ = translation["__intro__"].get("doc", "")
 
     def __set_library_listeners(self, library_components: list):
```

