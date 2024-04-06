# Comparing `tmp/DrissionRecorder-3.4.12.tar.gz` & `tmp/DrissionRecorder-3.4.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DrissionRecorder-3.4.12.tar", last modified: Fri Mar  8 00:50:56 2024, max compression
+gzip compressed data, was "DrissionRecorder-3.4.13.tar", last modified: Sat Apr  6 15:10:27 2024, max compression
```

## Comparing `DrissionRecorder-3.4.12.tar` & `DrissionRecorder-3.4.13.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2024-03-08 00:50:56.299885 DrissionRecorder-3.4.12/
-drwxrwxrwx   0        0        0        0 2024-03-08 00:50:56.284049 DrissionRecorder-3.4.12/DataRecorder/
--rw-rw-rw-   0        0        0      164 2024-03-08 00:41:48.000000 DrissionRecorder-3.4.12/DataRecorder/__init__.py
--rw-rw-rw-   0        0        0     6145 2023-09-04 13:51:02.000000 DrissionRecorder-3.4.12/DataRecorder/base.py
--rw-rw-rw-   0        0        0     1862 2023-09-04 06:32:26.000000 DrissionRecorder-3.4.12/DataRecorder/base.pyi
--rw-rw-rw-   0        0        0     1753 2023-08-16 02:32:26.000000 DrissionRecorder-3.4.12/DataRecorder/byte_recorder.py
--rw-rw-rw-   0        0        0      532 2023-08-17 00:59:46.000000 DrissionRecorder-3.4.12/DataRecorder/byte_recorder.pyi
--rw-rw-rw-   0        0        0     6404 2024-03-08 00:41:48.000000 DrissionRecorder-3.4.12/DataRecorder/db_recorder.py
--rw-rw-rw-   0        0        0      989 2024-03-08 00:41:48.000000 DrissionRecorder-3.4.12/DataRecorder/db_recorder.pyi
--rw-rw-rw-   0        0        0    21905 2024-01-03 06:45:47.000000 DrissionRecorder-3.4.12/DataRecorder/filler.py
--rw-rw-rw-   0        0        0     2876 2023-10-11 07:38:37.000000 DrissionRecorder-3.4.12/DataRecorder/filler.pyi
--rw-rw-rw-   0        0        0     9397 2023-09-05 07:25:47.000000 DrissionRecorder-3.4.12/DataRecorder/recorder.py
--rw-rw-rw-   0        0        0      988 2023-08-31 06:16:48.000000 DrissionRecorder-3.4.12/DataRecorder/recorder.pyi
--rw-rw-rw-   0        0        0    13977 2024-03-08 00:41:48.000000 DrissionRecorder-3.4.12/DataRecorder/setter.py
--rw-rw-rw-   0        0        0     3196 2023-10-11 07:38:37.000000 DrissionRecorder-3.4.12/DataRecorder/setter.pyI
-drwxrwxrwx   0        0        0        0 2024-03-08 00:50:56.284049 DrissionRecorder-3.4.12/DataRecorder/style/
--rw-rw-rw-   0        0        0       77 2023-08-04 03:31:44.000000 DrissionRecorder-3.4.12/DataRecorder/style/__init__.py
--rw-rw-rw-   0        0        0    28558 2023-08-04 03:31:44.000000 DrissionRecorder-3.4.12/DataRecorder/style/cell_style.py
--rw-rw-rw-   0        0        0     9416 2024-03-08 00:41:48.000000 DrissionRecorder-3.4.12/DataRecorder/tools.py
--rw-rw-rw-   0        0        0      989 2024-03-08 00:41:48.000000 DrissionRecorder-3.4.12/DataRecorder/tools.pyi
-drwxrwxrwx   0        0        0        0 2024-03-08 00:50:56.299885 DrissionRecorder-3.4.12/DrissionRecorder.egg-info/
--rw-rw-rw-   0        0        0     4847 2024-03-08 00:50:55.000000 DrissionRecorder-3.4.12/DrissionRecorder.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      677 2024-03-08 00:50:55.000000 DrissionRecorder-3.4.12/DrissionRecorder.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-08 00:50:55.000000 DrissionRecorder-3.4.12/DrissionRecorder.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-03-08 00:50:55.000000 DrissionRecorder-3.4.12/DrissionRecorder.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-03-08 00:50:55.000000 DrissionRecorder-3.4.12/DrissionRecorder.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1083 2021-08-17 07:03:54.000000 DrissionRecorder-3.4.12/LICENSE
--rw-rw-rw-   0        0        0       26 2023-04-28 02:15:42.000000 DrissionRecorder-3.4.12/MANIFEST.in
--rw-rw-rw-   0        0        0     4847 2024-03-08 00:50:56.299885 DrissionRecorder-3.4.12/PKG-INFO
--rw-rw-rw-   0        0        0     4339 2023-09-04 09:33:58.000000 DrissionRecorder-3.4.12/README.md
--rw-rw-rw-   0        0        0       42 2024-03-08 00:50:56.299885 DrissionRecorder-3.4.12/setup.cfg
--rw-rw-rw-   0        0        0      913 2024-03-08 00:49:42.000000 DrissionRecorder-3.4.12/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-06 15:10:27.672838 DrissionRecorder-3.4.13/
+drwxrwxrwx   0        0        0        0 2024-04-06 15:10:27.631317 DrissionRecorder-3.4.13/DrissionRecorder/
+-rw-rw-rw-   0        0        0      164 2024-04-06 15:04:16.000000 DrissionRecorder-3.4.13/DrissionRecorder/__init__.py
+-rw-rw-rw-   0        0        0     6240 2024-04-06 15:04:16.000000 DrissionRecorder-3.4.13/DrissionRecorder/base.py
+-rw-rw-rw-   0        0        0     1954 2024-04-06 15:04:16.000000 DrissionRecorder-3.4.13/DrissionRecorder/base.pyi
+-rw-rw-rw-   0        0        0     1818 2024-04-06 15:04:16.000000 DrissionRecorder-3.4.13/DrissionRecorder/byte_recorder.py
+-rw-rw-rw-   0        0        0      536 2024-04-06 15:04:16.000000 DrissionRecorder-3.4.13/DrissionRecorder/byte_recorder.pyi
+-rw-rw-rw-   0        0        0     6538 2024-04-06 15:04:16.000000 DrissionRecorder-3.4.13/DrissionRecorder/db_recorder.py
+-rw-rw-rw-   0        0        0      992 2024-04-06 15:04:16.000000 DrissionRecorder-3.4.13/DrissionRecorder/db_recorder.pyi
+-rw-rw-rw-   0        0        0    23153 2024-04-06 15:04:16.000000 DrissionRecorder-3.4.13/DrissionRecorder/filler.py
+-rw-rw-rw-   0        0        0     3287 2024-04-06 15:04:16.000000 DrissionRecorder-3.4.13/DrissionRecorder/filler.pyi
+-rw-rw-rw-   0        0        0     7078 2024-04-06 15:04:16.000000 DrissionRecorder-3.4.13/DrissionRecorder/recorder.py
+-rw-rw-rw-   0        0        0      988 2024-04-06 15:04:16.000000 DrissionRecorder-3.4.13/DrissionRecorder/recorder.pyi
+-rw-rw-rw-   0        0        0    14182 2024-04-06 15:04:16.000000 DrissionRecorder-3.4.13/DrissionRecorder/setter.py
+-rw-rw-rw-   0        0        0     3118 2024-04-06 15:04:16.000000 DrissionRecorder-3.4.13/DrissionRecorder/setter.pyI
+drwxrwxrwx   0        0        0        0 2024-04-06 15:10:27.657208 DrissionRecorder-3.4.13/DrissionRecorder/style/
+-rw-rw-rw-   0        0        0       77 2024-04-06 15:04:16.000000 DrissionRecorder-3.4.13/DrissionRecorder/style/__init__.py
+-rw-rw-rw-   0        0        0    28558 2024-04-06 15:04:16.000000 DrissionRecorder-3.4.13/DrissionRecorder/style/cell_style.py
+-rw-rw-rw-   0        0        0    15846 2024-04-06 15:04:16.000000 DrissionRecorder-3.4.13/DrissionRecorder/tools.py
+-rw-rw-rw-   0        0        0     1935 2024-04-06 15:04:16.000000 DrissionRecorder-3.4.13/DrissionRecorder/tools.pyi
+drwxrwxrwx   0        0        0        0 2024-04-06 15:10:27.657208 DrissionRecorder-3.4.13/DrissionRecorder.egg-info/
+-rw-rw-rw-   0        0        0     4512 2024-04-06 15:10:27.000000 DrissionRecorder-3.4.13/DrissionRecorder.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      745 2024-04-06 15:10:27.000000 DrissionRecorder-3.4.13/DrissionRecorder.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-06 15:10:27.000000 DrissionRecorder-3.4.13/DrissionRecorder.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-04-06 15:10:27.000000 DrissionRecorder-3.4.13/DrissionRecorder.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-04-06 15:10:27.000000 DrissionRecorder-3.4.13/DrissionRecorder.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1083 2024-04-06 15:04:16.000000 DrissionRecorder-3.4.13/LICENSE
+-rw-rw-rw-   0        0        0       30 2024-04-06 15:07:18.000000 DrissionRecorder-3.4.13/MANIFEST.in
+-rw-rw-rw-   0        0        0     4512 2024-04-06 15:10:27.672838 DrissionRecorder-3.4.13/PKG-INFO
+-rw-rw-rw-   0        0        0     4000 2024-04-06 15:07:18.000000 DrissionRecorder-3.4.13/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-06 15:10:27.672838 DrissionRecorder-3.4.13/setup.cfg
+-rw-rw-rw-   0        0        0      921 2024-04-06 15:07:18.000000 DrissionRecorder-3.4.13/setup.py
```

### Comparing `DrissionRecorder-3.4.12/DataRecorder/base.py` & `DrissionRecorder-3.4.13/DrissionRecorder/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,30 +6,32 @@
 
 from .setter import OriginalSetter, BaseSetter
 from .tools import get_usable_path
 
 
 class OriginalRecorder(object):
     """记录器的基类"""
