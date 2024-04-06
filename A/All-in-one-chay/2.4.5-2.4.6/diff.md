# Comparing `tmp/All-in-one-chay-2.4.5.tar.gz` & `tmp/All-in-one-chay-2.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "All-in-one-chay-2.4.5.tar", last modified: Mon Apr  1 14:34:38 2024, max compression
+gzip compressed data, was "All-in-one-chay-2.4.6.tar", last modified: Sat Apr  6 13:39:08 2024, max compression
```

## Comparing `All-in-one-chay-2.4.5.tar` & `All-in-one-chay-2.4.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-04-01 14:34:38.652609 All-in-one-chay-2.4.5/
--rw-rw-rw-   0        0        0     1091 2024-03-09 13:46:48.000000 All-in-one-chay-2.4.5/LICENSE
--rw-rw-rw-   0        0        0     1859 2024-04-01 14:34:38.650609 All-in-one-chay-2.4.5/PKG-INFO
--rw-rw-rw-   0        0        0     1220 2024-03-29 15:06:20.000000 All-in-one-chay-2.4.5/README.md
--rw-rw-rw-   0        0        0      622 2024-04-01 14:23:41.000000 All-in-one-chay-2.4.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-01 14:34:38.652609 All-in-one-chay-2.4.5/setup.cfg
--rw-rw-rw-   0        0        0      975 2024-04-01 14:23:43.000000 All-in-one-chay-2.4.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-01 14:34:38.627608 All-in-one-chay-2.4.5/src/
-drwxrwxrwx   0        0        0        0 2024-04-01 14:34:38.634608 All-in-one-chay-2.4.5/src/All-in-one_chayLichenyi/
--rw-rw-rw-   0        0        0     8943 2024-04-01 14:23:02.000000 All-in-one-chay-2.4.5/src/All-in-one_chayLichenyi/Allinone.py
--rw-rw-rw-   0        0        0        0 2024-02-23 09:19:09.000000 All-in-one-chay-2.4.5/src/All-in-one_chayLichenyi/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-01 14:34:38.643609 All-in-one-chay-2.4.5/src/All-in-one_chayLichenyi/module/
--rw-rw-rw-   0        0        0     9185 2024-02-09 06:24:29.000000 All-in-one-chay-2.4.5/src/All-in-one_chayLichenyi/module/book.py
--rw-rw-rw-   0        0        0     9096 2024-04-01 14:22:46.000000 All-in-one-chay-2.4.5/src/All-in-one_chayLichenyi/module/calculator.py
--rw-rw-rw-   0        0        0     1244 2024-02-09 06:24:29.000000 All-in-one-chay-2.4.5/src/All-in-one_chayLichenyi/module/erfenchazhao_py.py
--rw-rw-rw-   0        0        0     1695 2024-02-09 06:24:29.000000 All-in-one-chay-2.4.5/src/All-in-one_chayLichenyi/module/math_cal_py.py
--rw-rw-rw-   0        0        0     1381 2024-02-09 06:24:29.000000 All-in-one-chay-2.4.5/src/All-in-one_chayLichenyi/module/student_py.py
--rw-rw-rw-   0        0        0     6957 2024-02-09 06:24:29.000000 All-in-one-chay-2.4.5/src/All-in-one_chayLichenyi/module/tuxing_cal.py
--rw-rw-rw-   0        0        0     2804 2024-04-01 14:20:26.000000 All-in-one-chay-2.4.5/src/All-in-one_chayLichenyi/module/xiaogongju.py
-drwxrwxrwx   0        0        0        0 2024-04-01 14:34:38.649609 All-in-one-chay-2.4.5/src/All_in_one_chay.egg-info/
--rw-rw-rw-   0        0        0     1859 2024-04-01 14:34:38.000000 All-in-one-chay-2.4.5/src/All_in_one_chay.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      636 2024-04-01 14:34:38.000000 All-in-one-chay-2.4.5/src/All_in_one_chay.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-01 14:34:38.000000 All-in-one-chay-2.4.5/src/All_in_one_chay.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2024-04-01 14:34:38.000000 All-in-one-chay-2.4.5/src/All_in_one_chay.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-06 13:39:08.255291 All-in-one-chay-2.4.6/
+-rw-rw-rw-   0        0        0     1091 2024-03-09 13:46:48.000000 All-in-one-chay-2.4.6/LICENSE
+-rw-rw-rw-   0        0        0     1857 2024-04-06 13:39:08.254290 All-in-one-chay-2.4.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1220 2024-03-29 15:06:20.000000 All-in-one-chay-2.4.6/README.md
+-rw-rw-rw-   0        0        0      622 2024-04-06 13:37:57.000000 All-in-one-chay-2.4.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-06 13:39:08.255291 All-in-one-chay-2.4.6/setup.cfg
+-rw-rw-rw-   0        0        0      973 2024-04-06 13:38:46.000000 All-in-one-chay-2.4.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-06 13:39:08.233292 All-in-one-chay-2.4.6/src/
+drwxrwxrwx   0        0        0        0 2024-04-06 13:39:08.239291 All-in-one-chay-2.4.6/src/All-in-one_chayLichenyi/
+-rw-rw-rw-   0        0        0     9380 2024-04-06 13:37:26.000000 All-in-one-chay-2.4.6/src/All-in-one_chayLichenyi/Allinone.py
+-rw-rw-rw-   0        0        0        0 2024-02-23 09:19:09.000000 All-in-one-chay-2.4.6/src/All-in-one_chayLichenyi/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-06 13:39:08.247291 All-in-one-chay-2.4.6/src/All-in-one_chayLichenyi/module/
+-rw-rw-rw-   0        0        0     9185 2024-02-09 06:24:29.000000 All-in-one-chay-2.4.6/src/All-in-one_chayLichenyi/module/book.py
+-rw-rw-rw-   0        0        0    10521 2024-04-06 13:34:53.000000 All-in-one-chay-2.4.6/src/All-in-one_chayLichenyi/module/calculator.py
+-rw-rw-rw-   0        0        0      876 2024-04-05 15:36:03.000000 All-in-one-chay-2.4.6/src/All-in-one_chayLichenyi/module/erfenchazhao_py.py
+-rw-rw-rw-   0        0        0     1695 2024-02-09 06:24:29.000000 All-in-one-chay-2.4.6/src/All-in-one_chayLichenyi/module/math_cal_py.py
+-rw-rw-rw-   0        0        0     1381 2024-02-09 06:24:29.000000 All-in-one-chay-2.4.6/src/All-in-one_chayLichenyi/module/student_py.py
+-rw-rw-rw-   0        0        0     6957 2024-02-09 06:24:29.000000 All-in-one-chay-2.4.6/src/All-in-one_chayLichenyi/module/tuxing_cal.py
+-rw-rw-rw-   0        0        0     2804 2024-04-06 01:29:46.000000 All-in-one-chay-2.4.6/src/All-in-one_chayLichenyi/module/xiaogongju.py
+drwxrwxrwx   0        0        0        0 2024-04-06 13:39:08.253292 All-in-one-chay-2.4.6/src/All_in_one_chay.egg-info/
+-rw-rw-rw-   0        0        0     1857 2024-04-06 13:39:08.000000 All-in-one-chay-2.4.6/src/All_in_one_chay.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      636 2024-04-06 13:39:08.000000 All-in-one-chay-2.4.6/src/All_in_one_chay.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-06 13:39:08.000000 All-in-one-chay-2.4.6/src/All_in_one_chay.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2024-04-06 13:39:08.000000 All-in-one-chay-2.4.6/src/All_in_one_chay.egg-info/top_level.txt
```

### Comparing `All-in-one-chay-2.4.5/LICENSE` & `All-in-one-chay-2.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `All-in-one-chay-2.4.5/PKG-INFO` & `All-in-one-chay-2.4.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: All-in-one-chay
-Version: 2.4.5
+Version: 2.4.6
 Summary: 多功能一体机（All-in-one）
-Home-page: https://github.com/lichenyichay/All-in-one/releases/tag/v2.4.5
+Home-page: https://github.com/lichenyichay/All-in-one/releases/tag/v2.4.6
 Author: Chay
 Author-email: chay <lichenyi_2020@qq.com>
-Project-URL: Homepage, https://github.com/lichenyichay/All-in-one/releases/tag/v2.4.5
+Project-URL: Homepage, https://github.com/lichenyichay/All-in-one/releases/tag/v2.4.6
 Project-URL: Issues, https://github.com/lichenyichay/All-in-one/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.0.0
+Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # All-in-one
 多功能一体机
 说明如下：
 ```python
