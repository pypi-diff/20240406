# Comparing `tmp/MohuPy-0.2.7.tar.gz` & `tmp/MohuPy-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MohuPy-0.2.7.tar", last modified: Tue Apr  2 03:46:20 2024, max compression
+gzip compressed data, was "MohuPy-0.2.8.tar", last modified: Sat Apr  6 08:34:23 2024, max compression
```

## Comparing `MohuPy-0.2.7.tar` & `MohuPy-0.2.8.tar`

### file list

```diff
@@ -1,80 +1,81 @@
-drwxr-xr-x   0 yibow      (501) staff       (20)        0 2024-04-02 03:46:20.111111 MohuPy-0.2.7/
--rw-r--r--   0 yibow      (501) staff       (20)     1061 2023-01-29 07:30:33.000000 MohuPy-0.2.7/LICENSE
-drwxr-xr-x   0 yibow      (501) staff       (20)        0 2024-04-02 03:46:20.110593 MohuPy-0.2.7/MohuPy.egg-info/
--rw-r--r--   0 yibow      (501) staff       (20)     4175 2024-04-02 03:46:20.000000 MohuPy-0.2.7/MohuPy.egg-info/PKG-INFO
--rw-r--r--   0 yibow      (501) staff       (20)     1477 2024-04-02 03:46:20.000000 MohuPy-0.2.7/MohuPy.egg-info/SOURCES.txt
--rw-r--r--   0 yibow      (501) staff       (20)        1 2024-04-02 03:46:20.000000 MohuPy-0.2.7/MohuPy.egg-info/dependency_links.txt
--rw-r--r--   0 yibow      (501) staff       (20)       39 2024-04-02 03:46:20.000000 MohuPy-0.2.7/MohuPy.egg-info/requires.txt
--rw-r--r--   0 yibow      (501) staff       (20)        7 2024-04-02 03:46:20.000000 MohuPy-0.2.7/MohuPy.egg-info/top_level.txt
--rw-r--r--   0 yibow      (501) staff       (20)     4175 2024-04-02 03:46:20.110877 MohuPy-0.2.7/PKG-INFO
--rw-r--r--   0 yibow      (501) staff       (20)     3581 2023-11-29 10:30:24.000000 MohuPy-0.2.7/README.md
-drwxr-xr-x   0 yibow      (501) staff       (20)        0 2024-04-02 03:46:20.095346 MohuPy-0.2.7/mohupy/
--rw-r--r--   0 yibow      (501) staff       (20)      956 2023-11-29 08:28:50.000000 MohuPy-0.2.7/mohupy/__init__.py
-drwxr-xr-x   0 yibow      (501) staff       (20)        0 2024-04-02 03:46:20.096115 MohuPy-0.2.7/mohupy/config/
--rw-r--r--   0 yibow      (501) staff       (20)      460 2023-11-29 07:37:14.000000 MohuPy-0.2.7/mohupy/config/__init__.py
--rw-r--r--   0 yibow      (501) staff       (20)      268 2023-11-29 07:40:11.000000 MohuPy-0.2.7/mohupy/config/tnorms.py
--rw-r--r--   0 yibow      (501) staff       (20)     1233 2023-11-28 09:03:14.000000 MohuPy-0.2.7/mohupy/constant.py
-drwxr-xr-x   0 yibow      (501) staff       (20)        0 2024-04-02 03:46:20.099976 MohuPy-0.2.7/mohupy/core/
--rw-r--r--   0 yibow      (501) staff       (20)     1312 2023-12-23 07:04:59.000000 MohuPy-0.2.7/mohupy/core/__init__.py
--rw-r--r--   0 yibow      (501) staff       (20)     2835 2023-11-29 07:28:40.000000 MohuPy-0.2.7/mohupy/core/__nums_operation.py
--rw-r--r--   0 yibow      (501) staff       (20)     4408 2023-12-23 06:58:06.000000 MohuPy-0.2.7/mohupy/core/array.py
--rw-r--r--   0 yibow      (501) staff       (20)     8332 2023-12-19 06:12:31.000000 MohuPy-0.2.7/mohupy/core/attributes.py
--rw-r--r--   0 yibow      (501) staff       (20)      441 2023-11-28 07:07:28.000000 MohuPy-0.2.7/mohupy/core/base.py
--rw-r--r--   0 yibow      (501) staff       (20)    28339 2024-04-02 03:41:55.000000 MohuPy-0.2.7/mohupy/core/function.py
--rw-r--r--   0 yibow      (501) staff       (20)     2213 2023-12-23 07:05:05.000000 MohuPy-0.2.7/mohupy/core/fuzzfunc.py
--rw-r--r--   0 yibow      (501) staff       (20)     2188 2023-12-23 06:35:06.000000 MohuPy-0.2.7/mohupy/core/nums.py
--rw-r--r--   0 yibow      (501) staff       (20)    20508 2024-01-17 16:54:16.000000 MohuPy-0.2.7/mohupy/core/operation.py
--rw-r--r--   0 yibow      (501) staff       (20)     1175 2023-12-23 06:37:21.000000 MohuPy-0.2.7/mohupy/core/package.py
--rw-r--r--   0 yibow      (501) staff       (20)     1724 2023-11-28 07:11:34.000000 MohuPy-0.2.7/mohupy/core/regedit.py
-drwxr-xr-x   0 yibow      (501) staff       (20)        0 2024-04-02 03:46:20.100710 MohuPy-0.2.7/mohupy/function/
--rw-r--r--   0 yibow      (501) staff       (20)      420 2023-09-23 06:14:48.000000 MohuPy-0.2.7/mohupy/function/__init__.py
--rw-r--r--   0 yibow      (501) staff       (20)     9147 2023-10-01 12:31:19.000000 MohuPy-0.2.7/mohupy/function/func.py
--rw-r--r--   0 yibow      (501) staff       (20)     4505 2023-10-01 12:31:54.000000 MohuPy-0.2.7/mohupy/function/mem_func.py
-drwxr-xr-x   0 yibow      (501) staff       (20)        0 2024-04-02 03:46:20.100962 MohuPy-0.2.7/mohupy/generator/
--rw-r--r--   0 yibow      (501) staff       (20)      163 2023-10-01 08:16:28.000000 MohuPy-0.2.7/mohupy/generator/__init__.py
-drwxr-xr-x   0 yibow      (501) staff       (20)        0 2024-04-02 03:46:20.103392 MohuPy-0.2.7/mohupy/lib/
--rw-r--r--   0 yibow      (501) staff       (20)     1345 2023-12-02 09:45:46.000000 MohuPy-0.2.7/mohupy/lib/__init__.py
--rw-r--r--   0 yibow      (501) staff       (20)      491 2023-11-28 10:38:49.000000 MohuPy-0.2.7/mohupy/lib/base.py
--rw-r--r--   0 yibow      (501) staff       (20)     3710 2023-12-23 07:16:40.000000 MohuPy-0.2.7/mohupy/lib/construct.py
--rw-r--r--   0 yibow      (501) staff       (20)     4771 2024-03-24 04:05:54.000000 MohuPy-0.2.7/mohupy/lib/io.py
--rw-r--r--   0 yibow      (501) staff       (20)     2405 2023-11-29 05:15:05.000000 MohuPy-0.2.7/mohupy/lib/measure.py
--rw-r--r--   0 yibow      (501) staff       (20)     2946 2023-11-28 11:47:35.000000 MohuPy-0.2.7/mohupy/lib/other.py
--rw-r--r--   0 yibow      (501) staff       (20)     2226 2024-01-23 13:45:06.000000 MohuPy-0.2.7/mohupy/lib/plotlib.py
--rw-r--r--   0 yibow      (501) staff       (20)      430 2023-11-29 05:15:05.000000 MohuPy-0.2.7/mohupy/lib/string.py
--rw-r--r--   0 yibow      (501) staff       (20)     4769 2023-12-11 07:01:28.000000 MohuPy-0.2.7/mohupy/lib/utils.py
-drwxr-xr-x   0 yibow      (501) staff       (20)        0 2024-04-02 03:46:20.104326 MohuPy-0.2.7/mohupy/math/
--rw-r--r--   0 yibow      (501) staff       (20)      318 2023-11-29 08:28:01.000000 MohuPy-0.2.7/mohupy/math/__init__.py
--rw-r--r--   0 yibow      (501) staff       (20)      494 2023-11-29 05:40:06.000000 MohuPy-0.2.7/mohupy/math/base.py
--rw-r--r--   0 yibow      (501) staff       (20)     3116 2023-11-29 08:26:50.000000 MohuPy-0.2.7/mohupy/math/norms.py
--rw-r--r--   0 yibow      (501) staff       (20)     8366 2023-11-29 08:27:39.000000 MohuPy-0.2.7/mohupy/math/product.py
-drwxr-xr-x   0 yibow      (501) staff       (20)        0 2024-04-02 03:46:20.105769 MohuPy-0.2.7/mohupy/measure/
--rw-r--r--   0 yibow      (501) staff       (20)      710 2023-11-29 05:09:11.000000 MohuPy-0.2.7/mohupy/measure/__init__.py
--rw-r--r--   0 yibow      (501) staff       (20)    11003 2023-11-28 12:01:09.000000 MohuPy-0.2.7/mohupy/measure/fuzzmeas.py
--rw-r--r--   0 yibow      (501) staff       (20)     5312 2023-10-01 12:26:14.000000 MohuPy-0.2.7/mohupy/measure/hasse.py
--rw-r--r--   0 yibow      (501) staff       (20)     6189 2024-04-02 03:39:44.000000 MohuPy-0.2.7/mohupy/measure/indices.py
--rw-r--r--   0 yibow      (501) staff       (20)     6566 2023-12-01 08:41:17.000000 MohuPy-0.2.7/mohupy/measure/integral.py
--rw-r--r--   0 yibow      (501) staff       (20)     5549 2023-11-25 10:47:47.000000 MohuPy-0.2.7/mohupy/measure/utils.py
-drwxr-xr-x   0 yibow      (501) staff       (20)        0 2024-04-02 03:46:20.106511 MohuPy-0.2.7/mohupy/random/
--rw-r--r--   0 yibow      (501) staff       (20)      311 2023-11-29 10:29:10.000000 MohuPy-0.2.7/mohupy/random/__init__.py
--rw-r--r--   0 yibow      (501) staff       (20)      489 2023-11-29 05:39:47.000000 MohuPy-0.2.7/mohupy/random/base.py
--rw-r--r--   0 yibow      (501) staff       (20)     4235 2024-03-26 08:29:32.000000 MohuPy-0.2.7/mohupy/random/rand.py
-drwxr-xr-x   0 yibow      (501) staff       (20)        0 2024-04-02 03:46:20.108445 MohuPy-0.2.7/mohupy/regedit/
--rw-r--r--   0 yibow      (501) staff       (20)     1076 2023-11-29 07:34:01.000000 MohuPy-0.2.7/mohupy/regedit/__init__.py
--rw-r--r--   0 yibow      (501) staff       (20)     4218 2023-11-30 04:27:07.000000 MohuPy-0.2.7/mohupy/regedit/algebraic_operation.py
--rw-r--r--   0 yibow      (501) staff       (20)     3327 2023-12-23 07:12:54.000000 MohuPy-0.2.7/mohupy/regedit/construct.py
--rw-r--r--   0 yibow      (501) staff       (20)     4539 2023-11-29 05:10:14.000000 MohuPy-0.2.7/mohupy/regedit/distance.py
--rw-r--r--   0 yibow      (501) staff       (20)     6913 2023-11-29 09:13:44.000000 MohuPy-0.2.7/mohupy/regedit/plotlib.py
--rw-r--r--   0 yibow      (501) staff       (20)     2656 2024-03-26 08:25:56.000000 MohuPy-0.2.7/mohupy/regedit/random.py
--rw-r--r--   0 yibow      (501) staff       (20)     2730 2024-03-24 03:56:45.000000 MohuPy-0.2.7/mohupy/regedit/str2num.py
--rw-r--r--   0 yibow      (501) staff       (20)      740 2023-11-29 08:36:20.000000 MohuPy-0.2.7/mohupy/runtime.py
-drwxr-xr-x   0 yibow      (501) staff       (20)        0 2024-04-02 03:46:20.109417 MohuPy-0.2.7/mohupy/src/
--rw-r--r--   0 yibow      (501) staff       (20)      163 2023-11-29 05:46:37.000000 MohuPy-0.2.7/mohupy/src/__init__.py
--rw-r--r--   0 yibow      (501) staff       (20)     4050 2023-11-29 06:59:55.000000 MohuPy-0.2.7/mohupy/src/algebraic.py
--rw-r--r--   0 yibow      (501) staff       (20)      495 2023-11-29 06:04:46.000000 MohuPy-0.2.7/mohupy/src/base.py
--rw-r--r--   0 yibow      (501) staff       (20)     1216 2023-11-29 06:17:55.000000 MohuPy-0.2.7/mohupy/src/einstein.py
-drwxr-xr-x   0 yibow      (501) staff       (20)        0 2024-04-02 03:46:20.109703 MohuPy-0.2.7/mohupy/utils/
--rw-r--r--   0 yibow      (501) staff       (20)      163 2023-11-28 12:06:14.000000 MohuPy-0.2.7/mohupy/utils/__init__.py
--rw-r--r--   0 yibow      (501) staff       (20)       38 2024-04-02 03:46:20.111151 MohuPy-0.2.7/setup.cfg
--rw-r--r--   0 yibow      (501) staff       (20)      900 2024-02-13 17:46:21.000000 MohuPy-0.2.7/setup.py
-drwxr-xr-x   0 yibow      (501) staff       (20)        0 2024-04-02 03:46:20.110092 MohuPy-0.2.7/test/
--rw-r--r--   0 yibow      (501) staff       (20)      223 2023-12-19 12:55:05.000000 MohuPy-0.2.7/test/test.py
+drwxr-xr-x   0 yibow      (501) staff       (20)        0 2024-04-06 08:34:23.387270 MohuPy-0.2.8/
+-rw-r--r--   0 yibow      (501) staff       (20)     1061 2023-01-29 07:30:33.000000 MohuPy-0.2.8/LICENSE
+drwxr-xr-x   0 yibow      (501) staff       (20)        0 2024-04-06 08:34:23.386714 MohuPy-0.2.8/MohuPy.egg-info/
+-rw-r--r--   0 yibow      (501) staff       (20)     4175 2024-04-06 08:34:23.000000 MohuPy-0.2.8/MohuPy.egg-info/PKG-INFO
+-rw-r--r--   0 yibow      (501) staff       (20)     1613 2024-04-06 08:34:23.000000 MohuPy-0.2.8/MohuPy.egg-info/SOURCES.txt
+-rw-r--r--   0 yibow      (501) staff       (20)        1 2024-04-06 08:34:23.000000 MohuPy-0.2.8/MohuPy.egg-info/dependency_links.txt
+-rw-r--r--   0 yibow      (501) staff       (20)       39 2024-04-06 08:34:23.000000 MohuPy-0.2.8/MohuPy.egg-info/requires.txt
+-rw-r--r--   0 yibow      (501) staff       (20)        7 2024-04-06 08:34:23.000000 MohuPy-0.2.8/MohuPy.egg-info/top_level.txt
+-rw-r--r--   0 yibow      (501) staff       (20)     4175 2024-04-06 08:34:23.387029 MohuPy-0.2.8/PKG-INFO
+-rw-r--r--   0 yibow      (501) staff       (20)     3581 2023-11-29 10:30:24.000000 MohuPy-0.2.8/README.md
+drwxr-xr-x   0 yibow      (501) staff       (20)        0 2024-04-06 08:34:23.377083 MohuPy-0.2.8/mohupy/
+-rw-r--r--   0 yibow      (501) staff       (20)     1002 2024-04-06 03:45:30.000000 MohuPy-0.2.8/mohupy/__init__.py
+drwxr-xr-x   0 yibow      (501) staff       (20)        0 2024-04-06 08:34:23.377498 MohuPy-0.2.8/mohupy/config/
+-rw-r--r--   0 yibow      (501) staff       (20)      460 2023-11-29 07:37:14.000000 MohuPy-0.2.8/mohupy/config/__init__.py
+-rw-r--r--   0 yibow      (501) staff       (20)      268 2023-11-29 07:40:11.000000 MohuPy-0.2.8/mohupy/config/tnorms.py
+-rw-r--r--   0 yibow      (501) staff       (20)     1233 2023-11-28 09:03:14.000000 MohuPy-0.2.8/mohupy/constant.py
+drwxr-xr-x   0 yibow      (501) staff       (20)        0 2024-04-06 08:34:23.379864 MohuPy-0.2.8/mohupy/core/
+-rw-r--r--   0 yibow      (501) staff       (20)     1329 2024-04-06 07:57:17.000000 MohuPy-0.2.8/mohupy/core/__init__.py
+-rw-r--r--   0 yibow      (501) staff       (20)      549 2024-04-06 07:30:36.000000 MohuPy-0.2.8/mohupy/core/attribute.py
+-rw-r--r--   0 yibow      (501) staff       (20)     6309 2024-04-06 06:10:13.000000 MohuPy-0.2.8/mohupy/core/attributeClass.py
+-rw-r--r--   0 yibow      (501) staff       (20)     1656 2024-04-06 07:09:37.000000 MohuPy-0.2.8/mohupy/core/base.py
+-rw-r--r--   0 yibow      (501) staff       (20)     1922 2024-04-06 07:11:34.000000 MohuPy-0.2.8/mohupy/core/construct.py
+-rw-r--r--   0 yibow      (501) staff       (20)    22524 2024-04-06 07:29:37.000000 MohuPy-0.2.8/mohupy/core/funcitonClass.py
+-rw-r--r--   0 yibow      (501) staff       (20)     2702 2024-04-06 07:29:47.000000 MohuPy-0.2.8/mohupy/core/function.py
+-rw-r--r--   0 yibow      (501) staff       (20)     5156 2024-04-06 06:33:31.000000 MohuPy-0.2.8/mohupy/core/fuzzarray.py
+-rw-r--r--   0 yibow      (501) staff       (20)     2905 2024-04-06 07:37:10.000000 MohuPy-0.2.8/mohupy/core/fuzznums.py
+-rw-r--r--   0 yibow      (501) staff       (20)    20399 2024-04-06 07:11:56.000000 MohuPy-0.2.8/mohupy/core/operation.py
+-rw-r--r--   0 yibow      (501) staff       (20)     2661 2024-04-06 07:21:11.000000 MohuPy-0.2.8/mohupy/core/operationClass.py
+drwxr-xr-x   0 yibow      (501) staff       (20)        0 2024-04-06 08:34:23.380615 MohuPy-0.2.8/mohupy/core/operationLib/
+-rw-r--r--   0 yibow      (501) staff       (20)      617 2024-04-06 06:52:42.000000 MohuPy-0.2.8/mohupy/core/operationLib/__init__.py
+-rw-r--r--   0 yibow      (501) staff       (20)     4127 2024-04-06 06:47:12.000000 MohuPy-0.2.8/mohupy/core/operationLib/algebraic.py
+-rw-r--r--   0 yibow      (501) staff       (20)     4169 2024-04-06 06:57:19.000000 MohuPy-0.2.8/mohupy/core/operationLib/algebraicoperation.py
+-rw-r--r--   0 yibow      (501) staff       (20)     1214 2024-04-06 06:48:09.000000 MohuPy-0.2.8/mohupy/core/operationLib/einstein.py
+-rw-r--r--   0 yibow      (501) staff       (20)     1181 2024-04-06 07:14:44.000000 MohuPy-0.2.8/mohupy/core/operationpackage.py
+-rw-r--r--   0 yibow      (501) staff       (20)     1722 2024-04-06 06:36:47.000000 MohuPy-0.2.8/mohupy/core/regedit.py
+drwxr-xr-x   0 yibow      (501) staff       (20)        0 2024-04-06 08:34:23.381190 MohuPy-0.2.8/mohupy/function/
+-rw-r--r--   0 yibow      (501) staff       (20)      420 2023-09-23 06:14:48.000000 MohuPy-0.2.8/mohupy/function/__init__.py
+-rw-r--r--   0 yibow      (501) staff       (20)     9147 2023-10-01 12:31:19.000000 MohuPy-0.2.8/mohupy/function/func.py
+-rw-r--r--   0 yibow      (501) staff       (20)     4505 2023-10-01 12:31:54.000000 MohuPy-0.2.8/mohupy/function/mem_func.py
+drwxr-xr-x   0 yibow      (501) staff       (20)        0 2024-04-06 08:34:23.381372 MohuPy-0.2.8/mohupy/generator/
+-rw-r--r--   0 yibow      (501) staff       (20)      163 2023-10-01 08:16:28.000000 MohuPy-0.2.8/mohupy/generator/__init__.py
+drwxr-xr-x   0 yibow      (501) staff       (20)        0 2024-04-06 08:34:23.382726 MohuPy-0.2.8/mohupy/lib/
+-rw-r--r--   0 yibow      (501) staff       (20)     1333 2024-04-06 03:45:30.000000 MohuPy-0.2.8/mohupy/lib/__init__.py
+-rw-r--r--   0 yibow      (501) staff       (20)      491 2023-11-28 10:38:49.000000 MohuPy-0.2.8/mohupy/lib/base.py
+-rw-r--r--   0 yibow      (501) staff       (20)     3968 2024-04-06 07:49:52.000000 MohuPy-0.2.8/mohupy/lib/construct.py
+-rw-r--r--   0 yibow      (501) staff       (20)     4673 2024-04-06 07:51:48.000000 MohuPy-0.2.8/mohupy/lib/io.py
+-rw-r--r--   0 yibow      (501) staff       (20)     2405 2023-11-29 05:15:05.000000 MohuPy-0.2.8/mohupy/lib/measure.py
+-rw-r--r--   0 yibow      (501) staff       (20)     2940 2024-04-06 03:45:30.000000 MohuPy-0.2.8/mohupy/lib/other.py
+-rw-r--r--   0 yibow      (501) staff       (20)     2226 2024-01-23 13:45:06.000000 MohuPy-0.2.8/mohupy/lib/plotlib.py
+-rw-r--r--   0 yibow      (501) staff       (20)      468 2024-04-06 07:53:05.000000 MohuPy-0.2.8/mohupy/lib/string.py
+-rw-r--r--   0 yibow      (501) staff       (20)     4902 2024-04-06 07:54:21.000000 MohuPy-0.2.8/mohupy/lib/utils.py
+drwxr-xr-x   0 yibow      (501) staff       (20)        0 2024-04-06 08:34:23.383212 MohuPy-0.2.8/mohupy/math/
+-rw-r--r--   0 yibow      (501) staff       (20)      318 2023-11-29 08:28:01.000000 MohuPy-0.2.8/mohupy/math/__init__.py
+-rw-r--r--   0 yibow      (501) staff       (20)      494 2023-11-29 05:40:06.000000 MohuPy-0.2.8/mohupy/math/base.py
+-rw-r--r--   0 yibow      (501) staff       (20)     8536 2024-04-06 07:55:41.000000 MohuPy-0.2.8/mohupy/math/product.py
+drwxr-xr-x   0 yibow      (501) staff       (20)        0 2024-04-06 08:34:23.384217 MohuPy-0.2.8/mohupy/measure/
+-rw-r--r--   0 yibow      (501) staff       (20)      710 2023-11-29 05:09:11.000000 MohuPy-0.2.8/mohupy/measure/__init__.py
+-rw-r--r--   0 yibow      (501) staff       (20)    11003 2023-11-28 12:01:09.000000 MohuPy-0.2.8/mohupy/measure/fuzzmeas.py
+-rw-r--r--   0 yibow      (501) staff       (20)     5312 2023-10-01 12:26:14.000000 MohuPy-0.2.8/mohupy/measure/hasse.py
+-rw-r--r--   0 yibow      (501) staff       (20)     6189 2024-04-02 03:39:44.000000 MohuPy-0.2.8/mohupy/measure/indices.py
+-rw-r--r--   0 yibow      (501) staff       (20)     6566 2023-12-01 08:41:17.000000 MohuPy-0.2.8/mohupy/measure/integral.py
+-rw-r--r--   0 yibow      (501) staff       (20)     5549 2023-11-25 10:47:47.000000 MohuPy-0.2.8/mohupy/measure/utils.py
+drwxr-xr-x   0 yibow      (501) staff       (20)        0 2024-04-06 08:34:23.384801 MohuPy-0.2.8/mohupy/random/
+-rw-r--r--   0 yibow      (501) staff       (20)      342 2024-04-06 03:45:30.000000 MohuPy-0.2.8/mohupy/random/__init__.py
+-rw-r--r--   0 yibow      (501) staff       (20)      489 2023-11-29 05:39:47.000000 MohuPy-0.2.8/mohupy/random/base.py
+-rw-r--r--   0 yibow      (501) staff       (20)     4245 2024-04-06 07:47:24.000000 MohuPy-0.2.8/mohupy/random/rand.py
+drwxr-xr-x   0 yibow      (501) staff       (20)        0 2024-04-06 08:34:23.385965 MohuPy-0.2.8/mohupy/regedit/
+-rw-r--r--   0 yibow      (501) staff       (20)     1100 2024-04-06 07:43:14.000000 MohuPy-0.2.8/mohupy/regedit/__init__.py
+-rw-r--r--   0 yibow      (501) staff       (20)     4492 2024-04-06 07:43:49.000000 MohuPy-0.2.8/mohupy/regedit/algebraic_operation.py
+-rw-r--r--   0 yibow      (501) staff       (20)     3327 2023-12-23 07:12:54.000000 MohuPy-0.2.8/mohupy/regedit/construct.py
+-rw-r--r--   0 yibow      (501) staff       (20)     4539 2023-11-29 05:10:14.000000 MohuPy-0.2.8/mohupy/regedit/distance.py
+-rw-r--r--   0 yibow      (501) staff       (20)     6913 2023-11-29 09:13:44.000000 MohuPy-0.2.8/mohupy/regedit/plotlib.py
+-rw-r--r--   0 yibow      (501) staff       (20)     2685 2024-04-06 07:46:44.000000 MohuPy-0.2.8/mohupy/regedit/random.py
+-rw-r--r--   0 yibow      (501) staff       (20)     2724 2024-04-06 07:47:03.000000 MohuPy-0.2.8/mohupy/regedit/str2num.py
+-rw-r--r--   0 yibow      (501) staff       (20)      757 2024-04-06 07:57:39.000000 MohuPy-0.2.8/mohupy/runtime.py
+drwxr-xr-x   0 yibow      (501) staff       (20)        0 2024-04-06 08:34:23.386090 MohuPy-0.2.8/mohupy/tensor/
+-rw-r--r--   0 yibow      (501) staff       (20)      161 2024-04-06 05:45:55.000000 MohuPy-0.2.8/mohupy/tensor/__init__.py
+drwxr-xr-x   0 yibow      (501) staff       (20)        0 2024-04-06 08:34:23.386312 MohuPy-0.2.8/mohupy/utils/
+-rw-r--r--   0 yibow      (501) staff       (20)      163 2023-11-28 12:06:14.000000 MohuPy-0.2.8/mohupy/utils/__init__.py
+-rw-r--r--   0 yibow      (501) staff       (20)       38 2024-04-06 08:34:23.387323 MohuPy-0.2.8/setup.cfg
+-rw-r--r--   0 yibow      (501) staff       (20)      900 2024-02-13 17:46:21.000000 MohuPy-0.2.8/setup.py
```

### Comparing `MohuPy-0.2.7/LICENSE` & `MohuPy-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `MohuPy-0.2.7/MohuPy.egg-info/PKG-INFO` & `MohuPy-0.2.8/MohuPy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MohuPy
-Version: 0.2.7
+Version: 0.2.8
 Summary: MohuPy is a fuzzy set calculation library, which contains fuzzy numbers, fuzzy measure, fuzzy sets and fuzzy membership functions. 
 Home-page: https://github.com/yibocat/MohuPy
 Author: Yibo Wang
 Author-email: yibocat@yeah.net
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `MohuPy-0.2.7/MohuPy.egg-info/SOURCES.txt` & `MohuPy-0.2.8/MohuPy.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -8,24 +8,30 @@
 MohuPy.egg-info/top_level.txt
 mohupy/__init__.py
 mohupy/constant.py
 mohupy/runtime.py
 mohupy/config/__init__.py
 mohupy/config/tnorms.py
 mohupy/core/__init__.py