-    SUPPORTS = ('any',)
+    _SUPPORTS = ('any',)
 
     def __init__(self, path=None, cache_size=None):
         """
         :param path: 保存的文件路径
         :param cache_size: 每接收多少条记录写入文件，0为不自动写入
         """
         self._data = None
+        self._style_data = None
         self._path = None
         self._type = None
         self._lock = Lock()
         self._pause_add = False  # 文件写入时暂停接收输入
         self._pause_write = False  # 标记文件正在被一个线程写入
         self.show_msg = True
         self._setter = None
         self._data_count = 0  # 已缓存数据的条数
+        self._file_exists = False
 
         if path:
             self.set.path(path)
         self._cache = cache_size if cache_size is not None else 1000
 
     def __del__(self):
         """对象关闭时把剩下的数据写入文件"""
@@ -73,15 +75,15 @@
             new_path = str(get_usable_path(new_path))
             return_path = self._path = new_path
 
             if Path(original_path).exists():
                 from shutil import copy
                 copy(original_path, self._path)
 
-        if not self._data:
+        if not self._data and not self._style_data:
             return return_path
 
         if not self._path:
             raise ValueError('保存路径为空。')
 
         with self._lock:
             self._pause_add = True  # 写入文件前暂缓接收数据
@@ -147,15 +149,15 @@
         :return: None
         """
         self.set.path(path)
 
 
 class BaseRecorder(OriginalRecorder):
     """Recorder、Filler和DBRecorder的父类"""
-    SUPPORTS = ('xlsx', 'csv')
+    _SUPPORTS = ('xlsx', 'csv')
 
     def __init__(self, path=None, cache_size=None):
         """
         :param path: 保存的文件路径
         :param cache_size: 每接收多少条记录写入文件，0为不自动写入
         """
         super().__init__(path, cache_size)
```

### Comparing `DrissionRecorder-3.4.12/DataRecorder/base.pyi` & `DrissionRecorder-3.4.13/DrissionRecorder/base.pyi`

 * *Files 26% similar despite different names*

```diff
@@ -4,28 +4,30 @@
 from threading import Lock
 from typing import Union, Any, Optional
 
 from .setter import OriginalSetter, BaseSetter
 
 
 class OriginalRecorder(object):
-    SUPPORTS: tuple = ...
+    _SUPPORTS: tuple = ...
     _cache: int = ...
     _path: Optional[str] = ...
     _type: Optional[str] = ...
-    _data: Optional[list, dict] = ...
+    _data: Union[list, dict, None] = ...
+    _style_data: Union[list, dict, None] = ...
     _lock: Lock = ...
     _pause_add: bool = ...
     _pause_write: bool = ...
     show_msg: bool = ...
     _setter: Optional[OriginalSetter] = ...
     _data_count: int = ...
+    _file_exists: bool = ...
 
     def __init__(self,
-                 path: Optional[str, Path] = None,
+                 path: Union[str, Path, None] = None,
                  cache_size: int = None) -> None: ...
 
     def __del__(self) -> None: ...
 
     @property
     def set(self) -> OriginalSetter: ...
 
@@ -37,34 +39,34 @@
 
     @property
     def type(self) -> str: ...
 
     @property
     def data(self) -> Union[dict, list]: ...
 
-    def record(self, new_path: Optional[str, Path] = None) -> str: ...
+    def record(self, new_path: Union[None, str, Path] = None) -> str: ...
 
     def clear(self) -> None: ...
 
     @abstractmethod
     def add_data(self, data): ...
 
     @abstractmethod
     def _record(self): ...
 
 
 class BaseRecorder(OriginalRecorder):
-    SUPPORTS: tuple = ...
+    _SUPPORTS: tuple = ...
     _encoding: str = ...
     _before: list = ...
     _after: list = ...
     _table: Optional[str] = ...
     _setter: BaseSetter = ...
 
-    def __init__(self, path: Optional[str, Path] = None, cache_size: int = None) -> None: ...
+    def __init__(self, path: Union[None, str, Path] = None, cache_size: int = None) -> None: ...
 
     @property
     def set(self) -> BaseSetter: ...
 
     @property
     def before(self) -> Any: ...
```

### Comparing `DrissionRecorder-3.4.12/DataRecorder/byte_recorder.py` & `DrissionRecorder-3.4.13/DrissionRecorder/byte_recorder.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 from time import sleep
 
 from .base import OriginalRecorder
 
 
 class ByteRecorder(OriginalRecorder):
-    SUPPORTS = ('any',)
+    _SUPPORTS = ('any',)
     __END = (0, 2)
 
     def __init__(self, path=None, cache_size=None):
         """用于记录字节数据的工具
         :param path: 保存的文件路径
         :param cache_size: 每接收多少条记录写入文件，0为不自动写入
         """
@@ -34,17 +34,18 @@
         self._data_count += 1
 
         if 0 < self.cache_size <= self._data_count:
             self.record()
 
     def _record(self):
         """记录数据到文件"""
-        if not Path(self.path).exists():
+        if not self._file_exists and not Path(self.path).exists():
             with open(self.path, 'w'):
                 pass
+            self._file_exists = True
 
         with open(self.path, 'rb+') as f:
             previous = None
             for i in self._data:
                 loc = ByteRecorder.__END if i[1] is None else (i[1], 0)
                 if not (previous == loc == ByteRecorder.__END):
                     f.seek(loc[0], loc[1])
```

### Comparing `DrissionRecorder-3.4.12/DataRecorder/byte_recorder.pyi` & `DrissionRecorder-3.4.13/DrissionRecorder/byte_recorder.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 from pathlib import Path
 from typing import Union, Optional
 
 from .base import OriginalRecorder
 
 
 class ByteRecorder(OriginalRecorder):
-    SUPPORTS: tuple = ...
+    _SUPPORTS: tuple = ...
     __END: tuple = ...
     _data: list = ...
     data: list = ...
 
     def __init__(self,
-                 path: Optional[str, Path] = None,
+                 path: Union[None, str, Path] = None,
                  cache_size: int = None): ...
 
     def add_data(self,
                  data: bytes,
                  seek: int = None) -> None: ...
 
     def _record(self) -> None: ...
```

### Comparing `DrissionRecorder-3.4.12/DataRecorder/db_recorder.py` & `DrissionRecorder-3.4.13/DrissionRecorder/db_recorder.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # -*- coding:utf-8 -*-
 from pathlib import Path
 from sqlite3 import connect
 from time import sleep
 
 from .base import BaseRecorder
 from .setter import DBSetter
-from .tools import data_to_list_or_dict, ok_list
+from .tools import data_to_list_or_dict, ok_list, data_to_list_or_dict_simplify
 
 
 class DBRecorder(BaseRecorder):
-    SUPPORTS = ('db',)
+    _SUPPORTS = ('db',)
 
     def __init__(self, path=None, cache_size=None, table=None):
         """用于存储数据到sqlite的工具
         :param path: 保存的文件路径
         :param cache_size: 每接收多少条记录写入文件，0为不自动写入
         :param table: 默认表名
         """
@@ -54,15 +54,19 @@
         # 一维数组
         elif isinstance(data, dict) or (
                 isinstance(data, (list, tuple)) and not isinstance(data[0], (list, tuple, dict))):
             self._data.setdefault(table, []).append(data_to_list_or_dict(self, data))
             self._data_count += 1
 
         else:  # 二维数组
-            self._data.setdefault(table, []).extend([data_to_list_or_dict(self, d) for d in data])
+            if self.after or self.before:
+                dd = [data_to_list_or_dict(self, d) for d in data]
+            else:
+                dd = [data_to_list_or_dict_simplify(d) for d in data]
+            self._data.setdefault(table, []).extend(dd)
             self._data_count += len(data)
 
         if 0 < self.cache_size <= self._data_count:
             self.record()
 
     def run_sql(self, sql, single=True, commit=False):
         """执行sql语句并返回结果
