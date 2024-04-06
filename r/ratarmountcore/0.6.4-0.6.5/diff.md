# Comparing `tmp/ratarmountcore-0.6.4.tar.gz` & `tmp/ratarmountcore-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ratarmountcore-0.6.4.tar", last modified: Sat Mar 23 20:35:19 2024, max compression
+gzip compressed data, was "ratarmountcore-0.6.5.tar", last modified: Sat Apr  6 16:58:02 2024, max compression
```

## Comparing `ratarmountcore-0.6.4.tar` & `ratarmountcore-0.6.5.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 20:35:19.544695 ratarmountcore-0.6.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-03-23 20:35:09.000000 ratarmountcore-0.6.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6344 2024-03-23 20:35:19.544695 ratarmountcore-0.6.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4180 2024-03-23 20:35:09.000000 ratarmountcore-0.6.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-03-23 20:35:09.000000 ratarmountcore-0.6.4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 20:35:19.540696 ratarmountcore-0.6.4/ratarmountcore/
--rw-r--r--   0 runner    (1001) docker     (127)    14697 2024-03-23 20:35:09.000000 ratarmountcore-0.6.4/ratarmountcore/AutoMountLayer.py
--rw-r--r--   0 runner    (1001) docker     (127)    12753 2024-03-23 20:35:09.000000 ratarmountcore-0.6.4/ratarmountcore/BlockParallelReaders.py
--rw-r--r--   0 runner    (1001) docker     (127)    10917 2024-03-23 20:35:09.000000 ratarmountcore-0.6.4/ratarmountcore/FileVersionLayer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5508 2024-03-23 20:35:09.000000 ratarmountcore-0.6.4/ratarmountcore/FolderMountSource.py
--rw-r--r--   0 runner    (1001) docker     (127)     3574 2024-03-23 20:35:09.000000 ratarmountcore-0.6.4/ratarmountcore/MountSource.py
--rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-03-23 20:35:09.000000 ratarmountcore-0.6.4/ratarmountcore/ProgressBar.py
--rw-r--r--   0 runner    (1001) docker     (127)     9305 2024-03-23 20:35:09.000000 ratarmountcore-0.6.4/ratarmountcore/RarMountSource.py
--rw-r--r--   0 runner    (1001) docker     (127)     4344 2024-03-23 20:35:09.000000 ratarmountcore-0.6.4/ratarmountcore/SQLiteBlobFile.py
--rw-r--r--   0 runner    (1001) docker     (127)    51293 2024-03-23 20:35:09.000000 ratarmountcore-0.6.4/ratarmountcore/SQLiteIndex.py
--rw-r--r--   0 runner    (1001) docker     (127)    77761 2024-03-23 20:35:09.000000 ratarmountcore-0.6.4/ratarmountcore/SQLiteIndexedTar.py
--rw-r--r--   0 runner    (1001) docker     (127)     2777 2024-03-23 20:35:09.000000 ratarmountcore-0.6.4/ratarmountcore/SingleFileMountSource.py
--rw-r--r--   0 runner    (1001) docker     (127)    16835 2024-03-23 20:35:09.000000 ratarmountcore-0.6.4/ratarmountcore/StenciledFile.py
--rw-r--r--   0 runner    (1001) docker     (127)     4308 2024-03-23 20:35:09.000000 ratarmountcore-0.6.4/ratarmountcore/SubvolumesMountSource.py
--rw-r--r--   0 runner    (1001) docker     (127)     9376 2024-03-23 20:35:09.000000 ratarmountcore-0.6.4/ratarmountcore/UnionMountSource.py
--rw-r--r--   0 runner    (1001) docker     (127)    12261 2024-03-23 20:35:09.000000 ratarmountcore-0.6.4/ratarmountcore/ZipMountSource.py
--rw-r--r--   0 runner    (1001) docker     (127)     3045 2024-03-23 20:35:09.000000 ratarmountcore-0.6.4/ratarmountcore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11682 2024-03-23 20:35:09.000000 ratarmountcore-0.6.4/ratarmountcore/compressions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4859 2024-03-23 20:35:09.000000 ratarmountcore-0.6.4/ratarmountcore/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     9381 2024-03-23 20:35:09.000000 ratarmountcore-0.6.4/ratarmountcore/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-03-23 20:35:09.000000 ratarmountcore-0.6.4/ratarmountcore/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 20:35:19.544695 ratarmountcore-0.6.4/ratarmountcore.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6344 2024-03-23 20:35:19.000000 ratarmountcore-0.6.4/ratarmountcore.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-03-23 20:35:19.000000 ratarmountcore-0.6.4/ratarmountcore.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-23 20:35:19.000000 ratarmountcore-0.6.4/ratarmountcore.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      562 2024-03-23 20:35:19.000000 ratarmountcore-0.6.4/ratarmountcore.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-03-23 20:35:19.000000 ratarmountcore-0.6.4/ratarmountcore.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-03-23 20:35:19.544695 ratarmountcore-0.6.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-03-23 20:35:09.000000 ratarmountcore-0.6.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 20:35:19.544695 ratarmountcore-0.6.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4796 2024-03-23 20:35:09.000000 ratarmountcore-0.6.4/tests/test_AutoMountLayer.py
--rw-r--r--   0 runner    (1001) docker     (127)    11698 2024-03-23 20:35:09.000000 ratarmountcore-0.6.4/tests/test_BlockParallelReaders.py
--rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-03-23 20:35:09.000000 ratarmountcore-0.6.4/tests/test_RarMountSource.py
--rw-r--r--   0 runner    (1001) docker     (127)     2613 2024-03-23 20:35:09.000000 ratarmountcore-0.6.4/tests/test_SQLiteBlobFile.py
--rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-03-23 20:35:09.000000 ratarmountcore-0.6.4/tests/test_SQLiteIndex.py
--rw-r--r--   0 runner    (1001) docker     (127)    23056 2024-03-23 20:35:09.000000 ratarmountcore-0.6.4/tests/test_SQLiteIndexedTar.py
--rw-r--r--   0 runner    (1001) docker     (127)    10296 2024-03-23 20:35:09.000000 ratarmountcore-0.6.4/tests/test_StenciledFile.py
--rw-r--r--   0 runner    (1001) docker     (127)     8765 2024-03-23 20:35:09.000000 ratarmountcore-0.6.4/tests/test_SubvolumesMountSource.py
--rw-r--r--   0 runner    (1001) docker     (127)     7709 2024-03-23 20:35:09.000000 ratarmountcore-0.6.4/tests/test_UnionMountSource.py
--rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-03-23 20:35:09.000000 ratarmountcore-0.6.4/tests/test_ZipMountSource.py
--rw-r--r--   0 runner    (1001) docker     (127)     3625 2024-03-23 20:35:09.000000 ratarmountcore-0.6.4/tests/test_compressions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-03-23 20:35:09.000000 ratarmountcore-0.6.4/tests/test_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     6834 2024-03-23 20:35:09.000000 ratarmountcore-0.6.4/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:58:01.998101 ratarmountcore-0.6.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-06 16:57:51.000000 ratarmountcore-0.6.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6344 2024-04-06 16:58:01.998101 ratarmountcore-0.6.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4180 2024-04-06 16:57:51.000000 ratarmountcore-0.6.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-06 16:57:51.000000 ratarmountcore-0.6.5/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:58:01.990101 ratarmountcore-0.6.5/ratarmountcore/
+-rw-r--r--   0 runner    (1001) docker     (127)    14704 2024-04-06 16:57:51.000000 ratarmountcore-0.6.5/ratarmountcore/AutoMountLayer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12753 2024-04-06 16:57:51.000000 ratarmountcore-0.6.5/ratarmountcore/BlockParallelReaders.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10917 2024-04-06 16:57:51.000000 ratarmountcore-0.6.5/ratarmountcore/FileVersionLayer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5508 2024-04-06 16:57:51.000000 ratarmountcore-0.6.5/ratarmountcore/FolderMountSource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3510 2024-04-06 16:57:51.000000 ratarmountcore-0.6.5/ratarmountcore/MountSource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-04-06 16:57:51.000000 ratarmountcore-0.6.5/ratarmountcore/ProgressBar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9312 2024-04-06 16:57:51.000000 ratarmountcore-0.6.5/ratarmountcore/RarMountSource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4344 2024-04-06 16:57:51.000000 ratarmountcore-0.6.5/ratarmountcore/SQLiteBlobFile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51490 2024-04-06 16:57:51.000000 ratarmountcore-0.6.5/ratarmountcore/SQLiteIndex.py
+-rw-r--r--   0 runner    (1001) docker     (127)    78477 2024-04-06 16:57:51.000000 ratarmountcore-0.6.5/ratarmountcore/SQLiteIndexedTar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2934 2024-04-06 16:57:51.000000 ratarmountcore-0.6.5/ratarmountcore/SingleFileMountSource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16835 2024-04-06 16:57:51.000000 ratarmountcore-0.6.5/ratarmountcore/StenciledFile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4315 2024-04-06 16:57:51.000000 ratarmountcore-0.6.5/ratarmountcore/SubvolumesMountSource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9425 2024-04-06 16:57:51.000000 ratarmountcore-0.6.5/ratarmountcore/UnionMountSource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12292 2024-04-06 16:57:51.000000 ratarmountcore-0.6.5/ratarmountcore/ZipMountSource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3045 2024-04-06 16:57:51.000000 ratarmountcore-0.6.5/ratarmountcore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11682 2024-04-06 16:57:51.000000 ratarmountcore-0.6.5/ratarmountcore/compressions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4003 2024-04-06 16:57:51.000000 ratarmountcore-0.6.5/ratarmountcore/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9381 2024-04-06 16:57:51.000000 ratarmountcore-0.6.5/ratarmountcore/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-06 16:57:51.000000 ratarmountcore-0.6.5/ratarmountcore/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:58:01.994101 ratarmountcore-0.6.5/ratarmountcore.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6344 2024-04-06 16:58:01.000000 ratarmountcore-0.6.5/ratarmountcore.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-04-06 16:58:01.000000 ratarmountcore-0.6.5/ratarmountcore.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 16:58:01.000000 ratarmountcore-0.6.5/ratarmountcore.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-04-06 16:58:01.000000 ratarmountcore-0.6.5/ratarmountcore.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-06 16:58:01.000000 ratarmountcore-0.6.5/ratarmountcore.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-04-06 16:58:01.998101 ratarmountcore-0.6.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-04-06 16:57:51.000000 ratarmountcore-0.6.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:58:01.994101 ratarmountcore-0.6.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4796 2024-04-06 16:57:51.000000 ratarmountcore-0.6.5/tests/test_AutoMountLayer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11698 2024-04-06 16:57:51.000000 ratarmountcore-0.6.5/tests/test_BlockParallelReaders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-04-06 16:57:51.000000 ratarmountcore-0.6.5/tests/test_RarMountSource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2613 2024-04-06 16:57:51.000000 ratarmountcore-0.6.5/tests/test_SQLiteBlobFile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-04-06 16:57:51.000000 ratarmountcore-0.6.5/tests/test_SQLiteIndex.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23056 2024-04-06 16:57:51.000000 ratarmountcore-0.6.5/tests/test_SQLiteIndexedTar.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10296 2024-04-06 16:57:51.000000 ratarmountcore-0.6.5/tests/test_StenciledFile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8765 2024-04-06 16:57:51.000000 ratarmountcore-0.6.5/tests/test_SubvolumesMountSource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7709 2024-04-06 16:57:51.000000 ratarmountcore-0.6.5/tests/test_UnionMountSource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-04-06 16:57:51.000000 ratarmountcore-0.6.5/tests/test_ZipMountSource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3625 2024-04-06 16:57:51.000000 ratarmountcore-0.6.5/tests/test_compressions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-04-06 16:57:51.000000 ratarmountcore-0.6.5/tests/test_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6834 2024-04-06 16:57:51.000000 ratarmountcore-0.6.5/tests/test_utils.py
```

### Comparing `ratarmountcore-0.6.4/LICENSE` & `ratarmountcore-0.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ratarmountcore-0.6.4/PKG-INFO` & `ratarmountcore-0.6.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ratarmountcore
-Version: 0.6.4
+Version: 0.6.5
 Summary: Random Access Read-Only Tar Mount Library
 Home-page: https://github.com/mxmlnkn/ratarmount/ratarmountcore
 Author: Maximilian Knespel
 Author-email: mxmlnkn@github.de
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ratarmountcore-0.6.4/README.md` & `ratarmountcore-0.6.5/README.md`

 * *Files identical despite different names*

### Comparing `ratarmountcore-0.6.4/ratarmountcore/AutoMountLayer.py` & `ratarmountcore-0.6.5/ratarmountcore/AutoMountLayer.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 from dataclasses import dataclass
 from typing import Dict, IO, Iterable, List, Optional, Tuple, Union
 
 from .compressions import stripSuffixFromTarFile
 from .factory import openMountSource
 from .FolderMountSource import FolderMountSource