-mohupy/core/__nums_operation.py
-mohupy/core/array.py
-mohupy/core/attributes.py
+mohupy/core/attribute.py
+mohupy/core/attributeClass.py
 mohupy/core/base.py
+mohupy/core/construct.py
+mohupy/core/funcitonClass.py
 mohupy/core/function.py
-mohupy/core/fuzzfunc.py
-mohupy/core/nums.py
+mohupy/core/fuzzarray.py
+mohupy/core/fuzznums.py
 mohupy/core/operation.py
-mohupy/core/package.py
+mohupy/core/operationClass.py
+mohupy/core/operationpackage.py
 mohupy/core/regedit.py
+mohupy/core/operationLib/__init__.py
+mohupy/core/operationLib/algebraic.py
+mohupy/core/operationLib/algebraicoperation.py
+mohupy/core/operationLib/einstein.py
 mohupy/function/__init__.py
 mohupy/function/func.py
 mohupy/function/mem_func.py
 mohupy/generator/__init__.py
 mohupy/lib/__init__.py
 mohupy/lib/base.py
 mohupy/lib/construct.py
@@ -33,15 +39,14 @@
 mohupy/lib/measure.py
 mohupy/lib/other.py
 mohupy/lib/plotlib.py
 mohupy/lib/string.py
 mohupy/lib/utils.py
 mohupy/math/__init__.py
 mohupy/math/base.py