@@ -77,17 +81,15 @@
         if commit:
             self._conn.commit()
         self._close_connection()
         return r
 
     def _connect(self):
         """连接数据库"""
-        path = Path(self.path).parent
-        if not path.exists():
-            path.mkdir(parents=True, exist_ok=True)
+        Path(self.path).parent.mkdir(parents=True, exist_ok=True)
         self._conn = connect(self.path)
         self._cur = self._conn.cursor()
 
     def _close_connection(self):
         """关闭数据库 """
         if self._conn is not None:
             try:
```

### Comparing `DrissionRecorder-3.4.12/DataRecorder/db_recorder.pyi` & `DrissionRecorder-3.4.13/DrissionRecorder/db_recorder.pyi`

 * *Files 11% similar despite different names*

```diff
@@ -20,15 +20,15 @@
                  table: str = None): ...
 
     @property
     def set(self) -> DBSetter: ...
 
     def add_data(self, data: Any, table: str = None) -> None: ...
 
-    def run_sql(self, sql: str, single: bool = True, commit: bool = False) -> Optional[list, tuple]: ...
+    def run_sql(self, sql: str, single: bool = True, commit: bool = False) -> Union[None, list, tuple]: ...
 
     def _connect(self) -> None: ...
 
     def _close_connection(self) -> None: ...
 
     def _record(self) -> None: ...
```

### Comparing `DrissionRecorder-3.4.12/DataRecorder/filler.py` & `DrissionRecorder-3.4.13/DrissionRecorder/filler.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 # -*- coding:utf-8 -*-
 from csv import reader as csv_reader, writer as csv_writer
 from pathlib import Path
 from time import sleep
 
-from openpyxl import load_workbook, Workbook
+from openpyxl import load_workbook
 from openpyxl.utils import get_column_letter
 
 from .base import BaseRecorder
 from .setter import FillerSetter
 from .style.cell_style import CellStyle, NoneStyle
-from .tools import parse_coord, get_usable_coord, process_content, data_to_list_or_dict
+from .tools import (parse_coord, get_usable_coord, process_content, data_to_list_or_dict, ok_list, get_usable_coord_int,
+                    data_to_list_or_dict_simplify, get_css_head, get_wb, get_ws, get_xlsx_head, create_csv)
 
 
 class Filler(BaseRecorder):
     def __init__(self, path=None, cache_size=None, key_cols=True, begin_row=2,
                  sign_col=True, data_col=None, sign=None, deny_sign=False):
         """用于处理表格文件的工具
         :param path: 保存的文件路径
@@ -30,14 +31,16 @@
         self._quote_char = '"'  # csv文件引用符
         self._key_cols = None
         self._begin_row = None
         self._sign_col = None
         self._data_col = None
         self._sign = None
         self._deny_sign = False
+        self._fit_head = False
+        self._style_data = {}
         self.row_num_title = 'row'
         if not data_col:
             data_col = sign_col if sign_col else 1
         self.set.path(path, key_cols, begin_row, sign_col, data_col, sign, deny_sign)
         s = CellStyle()
         s.font.set_color("0000FF")
         s.font.set_underline('single')
@@ -74,31 +77,25 @@
         return self._begin_row
 
     @property
     def keys(self):
         """返回一个列表，由未执行的行数据组成。每行的格式为第一位为行号，其余为 key 列的值。
         eg.[3, '张三', 20]
         """
-        if not self.path or not Path(self.path).exists():
-            raise FileNotFoundError('未指定文件或文件不存在。')
-
         if self.type == 'csv':
             return get_csv_keys(self, False)
         elif self.type == 'xlsx':
             return get_xlsx_keys(self, False)
 
     @property
     def dict_keys(self):
         """返回一个列表，由未执行的行数据组成。每行的格式为dict，'row' 值为行号，其余值为第一行数据。
         如第一行数据为空，则用列号为值。如果begin_row为1，用列名作为值。
         eg.{'row': 2, 'name': '张三', 'C': '男'}
         """
-        if not self.path or not Path(self.path).exists():
-            raise FileNotFoundError('未指定文件或文件不存在。')
-
         if self.type == 'csv':
             return get_csv_keys(self, True)
         elif self.type == 'xlsx':
             return get_xlsx_keys(self, True)
 
     @property
     def set(self):
@@ -131,241 +128,170 @@
         """
         while self._pause_add:  # 等待其它线程写入结束
             sleep(.1)
 
         if not isinstance(data, (list, tuple)):
             data = (data,)
 
-        if coord not in ('set_link', 'cover_style', 'replace_style', 'set_img', 'set_width', 'set_height'):
+        to = self._data
+        if coord in ('cover_style', 'replace_style', 'set_width', 'set_height'):
+            to = self._style_data
+
+        elif coord not in ('set_link', 'set_img'):
             coord = parse_coord(coord, self.data_col)
             if not data:
                 data = ([],)
                 self._data_count += 1
             # 一维数组
             elif isinstance(data, dict) or (
                     isinstance(data, (list, tuple)) and not isinstance(data[0], (list, tuple, dict))):
                 data = (data_to_list_or_dict(self, data),)
                 self._data_count += 1
             else:  # 二维数组
-                data = [data_to_list_or_dict(self, d) for d in data]
+                if self.after or self.before:
+                    data = [data_to_list_or_dict(self, d) for d in data]
+                else:
+                    data = [data_to_list_or_dict_simplify(d) for d in data]
                 self._data_count += len(data)
 
+        else:
+            self._data_count += 1
+
         if self._type != 'xlsx':
-            self._data.append((coord, data))
+            to.append((coord, data))
 
         else:
             if table is None:
                 table = self._table
             elif isinstance(table, bool):
                 table = None
-
-            self._data.setdefault(table, []).append((coord, data))
+            to.setdefault(table, []).append((coord, data))
 
         if 0 < self.cache_size <= self._data_count:
             self.record()
 
-    def set_link(self, coord, link, content=None):
+    def set_link(self, coord, link, content=None, table=None):
         """为单元格设置超链接
         :param coord: 单元格坐标
         :param link: 超链接，为None时删除链接
         :param content: 单元格内容
+        :param table: 数据表名，仅支持xlsx格式。为None表示用set.table()方法设置的值，为bool表示活动的表格
         :return: None
         """
-        self.add_data((coord, link, content), 'set_link')
+        self.add_data((coord, link, content), 'set_link', table)
 
-    def set_style(self, coord, style, replace=True):
-        """为单元格设置样式
-        :param coord: 单元格坐标，输入数字可设置整行，输入列名字符串可设置整列，输入'A1:C5'格式可设置指定范围
+    def set_style(self, coord, style, replace=True, table=None):
+        """为单元格设置样式，可批量设置范围内的单元格
+        :param coord: 单元格坐标，输入数字可设置整行，输入列名字符串可设置整列，输入'A1:C5'、'a:d'、'1:5'格式可设置指定范围
         :param style: CellStyle对象，为None则清除单元格样式
         :param replace: 是否直接替换已有样式，运行效率较高，但不能单独修改某个属性
+        :param table: 数据表名，仅支持xlsx格式。为None表示用set.table()方法设置的值，为bool表示活动的表格
         :return: None
         """
         s = 'replace_style' if replace else 'cover_style'
-        self.add_data((coord, style), s)
+        self.add_data((coord, style), s, table)
 
-    def set_img(self, coord, img_path, width=None, height=None):
+    def set_img(self, coord, img_path, width=None, height=None, table=None):
         """
         :param coord: 单元格坐标，输入数字可设置整行，输入列名字符串可设置整列，输入'A1:C5'格式可设置指定范围
         :param img_path: 图片路径
         :param width: 图片宽
         :param height: 图片高
+        :param table: 数据表名，仅支持xlsx格式。为None表示用set.table()方法设置的值，为bool表示活动的表格
         :return: None
         """
         if isinstance(img_path, Path):
             img_path = str(img_path)
-        self.add_data((coord, img_path, width, height), 'set_img')
+        self.add_data((coord, img_path, width, height), 'set_img', table)
 
-    def set_row_height(self, row, height):
-        """设置行高
-        :param row: 行号
+    def set_row_height(self, row, height, table=None):
+        """设置行高，可设置连续多行
+        :param row: 行号，可传入范围，如'1:4'
         :param height: 行高
+        :param table: 数据表名，仅支持xlsx格式。为None表示用set.table()方法设置的值，为bool表示活动的表格
         :return: None
         """
-        self.add_data((row, height), 'set_height')
+        self.add_data((row, height), 'set_height', table)
 
-    def set_col_width(self, col, width):
-        """设置列宽
-        :param col: 列号，数字或字母
+    def set_col_width(self, col, width, table=None):
+        """设置列宽，可设置连续多列
+        :param col: 列号，数字或字母，可传入范围，如'1:4'、'a:d'
         :param width: 列宽
