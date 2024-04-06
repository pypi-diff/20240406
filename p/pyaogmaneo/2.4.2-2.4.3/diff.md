# Comparing `tmp/pyaogmaneo-2.4.2.tar.gz` & `tmp/pyaogmaneo-2.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyaogmaneo-2.4.2.tar", last modified: Thu Apr  4 20:07:52 2024, max compression
+gzip compressed data, was "pyaogmaneo-2.4.3.tar", last modified: Sat Apr  6 18:43:07 2024, max compression
```

## Comparing `pyaogmaneo-2.4.2.tar` & `pyaogmaneo-2.4.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:07:52.446229 pyaogmaneo-2.4.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:07:52.442229 pyaogmaneo-2.4.2/CMake/
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-04-04 20:07:40.000000 pyaogmaneo-2.4.2/CMake/FindAOgmaNeo.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     2237 2024-04-04 20:07:40.000000 pyaogmaneo-2.4.2/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)    17842 2024-04-04 20:07:40.000000 pyaogmaneo-2.4.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-04 20:07:40.000000 pyaogmaneo-2.4.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-04 20:07:52.446229 pyaogmaneo-2.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-04-04 20:07:40.000000 pyaogmaneo-2.4.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:07:52.446229 pyaogmaneo-2.4.2/pyaogmaneo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-04 20:07:52.000000 pyaogmaneo-2.4.2/pyaogmaneo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-04 20:07:52.000000 pyaogmaneo-2.4.2/pyaogmaneo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 20:07:52.000000 pyaogmaneo-2.4.2/pyaogmaneo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 20:07:52.000000 pyaogmaneo-2.4.2/pyaogmaneo.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-04 20:07:52.000000 pyaogmaneo-2.4.2/pyaogmaneo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-04 20:07:40.000000 pyaogmaneo-2.4.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 20:07:52.446229 pyaogmaneo-2.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4253 2024-04-04 20:07:40.000000 pyaogmaneo-2.4.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:07:52.442229 pyaogmaneo-2.4.2/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:07:52.446229 pyaogmaneo-2.4.2/source/pyaogmaneo/
--rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-04-04 20:07:40.000000 pyaogmaneo-2.4.2/source/pyaogmaneo/py_helpers.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-04-04 20:07:40.000000 pyaogmaneo-2.4.2/source/pyaogmaneo/py_helpers.h
--rw-r--r--   0 runner    (1001) docker     (127)    12600 2024-04-04 20:07:40.000000 pyaogmaneo-2.4.2/source/pyaogmaneo/py_hierarchy.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     7095 2024-04-04 20:07:40.000000 pyaogmaneo-2.4.2/source/pyaogmaneo/py_hierarchy.h
--rw-r--r--   0 runner    (1001) docker     (127)     7846 2024-04-04 20:07:40.000000 pyaogmaneo-2.4.2/source/pyaogmaneo/py_image_encoder.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-04-04 20:07:40.000000 pyaogmaneo-2.4.2/source/pyaogmaneo/py_image_encoder.h
--rw-r--r--   0 runner    (1001) docker     (127)    11694 2024-04-04 20:07:40.000000 pyaogmaneo-2.4.2/source/pyaogmaneo/py_module.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:43:07.476275 pyaogmaneo-2.4.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:43:07.472275 pyaogmaneo-2.4.3/CMake/
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-04-06 18:42:58.000000 pyaogmaneo-2.4.3/CMake/FindAOgmaNeo.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     2237 2024-04-06 18:42:58.000000 pyaogmaneo-2.4.3/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    17842 2024-04-06 18:42:58.000000 pyaogmaneo-2.4.3/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-06 18:42:58.000000 pyaogmaneo-2.4.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-06 18:43:07.476275 pyaogmaneo-2.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-04-06 18:42:58.000000 pyaogmaneo-2.4.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:43:07.476275 pyaogmaneo-2.4.3/pyaogmaneo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-06 18:43:07.000000 pyaogmaneo-2.4.3/pyaogmaneo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-06 18:43:07.000000 pyaogmaneo-2.4.3/pyaogmaneo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 18:43:07.000000 pyaogmaneo-2.4.3/pyaogmaneo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 18:43:07.000000 pyaogmaneo-2.4.3/pyaogmaneo.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-06 18:43:07.000000 pyaogmaneo-2.4.3/pyaogmaneo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-06 18:42:58.000000 pyaogmaneo-2.4.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 18:43:07.476275 pyaogmaneo-2.4.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4253 2024-04-06 18:42:58.000000 pyaogmaneo-2.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:43:07.472275 pyaogmaneo-2.4.3/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:43:07.472275 pyaogmaneo-2.4.3/source/pyaogmaneo/
+-rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-04-06 18:42:58.000000 pyaogmaneo-2.4.3/source/pyaogmaneo/py_helpers.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-04-06 18:42:58.000000 pyaogmaneo-2.4.3/source/pyaogmaneo/py_helpers.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12600 2024-04-06 18:42:58.000000 pyaogmaneo-2.4.3/source/pyaogmaneo/py_hierarchy.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7095 2024-04-06 18:42:58.000000 pyaogmaneo-2.4.3/source/pyaogmaneo/py_hierarchy.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7846 2024-04-06 18:42:58.000000 pyaogmaneo-2.4.3/source/pyaogmaneo/py_image_encoder.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-04-06 18:42:58.000000 pyaogmaneo-2.4.3/source/pyaogmaneo/py_image_encoder.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11694 2024-04-06 18:42:58.000000 pyaogmaneo-2.4.3/source/pyaogmaneo/py_module.cpp
```

### Comparing `pyaogmaneo-2.4.2/CMake/FindAOgmaNeo.cmake` & `pyaogmaneo-2.4.3/CMake/FindAOgmaNeo.cmake`

 * *Files identical despite different names*

### Comparing `pyaogmaneo-2.4.2/CMakeLists.txt` & `pyaogmaneo-2.4.3/CMakeLists.txt`

 * *Files 7% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     find_package(AOgmaNeo)
 else()
     message(STATUS "Not using system installation of AOgmaNeo, will download from repository")
 
     FetchContent_Declare(
         AOgmaNeo
         GIT_REPOSITORY https://github.com/ogmacorp/AOgmaNeo.git
-        GIT_TAG fc1df9371d97d425bd39dbd7d5bcd38a6d718c2c
+        GIT_TAG 3a2ad0f486b83587237789922fe9326ba9b6b03f
     )
 
     FetchContent_MakeAvailable(AOgmaNeo)
 endif()
 
 FetchContent_Declare(
     pybind11
```