-mohupy/math/norms.py
 mohupy/math/product.py
 mohupy/measure/__init__.py
 mohupy/measure/fuzzmeas.py
 mohupy/measure/hasse.py
 mohupy/measure/indices.py
 mohupy/measure/integral.py
 mohupy/measure/utils.py
@@ -51,13 +56,9 @@
 mohupy/regedit/__init__.py
 mohupy/regedit/algebraic_operation.py
 mohupy/regedit/construct.py
 mohupy/regedit/distance.py
 mohupy/regedit/plotlib.py
 mohupy/regedit/random.py
 mohupy/regedit/str2num.py
-mohupy/src/__init__.py
-mohupy/src/algebraic.py
-mohupy/src/base.py
-mohupy/src/einstein.py
-mohupy/utils/__init__.py
-test/test.py
+mohupy/tensor/__init__.py
+mohupy/utils/__init__.py
```

### Comparing `MohuPy-0.2.7/PKG-INFO` & `MohuPy-0.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MohuPy
-Version: 0.2.7
+Version: 0.2.8
 Summary: MohuPy is a fuzzy set calculation library, which contains fuzzy numbers, fuzzy measure, fuzzy sets and fuzzy membership functions. 
 Home-page: https://github.com/yibocat/MohuPy
 Author: Yibo Wang
 Author-email: yibocat@yeah.net
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `MohuPy-0.2.7/README.md` & `MohuPy-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `MohuPy-0.2.7/mohupy/__init__.py` & `MohuPy-0.2.8/mohupy/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,21 +18,24 @@
 # #                       fuzzPlot, fuzzString, fuzzDis,
 # #                       fuzzRandom, fuzzZeros, fuzzPoss,fuzzNegs)
 #
 # from .runtime import info
 # from .registry import *
 # from .config import Approx, approx
 
+__all__ = []
+
 from .config import *
 from .core import *
 from .function import *
 # from .generator import *
 from .lib import *
 from .math import *
 from .measure import *
 from .measure import integral, indices
 from .random import *
 from .regedit import *
 # from .utils import *
 from .runtime import info
 from .constant import *
 
+__all__ += ['random','measure']
```

### Comparing `MohuPy-0.2.7/mohupy/constant.py` & `MohuPy-0.2.8/mohupy/constant.py`

 * *Files identical despite different names*

### Comparing `MohuPy-0.2.7/mohupy/core/__init__.py` & `MohuPy-0.2.8/mohupy/core/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,42 +1,39 @@
-#  Copyright (c) yibocat 2023 All Rights Reserved
+#  Copyright (c) yibocat 2024 All Rights Reserved
 #  Python: 3.10.9
-#  Date: 2023/11/26 下午2:47
+#  Date: 2024/4/6 上午11:47
 #  Author: yibow
 #  Email: yibocat@yeah.net
 #  Software: MohuPy
+
 __all__ = []
 
-from .nums import Fuzznum
-from .array import Fuzzarray
 from .base import FuzzType
+from .fuzzarray import Fuzzarray
+from .fuzznums import Fuzznum
 
 from .function import normalize, broadcast_to
 from .regedit import Registry
-from .package import *
+from .operationpackage import *
+from .operationLib import archimedeanDict
 
-__all__ += ['FuzzType',
-            'Fuzznum',
-            'Fuzzarray',
-            'normalize',
-            'Registry',
-            'broadcast_to']
+__all__ += ['FuzzType', 'Fuzzarray', 'Fuzznum',
+            'normalize', 'broadcast_to', 'Registry', 'archimedeanDict']
 
-from .function import (isValid, isEmpty, isInitial, convert, qsort, unique,
+from .function import (valid, empty, initial, convert, qsort, unique,
                        append, remove, pop, reshape, squeeze, clear,
-                       ravel, flatten, getmax, getmin, getsum, getprod, mean,
-                       fmax, fmin)
+                       ravel, flatten, getmax, getmin, getsum,getprod,
+                       mean, fmax, fmin)
 from .operation import (add, sub, mul, div, pow, matmul, equal, inequal,
                         lt, gt, le, ge, getitem)
 
 __all__ += [
-    'isValid', 'isEmpty', 'isInitial', 'convert', 'qsort', 'unique',
+    'valid', 'empty', 'initial', 'convert', 'qsort', 'unique',
     'append', 'remove', 'pop', 'reshape', 'squeeze', 'clear',
     'ravel', 'flatten', 'getmax', 'getmin', 'getsum', 'getprod', 'mean',
     'fmax', 'fmin',
     'add', 'sub', 'mul', 'div', 'pow', 'matmul', 'equal', 'inequal',
     'lt', 'gt', 'le', 'ge', 'getitem'
 ]
 
-from .fuzzfunc import fuzznum, fuzzset
-
+from .construct import fuzznum, fuzzset
 __all__ += ['fuzznum', 'fuzzset']
```

### Comparing `MohuPy-0.2.7/mohupy/core/__nums_operation.py` & `MohuPy-0.2.8/mohupy/core/operationClass.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,75 +1,70 @@
-#  Copyright (c) yibocat 2023 All Rights Reserved
+#  Copyright (c) yibocat 2024 All Rights Reserved
 #  Python: 3.10.9
-#  Date: 2023/11/27 下午7:11
+#  Date: 2024/4/6 下午2:55
 #  Author: yibow
 #  Email: yibocat@yeah.net
 #  Software: MohuPy
 
-# from ..regedit.algebraic_operation import (algebAdd, algebSub,
-#                                            algebMul, algebDiv,
-#                                            algebPow, algebTim)
-
-from ..regedit import archimedeanDict
-from ..config import Norms
+from .operationLib import archimedeanDict
 
 
 class BasicOperation:
+    norms = 'algebraic'
 
     def __init__(self, qrung, mtype):
         self.qrung = qrung
         self.mtype = mtype
 
     def add(self, x, y):
-        from .nums import Fuzznum
+        from .fuzznums import Fuzznum
         newfn = Fuzznum()
         newfn.mtype = self.mtype
         newfn.qrung = self.qrung
-        newfn.md = archimedeanDict[Norms.arch]['add'][self.mtype](x.md, x.nmd, y.md, y.nmd, self.qrung)[0]
-        newfn.nmd = archimedeanDict[Norms.arch]['add'][self.mtype](x.md, x.nmd, y.md, y.nmd, self.qrung)[1]
+        newfn.md = archimedeanDict[self.norms]['add'][self.mtype](x.md, x.nmd, y.md, y.nmd, self.qrung)[0]
+        newfn.nmd = archimedeanDict[self.norms]['add'][self.mtype](x.md, x.nmd, y.md, y.nmd, self.qrung)[1]
         return newfn
 
     def sub(self, x, y):
-        from .nums import Fuzznum
+        from .fuzznums import Fuzznum
         newfn = Fuzznum()
         newfn.mtype = self.mtype
         newfn.qrung = self.qrung
-        newfn.md = archimedeanDict[Norms.arch]['sub'][self.mtype](x.md, x.nmd, y.md, y.nmd, self.qrung)[0]
-        newfn.nmd = archimedeanDict[Norms.arch]['sub'][self.mtype](x.md, x.nmd, y.md, y.nmd, self.qrung)[1]
+        newfn.md = archimedeanDict[self.norms]['sub'][self.mtype](x.md, x.nmd, y.md, y.nmd, self.qrung)[0]
+        newfn.nmd = archimedeanDict[self.norms]['sub'][self.mtype](x.md, x.nmd, y.md, y.nmd, self.qrung)[1]
         return newfn
 
     def mul(self, x, y):
-        from .nums import Fuzznum
+        from .fuzznums import Fuzznum
         newfn = Fuzznum()
         newfn.mtype = self.mtype
         newfn.qrung = self.qrung
-        newfn.md = archimedeanDict[Norms.arch]['mul'][self.mtype](x.md, x.nmd, y.md, y.nmd, self.qrung)[0]
-        newfn.nmd = archimedeanDict[Norms.arch]['mul'][self.mtype](x.md, x.nmd, y.md, y.nmd, self.qrung)[1]
+        newfn.md = archimedeanDict[self.norms]['mul'][self.mtype](x.md, x.nmd, y.md, y.nmd, self.qrung)[0]
+        newfn.nmd = archimedeanDict[self.norms]['mul'][self.mtype](x.md, x.nmd, y.md, y.nmd, self.qrung)[1]
         return newfn
 
     def div(self, x, y):
-        from .nums import Fuzznum
+        from .fuzznums import Fuzznum
         newfn = Fuzznum()
         newfn.mtype = self.mtype
         newfn.qrung = self.qrung
-        newfn.md = archimedeanDict[Norms.arch]['div'][self.mtype](x.md, x.nmd, y.md, y.nmd, self.qrung)[0]
-        newfn.nmd = archimedeanDict[Norms.arch]['div'][self.mtype](x.md, x.nmd, y.md, y.nmd, self.qrung)[1]
+        newfn.md = archimedeanDict[self.norms]['div'][self.mtype](x.md, x.nmd, y.md, y.nmd, self.qrung)[0]
+        newfn.nmd = archimedeanDict[self.norms]['div'][self.mtype](x.md, x.nmd, y.md, y.nmd, self.qrung)[1]
         return newfn
 
     def power(self, l, x):
-        from .nums import Fuzznum
+        from .fuzznums import Fuzznum
         newfn = Fuzznum()
         newfn.mtype = self.mtype
         newfn.qrung = self.qrung
-        newfn.md = archimedeanDict[Norms.arch]['pow'][self.mtype](l, x.md, x.nmd, self.qrung)[0]
-        newfn.nmd = archimedeanDict[Norms.arch]['pow'][self.mtype](l, x.md, x.nmd, self.qrung)[1]
+        newfn.md = archimedeanDict[self.norms]['pow'][self.mtype](l, x.md, x.nmd, self.qrung)[0]
+        newfn.nmd = archimedeanDict[self.norms]['pow'][self.mtype](l, x.md, x.nmd, self.qrung)[1]
         return newfn
 
     def times(self, l, x):
-        from .nums import Fuzznum
+        from .fuzznums import Fuzznum
         newfn = Fuzznum()
         newfn.mtype = self.mtype
         newfn.qrung = self.qrung
-        newfn.md = archimedeanDict[Norms.arch]['tim'][self.mtype](l, x.md, x.nmd, self.qrung)[0]
-        newfn.nmd = archimedeanDict[Norms.arch]['tim'][self.mtype](l, x.md, x.nmd, self.qrung)[1]
+        newfn.md = archimedeanDict[self.norms]['tim'][self.mtype](l, x.md, x.nmd, self.qrung)[0]
+        newfn.nmd = archimedeanDict[self.norms]['tim'][self.mtype](l, x.md, x.nmd, self.qrung)[1]
         return newfn
-
```

### Comparing `MohuPy-0.2.7/mohupy/core/function.py` & `MohuPy-0.2.8/mohupy/core/funcitonClass.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,41 +1,22 @@
-#  Copyright (c) yibocat 2023 All Rights Reserved
+#  Copyright (c) yibocat 2024 All Rights Reserved
 #  Python: 3.10.9
