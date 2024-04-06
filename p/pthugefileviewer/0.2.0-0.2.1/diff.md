# Comparing `tmp/pthugefileviewer-0.2.0.tar.gz` & `tmp/pthugefileviewer-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pthugefileviewer-0.2.0.tar", last modified: Mon Apr  1 21:02:17 2024, max compression
+gzip compressed data, was "pthugefileviewer-0.2.1.tar", last modified: Sat Apr  6 15:58:45 2024, max compression
```

## Comparing `pthugefileviewer-0.2.0.tar` & `pthugefileviewer-0.2.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:02:16.998155 pthugefileviewer-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 21:02:09.000000 pthugefileviewer-0.2.0/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-01 21:02:09.000000 pthugefileviewer-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2948 2024-04-01 21:02:16.998155 pthugefileviewer-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-04-01 21:02:09.000000 pthugefileviewer-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:02:16.998155 pthugefileviewer-0.2.0/pthugefileviewer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2948 2024-04-01 21:02:16.000000 pthugefileviewer-0.2.0/pthugefileviewer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-01 21:02:16.000000 pthugefileviewer-0.2.0/pthugefileviewer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 21:02:16.000000 pthugefileviewer-0.2.0/pthugefileviewer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-01 21:02:16.000000 pthugefileviewer-0.2.0/pthugefileviewer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-01 21:02:16.000000 pthugefileviewer-0.2.0/pthugefileviewer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-01 21:02:09.000000 pthugefileviewer-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-01 21:02:09.000000 pthugefileviewer-0.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-01 21:02:16.998155 pthugefileviewer-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-01 21:02:09.000000 pthugefileviewer-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:02:16.994155 pthugefileviewer-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:02:16.998155 pthugefileviewer-0.2.0/src/bin/
--rwxr-xr-x   0 runner    (1001) docker     (127)     6387 2024-04-01 21:02:09.000000 pthugefileviewer-0.2.0/src/bin/hfv-regexbuild
--rwxr-xr-x   0 runner    (1001) docker     (127)     1895 2024-04-01 21:02:09.000000 pthugefileviewer-0.2.0/src/bin/hfv-view
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:02:16.998155 pthugefileviewer-0.2.0/src/pthugefileviewer/
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-01 21:02:09.000000 pthugefileviewer-0.2.0/src/pthugefileviewer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6375 2024-04-01 21:02:09.000000 pthugefileviewer-0.2.0/src/pthugefileviewer/hugefilevieweruicontrol.py
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 21:02:09.000000 pthugefileviewer-0.2.0/src/pthugefileviewer/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:02:16.998155 pthugefileviewer-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     6942 2024-04-01 21:02:09.000000 pthugefileviewer-0.2.0/tests/test_hfv.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:58:45.853359 pthugefileviewer-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 15:58:37.000000 pthugefileviewer-0.2.1/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-06 15:58:37.000000 pthugefileviewer-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2948 2024-04-06 15:58:45.853359 pthugefileviewer-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-04-06 15:58:37.000000 pthugefileviewer-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:58:45.853359 pthugefileviewer-0.2.1/pthugefileviewer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2948 2024-04-06 15:58:45.000000 pthugefileviewer-0.2.1/pthugefileviewer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-06 15:58:45.000000 pthugefileviewer-0.2.1/pthugefileviewer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 15:58:45.000000 pthugefileviewer-0.2.1/pthugefileviewer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-06 15:58:45.000000 pthugefileviewer-0.2.1/pthugefileviewer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-06 15:58:45.000000 pthugefileviewer-0.2.1/pthugefileviewer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-06 15:58:37.000000 pthugefileviewer-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-06 15:58:37.000000 pthugefileviewer-0.2.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-06 15:58:45.853359 pthugefileviewer-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-06 15:58:37.000000 pthugefileviewer-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:58:45.849359 pthugefileviewer-0.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:58:45.853359 pthugefileviewer-0.2.1/src/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6387 2024-04-06 15:58:37.000000 pthugefileviewer-0.2.1/src/bin/hfv-regexbuild
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1895 2024-04-06 15:58:37.000000 pthugefileviewer-0.2.1/src/bin/hfv-view
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:58:45.853359 pthugefileviewer-0.2.1/src/pthugefileviewer/
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-06 15:58:37.000000 pthugefileviewer-0.2.1/src/pthugefileviewer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6411 2024-04-06 15:58:37.000000 pthugefileviewer-0.2.1/src/pthugefileviewer/hugefilevieweruicontrol.py
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 15:58:37.000000 pthugefileviewer-0.2.1/src/pthugefileviewer/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:58:45.853359 pthugefileviewer-0.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     7341 2024-04-06 15:58:37.000000 pthugefileviewer-0.2.1/tests/test_hfv.py
```

### Comparing `pthugefileviewer-0.2.0/LICENSE` & `pthugefileviewer-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pthugefileviewer-0.2.0/PKG-INFO` & `pthugefileviewer-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pthugefileviewer
-Version: 0.2.0
+Version: 0.2.1
 Summary: Huge file viewer control for prompt-toolkit
 Home-page: http://github.com/lpenz/pthugefileviewer
 Author: "Leandro Lisboa Penz"
 Author-email: "lpenz@lpenz.org"
 License: MIT
 Classifier: Development Status :: 1 - Planning
 Classifier: Environment :: Console
