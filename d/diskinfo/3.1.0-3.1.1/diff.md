# Comparing `tmp/diskinfo-3.1.0.tar.gz` & `tmp/diskinfo-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diskinfo-3.1.0.tar", last modified: Sun Mar 10 21:30:55 2024, max compression
+gzip compressed data, was "diskinfo-3.1.1.tar", last modified: Sat Apr  6 18:59:08 2024, max compression
```

## Comparing `diskinfo-3.1.0.tar` & `diskinfo-3.1.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 21:30:55.926952 diskinfo-3.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-03-10 21:30:52.000000 diskinfo-3.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4040 2024-03-10 21:30:55.926952 diskinfo-3.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-03-10 21:30:52.000000 diskinfo-3.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-03-10 21:30:52.000000 diskinfo-3.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-10 21:30:55.926952 diskinfo-3.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 21:30:55.918952 diskinfo-3.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 21:30:55.922952 diskinfo-3.1.0/src/diskinfo/
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-03-10 21:30:52.000000 diskinfo-3.1.0/src/diskinfo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12838 2024-03-10 21:30:52.000000 diskinfo-3.1.0/src/diskinfo/demo.py
--rw-r--r--   0 runner    (1001) docker     (127)    32708 2024-03-10 21:30:52.000000 diskinfo-3.1.0/src/diskinfo/disk.py
--rw-r--r--   0 runner    (1001) docker     (127)     6477 2024-03-10 21:30:52.000000 diskinfo-3.1.0/src/diskinfo/diskinfo.py
--rw-r--r--   0 runner    (1001) docker     (127)    11792 2024-03-10 21:30:52.000000 diskinfo-3.1.0/src/diskinfo/disksmart.py
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-03-10 21:30:52.000000 diskinfo-3.1.0/src/diskinfo/disktype.py
--rw-r--r--   0 runner    (1001) docker     (127)    29399 2024-03-10 21:30:52.000000 diskinfo-3.1.0/src/diskinfo/partition.py
--rw-r--r--   0 runner    (1001) docker     (127)     9108 2024-03-10 21:30:52.000000 diskinfo-3.1.0/src/diskinfo/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 21:30:55.926952 diskinfo-3.1.0/src/diskinfo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4040 2024-03-10 21:30:55.000000 diskinfo-3.1.0/src/diskinfo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-03-10 21:30:55.000000 diskinfo-3.1.0/src/diskinfo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-10 21:30:55.000000 diskinfo-3.1.0/src/diskinfo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-03-10 21:30:55.000000 diskinfo-3.1.0/src/diskinfo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-10 21:30:55.000000 diskinfo-3.1.0/src/diskinfo.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 21:30:55.926952 diskinfo-3.1.0/test/
--rw-r--r--   0 runner    (1001) docker     (127)    16068 2024-03-10 21:30:52.000000 diskinfo-3.1.0/test/test_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    28453 2024-03-10 21:30:52.000000 diskinfo-3.1.0/test/test_data_smart.py
--rw-r--r--   0 runner    (1001) docker     (127)    37869 2024-03-10 21:30:52.000000 diskinfo-3.1.0/test/test_disk.py
--rw-r--r--   0 runner    (1001) docker     (127)    23188 2024-03-10 21:30:52.000000 diskinfo-3.1.0/test/test_diskinfo.py
--rw-r--r--   0 runner    (1001) docker     (127)     3268 2024-03-10 21:30:52.000000 diskinfo-3.1.0/test/test_disksmart.py
--rw-r--r--   0 runner    (1001) docker     (127)     9973 2024-03-10 21:30:52.000000 diskinfo-3.1.0/test/test_partition.py
--rw-r--r--   0 runner    (1001) docker     (127)     8450 2024-03-10 21:30:52.000000 diskinfo-3.1.0/test/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:59:08.973962 diskinfo-3.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-06 18:59:02.000000 diskinfo-3.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3980 2024-04-06 18:59:08.973962 diskinfo-3.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-04-06 18:59:02.000000 diskinfo-3.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-04-06 18:59:02.000000 diskinfo-3.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 18:59:08.973962 diskinfo-3.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:59:08.965962 diskinfo-3.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:59:08.969962 diskinfo-3.1.1/src/diskinfo/
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-06 18:59:02.000000 diskinfo-3.1.1/src/diskinfo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12838 2024-04-06 18:59:02.000000 diskinfo-3.1.1/src/diskinfo/demo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32708 2024-04-06 18:59:02.000000 diskinfo-3.1.1/src/diskinfo/disk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6477 2024-04-06 18:59:02.000000 diskinfo-3.1.1/src/diskinfo/diskinfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11792 2024-04-06 18:59:02.000000 diskinfo-3.1.1/src/diskinfo/disksmart.py
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-06 18:59:02.000000 diskinfo-3.1.1/src/diskinfo/disktype.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29623 2024-04-06 18:59:02.000000 diskinfo-3.1.1/src/diskinfo/partition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9108 2024-04-06 18:59:02.000000 diskinfo-3.1.1/src/diskinfo/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:59:08.973962 diskinfo-3.1.1/src/diskinfo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3980 2024-04-06 18:59:08.000000 diskinfo-3.1.1/src/diskinfo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-06 18:59:08.000000 diskinfo-3.1.1/src/diskinfo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 18:59:08.000000 diskinfo-3.1.1/src/diskinfo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-06 18:59:08.000000 diskinfo-3.1.1/src/diskinfo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-06 18:59:08.000000 diskinfo-3.1.1/src/diskinfo.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:59:08.969962 diskinfo-3.1.1/test/
+-rw-r--r--   0 runner    (1001) docker     (127)    16068 2024-04-06 18:59:02.000000 diskinfo-3.1.1/test/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28453 2024-04-06 18:59:02.000000 diskinfo-3.1.1/test/test_data_smart.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37869 2024-04-06 18:59:02.000000 diskinfo-3.1.1/test/test_disk.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23188 2024-04-06 18:59:02.000000 diskinfo-3.1.1/test/test_diskinfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3268 2024-04-06 18:59:02.000000 diskinfo-3.1.1/test/test_disksmart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9973 2024-04-06 18:59:02.000000 diskinfo-3.1.1/test/test_partition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8450 2024-04-06 18:59:02.000000 diskinfo-3.1.1/test/test_utils.py
```

### Comparing `diskinfo-3.1.0/LICENSE` & `diskinfo-3.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `diskinfo-3.1.0/PKG-INFO` & `diskinfo-3.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diskinfo
-Version: 3.1.0
+Version: 3.1.1
 Summary: Disk information Python library for Linux
 Author-email: Peter Sulyok <peter@sulyok.net>
 License: MIT License
         
         Copyright (c) 2022 Peter Sulyok
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -49,15 +49,15 @@
 [![Issues](https://img.shields.io/github/issues/petersulyok/diskinfo)](https://github.com/petersulyok/diskinfo/issues)
 [![Supported Python Versions](https://img.shields.io/pypi/pyversions/diskinfo)](https://pypi.org/project/diskinfo)
 [![PyPI version](https://badge.fury.io/py/diskinfo.svg)](https://badge.fury.io/py/diskinfo)
 
 Disk information Python library can assist in collecting disk information on Linux. In more details, it can:
 
 - collect information about a specific disk
-- explore existing disks in the system
+- explore all existing disks in the system
 - translate between traditional and persistent disk names
 - read current disk temperature
 - read SMART data of a disk
 - read partition list of a disk 
 
 Installation
 ------------
@@ -66,16 +66,15 @@
     pip install diskinfo
 
 See the complete list of dependencies and requirements in the 
 [documentation](https://diskinfo.readthedocs.io/en/latest/intro.html#installation). 
 
 Demo
 ----
-The library contains a demo application with multiple screens ([`rich`](https://pypi.org/project/rich)
-needs to be installed):
+The library contains a demo application with multiple screens:
 
     pip install rich
     python -m diskinfo.demo
 
 ![Demo screen](https://github.com/petersulyok/diskinfo/raw/main/docs/diskinfo_rich_demo.png)
 
 See more demo screens in the [documentation](https://diskinfo.readthedocs.io/en/latest/intro.html#demo).
```