-#  Date: 2023/11/27 下午12:59
+#  Date: 2024/4/6 下午1:40
 #  Author: yibow
 #  Email: yibocat@yeah.net
 #  Software: MohuPy
-
-"""
-    Method file
-    which implements basic fuzzy number and fuzzy set operations. Most of the methods
-    can be run directly through the constructed set or number instance suffix, or with
-    mp.xxx (x), similar to np.xxx (x). All methods inherit from the method base class
-    Function, and need to specifically implement the abstract method of the base class,
-    which is the concrete implementation of each class or method. Each method is a class,
-    and then the function interface is used to implement the external call to that method.
-"""
-
 import copy
-import numpy as np
-
-from ..constant import Approx
 
+import numpy as np
 
-class Function:
-    """
-        The method base class consists of a call function and an abstract function.
-        Among them, function is the concrete implementation of its subclass method.
-    """
-
-    def __call__(self, *x):
-        return self.function(*x)
+from .base import Function
+from .fuzznums import Fuzznum
+from .fuzzarray import Fuzzarray
 
-    def function(self, *x):
-        raise NotImplementedError()
+from ..constant import Approx
 
 
 class InitializeNum(Function):
     """
         Initialization Method Class of Fuzzy Numbers(Fuzznum)
     """
 
@@ -92,18 +73,14 @@
             nonMemDegree = np.round(nmd, Approx.round)
 
             return mtype, memDegree, nonMemDegree
 
         raise TypeError(f'Unsupported data type or type error, md:{type(md)} and nmd:{type(nmd)}.')
 
 
-def initializeNum(qrung, md, nmd):
-    return InitializeNum()(qrung, md, nmd)
-
-
 class InitializeSet(Function):
     def function(self, qrung, mtype):
         if qrung is not None or mtype is not None:
             from .base import FuzzType
             assert mtype in FuzzType, f'Unsupported fuzzy types, mtype:{mtype}.'
             assert qrung > 0, f'Qrung must be greater than 0, qrung:{qrung}.'
 
@@ -111,22 +88,16 @@
             mtype = mtype
         else:
             qrung = None
             mtype = None
         return qrung, mtype
 
 
-def initializeSet(qrung, mtype):
-    return InitializeSet()(qrung, mtype)
-
-
 class Validity(Function):
     def function(self, x):
-        from .nums import Fuzznum
-        from .array import Fuzzarray
         if isinstance(x, Fuzznum):
             if x.mtype == 'qrofn':
                 if 0. <= x.md <= 1. and 0. <= x.nmd <= 1. \
                         and 0. <= x.md ** x.qrung + x.nmd ** x.qrung <= 1.:
                     return True
                 else:
                     return False
@@ -159,26 +130,20 @@
                 elif a4:
                     # print('a4')
                     return True
                 else:
                     return False
             raise TypeError(f'Unsupported mtype(type:{x.mtype}).')
         if isinstance(x, Fuzzarray):
-            vec_func = np.vectorize(lambda u: isValid(u))
+            vec_func = np.vectorize(lambda u: Validity()(u))
             return vec_func(x.array)
 
 
-def isValid(x):
-    return Validity()(x)
-
-
 class Empty(Function):
     def function(self, x, onlyfn):
-        from .nums import Fuzznum
-        from .array import Fuzzarray
         if isinstance(x, Fuzznum):
             if x.mtype == 'qrofn':
                 if x.md is None and x.nmd is None:
                     return True
                 else:
                     return False
             if x.mtype == 'ivfn':
@@ -190,33 +155,27 @@
                 if x.md.size == 0 and x.nmd.size == 0:
                     return True
                 else:
                     return False
             raise TypeError(f'Unsupported mtype, ,type:{x.mtype}.')
         if isinstance(x, Fuzzarray):
             if onlyfn:
-                vec_func = np.vectorize(lambda u: isEmpty(u, onlyfn))
+                vec_func = np.vectorize(lambda u: Empty()(u, onlyfn))
                 return vec_func(x.array)
             else:
                 return True if x.size == 0 else False
 
 
-def isEmpty(x, onlyfn=False):
-    return Empty()(x, onlyfn)
-
-
 class Initial(Function):
     """
         Determine whether the fuzzy set or fuzzy number is the initialized
         fuzzy set or fuzzy number
     """
 
     def function(self, x):
-        from .nums import Fuzznum
-        from .array import Fuzzarray
         if isinstance(x, Fuzznum):
             if x.qrung is not None:
                 return False
             if x.mtype is not None:
                 return False
             if x.md is not None:
                 return False
@@ -229,126 +188,97 @@
             if x.mtype is not None:
                 return False
             if x.array.size != 0:
                 return False
             return True
 
 
-def isInitial(x):
-    return Initial()(x)
-
-
 class Convert(Function):
     def function(self, x):
-        from .nums import Fuzznum
         if isinstance(x, Fuzznum):
             if x.mtype == 'qrofn':
                 return x.md, x.nmd
             if x.mtype == 'ivfn':
                 return x.md.tolist(), x.nmd.tolist()
             if x.mtype == 'qrohfn':
                 return x.md.tolist(), x.nmd.tolist()
         raise TypeError(f'Unsupported type: {type(x)}.')
 
 
-def convert(x):
-    return Convert()(x)
-
-
 class Qsort(Function):
     def function(self, x, reverse=True):
-        from .nums import Fuzznum
-        from .array import Fuzzarray
         if isinstance(x, Fuzznum):
             if x.mtype == 'qrohfn':
                 newfn = copy.deepcopy(x)
                 if reverse:
                     newfn.md = np.sort(x.md)
                     newfn.nmd = np.sort(x.nmd)
                 else:
                     newfn.md = np.abs(np.sort(-x.md))
                     newfn.nmd = np.abs(np.sort(-x.nmd))
                 return newfn
             else:
                 return x
         if isinstance(x, Fuzzarray):
-            vec_func = np.vectorize(lambda u: qsort(u, reverse=reverse))
+            vec_func = np.vectorize(lambda u: Qsort()(u, reverse=reverse))
             newset = Fuzzarray(x.qrung, x.mtype)
             newset.array = vec_func(x.array)
             return newset
 
 
-def qsort(x, reverse=True):
-    return Qsort()(x, reverse)
-
-
 class Unique(Function):
     """
         Simplify the membership and non-membership degrees with Approx.round precision
     """
 
     def function(self, x, onlyfn=False):
-        from .nums import Fuzznum
-        from .array import Fuzzarray
         if isinstance(x, Fuzznum):
             if x.mtype == 'qrohfn':
                 t = copy.deepcopy(x)
                 t.md = np.unique(x.md)
                 t.nmd = np.unique(x.nmd)
                 return t
             else:
                 return x
         if isinstance(x, Fuzzarray):
             if onlyfn:
-                vec_func = np.vectorize(lambda u: unique(u, onlyfn))
+                vec_func = np.vectorize(lambda u: Unique()(u, onlyfn))
                 newset = Fuzzarray(x.qrung, x.mtype)
                 newset.array = vec_func(x.array)
                 return newset
             else:
                 uni = np.unique(x.array)
                 newset = Fuzzarray(x.qrung, x.mtype)
                 newset.array = uni
                 return newset
 
 
-def unique(x, onlyfn=False):
-    return Unique()(x, onlyfn)
-
-
 class Transpose(Function):
     def function(self, x):
-        from .nums import Fuzznum
-        from .array import Fuzzarray
         if isinstance(x, Fuzznum):
             return copy.copy(x)
         if isinstance(x, Fuzzarray):
             st = x.array
             s = st.T
 
             newset = Fuzzarray(x.qrung, x.mtype)
             newset.array = s
             del st, s
             return newset
 
 
-def transpose(x):
-    return Transpose()(x)
-
-
 class Append(Function):
     """
         1. 模糊数 + 模糊数
         2. 模糊数 + 模糊集
         3. 模糊集 + 模糊数
         4. 模糊集 + 模糊集
     """
 
     def function(self, x, e):
-        from .nums import Fuzznum
-        from .array import Fuzzarray
         if isinstance(x, Fuzznum) and isinstance(e, Fuzznum):
             assert x.qrung == e.qrung, f'qrung mismatch(x.qrung:{x.qrung} and e.qrung:{e.qrung}).'
             assert x.mtype == e.mtype, f'mtype mismatch(x.mtype:{x.mtype} and e.mtype:{e.mtype}).'
             newset = Fuzzarray(x.qrung, x.mtype)
             newset.array = np.append(newset.array, [x, e])
             return newset
         if isinstance(x, Fuzznum) and isinstance(e, Fuzzarray):
@@ -386,163 +316,109 @@
                 e.array = np.append(e.array, x.array)
                 return e
             else:
                 return x
         raise TypeError(f'Unsupported type({type(x)} and {type(e)}).')
 
 
-def append(x, e):
-    return Append()(x, e)
-
-
 class Remove(Function):
     def function(self, x, e):
-        from .nums import Fuzznum
-        from .array import Fuzzarray
         if isinstance(x, Fuzznum):
             raise ValueError(f'Deletion is not supported for {str(x)}')
         if isinstance(x, Fuzzarray):
             assert x.size > 0, 'The set is empty, can not be removed.'
             assert e in x.array, f'{x} is not in the set.'
             x.array = np.delete(x.array, np.where(x.array == e))
             return x
 
 
-def remove(x, e):
-    return Remove()(x, e)
-
-
 class Pop(Function):
     def function(self, x, i):
-        from .nums import Fuzznum
-        from .array import Fuzzarray
         if isinstance(x, Fuzznum):
             raise ValueError(f'Deletion is not supported for {str(x)}')
         if isinstance(x, Fuzzarray):
             x.array = np.delete(x.array, i)
             return x
 
 
-def pop(x, e):
-    return Pop()(x, e)
-
-
 class Reshape(Function):
     def function(self, x, *shape):
-        from .nums import Fuzznum
-        from .array import Fuzzarray
         if isinstance(x, Fuzznum):
             newset = Fuzzarray(x.qrung, x.mtype)
             newset.array = np.reshape(x, *shape)
             return newset
         if isinstance(x, Fuzzarray):
             newset = Fuzzarray(x.qrung, x.mtype)
             newset.array = x.array.reshape(*shape)
             return newset
 
 
-def reshape(x, *shape):
-    return Reshape()(x, *shape)
-
-
 class Squeeze(Function):
     def function(self, x, axis):
-        from .nums import Fuzznum
-        from .array import Fuzzarray
         if isinstance(x, Fuzznum):
             return x
         if isinstance(x, Fuzzarray):
             newset = Fuzzarray(x.qrung, x.mtype)
             newset.array = np.squeeze(x.array, axis)
             return newset
 
 
-def squeeze(x, axis=None):
-    return Squeeze()(x, axis)
-
-
 class Broadcast(Function):
     def function(self, x, shape):
-        from .nums import Fuzznum
-        from .array import Fuzzarray
         if isinstance(x, Fuzznum):
             newset = Fuzzarray(x.qrung, x.mtype)
             newset.array = np.broadcast_to(x, shape)
             return newset
         if isinstance(x, Fuzzarray):
             newset = Fuzzarray(x.qrung, x.mtype)
             newset.array = np.broadcast_to(x.array, shape)
             return newset
 
 
-def broadcast_to(x, shape):
-    return Broadcast()(x, shape)
-
-
 class Clear(Function):
     def function(self, x):
-        from .nums import Fuzznum
-        from .array import Fuzzarray
         if isinstance(x, Fuzznum):
             x.qrung = None
             x.mtype = None
             x.md = None
             x.nmd = None
             return x
         if isinstance(x, Fuzzarray):
             x.array = np.array([], dtype=object)
             x.qrung = None
             x.mtype = None
             return x
 
 
-def clear(x):
-    return Clear()(x)
-
-
 class Ravel(Function):
     def function(self, x):
-        from .nums import Fuzznum
-        from .array import Fuzzarray
         if isinstance(x, Fuzznum):
             newset = Fuzzarray(x.qrung, x.mtype)
             newset.array = np.ravel(x)
             return newset
         if isinstance(x, Fuzzarray):
             newset = Fuzzarray(x.qrung, x.mtype)
             newset.array = np.ravel(x.array)
             return newset
 
 
-def ravel(x):
-    return Ravel()(x)
-
-
 class Flatten(Function):
     def function(self, x):
-        from .nums import Fuzznum
-        from .array import Fuzzarray
         if isinstance(x, Fuzznum):
             newset = Fuzzarray(x.qrung, x.mtype)
             newset.array = np.array([x])
             return newset
         if isinstance(x, Fuzzarray):
             newset = Fuzzarray(x.qrung, x.mtype)
             newset.array = x.array.flatten()
             return newset
 
 
-def flatten(x):
-    return Flatten()(x)
-
-
 class GetMax(Function):
     def function(self, x, show, axis):
-        from .nums import Fuzznum
-        from .array import Fuzzarray
         if isinstance(x, Fuzznum):
             return x
         if isinstance(x, Fuzzarray):
             if axis is None:
                 index = np.unravel_index(np.argmax(x.array), x.shape)
                 if show:
                     print(index)
@@ -553,22 +429,16 @@
                     return m
                 if isinstance(m, np.ndarray):
                     newset = Fuzzarray(x.qrung, x.mtype)
                     newset.array = m
                     return newset
 
 
-def getmax(x, show=False, axis=None):
-    return GetMax()(x, show, axis)
-
-
 class GetMin(Function):
     def function(self, x, show, axis):
-        from .nums import Fuzznum
-        from .array import Fuzzarray
         if isinstance(x, Fuzznum):
             return x
         if isinstance(x, Fuzzarray):
             if axis is None:
                 index = np.unravel_index(np.argmin(x.array), x.shape)
                 if show:
                     print(index)
