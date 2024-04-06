# Comparing `tmp/antidb-2024.3.14.tar.gz` & `tmp/antidb-2024.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "antidb-2024.3.14.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "antidb-2024.4.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `antidb-2024.3.14.tar` & `antidb-2024.4.6.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     8878 2023-09-28 19:55:43.040932 antidb-2024.3.14/README.md
--rw-r--r--   0        0        0     1054 2024-03-14 18:14:46.918505 antidb-2024.3.14/pyproject.toml
--rw-r--r--   0        0        0      248 2023-09-28 22:42:51.365775 antidb-2024.3.14/src/antidb/__init__.py
--rw-r--r--   0        0        0    12188 2024-03-13 20:42:26.088345 antidb-2024.3.14/src/antidb/antidb.py
--rw-r--r--   0        0        0     6875 2024-03-13 20:57:39.938599 antidb-2024.3.14/src/antidb/antisrt.py
--rw-r--r--   0        0        0     9739 1970-01-01 00:00:00.000000 antidb-2024.3.14/PKG-INFO
+-rw-r--r--   0        0        0     8878 2023-09-28 19:55:43.040932 antidb-2024.4.6/README.md
+-rw-r--r--   0        0        0     1053 2024-04-06 21:10:13.935674 antidb-2024.4.6/pyproject.toml
+-rw-r--r--   0        0        0      248 2023-09-28 22:42:51.365775 antidb-2024.4.6/src/antidb/__init__.py
+-rw-r--r--   0        0        0    12996 2024-04-06 19:20:19.118953 antidb-2024.4.6/src/antidb/antidb.py
+-rw-r--r--   0        0        0     8127 2024-03-27 09:50:55.182907 antidb-2024.4.6/src/antidb/antisrt.py
+-rw-r--r--   0        0        0     9738 1970-01-01 00:00:00.000000 antidb-2024.4.6/PKG-INFO
```

### Comparing `antidb-2024.3.14/README.md` & `antidb-2024.4.6/README.md`

 * *Files identical despite different names*

### Comparing `antidb-2024.3.14/pyproject.toml` & `antidb-2024.4.6/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core>=3.9.0"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "antidb"
-version = "2024.3.14"
+version = "2024.4.6"
 authors = [
     { name="Platon Bykadorov", email="platon.work@gmail.com" },
 ]
 description = "The simplest index-and-search engine for huge multiline text files. Focused primarily on bioinformatics. Inspired by tabix, but isn't its replacement. Written in Python. Works on top of Zstandard Seekable & pyzstd SeekableZstdFile."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `antidb-2024.3.14/src/antidb/antidb.py` & `antidb-2024.4.6/src/antidb/antidb.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,24 +6,23 @@
                     Any)
 from datetime import datetime
 from io import TextIOWrapper
 from decimal import Decimal
 from warnings import warn
 from bisect import bisect
 from functools import partial
-from .antisrt import (SrtRules,
-                      Srt)
+from .antisrt import Srt
 from pyzstd import (CParameter,
                     SeekableZstdFile,
                     ZstdFile)
 
-__version__ = 'v2.6.0'
+__version__ = 'v2.8.1'
 __authors__ = [{'name': 'Platon Bykadorov',
                 'email': 'platon.work@gmail.com',
-                'years': '2023'}]
+                'years': '2023-2024'}]
 
 
 def count_exec_time(any_func: Callable) -> Callable:
     def wrapper(*args: Any, **kwargs: Any):
         exec_time_start = datetime.now()
         any_func_res = any_func(*args, **kwargs)
         return (any_func.__name__,
@@ -40,39 +39,50 @@
 
 
 class Idx(Srt):
     def __init__(self,
                  db_file_path: str,
                  idx_prefix: str,
                  your_line_parser: Callable,
+                 your_line_parser_kwargs: None | dict = None,
                  compr_level: int = 6,
                  compr_frame_size: int = 1024 * 1024,
                  compr_chunk_size: int = 1024 * 1024 * 1024,
                  compr_chunk_elems_quan: int = 10000000,
                  unidx_lines_quan: int = 1000,
                  srt_rule: None | Callable = None,
-                 **srt_rule_kwargs: Any):
+                 srt_rule_kwargs: None | dict = None,
+                 cols_delimiter: str | None = '\t',
+                 col_inds: None | int | list | tuple = None):
         self.db_file_path = os.path.normpath(db_file_path)
         if os.path.basename(db_file_path).endswith('.zst'):
             self.db_zst_path = self.db_file_path[:]
         else:
             self.db_zst_path = self.db_file_path + '.zst'
         self.idx_prefix = idx_prefix
         self.your_line_parser = your_line_parser
+        if your_line_parser_kwargs:
+            self.your_line_parser_kwargs = your_line_parser_kwargs
+        else:
+            self.your_line_parser_kwargs = {}
         self.full_idx_path = f'{self.db_zst_path}.{self.idx_prefix}.full'
         self.full_idx_tmp_path = self.full_idx_path + '.tmp'
         self.full_idx_tmp_srtd_path = self.full_idx_tmp_path + '.srtd'
         self.mem_idx_path = f'{self.db_zst_path}.{self.idx_prefix}.mem'
         self.compr_settings = {CParameter.compressionLevel: compr_level}
         self.compr_frame_size = compr_frame_size
         self.compr_chunk_size = compr_chunk_size
         self.compr_chunk_elems_quan = compr_chunk_elems_quan
         self.unidx_lines_quan = unidx_lines_quan
+        if not srt_rule_kwargs:
+            srt_rule_kwargs = {}
         super().__init__(unsrtd_file_path=self.full_idx_tmp_path,
                          srt_rule=srt_rule,
+                         cols_delimiter=cols_delimiter,
+                         col_inds=col_inds,
                          **srt_rule_kwargs)
         self.perf = []
 
     def idx(self):
         if not os.path.exists(self.db_zst_path):
             self.perf.append(self.crt_db_zst())
             os.remove(self.db_file_path)
@@ -130,15 +140,16 @@
                 while True:
                     db_zst_lstart = db_zst_opened.tell()
                     db_zst_line = db_zst_opened.readline()
                     if not db_zst_line:
                         if chunk:
                             full_idx_tmp_opened.write('\n'.join(chunk) + '\n')
                         break
-                    your_line_parser_out = self.your_line_parser(db_zst_line)
+                    your_line_parser_out = self.your_line_parser(db_zst_line,
+                                                                 **self.your_line_parser_kwargs)
                     if not your_line_parser_out:
                         continue
                     elif type(your_line_parser_out) in [str, int, float, Decimal]:
                         chunk.append(f'{your_line_parser_out},{db_zst_lstart}')
                     elif type(your_line_parser_out) in [list, tuple, set]:
                         for your_val in your_line_parser_out:
                             chunk.append(f'{your_val},{db_zst_lstart}')
@@ -165,15 +176,15 @@
     def crt_mem_idx(self):
         with TextIOWrapper(SeekableZstdFile(self.full_idx_path,
                                             mode='r')) as full_idx_opened:
             with TextIOWrapper(ZstdFile(self.mem_idx_path,
                                         mode='w',
                                         level_or_option=self.compr_settings)) as mem_idx_opened:
                 mem_idx_opened.write(f'idx_srt_rule_name={self.srt_rule.__name__}\n')
-                mem_idx_opened.write(f'idx_srt_rule_kwargs={self.srt_rule_kwargs}\n')
+                mem_idx_opened.write(f'idx_srt_rule_settings={self.srt_rule_settings}\n')
                 mem_idx_opened.write(f'unidx_lines_quan={self.unidx_lines_quan}\n')
                 while True:
                     full_idx_lstart = full_idx_opened.tell()
                     full_idx_line = full_idx_opened.readline()
                     if not full_idx_line:
                         break
                     full_idx_your_val = full_idx_line.split(',')[0]
@@ -184,20 +195,24 @@
 
 
 class Prs(Idx):
     def __init__(self,
                  db_file_path: str,
                  idx_prefix: str,
                  srt_rule: None | Callable = None,
-                 **srt_rule_kwargs: Any):
+                 srt_rule_kwargs: None | dict = None,
+                 cols_delimiter: str | None = '\t',
+                 col_inds: None | int | list | tuple = None):
         super().__init__(db_file_path,
                          idx_prefix,
                          your_line_parser=None,
                          srt_rule=srt_rule,
-                         **srt_rule_kwargs)
+                         srt_rule_kwargs=srt_rule_kwargs,
+                         cols_delimiter=cols_delimiter,
+                         col_inds=col_inds)
         if not os.path.exists(self.db_zst_path):
             raise FileNotFoundError(self.db_zst_path)
         else:
             self.db_zst_opened = TextIOWrapper(SeekableZstdFile(self.db_zst_path,
                                                                 mode='r'))
         if not os.path.exists(self.full_idx_path):
             raise FileNotFoundError(self.full_idx_path)
@@ -206,33 +221,33 @@
                                                                   mode='r'))
         if not os.path.exists(self.mem_idx_path):
             raise FileNotFoundError(self.mem_idx_path)
         else:
             self.mem_idx_opened = TextIOWrapper(ZstdFile(self.mem_idx_path,
                                                          mode='r'))
         mem_idx = self.read_mem_idx()
-        self.idx_srt_rule_name, self.idx_srt_rule_kwargs, self.unidx_lines_quan = mem_idx[:3]
+        self.idx_srt_rule_name, self.idx_srt_rule_settings, self.unidx_lines_quan = mem_idx[:3]
         self.mem_idx_your_vals, self.full_idx_lstarts = mem_idx[3:]
         if self.idx_srt_rule_name != self.srt_rule.__name__:
             warn(f"""Your sort key name ({self.srt_rule.__name__}) doesn't
-                 match the index sort key name ({self.idx_srt_rule_name})""")
-        if self.idx_srt_rule_kwargs != self.srt_rule_kwargs:
-            warn(f"""Your sort key arguments ({self.srt_rule_kwargs}) don't
-                 match the index sort key arguments ({self.idx_srt_rule_kwargs})""")
+match the index sort key name ({self.idx_srt_rule_name})""")
+        if self.idx_srt_rule_settings != str(self.srt_rule_settings):
+            warn(f"""Your sort key settings ({self.srt_rule_settings}) don't
+match the index sort key settings ({self.idx_srt_rule_settings})""")
 
     def read_mem_idx(self):
         idx_srt_rule_name = self.mem_idx_opened.readline().rstrip().split('=')[1]
-        idx_srt_rule_kwargs = eval(self.mem_idx_opened.readline().rstrip().split('=')[1])
+        idx_srt_rule_settings = self.mem_idx_opened.readline().rstrip().split('=')[1]
         unidx_lines_quan = int(self.mem_idx_opened.readline().rstrip().split('=')[1])
         mem_idx_your_vals, full_idx_lstarts = [], []
         for mem_idx_line in self.mem_idx_opened:
             mem_idx_row = mem_idx_line.rstrip().split(',')
             mem_idx_your_vals.append(mem_idx_row[0])
-            full_idx_lstarts.append(int(mem_idx_row[1]))
-        return (idx_srt_rule_name, idx_srt_rule_kwargs, unidx_lines_quan,
+            full_idx_lstarts.append(int(mem_idx_row[-1]))
+        return (idx_srt_rule_name, idx_srt_rule_settings, unidx_lines_quan,
                 mem_idx_your_vals, full_idx_lstarts)
 
     def prs(self,
             your_vals: list | tuple | set | dict | str | int | float | Decimal) -> str:
         if type(your_vals) in [str,
                                int,
                                float,
@@ -249,16 +264,16 @@
             self.full_idx_opened.seek(full_idx_lstart)
             for line_idx in range(self.unidx_lines_quan + 1):
                 full_idx_line = self.full_idx_opened.readline()
                 if not full_idx_line:
                     break
                 full_idx_row = full_idx_line.rstrip().split(',')
                 if your_val == full_idx_row[0]:
-                    self.db_zst_opened.seek(int(full_idx_row[1]))
+                    self.db_zst_opened.seek(int(full_idx_row[-1]))
                     yield self.db_zst_opened.readline()
                     for full_idx_line in self.full_idx_opened:
                         full_idx_row = full_idx_line.rstrip().split(',')
                         if your_val != full_idx_row[0]:
                             break
-                        self.db_zst_opened.seek(int(full_idx_row[1]))
+                        self.db_zst_opened.seek(int(full_idx_row[-1]))
                         yield self.db_zst_opened.readline()
                     break
```