### Comparing `diskinfo-3.1.0/README.md` & `diskinfo-3.1.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [![Issues](https://img.shields.io/github/issues/petersulyok/diskinfo)](https://github.com/petersulyok/diskinfo/issues)
 [![Supported Python Versions](https://img.shields.io/pypi/pyversions/diskinfo)](https://pypi.org/project/diskinfo)
 [![PyPI version](https://badge.fury.io/py/diskinfo.svg)](https://badge.fury.io/py/diskinfo)
 
 Disk information Python library can assist in collecting disk information on Linux. In more details, it can:
 
 - collect information about a specific disk
-- explore existing disks in the system
+- explore all existing disks in the system
 - translate between traditional and persistent disk names
 - read current disk temperature
 - read SMART data of a disk
 - read partition list of a disk 
 
 Installation
 ------------
@@ -22,16 +22,15 @@
     pip install diskinfo
 
 See the complete list of dependencies and requirements in the 
 [documentation](https://diskinfo.readthedocs.io/en/latest/intro.html#installation). 
 
 Demo
 ----
-The library contains a demo application with multiple screens ([`rich`](https://pypi.org/project/rich)
-needs to be installed):
+The library contains a demo application with multiple screens:
 
     pip install rich
     python -m diskinfo.demo
 
 ![Demo screen](https://github.com/petersulyok/diskinfo/raw/main/docs/diskinfo_rich_demo.png)
 
 See more demo screens in the [documentation](https://diskinfo.readthedocs.io/en/latest/intro.html#demo).
```

### Comparing `diskinfo-3.1.0/pyproject.toml` & `diskinfo-3.1.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "diskinfo"
 description = "Disk information Python library for Linux"
 readme = "README.md"
-version = "3.1.0"
+version = "3.1.1"
 authors = [
     { name = "Peter Sulyok", email = "peter@sulyok.net" }
 ]
 requires-python = ">=3.8"
 keywords = ["disk", "linux"]
 license = {file = "LICENSE"}
 dependencies = [
@@ -50,15 +50,15 @@
     "unittest.main()"
     ]
 omit = [ "src/diskinfo/demo.py" ]
 
 # pylint options
 [tool.pylint.'MASTER']
 init-hook='import sys; sys.path.append("."); sys.path.append("./src"); sys.path.append("./test")'
-max-line-length=240
+max-line-length=120
 
 [tool.pylint.'MESSAGES CONTROL']
 disable= [
     "line-too-long", "missing-module-docstring", "too-many-locals", "too-many-branches", "too-many-arguments",
     "too-many-statements", "invalid-name", "protected-access", "too-many-instance-attributes",
     "too-many-public-methods", "too-few-public-methods", "duplicate-code"
     ]
```

### Comparing `diskinfo-3.1.0/src/diskinfo/__init__.py` & `diskinfo-3.1.1/src/diskinfo/__init__.py`

 * *Files identical despite different names*

### Comparing `diskinfo-3.1.0/src/diskinfo/demo.py` & `diskinfo-3.1.1/src/diskinfo/demo.py`

 * *Files identical despite different names*

### Comparing `diskinfo-3.1.0/src/diskinfo/disk.py` & `diskinfo-3.1.1/src/diskinfo/disk.py`

 * *Files identical despite different names*

### Comparing `diskinfo-3.1.0/src/diskinfo/diskinfo.py` & `diskinfo-3.1.1/src/diskinfo/diskinfo.py`

 * *Files identical despite different names*

### Comparing `diskinfo-3.1.0/src/diskinfo/disksmart.py` & `diskinfo-3.1.1/src/diskinfo/disksmart.py`

 * *Files identical despite different names*

### Comparing `diskinfo-3.1.0/src/diskinfo/disktype.py` & `diskinfo-3.1.1/src/diskinfo/disktype.py`

 * *Files identical despite different names*

### Comparing `diskinfo-3.1.0/src/diskinfo/partition.py` & `diskinfo-3.1.1/src/diskinfo/partition.py`

 * *Files 0% similar despite different names*

```diff
@@ -109,17 +109,26 @@
         if path_list:
             self.__byuuid_path = path_list[0]
         # other udev properties
         self.__part_scheme = _read_udev_property(path, "ID_PART_ENTRY_SCHEME=")
         self.__part_label = _read_udev_property(path, "ID_PART_ENTRY_NAME=")
         self.__part_uuid = _read_udev_property(path, "ID_PART_ENTRY_UUID=")
         self.__part_type = _read_udev_property(path, "ID_PART_ENTRY_TYPE=")
-        self.__part_number = int(_read_udev_property(path, "ID_PART_ENTRY_NUMBER="))
-        self.__part_offset = int(_read_udev_property(path, "ID_PART_ENTRY_OFFSET="))
-        self.__part_size = int(_read_udev_property(path, "ID_PART_ENTRY_SIZE="))
+        self.__part_number = 0
+        value = _read_udev_property(path, "ID_PART_ENTRY_NUMBER=")
+        if value:
+            self.__part_number = int(value)
+        self.__part_offset = -1
+        value = _read_udev_property(path, "ID_PART_ENTRY_OFFSET=")
+        if value:
+            self.__part_offset = int(value)
+        self.__part_size = 0
+        value = _read_udev_property(path, "ID_PART_ENTRY_SIZE=")
+        if value:
+            self.__part_size = int(value)
         value = _read_udev_property(path, "ID_FS_LABEL_ENC=")
         if value:
             self.__fs_label = value
         else:
             self.__fs_label = _read_udev_property(path, "ID_FS_LABEL=")
         value = _read_udev_property(path, "ID_FS_UUID_ENC=")
         if value:
```

### Comparing `diskinfo-3.1.0/src/diskinfo/utils.py` & `diskinfo-3.1.1/src/diskinfo/utils.py`

 * *Files identical despite different names*

### Comparing `diskinfo-3.1.0/src/diskinfo.egg-info/PKG-INFO` & `diskinfo-3.1.1/src/diskinfo.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diskinfo
-Version: 3.1.0
+Version: 3.1.1
 Summary: Disk information Python library for Linux
 Author-email: Peter Sulyok <peter@sulyok.net>
 License: MIT License
         
         Copyright (c) 2022 Peter Sulyok
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -49,15 +49,15 @@
 [![Issues](https://img.shields.io/github/issues/petersulyok/diskinfo)](https://github.com/petersulyok/diskinfo/issues)
 [![Supported Python Versions](https://img.shields.io/pypi/pyversions/diskinfo)](https://pypi.org/project/diskinfo)
 [![PyPI version](https://badge.fury.io/py/diskinfo.svg)](https://badge.fury.io/py/diskinfo)
 
 Disk information Python library can assist in collecting disk information on Linux. In more details, it can:
 
 - collect information about a specific disk
-- explore existing disks in the system
+- explore all existing disks in the system
 - translate between traditional and persistent disk names
 - read current disk temperature
 - read SMART data of a disk
 - read partition list of a disk 
 
 Installation
 ------------
@@ -66,16 +66,15 @@
     pip install diskinfo
 
 See the complete list of dependencies and requirements in the 
 [documentation](https://diskinfo.readthedocs.io/en/latest/intro.html#installation). 
 
 Demo
 ----
-The library contains a demo application with multiple screens ([`rich`](https://pypi.org/project/rich)
-needs to be installed):
+The library contains a demo application with multiple screens:
 
     pip install rich
     python -m diskinfo.demo
 
 ![Demo screen](https://github.com/petersulyok/diskinfo/raw/main/docs/diskinfo_rich_demo.png)
 
 See more demo screens in the [documentation](https://diskinfo.readthedocs.io/en/latest/intro.html#demo).
```

### Comparing `diskinfo-3.1.0/src/diskinfo.egg-info/SOURCES.txt` & `diskinfo-3.1.1/src/diskinfo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `diskinfo-3.1.0/test/test_data.py` & `diskinfo-3.1.1/test/test_data.py`

 * *Files identical despite different names*

### Comparing `diskinfo-3.1.0/test/test_data_smart.py` & `diskinfo-3.1.1/test/test_data_smart.py`

 * *Files identical despite different names*

### Comparing `diskinfo-3.1.0/test/test_disk.py` & `diskinfo-3.1.1/test/test_disk.py`

 * *Files identical despite different names*

### Comparing `diskinfo-3.1.0/test/test_diskinfo.py` & `diskinfo-3.1.1/test/test_diskinfo.py`

 * *Files identical despite different names*

### Comparing `diskinfo-3.1.0/test/test_disksmart.py` & `diskinfo-3.1.1/test/test_disksmart.py`

 * *Files identical despite different names*

### Comparing `diskinfo-3.1.0/test/test_partition.py` & `diskinfo-3.1.1/test/test_partition.py`

 * *Files identical despite different names*

### Comparing `diskinfo-3.1.0/test/test_utils.py` & `diskinfo-3.1.1/test/test_utils.py`

 * *Files identical despite different names*