@@ -579,22 +449,16 @@
                     return m
                 if isinstance(m, np.ndarray):
                     newset = Fuzzarray(x.qrung, x.mtype)
                     newset.array = m
                     return newset
 
 
-def getmin(x, show=False, axis=None):
-    return GetMin()(x, show, axis)
-
-
 class GetFmax(Function):
     def function(self, x, func, *args, show, axis):
-        from .nums import Fuzznum
-        from .array import Fuzzarray
         if isinstance(x, Fuzznum):
             raise TypeError(f'Unsupported type({type(x)})')
         if isinstance(x, Fuzzarray):
             slist = func(x.array, *args)
             if axis is None:
                 index = np.unravel_index(np.argmax(slist), x.shape)
                 if show:
@@ -606,22 +470,16 @@
                     return m
                 if isinstance(slist, np.ndarray):
                     newset = Fuzzarray(x.qrung, x.mtype)
                     newset.array = m
                     return newset
 
 
-def fmax(x, func, *args, show=False, axis=None):
-    return GetMax()(x, func, *args, show, axis)
-
-
 class GetFmin(Function):
     def function(self, x, func, *args, show, axis):
-        from .nums import Fuzznum
-        from .array import Fuzzarray
         if isinstance(x, Fuzznum):
             raise TypeError(f'Unsupported type({type(x)})')
         if isinstance(x, Fuzzarray):
             slist = func(x.array, *args)
             if axis is None:
                 index = np.unravel_index(np.argmin(slist), x.shape)
                 if show:
@@ -633,22 +491,16 @@
                     return m
                 if isinstance(slist, np.ndarray):
                     newset = Fuzzarray(x.qrung, x.mtype)
                     newset.array = m
                     return newset
 
 
-def fmin(x, func, *args, show=False, axis=None):
-    return GetFmin()(x, func, *args, show, axis)
-
-
 class GetSum(Function):
     def function(self, x, axis, keepdims):
-        from .nums import Fuzznum
-        from .array import Fuzzarray
         if isinstance(x, Fuzznum):
             return x
         if isinstance(x, Fuzzarray):
             if axis is None:
                 return np.sum(x.array)
             else:
                 s = np.sum(x.array, axis=axis, keepdims=keepdims)
@@ -656,22 +508,16 @@
                     return s
                 if isinstance(s, np.ndarray):
                     newset = Fuzzarray(x.qrung, x.mtype)
                     newset.array = s
                     return newset
 
 
-def getsum(x, axis=None, keepdims=False):
-    return GetSum()(x, axis, keepdims)
-
-
 class GetProd(Function):
     def function(self, x, axis, keepdims):
-        from .nums import Fuzznum
-        from .array import Fuzzarray
         if isinstance(x, Fuzznum):
             return x
         if isinstance(x, Fuzzarray):
             if axis is None:
                 return np.prod(x.array)
             else:
                 s = np.prod(x.array, axis=axis, keepdims=keepdims)
@@ -679,22 +525,16 @@
                     return s
                 if isinstance(s, np.ndarray):
                     newset = Fuzzarray(x.qrung, x.mtype)
                     newset.array = s
                     return newset
 
 
-def getprod(x, axis=None, keepdims=False):
-    return GetProd()(x, axis, keepdims)
-
-
 class Mean(Function):
     def function(self, x, axis):
-        from .nums import Fuzznum
-        from .array import Fuzzarray
         if isinstance(x, Fuzznum):
             return x
         if isinstance(x, Fuzzarray):
             if axis is None:
                 return np.mean(x.array)
             else:
                 s = np.mean(x.array, axis=axis)
@@ -702,18 +542,14 @@
                     return s
                 if isinstance(s, np.ndarray):
                     newset = Fuzzarray(x.qrung, x.mtype)
                     newset.array = s
                     return newset
 
 
-def mean(x, axis=None):
-    return Mean()(x, axis)
-
-
 class Normalize(Function):
     def function(self, d1, d2, t):
         """
             The normalization function for two q-rung orthopair hesitant fuzzy numbers.
                 The parameter 't' is the risk factor of normalization process, which in
                 the interval [0, 1]. 't=1' indicates optimistic normalization and
                 't=0' indicates pessimistic normalization.
@@ -775,79 +611,11 @@
                     d_1.nmd = np.append(d_1.nmd, __adj(u, t))
                     i += 1
             return d_1.qsort(), d_2.qsort()
         else:
             raise TypeError(f'Unsupported fuzzy type, {d1.mtype} and {d2.mtype}')
 
 
-def normalize(d1, d2, t=1.):
-    return Normalize()(d1, d2, t)
-
-
 # TODO：待实现
 class Absolute(Function):
     def function(self, x, y):
-        pass
-
-
-def absolute(x, y):
-    return Absolute()(x, y)
-
-
-# class FuzzNum(Function):
-#     """
-#         The method of generating fuzzy numbers is encapsulated in a fuzzy number
-#         class, which only generates fuzzy numbers and does not undertake other
-#         functions.
-#         'function' returns a fuzzy number of type Fuzznum
-#     """
-#
-#     def function(self, qrung, md, nmd):
-#         from .nums import Fuzznum
-#         return Fuzznum(qrung, md, nmd)
-#
-#
-# def fuzznum(qrung=None, md=None, nmd=None):
-#     return FuzzNum()(qrung, md, nmd)
-#
-#
-# class FuzzSet(Function):
-#     """
-#         This class is just a class for generating a fuzzy array,
-#             specifically implemented with function. Similar to the numpy.array method.
-#     """
-#
-#     def function(self, x):
-#         from .array import Fuzzarray
-#         from .nums import Fuzznum
-#         if x is None:
-#             return Fuzzarray()
-#         y = x
-#         if isinstance(x, Fuzznum):
-#             fl = np.asarray(y, dtype=object)
-#             flat = fl.flatten()
-#             r = np.random.choice(flat)
-#             newset = Fuzzarray(r.qrung, r.mtype)
-#             newset.array = fl
-#             return newset
-#         if isinstance(x, (list, tuple, np.ndarray)):
-#             y = np.asarray(x, dtype=object)
-#             y = y.flatten()
-#             mt = y[0].mtype
-#             for i in y:
-#                 if i.mtype != mt:
-#                     raise TypeError(f'Unsupported mtype: {i.mtype}.')
-#                 mt = i.mtype
-#
-#             t = np.random.choice(y)
-#             qrung = t.qrung
-#             mtype = t.mtype
-#
-#             newset = Fuzzarray(qrung, mtype)
-#             newset.array = np.array(x, dtype=object)
-#             return newset
-#
-#         raise TypeError(f'Unsupported type: {type(x)}.')
-#
-#
-# def fuzzset(x=None):
-#     return FuzzSet()(x)
+        ValueError(f'Not yet implemented!')
```

### Comparing `MohuPy-0.2.7/mohupy/core/fuzzfunc.py` & `MohuPy-0.2.8/mohupy/core/construct.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,49 +1,35 @@
-#  Copyright (c) yibocat 2023 All Rights Reserved
+#  Copyright (c) yibocat 2024 All Rights Reserved
 #  Python: 3.10.9
-#  Date: 2023/12/23 下午2:59
+#  Date: 2024/4/6 下午3:07
 #  Author: yibow
 #  Email: yibocat@yeah.net
 #  Software: MohuPy
 
 import numpy as np
-from .nums import Fuzznum
-from .array import Fuzzarray
 
+from .fuzznums import Fuzznum
+from .fuzzarray import Fuzzarray
 
-class FuzzFunc:
-    """
-        The method base class consists of a call function and an abstract function.
-        Among them, function is the concrete implementation of its subclass method.
-    """
-
-    def __call__(self, *x):
-        return self.function(*x)
+from .base import Construct
 
-    def function(self, *x):
-        raise NotImplementedError()
 
-
-class FuzzNum(FuzzFunc):
+class FuzzNum(Construct):
     """
         The method of generating fuzzy numbers is encapsulated in a fuzzy number
         class, which only generates fuzzy numbers and does not undertake other
         functions.
         'function' returns a fuzzy number of type Fuzznum
     """
 
     def function(self, qrung, md, nmd):
         return Fuzznum(qrung, md, nmd)
 
 
-def fuzznum(qrung=None, md=None, nmd=None) -> Fuzznum:
-    return FuzzNum()(qrung, md, nmd)
-
-
-class FuzzSet(FuzzFunc):
+class FuzzSet(Construct):
     """
         This class is just a class for generating a fuzzy array,
             specifically implemented with function. Similar to the numpy.array method.
     """
 
     def function(self, x):
         if x is None:
@@ -72,9 +58,13 @@
             newset = Fuzzarray(qrung, mtype)
             newset.array = np.array(x, dtype=object)
             return newset
 
         raise TypeError(f'Unsupported type: {type(x)}.')
 
 
+def fuzznum(qrung=None, md=None, nmd=None) -> Fuzznum:
+    return FuzzNum()(qrung, md, nmd)
+
+
 def fuzzset(x=None) -> Fuzzarray:
     return FuzzSet()(x)
```

### Comparing `MohuPy-0.2.7/mohupy/core/nums.py` & `MohuPy-0.2.8/mohupy/core/fuzznums.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,83 +1,119 @@
-#  Copyright (c) yibocat 2023 All Rights Reserved
+#  Copyright (c) yibocat 2024 All Rights Reserved
 #  Python: 3.10.9
-#  Date: 2023/11/26 下午3:05
+#  Date: 2024/4/6 下午12:47
 #  Author: yibow
 #  Email: yibocat@yeah.net
 #  Software: MohuPy
+from typing import Union
 
-from .base import mohunum
-from .attributes import score, acc, ind, comp
-from .function import initializeNum, transpose
-from .function import (isValid, isEmpty, isInitial, convert, qsort, unique,
-                       append, reshape, squeeze, clear,
-                       ravel, flatten, getmax, getmin, getsum, getprod, mean)
+from .base import MohuBase
 
 
-class Fuzznum(mohunum):
+class Fuzznum(MohuBase):
     qrung = None
     mtype = None
     md = None
     nmd = None
 
     def __init__(self, qrung=None, md=None, nmd=None):
         self.ndim = 0
         self.size = 1
         self.shape = ()
 
+        from .function import initializeNum
         if qrung is not None and md is not None and nmd is not None:
             self.qrung = qrung
             self.mtype, self.md, self.nmd = initializeNum(qrung, md, nmd)
 
     @property
     def T(self):
+        from .function import transpose
         return transpose(self)
 
     @property
     def score(self):
+        from .attribute import score
         return score(self)
 
     @property
     def acc(self):
+        from .attribute import acc
         return acc(self)
 
     @property
     def ind(self):
+        from .attribute import ind
         return ind(self)
 
     @property
-    def comp(self): return comp(self)
-
-    def isValid(self): return isValid(self)
-
-    def isEmpty(self, onlyfn=False): return isEmpty(self, onlyfn)
-
-    def isInitial(self): return isInitial(self)
-
-    def convert(self): return convert(self)
-
-    def qsort(self, reverse=False): return qsort(self, reverse)
-
-    def unique(self, onlyfn=False): return unique(self, onlyfn)
-
-    def append(self, e): return append(self, e)
-
-    def reshape(self, *shape): return reshape(self, *shape)
-
-    def squeeze(self, axis=None): return squeeze(self, axis)
-
-    def clear(self): return clear(self)
-
-    def ravel(self): return ravel(self)
-
-    def flatten(self): return flatten(self)
-
-    def max(self, show=False, axis=None): return getmax(self, show, axis)
-
-    def min(self, show=False, axis=None): return getmin(self, show, axis)
-
-    def sum(self, axis=None, keepdims=False): return getsum(self, axis, keepdims)
-
-    def prod(self, axis=None, keepdims=False): return getprod(self, axis, keepdims)
-
-    def mean(self, axis=None): return mean(self, axis)
-
+    def comp(self):
+        from .attribute import comp
+        return comp(self)
+
+    def valid(self):
+        from .function import valid
+        return valid(self)
+
+    def empty(self, onlyfn=False):
+        from .function import empty
+        return empty(self, onlyfn)
+
+    def initial(self):
+        from .function import initial
+        return initial(self)
+
+    def convert(self):
+        from .function import convert
+        return convert(self)
+
+    def qsort(self, reverse=False):
+        from .function import qsort
+        return qsort(self, reverse=reverse)
+
+    def unique(self, onlyfn=False):
+        from .function import unique
+        return unique(self, onlyfn)
+
+    def append(self, e):
+        from .function import append
+        return append(self, e)
+
+    def reshape(self, *shape):
+        from .function import reshape
+        return reshape(self, *shape)
+
+    def squeeze(self, axis=None):
+        from .function import squeeze
+        return squeeze(self, axis)
+
+    def clear(self):
+        from .function import clear
+        return clear(self)
+
+    def ravel(self):
+        from .function import ravel
+        return ravel(self)
+
+    def flatten(self):
+        from .function import flatten
+        return flatten(self)
+
+    def max(self, show=False, axis=None):
+        from .function import getmax
+        return getmax(self, show, axis)
+
+    def min(self, show=False, axis=None):
+        from .function import getmin
+        return getmin(self, show, axis)
+
+    def sum(self, axis=None, keepdims=False):
+        from .function import getsum
+        return getsum(self, axis, keepdims)
+
+    def prod(self, axis=None, keepdims=False):
+        from .function import getprod
+        return getprod(self, axis, keepdims)
+
+    def mean(self, axis=None):
+        from .function import mean
+        return mean(self, axis)
```

### Comparing `MohuPy-0.2.7/mohupy/core/operation.py` & `MohuPy-0.2.8/mohupy/core/operation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,38 +1,31 @@
-#  Copyright (c) yibocat 2023 All Rights Reserved
+#  Copyright (c) yibocat 2024 All Rights Reserved
 #  Python: 3.10.9