```

### Comparing `All-in-one-chay-2.4.5/README.md` & `All-in-one-chay-2.4.6/README.md`

 * *Files identical despite different names*

### Comparing `All-in-one-chay-2.4.5/pyproject.toml` & `All-in-one-chay-2.4.6/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "All-in-one-chay"
-version = "2.4.5"
+version = "2.4.6"
 authors = [
   { name="chay", email="lichenyi_2020@qq.com" },
 ]
 description = "多功能一体机（All-in-one）"
 readme = "README.md"
 requires-python = ">=3.5"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
-Homepage = "https://github.com/lichenyichay/All-in-one/releases/tag/v2.4.5"
+Homepage = "https://github.com/lichenyichay/All-in-one/releases/tag/v2.4.6"
 Issues = "https://github.com/lichenyichay/All-in-one/issues"
```

### Comparing `All-in-one-chay-2.4.5/setup.py` & `All-in-one-chay-2.4.6/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # coding:UTF-8
 import setuptools
 
 setuptools.setup(
     name="All-in-one-chay",
-    version="2.4.5",
+    version="2.4.6",
     author="Chay",
     author_email="lichenyi_2020@qq.com",
-    url="https://github.com/lichenyichay/All-in-one/releases/tag/v2.4.5",
+    url="https://github.com/lichenyichay/All-in-one/releases/tag/v2.4.6",
     description="All-in-one",
     long_description="多功能一体机",
-    python_requires=">=3.0.0",
+    python_requires=">=3.5",
     # packages=setuptools.find_packages("src"),
     packages_dir={"": "src"},
     packages_data={"": ["*.txt", "*.info", "*.properties"], "": ["data/*.*"]},
     exclude=["*.test", "*.test.*", "test.*", "test"],
     classifiers=['Environment :: Web Environment',
                  'Intended Audience :: Developers',
                  "License :: OSI Approved :: MIT License",
```

### Comparing `All-in-one-chay-2.4.5/src/All-in-one_chayLichenyi/Allinone.py` & `All-in-one-chay-2.4.6/src/All-in-one_chayLichenyi/Allinone.py`

 * *Files 3% similar despite different names*

```diff
@@ -62,14 +62,22 @@
         return calculator.istribonacci(args[0])
     elif fuwu=="判断泰波那契回文质数":
         return calculator.istribonaccihuiwenshuparam(args[0])
     elif fuwu=="判断泰波那契回文数":
         return calculator.istribonaccihuiwenshu(args[0])
     elif fuwu=="判断泰波那契质数":
         return calculator.istribonacciparam(args[0])
+    elif fuwu=="求第n个完全平方数":
+        return calculator.wanquanpingfangshu(args[0])
+    elif fuwu=="判断完全平方数":
+        return calculator.iswanquanpingfangshu(args[0])
+    elif fuwu=="判断斐波那契完全平方数":
+        return calculator.isfabwanquanpingfangshu(args[0])
+    elif fuwu=="判断泰波那契序列完全平方数":
+        return calculator.istribonacciwanquanpingfangshu(args[0])
     elif fuwu == "图形计算器":
         while True:
             huida = args[0]
             try:
                 args2=[]
                 for i in range(1,len(args)):
                     args2.append(args[i])
```

### Comparing `All-in-one-chay-2.4.5/src/All-in-one_chayLichenyi/module/book.py` & `All-in-one-chay-2.4.6/src/All-in-one_chayLichenyi/module/book.py`

 * *Files identical despite different names*

### Comparing `All-in-one-chay-2.4.5/src/All-in-one_chayLichenyi/module/calculator.py` & `All-in-one-chay-2.4.6/src/All-in-one_chayLichenyi/module/calculator.py`

 * *Files 9% similar despite different names*

```diff
@@ -312,8 +312,54 @@
 :return x 是否是泰波那契序列质数（True or False）
 作用：判断泰波那契序列质数
 '''
 def istribonacciparam(n:int):
     if istribonacci(n) and isparam(n):
         return True
     else:
-        return False
+        return False
+
+'''
+函数名：iswanquanpingfangshu
+调用形式：a = iswanquanpingfangshu(d)
+:param d  类型：int
+:return x d是否是完全平方数 类型：bool(True or False)
+作用：判断完全平方数
+'''   
+def iswanquanpingfangshu(num:int) -> bool:
+    a=math.sqrt(num)
+    if int(a)==a:
+        return True
+    else:
+        return False
+
+'''
+函数名：wanquanpingfangshu
+调用形式：a = wanquanpingfangshu(d)
+:param d  类型：int
+:return x 第d个完全平方数
+作用：求第d个完全平方数
+'''
+def wanquanpingfangshu(num:int) -> int:
+    return num**2
+
+'''
+函数名：isfabwanquanpingfangshu
+调用形式：a = isfabwanquanpingfangshu(d)
+:param d  类型：int
+:return x d是否是斐波那契完全平方数 类型：bool(True or False)
+作用：判断斐波那契完全平方数
+'''  
+def isfabwanquanpingfangshu(num:int) -> bool:
+    return isfab(num) and iswanquanpingfangshu(num)
+
+'''
+泰波那契序列 Tn 定义如下： 
+T0 = 0, T1 = 1, T2 = 1, 且在 n >= 0 的条件下 Tn+3 = Tn + Tn+1 + Tn+2
+函数名：istribonacciwanquanpingfangshu
+调用形式：a = istribonacciwanquanpingfangshu(d)
+:param x  类型：int
+:return x 是否是泰波那契序列完全平方数（True or False）
+作用：判断泰波那契序列完全平方数
+'''
+def istribonacciwanquanpingfangshu(num:int) -> bool:
+    return istribonacci(num) and iswanquanpingfangshu(num)
```

### Comparing `All-in-one-chay-2.4.5/src/All-in-one_chayLichenyi/module/math_cal_py.py` & `All-in-one-chay-2.4.6/src/All-in-one_chayLichenyi/module/math_cal_py.py`

 * *Files identical despite different names*

### Comparing `All-in-one-chay-2.4.5/src/All-in-one_chayLichenyi/module/student_py.py` & `All-in-one-chay-2.4.6/src/All-in-one_chayLichenyi/module/student_py.py`

 * *Files identical despite different names*

### Comparing `All-in-one-chay-2.4.5/src/All-in-one_chayLichenyi/module/tuxing_cal.py` & `All-in-one-chay-2.4.6/src/All-in-one_chayLichenyi/module/tuxing_cal.py`

 * *Files identical despite different names*

### Comparing `All-in-one-chay-2.4.5/src/All-in-one_chayLichenyi/module/xiaogongju.py` & `All-in-one-chay-2.4.6/src/All-in-one_chayLichenyi/module/xiaogongju.py`

 * *Files identical despite different names*

### Comparing `All-in-one-chay-2.4.5/src/All_in_one_chay.egg-info/PKG-INFO` & `All-in-one-chay-2.4.6/src/All_in_one_chay.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: All-in-one-chay
-Version: 2.4.5
+Version: 2.4.6
 Summary: 多功能一体机（All-in-one）
-Home-page: https://github.com/lichenyichay/All-in-one/releases/tag/v2.4.5
+Home-page: https://github.com/lichenyichay/All-in-one/releases/tag/v2.4.6
 Author: Chay
 Author-email: chay <lichenyi_2020@qq.com>
-Project-URL: Homepage, https://github.com/lichenyichay/All-in-one/releases/tag/v2.4.5
+Project-URL: Homepage, https://github.com/lichenyichay/All-in-one/releases/tag/v2.4.6
 Project-URL: Issues, https://github.com/lichenyichay/All-in-one/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.0.0
+Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # All-in-one
 多功能一体机
 说明如下：
 ```python
```

### Comparing `All-in-one-chay-2.4.5/src/All_in_one_chay.egg-info/SOURCES.txt` & `All-in-one-chay-2.4.6/src/All_in_one_chay.egg-info/SOURCES.txt`

 * *Files identical despite different names*

