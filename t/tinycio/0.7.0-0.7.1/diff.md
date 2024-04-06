# Comparing `tmp/tinycio-0.7.0.tar.gz` & `tmp/tinycio-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tinycio-0.7.0.tar", last modified: Sat Apr  6 02:56:51 2024, max compression
+gzip compressed data, was "tinycio-0.7.1.tar", last modified: Sat Apr  6 03:12:45 2024, max compression
```

## Comparing `tinycio-0.7.0.tar` & `tinycio-0.7.1.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxrwxrwx   0        0        0        0 2024-04-06 02:56:51.753777 tinycio-0.7.0/
--rw-rw-rw-   0        0        0     1085 2023-12-13 13:07:04.000000 tinycio-0.7.0/LICENSE.txt
--rw-rw-rw-   0        0        0     1754 2024-04-06 02:56:51.752777 tinycio-0.7.0/PKG-INFO
--rw-rw-rw-   0        0        0     1073 2023-12-22 22:36:31.000000 tinycio-0.7.0/README.md
--rw-rw-rw-   0        0        0     1099 2024-04-06 02:34:50.000000 tinycio-0.7.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-06 02:56:51.753777 tinycio-0.7.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-06 02:56:51.700765 tinycio-0.7.0/src/
-drwxrwxrwx   0        0        0        0 2024-04-06 02:56:51.719770 tinycio-0.7.0/src/tinycio/
--rw-rw-rw-   0        0        0      333 2023-12-20 19:54:11.000000 tinycio-0.7.0/src/tinycio/__init__.py
--rw-rw-rw-   0        0        0    12098 2024-01-28 19:40:42.000000 tinycio-0.7.0/src/tinycio/balance.py
--rw-rw-rw-   0        0        0     2946 2023-12-25 07:42:00.000000 tinycio-0.7.0/src/tinycio/codec.py
--rw-rw-rw-   0        0        0    51797 2024-04-06 01:37:04.000000 tinycio-0.7.0/src/tinycio/colorspace.py
--rw-rw-rw-   0        0        0    32181 2024-01-28 19:41:54.000000 tinycio-0.7.0/src/tinycio/correction.py
-drwxrwxrwx   0        0        0        0 2024-04-06 02:56:51.735773 tinycio-0.7.0/src/tinycio/fsio/
--rw-rw-rw-   0        0        0      191 2023-12-07 20:04:01.000000 tinycio-0.7.0/src/tinycio/fsio/__init__.py
--rw-rw-rw-   0        0        0     1987 2024-01-13 15:11:35.000000 tinycio-0.7.0/src/tinycio/fsio/format.py
--rw-rw-rw-   0        0        0     5424 2023-12-25 07:40:28.000000 tinycio-0.7.0/src/tinycio/fsio/imagefile.py
--rw-rw-rw-   0        0        0     3314 2023-12-25 07:40:39.000000 tinycio-0.7.0/src/tinycio/fsio/lutfile.py
--rw-rw-rw-   0        0        0      102 2023-12-14 19:20:02.000000 tinycio-0.7.0/src/tinycio/globals.py
--rw-rw-rw-   0        0        0     2215 2023-12-15 20:51:38.000000 tinycio-0.7.0/src/tinycio/loss.py
--rw-rw-rw-   0        0        0     9904 2023-12-25 07:42:04.000000 tinycio-0.7.0/src/tinycio/lut.py
-drwxrwxrwx   0        0        0        0 2024-04-06 02:56:51.736774 tinycio-0.7.0/src/tinycio/np_agx/
--rw-rw-rw-   0        0        0    11064 2023-12-11 19:03:49.000000 tinycio-0.7.0/src/tinycio/np_agx/agx.py
-drwxrwxrwx   0        0        0        0 2024-04-06 02:56:51.739774 tinycio-0.7.0/src/tinycio/numerics/
--rw-rw-rw-   0        0        0     1969 2023-12-25 07:39:27.000000 tinycio-0.7.0/src/tinycio/numerics/__init__.py
--rw-rw-rw-   0        0        0     3044 2023-12-15 12:09:46.000000 tinycio-0.7.0/src/tinycio/numerics/linalg.py
--rw-rw-rw-   0        0        0      482 2023-12-13 15:27:22.000000 tinycio-0.7.0/src/tinycio/numerics/util_pt.py
--rw-rw-rw-   0        0        0      964 2023-12-13 15:27:27.000000 tinycio-0.7.0/src/tinycio/numerics/util_py.py
--rw-rw-rw-   0        0        0   166640 2023-12-20 20:22:45.000000 tinycio-0.7.0/src/tinycio/numerics/vector.py
-drwxrwxrwx   0        0        0        0 2024-04-06 02:56:51.743775 tinycio-0.7.0/src/tinycio/scripts/
--rw-rw-rw-   0        0        0        0 2023-12-20 20:22:45.000000 tinycio-0.7.0/src/tinycio/scripts/__init__.py
--rw-rw-rw-   0        0        0     4731 2024-04-06 02:34:14.000000 tinycio-0.7.0/src/tinycio/scripts/color2color.py
--rw-rw-rw-   0        0        0     2694 2023-12-20 20:22:45.000000 tinycio-0.7.0/src/tinycio/scripts/hdr_codec.py
--rw-rw-rw-   0        0        0     4835 2023-12-20 20:22:45.000000 tinycio-0.7.0/src/tinycio/scripts/img2cube.py
--rw-rw-rw-   0        0        0      215 2023-12-20 20:22:45.000000 tinycio-0.7.0/src/tinycio/scripts/post_install.py
--rw-rw-rw-   0        0        0     4073 2023-12-20 23:13:42.000000 tinycio-0.7.0/src/tinycio/scripts/white_balance.py
--rw-rw-rw-   0        0        0     7087 2024-03-28 10:51:54.000000 tinycio-0.7.0/src/tinycio/spectral.py
--rw-rw-rw-   0        0        0     6612 2024-04-06 01:32:15.000000 tinycio-0.7.0/src/tinycio/tonemapping.py
--rw-rw-rw-   0        0        0    31442 2024-04-06 02:52:18.000000 tinycio-0.7.0/src/tinycio/usertypes.py
-drwxrwxrwx   0        0        0        0 2024-04-06 02:56:51.745776 tinycio-0.7.0/src/tinycio/util/
--rw-rw-rw-   0        0        0      334 2023-12-14 19:18:41.000000 tinycio-0.7.0/src/tinycio/util/__init__.py
--rw-rw-rw-   0        0        0    17822 2023-12-14 18:35:05.000000 tinycio-0.7.0/src/tinycio/util/colorutil.py
--rw-rw-rw-   0        0        0     3065 2023-12-14 19:21:16.000000 tinycio-0.7.0/src/tinycio/util/miscutil.py
-drwxrwxrwx   0        0        0        0 2024-04-06 02:56:51.752777 tinycio-0.7.0/src/tinycio.egg-info/
--rw-rw-rw-   0        0        0     1754 2024-04-06 02:56:51.000000 tinycio-0.7.0/src/tinycio.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1242 2024-04-06 02:56:51.000000 tinycio-0.7.0/src/tinycio.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-06 02:56:51.000000 tinycio-0.7.0/src/tinycio.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      287 2024-04-06 02:56:51.000000 tinycio-0.7.0/src/tinycio.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       47 2024-04-06 02:56:51.000000 tinycio-0.7.0/src/tinycio.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-06 02:56:51.000000 tinycio-0.7.0/src/tinycio.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-06 02:56:51.751777 tinycio-0.7.0/tests/
--rw-rw-rw-   0        0        0     1577 2023-12-25 06:28:22.000000 tinycio-0.7.0/tests/test_cc_load_save.py
--rw-rw-rw-   0        0        0     2675 2023-12-15 14:14:45.000000 tinycio-0.7.0/tests/test_codec.py
--rw-rw-rw-   0        0        0    14512 2024-01-01 03:02:31.000000 tinycio-0.7.0/tests/test_colorspace.py
--rw-rw-rw-   0        0        0    20740 2023-12-25 06:46:05.000000 tinycio-0.7.0/tests/test_numerics.py
--rw-rw-rw-   0        0        0     1400 2024-04-06 01:54:00.000000 tinycio-0.7.0/tests/test_tonemapping.py
--rw-rw-rw-   0        0        0     7075 2023-12-25 06:48:29.000000 tinycio-0.7.0/tests/test_tutorial.py
+drwxrwxrwx   0        0        0        0 2024-04-06 03:12:45.151880 tinycio-0.7.1/
+-rw-rw-rw-   0        0        0     1085 2023-12-13 13:07:04.000000 tinycio-0.7.1/LICENSE.txt
+-rw-rw-rw-   0        0        0     1754 2024-04-06 03:12:45.150880 tinycio-0.7.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1073 2023-12-22 22:36:31.000000 tinycio-0.7.1/README.md
+-rw-rw-rw-   0        0        0     1099 2024-04-06 03:08:59.000000 tinycio-0.7.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-06 03:12:45.151880 tinycio-0.7.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-06 03:12:45.079697 tinycio-0.7.1/src/
+drwxrwxrwx   0        0        0        0 2024-04-06 03:12:45.107867 tinycio-0.7.1/src/tinycio/
+-rw-rw-rw-   0        0        0      333 2023-12-20 19:54:11.000000 tinycio-0.7.1/src/tinycio/__init__.py
+-rw-rw-rw-   0        0        0    12098 2024-01-28 19:40:42.000000 tinycio-0.7.1/src/tinycio/balance.py
+-rw-rw-rw-   0        0        0     2946 2023-12-25 07:42:00.000000 tinycio-0.7.1/src/tinycio/codec.py
+-rw-rw-rw-   0        0        0    51797 2024-04-06 01:37:04.000000 tinycio-0.7.1/src/tinycio/colorspace.py
+-rw-rw-rw-   0        0        0    32181 2024-01-28 19:41:54.000000 tinycio-0.7.1/src/tinycio/correction.py
+drwxrwxrwx   0        0        0        0 2024-04-06 03:12:45.132874 tinycio-0.7.1/src/tinycio/fsio/
+-rw-rw-rw-   0        0        0      191 2023-12-07 20:04:01.000000 tinycio-0.7.1/src/tinycio/fsio/__init__.py
+-rw-rw-rw-   0        0        0     1987 2024-01-13 15:11:35.000000 tinycio-0.7.1/src/tinycio/fsio/format.py
+-rw-rw-rw-   0        0        0     5424 2023-12-25 07:40:28.000000 tinycio-0.7.1/src/tinycio/fsio/imagefile.py
+-rw-rw-rw-   0        0        0     3314 2023-12-25 07:40:39.000000 tinycio-0.7.1/src/tinycio/fsio/lutfile.py
+-rw-rw-rw-   0        0        0      102 2023-12-14 19:20:02.000000 tinycio-0.7.1/src/tinycio/globals.py
+-rw-rw-rw-   0        0        0     2215 2023-12-15 20:51:38.000000 tinycio-0.7.1/src/tinycio/loss.py
+-rw-rw-rw-   0        0        0     9904 2023-12-25 07:42:04.000000 tinycio-0.7.1/src/tinycio/lut.py
+drwxrwxrwx   0        0        0        0 2024-04-06 03:12:45.133876 tinycio-0.7.1/src/tinycio/np_agx/
+-rw-rw-rw-   0        0        0    11064 2023-12-11 19:03:49.000000 tinycio-0.7.1/src/tinycio/np_agx/agx.py
+drwxrwxrwx   0        0        0        0 2024-04-06 03:12:45.136877 tinycio-0.7.1/src/tinycio/numerics/
+-rw-rw-rw-   0        0        0     1969 2023-12-25 07:39:27.000000 tinycio-0.7.1/src/tinycio/numerics/__init__.py
+-rw-rw-rw-   0        0        0     3044 2023-12-15 12:09:46.000000 tinycio-0.7.1/src/tinycio/numerics/linalg.py
+-rw-rw-rw-   0        0        0      482 2023-12-13 15:27:22.000000 tinycio-0.7.1/src/tinycio/numerics/util_pt.py
+-rw-rw-rw-   0        0        0      964 2023-12-13 15:27:27.000000 tinycio-0.7.1/src/tinycio/numerics/util_py.py
+-rw-rw-rw-   0        0        0   166640 2023-12-20 20:22:45.000000 tinycio-0.7.1/src/tinycio/numerics/vector.py
+drwxrwxrwx   0        0        0        0 2024-04-06 03:12:45.140878 tinycio-0.7.1/src/tinycio/scripts/
+-rw-rw-rw-   0        0        0        0 2023-12-20 20:22:45.000000 tinycio-0.7.1/src/tinycio/scripts/__init__.py
+-rw-rw-rw-   0        0        0     4731 2024-04-06 02:34:14.000000 tinycio-0.7.1/src/tinycio/scripts/color2color.py
+-rw-rw-rw-   0        0        0     2694 2023-12-20 20:22:45.000000 tinycio-0.7.1/src/tinycio/scripts/hdr_codec.py
+-rw-rw-rw-   0        0        0     4835 2023-12-20 20:22:45.000000 tinycio-0.7.1/src/tinycio/scripts/img2cube.py
+-rw-rw-rw-   0        0        0      215 2023-12-20 20:22:45.000000 tinycio-0.7.1/src/tinycio/scripts/post_install.py
+-rw-rw-rw-   0        0        0     4073 2023-12-20 23:13:42.000000 tinycio-0.7.1/src/tinycio/scripts/white_balance.py
+-rw-rw-rw-   0        0        0     7087 2024-03-28 10:51:54.000000 tinycio-0.7.1/src/tinycio/spectral.py
+-rw-rw-rw-   0        0        0     6612 2024-04-06 01:32:15.000000 tinycio-0.7.1/src/tinycio/tonemapping.py
+-rw-rw-rw-   0        0        0    31442 2024-04-06 02:52:18.000000 tinycio-0.7.1/src/tinycio/usertypes.py
+drwxrwxrwx   0        0        0        0 2024-04-06 03:12:45.144878 tinycio-0.7.1/src/tinycio/util/
+-rw-rw-rw-   0        0        0      334 2023-12-14 19:18:41.000000 tinycio-0.7.1/src/tinycio/util/__init__.py
+-rw-rw-rw-   0        0        0    17822 2023-12-14 18:35:05.000000 tinycio-0.7.1/src/tinycio/util/colorutil.py
+-rw-rw-rw-   0        0        0     3065 2023-12-14 19:21:16.000000 tinycio-0.7.1/src/tinycio/util/miscutil.py
+drwxrwxrwx   0        0        0        0 2024-04-06 03:12:45.150880 tinycio-0.7.1/src/tinycio.egg-info/
+-rw-rw-rw-   0        0        0     1754 2024-04-06 03:12:45.000000 tinycio-0.7.1/src/tinycio.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1242 2024-04-06 03:12:45.000000 tinycio-0.7.1/src/tinycio.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-06 03:12:45.000000 tinycio-0.7.1/src/tinycio.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      287 2024-04-06 03:12:45.000000 tinycio-0.7.1/src/tinycio.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       47 2024-04-06 03:12:45.000000 tinycio-0.7.1/src/tinycio.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-06 03:12:45.000000 tinycio-0.7.1/src/tinycio.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-06 03:12:45.149879 tinycio-0.7.1/tests/
+-rw-rw-rw-   0        0        0     1577 2023-12-25 06:28:22.000000 tinycio-0.7.1/tests/test_cc_load_save.py
+-rw-rw-rw-   0        0        0     2675 2023-12-15 14:14:45.000000 tinycio-0.7.1/tests/test_codec.py
+-rw-rw-rw-   0        0        0    14512 2024-01-01 03:02:31.000000 tinycio-0.7.1/tests/test_colorspace.py
+-rw-rw-rw-   0        0        0    20740 2023-12-25 06:46:05.000000 tinycio-0.7.1/tests/test_numerics.py
+-rw-rw-rw-   0        0        0     1400 2024-04-06 01:54:00.000000 tinycio-0.7.1/tests/test_tonemapping.py
+-rw-rw-rw-   0        0        0     7075 2023-12-25 06:48:29.000000 tinycio-0.7.1/tests/test_tutorial.py
```

### Comparing `tinycio-0.7.0/LICENSE.txt` & `tinycio-0.7.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tinycio-0.7.0/PKG-INFO` & `tinycio-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tinycio
-Version: 0.7.0
+Version: 0.7.1
 Summary: A primitive, lightweight color management framework for PyTorch-involved projects
 Author-email: Sam Izdat <ghsamizdat@gmail.com>
 Project-URL: Homepage, https://sam-izdat.github.io/tinycio-docs
 Project-URL: Issues, https://github.com/Sam-Izdat/tinycio/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `tinycio-0.7.0/README.md` & `tinycio-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `tinycio-0.7.0/pyproject.toml` & `tinycio-0.7.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "tinycio"
