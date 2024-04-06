# Comparing `tmp/tinycio-0.6.3.tar.gz` & `tmp/tinycio-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tinycio-0.6.3.tar", last modified: Thu Mar 28 11:02:06 2024, max compression
+gzip compressed data, was "tinycio-0.7.0.tar", last modified: Sat Apr  6 02:56:51 2024, max compression
```

## Comparing `tinycio-0.6.3.tar` & `tinycio-0.7.0.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxrwxrwx   0        0        0        0 2024-03-28 11:02:06.252280 tinycio-0.6.3/
--rw-rw-rw-   0        0        0     1085 2023-12-13 13:07:04.000000 tinycio-0.6.3/LICENSE.txt
--rw-rw-rw-   0        0        0     1754 2024-03-28 11:02:06.251279 tinycio-0.6.3/PKG-INFO
--rw-rw-rw-   0        0        0     1073 2023-12-22 22:36:31.000000 tinycio-0.6.3/README.md
--rw-rw-rw-   0        0        0     1099 2024-03-28 10:57:50.000000 tinycio-0.6.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-28 11:02:06.252280 tinycio-0.6.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-03-28 11:02:06.117305 tinycio-0.6.3/src/
-drwxrwxrwx   0        0        0        0 2024-03-28 11:02:06.141920 tinycio-0.6.3/src/tinycio/
--rw-rw-rw-   0        0        0      333 2023-12-20 19:54:11.000000 tinycio-0.6.3/src/tinycio/__init__.py
--rw-rw-rw-   0        0        0    12098 2024-01-28 19:40:42.000000 tinycio-0.6.3/src/tinycio/balance.py
--rw-rw-rw-   0        0        0     2946 2023-12-25 07:42:00.000000 tinycio-0.6.3/src/tinycio/codec.py
--rw-rw-rw-   0        0        0    50809 2024-03-28 10:31:50.000000 tinycio-0.6.3/src/tinycio/colorspace.py
--rw-rw-rw-   0        0        0    32181 2024-01-28 19:41:54.000000 tinycio-0.6.3/src/tinycio/correction.py
-drwxrwxrwx   0        0        0        0 2024-03-28 11:02:06.165927 tinycio-0.6.3/src/tinycio/fsio/
--rw-rw-rw-   0        0        0      191 2023-12-07 20:04:01.000000 tinycio-0.6.3/src/tinycio/fsio/__init__.py
--rw-rw-rw-   0        0        0     1987 2024-01-13 15:11:35.000000 tinycio-0.6.3/src/tinycio/fsio/format.py
--rw-rw-rw-   0        0        0     5424 2023-12-25 07:40:28.000000 tinycio-0.6.3/src/tinycio/fsio/imagefile.py
--rw-rw-rw-   0        0        0     3314 2023-12-25 07:40:39.000000 tinycio-0.6.3/src/tinycio/fsio/lutfile.py
--rw-rw-rw-   0        0        0      102 2023-12-14 19:20:02.000000 tinycio-0.6.3/src/tinycio/globals.py
--rw-rw-rw-   0        0        0     2215 2023-12-15 20:51:38.000000 tinycio-0.6.3/src/tinycio/loss.py
--rw-rw-rw-   0        0        0     9904 2023-12-25 07:42:04.000000 tinycio-0.6.3/src/tinycio/lut.py
-drwxrwxrwx   0        0        0        0 2024-03-28 11:02:06.175198 tinycio-0.6.3/src/tinycio/np_agx/
--rw-rw-rw-   0        0        0    11064 2023-12-11 19:03:49.000000 tinycio-0.6.3/src/tinycio/np_agx/agx.py
-drwxrwxrwx   0        0        0        0 2024-03-28 11:02:06.190837 tinycio-0.6.3/src/tinycio/numerics/
--rw-rw-rw-   0        0        0     1969 2023-12-25 07:39:27.000000 tinycio-0.6.3/src/tinycio/numerics/__init__.py
--rw-rw-rw-   0        0        0     3044 2023-12-15 12:09:46.000000 tinycio-0.6.3/src/tinycio/numerics/linalg.py
--rw-rw-rw-   0        0        0      482 2023-12-13 15:27:22.000000 tinycio-0.6.3/src/tinycio/numerics/util_pt.py
--rw-rw-rw-   0        0        0      964 2023-12-13 15:27:27.000000 tinycio-0.6.3/src/tinycio/numerics/util_py.py
--rw-rw-rw-   0        0        0   166640 2023-12-20 20:22:45.000000 tinycio-0.6.3/src/tinycio/numerics/vector.py
-drwxrwxrwx   0        0        0        0 2024-03-28 11:02:06.203840 tinycio-0.6.3/src/tinycio/scripts/
--rw-rw-rw-   0        0        0        0 2023-12-20 20:22:45.000000 tinycio-0.6.3/src/tinycio/scripts/__init__.py
--rw-rw-rw-   0        0        0     4169 2023-12-20 23:16:15.000000 tinycio-0.6.3/src/tinycio/scripts/color2color.py
--rw-rw-rw-   0        0        0     2694 2023-12-20 20:22:45.000000 tinycio-0.6.3/src/tinycio/scripts/hdr_codec.py
--rw-rw-rw-   0        0        0     4835 2023-12-20 20:22:45.000000 tinycio-0.6.3/src/tinycio/scripts/img2cube.py
--rw-rw-rw-   0        0        0      215 2023-12-20 20:22:45.000000 tinycio-0.6.3/src/tinycio/scripts/post_install.py
--rw-rw-rw-   0        0        0     4073 2023-12-20 23:13:42.000000 tinycio-0.6.3/src/tinycio/scripts/white_balance.py
--rw-rw-rw-   0        0        0     7087 2024-03-28 10:51:54.000000 tinycio-0.6.3/src/tinycio/spectral.py
--rw-rw-rw-   0        0        0     6526 2023-12-25 07:34:51.000000 tinycio-0.6.3/src/tinycio/tonemapping.py
--rw-rw-rw-   0        0        0    30079 2024-02-25 23:13:23.000000 tinycio-0.6.3/src/tinycio/usertypes.py
-drwxrwxrwx   0        0        0        0 2024-03-28 11:02:06.205839 tinycio-0.6.3/src/tinycio/util/
--rw-rw-rw-   0        0        0      334 2023-12-14 19:18:41.000000 tinycio-0.6.3/src/tinycio/util/__init__.py
--rw-rw-rw-   0        0        0    17822 2023-12-14 18:35:05.000000 tinycio-0.6.3/src/tinycio/util/colorutil.py
--rw-rw-rw-   0        0        0     3065 2023-12-14 19:21:16.000000 tinycio-0.6.3/src/tinycio/util/miscutil.py
-drwxrwxrwx   0        0        0        0 2024-03-28 11:02:06.250279 tinycio-0.6.3/src/tinycio.egg-info/
--rw-rw-rw-   0        0        0     1754 2024-03-28 11:02:06.000000 tinycio-0.6.3/src/tinycio.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1242 2024-03-28 11:02:06.000000 tinycio-0.6.3/src/tinycio.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-28 11:02:06.000000 tinycio-0.6.3/src/tinycio.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      287 2024-03-28 11:02:06.000000 tinycio-0.6.3/src/tinycio.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       47 2024-03-28 11:02:06.000000 tinycio-0.6.3/src/tinycio.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-03-28 11:02:06.000000 tinycio-0.6.3/src/tinycio.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-03-28 11:02:06.249278 tinycio-0.6.3/tests/
--rw-rw-rw-   0        0        0     1577 2023-12-25 06:28:22.000000 tinycio-0.6.3/tests/test_cc_load_save.py
--rw-rw-rw-   0        0        0     2675 2023-12-15 14:14:45.000000 tinycio-0.6.3/tests/test_codec.py
--rw-rw-rw-   0        0        0    14512 2024-01-01 03:02:31.000000 tinycio-0.6.3/tests/test_colorspace.py
--rw-rw-rw-   0        0        0    20740 2023-12-25 06:46:05.000000 tinycio-0.6.3/tests/test_numerics.py
--rw-rw-rw-   0        0        0     1253 2023-12-31 23:57:22.000000 tinycio-0.6.3/tests/test_tonemapping.py
--rw-rw-rw-   0        0        0     7075 2023-12-25 06:48:29.000000 tinycio-0.6.3/tests/test_tutorial.py
+drwxrwxrwx   0        0        0        0 2024-04-06 02:56:51.753777 tinycio-0.7.0/
+-rw-rw-rw-   0        0        0     1085 2023-12-13 13:07:04.000000 tinycio-0.7.0/LICENSE.txt
+-rw-rw-rw-   0        0        0     1754 2024-04-06 02:56:51.752777 tinycio-0.7.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1073 2023-12-22 22:36:31.000000 tinycio-0.7.0/README.md
+-rw-rw-rw-   0        0        0     1099 2024-04-06 02:34:50.000000 tinycio-0.7.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-06 02:56:51.753777 tinycio-0.7.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-06 02:56:51.700765 tinycio-0.7.0/src/
+drwxrwxrwx   0        0        0        0 2024-04-06 02:56:51.719770 tinycio-0.7.0/src/tinycio/
+-rw-rw-rw-   0        0        0      333 2023-12-20 19:54:11.000000 tinycio-0.7.0/src/tinycio/__init__.py
+-rw-rw-rw-   0        0        0    12098 2024-01-28 19:40:42.000000 tinycio-0.7.0/src/tinycio/balance.py
+-rw-rw-rw-   0        0        0     2946 2023-12-25 07:42:00.000000 tinycio-0.7.0/src/tinycio/codec.py
+-rw-rw-rw-   0        0        0    51797 2024-04-06 01:37:04.000000 tinycio-0.7.0/src/tinycio/colorspace.py
+-rw-rw-rw-   0        0        0    32181 2024-01-28 19:41:54.000000 tinycio-0.7.0/src/tinycio/correction.py
+drwxrwxrwx   0        0        0        0 2024-04-06 02:56:51.735773 tinycio-0.7.0/src/tinycio/fsio/
+-rw-rw-rw-   0        0        0      191 2023-12-07 20:04:01.000000 tinycio-0.7.0/src/tinycio/fsio/__init__.py
+-rw-rw-rw-   0        0        0     1987 2024-01-13 15:11:35.000000 tinycio-0.7.0/src/tinycio/fsio/format.py
+-rw-rw-rw-   0        0        0     5424 2023-12-25 07:40:28.000000 tinycio-0.7.0/src/tinycio/fsio/imagefile.py
+-rw-rw-rw-   0        0        0     3314 2023-12-25 07:40:39.000000 tinycio-0.7.0/src/tinycio/fsio/lutfile.py
+-rw-rw-rw-   0        0        0      102 2023-12-14 19:20:02.000000 tinycio-0.7.0/src/tinycio/globals.py
+-rw-rw-rw-   0        0        0     2215 2023-12-15 20:51:38.000000 tinycio-0.7.0/src/tinycio/loss.py
+-rw-rw-rw-   0        0        0     9904 2023-12-25 07:42:04.000000 tinycio-0.7.0/src/tinycio/lut.py
+drwxrwxrwx   0        0        0        0 2024-04-06 02:56:51.736774 tinycio-0.7.0/src/tinycio/np_agx/
+-rw-rw-rw-   0        0        0    11064 2023-12-11 19:03:49.000000 tinycio-0.7.0/src/tinycio/np_agx/agx.py
+drwxrwxrwx   0        0        0        0 2024-04-06 02:56:51.739774 tinycio-0.7.0/src/tinycio/numerics/
+-rw-rw-rw-   0        0        0     1969 2023-12-25 07:39:27.000000 tinycio-0.7.0/src/tinycio/numerics/__init__.py
+-rw-rw-rw-   0        0        0     3044 2023-12-15 12:09:46.000000 tinycio-0.7.0/src/tinycio/numerics/linalg.py
+-rw-rw-rw-   0        0        0      482 2023-12-13 15:27:22.000000 tinycio-0.7.0/src/tinycio/numerics/util_pt.py
+-rw-rw-rw-   0        0        0      964 2023-12-13 15:27:27.000000 tinycio-0.7.0/src/tinycio/numerics/util_py.py
+-rw-rw-rw-   0        0        0   166640 2023-12-20 20:22:45.000000 tinycio-0.7.0/src/tinycio/numerics/vector.py
+drwxrwxrwx   0        0        0        0 2024-04-06 02:56:51.743775 tinycio-0.7.0/src/tinycio/scripts/
+-rw-rw-rw-   0        0        0        0 2023-12-20 20:22:45.000000 tinycio-0.7.0/src/tinycio/scripts/__init__.py
+-rw-rw-rw-   0        0        0     4731 2024-04-06 02:34:14.000000 tinycio-0.7.0/src/tinycio/scripts/color2color.py
+-rw-rw-rw-   0        0        0     2694 2023-12-20 20:22:45.000000 tinycio-0.7.0/src/tinycio/scripts/hdr_codec.py
+-rw-rw-rw-   0        0        0     4835 2023-12-20 20:22:45.000000 tinycio-0.7.0/src/tinycio/scripts/img2cube.py
+-rw-rw-rw-   0        0        0      215 2023-12-20 20:22:45.000000 tinycio-0.7.0/src/tinycio/scripts/post_install.py
+-rw-rw-rw-   0        0        0     4073 2023-12-20 23:13:42.000000 tinycio-0.7.0/src/tinycio/scripts/white_balance.py
+-rw-rw-rw-   0        0        0     7087 2024-03-28 10:51:54.000000 tinycio-0.7.0/src/tinycio/spectral.py
+-rw-rw-rw-   0        0        0     6612 2024-04-06 01:32:15.000000 tinycio-0.7.0/src/tinycio/tonemapping.py
+-rw-rw-rw-   0        0        0    31442 2024-04-06 02:52:18.000000 tinycio-0.7.0/src/tinycio/usertypes.py
+drwxrwxrwx   0        0        0        0 2024-04-06 02:56:51.745776 tinycio-0.7.0/src/tinycio/util/
+-rw-rw-rw-   0        0        0      334 2023-12-14 19:18:41.000000 tinycio-0.7.0/src/tinycio/util/__init__.py
+-rw-rw-rw-   0        0        0    17822 2023-12-14 18:35:05.000000 tinycio-0.7.0/src/tinycio/util/colorutil.py
+-rw-rw-rw-   0        0        0     3065 2023-12-14 19:21:16.000000 tinycio-0.7.0/src/tinycio/util/miscutil.py
+drwxrwxrwx   0        0        0        0 2024-04-06 02:56:51.752777 tinycio-0.7.0/src/tinycio.egg-info/
+-rw-rw-rw-   0        0        0     1754 2024-04-06 02:56:51.000000 tinycio-0.7.0/src/tinycio.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1242 2024-04-06 02:56:51.000000 tinycio-0.7.0/src/tinycio.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-06 02:56:51.000000 tinycio-0.7.0/src/tinycio.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      287 2024-04-06 02:56:51.000000 tinycio-0.7.0/src/tinycio.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       47 2024-04-06 02:56:51.000000 tinycio-0.7.0/src/tinycio.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-06 02:56:51.000000 tinycio-0.7.0/src/tinycio.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-06 02:56:51.751777 tinycio-0.7.0/tests/
+-rw-rw-rw-   0        0        0     1577 2023-12-25 06:28:22.000000 tinycio-0.7.0/tests/test_cc_load_save.py
+-rw-rw-rw-   0        0        0     2675 2023-12-15 14:14:45.000000 tinycio-0.7.0/tests/test_codec.py
+-rw-rw-rw-   0        0        0    14512 2024-01-01 03:02:31.000000 tinycio-0.7.0/tests/test_colorspace.py
+-rw-rw-rw-   0        0        0    20740 2023-12-25 06:46:05.000000 tinycio-0.7.0/tests/test_numerics.py
+-rw-rw-rw-   0        0        0     1400 2024-04-06 01:54:00.000000 tinycio-0.7.0/tests/test_tonemapping.py
+-rw-rw-rw-   0        0        0     7075 2023-12-25 06:48:29.000000 tinycio-0.7.0/tests/test_tutorial.py
```

### Comparing `tinycio-0.6.3/LICENSE.txt` & `tinycio-0.7.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tinycio-0.6.3/PKG-INFO` & `tinycio-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tinycio
-Version: 0.6.3
+Version: 0.7.0
 Summary: A primitive, lightweight color management framework for PyTorch-involved projects
 Author-email: Sam Izdat <ghsamizdat@gmail.com>
 Project-URL: Homepage, https://sam-izdat.github.io/tinycio-docs
 Project-URL: Issues, https://github.com/Sam-Izdat/tinycio/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `tinycio-0.6.3/README.md` & `tinycio-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `tinycio-0.6.3/pyproject.toml` & `tinycio-0.7.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "tinycio"
