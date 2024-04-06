# Comparing `tmp/DataRecorder-3.4.8.tar.gz` & `tmp/DataRecorder-3.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DataRecorder-3.4.8.tar", last modified: Wed Sep 13 15:35:30 2023, max compression
+gzip compressed data, was "DataRecorder-3.4.9.tar", last modified: Wed Oct 11 08:00:31 2023, max compression
```

## Comparing `DataRecorder-3.4.8.tar` & `DataRecorder-3.4.9.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-09-13 15:35:30.417604 DataRecorder-3.4.8/
-drwxrwxrwx   0        0        0        0 2023-09-13 15:35:30.410717 DataRecorder-3.4.8/DataRecorder/
--rw-rw-rw-   0        0        0      138 2023-08-04 02:16:31.000000 DataRecorder-3.4.8/DataRecorder/__init__.py
--rw-rw-rw-   0        0        0     6145 2023-09-05 12:26:12.000000 DataRecorder-3.4.8/DataRecorder/base.py
--rw-rw-rw-   0        0        0     1862 2023-09-05 12:26:12.000000 DataRecorder-3.4.8/DataRecorder/base.pyi
--rw-rw-rw-   0        0        0     1753 2023-08-16 02:32:24.000000 DataRecorder-3.4.8/DataRecorder/byte_recorder.py
--rw-rw-rw-   0        0        0      532 2023-08-17 00:59:45.000000 DataRecorder-3.4.8/DataRecorder/byte_recorder.pyi
--rw-rw-rw-   0        0        0     6238 2023-09-05 12:26:12.000000 DataRecorder-3.4.8/DataRecorder/db_recorder.py
--rw-rw-rw-   0        0        0     1019 2023-08-17 00:59:45.000000 DataRecorder-3.4.8/DataRecorder/db_recorder.pyi
--rw-rw-rw-   0        0        0    22007 2023-09-13 15:19:04.000000 DataRecorder-3.4.8/DataRecorder/filler.py
--rw-rw-rw-   0        0        0     2876 2023-09-13 15:33:00.000000 DataRecorder-3.4.8/DataRecorder/filler.pyi
--rw-rw-rw-   0        0        0     9397 2023-09-05 12:26:12.000000 DataRecorder-3.4.8/DataRecorder/recorder.py
--rw-rw-rw-   0        0        0      988 2023-08-31 06:16:47.000000 DataRecorder-3.4.8/DataRecorder/recorder.pyi
--rw-rw-rw-   0        0        0    13648 2023-09-13 15:34:59.000000 DataRecorder-3.4.8/DataRecorder/setter.py
--rw-rw-rw-   0        0        0     3196 2023-09-13 15:19:04.000000 DataRecorder-3.4.8/DataRecorder/setter.pyI
-drwxrwxrwx   0        0        0        0 2023-09-13 15:35:30.415100 DataRecorder-3.4.8/DataRecorder/style/
--rw-rw-rw-   0        0        0       77 2023-08-04 03:31:42.000000 DataRecorder-3.4.8/DataRecorder/style/__init__.py
--rw-rw-rw-   0        0        0    28558 2023-08-04 03:31:42.000000 DataRecorder-3.4.8/DataRecorder/style/cell_style.py
--rw-rw-rw-   0        0        0     9200 2023-09-05 12:26:12.000000 DataRecorder-3.4.8/DataRecorder/tools.py
--rw-rw-rw-   0        0        0      915 2023-08-04 03:31:42.000000 DataRecorder-3.4.8/DataRecorder/tools.pyi
-drwxrwxrwx   0        0        0        0 2023-09-13 15:35:30.415100 DataRecorder-3.4.8/DataRecorder.egg-info/
--rw-rw-rw-   0        0        0     4838 2023-09-13 15:35:30.000000 DataRecorder-3.4.8/DataRecorder.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      657 2023-09-13 15:35:30.000000 DataRecorder-3.4.8/DataRecorder.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-09-13 15:35:30.000000 DataRecorder-3.4.8/DataRecorder.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-09-13 15:35:30.000000 DataRecorder-3.4.8/DataRecorder.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-09-13 15:35:30.000000 DataRecorder-3.4.8/DataRecorder.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1083 2022-01-26 11:22:47.000000 DataRecorder-3.4.8/LICENSE
--rw-rw-rw-   0        0        0       26 2023-03-26 03:46:04.000000 DataRecorder-3.4.8/MANIFEST.in
--rw-rw-rw-   0        0        0     4838 2023-09-13 15:35:30.417604 DataRecorder-3.4.8/PKG-INFO
--rw-rw-rw-   0        0        0     4339 2023-09-04 13:49:44.000000 DataRecorder-3.4.8/README.md
--rw-rw-rw-   0        0        0       42 2023-09-13 15:35:30.417604 DataRecorder-3.4.8/setup.cfg
--rw-rw-rw-   0        0        0      863 2023-09-13 15:19:04.000000 DataRecorder-3.4.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-10-11 08:00:31.701275 DataRecorder-3.4.9/
+drwxrwxrwx   0        0        0        0 2023-10-11 08:00:31.625717 DataRecorder-3.4.9/DataRecorder/
+-rw-rw-rw-   0        0        0      138 2023-08-04 02:16:32.000000 DataRecorder-3.4.9/DataRecorder/__init__.py
+-rw-rw-rw-   0        0        0     6145 2023-09-04 13:51:02.000000 DataRecorder-3.4.9/DataRecorder/base.py
+-rw-rw-rw-   0        0        0     1862 2023-09-04 06:32:26.000000 DataRecorder-3.4.9/DataRecorder/base.pyi
+-rw-rw-rw-   0        0        0     1753 2023-08-16 02:32:26.000000 DataRecorder-3.4.9/DataRecorder/byte_recorder.py
+-rw-rw-rw-   0        0        0      532 2023-08-17 00:59:46.000000 DataRecorder-3.4.9/DataRecorder/byte_recorder.pyi
+-rw-rw-rw-   0        0        0     6238 2023-09-05 06:16:52.000000 DataRecorder-3.4.9/DataRecorder/db_recorder.py
+-rw-rw-rw-   0        0        0     1019 2023-08-17 00:59:46.000000 DataRecorder-3.4.9/DataRecorder/db_recorder.pyi
+-rw-rw-rw-   0        0        0    22054 2023-10-11 07:48:38.000000 DataRecorder-3.4.9/DataRecorder/filler.py
+-rw-rw-rw-   0        0        0     2876 2023-10-11 07:38:37.000000 DataRecorder-3.4.9/DataRecorder/filler.pyi
+-rw-rw-rw-   0        0        0     9397 2023-09-05 07:25:47.000000 DataRecorder-3.4.9/DataRecorder/recorder.py
+-rw-rw-rw-   0        0        0      988 2023-08-31 06:16:48.000000 DataRecorder-3.4.9/DataRecorder/recorder.pyi
+-rw-rw-rw-   0        0        0    13648 2023-10-11 07:38:37.000000 DataRecorder-3.4.9/DataRecorder/setter.py
+-rw-rw-rw-   0        0        0     3196 2023-10-11 07:38:37.000000 DataRecorder-3.4.9/DataRecorder/setter.pyI
+drwxrwxrwx   0        0        0        0 2023-10-11 08:00:31.682174 DataRecorder-3.4.9/DataRecorder/style/
+-rw-rw-rw-   0        0        0       77 2023-08-04 03:31:44.000000 DataRecorder-3.4.9/DataRecorder/style/__init__.py
+-rw-rw-rw-   0        0        0    28558 2023-08-04 03:31:44.000000 DataRecorder-3.4.9/DataRecorder/style/cell_style.py
+-rw-rw-rw-   0        0        0     9200 2023-09-04 06:32:26.000000 DataRecorder-3.4.9/DataRecorder/tools.py
+-rw-rw-rw-   0        0        0      915 2023-08-04 03:31:44.000000 DataRecorder-3.4.9/DataRecorder/tools.pyi
+drwxrwxrwx   0        0        0        0 2023-10-11 08:00:31.675123 DataRecorder-3.4.9/DataRecorder.egg-info/
+-rw-rw-rw-   0        0        0     4838 2023-10-11 08:00:30.000000 DataRecorder-3.4.9/DataRecorder.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      657 2023-10-11 08:00:30.000000 DataRecorder-3.4.9/DataRecorder.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-10-11 08:00:30.000000 DataRecorder-3.4.9/DataRecorder.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-10-11 08:00:30.000000 DataRecorder-3.4.9/DataRecorder.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-10-11 08:00:30.000000 DataRecorder-3.4.9/DataRecorder.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1083 2021-08-17 07:03:54.000000 DataRecorder-3.4.9/LICENSE
+-rw-rw-rw-   0        0        0       26 2023-04-28 02:15:42.000000 DataRecorder-3.4.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     4838 2023-10-11 08:00:31.699289 DataRecorder-3.4.9/PKG-INFO
+-rw-rw-rw-   0        0        0     4339 2023-09-04 09:33:58.000000 DataRecorder-3.4.9/README.md
+-rw-rw-rw-   0        0        0       42 2023-10-11 08:00:31.701275 DataRecorder-3.4.9/setup.cfg
+-rw-rw-rw-   0        0        0      863 2023-10-11 07:59:16.000000 DataRecorder-3.4.9/setup.py
```

### Comparing `DataRecorder-3.4.8/DataRecorder/base.py` & `DataRecorder-3.4.9/DataRecorder/base.py`

 * *Files identical despite different names*

### Comparing `DataRecorder-3.4.8/DataRecorder/base.pyi` & `DataRecorder-3.4.9/DataRecorder/base.pyi`

 * *Files identical despite different names*

### Comparing `DataRecorder-3.4.8/DataRecorder/byte_recorder.py` & `DataRecorder-3.4.9/DataRecorder/byte_recorder.py`

 * *Files identical despite different names*

### Comparing `DataRecorder-3.4.8/DataRecorder/byte_recorder.pyi` & `DataRecorder-3.4.9/DataRecorder/byte_recorder.pyi`

 * *Files identical despite different names*

### Comparing `DataRecorder-3.4.8/DataRecorder/db_recorder.py` & `DataRecorder-3.4.9/DataRecorder/db_recorder.py`

 * *Files identical despite different names*

### Comparing `DataRecorder-3.4.8/DataRecorder/db_recorder.pyi` & `DataRecorder-3.4.9/DataRecorder/db_recorder.pyi`

 * *Files identical despite different names*

### Comparing `DataRecorder-3.4.8/DataRecorder/filler.py` & `DataRecorder-3.4.9/DataRecorder/filler.py`

 * *Files 1% similar despite different names*

```diff
@@ -399,36 +399,38 @@
 
     if ws.max_column is None:  # 遇到过read_only时无法获取列数的文件
         wb.close()
         wb = load_workbook(filler.path, data_only=True)
         ws = wb[filler.table] if filler.table else wb.active
 
     rows = ws.rows