-version = "0.7.0"
+version = "0.7.1"
 authors = [
   { name="Sam Izdat", email="ghsamizdat@gmail.com" },
 ]
 description = "A primitive, lightweight color management framework for PyTorch-involved projects"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `tinycio-0.7.0/src/tinycio/balance.py` & `tinycio-0.7.1/src/tinycio/balance.py`

 * *Files identical despite different names*

### Comparing `tinycio-0.7.0/src/tinycio/codec.py` & `tinycio-0.7.1/src/tinycio/codec.py`

 * *Files identical despite different names*

### Comparing `tinycio-0.7.0/src/tinycio/colorspace.py` & `tinycio-0.7.1/src/tinycio/colorspace.py`

 * *Files identical despite different names*

### Comparing `tinycio-0.7.0/src/tinycio/correction.py` & `tinycio-0.7.1/src/tinycio/correction.py`

 * *Files identical despite different names*

### Comparing `tinycio-0.7.0/src/tinycio/fsio/format.py` & `tinycio-0.7.1/src/tinycio/fsio/format.py`

 * *Files identical despite different names*

### Comparing `tinycio-0.7.0/src/tinycio/fsio/imagefile.py` & `tinycio-0.7.1/src/tinycio/fsio/imagefile.py`

 * *Files identical despite different names*