-#  Date: 2023/11/27 下午7:15
+#  Date: 2024/4/6 下午3:01
 #  Author: yibow
 #  Email: yibocat@yeah.net
 #  Software: MohuPy
 
 import numpy as np
 
-from .nums import Fuzznum
-from .array import Fuzzarray
-
-from .__nums_operation import BasicOperation
-
-
-class Operation:
-    def __call__(self, *args):
-        return self.function(*args)
-
-    def function(self, *args):
-        raise NotImplementedError()
+from .base import Operation
+from .fuzznums import Fuzznum
+from .fuzzarray import Fuzzarray
+from .operationClass import BasicOperation
 
 
 class Addition(Operation):
     def function(self, x, y):
         """
             1. 模糊数 + 模糊数
             2. 模糊数 + 模糊集合
             3. 模糊集合 + 模糊数
             4. 模糊集合 + 模糊集合
         """
+
         def __add(x0, x1):
             assert x0.mtype == x1.mtype, f"mtype does not match('{x.mtype}' and '{x1.mtype}')."
             assert x0.qrung == x1.qrung, f"qrung does not match({x.qrung} and {x1.qrung})."
 
             operation = BasicOperation(x0.qrung, x0.mtype)
             return operation.add(x0, x1)
 
@@ -70,14 +63,15 @@
     def function(self, x, y):
         """
             1. 模糊数 - 模糊数
             2. 模糊数 - 模糊集合
             3. 模糊集合 - 模糊数
             4. 模糊集合 - 模糊集合
         """
+
         def __sub(x0, x1):
             assert x0.mtype == x1.mtype, f"mtype does not match('{x.mtype}' and '{x1.mtype}')."
             assert x0.qrung == x1.qrung, f"qrung does not match({x.qrung} and {x1.qrung})."
             operation = BasicOperation(x0.qrung, x0.mtype)
             return operation.sub(x0, x1)
 
         # 模糊数 - 模糊数
@@ -124,14 +118,15 @@
             8. 模糊集合 * 数
 
             9. 数 * 模糊数
             10.数 * 模糊集合
             11.数集合 * 模糊数
             12.数集合 * 模糊集合
         """
+
         def __mul(x0, x1):
             if isinstance(x0, Fuzznum) and isinstance(x1, Fuzznum):
                 assert x0.mtype == x1.mtype, f"mtype does not match('{x0.mtype}' and '{x1.mtype}')."
                 assert x0.qrung == x1.qrung, f"qrung does not match({x0.qrung} and {x1.qrung})."
                 operation = BasicOperation(x0.qrung, x0.mtype)
                 return operation.mul(x0, x1)
 
@@ -223,24 +218,25 @@
             4. 模糊数 / 数集合
 
             5. 模糊集合 / 模糊集合
             6. 模糊集合 / 模糊数
             7. 模糊集合 / 数集合
             8. 模糊集合 / 数
         """
+
         def __div(x0, x1):
             if isinstance(x0, Fuzznum) and isinstance(x1, Fuzznum):
                 assert x0.mtype == x1.mtype, f"mtype does not match: ('{x0.mtype}', '{x1.mtype}')."
                 assert x0.qrung == x1.qrung, f"qrung does not match: ({x0.qrung}, {x1.qrung})."
                 operation = BasicOperation(x0.qrung, x.mtype)
                 return operation.div(x0, x1)
             if isinstance(x0, Fuzznum) and isinstance(x1, (int, float, np.float_, np.int_)):
                 assert x1 > 0, f"value must be greater than 0: ({x1} <= 0)."
                 operation = BasicOperation(x0.qrung, x0.mtype)
-                return operation.times((1/x1), x0)
+                return operation.times((1 / x1), x0)
 
         if isinstance(x, Fuzznum) and isinstance(y, Fuzznum):
             return __div(x, y)
 
         if isinstance(x, Fuzznum) and isinstance(y, (int, float, np.float_, np.int_)):
             return __div(x, y)
 
@@ -292,14 +288,15 @@
     def function(self, x):
         """
             1. 模糊数 ** 数
             2. 模糊数 ** 数集合
             3. 模糊集合 ** 数
             4. 模糊集合 ** 数集合
         """
+
         def __pow(x0, p):
             assert p > 0, f"value must be greater than 0: ({self.p} <= 0)."
             operation = BasicOperation(x0.qrung, x0.mtype)
             return operation.power(p, x0)
 
         if isinstance(x, Fuzznum) and isinstance(self.p, (int, float, np.float_, np.int_)):
             return __pow(x, self.p)
@@ -345,14 +342,15 @@
     def function(self, x, y):
         """
             1. 模糊数 == 模糊数
             2. 模糊数 == 模糊集合
             3. 模糊集合 == 模糊数
             4. 模糊集合 == 模糊集合
         """
+
         def __eq(x0, x1):
             assert x0.mtype == x1.mtype, f"mtype does not match: ('{x0.mtype}', '{x1.mtype}')."
             assert x0.qrung == x1.qrung, f"qrung does not match: ({x0.qrung}, {x1.qrung})."
             return x0.md == x1.md and x0.nmd == x1.nmd
 
         if isinstance(x, Fuzznum) and isinstance(y, Fuzznum):
             return __eq(x, y)
@@ -378,14 +376,15 @@
     def function(self, x, y):
         """
             1. 模糊数 != 模糊数
             2. 模糊数 != 模糊集合
             3. 模糊集合 != 模糊数
             4. 模糊集合 != 模糊集合
         """
+
         def __ne(x0, x1):
             assert x0.mtype == x1.mtype, f"mtype does not match: ('{x0.mtype}', '{x1.mtype}')."
             assert x0.qrung == x1.qrung, f"qrung does not match: ({x0.qrung}, {x1.qrung})."
             return x0.md != x1.md or x0.nmd != x1.nmd
 
         if isinstance(x, Fuzznum) and isinstance(y, Fuzznum):
             return __ne(x, y)
@@ -411,14 +410,15 @@
     def function(self, x, y):
         """
             1. 模糊数 < 模糊数
             2. 模糊数 < 模糊集合
             3. 模糊集合 < 模糊数
             4. 模糊集合 < 模糊集合
         """
+
         def __lt(x0, x1):
             assert x0.mtype == x1.mtype, f"mtype does not match: ('{x0.mtype}', '{x1.mtype}')."
             assert x0.qrung == x1.qrung, f"qrung does not match: ({x0.qrung}, {x1.qrung})."
             # if x0.mtype == 'ivfn' or x0.mtype == 'qrohfn':
             #     return x0.score < x1.score
             # else:
             #     from .. import fuzznum
@@ -452,14 +452,15 @@
     def function(self, x, y):
         """
             1. 模糊数 > 模糊数
             2. 模糊数 > 模糊集合
             3. 模糊集合 > 模糊数
             4. 模糊集合 > 模糊集合
         """
+
         def __gt(x0, x1):
             assert x0.mtype == x1.mtype, f"mtype does not match: ('{x0.mtype}', '{x1.mtype}')."
             assert x0.qrung == x1.qrung, f"qrung does not match: ({x0.qrung}, {x1.qrung})."
             # if x0.mtype == 'ivfn' or x0.mtype == 'qrohfn':
             #     return x0.score > x1.score
             # else:
             #     from .. import fuzznum
@@ -493,14 +494,15 @@
     def function(self, x, y):
         """
             1. 模糊数 <= 模糊数
             2. 模糊数 <= 模糊集合
             3. 模糊集合 <= 模糊数
             4. 模糊集合 <= 模糊集合
         """
+
         def __le(x0, x1):
             assert x0.mtype == x1.mtype, f"mtype does not match: ('{x0.mtype}', '{x1.mtype}')."
             assert x0.qrung == x1.qrung, f"qrung does not match: ({x0.qrung}, {x1.qrung})."
             # if x0.mtype == 'ivfn' or x0.mtype == 'qrohfn':
             #     return x0.score <= x1.score
             # else:
             #     from .. import fuzznum
@@ -534,14 +536,15 @@
     def function(self, x, y):
         """
             1. 模糊数 >= 模糊数
             2. 模糊数 >= 模糊集合
             3. 模糊集合 >= 模糊数
             4. 模糊集合 >= 模糊集合
         """
+
         def __ge(x0, x1):
             assert x0.mtype == x1.mtype, f"mtype does not match: ('{x0.mtype}', '{x1.mtype}')."
             assert x0.qrung == x1.qrung, f"qrung does not match: ({x0.qrung}, {x1.qrung})."
             # if x0.mtype == 'ivfn' or x0.mtype == 'qrohfn':
             #     return x0.score >= x1.score
             # else:
             #     from .. import fuzznum
@@ -572,15 +575,15 @@
 
 
 class GetItem(Operation):
     def __init__(self, slices):
         self.slices = slices
 
     def function(self, x):
-        from .fuzzfunc import fuzzset
+        from .construct import fuzzset
         y = x.array[self.slices]
         if isinstance(y, np.ndarray):
             return fuzzset(y)
         else:
             return y
```

### Comparing `MohuPy-0.2.7/mohupy/core/package.py` & `MohuPy-0.2.8/mohupy/core/operationpackage.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-#  Copyright (c) yibocat 2023 All Rights Reserved
+#  Copyright (c) yibocat 2024 All Rights Reserved
 #  Python: 3.10.9
-#  Date: 2023/11/27 下午7:49
+#  Date: 2024/4/6 下午3:12
 #  Author: yibow
 #  Email: yibocat@yeah.net
 #  Software: MohuPy
-from .nums import Fuzznum
-from .array import Fuzzarray
-from .attributes import report, string
+
+from .fuzznums import Fuzznum
+from .fuzzarray import Fuzzarray
+from .attribute import report, string
 from .operation import (add, sub, mul, div,
                         pow, equal, inequal,
                         lt, gt, le, ge, matmul, getitem)
 
 Fuzznum.__repr__ = report
 Fuzznum.__str__ = string
 Fuzznum.__add__ = add
```

### Comparing `MohuPy-0.2.7/mohupy/core/regedit.py` & `MohuPy-0.2.8/mohupy/core/regedit.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
-#  Copyright (c) yibocat 2023 All Rights Reserved
+#  Copyright (c) yibocat 2024 All Rights Reserved
 #  Python: 3.10.9
-#  Date: 2023/11/27 下午7:01
+#  Date: 2024/4/6 下午2:35
 #  Author: yibow
 #  Email: yibocat@yeah.net
 #  Software: MohuPy
+
 from collections.abc import MutableMapping
 
 
 class Registry(MutableMapping):
     __slots__ = "__dict"
 
     def __init__(self, *args, **kwargs):
@@ -56,8 +57,8 @@
     def keys(self):
         return self.__dict.keys()
 
     def values(self):
         return self.__dict.values()
 
     def items(self):
-        return self.__dict.items()
+        return self.__dict.items()
```

### Comparing `MohuPy-0.2.7/mohupy/function/func.py` & `MohuPy-0.2.8/mohupy/function/func.py`

 * *Files identical despite different names*

### Comparing `MohuPy-0.2.7/mohupy/function/mem_func.py` & `MohuPy-0.2.8/mohupy/function/mem_func.py`

 * *Files identical despite different names*

### Comparing `MohuPy-0.2.7/mohupy/lib/__init__.py` & `MohuPy-0.2.8/mohupy/lib/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,25 +17,25 @@
 
 from .construct import (zeros, poss, negs, full,
                         zeros_like, poss_like, negs_like, full_like)
 from .io import savez, loadz, to_csv, load_csv
 from .string import str2fuzz
 from .measure import distance
 from .plotlib import plot
-from .other import random_split, plot_stats, show_decision_mat
+from .other import rsplit, plot_stats, show_decision_mat
 from .utils import isscalar, func4fuzz, asfuzzyarray, absolute, relu
 
 __all__ += ['zeros', 'poss', 'negs', 'full',
             'zeros_like', 'poss_like',
             'negs_like', 'full_like',
             'savez', 'loadz',
             'to_csv', 'load_csv', 'str2fuzz',
             'distance',
             'plot',
-            'random_split',
+            'rsplit',
             'plot_stats',
             'show_decision_mat',
             'isscalar',
             'func4fuzz',
             'asfuzzyarray',
             'absolute',
             'relu']
```

### Comparing `MohuPy-0.2.7/mohupy/lib/construct.py` & `MohuPy-0.2.8/mohupy/lib/construct.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 #  Copyright (c) yibocat 2023 All Rights Reserved
 #  Python: 3.10.9
 #  Date: 2023/11/28 下午4:25
 #  Author: yibow
 #  Email: yibocat@yeah.net
 #  Software: MohuPy
+from typing import Union
+
 import numpy as np
 
 from ..core import Fuzznum, Fuzzarray
 from ..regedit.construct import fuzzZeros, fuzzPoss, fuzzNegs, fuzzZero, fuzzPos, fuzzNeg
 from .base import Library
 
 
@@ -30,15 +32,15 @@
         """
         if len(n) != 0:
             return fuzzZeros[mtype](q, *n)
         else:
             return fuzzZero[mtype](q)
 
 
-def zeros(q, mtype, *n):
+def zeros(q, mtype, *n) -> Union[Fuzznum, Fuzzarray]:
     return Zeros()(q, mtype, *n)
 
 
 class Poss(Library):
     def function(self, q, mtype, *n):
         """
         Generate an *n all-positive fuzzy set
@@ -57,15 +59,15 @@
         """
         if len(n) != 0:
             return fuzzPoss[mtype](q, *n)
         else:
             return fuzzPos[mtype](q)
 
 
-def poss(q, mtype, *n):
+def poss(q, mtype, *n) -> Union[Fuzznum, Fuzzarray]:
     return Poss()(q, mtype, *n)
 
 
 class Negs(Library):
     def function(self, q, mtype, *n):
         """
         Generate an *n all-negative fuzzy set