+    loop = 0
     if as_dict:
         title = [filler.row_num_title]
         if filler.begin_row == 1:
             t = [get_column_letter(x) for x in range(1, ws.max_column + 1)
                  if filler.key_cols is True or x in filler.key_cols]
         else:
             try:
                 t = next(rows)
                 t = [x.value if x.value else get_column_letter(k) for k, x in enumerate(t, 1)
                      if filler.key_cols is True or k in filler.key_cols]
+                loop = 1
 
             except StopIteration:
                 return []
 
         if len(t) != len(set(t)):
             raise RuntimeError('表头出现内容重复。')
         if filler.row_num_title in t:
             raise RuntimeError(f'表头"{filler.row_num_title}"列与行号列重复，请用set.row_num_title()方法设置不同的表头。')
         title.extend(t)
 
     try:
-        for _ in range(filler.begin_row - 1):
+        for _ in range(filler.begin_row - loop - 1):
             next(rows)
     except StopIteration:
         return []
 
     # ---------------------------------------------------------
 
     if filler.sign_col is True or filler.sign_col > ws.max_column:  # 获取所有行
```

### Comparing `DataRecorder-3.4.8/DataRecorder/filler.pyi` & `DataRecorder-3.4.9/DataRecorder/filler.pyi`

 * *Files identical despite different names*

### Comparing `DataRecorder-3.4.8/DataRecorder/recorder.py` & `DataRecorder-3.4.9/DataRecorder/recorder.py`

 * *Files identical despite different names*

### Comparing `DataRecorder-3.4.8/DataRecorder/recorder.pyi` & `DataRecorder-3.4.9/DataRecorder/recorder.pyi`

 * *Files identical despite different names*

### Comparing `DataRecorder-3.4.8/DataRecorder/setter.py` & `DataRecorder-3.4.9/DataRecorder/setter.py`

 * *Files identical despite different names*

### Comparing `DataRecorder-3.4.8/DataRecorder/setter.pyI` & `DataRecorder-3.4.9/DataRecorder/setter.pyI`

 * *Files identical despite different names*

### Comparing `DataRecorder-3.4.8/DataRecorder/style/cell_style.py` & `DataRecorder-3.4.9/DataRecorder/style/cell_style.py`

 * *Files identical despite different names*

### Comparing `DataRecorder-3.4.8/DataRecorder/tools.py` & `DataRecorder-3.4.9/DataRecorder/tools.py`

 * *Files identical despite different names*

### Comparing `DataRecorder-3.4.8/DataRecorder/tools.pyi` & `DataRecorder-3.4.9/DataRecorder/tools.pyi`

 * *Files identical despite different names*

### Comparing `DataRecorder-3.4.8/DataRecorder.egg-info/PKG-INFO` & `DataRecorder-3.4.9/DataRecorder.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DataRecorder
-Version: 3.4.8
+Version: 3.4.9
 Summary: 用于记录数据的模块。
 Home-page: https://gitee.com/g1879/DataRecorder
 Author: g1879
 Author-email: g1879@qq.com
 License: MIT
 Keywords: DataRecorder
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `DataRecorder-3.4.8/DataRecorder.egg-info/SOURCES.txt` & `DataRecorder-3.4.9/DataRecorder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `DataRecorder-3.4.8/LICENSE` & `DataRecorder-3.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `DataRecorder-3.4.8/PKG-INFO` & `DataRecorder-3.4.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DataRecorder
-Version: 3.4.8
+Version: 3.4.9
 Summary: 用于记录数据的模块。
 Home-page: https://gitee.com/g1879/DataRecorder
 Author: g1879
 Author-email: g1879@qq.com
 License: MIT
 Keywords: DataRecorder
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `DataRecorder-3.4.8/README.md` & `DataRecorder-3.4.9/README.md`

 * *Files identical despite different names*

### Comparing `DataRecorder-3.4.8/setup.py` & `DataRecorder-3.4.9/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name="DataRecorder",
-    version="3.4.8",
+    version="3.4.9",
     author="g1879",
     author_email="g1879@qq.com",
     description="用于记录数据的模块。",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT",
     keywords="DataRecorder",
```