### Comparing `tinycio-0.7.0/src/tinycio/fsio/lutfile.py` & `tinycio-0.7.1/src/tinycio/fsio/lutfile.py`

 * *Files identical despite different names*

### Comparing `tinycio-0.7.0/src/tinycio/loss.py` & `tinycio-0.7.1/src/tinycio/loss.py`

 * *Files identical despite different names*

### Comparing `tinycio-0.7.0/src/tinycio/lut.py` & `tinycio-0.7.1/src/tinycio/lut.py`

 * *Files identical despite different names*

### Comparing `tinycio-0.7.0/src/tinycio/np_agx/agx.py` & `tinycio-0.7.1/src/tinycio/np_agx/agx.py`

 * *Files identical despite different names*

### Comparing `tinycio-0.7.0/src/tinycio/numerics/__init__.py` & `tinycio-0.7.1/src/tinycio/numerics/__init__.py`

 * *Files identical despite different names*

### Comparing `tinycio-0.7.0/src/tinycio/numerics/linalg.py` & `tinycio-0.7.1/src/tinycio/numerics/linalg.py`

 * *Files identical despite different names*

### Comparing `tinycio-0.7.0/src/tinycio/numerics/util_py.py` & `tinycio-0.7.1/src/tinycio/numerics/util_py.py`

 * *Files identical despite different names*