-version = "0.6.3"
+version = "0.7.0"
 authors = [
   { name="Sam Izdat", email="ghsamizdat@gmail.com" },
 ]
 description = "A primitive, lightweight color management framework for PyTorch-involved projects"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `tinycio-0.6.3/src/tinycio/balance.py` & `tinycio-0.7.0/src/tinycio/balance.py`

 * *Files identical despite different names*

### Comparing `tinycio-0.6.3/src/tinycio/codec.py` & `tinycio-0.7.0/src/tinycio/codec.py`

 * *Files identical despite different names*

### Comparing `tinycio-0.6.3/src/tinycio/colorspace.py` & `tinycio-0.7.0/src/tinycio/colorspace.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
         CIELAB      = 1<<18 
         CIELUV      = 1<<19 
         HSV         = 1<<20 
         HSL         = 1<<21 
         OKHSV       = 1<<22
         OKHSL       = 1<<23
 
-        SCENE_LINEAR    = SRGB_LIN | REC2020_LIN | DCI_P3_LIN | ACESCG | ACES2065_1 | CIE_XYZ
+        SCENE_LINEAR    = SRGB_LIN | REC2020_LIN | DCI_P3_LIN | ACESCG | ACES2065_1 | LMS | CIE_XYZ
         PERCEPTUAL      = OKLAB | CIELAB | CIELUV | OKHSL | OKHSV
         CYLINDRICAL     = HSL | HSV | OKHSL | OKHSV
 
         GAMUT_SRGB      = SRGB | SRGB_LIN | REC709 | HSL | HSV
         GAMUT_AP0       = ACES2065_1
         GAMUT_AP1       = ACESCG | ACESCC | ACESCCT
         GAMUT_REC2020   = REC2020 | REC2020_LIN