```

### Comparing `pthugefileviewer-0.2.0/README.md` & `pthugefileviewer-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `pthugefileviewer-0.2.0/pthugefileviewer.egg-info/PKG-INFO` & `pthugefileviewer-0.2.1/pthugefileviewer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pthugefileviewer
-Version: 0.2.0
+Version: 0.2.1
 Summary: Huge file viewer control for prompt-toolkit
 Home-page: http://github.com/lpenz/pthugefileviewer
 Author: "Leandro Lisboa Penz"
 Author-email: "lpenz@lpenz.org"
 License: MIT
 Classifier: Development Status :: 1 - Planning
 Classifier: Environment :: Console
```

### Comparing `pthugefileviewer-0.2.0/setup.cfg` & `pthugefileviewer-0.2.1/setup.cfg`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pthugefileviewer
-version = 0.2.0
+version = 0.2.1
 description = Huge file viewer control for prompt-toolkit
 license = MIT
 license_files = LICENSE
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = "Leandro Lisboa Penz"
 author_email = "lpenz@lpenz.org"
```

### Comparing `pthugefileviewer-0.2.0/src/bin/hfv-regexbuild` & `pthugefileviewer-0.2.1/src/bin/hfv-regexbuild`

 * *Files identical despite different names*

### Comparing `pthugefileviewer-0.2.0/src/bin/hfv-view` & `pthugefileviewer-0.2.1/src/bin/hfv-view`

 * *Files identical despite different names*

### Comparing `pthugefileviewer-0.2.0/src/pthugefileviewer/hugefilevieweruicontrol.py` & `pthugefileviewer-0.2.1/src/pthugefileviewer/hugefilevieweruicontrol.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,23 +85,23 @@
     def get_lines(self) -> List[bytes]:
         with self.tmp_offset():
             lines = []
             for _ in range(self._height):
                 line = self._mm.readline()
                 if not line:
                     break
-                line = line.strip()
+                line = line.rstrip()
                 lines.append(line)
             return lines
 
     def update_lines(self) -> None:
         self._lines = [
             [("", line.decode("utf-8", errors="replace"))] for line in self.get_lines()
         ]
-        if self.height > len(self._lines):
+        if self.height > len(self._lines) and self.offset < self._offset_max:
             self.go_up(self._height - len(self._lines))
 
     def get_char(self, offset: Optional[int] = None) -> bytes:
         with self.tmp_offset():
             if offset is not None:
                 self.offset = offset
             return self._mm.read(1)
```

### Comparing `pthugefileviewer-0.2.0/tests/test_hfv.py` & `pthugefileviewer-0.2.1/tests/test_hfv.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,40 +3,51 @@
 import tempfile
 import unittest
 from typing import List
 
 from pthugefileviewer.hugefilevieweruicontrol import HugeFileViewerUIControl
 
 
+def tobytes(lines: List[str]) -> List[bytes]:
+    return [bytes(line, "ascii") for line in lines]
+
+
 class Base:
     def controlFor(self, height: int, contents: bytes) -> HugeFileViewerUIControl:
         with tempfile.TemporaryFile() as fd:
             fd.write(contents)
             fd.flush()
             control = HugeFileViewerUIControl(fd)
             control.height = height
             return control
 
     def controlLines(
         self, height: int, lines: List[str], newlines: int = 0
     ) -> HugeFileViewerUIControl:
         suffix = b"\n" * newlines
-        return self.controlFor(
-            height, b"\n".join([bytes(line, "ascii") for line in lines]) + suffix
-        )
+        return self.controlFor(height, b"\n".join(tobytes(lines)) + suffix)
 
     def controlNums(
         self, height: int, limit: int, newlines: int = 0
     ) -> HugeFileViewerUIControl:
         return self.controlLines(height, [f"{i}" for i in range(limit)], newlines)
 
 
 class TestBasic(unittest.TestCase, Base):
     newlines = 0
 
+    def test_no_lstrip(self) -> None:
+        lines = ["    after spaces"]
+        control = self.controlLines(1, lines, self.newlines)
+        self.assertEqual(control.get_lines(), tobytes(lines))
+
+    def test_too_high(self) -> None:
+        control = self.controlNums(3, 1, self.newlines)
+        self.assertEqual(control.get_lines(), [b"0"])
+
     def test_updown(self) -> None:
         control = self.controlNums(3, 5, self.newlines)
         self.assertEqual(control.get_lines(), [b"0", b"1", b"2"])
         self.assertEqual(control.get_lines(), [b"0", b"1", b"2"])
         control.go_down()
         self.assertEqual(control.get_lines(), [b"1", b"2", b"3"])
         control.go_down()
```