### Comparing `tinycio-0.7.0/src/tinycio/numerics/vector.py` & `tinycio-0.7.1/src/tinycio/numerics/vector.py`

 * *Files identical despite different names*

### Comparing `tinycio-0.7.0/src/tinycio/scripts/color2color.py` & `tinycio-0.7.1/src/tinycio/scripts/color2color.py`

 * *Files identical despite different names*

### Comparing `tinycio-0.7.0/src/tinycio/scripts/hdr_codec.py` & `tinycio-0.7.1/src/tinycio/scripts/hdr_codec.py`

 * *Files identical despite different names*

### Comparing `tinycio-0.7.0/src/tinycio/scripts/img2cube.py` & `tinycio-0.7.1/src/tinycio/scripts/img2cube.py`

 * *Files identical despite different names*

### Comparing `tinycio-0.7.0/src/tinycio/scripts/white_balance.py` & `tinycio-0.7.1/src/tinycio/scripts/white_balance.py`

 * *Files identical despite different names*

### Comparing `tinycio-0.7.0/src/tinycio/spectral.py` & `tinycio-0.7.1/src/tinycio/spectral.py`

 * *Files identical despite different names*

### Comparing `tinycio-0.7.0/src/tinycio/tonemapping.py` & `tinycio-0.7.1/src/tinycio/tonemapping.py`

 * *Files identical despite different names*