@@ -102,14 +102,37 @@
 
     # NOTE: Includes "D60"/D65 white point conversion
     mat_acescg_to_srgb = [
         [ 1.705050993,  -0.6217921206,-0.083258872],
         [-0.1302564175,  1.140804737, -0.01054831907],
         [-0.02400335681,-0.1289689761, 1.152972333]]
 
+    mat_aces_rrt_sat = [
+        [0.970889, 0.026963, 0.002148],
+        [0.010889, 0.986963, 0.002148],
+        [0.010889, 0.026963, 0.962148]]
+
+    mat_aces_rrt_sat_inv = [
+        [ 1.03032  , -0.0280865, -0.0022375],
+        [-0.0113427,  1.01358  , -0.0022375],
+        [-0.0113427, -0.0280865,  1.03943]]
+
+    # sRGB => XYZ => D65_2_D60 => AP1 => RRT_SAT
+    mat_srgb_to_ap1_tm = [
+        [0.59719, 0.35458, 0.04823],
+        [0.07600, 0.90834, 0.01566],
+        [0.02840, 0.13383, 0.83777]]
+
+    # ODT_SAT => XYZ => D60_2_D65 => sRGB
+    mat_ap1_to_srgb_tm = [
+        [ 1.60475, -0.53108, -0.07367],
+        [-0.10208,  1.10813, -0.00605],
+        [-0.00327, -0.07276,  1.07602]
+        ]
+
     # NOTE: Includes "D60"/D65 white point conversion
     mat_srgb_to_aces2065_1 = [
         [ 0.439632982,  0.382988698, 0.17737832],
         [ 0.0897764431, 0.813439429, 0.0967841284],
         [ 0.0175411704, 0.111546553, 0.870912277]]
 
     # NOTE: Includes "D60"/D65 white point conversion