+        :param table: 数据表名，仅支持xlsx格式。为None表示用set.table()方法设置的值，为bool表示活动的表格
         :return: None
         """
-        if isinstance(col, int):
-            col = get_column_letter(col)
-        self.add_data((col, width), 'set_width')
+        self.add_data((col, width), 'set_width', table)
 
     def _record(self):
         """记录数据"""
         if self.type == 'xlsx':
             self._to_xlsx()
         elif self.type == 'csv':
             self._to_csv()
+        self._style_data = {}
 
     def _to_xlsx(self):
         """填写数据到xlsx文件"""
-        if Path(self.path).exists():
-            wb = load_workbook(self.path)
-            new = False
-        else:
-            wb = Workbook()
-            new = True
-
+        wb, new_file = get_wb(self)
         tables = [i.title for i in wb.worksheets]
-        for table, table_data in self._data.items():
-            if table is None:
-                ws = wb.active
-
-            else:
-                if table in tables:
-                    ws = wb[table]
-                elif new is True:
-                    new = False
-                    ws = wb.active
-                    ws.title = table
-                    tables.append(table)
-                else:
-                    ws = wb.create_sheet(title=table)
-                    tables.append(table)
-
-            max_col = ws.max_column
-            empty = ws.max_column == ws.max_row == 1 and ws[1][0].value is None
 
-            for data in table_data:
-                if empty:  # 如果是空文件，最大行数设为0，避免直接添加时出现空行
-                    max_row = 0
+        for table in {}.fromkeys(list(self._data.keys()) + list(self._style_data.keys())):
+            ws, new_sheet = get_ws(wb, table, tables, new_file)
+            begin = get_xlsx_head(self, new_file, new_sheet, self._data[table][0], ws, True)
+            empty = not any([i.value for i in ws[1]]) and ws.max_row == 1
+            head = self._head.get(ws.title, None) if self._fit_head else None
+
+            if self._data:  # 处理表头
+                for table_data in self._data[table][begin:]:
+                    set_data_to_ws(ws, table_data, empty, head, self)
                     empty = False
-                else:
-                    max_row = ws.max_row
-
-                if data[0] == 'set_link':
-                    coord = parse_coord(data[1][0], self.data_col)
-                    row, col = get_usable_coord(coord, max_row, max_col)
-                    cell = ws.cell(row, col)
-                    has_link = True if cell.hyperlink else Filler
-                    cell.hyperlink = None if data[1][1] is None else process_content(data[1][1], True)
-                    if data[1][2] is not None:
-                        cell.value = process_content(data[1][2], True)
-                    if data[1][1]:
-                        if self._link_style:
-                            self._link_style.to_cell(cell, replace=False)
-                    elif has_link:
-                        NoneStyle().to_cell(cell, replace=False)
-                    continue
-
-                elif data[0] in ('replace_style', 'cover_style'):
-                    mode = data[0] == 'replace_style'
-                    coord = data[1][0]
-                    style = NoneStyle() if data[1][1] is None else data[1][1]
-                    if isinstance(coord, int) or (isinstance(coord, str) and coord.isdigit()):
-                        for c in ws[coord]:
-                            style.to_cell(c, replace=mode)
-                        continue
-
-                    elif isinstance(coord, str) and ':' in coord:
-                        for c in ws[coord]:
-                            for cc in c:
-                                style.to_cell(cc, replace=mode)
-                        continue
-
-                    coord = parse_coord(coord, self.data_col)
-                    row, col = get_usable_coord(coord, max_row, max_col)
-                    style.to_cell(ws.cell(row, col), replace=mode)
-                    continue
-
-                elif data[0] == 'set_img':
-                    coord, img_path, width, height = data[1]
-                    coord = parse_coord(coord, self.data_col)
-                    row, col = get_usable_coord(coord, max_row, max_col)
-
-                    from openpyxl.drawing.image import Image
-                    from openpyxl.utils import get_column_letter
-                    img = Image(img_path)
-                    if width and height:
-                        img.width = width
-                        img.height = height
-                    elif width:
-                        img.height = int(img.height * (width / img.width))
-                        img.width = width
-                    elif height:
-                        img.width = int(img.width * (height / img.height))
-                        img.height = height
-                    col = get_column_letter(col)
-                    ws.add_image(img, f'{col}{row}')
-                    continue
-
-                elif data[0] == 'set_width':
-                    col, width = data[1]
-                    ws.column_dimensions[col].width = width
-                    continue
-
-                elif data[0] == 'set_height':
-                    row, height = data[1]
-                    ws.row_dimensions[row].height = height
-                    continue
 
-                row, col = get_usable_coord(data[0], max_row, max_col)
-                now_data = (data[1],) if not isinstance(data[1][0], (list, tuple, dict)) else data[1]
+            if self._style_data:
+                for table_data in self._style_data[table]:
+                    set_style_to_ws(ws, table_data, self)
 
-                for r, i in enumerate(now_data, row):
-                    if isinstance(i, dict):
-                        i = i.values()
-                    for key, j in enumerate(i):
-                        ws.cell(r, col + key).value = process_content(j, True)
+            new_file = False
 
         wb.save(self.path)
         wb.close()
 
     def _to_csv(self):
         """填写数据到xlsx文件"""
-        if not Path(self.path).exists():
-            with open(self.path, 'w', encoding=self.encoding):
-                pass
+        if self._head is not None and not self._file_exists:
+            create_csv(self)
+        elif self._head is None:
+            get_css_head(self, True)
 
         with open(self.path, 'r', encoding=self.encoding) as f:
             reader = csv_reader(f, delimiter=self.delimiter, quotechar=self.quote_char)
             lines = list(reader)
             lines_count = len(lines)
 
             for i in self._data:
                 if i[0] == 'set_link':
                     coord = parse_coord(i[1][0], self.data_col)
                     now_data = (f'=HYPERLINK("{i[1][1]}","{i[1][2] or i[1][1]}")',)
 
-                elif i[0] in ('cover_style', 'replace_style', 'set_img', 'set_width', 'set_height'):
+                elif i[0] == 'set_img':
                     continue
 
                 else:
                     coord = i[0]
                     now_data = i[1]
 
-                row, col = get_usable_coord(coord, lines_count, len(lines[0]) if lines_count else 1)
+                row, col = get_usable_coord_int(coord, lines_count, len(lines[0]) if lines_count else 1)
                 now_data = (now_data,) if not isinstance(now_data[0], (list, tuple, dict)) else now_data
 
                 for r, data in enumerate(now_data, row):
                     if isinstance(data, dict):
-                        data = list(data.values())
+                        if self._fit_head and self._head:
+                            data = ok_list([data.get(h, None) for h in self._head])
+                            col = 1
+                        else:
+                            data = ok_list(data.values())
 
                     for _ in range(r - lines_count):  # 若行数不够，填充行数
                         lines.append([])
                         lines_count += 1
 
                     row_num = r - 1
 
@@ -493,15 +419,15 @@
             else:
                 t = [x if x else get_column_letter(k) for k, x in enumerate(lines[0], 1)
                      if filler.key_cols is True or k in filler.key_cols]
 
             if len(t) != len(set(t)):
                 raise RuntimeError('表头内容重复。')
             if filler.row_num_title in t:
-                raise RuntimeError(f'表头"{filler.row_num_title}"列与行号列重复，请用set.row_num_title()方法设置不同的表头。')
+                raise RuntimeError(f'表头"{filler.row_num_title}"列与行号列重复，用set.row_num_title()设置表头。')
             title.extend(t)
 
         if sign_col is not True:  # 获取符合条件的行
             sign_col -= 1
             for ind, line in enumerate(lines[begin_row:], begin_row + 1):
                 row_sign = '' if sign_col > len(line) - 1 else line[sign_col]
                 if row_sign != sign if filler.deny_sign else row_sign == sign:
@@ -516,7 +442,109 @@
                     res.append([ind] + line)
                 else:  # 只获取对应的列
                     res.append([ind] + [line[i - 1] for i in filler.key_cols])
 
     if as_dict:
         res = [dict(zip(title, v)) for v in res]
     return res
+
+
+def set_data_to_ws(ws, data, empty, head, filler):
+    """批量写入数据到sheet"""
+    max_row = 0 if empty else ws.max_row
+    if data[0] == 'set_link':
+        coord = parse_coord(data[1][0], filler.data_col)
+        row, col = get_usable_coord(coord, max_row, ws)
+        cell = ws.cell(row, col)
+        has_link = True if cell.hyperlink else Filler
+        cell.hyperlink = None if data[1][1] is None else process_content(data[1][1], True)
+        if data[1][2] is not None:
+            cell.value = process_content(data[1][2], True)
+        if data[1][1]:
+            if filler._link_style:
+                filler._link_style.to_cell(cell, replace=False)
+        elif has_link:
+            NoneStyle().to_cell(cell, replace=False)
+        return
+
+    elif data[0] == 'set_img':
+        coord, img_path, width, height = data[1]
+        coord = parse_coord(coord, filler.data_col)
+        row, col = get_usable_coord(coord, max_row, ws)
+
+        from openpyxl.drawing.image import Image
+        img = Image(img_path)
+        if width and height:
+            img.width = width
+            img.height = height
+        elif width:
+            img.height = int(img.height * (width / img.width))
+            img.width = width
+        elif height:
+            img.width = int(img.width * (height / img.height))
+            img.height = height
+        col = get_column_letter(col)
+        ws.add_image(img, f'{col}{row}')
+        return
+
+    row, col = get_usable_coord(data[0], max_row, ws)
+    now_data = (data[1],) if not isinstance(data[1][0], (list, tuple, dict)) else data[1]
+
+    if head:  # 自动匹配表头
+        for r, i in enumerate(now_data, row):
+            if isinstance(i, dict):
+                i = [i.get(h, None) for h in head]
+                col = 1
+
+            for key, j in enumerate(i):
+                ws.cell(r, col + key).value = process_content(j, True)
+
+    else:
+        for r, i in enumerate(now_data, row):
+            if isinstance(i, dict):
+                i = i.values()
+            for key, j in enumerate(i):
+                ws.cell(r, col + key).value = process_content(j, True)
+
+
+def set_style_to_ws(ws, data, filler):
+    """批量设置单元格格式到sheet"""
+    if data[0] in ('replace_style', 'cover_style'):
+        mode = data[0] == 'replace_style'
+        coord = data[1][0]
+        style = NoneStyle() if data[1][1] is None else data[1][1]
+        if isinstance(coord, int) or (isinstance(coord, str) and coord.isdigit()):
+            for c in ws[coord]:
+                style.to_cell(c, replace=mode)
+            return
+
+        elif isinstance(coord, str):
+            if ':' in coord:
+                for c in ws[coord]:
+                    for cc in c:
+                        style.to_cell(cc, replace=mode)
+                return
+            elif coord.isdigit() or coord.isalpha():
+                for c in ws[coord]:
+                    style.to_cell(c, replace=mode)
+                return
+
+        coord = parse_coord(coord, filler.data_col)
+        row, col = get_usable_coord(coord, ws.max_row, ws)
+        style.to_cell(ws.cell(row, col), replace=mode)
+
+    elif data[0] == 'set_width':
+        col, width = data[1]
+        if isinstance(col, int):
+            col = get_column_letter(col)
+        for c in col.split(':'):
+            if c.isdigit():
+                c = get_column_letter(int(c))
+            ws.column_dimensions[c].width = width
+
+    elif data[0] == 'set_height':
+        row, height = data[1]
+        if isinstance(row, int):
+            ws.row_dimensions[row].height = height
+        elif isinstance(row, str):
+            for r in row.split(':'):
+                ws.row_dimensions[int(r)].height = height
```

### Comparing `DrissionRecorder-3.4.12/DataRecorder/filler.pyi` & `DrissionRecorder-3.4.13/DrissionRecorder/filler.pyi`

 * *Files 24% similar despite different names*

```diff
@@ -5,47 +5,50 @@
 from .base import BaseRecorder
 from .style import CellStyle
 from .setter import FillerSetter
 
 
 class Filler(BaseRecorder):
     _set: FillerSetter = ...
-    _key_cols: Optional[List[int], bool] = ...
-    _begin_row: Optional[str, int] = ...
-    _sign_col: Optional[int, bool] = ...
+    _key_cols: Union[List[int], bool, None] = ...
+    _begin_row: Union[None, str, int] = ...
+    _sign_col: Union[None, int, bool] = ...
     _data_col: Optional[int] = ...
     _sign: Any = ...
     _deny_sign: bool = ...
     _link_style: CellStyle = ...
     _quote_char: str = ...
     _delimiter: str = ...
     _data: Union[list, dict] = ...
+    _head: Union[None, list, dict] = ...
+    _fit_head: bool = ...
     data: Union[list, dict] = ...
     row_num_title: str = ...
+    _style_data: Union[list, dict] = ...
 
-    def __init__(self, path: Optional[str, Path] = None,
+    def __init__(self, path: Union[None, str, Path] = None,
                  cache_size: int = None,
                  key_cols: Union[str, int, list, tuple, bool] = True,
                  begin_row: int = 2,
                  sign_col: Union[str, int, bool] = True,
-                 data_col: Optional[int, str] = None,
+                 data_col: Union[None, int, str] = None,
                  sign: Any = None,
                  deny_sign: bool = False) -> None: ...
 
     @property
     def sign(self) -> str: ...
 
     @property
     def deny_sign(self) -> bool: ...
 
     @property
     def key_cols(self) -> Union[List[int], bool]: ...
 
     @property
-    def sign_col(self) -> Optional[int, bool]: ...
+    def sign_col(self) -> Union[None, int, bool]: ...
 
     @property
     def data_col(self) -> int: ...
 
     @property
     def begin_row(self) -> Union[str, int]: ...
 
@@ -61,31 +64,36 @@
     @property
     def delimiter(self) -> str: ...
 
     @property
     def quote_char(self) -> str: ...
 
     def add_data(self, data: Any,
-                 coord: Union[list, Tuple[Optional[int, str], Union[int, str]], str, int] = 'newline',
+                 coord: Union[list, Tuple[Union[None, int, str], Union[int, str]], str, int] = 'newline',
                  table: Union[str, bool] = None) -> None: ...
 
     def set_link(self,
                  coord: Union[int, str, tuple, list],
                  link: Optional[str],
-                 content: Optional[int, str, float] = None) -> None: ...
+                 content: Union[None, int, str, float] = None,
+                 table: Union[str, bool] = None) -> None: ...
 
     def set_style(self, coord: Union[int, str, tuple, list], style: Optional[CellStyle],
-                  replace: bool = True) -> None: ...
+                  replace: bool = True,
+                  table: Union[str, bool] = None) -> None: ...
 
-    def set_img(self, coord: Union[int, str, tuple, list], img_path: Optional[str, Path], width: float = None,
-                height: float = None) -> None: ...
+    def set_img(self, coord: Union[int, str, tuple, list], img_path: Union[None, str, Path], width: float = None,
+                height: float = None,
+                table: Union[str, bool] = None) -> None: ...
 
-    def set_row_height(self, row: int, height: float) -> None: ...
+    def set_row_height(self, row: Union[int, str], height: float,
+                       table: Union[str, bool] = None) -> None: ...
 
-    def set_col_width(self, col: Union[int, str], width: float) -> None: ...
+    def set_col_width(self, col: Union[int, str], width: float,
+                      table: Union[str, bool] = None) -> None: ...
 
     def _record(self) -> None: ...
 
     def _to_xlsx(self) -> None: ...
 
     def _to_csv(self) -> None: ...
```

### Comparing `DrissionRecorder-3.4.12/DataRecorder/recorder.pyi` & `DrissionRecorder-3.4.13/DrissionRecorder/recorder.pyi`

 * *Files identical despite different names*

### Comparing `DrissionRecorder-3.4.12/DataRecorder/setter.py` & `DrissionRecorder-3.4.13/DrissionRecorder/setter.py`

 * *Files 4% similar despite different names*

```diff
@@ -82,35 +82,37 @@
         :param encoding: 编码格式
         :return: None
         """
         self._recorder._encoding = encoding
 
 
 class SheetLikeSetter(BaseSetter):