### Comparing `tinycio-0.7.0/src/tinycio/usertypes.py` & `tinycio-0.7.1/src/tinycio/usertypes.py`

 * *Files identical despite different names*

### Comparing `tinycio-0.7.0/src/tinycio/util/colorutil.py` & `tinycio-0.7.1/src/tinycio/util/colorutil.py`

 * *Files identical despite different names*

### Comparing `tinycio-0.7.0/src/tinycio/util/miscutil.py` & `tinycio-0.7.1/src/tinycio/util/miscutil.py`

 * *Files identical despite different names*

### Comparing `tinycio-0.7.0/src/tinycio.egg-info/PKG-INFO` & `tinycio-0.7.1/src/tinycio.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tinycio
-Version: 0.7.0
+Version: 0.7.1
 Summary: A primitive, lightweight color management framework for PyTorch-involved projects
 Author-email: Sam Izdat <ghsamizdat@gmail.com>
 Project-URL: Homepage, https://sam-izdat.github.io/tinycio-docs
 Project-URL: Issues, https://github.com/Sam-Izdat/tinycio/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `tinycio-0.7.0/src/tinycio.egg-info/SOURCES.txt` & `tinycio-0.7.1/src/tinycio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tinycio-0.7.0/tests/test_cc_load_save.py` & `tinycio-0.7.1/tests/test_cc_load_save.py`

 * *Files identical despite different names*

### Comparing `tinycio-0.7.0/tests/test_codec.py` & `tinycio-0.7.1/tests/test_codec.py`

 * *Files identical despite different names*

### Comparing `tinycio-0.7.0/tests/test_colorspace.py` & `tinycio-0.7.1/tests/test_colorspace.py`

 * *Files identical despite different names*

### Comparing `tinycio-0.7.0/tests/test_numerics.py` & `tinycio-0.7.1/tests/test_numerics.py`

 * *Files identical despite different names*

### Comparing `tinycio-0.7.0/tests/test_tonemapping.py` & `tinycio-0.7.1/tests/test_tonemapping.py`

 * *Files identical despite different names*

### Comparing `tinycio-0.7.0/tests/test_tutorial.py` & `tinycio-0.7.1/tests/test_tutorial.py`

 * *Files identical despite different names*