@@ -398,14 +421,22 @@
         Y = xyy[2:3]
         y[y <= 0.] = eps
         X = (Y / y) * x
         Z = (Y / y) * (1. - x - y)
         return torch.cat([X, Y, Z], dim=0)
 
     @classmethod
+    def _ap1_rrt_sat(cls, im:torch.Tensor) -> torch.Tensor:
+        return mm(im, cls.mat_aces_rrt_sat)
+
+    @classmethod
+    def _ap1_rrt_sat_inv(cls, im:torch.Tensor) -> torch.Tensor:
+        return mm(im, cls.mat_aces_rrt_sat_inv)
+
+    @classmethod
     def _xyz_to_lms(cls, xyz:torch.Tensor) -> torch.Tensor:
         """
         Convert CIE XYZ color space to LMS color space.
 
         :param xyz: Input CIE XYZ color space tensor
         :return: LMS color space tensor
         """
```

### Comparing `tinycio-0.6.3/src/tinycio/correction.py` & `tinycio-0.7.0/src/tinycio/correction.py`

 * *Files identical despite different names*

### Comparing `tinycio-0.6.3/src/tinycio/fsio/format.py` & `tinycio-0.7.0/src/tinycio/fsio/format.py`

 * *Files identical despite different names*

### Comparing `tinycio-0.6.3/src/tinycio/fsio/imagefile.py` & `tinycio-0.7.0/src/tinycio/fsio/imagefile.py`

 * *Files identical despite different names*

### Comparing `tinycio-0.6.3/src/tinycio/fsio/lutfile.py` & `tinycio-0.7.0/src/tinycio/fsio/lutfile.py`

 * *Files identical despite different names*

### Comparing `tinycio-0.6.3/src/tinycio/loss.py` & `tinycio-0.7.0/src/tinycio/loss.py`

 * *Files identical despite different names*

### Comparing `tinycio-0.6.3/src/tinycio/lut.py` & `tinycio-0.7.0/src/tinycio/lut.py`

 * *Files identical despite different names*

### Comparing `tinycio-0.6.3/src/tinycio/np_agx/agx.py` & `tinycio-0.7.0/src/tinycio/np_agx/agx.py`

 * *Files identical despite different names*

### Comparing `tinycio-0.6.3/src/tinycio/numerics/__init__.py` & `tinycio-0.7.0/src/tinycio/numerics/__init__.py`

 * *Files identical despite different names*

### Comparing `tinycio-0.6.3/src/tinycio/numerics/linalg.py` & `tinycio-0.7.0/src/tinycio/numerics/linalg.py`

 * *Files identical despite different names*

### Comparing `tinycio-0.6.3/src/tinycio/numerics/util_py.py` & `tinycio-0.7.0/src/tinycio/numerics/util_py.py`

 * *Files identical despite different names*

### Comparing `tinycio-0.6.3/src/tinycio/numerics/vector.py` & `tinycio-0.7.0/src/tinycio/numerics/vector.py`

 * *Files identical despite different names*

### Comparing `tinycio-0.6.3/src/tinycio/scripts/color2color.py` & `tinycio-0.7.0/src/tinycio/scripts/color2color.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,39 +12,53 @@
     parser.add_argument(
         'ics', 
         type=str, 
         choices=[
             'cie_xyz', 'cie_xyy', 'srgb', 'srgb_lin',
             'rec709', 'rec2020', 'rec2020_lin', 
             'dci_p3', 'dci_p3_lin', 'display_p3',
-            'acescg', 'aces2065_1', 'lms', 'hsl', 'hsv',
-            'oklab', 'cielab'],
+            'acescg', 'aces2065_1', 'acescc', 'lms', 
+            'hsl', 'hsv', 'oklab', 'cielab'],
         metavar='input-color-space', # because bad formatting is bad :(
         help='Input color space\n' + \
             'CHOICES:\n' + \
             '    cie_xyz, cie_xyy, srgb, srgb_lin, \n' + \
             '    rec709, rec2020, rec_2020_lin, \n' + \
             '    dci_p3, dci_p3_lin, display_p3, \n' + \