-    def head(self, head, table=None):
+    def head(self, head, table=None, to_file=True):
         """设置表头。只有 csv 和 xlsx 格式支持设置表头
         :param head: 表头，列表或元组
         :param table: 表名，只xlsx格式文件有效
+        :param to_file: 是否写入到文件
         :return: None
         """
-        if not self._recorder.path:
-            raise FileNotFoundError('未指定文件。')
-        if not isinstance(head, (list, tuple)):
-            raise TypeError('head参数只能是list或tuple格式。')
-
-        if self._recorder.type == 'xlsx':
-            table = table or self._recorder.table
-            set_xlsx_head(self._recorder.path, head, table)
-
-        elif self._recorder.type == 'csv':
-            set_csv_head(self._recorder.path, head, self._recorder.encoding, self._recorder.delimiter,
-                         self._recorder.quote_char)
+        self._recorder.record()
+        with self._recorder._lock:
+            if not self._recorder.path:
+                raise FileNotFoundError('未指定文件。')
+            if not isinstance(head, (list, tuple)):
+                raise TypeError('head参数只能是list或tuple格式。')
+
+            if self._recorder.type == 'xlsx':
+                table = table or self._recorder.table
+                set_xlsx_head(self._recorder, head, table, to_file)
 
-        else:
-            raise TypeError('只能对xlsx和csv文件设置表头。')
+            elif self._recorder.type == 'csv':
+                set_csv_head(self._recorder, head, to_file)
+
+            else:
+                raise TypeError('只能对xlsx和csv文件设置表头。')
 
     def delimiter(self, delimiter):
         """设置csv文件分隔符
         :param delimiter: 分隔符
         :return: None
         """
         self._recorder._delimiter = delimiter
@@ -136,31 +138,47 @@
                 file_type = suffix[1:]
             elif not self._recorder.type:
                 file_type = 'csv'
 
         if file_type:
             self.file_type(file_type)
 