@@ -84,15 +86,15 @@
         """
         if len(n) != 0:
             return fuzzNegs[mtype](q, *n)
         else:
             return fuzzNeg[mtype](q)
 
 
-def negs(q, mtype, *n):
+def negs(q, mtype, *n) -> Union[Fuzznum, Fuzzarray]:
     return Negs()(q, mtype, *n)
 
 
 class Full(Library):
     def function(self, x: Fuzznum, *n):
         """
         Generate an *n any fuzzy number fuzzy set
@@ -109,57 +111,57 @@
         """
         s = np.full(n, x, dtype=object)
         newset = Fuzzarray(x.qrung, x.mtype)
         newset.array = s
         return newset
 
 
-def full(x: Fuzznum, *n):
+def full(x: Fuzznum, *n) -> Union[Fuzznum, Fuzzarray]:
     return Full()(x, *n)
 
 
 class ZerosLike(Library):
     """
         Constructing full zeros fuzzy arrays of the same shape
     """
     def function(self, f: Fuzzarray):
         return zeros(f.qrung, f.mtype, *f.shape)
 
 
-def zeros_like(f: Fuzzarray):
+def zeros_like(f: Fuzzarray) -> Union[Fuzznum, Fuzzarray]:
     return ZerosLike()(f)
 
 
 class PossLike(Library):
     """
         Constructing full zeros fuzzy arrays of the same shape
     """
     def function(self, f: Fuzzarray):
         return poss(f.qrung, f.mtype, *f.shape)
 
 
-def poss_like(f: Fuzzarray):
+def poss_like(f: Fuzzarray) -> Union[Fuzznum, Fuzzarray]:
     return PossLike()(f)
 
 
 class NegsLike(Library):
     """
         Constructing full zeros fuzzy arrays of the same shape
     """
     def function(self, f: Fuzzarray):
         return negs(f.qrung, f.mtype, *f.shape)
 
 
-def negs_like(f: Fuzzarray):
+def negs_like(f: Fuzzarray) -> Union[Fuzznum, Fuzzarray]:
     return NegsLike()(f)
 
 
 class FullLike(Library):
     """
         Constructing full zeros fuzzy arrays of the same shape
     """
     def function(self, f: Fuzzarray, x: Fuzznum):
         return full(x, *f.shape)
 
 
-def full_like(f: Fuzzarray):
+def full_like(f: Fuzzarray) -> Union[Fuzznum, Fuzzarray]:
     return FullLike()(f)
```

### Comparing `MohuPy-0.2.7/mohupy/lib/io.py` & `MohuPy-0.2.8/mohupy/lib/io.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,16 +5,15 @@
 #  Email: yibocat@yeah.net
 #  Software: MohuPy
 import warnings
 
 import numpy as np
 import pandas as pd
 
-from ..core.nums import Fuzznum
-from ..core.array import Fuzzarray
+from ..core import Fuzznum, Fuzzarray
 
 from .base import Library
 
 
 class Savez(Library):
     """
         Save data to npz file
@@ -47,29 +46,27 @@
 
     def function(self, x, path):
         # from ..base.nums import Fuzznum
         # from ..base.array import Fuzzarray
         if isinstance(x, Fuzznum):
             raise IOError(f'Invalid load for {type(x)}.')
         if isinstance(x, Fuzzarray):
-            if x.isInitial():
+            if x.initial():
                 new = np.load(path, allow_pickle=True)
                 x.qrung = new['qrung']
                 x.mtype = new['mtype']
                 x.array = new['array']
-                return True
             else:
                 warnings.warn('Loading existing data will overwrite the original data!', Warning)
                 x = x.clear()
                 new = np.load(path, allow_pickle=True)
                 x.qrung = new['qrung']
                 x.mtype = new['mtype']
                 x.array = new['array']
-                return True
-        return False
+        raise IOError(f'Invalid load for {type(x)}.')
 
 
 def loadz(x, path):
     return Loadz()(x, path)
 
 
 class ToCSV(Library):
@@ -98,18 +95,16 @@
         self.header = header
         self.index_col = index_col
 
     def function(self, f: Fuzzarray, path: str, float_format: int):
         if 0 <= f.ndim <= 2:
             try:
                 pd.DataFrame(f.array, columns=self.header, index=self.index_col).to_csv(path, float_format=f'%.{float_format}f')
-                return True
             except Exception as e:
                 print(f'{e}: Save failed.')
-                return False
         else:
             raise ValueError(f'The ndim of fuzzy array is invalid: ndim={f.ndim}')
 
 
 def to_csv(x: Fuzzarray, path: str, header=None, index_col=None, float_format=5):
     return ToCSV(header, index_col)(x, path, float_format)
 
@@ -157,10 +152,10 @@
             newset = Fuzzarray(q, mtype)
             newset.array = f
             return newset
         except Exception as e:
             print(f'{e}: Load failed.')
 
 
-def load_csv(path: str, q: int, mtype: str, header='infer', index_col=0):
+def load_csv(path: str, q: int, mtype: str, header='infer', index_col=0) -> Fuzzarray:
     return LoadCSV(header, index_col)(path, q, mtype)
```

### Comparing `MohuPy-0.2.7/mohupy/lib/measure.py` & `MohuPy-0.2.8/mohupy/lib/measure.py`

 * *Files identical despite different names*

### Comparing `MohuPy-0.2.7/mohupy/lib/other.py` & `MohuPy-0.2.8/mohupy/lib/other.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
     ax2 = fig.add_subplot(2, 1, 2)  # 创建子图2
     s.hist(bins=30, alpha=0.5, ax=ax2)
     s.plot(kind='kde', secondary_y=True, ax=ax2)
     plt.grid()
 
 
-def random_split(data, l):
+def rsplit(data, l):
     """
         Randomly split a dataset into two datasets proportionally.
         Parameters
         ----------
             data : pandas.DataFrame
                 Input data.
             l : float
```

### Comparing `MohuPy-0.2.7/mohupy/lib/plotlib.py` & `MohuPy-0.2.8/mohupy/lib/plotlib.py`

 * *Files identical despite different names*

### Comparing `MohuPy-0.2.7/mohupy/lib/utils.py` & `MohuPy-0.2.8/mohupy/lib/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #  Copyright (c) yibocat 2023 All Rights Reserved
 #  Python: 3.10.9
 #  Date: 2023/11/28 下午7:49
 #  Author: yibow
 #  Email: yibocat@yeah.net
 #  Software: MohuPy
 import warnings
+from typing import Union
 
 import numpy as np
 
 from .base import Library
 from ..core import Fuzznum, Fuzzarray
 
 
@@ -17,15 +18,15 @@
         if isinstance(x, Fuzznum):
             return True
         if isinstance(x, Fuzzarray):
             return False
         raise TypeError(f'Unsupported type: {type(x)}')
 
 
-def isscalar(x):
+def isscalar(x) -> bool:
     return Isscalar()(x)
 
 
 class FuncForFuzz(Library):
     def function(self, x, func, *args):
         """
             Apply a function to a fuzzy set.
@@ -52,15 +53,15 @@
         if isinstance(x, Fuzzarray):
             vec_func = np.vectorize(func)
             newset = Fuzzarray(x.qrung, x.mtype)
             newset.array = vec_func(x, *args)
             return newset
 
 
-def func4fuzz(x, func, *args):
+def func4fuzz(x, func, *args) -> Union[Fuzznum, Fuzzarray]:
     return FuncForFuzz()(x, func, *args)
 
 
 class AsFuzzarray(Library):
     def function(self, x, copy):
         """
             Convert a fuzzy numpy array to a fuzzy set.
@@ -86,15 +87,15 @@
         r = np.random.choice(flat)
 
         newset = Fuzzarray(r.qrung, r.mtype)
         newset.array = fl
         return newset
 
 
-def asfuzzyarray(x, copy=False):
+def asfuzzyarray(x, copy=False) -> Fuzzarray:
     return AsFuzzarray()(x, copy)
 
 
 # TODO: 有待商榷，该函数暂时以两者个差为返回值。实际上该方法并不合理
 class Absolute(Library):
     def function(self, a, b):
         y = lambda t, s: t - s if t > s else s - t
@@ -117,15 +118,15 @@
             result = vec_func(a.array, b.array)
             newset = Fuzzarray(a.qrung, a.mtype)
             newset.array = result
             return newset
         raise TypeError(f'Unsupported type: {type(a)} or {type(b)}.')
 
 
-def absolute(a, b):
+def absolute(a, b) -> Union[Fuzznum, Fuzzarray]:
     warnings.warn(f'This function calculates the difference between the two fuzzy numbers, but it is not reasonable. '
                   f'It is recommended to use the \'abs()\'.')
     return Absolute()(a, b)
 
 
 class Relu(Library):
     def function(self, x, op):
@@ -150,10 +151,10 @@
             vec_func = np.vectorize(relu)
             newset = Fuzzarray(x.qrung, x.mtype)
             newset.array = vec_func(x.array, op.array)
             return newset
         raise TypeError(f'Unsupported type: {type(x)} or {type(op)}.')
 
 
-def relu(x, op=None):
+def relu(x, op=None) -> Union[Fuzznum, Fuzzarray]:
     return Relu()(x, op)
```

### Comparing `MohuPy-0.2.7/mohupy/math/product.py` & `MohuPy-0.2.8/mohupy/math/product.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 #  Copyright (c) yibocat 2023 All Rights Reserved
 #  Python: 3.10.9
 #  Date: 2023/11/29 下午3:47
 #  Author: yibow
 #  Email: yibocat@yeah.net
 #  Software: MohuPy
+from typing import Union
 
 import numpy as np
 
 from .base import Mathematics
 from ..core import Fuzznum, Fuzzarray
 
 
@@ -55,15 +56,15 @@
                 newset = Fuzzarray(x.qrung, x.mtype)
                 result = np.dot(x.array, y.array)
                 newset.array = result
                 return newset
         raise ValueError(f'Invalid input type {type(x)} and {type(y)}')
 
 
-def dot(x, y):
+def dot(x, y) -> Union[Fuzznum, Fuzzarray]:
     return Dot()(x, y)
 
 
 class Inner(Mathematics):
     def function(self, x, y):
         """
             Returns the inner product of two Fuzzarray.
@@ -107,15 +108,15 @@
                 newset = Fuzzarray(x.qrung, x.mtype)
                 result = np.inner(x.array, y.array)
                 newset.array = result
                 return newset
         raise ValueError(f'Invalid input type {type(x)} and {type(y)}')
 
 
-def inner(x, y):
+def inner(x, y) -> Union[Fuzznum, Fuzzarray]:
     return Inner()(x, y)
 
 
 class Outer(Mathematics):
     def function(self, x, y):
         """
             Returns the outer product of two Fuzzarray.
@@ -153,15 +154,15 @@
             newset = Fuzzarray(x.qrung, x.mtype)
             result = np.outer(x.array, y.array)
             newset.array = result
             return newset
         raise ValueError(f'Invalid input type {type(x)} and {type(y)}')
 
 
-def outer(x, y):
+def outer(x, y) -> Union[Fuzznum, Fuzzarray]:
     return Outer()(x, y)
 
 
 class Cartadd(Mathematics):
     def function(self, x, y):
         """
             Returns the cartesian sum of two Fuzzarray.
@@ -212,15 +213,15 @@
                 return np.add.outer(x.array, y.array)
             else:
                 newset = Fuzzarray(x.qrung, x.mtype)
                 newset.array = np.add.outer(x.array, y.array)
                 return newset
 
 
-def cartadd(x, y):
+def cartadd(x, y) -> Union[Fuzznum, Fuzzarray]:
     return Cartadd()(x, y)
 
 
 class Cartprod(Mathematics):
     def function(self, x, y):
         """
             Returns the cartesian product of two Fuzzarray.
@@ -251,9 +252,9 @@
             return newset
         if isinstance(x, Fuzzarray) and isinstance(y, Fuzzarray):
             newset = Fuzzarray(x.qrung, x.mtype)
             newset.array = np.asarray(np.meshgrid(x.array, y.array))
             return newset
 
 
-def cartprod(x, y):
+def cartprod(x, y) -> Union[Fuzznum, Fuzzarray]:
     return Cartprod()(x, y)
```

### Comparing `MohuPy-0.2.7/mohupy/measure/__init__.py` & `MohuPy-0.2.8/mohupy/measure/__init__.py`

 * *Files identical despite different names*

### Comparing `MohuPy-0.2.7/mohupy/measure/fuzzmeas.py` & `MohuPy-0.2.8/mohupy/measure/fuzzmeas.py`

 * *Files identical despite different names*

### Comparing `MohuPy-0.2.7/mohupy/measure/hasse.py` & `MohuPy-0.2.8/mohupy/measure/hasse.py`

 * *Files identical despite different names*

### Comparing `MohuPy-0.2.7/mohupy/measure/indices.py` & `MohuPy-0.2.8/mohupy/measure/indices.py`

 * *Files identical despite different names*

### Comparing `MohuPy-0.2.7/mohupy/measure/integral.py` & `MohuPy-0.2.8/mohupy/measure/integral.py`

 * *Files identical despite different names*

### Comparing `MohuPy-0.2.7/mohupy/measure/utils.py` & `MohuPy-0.2.8/mohupy/measure/utils.py`

 * *Files identical despite different names*

### Comparing `MohuPy-0.2.7/mohupy/random/rand.py` & `MohuPy-0.2.8/mohupy/random/rand.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 #  Copyright (c) yibocat 2023 All Rights Reserved
 #  Python: 3.10.9
 #  Date: 2023/10/16 下午8:22
 #  Author: yibow
 #  Email: yibocat@yeah.net
 #  Software: MohuPy
-from typing import Union
-
-from .base import Random
 
 import numpy as np
 
+from typing import Union
+
+from .base import Random
 from ..core import Fuzzarray, Fuzznum
 
 
 class RandNum(Random):
 
     def __init__(self, minnum, maxnum):
         self.minnum = minnum
@@ -111,15 +111,15 @@
         """
         if len(n) == 0:
             return randnum(q, mtype, minnum=self.minnum, maxnum=self.maxnum)
         else:
             return randset(q, mtype, *n, minnum=self.minnum, maxnum=self.maxnum)
 
 