-from .MountSource import FileInfo, MountSource
+from .MountSource import FileInfo, MountSource, createRootFileInfo
 from .SQLiteIndexedTar import SQLiteIndexedTar, SQLiteIndexedTarUserData
 from .utils import overrides
 
 
 class AutoMountLayer(MountSource):
     """
     This mount source takes another mount source and automatically shows the contents of files which are archives.
@@ -34,15 +34,15 @@
         self.options = options
         self.recursionDepth: int = -1 if self.options.get('recursive', False) else 0
         if 'recursionDepth' in self.options:
             self.recursionDepth = int(self.options['recursionDepth'])
         self.lazyMounting: bool = self.options.get('lazyMounting', False)
         self.printDebug = int(options.get("printDebug", 0)) if isinstance(options.get("printDebug", 0), int) else 0
 
-        rootFileInfo = MountSource._createRootFileInfo(userdata=['/'])
+        rootFileInfo = createRootFileInfo(userdata=['/'])
 
         # Mount points are specified without trailing slash and with leading slash
         # representing root of this mount source.
         # Disable false positive introduced when updating pylint from 2.6 to 2.12.
         # It now thinks that the assignment is to AutoMountLayer instead of self.mounted.
         # pylint: disable=used-before-assignment
         self.mounted: Dict[str, AutoMountLayer.MountInfo] = {'/': AutoMountLayer.MountInfo(mountSource, rootFileInfo)}
```

### Comparing `ratarmountcore-0.6.4/ratarmountcore/BlockParallelReaders.py` & `ratarmountcore-0.6.5/ratarmountcore/BlockParallelReaders.py`

 * *Files identical despite different names*

### Comparing `ratarmountcore-0.6.4/ratarmountcore/FileVersionLayer.py` & `ratarmountcore-0.6.5/ratarmountcore/FileVersionLayer.py`

 * *Files identical despite different names*

### Comparing `ratarmountcore-0.6.4/ratarmountcore/FolderMountSource.py` & `ratarmountcore-0.6.5/ratarmountcore/FolderMountSource.py`

 * *Files identical despite different names*

### Comparing `ratarmountcore-0.6.4/ratarmountcore/MountSource.py` & `ratarmountcore-0.6.5/ratarmountcore/MountSource.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,20 +89,20 @@
 
     # If the derived MountSource opens some file object or similar in its constructor
     # then it should override this and close the file object.
     @abstractmethod
     def __exit__(self, exception_type, exception_value, exception_traceback):
         pass
 
-    @staticmethod
-    def _createRootFileInfo(userdata: List[Any]):
-        return FileInfo(
-            # fmt: off
-            size     = 0,
-            mtime    = int(time.time()),
-            mode     = 0o777 | stat.S_IFDIR,
-            linkname = "",
-            uid      = os.getuid(),
-            gid      = os.getgid(),
-            userdata = [None],
-            # fmt: on
-        )
+
+def createRootFileInfo(userdata: List[Any]):
+    return FileInfo(
+        # fmt: off
+        size     = 0,
+        mtime    = int(time.time()),
+        mode     = 0o777 | stat.S_IFDIR,
+        linkname = "",
+        uid      = os.getuid(),
+        gid      = os.getgid(),
+        userdata = userdata,
+        # fmt: on
+    )
```

### Comparing `ratarmountcore-0.6.4/ratarmountcore/ProgressBar.py` & `ratarmountcore-0.6.5/ratarmountcore/ProgressBar.py`

 * *Files identical despite different names*

### Comparing `ratarmountcore-0.6.4/ratarmountcore/RarMountSource.py` & `ratarmountcore-0.6.5/ratarmountcore/RarMountSource.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import datetime
 import io
 import os
 import stat
 import time
 from typing import cast, Dict, IO, Iterable, List, Optional, Union
 
-from .MountSource import FileInfo, MountSource
+from .MountSource import FileInfo, MountSource, createRootFileInfo
 from .utils import overrides
 
 try:
     import rarfile
 except ImportError:
     pass
 
@@ -204,15 +204,15 @@
             if getName(normalizedPath)
         }
 
     def _getFileInfos(self, path: str) -> List[FileInfo]:
         # If we have a fileInfo for the given directory path, then everything is fine.
         pathAsDir = path.strip('/') + '/'
         if pathAsDir == '/':
-            return [MountSource._createRootFileInfo(userdata=[None])]
+            return [createRootFileInfo(userdata=[None])]
 
         infoList = [
             RarMountSource._convertToFileInfo(normalizedPath, info)
             for normalizedPath, info in self.files.items()
             if normalizedPath.rstrip('/') == path.lstrip('/')
         ]
```

### Comparing `ratarmountcore-0.6.4/ratarmountcore/SQLiteBlobFile.py` & `ratarmountcore-0.6.5/ratarmountcore/SQLiteBlobFile.py`

 * *Files identical despite different names*

### Comparing `ratarmountcore-0.6.4/ratarmountcore/SQLiteIndex.py` & `ratarmountcore-0.6.5/ratarmountcore/SQLiteIndex.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 try:
     import rapidgzip
 except ImportError:
     pass
 
 from .version import __version__
-from .MountSource import FileInfo, MountSource
+from .MountSource import FileInfo, createRootFileInfo
 from .compressions import TAR_COMPRESSION_FORMATS
 from .SQLiteBlobFile import SQLiteBlobsFile, WriteSQLiteBlobs
 from .utils import RatarmountError, IndexNotOpenError, InvalidIndexError, findModuleVersion
 
 
 def getSqliteTables(connection: sqlite3.Connection):
     return [x[0] for x in connection.execute('SELECT name FROM sqlite_master WHERE type="table"')]
@@ -138,14 +138,18 @@
              *   PATCH version when you make backwards compatible bug fixes. */
             "major"    INTEGER,
             "minor"    INTEGER,
             "patch"    INTEGER
         );
     """
 