### Comparing `pyaogmaneo-2.4.2/LICENSE.md` & `pyaogmaneo-2.4.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyaogmaneo-2.4.2/PKG-INFO` & `pyaogmaneo-2.4.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaogmaneo
-Version: 2.4.2
+Version: 2.4.3
 Summary: Python bindings for the AOgmaNeo library
 Home-page: https://ogmacorp.com/
 Author: Ogma Intelligent Systems Corp
 Author-email: info@ogmacorp.com
 License: Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `pyaogmaneo-2.4.2/README.md` & `pyaogmaneo-2.4.3/README.md`

 * *Files identical despite different names*

### Comparing `pyaogmaneo-2.4.2/pyaogmaneo.egg-info/PKG-INFO` & `pyaogmaneo-2.4.3/pyaogmaneo.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaogmaneo
-Version: 2.4.2
+Version: 2.4.3
 Summary: Python bindings for the AOgmaNeo library
 Home-page: https://ogmacorp.com/
 Author: Ogma Intelligent Systems Corp
 Author-email: info@ogmacorp.com
 License: Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `pyaogmaneo-2.4.2/setup.py` & `pyaogmaneo-2.4.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,15 +84,15 @@
             os.makedirs(self.build_temp)
 
         subprocess.check_call([ 'cmake', ext.sourcedir ] + cmake_args, cwd=self.build_temp, env=env)
         subprocess.check_call([ 'cmake', '--build', '.' ] + build_args, cwd=self.build_temp)
 
 setup(
     name="pyaogmaneo",
-    version="2.4.2",
+    version="2.4.3",
     description="Python bindings for the AOgmaNeo library",
     long_description='https://github.com/ogmacorp/PyAOgmaNeo',
     author='Ogma Intelligent Systems Corp',
     author_email='info@ogmacorp.com',
     url='https://ogmacorp.com/',
     license='Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License',
     classifiers=[
```

### Comparing `pyaogmaneo-2.4.2/source/pyaogmaneo/py_helpers.cpp` & `pyaogmaneo-2.4.3/source/pyaogmaneo/py_helpers.cpp`

 * *Files identical despite different names*

### Comparing `pyaogmaneo-2.4.2/source/pyaogmaneo/py_helpers.h` & `pyaogmaneo-2.4.3/source/pyaogmaneo/py_helpers.h`

 * *Files identical despite different names*

### Comparing `pyaogmaneo-2.4.2/source/pyaogmaneo/py_hierarchy.cpp` & `pyaogmaneo-2.4.3/source/pyaogmaneo/py_hierarchy.cpp`

 * *Files identical despite different names*

### Comparing `pyaogmaneo-2.4.2/source/pyaogmaneo/py_hierarchy.h` & `pyaogmaneo-2.4.3/source/pyaogmaneo/py_hierarchy.h`

 * *Files identical despite different names*

### Comparing `pyaogmaneo-2.4.2/source/pyaogmaneo/py_image_encoder.cpp` & `pyaogmaneo-2.4.3/source/pyaogmaneo/py_image_encoder.cpp`

 * *Files identical despite different names*

### Comparing `pyaogmaneo-2.4.2/source/pyaogmaneo/py_image_encoder.h` & `pyaogmaneo-2.4.3/source/pyaogmaneo/py_image_encoder.h`

 * *Files identical despite different names*

### Comparing `pyaogmaneo-2.4.2/source/pyaogmaneo/py_module.cpp` & `pyaogmaneo-2.4.3/source/pyaogmaneo/py_module.cpp`

 * *Files identical despite different names*