-def rand(q: int, mtype: str, *n, minnum=1, maxnum=5) -> Union[Fuzzarray, Fuzznum]:
+def rand(q: int, mtype: str = 'qrofn', *n, minnum=1, maxnum=5) -> Union[Fuzzarray, Fuzznum]:
     return Rand(minnum, maxnum)(q, mtype, *n)
 
 
 class Choice(Random):
     def function(self, f, n, replace):
         """
             Randomly select a fuzzy number
```

### Comparing `MohuPy-0.2.7/mohupy/regedit/__init__.py` & `MohuPy-0.2.8/mohupy/regedit/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -22,22 +22,22 @@
     'fuzzNeg',
     'fuzzDis',
     'fuzzString',
     'fuzzRandom',
     'fuzzPlot',
 ]
 
-### Archimedean Norms Dictionary(AND)
-archimedeanDict = dict()
-__all__ += ['archimedeanDict']
-
-
-### Add algebraic norms to AND
-from .algebraic_operation import algebAdd, algebSub, algebMul, algebDiv, algebPow, algebTim
-archimedeanDict['algebraic'] = {'add': algebAdd,
-                                'sub': algebSub,
-                                'mul': algebMul,
-                                'div': algebDiv,
-                                'pow': algebPow,
-                                'tim': algebTim}
+# ### Archimedean Norms Dictionary(AND)
+# archimedeanDict = dict()
+# __all__ += ['archimedeanDict']
+#
+#
+# ### Add algebraic norms to AND
+# from .algebraic_operation import algebAdd, algebSub, algebMul, algebDiv, algebPow, algebTim
+# archimedeanDict['algebraic'] = {'add': algebAdd,
+#                                 'sub': algebSub,
+#                                 'mul': algebMul,
+#                                 'div': algebDiv,
+#                                 'pow': algebPow,
+#                                 'tim': algebTim}
```

### Comparing `MohuPy-0.2.7/mohupy/regedit/algebraic_operation.py` & `MohuPy-0.2.8/mohupy/core/operationLib/algebraicoperation.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-#  Copyright (c) yibocat 2023 All Rights Reserved
+#  Copyright (c) yibocat 2024 All Rights Reserved
 #  Python: 3.10.9
-#  Date: 2023/11/29 下午2:37
+#  Date: 2024/4/6 下午2:49
 #  Author: yibow
 #  Email: yibocat@yeah.net
 #  Software: MohuPy
 
 import warnings
 
 import numpy as np
-from ..src.algebraic import (algebraic_add, algebraic_sub,
-                             algebraic_mul, algebraic_div,
-                             algebraic_pow, algebraic_times)
 
-from ..core.regedit import Registry
+from .algebraic import (algebraic_add,algebraic_sub,algebraic_mul,
+                        algebraic_div,algebraic_pow,algebraic_times)
+
+from ..regedit import Registry
 
 algebAdd = Registry()
 algebSub = Registry()
 algebMul = Registry()
 algebDiv = Registry()
 algebPow = Registry()
 algebTim = Registry()
```

### Comparing `MohuPy-0.2.7/mohupy/regedit/construct.py` & `MohuPy-0.2.8/mohupy/regedit/construct.py`

 * *Files identical despite different names*

### Comparing `MohuPy-0.2.7/mohupy/regedit/distance.py` & `MohuPy-0.2.8/mohupy/regedit/distance.py`

 * *Files identical despite different names*

### Comparing `MohuPy-0.2.7/mohupy/regedit/plotlib.py` & `MohuPy-0.2.8/mohupy/regedit/plotlib.py`

 * *Files identical despite different names*

### Comparing `MohuPy-0.2.7/mohupy/regedit/random.py` & `MohuPy-0.2.8/mohupy/regedit/random.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #  Copyright (c) yibocat 2023 All Rights Reserved
 #  Python: 3.10.9
 #  Date: 2023/11/28 下午3:12
 #  Author: yibow
 #  Email: yibocat@yeah.net
 #  Software: MohuPy
 import numpy as np
+np.set_printoptions(suppress=True)
 
 from ..core.regedit import Registry
 from ..constant import Approx
 
 fuzzRandom = Registry()
 
 
@@ -31,15 +32,15 @@
             Fuzznum
     """
     from ..core import fuzznum
     newfn = fuzznum(q, 0., 0.)
     while True:
         newfn.md = np.round(np.random.rand(), Approx.round)
         newfn.nmd = np.round(np.random.rand(), Approx.round)
-        if newfn.isValid():
+        if newfn.valid():
             break
     return newfn
 
 
 @fuzzRandom('ivfn')
 def random_ivfn(q, minnum=None, maxnum=None):
     """
@@ -59,15 +60,15 @@
             fuzznum
     """
     from ..core import fuzznum
     newfn = fuzznum(q, (0., 0.), (0., 0.))
     while True:
         newfn.md = np.round(np.asarray([np.random.rand(), np.random.rand()]), Approx.round)
         newfn.nmd = np.round(np.asarray([np.random.rand(), np.random.rand()]), Approx.round)
-        if newfn.isValid():
+        if newfn.valid():
             break
     return newfn
 
 
 @fuzzRandom('qrohfn')
 def random_qrohfn(q, minnum, maxnum):
     """
@@ -88,11 +89,11 @@
     from ..core import fuzznum
     newfn = fuzznum(q, [], [])
     newfn.md = np.round(np.random.rand(np.random.randint(minnum, maxnum)), Approx.round)
     newfn.nmd = np.round(np.random.rand(np.random.randint(minnum, maxnum)), Approx.round)
     while True:
         newfn.md = np.round(np.random.rand(np.random.randint(minnum, maxnum)), Approx.round)
         newfn.nmd = np.round(np.random.rand(np.random.randint(minnum, maxnum)), Approx.round)
-        if newfn.isValid():
+        if newfn.valid():
             break
     return newfn
```

### Comparing `MohuPy-0.2.7/mohupy/regedit/str2num.py` & `MohuPy-0.2.8/mohupy/regedit/str2num.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     assert len(t) == 1, \
         'data format error.'
     x = re.findall(r'\d.?\d*', t[0])
     assert len(x) == 2, \
         'data format error.'
     newfn.md = float(x[0])
     newfn.nmd = float(x[1])
-    assert newfn.isValid(), f'data format is correct, but the data is invalid: {s}'
+    assert newfn.valid(), f'data format is correct, but the data is invalid: {s}'
     return newfn
 
 
 @fuzzString('ivfn')
 def str2ivfn(s: str, q) -> Fuzznum:
     from ..core import fuzznum
     newfn = fuzznum(q, (0., 0.), (0., 0.))
@@ -56,15 +56,15 @@
     assert len(md) == 2 and len(nmd) == 2, \
         'data format error.'
 
     m = [float(md[0]), float(md[1])]
     n = [float(nmd[0]), float(nmd[1])]
     newfn.md = m
     newfn.nmd = n
-    assert newfn.isValid(), f'data format is correct, but the data is invalid: {s}'
+    assert newfn.valid(), f'data format is correct, but the data is invalid: {s}'
     return newfn
 
 
 @fuzzString('qrohfn')
 def str2qrohfn(s: str, q) -> Fuzznum:
     """
         Convert input data to Q-rung orthopair hesitant fuzzy element.
@@ -93,10 +93,10 @@
     nmd = re.findall(r'\d.?\d*', t2[1])
 
     for i in range(len(md)):
         newfn.md = np.append(newfn.md, np.float_(md[i]))
     for j in range(len(nmd)):
         newfn.nmd = np.append(newfn.nmd, np.float_(nmd[j]))
 
-    assert newfn.isValid(), f'data format is correct, but the data is invalid: {s}'
+    assert newfn.valid(), f'data format is correct, but the data is invalid: {s}'
     return newfn
```

### Comparing `MohuPy-0.2.7/mohupy/runtime.py` & `MohuPy-0.2.8/mohupy/runtime.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 # Initialize fuzzy parent class, also indicates the currently used fuzzy number type
 # It is worth noting: fuzzyParent is a dictionary whose keys represent parent classes
 # and values represent subclasses.
 # fuzzParent = mohuParent.memo
 
 from .regedit import *
-from .core import FuzzType
+from .core import FuzzType, archimedeanDict
 
 
 class info:
     type = FuzzType
     archDict = archimedeanDict
 
     zeros = fuzzZeros
```

### Comparing `MohuPy-0.2.7/mohupy/src/algebraic.py` & `MohuPy-0.2.8/mohupy/core/operationLib/algebraic.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,79 +1,19 @@
-#  Copyright (c) yibocat 2023 All Rights Reserved
+#  Copyright (c) yibocat 2024 All Rights Reserved
 #  Python: 3.10.9
-#  Date: 2023/11/29 下午1:49
+#  Date: 2024/4/6 下午2:43
 #  Author: yibow
 #  Email: yibocat@yeah.net
 #  Software: MohuPy
 
 import numpy as np
 
-from .base import Archimedean
-from ..constant import Approx
-
-
-class AlgebT(Archimedean):
-    def function(self, x):
-        return np.log2(x)
-
-
-def algebTao(x):
-    return AlgebT()(x)
-
-
-class AlgebInT(Archimedean):
-    def function(self, x):
-        return 1 / (2 ** x)
-
-
-def algebInTao(x):
-    return AlgebInT()(x)
-
-
-class AlgebS(Archimedean):
-    def function(self, x):
-        return np.log2(1 - x)
-
-
-def algebS(x):
-    return AlgebS()(x)
-
-
-class AlgebInS(Archimedean):
-    def function(self, x):
-        return 1 - 1 / (2 ** x)
-
-
-def algebInS(x):
-    return AlgebInS()(x)
-
-
-class AlgebTNorm(Archimedean):
-    def function(self, x, y):
-        """
-            AlgebInT()((AlgebT()(x) + AlgebT()(y)))
-        """
-        return x * y
-
-
-def algebTNorm(x, y):
-    return AlgebTNorm()(x, y)
-
-
-class AlgebSNorm(Archimedean):
-    def function(self, x, y):
-        """
-            AlgebInS()((AlgebS()(x) + AlgebS()(y)))
-        """
-        return x + y - x * y
-
-
-def algebSNorm(x, y):
-    return AlgebSNorm()(x, y)
+from ..base import Archimedean
 
+from ...constant import Approx
 
 """
 The following is a quick calculation of Algebraic norms in fuzzy number. 
 The code has been used for the calculation of 'Fuzznum' and 'Fuzzarray', 
 so the Archimedean class is no longer used to complete the operation.
 """
 
@@ -162,7 +102,72 @@
     :param x0:  第一个数的隶属度
     :param y0:  第一个数的非隶属度
     :param q:   Q 阶
     """
     md = np.round((1. - (1. - x0 ** q) ** p) ** (1. / q), Approx.round)
     nmd = np.round(y0 ** p, Approx.round)
     return md, nmd
+
+
+"""
+The following is a calculation of Algebraic norms in fuzzy number.
+"""
+
+
+class AlgebT(Archimedean):
+    def function(self, x):
+        return np.log2(x)
+
+
+def algebTao(x):
+    return AlgebT()(x)
+
+
+class AlgebInT(Archimedean):
+    def function(self, x):
+        return 1 / (2 ** x)
+
+
+def algebInTao(x):
+    return AlgebInT()(x)
+
+
+class AlgebS(Archimedean):
+    def function(self, x):
+        return np.log2(1 - x)
+
+
+def algebS(x):
+    return AlgebS()(x)
+
+
+class AlgebInS(Archimedean):
+    def function(self, x):
+        return 1 - 1 / (2 ** x)
+
+
+def algebInS(x):
+    return AlgebInS()(x)
+
+
+class AlgebTNorm(Archimedean):
+    def function(self, x, y):
+        """
+            AlgebInT()((AlgebT()(x) + AlgebT()(y)))
+        """
+        return x * y
+
+
+def algebTNorm(x, y):
+    return AlgebTNorm()(x, y)
+
+
+class AlgebSNorm(Archimedean):
+    def function(self, x, y):
+        """
+            AlgebInS()((AlgebS()(x) + AlgebS()(y)))
+        """
+        return x + y - x * y
+
+
+def algebSNorm(x, y):
+    return AlgebSNorm()(x, y)
```

### Comparing `MohuPy-0.2.7/mohupy/src/einstein.py` & `MohuPy-0.2.8/mohupy/core/operationLib/einstein.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-#  Copyright (c) yibocat 2023 All Rights Reserved
+#  Copyright (c) yibocat 2024 All Rights Reserved
 #  Python: 3.10.9
-#  Date: 2023/11/29 下午2:15
+#  Date: 2024/4/6 下午2:47
 #  Author: yibow
 #  Email: yibocat@yeah.net
 #  Software: MohuPy
-
 import numpy as np
 
-from .base import Archimedean
+from ..base import Archimedean
 
 
 class EinsT(Archimedean):
     def function(self, x):
         return np.log2((2 - x) / x)
```

### Comparing `MohuPy-0.2.7/setup.py` & `MohuPy-0.2.8/setup.py`

 * *Files identical despite different names*

