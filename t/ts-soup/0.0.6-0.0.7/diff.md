# Comparing `tmp/ts-soup-0.0.6.tar.gz` & `tmp/ts-soup-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\PythonProjects\load_predict\syncdbs_new\dist\.tmp-ti3kbx8q\ts-soup-0.0.6.tar", last modified: Fri Apr  5 21:50:44 2024, max compression
+gzip compressed data, was "D:\PythonProjects\load_predict\syncdbs_new\dist\.tmp-3az4yhp3\ts-soup-0.0.7.tar", last modified: Sat Apr  6 00:03:57 2024, max compression
```

## Comparing `ts-soup-0.0.6.tar` & `ts-soup-0.0.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-05 21:50:44.069219 ts-soup-0.0.6/
--rw-rw-rw-   0        0        0     1028 2024-04-05 21:50:44.068221 ts-soup-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0      686 2024-04-05 12:25:36.000000 ts-soup-0.0.6/README.md
--rw-rw-rw-   0        0        0       42 2024-04-05 21:50:44.069219 ts-soup-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      605 2024-04-05 21:50:07.000000 ts-soup-0.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-05 21:50:44.060219 ts-soup-0.0.6/ts_soup/
--rw-rw-rw-   0        0        0      307 2024-04-05 10:42:41.000000 ts-soup-0.0.6/ts_soup/__init__.py
--rw-rw-rw-   0        0        0     1418 2024-04-05 21:49:15.000000 ts-soup-0.0.6/ts_soup/app.py
--rw-rw-rw-   0        0        0    18128 2024-04-05 21:49:15.000000 ts-soup-0.0.6/ts_soup/common.py
-drwxrwxrwx   0        0        0        0 2024-04-05 21:50:44.066219 ts-soup-0.0.6/ts_soup/workers/
--rw-rw-rw-   0        0        0       78 2024-04-05 04:01:53.000000 ts-soup-0.0.6/ts_soup/workers/__init__.py
--rw-rw-rw-   0        0        0     3689 2024-04-05 09:36:43.000000 ts-soup-0.0.6/ts_soup/workers/sources.py
--rw-rw-rw-   0        0        0     5793 2024-04-05 11:44:31.000000 ts-soup-0.0.6/ts_soup/workers/targets.py
-drwxrwxrwx   0        0        0        0 2024-04-05 21:50:44.067219 ts-soup-0.0.6/ts_soup.egg-info/
--rw-rw-rw-   0        0        0     1028 2024-04-05 21:50:44.000000 ts-soup-0.0.6/ts_soup.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      277 2024-04-05 21:50:44.000000 ts-soup-0.0.6/ts_soup.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 21:50:44.000000 ts-soup-0.0.6/ts_soup.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-04-05 21:50:44.000000 ts-soup-0.0.6/ts_soup.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-06 00:03:57.285826 ts-soup-0.0.7/
+-rw-rw-rw-   0        0        0     1028 2024-04-06 00:03:57.284814 ts-soup-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0      686 2024-04-05 12:25:36.000000 ts-soup-0.0.7/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-06 00:03:57.285826 ts-soup-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      605 2024-04-06 00:03:51.000000 ts-soup-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-06 00:03:57.276080 ts-soup-0.0.7/ts_soup/
+-rw-rw-rw-   0        0        0      307 2024-04-05 10:42:41.000000 ts-soup-0.0.7/ts_soup/__init__.py
+-rw-rw-rw-   0        0        0     1418 2024-04-05 21:49:15.000000 ts-soup-0.0.7/ts_soup/app.py
+-rw-rw-rw-   0        0        0    18279 2024-04-05 23:44:56.000000 ts-soup-0.0.7/ts_soup/common.py
+drwxrwxrwx   0        0        0        0 2024-04-06 00:03:57.282486 ts-soup-0.0.7/ts_soup/workers/
+-rw-rw-rw-   0        0        0       78 2024-04-05 04:01:53.000000 ts-soup-0.0.7/ts_soup/workers/__init__.py
+-rw-rw-rw-   0        0        0     3689 2024-04-05 09:36:43.000000 ts-soup-0.0.7/ts_soup/workers/sources.py
+-rw-rw-rw-   0        0        0     5793 2024-04-05 11:44:31.000000 ts-soup-0.0.7/ts_soup/workers/targets.py
+drwxrwxrwx   0        0        0        0 2024-04-06 00:03:57.283486 ts-soup-0.0.7/ts_soup.egg-info/
+-rw-rw-rw-   0        0        0     1028 2024-04-06 00:03:57.000000 ts-soup-0.0.7/ts_soup.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      277 2024-04-06 00:03:57.000000 ts-soup-0.0.7/ts_soup.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-06 00:03:57.000000 ts-soup-0.0.7/ts_soup.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-04-06 00:03:57.000000 ts-soup-0.0.7/ts_soup.egg-info/top_level.txt
```

### Comparing `ts-soup-0.0.6/PKG-INFO` & `ts-soup-0.0.7/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ts-soup
-Version: 0.0.6
+Version: 0.0.7
 Summary: date series data synchronization
 Author: feihan ye
 Author-email: 445280206@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `ts-soup-0.0.6/README.md` & `ts-soup-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `ts-soup-0.0.6/setup.py` & `ts-soup-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r",encoding='utf8') as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="ts-soup",
-  version="0.0.6",
+  version="0.0.7",
   author="feihan ye",
   author_email="445280206@qq.com",
   description="date series data synchronization",
   long_description=long_description,
   long_description_content_type="text/markdown",
   # url="https://github.com/pypa/sampleproject",
   packages=setuptools.find_packages(),
```

### Comparing `ts-soup-0.0.6/ts_soup/app.py` & `ts-soup-0.0.7/ts_soup/app.py`

 * *Files identical despite different names*

### Comparing `ts-soup-0.0.6/ts_soup/common.py` & `ts-soup-0.0.7/ts_soup/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -223,19 +223,22 @@
             data = source.build_source(self.to_update_date)
             """
             判断数据源（empty_check设置为True的）是否存在空，如果存在空则视所有数据源都为空，当天数据未更新
             主要目的是为了避免需要频繁在funcs的处理逻辑中增加判空的判断，也可以手动给某数据源设置为False,如果某数据源
             empty_check设置为False，需要在数据处理逻辑中对data_source是否为空进行判断，不然当下文在进行数据处理时
             使用行列索引，如果df是空容易导致keyError错误。
             """
-            if data.empty and source.empty_check:
-                self.any_source_empty = True
-                for _ in self.targets:
-                    self.value.append(None)
-                return
+            if hasattr(source,'empty_check'):
+                if source.empty_check and data.empty:
+                    self.any_source_empty = True
+                    for _ in self.targets:
+                        self.value.append(None)
+                    return
+            else:
+                raise ValueError("source.empty_check未设置")
 
             self.source_data.append(data)
 
     def handle_result(self):
         """
         处理结果的方法
         1.有分表的处理：
```

### Comparing `ts-soup-0.0.6/ts_soup/workers/sources.py` & `ts-soup-0.0.7/ts_soup/workers/sources.py`

 * *Files identical despite different names*

### Comparing `ts-soup-0.0.6/ts_soup/workers/targets.py` & `ts-soup-0.0.7/ts_soup/workers/targets.py`

 * *Files identical despite different names*

### Comparing `ts-soup-0.0.6/ts_soup.egg-info/PKG-INFO` & `ts-soup-0.0.7/ts_soup.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ts-soup
-Version: 0.0.6
+Version: 0.0.7
 Summary: date series data synchronization
 Author: feihan ye
 Author-email: 445280206@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