-            '    acescg, aces2065_1, lms, hsl, hsv \n' + \
-            '    oklab, cielab'
+            '    acescg, acescc, aces2065_1, \n' + \
+            '    lms, hsl, hsv, oklab, cielab'
         )
     parser.add_argument('output', type=str, help='Output image file path')
     parser.add_argument(
         'ocs',
         type=str, 
         choices=[
-            'cie_xyz', 'cie_xyy', 'srgb', 'srgb_linear',
-            'rec709', 'rec2020', 'dci_p3', 'display_p3',
-            'acescg', 'aces2065_1', 'lms', 'hsl', 'hsv',
-            'oklab', 'cielab'],
+            'cie_xyz', 'cie_xyy', 'srgb', 'srgb_lin',
+            'rec709', 'rec2020', 'rec2020_lin', 
+            'dci_p3', 'dci_p3_lin', 'display_p3',
+            'acescg', 'aces2065_1', 'acescc', 'lms', 
+            'hsl', 'hsv', 'oklab', 'cielab'],
         metavar='output-color-space',
         help='Output color space\n' + \
             'CHOICES: [same as above]'  
         )
     parser.add_argument(
+        '--tmcs', 
+        type=str, 
+        default="srgb_lin", 
+        const="srgb_lin",
+        nargs='?',
+        choices=['srgb_lin', 'rec2020_lin', 'dci_p3_lin', 'acescg', 'aces2065_1'],
+        metavar='', 
+        help='Tone mapping color space (default: %(default)s)\n' + \
+            'CHOICES:\n' + \
+            '    srgb_lin, rec2020_lin \n' + \
+            '    dci_p3_lin, acescg, aces2065_1 \n'
+        )
+    parser.add_argument(
         '--igf', 
         type=str, 
         default="unknown", 
         const="unknown",
         nargs='?',
         choices=['sfloat16','sfloat32','uint8','uint16','uint32'],
         metavar='', 
@@ -97,15 +111,15 @@
         if alpha:
             im = fsio.load_image(fp_in, graphics_format=fsio.GraphicsFormat[gf_in])
             ac = im[3:4,...] if im.size(0) == 4 else None
             im = ColorImage(fsio.truncate_image(im), color_space=cs_in)
         else:
             im = ColorImage.load(fp_in, color_space=cs_in, graphics_format=gf_in)
 
-        im = im.tone_map(tm) # it's okay to pass "NONE"
+        im = im.tone_map(tm, target_color_space=args.tmcs) # it's okay to pass "NONE"
         im = im.to_color_space(cs_out)
         if ac is not None: im = torch.cat([im, ac], dim=0)
         im.save(fp_out, gf_out)
         print(f'saved image to: {os.path.realpath(fp_out)}')
     except Exception as e: 
         print(f'cannot convert: {e}')
```

### Comparing `tinycio-0.6.3/src/tinycio/scripts/hdr_codec.py` & `tinycio-0.7.0/src/tinycio/scripts/hdr_codec.py`

 * *Files identical despite different names*

### Comparing `tinycio-0.6.3/src/tinycio/scripts/img2cube.py` & `tinycio-0.7.0/src/tinycio/scripts/img2cube.py`

 * *Files identical despite different names*

### Comparing `tinycio-0.6.3/src/tinycio/scripts/white_balance.py` & `tinycio-0.7.0/src/tinycio/scripts/white_balance.py`

 * *Files identical despite different names*

### Comparing `tinycio-0.6.3/src/tinycio/spectral.py` & `tinycio-0.7.0/src/tinycio/spectral.py`

 * *Files identical despite different names*

### Comparing `tinycio-0.6.3/src/tinycio/tonemapping.py` & `tinycio-0.7.0/src/tinycio/tonemapping.py`

 * *Files 2% similar despite different names*

```diff
@@ -166,25 +166,26 @@
         numerator = l_old * (1. + (l_old / (max_white_l * max_white_l)))
         l_new = numerator / (1. + l_old)
         return torch.clamp(cls.__change_luminance(im, l_new), 0., 1.)
 
     @classmethod
     def _aces_fitted(cls, im:torch.Tensor):
         """
-        Apply ACES (fitted version) tone mapping.
+        Apply ACES (Stephen Hill's fitted version) tone mapping.
         
         .. note::
         
             expects [C, H, W] input in ACESCcg color space, return ACEScg image tensor
 
         :param torch.Tensor im: Input image tensor.
         :return: Tone-mapped image tensor.
         :rtype: torch.Tensor
         """
         C, H, W = im.size()
 
         # RRT and ODT
+        im = ColorSpace._ap1_rrt_sat(im)
         a = im * (im + 0.0245786) - 0.000090537
         b = im * (0.983729 * im + 0.4329510) + 0.238081
-        im  = a / b
+        im  = ColorSpace._ap1_rrt_sat_inv(a / b)
 
         return torch.clamp(im, 0., 1.)
```

### Comparing `tinycio-0.6.3/src/tinycio/usertypes.py` & `tinycio-0.7.0/src/tinycio/usertypes.py`

 * *Files 2% similar despite different names*

```diff
@@ -307,38 +307,59 @@
         if type(color_space) is str: color_space = ColorSpace.Variant[color_space.strip().upper()]
         assert isinstance(color_space, ColorSpace.Variant), "Invalid color space"
         res = None
         res = ColorSpace.convert(self.clone(), source=self.color_space, destination=color_space)
         res = ColorImage(res, color_space=color_space)
         return res
 
-    def tone_map(self, tone_mapper:Union[str,ToneMapping.Variant]) -> ColorImage:
+    def tone_map(self, 
+        tone_mapper:Union[str,ToneMapping.Variant], 
+        target_color_space:Union[str,ColorSpace.Variant]=ColorSpace.Variant.SRGB_LIN) -> ColorImage:
         """
         Apply tone mapping and return as new :class:`ColorImage`.
 
         .. note::
 
+            Image will be returned and (if the TMO allows) tone mapped in the desired target color space. 
             Any needed color space conversion will be handled automatically.
 
         :param tone_mapper: Tone mapper to use.
         :type tone_mapper: str | ToneMapping.Variant
+        :param target_color_space: The desired color space the image should be tone mapped for. 
+            Must be a scene-linear RGB color space. The image will be returned in this color space. 
+            If the TMO requires a different color space, the image will converted after tone mapping. 
+            Some TMOs may have been designed with linear sRGB in mind and may not perform as expected 
+            in a different color space.
+        :type target_color_space: str | ColorSpace.Variant
         :return: New tone mapped :class:`ColorImage`.
         """
         if type(tone_mapper) is str: tone_mapper = ToneMapping.Variant[tone_mapper.strip().upper()]
-        assert isinstance(tone_mapper, ToneMapping.Variant), "Invalid tone mapper"
+        if type(target_color_space) is str: target_color_space = ColorSpace.Variant[target_color_space.strip().upper()]
         ip = self.clone()
-        cs_tm = self.color_space
+
+        assert isinstance(tone_mapper, ToneMapping.Variant), "Invalid tone mapper"
+        assert target_color_space & ColorSpace.Variant.SCENE_LINEAR, "target color space expected to be scene-linear"
+        assert (target_color_space & ColorSpace.Variant.SCENE_LINEAR & ColorSpace.Variant.MODEL_RGB), \
+            "target color space must be a in a scene-linear RGB color space"
+        assert self.color_space != ColorSpace.Variant.UNKNOWN and self.color_space != ColorSpace.Variant.NONCOLOR, \
+            "input image must have a valid color space"
+        
+        res = None
+
         if tone_mapper == ToneMapping.Variant.ACESCG:
-            cs_tm = ColorSpace.Variant.ACESCG
-        elif not (self.color_space & ColorSpace.Variant.SCENE_LINEAR & ColorSpace.Variant.MODEL_RGB):
-            cs_tm = ColorSpace.Variant.SRGB_LIN
-        res = ColorSpace.convert(ip, source=self.color_space, destination=cs_tm)
+            res = ColorSpace.convert(ip, source=self.color_space, destination=ColorSpace.Variant.ACESCG)
+        else:
+            res = ColorSpace.convert(ip, source=self.color_space, destination=target_color_space)
+        
         res = ToneMapping.apply(res, tone_mapper=tone_mapper)
-        res = ColorSpace.convert(res, source=cs_tm, destination=self.color_space)
-        return ColorImage(res, color_space=self.color_space)
+
+        if tone_mapper == ToneMapping.Variant.ACESCG:
+            res = ColorSpace.convert(res, source=ColorSpace.Variant.ACESCG, destination=target_color_space)
+
+        return ColorImage(res.clamp(0., 1.), color_space=target_color_space)
 
     def lut(self, lut:Union[str, LookupTable], lut_format=LUTFormat.UNKNOWN) -> ColorImage:
         """
         Apply a :class:`LookupTable` and return as new :class:`ColorImage`.
 
         :param lut: :class:`.LookupTable` or LUT file path
         :param lut_format: Format of the LUT, if loading from file.
```

### Comparing `tinycio-0.6.3/src/tinycio/util/colorutil.py` & `tinycio-0.7.0/src/tinycio/util/colorutil.py`

 * *Files identical despite different names*

### Comparing `tinycio-0.6.3/src/tinycio/util/miscutil.py` & `tinycio-0.7.0/src/tinycio/util/miscutil.py`

 * *Files identical despite different names*

### Comparing `tinycio-0.6.3/src/tinycio.egg-info/PKG-INFO` & `tinycio-0.7.0/src/tinycio.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tinycio
-Version: 0.6.3
+Version: 0.7.0
 Summary: A primitive, lightweight color management framework for PyTorch-involved projects
 Author-email: Sam Izdat <ghsamizdat@gmail.com>
 Project-URL: Homepage, https://sam-izdat.github.io/tinycio-docs
 Project-URL: Issues, https://github.com/Sam-Izdat/tinycio/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `tinycio-0.6.3/src/tinycio.egg-info/SOURCES.txt` & `tinycio-0.7.0/src/tinycio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tinycio-0.6.3/tests/test_cc_load_save.py` & `tinycio-0.7.0/tests/test_cc_load_save.py`

 * *Files identical despite different names*

### Comparing `tinycio-0.6.3/tests/test_codec.py` & `tinycio-0.7.0/tests/test_codec.py`

 * *Files identical despite different names*

### Comparing `tinycio-0.6.3/tests/test_colorspace.py` & `tinycio-0.7.0/tests/test_colorspace.py`

 * *Files identical despite different names*

### Comparing `tinycio-0.6.3/tests/test_numerics.py` & `tinycio-0.7.0/tests/test_numerics.py`

 * *Files identical despite different names*

### Comparing `tinycio-0.6.3/tests/test_tonemapping.py` & `tinycio-0.7.0/tests/test_tonemapping.py`

 * *Files 13% similar despite different names*

```diff
@@ -20,20 +20,20 @@
             v2,
             atol=tol)
 
     def test_cs(self):
         # Checks color space conversion consistency
         for tm in self.tm_list:
             im = ColorImage.load('../doc/images/test_image.png', 'SRGB')
-            im1 = im.tone_map(tm)
-            im2 = im.to_color_space('CIE_XYZ').tone_map(tm).to_color_space('SRGB')
+            im1 = im.tone_map(tm, target_color_space='SRGB_LIN').to_color_space('SRGB')
+            im2 = im.to_color_space('CIE_XYZ').tone_map(tm, target_color_space='SRGB_LIN').to_color_space('SRGB')
             compare = self.check_diff_torch(im1, im2, self.err_tol)
             self.assertTrue(compare)
-            im2 = im.to_color_space('REC2020').tone_map(tm).to_color_space('SRGB')
+            im2 = im.to_color_space('REC2020').tone_map(tm, target_color_space='SRGB_LIN').to_color_space('SRGB')
             compare = self.check_diff_torch(im1, im2, self.err_tol)
             self.assertTrue(compare)
-            im2 = im.to_color_space('LMS').tone_map(tm).to_color_space('SRGB')
+            im2 = im.to_color_space('LMS').tone_map(tm, target_color_space='SRGB_LIN').to_color_space('SRGB')
             compare = self.check_diff_torch(im1, im2, self.err_tol)
             self.assertTrue(compare)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `tinycio-0.6.3/tests/test_tutorial.py` & `tinycio-0.7.0/tests/test_tutorial.py`

 * *Files identical despite different names*