-        self._recorder._data = {} if self._recorder._type == 'xlsx' else []
+        if self._recorder._type == 'xlsx':
+            self._recorder._data = {}
+            self._recorder._head = {}
+            self._recorder._style_data = {}
+        else:
+            self._recorder._data = []
+            self._recorder._head = None
 
     def file_type(self, file_type):
         """指定文件类型，无视文件后缀名"""
-        if 'any' not in self._recorder.SUPPORTS and file_type not in self._recorder.SUPPORTS:
-            raise TypeError(f'只支持{"、".join(self._recorder.SUPPORTS)}格式文件。')
+        if 'any' not in self._recorder._SUPPORTS and file_type not in self._recorder._SUPPORTS:
+            raise TypeError(f'只支持{"、".join(self._recorder._SUPPORTS)}格式文件。')
         self._recorder._type = file_type
 
     def table(self, name):
         """设置默认表名
         :param name: 表名
         :return: None
         """
         if isinstance(name, bool):
             name = None
         self._recorder._table = name
 
+    def fit_head(self, on_off=True):
+        """设置是否自动匹配表头
+        :param on_off: bool表示开关
+        :return: None
+        """
+        if self._recorder.type not in ('csv', 'xlsx'):
+            raise TypeError('只有csv或xlsx格式可设置fit_head。')
+        self._recorder.record()
+        self._recorder._fit_head = on_off
+
 
 class FillerSetter(SheetLikeSetter):
     def sign(self, value):
         """设置sign值
         :param value: 筛选条件
         :return: None
         """
@@ -284,40 +302,14 @@
         """设置文件路径
         :param path: 文件路径
         :param file_type: 要设置的文件类型，为空则从文件名中获取
         :return: None
         """
         super().path(path=path, file_type=file_type)
         self._recorder._row_styles = None
-        self._recorder._head = {} if self._recorder.type == 'xlsx' else None
-
-    def head(self, head, table=None):
-        """设置表头。只有 csv 和 xlsx 格式支持设置表头
-        :param head: 表头，列表或元组
-        :param table: 表名，只xlsx格式文件有效
-        :return: None
-        """
-        super().head(head, table)
-        if self._recorder.type == 'xlsx':
-            if not self._recorder._head or not isinstance(self._recorder._head, dict):
-                self._recorder._head = {table: head}
-            else:
-                self._recorder._head[table] = head
-
-        elif self._recorder.type == 'csv':
-            self._recorder._head = head
-
-    def fit_head(self, on_off=True):
-        """设置是否自动匹配表头
-        :param on_off: bool表示开关
-        :return: None
-        """
-        if self._recorder.type not in ('csv', 'xlsx'):
-            raise TypeError('只有csv或xlsx格式可设置fit_head。')
-        self._recorder._fit_head = on_off
 
 
 class DBSetter(BaseSetter):
     def path(self, path, table=None):
         """重写父类方法
         :param path: 文件路径
         :param table: 数据表名称
@@ -336,65 +328,81 @@
                 r = self._recorder.run_sql("select name from sqlite_master where type='table'")
                 self._recorder._table = r[0] if r else None
 
             self._recorder._data = {}
             self._recorder._close_connection()
 
 
-def set_csv_head(file_path, head, encoding='utf-8', delimiter=',', quote_char='"'):
+def set_csv_head(recorder, head, to_file):
     """设置csv文件的表头
-    :param file_path: 文件路径
+    :param recorder: Recorder或Filler对象
     :param head: 表头列表或元组
-    :param encoding: 编码
-    :param delimiter: 分隔符
-    :param quote_char: 引用符
+    :param to_file: 是否写入文件
     :return: None
     """
+    recorder._head = head
+    if not to_file:
+        return
+
     from csv import writer
-    if Path(file_path).exists():
-        with open(file_path, 'r', newline='', encoding=encoding) as f:
+    if recorder._file_exists or Path(recorder.path).exists():
+        with open(recorder.path, 'r', newline='', encoding=recorder._encoding) as f:
             content = "".join(f.readlines()[1:])
 
-        with open(file_path, 'w', newline='', encoding=encoding) as f:
-            csv_write = writer(f, delimiter=delimiter, quotechar=quote_char)
+        with open(recorder.path, 'w', newline='', encoding=recorder._encoding) as f:
+            csv_write = writer(f, delimiter=recorder._delimiter, quotechar=recorder._quote_char)
             csv_write.writerow(ok_list(head))
 
-        with open(file_path, 'a+', newline='', encoding=encoding) as f:
+        with open(recorder.path, 'a+', newline='', encoding=recorder._encoding) as f:
             f.write(f'{content}')
 
     else:
-        Path(file_path).parent.mkdir(parents=True, exist_ok=True)
-        with open(file_path, 'w', newline='', encoding=encoding) as f:
-            csv_write = writer(f, delimiter=delimiter, quotechar=quote_char)
+        Path(recorder.path).parent.mkdir(parents=True, exist_ok=True)
+        with open(recorder.path, 'w', newline='', encoding=recorder._encoding) as f:
+            csv_write = writer(f, delimiter=recorder._delimiter, quotechar=recorder._quote_char)
             csv_write.writerow(ok_list(head))
 
 
-def set_xlsx_head(file_path, head, table):
+def set_xlsx_head(recorder, head, table, to_file):
     """设置xlsx文件的表头
-    :param file_path: 文件路径
+    :param recorder: Recorder或Filler对象
     :param head: 表头列表或元组
     :param table: 工作表名称