### Comparing `antidb-2024.3.14/src/antidb/antisrt.py` & `antidb-2024.4.6/src/antidb/antisrt.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 import os
 from typing import (Callable,
                     Any)
 from inspect import stack
 from heapq import merge
 from functools import partial
 
-__version__ = 'v2.1.0'
+__version__ = 'v3.0.0'
 __authors__ = [{'name': 'Platon Bykadorov',
                 'email': 'platon.work@gmail.com',
-                'years': '2023'}]
+                'years': '2023-2024'}]
 
 
 class DelimitersMatchError(Exception):
     def __init__(self,
                  cols_delimiter,
                  dec_delimiter):
         err_msg = f'''\nColums delimiter ({cols_delimiter})
@@ -26,38 +26,50 @@
                  func_name):
         err_msg = f'''\nThere are no source file(s)
 for {func_name} function/method'''
         super().__init__(err_msg)
 
 
 class SrtRules():
-    @staticmethod
-    def natur(src_file_line: str,
-              cols_delimiter: str = '\t',
+    def __init__(self,
+                 cols_delimiter: str | None = '\t',
+                 col_inds: None | int | list | tuple = None):
+        self.cols_delimiter = cols_delimiter
+        self.col_inds = col_inds
+
+    def get_cols(self,
+                 src_file_line: str):
+        if self.cols_delimiter:
+            src_file_row = src_file_line.rstrip().split(self.cols_delimiter)
+        else:
+            src_file_row = [src_file_line.rstrip()]
+        if type(self.col_inds) is int:
+            src_file_row = [src_file_row[self.col_inds]]
+        elif type(self.col_inds) in [list, tuple]:
+            src_file_row = [src_file_row[col_ind]
+                            for col_ind in self.col_inds]
+        return src_file_row
+
+    def natur(self,
+              src_file_line: str,
               dec_delimiter: str = '.',
-              col_inds: None | int | list | tuple = None,
               nums_first: bool = True) -> list:
-        if cols_delimiter == dec_delimiter:
-            raise DelimitersMatchError(cols_delimiter,
+        if self.cols_delimiter == dec_delimiter:
+            raise DelimitersMatchError(self.cols_delimiter,
                                        dec_delimiter)
-        src_file_row = src_file_line.rstrip().split(cols_delimiter)
-        if type(col_inds) is int:
-            src_file_row = [src_file_row[col_inds]]
-        elif type(col_inds) in [list, tuple]:
-            src_file_row = [src_file_row[col_ind]
-                            for col_ind in col_inds]
+        src_file_row = self.get_cols(src_file_line)
         if dec_delimiter == '.':
-            split_cell = r'(-?\d+(?:\.\d*)?(?:[Ee][+-]?\d+)?)'
+            natur_split_cell = r'(-?\d+(?:\.\d*)?(?:[Ee][+-]?\d+)?)'
         elif dec_delimiter == ',':
-            split_cell = r'(-?\d+(?:,\d*)?(?:[Ee][+-]?\d+)?)'
+            natur_split_cell = r'(-?\d+(?:,\d*)?(?:[Ee][+-]?\d+)?)'
         spl_file_row = []
         for cell in src_file_row:
             subcells = list(filter(lambda subcell:
                                    subcell,
-                                   re.split(split_cell,
+                                   re.split(natur_split_cell,
                                             cell)))
             for subcell_ind in range(len(subcells)):
                 try:
                     subcells[subcell_ind] = int(subcells[subcell_ind])
                 except ValueError:
                     try:
                         subcells[subcell_ind] = float(subcells[subcell_ind])
@@ -71,37 +83,56 @@
                 if nums_first:
                     subcells.insert(0, float('+inf'))
                 else:
                     subcells.insert(0, float('-inf'))
             spl_file_row.append(subcells)
         return spl_file_row
 
+    def letts_nums(self,
+                   src_file_line: str) -> list:
+        src_file_row = self.get_cols(src_file_line)
+        spl_file_row = []
+        for cell in src_file_row:
+            letts = re.search(r'^[a-zA-Z]+',
+                              cell).group()
+            nums = int(re.search(f'(?<=^{letts})\d+$',
+                                 cell).group())
+            spl_file_row.append([letts,
+                                 nums])
+        return spl_file_row
+
 
 class Srt(SrtRules):
     def __init__(self,
                  unsrtd_file_path: None | str = None,
                  presrtd_file_paths: None | list = None,
                  srt_rule: None | Callable = None,
+                 cols_delimiter: str | None = '\t',
+                 col_inds: None | int | list | tuple = None,
                  **srt_rule_kwargs: Any):
         if unsrtd_file_path:
             self.unsrtd_file_path = os.path.normpath(unsrtd_file_path)
         else:
             self.unsrtd_file_path = None
         if presrtd_file_paths:
             self.presrtd_file_paths = presrtd_file_paths
         else:
             self.presrtd_file_paths = []
+        super().__init__(cols_delimiter,
+                         col_inds)
         if srt_rule:
             self.srt_rule = srt_rule
         else:
             self.srt_rule = self.natur
         if srt_rule_kwargs:
             self.srt_rule_kwargs = srt_rule_kwargs
         else:
             self.srt_rule_kwargs = {}
+        self.srt_rule_settings = {'cols_delimiter': self.cols_delimiter,
+                                  'col_inds': self.col_inds} | self.srt_rule_kwargs
 
     @staticmethod
     def iter_file(file_path: str) -> str:
         with open(file_path) as file_opened:
             for file_line in file_opened:
                 yield file_line
```

### Comparing `antidb-2024.3.14/PKG-INFO` & `antidb-2024.4.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antidb
-Version: 2024.3.14
+Version: 2024.4.6
 Summary: The simplest index-and-search engine for huge multiline text files. Focused primarily on bioinformatics. Inspired by tabix, but isn't its replacement. Written in Python. Works on top of Zstandard Seekable & pyzstd SeekableZstdFile.
 Keywords: python,search-engine,parser,performance,bioinformatics,big-data,dbms,indexer,zstd,zstandard,seekable,pyzstd
 Author-email: Platon Bykadorov <platon.work@gmail.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