+    # Check some of the first and last files in the archive and some random selection in between.
+    # Do not verify folders because parent folders and root get automatically added!
+    FROM_REGULAR_FILES = f"""FROM "files" WHERE (mode & {stat.S_IFREG}) != 0"""
+
     def __init__(
         self,
         indexFilePath: Optional[str],
         indexFolders: Optional[List[str]] = None,
         archiveFilePath: Optional[str] = None,
         encoding: str = tarfile.ENCODING,
         checkMetadata: Optional[Callable[[Dict[str, Any]], None]] = None,
@@ -194,15 +198,15 @@
         # For latter, ignore the special empty folder [''], which means that the indexes are stored
         # besides the archives.
         # Why all this exceptions? Because the index-minimum-file-count, which is set by default,
         # is only intended to avoid littering folders with index files in the common use case of mounting
         # a folder of archives or single small archives recursively. If the user goes through the trouble
         # of specifying an index file or folder, then littering should not be a problem as index creations
         # are expected by the user.
-        if self.indexMinimumFileCount > 0 and not indexFilePath and (not indexFolders or not any(indexFolders)):
+        if self.indexMinimumFileCount > 0 and not indexFilePath:
             if self.printDebug >= 3:
                 print(
                     f"[Info] Because of the given positive index minimum file count ({self.indexMinimumFileCount}) "
                     "and because no explicit index file path is given, try to open an SQLite database in memory first."
                 )
             self.preferMemory = True
 
@@ -624,15 +628,15 @@
         Return metadata for all versions of a file possibly appearing more than once
         in the index as a directory dictionary or an empty dictionary if the path does not exist.
 
         path : full path to file where '/' denotes TAR's root, e.g., '/', or '/foo'
         """
 
         if path == '/':
-            return {'/': MountSource._createRootFileInfo(userdata=[SQLiteIndexedTarUserData(0, 0, False, False)])}
+            return {'/': createRootFileInfo(userdata=[SQLiteIndexedTarUserData(0, 0, False, False)])}
 
         path, name = self._queryNormpath(path).rsplit('/', 1)
         rows = self.getConnection().execute(
             'SELECT * FROM "files" WHERE "path" == (?) AND "name" == (?) ORDER BY "offsetheader" ASC', (path, name)
         )
         result = {str(version + 1): self._rowToFileInfo(row) for version, row in enumerate(rows)}
         return result
@@ -653,15 +657,15 @@
                       FUSE already does this by calling getattr for all parent folders in the specified path first.
         """
 
         if not isinstance(fileVersion, int):
             raise RatarmountError("The specified file version must be an integer!")
 
         if path == '/':
-            return MountSource._createRootFileInfo(userdata=[SQLiteIndexedTarUserData(0, 0, False, False)])
+            return createRootFileInfo(userdata=[SQLiteIndexedTarUserData(0, 0, False, False)])
 
         path, name = self._queryNormpath(path).rsplit('/', 1)
         row = (
             self.getConnection()
             .execute(
                 f"""
             SELECT * FROM "files"
```

### Comparing `ratarmountcore-0.6.4/ratarmountcore/SQLiteIndexedTar.py` & `ratarmountcore-0.6.5/ratarmountcore/SQLiteIndexedTar.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 import io
 import json
+import math
 import multiprocessing.pool
 import os
 import platform
 import re
 import sqlite3
 import stat
 import sys
@@ -41,15 +42,14 @@
 from .MountSource import FileInfo, MountSource
 from .ProgressBar import ProgressBar
 from .SQLiteIndex import SQLiteIndex, SQLiteIndexedTarUserData
 from .StenciledFile import StenciledFile
 from .compressions import findAvailableOpen, getGzipInfo, TAR_COMPRESSION_FORMATS
 from .utils import (
     RatarmountError,
-    IndexNotOpenError,
     InvalidIndexError,
     CompressionError,
     ceilDiv,
     isOnSlowDrive,
     overrides,
 )
 from .BlockParallelReaders import ParallelXZReader
@@ -1165,17 +1165,20 @@
         # reading because it is not specified how many zero-byte blocks there may be at the end:
         # > At the end of the archive file there shall be two 512-byte blocks filled with binary zeros,
         # > interpreted as an end-of-archive indicator.
         # For example, GNU tar rounds up to 10 KiB for very small archives but will (have to) append further
         # files right after the the last non-zero block, which might be at offset 512 for empty files.
         # > The user can specify a blocking factor, which is the number of blocks per record.
         # > The default is 20, producing 10 KiB records.
-        pastEndOffset, isSparse = sqlConnection.execute(
+        result = sqlConnection.execute(
             "SELECT offset + size, issparse FROM files ORDER BY offset DESC LIMIT 1"
         ).fetchone()
+        if not result:
+            raise InvalidIndexError("The index contains no files!")
+        pastEndOffset, isSparse = result
 
         if isSparse:
             return None
 
         # Round up to next TAR block
         if pastEndOffset % 512 != 0:
             pastEndOffset += 512 - (pastEndOffset % 512)
@@ -1341,59 +1344,64 @@
                 print("[Warning] The arguments used for creating the found index differ from the arguments ")
                 print("[Warning] given for mounting the archive now. In order to apply these changes, ")
                 print("[Warning] recreate the index using the --recreate-index option!")
                 for arg, oldState, newState in differingArgs:
                     print(f"[Warning] {arg}: index: {oldState}, current: {newState}")
 
     def _checkIndexValidity(self) -> bool:
-        if not self.index.sqlConnection:
-            raise IndexNotOpenError("This method can not be called without an opened index database!")
-
         # Check some of the first and last files in the archive and some random selection in between.
-        result = self.index.sqlConnection.execute(
+        selectFiles = "SELECT * " + SQLiteIndex.FROM_REGULAR_FILES
+        result = self.index.getConnection().execute(
             f"""
-            SELECT * FROM ( SELECT * FROM files ORDER BY offset ASC LIMIT 100 )
+            SELECT * FROM ( {selectFiles} ORDER BY offset ASC LIMIT 100 )
             UNION
-            SELECT * FROM ( SELECT * FROM files ORDER BY RANDOM() LIMIT {SQLiteIndex.NUMBER_OF_METADATA_TO_VERIFY} )
+            SELECT * FROM ( {selectFiles} ORDER BY RANDOM() LIMIT {SQLiteIndex.NUMBER_OF_METADATA_TO_VERIFY} )
             UNION
-            SELECT * FROM ( SELECT * FROM files ORDER BY offset DESC LIMIT 100 )
+            SELECT * FROM ( {selectFiles} ORDER BY offset DESC LIMIT 100 )
             ORDER BY offset
         """
         )
 
         t0 = time.time()
 
         oldOffset = self.tarFileObject.tell()
         try:
             for row in result:
                 # As for the stencil size, 512 B (one TAR block) would be enough for most cases except for
                 # features like GNU LongLink which store additional metadata in further TAR blocks.
-                offset_header = int(row[2])
-                with StenciledFile(fileStencils=[(self.tarFileObject, offset_header, 2 * 512)]) as file:
+                offsetHeader = int(row[2])
+                offsetData = int(row[3])
+                headerBlockCount = max(1, int(math.ceil((offsetData - offsetHeader) / 512))) * 512
+                with StenciledFile(fileStencils=[(self.tarFileObject, offsetHeader, headerBlockCount)]) as file:
                     with tarfile.open(fileobj=file, mode='r|', ignore_zeros=True, encoding=self.encoding) as archive:
                         tarInfo = next(iter(archive))
                         realFileInfos, _, _ = _TarFileMetadataReader._processTarInfo(
                             tarInfo,
                             file,  # only used for isGnuIncremental == True
                             "",  # pathPrefix
-                            offset_header,  # will be added to all offsets to get the real offset
+                            offsetHeader,  # will be added to all offsets to get the real offset
                             self._isGnuIncremental,
                             False,  # mountRecursively
                             self.printDebug,
                         )
 
                         # Bool columns will have been converted to int 0 or 1 when reading from SQLite.
                         # In order to compare with the read result correctly, we need to convert them to bool, too.
                         storedFileInfo = list(row)
                         for index in [-1, -2]:
                             if storedFileInfo[index] not in [0, 1]:
                                 return False
                             storedFileInfo[index] = bool(storedFileInfo[index])
 
                         if tuple(storedFileInfo) != realFileInfos[0]:
+                            if self.printDebug >= 3:
+                                print("[Info] Stored file info:")
+                                print("[Info]", storedFileInfo)
+                                print("[Info] differs from recomputed one:")
+                                print("[Info]", realFileInfos[0])
                             return False
 
             return True
         except tarfile.TarError:
             # Not even worth warning because this simply might happen if the index is not valid anymore.
             return False
         finally:
@@ -1508,19 +1516,21 @@
                 fileobj,
                 compression=compression,
                 gzipSeekPointSpacing=gzipSeekPointSpacing,
                 prioritizedBackends=prioritizedBackends,
                 printDebug=printDebug,
             ):
                 isRealFile = hasattr(fileobj, 'name') and fileobj.name and os.path.isfile(fileobj.name)
-                tar_file = rapidgzip.RapidgzipFile(
-                    fileobj,
-                    parallelization=1 if isRealFile and isOnSlowDrive(fileobj.name) else parallelization,
-                    verbose=printDebug >= 2,
-                )
+                parallelization = 1 if isRealFile and isOnSlowDrive(fileobj.name) else parallelization
+                if printDebug >= 3:
+                    print(
+                        f"[Info] Parallelization to use for rapidgzip backend: {parallelization}, "
+                        f"slow drive detected: {isOnSlowDrive(fileobj.name)}"
+                    )
+                tar_file = rapidgzip.RapidgzipFile(fileobj, parallelization=parallelization, verbose=printDebug >= 2)
             else:
                 # The buffer size must be much larger than the spacing or else there will be large performance penalties
                 # even for reading sequentially, see https://github.com/pauldmccarthy/indexed_gzip/issues/89
                 # Use 4x spacing because each raw read seeks from the last index point even if the position did not change
                 # since the last read call. On average, this incurs an overhead of spacing / 2. For 3x spacing, this
                 # overhead would be 1/6 = 17%, which should be negligible. The increased memory-usage is not an issue
                 # because internally many buffers are allocated with 4 * spacing size.
```

### Comparing `ratarmountcore-0.6.4/ratarmountcore/SingleFileMountSource.py` & `ratarmountcore-0.6.5/ratarmountcore/SingleFileMountSource.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,15 +21,17 @@
             raise ValueError("File object must belong to a non-folder path!")
 
         self.fileObjectLock = threading.Lock()
         self.fileobj = fileobj
         self.mtime = int(time.time())
         self.size: int = self.fileobj.seek(0, io.SEEK_END)
 
-        self.fileInfo = FileInfo(
+    def _createFileInfo(self):
+        # This must be a function and cannot be cached into a member in order to avoid userdata being a shared list!
+        return FileInfo(
             # fmt: off
             size     = self.size,
             mtime    = self.mtime,
             mode     = int(0o777 | stat.S_IFREG),
             linkname = '',
             uid      = 0,
             gid      = 0,
@@ -57,19 +59,19 @@
                 uid      = 0,
                 gid      = 0,
                 userdata = [],
                 # fmt: on
             )
             return fileInfo
 
-        return self.fileInfo if path == self.path else None
+        return self._createFileInfo() if path == self.path else None
 
     @overrides(MountSource)
     def open(self, fileInfo: FileInfo) -> IO[bytes]:
-        if fileInfo != self.fileInfo:
+        if fileInfo != self._createFileInfo():
             raise ValueError("Only files may be opened!")
         # Use StenciledFile so that the returned file objects can be idependently seeked!
         return StenciledFile(fileStencils=[(self.fileobj, 0, self.size)], fileObjectLock=self.fileObjectLock)
 
     @overrides(MountSource)
     def isImmutable(self) -> bool:
         return True
```

### Comparing `ratarmountcore-0.6.4/ratarmountcore/StenciledFile.py` & `ratarmountcore-0.6.5/ratarmountcore/StenciledFile.py`

 * *Files identical despite different names*

### Comparing `ratarmountcore-0.6.4/ratarmountcore/SubvolumesMountSource.py` & `ratarmountcore-0.6.5/ratarmountcore/SubvolumesMountSource.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 from typing import Dict, Iterable, IO, Optional, Tuple, Union
 
-from .MountSource import FileInfo, MountSource
+from .MountSource import FileInfo, MountSource, createRootFileInfo
 from .utils import overrides
 
 
 class SubvolumesMountSource(MountSource):
     def __init__(self, mountSources: Dict[str, MountSource], printDebug: int = 0) -> None:
         """
         mountSources : List of mount sources to mount as subfolders.
@@ -15,15 +15,15 @@
         self.mountSources: Dict[str, MountSource] = mountSources
         self.printDebug = printDebug
 
         for name in self.mountSources.keys():
             if '/' in name:
                 raise ValueError(f"Mount source names may not contain slashes! ({name})")
 
-        self.rootFileInfo = MountSource._createRootFileInfo(userdata=[None])
+        self.rootFileInfo = createRootFileInfo(userdata=[None])
 
     def _findMountSource(self, path: str) -> Optional[Tuple[str, str]]:
         path = path.lstrip('/')
         subvolume, subpath = path.split('/', maxsplit=1) if '/' in path else [path, ""]
         return (subvolume, '/' + subpath) if subvolume in self.mountSources else None
 
     @overrides(MountSource)
```

### Comparing `ratarmountcore-0.6.4/ratarmountcore/UnionMountSource.py` & `ratarmountcore-0.6.5/ratarmountcore/UnionMountSource.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,26 +3,27 @@
 
 import os
 import stat
 import time
 
 from typing import Dict, Iterable, IO, List, Optional, Set, Tuple, Union
 
-from .MountSource import FileInfo, MountSource
+from .MountSource import FileInfo, MountSource, createRootFileInfo
 from .utils import overrides
 
 
 class UnionMountSource(MountSource):
     def __init__(
         self,
         mountSources: List[MountSource],
         printDebug: int = 0,
         maxCacheDepth: int = 1024,
         maxCacheEntries: int = 100000,
         maxSecondsToCache: float = 60,
+        # pylint: disable=unused-argument
         **options,
     ) -> None:
         """
         mountSources:
             List of mount sources for which to show a union view. The rightmost mount sources have
             the highest precedence. Meaning, if a file with the same name exists in multiple mount
             sources, then by default the file of the rightmost mount source will be returned.
@@ -34,15 +35,15 @@
             and it shouldn't take minutes! Note that there always can be an edge case with hundred
             thousands of files in one folder, which can take an arbitrary amount of time to cache.
         """
         self.mountSources: List[MountSource] = mountSources
         self.printDebug = printDebug
         self.folderCache: Dict[str, List[MountSource]] = {"/": self.mountSources}
         self.folderCacheDepth = 0  # depth 1 means, we only cached top-level directories.
-        self.rootFileInfo = MountSource._createRootFileInfo(userdata=[None])
+        self.rootFileInfo = createRootFileInfo(userdata=[None])
 
         if len(self.mountSources) > 1:
             self._buildFolderCache(maxCacheDepth, maxCacheEntries, maxSecondsToCache)
 
     def _buildFolderCache(self, maxCacheDepth: int, maxCacheEntries: int, maxSecondsToCache: float) -> None:
         t0 = time.time()
```

### Comparing `ratarmountcore-0.6.4/ratarmountcore/ZipMountSource.py` & `ratarmountcore-0.6.5/ratarmountcore/ZipMountSource.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,15 @@
         writeIndex             : bool                = False,
         clearIndexCache        : bool                = False,
         indexFilePath          : Optional[str]       = None,
         indexFolders           : Optional[List[str]] = None,
         encoding               : str                 = tarfile.ENCODING,
         verifyModificationTime : bool                = False,
         printDebug             : int                 = 0,
+        indexMinimumFileCount  : int                 = 1000,
         **options
         # fmt: on
     ) -> None:
         self.fileObject = zipfile.ZipFile(fileOrPath, 'r')
         self.archiveFilePath = fileOrPath if isinstance(fileOrPath, str) else None
         self.encoding = encoding
         self.verifyModificationTime = verifyModificationTime
@@ -44,15 +45,15 @@
         self.index = SQLiteIndex(
             indexFilePath,
             indexFolders=indexFolders,
             archiveFilePath=self.archiveFilePath,
             encoding=self.encoding,
             checkMetadata=self._checkMetadata,
             printDebug=self.printDebug,
-            preferMemory=len(self.files) < options.get("indexMinimumFileCount", 1000),
+            indexMinimumFileCount=indexMinimumFileCount,
         )
 
         if clearIndexCache:
             self.index.clearIndexes()
 
         isFileObject = not isinstance(fileOrPath, str)
```

### Comparing `ratarmountcore-0.6.4/ratarmountcore/__init__.py` & `ratarmountcore-0.6.5/ratarmountcore/__init__.py`

 * *Files identical despite different names*

### Comparing `ratarmountcore-0.6.4/ratarmountcore/compressions.py` & `ratarmountcore-0.6.5/ratarmountcore/compressions.py`

 * *Files identical despite different names*

### Comparing `ratarmountcore-0.6.4/ratarmountcore/factory.py` & `ratarmountcore-0.6.5/ratarmountcore/factory.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import os
 import sys
 import traceback
 
 from typing import IO, Union
 
-from .compressions import supportedCompressions, checkForSplitFile, rarfile, zipfile
+from .compressions import checkForSplitFile, rarfile, zipfile
 from .utils import CompressionError, RatarmountError
 from .MountSource import MountSource
 from .FolderMountSource import FolderMountSource
 from .RarMountSource import RarMountSource
 from .SingleFileMountSource import SingleFileMountSource
 from .SQLiteIndexedTar import SQLiteIndexedTar
 from .StenciledFile import JoinedFileFromFactory
@@ -70,31 +70,21 @@
             traceback.print_exc()
     finally:
         if hasattr(fileOrPath, 'seek'):
             fileOrPath.seek(0)  # type: ignore
 
     if 'zipfile' in sys.modules and zipfile is not None:
         try:
-            # is_zipfile is much too lax when testing for ZIPs because it's only testing for the central directory
-            # at the end of the file not the magic bits at the beginning. Meaning, if another non-ZIP archive has
-            # zip contents at the end, then it might get misclassified! Thefore, manually check for PK at start.
-            # https://bugs.python.org/issue16735
-            # https://bugs.python.org/issue28494
-            # https://bugs.python.org/issue42096
-            # https://bugs.python.org/issue45287
-            # TODO This will not recognize self-extracting ZIP archives, so for now, those are simply not supported!
-            if isinstance(fileOrPath, str):
-                with open(fileOrPath, 'rb') as file:
-                    if supportedCompressions['zip'].checkHeader(file) and zipfile.is_zipfile(fileOrPath):
-                        return ZipMountSource(fileOrPath, **options)
-            else:
-                # TODO One problem here is when trying to read and then seek back but there also is no peek method.
-                #      https://github.com/markokr/rarfile/issues/73
-                if fileOrPath.read(2) == b'PK' and zipfile.is_zipfile(fileOrPath):
-                    return ZipMountSource(fileOrPath, **options)
+            # is_zipfile might yields some false positives, but those should then raise exceptions, which
+            # are caught, so it should be fine. See: https://bugs.python.org/issue42096
+            if zipfile.is_zipfile(fileOrPath):
+                mountSource = ZipMountSource(fileOrPath, **options)
+                if printDebug >= 2:
+                    print("[Info] Opened archive as ZIP file.")
+                return mountSource
         except Exception as exception:
             if printDebug >= 1:
                 print("[Info] Checking for ZIP file raised an exception:", exception)
             if printDebug >= 3:
                 traceback.print_exc()
         finally:
             if hasattr(fileOrPath, 'seek'):
```

### Comparing `ratarmountcore-0.6.4/ratarmountcore/utils.py` & `ratarmountcore-0.6.5/ratarmountcore/utils.py`

 * *Files identical despite different names*

### Comparing `ratarmountcore-0.6.4/ratarmountcore.egg-info/PKG-INFO` & `ratarmountcore-0.6.5/ratarmountcore.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ratarmountcore
-Version: 0.6.4
+Version: 0.6.5
 Summary: Random Access Read-Only Tar Mount Library
 Home-page: https://github.com/mxmlnkn/ratarmount/ratarmountcore
 Author: Maximilian Knespel
 Author-email: mxmlnkn@github.de
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ratarmountcore-0.6.4/ratarmountcore.egg-info/SOURCES.txt` & `ratarmountcore-0.6.5/ratarmountcore.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ratarmountcore-0.6.4/ratarmountcore.egg-info/requires.txt` & `ratarmountcore-0.6.5/ratarmountcore.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `ratarmountcore-0.6.4/setup.cfg` & `ratarmountcore-0.6.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `ratarmountcore-0.6.4/setup.py` & `ratarmountcore-0.6.5/setup.py`

 * *Files identical despite different names*

### Comparing `ratarmountcore-0.6.4/tests/test_AutoMountLayer.py` & `ratarmountcore-0.6.5/tests/test_AutoMountLayer.py`

 * *Files identical despite different names*

### Comparing `ratarmountcore-0.6.4/tests/test_BlockParallelReaders.py` & `ratarmountcore-0.6.5/tests/test_BlockParallelReaders.py`

 * *Files identical despite different names*

### Comparing `ratarmountcore-0.6.4/tests/test_RarMountSource.py` & `ratarmountcore-0.6.5/tests/test_RarMountSource.py`

 * *Files identical despite different names*

### Comparing `ratarmountcore-0.6.4/tests/test_SQLiteBlobFile.py` & `ratarmountcore-0.6.5/tests/test_SQLiteBlobFile.py`

 * *Files identical despite different names*

### Comparing `ratarmountcore-0.6.4/tests/test_SQLiteIndex.py` & `ratarmountcore-0.6.5/tests/test_SQLiteIndex.py`

 * *Files identical despite different names*

### Comparing `ratarmountcore-0.6.4/tests/test_SQLiteIndexedTar.py` & `ratarmountcore-0.6.5/tests/test_SQLiteIndexedTar.py`

 * *Files identical despite different names*

### Comparing `ratarmountcore-0.6.4/tests/test_StenciledFile.py` & `ratarmountcore-0.6.5/tests/test_StenciledFile.py`

 * *Files identical despite different names*

### Comparing `ratarmountcore-0.6.4/tests/test_SubvolumesMountSource.py` & `ratarmountcore-0.6.5/tests/test_SubvolumesMountSource.py`

 * *Files identical despite different names*

### Comparing `ratarmountcore-0.6.4/tests/test_UnionMountSource.py` & `ratarmountcore-0.6.5/tests/test_UnionMountSource.py`

 * *Files identical despite different names*

### Comparing `ratarmountcore-0.6.4/tests/test_ZipMountSource.py` & `ratarmountcore-0.6.5/tests/test_ZipMountSource.py`

 * *Files identical despite different names*

### Comparing `ratarmountcore-0.6.4/tests/test_compressions.py` & `ratarmountcore-0.6.5/tests/test_compressions.py`

 * *Files identical despite different names*

### Comparing `ratarmountcore-0.6.4/tests/test_factory.py` & `ratarmountcore-0.6.5/tests/test_factory.py`

 * *Files identical despite different names*

### Comparing `ratarmountcore-0.6.4/tests/test_utils.py` & `ratarmountcore-0.6.5/tests/test_utils.py`

 * *Files identical despite different names*