+    :param to_file: 是否写入文件
     :return: None
     """
-    if Path(file_path).exists():
-        wb = load_workbook(file_path)
+    if not to_file:
+        if table:
+            recorder._head[table] = head
+        elif recorder._file_exists or Path(recorder.path).exists():
+            wb = load_workbook(recorder.path)
+            ws = wb.active
+            recorder._head[ws.title] = head
+            wb.close()
+        else:
+            recorder._head['Sheet'] = head
+        return
+
+    if recorder._file_exists or Path(recorder.path).exists():
+        wb = load_workbook(recorder.path)
         if table:
             ws = wb[table] if table in [i.title for i in wb.worksheets] else wb.create_sheet(title=table)
         else:
             ws = wb.active
 
     else:
-        Path(file_path).parent.mkdir(parents=True, exist_ok=True)
+        Path(recorder.path).parent.mkdir(parents=True, exist_ok=True)
         wb = Workbook()
         ws = wb.active
         if table:
             ws.title = table
 
     if len(ws[1]) > len(head):
         head = list(head)
         head.extend([None] * (len(ws[1]) - len(head)))
 
     for key, i in enumerate(head, 1):
         ws.cell(1, key).value = process_content(i, True)
 
-    wb.save(file_path)
+    recorder._head[ws.title] = head
+    wb.save(recorder.path)
     wb.close()
```

### Comparing `DrissionRecorder-3.4.12/DataRecorder/setter.pyI` & `DrissionRecorder-3.4.13/DrissionRecorder/setter.pyI`

 * *Files 7% similar despite different names*

```diff
@@ -32,26 +32,28 @@
 
     def encoding(self, encoding: str) -> None: ...
 
 
 class SheetLikeSetter(BaseSetter):
     _recorder: Union[Filler, Recorder] = ...
 
-    def head(self, head: Union[list, tuple], table: str = None) -> None: ...
+    def head(self, head: Union[list, tuple], table: str = None, to_file: bool = True) -> None: ...
 
     def delimiter(self, delimiter: str) -> None: ...
 
     def quote_char(self, quote_char: str) -> None: ...
 
     def path(self, path: Union[str, Path], file_type: str = None) -> None: ...
 
     def file_type(self, file_type: str) -> None: ...
 
     def table(self, name: Union[str, bool]) -> None: ...
 
+    def fit_head(self, on_off: bool = True) -> None: ...
+
 
 class FillerSetter(SheetLikeSetter):
     _recorder: Filler = ...
 
     def __init__(self, recorder: Filler): ...
 
     def sign(self, value: Any) -> None: ...
@@ -84,25 +86,20 @@
 
     def col_height(self, height: float) -> None: ...
 
     def style(self, style: CellStyle) -> None: ...
 
     def path(self, path: Union[str, Path], file_type: str = None) -> None: ...
 
-    def head(self, head: Union[list, tuple], table: str = None) -> None: ...
-
-    def fit_head(self, on_off: bool = True) -> None: ...
-
 
 class DBSetter(BaseSetter):
     _recorder: DBRecorder = ...
 
     def __init__(self, recorder: DBRecorder): ...
 
     def path(self, path: Union[str, Path], table: Optional[str] = None) -> None: ...
 
 
-def set_csv_head(file_path: str, head: Union[list, tuple], encoding: str = 'utf-8', delimiter: str = ',',
-                 quote_char: str = '"'): ...
+def set_csv_head(recorder: Union[Recorder, Filler], head: Union[list, tuple], to_file: bool): ...
 
 
-def set_xlsx_head(file_path: str, head: Union[list, tuple], table: str) -> None: ...
+def set_xlsx_head(recorder: Union[Recorder, Filler], head: Union[list, tuple], table: str, to_file: bool) -> None: ...
```

### Comparing `DrissionRecorder-3.4.12/DataRecorder/style/cell_style.py` & `DrissionRecorder-3.4.13/DrissionRecorder/style/cell_style.py`

 * *Files identical despite different names*

### Comparing `DrissionRecorder-3.4.12/DataRecorder/tools.pyi` & `DrissionRecorder-3.4.13/DrissionRecorder/tools.pyi`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 # -*- coding:utf-8 -*-
 from pathlib import Path
 from typing import Union, Tuple, Any, Optional
 
+from openpyxl.worksheet.worksheet import Worksheet
+
 from .base import BaseRecorder
+from .filler import Filler
+from .recorder import Recorder
 
 
 def align_csv(path: Union[str, Path], encoding: str = 'utf-8', delimiter: str = ',', quotechar: str = '"') -> None: ...
 
 
 def get_usable_path(path: Union[str, Path], is_file: bool = True, parents: bool = True) -> Path: ...
 
@@ -16,17 +20,43 @@
 
 def get_long(txt) -> int: ...
 
 
 def parse_coord(coord: Optional[int, str, list, tuple] = None, data_col: int = None) -> Tuple[Optional[int], int]: ...
 
 
-def process_content(content: Any, excel: bool = False) -> Optional[int, str, float]: ...
+def process_content(content: Any, excel: bool = False) -> Union[None, int, str, float]: ...
 
 
 def ok_list(data_list: Union[list, dict], excel: bool = False, as_str: bool = False) -> list: ...
 
 
-def get_usable_coord(coord: Union[tuple, list], max_row: int, max_col: int) -> Tuple[int, int]: ...
+def get_usable_coord_int(coord: Union[tuple, list],
+                         max_row: int,
+                         max_col: Union[int, Worksheet]) -> Tuple[int, int]: ...
+
+
+def get_usable_coord(coord: Union[tuple, list],
+                     max_row: int,
+                     ws: Worksheet) -> Tuple[int, int]: ...
+
+
+def data_to_list_or_dict_simplify(data: Union[list, tuple, dict, None]) -> Union[list, dict]: ...
+
+
+def data_to_list_or_dict(recorder: BaseRecorder, data: Union[list, tuple, dict, None]) -> Union[list, dict]: ...
+
+
+def get_css_head(recorder: Union[Recorder, Filler], is_filler: bool = False) -> Optional[list]: ...
+
+
+def get_xlsx_head(recorder: Union[Recorder, Filler], new_file: bool, new_sheet: bool,
+                  first_data:Union[dict, list, tuple], ws: Worksheet, is_filler: bool = False) -> int: ...
+
+
+def create_csv(recorder: Union[Recorder, Filler]) -> None: ...
+
+
+def get_wb(recorder: Union[Recorder, Filler]) -> tuple: ...
 
 
-def data_to_list_or_dict(recorder: BaseRecorder, data: Union[list, tuple, dict]) -> Union[list, dict]: ...
+def get_ws(wb, table, tables, new_file) -> tuple: ...
```

### Comparing `DrissionRecorder-3.4.12/DrissionRecorder.egg-info/PKG-INFO` & `DrissionRecorder-3.4.13/DrissionRecorder.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 Metadata-Version: 2.1
 Name: DrissionRecorder
-Version: 3.4.12
+Version: 3.4.13
 Summary: 用于记录数据的模块。
-Home-page: https://gitee.com/g1879/DataRecorder
+Home-page: https://gitee.com/g1879/DrissionRecorder
 Author: g1879
 Author-email: g1879@qq.com
 License: MIT
 Keywords: DrissionRecorder
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: BSD License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ⭐️ 简介
 
-本库是一个基于 python 的工具集，用于记录数据到文件（含 sqlite）。
+本库是一个基于 python 的工具集，用于记录数据到文件。
 
-使用方便，代码简洁， 是一个可靠、省心且实用的工具。
+使用方便，代码简洁，是一个可靠、省心且实用的工具。
 
-还支持多线程同时写入文件。
+支持多线程同时写入文件。
 
 **交流QQ群：** 897838127
 
 **联系邮箱：** g1879@qq.com
 
-**使用手册：** 📒[点击打开](http://g1879.gitee.io/datarecorderdocs/)
+**使用手册：** 📒[点击打开](http://g1879.gitee.io/DrissionRecorderDocs/)
 
 # ✨️ 理念
 
 简单，可靠，省心。
 
 # 📕 背景
 
@@ -62,67 +62,63 @@
 ## ⚡ 记录器`Recorder`
 
 `Recorder`的功能简单直观高效实用，只做一个动作，就是不断接收数据，按顺序往文件里添加。可以接收单行数据，或二维数据一次写入多行。
 
 它支持 csv、xlsx、json、txt 四种格式文件。
 
 ```python
-from DataRecorder import Recorder
+from DrissionRecorder import Recorder
 
 data = ((1, 2, 3, 4), 
         (5, 6, 7, 8))
 
 r = Recorder('data.csv')
 r.add_data(data)  # 一次记录多行数据
 r.add_data('abc')  # 记录单行数据
 ```
 
 ## ⚡ 表格填充器`Filler`
 
-`Filler`用于对表格文件填写数据，可以指定填其坐标。它的使用非常灵活，可以指定坐标为左上角，填入一片二维数据。还封装了记录数据处理进度的功能（比如断点续爬）。除此以外，它还能给单元格设置链接。
+`Filler`用于对表格文件填写数据，可以指定填其坐标。它的使用非常灵活，可以指定坐标为左上角，填入一片二维数据。还封装了记录数据处理进度的功能（比如断点续爬）。
+
+除此以外，它还能给单元格设置链接和样式。
 
 它只支持 csv 和 xlsx 格式文件。
 
 ```python
-from DataRecorder import Filler
+from DrissionRecorder import Filler
 
 f = Filler('results.csv')
 f.add_data((1, 2, 3, 4), 'a2')  # 从A2单元格开始，写入一行数据
 f.add_data(((1, 2), (3, 4)), 'd4')  # 以D4单元格为左上角，写入一片二维数据
 ```
 
 ## ⚡ 二进制数据记录器`ByteRecorder`
 
 `ByteRecorder`用法最简单，它和`Recorder`类似，记录多个数据然后按顺序写入文件。不一样的是它只接收二进制数据，每次`add_data()`只能输入一条数据，而且没有行的概念。
 
-可以用来和作者的另一个工具 [FlowViewer](https://gitee.com/g1879/FlowViewer) 配合使用，用来获取浏览器加载的文件，或用来记录下载的文件。可指定每个数据写入文件中的位置，以支持多线程下载文件。
-
 支持任意文件格式。
 
 ```python
-from DataRecorder import ByteRecorder
+from DrissionRecorder import ByteRecorder
 
 b = ByteRecorder('data.file')
-b.add_data(b'xxxxxxxxxxx')  # 向文件写入二进制数据
+b.add_data(b'*****************')  # 向文件写入二进制数据
 ```
 
 ## ⚡ 数据库记录器`DBRecorder`
 
 支持 sqlite，用法和`Recorder`一致，支持自动创建数据库、数据表、数据列。
 
 ```python
-from DataRecorder import DBRecorder
+from DrissionRecorder import DBRecorder
 
 d = DBRecorder('data.db')
 d.add_data({'name': '张三', 'age': 25}, table='user')  # 插入数据到user表
 d.record()
 ```
 
-# 🛠 使用方法
-
-[📒点击跳转到使用手册](http://g1879.gitee.io/datarecorderdocs/)
-
 # ☕ 请我喝咖啡
 
 如果本项目对您有所帮助，不妨请作者我喝杯咖啡 ：）
 
-![](https://gitee.com/g1879/DrissionPage-demos/raw/master/pics/code.jpg)
+![](https://gitee.com/g1879/DrissionPageDocs/raw/master/static/img/code.jpg)
```

### Comparing `DrissionRecorder-3.4.12/LICENSE` & `DrissionRecorder-3.4.13/LICENSE`

 * *Files identical despite different names*

### Comparing `DrissionRecorder-3.4.12/PKG-INFO` & `DrissionRecorder-3.4.13/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 Metadata-Version: 2.1
 Name: DrissionRecorder
-Version: 3.4.12
+Version: 3.4.13
 Summary: 用于记录数据的模块。
-Home-page: https://gitee.com/g1879/DataRecorder
+Home-page: https://gitee.com/g1879/DrissionRecorder
 Author: g1879
 Author-email: g1879@qq.com
 License: MIT
 Keywords: DrissionRecorder
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: BSD License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ⭐️ 简介
 
-本库是一个基于 python 的工具集，用于记录数据到文件（含 sqlite）。
+本库是一个基于 python 的工具集，用于记录数据到文件。
 
-使用方便，代码简洁， 是一个可靠、省心且实用的工具。
+使用方便，代码简洁，是一个可靠、省心且实用的工具。
 
-还支持多线程同时写入文件。
+支持多线程同时写入文件。
 
 **交流QQ群：** 897838127
 
 **联系邮箱：** g1879@qq.com
 
-**使用手册：** 📒[点击打开](http://g1879.gitee.io/datarecorderdocs/)
+**使用手册：** 📒[点击打开](http://g1879.gitee.io/DrissionRecorderDocs/)
 
 # ✨️ 理念
 
 简单，可靠，省心。
 
 # 📕 背景
 
@@ -62,67 +62,63 @@
 ## ⚡ 记录器`Recorder`
 
 `Recorder`的功能简单直观高效实用，只做一个动作，就是不断接收数据，按顺序往文件里添加。可以接收单行数据，或二维数据一次写入多行。
 
 它支持 csv、xlsx、json、txt 四种格式文件。
 
 ```python
-from DataRecorder import Recorder
+from DrissionRecorder import Recorder
 
 data = ((1, 2, 3, 4), 
         (5, 6, 7, 8))
 
 r = Recorder('data.csv')
 r.add_data(data)  # 一次记录多行数据
 r.add_data('abc')  # 记录单行数据
 ```
 
 ## ⚡ 表格填充器`Filler`
 
-`Filler`用于对表格文件填写数据，可以指定填其坐标。它的使用非常灵活，可以指定坐标为左上角，填入一片二维数据。还封装了记录数据处理进度的功能（比如断点续爬）。除此以外，它还能给单元格设置链接。
+`Filler`用于对表格文件填写数据，可以指定填其坐标。它的使用非常灵活，可以指定坐标为左上角，填入一片二维数据。还封装了记录数据处理进度的功能（比如断点续爬）。
+
+除此以外，它还能给单元格设置链接和样式。
 
 它只支持 csv 和 xlsx 格式文件。
 
 ```python
-from DataRecorder import Filler
+from DrissionRecorder import Filler
 
 f = Filler('results.csv')
 f.add_data((1, 2, 3, 4), 'a2')  # 从A2单元格开始，写入一行数据
 f.add_data(((1, 2), (3, 4)), 'd4')  # 以D4单元格为左上角，写入一片二维数据
 ```
 
 ## ⚡ 二进制数据记录器`ByteRecorder`
 
 `ByteRecorder`用法最简单，它和`Recorder`类似，记录多个数据然后按顺序写入文件。不一样的是它只接收二进制数据，每次`add_data()`只能输入一条数据，而且没有行的概念。
 
-可以用来和作者的另一个工具 [FlowViewer](https://gitee.com/g1879/FlowViewer) 配合使用，用来获取浏览器加载的文件，或用来记录下载的文件。可指定每个数据写入文件中的位置，以支持多线程下载文件。
-
 支持任意文件格式。
 
 ```python
-from DataRecorder import ByteRecorder
+from DrissionRecorder import ByteRecorder
 
 b = ByteRecorder('data.file')
-b.add_data(b'xxxxxxxxxxx')  # 向文件写入二进制数据
+b.add_data(b'*****************')  # 向文件写入二进制数据
 ```
 
 ## ⚡ 数据库记录器`DBRecorder`
 
 支持 sqlite，用法和`Recorder`一致，支持自动创建数据库、数据表、数据列。
 
 ```python
-from DataRecorder import DBRecorder
+from DrissionRecorder import DBRecorder
 
 d = DBRecorder('data.db')
 d.add_data({'name': '张三', 'age': 25}, table='user')  # 插入数据到user表
 d.record()
 ```
 
-# 🛠 使用方法
-
-[📒点击跳转到使用手册](http://g1879.gitee.io/datarecorderdocs/)
-
 # ☕ 请我喝咖啡
 
 如果本项目对您有所帮助，不妨请作者我喝杯咖啡 ：）
 
-![](https://gitee.com/g1879/DrissionPage-demos/raw/master/pics/code.jpg)
+![](https://gitee.com/g1879/DrissionPageDocs/raw/master/static/img/code.jpg)
```

### Comparing `DrissionRecorder-3.4.12/README.md` & `DrissionRecorder-3.4.13/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # ⭐️ 简介
 
-本库是一个基于 python 的工具集，用于记录数据到文件（含 sqlite）。
+本库是一个基于 python 的工具集，用于记录数据到文件。
 
-使用方便，代码简洁， 是一个可靠、省心且实用的工具。
+使用方便，代码简洁，是一个可靠、省心且实用的工具。
 
-还支持多线程同时写入文件。
+支持多线程同时写入文件。
 
 **交流QQ群：** 897838127
 
 **联系邮箱：** g1879@qq.com
 
-**使用手册：** 📒[点击打开](http://g1879.gitee.io/datarecorderdocs/)
+**使用手册：** 📒[点击打开](http://g1879.gitee.io/DrissionRecorderDocs/)
 
 # ✨️ 理念
 
 简单，可靠，省心。
 
 # 📕 背景
 
@@ -45,67 +45,63 @@
 ## ⚡ 记录器`Recorder`
 
 `Recorder`的功能简单直观高效实用，只做一个动作，就是不断接收数据，按顺序往文件里添加。可以接收单行数据，或二维数据一次写入多行。
 
 它支持 csv、xlsx、json、txt 四种格式文件。
 
 ```python
-from DataRecorder import Recorder
+from DrissionRecorder import Recorder
 
 data = ((1, 2, 3, 4), 
         (5, 6, 7, 8))
 
 r = Recorder('data.csv')
 r.add_data(data)  # 一次记录多行数据
 r.add_data('abc')  # 记录单行数据
 ```
 
 ## ⚡ 表格填充器`Filler`
 
-`Filler`用于对表格文件填写数据，可以指定填其坐标。它的使用非常灵活，可以指定坐标为左上角，填入一片二维数据。还封装了记录数据处理进度的功能（比如断点续爬）。除此以外，它还能给单元格设置链接。
+`Filler`用于对表格文件填写数据，可以指定填其坐标。它的使用非常灵活，可以指定坐标为左上角，填入一片二维数据。还封装了记录数据处理进度的功能（比如断点续爬）。
+
+除此以外，它还能给单元格设置链接和样式。
 
 它只支持 csv 和 xlsx 格式文件。
 
 ```python
-from DataRecorder import Filler
+from DrissionRecorder import Filler
 
 f = Filler('results.csv')
 f.add_data((1, 2, 3, 4), 'a2')  # 从A2单元格开始，写入一行数据
 f.add_data(((1, 2), (3, 4)), 'd4')  # 以D4单元格为左上角，写入一片二维数据
 ```
 
 ## ⚡ 二进制数据记录器`ByteRecorder`
 
 `ByteRecorder`用法最简单，它和`Recorder`类似，记录多个数据然后按顺序写入文件。不一样的是它只接收二进制数据，每次`add_data()`只能输入一条数据，而且没有行的概念。
 
-可以用来和作者的另一个工具 [FlowViewer](https://gitee.com/g1879/FlowViewer) 配合使用，用来获取浏览器加载的文件，或用来记录下载的文件。可指定每个数据写入文件中的位置，以支持多线程下载文件。
-
 支持任意文件格式。
 
 ```python
-from DataRecorder import ByteRecorder
+from DrissionRecorder import ByteRecorder
 
 b = ByteRecorder('data.file')
-b.add_data(b'xxxxxxxxxxx')  # 向文件写入二进制数据
+b.add_data(b'*****************')  # 向文件写入二进制数据
 ```
 
 ## ⚡ 数据库记录器`DBRecorder`
 
 支持 sqlite，用法和`Recorder`一致，支持自动创建数据库、数据表、数据列。
 
 ```python
-from DataRecorder import DBRecorder
+from DrissionRecorder import DBRecorder
 
 d = DBRecorder('data.db')
 d.add_data({'name': '张三', 'age': 25}, table='user')  # 插入数据到user表
 d.record()
 ```
 
-# 🛠 使用方法
-
-[📒点击跳转到使用手册](http://g1879.gitee.io/datarecorderdocs/)
-
 # ☕ 请我喝咖啡
 
 如果本项目对您有所帮助，不妨请作者我喝杯咖啡 ：）
 
-![](https://gitee.com/g1879/DrissionPage-demos/raw/master/pics/code.jpg)
+![](https://gitee.com/g1879/DrissionPageDocs/raw/master/static/img/code.jpg)
```

### Comparing `DrissionRecorder-3.4.12/setup.py` & `DrissionRecorder-3.4.13/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # -*- coding:utf-8 -*-
 from setuptools import setup, find_packages
-from DataRecorder import __version__
+from DrissionRecorder import __version__
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name="DrissionRecorder",
     version=__version__,
     author="g1879",
     author_email="g1879@qq.com",
     description="用于记录数据的模块。",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT",
     keywords="DrissionRecorder",
-    url="https://gitee.com/g1879/DataRecorder",
+    url="https://gitee.com/g1879/DrissionRecorder",
     include_package_data=True,
     packages=find_packages(),
     install_requires=[
         "openpyxl"
     ],
     classifiers=[
         "Programming Language :: Python :: 3.6",
```

