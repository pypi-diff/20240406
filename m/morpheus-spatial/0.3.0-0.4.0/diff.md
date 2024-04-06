# Comparing `tmp/morpheus_spatial-0.3.0.tar.gz` & `tmp/morpheus_spatial-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "morpheus_spatial-0.3.0.tar", max compression
+gzip compressed data, was "morpheus_spatial-0.4.0.tar", max compression
```

## Comparing `morpheus_spatial-0.3.0.tar` & `morpheus_spatial-0.4.0.tar`

### file list

```diff
@@ -1,40 +1,42 @@
--rw-r--r--   0        0        0     1465 2024-03-24 22:07:48.345779 morpheus_spatial-0.3.0/README.md
--rw-r--r--   0        0        0      599 2024-03-24 22:44:29.636239 morpheus_spatial-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      172 2024-03-24 20:40:40.558026 morpheus_spatial-0.3.0/src/morpheus/__init__.py
--rw-r--r--   0        0        0        0 2024-03-24 19:57:48.985646 morpheus_spatial-0.3.0/src/morpheus/api/__init__py
--rw-r--r--   0        0        0      535 2024-03-24 20:40:40.558500 morpheus_spatial-0.3.0/src/morpheus/api/__pycache__/defaults.cpython-39.pyc
--rw-r--r--   0        0        0     7022 2024-03-24 20:40:40.559130 morpheus_spatial-0.3.0/src/morpheus/api/__pycache__/interfaces.cpython-39.pyc
--rw-r--r--   0        0        0      453 2024-03-24 19:57:49.004227 morpheus_spatial-0.3.0/src/morpheus/api/defaults.py
--rw-r--r--   0        0        0     6889 2024-03-24 19:57:49.010975 morpheus_spatial-0.3.0/src/morpheus/api/interfaces.py
--rw-r--r--   0        0        0       77 2024-03-24 20:40:40.559608 morpheus_spatial-0.3.0/src/morpheus/classification/__init__.py
--rw-r--r--   0        0        0      276 2024-03-24 20:40:58.819685 morpheus_spatial-0.3.0/src/morpheus/classification/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     4787 2024-03-24 20:40:58.763994 morpheus_spatial-0.3.0/src/morpheus/classification/__pycache__/classifier.cpython-39.pyc
--rw-r--r--   0        0        0     1728 2024-03-24 20:40:58.818768 morpheus_spatial-0.3.0/src/morpheus/classification/__pycache__/train.cpython-39.pyc
--rw-r--r--   0        0        0     5504 2024-03-24 20:40:40.561582 morpheus_spatial-0.3.0/src/morpheus/classification/classifier.py
--rw-r--r--   0        0        0     2058 2024-03-24 20:40:40.562027 morpheus_spatial-0.3.0/src/morpheus/classification/train.py
--rw-r--r--   0        0        0       35 2024-03-24 19:57:49.050136 morpheus_spatial-0.3.0/src/morpheus/confidence/__init__.py
--rw-r--r--   0        0        0      218 2024-03-24 20:40:40.562476 morpheus_spatial-0.3.0/src/morpheus/confidence/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     6828 2024-03-24 20:40:40.562985 morpheus_spatial-0.3.0/src/morpheus/confidence/__pycache__/trustscore.cpython-39.pyc
--rw-r--r--   0        0        0     8238 2024-03-24 19:57:49.069331 morpheus_spatial-0.3.0/src/morpheus/confidence/trustscore.py
--rw-r--r--   0        0        0      679 2024-03-24 19:57:49.079309 morpheus_spatial-0.3.0/src/morpheus/configuration/Types.py
--rw-r--r--   0        0        0       21 2024-03-24 19:57:49.085704 morpheus_spatial-0.3.0/src/morpheus/configuration/__init__.py
--rw-r--r--   0        0        0      154 2024-03-24 19:57:49.093969 morpheus_spatial-0.3.0/src/morpheus/counterfactual/__init__.py
--rw-r--r--   0        0        0      316 2024-03-24 20:40:40.563441 morpheus_spatial-0.3.0/src/morpheus/counterfactual/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0    21860 2024-03-24 20:40:40.567445 morpheus_spatial-0.3.0/src/morpheus/counterfactual/__pycache__/cf.cpython-39.pyc
--rw-r--r--   0        0        0    10519 2024-03-24 21:54:20.771294 morpheus_spatial-0.3.0/src/morpheus/counterfactual/__pycache__/generate.cpython-39.pyc
--rw-r--r--   0        0        0    34032 2024-03-24 19:57:49.191892 morpheus_spatial-0.3.0/src/morpheus/counterfactual/cf.py
--rw-r--r--   0        0        0    12251 2024-03-24 21:54:17.058186 morpheus_spatial-0.3.0/src/morpheus/counterfactual/generate.py
--rw-r--r--   0        0        0       44 2024-03-24 19:57:49.234244 morpheus_spatial-0.3.0/src/morpheus/datasets/__init__.py
--rw-r--r--   0        0        0    14299 2024-03-24 22:34:11.722417 morpheus_spatial-0.3.0/src/morpheus/datasets/__pycache__/spatial_dataset.cpython-39.pyc
--rw-r--r--   0        0        0     2874 2024-03-24 20:40:40.572611 morpheus_spatial-0.3.0/src/morpheus/datasets/__pycache__/torch_dataset.cpython-39.pyc
--rw-r--r--   0        0        0    18422 2024-03-24 22:30:27.333512 morpheus_spatial-0.3.0/src/morpheus/datasets/spatial_dataset.py
--rw-r--r--   0        0        0     3360 2024-03-24 19:57:49.314337 morpheus_spatial-0.3.0/src/morpheus/datasets/torch_dataset.py
--rw-r--r--   0        0        0        0 2024-03-24 19:57:49.315867 morpheus_spatial-0.3.0/src/morpheus/utils/__init__.py
--rw-r--r--   0        0        0      168 2024-03-24 20:40:40.573764 morpheus_spatial-0.3.0/src/morpheus/utils/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0      945 2024-03-24 20:40:40.574200 morpheus_spatial-0.3.0/src/morpheus/utils/__pycache__/saving.cpython-39.pyc
--rw-r--r--   0        0        0      188 2024-03-24 20:40:40.574625 morpheus_spatial-0.3.0/src/morpheus/utils/__pycache__/version.cpython-39.pyc
--rw-r--r--   0        0        0     5862 2024-03-24 19:57:49.343166 morpheus_spatial-0.3.0/src/morpheus/utils/patchify.py
--rw-r--r--   0        0        0      893 2024-03-24 19:57:49.348980 morpheus_spatial-0.3.0/src/morpheus/utils/saving.py
--rw-r--r--   0        0        0      259 2024-03-24 19:57:49.352361 morpheus_spatial-0.3.0/src/morpheus/utils/set_seeds.py
--rw-r--r--   0        0        0      212 2024-03-24 19:57:49.358398 morpheus_spatial-0.3.0/src/morpheus/utils/version.py
--rw-r--r--   0        0        0     2168 1970-01-01 00:00:00.000000 morpheus_spatial-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1465 2024-03-24 22:07:48.345779 morpheus_spatial-0.4.0/README.md
+-rw-r--r--   0        0        0      611 2024-04-06 01:12:20.348217 morpheus_spatial-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      172 2024-03-24 20:40:40.558026 morpheus_spatial-0.4.0/src/morpheus/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-24 19:57:48.985646 morpheus_spatial-0.4.0/src/morpheus/api/__init__py
+-rw-r--r--   0        0        0      535 2024-03-24 20:40:40.558500 morpheus_spatial-0.4.0/src/morpheus/api/__pycache__/defaults.cpython-39.pyc
+-rw-r--r--   0        0        0     7022 2024-03-24 20:40:40.559130 morpheus_spatial-0.4.0/src/morpheus/api/__pycache__/interfaces.cpython-39.pyc
+-rw-r--r--   0        0        0      453 2024-03-24 19:57:49.004227 morpheus_spatial-0.4.0/src/morpheus/api/defaults.py
+-rw-r--r--   0        0        0     6889 2024-03-24 19:57:49.010975 morpheus_spatial-0.4.0/src/morpheus/api/interfaces.py
+-rw-r--r--   0        0        0       77 2024-03-24 20:40:40.559608 morpheus_spatial-0.4.0/src/morpheus/classification/__init__.py
+-rw-r--r--   0        0        0      276 2024-03-24 20:40:58.819685 morpheus_spatial-0.4.0/src/morpheus/classification/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     4787 2024-03-24 20:40:58.763994 morpheus_spatial-0.4.0/src/morpheus/classification/__pycache__/classifier.cpython-39.pyc
+-rw-r--r--   0        0        0     1728 2024-03-24 20:40:58.818768 morpheus_spatial-0.4.0/src/morpheus/classification/__pycache__/train.cpython-39.pyc
+-rw-r--r--   0        0        0     5504 2024-03-24 20:40:40.561582 morpheus_spatial-0.4.0/src/morpheus/classification/classifier.py
+-rw-r--r--   0        0        0     2058 2024-03-24 20:40:40.562027 morpheus_spatial-0.4.0/src/morpheus/classification/train.py
+-rw-r--r--   0        0        0       35 2024-03-24 19:57:49.050136 morpheus_spatial-0.4.0/src/morpheus/confidence/__init__.py
+-rw-r--r--   0        0        0      218 2024-03-24 20:40:40.562476 morpheus_spatial-0.4.0/src/morpheus/confidence/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     6828 2024-03-24 20:40:40.562985 morpheus_spatial-0.4.0/src/morpheus/confidence/__pycache__/trustscore.cpython-39.pyc
+-rw-r--r--   0        0        0     8238 2024-03-24 19:57:49.069331 morpheus_spatial-0.4.0/src/morpheus/confidence/trustscore.py
+-rw-r--r--   0        0        0      679 2024-03-24 19:57:49.079309 morpheus_spatial-0.4.0/src/morpheus/configuration/Types.py
+-rw-r--r--   0        0        0       21 2024-03-24 19:57:49.085704 morpheus_spatial-0.4.0/src/morpheus/configuration/__init__.py
+-rw-r--r--   0        0        0      154 2024-03-24 19:57:49.093969 morpheus_spatial-0.4.0/src/morpheus/counterfactual/__init__.py
+-rw-r--r--   0        0        0      316 2024-03-24 20:40:40.563441 morpheus_spatial-0.4.0/src/morpheus/counterfactual/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0    26923 2024-04-06 01:07:40.040504 morpheus_spatial-0.4.0/src/morpheus/counterfactual/__pycache__/cf.cpython-39.pyc
+-rw-r--r--   0        0        0    10429 2024-04-06 00:56:25.424106 morpheus_spatial-0.4.0/src/morpheus/counterfactual/__pycache__/generate.cpython-39.pyc
+-rw-r--r--   0        0        0    48197 2024-04-06 01:05:26.035891 morpheus_spatial-0.4.0/src/morpheus/counterfactual/cf.py
+-rw-r--r--   0        0        0    34031 2024-04-05 06:20:06.264699 morpheus_spatial-0.4.0/src/morpheus/counterfactual/cf_in_progress.py
+-rw-r--r--   0        0        0    12218 2024-04-05 23:40:35.387029 morpheus_spatial-0.4.0/src/morpheus/counterfactual/generate.py
+-rw-r--r--   0        0        0       44 2024-03-24 19:57:49.234244 morpheus_spatial-0.4.0/src/morpheus/datasets/__init__.py
+-rw-r--r--   0        0        0    14299 2024-03-24 22:34:11.722417 morpheus_spatial-0.4.0/src/morpheus/datasets/__pycache__/spatial_dataset.cpython-39.pyc
+-rw-r--r--   0        0        0     2874 2024-03-24 20:40:40.572611 morpheus_spatial-0.4.0/src/morpheus/datasets/__pycache__/torch_dataset.cpython-39.pyc
+-rw-r--r--   0        0        0    18422 2024-03-24 22:30:27.333512 morpheus_spatial-0.4.0/src/morpheus/datasets/spatial_dataset.py
+-rw-r--r--   0        0        0     3360 2024-03-24 19:57:49.314337 morpheus_spatial-0.4.0/src/morpheus/datasets/torch_dataset.py
+-rw-r--r--   0        0        0        0 2024-03-24 19:57:49.315867 morpheus_spatial-0.4.0/src/morpheus/utils/__init__.py
+-rw-r--r--   0        0        0      168 2024-03-24 20:40:40.573764 morpheus_spatial-0.4.0/src/morpheus/utils/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0      945 2024-03-24 20:40:40.574200 morpheus_spatial-0.4.0/src/morpheus/utils/__pycache__/saving.cpython-39.pyc
+-rw-r--r--   0        0        0      188 2024-03-24 20:40:40.574625 morpheus_spatial-0.4.0/src/morpheus/utils/__pycache__/version.cpython-39.pyc
+-rw-r--r--   0        0        0     2880 2024-04-05 06:18:14.436561 morpheus_spatial-0.4.0/src/morpheus/utils/gradients.py
+-rw-r--r--   0        0        0     5862 2024-03-24 19:57:49.343166 morpheus_spatial-0.4.0/src/morpheus/utils/patchify.py
+-rw-r--r--   0        0        0      893 2024-03-24 19:57:49.348980 morpheus_spatial-0.4.0/src/morpheus/utils/saving.py
+-rw-r--r--   0        0        0      259 2024-03-24 19:57:49.352361 morpheus_spatial-0.4.0/src/morpheus/utils/set_seeds.py
+-rw-r--r--   0        0        0      212 2024-03-24 19:57:49.358398 morpheus_spatial-0.4.0/src/morpheus/utils/version.py
+-rw-r--r--   0        0        0     2180 1970-01-01 00:00:00.000000 morpheus_spatial-0.4.0/PKG-INFO
```

### Comparing `morpheus_spatial-0.3.0/README.md` & `morpheus_spatial-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `morpheus_spatial-0.3.0/pyproject.toml` & `morpheus_spatial-0.4.0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 [tool.poetry]
 name = "morpheus-spatial"
-version = "0.3.0"
+version = "0.4.0"
 description = ""
 authors = ["neonine2 <jerry.wang95@yahoo.ca>"]
 readme = "README.md"
 packages = [{include = "morpheus", from = "src"}]
 
 [tool.poetry.dependencies]
-python = ">=3.9, <4.0"
-lightning = "^2.2.0.post0"
+python = ">=3.9, <3.12"
+lightning = "^2.0.0"
 pandas = "^2.2.1"
-torchvision = "^0.17.1"
+torchvision = "^0.15.1"
 h5py = "^3.10.0"
 dill = "^0.3.8"
 scikit-learn = "^1.4.1.post1"
-
+tensorflow = "2.11.1"
+torch = "2.0.0"
 
 [tool.poetry.group.test.dependencies]
 pytest = "^8.1.0"
 
-
 [tool.poetry.group.dev.dependencies]
 ipykernel = "^6.29.3"
-dask = "^2024.3.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `morpheus_spatial-0.3.0/src/morpheus/api/__pycache__/defaults.cpython-39.pyc` & `morpheus_spatial-0.4.0/src/morpheus/api/__pycache__/defaults.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `morpheus_spatial-0.3.0/src/morpheus/api/__pycache__/interfaces.cpython-39.pyc` & `morpheus_spatial-0.4.0/src/morpheus/api/__pycache__/interfaces.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `morpheus_spatial-0.3.0/src/morpheus/api/interfaces.py` & `morpheus_spatial-0.4.0/src/morpheus/api/interfaces.py`

 * *Files identical despite different names*

### Comparing `morpheus_spatial-0.3.0/src/morpheus/classification/__pycache__/classifier.cpython-39.pyc` & `morpheus_spatial-0.4.0/src/morpheus/classification/__pycache__/classifier.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `morpheus_spatial-0.3.0/src/morpheus/classification/__pycache__/train.cpython-39.pyc` & `morpheus_spatial-0.4.0/src/morpheus/classification/__pycache__/train.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `morpheus_spatial-0.3.0/src/morpheus/classification/classifier.py` & `morpheus_spatial-0.4.0/src/morpheus/classification/classifier.py`

 * *Files identical despite different names*

### Comparing `morpheus_spatial-0.3.0/src/morpheus/classification/train.py` & `morpheus_spatial-0.4.0/src/morpheus/classification/train.py`

 * *Files identical despite different names*

### Comparing `morpheus_spatial-0.3.0/src/morpheus/confidence/__pycache__/trustscore.cpython-39.pyc` & `morpheus_spatial-0.4.0/src/morpheus/confidence/__pycache__/trustscore.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `morpheus_spatial-0.3.0/src/morpheus/confidence/trustscore.py` & `morpheus_spatial-0.4.0/src/morpheus/confidence/trustscore.py`

 * *Files identical despite different names*

### Comparing `morpheus_spatial-0.3.0/src/morpheus/configuration/Types.py` & `morpheus_spatial-0.4.0/src/morpheus/configuration/Types.py`

 * *Files identical despite different names*

### Comparing `morpheus_spatial-0.3.0/src/morpheus/counterfactual/__pycache__/cf.cpython-39.pyc` & `morpheus_spatial-0.4.0/src/morpheus/counterfactual/__pycache__/cf.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Sun Mar 24 19:57:49 2024 UTC, .py size: 34032 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 24% similar despite different names*

```diff
@@ -1,1367 +1,1683 @@
-00000000: 610d 0d0a 0000 0000 bd85 0066 f084 0000  a..........f....
+00000000: 610d 0d0a 0000 0000 d69f 1066 45bc 0000  a..........fE...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0005 0000 0040 0000 0073 b000 0000 6400  .....@...s....d.
+00000020: 0005 0000 0040 0000 0073 e200 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
-00000040: 6401 6c02 5a02 6400 6401 6c03 5a04 6400  d.l.Z.d.d.l.Z.d.
-00000050: 6402 6c05 6d06 5a06 6d07 5a07 6d08 5a08  d.l.m.Z.m.Z.m.Z.
-00000060: 6d09 5a09 0100 6400 6401 6c0a 5a0b 6400  m.Z...d.d.l.Z.d.
-00000070: 6401 6c0c 5a0c 6400 6401 6c0d 5a0d 6400  d.l.Z.d.d.l.Z.d.
-00000080: 6401 6c0e 6d0f 5a0f 0100 6403 6404 6c10  d.l.m.Z...d.d.l.
-00000090: 6d11 5a11 6d12 5a12 0100 6403 6405 6c13  m.Z.m.Z...d.d.l.
-000000a0: 6d14 5a14 6d15 5a15 6d16 5a16 0100 4700  m.Z.m.Z.m.Z...G.
-000000b0: 6406 6407 8400 6407 6514 6516 8304 5a17  d.d...d.e.e...Z.
-000000c0: 6408 6409 8400 5a18 640a 640b 8400 5a19  d.d...Z.d.d...Z.
-000000d0: 640e 640c 640d 8401 5a1a 6401 5300 290f  d.d.d...Z.d.S.).
-000000e0: e900 0000 004e 2904 da08 4361 6c6c 6162  .....N)...Callab
-000000f0: 6c65 da08 4f70 7469 6f6e 616c da05 5475  le..Optional..Tu
-00000100: 706c 65da 0555 6e69 6f6e e902 0000 0029  ple..Union.....)
-00000110: 02da 0c44 4546 4155 4c54 5f44 4154 41da  ...DEFAULT_DATA.
-00000120: 0c44 4546 4155 4c54 5f4d 4554 4129 03da  .DEFAULT_META)..
-00000130: 0945 7870 6c61 696e 6572 da0b 4578 706c  .Explainer..Expl
-00000140: 616e 6174 696f 6eda 0846 6974 4d69 7869  anation..FitMixi
-00000150: 6e63 0000 0000 0000 0000 0000 0000 0000  nc..............
-00000160: 0000 1700 0000 0000 0000 73b2 0100 0065  ..........s....e
-00000170: 005a 0164 005a 0264 3365 0365 0465 056a  .Z.d.Z.d3e.e.e.j
-00000180: 0667 0165 056a 0666 0219 0065 076a 086a  .g.e.j.f...e.j.j
-00000190: 0966 0219 0065 0365 0465 056a 0667 0165  .f...e.e.e.j.g.e
-000001a0: 056a 0666 0219 0065 076a 086a 0966 0219  .j.f...e.j.j.f..
-000001b0: 0065 0a65 0b65 0b65 0c65 0365 0b65 056a  .e.e.e.e.e.e.e.j
-000001c0: 0666 0219 0065 0365 0b65 056a 0666 0219  .f...e.e.e.j.f..
-000001d0: 0066 0219 0065 0b65 0d65 076a 086a 0919  .f...e.e.e.j.j..
-000001e0: 0065 0d65 076a 086a 0919 0065 0b65 0e65  .e.e.j.j...e.e.e
-000001f0: 0b65 0f65 0b65 0f65 0a65 0a65 0f65 0d65  .e.e.e.e.e.e.e.e
-00000200: 1019 0065 0e64 0464 0d9c 1587 0066 0164  ...e.d.d.....f.d
-00000210: 0e64 0f84 0d5a 1164 1064 1184 005a 1264  .d...Z.d.d...Z.d
-00000220: 1264 1384 005a 1364 1464 1584 005a 1464  .d...Z.d.d...Z.d
-00000230: 1664 1784 005a 1564 1864 1984 005a 1664  .d...Z.d.d...Z.d
-00000240: 1a64 1b84 005a 1764 1c64 1d84 005a 1864  .d...Z.d.d...Z.d
-00000250: 1e64 1f84 005a 1964 2064 2184 005a 1a64  .d...Z.d d!..Z.d
-00000260: 2264 2384 005a 1b65 05a0 1c67 00a1 0165  "d#..Z.e...g...e
-00000270: 05a0 1c67 00a1 0166 0265 056a 0665 056a  ...g...f.e.j.e.j
-00000280: 0664 0064 249c 0364 2564 2684 055a 1d64  .d.d$..d%d&..Z.d
-00000290: 3465 056a 0665 0f65 0f65 0b65 0b64 289c  4e.j.e.e.e.e.d(.
-000002a0: 0564 2964 2a84 055a 1e64 3565 056a 0665  .d)d*..Z.d5e.j.e
-000002b0: 056a 0665 0d65 1f19 0065 0d65 0f19 0065  .j.e.e...e.e...e
-000002c0: 1065 0b65 0e65 0f65 0c65 056a 0665 0c65  .e.e.e.e.e.j.e.e
-000002d0: 056a 0665 056a 0666 0219 0066 0219 0064  .j.e.j.f...f...d
-000002e0: 2d9c 0964 2e64 2f84 055a 2064 3665 056a  -..d.d/..Z d6e.j
-000002f0: 0665 0d65 056a 0619 0065 0d65 1f19 0065  .e.e.j...e.e...e
-00000300: 0d65 0f19 0065 1065 0b65 0f65 2164 309c  .e...e.e.e.e!d0.
-00000310: 0864 3164 3284 055a 2287 0004 005a 2353  .d1d2..Z"....Z#S
-00000320: 0029 37da 0e43 6f75 6e74 6572 6661 6374  .)7..Counterfact
-00000330: 7561 6ce7 0000 0000 0000 0000 e79a 9999  ual.............
-00000340: 9999 99b9 3fa9 0267 0000 0020 5fa0 02c2  ....?..g... _...
-00000350: e700 0000 205f a002 424e 46e7 7b14 ae47  .... _..BNF.{..G
-00000360: e17a 843f e9e8 0300 00e7 0000 0000 0000  .z.?............
-00000370: 2440 e90a 0000 00a9 02e7 fca9 f1d2 4d62  $@............Mb
-00000380: 503f 7216 0000 00a9 0267 0000 0000 0040  P?r......g.....@
-00000390: 8fc0 6700 0000 0000 408f 40e9 0100 0000  ..g.....@.@.....
-000003a0: 2915 da07 7072 6564 6963 74da 0f69 6e70  )...predict..inp
-000003b0: 7574 5f74 7261 6e73 666f 726d da05 7368  ut_transform..sh
-000003c0: 6170 65da 056b 6170 7061 da04 6265 7461  ape..kappa..beta
-000003d0: da0d 6665 6174 7572 655f 7261 6e67 65da  ..feature_range.
-000003e0: 0567 616d 6d61 da08 6165 5f6d 6f64 656c  .gamma..ae_model
-000003f0: da09 656e 635f 6d6f 6465 6cda 0574 6865  ..enc_model..the
-00000400: 7461 da0a 7573 655f 6b64 7472 6565 da12  ta..use_kdtree..
-00000410: 6c65 6172 6e69 6e67 5f72 6174 655f 696e  learning_rate_in
-00000420: 6974 da0e 6d61 785f 6974 6572 6174 696f  it..max_iteratio
-00000430: 6e73 da06 635f 696e 6974 da07 635f 7374  ns..c_init..c_st
-00000440: 6570 73da 0365 7073 da04 636c 6970 da0f  eps..eps..clip..
-00000450: 7570 6461 7465 5f6e 756d 5f67 7261 64da  update_num_grad.
-00000460: 0a74 7275 7374 7363 6f72 65da 0776 6572  .trustscore..ver
-00000470: 626f 7365 da06 7265 7475 726e 6315 0000  bose..returnc...
-00000480: 0000 0000 0000 0000 001b 0000 0005 0000  ................
-00000490: 0003 0000 0073 f001 0000 7400 8300 6a01  .....s....t...j.
-000004a0: 7402 a003 7404 a101 6401 8d01 0100 7405  t...t...d.....t.
-000004b0: 8801 8301 6402 6b04 723e 8801 6403 6404  ....d.k.r>..d.d.
-000004c0: 8502 1900 7d15 8801 6405 1900 8801 6406  ....}...d.....d.
-000004d0: 1900 6602 8901 6e04 8801 7d15 7406 8300  ..f...n...}.t...
-000004e0: 7d16 6700 6407 a201 7d17 7c17 4400 5d0e  }.g.d...}.|.D.].
-000004f0: 7d18 7c16 a007 7c18 a101 0100 7154 7c00  }.|...|.....qT|.
-00000500: 6a08 6408 1900 a009 7c16 a101 0100 7c01  j.d.....|.....|.
-00000510: 7c00 5f0a 7c13 7c00 5f0b 7c00 a00a 740c  |._.|.|._.|...t.
-00000520: 6a0d 8801 6409 8d01 a101 6a0e 6403 1900  j...d.....j.d...
-00000530: 7c00 5f0f 7410 7c08 740c 6a11 6a12 8302  |._.t.|.t.j.j...
-00000540: 7d19 7410 7c09 740c 6a11 6a12 8302 7d1a  }.t.|.t.j.j...}.
-00000550: 7c1a 72c2 640a 7c00 5f13 6e06 640b 7c00  |.r.d.|._.n.d.|.
-00000560: 5f13 7c19 72d4 640a 7c00 5f14 6e06 640b  _.|.r.d.|._.n.d.
-00000570: 7c00 5f14 7c0b 72ee 7c00 6a13 72ee 7415  |._.|.r.|.j.r.t.
-00000580: a016 640c a101 0100 7c0b 73fa 7c00 6a13  ..d.....|.s.|.j.
-00000590: 9001 7202 640a 7c00 5f17 6e06 640b 7c00  ..r.d.|._.n.d.|.
-000005a0: 5f17 7c00 6a08 6408 1900 6a09 7c00 6a17  _.|.j.d...j.|.j.
-000005b0: 640d 8d01 0100 8801 7c00 5f0e 7c15 7c00  d.......|._.|.|.
-000005c0: 5f18 7c04 7c00 5f19 7c05 7c00 5f1a 7c07  _.|.|._.|.|._.|.
-000005d0: 7c00 5f1b 7c0a 7c00 5f1c 7c08 7c00 5f1d  |._.|.|._.|.|._.
-000005e0: 7c09 7c00 5f1e 7c0b 7c00 5f1f 8801 6405  |.|._.|.|._...d.
-000005f0: 1900 7c00 5f20 7c0d 7c00 5f21 740c 6a22  ..|._ |.|._!t.j"
-00000600: 7c0e 740c 6a23 640e 8d02 7c00 5f24 7c0f  |.t.j#d...|._$|.
-00000610: 7c00 5f25 7426 8700 8701 6602 640f 6410  |._%t&....f.d.d.
-00000620: 8408 7427 6402 8301 4400 8301 8301 7c00  ..t'd...D.....|.
-00000630: 5f28 7c12 7c00 5f29 7c10 7c00 5f2a 7c11  _(|.|._)|.|._*|.
-00000640: 7c00 5f2b 7c02 7c00 5f2c 7c0c 7c00 5f2d  |._+|.|._,|.|._-
-00000650: 7c14 7c00 5f2e 7c00 6a13 9001 72de 7c00  |.|._.|.j...r.|.
-00000660: 6a1e a00a 742f a00d 7c00 6a0e a101 a101  j...t/..|.j.....
-00000670: 6a0e 7c00 5f30 6e08 7c00 6a0e 7c00 5f30  j.|._0n.|.j.|._0
-00000680: 7431 7415 5f32 6404 5300 2911 6147 0900  t1t._2d.S.).aG..
-00000690: 000a 2020 2020 2020 2020 496e 6974 6961  ..        Initia
-000006a0: 6c69 7a65 2070 726f 746f 7479 7069 6361  lize prototypica
-000006b0: 6c20 636f 756e 7465 7266 6163 7475 616c  l counterfactual
-000006c0: 206d 6574 686f 642e 0a0a 2020 2020 2020   method...      
-000006d0: 2020 5061 7261 6d65 7465 7273 0a20 2020    Parameters.   
-000006e0: 2020 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a       ----------.
-000006f0: 2020 2020 2020 2020 7072 6564 6963 740a          predict.
-00000700: 2020 2020 2020 2020 2020 2020 6070 7974              `pyt
-00000710: 6f72 6368 6020 6d6f 6465 6c27 7320 7072  orch` model's pr
-00000720: 6564 6963 7469 6f6e 2066 756e 6374 696f  ediction functio
-00000730: 6e20 7265 7475 726e 696e 6720 636c 6173  n returning clas
-00000740: 7320 7072 6f62 6162 696c 6974 6965 732e  s probabilities.
-00000750: 0a20 2020 2020 2020 2073 6861 7065 0a20  .        shape. 
-00000760: 2020 2020 2020 2020 2020 2053 6861 7065             Shape
-00000770: 206f 6620 696e 7075 7420 6461 7461 2073   of input data s
-00000780: 7461 7274 696e 6720 7769 7468 2062 6174  tarting with bat
-00000790: 6368 2073 697a 652e 0a20 2020 2020 2020  ch size..       
-000007a0: 206b 6170 7061 0a20 2020 2020 2020 2020   kappa.         
-000007b0: 2020 2043 6f6e 6669 6465 6e63 6520 7061     Confidence pa
-000007c0: 7261 6d65 7465 7220 666f 7220 7468 6520  rameter for the 
-000007d0: 6174 7461 636b 206c 6f73 7320 7465 726d  attack loss term
-000007e0: 2e0a 2020 2020 2020 2020 6265 7461 0a20  ..        beta. 
-000007f0: 2020 2020 2020 2020 2020 2052 6567 756c             Regul
-00000800: 6172 697a 6174 696f 6e20 636f 6e73 7461  arization consta
-00000810: 6e74 2066 6f72 204c 3120 6c6f 7373 2074  nt for L1 loss t
-00000820: 6572 6d2e 0a20 2020 2020 2020 2066 6561  erm..        fea
-00000830: 7475 7265 5f72 616e 6765 0a20 2020 2020  ture_range.     
-00000840: 2020 2020 2020 2054 7570 6c65 2077 6974         Tuple wit
-00000850: 6820 606d 696e 6020 616e 6420 606d 6178  h `min` and `max
-00000860: 6020 7261 6e67 6573 2074 6f20 616c 6c6f  ` ranges to allo
-00000870: 7720 666f 7220 7065 7274 7572 6265 6420  w for perturbed 
-00000880: 696e 7374 616e 6365 732e 2060 4d69 6e60  instances. `Min`
-00000890: 2061 6e64 2060 6d61 7860 2072 616e 6765   and `max` range
-000008a0: 7320 6361 6e20 6265 2060 666c 6f61 7460  s can be `float`
-000008b0: 0a20 2020 2020 2020 2020 2020 206f 7220  .            or 
-000008c0: 606e 756d 7079 6020 6172 7261 7973 2077  `numpy` arrays w
-000008d0: 6974 6820 6469 6d65 6e73 696f 6e20 2831  ith dimension (1
-000008e0: 7820 6e62 206f 6620 6665 6174 7572 6573  x nb of features
-000008f0: 2920 666f 7220 6665 6174 7572 652d 7769  ) for feature-wi
-00000900: 7365 2072 616e 6765 732e 0a20 2020 2020  se ranges..     
-00000910: 2020 2067 616d 6d61 0a20 2020 2020 2020     gamma.       
-00000920: 2020 2020 2052 6567 756c 6172 697a 6174       Regularizat
-00000930: 696f 6e20 636f 6e73 7461 6e74 2066 6f72  ion constant for
-00000940: 206f 7074 696f 6e61 6c20 6175 746f 2d65   optional auto-e
-00000950: 6e63 6f64 6572 206c 6f73 7320 7465 726d  ncoder loss term
-00000960: 2e0a 2020 2020 2020 2020 6165 5f6d 6f64  ..        ae_mod
-00000970: 656c 0a20 2020 2020 2020 2020 2020 204f  el.            O
-00000980: 7074 696f 6e61 6c20 6175 746f 2d65 6e63  ptional auto-enc
-00000990: 6f64 6572 206d 6f64 656c 2075 7365 6420  oder model used 
-000009a0: 666f 7220 6c6f 7373 2072 6567 756c 6172  for loss regular
-000009b0: 697a 6174 696f 6e2e 0a20 2020 2020 2020  ization..       
-000009c0: 2065 6e63 5f6d 6f64 656c 0a20 2020 2020   enc_model.     
-000009d0: 2020 2020 2020 204f 7074 696f 6e61 6c20         Optional 
-000009e0: 656e 636f 6465 7220 6d6f 6465 6c20 7573  encoder model us
-000009f0: 6564 2074 6f20 6775 6964 6520 696e 7374  ed to guide inst
-00000a00: 616e 6365 2070 6572 7475 7262 6174 696f  ance perturbatio
-00000a10: 6e73 2074 6f77 6172 6473 2061 2063 6c61  ns towards a cla
-00000a20: 7373 2070 726f 746f 7479 7065 2e0a 2020  ss prototype..  
-00000a30: 2020 2020 2020 7468 6574 610a 2020 2020        theta.    
-00000a40: 2020 2020 2020 2020 436f 6e73 7461 6e74          Constant
-00000a50: 2066 6f72 2074 6865 2070 726f 746f 7479   for the prototy
-00000a60: 7065 2073 6561 7263 6820 6c6f 7373 2074  pe search loss t
-00000a70: 6572 6d2e 0a20 2020 2020 2020 2075 7365  erm..        use
-00000a80: 5f6b 6474 7265 650a 2020 2020 2020 2020  _kdtree.        
-00000a90: 2020 2020 5768 6574 6865 7220 746f 2075      Whether to u
-00000aa0: 7365 206b 2d64 2074 7265 6573 2066 6f72  se k-d trees for
-00000ab0: 2074 6865 2070 726f 746f 7479 7065 206c   the prototype l
-00000ac0: 6f73 7320 7465 726d 2069 6620 6e6f 2065  oss term if no e
-00000ad0: 6e63 6f64 6572 2069 7320 6176 6169 6c61  ncoder is availa
-00000ae0: 626c 652e 0a20 2020 2020 2020 206c 6561  ble..        lea
-00000af0: 726e 696e 675f 7261 7465 5f69 6e69 740a  rning_rate_init.
-00000b00: 2020 2020 2020 2020 2020 2020 496e 6974              Init
-00000b10: 6961 6c20 6c65 6172 6e69 6e67 2072 6174  ial learning rat
-00000b20: 6520 6f66 206f 7074 696d 697a 6572 2e0a  e of optimizer..
-00000b30: 2020 2020 2020 2020 6d61 785f 6974 6572          max_iter
-00000b40: 6174 696f 6e73 0a20 2020 2020 2020 2020  ations.         
-00000b50: 2020 204d 6178 696d 756d 206e 756d 6265     Maximum numbe
-00000b60: 7220 6f66 2069 7465 7261 7469 6f6e 7320  r of iterations 
-00000b70: 666f 7220 6669 6e64 696e 6720 6120 636f  for finding a co
-00000b80: 756e 7465 7266 6163 7475 616c 2e0a 2020  unterfactual..  
-00000b90: 2020 2020 2020 635f 696e 6974 0a20 2020        c_init.   
-00000ba0: 2020 2020 2020 2020 2049 6e69 7469 616c           Initial
-00000bb0: 2076 616c 7565 2074 6f20 7363 616c 6520   value to scale 
-00000bc0: 7468 6520 6174 7461 636b 206c 6f73 7320  the attack loss 
-00000bd0: 7465 726d 2e0a 2020 2020 2020 2020 635f  term..        c_
-00000be0: 7374 6570 730a 2020 2020 2020 2020 2020  steps.          
-00000bf0: 2020 4e75 6d62 6572 206f 6620 6974 6572    Number of iter
-00000c00: 6174 696f 6e73 2074 6f20 6164 6a75 7374  ations to adjust
-00000c10: 2074 6865 2063 6f6e 7374 616e 7420 7363   the constant sc
-00000c20: 616c 696e 6720 7468 6520 6174 7461 636b  aling the attack
-00000c30: 206c 6f73 7320 7465 726d 2e0a 2020 2020   loss term..    
-00000c40: 2020 2020 6570 730a 2020 2020 2020 2020      eps.        
-00000c50: 2020 2020 4966 206e 756d 6572 6963 616c      If numerical
-00000c60: 2067 7261 6469 656e 7473 2061 7265 2075   gradients are u
-00000c70: 7365 6420 746f 2063 6f6d 7075 7465 2060  sed to compute `
-00000c80: 644c 2f64 7820 3d20 2864 4c2f 6470 2920  dL/dx = (dL/dp) 
-00000c90: 2a20 2864 702f 6478 2960 2c20 7468 656e  * (dp/dx)`, then
-00000ca0: 2060 6570 735b 305d 6020 6973 2075 7365   `eps[0]` is use
-00000cb0: 6420 746f 0a20 2020 2020 2020 2020 2020  d to.           
-00000cc0: 2063 616c 6375 6c61 7465 2060 644c 2f64   calculate `dL/d
-00000cd0: 7060 2061 6e64 2060 6570 735b 315d 6020  p` and `eps[1]` 
-00000ce0: 6973 2075 7365 6420 666f 7220 6064 702f  is used for `dp/
-00000cf0: 6478 602e 2060 6570 735b 305d 6020 616e  dx`. `eps[0]` an
-00000d00: 6420 6065 7073 5b31 5d60 2063 616e 2062  d `eps[1]` can b
-00000d10: 6520 6120 636f 6d62 696e 6174 696f 6e20  e a combination 
-00000d20: 6f66 2060 666c 6f61 7460 0a20 2020 2020  of `float`.     
-00000d30: 2020 2020 2020 2076 616c 7565 7320 616e         values an
-00000d40: 6420 606e 756d 7079 6020 6172 7261 7973  d `numpy` arrays
-00000d50: 2e20 466f 7220 6065 7073 5b30 5d60 2c20  . For `eps[0]`, 
-00000d60: 7468 6520 6172 7261 7920 6469 6d65 6e73  the array dimens
-00000d70: 696f 6e20 7368 6f75 6c64 2062 6520 2831  ion should be (1
-00000d80: 7820 6e62 206f 6620 7072 6564 6963 7469  x nb of predicti
-00000d90: 6f6e 2063 6174 6567 6f72 6965 7329 0a20  on categories). 
-00000da0: 2020 2020 2020 2020 2020 2061 6e64 2066             and f
-00000db0: 6f72 2060 6570 735b 315d 6020 6974 2073  or `eps[1]` it s
-00000dc0: 686f 756c 6420 6265 2028 3178 206e 6220  hould be (1x nb 
-00000dd0: 6f66 2066 6561 7475 7265 7329 2e0a 2020  of features)..  
-00000de0: 2020 2020 2020 636c 6970 0a20 2020 2020        clip.     
-00000df0: 2020 2020 2020 2054 7570 6c65 2077 6974         Tuple wit
-00000e00: 6820 6d69 6e20 616e 6420 6d61 7820 636c  h min and max cl
-00000e10: 6970 2072 616e 6765 7320 666f 7220 626f  ip ranges for bo
-00000e20: 7468 2074 6865 206e 756d 6572 6963 616c  th the numerical
-00000e30: 2067 7261 6469 656e 7473 2061 6e64 2074   gradients and t
-00000e40: 6865 2067 7261 6469 656e 7473 0a20 2020  he gradients.   
-00000e50: 2020 2020 2020 2020 206f 6274 6169 6e65           obtaine
-00000e60: 6420 6672 6f6d 2074 6865 2060 7465 6e73  d from the `tens
-00000e70: 6f72 666c 6f77 6020 6772 6170 682e 0a20  orflow` graph.. 
-00000e80: 2020 2020 2020 2075 7064 6174 655f 6e75         update_nu
-00000e90: 6d5f 6772 6164 0a20 2020 2020 2020 2020  m_grad.         
-00000ea0: 2020 2049 6620 6e75 6d65 7269 6361 6c20     If numerical 
-00000eb0: 6772 6164 6965 6e74 7320 6172 6520 7573  gradients are us
-00000ec0: 6564 2c20 7468 6579 2077 696c 6c20 6265  ed, they will be
-00000ed0: 2075 7064 6174 6564 2065 7665 7279 2060   updated every `
-00000ee0: 7570 6461 7465 5f6e 756d 5f67 7261 6460  update_num_grad`
-00000ef0: 2069 7465 7261 7469 6f6e 732e 0a20 2020   iterations..   
-00000f00: 2020 2020 2074 7275 7374 7363 6f72 650a       trustscore.
-00000f10: 2020 2020 2020 2020 2020 2020 4469 7265              Dire
-00000f20: 6374 6f72 7920 7768 6572 6520 7472 7573  ctory where trus
-00000f30: 7473 636f 7265 206f 626a 6563 7420 6973  tscore object is
-00000f40: 2074 6f20 6265 2075 7365 640a 2020 2020   to be used.    
-00000f50: 2020 2020 7365 7373 0a20 2020 2020 2020      sess.       
-00000f60: 2020 2020 204f 7074 696f 6e61 6c20 6074       Optional `t
-00000f70: 656e 736f 7266 6c6f 7760 2073 6573 7369  ensorflow` sessi
-00000f80: 6f6e 2074 6861 7420 7769 6c6c 2062 6520  on that will be 
-00000f90: 7573 6564 2069 6620 7061 7373 6564 2069  used if passed i
-00000fa0: 6e73 7465 6164 206f 6620 6372 6561 7469  nstead of creati
-00000fb0: 6e67 206f 7220 696e 6665 7272 696e 6720  ng or inferring 
-00000fc0: 6f6e 6520 696e 7465 726e 616c 6c79 2e0a  one internally..
-00000fd0: 2020 2020 2020 2020 2901 da04 6d65 7461          )...meta
-00000fe0: 7206 0000 0072 1800 0000 4e72 0100 0000  r....r....Nr....
-00000ff0: e9ff ffff ff29 06da 0473 656c 6672 1900  .....)...selfr..
-00001000: 0000 721a 0000 0072 2000 0000 7221 0000  ..r....r ...r!..
-00001010: 00da 095f 5f63 6c61 7373 5f5f da06 7061  ...__class__..pa
-00001020: 7261 6d73 2901 da04 7369 7a65 5446 7a55  rams)...sizeTFzU
-00001030: 426f 7468 2061 6e20 656e 636f 6465 7220  Both an encoder 
-00001040: 616e 6420 6b2d 6420 7472 6565 7320 656e  and k-d trees en
-00001050: 6162 6c65 642e 2055 7369 6e67 2074 6865  abled. Using the
-00001060: 2065 6e63 6f64 6572 2066 6f72 2074 6865   encoder for the
-00001070: 2070 726f 746f 7479 7065 206c 6f73 7320   prototype loss 
-00001080: 7465 726d 2e29 01da 0d65 6e63 5f6f 725f  term.)...enc_or_
-00001090: 6b64 7472 6565 a901 da05 6474 7970 6563  kdtree....dtypec
-000010a0: 0100 0000 0000 0000 0000 0000 0200 0000  ................
-000010b0: 0700 0000 1300 0000 7348 0000 0067 007c  ........sH...g.|
-000010c0: 005d 407d 0174 0088 007c 0119 0074 0183  .]@}.t...|...t..
-000010d0: 0272 3c74 02a0 0388 0164 0064 0185 0219  .r<t.....d.d....
-000010e0: 00a1 0188 007c 0119 0014 0064 0164 0164  .....|.....d.d.d
-000010f0: 0185 0266 0219 006e 0688 007c 0119 0091  ...f...n...|....
-00001100: 0271 0453 0029 0272 1800 0000 4e29 04da  .q.S.).r....N)..
-00001110: 0a69 7369 6e73 7461 6e63 65da 0566 6c6f  .isinstance..flo
-00001120: 6174 da05 746f 7263 68da 046f 6e65 7329  at..torch..ones)
-00001130: 02da 022e 30da 015f a902 721e 0000 0072  ....0.._..r....r
-00001140: 1b00 0000 a900 fa50 2f63 656e 7472 616c  .......P/central
-00001150: 2f68 6f6d 652f 7a77 616e 6732 2f6d 6f72  /home/zwang2/mor
-00001160: 7068 6575 732d 7370 6174 6961 6c2f 6d6f  pheus-spatial/mo
-00001170: 7270 6865 7573 2f73 7263 2f6d 6f72 7068  rpheus/src/morph
-00001180: 6575 732f 636f 756e 7465 7266 6163 7475  eus/counterfactu
-00001190: 616c 2f63 662e 7079 da0a 3c6c 6973 7463  al/cf.py..<listc
-000011a0: 6f6d 703e 9d00 0000 7308 0000 0006 0602  omp>....s.......
-000011b0: fd0c ff28 027a 2b43 6f75 6e74 6572 6661  ...(.z+Counterfa
-000011c0: 6374 7561 6c2e 5f5f 696e 6974 5f5f 2e3c  ctual.__init__.<
-000011d0: 6c6f 6361 6c73 3e2e 3c6c 6973 7463 6f6d  locals>.<listcom
-000011e0: 703e 2933 da05 7375 7065 72da 085f 5f69  p>)3..super..__i
-000011f0: 6e69 745f 5fda 0463 6f70 79da 0864 6565  nit__..copy..dee
-00001200: 7063 6f70 7972 0800 0000 da03 6c65 6eda  pcopyr......len.
-00001210: 066c 6f63 616c 73da 0370 6f70 722e 0000  .locals..popr...
-00001220: 00da 0675 7064 6174 6572 1900 0000 722b  ...updater....r+
-00001230: 0000 0072 3900 0000 da05 7a65 726f 7372  ...r9.....zerosr
-00001240: 1b00 0000 da07 636c 6173 7365 7372 3700  ......classesr7.
-00001250: 0000 da02 6e6e da06 4d6f 6475 6c65 7221  ....nn..Moduler!
-00001260: 0000 0072 2000 0000 da08 7761 726e 696e  ...r .....warnin
-00001270: 6773 da04 7761 726e 7234 0000 00da 0b70  gs..warnr4.....p
-00001280: 6174 6368 5f73 6861 7065 721c 0000 0072  atch_shaper....r
-00001290: 1d00 0000 721f 0000 0072 2200 0000 da02  ....r....r".....
-000012a0: 6165 da03 656e 6372 2300 0000 da0a 6261  ae..encr#.....ba
-000012b0: 7463 685f 7369 7a65 7225 0000 00da 0674  tch_sizer%.....t
-000012c0: 656e 736f 72da 0766 6c6f 6174 3332 7226  ensor..float32r&
-000012d0: 0000 0072 2700 0000 da05 7475 706c 65da  ...r'.....tuple.
-000012e0: 0572 616e 6765 721e 0000 0072 2a00 0000  .ranger....r*...
-000012f0: 7228 0000 0072 2900 0000 721a 0000 0072  r(...r)...r....r
-00001300: 2400 0000 722c 0000 00da 026e 70da 0973  $...r,.....np..s
-00001310: 6861 7065 5f65 6e63 da0e 7369 6d70 6c65  hape_enc..simple
-00001320: 5f77 6172 6e69 6e67 da0b 7368 6f77 7761  _warning..showwa
-00001330: 726e 696e 6729 1b72 3000 0000 7219 0000  rning).r0...r...
-00001340: 0072 1a00 0000 721b 0000 0072 1c00 0000  .r....r....r....
-00001350: 721d 0000 0072 1e00 0000 721f 0000 0072  r....r....r....r
-00001360: 2000 0000 7221 0000 0072 2200 0000 7223   ...r!...r"...r#
-00001370: 0000 0072 2400 0000 7225 0000 0072 2600  ...r$...r%...r&.
-00001380: 0000 7227 0000 0072 2800 0000 7229 0000  ..r'...r(...r)..
-00001390: 0072 2a00 0000 722b 0000 0072 2c00 0000  .r*...r+...r,...
-000013a0: 724f 0000 0072 3200 0000 da06 7265 6d6f  rO...r2.....remo
-000013b0: 7665 da03 6b65 795a 0569 735f 6165 5a06  ve..keyZ.is_aeZ.
-000013c0: 6973 5f65 6e63 a901 7231 0000 0072 3d00  is_enc..r1...r=.
-000013d0: 0000 723f 0000 0072 4200 0000 1200 0000  ..r?...rB.......
-000013e0: 7376 0000 0000 4b14 030c 0102 0106 ff04  sv....K.........
-000013f0: 0312 0204 0106 0108 0808 010c 0110 0106  ................
-00001400: 0106 011a 020e 010e 0204 0108 0206 0204  ................
-00001410: 0108 0206 020a 0104 0102 ff04 040c 0108  ................
-00001420: 0206 0114 0206 0106 0106 0106 0106 0106  ................
-00001430: 0106 0106 0106 010a 0106 0112 0106 0102  ................
-00001440: 010c 0606 fa04 ff06 0a06 0106 0106 0106  ................
-00001450: 0106 0106 0308 011a 0308 037a 1743 6f75  ...........z.Cou
-00001460: 6e74 6572 6661 6374 7561 6c2e 5f5f 696e  nterfactual.__in
-00001470: 6974 5f5f 6302 0000 0000 0000 0000 0000  it__c...........
-00001480: 0007 0000 0005 0000 0043 0000 0073 9a00  .........C...s..
-00001490: 0000 7c00 6a00 7c00 6a01 1800 7c00 6a02  ..|.j.|.j...|.j.
-000014a0: 6b04 7d02 7403 a004 7c00 6a00 7c00 6a01  k.}.t...|.j.|.j.
-000014b0: 1800 a101 7c00 6a02 6b01 7d03 7c00 6a00  ....|.j.k.}.|.j.
-000014c0: 7c00 6a01 1800 7c00 6a02 0b00 6b00 7d04  |.j...|.j...k.}.
-000014d0: 7403 a005 7c00 6a00 7c00 6a02 1800 7c01  t...|.j.|.j...|.
-000014e0: 6401 1900 a102 7d05 7403 a006 7c00 6a00  d.....}.t...|.j.
-000014f0: 7c00 6a02 1700 7c01 6402 1900 a102 7d06  |.j...|.d.....}.
-00001500: 7c02 a007 a100 7c05 1400 7c03 a007 a100  |.....|...|.....
-00001510: 7c00 6a01 1400 1700 7c04 a007 a100 7c06  |.j.....|.....|.
-00001520: 1400 1700 7c00 5f08 6400 5300 2903 4e72  ....|._.d.S.).Nr
-00001530: 1800 0000 7201 0000 0029 09da 0561 6476  ....r....)...adv
-00001540: 5f73 da04 6f72 6967 721d 0000 0072 3900  _s..origr....r9.
-00001550: 0000 da03 6162 73da 036d 696e da03 6d61  ....abs..min..ma
-00001560: 7872 3800 0000 da0a 6173 7369 676e 5f61  xr8.....assign_a
-00001570: 6476 2907 7230 0000 0072 1e00 0000 5a06  dv).r0...r....Z.
-00001580: 636f 6e64 5f30 5a06 636f 6e64 5f31 5a06  cond_0Z.cond_1Z.
-00001590: 636f 6e64 5f32 da05 7570 7065 72da 056c  cond_2..upper..l
-000015a0: 6f77 6572 723e 0000 0072 3e00 0000 723f  owerr>...r>...r?
-000015b0: 0000 00da 1e63 6f6d 7075 7465 5f73 6872  .....compute_shr
-000015c0: 696e 6b61 6765 5f74 6872 6573 686f 6c64  inkage_threshold
-000015d0: 696e 67b7 0000 0073 0e00 0000 0002 1201  ing....s........
-000015e0: 1801 1403 1801 1804 24ff 7a2d 436f 756e  ........$.z-Coun
-000015f0: 7465 7266 6163 7475 616c 2e63 6f6d 7075  terfactual.compu
-00001600: 7465 5f73 6872 696e 6b61 6765 5f74 6872  te_shrinkage_thr
-00001610: 6573 686f 6c64 696e 6763 0100 0000 0000  esholdingc......
-00001620: 0000 0000 0000 0100 0000 0600 0000 4300  ..............C.
-00001630: 0000 734e 0000 007c 006a 007c 006a 0064  ..sN...|.j.|.j.d
-00001640: 0117 001b 007c 005f 017c 006a 027c 006a  .....|._.|.j.|.j
-00001650: 017c 006a 027c 006a 0318 0014 0017 007c  .|.j.|.j.......|
-00001660: 005f 0474 05a0 067c 006a 047c 006a 0764  ._.t...|.j.|.j.d
-00001670: 0219 007c 006a 0764 0319 00a1 037c 005f  ...|.j.d.....|._
-00001680: 0464 0053 0029 044e 6700 0000 0000 0008  .d.S.).Ng.......
-00001690: 4072 0100 0000 7218 0000 0029 08da 0b67  @r....r....)...g
-000016a0: 6c6f 6261 6c5f 7374 6570 da02 7a74 7263  lobal_step..ztrc
-000016b0: 0000 00da 0361 6476 da0c 6173 7369 676e  .....adv..assign
-000016c0: 5f61 6476 5f73 7239 0000 00da 0563 6c61  _adv_sr9.....cla
-000016d0: 6d70 721e 0000 00a9 0172 3000 0000 723e  mpr......r0...r>
-000016e0: 0000 0072 3e00 0000 723f 0000 00da 1f63  ...r>...r?.....c
-000016f0: 6f6d 7075 7465 5f70 6572 7475 7262 6174  ompute_perturbat
-00001700: 696f 6e5f 7072 6f6a 6563 7469 6f6e c600  ion_projection..
-00001710: 0000 730a 0000 0000 0212 011a 0304 0114  ..s.............
-00001720: ff7a 2e43 6f75 6e74 6572 6661 6374 7561  .z.Counterfactua
-00001730: 6c2e 636f 6d70 7574 655f 7065 7274 7572  l.compute_pertur
-00001740: 6261 7469 6f6e 5f70 726f 6a65 6374 696f  bation_projectio
-00001750: 6e63 0100 0000 0000 0000 0000 0000 0100  nc..............
-00001760: 0000 0200 0000 4300 0000 7320 0000 007c  ......C...s ...|
-00001770: 006a 00a0 01a1 007c 005f 027c 006a 036a  .j.....|._.|.j.j
-00001780: 04a0 01a1 007c 006a 055f 0464 0053 00a9  .....|.j._.d.S..
-00001790: 014e 2906 7263 0000 00da 0563 6c6f 6e65  .N).rc.....clone
-000017a0: 7269 0000 0072 6a00 0000 da04 6461 7461  ri...rj.....data
-000017b0: 725e 0000 0072 6c00 0000 723e 0000 0072  r^...rl...r>...r
-000017c0: 3e00 0000 723f 0000 00da 1675 7064 6174  >...r?.....updat
-000017d0: 655f 636f 756e 7465 7266 6163 7475 616c  e_counterfactual
-000017e0: 73d0 0000 0073 0400 0000 0002 0c01 7a25  s....s........z%
-000017f0: 436f 756e 7465 7266 6163 7475 616c 2e75  Counterfactual.u
-00001800: 7064 6174 655f 636f 756e 7465 7266 6163  pdate_counterfac
-00001810: 7475 616c 7363 0100 0000 0000 0000 0000  tualsc..........
-00001820: 0000 0100 0000 0200 0000 4300 0000 7320  ..........C...s 
-00001830: 0000 007c 006a 007c 006a 0118 007c 005f  ...|.j.|.j...|._
-00001840: 027c 006a 007c 006a 0318 007c 005f 0464  .|.j.|.j...|._.d
-00001850: 0053 0072 6e00 0000 2905 725f 0000 0072  .S.rn...).r_...r
-00001860: 6900 0000 da05 6465 6c74 6172 5e00 0000  i.....deltar^...
-00001870: da07 6465 6c74 615f 7372 6c00 0000 723e  ..delta_srl...r>
-00001880: 0000 0072 3e00 0000 723f 0000 00da 1263  ...r>...r?.....c
-00001890: 6f6d 7075 7465 5f64 6576 6961 7469 6f6e  ompute_deviation
-000018a0: 73d5 0000 0073 0400 0000 0002 0e01 7a21  s....s........z!
-000018b0: 436f 756e 7465 7266 6163 7475 616c 2e63  Counterfactual.c
-000018c0: 6f6d 7075 7465 5f64 6576 6961 7469 6f6e  ompute_deviation
-000018d0: 7363 0200 0000 0000 0000 0000 0000 0300  sc..............
-000018e0: 0000 0500 0000 4300 0000 73da 0000 007c  ......C...s....|
-000018f0: 00a0 00a1 0001 0074 0174 0264 0174 037c  .......t.t.d.t.|
-00001900: 0183 0183 0283 017d 0274 046a 057c 006a  .......}.t.j.|.j
-00001910: 0664 0213 007c 0264 038d 027c 005f 0774  .d...|.d...|._.t
-00001920: 046a 057c 006a 0864 0213 007c 0264 038d  .j.|.j.d...|.d..
-00001930: 027c 005f 0974 046a 0574 04a0 0a7c 006a  .|._.t.j.t...|.j
-00001940: 06a1 017c 0264 038d 027c 005f 0b74 046a  ...|.d...|._.t.j
-00001950: 0574 04a0 0a7c 006a 08a1 017c 0264 038d  .t...|.j...|.d..
-00001960: 027c 005f 0c7c 006a 077c 006a 0b7c 006a  .|._.|.j.|.j.|.j
-00001970: 0d14 0017 007c 005f 0e7c 006a 097c 006a  .....|._.|.j.|.j
-00001980: 0c7c 006a 0d14 0017 007c 005f 0f74 04a0  .|.j.....|._.t..
-00001990: 057c 006a 0ba1 017c 005f 1074 04a0 057c  .|.j...|._.t...|
-000019a0: 006a 0ca1 017c 005f 1174 04a0 057c 006a  .j...|._.t...|.j
-000019b0: 07a1 017c 005f 1274 04a0 057c 006a 09a1  ...|._.t...|.j..
-000019c0: 017c 005f 1364 0053 0029 044e 7218 0000  .|._.d.S.).Nr...
-000019d0: 0072 0600 0000 a901 da03 6469 6d29 1472  .r........dim).r
-000019e0: 7400 0000 7255 0000 0072 5600 0000 7245  t...rU...rV...rE
-000019f0: 0000 0072 3900 0000 da03 7375 6d72 7200  ...r9.....sumrr.
-00001a00: 0000 da02 6c32 7273 0000 005a 046c 325f  ....l2rs...Z.l2_
-00001a10: 7372 6000 0000 da02 6c31 5a04 6c31 5f73  sr`.....l1Z.l1_s
-00001a20: 721d 0000 00da 056c 315f 6c32 5a07 6c31  r......l1_l2Z.l1
-00001a30: 5f6c 325f 73da 076c 6f73 735f 6c31 5a09  _l2_s..loss_l1Z.
-00001a40: 6c6f 7373 5f6c 315f 73da 076c 6f73 735f  loss_l1_s..loss_
-00001a50: 6c32 da09 6c6f 7373 5f6c 325f 7329 0372  l2..loss_l2_s).r
-00001a60: 3000 0000 721b 0000 005a 0661 785f 7375  0...r....Z.ax_su
-00001a70: 6d72 3e00 0000 723e 0000 0072 3f00 0000  mr>...r>...r?...
-00001a80: da14 636f 6d70 7574 655f 6c31 5f6c 325f  ..compute_l1_l2_
-00001a90: 6c6f 7373 6573 da00 0000 7318 0000 0000  losses....s.....
-00001aa0: 0208 0212 0216 0116 0218 0118 0214 0114  ................
-00001ab0: 030e 010e 010e 017a 2343 6f75 6e74 6572  .......z#Counter
-00001ac0: 6661 6374 7561 6c2e 636f 6d70 7574 655f  factual.compute_
-00001ad0: 6c31 5f6c 325f 6c6f 7373 6573 6301 0000  l1_l2_lossesc...
-00001ae0: 0000 0000 0000 0000 0001 0000 0005 0000  ................
-00001af0: 0043 0000 0073 7c00 0000 7c00 6a00 7260  .C...s|...|.j.r`
-00001b00: 7c00 a001 7c00 6a02 a101 7c00 5f03 7c00  |...|.j...|._.|.
-00001b10: a001 7c00 6a04 a101 7c00 5f05 7c00 6a06  ..|.j...|._.|.j.
-00001b20: 7407 a008 7c00 6a03 7c00 6a02 1800 a101  t...|.j.|.j.....
-00001b30: 6401 1300 1400 7c00 5f09 7c00 6a06 7407  d.....|._.|.j.t.
-00001b40: a008 7c00 6a05 7c00 6a04 1800 a101 6401  ..|.j.|.j.....d.
-00001b50: 1300 1400 7c00 5f0a 6e18 7407 a00b 6402  ....|._.n.t...d.
-00001b60: a101 7c00 5f09 7407 a00b 6402 a101 7c00  ..|._.t...d...|.
-00001b70: 5f0a 6400 5300 2903 4e72 0600 0000 720d  _.d.S.).Nr....r.
-00001b80: 0000 0029 0c72 2000 0000 7250 0000 0072  ...).r ...rP...r
-00001b90: 6900 0000 5a06 6164 765f 6165 725e 0000  i...Z.adv_aer^..
-00001ba0: 005a 0861 6476 5f61 655f 7372 1f00 0000  .Z.adv_ae_sr....
-00001bb0: 7239 0000 00da 046e 6f72 6dda 076c 6f73  r9.....norm..los
-00001bc0: 735f 6165 da09 6c6f 7373 5f61 655f 7372  s_ae..loss_ae_sr
-00001bd0: 5300 0000 726c 0000 0072 3e00 0000 723e  S...rl...r>...r>
-00001be0: 0000 0072 3f00 0000 da18 636f 6d70 7574  ...r?.....comput
-00001bf0: 655f 6175 746f 656e 636f 6465 725f 6c6f  e_autoencoder_lo
-00001c00: 7373 ef00 0000 730e 0000 0000 0206 020e  ss....s.........
-00001c10: 010e 021e 0120 020c 017a 2743 6f75 6e74  ..... ...z'Count
-00001c20: 6572 6661 6374 7561 6c2e 636f 6d70 7574  erfactual.comput
-00001c30: 655f 6175 746f 656e 636f 6465 725f 6c6f  e_autoencoder_lo
-00001c40: 7373 6301 0000 0000 0000 0000 0000 0005  ssc.............
-00001c50: 0000 0005 0000 0043 0000 0073 5001 0000  .......C...sP...
-00001c60: 7c00 6a00 6401 6b02 724c 7c00 6a01 6402  |.j.d.k.rL|.j.d.
-00001c70: 6b02 724c 7c00 a002 7c00 6a03 a101 7c00  k.rL|...|.j...|.
-00001c80: 5f04 7c00 a002 7c00 6a05 a101 7c00 5f06  _.|...|.j...|._.
-00001c90: 7407 a008 6401 a101 7c00 5f09 7407 a008  t...d...|._.t...
-00001ca0: 6401 a101 7c00 5f0a 9001 6e00 7c00 a002  d...|._...n.|...
-00001cb0: 7c00 6a03 a101 7c00 5f04 7c00 a002 7c00  |.j...|._.|...|.
-00001cc0: 6a05 a101 7c00 5f06 7407 6a0b 7c00 6a0c  j...|._.t.j.|.j.
-00001cd0: 7c00 6a04 1400 6402 6403 8d02 7c00 5f0d  |.j...d.d...|._.
-00001ce0: 7407 6a0b 7c00 6a0c 7c00 6a06 1400 6402  t.j.|.j.|.j...d.
-00001cf0: 6403 8d02 7d01 7407 6a0e 6402 7c00 6a0c  d...}.t.j.d.|.j.
-00001d00: 1800 7c00 6a04 1400 7c00 6a0c 6404 1400  ..|.j...|.j.d...
-00001d10: 1800 6402 6403 8d02 6405 1900 7c00 5f0f  ..d.d...d...|._.
-00001d20: 7407 6a0e 6402 7c00 6a0c 1800 7c00 6a06  t.j.d.|.j...|.j.
-00001d30: 1400 7c00 6a0c 6404 1400 1800 6402 6403  ..|.j.d.....d.d.
-00001d40: 8d02 6405 1900 7d02 7407 a010 7407 a008  ..d...}.t...t...
-00001d50: 6401 a101 7c00 6a0f 0b00 7c00 6a0d 1700  d...|.j...|.j...
-00001d60: 7c00 6a11 1700 a102 7d03 7407 a010 7407  |.j.....}.t...t.
-00001d70: a008 6401 a101 7c02 0b00 7c01 1700 7c00  ..d...|...|...|.
-00001d80: 6a11 1700 a102 7d04 7407 a00b 7c00 6a12  j.....}.t...|.j.
-00001d90: 7c03 1400 a101 7c00 5f09 7407 a00b 7c00  |.....|._.t...|.
-00001da0: 6a12 7c04 1400 a101 7c00 5f0a 6400 5300  j.|.....|._.d.S.
-00001db0: 2906 4e72 0d00 0000 7218 0000 0072 7500  ).Nr....r....ru.
-00001dc0: 0000 6910 2700 0072 0100 0000 2913 7226  ..i.'..r....).r&
-00001dd0: 0000 0072 2700 0000 7219 0000 0072 6900  ...r'...r....ri.
-00001de0: 0000 da0a 7072 6564 5f70 726f 6261 725e  ....pred_probar^
-00001df0: 0000 005a 0c70 7265 645f 7072 6f62 615f  ...Z.pred_proba_
-00001e00: 7372 3900 0000 7253 0000 00da 0b6c 6f73  sr9...rS.....los
-00001e10: 735f 6174 7461 636b da0d 6c6f 7373 5f61  s_attack..loss_a
-00001e20: 7474 6163 6b5f 7372 7700 0000 da06 7461  ttack_srw.....ta
-00001e30: 7267 6574 da0c 7461 7267 6574 5f70 726f  rget..target_pro
-00001e40: 6261 7262 0000 00da 136e 6f6e 7461 7267  barb.....nontarg
-00001e50: 6574 5f70 726f 6261 5f6d 6178 da07 6d61  et_proba_max..ma
-00001e60: 7869 6d75 6d72 1c00 0000 da05 636f 6e73  ximumr......cons
-00001e70: 7429 0572 3000 0000 5a0e 7461 7267 6574  t).r0...Z.target
-00001e80: 5f70 726f 6261 5f73 5a15 6e6f 6e74 6172  _proba_sZ.nontar
-00001e90: 6765 745f 7072 6f62 615f 6d61 785f 7372  get_proba_max_sr
-00001ea0: 8400 0000 7285 0000 0072 3e00 0000 723e  ....r....r>...r>
-00001eb0: 0000 0072 3f00 0000 da13 636f 6d70 7574  ...r?.....comput
-00001ec0: 655f 6174 7461 636b 5f6c 6f73 73fc 0000  e_attack_loss...
-00001ed0: 0073 3800 0000 0001 1401 0e01 0e02 0c01  .s8.............
-00001ee0: 1002 0e01 0e03 1801 1603 0401 1aff 0402  ................
-00001ef0: 02fe 0603 0401 1aff 0402 02fe 0405 0401  ................
-00001f00: 0801 12fe 0404 0401 16ff 0405 1201 7a22  ..............z"
-00001f10: 436f 756e 7465 7266 6163 7475 616c 2e63  Counterfactual.c
-00001f20: 6f6d 7075 7465 5f61 7474 6163 6b5f 6c6f  ompute_attack_lo
-00001f30: 7373 6301 0000 0000 0000 0000 0000 0001  ssc.............
-00001f40: 0000 0006 0000 0043 0000 0073 b000 0000  .......C...s....
-00001f50: 7c00 6a00 7250 7c00 6a01 7402 a003 7c00  |.j.rP|.j.t...|.
-00001f60: a004 7c00 6a05 a101 7c00 6a06 1800 a101  ..|.j...|.j.....
-00001f70: 6401 1300 1400 7c00 5f07 7c00 6a01 7402  d.....|._.|.j.t.
-00001f80: a003 7c00 a004 7c00 6a08 a101 7c00 6a06  ..|...|.j...|.j.
-00001f90: 1800 a101 6401 1300 1400 7c00 5f09 6e5c  ....d.....|._.n\
-00001fa0: 7c00 6a0a 7294 7c00 6a01 7402 a003 7c00  |.j.r.|.j.t...|.
-00001fb0: 6a05 7c00 6a06 1800 a101 6401 1300 1400  j.|.j.....d.....
-00001fc0: 7c00 5f07 7c00 6a01 7402 a003 7c00 6a08  |._.|.j.t...|.j.
-00001fd0: 7c00 6a06 1800 a101 6401 1300 1400 7c00  |.j.....d.....|.
-00001fe0: 5f09 6e18 7402 a00b 6402 a101 7c00 5f07  _.n.t...d...|._.
-00001ff0: 7402 a00b 6402 a101 7c00 5f09 6403 5300  t...d...|._.d.S.
-00002000: 2904 7a1b 436f 6d70 7574 6520 7468 6520  ).z.Compute the 
-00002010: 7072 6f74 6f74 7970 6520 6c6f 7373 2e72  prototype loss.r
-00002020: 0600 0000 720d 0000 004e 290c 7221 0000  ....r....N).r!..
-00002030: 0072 2200 0000 7239 0000 0072 7f00 0000  .r"...r9...r....
-00002040: 7251 0000 0072 6900 0000 da0c 7461 7267  rQ...ri.....targ
-00002050: 6574 5f70 726f 746f da0a 6c6f 7373 5f70  et_proto..loss_p
-00002060: 726f 746f 725e 0000 00da 0c6c 6f73 735f  rotor^.....loss_
-00002070: 7072 6f74 6f5f 7372 2300 0000 7253 0000  proto_sr#...rS..
-00002080: 0072 6c00 0000 723e 0000 0072 3e00 0000  .rl...r>...r>...
-00002090: 723f 0000 00da 1663 6f6d 7075 7465 5f70  r?.....compute_p
-000020a0: 726f 746f 7479 7065 5f6c 6f73 7320 0100  rototype_loss ..
-000020b0: 0073 1600 0000 0002 0602 20ff 0404 20ff  .s........ ... .
-000020c0: 0603 0601 1e02 1aff 0604 0c01 7a25 436f  ............z%Co
-000020d0: 756e 7465 7266 6163 7475 616c 2e63 6f6d  unterfactual.com
-000020e0: 7075 7465 5f70 726f 746f 7479 7065 5f6c  pute_prototype_l
-000020f0: 6f73 7363 0100 0000 0000 0000 0000 0000  ossc............
-00002100: 0100 0000 0300 0000 4300 0000 7368 0000  ........C...sh..
-00002110: 007c 00a0 00a1 0001 007c 00a0 017c 006a  .|.......|...|.j
-00002120: 02a1 0101 007c 00a0 03a1 0001 007c 00a0  .....|.......|..
-00002130: 04a1 0001 007c 006a 057c 006a 0617 007c  .....|.j.|.j...|
-00002140: 006a 0717 007c 006a 0817 007c 005f 097c  .j...|.j...|._.|
-00002150: 006a 0a7c 006a 0b17 007c 006a 0c17 007c  .j.|.j...|.j...|
-00002160: 006a 0d7c 006a 0e14 0017 007c 006a 0f17  .j.|.j.....|.j..
-00002170: 007c 005f 1064 0053 0072 6e00 0000 2911  .|._.d.S.rn...).
-00002180: 728b 0000 0072 7e00 0000 721b 0000 0072  r....r~...r....r
-00002190: 8200 0000 728f 0000 0072 8500 0000 727d  ....r....r....r}
-000021a0: 0000 0072 8100 0000 728e 0000 00da 086c  ...r....r......l
-000021b0: 6f73 735f 6f70 7472 8400 0000 727c 0000  oss_optr....r|..
-000021c0: 0072 8000 0000 721d 0000 0072 7b00 0000  .r....r....r{...
-000021d0: 728d 0000 00da 0a6c 6f73 735f 746f 7461  r......loss_tota
-000021e0: 6c72 6c00 0000 723e 0000 0072 3e00 0000  lrl...r>...r>...
-000021f0: 723f 0000 00da 1563 6f6d 7075 7465 5f63  r?.....compute_c
-00002200: 6f6d 6269 6e65 645f 6c6f 7373 3201 0000  ombined_loss2...
-00002210: 7320 0000 0000 0308 010c 0108 0108 0416  s ..............
-00002220: ff04 0504 0104 ff02 0204 fe02 030a fd02  ................
-00002230: 0404 fc02 ff7a 2443 6f75 6e74 6572 6661  .....z$Counterfa
-00002240: 6374 7561 6c2e 636f 6d70 7574 655f 636f  ctual.compute_co
-00002250: 6d62 696e 6564 5f6c 6f73 7363 0200 0000  mbined_lossc....
-00002260: 0000 0000 0000 0000 0300 0000 0400 0000  ................
-00002270: 0300 0000 733a 0000 0074 006a 0188 016a  ....s:...t.j...j
-00002280: 0267 0188 0064 018d 0288 015f 0387 0087  .g...d....._....
-00002290: 0166 0264 0264 0384 087d 0274 006a 046a  .f.d.d...}.t.j.j
-000022a0: 0588 016a 037c 0264 048d 0288 015f 0664  ...j.|.d....._.d
-000022b0: 0553 0029 067a 1f53 6574 2075 7020 7468  .S.).z.Set up th
-000022c0: 6520 7472 6169 6e69 6e67 2070 6172 616d  e training param
-000022d0: 6574 6572 732e 2901 da02 6c72 6301 0000  eters.)...lrc...
-000022e0: 0000 0000 0000 0000 0001 0000 0004 0000  ................
-000022f0: 0013 0000 0073 1600 0000 8800 6401 7c00  .....s......d.|.
-00002300: 8801 6a00 1b00 1800 6402 1300 1400 5300  ..j.....d.....S.
-00002310: 2903 4e72 1800 0000 6700 0000 0000 00e0  ).Nr....g.......
-00002320: 3f29 0172 2500 0000 2901 da05 6570 6f63  ?).r%...)...epoc
-00002330: 68a9 0272 2400 0000 7230 0000 0072 3e00  h..r$...r0...r>.
-00002340: 0000 723f 0000 00da 083c 6c61 6d62 6461  ..r?.....<lambda
-00002350: 3e4b 0100 00f3 0000 0000 7a2f 436f 756e  >K........z/Coun
-00002360: 7465 7266 6163 7475 616c 2e73 6574 7570  terfactual.setup
-00002370: 5f74 7261 696e 696e 672e 3c6c 6f63 616c  _training.<local
-00002380: 733e 2e3c 6c61 6d62 6461 3e29 02da 096f  s>.<lambda>)...o
-00002390: 7074 696d 697a 6572 da09 6c72 5f6c 616d  ptimizer..lr_lam
-000023a0: 6264 614e 2907 da05 6f70 7469 6dda 0353  bdaN)...optim..S
-000023b0: 4744 725e 0000 0072 9800 0000 da0c 6c72  GDr^...r......lr
-000023c0: 5f73 6368 6564 756c 6572 da08 4c61 6d62  _scheduler..Lamb
-000023d0: 6461 4c52 da0d 6c65 6172 6e69 6e67 5f72  daLR..learning_r
-000023e0: 6174 6529 0372 3000 0000 7224 0000 005a  ate).r0...r$...Z
-000023f0: 116c 616d 6264 615f 706f 6c79 5f64 6563  .lambda_poly_dec
-00002400: 6179 723e 0000 0072 9500 0000 723f 0000  ayr>...r....r?..
-00002410: 00da 0e73 6574 7570 5f74 7261 696e 696e  ...setup_trainin
-00002420: 6747 0100 0073 0c00 0000 0002 1402 0cff  gG...s..........
-00002430: 0203 0601 06ff 7a1d 436f 756e 7465 7266  ......z.Counterf
-00002440: 6163 7475 616c 2e73 6574 7570 5f74 7261  actual.setup_tra
-00002450: 696e 696e 6729 03da 0a74 7261 696e 5f64  ining)...train_d
-00002460: 6174 61da 0570 7265 6473 722d 0000 0063  ata..predsr-...c
-00002470: 0300 0000 0000 0000 0000 0000 0a00 0000  ................
-00002480: 0600 0000 4300 0000 73c8 0000 0074 0083  ....C...s....t..
-00002490: 007d 0364 0164 0267 027d 047c 0444 005d  .}.d.d.g.}.|.D.]
-000024a0: 0e7d 057c 03a0 017c 05a1 0101 0071 127c  .}.|...|.....q.|
-000024b0: 006a 0264 0319 00a0 037c 03a1 0101 007c  .j.d.....|.....|
-000024c0: 006a 0472 a47c 006a 05a0 067c 01a1 017d  .j.r.|.j...|...}
-000024d0: 0669 007c 005f 0769 007c 005f 0874 097c  .i.|._.i.|._.t.|
-000024e0: 006a 0a83 0144 005d 467d 0774 0ba0 0c7c  .j...D.]F}.t...|
-000024f0: 027c 076b 02a1 0164 0419 007d 0874 0b6a  .|.k...d...}.t.j
-00002500: 0d74 0b6a 0e7c 067c 0819 0064 0464 058d  .t.j.|.|...d.d..
-00002510: 0264 0464 058d 027c 006a 077c 073c 007c  .d.d...|.j.|.<.|
-00002520: 067c 0819 007c 006a 087c 073c 0071 5a6e  .|...|.j.|.<.qZn
-00002530: 207c 006a 0f72 c474 107c 006a 1183 017d   |.j.r.t.|.j...}
-00002540: 097c 096a 127c 005f 127c 096a 137c 005f  .|.j.|._.|.j.|._
-00002550: 147c 0053 0029 0661 2801 0000 0a20 2020  .|.S.).a(....   
-00002560: 2020 2020 2047 6574 2070 726f 746f 7479       Get prototy
-00002570: 7065 7320 666f 7220 6561 6368 2063 6c61  pes for each cla
-00002580: 7373 2075 7369 6e67 2074 6865 2065 6e63  ss using the enc
-00002590: 6f64 6572 206f 7220 6b2d 6420 7472 6565  oder or k-d tree
-000025a0: 732e 0a20 2020 2020 2020 2054 6865 2070  s..        The p
-000025b0: 726f 746f 7479 7065 7320 6172 6520 7573  rototypes are us
-000025c0: 6564 2066 6f72 2074 6865 2065 6e63 6f64  ed for the encod
-000025d0: 6572 206c 6f73 7320 7465 726d 206f 7220  er loss term or 
-000025e0: 746f 2063 616c 6375 6c61 7465 2074 6865  to calculate the
-000025f0: 206f 7074 696f 6e61 6c20 7472 7573 7420   optional trust 
-00002600: 7363 6f72 6573 2e0a 0a20 2020 2020 2020  scores...       
-00002610: 2050 6172 616d 6574 6572 730a 2020 2020   Parameters.    
-00002620: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20      ----------. 
-00002630: 2020 2020 2020 2074 7261 696e 5f64 6174         train_dat
-00002640: 610a 2020 2020 2020 2020 2020 2020 5265  a.            Re
-00002650: 7072 6573 656e 7461 7469 7665 2073 616d  presentative sam
-00002660: 706c 6520 6672 6f6d 2074 6865 2074 7261  ple from the tra
-00002670: 696e 696e 6720 6461 7461 2e0a 2020 2020  ining data..    
-00002680: 2020 2020 7230 0000 0072 a000 0000 7232      r0...r....r2
-00002690: 0000 0072 0100 0000 a901 da04 6178 6973  ...r........axis
-000026a0: 2915 7246 0000 0072 4700 0000 722e 0000  ).rF...rG...r...
-000026b0: 0072 4800 0000 7221 0000 0072 5100 0000  .rH...r!...rQ...
-000026c0: 7219 0000 00da 0b63 6c61 7373 5f70 726f  r......class_pro
-000026d0: 746f da09 636c 6173 735f 656e 6372 5600  to..class_encrV.
-000026e0: 0000 724a 0000 0072 5700 0000 da05 7768  ..rJ...rW.....wh
-000026f0: 6572 65da 0b65 7870 616e 645f 6469 6d73  ere..expand_dims
-00002700: da04 6d65 616e 7223 0000 00da 0b6c 6f61  ..meanr#.....loa
-00002710: 645f 6f62 6a65 6374 722b 0000 00da 076b  d_objectr+.....k
-00002720: 6474 7265 6573 5a08 585f 6b64 7472 6565  dtreesZ.X_kdtree
-00002730: da0a 585f 6279 5f63 6c61 7373 290a 7230  ..X_by_class).r0
-00002740: 0000 0072 a000 0000 72a1 0000 0072 3200  ...r....r....r2.
-00002750: 0000 725b 0000 0072 5c00 0000 5a08 656e  ..r[...r\...Z.en
-00002760: 635f 6461 7461 da01 69da 0369 6478 da02  c_data..i..idx..
-00002770: 7473 723e 0000 0072 3e00 0000 723f 0000  tsr>...r>...r?..
-00002780: 00da 0366 6974 5101 0000 7328 0000 0000  ...fitQ...s(....
-00002790: 0f06 0108 0108 010c 0210 0206 010c 0106  ................
-000027a0: 0106 010e 0112 0104 0112 ff0c 0312 0106  ................
-000027b0: 040a 0108 0108 017a 1243 6f75 6e74 6572  .......z.Counter
-000027c0: 6661 6374 7561 6c2e 6669 74e7 bbbd d7d9  factual.fit.....
-000027d0: df7c db3d 2905 da01 58da 0961 6476 5f63  .|.=)...X..adv_c
-000027e0: 6c61 7373 da0a 6f72 6967 5f63 6c61 7373  lass..orig_class
-000027f0: 7228 0000 0072 2d00 0000 6305 0000 0000  r(...r-...c.....
-00002800: 0000 0000 0000 000a 0000 0004 0000 0043  ...............C
-00002810: 0000 0073 9600 0000 7c00 6a00 7248 7c00  ...s....|.j.rH|.
-00002820: 6a01 a002 7c01 a101 7d05 7c00 6a03 7c02  j...|...}.|.j.|.
-00002830: 1900 7d06 7c00 6a03 7c03 1900 7d07 7404  ..}.|.j.|...}.t.
-00002840: 6a05 a006 7c05 7c06 1800 a101 7d08 7404  j...|.|.....}.t.
-00002850: 6a05 a006 7c05 7c07 1800 a101 7d09 6e42  j...|.|.....}.nB
-00002860: 7c00 6a07 7280 7c00 6a08 7c02 1900 6a09  |.j.r.|.j.|...j.
-00002870: 740a 6401 6402 8d02 6403 1900 7d08 7c00  t.d.d...d...}.|.
-00002880: 6a08 7c03 1900 6a09 740a 6401 6402 8d02  j.|...j.t.d.d...
-00002890: 6403 1900 7d09 6e0a 740b a00c 6404 a101  d...}.n.t...d...
-000028a0: 0100 7c09 7c08 7c04 1700 1b00 5300 2905  ..|.|.|.....S.).
-000028b0: 61f5 0100 000a 2020 2020 2020 2020 5061  a.....        Pa
-000028c0: 7261 6d65 7465 7273 0a20 2020 2020 2020  rameters.       
-000028d0: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020   ----------.    
-000028e0: 2020 2020 580a 2020 2020 2020 2020 2020      X.          
-000028f0: 2020 5065 7274 7572 6261 7469 6f6e 2e0a    Perturbation..
-00002900: 2020 2020 2020 2020 6164 765f 636c 6173          adv_clas
-00002910: 730a 2020 2020 2020 2020 2020 2020 5072  s.            Pr
-00002920: 6564 6963 7465 6420 636c 6173 7320 6f6e  edicted class on
-00002930: 2074 6865 2070 6572 7475 7262 6564 2069   the perturbed i
-00002940: 6e73 7461 6e63 652e 0a20 2020 2020 2020  nstance..       
-00002950: 206f 7269 675f 636c 6173 730a 2020 2020   orig_class.    
-00002960: 2020 2020 2020 2020 5072 6564 6963 7465          Predicte
-00002970: 6420 636c 6173 7320 6f6e 2074 6865 206f  d class on the o
-00002980: 7269 6769 6e61 6c20 696e 7374 616e 6365  riginal instance
-00002990: 2e0a 2020 2020 2020 2020 6570 730a 2020  ..        eps.  
-000029a0: 2020 2020 2020 2020 2020 536d 616c 6c20            Small 
-000029b0: 6e75 6d62 6572 2074 6f20 6176 6f69 6420  number to avoid 
-000029c0: 6469 7669 6469 6e67 2062 7920 302e 0a0a  dividing by 0...
-000029d0: 2020 2020 2020 2020 5265 7475 726e 730a          Returns.
-000029e0: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d0a          -------.
-000029f0: 2020 2020 2020 2020 5261 7469 6f20 6265          Ratio be
-00002a00: 7477 6565 6e20 7468 6520 6469 7374 616e  tween the distan
-00002a10: 6365 2074 6f20 7468 6520 7072 6f74 6f74  ce to the protot
-00002a20: 7970 6520 6f66 2074 6865 2070 7265 6469  ype of the predi
-00002a30: 6374 6564 2063 6c61 7373 2066 6f72 2074  cted class for t
-00002a40: 6865 206f 7269 6769 6e61 6c20 696e 7374  he original inst
-00002a50: 616e 6365 2061 6e64 2020 2020 2020 2020  ance and        
-00002a60: 2074 6865 2070 726f 746f 7479 7065 206f   the prototype o
-00002a70: 6620 7468 6520 7072 6564 6963 7465 6420  f the predicted 
-00002a80: 636c 6173 7320 666f 7220 7468 6520 7065  class for the pe
-00002a90: 7274 7572 6265 6420 696e 7374 616e 6365  rturbed instance
-00002aa0: 2e0a 2020 2020 2020 2020 7218 0000 00a9  ..        r.....
-00002ab0: 01da 016b 7201 0000 007a 4b4e 6565 6420  ...kr....zKNeed 
-00002ac0: 6569 7468 6572 2061 6e20 656e 636f 6465  either an encode
-00002ad0: 7220 6f72 2074 6865 206b 2d64 2074 7265  r or the k-d tre
-00002ae0: 6573 2065 6e61 626c 6564 2074 6f20 636f  es enabled to co
-00002af0: 6d70 7574 6520 6469 7374 616e 6365 2073  mpute distance s
-00002b00: 636f 7265 732e 290d 7221 0000 0072 5100  cores.).r!...rQ.
-00002b10: 0000 7219 0000 0072 a400 0000 7257 0000  ..r....r....rW..
-00002b20: 00da 066c 696e 616c 6772 7f00 0000 7223  ...linalgr....r#
-00002b30: 0000 0072 aa00 0000 da05 7175 6572 795a  ...r......queryZ
-00002b40: 0658 7061 7463 6872 4d00 0000 724e 0000  .XpatchrM...rN..
-00002b50: 0029 0a72 3000 0000 72b1 0000 0072 b200  .).r0...r....r..
-00002b60: 0000 72b3 0000 0072 2800 0000 da05 585f  ..r....r(.....X_
-00002b70: 656e 635a 0961 6476 5f70 726f 746f 5a0a  encZ.adv_protoZ.
-00002b80: 6f72 6967 5f70 726f 746f 5a08 6469 7374  orig_protoZ.dist
-00002b90: 5f61 6476 5a09 6469 7374 5f6f 7269 6772  _advZ.dist_origr
-00002ba0: 3e00 0000 723e 0000 0072 3f00 0000 da05  >...r>...r?.....
-00002bb0: 7363 6f72 657a 0100 0073 1a00 0000 0014  scorez...s......
-00002bc0: 0601 0c01 0a01 0a01 1001 1201 0603 1801  ................
-00002bd0: 1a02 0401 02ff 0403 7a14 436f 756e 7465  ........z.Counte
-00002be0: 7266 6163 7475 616c 2e73 636f 7265 72a8  rfactual.scorer.
-00002bf0: 0000 00e9 6400 0000 2909 72b1 0000 00da  ....d...).r.....
-00002c00: 0159 da0c 7461 7267 6574 5f63 6c61 7373  .Y..target_class
-00002c10: 72b5 0000 00da 066b 5f74 7970 65da 0974  r......k_type..t
-00002c20: 6872 6573 686f 6c64 722c 0000 00da 0b70  hresholdr,.....p
-00002c30: 7269 6e74 5f65 7665 7279 722d 0000 0063  rint_everyr-...c
-00002c40: 0900 0000 0000 0000 0000 0000 2c00 0000  ............,...
-00002c50: 0b00 0000 0300 0000 73a4 0700 0088 006a  ........s......j
-00002c60: 007c 016a 0164 0119 006b 0273 144a 0082  .|.j.d...k.s.J..
-00002c70: 0174 0274 0374 0474 056a 0666 0319 0074  .t.t.t.t.j.f...t
-00002c80: 0474 0764 029c 0387 0066 0164 0364 0484  .t.d.....f.d.d..
-00002c90: 0c7d 097c 0364 0575 0072 8c74 0874 0988  .}.|.d.u.r.t.t..
-00002ca0: 006a 0a83 0183 017d 037c 03a0 0b74 056a  .j.....}.|...t.j
-00002cb0: 0c7c 0264 0664 078d 02a1 0101 0088 006a  .|.d.d.........j
-00002cc0: 0d72 8c74 0e64 08a0 0f74 056a 0c7c 0264  .r.t.d...t.j.|.d
-00002cd0: 0664 078d 02a1 0183 0101 0074 0e64 09a0  .d.........t.d..
-00002ce0: 0f7c 03a1 0183 0101 007c 017d 0a69 007d  .|.......|.}.i.}
-00002cf0: 0b88 006a 1090 0172 9888 006a 11a0 1288  ...j...r...j....
-00002d00: 00a0 137c 01a1 01a1 017d 0c7c 0464 0575  ...|.....}.|.d.u
-00002d10: 0072 bc88 006a 146e 0488 006a 157d 0d7c  .r...j.n...j.}.|
-00002d20: 0da0 16a1 0044 005d ca5c 027d 0e7d 0f7c  .....D.].\.}.}.|
-00002d30: 0e7c 0376 0172 dc71 ca7c 0464 0575 0072  .|.v.r.q.|.d.u.r
-00002d40: fa74 056a 17a0 187c 0c7c 0f18 00a1 017c  .t.j...|.|.....|
-00002d50: 0b7c 0e3c 0071 ca7c 0464 0575 0172 ca74  .|.<.q.|.d.u.r.t
-00002d60: 056a 176a 187c 0ca0 197c 0c6a 0164 0119  .j.j.|...|.j.d..
-00002d70: 0064 0aa1 027c 0fa0 197c 0f6a 0164 0119  .d...|...|.j.d..
-00002d80: 0064 0aa1 0218 0064 0664 078d 027d 1074  .d.....d.d...}.t
-00002d90: 05a0 1a7c 10a1 0164 057c 0485 0219 007d  ...|...d.|.....}
-00002da0: 117c 0564 0b6b 0290 0172 6274 05a0 1b7c  .|.d.k...rbt...|
-00002db0: 107c 1119 00a1 017c 0b7c 0e3c 006e 107c  .|.....|.|.<.n.|
-00002dc0: 107c 1164 0a19 0019 007c 0b7c 0e3c 0074  .|.d.....|.|.<.t
-00002dd0: 056a 1c74 056a 1b7c 0f7c 1119 0064 0164  .j.t.j.|.|...d.d
-00002de0: 078d 0264 0164 078d 0288 006a 147c 0e3c  ...d.d.....j.|.<
-00002df0: 0071 ca6e 8888 006a 1d90 0272 207c 0464  .q.n...j...r |.d
-00002e00: 0575 0090 0172 ae64 067d 0469 0088 005f  .u...r.d.}.i..._
-00002e10: 1474 0988 006a 0a83 0144 005d 607d 0e7c  .t...j...D.]`}.|
-00002e20: 0e7c 0376 0190 0172 d090 0171 be88 006a  .|.v...r...q...j
-00002e30: 1e7c 0e19 006a 1f7c 0a7c 0464 0c8d 025c  .|...j.|.|.d...\
-00002e40: 027d 127d 137c 1264 0119 0064 0a19 007c  .}.}.|.d...d...|
-00002e50: 0b7c 0e3c 0088 006a 207c 0e19 007c 1364  .|.<...j |...|.d
-00002e60: 0119 0064 0a19 0019 00a0 1964 0664 0aa1  ...d.......d.d..
-00002e70: 0288 006a 147c 0e3c 0090 0171 be88 006a  ...j.|.<...q...j
-00002e80: 2190 0272 5e74 227c 0b7c 0b6a 2364 0d8d  !..r^t"|.|.j#d..
-00002e90: 0288 005f 2488 006a 1488 006a 2419 007d  ..._$..j...j$..}
-00002ea0: 1488 006a 0d90 0272 7074 0e64 0ea0 0f88  ...j...rpt.d....
-00002eb0: 006a 24a1 0183 0101 006e 1274 256a 2688  .j$......n.t%j&.
-00002ec0: 006a 2774 256a 2864 0f8d 0201 0074 25a0  .j't%j(d.....t%.
-00002ed0: 2688 006a 00a1 017d 1574 25a0 2988 006a  &..j...}.t%.)..j
-00002ee0: 00a1 0188 006a 2a14 007d 1674 25a0 2988  .....j*..}.t%.).
-00002ef0: 006a 00a1 0164 1014 007d 1764 1067 0188  .j...d...}.d.g..
-00002f00: 006a 0014 007d 1874 25a0 2688 006a 0164  .j...}.t%.&..j.d
-00002f10: 0664 0585 0219 00a1 0167 0188 006a 0014  .d.......g...j..
-00002f20: 007d 1974 25a0 2688 006a 01a1 0174 25a0  .}.t%.&..j...t%.
-00002f30: 2688 006a 01a1 0166 027d 1a64 1164 1284  &..j...f.}.d.d..
-00002f40: 0074 0988 006a 2b83 0144 0083 0188 005f  .t...j+..D....._
-00002f50: 2c74 0988 006a 2b83 0144 0090 045d 707d  ,t...j+..D...]p}
-00002f60: 1b7c 0aa0 2da1 00a0 2ea1 0088 005f 2f7c  .|..-........_/|
-00002f70: 02a0 2da1 00a0 2ea1 0088 005f 307c 16a0  ..-........_0|..
-00002f80: 2da1 00a0 2ea1 0088 005f 317c 0aa0 2da1  -........_1|..-.
-00002f90: 00a0 2ea1 0088 005f 327c 0aa0 2da1 00a0  ......._2|..-...
-00002fa0: 2ea1 00a0 33a1 0088 005f 347c 14a0 2da1  ....3...._4|..-.
-00002fb0: 00a0 2ea1 0088 005f 3588 00a0 3688 006a  ......._5...6..j
-00002fc0: 37a1 0101 0064 1067 0188 006a 0014 007d  7....d.g...j...}
-00002fd0: 1c64 0a67 0188 006a 0014 007d 1d64 0188  .d.g...j...}.d..
-00002fe0: 005f 3874 0988 006a 3983 0144 0090 035d  ._8t...j9..D...]
-00002ff0: 147d 1e88 006a 3aa0 3ba1 0001 0088 00a0  .}...j:.;.......
-00003000: 3ca1 0001 0088 006a 3da0 3ea1 0001 0074  <......j=.>....t
-00003010: 25a0 3fa1 008f 2c01 0088 006a 346a 40a0  %.?...,....j4j@.
-00003020: 4188 006a 4264 0119 0088 006a 4264 0619  A..jBd.....jBd..
-00003030: 00a1 0201 0057 0064 0504 0004 0083 0301  .....W.d........
-00003040: 006e 1231 0090 0373 ee30 0001 0001 0001  .n.1...s.0......
-00003050: 0059 0001 0088 006a 346a 407d 1f88 006a  .Y.....j4j@}...j
-00003060: 3aa0 43a1 0001 0088 006a 44a0 43a1 0001  :.C......jD.C...
-00003070: 0074 25a0 3fa1 008f 2c01 0088 00a0 4588  .t%.?...,.....E.
-00003080: 006a 46a1 0101 0088 00a0 47a1 0001 0088  .jF.......G.....
-00003090: 00a0 48a1 0001 0057 0064 0504 0004 0083  ..H....W.d......
-000030a0: 0301 006e 1231 0090 0473 5030 0001 0001  ...n.1...sP0....
-000030b0: 0001 0059 0001 0088 00a0 3ca1 0001 007c  ...Y......<....|
-000030c0: 1e7c 0816 0064 016b 0290 0472 9474 25a0  .|...d.k...r.t%.
-000030d0: 4988 006a 4a7c 0214 00a1 017d 2074 25a0  I..jJ|.....} t%.
-000030e0: 4b64 067c 0218 0088 006a 4a14 00a1 017d  Kd.|.....jJ....}
-000030f0: 2188 006a 0d90 0572 787c 1e7c 0816 0064  !..j...rx|.|...d
-00003100: 016b 0290 0572 7874 0e64 13a0 0f7c 1e7c  .k...rxt.d...|.|
-00003110: 1664 0119 00a1 0283 0101 0074 0e64 14a0  .d.........t.d..
-00003120: 0f88 006a 4c88 006a 4da1 0283 0101 0074  ...jL..jM......t
-00003130: 0e64 15a0 0f88 006a 4e88 006a 4f88 006a  .d.....jN..jO..j
-00003140: 50a1 0383 0101 0074 0e64 16a0 0f88 006a  P......t.d.....j
-00003150: 51a1 0183 0101 0074 0e64 17a0 0f7c 207c  Q......t.d...| |
-00003160: 21a1 0283 0101 007c 1f64 0575 0190 0572  !......|.d.u...r
-00003170: 5e7c 1fa0 2ea1 00a0 52a1 00a0 53a1 007d  ^|......R...S..}
-00003180: 2274 0e64 18a0 0f7c 22a0 22a1 007c 22a0  "t.d...|"."..|".
-00003190: 4ba1 00a1 0283 0101 0074 0e64 19a0 0f7c  K........t.d...|
-000031a0: 22a0 1ba1 0074 05a0 1b74 05a0 547c 22a1  "....t...t..T|".
-000031b0: 01a1 01a1 0283 0101 006e 1074 0e64 1a83  .........n.t.d..
-000031c0: 0101 0074 0e64 1b83 0101 0074 556a 56a0  ...t.d.....tUjV.
-000031d0: 57a1 0001 0074 5874 5988 006a 5a88 006a  W....tXtY..jZ..j
-000031e0: 4a88 006a 3283 0383 0144 0090 015d 045c  J..j2....D...].\
-000031f0: 027d 235c 037d 247d 257d 2674 25a0 0c7c  .}#\.}$}%}&t%..|
-00003200: 027c 2319 00a1 017d 2774 25a0 0c7c 25a1  .|#....}'t%..|%.
-00003210: 017d 287c 26a0 5b64 01a1 017d 267c 0664  .}(|&.[d...}&|.d
-00003220: 1c6b 0490 0572 e888 00a0 5c7c 2674 05a0  .k...r....\|&t..
-00003230: 0c74 4aa1 017c 27a1 037d 297c 297c 066b  .tJ..|'..})|)|.k
-00003240: 047d 2a6e 0464 1d7d 2a7c 247c 1c7c 2319  .}*n.d.}*|$|.|#.
-00003250: 006b 0090 0672 2e7c 097c 257c 2783 0290  .k...r.|.|%|'...
-00003260: 0672 2e7c 2a90 0672 2e7c 287c 0376 0090  .r.|*..r.|(|.v..
-00003270: 0672 2e7c 247c 1c7c 233c 007c 287c 1d7c  .r.|$|.|#<.|(|.|
-00003280: 233c 0074 0e7c 2883 0101 007c 247c 187c  #<.t.|(....|$|.|
-00003290: 2319 006b 0090 0572 8e7c 097c 257c 2783  #..k...r.|.|%|'.
-000032a0: 0290 0572 8e7c 2a90 0572 8e7c 287c 0376  ...r.|*..r.|(|.v
-000032b0: 0090 0572 8e88 006a 0d90 0672 6874 0e64  ...r...j...rht.d
-000032c0: 1e83 0101 007c 247c 187c 233c 007c 267c  .....|$|.|#<.|&|
-000032d0: 197c 233c 007c 1f7d 1a64 1d88 005f 5d88  .|#<.|.}.d..._].
-000032e0: 006a 2c7c 1b19 00a0 5e7c 26a1 0101 0090  .j,|....^|&.....
-000032f0: 0571 8e88 0004 006a 3864 0637 0002 005f  .q.....j8d.7..._
-00003300: 3890 0371 9074 0988 006a 0083 0144 005d  8..q.t...j...D.]
-00003310: ba7d 237c 097c 1d7c 2319 0074 05a0 0c7c  .}#|.|.|#..t...|
-00003320: 027c 2319 00a1 0183 0290 0772 1c7c 1d7c  .|#........r.|.|
-00003330: 2319 0064 0a6b 0390 0772 1c74 227c 177c  #..d.k...r.t"|.|
-00003340: 2319 007c 167c 2319 0083 027c 177c 233c  #..|.|#....|.|#<
-00003350: 007c 177c 2319 0064 1f6b 0090 0772 6a7c  .|.|#..d.k...rj|
-00003360: 157c 2319 007c 177c 2319 0017 0064 201b  .|#..|.|#....d .
-00003370: 007c 167c 233c 006e 4e74 4b7c 157c 2319  .|.|#<.nNtK|.|#.
-00003380: 007c 167c 2319 0083 027c 157c 233c 007c  .|.|#....|.|#<.|
-00003390: 177c 2319 0064 1f6b 0090 0772 5a7c 157c  .|#..d.k...rZ|.|
-000033a0: 2319 007c 177c 2319 0017 0064 201b 007c  #..|.|#....d ..|
-000033b0: 167c 233c 006e 107c 167c 2305 0019 0064  .|#<.n.|.|#....d
-000033c0: 2139 0003 003c 0090 0671 b290 0271 fe74  !9...<...q...q.t
-000033d0: 056a 5f7c 1964 0164 078d 027d 2b7c 2b6a  .j_|.d.d...}+|+j
-000033e0: 0188 006a 016b 0390 0772 9c74 056a 1c7c  ...j.k...r.t.j.|
-000033f0: 2b64 0164 078d 027d 2b7c 2b7c 1a66 0253  +d.d...}+|+|.f.S
-00003400: 0029 2261 9f06 0000 0a20 2020 2020 2020  .)"a.....       
-00003410: 2046 696e 6420 6120 636f 756e 7465 7266   Find a counterf
-00003420: 6163 7475 616c 2028 4346 2920 666f 7220  actual (CF) for 
-00003430: 696e 7374 616e 6365 2060 5860 2075 7369  instance `X` usi
-00003440: 6e67 2061 2066 6173 7420 6974 6572 6174  ng a fast iterat
-00003450: 6976 6520 7368 7269 6e6b 6167 652d 7468  ive shrinkage-th
-00003460: 7265 7368 6f6c 6469 6e67 2061 6c67 6f72  resholding algor
-00003470: 6974 686d 2028 4649 5354 4129 2e0a 0a20  ithm (FISTA)... 
-00003480: 2020 2020 2020 2050 6172 616d 6574 6572         Parameter
-00003490: 7320 6d6b 0a20 2020 2020 2020 202d 2d2d  s mk.        ---
-000034a0: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
-000034b0: 580a 2020 2020 2020 2020 2020 2020 496e  X.            In
-000034c0: 7374 616e 6365 2074 6f20 6174 7461 636b  stance to attack
-000034d0: 2e0a 2020 2020 2020 2020 590a 2020 2020  ..        Y.    
-000034e0: 2020 2020 2020 2020 4c61 6265 6c73 2066          Labels f
-000034f0: 6f72 2060 5860 2061 7320 6f6e 652d 686f  or `X` as one-ho
-00003500: 742d 656e 636f 6469 6e67 2e0a 2020 2020  t-encoding..    
-00003510: 2020 2020 7461 7267 6574 5f63 6c61 7373      target_class
-00003520: 0a20 2020 2020 2020 2020 2020 204c 6973  .            Lis
-00003530: 7420 7769 7468 2074 6172 6765 7420 636c  t with target cl
-00003540: 6173 7365 7320 7573 6564 2074 6f20 6669  asses used to fi
-00003550: 6e64 2063 6c6f 7365 7374 2070 726f 746f  nd closest proto
-00003560: 7479 7065 2e20 4966 2060 604e 6f6e 6560  type. If ``None`
-00003570: 602c 2074 6865 206e 6561 7265 7374 2070  `, the nearest p
-00003580: 726f 746f 7479 7065 0a20 2020 2020 2020  rototype.       
-00003590: 2020 2020 2065 7863 6570 7420 666f 7220       except for 
-000035a0: 7468 6520 7072 6564 6963 7420 636c 6173  the predict clas
-000035b0: 7320 6f6e 2074 6865 2069 6e73 7461 6e63  s on the instanc
-000035c0: 6520 6973 2075 7365 642e 0a20 2020 2020  e is used..     
-000035d0: 2020 206b 0a20 2020 2020 2020 2020 2020     k.           
-000035e0: 204e 756d 6265 7220 6f66 206e 6561 7265   Number of neare
-000035f0: 7374 2069 6e73 7461 6e63 6573 2075 7365  st instances use
-00003600: 6420 746f 2064 6566 696e 6520 7468 6520  d to define the 
-00003610: 7072 6f74 6f74 7970 6520 666f 7220 6120  prototype for a 
-00003620: 636c 6173 732e 2044 6566 6175 6c74 7320  class. Defaults 
-00003630: 746f 2075 7369 6e67 2061 6c6c 0a20 2020  to using all.   
-00003640: 2020 2020 2020 2020 2069 6e73 7461 6e63           instanc
-00003650: 6573 2062 656c 6f6e 6769 6e67 2074 6f20  es belonging to 
-00003660: 7468 6520 636c 6173 7320 6966 2061 6e20  the class if an 
-00003670: 656e 636f 6465 7220 6973 2075 7365 6420  encoder is used 
-00003680: 616e 6420 746f 2031 2066 6f72 206b 2d64  and to 1 for k-d
-00003690: 2074 7265 6573 2e0a 2020 2020 2020 2020   trees..        
-000036a0: 6b5f 7479 7065 0a20 2020 2020 2020 2020  k_type.         
-000036b0: 2020 2055 7365 2065 6974 6865 7220 7468     Use either th
-000036c0: 6520 6176 6572 6167 6520 656e 636f 6469  e average encodi
-000036d0: 6e67 206f 6620 7468 6520 6b20 6e65 6172  ng of the k near
-000036e0: 6573 7420 696e 7374 616e 6365 7320 696e  est instances in
-000036f0: 2061 2063 6c61 7373 2028 6060 6b5f 7479   a class (``k_ty
-00003700: 7065 3d27 6d65 616e 2760 6029 206f 720a  pe='mean'``) or.
-00003710: 2020 2020 2020 2020 2020 2020 7468 6520              the 
-00003720: 6b2d 6e65 6172 6573 7420 656e 636f 6469  k-nearest encodi
-00003730: 6e67 2069 6e20 7468 6520 636c 6173 7320  ng in the class 
-00003740: 2860 606b 5f74 7970 653d 2770 6f69 6e74  (``k_type='point
-00003750: 2760 6029 2074 6f20 6465 6669 6e65 2074  '``) to define t
-00003760: 6865 2070 726f 746f 7479 7065 206f 6620  he prototype of 
-00003770: 7468 6174 2063 6c61 7373 2e0a 2020 2020  that class..    
-00003780: 2020 2020 2020 2020 4f6e 6c79 2072 656c          Only rel
-00003790: 6576 616e 7420 6966 2061 6e20 656e 636f  evant if an enco
-000037a0: 6465 7220 6973 2075 7365 6420 746f 2064  der is used to d
-000037b0: 6566 696e 6520 7468 6520 7072 6f74 6f74  efine the protot
-000037c0: 7970 6573 2e0a 2020 2020 2020 2020 7468  ypes..        th
-000037d0: 7265 7368 6f6c 640a 2020 2020 2020 2020  reshold.        
-000037e0: 2020 2020 5468 7265 7368 6f6c 6420 6c65      Threshold le
-000037f0: 7665 6c20 666f 7220 7468 6520 7261 7469  vel for the rati
-00003800: 6f20 6265 7477 6565 6e20 7468 6520 6469  o between the di
-00003810: 7374 616e 6365 206f 6620 7468 6520 636f  stance of the co
-00003820: 756e 7465 7266 6163 7475 616c 2074 6f20  unterfactual to 
-00003830: 7468 6520 7072 6f74 6f74 7970 6520 6f66  the prototype of
-00003840: 2074 6865 0a20 2020 2020 2020 2020 2020   the.           
-00003850: 2070 7265 6469 6374 6564 2063 6c61 7373   predicted class
-00003860: 2066 6f72 2074 6865 206f 7269 6769 6e61   for the origina
-00003870: 6c20 696e 7374 616e 6365 206f 7665 7220  l instance over 
-00003880: 7468 6520 6469 7374 616e 6365 2074 6f20  the distance to 
-00003890: 7468 6520 7072 6f74 6f74 7970 6520 6f66  the prototype of
-000038a0: 2074 6865 2070 7265 6469 6374 6564 2063   the predicted c
-000038b0: 6c61 7373 0a20 2020 2020 2020 2020 2020  lass.           
-000038c0: 2066 6f72 2074 6865 2063 6f75 6e74 6572   for the counter
-000038d0: 6661 6374 7561 6c2e 2049 6620 7468 6520  factual. If the 
-000038e0: 7472 7573 7420 7363 6f72 6520 6973 2062  trust score is b
-000038f0: 656c 6f77 2074 6865 2074 6872 6573 686f  elow the thresho
-00003900: 6c64 2c20 7468 6520 7072 6f70 6f73 6564  ld, the proposed
-00003910: 2063 6f75 6e74 6572 6661 6374 7561 6c20   counterfactual 
-00003920: 646f 6573 0a20 2020 2020 2020 2020 2020  does.           
-00003930: 206e 6f74 206d 6565 7420 7468 6520 7265   not meet the re
-00003940: 7175 6972 656d 656e 7473 2e0a 2020 2020  quirements..    
-00003950: 2020 2020 7665 7262 6f73 650a 2020 2020      verbose.    
-00003960: 2020 2020 2020 2020 5072 696e 7420 696e          Print in
-00003970: 7465 726d 6564 6961 7465 2072 6573 756c  termediate resul
-00003980: 7473 206f 6620 6f70 7469 6d69 7a61 7469  ts of optimizati
-00003990: 6f6e 2069 6620 6060 5472 7565 6060 2e0a  on if ``True``..
-000039a0: 2020 2020 2020 2020 7072 696e 745f 6576          print_ev
-000039b0: 6572 790a 2020 2020 2020 2020 2020 2020  ery.            
-000039c0: 5072 696e 7420 6672 6571 7565 6e63 7920  Print frequency 
-000039d0: 6966 2076 6572 626f 7365 2069 7320 6060  if verbose is ``
-000039e0: 5472 7565 6060 2e0a 2020 2020 2020 2020  True``..        
-000039f0: 6c6f 675f 6576 6572 790a 2020 2020 2020  log_every.      
-00003a00: 2020 2020 2020 6074 656e 736f 7262 6f61        `tensorboa
-00003a10: 7264 6020 6c6f 6720 6672 6571 7565 6e63  rd` log frequenc
-00003a20: 7920 6966 2077 7269 7465 2064 6972 6563  y if write direc
-00003a30: 746f 7279 2069 7320 7370 6563 6966 6965  tory is specifie
-00003a40: 642e 0a0a 2020 2020 2020 2020 5265 7475  d...        Retu
-00003a50: 726e 730a 2020 2020 2020 2020 2d2d 2d2d  rns.        ----
-00003a60: 2d2d 2d0a 2020 2020 2020 2020 4f76 6572  ---.        Over
-00003a70: 616c 6c20 6265 7374 2061 7474 6163 6b20  all best attack 
-00003a80: 616e 6420 6772 6164 6965 6e74 7320 666f  and gradients fo
-00003a90: 7220 7468 6174 2061 7474 6163 6b2e 0a20  r that attack.. 
-00003aa0: 2020 2020 2020 2072 0100 0000 2903 da01         r....)...
-00003ab0: 78da 0179 722d 0000 0063 0200 0000 0000  x..yr-...c......
-00003ac0: 0000 0000 0000 0200 0000 0500 0000 1300  ................
-00003ad0: 0000 7346 0000 0074 007c 0074 0174 0274  ..sF...t.|.t.t.t
-00003ae0: 036a 0466 0383 0273 3e74 057c 0083 0173  .j.f...s>t.|...s
-00003af0: 3e7c 00a0 06a1 007d 007c 007c 0105 0019  >|.....}.|.|....
-00003b00: 0088 006a 0737 0003 003c 0074 08a0 097c  ...j.7...<.t...|
-00003b10: 00a1 017d 007c 007c 016b 0353 0029 0161  ...}.|.|.k.S.).a
-00003b20: 8501 0000 0a20 2020 2020 2020 2020 2020  .....           
-00003b30: 2043 6f6d 7061 7265 2070 7265 6469 6374   Compare predict
-00003b40: 696f 6e73 2077 6974 6820 7461 7267 6574  ions with target
-00003b50: 206c 6162 656c 7320 616e 6420 7265 7475   labels and retu
-00003b60: 726e 2077 6865 7468 6572 2063 6f75 6e74  rn whether count
-00003b70: 6572 6661 6374 7561 6c20 636f 6e64 6974  erfactual condit
-00003b80: 696f 6e73 2068 6f6c 642e 0a0a 2020 2020  ions hold...    
-00003b90: 2020 2020 2020 2020 5061 7261 6d65 7465          Paramete
-00003ba0: 7273 0a20 2020 2020 2020 2020 2020 202d  rs.            -
-00003bb0: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 2020  ---------.      
-00003bc0: 2020 2020 2020 780a 2020 2020 2020 2020        x.        
-00003bd0: 2020 2020 2020 2020 5072 6564 6963 7465          Predicte
-00003be0: 6420 636c 6173 7320 7072 6f62 6162 696c  d class probabil
-00003bf0: 6974 6965 7320 6f72 206c 6162 656c 732e  ities or labels.
-00003c00: 0a20 2020 2020 2020 2020 2020 2079 0a20  .            y. 
-00003c10: 2020 2020 2020 2020 2020 2020 2020 2054                 T
-00003c20: 6172 6765 7420 6f72 2070 7265 6469 6374  arget or predict
-00003c30: 6564 206c 6162 656c 732e 0a0a 2020 2020  ed labels...    
-00003c40: 2020 2020 2020 2020 5265 7475 726e 730a          Returns.
-00003c50: 2020 2020 2020 2020 2020 2020 2d2d 2d2d              ----
-00003c60: 2d2d 2d0a 2020 2020 2020 2020 2020 2020  ---.            
-00003c70: 426f 6f6c 2077 6865 7468 6572 2063 6f75  Bool whether cou
-00003c80: 6e74 6572 6661 6374 7561 6c20 636f 6e64  nterfactual cond
-00003c90: 6974 696f 6e73 2068 6f6c 642e 0a20 2020  itions hold..   
-00003ca0: 2020 2020 2020 2020 2029 0a72 3700 0000           ).r7...
-00003cb0: 7238 0000 00da 0369 6e74 7257 0000 00da  r8.....intrW....
-00003cc0: 0569 6e74 3634 da1d 6973 5f73 696e 676c  .int64..is_singl
-00003cd0: 655f 666c 6f61 745f 6f72 5f69 6e74 5f74  e_float_or_int_t
-00003ce0: 656e 736f 7272 6f00 0000 721c 0000 0072  ensorro...r....r
-00003cf0: 3900 0000 da06 6172 676d 6178 2902 72c0  9.....argmax).r.
-00003d00: 0000 0072 c100 0000 726c 0000 0072 3e00  ...r....rl...r>.
-00003d10: 0000 723f 0000 00da 0763 6f6d 7061 7265  ..r?.....compare
-00003d20: d101 0000 730e 0000 0000 0f12 0106 ff02  ....s...........
-00003d30: 0308 0112 010a 017a 2643 6f75 6e74 6572  .......z&Counter
-00003d40: 6661 6374 7561 6c2e 6174 7461 636b 2e3c  factual.attack.<
-00003d50: 6c6f 6361 6c73 3e2e 636f 6d70 6172 654e  locals>.compareN
-00003d60: 7218 0000 0072 a200 0000 7a13 5072 6564  r....r....z.Pred
-00003d70: 6963 7465 6420 636c 6173 733a 207b 7d7a  icted class: {}z
-00003d80: 1254 6172 6765 7420 636c 6173 7365 733a  .Target classes:
-00003d90: 207b 7d72 2f00 0000 72a8 0000 0072 b400   {}r/...r....r..
-00003da0: 0000 2901 725c 0000 007a 1350 726f 746f  ..).r\...z.Proto
-00003db0: 7479 7065 2063 6c61 7373 3a20 7b7d 7235  type class: {}r5
-00003dc0: 0000 0072 1000 0000 6301 0000 0000 0000  ...r....c.......
-00003dd0: 0000 0000 0002 0000 0004 0000 0053 0000  .............S..
-00003de0: 0073 1200 0000 6900 7c00 5d0a 7d01 7c01  .s....i.|.].}.|.
-00003df0: 6700 9302 7104 5300 723e 0000 0072 3e00  g...q.S.r>...r>.
-00003e00: 0000 2902 723b 0000 0072 ac00 0000 723e  ..).r;...r....r>
-00003e10: 0000 0072 3e00 0000 723f 0000 00da 0a3c  ...r>...r?.....<
-00003e20: 6469 6374 636f 6d70 3e29 0200 0072 9700  dictcomp>)...r..
-00003e30: 0000 7a29 436f 756e 7465 7266 6163 7475  ..z)Counterfactu
-00003e40: 616c 2e61 7474 6163 6b2e 3c6c 6f63 616c  al.attack.<local
-00003e50: 733e 2e3c 6469 6374 636f 6d70 3e7a 190a  s>.<dictcomp>z..
-00003e60: 4974 6572 6174 696f 6e3a 207b 7d3b 2043  Iteration: {}; C
-00003e70: 6f6e 7374 3a20 7b7d 7a27 4c6f 7373 2074  onst: {}z'Loss t
-00003e80: 6f74 616c 3a20 7b3a 2e33 667d 2c20 6c6f  otal: {:.3f}, lo
-00003e90: 7373 2061 7474 6163 6b3a 207b 3a2e 3366  ss attack: {:.3f
-00003ea0: 7d7a 274c 323a 207b 3a2e 3366 7d2c 204c  }z'L2: {:.3f}, L
-00003eb0: 313a 207b 3a2e 3366 7d2c 206c 6f73 7320  1: {:.3f}, loss 
-00003ec0: 4145 3a20 7b3a 2e33 667d 7a12 4c6f 7373  AE: {:.3f}z.Loss
-00003ed0: 2070 726f 746f 3a20 7b3a 2e33 667d 7a32   proto: {:.3f}z2
-00003ee0: 5461 7267 6574 2070 726f 6261 3a20 7b3a  Target proba: {:
-00003ef0: 2e32 667d 2c20 6d61 7820 6e6f 6e20 7461  .2f}, max non ta
-00003f00: 7267 6574 2070 726f 6261 3a20 7b3a 2e32  rget proba: {:.2
-00003f10: 667d 7a1f 4772 6164 6965 6e74 206d 696e  f}z.Gradient min
-00003f20: 2f6d 6178 3a20 7b3a 2e33 667d 2f7b 3a2e  /max: {:.3f}/{:.
-00003f30: 3366 7d7a 2547 7261 6469 656e 7420 6d65  3f}z%Gradient me
-00003f40: 616e 2f61 6273 206d 6561 6e3a 207b 3a2e  an/abs mean: {:.
-00003f50: 3366 7d2f 7b3a 2e33 667d 7a16 4772 6164  3f}/{:.3f}z.Grad
-00003f60: 6965 6e74 206d 696e 2f6d 6178 3a20 4e6f  ient min/max: No
-00003f70: 6e65 7a1c 4772 6164 6965 6e74 206d 6561  nez.Gradient mea
-00003f80: 6e2f 6162 7320 6d65 616e 3a20 4e6f 6e65  n/abs mean: None
-00003f90: 720d 0000 0054 7a1f 0a4e 6577 2062 6573  r....Tz..New bes
-00003fa0: 7420 636f 756e 7465 7266 6163 7475 616c  t counterfactual
-00003fb0: 2066 6f75 6e64 2167 0000 0000 65cd cd41   found!g....e..A
-00003fc0: 7206 0000 0072 1400 0000 2960 7252 0000  r....r....)`rR..
-00003fd0: 0072 1b00 0000 7205 0000 0072 3800 0000  .r....r....r8...
-00003fe0: 72c2 0000 0072 5700 0000 da07 6e64 6172  r....rW.....ndar
-00003ff0: 7261 79da 0462 6f6f 6cda 046c 6973 7472  ray..bool..listr
-00004000: 5600 0000 724a 0000 0072 5b00 0000 72c5  V...rJ...r[...r.
-00004010: 0000 0072 2c00 0000 da05 7072 696e 74da  ...r,.....print.
-00004020: 0666 6f72 6d61 7472 2100 0000 7251 0000  .formatr!...rQ..
-00004030: 0072 1900 0000 721a 0000 0072 a400 0000  .r....r....r....
-00004040: 72a5 0000 00da 0569 7465 6d73 72b6 0000  r......itemsr...
-00004050: 0072 7f00 0000 da07 7265 7368 6170 65da  .r......reshape.
-00004060: 0761 7267 736f 7274 72a8 0000 0072 a700  .argsortr....r..
-00004070: 0000 7223 0000 0072 aa00 0000 72b7 0000  ..r#...r....r...
-00004080: 0072 ab00 0000 7234 0000 0072 6100 0000  .r....r4...ra...
-00004090: da03 6765 74da 0869 645f 7072 6f74 6f72  ..get..id_protor
-000040a0: 3900 0000 7249 0000 0072 5800 0000 7254  9...rI...rX...rT
-000040b0: 0000 0072 3a00 0000 7226 0000 0072 2700  ...r:...r&...r'.
-000040c0: 0000 da09 6366 5f67 6c6f 6261 6c72 6f00  ....cf_globalro.
-000040d0: 0000 da06 6465 7461 6368 725f 0000 0072  ....detachr_...r
-000040e0: 8600 0000 728a 0000 0072 6900 0000 da0e  ....r....ri.....
-000040f0: 7265 7175 6972 6573 5f67 7261 645f 725e  requires_grad_r^
-00004100: 0000 0072 8c00 0000 729f 0000 0072 2400  ...r....r....r$.
-00004110: 0000 7267 0000 0072 2500 0000 7298 0000  ..rg...r%...r...
-00004120: 00da 097a 6572 6f5f 6772 6164 7292 0000  ...zero_gradr...
-00004130: 0072 9000 0000 da08 6261 636b 7761 7264  .r......backward
-00004140: da07 6e6f 5f67 7261 64da 0467 7261 64da  ..no_grad..grad.
-00004150: 0663 6c61 6d70 5f72 2900 0000 da04 7374  .clamp_r).....st
-00004160: 6570 729e 0000 0072 6600 0000 721e 0000  epr....rf...r...
-00004170: 0072 6d00 0000 7271 0000 0072 7700 0000  .rm...rq...rw...
-00004180: 7283 0000 0072 6200 0000 7291 0000 0072  r....rb...r....r
-00004190: 8400 0000 727c 0000 0072 7b00 0000 7280  ....r|...r{...r.
-000041a0: 0000 0072 8d00 0000 da03 6370 75da 056e  ...r......cpu..n
-000041b0: 756d 7079 7260 0000 00da 0373 7973 da06  umpyr`.....sys..
-000041c0: 7374 646f 7574 da05 666c 7573 68da 0965  stdout..flush..e
-000041d0: 6e75 6d65 7261 7465 da03 7a69 7072 7a00  numerate..ziprz.
-000041e0: 0000 da09 756e 7371 7565 657a 6572 b900  ....unsqueezer..
-000041f0: 0000 da0b 6265 7374 5f61 7474 6163 6bda  ....best_attack.
-00004200: 0661 7070 656e 64da 0b63 6f6e 6361 7465  .append..concate
-00004210: 6e61 7465 292c 7230 0000 0072 b100 0000  nate),r0...r....
-00004220: 72bb 0000 0072 bc00 0000 72b5 0000 0072  r....r....r....r
-00004230: bd00 0000 72be 0000 0072 2c00 0000 72bf  ....r....r,...r.
-00004240: 0000 0072 c600 0000 5a05 585f 6e75 6d5a  ...r....Z.X_numZ
-00004250: 0a64 6973 745f 7072 6f74 6f72 b800 0000  .dist_protor....
-00004260: da0a 636c 6173 735f 6469 6374 da01 63da  ..class_dict..c.
-00004270: 0176 5a06 6469 7374 5f6b 72ad 0000 005a  .vZ.dist_kr....Z
-00004280: 0664 6973 745f 635a 0569 6478 5f63 5a09  .dist_cZ.idx_cZ.
-00004290: 7072 6f74 6f5f 7661 6c5a 0863 6f6e 7374  proto_valZ.const
-000042a0: 5f6c 6272 8a00 0000 5a08 636f 6e73 745f  _lbr....Z.const_
-000042b0: 7562 5a11 6f76 6572 616c 6c5f 6265 7374  ubZ.overall_best
-000042c0: 5f64 6973 745a 136f 7665 7261 6c6c 5f62  _distZ.overall_b
-000042d0: 6573 745f 6174 7461 636b 5a11 6f76 6572  est_attackZ.over
-000042e0: 616c 6c5f 6265 7374 5f67 7261 6472 3c00  all_best_gradr<.
-000042f0: 0000 5a11 6375 7272 656e 745f 6265 7374  ..Z.current_best
-00004300: 5f64 6973 745a 1263 7572 7265 6e74 5f62  _distZ.current_b
-00004310: 6573 745f 7072 6f62 6172 ac00 0000 da09  est_probar......
-00004320: 6772 6164 6965 6e74 7372 8700 0000 7288  gradientsr....r.
-00004330: 0000 005a 0c67 7261 6469 656e 7473 5f6e  ...Z.gradients_n
-00004340: 70da 0962 6174 6368 5f69 6478 da04 6469  p..batch_idx..di
-00004350: 7374 da05 7072 6f62 615a 0761 6476 5f69  st..probaZ.adv_i
-00004360: 6478 da07 595f 636c 6173 7372 b200 0000  dx..Y_classr....
-00004370: 72b9 0000 005a 0f61 626f 7665 5f74 6872  r....Z.above_thr
-00004380: 6573 686f 6c64 72e3 0000 0072 3e00 0000  esholdr....r>...
-00004390: 726c 0000 0072 3f00 0000 da06 6174 7461  rl...r?.....atta
-000043a0: 636b 9f01 0000 7352 0100 0000 3014 0222  ck....sR....0.."
-000043b0: 1808 010e 0114 0106 0118 010e 0104 0304  ................
-000043c0: 0108 0212 0114 0210 0108 0102 0108 0116  ................
-000043d0: 0108 0106 0122 0102 fe06 0412 010a 0114  ....."..........
-000043e0: 0210 0104 0112 ff10 0308 010a 0104 0106  ................
-000043f0: 010e 010a 0104 0118 0110 0128 0208 0110  ...........(....
-00004400: 010c 0108 0112 0212 040c 0112 0110 030c  ................
-00004410: 011c 0118 0316 0310 030e 010e 010e 010e  ................
-00004420: 0112 010e 030c 030c 010c 0106 0210 020a  ................
-00004430: 0308 030a 030a 013c 0108 030a 030a 030a  .......<........
-00004440: 010c 0108 0128 0508 020e 0110 0114 0216  .....(..........
-00004450: 0114 0102 0104 0108 ff02 ff04 0502 0104  ................
-00004460: 010c ff02 ff04 0510 0102 0104 0104 ff02  ................
-00004470: ff04 060a 0210 0102 0104 010c ff02 ff04  ................
-00004480: 0522 0208 0108 010a 0502 0110 ff14 030e  ."..............
-00004490: 010a 010a 030a 0114 010a 0204 040a ff04  ................
-000044a0: 0208 fe04 0302 fd04 0406 fc04 0608 0108  ................
-000044b0: 0108 040a ff04 0208 fe04 0302 fd04 0406  ................
-000044c0: fc04 0608 0108 0108 0108 0104 0106 0114  ................
-000044d0: 0312 030e 0216 ff04 020a fe04 0616 010e  ................
-000044e0: 020e 0102 fe0a 0602 010c ff08 030e 020e  ................
-000044f0: 0102 fe0a 0418 030e 010e 010e 027a 1543  .............z.C
-00004500: 6f75 6e74 6572 6661 6374 7561 6c2e 6174  ounterfactual.at
-00004510: 7461 636b 2908 72b1 0000 0072 bb00 0000  tack).r....r....
-00004520: 72bc 0000 0072 b500 0000 72bd 0000 0072  r....r....r....r
-00004530: be00 0000 72bf 0000 0072 2d00 0000 6308  ....r....r-...c.
-00004540: 0000 0000 0000 0000 0000 0010 0000 000a  ................
-00004550: 0000 0043 0000 0073 7a01 0000 7c01 6a00  ...C...sz...|.j.
-00004560: 6401 1900 6402 6b03 7220 7401 a002 6403  d...d.k.r t...d.
-00004570: 7c01 6a00 6401 1900 a102 0100 7403 a004  |.j.d.......t...
-00004580: 7405 a101 7d08 7c00 a006 7c01 a101 7d09  t...}.|...|...}.
-00004590: 7c02 6404 7500 7276 7407 a008 7c09 6a00  |.d.u.rvt...|.j.
-000045a0: a101 7d0a 7407 6a09 7c09 6402 6405 8d02  ..}.t.j.|.d.d...
-000045b0: 7d0b 6402 7c0a 7407 a00a 7c09 6a00 6401  }.d.|.t...|.j.d.
-000045c0: 1900 a101 7c0b 6602 3c00 7c0a a00b a100  ....|.f.<.|.....
-000045d0: 7d02 7c09 7c08 6406 3c00 740c 6a09 7c09  }.|.|.d.<.t.j.|.
-000045e0: 6402 6407 8d02 6401 1900 7c08 6408 3c00  d.d...d...|.d.<.
-000045f0: 6409 7c00 5f0d 7c00 6a0e 7c01 7c02 7c03  d.|._.|.j.|.|.|.
-00004600: 7c04 7c05 7c00 6a0f 7c06 7c07 640a 8d08  |.|.|.j.|.|.d...
-00004610: 5c02 7d0c 7d0d 7c00 6a10 72ca 7c00 6a11  \.}.}.|.j.r.|.j.
-00004620: 7c08 640b 3c00 7c00 6a0d 73f2 7401 a002  |.d.<.|.j.s.t...
-00004630: 640c a101 0100 7412 7403 a004 7c00 6a13  d.....t.t...|.j.
-00004640: a101 7c08 640d 8d02 7d0e 7c0e 5300 7c00  ..|.d...}.|.S.|.
-00004650: 6a14 7c08 640e 3c00 6900 7c08 640f 3c00  j.|.d.<.i.|.d.<.
-00004660: 7c0c 7c08 640f 1900 6410 3c00 7c00 a006  |.|.d...d.<.|...
-00004670: 740c a015 7c0c a101 a101 a016 a100 a017  t...|...........
-00004680: a100 7d0f 7c0f 7c08 640f 1900 6411 3c00  ..}.|.|.d...d.<.
-00004690: 7407 6a09 7c0f 6402 6405 8d02 6401 1900  t.j.|.d.d...d...
-000046a0: 7c08 640f 1900 6412 3c00 7c0d a016 a100  |.d...d.<.|.....
-000046b0: a017 a100 7c08 640f 1900 6413 3c00 7412  ....|.d...d.<.t.
-000046c0: 7403 a004 7c00 6a13 a101 7c08 640d 8d02  t...|.j...|.d...
-000046d0: 7d0e 7c0e 5300 2914 61ab 0600 000a 2020  }.|.S.).a.....  
-000046e0: 2020 2020 2020 4578 706c 6169 6e20 696e        Explain in
-000046f0: 7374 616e 6365 2061 6e64 2072 6574 7572  stance and retur
-00004700: 6e20 636f 756e 7465 7266 6163 7475 616c  n counterfactual
-00004710: 2077 6974 6820 6d65 7461 6461 7461 2e0a   with metadata..
-00004720: 0a20 2020 2020 2020 2050 6172 616d 6574  .        Paramet
-00004730: 6572 730a 2020 2020 2020 2020 2d2d 2d2d  ers.        ----
-00004740: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 2058  ------.        X
-00004750: 0a20 2020 2020 2020 2020 2020 2049 6e69  .            Ini
-00004760: 7469 616c 2070 6572 7475 7262 6174 696f  tial perturbatio
-00004770: 6e0a 2020 2020 2020 2020 590a 2020 2020  n.        Y.    
-00004780: 2020 2020 2020 2020 4c61 6265 6c73 2066          Labels f
-00004790: 6f72 2060 5860 2061 7320 6f6e 652d 686f  or `X` as one-ho
-000047a0: 742d 656e 636f 6469 6e67 2e0a 2020 2020  t-encoding..    
-000047b0: 2020 2020 7461 7267 6574 5f63 6c61 7373      target_class
-000047c0: 0a20 2020 2020 2020 2020 2020 204c 6973  .            Lis
-000047d0: 7420 7769 7468 2074 6172 6765 7420 636c  t with target cl
-000047e0: 6173 7365 7320 7573 6564 2074 6f20 6669  asses used to fi
-000047f0: 6e64 2063 6c6f 7365 7374 2070 726f 746f  nd closest proto
-00004800: 7479 7065 2e20 4966 2060 604e 6f6e 6560  type. If ``None`
-00004810: 602c 2074 6865 206e 6561 7265 7374 2070  `, the nearest p
-00004820: 726f 746f 7479 7065 0a20 2020 2020 2020  rototype.       
-00004830: 2020 2020 2065 7863 6570 7420 666f 7220       except for 
-00004840: 7468 6520 7072 6564 6963 7420 636c 6173  the predict clas
-00004850: 7320 6f6e 2074 6865 2069 6e73 7461 6e63  s on the instanc
-00004860: 6520 6973 2075 7365 642e 0a20 2020 2020  e is used..     
-00004870: 2020 206b 0a20 2020 2020 2020 2020 2020     k.           
-00004880: 204e 756d 6265 7220 6f66 206e 6561 7265   Number of neare
-00004890: 7374 2069 6e73 7461 6e63 6573 2075 7365  st instances use
-000048a0: 6420 746f 2064 6566 696e 6520 7468 6520  d to define the 
-000048b0: 7072 6f74 6f74 7970 6520 666f 7220 6120  prototype for a 
-000048c0: 636c 6173 732e 2044 6566 6175 6c74 7320  class. Defaults 
-000048d0: 746f 2075 7369 6e67 2061 6c6c 0a20 2020  to using all.   
-000048e0: 2020 2020 2020 2020 2069 6e73 7461 6e63           instanc
-000048f0: 6573 2062 656c 6f6e 6769 6e67 2074 6f20  es belonging to 
-00004900: 7468 6520 636c 6173 7320 6966 2061 6e20  the class if an 
-00004910: 656e 636f 6465 7220 6973 2075 7365 6420  encoder is used 
-00004920: 616e 6420 746f 2031 2066 6f72 206b 2d64  and to 1 for k-d
-00004930: 2074 7265 6573 2e0a 2020 2020 2020 2020   trees..        
-00004940: 6b5f 7479 7065 0a20 2020 2020 2020 2020  k_type.         
-00004950: 2020 2055 7365 2065 6974 6865 7220 7468     Use either th
-00004960: 6520 6176 6572 6167 6520 656e 636f 6469  e average encodi
-00004970: 6e67 206f 6620 7468 6520 606b 6020 6e65  ng of the `k` ne
-00004980: 6172 6573 7420 696e 7374 616e 6365 7320  arest instances 
-00004990: 696e 2061 2063 6c61 7373 2028 6060 6b5f  in a class (``k_
-000049a0: 7479 7065 3d27 6d65 616e 2760 6029 206f  type='mean'``) o
-000049b0: 720a 2020 2020 2020 2020 2020 2020 7468  r.            th
-000049c0: 6520 6b2d 6e65 6172 6573 7420 656e 636f  e k-nearest enco
-000049d0: 6469 6e67 2069 6e20 7468 6520 636c 6173  ding in the clas
-000049e0: 7320 2860 606b 5f74 7970 653d 2770 6f69  s (``k_type='poi
-000049f0: 6e74 2760 6029 2074 6f20 6465 6669 6e65  nt'``) to define
-00004a00: 2074 6865 2070 726f 746f 7479 7065 206f   the prototype o
-00004a10: 6620 7468 6174 2063 6c61 7373 2e0a 2020  f that class..  
-00004a20: 2020 2020 2020 2020 2020 4f6e 6c79 2072            Only r
-00004a30: 656c 6576 616e 7420 6966 2061 6e20 656e  elevant if an en
-00004a40: 636f 6465 7220 6973 2075 7365 6420 746f  coder is used to
-00004a50: 2064 6566 696e 6520 7468 6520 7072 6f74   define the prot
-00004a60: 6f74 7970 6573 2e0a 2020 2020 2020 2020  otypes..        
-00004a70: 7468 7265 7368 6f6c 640a 2020 2020 2020  threshold.      
-00004a80: 2020 2020 2020 5468 7265 7368 6f6c 6420        Threshold 
-00004a90: 6c65 7665 6c20 666f 7220 7468 6520 7261  level for the ra
-00004aa0: 7469 6f20 6265 7477 6565 6e20 7468 6520  tio between the 
-00004ab0: 6469 7374 616e 6365 206f 6620 7468 6520  distance of the 
-00004ac0: 636f 756e 7465 7266 6163 7475 616c 2074  counterfactual t
-00004ad0: 6f20 7468 6520 7072 6f74 6f74 7970 6520  o the prototype 
-00004ae0: 6f66 2074 6865 0a20 2020 2020 2020 2020  of the.         
-00004af0: 2020 2070 7265 6469 6374 6564 2063 6c61     predicted cla
-00004b00: 7373 2066 6f72 2074 6865 206f 7269 6769  ss for the origi
-00004b10: 6e61 6c20 696e 7374 616e 6365 206f 7665  nal instance ove
-00004b20: 7220 7468 6520 6469 7374 616e 6365 2074  r the distance t
-00004b30: 6f20 7468 6520 7072 6f74 6f74 7970 6520  o the prototype 
-00004b40: 6f66 2074 6865 2070 7265 6469 6374 6564  of the predicted
-00004b50: 2063 6c61 7373 0a20 2020 2020 2020 2020   class.         
-00004b60: 2020 2066 6f72 2074 6865 2063 6f75 6e74     for the count
-00004b70: 6572 6661 6374 7561 6c2e 2049 6620 7468  erfactual. If th
-00004b80: 6520 7472 7573 7420 7363 6f72 6520 6973  e trust score is
-00004b90: 2062 656c 6f77 2074 6865 2074 6872 6573   below the thres
-00004ba0: 686f 6c64 2c20 7468 6520 7072 6f70 6f73  hold, the propos
-00004bb0: 6564 2063 6f75 6e74 6572 6661 6374 7561  ed counterfactua
-00004bc0: 6c20 646f 6573 0a20 2020 2020 2020 2020  l does.         
-00004bd0: 2020 206e 6f74 206d 6565 7420 7468 6520     not meet the 
-00004be0: 7265 7175 6972 656d 656e 7473 2e0a 2020  requirements..  
-00004bf0: 2020 2020 2020 7665 7262 6f73 650a 2020        verbose.  
-00004c00: 2020 2020 2020 2020 2020 5072 696e 7420            Print 
-00004c10: 696e 7465 726d 6564 6961 7465 2072 6573  intermediate res
-00004c20: 756c 7473 206f 6620 6f70 7469 6d69 7a61  ults of optimiza
-00004c30: 7469 6f6e 2069 6620 6060 5472 7565 6060  tion if ``True``
-00004c40: 2e0a 2020 2020 2020 2020 7072 696e 745f  ..        print_
-00004c50: 6576 6572 790a 2020 2020 2020 2020 2020  every.          
-00004c60: 2020 5072 696e 7420 6672 6571 7565 6e63    Print frequenc
-00004c70: 7920 6966 2076 6572 626f 7365 2069 7320  y if verbose is 
-00004c80: 6060 5472 7565 6060 2e0a 2020 2020 2020  ``True``..      
-00004c90: 2020 6c6f 675f 6576 6572 790a 2020 2020    log_every.    
-00004ca0: 2020 2020 2020 2020 6074 656e 736f 7262          `tensorb
-00004cb0: 6f61 7264 6020 6c6f 6720 6672 6571 7565  oard` log freque
-00004cc0: 6e63 7920 6966 2077 7269 7465 2064 6972  ncy if write dir
-00004cd0: 6563 746f 7279 2069 7320 7370 6563 6966  ectory is specif
-00004ce0: 6965 640a 0a20 2020 2020 2020 2052 6574  ied..        Ret
-00004cf0: 7572 6e73 0a20 2020 2020 2020 202d 2d2d  urns.        ---
-00004d00: 2d2d 2d2d 0a20 2020 2020 2020 2065 7870  ----.        exp
-00004d10: 6c61 6e61 7469 6f6e 0a20 2020 2020 2020  lanation.       
-00004d20: 2020 2020 2060 4578 706c 616e 6174 696f       `Explanatio
-00004d30: 6e60 206f 626a 6563 7420 636f 6e74 6169  n` object contai
-00004d40: 6e69 6e67 2074 6865 2063 6f75 6e74 6572  ning the counter
-00004d50: 6661 6374 7561 6c20 7769 7468 2061 6464  factual with add
-00004d60: 6974 696f 6e61 6c20 6d65 7461 6461 7461  itional metadata
-00004d70: 2061 7320 6174 7472 6962 7574 6573 2e0a   as attributes..
-00004d80: 2020 2020 2020 2020 7201 0000 0072 1800          r....r..
-00004d90: 0000 7a59 4375 7272 656e 746c 7920 6f6e  ..zYCurrently on
-00004da0: 6c79 2073 696e 676c 6520 696e 7374 616e  ly single instan
-00004db0: 6365 2065 7870 6c61 6e61 7469 6f6e 7320  ce explanations 
-00004dc0: 7375 7070 6f72 7465 6420 2866 6972 7374  supported (first
-00004dd0: 2064 696d 203d 2031 292c 2062 7574 2066   dim = 1), but f
-00004de0: 6972 7374 2064 696d 203d 2025 734e 72a2  irst dim = %sNr.
-00004df0: 0000 00da 0a6f 7269 675f 7072 6f62 6172  .....orig_probar
-00004e00: 7500 0000 72b3 0000 0046 2907 72bb 0000  u...r....F).r...
-00004e10: 0072 bc00 0000 72b5 0000 0072 bd00 0000  .r....r....r....
-00004e20: 722c 0000 0072 be00 0000 72bf 0000 0072  r,...r....r....r
-00004e30: d100 0000 7a18 4e6f 2063 6f75 6e74 6572  ....z.No counter
-00004e40: 6661 6374 7561 6c20 666f 756e 6421 2902  factual found!).
-00004e50: 722e 0000 0072 7000 0000 da03 616c 6cda  r....rp.....all.
-00004e60: 0263 6672 b100 0000 72ec 0000 00da 0563  .cfr....r......c
-00004e70: 6c61 7373 da05 6772 6164 7329 1872 1b00  lass..grads).r..
-00004e80: 0000 724d 0000 0072 4e00 0000 7243 0000  ..rM...rN...rC..
-00004e90: 0072 4400 0000 7207 0000 0072 1900 0000  .rD...r....r....
-00004ea0: 7257 0000 0072 4900 0000 72c5 0000 00da  rW...rI...r.....
-00004eb0: 0661 7261 6e67 6572 6f00 0000 7239 0000  .arangero...r9..
-00004ec0: 0072 e300 0000 72ee 0000 0072 2c00 0000  .r....r....r,...
-00004ed0: 7234 0000 0072 d100 0000 720a 0000 0072  r4...r....r....r
-00004ee0: 2e00 0000 72d2 0000 00da 0a66 726f 6d5f  ....r......from_
-00004ef0: 6e75 6d70 7972 d300 0000 72dc 0000 0029  numpyr....r....)
-00004f00: 1072 3000 0000 72b1 0000 0072 bb00 0000  .r0...r....r....
-00004f10: 72bc 0000 0072 b500 0000 72bd 0000 0072  r....r....r....r
-00004f20: be00 0000 72bf 0000 0072 7000 0000 5a07  ....r....rp...Z.
-00004f30: 595f 7072 6f62 615a 0559 5f6f 6865 72ed  Y_probaZ.Y_oher.
-00004f40: 0000 0072 e300 0000 72f3 0000 00da 0b65  ...r....r......e
-00004f50: 7870 6c61 6e61 7469 6f6e 5a06 595f 7065  xplanationZ.Y_pe
-00004f60: 7274 723e 0000 0072 3e00 0000 723f 0000  rtr>...r>...r?..
-00004f70: 00da 0765 7870 6c61 696e d202 0000 7350  ...explain....sP
-00004f80: 0000 0000 2f0e 0104 0102 0208 fd04 070a  ..../...........
-00004f90: 030a 0108 010c 010e 0118 0108 0108 0116  ................
-00004fa0: 0306 0104 0102 0102 0102 0102 0102 0104  ................
-00004fb0: 0102 0102 f80a 0c06 010a 0306 010a 0314  ................
-00004fc0: 0104 020a 0108 010c 0118 010c 011a 0114  ................
-00004fd0: 0314 027a 1643 6f75 6e74 6572 6661 6374  ...z.Counterfact
-00004fe0: 7561 6c2e 6578 706c 6169 6e29 1172 0d00  ual.explain).r..
-00004ff0: 0000 720e 0000 0072 0f00 0000 720d 0000  ..r....r....r...
-00005000: 004e 4e72 0d00 0000 4672 1100 0000 7212  .NNr....Fr....r.
-00005010: 0000 0072 1300 0000 7214 0000 0072 1500  ...r....r....r..
-00005020: 0000 7217 0000 0072 1800 0000 4e46 2901  ..r....r....NF).
-00005030: 72b0 0000 0029 064e 4e72 a800 0000 720d  r....).NNr....r.
-00005040: 0000 0046 72ba 0000 0029 064e 4e4e 72a8  ...Fr....).NNNr.
-00005050: 0000 0072 0d00 0000 72ba 0000 0029 24da  ...r....r....)$.
-00005060: 085f 5f6e 616d 655f 5fda 0a5f 5f6d 6f64  .__name__..__mod
-00005070: 756c 655f 5fda 0c5f 5f71 7561 6c6e 616d  ule__..__qualnam
-00005080: 655f 5f72 0500 0000 7202 0000 0072 5700  e__r....r....rW.
-00005090: 0000 72c8 0000 0072 3900 0000 724b 0000  ..r....r9...rK..
-000050a0: 0072 4c00 0000 7255 0000 0072 3800 0000  .rL...rU...r8...
-000050b0: 7204 0000 0072 0300 0000 72c9 0000 0072  r....r....r....r
-000050c0: c200 0000 da03 7374 7272 4200 0000 7266  ......strrB...rf
-000050d0: 0000 0072 6d00 0000 7271 0000 0072 7400  ...rm...rq...rt.
-000050e0: 0000 727e 0000 0072 8200 0000 728b 0000  ..r~...r....r...
-000050f0: 0072 8f00 0000 7292 0000 0072 9f00 0000  .r....r....r....
-00005100: da05 6172 7261 7972 af00 0000 72b9 0000  ..arrayr....r...
-00005110: 0072 ca00 0000 72ee 0000 0072 0a00 0000  .r....r....r....
-00005120: 72f7 0000 00da 0d5f 5f63 6c61 7373 6365  r......__classce
-00005130: 6c6c 5f5f 723e 0000 0072 3e00 0000 725d  ll__r>...r>...r]
-00005140: 0000 0072 3f00 0000 720c 0000 0011 0000  ...r?...r.......
-00005150: 0073 c400 0000 0806 0001 0001 0004 0001  .s..............
-00005160: 0001 0001 0001 0001 0001 0001 0001 0001  ................
-00005170: 0001 0001 0001 0001 00e8 0202 1c01 1c01  ................
-00005180: 0201 0201 0201 1e04 0201 0a01 0a01 0201  ................
-00005190: 0201 0201 0201 0201 0201 0201 0201 0201  ................
-000051a0: 0601 0201 02e7 107f 0026 080f 080a 0805  .........&......
-000051b0: 0805 0815 080d 0824 0812 0815 080c 0801  .......$........
-000051c0: 08fd 0202 0401 0401 02fc 0c2a 00ff 0201  ...........*....
-000051d0: 0a01 02fe 0c29 0001 0001 0001 0001 0001  .....)..........
-000051e0: 00f7 0202 0401 0401 0601 0601 0201 0201  ................
-000051f0: 0201 0201 18f6 0c7f 007f 0039 0001 0001  ...........9....
-00005200: 0001 0001 0001 00f7 0203 0401 0801 0601  ................
-00005210: 0601 0201 0201 0201 02f6 720c 0000 0063  ..........r....c
-00005220: 0100 0000 0000 0000 0000 0000 0200 0000  ................
-00005230: 0800 0000 4300 0000 7338 0000 0074 007c  ....C...s8...t.|
-00005240: 0064 0183 028f 1a7d 0174 01a0 027c 01a1  .d.....}.t...|..
-00005250: 0157 0002 0064 0004 0004 0083 0301 0053  .W...d.........S
-00005260: 0031 0073 2a30 0001 0001 0001 0059 0001  .1.s*0.......Y..
-00005270: 0064 0053 0029 024e da02 7262 2903 da04  .d.S.).N..rb)...
-00005280: 6f70 656e da06 7069 636b 6c65 da04 6c6f  open..pickle..lo
-00005290: 6164 2902 da08 6669 6c65 6e61 6d65 da04  ad)...filename..
-000052a0: 6f75 7470 723e 0000 0072 3e00 0000 723f  outpr>...r>...r?
-000052b0: 0000 0072 a900 0000 3c03 0000 7304 0000  ...r....<...s...
-000052c0: 0000 010c 0172 a900 0000 6301 0000 0000  .....r....c.....
-000052d0: 0000 0000 0000 0001 0000 0005 0000 0043  ...............C
-000052e0: 0000 0073 5400 0000 7400 7c00 7401 6a02  ...sT...t.|.t.j.
-000052f0: 8302 7250 7c00 a003 a100 6401 6b02 7250  ..rP|.....d.k.rP
-00005300: 7c00 6a04 7401 6a05 7401 6a06 7401 6a07  |.j.t.j.t.j.t.j.
-00005310: 7401 6a08 6604 7600 7236 6402 5300 7c00  t.j.f.v.r6d.S.|.
-00005320: 6a04 7401 6a09 7401 6a0a 7401 6a0b 6603  j.t.j.t.j.t.j.f.
-00005330: 7600 7250 6402 5300 6403 5300 2904 4e72  v.rPd.S.d.S.).Nr
-00005340: 1800 0000 5446 290c 7237 0000 0072 3900  ....TF).r7...r9.
-00005350: 0000 da06 5465 6e73 6f72 da05 6e75 6d65  ....Tensor..nume
-00005360: 6c72 3600 0000 da05 696e 7433 3272 c300  lr6.....int32r..
-00005370: 0000 da05 696e 7431 36da 0469 6e74 3872  ....int16..int8r
-00005380: 5400 0000 da07 666c 6f61 7436 34da 0766  T.....float64..f
-00005390: 6c6f 6174 3136 2901 72c0 0000 0072 3e00  loat16).r....r>.
-000053a0: 0000 723e 0000 0072 3f00 0000 72c4 0000  ..r>...r?...r...
-000053b0: 0041 0300 0073 0c00 0000 0002 1802 1a01  .A...s..........
-000053c0: 0402 1601 0402 72c4 0000 0063 0600 0000  ......r....c....
-000053d0: 0000 0000 0000 0000 0600 0000 0400 0000  ................
-000053e0: 4300 0000 7318 0000 0074 007c 016a 019b  C...s....t.|.j..
-000053f0: 0064 017c 009b 009d 0383 0101 0064 0053  .d.|.........d.S
-00005400: 0029 024e 7a02 3a20 2902 72cb 0000 0072  .).Nz.: ).r....r
-00005410: f800 0000 2906 da07 6d65 7373 6167 65da  ....)...message.
-00005420: 0863 6174 6567 6f72 7972 0201 0000 da06  .categoryr......
-00005430: 6c69 6e65 6e6f da04 6669 6c65 da04 6c69  lineno..file..li
-00005440: 6e65 723e 0000 0072 3e00 0000 723f 0000  ner>...r>...r?..
-00005450: 0072 5900 0000 4f03 0000 7302 0000 0000  .rY...O...s.....
-00005460: 0172 5900 0000 2902 4e4e 291b da02 6f73  .rY...).NN)...os
-00005470: 7243 0000 0072 dd00 0000 da07 5f70 6963  rC...r......_pic
-00005480: 6b6c 6572 0001 0000 da06 7479 7069 6e67  kler......typing
-00005490: 7202 0000 0072 0300 0000 7204 0000 0072  r....r....r....r
-000054a0: 0500 0000 72dc 0000 0072 5700 0000 724d  ....r....rW...rM
-000054b0: 0000 0072 3900 0000 da0b 746f 7263 682e  ...r9.....torch.
-000054c0: 6f70 7469 6d72 9a00 0000 5a0c 6170 692e  optimr....Z.api.
-000054d0: 6465 6661 756c 7473 7207 0000 0072 0800  defaultsr....r..
-000054e0: 0000 5a0e 6170 692e 696e 7465 7266 6163  ..Z.api.interfac
-000054f0: 6573 7209 0000 0072 0a00 0000 720b 0000  esr....r....r...
-00005500: 0072 0c00 0000 72a9 0000 0072 c400 0000  .r....r....r....
-00005510: 7259 0000 0072 3e00 0000 723e 0000 0072  rY...r>...r>...r
-00005520: 3e00 0000 723f 0000 00da 083c 6d6f 6475  >...r?.....<modu
-00005530: 6c65 3e01 0000 0073 2800 0000 0801 0801  le>....s(.......
-00005540: 0801 0801 1801 0801 0802 0801 0c02 1001  ................
-00005550: 1404 127f 007f 007f 007f 007f 007f 0031  ...............1
-00005560: 0805 080e                                ....
+00000040: 6401 6c02 5a02 6400 6401 6c03 5a03 6400  d.l.Z.d.d.l.Z.d.
+00000050: 6401 6c04 5a05 6400 6402 6c06 6d07 5a07  d.l.Z.d.d.l.m.Z.
+00000060: 6d08 5a08 6d09 5a09 6d0a 5a0a 6d0b 5a0b  m.Z.m.Z.m.Z.m.Z.
+00000070: 0100 6400 6401 6c0c 5a0d 6400 6401 6c0e  ..d.d.l.Z.d.d.l.
+00000080: 6d0f 0200 0100 6d10 5a11 0100 6403 6404  m.....m.Z...d.d.
+00000090: 6c12 6d13 5a13 6d14 5a14 0100 6403 6405  l.m.Z.m.Z...d.d.
+000000a0: 6c15 6d16 5a16 6d17 5a17 6d18 5a18 0100  l.m.Z.m.Z.m.Z...
+000000b0: 6403 6406 6c19 6d1a 5a1a 0100 6400 6401  d.d.l.m.Z...d.d.
+000000c0: 6c1b 5a1b 6502 a01c 651d a101 5a1e 6511  l.Z.e...e...Z.e.
+000000d0: 6a02 a01f 6511 6a02 6a20 a101 0100 6511  j...e.j.j ....e.
+000000e0: 6a0f 6a10 a021 a100 0100 4700 6407 6408  j.j..!....G.d.d.
+000000f0: 8400 6408 6516 6518 8304 5a22 6409 640a  ..d.e.e...Z"d.d.
+00000100: 8400 5a23 640b 640c 8400 5a24 6401 5300  ..Z#d.d...Z$d.S.
+00000110: 290d e900 0000 004e 2905 da03 416e 79da  )......N)...Any.
+00000120: 0843 616c 6c61 626c 65da 084f 7074 696f  .Callable..Optio
+00000130: 6e61 6cda 0554 7570 6c65 da05 556e 696f  nal..Tuple..Unio
+00000140: 6ee9 0200 0000 2902 da0c 4445 4641 554c  n.....)...DEFAUL
+00000150: 545f 4441 5441 da0c 4445 4641 554c 545f  T_DATA..DEFAULT_
+00000160: 4d45 5441 2903 da09 4578 706c 6169 6e65  META)...Explaine
+00000170: 72da 0b45 7870 6c61 6e61 7469 6f6e da08  r..Explanation..
+00000180: 4669 744d 6978 696e 2901 da07 7065 7274  FitMixin)...pert
+00000190: 7572 6263 0000 0000 0000 0000 0000 0000  urbc............
+000001a0: 0000 0000 1900 0000 0000 0000 73ae 0100  ............s...
+000001b0: 0065 005a 0164 005a 0264 2565 0365 0465  .e.Z.d.Z.d%e.e.e
+000001c0: 056a 0667 0165 056a 0666 0219 0065 076a  .j.g.e.j.f...e.j
+000001d0: 086a 0966 0219 0065 0365 0465 056a 0667  .j.f...e.e.e.j.g
+000001e0: 0165 056a 0666 0219 0065 076a 086a 0966  .e.j.f...e.j.j.f
+000001f0: 0219 0065 0a65 0b65 0b65 0c65 0365 0b65  ...e.e.e.e.e.e.e
+00000200: 056a 0666 0219 0065 0365 0b65 056a 0666  .j.f...e.e.e.j.f
+00000210: 0219 0066 0219 0065 0b65 0d65 076a 086a  ...f...e.e.e.j.j
+00000220: 0919 0065 0d65 076a 086a 0919 0065 0b65  ...e.e.j.j...e.e
+00000230: 0e65 0b65 0f65 0b65 0f65 0a65 0a65 0f65  .e.e.e.e.e.e.e.e
+00000240: 0d65 1019 0065 0d65 1019 0065 0d65 076a  .e...e.e...e.e.j
+00000250: 1119 0065 0e64 0464 0d9c 1787 0066 0164  ...e.d.d.....f.d
+00000260: 0e64 0f84 0d5a 1265 05a0 1367 00a1 0165  .d...Z.e...g...e
+00000270: 05a0 1367 00a1 0164 0466 0365 056a 0665  ...g...d.f.e.j.e
+00000280: 056a 0665 0d65 1419 0064 0064 109c 0464  .j.e.e...d.d...d
+00000290: 1164 1284 055a 1565 056a 0665 056a 0665  .d...Z.e.j.e.j.e
+000002a0: 056a 0664 139c 0364 1464 1584 045a 1665  .j.d...d.d...Z.e
+000002b0: 056a 0665 056a 0665 0a65 056a 0664 169c  .j.e.j.e.e.j.d..
+000002c0: 0464 1764 1884 045a 1764 2665 056a 0665  .d.d...Z.d&e.j.e
+000002d0: 0f65 0f65 0b65 0b64 1a9c 0564 1b64 1c84  .e.e.e.d...d.d..
+000002e0: 055a 1864 2765 056a 0665 056a 0665 0d65  .Z.d'e.j.e.j.e.e
+000002f0: 1919 0065 0d65 0f19 0065 1065 0b65 0e65  ...e.e...e.e.e.e
+00000300: 0f65 0f65 0c65 056a 0665 0c65 056a 0665  .e.e.e.j.e.e.j.e
+00000310: 056a 0666 0219 0066 0219 0064 1f9c 0a64  .j.f...f...d...d
+00000320: 2064 2184 055a 1a64 2865 056a 0665 0d65   d!..Z.d(e.j.e.e
+00000330: 056a 0619 0065 0d65 1919 0065 0d65 0f19  .j...e.e...e.e..
+00000340: 0065 1065 0b65 0f65 0f65 1b64 229c 0964  .e.e.e.e.e.d"..d
+00000350: 2364 2484 055a 1c87 0004 005a 1d53 0029  #d$..Z.....Z.S.)
+00000360: 29da 0e43 6f75 6e74 6572 6661 6374 7561  )..Counterfactua
+00000370: 6ce7 0000 0000 0000 0000 e79a 9999 9999  l...............
+00000380: 99b9 3fa9 0267 0000 0020 5fa0 02c2 e700  ..?..g... _.....
+00000390: 0000 205f a002 424e 46e7 7b14 ae47 e17a  .. _..BNF.{..G.z
+000003a0: 843f e9e8 0300 00e7 0000 0000 0000 2440  .?............$@
+000003b0: e90a 0000 00a9 02e7 fca9 f1d2 4d62 503f  ............MbP?
+000003c0: 7218 0000 00a9 0267 0000 0000 0040 8fc0  r......g.....@..
+000003d0: 6700 0000 0000 408f 40e9 0100 0000 2917  g.....@.@.....).
+000003e0: da07 7072 6564 6963 74da 0f69 6e70 7574  ..predict..input
+000003f0: 5f74 7261 6e73 666f 726d da05 7368 6170  _transform..shap
+00000400: 65da 056b 6170 7061 da04 6265 7461 da0d  e..kappa..beta..
+00000410: 6665 6174 7572 655f 7261 6e67 65da 0567  feature_range..g
+00000420: 616d 6d61 da08 6165 5f6d 6f64 656c da09  amma..ae_model..
+00000430: 656e 635f 6d6f 6465 6cda 0574 6865 7461  enc_model..theta
+00000440: da0a 7573 655f 6b64 7472 6565 da12 6c65  ..use_kdtree..le
+00000450: 6172 6e69 6e67 5f72 6174 655f 696e 6974  arning_rate_init
+00000460: da0e 6d61 785f 6974 6572 6174 696f 6e73  ..max_iterations
+00000470: da06 635f 696e 6974 da07 635f 7374 6570  ..c_init..c_step
+00000480: 73da 0365 7073 da04 636c 6970 da0f 7570  s..eps..clip..up
+00000490: 6461 7465 5f6e 756d 5f67 7261 64da 0a74  date_num_grad..t
+000004a0: 7275 7374 7363 6f72 65da 0977 7269 7465  rustscore..write
+000004b0: 5f64 6972 da04 7365 7373 da07 7665 7262  _dir..sess..verb
+000004c0: 6f73 65da 0672 6574 7572 6e63 1700 0000  ose..returnc....
+000004d0: 0000 0000 0000 0000 2d00 0000 0c00 0000  ........-.......
+000004e0: 0300 0000 73a2 0c00 0074 0083 006a 0174  ....s....t...j.t
+000004f0: 02a0 0374 04a1 0164 018d 0101 0074 0588  ...t...d.....t..
+00000500: 0183 0164 026b 0472 3e88 0164 0364 0485  ...d.k.r>..d.d..
+00000510: 0219 007d 1788 0164 0519 0088 0164 0619  ...}...d.....d..
+00000520: 0066 0289 016e 0488 017d 1774 0683 007d  .f...n...}.t...}
+00000530: 1867 0064 07a2 017d 197c 1944 005d 0e7d  .g.d...}.|.D.].}
+00000540: 1a7c 18a0 077c 1aa1 0101 0071 547c 006a  .|...|.....qT|.j
+00000550: 0864 0819 00a0 097c 18a1 0101 007c 017c  .d.....|.....|.|
+00000560: 005f 0a7c 137c 005f 0b74 0c7c 0174 0d6a  ._.|.|._.t.|.t.j
+00000570: 0e6a 0f83 027d 1b74 0d6a 106a 116a 0e6a  .j...}.t.j.j.j.j
+00000580: 12a0 13a1 007d 1c74 0c7c 0874 0d6a 0e6a  .....}.t.|.t.j.j
+00000590: 0f83 027d 1d74 0c7c 0974 0d6a 0e6a 0f83  ...}.t.|.t.j.j..
+000005a0: 027d 1e7c 006a 0864 0819 006a 097c 1b7c  .}.|.j.d...j.|.|
+000005b0: 1d7c 1e64 098d 0301 0074 0c7c 1574 0d6a  .|.d.....t.|.t.j
+000005c0: 1483 0272 e47c 157c 005f 156e 067c 1c7c  ...r.|.|._.n.|.|
+000005d0: 005f 157c 1b90 0172 1264 0a7c 005f 167c  ._.|...r.d.|._.|
+000005e0: 006a 0aa0 0a74 17a0 1888 01a1 01a1 016a  .j...t.........j
+000005f0: 1964 0319 007c 005f 1a6e 3264 0b7c 005f  .d...|._.n2d.|._
+00000600: 167c 00a0 0a74 1b6a 1888 0164 0c8d 01a1  .|...t.j...d....
+00000610: 016a 1964 0319 007c 005f 1a74 1c64 0d7c  .j.d...|._.t.d.|
+00000620: 006a 1a9b 0064 0e9d 0383 0101 007c 1e90  .j...d.......|..
+00000630: 0172 5264 0a7c 005f 1d6e 0664 0b7c 005f  .rRd.|._.n.d.|._
+00000640: 1d7c 1d90 0172 6664 0a7c 005f 1e6e 0664  .|...rfd.|._.n.d
+00000650: 0b7c 005f 1e7c 0b90 0172 847c 006a 1d90  .|._.|...r.|.j..
+00000660: 0172 8474 1fa0 2064 0fa1 0101 007c 0b90  .r.t.. d.....|..
+00000670: 0173 927c 006a 1d90 0172 9a64 0a7c 005f  .s.|.j...r.d.|._
+00000680: 216e 0664 0b7c 005f 217c 006a 0864 0819  !n.d.|._!|.j.d..
+00000690: 006a 097c 006a 2164 108d 0101 007c 006a  .j.|.j!d.....|.j
+000006a0: 0864 0819 006a 0964 0b64 118d 0101 0088  .d...j.d.d......
+000006b0: 017c 005f 197c 177c 005f 227c 047c 005f  .|._.|.|._"|.|._
+000006c0: 237c 057c 005f 247c 077c 005f 257c 0a7c  #|.|._$|.|._%|.|
+000006d0: 005f 267c 087c 005f 277c 097c 005f 287c  ._&|.|._'|.|._(|
+000006e0: 0b7c 005f 2988 0164 0519 007c 005f 2a7c  .|._)..d...|._*|
+000006f0: 0d7c 005f 2b7c 0e7c 005f 2c7c 0f7c 005f  .|._+|.|._,|.|._
+00000700: 2d74 2e87 0087 0166 0264 1264 1384 0874  -t.....f.d.d...t
+00000710: 2f64 0283 0144 0083 0183 017c 005f 307c  /d...D.....|._0|
+00000720: 127c 005f 317c 107c 005f 327c 117c 005f  .|._1|.|._2|.|._
+00000730: 337c 027c 005f 347c 147c 005f 357c 167c  3|.|._4|.|._5|.|
+00000740: 005f 3674 0d6a 3774 17a0 1888 01a1 0174  ._6t.j7t.......t
+00000750: 0d6a 3864 1464 158d 037c 005f 3974 0d6a  .j8d.d...|._9t.j
+00000760: 3774 17a0 1888 01a1 0174 0d6a 3864 1664  7t.......t.j8d.d
+00000770: 158d 037c 005f 3a74 0d6a 3774 17a0 1888  ...|._:t.j7t....
+00000780: 01a1 0174 0d6a 3864 1764 158d 037c 005f  ...t.j8d.d...|._
+00000790: 3b74 0d6a 3774 17a0 187c 006a 2a7c 006a  ;t.j7t...|.j*|.j
+000007a0: 1a66 02a1 0174 0d6a 3864 1864 158d 037c  .f...t.j8d.d...|
+000007b0: 005f 3c7c 006a 1d90 0272 ec7c 006a 28a0  ._<|.j...r.|.j(.
+000007c0: 0a74 17a0 187c 006a 19a1 01a1 016a 197c  .t...|.j.....j.|
+000007d0: 005f 3d6e 087c 006a 197c 005f 3d74 0d6a  ._=n.|.j.|._=t.j
+000007e0: 3774 17a0 187c 006a 3da1 0174 0d6a 3864  7t...|.j=..t.j8d
+000007f0: 1964 158d 037c 005f 3e74 0d6a 3774 17a0  .d...|._>t.j7t..
+00000800: 187c 006a 2aa1 0174 0d6a 3864 1a64 158d  .|.j*..t.j8d.d..
+00000810: 037c 005f 3f74 0d6a 3764 1b64 0b64 1c64  .|._?t.j7d.d.d.d
+00000820: 1d8d 037c 005f 4074 0d6a 4174 0d6a 3888  ...|._@t.jAt.j8.
+00000830: 0164 1e64 1f8d 037c 005f 4274 0d6a 4174  .d.d...|._Bt.jAt
+00000840: 0d6a 3888 0164 2064 1f8d 037c 005f 4374  .j8..d d...|._Ct
+00000850: 0d6a 4174 0d6a 3888 0164 2164 1f8d 037c  .jAt.j8..d!d...|
+00000860: 005f 4474 0d6a 4174 0d6a 387c 006a 2a7c  ._Dt.jAt.j8|.j*|
+00000870: 006a 1a66 0264 2264 1f8d 037c 005f 4574  .j.f.d"d...|._Et
+00000880: 0d6a 4174 0d6a 387c 006a 2a67 0164 2364  .jAt.j8|.j*g.d#d
+00000890: 1f8d 037c 005f 4674 0d6a 4174 0d6a 387c  ...|._Ft.jAt.j8|
+000008a0: 006a 3d64 2464 1f8d 037c 005f 4774 0da0  .j=d$d...|._Gt..
+000008b0: 4864 25a1 0190 018f 067d 1f74 0da0 4974  Hd%......}.t..It
+000008c0: 0da0 4a74 0da0 4b7c 006a 3b7c 006a 39a1  ..Jt..K|.j;|.j9.
+000008d0: 027c 006a 24a1 0274 0d6a 38a1 0274 0da0  .|.j$..t.j8..t..
+000008e0: 4974 0da0 4c74 0da0 4d74 0da0 4b7c 006a  It..Lt..Mt..K|.j
+000008f0: 3b7c 006a 39a1 02a1 017c 006a 24a1 0274  ;|.j9....|.j$..t
+00000900: 0d6a 38a1 0274 0da0 4974 0da0 4e74 0da0  .j8..t..It..Nt..
+00000910: 4b7c 006a 3b7c 006a 39a1 0274 0da0 4f7c  K|.j;|.j9..t..O|
+00000920: 006a 24a1 01a1 0274 0d6a 38a1 0267 037d  .j$....t.j8..g.}
+00000930: 2074 0da0 5074 0da0 4b7c 006a 3b7c 006a   t..Pt..K|.j;|.j
+00000940: 24a1 0274 0da0 4988 0064 0319 0074 0d6a  $..t..I..d...t.j
+00000950: 38a1 02a1 027d 2174 0da0 5174 0da0 527c  8....}!t..Qt..R|
+00000960: 006a 3b7c 006a 24a1 0274 0da0 4988 0064  .j;|.j$..t..I..d
+00000970: 0519 0074 0d6a 38a1 02a1 027d 2274 0da0  ...t.j8....}"t..
+00000980: 537c 2064 0519 007c 21a1 0274 0da0 537c  S| d...|!..t..S|
+00000990: 2064 0319 007c 006a 39a1 0217 0074 0da0   d...|.j9....t..
+000009a0: 537c 2064 0219 007c 22a1 0217 007c 005f  S| d...|"....|._
+000009b0: 4357 0064 0404 0004 0083 0301 006e 1231  CW.d.........n.1
+000009c0: 0090 0473 de30 0001 0001 0001 0059 0001  ...s.0.......Y..
+000009d0: 0074 0da0 4864 26a1 018f 8a7d 1f74 0da0  .t..Hd&....}.t..
+000009e0: 547c 006a 407c 006a 4074 0da0 4964 2774  T|.j@|.j@t..Id't
+000009f0: 0d6a 38a1 0217 00a1 027c 005f 557c 006a  .j8......|._U|.j
+00000a00: 4374 0da0 537c 006a 557c 006a 437c 006a  Ct..S|.jU|.jC|.j
+00000a10: 3a18 00a1 0217 007c 005f 4474 0da0 507c  :......|._Dt..P|
+00000a20: 006a 4474 0da0 4988 0064 0319 0074 0d6a  .jDt..I..d...t.j
+00000a30: 38a1 02a1 027c 005f 4474 0da0 517c 006a  8....|._Dt..Q|.j
+00000a40: 4474 0da0 4988 0064 0519 0074 0d6a 38a1  Dt..I..d...t.j8.
+00000a50: 02a1 027c 005f 4457 0064 0404 0004 0083  ...|._DW.d......
+00000a60: 0301 006e 1231 0090 0573 8430 0001 0001  ...n.1...s.0....
+00000a70: 0001 0059 0001 0074 0da0 4864 28a1 018f  ...Y...t..Hd(...
+00000a80: 347d 1f74 0da0 567c 006a 3a7c 006a 43a1  4}.t..V|.j:|.jC.
+00000a90: 027c 005f 5774 0da0 567c 006a 3b7c 006a  .|._Wt..V|.j;|.j
+00000aa0: 44a1 027c 005f 5857 0064 0404 0004 0083  D..|._XW.d......
+00000ab0: 0301 006e 1231 0090 0573 d430 0001 0001  ...n.1...s.0....
+00000ac0: 0001 0059 0001 0074 0da0 4864 29a1 018f  ...Y...t..Hd)...
+00000ad0: 2c7d 1f7c 006a 397c 006a 3a18 007c 005f  ,}.|.j9|.j:..|._
+00000ae0: 597c 006a 397c 006a 3b18 007c 005f 5a57  Y|.j9|.j;..|._ZW
+00000af0: 0064 0404 0004 0083 0301 006e 1231 0090  .d.........n.1..
+00000b00: 0673 1c30 0001 0001 0001 0059 0001 0074  .s.0.......Y...t
+00000b10: 5b74 17a0 5c64 0374 0588 0183 01a1 0283  [t..\d.t........
+00000b20: 017d 2374 0da0 4864 2aa1 018f d87d 1f74  .}#t..Hd*....}.t
+00000b30: 0d6a 5d74 0da0 5e7c 006a 59a1 017c 2364  .j]t..^|.jY..|#d
+00000b40: 2b8d 027c 005f 5f74 0d6a 5d74 0da0 5e7c  +..|.__t.j]t..^|
+00000b50: 006a 5aa1 017c 2364 2b8d 027c 005f 6074  .jZ..|#d+..|._`t
+00000b60: 0d6a 5d74 0da0 4d7c 006a 59a1 017c 2364  .j]t..M|.jY..|#d
+00000b70: 2b8d 027c 005f 6174 0d6a 5d74 0da0 4d7c  +..|._at.j]t..M|
+00000b80: 006a 5aa1 017c 2364 2b8d 027c 005f 627c  .jZ..|#d+..|._b|
+00000b90: 006a 5f74 0da0 537c 006a 617c 006a 24a1  .j_t..S|.ja|.j$.
+00000ba0: 0217 007c 005f 637c 006a 6074 0da0 537c  ...|._c|.j`t..S|
+00000bb0: 006a 627c 006a 24a1 0217 007c 005f 6474  .jb|.j$....|._dt
+00000bc0: 0da0 5d7c 006a 61a1 017c 005f 6574 0da0  ..]|.ja..|._et..
+00000bd0: 5d7c 006a 62a1 017c 005f 6674 0da0 5d7c  ]|.jb..|._ft..]|
+00000be0: 006a 5fa1 017c 005f 6774 0da0 5d7c 006a  .j_..|._gt..]|.j
+00000bf0: 60a1 017c 005f 6857 0064 0404 0004 0083  `..|._hW.d......
+00000c00: 0301 006e 1231 0090 0773 2430 0001 0001  ...n.1...s$0....
+00000c10: 0001 0059 0001 007c 006a 3a7c 005f 697c  ...Y...|.j:|._i|
+00000c20: 006a 3b7c 005f 6a74 0da0 4864 2ca1 018f  .j;|._jt..Hd,...
+00000c30: 8e7d 1f7c 006a 1e90 0772 b07c 00a0 277c  .}.|.j...r.|..'|
+00000c40: 006a 69a1 017c 005f 6b7c 00a0 277c 006a  .ji..|._k|..'|.j
+00000c50: 6aa1 017c 005f 6c7c 006a 2574 0da0 5e74  j..|._l|.j%t..^t
+00000c60: 0da0 6d7c 006a 6b7c 006a 3a18 00a1 01a1  ..m|.jk|.j:.....
+00000c70: 0114 007c 005f 6e7c 006a 2574 0da0 5e74  ...|._n|.j%t..^t
+00000c80: 0da0 6d7c 006a 6c7c 006a 3b18 00a1 01a1  ..m|.jl|.j;.....
+00000c90: 0114 007c 005f 6f6e 1874 0da0 7064 1ba1  ...|._on.t..pd..
+00000ca0: 017c 005f 6e74 0da0 7064 1ba1 017c 005f  .|._nt..pd...|._
+00000cb0: 6f57 0064 0404 0004 0083 0301 006e 1231  oW.d.........n.1
+00000cc0: 0090 0773 de30 0001 0001 0001 0059 0001  ...s.0.......Y..
+00000cd0: 0074 0da0 4864 2da1 0190 018f 5c7d 1f7c  .t..Hd-.....\}.|
+00000ce0: 006a 1690 0873 1074 0da0 4174 0d6a 38a1  .j...s.t..At.j8.
+00000cf0: 017c 005f 7190 016e 327c 006a 2c64 1b6b  .|._q..n2|.j,d.k
+00000d00: 0290 0872 5e7c 006a 2d64 036b 0290 0872  ...r^|.j-d.k...r
+00000d10: 5e7c 00a0 0a7c 006a 69a1 017c 005f 727c  ^|...|.ji..|._r|
+00000d20: 00a0 0a7c 006a 6aa1 017c 005f 7374 0da0  ...|.jj..|._st..
+00000d30: 7064 1ba1 017c 005f 7174 0da0 7064 1ba1  pd...|._qt..pd..
+00000d40: 017c 005f 746e e47c 00a0 0a7c 006a 69a1  .|._tn.|...|.ji.
+00000d50: 017c 005f 727c 00a0 0a7c 006a 6aa1 017c  .|._r|...|.jj..|
+00000d60: 005f 7374 0da0 5d7c 006a 3c7c 006a 7214  ._st..]|.j<|.jr.
+00000d70: 0064 03a1 027c 005f 7574 0da0 5d7c 006a  .d...|._ut..]|.j
+00000d80: 3c7c 006a 7314 0064 03a1 027d 2474 0da0  <|.js..d...}$t..
+00000d90: 7664 037c 006a 3c18 007c 006a 7214 007c  vd.|.j<..|.jr..|
+00000da0: 006a 3c64 2e14 0018 0064 03a1 027c 005f  .j<d.....d...|._
+00000db0: 7774 0da0 7664 037c 006a 3c18 007c 006a  wt..vd.|.j<..|.j
+00000dc0: 7314 007c 006a 3c64 2e14 0018 0064 03a1  s..|.j<d.....d..
+00000dd0: 027d 2574 0da0 5164 1b7c 006a 770b 007c  .}%t..Qd.|.jw..|
+00000de0: 006a 7517 007c 006a 2317 00a1 027d 2674  .ju..|.j#....}&t
+00000df0: 0da0 5164 1b7c 250b 007c 2417 007c 006a  ..Qd.|%..|$..|.j
+00000e00: 2317 00a1 027d 2774 0da0 5d7c 006a 3f7c  #....}'t..]|.j?|
+00000e10: 2614 00a1 017c 005f 7174 0da0 5d7c 006a  &....|._qt..]|.j
+00000e20: 3f7c 2714 00a1 017c 005f 7457 0064 0404  ?|'....|._tW.d..
+00000e30: 0004 0083 0301 006e 1231 0090 0973 5830  .......n.1...sX0
+00000e40: 0001 0001 0001 0059 0001 0074 0da0 4864  .......Y...t..Hd
+00000e50: 2fa1 018f c87d 1f7c 006a 1d90 0972 c47c  /....}.|.j...r.|
+00000e60: 006a 2674 0da0 5e74 0da0 6d7c 00a0 287c  .j&t..^t..m|..(|
+00000e70: 006a 69a1 017c 006a 3e18 00a1 01a1 0114  .ji..|.j>.......
+00000e80: 007c 005f 787c 006a 2674 0da0 5e74 0da0  .|._x|.j&t..^t..
+00000e90: 6d7c 00a0 287c 006a 6aa1 017c 006a 3e18  m|..(|.jj..|.j>.
+00000ea0: 00a1 01a1 0114 007c 005f 796e 627c 006a  .......|._ynb|.j
+00000eb0: 2990 0a72 0e7c 006a 2674 0da0 5e74 0da0  )..r.|.j&t..^t..
+00000ec0: 6d7c 006a 3a7c 006a 3e18 00a1 01a1 0114  m|.j:|.j>.......
+00000ed0: 007c 005f 787c 006a 2674 0da0 5e74 0da0  .|._x|.j&t..^t..
+00000ee0: 6d7c 006a 3b7c 006a 3e18 00a1 01a1 0114  m|.j;|.j>.......
+00000ef0: 007c 005f 796e 1874 0da0 7064 1ba1 017c  .|._yn.t..pd...|
+00000f00: 005f 7874 0da0 7064 1ba1 017c 005f 7957  ._xt..pd...|._yW
+00000f10: 0064 0404 0004 0083 0301 006e 1231 0090  .d.........n.1..
+00000f20: 0a73 3c30 0001 0001 0001 0059 0001 0074  .s<0.......Y...t
+00000f30: 0da0 4864 30a1 018f 727d 1f7c 006a 1690  ..Hd0...r}.|.j..
+00000f40: 0a72 767c 006a 747c 006a 6817 007c 006a  .rv|.jt|.jh..|.j
+00000f50: 6f17 007c 006a 7917 007c 005f 7a6e 147c  o..|.jy..|._zn.|
+00000f60: 006a 687c 006a 6f17 007c 006a 7917 007c  .jh|.jo..|.jy..|
+00000f70: 005f 7a7c 006a 717c 006a 6717 007c 006a  ._z|.jq|.jg..|.j
+00000f80: 6e17 0074 0da0 537c 006a 247c 006a 65a1  n..t..S|.j$|.je.
+00000f90: 0217 007c 006a 7817 007c 005f 7b57 0064  ...|.jx..|._{W.d
+00000fa0: 0404 0004 0083 0301 006e 1231 0090 0a73  .........n.1...s
+00000fb0: ca30 0001 0001 0001 0059 0001 0074 0da0  .0.......Y...t..
+00000fc0: 4864 31a1 018f c67d 1f74 0d6a 7c6a 7d7c  Hd1....}.t.j|j}|
+00000fd0: 0c7c 006a 407c 006a 2b64 0564 3264 338d  .|.j@|.j+d.d2d3.
+00000fe0: 057c 005f 7e74 0d6a 7ca0 7f7c 006a 7ea1  .|._~t.j|..|.j~.
+00000ff0: 017d 2874 8064 3464 3584 0074 0da0 81a1  .}(t.d4d5..t....
+00001000: 0044 0083 0183 0189 027c 286a 827c 006a  .D.......|(j.|.j
+00001010: 7a7c 006a 3b67 0164 368d 027c 005f 8374  z|.j;g.d6..|._.t
+00001020: 0d6a 4174 0d6a 3864 3764 1f8d 027c 005f  .jAt.j8d7d...|._
+00001030: 8464 3864 1384 0074 0da0 85a1 0044 0083  .d8d...t.....D..
+00001040: 0164 0619 007d 297c 006a 847c 2966 0267  .d...})|.j.|)f.g
+00001050: 017d 2a7c 286a 867c 2a7c 006a 4064 398d  .}*|(j.|*|.j@d9.
+00001060: 027c 005f 8774 0da0 81a1 007d 2b87 0266  .|._.t.....}+..f
+00001070: 0164 3a64 1384 087c 2b44 0083 017d 2c57  .d:d...|+D...},W
+00001080: 0064 0404 0004 0083 0301 006e 1231 0090  .d.........n.1..
+00001090: 0b73 ac30 0001 0001 0001 0059 0001 0067  .s.0.......Y...g
+000010a0: 007c 005f 887c 006a 88a0 897c 006a 39a0  .|._.|.j...|.j9.
+000010b0: 567c 006a 42a1 01a1 0101 007c 006a 88a0  V|.jB......|.j..
+000010c0: 897c 006a 3ca0 567c 006a 45a1 01a1 0101  .|.j<.V|.jE.....
+000010d0: 007c 006a 88a0 897c 006a 3fa0 567c 006a  .|.j...|.j?.V|.j
+000010e0: 46a1 01a1 0101 007c 006a 88a0 897c 006a  F......|.j...|.j
+000010f0: 3aa0 567c 006a 43a1 01a1 0101 007c 006a  :.V|.jC......|.j
+00001100: 88a0 897c 006a 3ba0 567c 006a 44a1 01a1  ...|.j;.V|.jD...
+00001110: 0101 007c 006a 88a0 897c 006a 3ea0 567c  ...|.j...|.j>.V|
+00001120: 006a 47a1 01a1 0101 0074 0d6a 8a7c 006a  .jG......t.j.|.j
+00001130: 4067 017c 006a 3b67 0117 007c 006a 3a67  @g.|.j;g...|.j:g
+00001140: 0117 007c 2c17 0064 368d 017c 005f 8b7c  ...|,..d6..|._.|
+00001150: 006a 3564 0475 0190 0c72 9874 0d6a 8ca0  .j5d.u...r.t.j..
+00001160: 8d7c 1474 0da0 8ea1 00a1 027c 005f 8f7c  .|.t.......|._.|
+00001170: 006a 8fa0 9074 0da0 8ea1 00a1 0101 006e  .j...t.........n
+00001180: 0664 047c 005f 8f64 0453 0029 3b61 a609  .d.|._.d.S.);a..
+00001190: 0000 0a20 2020 2020 2020 2049 6e69 7469  ...        Initi
+000011a0: 616c 697a 6520 7072 6f74 6f74 7970 6963  alize prototypic
+000011b0: 616c 2063 6f75 6e74 6572 6661 6374 7561  al counterfactua
+000011c0: 6c20 6d65 7468 6f64 2e0a 0a20 2020 2020  l method...     
+000011d0: 2020 2050 6172 616d 6574 6572 730a 2020     Parameters.  
+000011e0: 2020 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d        ----------
+000011f0: 0a20 2020 2020 2020 2070 7265 6469 6374  .        predict
+00001200: 0a20 2020 2020 2020 2020 2020 2060 7465  .            `te
+00001210: 6e73 6f72 666c 6f77 6020 6d6f 6465 6c20  nsorflow` model 
+00001220: 6f72 2061 6e79 206f 7468 6572 206d 6f64  or any other mod
+00001230: 656c 2773 2070 7265 6469 6374 696f 6e20  el's prediction 
+00001240: 6675 6e63 7469 6f6e 2072 6574 7572 6e69  function returni
+00001250: 6e67 2063 6c61 7373 2070 726f 6261 6269  ng class probabi
+00001260: 6c69 7469 6573 2e0a 2020 2020 2020 2020  lities..        
+00001270: 7368 6170 650a 2020 2020 2020 2020 2020  shape.          
+00001280: 2020 5368 6170 6520 6f66 2069 6e70 7574    Shape of input
+00001290: 2064 6174 6120 7374 6172 7469 6e67 2077   data starting w
+000012a0: 6974 6820 6261 7463 6820 7369 7a65 2e0a  ith batch size..
+000012b0: 2020 2020 2020 2020 6b61 7070 610a 2020          kappa.  
+000012c0: 2020 2020 2020 2020 2020 436f 6e66 6964            Confid
+000012d0: 656e 6365 2070 6172 616d 6574 6572 2066  ence parameter f
+000012e0: 6f72 2074 6865 2061 7474 6163 6b20 6c6f  or the attack lo
+000012f0: 7373 2074 6572 6d2e 0a20 2020 2020 2020  ss term..       
+00001300: 2062 6574 610a 2020 2020 2020 2020 2020   beta.          
+00001310: 2020 5265 6775 6c61 7269 7a61 7469 6f6e    Regularization
+00001320: 2063 6f6e 7374 616e 7420 666f 7220 4c31   constant for L1
+00001330: 206c 6f73 7320 7465 726d 2e0a 2020 2020   loss term..    
+00001340: 2020 2020 6665 6174 7572 655f 7261 6e67      feature_rang
+00001350: 650a 2020 2020 2020 2020 2020 2020 5475  e.            Tu
+00001360: 706c 6520 7769 7468 2060 6d69 6e60 2061  ple with `min` a
+00001370: 6e64 2060 6d61 7860 2072 616e 6765 7320  nd `max` ranges 
+00001380: 746f 2061 6c6c 6f77 2066 6f72 2070 6572  to allow for per
+00001390: 7475 7262 6564 2069 6e73 7461 6e63 6573  turbed instances
+000013a0: 2e20 604d 696e 6020 616e 6420 606d 6178  . `Min` and `max
+000013b0: 6020 7261 6e67 6573 2063 616e 2062 6520  ` ranges can be 
+000013c0: 6066 6c6f 6174 600a 2020 2020 2020 2020  `float`.        
+000013d0: 2020 2020 6f72 2060 6e75 6d70 7960 2061      or `numpy` a
+000013e0: 7272 6179 7320 7769 7468 2064 696d 656e  rrays with dimen
+000013f0: 7369 6f6e 2028 3178 206e 6220 6f66 2066  sion (1x nb of f
+00001400: 6561 7475 7265 7329 2066 6f72 2066 6561  eatures) for fea
+00001410: 7475 7265 2d77 6973 6520 7261 6e67 6573  ture-wise ranges
+00001420: 2e0a 2020 2020 2020 2020 6761 6d6d 610a  ..        gamma.
+00001430: 2020 2020 2020 2020 2020 2020 5265 6775              Regu
+00001440: 6c61 7269 7a61 7469 6f6e 2063 6f6e 7374  larization const
+00001450: 616e 7420 666f 7220 6f70 7469 6f6e 616c  ant for optional
+00001460: 2061 7574 6f2d 656e 636f 6465 7220 6c6f   auto-encoder lo
+00001470: 7373 2074 6572 6d2e 0a20 2020 2020 2020  ss term..       
+00001480: 2061 655f 6d6f 6465 6c0a 2020 2020 2020   ae_model.      
+00001490: 2020 2020 2020 4f70 7469 6f6e 616c 2061        Optional a
+000014a0: 7574 6f2d 656e 636f 6465 7220 6d6f 6465  uto-encoder mode
+000014b0: 6c20 7573 6564 2066 6f72 206c 6f73 7320  l used for loss 
+000014c0: 7265 6775 6c61 7269 7a61 7469 6f6e 2e0a  regularization..
+000014d0: 2020 2020 2020 2020 656e 635f 6d6f 6465          enc_mode
+000014e0: 6c0a 2020 2020 2020 2020 2020 2020 4f70  l.            Op
+000014f0: 7469 6f6e 616c 2065 6e63 6f64 6572 206d  tional encoder m
+00001500: 6f64 656c 2075 7365 6420 746f 2067 7569  odel used to gui
+00001510: 6465 2069 6e73 7461 6e63 6520 7065 7274  de instance pert
+00001520: 7572 6261 7469 6f6e 7320 746f 7761 7264  urbations toward
+00001530: 7320 6120 636c 6173 7320 7072 6f74 6f74  s a class protot
+00001540: 7970 652e 0a20 2020 2020 2020 2074 6865  ype..        the
+00001550: 7461 0a20 2020 2020 2020 2020 2020 2043  ta.            C
+00001560: 6f6e 7374 616e 7420 666f 7220 7468 6520  onstant for the 
+00001570: 7072 6f74 6f74 7970 6520 7365 6172 6368  prototype search
+00001580: 206c 6f73 7320 7465 726d 2e0a 2020 2020   loss term..    
+00001590: 2020 2020 7573 655f 6b64 7472 6565 0a20      use_kdtree. 
+000015a0: 2020 2020 2020 2020 2020 2057 6865 7468             Wheth
+000015b0: 6572 2074 6f20 7573 6520 6b2d 6420 7472  er to use k-d tr
+000015c0: 6565 7320 666f 7220 7468 6520 7072 6f74  ees for the prot
+000015d0: 6f74 7970 6520 6c6f 7373 2074 6572 6d20  otype loss term 
+000015e0: 6966 206e 6f20 656e 636f 6465 7220 6973  if no encoder is
+000015f0: 2061 7661 696c 6162 6c65 2e0a 2020 2020   available..    
+00001600: 2020 2020 6c65 6172 6e69 6e67 5f72 6174      learning_rat
+00001610: 655f 696e 6974 0a20 2020 2020 2020 2020  e_init.         
+00001620: 2020 2049 6e69 7469 616c 206c 6561 726e     Initial learn
+00001630: 696e 6720 7261 7465 206f 6620 6f70 7469  ing rate of opti
+00001640: 6d69 7a65 722e 0a20 2020 2020 2020 206d  mizer..        m
+00001650: 6178 5f69 7465 7261 7469 6f6e 730a 2020  ax_iterations.  
+00001660: 2020 2020 2020 2020 2020 4d61 7869 6d75            Maximu
+00001670: 6d20 6e75 6d62 6572 206f 6620 6974 6572  m number of iter
+00001680: 6174 696f 6e73 2066 6f72 2066 696e 6469  ations for findi
+00001690: 6e67 2061 2063 6f75 6e74 6572 6661 6374  ng a counterfact
+000016a0: 7561 6c2e 0a20 2020 2020 2020 2063 5f69  ual..        c_i
+000016b0: 6e69 740a 2020 2020 2020 2020 2020 2020  nit.            
+000016c0: 496e 6974 6961 6c20 7661 6c75 6520 746f  Initial value to
+000016d0: 2073 6361 6c65 2074 6865 2061 7474 6163   scale the attac
+000016e0: 6b20 6c6f 7373 2074 6572 6d2e 0a20 2020  k loss term..   
+000016f0: 2020 2020 2063 5f73 7465 7073 0a20 2020       c_steps.   
+00001700: 2020 2020 2020 2020 204e 756d 6265 7220           Number 
+00001710: 6f66 2069 7465 7261 7469 6f6e 7320 746f  of iterations to
+00001720: 2061 646a 7573 7420 7468 6520 636f 6e73   adjust the cons
+00001730: 7461 6e74 2073 6361 6c69 6e67 2074 6865  tant scaling the
+00001740: 2061 7474 6163 6b20 6c6f 7373 2074 6572   attack loss ter
+00001750: 6d2e 0a20 2020 2020 2020 2065 7073 0a20  m..        eps. 
+00001760: 2020 2020 2020 2020 2020 2049 6620 6e75             If nu
+00001770: 6d65 7269 6361 6c20 6772 6164 6965 6e74  merical gradient
+00001780: 7320 6172 6520 7573 6564 2074 6f20 636f  s are used to co
+00001790: 6d70 7574 6520 6064 4c2f 6478 203d 2028  mpute `dL/dx = (
+000017a0: 644c 2f64 7029 202a 2028 6470 2f64 7829  dL/dp) * (dp/dx)
+000017b0: 602c 2074 6865 6e20 6065 7073 5b30 5d60  `, then `eps[0]`
+000017c0: 2069 7320 7573 6564 2074 6f0a 2020 2020   is used to.    
+000017d0: 2020 2020 2020 2020 6361 6c63 756c 6174          calculat
+000017e0: 6520 6064 4c2f 6470 6020 616e 6420 6065  e `dL/dp` and `e
+000017f0: 7073 5b31 5d60 2069 7320 7573 6564 2066  ps[1]` is used f
+00001800: 6f72 2060 6470 2f64 7860 2e20 6065 7073  or `dp/dx`. `eps
+00001810: 5b30 5d60 2061 6e64 2060 6570 735b 315d  [0]` and `eps[1]
+00001820: 6020 6361 6e20 6265 2061 2063 6f6d 6269  ` can be a combi
+00001830: 6e61 7469 6f6e 206f 6620 6066 6c6f 6174  nation of `float
+00001840: 600a 2020 2020 2020 2020 2020 2020 7661  `.            va
+00001850: 6c75 6573 2061 6e64 2060 6e75 6d70 7960  lues and `numpy`
+00001860: 2061 7272 6179 732e 2046 6f72 2060 6570   arrays. For `ep
+00001870: 735b 305d 602c 2074 6865 2061 7272 6179  s[0]`, the array
+00001880: 2064 696d 656e 7369 6f6e 2073 686f 756c   dimension shoul
+00001890: 6420 6265 2028 3178 206e 6220 6f66 2070  d be (1x nb of p
+000018a0: 7265 6469 6374 696f 6e20 6361 7465 676f  rediction catego
+000018b0: 7269 6573 290a 2020 2020 2020 2020 2020  ries).          
+000018c0: 2020 616e 6420 666f 7220 6065 7073 5b31    and for `eps[1
+000018d0: 5d60 2069 7420 7368 6f75 6c64 2062 6520  ]` it should be 
+000018e0: 2831 7820 6e62 206f 6620 6665 6174 7572  (1x nb of featur
+000018f0: 6573 292e 0a20 2020 2020 2020 2063 6c69  es)..        cli
+00001900: 700a 2020 2020 2020 2020 2020 2020 5475  p.            Tu
+00001910: 706c 6520 7769 7468 206d 696e 2061 6e64  ple with min and
+00001920: 206d 6178 2063 6c69 7020 7261 6e67 6573   max clip ranges
+00001930: 2066 6f72 2062 6f74 6820 7468 6520 6e75   for both the nu
+00001940: 6d65 7269 6361 6c20 6772 6164 6965 6e74  merical gradient
+00001950: 7320 616e 6420 7468 6520 6772 6164 6965  s and the gradie
+00001960: 6e74 730a 2020 2020 2020 2020 2020 2020  nts.            
+00001970: 6f62 7461 696e 6564 2066 726f 6d20 7468  obtained from th
+00001980: 6520 6074 656e 736f 7266 6c6f 7760 2067  e `tensorflow` g
+00001990: 7261 7068 2e0a 2020 2020 2020 2020 7570  raph..        up
+000019a0: 6461 7465 5f6e 756d 5f67 7261 640a 2020  date_num_grad.  
+000019b0: 2020 2020 2020 2020 2020 4966 206e 756d            If num
+000019c0: 6572 6963 616c 2067 7261 6469 656e 7473  erical gradients
+000019d0: 2061 7265 2075 7365 642c 2074 6865 7920   are used, they 
+000019e0: 7769 6c6c 2062 6520 7570 6461 7465 6420  will be updated 
+000019f0: 6576 6572 7920 6075 7064 6174 655f 6e75  every `update_nu
+00001a00: 6d5f 6772 6164 6020 6974 6572 6174 696f  m_grad` iteratio
+00001a10: 6e73 2e0a 2020 2020 2020 2020 7472 7573  ns..        trus
+00001a20: 7473 636f 7265 0a20 2020 2020 2020 2020  tscore.         
+00001a30: 2020 2044 6972 6563 746f 7279 2077 6865     Directory whe
+00001a40: 7265 2074 7275 7374 7363 6f72 6520 6f62  re trustscore ob
+00001a50: 6a65 6374 2069 7320 746f 2062 6520 7573  ject is to be us
+00001a60: 6564 0a20 2020 2020 2020 2077 7269 7465  ed.        write
+00001a70: 5f64 6972 0a20 2020 2020 2020 2020 2020  _dir.           
+00001a80: 2044 6972 6563 746f 7279 2074 6f20 7772   Directory to wr
+00001a90: 6974 6520 6074 656e 736f 7262 6f61 7264  ite `tensorboard
+00001aa0: 6020 6669 6c65 7320 746f 2e0a 2020 2020  ` files to..    
+00001ab0: 2020 2020 7365 7373 0a20 2020 2020 2020      sess.       
+00001ac0: 2020 2020 204f 7074 696f 6e61 6c20 6074       Optional `t
+00001ad0: 656e 736f 7266 6c6f 7760 2073 6573 7369  ensorflow` sessi
+00001ae0: 6f6e 2074 6861 7420 7769 6c6c 2062 6520  on that will be 
+00001af0: 7573 6564 2069 6620 7061 7373 6564 2069  used if passed i
+00001b00: 6e73 7465 6164 206f 6620 6372 6561 7469  nstead of creati
+00001b10: 6e67 206f 7220 696e 6665 7272 696e 6720  ng or inferring 
+00001b20: 6f6e 6520 696e 7465 726e 616c 6c79 2e0a  one internally..
+00001b30: 2020 2020 2020 2020 2901 da04 6d65 7461          )...meta
+00001b40: 7207 0000 0072 1a00 0000 4e72 0100 0000  r....r....Nr....
+00001b50: e9ff ffff ff29 07da 0473 656c 6672 1b00  .....)...selfr..
+00001b60: 0000 721c 0000 0072 2200 0000 7223 0000  ..r....r"...r#..
+00001b70: 0072 2f00 0000 da09 5f5f 636c 6173 735f  .r/.....__class_
+00001b80: 5fda 0670 6172 616d 7329 03da 0869 735f  _..params)...is_
+00001b90: 6d6f 6465 6cda 0569 735f 6165 da06 6973  model..is_ae..is
+00001ba0: 5f65 6e63 5446 2901 da04 7369 7a65 7a15  _encTF)...sizez.
+00001bb0: 426c 6163 6b20 626f 7820 6d6f 6465 6c20  Black box model 
+00001bc0: 7769 7468 207a 0820 636c 6173 7365 737a  with z. classesz
+00001bd0: 5542 6f74 6820 616e 2065 6e63 6f64 6572  UBoth an encoder
+00001be0: 2061 6e64 206b 2d64 2074 7265 6573 2065   and k-d trees e
+00001bf0: 6e61 626c 6564 2e20 5573 696e 6720 7468  nabled. Using th
+00001c00: 6520 656e 636f 6465 7220 666f 7220 7468  e encoder for th
+00001c10: 6520 7072 6f74 6f74 7970 6520 6c6f 7373  e prototype loss
+00001c20: 2074 6572 6d2e 2901 da0d 656e 635f 6f72   term.)...enc_or
+00001c30: 5f6b 6474 7265 6529 01da 0669 735f 6361  _kdtree)...is_ca
+00001c40: 7463 0100 0000 0000 0000 0000 0000 0200  tc..............
+00001c50: 0000 0700 0000 1300 0000 734e 0000 0067  ..........sN...g
+00001c60: 007c 005d 467d 0174 0088 007c 0119 0074  .|.]F}.t...|...t
+00001c70: 0183 0272 3c74 02a0 0388 0164 0064 0185  ...r<t.....d.d..
+00001c80: 0219 00a1 0188 007c 0119 0014 0064 0164  .......|.....d.d
+00001c90: 0164 0185 0266 0219 006e 0c74 02a0 0488  .d...f...n.t....
+00001ca0: 007c 0119 00a1 0191 0271 0453 0029 0272  .|.......q.S.).r
+00001cb0: 1a00 0000 4e29 05da 0a69 7369 6e73 7461  ....N)...isinsta
+00001cc0: 6e63 65da 0566 6c6f 6174 da02 6e70 da04  nce..float..np..
+00001cd0: 6f6e 6573 da05 6172 7261 7929 02da 022e  ones..array)....
+00001ce0: 30da 015f 2902 7220 0000 0072 1d00 0000  0.._).r ...r....
+00001cf0: a900 fa50 2f63 656e 7472 616c 2f68 6f6d  ...P/central/hom
+00001d00: 652f 7a77 616e 6732 2f6d 6f72 7068 6575  e/zwang2/morpheu
+00001d10: 732d 7370 6174 6961 6c2f 6d6f 7270 6865  s-spatial/morphe
+00001d20: 7573 2f73 7263 2f6d 6f72 7068 6575 732f  us/src/morpheus/
+00001d30: 636f 756e 7465 7266 6163 7475 616c 2f63  counterfactual/c
+00001d40: 662e 7079 da0a 3c6c 6973 7463 6f6d 703e  f.py..<listcomp>
+00001d50: bd00 0000 7308 0000 0006 0602 fd0c ff28  ....s..........(
+00001d60: 027a 2b43 6f75 6e74 6572 6661 6374 7561  .z+Counterfactua
+00001d70: 6c2e 5f5f 696e 6974 5f5f 2e3c 6c6f 6361  l.__init__.<loca
+00001d80: 6c73 3e2e 3c6c 6973 7463 6f6d 703e da04  ls>.<listcomp>..
+00001d90: 6f72 6967 2902 da05 6474 7970 65da 046e  orig)...dtype..n
+00001da0: 616d 65da 0361 6476 da05 6164 765f 73da  ame..adv..adv_s.
+00001db0: 0674 6172 6765 74da 0c74 6172 6765 745f  .target..target_
+00001dc0: 7072 6f74 6fda 0563 6f6e 7374 720f 0000  proto..constr...
+00001dd0: 00da 0b67 6c6f 6261 6c5f 7374 6570 2902  ...global_step).
+00001de0: 5a09 7472 6169 6e61 626c 6572 4900 0000  Z.trainablerI...
+00001df0: da0b 6173 7369 676e 5f6f 7269 67a9 0172  ..assign_orig..r
+00001e00: 4900 0000 da0a 6173 7369 676e 5f61 6476  I.....assign_adv
+00001e10: da0c 6173 7369 676e 5f61 6476 5f73 da0d  ..assign_adv_s..
+00001e20: 6173 7369 676e 5f74 6172 6765 74da 0c61  assign_target..a
+00001e30: 7373 6967 6e5f 636f 6e73 74da 1361 7373  ssign_const..ass
+00001e40: 6967 6e5f 7461 7267 6574 5f70 726f 746f  ign_target_proto
+00001e50: 5a16 7368 7269 6e6b 6167 655f 7468 7265  Z.shrinkage_thre
+00001e60: 7368 6f6c 6469 6e67 5a0e 7065 7274 7572  sholdingZ.pertur
+00001e70: 6261 7469 6f6e 5f79 e903 0000 005a 0a75  bation_y.....Z.u
+00001e80: 7064 6174 655f 6164 765a 0c75 7064 6174  pdate_advZ.updat
+00001e90: 655f 6465 6c74 61da 0a6c 6f73 735f 6c31  e_delta..loss_l1
+00001ea0: 5f6c 32a9 01da 0461 7869 73da 076c 6f73  _l2....axis..los
+00001eb0: 735f 6165 da0b 6c6f 7373 5f61 7474 6163  s_ae..loss_attac
+00001ec0: 6be9 1027 0000 5a0e 6c6f 7373 5f70 726f  k..'..Z.loss_pro
+00001ed0: 746f 7479 7065 5a0d 6c6f 7373 5f63 6f6d  totypeZ.loss_com
+00001ee0: 6269 6e65 64da 0874 7261 696e 696e 6767  bined..trainingg
+00001ef0: 0000 0000 0000 e03f 2901 da05 706f 7765  .......?)...powe
+00001f00: 7263 0100 0000 0000 0000 0000 0000 0200  rc..............
+00001f10: 0000 0200 0000 7300 0000 7314 0000 007c  ......s...s....|
+00001f20: 005d 0c7d 017c 016a 0056 0001 0071 0264  .].}.|.j.V...q.d
+00001f30: 0053 0029 014e 7251 0000 00a9 0272 4200  .S.).NrQ.....rB.
+00001f40: 0000 da01 7872 4400 0000 7244 0000 0072  ....xrD...rD...r
+00001f50: 4500 0000 da09 3c67 656e 6578 7072 3ea9  E.....<genexpr>.
+00001f60: 0100 00f3 0000 0000 7a2a 436f 756e 7465  ........z*Counte
+00001f70: 7266 6163 7475 616c 2e5f 5f69 6e69 745f  rfactual.__init_
+00001f80: 5f2e 3c6c 6f63 616c 733e 2e3c 6765 6e65  _.<locals>.<gene
+00001f90: 7870 723e 2901 da08 7661 725f 6c69 7374  xpr>)...var_list
+00001fa0: 5a0a 6772 6164 5f61 6476 5f73 6301 0000  Z.grad_adv_sc...
+00001fb0: 0000 0000 0000 0000 0002 0000 0005 0000  ................
+00001fc0: 0053 0000 0073 1c00 0000 6700 7c00 5d14  .S...s....g.|.].
+00001fd0: 7d01 7c01 6a00 a001 6400 a101 7204 7c01  }.|.j...d...r.|.
+00001fe0: 9102 7104 5300 2901 724b 0000 0029 0272  ..q.S.).rK...).r
+00001ff0: 4900 0000 da0a 7374 6172 7473 7769 7468  I.....startswith
+00002000: 2902 7242 0000 005a 0474 7661 7272 4400  ).rB...Z.tvarrD.
+00002010: 0000 7244 0000 0072 4500 0000 7246 0000  ..rD...rE...rF..
+00002020: 00b0 0100 0073 0600 0000 0602 0201 0cfe  .....s..........
+00002030: 2901 724f 0000 0063 0100 0000 0000 0000  ).rO...c........
+00002040: 0000 0000 0200 0000 0400 0000 1300 0000  ................
+00002050: 731a 0000 0067 007c 005d 127d 017c 016a  s....g.|.].}.|.j
+00002060: 0088 0076 0172 047c 0191 0271 0453 0072  ...v.r.|...q.S.r
+00002070: 4400 0000 7251 0000 0072 6000 0000 2901  D...rQ...r`...).
+00002080: da0a 7374 6172 745f 7661 7273 7244 0000  ..start_varsrD..
+00002090: 0072 4500 0000 7246 0000 00bd 0100 0072  .rE...rF.......r
+000020a0: 6300 0000 2991 da05 7375 7065 72da 085f  c...)...super.._
+000020b0: 5f69 6e69 745f 5fda 0463 6f70 79da 0864  _init__..copy..d
+000020c0: 6565 7063 6f70 7972 0900 0000 da03 6c65  eepcopyr......le
+000020d0: 6eda 066c 6f63 616c 73da 0370 6f70 7232  n..locals..popr2
+000020e0: 0000 00da 0675 7064 6174 6572 1b00 0000  .....updater....
+000020f0: 722d 0000 0072 3d00 0000 da02 7466 da05  r-...r=.....tf..
+00002100: 6b65 7261 73da 054d 6f64 656c da06 636f  keras..Model..co
+00002110: 6d70 6174 da02 7631 da07 6261 636b 656e  mpat..v1..backen
+00002120: 645a 0b67 6574 5f73 6573 7369 6f6e da07  dZ.get_session..
+00002130: 5365 7373 696f 6e72 2f00 0000 da05 6d6f  Sessionr/.....mo
+00002140: 6465 6c72 3f00 0000 da05 7a65 726f 7372  delr?.....zerosr
+00002150: 1d00 0000 da07 636c 6173 7365 73da 0574  ......classes..t
+00002160: 6f72 6368 da05 7072 696e 7472 2300 0000  orch..printr#...
+00002170: 7222 0000 00da 066c 6f67 6765 72da 0777  r".....logger..w
+00002180: 6172 6e69 6e67 723b 0000 00da 0b70 6174  arningr;.....pat
+00002190: 6368 5f73 6861 7065 721e 0000 0072 1f00  ch_shaper....r..
+000021a0: 0000 7221 0000 0072 2400 0000 da02 6165  ..r!...r$.....ae
+000021b0: da03 656e 6372 2500 0000 da0a 6261 7463  ..encr%.....batc
+000021c0: 685f 7369 7a65 7227 0000 0072 2800 0000  h_sizer'...r(...
+000021d0: 7229 0000 00da 0574 7570 6c65 da05 7261  r).....tuple..ra
+000021e0: 6e67 6572 2000 0000 722c 0000 0072 2a00  nger ...r,...r*.
+000021f0: 0000 722b 0000 0072 1c00 0000 722e 0000  ..r+...r....r...
+00002200: 0072 3000 0000 da08 5661 7269 6162 6c65  .r0.....Variable
+00002210: da07 666c 6f61 7433 3272 4700 0000 724a  ..float32rG...rJ
+00002220: 0000 0072 4b00 0000 724c 0000 00da 0973  ...rK...rL.....s
+00002230: 6861 7065 5f65 6e63 724d 0000 0072 4e00  hape_encrM...rN.
+00002240: 0000 724f 0000 00da 0b70 6c61 6365 686f  ..rO.....placeho
+00002250: 6c64 6572 7250 0000 0072 5200 0000 7253  lderrP...rR...rS
+00002260: 0000 0072 5400 0000 7255 0000 0072 5600  ...rT...rU...rV.
+00002270: 0000 5a0a 6e61 6d65 5f73 636f 7065 da04  ..Z.name_scope..
+00002280: 6361 7374 da07 6772 6561 7465 72da 0873  cast..greater..s
+00002290: 7562 7472 6163 74da 0a6c 6573 735f 6571  ubtract..less_eq
+000022a0: 7561 6cda 0361 6273 da04 6c65 7373 da08  ual..abs..less..
+000022b0: 6e65 6761 7469 7665 da07 6d69 6e69 6d75  negative..minimu
+000022c0: 6dda 076d 6178 696d 756d da03 6164 64da  m..maximum..add.
+000022d0: 086d 756c 7469 706c 79da 0664 6976 6964  .multiply..divid
+000022e0: 65da 027a 74da 0661 7373 6967 6eda 0b61  e..zt..assign..a
+000022f0: 6476 5f75 7064 6174 6572 da0d 6164 765f  dv_updater..adv_
+00002300: 7570 6461 7465 725f 73da 0564 656c 7461  updater_s..delta
+00002310: da07 6465 6c74 615f 73da 046c 6973 74da  ..delta_s..list.
+00002320: 0661 7261 6e67 65da 0a72 6564 7563 655f  .arange..reduce_
+00002330: 7375 6dda 0673 7175 6172 65da 026c 325a  sum..square..l2Z
+00002340: 046c 325f 73da 026c 315a 046c 315f 73da  .l2_s..l1Z.l1_s.
+00002350: 056c 315f 6c32 5a07 6c31 5f6c 325f 73da  .l1_l2Z.l1_l2_s.
+00002360: 076c 6f73 735f 6c31 5a09 6c6f 7373 5f6c  .loss_l1Z.loss_l
+00002370: 315f 73da 076c 6f73 735f 6c32 5a09 6c6f  1_s..loss_l2Z.lo
+00002380: 7373 5f6c 325f 735a 0761 6476 5f63 6174  ss_l2_sZ.adv_cat
+00002390: 5a09 6164 765f 6361 745f 735a 0661 6476  Z.adv_cat_sZ.adv
+000023a0: 5f61 655a 0861 6476 5f61 655f 73da 046e  _aeZ.adv_ae_s..n
+000023b0: 6f72 6d72 5b00 0000 5a09 6c6f 7373 5f61  ormr[...Z.loss_a
+000023c0: 655f 73da 0863 6f6e 7374 616e 7472 5c00  e_s..constantr\.
+000023d0: 0000 da0a 7072 6564 5f70 726f 6261 5a0c  ....pred_probaZ.
+000023e0: 7072 6564 5f70 726f 6261 5f73 da0d 6c6f  pred_proba_s..lo
+000023f0: 7373 5f61 7474 6163 6b5f 73da 0c74 6172  ss_attack_s..tar
+00002400: 6765 745f 7072 6f62 615a 0a72 6564 7563  get_probaZ.reduc
+00002410: 655f 6d61 78da 136e 6f6e 7461 7267 6574  e_max..nontarget
+00002420: 5f70 726f 6261 5f6d 6178 da0a 6c6f 7373  _proba_max..loss
+00002430: 5f70 726f 746f 5a0c 6c6f 7373 5f70 726f  _protoZ.loss_pro
+00002440: 746f 5f73 da08 6c6f 7373 5f6f 7074 da0a  to_s..loss_opt..
+00002450: 6c6f 7373 5f74 6f74 616c da05 7472 6169  loss_total..trai
+00002460: 6e5a 1070 6f6c 796e 6f6d 6961 6c5f 6465  nZ.polynomial_de
+00002470: 6361 79da 0d6c 6561 726e 696e 675f 7261  cay..learning_ra
+00002480: 7465 5a18 4772 6164 6965 6e74 4465 7363  teZ.GradientDesc
+00002490: 656e 744f 7074 696d 697a 6572 da03 7365  entOptimizer..se
+000024a0: 745a 1067 6c6f 6261 6c5f 7661 7269 6162  tZ.global_variab
+000024b0: 6c65 735a 1163 6f6d 7075 7465 5f67 7261  lesZ.compute_gra
+000024c0: 6469 656e 7473 da0d 636f 6d70 7574 655f  dients..compute_
+000024d0: 6772 6164 73da 0767 7261 645f 7068 5a13  grads..grad_phZ.
+000024e0: 7472 6169 6e61 626c 655f 7661 7269 6162  trainable_variab
+000024f0: 6c65 735a 0f61 7070 6c79 5f67 7261 6469  lesZ.apply_gradi
+00002500: 656e 7473 da0b 6170 706c 795f 6772 6164  ents..apply_grad
+00002510: 73da 0573 6574 7570 da06 6170 7065 6e64  s..setup..append
+00002520: 5a15 7661 7269 6162 6c65 735f 696e 6974  Z.variables_init
+00002530: 6961 6c69 7a65 72da 0469 6e69 74da 0773  ializer..init..s
+00002540: 756d 6d61 7279 5a0a 4669 6c65 5772 6974  ummaryZ.FileWrit
+00002550: 6572 5a11 6765 745f 6465 6661 756c 745f  erZ.get_default_
+00002560: 6772 6170 68da 0677 7269 7465 72da 0961  graph..writer..a
+00002570: 6464 5f67 7261 7068 292d 7234 0000 0072  dd_graph)-r4...r
+00002580: 1b00 0000 721c 0000 0072 1d00 0000 721e  ....r....r....r.
+00002590: 0000 0072 1f00 0000 7220 0000 0072 2100  ...r....r ...r!.
+000025a0: 0000 7222 0000 0072 2300 0000 7224 0000  ..r"...r#...r$..
+000025b0: 0072 2500 0000 7226 0000 0072 2700 0000  .r%...r&...r'...
+000025c0: 7228 0000 0072 2900 0000 722a 0000 0072  r(...r)...r*...r
+000025d0: 2b00 0000 722c 0000 0072 2d00 0000 722e  +...r,...r-...r.
+000025e0: 0000 0072 2f00 0000 7230 0000 0072 7d00  ...r/...r0...r}.
+000025f0: 0000 7236 0000 00da 0672 656d 6f76 65da  ..r6.....remove.
+00002600: 036b 6579 7237 0000 005a 0a6d 6f64 656c  .keyr7...Z.model
+00002610: 5f73 6573 7372 3800 0000 7239 0000 00da  _sessr8...r9....
+00002620: 0573 636f 7065 da04 636f 6e64 da05 7570  .scope..cond..up
+00002630: 7065 72da 056c 6f77 6572 5a06 6178 5f73  per..lowerZ.ax_s
+00002640: 756d 5a0e 7461 7267 6574 5f70 726f 6261  umZ.target_proba
+00002650: 5f73 5a15 6e6f 6e74 6172 6765 745f 7072  _sZ.nontarget_pr
+00002660: 6f62 615f 6d61 785f 7372 5c00 0000 72a5  oba_max_sr\...r.
+00002670: 0000 00da 096f 7074 696d 697a 6572 da03  .....optimizer..
+00002680: 7661 725a 0c67 7261 645f 616e 645f 7661  varZ.grad_and_va
+00002690: 725a 0865 6e64 5f76 6172 735a 086e 6577  rZ.end_varsZ.new
+000026a0: 5f76 6172 73a9 0172 3500 0000 2903 7220  _vars..r5...).r 
+000026b0: 0000 0072 1d00 0000 7266 0000 0072 4500  ...r....rf...rE.
+000026c0: 0000 7268 0000 0018 0000 0073 1a02 0000  ..rh.......s....
+000026d0: 004f 1403 0c01 0201 06ff 0403 1202 0401  .O..............
+000026e0: 0601 0809 0801 0c01 1002 0601 0603 0e01  ................
+000026f0: 1001 0e01 0e01 1603 0c01 0802 0602 0601  ................
+00002700: 0601 1c02 0601 1a01 1202 0601 0802 0602  ................
+00002710: 0601 0802 0602 0e01 0401 02ff 0404 0e01  ................
+00002720: 0802 0601 1402 1202 0601 0601 0601 0601  ................
+00002730: 0601 0601 0601 0602 0601 0a01 0601 0601  ................
+00002740: 0601 0201 0c06 06fa 04ff 060a 0601 0601  ................
+00002750: 0601 0601 0601 0603 1a01 1a01 1a01 0401  ................
+00002760: 16ff 0806 0801 1a03 0803 0401 10ff 0805  ................
+00002770: 0401 10ff 0803 1203 1401 1401 1401 0401  ................
+00002780: 10ff 0803 0401 0cff 0803 0401 0aff 0806  ................
+00002790: 0e02 0401 1801 04fe 0204 0401 0401 18ff  ................
+000027a0: 0203 04fc 0206 0401 1e01 04fe 02f5 0410  ................
+000027b0: 0401 0e01 10fe 0404 0401 1eff 0404 0e01  ................
+000027c0: 10ff 0202 0efe 02ff 2407 0c01 0401 16ff  ........$.......
+000027d0: 0603 0801 0eff 0804 0401 14ff 0603 0401  ................
+000027e0: 14ff 2605 0c01 1201 3203 0c01 0e01 2e03  ..&.....2.......
+000027f0: 1401 0c01 1801 1801 1801 1801 1801 1803  ................
+00002800: 0e01 0e01 0e01 2e02 0801 0802 0c02 0802  ................
+00002810: 0e01 0e02 2001 0801 10ff 0a04 0c01 2c02  .... .........,.
+00002820: 0e01 0801 1202 08ff 0401 08ff 0404 0e01  ................
+00002830: 0e02 0c01 0e03 0e01 0e03 1601 1403 0401  ................
+00002840: 1aff 0603 0401 1aff 0405 0401 14ff 0403  ................
+00002850: 0401 10ff 0405 1201 3202 0c02 0801 0801  ........2.......
+00002860: 16ff 0803 0801 16ff 0a03 0801 0801 10ff  ................
+00002870: 0803 0801 10ff 0a04 0c01 2c02 0c02 0802  ..........,.....
+00002880: 0401 04ff 0202 04fe 0203 04fd 02ff 0607  ................
+00002890: 1404 0401 04ff 0202 04fe 0203 0efd 0204  ................
+000028a0: 04fc 02ff 2408 0c01 0601 0eff 0803 0e01  ....$...........
+000028b0: 1603 0401 0aff 0803 1201 0602 06fe 0405  ................
+000028c0: 02fb 0408 0c01 0401 06ff 0803 0801 3203  ..............2.
+000028d0: 0601 1601 1601 1601 1601 1601 1605 0401  ................
+000028e0: 1aff 0804 0c01 1401 1202 7a17 436f 756e  ..........z.Coun
+000028f0: 7465 7266 6163 7475 616c 2e5f 5f69 6e69  terfactual.__ini
+00002900: 745f 5f29 04da 0a74 7261 696e 5f64 6174  t__)...train_dat
+00002910: 61da 0570 7265 6473 da11 7472 7573 7473  a..preds..trusts
+00002920: 636f 7265 5f6b 7761 7267 7372 3100 0000  core_kwargsr1...
+00002930: 6304 0000 0000 0000 0000 0000 000b 0000  c...............
+00002940: 0006 0000 0043 0000 0073 c800 0000 7400  .....C...s....t.
+00002950: 8300 7d04 6401 6402 6702 7d05 7c05 4400  ..}.d.d.g.}.|.D.
+00002960: 5d0e 7d06 7c04 a001 7c06 a101 0100 7112  ].}.|...|.....q.
+00002970: 7c00 6a02 6403 1900 a003 7c04 a101 0100  |.j.d.....|.....
+00002980: 7c00 6a04 72a4 7c00 6a05 a006 7c01 a101  |.j.r.|.j...|...
+00002990: 7d07 6900 7c00 5f07 6900 7c00 5f08 7409  }.i.|._.i.|._.t.
+000029a0: 7c00 6a0a 8301 4400 5d46 7d08 740b a00c  |.j...D.]F}.t...
+000029b0: 7c02 7c08 6b02 a101 6404 1900 7d09 740b  |.|.k...d...}.t.
+000029c0: 6a0d 740b 6a0e 7c07 7c09 1900 6404 6405  j.t.j.|.|...d.d.
+000029d0: 8d02 6404 6405 8d02 7c00 6a07 7c08 3c00  ..d.d...|.j.|.<.
+000029e0: 7c07 7c09 1900 7c00 6a08 7c08 3c00 715a  |.|...|.j.|.<.qZ
+000029f0: 6e20 7c00 6a0f 72c4 7410 7c00 6a11 8301  n |.j.r.t.|.j...
+00002a00: 7d0a 7c0a 6a12 7c00 5f12 7c0a 6a13 7c00  }.|.j.|._.|.j.|.
+00002a10: 5f14 7c00 5300 2906 6188 0100 000a 2020  _.|.S.).a.....  
+00002a20: 2020 2020 2020 4765 7420 7072 6f74 6f74        Get protot
+00002a30: 7970 6573 2066 6f72 2065 6163 6820 636c  ypes for each cl
+00002a40: 6173 7320 7573 696e 6720 7468 6520 656e  ass using the en
+00002a50: 636f 6465 7220 6f72 206b 2d64 2074 7265  coder or k-d tre
+00002a60: 6573 2e0a 2020 2020 2020 2020 5468 6520  es..        The 
+00002a70: 7072 6f74 6f74 7970 6573 2061 7265 2075  prototypes are u
+00002a80: 7365 6420 666f 7220 7468 6520 656e 636f  sed for the enco
+00002a90: 6465 7220 6c6f 7373 2074 6572 6d20 6f72  der loss term or
+00002aa0: 2074 6f20 6361 6c63 756c 6174 6520 7468   to calculate th
+00002ab0: 6520 6f70 7469 6f6e 616c 2074 7275 7374  e optional trust
+00002ac0: 2073 636f 7265 732e 0a0a 2020 2020 2020   scores...      
+00002ad0: 2020 5061 7261 6d65 7465 7273 0a20 2020    Parameters.   
+00002ae0: 2020 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a       ----------.
+00002af0: 2020 2020 2020 2020 7472 6169 6e5f 6461          train_da
+00002b00: 7461 0a20 2020 2020 2020 2020 2020 2052  ta.            R
+00002b10: 6570 7265 7365 6e74 6174 6976 6520 7361  epresentative sa
+00002b20: 6d70 6c65 2066 726f 6d20 7468 6520 7472  mple from the tr
+00002b30: 6169 6e69 6e67 2064 6174 612e 0a20 2020  aining data..   
+00002b40: 2020 2020 2074 7275 7374 7363 6f72 655f       trustscore_
+00002b50: 6b77 6172 6773 0a20 2020 2020 2020 2020  kwargs.         
+00002b60: 2020 204f 7074 696f 6e61 6c20 6172 6775     Optional argu
+00002b70: 6d65 6e74 7320 746f 2069 6e69 7469 616c  ments to initial
+00002b80: 697a 6520 7468 6520 7472 7573 7420 7363  ize the trust sc
+00002b90: 6f72 6573 206d 6574 686f 642e 0a20 2020  ores method..   
+00002ba0: 2020 2020 2072 3400 0000 72c0 0000 0072       r4...r....r
+00002bb0: 3600 0000 7201 0000 0072 5900 0000 2915  6...r....rY...).
+00002bc0: 726c 0000 0072 6d00 0000 7232 0000 0072  rl...rm...r2...r
+00002bd0: 6e00 0000 7223 0000 0072 7f00 0000 721b  n...r#...r....r.
+00002be0: 0000 00da 0b63 6c61 7373 5f70 726f 746f  .....class_proto
+00002bf0: da09 636c 6173 735f 656e 6372 8200 0000  ..class_encr....
+00002c00: 7278 0000 0072 3f00 0000 da05 7768 6572  rx...r?.....wher
+00002c10: 65da 0b65 7870 616e 645f 6469 6d73 da04  e..expand_dims..
+00002c20: 6d65 616e 7225 0000 00da 0b6c 6f61 645f  meanr%.....load_
+00002c30: 6f62 6a65 6374 722d 0000 00da 076b 6474  objectr-.....kdt
+00002c40: 7265 6573 5a08 585f 6b64 7472 6565 da0a  reesZ.X_kdtree..
+00002c50: 585f 6279 5f63 6c61 7373 290b 7234 0000  X_by_class).r4..
+00002c60: 0072 c000 0000 72c1 0000 0072 c200 0000  .r....r....r....
+00002c70: 7236 0000 0072 b700 0000 72b8 0000 005a  r6...r....r....Z
+00002c80: 0865 6e63 5f64 6174 61da 0169 da03 6964  .enc_data..i..id
+00002c90: 78da 0274 7372 4400 0000 7244 0000 0072  x..tsrD...rD...r
+00002ca0: 4500 0000 da03 6669 74d5 0100 0073 2800  E.....fit....s(.
+00002cb0: 0000 0012 0601 0801 0801 0c02 1002 0601  ................
+00002cc0: 0c01 0601 0601 0e01 1201 0401 12ff 0c03  ................
+00002cd0: 1201 0601 0a01 0801 0801 7a12 436f 756e  ..........z.Coun
+00002ce0: 7465 7266 6163 7475 616c 2e66 6974 2903  terfactual.fit).
+00002cf0: 72a4 0000 00da 0159 7231 0000 0063 0300  r......Yr1...c..
+00002d00: 0000 0000 0000 0000 0000 0700 0000 0500  ................
+00002d10: 0000 4300 0000 735e 0000 0074 00a0 017c  ..C...s^...t...|
+00002d20: 017c 0214 00a1 017d 0374 00a0 0264 017c  .|.....}.t...d.|
+00002d30: 0218 007c 0114 0064 027c 0214 0018 00a1  ...|...d.|......
+00002d40: 017d 0474 00a0 0364 037c 040b 007c 0317  .}.t...d.|...|..
+00002d50: 007c 006a 0417 00a1 027d 0574 00a0 017c  .|.j.....}.t...|
+00002d60: 006a 056a 067c 006a 0764 048d 017c 0514  .j.j.|.j.d...|..
+00002d70: 00a1 017d 067c 0653 0029 0561 1701 0000  ...}.|.S.).a....
+00002d80: 0a20 2020 2020 2020 2043 6f6d 7075 7465  .        Compute
+00002d90: 2074 6865 2061 7474 6163 6b20 6c6f 7373   the attack loss
+00002da0: 2e0a 0a20 2020 2020 2020 2050 6172 616d  ...        Param
+00002db0: 6574 6572 730a 2020 2020 2020 2020 2d2d  eters.        --
+00002dc0: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020 2020  --------.       
+00002dd0: 2070 7265 645f 7072 6f62 610a 2020 2020   pred_proba.    
+00002de0: 2020 2020 2020 2020 5072 6564 6963 7469          Predicti
+00002df0: 6f6e 2070 726f 6261 6269 6c69 7469 6573  on probabilities
+00002e00: 206f 6620 616e 2069 6e73 7461 6e63 652e   of an instance.
+00002e10: 0a20 2020 2020 2020 2059 0a20 2020 2020  .        Y.     
+00002e20: 2020 2020 2020 204f 6e65 2d68 6f74 2072         One-hot r
+00002e30: 6570 7265 7365 6e74 6174 696f 6e20 6f66  epresentation of
+00002e40: 2069 6e73 7461 6e63 6520 6c61 6265 6c73   instance labels
+00002e50: 2e0a 0a20 2020 2020 2020 2052 6574 7572  ...        Retur
+00002e60: 6e73 0a20 2020 2020 2020 202d 2d2d 2d2d  ns.        -----
+00002e70: 2d2d 0a20 2020 2020 2020 204c 6f73 7320  --.        Loss 
+00002e80: 6f66 2074 6865 2061 7474 6163 6b2e 0a20  of the attack.. 
+00002e90: 2020 2020 2020 2072 1a00 0000 725d 0000         r....r]..
+00002ea0: 0072 0f00 0000 a901 da07 7365 7373 696f  .r........sessio
+00002eb0: 6e29 0872 3f00 0000 da03 7375 6dda 036d  n).r?.....sum..m
+00002ec0: 6178 728f 0000 0072 1e00 0000 724e 0000  axr....r....rN..
+00002ed0: 00da 0465 7661 6c72 2f00 0000 2907 7234  ...evalr/...).r4
+00002ee0: 0000 0072 a400 0000 72cf 0000 0072 a600  ...r....r....r..
+00002ef0: 0000 72a7 0000 00da 046c 6f73 7372 5c00  ..r......lossr\.
+00002f00: 0000 7244 0000 0072 4400 0000 7245 0000  ..rD...rD...rE..
+00002f10: 00da 076c 6f73 735f 666e fe01 0000 730a  ...loss_fn....s.
+00002f20: 0000 0000 100e 021a 0218 021a 017a 1643  .............z.C
+00002f30: 6f75 6e74 6572 6661 6374 7561 6c2e 6c6f  ounterfactual.lo
+00002f40: 7373 5f66 6e29 04da 0158 72cf 0000 00da  ss_fn)...Xr.....
+00002f50: 0b67 7261 6473 5f73 6861 7065 7231 0000  .grads_shaper1..
+00002f60: 0063 0400 0000 0000 0000 0000 0000 1500  .c..............
+00002f70: 0000 0600 0000 0300 0000 73e8 0100 0074  ..........s....t
+00002f80: 00a0 017c 01a1 017d 047c 00a0 027c 04a1  ...|...}.|...|..
+00002f90: 01a0 03a1 00a0 04a1 007d 0574 057c 057c  .........}.t.|.|
+00002fa0: 006a 0664 0119 0064 0264 038d 035c 027d  .j.d...d.d...\.}
+00002fb0: 067d 0787 0066 0164 0464 0584 087d 0887  .}...f.d.d...}..
+00002fc0: 0066 0164 0664 0784 087d 0974 07a0 087c  .f.d.d...}.t...|
+00002fd0: 087c 0583 017c 097c 0583 0118 007c 006a  .|...|.|.....|.j
+00002fe0: 090b 006b 01a1 0164 0119 007d 0a74 0a7c  ...k...d...}.t.|
+00002ff0: 0a83 017c 016a 0b64 0119 006b 0272 9c74  ...|.j.d...k.r.t
+00003000: 07a0 0c64 0867 017c 016a 0b64 0864 0985  ...d.g.|.j.d.d..
+00003010: 0219 00a2 0152 00a1 0153 007c 087c 0683  .....R...S.|.|..
+00003020: 017c 087c 0783 0118 007d 0b7c 097c 0683  .|.|.....}.|.|..
+00003030: 017c 097c 0783 0118 007d 0c7c 0b7c 0c18  .|.|.....}.|.|..
+00003040: 007d 0d74 07a0 0d7c 0d7c 016a 0b64 0119  .}.t...|.|.j.d..
+00003050: 0064 0a66 02a1 0264 0b7c 006a 0664 0119  .d.f...d.|.j.d..
+00003060: 0014 001b 007d 0d74 057c 017c 006a 0664  .....}.t.|.|.j.d
+00003070: 0819 0064 0c64 038d 035c 027d 0e7d 0f74  ...d.d...\.}.}.t
+00003080: 076a 0e7c 0e7c 0f67 0264 0164 0d8d 027d  .j.|.|.g.d.d...}
+00003090: 107c 00a0 0274 00a0 017c 10a1 01a1 01a0  .|...t...|......
+000030a0: 03a1 00a0 04a1 007d 117c 0e6a 0b64 0119  .......}.|.j.d..
+000030b0: 007d 127c 1164 097c 1285 0219 007c 117c  .}.|.d.|.....|.|
+000030c0: 1264 0985 0219 0018 007d 1374 076a 0d74  .d.......}.t.j.t
+000030d0: 07a0 0d7c 137c 016a 0b64 0119 0064 0a66  ...|.|.j.d...d.f
+000030e0: 02a1 027c 016a 0b64 0119 007c 056a 0b64  ...|.j.d...|.j.d
+000030f0: 0819 0064 0a66 0364 0e64 0f8d 0364 0b7c  ...d.f.d.d...d.|
+00003100: 006a 0664 0819 0014 001b 007d 1374 07a0  .j.d.......}.t..
+00003110: 0f64 107c 0d7c 13a1 037d 1474 0a7c 0a83  .d.|.|...}.t.|..
+00003120: 0164 016b 0490 0172 c274 07a0 0c7c 146a  .d.k...r.t...|.j
+00003130: 0b64 0864 0985 0219 00a1 017c 147c 0a3c  .d.d.......|.|.<
+00003140: 0074 076a 107c 1464 0164 0d8d 027d 1474  .t.j.|.d.d...}.t
+00003150: 07a0 0d7c 147c 006a 1166 017c 0317 00a1  ...|.|.j.f.|....
+00003160: 027d 147c 1453 0029 1161 b801 0000 0a20  .}.|.S.).a..... 
+00003170: 2020 2020 2020 2043 6f6d 7075 7465 206e         Compute n
+00003180: 756d 6572 6963 616c 2067 7261 6469 656e  umerical gradien
+00003190: 7473 206f 6620 7468 6520 6174 7461 636b  ts of the attack
+000031a0: 206c 6f73 7320 7465 726d 3a0a 2020 2020   loss term:.    
+000031b0: 2020 2020 6064 4c2f 6478 203d 2028 644c      `dL/dx = (dL
+000031c0: 2f64 5029 2a28 6450 2f64 7829 6020 7769  /dP)*(dP/dx)` wi
+000031d0: 7468 2060 4c20 3d20 6c6f 7373 5f61 7474  th `L = loss_att
+000031e0: 6163 6b5f 733b 2050 203d 2070 7265 6469  ack_s; P = predi
+000031f0: 6374 3b20 7820 3d20 6164 765f 7360 2e0a  ct; x = adv_s`..
+00003200: 0a20 2020 2020 2020 2050 6172 616d 6574  .        Paramet
+00003210: 6572 730a 2020 2020 2020 2020 2d2d 2d2d  ers.        ----
+00003220: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 2058  ------.        X
+00003230: 0a20 2020 2020 2020 2020 2020 2049 6e73  .            Ins
+00003240: 7461 6e63 6520 6172 6f75 6e64 2077 6869  tance around whi
+00003250: 6368 2067 7261 6469 656e 7420 6973 2065  ch gradient is e
+00003260: 7661 6c75 6174 6564 2e0a 2020 2020 2020  valuated..      
+00003270: 2020 590a 2020 2020 2020 2020 2020 2020    Y.            
+00003280: 4f6e 652d 686f 7420 7265 7072 6573 656e  One-hot represen
+00003290: 7461 7469 6f6e 206f 6620 696e 7374 616e  tation of instan
+000032a0: 6365 206c 6162 656c 732e 0a20 2020 2020  ce labels..     
+000032b0: 2020 2067 7261 6473 5f73 6861 7065 0a20     grads_shape. 
+000032c0: 2020 2020 2020 2020 2020 2053 6861 7065             Shape
+000032d0: 206f 6620 6772 6164 6965 6e74 732e 0a0a   of gradients...
+000032e0: 2020 2020 2020 2020 5265 7475 726e 730a          Returns.
+000032f0: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d0a          -------.
+00003300: 2020 2020 2020 2020 4172 7261 7920 7769          Array wi
+00003310: 7468 2067 7261 6469 656e 7473 2e0a 2020  th gradients..  
+00003320: 2020 2020 2020 7201 0000 0054 2901 da05        r....T)...
+00003330: 7072 6f62 6163 0100 0000 0000 0000 0000  probac..........
+00003340: 0000 0100 0000 0400 0000 1300 0000 7312  ..............s.
+00003350: 0000 0074 006a 0188 007c 0014 0064 0164  ...t.j...|...d.d
+00003360: 028d 0253 00a9 034e 721a 0000 0072 5900  ...S...Nr....rY.
+00003370: 0000 2902 723f 0000 0072 d200 0000 a901  ..).r?...r......
+00003380: 5a0a 7072 6564 735f 7065 7274 a901 72cf  Z.preds_pert..r.
+00003390: 0000 0072 4400 0000 7245 0000 00da 0166  ...rD...rE.....f
+000033a0: 3302 0000 7302 0000 0000 017a 2743 6f75  3...s......z'Cou
+000033b0: 6e74 6572 6661 6374 7561 6c2e 6765 745f  nterfactual.get_
+000033c0: 6772 6164 6965 6e74 732e 3c6c 6f63 616c  gradients.<local
+000033d0: 733e 2e66 6301 0000 0000 0000 0000 0000  s>.fc...........
+000033e0: 0001 0000 0004 0000 0013 0000 0073 1600  .............s..
+000033f0: 0000 7400 6a01 6401 8800 1800 7c00 1400  ..t.j.d.....|...
+00003400: 6401 6402 8d02 5300 72da 0000 0029 0272  d.d...S.r....).r
+00003410: 3f00 0000 72d3 0000 0072 db00 0000 72dc  ?...r....r....r.
+00003420: 0000 0072 4400 0000 7245 0000 00da 0167  ...rD...rE.....g
+00003430: 3602 0000 7302 0000 0000 017a 2743 6f75  6...s......z'Cou
+00003440: 6e74 6572 6661 6374 7561 6c2e 6765 745f  nterfactual.get_
+00003450: 6772 6164 6965 6e74 732e 3c6c 6f63 616c  gradients.<local
+00003460: 733e 2e67 721a 0000 004e 7233 0000 0072  s>.gr....Nr3...r
+00003470: 0700 0000 4672 5900 0000 da01 4629 01da  ....FrY.....F)..
+00003480: 056f 7264 6572 7a0a 696a 2c69 6a6b 2d3e  .orderz.ij,ijk->
+00003490: 696b 2912 7279 0000 00da 0674 656e 736f  ik).ry.....tenso
+000034a0: 7272 1b00 0000 da06 6465 7461 6368 da05  rr......detach..
+000034b0: 6e75 6d70 7972 0d00 0000 722a 0000 0072  numpyr....r*...r
+000034c0: 3f00 0000 72c5 0000 0072 1e00 0000 726b  ?...r....r....rk
+000034d0: 0000 0072 1d00 0000 7277 0000 00da 0772  ...r....rw.....r
+000034e0: 6573 6861 7065 da0b 636f 6e63 6174 656e  eshape..concaten
+000034f0: 6174 65da 0665 696e 7375 6d72 c700 0000  ate..einsumr....
+00003500: 7280 0000 0029 1572 3400 0000 72d7 0000  r....).r4...r...
+00003510: 0072 cf00 0000 72d8 0000 005a 0658 5f70  .r....r....Z.X_p
+00003520: 7265 6472 c100 0000 5a0e 7072 6564 735f  redr....Z.preds_
+00003530: 7065 7274 5f70 6f73 5a0e 7072 6564 735f  pert_posZ.preds_
+00003540: 7065 7274 5f6e 6567 72dd 0000 0072 de00  pert_negr....r..
+00003550: 0000 5a0a 6964 785f 6e6f 6772 6164 5a05  ..Z.idx_nogradZ.
+00003560: 646c 5f64 665a 0564 6c5f 6467 5a05 646c  dl_dfZ.dl_dgZ.dl
+00003570: 5f64 705a 0a58 5f70 6572 745f 706f 735a  _dpZ.X_pert_posZ
+00003580: 0a58 5f70 6572 745f 6e65 675a 0658 5f70  .X_pert_negZ.X_p
+00003590: 6572 745a 0c70 7265 6473 5f63 6f6e 6361  ertZ.preds_conca
+000035a0: 745a 066e 5f70 6572 745a 0564 705f 6478  tZ.n_pertZ.dp_dx
+000035b0: da05 6772 6164 7372 4400 0000 72dc 0000  ..gradsrD...r...
+000035c0: 0072 4500 0000 da0d 6765 745f 6772 6164  .rE.....get_grad
+000035d0: 6965 6e74 7317 0200 0073 4400 0000 0014  ients....sD.....
+000035e0: 0a03 1201 0201 0cff 0a04 0c03 0c04 2201  ..............".
+000035f0: 1201 1c01 1001 1001 0801 2403 0201 0cff  ..........$.....
+00003600: 0a03 1201 1801 0a01 1801 0401 1401 1401  ................
+00003610: 02fd 0405 0cfb 0409 0e02 0e01 1801 0e01  ................
+00003620: 1401 7a1c 436f 756e 7465 7266 6163 7475  ..z.Counterfactu
+00003630: 616c 2e67 6574 5f67 7261 6469 656e 7473  al.get_gradients
+00003640: e7bb bdd7 d9df 7cdb 3d29 0572 d700 0000  ......|.=).r....
+00003650: da09 6164 765f 636c 6173 73da 0a6f 7269  ..adv_class..ori
+00003660: 675f 636c 6173 7372 2a00 0000 7231 0000  g_classr*...r1..
+00003670: 0063 0500 0000 0000 0000 0000 0000 0a00  .c..............
+00003680: 0000 0400 0000 4300 0000 7396 0000 007c  ......C...s....|
+00003690: 006a 0072 487c 006a 01a0 027c 01a1 017d  .j.rH|.j...|...}
+000036a0: 057c 006a 037c 0219 007d 067c 006a 037c  .|.j.|...}.|.j.|
+000036b0: 0319 007d 0774 046a 05a0 067c 057c 0618  ...}.t.j...|.|..
+000036c0: 00a1 017d 0874 046a 05a0 067c 057c 0718  ...}.t.j...|.|..
+000036d0: 00a1 017d 096e 427c 006a 0772 807c 006a  ...}.nB|.j.r.|.j
+000036e0: 087c 0219 006a 0974 0a64 0164 028d 0264  .|...j.t.d.d...d
+000036f0: 0319 007d 087c 006a 087c 0319 006a 0974  ...}.|.j.|...j.t
+00003700: 0a64 0164 028d 0264 0319 007d 096e 0a74  .d.d...d...}.n.t
+00003710: 0ba0 0c64 04a1 0101 007c 097c 087c 0417  ...d.....|.|.|..
+00003720: 001b 0053 0029 0561 f501 0000 0a20 2020  ...S.).a.....   
+00003730: 2020 2020 2050 6172 616d 6574 6572 730a       Parameters.
+00003740: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d2d          --------
+00003750: 2d2d 0a20 2020 2020 2020 2058 0a20 2020  --.        X.   
+00003760: 2020 2020 2020 2020 2050 6572 7475 7262           Perturb
+00003770: 6174 696f 6e2e 0a20 2020 2020 2020 2061  ation..        a
+00003780: 6476 5f63 6c61 7373 0a20 2020 2020 2020  dv_class.       
+00003790: 2020 2020 2050 7265 6469 6374 6564 2063       Predicted c
+000037a0: 6c61 7373 206f 6e20 7468 6520 7065 7274  lass on the pert
+000037b0: 7572 6265 6420 696e 7374 616e 6365 2e0a  urbed instance..
+000037c0: 2020 2020 2020 2020 6f72 6967 5f63 6c61          orig_cla
+000037d0: 7373 0a20 2020 2020 2020 2020 2020 2050  ss.            P
+000037e0: 7265 6469 6374 6564 2063 6c61 7373 206f  redicted class o
+000037f0: 6e20 7468 6520 6f72 6967 696e 616c 2069  n the original i
+00003800: 6e73 7461 6e63 652e 0a20 2020 2020 2020  nstance..       
+00003810: 2065 7073 0a20 2020 2020 2020 2020 2020   eps.           
+00003820: 2053 6d61 6c6c 206e 756d 6265 7220 746f   Small number to
+00003830: 2061 766f 6964 2064 6976 6964 696e 6720   avoid dividing 
+00003840: 6279 2030 2e0a 0a20 2020 2020 2020 2052  by 0...        R
+00003850: 6574 7572 6e73 0a20 2020 2020 2020 202d  eturns.        -
+00003860: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 2052  ------.        R
+00003870: 6174 696f 2062 6574 7765 656e 2074 6865  atio between the
+00003880: 2064 6973 7461 6e63 6520 746f 2074 6865   distance to the
+00003890: 2070 726f 746f 7479 7065 206f 6620 7468   prototype of th
+000038a0: 6520 7072 6564 6963 7465 6420 636c 6173  e predicted clas
+000038b0: 7320 666f 7220 7468 6520 6f72 6967 696e  s for the origin
+000038c0: 616c 2069 6e73 7461 6e63 6520 616e 6420  al instance and 
+000038d0: 2020 2020 2020 2020 7468 6520 7072 6f74          the prot
+000038e0: 6f74 7970 6520 6f66 2074 6865 2070 7265  otype of the pre
+000038f0: 6469 6374 6564 2063 6c61 7373 2066 6f72  dicted class for
+00003900: 2074 6865 2070 6572 7475 7262 6564 2069   the perturbed i
+00003910: 6e73 7461 6e63 652e 0a20 2020 2020 2020  nstance..       
+00003920: 2072 1a00 0000 a901 da01 6b72 0100 0000   r........kr....
+00003930: 7a4b 4e65 6564 2065 6974 6865 7220 616e  zKNeed either an
+00003940: 2065 6e63 6f64 6572 206f 7220 7468 6520   encoder or the 
+00003950: 6b2d 6420 7472 6565 7320 656e 6162 6c65  k-d trees enable
+00003960: 6420 746f 2063 6f6d 7075 7465 2064 6973  d to compute dis
+00003970: 7461 6e63 6520 7363 6f72 6573 2e29 0d72  tance scores.).r
+00003980: 2300 0000 727f 0000 0072 1b00 0000 72c3  #...r....r....r.
+00003990: 0000 0072 3f00 0000 da06 6c69 6e61 6c67  ...r?.....linalg
+000039a0: 72a2 0000 0072 2500 0000 72c9 0000 00da  r....r%...r.....
+000039b0: 0571 7565 7279 5a06 5870 6174 6368 727b  .queryZ.Xpatchr{
+000039c0: 0000 0072 7c00 0000 290a 7234 0000 0072  ...r|...).r4...r
+000039d0: d700 0000 72ea 0000 0072 eb00 0000 722a  ....r....r....r*
+000039e0: 0000 00da 0558 5f65 6e63 5a09 6164 765f  .....X_encZ.adv_
+000039f0: 7072 6f74 6f5a 0a6f 7269 675f 7072 6f74  protoZ.orig_prot
+00003a00: 6f5a 0864 6973 745f 6164 765a 0964 6973  oZ.dist_advZ.dis
+00003a10: 745f 6f72 6967 7244 0000 0072 4400 0000  t_origrD...rD...
+00003a20: 7245 0000 00da 0573 636f 7265 5b02 0000  rE.....score[...
+00003a30: 731a 0000 0000 1406 010c 010a 010a 0110  s...............
+00003a40: 0112 0106 0318 011a 0204 0102 ff04 037a  ...............z
+00003a50: 1443 6f75 6e74 6572 6661 6374 7561 6c2e  .Counterfactual.
+00003a60: 7363 6f72 6572 c700 0000 e964 0000 0029  scorer.....d...)
+00003a70: 0a72 d700 0000 72cf 0000 00da 0c74 6172  .r....r......tar
+00003a80: 6765 745f 636c 6173 7372 ed00 0000 da06  get_classr......
+00003a90: 6b5f 7479 7065 da09 7468 7265 7368 6f6c  k_type..threshol
+00003aa0: 6472 3000 0000 da0b 7072 696e 745f 6576  dr0.....print_ev
+00003ab0: 6572 79da 096c 6f67 5f65 7665 7279 7231  ery..log_everyr1
+00003ac0: 0000 0063 0a00 0000 0000 0000 0000 0000  ...c............
+00003ad0: 4400 0000 0d00 0000 0300 0000 7328 0a00  D...........s(..
+00003ae0: 0088 006a 007c 016a 0164 0119 006b 0273  ...j.|.j.d...k.s
+00003af0: 144a 0082 0174 0274 0374 0474 056a 0666  .J...t.t.t.t.j.f
+00003b00: 0319 0074 0474 0764 029c 0387 0066 0164  ...t.t.d.....f.d
+00003b10: 0364 0484 0c7d 0a7c 0364 0575 0072 8a74  .d...}.|.d.u.r.t
+00003b20: 0874 0988 006a 0a83 0183 017d 037c 03a0  .t...j.....}.|..
+00003b30: 0b74 056a 0c7c 0264 0664 078d 02a1 0101  .t.j.|.d.d......
+00003b40: 007c 0772 8a74 0d64 08a0 0e74 056a 0c7c  .|.r.t.d...t.j.|
+00003b50: 0264 0664 078d 02a1 0183 0101 0074 0d64  .d.d.........t.d
+00003b60: 09a0 0e7c 03a1 0183 0101 007c 017d 0b69  ...|.......|.}.i
+00003b70: 007d 0c88 006a 0f90 0172 9688 006a 10a0  .}...j...r...j..
+00003b80: 1188 00a0 127c 01a1 01a1 017d 0d7c 0464  .....|.....}.|.d
+00003b90: 0575 0072 ba88 006a 136e 0488 006a 147d  .u.r...j.n...j.}
+00003ba0: 0e7c 0ea0 15a1 0044 005d ca5c 027d 0f7d  .|.....D.].\.}.}
+00003bb0: 107c 0f7c 0376 0172 da71 c87c 0464 0575  .|.|.v.r.q.|.d.u
+00003bc0: 0072 f874 056a 16a0 177c 0d7c 1018 00a1  .r.t.j...|.|....
+00003bd0: 017c 0c7c 0f3c 0071 c87c 0464 0575 0172  .|.|.<.q.|.d.u.r
+00003be0: c874 056a 166a 177c 0da0 187c 0d6a 0164  .t.j.j.|...|.j.d
+00003bf0: 0119 0064 0aa1 027c 10a0 187c 106a 0164  ...d...|...|.j.d
+00003c00: 0119 0064 0aa1 0218 0064 0664 078d 027d  ...d.....d.d...}
+00003c10: 1174 05a0 197c 11a1 0164 057c 0485 0219  .t...|...d.|....
+00003c20: 007d 127c 0564 0b6b 0290 0172 6074 05a0  .}.|.d.k...r`t..
+00003c30: 1a7c 117c 1219 00a1 017c 0c7c 0f3c 006e  .|.|.....|.|.<.n
+00003c40: 107c 117c 1264 0a19 0019 007c 0c7c 0f3c  .|.|.d.....|.|.<
+00003c50: 0074 056a 1b74 056a 1a7c 107c 1219 0064  .t.j.t.j.|.|...d
+00003c60: 0164 078d 0264 0164 078d 0288 006a 137c  .d...d.d.....j.|
+00003c70: 0f3c 0071 c86e 8888 006a 1c90 0272 1e7c  .<.q.n...j...r.|
+00003c80: 0464 0575 0090 0172 ac64 067d 0469 0088  .d.u...r.d.}.i..
+00003c90: 005f 1374 0988 006a 0a83 0144 005d 607d  ._.t...j...D.]`}
+00003ca0: 0f7c 0f7c 0376 0190 0172 ce90 0171 bc88  .|.|.v...r...q..
+00003cb0: 006a 1d7c 0f19 006a 1e7c 0b7c 0464 0c8d  .j.|...j.|.|.d..
+00003cc0: 025c 027d 137d 147c 1364 0119 0064 0a19  .\.}.}.|.d...d..
+00003cd0: 007c 0c7c 0f3c 0088 006a 1f7c 0f19 007c  .|.|.<...j.|...|
+00003ce0: 1464 0119 0064 0a19 0019 00a0 1864 0664  .d...d.......d.d
+00003cf0: 0aa1 0288 006a 137c 0f3c 0090 0171 bc88  .....j.|.<...q..
+00003d00: 006a 2090 0272 5a74 217c 0c7c 0c6a 2264  .j ..rZt!|.|.j"d
+00003d10: 0d8d 0288 005f 2388 006a 1388 006a 2319  ....._#..j...j#.
+00003d20: 007d 157c 0790 0272 6674 0d64 0ea0 0e88  .}.|...rft.d....
+00003d30: 006a 23a1 0183 0101 006e 0c74 05a0 2488  .j#......n.t..$.
+00003d40: 006a 25a1 017d 1588 006a 017d 1674 05a0  .j%..}...j.}.t..
+00003d50: 2488 006a 00a1 017d 1774 05a0 2688 006a  $..j...}.t..&..j
+00003d60: 00a1 0188 006a 2714 007d 1874 05a0 2688  .....j'..}.t..&.
+00003d70: 006a 00a1 0164 0f14 007d 1964 0f67 0188  .j...d...}.d.g..
+00003d80: 006a 0014 007d 1a74 05a0 2488 006a 0164  .j...}.t..$..j.d
+00003d90: 0664 0585 0219 00a1 0167 0188 006a 0014  .d.......g...j..
+00003da0: 007d 1b74 05a0 2488 006a 01a1 0174 05a0  .}.t..$..j...t..
+00003db0: 2488 006a 01a1 0166 027d 1c64 1064 1184  $..j...f.}.d.d..
+00003dc0: 0074 0988 006a 2883 0144 0083 0188 005f  .t...j(..D....._
+00003dd0: 2974 0988 006a 2883 0144 0090 065d f87d  )t...j(..D...].}
+00003de0: 1d88 006a 2aa0 2b88 006a 2ca1 0101 0064  ...j*.+..j,....d
+00003df0: 0f67 0188 006a 0014 007d 1e64 0a67 0188  .g...j...}.d.g..
+00003e00: 006a 0014 007d 1f88 006a 2d7c 0b88 006a  .j...}...j-|...j
+00003e10: 2e7c 0288 006a 2f7c 1888 006a 307c 0b88  .|...j/|...j0|..
+00003e20: 006a 317c 0b88 006a 327c 1569 067d 2088  .j1|...j2|.i.} .
+00003e30: 006a 2a6a 2b88 006a 337c 2064 128d 0201  .j*j+..j3| d....
+00003e40: 0067 0067 0002 007d 217d 2274 0988 006a  .g.g...}!}"t...j
+00003e50: 3483 0144 0090 055d b47d 2374 05a0 247c  4..D...].}#t..$|
+00003e60: 16a1 017d 2474 05a0 247c 16a1 017d 2588  ...}$t..$|...}%.
+00003e70: 006a 3590 0473 9688 006a 2764 136b 0390  .j5..s...j'd.k..
+00003e80: 0373 ae88 006a 2864 066b 0490 0472 9688  .s...j(d.k...r..
+00003e90: 006a 366a 3788 006a 2a64 148d 017d 2688  .j6j7..j*d...}&.
+00003ea0: 006a 386a 3788 006a 2a64 148d 017d 277c  .j8j7..j*d...}'|
+00003eb0: 21a0 397c 26a1 0101 007c 22a0 397c 27a1  !.9|&....|".9|'.
+00003ec0: 0101 007c 2388 006a 3a16 0064 016b 0290  ...|#..j:..d.k..
+00003ed0: 0472 967c 2364 016b 0490 0472 9688 006a  .r.|#d.k...r...j
+00003ee0: 3b6a 3788 006a 2a64 148d 017d 0f74 05a0  ;j7..j*d...}.t..
+00003ef0: 3c7c 21a1 017d 2174 05a0 3c7c 22a1 017d  <|!..}!t..<|"..}
+00003f00: 2288 006a 3d7c 217c 027c 1664 0664 0585  "..j=|!|.|.d.d..
+00003f10: 0219 0064 158d 037c 0f14 007d 2488 006a  ...d...|...}$..j
+00003f20: 3d7c 227c 027c 1664 0664 0585 0219 0064  =|"|.|.d.d.....d
+00003f30: 158d 037c 0f14 007d 2574 05a0 3e7c 2488  ...|...}%t..>|$.
+00003f40: 006a 3e64 0119 0088 006a 3e64 0619 00a1  .j>d.....j>d....
+00003f50: 037d 2474 05a0 3e7c 2588 006a 3e64 0119  .}$t..>|%..j>d..
+00003f60: 0088 006a 3e64 0619 00a1 037d 2567 0067  ...j>d.....}%g.g
+00003f70: 0002 007d 217d 2288 006a 2aa0 2b88 006a  ...}!}"..j*.+..j
+00003f80: 3fa1 017d 2864 1664 1784 007c 2844 0083  ?..}(d.d...|(D..
+00003f90: 0164 0119 007d 2974 05a0 3e7c 2988 006a  .d...})t..>|)..j
+00003fa0: 3e64 0119 0088 006a 3e64 0619 00a1 037d  >d.....j>d.....}
+00003fb0: 297c 297c 2517 007d 2a88 006a 2a6a 2b88  )|)|%..}*..j*j+.
+00003fc0: 006a 4088 006a 417c 2a69 0164 128d 0201  .j@..jA|*i.d....
+00003fd0: 0088 006a 2aa0 2b88 006a 4288 006a 4388  ...j*.+..jB..jC.
+00003fe0: 006a 4488 006a 4567 04a1 0101 0088 006a  .jD..jEg.......j
+00003ff0: 3590 0572 4088 006a 2aa0 2b88 006a 4688  5..r@..j*.+..jF.
+00004000: 006a 4788 006a 4888 006a 4988 006a 3667  .jG..jH..jI..j6g
+00004010: 05a1 015c 057d 2b7d 2c7d 2d7d 2e7d 2f6e  ...\.}+},}-}.}/n
+00004020: 6a88 006a 366a 3788 006a 2a64 148d 017d  j..j6j7..j*d...}
+00004030: 2674 4a6a 4b7c 2674 4a6a 4c64 188d 027d  &tJjK|&tJjLd...}
+00004040: 2688 00a0 117c 26a1 01a0 4da1 00a0 4ea1  &....|&...M...N.
+00004050: 007d 2e88 00a0 4f7c 2e7c 02a1 027d 2c88  .}....O|.|...},.
+00004060: 006a 477c 2c69 017d 2088 006a 2a6a 2b88  .jG|,i.} ..j*j+.
+00004070: 006a 4688 006a 4888 006a 3667 037c 2064  .jF..jH..j6g.| d
+00004080: 128d 025c 037d 2b7d 2d7d 2f7c 237c 0916  ...\.}+}-}/|#|..
+00004090: 0064 016b 0290 0573 c67c 237c 0816 0064  .d.k...s.|#|...d
+000040a0: 016b 0290 0672 1a88 006a 2aa0 2b88 006a  .k...r...j*.+..j
+000040b0: 5088 006a 5188 006a 5288 006a 5367 04a1  P..jQ..jR..jSg..
+000040c0: 015c 047d 307d 317d 327d 3374 05a0 547c  .\.}0}1}2}3t..T|
+000040d0: 2e7c 0214 00a1 017d 3474 05a0 5564 067c  .|.....}4t..Ud.|
+000040e0: 0218 007c 2e14 00a1 017d 357c 2d7c 2c17  ...|.....}5|-|,.
+000040f0: 007c 3217 007c 3317 007d 367c 237c 0916  .|2..|3..}6|#|..
+00004100: 0064 016b 0290 0772 2488 006a 5664 0575  .d.k...r$..jVd.u
+00004110: 0190 0772 2488 006a 2aa0 2b88 006a 5788  ...r$..j*.+..jW.
+00004120: 006a 5888 006a 5967 03a1 015c 037d 377d  .jX..jYg...\.}7}
+00004130: 387d 3974 5aa0 5ba1 007d 3a7c 3a6a 5c6a  8}9tZ.[..}:|:j\j
+00004140: 5d64 197c 3664 1a8d 0201 007c 3a6a 5c6a  ]d.|6d.....|:j\j
+00004150: 5d64 1b7c 2b64 1a8d 0201 007c 3a6a 5c6a  ]d.|+d.....|:j\j
+00004160: 5d64 1c7c 3164 1a8d 0201 007c 3a6a 5c6a  ]d.|1d.....|:j\j
+00004170: 5d64 1d7c 3064 1a8d 0201 007c 3a6a 5c6a  ]d.|0d.....|:j\j
+00004180: 5d64 1e7c 3264 1a8d 0201 007c 3a6a 5c6a  ]d.|2d.....|:j\j
+00004190: 5d64 1f7c 3364 1a8d 0201 007c 3a6a 5c6a  ]d.|3d.....|:j\j
+000041a0: 5d64 207c 1864 0119 0064 1a8d 0201 007c  ]d |.d...d.....|
+000041b0: 3a6a 5c6a 5d64 217c 2c64 1a8d 0201 007c  :j\j]d!|,d.....|
+000041c0: 3a6a 5c6a 5d64 227c 3764 1a8d 0201 007c  :j\j]d"|7d.....|
+000041d0: 3a6a 5c6a 5d64 237c 3864 1a8d 0201 007c  :j\j]d#|8d.....|
+000041e0: 3a6a 5c6a 5d64 247c 3964 1a8d 0201 0088  :j\j]d$|9d......
+000041f0: 006a 56a0 5e7c 3aa1 0101 0088 006a 56a0  .jV.^|:......jV.
+00004200: 5fa1 0001 007c 0790 0872 127c 237c 0816  _....|...r.|#|..
+00004210: 0064 016b 0290 0872 1274 0d64 25a0 0e7c  .d.k...r.t.d%..|
+00004220: 237c 1864 0119 00a1 0283 0101 0074 0d64  #|.d.........t.d
+00004230: 26a0 0e7c 2b7c 2ca1 0283 0101 0074 0d64  &..|+|,......t.d
+00004240: 27a0 0e7c 307c 317c 32a1 0383 0101 0074  '..|0|1|2......t
+00004250: 0d64 28a0 0e7c 33a1 0183 0101 0074 0d64  .d(..|3......t.d
+00004260: 29a0 0e7c 347c 35a1 0283 0101 0074 0d64  )..|4|5......t.d
+00004270: 2aa0 0e7c 29a0 21a1 007c 29a0 55a1 00a1  *..|).!..|).U...
+00004280: 0283 0101 0074 0d64 2ba0 0e74 05a0 1a7c  .....t.d+..t...|
+00004290: 29a1 0174 05a0 1a74 05a0 607c 29a1 01a1  )..t...t..`|)...
+000042a0: 01a1 0283 0101 0088 006a 3590 0873 0874  .........j5..s.t
+000042b0: 0d64 2ca0 0e7c 24a0 21a1 007c 24a0 55a1  .d,..|$.!..|$.U.
+000042c0: 00a1 0283 0101 0074 0d64 2da0 0e74 05a0  .......t.d-..t..
+000042d0: 1a7c 24a1 0174 05a0 1a74 05a0 607c 24a1  .|$..t...t..`|$.
+000042e0: 01a1 01a1 0283 0101 0074 616a 62a0 5fa1  .........tajb._.
+000042f0: 0001 0074 6374 647c 2d7c 2e7c 2f83 0383  ...tctd|-|.|/...
+00004300: 0144 0090 015d 025c 027d 3b5c 037d 3c7d  .D...].\.};\.}<}
+00004310: 3d7d 3e74 05a0 0c7c 027c 3b19 00a1 017d  =}>t...|.|;....}
+00004320: 3f74 05a0 0c7c 3da1 017d 4074 056a 1b7c  ?t...|=..}@t.j.|
+00004330: 3e64 0164 078d 027d 3e7c 0664 136b 0490  >d.d...}>|.d.k..
+00004340: 0872 8088 00a0 657c 3e74 05a0 0c7c 2ea1  .r....e|>t...|..
+00004350: 017c 3fa1 037d 417c 417c 066b 047d 426e  .|?..}A|A|.k.}Bn
+00004360: 0464 2e7d 427c 3c7c 1e7c 3b19 006b 0090  .d.}B|<|.|;..k..
+00004370: 0872 be7c 0a7c 3d7c 3f83 0290 0872 be7c  .r.|.|=|?....r.|
+00004380: 4290 0872 be7c 407c 0376 0090 0872 be7c  B..r.|@|.v...r.|
+00004390: 3c7c 1e7c 3b3c 007c 407c 1f7c 3b3c 007c  <|.|;<.|@|.|;<.|
+000043a0: 3c7c 1a7c 3b19 006b 0090 0872 227c 0a7c  <|.|;..k...r"|.|
+000043b0: 3d7c 3f83 0290 0872 227c 4290 0872 227c  =|?....r"|B..r"|
+000043c0: 407c 0376 0090 0872 227c 0790 0872 f674  @|.v...r"|...r.t
+000043d0: 0d64 2f83 0101 007c 3c7c 1a7c 3b3c 007c  .d/....|<|.|;<.|
+000043e0: 3e7c 1b7c 3b3c 007c 297c 2466 027d 1c64  >|.|;<.|)|$f.}.d
+000043f0: 2e88 005f 6688 006a 297c 1d19 00a0 397c  ..._f..j)|....9|
+00004400: 3ea1 0101 0090 0871 2290 0371 7474 0988  >......q"..qtt..
+00004410: 006a 0083 0144 005d ba7d 3b7c 0a7c 1f7c  .j...D.].};|.|.|
+00004420: 3b19 0074 05a0 0c7c 027c 3b19 00a1 0183  ;..t...|.|;.....
+00004430: 0290 0972 a07c 1f7c 3b19 0064 0a6b 0390  ...r.|.|;..d.k..
+00004440: 0972 a074 217c 197c 3b19 007c 187c 3b19  .r.t!|.|;..|.|;.
+00004450: 0083 027c 197c 3b3c 007c 197c 3b19 0064  ...|.|;<.|.|;..d
+00004460: 306b 0090 0972 ee7c 177c 3b19 007c 197c  0k...r.|.|;..|.|
+00004470: 3b19 0017 0064 311b 007c 187c 3b3c 006e  ;....d1..|.|;<.n
+00004480: 4e74 557c 177c 3b19 007c 187c 3b19 0083  NtU|.|;..|.|;...
+00004490: 027c 177c 3b3c 007c 197c 3b19 0064 306b  .|.|;<.|.|;..d0k
+000044a0: 0090 0972 de7c 177c 3b19 007c 197c 3b19  ...r.|.|;..|.|;.
+000044b0: 0017 0064 311b 007c 187c 3b3c 006e 107c  ...d1..|.|;<.n.|
+000044c0: 187c 3b05 0019 0064 3239 0003 003c 0090  .|;....d29...<..
+000044d0: 0971 3690 0271 fa74 056a 3c7c 1b64 0164  .q6..q.t.j<|.d.d
+000044e0: 078d 027d 437c 436a 0188 006a 016b 0390  ...}C|Cj...j.k..
+000044f0: 0a72 2074 056a 1b7c 4364 0164 078d 027d  .r t.j.|Cd.d...}
+00004500: 437c 437c 1c66 0253 0029 3361 9f06 0000  C|C|.f.S.)3a....
+00004510: 0a20 2020 2020 2020 2046 696e 6420 6120  .        Find a 
+00004520: 636f 756e 7465 7266 6163 7475 616c 2028  counterfactual (
+00004530: 4346 2920 666f 7220 696e 7374 616e 6365  CF) for instance
+00004540: 2060 5860 2075 7369 6e67 2061 2066 6173   `X` using a fas
+00004550: 7420 6974 6572 6174 6976 6520 7368 7269  t iterative shri
+00004560: 6e6b 6167 652d 7468 7265 7368 6f6c 6469  nkage-thresholdi
+00004570: 6e67 2061 6c67 6f72 6974 686d 2028 4649  ng algorithm (FI
+00004580: 5354 4129 2e0a 0a20 2020 2020 2020 2050  STA)...        P
+00004590: 6172 616d 6574 6572 7320 6d6b 0a20 2020  arameters mk.   
+000045a0: 2020 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a       ----------.
+000045b0: 2020 2020 2020 2020 580a 2020 2020 2020          X.      
+000045c0: 2020 2020 2020 496e 7374 616e 6365 2074        Instance t
+000045d0: 6f20 6174 7461 636b 2e0a 2020 2020 2020  o attack..      
+000045e0: 2020 590a 2020 2020 2020 2020 2020 2020    Y.            
+000045f0: 4c61 6265 6c73 2066 6f72 2060 5860 2061  Labels for `X` a
+00004600: 7320 6f6e 652d 686f 742d 656e 636f 6469  s one-hot-encodi
+00004610: 6e67 2e0a 2020 2020 2020 2020 7461 7267  ng..        targ
+00004620: 6574 5f63 6c61 7373 0a20 2020 2020 2020  et_class.       
+00004630: 2020 2020 204c 6973 7420 7769 7468 2074       List with t
+00004640: 6172 6765 7420 636c 6173 7365 7320 7573  arget classes us
+00004650: 6564 2074 6f20 6669 6e64 2063 6c6f 7365  ed to find close
+00004660: 7374 2070 726f 746f 7479 7065 2e20 4966  st prototype. If
+00004670: 2060 604e 6f6e 6560 602c 2074 6865 206e   ``None``, the n
+00004680: 6561 7265 7374 2070 726f 746f 7479 7065  earest prototype
+00004690: 0a20 2020 2020 2020 2020 2020 2065 7863  .            exc
+000046a0: 6570 7420 666f 7220 7468 6520 7072 6564  ept for the pred
+000046b0: 6963 7420 636c 6173 7320 6f6e 2074 6865  ict class on the
+000046c0: 2069 6e73 7461 6e63 6520 6973 2075 7365   instance is use
+000046d0: 642e 0a20 2020 2020 2020 206b 0a20 2020  d..        k.   
+000046e0: 2020 2020 2020 2020 204e 756d 6265 7220           Number 
+000046f0: 6f66 206e 6561 7265 7374 2069 6e73 7461  of nearest insta
+00004700: 6e63 6573 2075 7365 6420 746f 2064 6566  nces used to def
+00004710: 696e 6520 7468 6520 7072 6f74 6f74 7970  ine the prototyp
+00004720: 6520 666f 7220 6120 636c 6173 732e 2044  e for a class. D
+00004730: 6566 6175 6c74 7320 746f 2075 7369 6e67  efaults to using
+00004740: 2061 6c6c 0a20 2020 2020 2020 2020 2020   all.           
+00004750: 2069 6e73 7461 6e63 6573 2062 656c 6f6e   instances belon
+00004760: 6769 6e67 2074 6f20 7468 6520 636c 6173  ging to the clas
+00004770: 7320 6966 2061 6e20 656e 636f 6465 7220  s if an encoder 
+00004780: 6973 2075 7365 6420 616e 6420 746f 2031  is used and to 1
+00004790: 2066 6f72 206b 2d64 2074 7265 6573 2e0a   for k-d trees..
+000047a0: 2020 2020 2020 2020 6b5f 7479 7065 0a20          k_type. 
+000047b0: 2020 2020 2020 2020 2020 2055 7365 2065             Use e
+000047c0: 6974 6865 7220 7468 6520 6176 6572 6167  ither the averag
+000047d0: 6520 656e 636f 6469 6e67 206f 6620 7468  e encoding of th
+000047e0: 6520 6b20 6e65 6172 6573 7420 696e 7374  e k nearest inst
+000047f0: 616e 6365 7320 696e 2061 2063 6c61 7373  ances in a class
+00004800: 2028 6060 6b5f 7479 7065 3d27 6d65 616e   (``k_type='mean
+00004810: 2760 6029 206f 720a 2020 2020 2020 2020  '``) or.        
+00004820: 2020 2020 7468 6520 6b2d 6e65 6172 6573      the k-neares
+00004830: 7420 656e 636f 6469 6e67 2069 6e20 7468  t encoding in th
+00004840: 6520 636c 6173 7320 2860 606b 5f74 7970  e class (``k_typ
+00004850: 653d 2770 6f69 6e74 2760 6029 2074 6f20  e='point'``) to 
+00004860: 6465 6669 6e65 2074 6865 2070 726f 746f  define the proto
+00004870: 7479 7065 206f 6620 7468 6174 2063 6c61  type of that cla
+00004880: 7373 2e0a 2020 2020 2020 2020 2020 2020  ss..            
+00004890: 4f6e 6c79 2072 656c 6576 616e 7420 6966  Only relevant if
+000048a0: 2061 6e20 656e 636f 6465 7220 6973 2075   an encoder is u
+000048b0: 7365 6420 746f 2064 6566 696e 6520 7468  sed to define th
+000048c0: 6520 7072 6f74 6f74 7970 6573 2e0a 2020  e prototypes..  
+000048d0: 2020 2020 2020 7468 7265 7368 6f6c 640a        threshold.
+000048e0: 2020 2020 2020 2020 2020 2020 5468 7265              Thre
+000048f0: 7368 6f6c 6420 6c65 7665 6c20 666f 7220  shold level for 
+00004900: 7468 6520 7261 7469 6f20 6265 7477 6565  the ratio betwee
+00004910: 6e20 7468 6520 6469 7374 616e 6365 206f  n the distance o
+00004920: 6620 7468 6520 636f 756e 7465 7266 6163  f the counterfac
+00004930: 7475 616c 2074 6f20 7468 6520 7072 6f74  tual to the prot
+00004940: 6f74 7970 6520 6f66 2074 6865 0a20 2020  otype of the.   
+00004950: 2020 2020 2020 2020 2070 7265 6469 6374           predict
+00004960: 6564 2063 6c61 7373 2066 6f72 2074 6865  ed class for the
+00004970: 206f 7269 6769 6e61 6c20 696e 7374 616e   original instan
+00004980: 6365 206f 7665 7220 7468 6520 6469 7374  ce over the dist
+00004990: 616e 6365 2074 6f20 7468 6520 7072 6f74  ance to the prot
+000049a0: 6f74 7970 6520 6f66 2074 6865 2070 7265  otype of the pre
+000049b0: 6469 6374 6564 2063 6c61 7373 0a20 2020  dicted class.   
+000049c0: 2020 2020 2020 2020 2066 6f72 2074 6865           for the
+000049d0: 2063 6f75 6e74 6572 6661 6374 7561 6c2e   counterfactual.
+000049e0: 2049 6620 7468 6520 7472 7573 7420 7363   If the trust sc
+000049f0: 6f72 6520 6973 2062 656c 6f77 2074 6865  ore is below the
+00004a00: 2074 6872 6573 686f 6c64 2c20 7468 6520   threshold, the 
+00004a10: 7072 6f70 6f73 6564 2063 6f75 6e74 6572  proposed counter
+00004a20: 6661 6374 7561 6c20 646f 6573 0a20 2020  factual does.   
+00004a30: 2020 2020 2020 2020 206e 6f74 206d 6565           not mee
+00004a40: 7420 7468 6520 7265 7175 6972 656d 656e  t the requiremen
+00004a50: 7473 2e0a 2020 2020 2020 2020 7665 7262  ts..        verb
+00004a60: 6f73 650a 2020 2020 2020 2020 2020 2020  ose.            
+00004a70: 5072 696e 7420 696e 7465 726d 6564 6961  Print intermedia
+00004a80: 7465 2072 6573 756c 7473 206f 6620 6f70  te results of op
+00004a90: 7469 6d69 7a61 7469 6f6e 2069 6620 6060  timization if ``
+00004aa0: 5472 7565 6060 2e0a 2020 2020 2020 2020  True``..        
+00004ab0: 7072 696e 745f 6576 6572 790a 2020 2020  print_every.    
+00004ac0: 2020 2020 2020 2020 5072 696e 7420 6672          Print fr
+00004ad0: 6571 7565 6e63 7920 6966 2076 6572 626f  equency if verbo
+00004ae0: 7365 2069 7320 6060 5472 7565 6060 2e0a  se is ``True``..
+00004af0: 2020 2020 2020 2020 6c6f 675f 6576 6572          log_ever
+00004b00: 790a 2020 2020 2020 2020 2020 2020 6074  y.            `t
+00004b10: 656e 736f 7262 6f61 7264 6020 6c6f 6720  ensorboard` log 
+00004b20: 6672 6571 7565 6e63 7920 6966 2077 7269  frequency if wri
+00004b30: 7465 2064 6972 6563 746f 7279 2069 7320  te directory is 
+00004b40: 7370 6563 6966 6965 642e 0a0a 2020 2020  specified...    
+00004b50: 2020 2020 5265 7475 726e 730a 2020 2020      Returns.    
+00004b60: 2020 2020 2d2d 2d2d 2d2d 2d0a 2020 2020      -------.    
+00004b70: 2020 2020 4f76 6572 616c 6c20 6265 7374      Overall best
+00004b80: 2061 7474 6163 6b20 616e 6420 6772 6164   attack and grad
+00004b90: 6965 6e74 7320 666f 7220 7468 6174 2061  ients for that a
+00004ba0: 7474 6163 6b2e 0a20 2020 2020 2020 2072  ttack..        r
+00004bb0: 0100 0000 2903 7261 0000 00da 0179 7231  ....).ra.....yr1
+00004bc0: 0000 0063 0200 0000 0000 0000 0000 0000  ...c............
+00004bd0: 0200 0000 0500 0000 1300 0000 7340 0000  ............s@..
+00004be0: 0074 007c 0074 0174 0274 036a 0466 0383  .t.|.t.t.t.j.f..
+00004bf0: 0273 3874 03a0 057c 00a1 017d 007c 007c  .s8t...|...}.|.|
+00004c00: 0105 0019 0088 006a 0637 0003 003c 0074  .......j.7...<.t
+00004c10: 03a0 077c 00a1 017d 007c 007c 016b 0353  ...|...}.|.|.k.S
+00004c20: 0029 0161 8501 0000 0a20 2020 2020 2020  .).a.....       
+00004c30: 2020 2020 2043 6f6d 7061 7265 2070 7265       Compare pre
+00004c40: 6469 6374 696f 6e73 2077 6974 6820 7461  dictions with ta
+00004c50: 7267 6574 206c 6162 656c 7320 616e 6420  rget labels and 
+00004c60: 7265 7475 726e 2077 6865 7468 6572 2063  return whether c
+00004c70: 6f75 6e74 6572 6661 6374 7561 6c20 636f  ounterfactual co
+00004c80: 6e64 6974 696f 6e73 2068 6f6c 642e 0a0a  nditions hold...
+00004c90: 2020 2020 2020 2020 2020 2020 5061 7261              Para
+00004ca0: 6d65 7465 7273 0a20 2020 2020 2020 2020  meters.         
+00004cb0: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
+00004cc0: 2020 2020 2020 2020 2020 780a 2020 2020            x.    
+00004cd0: 2020 2020 2020 2020 2020 2020 5072 6564              Pred
+00004ce0: 6963 7465 6420 636c 6173 7320 7072 6f62  icted class prob
+00004cf0: 6162 696c 6974 6965 7320 6f72 206c 6162  abilities or lab
+00004d00: 656c 732e 0a20 2020 2020 2020 2020 2020  els..           
+00004d10: 2079 0a20 2020 2020 2020 2020 2020 2020   y.             
+00004d20: 2020 2054 6172 6765 7420 6f72 2070 7265     Target or pre
+00004d30: 6469 6374 6564 206c 6162 656c 732e 0a0a  dicted labels...
+00004d40: 2020 2020 2020 2020 2020 2020 5265 7475              Retu
+00004d50: 726e 730a 2020 2020 2020 2020 2020 2020  rns.            
+00004d60: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
+00004d70: 2020 2020 426f 6f6c 2077 6865 7468 6572      Bool whether
+00004d80: 2063 6f75 6e74 6572 6661 6374 7561 6c20   counterfactual 
+00004d90: 636f 6e64 6974 696f 6e73 2068 6f6c 642e  conditions hold.
+00004da0: 0a20 2020 2020 2020 2020 2020 2029 0872  .            ).r
+00004db0: 3d00 0000 723e 0000 00da 0369 6e74 723f  =...r>.....intr?
+00004dc0: 0000 00da 0569 6e74 3634 7269 0000 0072  .....int64ri...r
+00004dd0: 1e00 0000 da06 6172 676d 6178 2902 7261  ......argmax).ra
+00004de0: 0000 0072 f800 0000 a901 7234 0000 0072  ...r......r4...r
+00004df0: 4400 0000 7245 0000 00da 0763 6f6d 7061  D...rE.....compa
+00004e00: 7265 b302 0000 730a 0000 0000 0f12 010a  re....s.........
+00004e10: 0112 010a 017a 2643 6f75 6e74 6572 6661  .....z&Counterfa
+00004e20: 6374 7561 6c2e 6174 7461 636b 2e3c 6c6f  ctual.attack.<lo
+00004e30: 6361 6c73 3e2e 636f 6d70 6172 654e 721a  cals>.compareNr.
+00004e40: 0000 0072 5900 0000 7a13 5072 6564 6963  ...rY...z.Predic
+00004e50: 7465 6420 636c 6173 733a 207b 7d7a 1254  ted class: {}z.T
+00004e60: 6172 6765 7420 636c 6173 7365 733a 207b  arget classes: {
+00004e70: 7d72 3300 0000 72c7 0000 0072 ec00 0000  }r3...r....r....
+00004e80: 2901 72b8 0000 007a 1350 726f 746f 7479  ).r....z.Prototy
+00004e90: 7065 2063 6c61 7373 3a20 7b7d 7212 0000  pe class: {}r...
+00004ea0: 0063 0100 0000 0000 0000 0000 0000 0200  .c..............
+00004eb0: 0000 0400 0000 5300 0000 7312 0000 0069  ......S...s....i
+00004ec0: 007c 005d 0a7d 017c 0167 0093 0271 0453  .|.].}.|.g...q.S
+00004ed0: 0072 4400 0000 7244 0000 0029 0272 4200  .rD...rD...).rB.
+00004ee0: 0000 72cb 0000 0072 4400 0000 7244 0000  ..r....rD...rD..
+00004ef0: 0072 4500 0000 da0a 3c64 6963 7463 6f6d  .rE.....<dictcom
+00004f00: 703e 1003 0000 7263 0000 007a 2943 6f75  p>....rc...z)Cou
+00004f10: 6e74 6572 6661 6374 7561 6c2e 6174 7461  nterfactual.atta
+00004f20: 636b 2e3c 6c6f 6361 6c73 3e2e 3c64 6963  ck.<locals>.<dic
+00004f30: 7463 6f6d 703e 2901 da09 6665 6564 5f64  tcomp>)...feed_d
+00004f40: 6963 7472 0f00 0000 72d0 0000 0029 0172  ictr....r....).r
+00004f50: d800 0000 6301 0000 0000 0000 0000 0000  ....c...........
+00004f60: 0003 0000 0004 0000 0053 0000 0073 1400  .........S...s..
+00004f70: 0000 6700 7c00 5d0c 5c02 7d01 7d02 7c01  ..g.|.].\.}.}.|.
+00004f80: 9102 7104 5300 7244 0000 0072 4400 0000  ..q.S.rD...rD...
+00004f90: 2903 7242 0000 0072 de00 0000 7243 0000  ).rB...r....rC..
+00004fa0: 0072 4400 0000 7244 0000 0072 4500 0000  .rD...rD...rE...
+00004fb0: 7246 0000 0050 0300 0072 6300 0000 7a29  rF...P...rc...z)
+00004fc0: 436f 756e 7465 7266 6163 7475 616c 2e61  Counterfactual.a
+00004fd0: 7474 6163 6b2e 3c6c 6f63 616c 733e 2e3c  ttack.<locals>.<
+00004fe0: 6c69 7374 636f 6d70 3e29 0172 4800 0000  listcomp>).rH...
+00004ff0: 7a0e 6c6f 7373 2f4f 7074 696d 697a 6564  z.loss/Optimized
+00005000: 2902 da03 7461 675a 0c73 696d 706c 655f  )...tagZ.simple_
+00005010: 7661 6c75 657a 0a6c 6f73 732f 546f 7461  valuez.loss/Tota
+00005020: 6c7a 076c 6f73 732f 4c31 7a07 6c6f 7373  lz.loss/L1z.loss
+00005030: 2f4c 327a 106c 6f73 732f 4175 746f 456e  /L2z.loss/AutoEn
+00005040: 636f 6465 727a 136c 6f73 732f 436c 6173  coderz.loss/Clas
+00005050: 7350 726f 746f 7479 7065 7a0e 6c6f 7373  sPrototypez.loss
+00005060: 2f50 7265 6453 6361 6c65 7a0d 6c6f 7373  /PredScalez.loss
+00005070: 2f50 7265 644c 6f73 737a 0b74 7261 696e  /PredLossz.train
+00005080: 696e 672f 6c72 7a0a 7472 6169 6e69 6e67  ing/lrz.training
+00005090: 2f7a 7a13 7472 6169 6e69 6e67 2f47 6c6f  /zz.training/Glo
+000050a0: 6261 6c53 7465 707a 190a 4974 6572 6174  balStepz..Iterat
+000050b0: 696f 6e3a 207b 7d3b 2043 6f6e 7374 3a20  ion: {}; Const: 
+000050c0: 7b7d 7a27 4c6f 7373 2074 6f74 616c 3a20  {}z'Loss total: 
+000050d0: 7b3a 2e33 667d 2c20 6c6f 7373 2061 7474  {:.3f}, loss att
+000050e0: 6163 6b3a 207b 3a2e 3366 7d7a 274c 323a  ack: {:.3f}z'L2:
+000050f0: 207b 3a2e 3366 7d2c 204c 313a 207b 3a2e   {:.3f}, L1: {:.
+00005100: 3366 7d2c 206c 6f73 7320 4145 3a20 7b3a  3f}, loss AE: {:
+00005110: 2e33 667d 7a12 4c6f 7373 2070 726f 746f  .3f}z.Loss proto
+00005120: 3a20 7b3a 2e33 667d 7a32 5461 7267 6574  : {:.3f}z2Target
+00005130: 2070 726f 6261 3a20 7b3a 2e32 667d 2c20   proba: {:.2f}, 
+00005140: 6d61 7820 6e6f 6e20 7461 7267 6574 2070  max non target p
+00005150: 726f 6261 3a20 7b3a 2e32 667d 7a25 4772  roba: {:.2f}z%Gr
+00005160: 6164 6965 6e74 2067 7261 7068 206d 696e  adient graph min
+00005170: 2f6d 6178 3a20 7b3a 2e33 667d 2f7b 3a2e  /max: {:.3f}/{:.
+00005180: 3366 7d7a 2b47 7261 6469 656e 7420 6772  3f}z+Gradient gr
+00005190: 6170 6820 6d65 616e 2f61 6273 206d 6561  aph mean/abs mea
+000051a0: 6e3a 207b 3a2e 3366 7d2f 7b3a 2e33 667d  n: {:.3f}/{:.3f}
+000051b0: 7a30 4772 6164 6965 6e74 206e 756d 6572  z0Gradient numer
+000051c0: 6963 616c 2061 7474 6163 6b20 6d69 6e2f  ical attack min/
+000051d0: 6d61 783a 207b 3a2e 3366 7d2f 7b3a 2e33  max: {:.3f}/{:.3
+000051e0: 667d 7a2f 4772 6164 6965 6e74 206e 756d  f}z/Gradient num
+000051f0: 6572 6963 616c 206d 6561 6e2f 6162 7320  erical mean/abs 
+00005200: 6d65 616e 3a20 7b3a 2e33 667d 2f7b 3a2e  mean: {:.3f}/{:.
+00005210: 3366 7d54 7a1f 0a4e 6577 2062 6573 7420  3f}Tz..New best 
+00005220: 636f 756e 7465 7266 6163 7475 616c 2066  counterfactual f
+00005230: 6f75 6e64 2167 0000 0000 65cd cd41 7207  ound!g....e..Ar.
+00005240: 0000 0072 1600 0000 2967 7280 0000 0072  ...r....)gr....r
+00005250: 1d00 0000 7206 0000 0072 3e00 0000 72f9  ....r....r>...r.
+00005260: 0000 0072 3f00 0000 da07 6e64 6172 7261  ...r?.....ndarra
+00005270: 79da 0462 6f6f 6c72 9900 0000 7282 0000  y..boolr....r...
+00005280: 0072 7800 0000 72b7 0000 0072 fb00 0000  .rx...r....r....
+00005290: 727a 0000 00da 0666 6f72 6d61 7472 2300  rz.....formatr#.
+000052a0: 0000 727f 0000 0072 1b00 0000 721c 0000  ..r....r....r...
+000052b0: 0072 c300 0000 72c4 0000 00da 0569 7465  .r....r......ite
+000052c0: 6d73 72ee 0000 0072 a200 0000 72e4 0000  msr....r....r...
+000052d0: 00da 0761 7267 736f 7274 72c7 0000 0072  ...argsortr....r
+000052e0: c600 0000 7225 0000 0072 c900 0000 72ef  ....r%...r....r.
+000052f0: 0000 0072 ca00 0000 723b 0000 00da 036d  ...r....r;.....m
+00005300: 696e da03 6765 74da 0869 645f 7072 6f74  in..get..id_prot
+00005310: 6f72 7700 0000 7285 0000 0072 4000 0000  orw...r....r@...
+00005320: 7228 0000 0072 2900 0000 da09 6366 5f67  r(...r).....cf_g
+00005330: 6c6f 6261 6c72 2f00 0000 da03 7275 6e72  lobalr/.....runr
+00005340: b300 0000 7250 0000 0072 5400 0000 7255  ....rP...rT...rU
+00005350: 0000 0072 5200 0000 7253 0000 0072 5600  ...rR...rS...rV.
+00005360: 0000 72b1 0000 0072 2700 0000 7276 0000  ..r....r'...rv..
+00005370: 0072 4a00 0000 72d4 0000 0072 4b00 0000  .rJ...r....rK...
+00005380: 72b2 0000 0072 2c00 0000 724e 0000 0072  r....r,...rN...r
+00005390: e500 0000 72e8 0000 0072 2b00 0000 72ae  ....r....r+...r.
+000053a0: 0000 0072 b000 0000 72af 0000 0072 9500  ...r....r....r..
+000053b0: 0000 7296 0000 0072 9700 0000 7298 0000  ..r....r....r...
+000053c0: 0072 aa00 0000 725c 0000 0072 9f00 0000  .r....r\...r....
+000053d0: 72a4 0000 0072 7900 0000 72e1 0000 0072  r....ry...r....r
+000053e0: 8400 0000 72e2 0000 0072 e300 0000 72d6  ....r....r....r.
+000053f0: 0000 0072 a100 0000 72a0 0000 0072 5b00  ...r....r....r[.
+00005400: 0000 72a8 0000 0072 d200 0000 72d3 0000  ..r....r....r...
+00005410: 0072 b500 0000 72ac 0000 0072 9300 0000  .r....r....r....
+00005420: 724f 0000 0072 6f00 0000 da07 5375 6d6d  rO...ro.....Summ
+00005430: 6172 79da 0576 616c 7565 7290 0000 00da  ary..valuer.....
+00005440: 0b61 6464 5f73 756d 6d61 7279 da05 666c  .add_summary..fl
+00005450: 7573 6872 8b00 0000 da03 7379 73da 0673  ushr......sys..s
+00005460: 7464 6f75 74da 0965 6e75 6d65 7261 7465  tdout..enumerate
+00005470: da03 7a69 7072 f100 0000 da0b 6265 7374  ..zipr......best
+00005480: 5f61 7474 6163 6b29 4472 3400 0000 72d7  _attack)Dr4...r.
+00005490: 0000 0072 cf00 0000 72f3 0000 0072 ed00  ...r....r....r..
+000054a0: 0000 72f4 0000 0072 f500 0000 7230 0000  ..r....r....r0..
+000054b0: 0072 f600 0000 72f7 0000 0072 fd00 0000  .r....r....r....
+000054c0: 5a05 585f 6e75 6d5a 0a64 6973 745f 7072  Z.X_numZ.dist_pr
+000054d0: 6f74 6f72 f000 0000 da0a 636c 6173 735f  otor......class_
+000054e0: 6469 6374 da01 63da 0176 5a06 6469 7374  dict..c..vZ.dist
+000054f0: 5f6b 72cc 0000 005a 0664 6973 745f 635a  _kr....Z.dist_cZ
+00005500: 0569 6478 5f63 5a09 7072 6f74 6f5f 7661  .idx_cZ.proto_va
+00005510: 6c5a 0a70 6572 745f 7368 6170 655a 0863  lZ.pert_shapeZ.c
+00005520: 6f6e 7374 5f6c 6272 4e00 0000 5a08 636f  onst_lbrN...Z.co
+00005530: 6e73 745f 7562 5a11 6f76 6572 616c 6c5f  nst_ubZ.overall_
+00005540: 6265 7374 5f64 6973 745a 136f 7665 7261  best_distZ.overa
+00005550: 6c6c 5f62 6573 745f 6174 7461 636b 5a11  ll_best_attackZ.
+00005560: 6f76 6572 616c 6c5f 6265 7374 5f67 7261  overall_best_gra
+00005570: 6472 4300 0000 5a11 6375 7272 656e 745f  drC...Z.current_
+00005580: 6265 7374 5f64 6973 745a 1263 7572 7265  best_distZ.curre
+00005590: 6e74 5f62 6573 745f 7072 6f62 6172 ff00  nt_best_probar..
+000055a0: 0000 5a0b 585f 6465 725f 6261 7463 685a  ..Z.X_der_batchZ
+000055b0: 0d58 5f64 6572 5f62 6174 6368 5f73 72cb  .X_der_batch_sr.
+000055c0: 0000 00da 0967 7261 6473 5f6e 756d 5a0b  .....grads_numZ.
+000055d0: 6772 6164 735f 6e75 6d5f 735a 0558 5f64  grads_num_sZ.X_d
+000055e0: 6572 5a07 585f 6465 725f 735a 1067 7261  erZ.X_der_sZ.gra
+000055f0: 6473 5f76 6172 735f 6772 6170 68da 0b67  ds_vars_graph..g
+00005600: 7261 6473 5f67 7261 7068 72e7 0000 005a  rads_graphr....Z
+00005610: 086c 6f73 735f 746f 7472 5c00 0000 7258  .loss_totr\...rX
+00005620: 0000 0072 a400 0000 724a 0000 0072 a100  ...r....rJ...r..
+00005630: 0000 72a0 0000 0072 5b00 0000 72a8 0000  ..r....r[...r...
+00005640: 0072 a600 0000 72a7 0000 0072 a900 0000  .r....r....r....
+00005650: da02 6c72 7293 0000 00da 0267 7372 b400  ..lrr......gsr..
+00005660: 0000 da09 6261 7463 685f 6964 78da 0464  ....batch_idx..d
+00005670: 6973 7472 d900 0000 5a07 6164 765f 6964  istr....Z.adv_id
+00005680: 78da 0759 5f63 6c61 7373 72ea 0000 0072  x..Y_classr....r
+00005690: f100 0000 5a0f 6162 6f76 655f 7468 7265  ....Z.above_thre
+000056a0: 7368 6f6c 6472 1301 0000 7244 0000 0072  sholdr....rD...r
+000056b0: fc00 0000 7245 0000 00da 0661 7474 6163  ....rE.....attac
+000056c0: 6b80 0200 0073 f001 0000 0031 1402 2216  k....s.....1..".
+000056d0: 0801 0e01 1401 0401 1801 0e02 0403 0401  ................
+000056e0: 0802 1201 1402 1001 0801 0201 0801 1601  ................
+000056f0: 0801 0601 2201 02fe 0604 1201 0a01 1402  ...."...........
+00005700: 1001 0401 12ff 1003 0801 0a01 0401 0601  ................
+00005710: 0e01 0a01 0403 1801 1001 2802 0801 1002  ..........(.....
+00005720: 0c01 0601 1202 0c03 0604 0c01 1201 1003  ................
+00005730: 0c01 1c01 1803 1603 1003 0e03 0c01 0c04  ................
+00005740: 0601 0601 0601 0601 0601 06fa 0409 1202  ................
+00005750: 0a02 1003 0a01 0a03 2001 1001 1001 0a01  ........ .......
+00005760: 0a03 0cff 0401 06ff 0403 1001 0a01 0a02  ................
+00005770: 0401 0eff 0403 02fd 02ff 0207 0401 0eff  ................
+00005780: 0403 02fd 02ff 0207 1a01 1a01 0a03 0e01  ................
+00005790: 1201 1a03 0801 1803 0601 12ff 0407 0801  ................
+000057a0: 0602 0401 0401 0401 0401 04fb 02ff 100a  ................
+000057b0: 0601 04ff 0604 1001 1203 0c01 0a01 0601  ................
+000057c0: 10ff 0c04 1c01 0601 12ff 0c03 0e01 1201  ................
+000057d0: 1002 1a01 0601 0eff 0a05 0801 1001 1001  ................
+000057e0: 1001 1001 1001 0601 04ff 0603 1401 1001  ................
+000057f0: 1001 1001 1001 0c01 0a02 1401 1401 0201  ................
+00005800: 0401 04ff 02ff 0405 0201 0401 06ff 02ff  ................
+00005810: 0405 0e01 0201 0401 04ff 02ff 0405 0201  ................
+00005820: 0401 0cff 02ff 0405 0201 0401 16ff 02ff  ................
+00005830: 0405 0801 0201 0401 0cff 02ff 0405 0201  ................
+00005840: 0401 16ff 02ff 0405 0a05 0201 0aff 1403  ................
+00005850: 0e01 0a01 0e03 0a01 1401 0a02 0404 0aff  ................
+00005860: 0402 08fe 0403 02fd 0404 06fc 0406 0801  ................
+00005870: 0804 0aff 0402 08fe 0403 02fd 0404 06fc  ................
+00005880: 0406 0601 0801 0801 0801 0801 0601 1803  ................
+00005890: 0e02 16ff 0402 0afe 0406 1601 0e02 0e01  ................
+000058a0: 02fe 0a06 0201 0cff 0803 0e02 0e01 02fe  ................
+000058b0: 0a04 1803 0e01 0e01 0e02 7a15 436f 756e  ..........z.Coun
+000058c0: 7465 7266 6163 7475 616c 2e61 7474 6163  terfactual.attac
+000058d0: 6b29 0972 d700 0000 72cf 0000 0072 f300  k).r....r....r..
+000058e0: 0000 72ed 0000 0072 f400 0000 72f5 0000  ..r....r....r...
+000058f0: 0072 f600 0000 72f7 0000 0072 3100 0000  .r....r....r1...
+00005900: 6309 0000 0000 0000 0000 0000 0014 0000  c...............
+00005910: 000b 0000 0043 0000 0073 be01 0000 7400  .....C...s....t.
+00005920: 8300 7d09 6700 6401 a201 7d0a 7c0a 4400  ..}.g.d...}.|.D.
+00005930: 5d0e 7d0b 7c09 a001 7c0b a101 0100 7112  ].}.|...|.....q.
+00005940: 7c01 6a02 6402 1900 6403 6b03 7242 7403  |.j.d...d.k.rBt.
+00005950: a004 6404 7c01 6a02 6402 1900 a102 0100  ..d.|.j.d.......
+00005960: 7405 a006 7407 a101 7d0c 7c00 6a08 7260  t...t...}.|.j.r`
+00005970: 7c00 6a09 a009 7c01 a101 7d0d 6e0a 7c00  |.j...|...}.n.|.
+00005980: a009 7c01 a101 7d0d 740a a00b 7c0d 6a02  ..|...}.t...|.j.
+00005990: a101 7d0e 740a 6a0c 7c0d a00d a100 6403  ..}.t.j.|.....d.
+000059a0: 6405 8d02 7d0f 6403 7c0e 740a a00e 7c0d  d...}.d.|.t...|.
+000059b0: 6a02 6402 1900 a101 7c0f 6602 3c00 7c0e  j.d.....|.f.<.|.
+000059c0: a005 a100 7d02 7c0d 7c0c 6406 3c00 740a  ....}.|.|.d.<.t.
+000059d0: 6a0c 7c02 6403 6405 8d02 6402 1900 7c0c  j.|.d.d...d...|.
+000059e0: 6407 3c00 6408 7c00 5f0f 7c00 6a10 7c01  d.<.d.|._.|.j.|.
+000059f0: 7c02 7c03 7c04 7c05 7c00 6a11 7c06 7c07  |.|.|.|.|.j.|.|.
+00005a00: 7c08 6409 8d09 5c02 7d10 7d11 7c00 6a12  |.d...\.}.}.|.j.
+00005a10: 72fe 7c00 6a13 7c0c 640a 3c00 7c00 6a0f  r.|.j.|.d.<.|.j.
+00005a20: 9001 7328 7403 a004 640b a101 0100 7414  ..s(t...d.....t.
+00005a30: 7405 a006 7c00 6a15 a101 7c0c 640c 8d02  t...|.j...|.d...
+00005a40: 7d12 7c12 5300 7c00 6a16 7c0c 640d 3c00  }.|.S.|.j.|.d.<.
+00005a50: 6900 7c0c 640e 3c00 7c10 7c0c 640e 1900  i.|.d.<.|.|.d...
+00005a60: 640f 3c00 7c00 a009 7417 a018 7c10 a101  d.<.|...t...|...
+00005a70: a101 a00d a100 a019 a100 7d13 740a 6a0c  ..........}.t.j.
+00005a80: 7c13 6403 6405 8d02 6402 1900 7c0c 640e  |.d.d...d...|.d.
+00005a90: 1900 6410 3c00 7c13 7c0c 640e 1900 6411  ..d.<.|.|.d...d.
+00005aa0: 3c00 7c11 6402 1900 7c11 6403 1900 0200  <.|.d...|.d.....
+00005ab0: 7c0c 640e 1900 6412 3c00 7c0c 640e 1900  |.d...d.<.|.d...
+00005ac0: 6413 3c00 7414 7405 a006 7c00 6a15 a101  d.<.t.t...|.j...
+00005ad0: 7c0c 640c 8d02 7d12 7c12 5300 2914 61ab  |.d...}.|.S.).a.
+00005ae0: 0600 000a 2020 2020 2020 2020 4578 706c  ....        Expl
+00005af0: 6169 6e20 696e 7374 616e 6365 2061 6e64  ain instance and
+00005b00: 2072 6574 7572 6e20 636f 756e 7465 7266   return counterf
+00005b10: 6163 7475 616c 2077 6974 6820 6d65 7461  actual with meta
+00005b20: 6461 7461 2e0a 0a20 2020 2020 2020 2050  data...        P
+00005b30: 6172 616d 6574 6572 730a 2020 2020 2020  arameters.      
+00005b40: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020    ----------.   
+00005b50: 2020 2020 2058 0a20 2020 2020 2020 2020       X.         
+00005b60: 2020 2049 6e69 7469 616c 2070 6572 7475     Initial pertu
+00005b70: 7262 6174 696f 6e0a 2020 2020 2020 2020  rbation.        
+00005b80: 590a 2020 2020 2020 2020 2020 2020 4c61  Y.            La
+00005b90: 6265 6c73 2066 6f72 2060 5860 2061 7320  bels for `X` as 
+00005ba0: 6f6e 652d 686f 742d 656e 636f 6469 6e67  one-hot-encoding
+00005bb0: 2e0a 2020 2020 2020 2020 7461 7267 6574  ..        target
+00005bc0: 5f63 6c61 7373 0a20 2020 2020 2020 2020  _class.         
+00005bd0: 2020 204c 6973 7420 7769 7468 2074 6172     List with tar
+00005be0: 6765 7420 636c 6173 7365 7320 7573 6564  get classes used
+00005bf0: 2074 6f20 6669 6e64 2063 6c6f 7365 7374   to find closest
+00005c00: 2070 726f 746f 7479 7065 2e20 4966 2060   prototype. If `
+00005c10: 604e 6f6e 6560 602c 2074 6865 206e 6561  `None``, the nea
+00005c20: 7265 7374 2070 726f 746f 7479 7065 0a20  rest prototype. 
+00005c30: 2020 2020 2020 2020 2020 2065 7863 6570             excep
+00005c40: 7420 666f 7220 7468 6520 7072 6564 6963  t for the predic
+00005c50: 7420 636c 6173 7320 6f6e 2074 6865 2069  t class on the i
+00005c60: 6e73 7461 6e63 6520 6973 2075 7365 642e  nstance is used.
+00005c70: 0a20 2020 2020 2020 206b 0a20 2020 2020  .        k.     
+00005c80: 2020 2020 2020 204e 756d 6265 7220 6f66         Number of
+00005c90: 206e 6561 7265 7374 2069 6e73 7461 6e63   nearest instanc
+00005ca0: 6573 2075 7365 6420 746f 2064 6566 696e  es used to defin
+00005cb0: 6520 7468 6520 7072 6f74 6f74 7970 6520  e the prototype 
+00005cc0: 666f 7220 6120 636c 6173 732e 2044 6566  for a class. Def
+00005cd0: 6175 6c74 7320 746f 2075 7369 6e67 2061  aults to using a
+00005ce0: 6c6c 0a20 2020 2020 2020 2020 2020 2069  ll.            i
+00005cf0: 6e73 7461 6e63 6573 2062 656c 6f6e 6769  nstances belongi
+00005d00: 6e67 2074 6f20 7468 6520 636c 6173 7320  ng to the class 
+00005d10: 6966 2061 6e20 656e 636f 6465 7220 6973  if an encoder is
+00005d20: 2075 7365 6420 616e 6420 746f 2031 2066   used and to 1 f
+00005d30: 6f72 206b 2d64 2074 7265 6573 2e0a 2020  or k-d trees..  
+00005d40: 2020 2020 2020 6b5f 7479 7065 0a20 2020        k_type.   
+00005d50: 2020 2020 2020 2020 2055 7365 2065 6974           Use eit
+00005d60: 6865 7220 7468 6520 6176 6572 6167 6520  her the average 
+00005d70: 656e 636f 6469 6e67 206f 6620 7468 6520  encoding of the 
+00005d80: 606b 6020 6e65 6172 6573 7420 696e 7374  `k` nearest inst
+00005d90: 616e 6365 7320 696e 2061 2063 6c61 7373  ances in a class
+00005da0: 2028 6060 6b5f 7479 7065 3d27 6d65 616e   (``k_type='mean
+00005db0: 2760 6029 206f 720a 2020 2020 2020 2020  '``) or.        
+00005dc0: 2020 2020 7468 6520 6b2d 6e65 6172 6573      the k-neares
+00005dd0: 7420 656e 636f 6469 6e67 2069 6e20 7468  t encoding in th
+00005de0: 6520 636c 6173 7320 2860 606b 5f74 7970  e class (``k_typ
+00005df0: 653d 2770 6f69 6e74 2760 6029 2074 6f20  e='point'``) to 
+00005e00: 6465 6669 6e65 2074 6865 2070 726f 746f  define the proto
+00005e10: 7479 7065 206f 6620 7468 6174 2063 6c61  type of that cla
+00005e20: 7373 2e0a 2020 2020 2020 2020 2020 2020  ss..            
+00005e30: 4f6e 6c79 2072 656c 6576 616e 7420 6966  Only relevant if
+00005e40: 2061 6e20 656e 636f 6465 7220 6973 2075   an encoder is u
+00005e50: 7365 6420 746f 2064 6566 696e 6520 7468  sed to define th
+00005e60: 6520 7072 6f74 6f74 7970 6573 2e0a 2020  e prototypes..  
+00005e70: 2020 2020 2020 7468 7265 7368 6f6c 640a        threshold.
+00005e80: 2020 2020 2020 2020 2020 2020 5468 7265              Thre
+00005e90: 7368 6f6c 6420 6c65 7665 6c20 666f 7220  shold level for 
+00005ea0: 7468 6520 7261 7469 6f20 6265 7477 6565  the ratio betwee
+00005eb0: 6e20 7468 6520 6469 7374 616e 6365 206f  n the distance o
+00005ec0: 6620 7468 6520 636f 756e 7465 7266 6163  f the counterfac
+00005ed0: 7475 616c 2074 6f20 7468 6520 7072 6f74  tual to the prot
+00005ee0: 6f74 7970 6520 6f66 2074 6865 0a20 2020  otype of the.   
+00005ef0: 2020 2020 2020 2020 2070 7265 6469 6374           predict
+00005f00: 6564 2063 6c61 7373 2066 6f72 2074 6865  ed class for the
+00005f10: 206f 7269 6769 6e61 6c20 696e 7374 616e   original instan
+00005f20: 6365 206f 7665 7220 7468 6520 6469 7374  ce over the dist
+00005f30: 616e 6365 2074 6f20 7468 6520 7072 6f74  ance to the prot
+00005f40: 6f74 7970 6520 6f66 2074 6865 2070 7265  otype of the pre
+00005f50: 6469 6374 6564 2063 6c61 7373 0a20 2020  dicted class.   
+00005f60: 2020 2020 2020 2020 2066 6f72 2074 6865           for the
+00005f70: 2063 6f75 6e74 6572 6661 6374 7561 6c2e   counterfactual.
+00005f80: 2049 6620 7468 6520 7472 7573 7420 7363   If the trust sc
+00005f90: 6f72 6520 6973 2062 656c 6f77 2074 6865  ore is below the
+00005fa0: 2074 6872 6573 686f 6c64 2c20 7468 6520   threshold, the 
+00005fb0: 7072 6f70 6f73 6564 2063 6f75 6e74 6572  proposed counter
+00005fc0: 6661 6374 7561 6c20 646f 6573 0a20 2020  factual does.   
+00005fd0: 2020 2020 2020 2020 206e 6f74 206d 6565           not mee
+00005fe0: 7420 7468 6520 7265 7175 6972 656d 656e  t the requiremen
+00005ff0: 7473 2e0a 2020 2020 2020 2020 7665 7262  ts..        verb
+00006000: 6f73 650a 2020 2020 2020 2020 2020 2020  ose.            
+00006010: 5072 696e 7420 696e 7465 726d 6564 6961  Print intermedia
+00006020: 7465 2072 6573 756c 7473 206f 6620 6f70  te results of op
+00006030: 7469 6d69 7a61 7469 6f6e 2069 6620 6060  timization if ``
+00006040: 5472 7565 6060 2e0a 2020 2020 2020 2020  True``..        
+00006050: 7072 696e 745f 6576 6572 790a 2020 2020  print_every.    
+00006060: 2020 2020 2020 2020 5072 696e 7420 6672          Print fr
+00006070: 6571 7565 6e63 7920 6966 2076 6572 626f  equency if verbo
+00006080: 7365 2069 7320 6060 5472 7565 6060 2e0a  se is ``True``..
+00006090: 2020 2020 2020 2020 6c6f 675f 6576 6572          log_ever
+000060a0: 790a 2020 2020 2020 2020 2020 2020 6074  y.            `t
+000060b0: 656e 736f 7262 6f61 7264 6020 6c6f 6720  ensorboard` log 
+000060c0: 6672 6571 7565 6e63 7920 6966 2077 7269  frequency if wri
+000060d0: 7465 2064 6972 6563 746f 7279 2069 7320  te directory is 
+000060e0: 7370 6563 6966 6965 640a 0a20 2020 2020  specified..     
+000060f0: 2020 2052 6574 7572 6e73 0a20 2020 2020     Returns.     
+00006100: 2020 202d 2d2d 2d2d 2d2d 0a20 2020 2020     -------.     
+00006110: 2020 2065 7870 6c61 6e61 7469 6f6e 0a20     explanation. 
+00006120: 2020 2020 2020 2020 2020 2060 4578 706c             `Expl
+00006130: 616e 6174 696f 6e60 206f 626a 6563 7420  anation` object 
+00006140: 636f 6e74 6169 6e69 6e67 2074 6865 2063  containing the c
+00006150: 6f75 6e74 6572 6661 6374 7561 6c20 7769  ounterfactual wi
+00006160: 7468 2061 6464 6974 696f 6e61 6c20 6d65  th additional me
+00006170: 7461 6461 7461 2061 7320 6174 7472 6962  tadata as attrib
+00006180: 7574 6573 2e0a 2020 2020 2020 2020 2903  utes..        ).
+00006190: 7234 0000 0072 d700 0000 72cf 0000 0072  r4...r....r....r
+000061a0: 0100 0000 721a 0000 007a 5943 7572 7265  ....r....zYCurre
+000061b0: 6e74 6c79 206f 6e6c 7920 7369 6e67 6c65  ntly only single
+000061c0: 2069 6e73 7461 6e63 6520 6578 706c 616e   instance explan
+000061d0: 6174 696f 6e73 2073 7570 706f 7274 6564  ations supported
+000061e0: 2028 6669 7273 7420 6469 6d20 3d20 3129   (first dim = 1)
+000061f0: 2c20 6275 7420 6669 7273 7420 6469 6d20  , but first dim 
+00006200: 3d20 2573 7259 0000 00da 0a6f 7269 675f  = %srY.....orig_
+00006210: 7072 6f62 6172 eb00 0000 4629 0872 cf00  probar....F).r..
+00006220: 0000 72f3 0000 0072 ed00 0000 72f4 0000  ..r....r....r...
+00006230: 0072 3000 0000 72f5 0000 0072 f600 0000  .r0...r....r....
+00006240: 72f7 0000 0072 0801 0000 7a18 4e6f 2063  r....r....z.No c
+00006250: 6f75 6e74 6572 6661 6374 7561 6c20 666f  ounterfactual fo
+00006260: 756e 6421 2902 7232 0000 00da 0464 6174  und!).r2.....dat
+00006270: 61da 0361 6c6c da02 6366 72d7 0000 00da  a..all..cfr.....
+00006280: 0563 6c61 7373 72d9 0000 0072 1801 0000  .classr....r....
+00006290: 7217 0100 0029 1a72 6c00 0000 726d 0000  r....).rl...rm..
+000062a0: 0072 1d00 0000 727b 0000 0072 7c00 0000  .r....r{...r|...
+000062b0: 7269 0000 0072 6a00 0000 7208 0000 0072  ri...rj...r....r
+000062c0: 7600 0000 721b 0000 0072 3f00 0000 7277  v...r....r?...rw
+000062d0: 0000 0072 fb00 0000 72e2 0000 0072 9a00  ...r....r....r..
+000062e0: 0000 7213 0100 0072 1e01 0000 7230 0000  ..r....r....r0..
+000062f0: 0072 3b00 0000 7208 0100 0072 0b00 0000  .r;...r....r....
+00006300: 7232 0000 0072 0901 0000 7279 0000 0072  r2...r....ry...r
+00006310: e100 0000 72e3 0000 0029 1472 3400 0000  ....r....).r4...
+00006320: 72d7 0000 0072 cf00 0000 72f3 0000 0072  r....r....r....r
+00006330: ed00 0000 72f4 0000 0072 f500 0000 72f6  ....r....r....r.
+00006340: 0000 0072 f700 0000 7236 0000 0072 b700  ...r....r6...r..
+00006350: 0000 72b8 0000 0072 2001 0000 5a07 595f  ..r....r ...Z.Y_
+00006360: 7072 6f62 615a 0559 5f6f 6865 721d 0100  probaZ.Y_oher...
+00006370: 0072 1301 0000 72e7 0000 00da 0b65 7870  .r....r......exp
+00006380: 6c61 6e61 7469 6f6e 5a06 595f 7065 7274  lanationZ.Y_pert
+00006390: 7244 0000 0072 4400 0000 7245 0000 00da  rD...rD...rE....
+000063a0: 0765 7870 6c61 696e 0b04 0000 735c 0000  .explain....s\..
+000063b0: 0000 3106 0108 0108 010c 020e 0104 0102  ..1.............
+000063c0: 0208 fd04 070a 0306 010e 020a 010c 0112  ................
+000063d0: 0118 0108 0108 0316 0306 0104 0102 0102  ................
+000063e0: 0102 0102 0102 0104 0102 0102 0102 f70a  ................
+000063f0: 0c06 010a 0308 010a 0314 0104 020a 0108  ................
+00006400: 010c 0118 011a 010c 0122 0314 027a 1643  ........."...z.C
+00006410: 6f75 6e74 6572 6661 6374 7561 6c2e 6578  ounterfactual.ex
+00006420: 706c 6169 6e29 1372 0f00 0000 7210 0000  plain).r....r...
+00006430: 0072 1100 0000 720f 0000 004e 4e72 0f00  .r....r....NNr..
+00006440: 0000 4672 1300 0000 7214 0000 0072 1500  ..Fr....r....r..
+00006450: 0000 7216 0000 0072 1700 0000 7219 0000  ..r....r....r...
+00006460: 0072 1a00 0000 4e4e 4e46 2901 72e9 0000  .r....NNNF).r...
+00006470: 0029 074e 4e72 c700 0000 720f 0000 0046  .).NNr....r....F
+00006480: 72f2 0000 0072 f200 0000 2907 4e4e 4e72  r....r....).NNNr
+00006490: c700 0000 720f 0000 0072 f200 0000 72f2  ....r....r....r.
+000064a0: 0000 0029 1eda 085f 5f6e 616d 655f 5fda  ...)...__name__.
+000064b0: 0a5f 5f6d 6f64 756c 655f 5fda 0c5f 5f71  .__module__..__q
+000064c0: 7561 6c6e 616d 655f 5f72 0600 0000 7203  ualname__r....r.
+000064d0: 0000 0072 3f00 0000 7201 0100 0072 6f00  ...r?...r....ro.
+000064e0: 0000 7270 0000 0072 7100 0000 7281 0000  ..rp...rq...r...
+000064f0: 0072 3e00 0000 7205 0000 0072 0400 0000  .r>...r....r....
+00006500: 7202 0100 0072 f900 0000 da03 7374 7272  r....r......strr
+00006510: 7500 0000 7268 0000 0072 4100 0000 da04  u...rh...rA.....
+00006520: 6469 6374 72ce 0000 0072 d600 0000 72e8  dictr....r....r.
+00006530: 0000 0072 f100 0000 7299 0000 0072 1e01  ...r....r....r..
+00006540: 0000 720b 0000 0072 2501 0000 da0d 5f5f  ..r....r%.....__
+00006550: 636c 6173 7363 656c 6c5f 5f72 4400 0000  classcell__rD...
+00006560: 7244 0000 0072 bf00 0000 7245 0000 0072  rD...r....rE...r
+00006570: 0e00 0000 1600 0000 73d2 0000 0008 0700  ........s.......
+00006580: 0100 0100 0400 0100 0100 0100 0100 0100  ................
+00006590: 0100 0100 0100 0100 0100 0100 0100 0100  ................
+000065a0: 0100 0100 e602 021c 011c 0102 0102 0102  ................
+000065b0: 011e 0402 010a 010a 0102 0102 0102 0102  ................
+000065c0: 0102 0102 0102 0102 0102 0106 0106 0108  ................
+000065d0: 0102 0102 e510 7f00 7f00 7f00 4208 0108  ............B...
+000065e0: 0102 fc02 0204 0104 0106 0102 fb0c 2918  ..............).
+000065f0: 1a0a 0104 fe0c 4500 ff02 010a 0102 fe0c  ......E.........
+00006600: 2900 0100 0100 0100 0100 0100 0100 f602  )...............
+00006610: 0204 0104 0106 0106 0102 0102 0102 0102  ................
+00006620: 0102 0118 f50c 7f00 7f00 7f00 1200 0100  ................
+00006630: 0100 0100 0100 0100 0100 f602 0304 0108  ................
+00006640: 0106 0106 0102 0102 0102 0102 0102 f572  ...............r
+00006650: 0e00 0000 6302 0000 0000 0000 0000 0000  ....c...........
+00006660: 0003 0000 0008 0000 0043 0000 0073 3c00  .........C...s<.
+00006670: 0000 7400 7c01 6401 8302 8f1e 7d02 7401  ..t.|.d.....}.t.
+00006680: a002 7c00 7c02 6402 a103 0100 5700 6400  ..|.|.d.....W.d.
+00006690: 0400 0400 8303 0100 6e10 3100 732e 3000  ........n.1.s.0.
+000066a0: 0100 0100 0100 5900 0100 6400 5300 2903  ......Y...d.S.).
+000066b0: 4eda 0277 6272 3300 0000 2903 da04 6f70  N..wbr3...)...op
+000066c0: 656e da06 7069 636b 6c65 da04 6475 6d70  en..pickle..dump
+000066d0: 2903 da03 6f62 6ada 0866 696c 656e 616d  )...obj..filenam
+000066e0: 65da 046f 7574 7072 4400 0000 7244 0000  e..outprD...rD..
+000066f0: 0072 4500 0000 da0b 7361 7665 5f6f 626a  .rE.....save_obj
+00006700: 6563 7480 0400 0073 0400 0000 0001 0c01  ect....s........
+00006710: 7233 0100 0063 0100 0000 0000 0000 0000  r3...c..........
+00006720: 0000 0200 0000 0800 0000 4300 0000 7338  ..........C...s8
+00006730: 0000 0074 007c 0064 0183 028f 1a7d 0174  ...t.|.d.....}.t
+00006740: 01a0 027c 01a1 0157 0002 0064 0004 0004  ...|...W...d....
+00006750: 0083 0301 0053 0031 0073 2a30 0001 0001  .....S.1.s*0....
+00006760: 0001 0059 0001 0064 0053 0029 024e da02  ...Y...d.S.).N..
+00006770: 7262 2903 722d 0100 0072 2e01 0000 da04  rb).r-...r......
+00006780: 6c6f 6164 2902 7231 0100 0072 3201 0000  load).r1...r2...
+00006790: 7244 0000 0072 4400 0000 7245 0000 0072  rD...rD...rE...r
+000067a0: c800 0000 8504 0000 7304 0000 0000 010c  ........s.......
+000067b0: 0172 c800 0000 2925 da02 6f73 7269 0000  .r....)%..osri..
+000067c0: 00da 076c 6f67 6769 6e67 720f 0100 00da  ...loggingr.....
+000067d0: 075f 7069 636b 6c65 722e 0100 00da 0674  ._pickler......t
+000067e0: 7970 696e 6772 0200 0000 7203 0000 0072  ypingr....r....r
+000067f0: 0400 0000 7205 0000 0072 0600 0000 72e3  ....r....r....r.
+00006800: 0000 0072 3f00 0000 5a14 7465 6e73 6f72  ...r?...Z.tensor
+00006810: 666c 6f77 2e63 6f6d 7061 742e 7631 7272  flow.compat.v1rr
+00006820: 0000 0072 7300 0000 726f 0000 005a 0c61  ...rs...ro...Z.a
+00006830: 7069 2e64 6566 6175 6c74 7372 0800 0000  pi.defaultsr....
+00006840: 7209 0000 005a 0e61 7069 2e69 6e74 6572  r....Z.api.inter
+00006850: 6661 6365 7372 0a00 0000 720b 0000 0072  facesr....r....r
+00006860: 0c00 0000 5a0f 7574 696c 732e 6772 6164  ....Z.utils.grad
+00006870: 6965 6e74 7372 0d00 0000 7279 0000 00da  ientsr....ry....
+00006880: 0967 6574 4c6f 6767 6572 7226 0100 0072  .getLoggerr&...r
+00006890: 7b00 0000 5a0d 7365 745f 7665 7262 6f73  {...Z.set_verbos
+000068a0: 6974 79da 0545 5252 4f52 5a17 6469 7361  ity..ERRORZ.disa
+000068b0: 626c 655f 6561 6765 725f 6578 6563 7574  ble_eager_execut
+000068c0: 696f 6e72 0e00 0000 7233 0100 0072 c800  ionr....r3...r..
+000068d0: 0000 7244 0000 0072 4400 0000 7244 0000  ..rD...rD...rD..
+000068e0: 0072 4500 0000 da08 3c6d 6f64 756c 653e  .rE.....<module>
+000068f0: 0100 0000 7332 0000 0008 0108 0108 0108  ....s2..........
+00006900: 0108 011c 0108 0112 0210 0114 010c 0108  ................
+00006910: 020a 0110 030c 0312 7f00 7f00 7f00 7f00  ................
+00006920: 7f00 7f00 7f00 7f00 7208 05              ........r..
```

### Comparing `morpheus_spatial-0.3.0/src/morpheus/counterfactual/__pycache__/generate.cpython-39.pyc` & `morpheus_spatial-0.4.0/src/morpheus/counterfactual/__pycache__/generate.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Sun Mar 24 21:54:17 2024 UTC, .py size: 12251 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 9% similar despite different names*

```diff
@@ -1,658 +1,652 @@
-00000000: 610d 0d0a 0000 0000 09a1 0066 db2f 0000  a..........f./..
+00000000: 610d 0d0a 0000 0000 f38b 1066 ba2f 0000  a..........f./..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0011 0000 0040 0000 0073 6601 0000 6400  .....@...sf...d.
+00000020: 0011 0000 0040 0000 0073 5a01 0000 6400  .....@...sZ...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a03 6400 6401 6c04 5a05 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6401 6c06 5a07 6400 6402 6c08 6d09 5a09  d.l.Z.d.d.l.m.Z.
 00000060: 0100 6400 6401 6c0a 5a0a 6400 6403 6c0b  ..d.d.l.Z.d.d.l.
-00000070: 6d0b 5a0b 0100 6400 6404 6c0c 6d0d 5a0d  m.Z...d.d.l.m.Z.
-00000080: 0100 6405 6406 6c0e 6d0f 5a0f 0100 6407  ..d.d.l.m.Z...d.
-00000090: 6408 6c10 6d11 5a11 0100 6405 6409 6c12  d.l.m.Z...d.d.l.
-000000a0: 6d13 5a13 0100 6405 640a 6c14 6d15 5a15  m.Z...d.d.l.m.Z.
-000000b0: 6d16 5a16 6d17 5a17 6d18 5a18 0100 650a  m.Z.m.Z.m.Z...e.
-000000c0: 6a19 640b 650a 6a1a 640c 8d02 5a1b 6423  j.d.e.j.d...Z.d#
-000000d0: 650f 651c 650a 6a1d 6a1e 651f 6520 6507  e.e.e.j.j.e.e e.
-000000e0: 6a21 6522 6523 6523 651c 6523 6524 6509  j!e"e#e#e.e#e$e.
-000000f0: 6520 1900 640f 9c0d 6410 6411 8405 5a25  e ..d...d.d...Z%
-00000100: 6424 6505 6a26 6505 6a26 651c 650a 6a1d  d$e.j&e.j&e.e.j.
-00000110: 6a1e 651f 651f 6505 6a26 6505 6a26 6523  j.e.e.e.j&e.j&e#
-00000120: 6524 6520 6523 651c 6522 6401 6412 9c0f  e$e e#e.e"d.d...
-00000130: 6413 6414 8405 5a27 6425 6523 650a 6a1d  d.d...Z'd%e#e.j.
-00000140: 6a1e 651f 651f 6509 6520 1900 6415 9c05  j.e.e.e.e ..d...
-00000150: 6416 6417 8405 5a28 6418 6419 8400 5a29  d.d...Z(d.d...Z)
-00000160: 641a 641b 8400 5a2a 641c 641d 8400 5a2b  d.d...Z*d.d...Z+
-00000170: 6426 650a 6a2c 652d 650a 6a2c 641e 9c03  d&e.j,e-e.j,d...
-00000180: 641f 6420 8405 5a2e 6421 6422 8400 5a2f  d.d ..Z.d!d"..Z/
-00000190: 6401 5300 2927 e900 0000 004e 2901 da08  d.S.)'.....N)...
-000001a0: 4f70 7469 6f6e 616c 2901 da04 7471 646d  Optional)...tqdm
-000001b0: 2901 da04 506f 6f6c e902 0000 0029 01da  )...Pool.....)..
-000001c0: 0e53 7061 7469 616c 4461 7461 7365 74e9  .SpatialDataset.
-000001d0: 0100 0000 2901 da0e 436f 756e 7465 7266  ....)...Counterf
-000001e0: 6163 7475 616c 2901 da0a 5472 7573 7453  actual)...TrustS
-000001f0: 636f 7265 2904 da06 5370 6c69 7473 da07  core)...Splits..
-00000200: 436f 6c4e 616d 65da 1144 6566 6175 6c74  ColName..Default
-00000210: 466f 6c64 6572 4e61 6d65 da0f 4465 6661  FolderName..Defa
-00000220: 756c 7446 696c 654e 616d 6567 2342 920c  ultFileNameg#B..
-00000230: a19c c73b a901 da05 6474 7970 65e7 0000  ...;....dtype...
-00000240: 0000 0000 e03f 4629 0dda 0764 6174 6173  .....?F)...datas
-00000250: 6574 da0c 7461 7267 6574 5f63 6c61 7373  et..target_class
-00000260: da05 6d6f 6465 6cda 1263 6861 6e6e 656c  ..model..channel
-00000270: 5f74 6f5f 7065 7274 7572 62da 136f 7074  _to_perturb..opt
-00000280: 696d 697a 6174 696f 6e5f 7061 7261 6d73  imization_params
-00000290: da06 696d 6167 6573 da09 7468 7265 7368  ..images..thresh
-000002a0: 6f6c 64da 0b6b 6474 7265 655f 7061 7468  old..kdtree_path
-000002b0: da08 7361 7665 5f64 6972 da0b 6e75 6d5f  ..save_dir..num_
-000002c0: 776f 726b 6572 73da 0a74 7261 696e 5f64  workers..train_d
-000002d0: 6174 61da 0776 6572 626f 7365 da11 7472  ata..verbose..tr
-000002e0: 7573 7473 636f 7265 5f6b 7761 7267 7363  ustscore_kwargsc
-000002f0: 0d00 0000 0000 0000 0000 0000 1e00 0000  ................
-00000300: 1100 0000 0300 0000 7302 0200 0074 007c  ........s....t.|
-00000310: 0583 017d 0d74 0174 026a 03a0 047c 006a  ...}.t.t.j...|.j
-00000320: 0564 01a1 0283 018f 2a7d 0e74 06a0 077c  .d......*}.t...|
-00000330: 0ea1 017d 0f7c 0f64 0219 007d 107c 0f64  ...}.|.d...}.|.d
-00000340: 0319 007d 1157 0064 0404 0004 0083 0301  ...}.W.d........
-00000350: 006e 1031 0073 4c30 0001 0001 0001 0059  .n.1.sL0.......Y
-00000360: 0001 007c 0a64 0475 0072 7274 026a 03a0  ...|.d.u.rrt.j..
-00000370: 047c 006a 0574 086a 096a 0aa1 027d 0a7c  .|.j.t.j.j...}.|
-00000380: 0764 0475 0072 8e74 026a 03a0 047c 006a  .d.u.r.t.j...|.j
-00000390: 0b74 0c6a 0d6a 0aa1 027d 077c 0564 0475  .t.j.j...}.|.d.u
-000003a0: 0072 9c7c 006a 0e7d 057c 0864 0475 0072  .r.|.j.}.|.d.u.r
-000003b0: b874 026a 03a0 047c 006a 0b74 0f6a 106a  .t.j...|.j.t.j.j
-000003c0: 0aa1 027d 0874 026a 117c 0864 0564 068d  ...}.t.j.|.d.d..
-000003d0: 0201 007c 087c 005f 1274 026a 03a0 137c  ...|.|._.t.j...|
-000003e0: 07a1 0173 f274 147c 077c 0a7c 027c 107c  ...s.t.|.|.|.|.|
-000003f0: 117c 0c83 0601 0074 1564 0783 0101 0067  .|.....t.d.....g
-00000400: 007d 1274 167c 0d83 0144 005d 847d 137c  .}.t.|...D.].}.|
-00000410: 006a 177c 056a 187c 1319 0074 196a 1a6a  .j.|.j.|...t.j.j
-00000420: 0a19 007c 056a 187c 1319 007c 006a 1b19  ...|.j.|...|.j..
-00000430: 007c 056a 187c 1319 0074 196a 1c6a 0a19  .|.j.|...t.j.j..
-00000440: 0064 088d 037d 1474 1da0 1e7c 14a1 015c  .d...}.t...|...\
-00000450: 027d 157d 167c 006a 0e6a 187c 1619 007c  .}.}.|.j.j.|...|
-00000460: 006a 1b19 007d 177c 12a0 1f7c 157c 177c  .j...}.|...|.|.|
-00000470: 017c 027c 006a 207c 037c 107c 117c 077c  .|.|.j |.|.|.|.|
-00000480: 0b7c 047c 087c 167c 0666 0ea1 0101 0071  .|.|.|.|.f.....q
-00000490: fe7c 0964 096b 0490 0172 9264 056e 0264  .|.d.k...r.d.n.d
-000004a0: 0a7d 187c 1890 0172 e264 0b64 0c6c 216d  .}.|...r.d.d.l!m
-000004b0: 227d 1901 0064 0b64 046c 237d 1a7c 1964  "}...d.d.l#}.|.d
-000004c0: 0d64 0e84 0083 0189 0087 0066 0164 0f64  .d.........f.d.d
-000004d0: 1084 087c 1244 0083 017d 1b7c 1a6a 247c  ...|.D...}.|.j$|
-000004e0: 1b64 117c 0964 129c 028e 017d 1c6e 1c74  .d.|.d.....}.n.t
-000004f0: 257c 127c 0d64 138d 0244 005d 0e7d 1d74  %|.|.d...D.].}.t
-00000500: 267c 1d8e 0001 0090 0171 ee64 0453 0029  &|.......q.d.S.)
-00000510: 1461 da03 0000 0a20 2020 2047 656e 6572  .a.....    Gener
-00000520: 6174 6520 636f 756e 7465 7266 6163 7475  ate counterfactu
-00000530: 616c 7320 666f 7220 7468 6520 6461 7461  als for the data
-00000540: 7365 742e 0a0a 2020 2020 4172 6773 3a0a  set...    Args:.
-00000550: 2020 2020 2020 2020 6461 7461 7365 7420          dataset 
-00000560: 2853 7061 7469 616c 4461 7461 7365 7429  (SpatialDataset)
-00000570: 3a20 4461 7461 7365 7420 746f 2067 656e  : Dataset to gen
-00000580: 6572 6174 6520 636f 756e 7465 7266 6163  erate counterfac
-00000590: 7475 616c 7320 666f 722e 0a20 2020 2020  tuals for..     
-000005a0: 2020 2074 6172 6765 745f 636c 6173 7320     target_class 
-000005b0: 2869 6e74 293a 2054 6172 6765 7420 636c  (int): Target cl
-000005c0: 6173 7320 666f 7220 7468 6520 636f 756e  ass for the coun
-000005d0: 7465 7266 6163 7475 616c 732e 0a20 2020  terfactuals..   
-000005e0: 2020 2020 206d 6f64 656c 2028 746f 7263       model (torc
-000005f0: 682e 6e6e 2e4d 6f64 756c 6529 3a20 4d6f  h.nn.Module): Mo
-00000600: 6465 6c20 746f 2067 656e 6572 6174 6520  del to generate 
-00000610: 636f 756e 7465 7266 6163 7475 616c 7320  counterfactuals 
-00000620: 666f 722e 0a20 2020 2020 2020 2063 6861  for..        cha
-00000630: 6e6e 656c 5f74 6f5f 7065 7274 7572 6220  nnel_to_perturb 
-00000640: 286c 6973 7429 3a20 4c69 7374 206f 6620  (list): List of 
-00000650: 6368 616e 6e65 6c73 2074 6f20 7065 7274  channels to pert
-00000660: 7572 622e 0a20 2020 2020 2020 206f 7074  urb..        opt
-00000670: 696d 697a 6174 696f 6e5f 7061 7261 6d73  imization_params
-00000680: 2028 6469 6374 293a 2044 6963 7469 6f6e   (dict): Diction
-00000690: 6172 7920 636f 6e74 6169 6e69 6e67 2074  ary containing t
-000006a0: 6865 2070 6172 616d 6574 6572 7320 666f  he parameters fo
-000006b0: 7220 7468 6520 6f70 7469 6d69 7a61 7469  r the optimizati
-000006c0: 6f6e 2e0a 2020 2020 2020 2020 696d 6167  on..        imag
-000006d0: 6573 2028 7064 2e44 6174 6146 7261 6d65  es (pd.DataFrame
-000006e0: 2c20 6f70 7469 6f6e 616c 293a 2049 6d61  , optional): Ima
-000006f0: 6765 7320 746f 2067 656e 6572 6174 6520  ges to generate 
-00000700: 636f 756e 7465 7266 6163 7475 616c 7320  counterfactuals 
-00000710: 666f 722e 2044 6566 6175 6c74 7320 746f  for. Defaults to
-00000720: 204e 6f6e 652e 0a20 2020 2020 2020 2074   None..        t
-00000730: 6872 6573 686f 6c64 2028 666c 6f61 742c  hreshold (float,
-00000740: 206f 7074 696f 6e61 6c29 3a20 5468 7265   optional): Thre
-00000750: 7368 6f6c 6420 666f 7220 7468 6520 7072  shold for the pr
-00000760: 6564 6963 7469 6f6e 2070 726f 6261 6269  ediction probabi
-00000770: 6c69 7479 2e20 4465 6661 756c 7473 2074  lity. Defaults t
-00000780: 6f20 302e 352e 0a20 2020 2020 2020 206b  o 0.5..        k
-00000790: 6474 7265 655f 7061 7468 2028 7374 722c  dtree_path (str,
-000007a0: 206f 7074 696f 6e61 6c29 3a20 5061 7468   optional): Path
-000007b0: 2074 6f20 7468 6520 6b64 7472 6565 2066   to the kdtree f
-000007c0: 696c 652e 2044 6566 6175 6c74 7320 746f  ile. Defaults to
-000007d0: 204e 6f6e 652e 0a20 2020 2020 2020 2073   None..        s
-000007e0: 6176 655f 6469 7220 2873 7472 2c20 6f70  ave_dir (str, op
-000007f0: 7469 6f6e 616c 293a 2044 6972 6563 746f  tional): Directo
-00000800: 7279 2077 6865 7265 206f 7574 7075 7420  ry where output 
-00000810: 7769 6c6c 2062 6520 7361 7665 642e 2044  will be saved. D
-00000820: 6566 6175 6c74 7320 746f 204e 6f6e 652e  efaults to None.
-00000830: 0a20 2020 2020 2020 206e 756d 5f77 6f72  .        num_wor
-00000840: 6b65 7273 2028 626f 6f6c 2c20 6f70 7469  kers (bool, opti
-00000850: 6f6e 616c 293a 204e 756d 6265 7220 6f66  onal): Number of
-00000860: 2077 6f72 6b65 7273 2074 6f20 7573 6520   workers to use 
-00000870: 666f 7220 7061 7261 6c6c 656c 2070 726f  for parallel pro
-00000880: 6365 7373 696e 672e 2044 6566 6175 6c74  cessing. Default
-00000890: 7320 746f 204e 6f6e 652e 0a20 2020 2020  s to None..     
-000008a0: 2020 2074 7261 696e 5f64 6174 6120 2873     train_data (s
-000008b0: 7472 2c20 6f70 7469 6f6e 616c 293a 2050  tr, optional): P
-000008c0: 6174 6820 746f 2074 6865 2074 7261 696e  ath to the train
-000008d0: 696e 6720 6461 7461 2e20 4465 6661 756c  ing data. Defaul
-000008e0: 7473 2074 6f20 4e6f 6e65 2e0a 2020 2020  ts to None..    
-000008f0: 7a19 6e6f 726d 616c 697a 6174 696f 6e5f  z.normalization_
-00000900: 7061 7261 6d73 2e6a 736f 6eda 046d 6561  params.json..mea
-00000910: 6eda 0573 7464 6576 4e54 a901 da08 6578  n..stdevNT....ex
-00000920: 6973 745f 6f6b 7a0c 6b64 7472 6565 2073  ist_okz.kdtree s
-00000930: 6176 6564 2903 da08 7061 7463 685f 6964  aved)...patch_id
-00000940: da05 6c61 6265 6cda 0573 706c 6974 7207  ..label..splitr.
-00000950: 0000 0046 7201 0000 0029 01da 0764 656c  ...Fr....)...del
-00000960: 6179 6564 6301 0000 0000 0000 0000 0000  ayedc...........
-00000970: 0001 0000 0002 0000 0053 0000 0073 0800  .........S...s..
-00000980: 0000 7400 7c00 8e00 5300 a901 4e29 01da  ..t.|...S...N)..
-00000990: 0f67 656e 6572 6174 655f 6f6e 655f 6366  .generate_one_cf
-000009a0: 2901 da04 6172 6773 a900 7229 0000 00fa  )...args..r)....
-000009b0: 562f 6365 6e74 7261 6c2f 686f 6d65 2f7a  V/central/home/z
-000009c0: 7761 6e67 322f 6d6f 7270 6865 7573 2d73  wang2/morpheus-s
-000009d0: 7061 7469 616c 2f6d 6f72 7068 6575 732f  patial/morpheus/
-000009e0: 7372 632f 6d6f 7270 6865 7573 2f63 6f75  src/morpheus/cou
-000009f0: 6e74 6572 6661 6374 7561 6c2f 6765 6e65  nterfactual/gene
-00000a00: 7261 7465 2e70 79da 1767 656e 6572 6174  rate.py..generat
-00000a10: 655f 6f6e 655f 6366 5f64 656c 6179 6564  e_one_cf_delayed
-00000a20: 7d00 0000 7302 0000 0000 027a 3367 6574  }...s......z3get
-00000a30: 5f63 6f75 6e74 6572 6661 6374 7561 6c2e  _counterfactual.
-00000a40: 3c6c 6f63 616c 733e 2e67 656e 6572 6174  <locals>.generat
-00000a50: 655f 6f6e 655f 6366 5f64 656c 6179 6564  e_one_cf_delayed
-00000a60: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
-00000a70: 0004 0000 0013 0000 0073 1400 0000 6700  .........s....g.
-00000a80: 7c00 5d0c 7d01 8800 7c01 8301 9102 7104  |.].}...|.....q.
-00000a90: 5300 7229 0000 0072 2900 0000 2902 da02  S.r)...r)...)...
-00000aa0: 2e30 7228 0000 00a9 0172 2b00 0000 7229  .0r(.....r+...r)
-00000ab0: 0000 0072 2a00 0000 da0a 3c6c 6973 7463  ...r*.....<listc
-00000ac0: 6f6d 703e 8100 0000 f300 0000 007a 2667  omp>.........z&g
-00000ad0: 6574 5f63 6f75 6e74 6572 6661 6374 7561  et_counterfactua
-00000ae0: 6c2e 3c6c 6f63 616c 733e 2e3c 6c69 7374  l.<locals>.<list
-00000af0: 636f 6d70 3eda 0970 726f 6365 7373 6573  comp>..processes
-00000b00: 2902 da09 7363 6865 6475 6c65 7272 1a00  )...schedulerr..
-00000b10: 0000 2901 da05 746f 7461 6c29 27da 036c  ..)...total)'..l
-00000b20: 656e da04 6f70 656e da02 6f73 da04 7061  en..open..os..pa
-00000b30: 7468 da04 6a6f 696e da09 7370 6c69 745f  th..join..split_
-00000b40: 6469 72da 046a 736f 6eda 046c 6f61 6472  dir..json..loadr
-00000b50: 0a00 0000 da05 7472 6169 6eda 0576 616c  ......train..val
-00000b60: 7565 da08 726f 6f74 5f64 6972 720d 0000  ue..root_dirr...
-00000b70: 00da 066b 6474 7265 65da 086d 6574 6164  ...kdtree..metad
-00000b80: 6174 6172 0c00 0000 da0e 636f 756e 7465  atar......counte
-00000b90: 7266 6163 7475 616c da08 6d61 6b65 6469  rfactual..makedi
-00000ba0: 7273 da06 6366 5f64 6972 da06 6578 6973  rs..cf_dir..exis
-00000bb0: 7473 da0c 6275 696c 645f 6b64 7472 6565  ts..build_kdtree
-00000bc0: da05 7072 696e 74da 0572 616e 6765 da13  ..print..range..
-00000bd0: 6765 6e65 7261 7465 5f70 6174 6368 5f70  generate_patch_p
-00000be0: 6174 68da 0469 6c6f 6372 0b00 0000 7222  ath..ilocr....r"
-00000bf0: 0000 00da 0a6c 6162 656c 5f6e 616d 65da  .....label_name.
-00000c00: 0673 706c 6974 7372 0600 0000 da11 6c6f  .splitsr......lo
-00000c10: 6164 5f73 696e 676c 655f 696d 6167 65da  ad_single_image.
-00000c20: 0661 7070 656e 64da 0d63 6861 6e6e 656c  .append..channel
-00000c30: 5f6e 616d 6573 da04 6461 736b 7225 0000  _names..daskr%..
-00000c40: 00da 1464 6173 6b2e 6d75 6c74 6970 726f  ...dask.multipro
-00000c50: 6365 7373 696e 67da 0763 6f6d 7075 7465  cessing..compute
-00000c60: 7203 0000 0072 2700 0000 291e 7211 0000  r....r'...).r...
-00000c70: 0072 1200 0000 7213 0000 0072 1400 0000  .r....r....r....
-00000c80: 7215 0000 0072 1600 0000 7217 0000 0072  r....r....r....r
-00000c90: 1800 0000 7219 0000 0072 1a00 0000 721b  ....r....r....r.
-00000ca0: 0000 0072 1c00 0000 721d 0000 00da 0a6e  ...r....r......n
-00000cb0: 756d 5f69 6d61 6765 73da 096a 736f 6e5f  um_images..json_
-00000cc0: 6669 6c65 da14 6e6f 726d 616c 697a 6174  file..normalizat
-00000cd0: 696f 6e5f 7061 7261 6d73 da02 6d75 721f  ion_params..mur.
-00000ce0: 0000 00da 1467 656e 6572 6174 655f 6f6e  .....generate_on
-00000cf0: 655f 6366 5f61 7267 73da 0169 da08 696d  e_cf_args..i..im
-00000d00: 675f 7061 7468 da03 696d 6772 2200 0000  g_path..imgr"...
-00000d10: 7223 0000 00da 0870 6172 616c 6c65 6c72  r#.....parallelr
-00000d20: 2500 0000 724e 0000 00da 0a64 6173 6b5f  %...rN.....dask_
-00000d30: 7461 736b 73da 015f 7228 0000 0072 2900  tasks.._r(...r).
-00000d40: 0000 722d 0000 0072 2a00 0000 da12 6765  ..r-...r*.....ge
-00000d50: 745f 636f 756e 7465 7266 6163 7475 616c  t_counterfactual
-00000d60: 1c00 0000 7376 0000 0000 1f08 0302 010e  ....sv..........
-00000d70: ff04 0202 010a 0108 0126 0308 0114 0108  .........&......
-00000d80: 0114 0108 0106 0308 0106 010a ff04 030e  ................
-00000d90: 0106 030c 0112 0108 0304 010c 0104 0110  ................
-00000da0: 010e 0110 fd06 050e 0112 0104 0202 0102  ................
-00000db0: 0102 0102 0104 0102 0102 0102 0102 0102  ................
-00000dc0: 0102 0102 0102 0102 f202 ff06 1412 0106  ................
-00000dd0: 010c 0108 0202 010a 0312 0114 0210 0172  ...............r
-00000de0: 5c00 0000 290f da0e 6f72 6967 696e 616c  \...)...original
-00000df0: 5f70 6174 6368 da0e 6f72 6967 696e 616c  _patch..original
-00000e00: 5f63 6c61 7373 7212 0000 0072 1300 0000  _classr....r....
-00000e10: da07 6368 616e 6e65 6c72 1400 0000 7254  ..channelr....rT
-00000e20: 0000 0072 1f00 0000 7218 0000 0072 1c00  ...r....r....r..
-00000e30: 0000 7215 0000 0072 1900 0000 7222 0000  ..r....r....r"..
-00000e40: 0072 1700 0000 da06 7265 7475 726e 630e  .r......returnc.
-00000e50: 0000 0000 0000 0000 0000 0022 0000 0007  ..........."....
-00000e60: 0000 0003 0000 0073 4403 0000 7400 a001  .......sD...t...
-00000e70: 8804 a101 a002 a100 7400 a001 8803 a101  ........t.......
-00000e80: a002 a100 0200 8904 8903 7c00 6a03 5c03  ..........|.j.\.
-00000e90: 7d0e 7d0f 7d10 7400 a004 7c00 a101 a002  }.}.}.t...|.....
-00000ea0: a100 8803 1800 8804 1b00 7d00 7400 6a01  ..........}.t.j.
-00000eb0: 7c01 6701 7400 6a05 6401 8d02 7d01 7400  |.g.t.j.d...}.t.
-00000ec0: 6a06 7c00 6402 6403 8d02 7d11 8802 6a07  j.|.d.d...}...j.
-00000ed0: 6404 6b02 726e 7c11 7d00 7c11 8804 1400  d.k.rn|.}.|.....
-00000ee0: 8803 1700 8905 8802 6a07 6404 6b02 729a  ........j.d.k.r.
-00000ef0: 8702 6601 6405 6406 8408 8900 6407 6406  ..f.d.d.....d.d.
-00000f00: 8400 7d12 6e38 7c00 6408 6408 6408 8502  ..}.n8|.d.d.d...
-00000f10: 6602 1900 8804 1400 8803 1700 8906 8703  f...............
-00000f20: 8704 8705 8706 6604 6409 6406 8408 7d13  ......f.d.d...}.
-00000f30: 7408 7c13 8802 8302 5c02 8900 7d12 7409  t.|.....\...}.t.
-00000f40: a00a 8701 6601 640a 640b 8408 7c04 4400  ....f.d.d...|.D.
-00000f50: 8301 a101 7d14 7400 a00b 8803 0b00 8804  ....}.t.........
-00000f60: 1b00 7400 a00c 7c10 a101 640c 1400 a102  ..t...|...d.....
-00000f70: 7400 a00c 7c10 a101 640d 1400 6602 7d15  t...|...d...f.}.
-00000f80: 7c11 7c14 0f00 1900 740d 1800 7c15 640e  |.|.....t...|.d.
-00000f90: 1900 7c14 0f00 3c00 7c11 7c14 0f00 1900  ..|...<.|.|.....
-00000fa0: 740d 1700 7c15 640f 1900 7c14 0f00 3c00  t...|.d...|...<.
-00000fb0: 8700 6601 6410 6406 8408 7d16 7c16 7c11  ..f.d.d...}.|.|.
-00000fc0: 6408 6408 6408 8502 6602 1900 8301 a00e  d.d.d...f.......
-00000fd0: a100 a00f a100 a010 a100 7d17 7c09 9001  ..........}.|...
-00000fe0: 7284 7411 6411 7c17 9b00 9d02 8301 0100  r.t.d.|.........
-00000ff0: 7c17 6402 1900 7c0d 6b04 7d18 7c18 7c02  |.d...|.k.}.|.|.
-00001000: 6b02 9001 72a6 7411 6412 8301 0100 6408  k...r.t.d.....d.
-00001010: 5300 6413 7c00 6a03 1700 7d19 7412 7c16  S.d.|.j...}.t.|.
-00001020: 7c12 7c19 6603 7c15 7c08 7c09 6414 9c03  |.|.f.|.|.|.d...
-00001030: 7c0a a401 8e01 7d1a 7c1a a013 a100 0100  |.....}.|.......
-00001040: 7c1a 6a14 7c11 6408 6408 6408 8502 6602  |.j.|.d.d.d...f.
-00001050: 1900 7c01 6408 6408 6408 8502 6602 1900  ..|.d.d.d...f...
-00001060: 7c02 6701 6415 8d03 7d1b 7c1b 6a15 6408  |.g.d...}.|.j.d.
-00001070: 7501 9003 7240 7c1b 6a15 6416 1900 640e  u...r@|.j.d...d.
-00001080: 1900 7d1c 7c1b 6a15 6417 1900 640e 1900  ..}.|.j.d...d...
-00001090: 7d1a 7c12 7400 a004 7c1a 6408 6408 6408  }.|.t...|.d.d.d.
-000010a0: 8502 6602 1900 a101 8301 7d1a 8802 6a07  ..f.......}...j.
-000010b0: 6404 6b02 9002 7254 8800 7c1a 8301 6e06  d.k...rT..|...n.
-000010c0: 8802 7c1a 8301 7d1d 8802 6a07 6404 6b03  ..|...}...j.d.k.
-000010d0: 9002 7274 7400 a016 7c1a 6418 a102 7d1a  ..rtt...|.d...}.
-000010e0: 7411 6419 7c1c 9b00 9d02 8301 0100 7411  t.d.|.........t.
-000010f0: 641a 7c1d 9b00 9d02 8301 0100 7417 7c1a  d.|.........t.|.
-00001100: 8804 1400 8803 1700 7c1a 6a18 640f 1800  ........|.j.d...
-00001110: 641b 8d02 7d1e 7c11 8804 1400 8803 1700  d...}.|.........
-00001120: 7d00 7c1e 7c00 1800 7c00 1b00 641c 1400  }.|.|...|...d...
-00001130: 7d1f 7411 641d 7c1f 9b00 9d02 8301 0100  }.t.d.|.........
-00001140: 7419 741a 7c04 7c14 1900 7c1f 7c14 1900  t.t.|.|...|.|...
-00001150: a010 a100 8302 8301 7d20 7411 641e 7c20  ........} t.d.| 
-00001160: 9b00 9d02 8301 0100 7c0b 6408 7501 9003  ........|.d.u...
-00001170: 7240 741b 6a1c 7c0b 641f 6420 8d02 0100  r@t.j.|.d.d ....
-00001180: 741b 6a1d a01e 7c0b 6421 7c0c 9b00 6422  t.j...|.d!|...d"
-00001190: 9d03 a102 7d21 7409 6a1f 7c21 7c1b 7c20  ....}!t.j.|!|.| 
-000011a0: 7c04 7c14 1900 6423 8d04 0100 7c1b 5300  |.|...d#....|.S.
-000011b0: 2924 619a 0300 000a 2020 2020 4765 6e65  )$a.....    Gene
-000011c0: 7261 7465 2063 6f75 6e74 6572 6661 6374  rate counterfact
-000011d0: 7561 6c73 2066 6f72 2061 2067 6976 656e  uals for a given
-000011e0: 2069 6d61 6765 2070 6174 6368 2e0a 0a20   image patch... 
-000011f0: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
-00001200: 2020 6f72 6967 696e 616c 5f70 6174 6368    original_patch
-00001210: 2028 6e70 2e6e 6461 7272 6179 293a 204f   (np.ndarray): O
-00001220: 7269 6769 6e61 6c20 7061 7463 6820 746f  riginal patch to
-00001230: 2062 6520 6578 706c 6169 6e65 642e 0a20   be explained.. 
-00001240: 2020 2020 2020 2020 6f72 6967 696e 616c          original
-00001250: 5f63 6c61 7373 2028 6e70 2e6e 6461 7272  _class (np.ndarr
-00001260: 6179 293a 204f 7269 6769 6e61 6c20 6c61  ay): Original la
-00001270: 6265 6c20 6f66 2074 6865 2070 6174 6368  bel of the patch
-00001280: 2e0a 2020 2020 2020 2020 206d 6f64 656c  ..         model
-00001290: 2028 746f 7263 682e 6e6e 2e4d 6f64 756c   (torch.nn.Modul
-000012a0: 6529 3a20 4d6f 6465 6c20 746f 2062 6520  e): Model to be 
-000012b0: 6578 706c 6169 6e65 642e 0a20 2020 2020  explained..     
-000012c0: 2020 2020 6368 616e 6e65 6c5f 746f 5f70      channel_to_p
-000012d0: 6572 7475 7262 2028 6c69 7374 293a 204c  erturb (list): L
-000012e0: 6973 7420 6f66 2063 6861 6e6e 656c 7320  ist of channels 
-000012f0: 746f 2070 6572 7475 7262 2e0a 2020 2020  to perturb..    
-00001300: 2020 2020 206e 6f72 6d61 6c69 7a61 7469       normalizati
-00001310: 6f6e 5f70 6172 616d 7320 2864 6963 7429  on_params (dict)
-00001320: 3a20 4469 6374 696f 6e61 7279 2063 6f6e  : Dictionary con
-00001330: 7461 696e 696e 6720 7468 6520 6d65 616e  taining the mean
-00001340: 2061 6e64 2073 7461 6e64 6172 6420 6465   and standard de
-00001350: 7669 6174 696f 6e20 6f66 2065 6163 6820  viation of each 
-00001360: 6368 616e 6e65 6c2e 0a20 2020 2020 2020  channel..       
-00001370: 2020 7472 6169 6e5f 6461 7461 2028 7374    train_data (st
-00001380: 722c 206f 7074 696f 6e61 6c29 3a20 5061  r, optional): Pa
-00001390: 7468 2074 6f20 7468 6520 7472 6169 6e69  th to the traini
-000013a0: 6e67 2064 6174 612e 2044 6566 6175 6c74  ng data. Default
-000013b0: 7320 746f 204e 6f6e 652e 0a20 2020 2020  s to None..     
-000013c0: 2020 2020 6f70 7469 6d69 7a61 7469 6f6e      optimization
-000013d0: 5f70 6172 616d 7320 2864 6963 742c 206f  _params (dict, o
-000013e0: 7074 696f 6e61 6c29 3a20 4469 6374 696f  ptional): Dictio
-000013f0: 6e61 7279 2063 6f6e 7461 696e 696e 6720  nary containing 
-00001400: 7468 6520 7061 7261 6d65 7465 7273 2066  the parameters f
-00001410: 6f72 2074 6865 206f 7074 696d 697a 6174  or the optimizat
-00001420: 696f 6e2e 2044 6566 6175 6c74 7320 746f  ion. Defaults to
-00001430: 207b 7d2e 0a20 2020 2020 2020 2020 7361   {}..         sa
-00001440: 7665 5f64 6972 2028 7374 722c 206f 7074  ve_dir (str, opt
-00001450: 696f 6e61 6c29 3a20 4469 7265 6374 6f72  ional): Director
-00001460: 7920 7768 6572 6520 6f75 7470 7574 2077  y where output w
-00001470: 696c 6c20 6265 2073 6176 6564 2e20 4465  ill be saved. De
-00001480: 6661 756c 7473 2074 6f20 4e6f 6e65 2e0a  faults to None..
-00001490: 2020 2020 2020 2020 2070 6174 6368 5f69           patch_i
-000014a0: 6420 2869 6e74 2c20 6f70 7469 6f6e 616c  d (int, optional
-000014b0: 293a 2050 6174 6368 2049 442e 2044 6566  ): Patch ID. Def
-000014c0: 6175 6c74 7320 746f 204e 6f6e 652e 0a20  aults to None.. 
-000014d0: 2020 2020 2020 2020 7468 7265 7368 6f6c          threshol
-000014e0: 6420 2866 6c6f 6174 2c20 6f70 7469 6f6e  d (float, option
-000014f0: 616c 293a 2054 6872 6573 686f 6c64 2066  al): Threshold f
-00001500: 6f72 2074 6865 2070 7265 6469 6374 696f  or the predictio
-00001510: 6e20 7072 6f62 6162 696c 6974 792e 2044  n probability. D
-00001520: 6566 6175 6c74 7320 746f 2030 2e35 2e0a  efaults to 0.5..
-00001530: 0a20 2020 2020 5265 7475 726e 733a 0a20  .     Returns:. 
-00001540: 2020 2020 2020 2020 4e6f 6e65 0a20 2020          None.   
-00001550: 2072 0e00 0000 2902 7201 0000 0072 0700   r....).r....r..
-00001560: 0000 a901 da03 6469 6dda 036d 6c70 6301  ......dim..mlpc.
-00001570: 0000 0000 0000 0000 0000 0001 0000 0004  ................
-00001580: 0000 0013 0000 0073 1600 0000 7400 6a01  .......s....t.j.
-00001590: 6a02 6a03 8800 7c00 8301 6401 6402 8d02  j.j...|...d.d...
-000015a0: 5300 2903 4e72 0700 0000 7261 0000 0029  S.).Nr....ra...)
-000015b0: 04da 0574 6f72 6368 da02 6e6e da0a 6675  ...torch..nn..fu
-000015c0: 6e63 7469 6f6e 616c da07 736f 6674 6d61  nctional..softma
-000015d0: 78a9 01da 0178 2901 7213 0000 0072 2900  x....x).r....r).
-000015e0: 0000 722a 0000 00da 083c 6c61 6d62 6461  ..r*.....<lambda
-000015f0: 3eba 0000 0072 2f00 0000 7a21 6765 6e65  >....r/...z!gene
-00001600: 7261 7465 5f6f 6e65 5f63 662e 3c6c 6f63  rate_one_cf.<loc
-00001610: 616c 733e 2e3c 6c61 6d62 6461 3e63 0100  als>.<lambda>c..
-00001620: 0000 0000 0000 0000 0000 0100 0000 0100  ................
-00001630: 0000 5300 0000 7304 0000 007c 0053 0072  ..S...s....|.S.r
-00001640: 2600 0000 7229 0000 0072 6800 0000 7229  &...r)...rh...r)
-00001650: 0000 0072 2900 0000 722a 0000 0072 6a00  ...r)...r*...rj.
-00001660: 0000 bb00 0000 722f 0000 004e 6301 0000  ......r/...Nc...
-00001670: 0000 0000 0000 0000 0001 0000 0006 0000  ................
-00001680: 0013 0000 0073 1000 0000 7400 7c00 8803  .....s....t.|...
-00001690: 8800 8801 8802 8305 5300 7226 0000 0029  ........S.r&...)
-000016a0: 01da 0b61 6c74 6572 5f69 6d61 6765 2901  ...alter_image).
-000016b0: da01 7929 0472 5400 0000 721f 0000 00da  ..y).rT...r.....
-000016c0: 0d75 6e6e 6f72 6d65 645f 6d65 616e da0e  .unnormed_mean..
-000016d0: 756e 6e6f 726d 6564 5f70 6174 6368 7229  unnormed_patchr)
-000016e0: 0000 0072 2a00 0000 726a 0000 00be 0000  ...r*...rj......
-000016f0: 0072 2f00 0000 6301 0000 0000 0000 0000  .r/...c.........
-00001700: 0000 0002 0000 0004 0000 0013 0000 0073  ...............s
-00001710: 1c00 0000 6700 7c00 5d14 7d01 7c01 8800  ....g.|.].}.|...
-00001720: 7600 7214 6400 6e02 6401 9102 7104 5300  v.r.d.n.d...q.S.
-00001730: 2902 5446 7229 0000 0029 0272 2c00 0000  ).TFr)...).r,...
-00001740: da04 6e61 6d65 2901 7214 0000 0072 2900  ..name).r....r).
-00001750: 0000 722a 0000 0072 2e00 0000 c300 0000  ..r*...r........
-00001760: 722f 0000 007a 2367 656e 6572 6174 655f  r/...z#generate_
-00001770: 6f6e 655f 6366 2e3c 6c6f 6361 6c73 3e2e  one_cf.<locals>.
-00001780: 3c6c 6973 7463 6f6d 703e e9fc ffff ffe9  <listcomp>......
-00001790: 0400 0000 7201 0000 0072 0700 0000 6301  ....r....r....c.
-000017a0: 0000 0000 0000 0000 0000 0001 0000 0002  ................
-000017b0: 0000 0013 0000 0073 0800 0000 8800 7c00  .......s......|.
-000017c0: 8301 5300 7226 0000 0072 2900 0000 7268  ..S.r&...r)...rh
-000017d0: 0000 0029 01da 0d61 6c74 6572 6564 5f6d  ...)...altered_m
-000017e0: 6f64 656c 7229 0000 0072 2a00 0000 726a  odelr)...r*...rj
-000017f0: 0000 00ca 0000 0072 2f00 0000 7a15 496e  .......r/...z.In
-00001800: 6974 6961 6c20 7072 6f62 6162 696c 6974  itial probabilit
-00001810: 793a 207a 4549 6e73 7461 6e63 6520 616c  y: zEInstance al
-00001820: 7265 6164 7920 636c 6173 7369 6669 6564  ready classified
-00001830: 2061 7320 7461 7267 6574 2063 6c61 7373   as target class
-00001840: 2c20 6e6f 2063 6f75 6e74 6572 6661 6374  , no counterfact
-00001850: 7561 6c20 6e65 6564 6564 2901 7207 0000  ual needed).r...
-00001860: 0029 03da 0d66 6561 7475 7265 5f72 616e  .)...feature_ran
-00001870: 6765 da0a 7472 7573 7473 636f 7265 721c  ge..trustscorer.
-00001880: 0000 0029 03da 0158 da01 5972 1200 0000  ...)...X..Yr....
-00001890: da05 7072 6f62 6172 7500 0000 2904 7201  ..probaru...).r.
-000018a0: 0000 0072 0500 0000 e903 0000 0072 0700  ...r.........r..
-000018b0: 0000 7a1c 436f 756e 7465 7266 6163 7475  ..z.Counterfactu
-000018c0: 616c 2070 726f 6261 6269 6c69 7479 3a20  al probability: 
-000018d0: 7a16 436f 6d70 7574 6564 2070 726f 6261  z.Computed proba
-000018e0: 6269 6c69 7479 3a20 a901 da0c 7072 6573  bility: ....pres
-000018f0: 6572 7665 4178 6973 e964 0000 007a 0a63  erveAxis.d...z.c
-00001900: 6620 6465 6c74 613a 207a 0e63 6620 7065  f delta: z.cf pe
-00001910: 7274 7572 6265 643a 2054 7220 0000 00da  rturbed: Tr ....
-00001920: 0670 6174 6368 5f7a 042e 6e70 7a29 03da  .patch_z..npz)..
-00001930: 0b65 7870 6c61 6e61 7469 6f6e da0c 6366  .explanation..cf
-00001940: 5f70 6572 7475 7262 6564 7214 0000 0029  _perturbedr....)
-00001950: 2072 6400 0000 da06 7465 6e73 6f72 da05   rd.....tensor..
-00001960: 666c 6f61 74da 0573 6861 7065 da0a 6672  float..shape..fr
-00001970: 6f6d 5f6e 756d 7079 da05 696e 7436 3472  om_numpy..int64r
-00001980: 1e00 0000 da04 6172 6368 da0e 6164 645f  ......arch..add_
-00001990: 696e 6974 5f6c 6179 6572 da02 6e70 da05  init_layer..np..
-000019a0: 6172 7261 79da 076d 6178 696d 756d da04  array..maximum..
-000019b0: 6f6e 6573 da07 4550 5349 4c4f 4eda 0664  ones..EPSILON..d
-000019c0: 6574 6163 68da 0363 7075 da05 6e75 6d70  etach..cpu..nump
-000019d0: 7972 4500 0000 7208 0000 00da 0366 6974  yrE...r......fit
-000019e0: da07 6578 706c 6169 6eda 0263 66da 0770  ..explain..cf..p
-000019f0: 6572 6d75 7465 da18 6d65 616e 5f70 7265  ermute..mean_pre
-00001a00: 7365 7276 655f 6469 6d65 6e73 696f 6e73  serve_dimensions
-00001a10: da04 6e64 696d da04 6469 6374 da03 7a69  ..ndim..dict..zi
-00001a20: 7072 3500 0000 7241 0000 0072 3600 0000  pr5...rA...r6...
-00001a30: 7237 0000 00da 0573 6176 657a 2922 725d  r7.....savez)"r]
-00001a40: 0000 0072 5e00 0000 7212 0000 0072 1300  ...r^...r....r..
-00001a50: 0000 725f 0000 0072 1400 0000 7254 0000  ..r_...r....rT..
-00001a60: 0072 1f00 0000 7218 0000 0072 1c00 0000  .r....r....r....
-00001a70: 7215 0000 0072 1900 0000 7222 0000 0072  r....r....r"...r
-00001a80: 1700 0000 da01 4872 5b00 0000 da01 43da  ......Hr[.....C.
-00001a90: 0658 5f6d 6561 6eda 0f69 6e70 7574 5f74  .X_mean..input_t
-00001aa0: 7261 6e73 666f 726d da08 696e 6974 5f66  ransform..init_f
-00001ab0: 756e da0c 6973 5f70 6572 7475 7262 6564  un..is_perturbed
-00001ac0: 7273 0000 00da 0a70 7265 6469 6374 5f66  rs.....predict_f
-00001ad0: 6eda 0a6f 7269 675f 7072 6f62 61da 0470  n..orig_proba..p
-00001ae0: 7265 6472 8100 0000 7290 0000 0072 7d00  redr....r....r}.
-00001af0: 0000 da07 6366 5f70 726f 62da 1c63 6f75  ....cf_prob..cou
-00001b00: 6e74 6572 6661 6374 7561 6c5f 7072 6f62  nterfactual_prob
-00001b10: 6162 696c 6974 6965 73da 0b58 5f70 6572  abilities..X_per
-00001b20: 7475 7262 6564 da08 6366 5f64 656c 7461  turbed..cf_delta
-00001b30: 727e 0000 00da 0a73 6176 6564 5f66 696c  r~.....saved_fil
-00001b40: 6572 2900 0000 2907 7272 0000 0072 1400  er)...).rr...r..
-00001b50: 0000 7213 0000 0072 5400 0000 721f 0000  ..r....rT...r...
-00001b60: 0072 6d00 0000 726e 0000 0072 2a00 0000  .rm...rn...r*...
-00001b70: 7227 0000 0088 0000 0073 9400 0000 0024  r'.......s.....$
-00001b80: 0c01 0cfe 0604 0c01 1601 1201 0e02 0a01  ................
-00001b90: 0403 0c01 0a01 0c01 0a02 1801 1201 0e03  ................
-00001ba0: 0401 10ff 0403 2a01 1801 1803 0c03 2001  ......*....... .
-00001bb0: 0601 0e01 0c01 0a01 0801 0403 0a01 0201  ................
-00001bc0: 0201 0201 02fd 0204 0201 0201 02fa 0407  ................
-00001bd0: 02f9 0609 0803 0401 20ff 0604 0c01 0e01  ........ .......
-00001be0: 0e03 1a02 1aff 0203 0c01 0c02 0e01 0e01  ................
-00001bf0: 0201 12ff 0603 0c01 1001 0e01 1a01 0e02  ................
-00001c00: 0a01 0e01 1601 0401 0201 0201 0201 06fc  ................
-00001c10: 0606 7227 0000 0029 0572 1b00 0000 7213  ..r'...).r....r.
-00001c20: 0000 0072 5400 0000 721f 0000 0072 1d00  ...rT...r....r..
-00001c30: 0000 6306 0000 0000 0000 0000 0000 000b  ..c.............
-00001c40: 0000 0006 0000 0043 0000 0073 b400 0000  .......C...s....
-00001c50: 7400 7c01 8301 7d06 7401 a002 7c06 7403  t.|...}.t...|.t.
-00001c60: a004 7c03 a101 1800 7403 a004 7c04 a101  ..|.....t...|...
-00001c70: 1b00 a101 a005 a100 7d06 7c02 6a06 6401  ........}.|.j.d.
-00001c80: 6b02 7242 7401 a007 7c06 6402 a102 7d07  k.rBt...|.d...}.
-00001c90: 6e0c 7401 a008 7c06 6403 a102 7d07 7c02  n.t...|.d...}.|.
-00001ca0: 7c07 8301 a009 a100 a00a a100 7d08 7403  |...........}.t.
-00001cb0: 6a0b 7c08 6404 6405 8d02 7d09 7c05 6400  j.|.d.d...}.|.d.
-00001cc0: 7501 7284 740c 6600 6900 7c05 a401 8e01  u.r.t.f.i.|.....
-00001cd0: 7d0a 6e06 740c 8300 7d0a 7401 a007 7c06  }.n.t...}.t...|.
-00001ce0: 6402 a102 7d06 7c0a 6a0d 7c06 7c09 6406  d...}.|.j.|.|.d.
-00001cf0: 6407 8d03 0100 740e 7c0a 7c00 8302 0100  d.....t.|.|.....
-00001d00: 6400 5300 2908 4e72 6300 0000 2902 7207  d.S.).Nrc...).r.
-00001d10: 0000 0072 0500 0000 a904 7201 0000 0072  ...r......r....r
-00001d20: 7800 0000 7207 0000 0072 0500 0000 7207  x...r....r....r.
-00001d30: 0000 00a9 01da 0461 7869 7372 0500 0000  .......axisr....
-00001d40: 2901 da07 636c 6173 7365 7329 0fda 176c  )...classes)...l
-00001d50: 6f61 645f 6e70 795f 6669 6c65 735f 746f  oad_npy_files_to
-00001d60: 5f61 7272 6179 7264 0000 0072 8200 0000  _arrayrd...r....
-00001d70: 7286 0000 0072 8700 0000 7280 0000 0072  r....r....r....r
-00001d80: 8400 0000 721e 0000 0072 9100 0000 728b  ....r....r....r.
-00001d90: 0000 0072 8d00 0000 da06 6172 676d 6178  ...r......argmax
-00001da0: 7209 0000 0072 8e00 0000 da0b 7361 7665  r....r......save
-00001db0: 5f6f 626a 6563 7429 0b72 1800 0000 721b  _object).r....r.
-00001dc0: 0000 0072 1300 0000 7254 0000 0072 1f00  ...r....rT...r..
-00001dd0: 0000 721d 0000 00da 0b74 7261 696e 5f70  ..r......train_p
-00001de0: 6174 6368 da03 585f 74da 096d 6f64 656c  atch..X_t..model
-00001df0: 5f6f 7574 da05 7072 6564 73da 0274 7372  _out..preds..tsr
-00001e00: 2900 0000 7229 0000 0072 2a00 0000 7244  )...r)...r*...rD
-00001e10: 0000 000a 0100 0073 1e00 0000 0008 0801  .......s........
-00001e20: 0401 16ff 0803 0a01 0e02 0c02 1001 0e02  ................
-00001e30: 0801 1002 0601 0c01 1001 7244 0000 0063  ..........rD...c
-00001e40: 0100 0000 0000 0000 0000 0000 0900 0000  ................
-00001e50: 0600 0000 4300 0000 7372 0000 0067 007d  ....C...sr...g.}
-00001e60: 0164 0164 0267 027d 027c 0244 005d 4e7d  .d.d.g.}.|.D.]N}
-00001e70: 0374 006a 01a0 027c 007c 03a1 027d 0474  .t.j...|.|...}.t
-00001e80: 00a0 037c 04a1 0144 005d 307d 057c 05a0  ...|...D.]0}.|..
-00001e90: 0464 03a1 0172 2c74 006a 01a0 027c 047c  .d...r,t.j...|.|
-00001ea0: 05a1 027d 0674 05a0 067c 06a1 017d 077c  ...}.t...|...}.|
-00001eb0: 01a0 077c 07a1 0101 0071 2c71 1074 056a  ...|.....q,q.t.j
-00001ec0: 087c 0164 0464 058d 027d 087c 0853 0029  .|.d.d...}.|.S.)
-00001ed0: 064e da01 30da 0131 7a04 2e6e 7079 7201  .N..0..1z..npyr.
-00001ee0: 0000 0072 a600 0000 2909 7235 0000 0072  ...r....).r5...r
-00001ef0: 3600 0000 7237 0000 00da 076c 6973 7464  6...r7.....listd
-00001f00: 6972 da08 656e 6473 7769 7468 7286 0000  ir..endswithr...
-00001f10: 0072 3a00 0000 724c 0000 00da 0573 7461  .r:...rL.....sta
-00001f20: 636b 2909 da08 6261 7365 5f64 6972 da06  ck)...base_dir..
-00001f30: 6172 7261 7973 da08 7375 625f 6469 7273  arrays..sub_dirs
-00001f40: da07 7375 625f 6469 72da 0c73 7562 5f64  ..sub_dir..sub_d
-00001f50: 6972 5f70 6174 68da 0466 696c 65da 0966  ir_path..file..f
-00001f60: 696c 655f 7061 7468 7287 0000 00da 0b66  ile_pathr......f
-00001f70: 696e 616c 5f61 7272 6179 7229 0000 0072  inal_arrayr)...r
-00001f80: 2900 0000 722a 0000 0072 a900 0000 2701  )...r*...r....'.
-00001f90: 0000 7316 0000 0000 0104 0108 0208 010e  ..s.............
-00001fa0: 010e 010a 010e 010a 010e 030e 0172 a900  .............r..
-00001fb0: 0000 6305 0000 0000 0000 0000 0000 0007  ..c.............
-00001fc0: 0000 0007 0000 0043 0000 0073 3800 0000  .......C...s8...
-00001fd0: 7c00 7c03 1400 7c02 1700 7d05 7c01 7c05  |.|...|...}.|.|.
-00001fe0: 7c04 1b00 6400 6400 8502 6400 6400 6400  |...d.d...d.d.d.
-00001ff0: 6400 8502 6604 1900 1400 7d06 7c06 7c02  d...f.....}.|.|.
-00002000: 1800 7c03 1b00 5300 7226 0000 0072 2900  ..|...S.r&...r).
-00002010: 0000 2907 726c 0000 0072 6e00 0000 7254  ..).rl...rn...rT
-00002020: 0000 0072 1f00 0000 726d 0000 00da 0a75  ...r....rm.....u
-00002030: 6e6e 6f72 6d65 645f 79da 096e 6577 5f70  nnormed_y..new_p
-00002040: 6174 6368 7229 0000 0072 2900 0000 722a  atchr)...r)...r*
-00002050: 0000 0072 6b00 0000 3801 0000 7306 0000  ...rk...8...s...
-00002060: 0000 010c 0120 0172 6b00 0000 6302 0000  ..... .rk...c...
-00002070: 0000 0000 0000 0000 0005 0000 0004 0000  ................
-00002080: 0003 0000 0073 3400 0000 4700 8700 6601  .....s4...G...f.
-00002090: 6401 6402 8408 6402 7400 6a01 6a02 8303  d.d...d.t.j.j...
-000020a0: 7d02 7c02 8300 7d03 7400 6a01 a003 7c03  }.|...}.t.j...|.
-000020b0: 7c01 a102 7d04 7c04 7c03 6602 5300 2903  |...}.|.|.f.S.).
-000020c0: 6116 0100 000a 2020 2020 4164 6420 616e  a.....    Add an
-000020d0: 2069 6e69 7469 616c 697a 6174 696f 6e20   initialization 
-000020e0: 6c61 7965 7220 746f 2074 6865 206d 6f64  layer to the mod
-000020f0: 656c 2e0a 0a20 2020 2041 7267 733a 0a20  el...    Args:. 
-00002100: 2020 2020 2020 2069 6e69 745f 6675 6e20         init_fun 
-00002110: 2863 616c 6c61 626c 6529 3a20 496e 6974  (callable): Init
-00002120: 6961 6c69 7a61 7469 6f6e 2066 756e 6374  ialization funct
-00002130: 696f 6e2e 0a20 2020 2020 2020 206d 6f64  ion..        mod
-00002140: 656c 2028 746f 7263 682e 6e6e 2e4d 6f64  el (torch.nn.Mod
-00002150: 756c 6529 3a20 4f72 6967 696e 616c 206d  ule): Original m
-00002160: 6f64 656c 2e0a 0a20 2020 2052 6574 7572  odel...    Retur
-00002170: 6e73 3a0a 2020 2020 2020 2020 7475 706c  ns:.        tupl
-00002180: 653a 2028 746f 7263 682e 6e6e 2e4d 6f64  e: (torch.nn.Mod
-00002190: 756c 652c 2074 6f72 6368 2e6e 6e2e 4d6f  ule, torch.nn.Mo
-000021a0: 6475 6c65 2920 2d20 4d6f 6469 6669 6564  dule) - Modified
-000021b0: 206d 6f64 656c 2061 6e64 2069 6e70 7574   model and input
-000021c0: 2074 7261 6e73 666f 726d 6174 696f 6e20   transformation 
-000021d0: 6c61 7965 722e 0a20 2020 2063 0000 0000  layer..    c....
-000021e0: 0000 0000 0000 0000 0000 0000 0300 0000  ................
-000021f0: 0000 0000 7318 0000 0065 005a 0164 005a  ....s....e.Z.d.Z
-00002200: 0287 0066 0164 0164 0284 085a 0364 0353  ...f.d.d...Z.d.S
-00002210: 0029 047a 2061 6464 5f69 6e69 745f 6c61  .).z add_init_la
-00002220: 7965 722e 3c6c 6f63 616c 733e 2e49 6e70  yer.<locals>.Inp
-00002230: 7574 4675 6e63 0200 0000 0000 0000 0000  utFunc..........
-00002240: 0000 0200 0000 0400 0000 1300 0000 7314  ..............s.
-00002250: 0000 0074 00a0 0188 007c 0183 0164 01a1  ...t.....|...d..
-00002260: 02a0 02a1 0053 0029 024e 72a5 0000 0029  .....S.).Nr....)
-00002270: 0372 6400 0000 7291 0000 0072 8000 0000  .rd...r....r....
-00002280: 2902 da04 7365 6c66 da05 696e 7075 74a9  )...self..input.
-00002290: 0172 9b00 0000 7229 0000 0072 2a00 0000  .r....r)...r*...
-000022a0: da07 666f 7277 6172 644b 0100 0073 0200  ..forwardK...s..
-000022b0: 0000 0001 7a28 6164 645f 696e 6974 5f6c  ....z(add_init_l
-000022c0: 6179 6572 2e3c 6c6f 6361 6c73 3e2e 496e  ayer.<locals>.In
-000022d0: 7075 7446 756e 2e66 6f72 7761 7264 4e29  putFun.forwardN)
-000022e0: 04da 085f 5f6e 616d 655f 5fda 0a5f 5f6d  ...__name__..__m
-000022f0: 6f64 756c 655f 5fda 0c5f 5f71 7561 6c6e  odule__..__qualn
-00002300: 616d 655f 5f72 c300 0000 7229 0000 0072  ame__r....r)...r
-00002310: c200 0000 7229 0000 0072 2a00 0000 da08  ....r)...r*.....
-00002320: 496e 7075 7446 756e 4a01 0000 7302 0000  InputFunJ...s...
-00002330: 0008 0172 c700 0000 2904 7264 0000 0072  ...r....).rd...r
-00002340: 6500 0000 da06 4d6f 6475 6c65 da0a 5365  e.....Module..Se
-00002350: 7175 656e 7469 616c 2905 729b 0000 0072  quential).r....r
-00002360: 1300 0000 72c7 0000 0072 9a00 0000 da0e  ....r....r......
-00002370: 636f 6d70 6c65 7465 5f6d 6f64 656c 7229  complete_modelr)
-00002380: 0000 0072 c200 0000 722a 0000 0072 8500  ...r....r*...r..
-00002390: 0000 3e01 0000 7308 0000 0000 0c18 0406  ..>...s.........
-000023a0: 010e 0172 8500 0000 2903 727f 0000 0072  ...r....).r....r
-000023b0: 7a00 0000 7260 0000 0063 0200 0000 0000  z...r`...c......
-000023c0: 0000 0000 0000 0400 0000 0300 0000 0300  ................
-000023d0: 0000 7338 0000 0074 0088 0074 0183 0272  ..s8...t...t...r
-000023e0: 1088 0066 0189 0087 0066 0164 0164 0284  ...f.....f.d.d..
-000023f0: 0874 027c 006a 0383 0144 0083 017d 027c  .t.|.j...D...}.|
-00002400: 006a 047c 0264 038d 017d 037c 0353 0029  .j.|.d...}.|.S.)
-00002410: 0461 2701 0000 0a20 2020 2043 6f6d 7075  .a'....    Compu
-00002420: 7465 2074 6865 206d 6561 6e20 616c 6f6e  te the mean alon
-00002430: 6720 616c 6c20 6469 6d65 6e73 696f 6e73  g all dimensions
-00002440: 2065 7863 6570 7420 7468 6f73 6520 7370   except those sp
-00002450: 6563 6966 6965 6420 696e 2070 7265 7365  ecified in prese
-00002460: 7276 6541 7869 732e 0a0a 2020 2020 4172  rveAxis...    Ar
-00002470: 6773 3a0a 2020 2020 2020 2020 7465 6e73  gs:.        tens
-00002480: 6f72 2028 746f 7263 682e 5465 6e73 6f72  or (torch.Tensor
-00002490: 293a 2049 6e70 7574 2074 656e 736f 722e  ): Input tensor.
-000024a0: 0a20 2020 2020 2020 2070 7265 7365 7276  .        preserv
-000024b0: 6541 7869 7320 2874 7570 6c65 2c20 6f70  eAxis (tuple, op
-000024c0: 7469 6f6e 616c 293a 2044 696d 656e 7369  tional): Dimensi
-000024d0: 6f6e 7320 746f 2070 7265 7365 7276 652e  ons to preserve.
-000024e0: 2044 6566 6175 6c74 7320 746f 204e 6f6e   Defaults to Non
-000024f0: 652e 0a0a 2020 2020 5265 7475 726e 733a  e...    Returns:
-00002500: 0a20 2020 2020 2020 2074 6f72 6368 2e54  .        torch.T
-00002510: 656e 736f 723a 2054 656e 736f 7220 7769  ensor: Tensor wi
-00002520: 7468 2070 7265 7365 7276 6564 2064 696d  th preserved dim
-00002530: 656e 7369 6f6e 732e 0a20 2020 2063 0100  ensions..    c..
-00002540: 0000 0000 0000 0000 0000 0200 0000 0400  ................
-00002550: 0000 1300 0000 7318 0000 0067 007c 005d  ......s....g.|.]
-00002560: 107d 017c 0188 0076 0172 047c 0191 0271  .}.|...v.r.|...q
-00002570: 0453 0072 2900 0000 7229 0000 0029 0272  .S.r)...r)...).r
-00002580: 2c00 0000 7256 0000 0072 7900 0000 7229  ,...rV...ry...r)
-00002590: 0000 0072 2a00 0000 722e 0000 0063 0100  ...r*...r....c..
-000025a0: 0072 2f00 0000 7a2c 6d65 616e 5f70 7265  .r/...z,mean_pre
-000025b0: 7365 7276 655f 6469 6d65 6e73 696f 6e73  serve_dimensions
-000025c0: 2e3c 6c6f 6361 6c73 3e2e 3c6c 6973 7463  .<locals>.<listc
-000025d0: 6f6d 703e 7261 0000 0029 05da 0a69 7369  omp>ra...)...isi
-000025e0: 6e73 7461 6e63 65da 0369 6e74 7246 0000  nstance..intrF..
-000025f0: 0072 9300 0000 721e 0000 0029 0472 7f00  .r....r....).r..
-00002600: 0000 727a 0000 00da 0e64 696d 735f 746f  ..rz.....dims_to
-00002610: 5f72 6564 7563 65da 0672 6573 756c 7472  _reduce..resultr
-00002620: 2900 0000 7279 0000 0072 2a00 0000 7292  )...ry...r*...r.
-00002630: 0000 0053 0100 0073 0a00 0000 000d 0a01  ...S...s........
-00002640: 0602 1801 0c01 7292 0000 0063 0200 0000  ......r....c....
-00002650: 0000 0000 0000 0000 0300 0000 0800 0000  ................
-00002660: 4300 0000 733c 0000 0074 007c 0164 0183  C...s<...t.|.d..
-00002670: 028f 1e7d 0274 01a0 027c 007c 0264 02a1  ...}.t...|.|.d..
-00002680: 0301 0057 0064 0004 0004 0083 0301 006e  ...W.d.........n
-00002690: 1031 0073 2e30 0001 0001 0001 0059 0001  .1.s.0.......Y..
-000026a0: 0064 0053 0029 034e da02 7762 e9ff ffff  .d.S.).N..wb....
-000026b0: ff29 0372 3400 0000 da06 7069 636b 6c65  .).r4.....pickle
-000026c0: da04 6475 6d70 2903 da03 6f62 6ada 0866  ..dump)...obj..f
-000026d0: 696c 656e 616d 65da 046f 7574 7072 2900  ilename..outpr).
-000026e0: 0000 7229 0000 0072 2a00 0000 72ab 0000  ..r)...r*...r...
-000026f0: 0068 0100 0073 0400 0000 0001 0c01 72ab  .h...s........r.
-00002700: 0000 0029 084e 7210 0000 004e 4e72 0700  ...).Nr....NNr..
-00002710: 0000 4e46 4e29 0546 4e4e 4e72 1000 0000  ..NFN).FNNNr....
-00002720: 2901 4e29 014e 2930 7235 0000 0072 3900  ).N).N)0r5...r9.
-00002730: 0000 da07 5f70 6963 6b6c 6572 d100 0000  ...._pickler....
-00002740: 728d 0000 0072 8600 0000 da06 7061 6e64  r....r......pand
-00002750: 6173 da02 7064 da06 7479 7069 6e67 7202  as..pd..typingr.
-00002760: 0000 0072 6400 0000 7203 0000 00da 0f6d  ...rd...r......m
-00002770: 756c 7469 7072 6f63 6573 7369 6e67 7204  ultiprocessingr.
-00002780: 0000 00da 0864 6174 6173 6574 7372 0600  .....datasetsr..
-00002790: 0000 7290 0000 0072 0800 0000 da0a 636f  ..r....r......co
-000027a0: 6e66 6964 656e 6365 7209 0000 00da 0d63  nfidencer......c
-000027b0: 6f6e 6669 6775 7261 7469 6f6e 720a 0000  onfigurationr...
-000027c0: 0072 0b00 0000 720c 0000 0072 0d00 0000  .r....r....r....
-000027d0: 727f 0000 00da 0766 6c6f 6174 3332 728a  r......float32r.
-000027e0: 0000 0072 cc00 0000 7265 0000 0072 c800  ...r....re...r..
-000027f0: 0000 da04 6c69 7374 7294 0000 00da 0944  ....listr......D
-00002800: 6174 6146 7261 6d65 7280 0000 00da 0373  ataFramer......s
-00002810: 7472 da04 626f 6f6c 725c 0000 00da 076e  tr..boolr\.....n
-00002820: 6461 7272 6179 7227 0000 0072 4400 0000  darrayr'...rD...
-00002830: 72a9 0000 0072 6b00 0000 7285 0000 00da  r....rk...r.....
-00002840: 0654 656e 736f 72da 0574 7570 6c65 7292  .Tensor..tupler.
-00002850: 0000 0072 ab00 0000 7229 0000 0072 2900  ...r....r)...r).
-00002860: 0000 7229 0000 0072 2a00 0000 da08 3c6d  ..r)...r*.....<m
-00002870: 6f64 756c 653e 0100 0000 7398 0000 0008  odule>....s.....
-00002880: 0108 0108 0108 0108 010c 0108 020c 010c  ................
-00002890: 050c 010c 010c 0118 0710 0900 0100 0100  ................
-000028a0: 0100 0100 0100 0100 0100 f302 0102 0102  ................
-000028b0: 0106 0102 0102 0104 0102 0102 0102 0102  ................
-000028c0: 0102 0102 0106 f30c 7600 0100 0100 0100  ........v.......
-000028d0: 0100 f202 0104 0104 0102 0106 0102 0102  ................
-000028e0: 0104 0104 0102 0102 0102 0102 0102 0102  ................
-000028f0: 0102 f10c 7f00 0900 fa02 0202 0106 0102  ................
-00002900: 0102 0106 fa0c 1d08 1108 0608 1600 ff02  ................
-00002910: 0106 0104 fe0c 15                        .......
+00000070: 6d0b 5a0b 0100 6404 6405 6c0c 6d0d 5a0d  m.Z...d.d.l.m.Z.
+00000080: 0100 6406 6407 6c0e 6d0f 5a0f 0100 6404  ..d.d.l.m.Z...d.
+00000090: 6408 6c10 6d11 5a11 0100 6404 6409 6c12  d.l.m.Z...d.d.l.
+000000a0: 6d13 5a13 6d14 5a14 6d15 5a15 6d16 5a16  m.Z.m.Z.m.Z.m.Z.
+000000b0: 0100 650a 6a17 640a 650a 6a18 640b 8d02  ..e.j.d.e.j.d...
+000000c0: 5a19 6422 650d 651a 650a 6a1b 6a1c 651d  Z.d"e.e.e.j.j.e.
+000000d0: 651e 6507 6a1f 6520 6521 6521 651a 6521  e.e.j.e e!e!e.e!
+000000e0: 6522 6509 651e 1900 640e 9c0d 640f 6410  e"e.e...d...d.d.
+000000f0: 8405 5a23 6423 6505 6a24 6505 6a24 651a  ..Z#d#e.j$e.j$e.
+00000100: 650a 6a1b 6a1c 651d 651d 6505 6a24 6505  e.j.j.e.e.e.j$e.
+00000110: 6a24 6521 6522 651e 6521 651a 6520 6401  j$e!e"e.e!e.e d.
+00000120: 6411 9c0f 6412 6413 8405 5a25 6424 6521  d...d.d...Z%d$e!
+00000130: 650a 6a1b 6a1c 651d 651d 6509 651e 1900  e.j.j.e.e.e.e...
+00000140: 6414 9c05 6415 6416 8405 5a26 6417 6418  d...d.d...Z&d.d.
+00000150: 8400 5a27 6419 641a 8400 5a28 641b 641c  ..Z'd.d...Z(d.d.
+00000160: 8400 5a29 6425 650a 6a2a 652b 650a 6a2a  ..Z)d%e.j*e+e.j*
+00000170: 641d 9c03 641e 641f 8405 5a2c 6420 6421  d...d.d...Z,d d!
+00000180: 8400 5a2d 6401 5300 2926 e900 0000 004e  ..Z-d.S.)&.....N
+00000190: 2901 da08 4f70 7469 6f6e 616c 2901 da04  )...Optional)...
+000001a0: 7471 646d e902 0000 0029 01da 0e53 7061  tqdm.....)...Spa
+000001b0: 7469 616c 4461 7461 7365 74e9 0100 0000  tialDataset.....
+000001c0: 2901 da0e 436f 756e 7465 7266 6163 7475  )...Counterfactu
+000001d0: 616c 2901 da0a 5472 7573 7453 636f 7265  al)...TrustScore
+000001e0: 2904 da06 5370 6c69 7473 da07 436f 6c4e  )...Splits..ColN
+000001f0: 616d 65da 1144 6566 6175 6c74 466f 6c64  ame..DefaultFold
+00000200: 6572 4e61 6d65 da0f 4465 6661 756c 7446  erName..DefaultF
+00000210: 696c 654e 616d 6567 2342 920c a19c c73b  ileNameg#B.....;
+00000220: a901 da05 6474 7970 65e7 0000 0000 0000  ....dtype.......
+00000230: e03f 4629 0dda 0764 6174 6173 6574 da0c  .?F)...dataset..
+00000240: 7461 7267 6574 5f63 6c61 7373 da05 6d6f  target_class..mo
+00000250: 6465 6cda 1263 6861 6e6e 656c 5f74 6f5f  del..channel_to_
+00000260: 7065 7274 7572 62da 136f 7074 696d 697a  perturb..optimiz
+00000270: 6174 696f 6e5f 7061 7261 6d73 da06 696d  ation_params..im
+00000280: 6167 6573 da09 7468 7265 7368 6f6c 64da  ages..threshold.
+00000290: 0b6b 6474 7265 655f 7061 7468 da08 7361  .kdtree_path..sa
+000002a0: 7665 5f64 6972 da0b 6e75 6d5f 776f 726b  ve_dir..num_work
+000002b0: 6572 73da 0a74 7261 696e 5f64 6174 61da  ers..train_data.
+000002c0: 0776 6572 626f 7365 da11 7472 7573 7473  .verbose..trusts
+000002d0: 636f 7265 5f6b 7761 7267 7363 0d00 0000  core_kwargsc....
+000002e0: 0000 0000 0000 0000 1e00 0000 1100 0000  ................
+000002f0: 0300 0000 7302 0200 0074 007c 0583 017d  ....s....t.|...}
+00000300: 0d74 0174 026a 03a0 047c 006a 0564 01a1  .t.t.j...|.j.d..
+00000310: 0283 018f 2a7d 0e74 06a0 077c 0ea1 017d  ....*}.t...|...}
+00000320: 0f7c 0f64 0219 007d 107c 0f64 0319 007d  .|.d...}.|.d...}
+00000330: 1157 0064 0404 0004 0083 0301 006e 1031  .W.d.........n.1
+00000340: 0073 4c30 0001 0001 0001 0059 0001 007c  .sL0.......Y...|
+00000350: 0a64 0475 0072 7274 026a 03a0 047c 006a  .d.u.rrt.j...|.j
+00000360: 0574 086a 096a 0aa1 027d 0a7c 0764 0475  .t.j.j...}.|.d.u
+00000370: 0072 8e74 026a 03a0 047c 006a 0b74 0c6a  .r.t.j...|.j.t.j
+00000380: 0d6a 0aa1 027d 077c 0564 0475 0072 9c7c  .j...}.|.d.u.r.|
+00000390: 006a 0e7d 057c 0864 0475 0072 b874 026a  .j.}.|.d.u.r.t.j
+000003a0: 03a0 047c 006a 0b74 0f6a 106a 0aa1 027d  ...|.j.t.j.j...}
+000003b0: 0874 026a 117c 0864 0564 068d 0201 007c  .t.j.|.d.d.....|
+000003c0: 087c 005f 1274 026a 03a0 137c 07a1 0173  .|._.t.j...|...s
+000003d0: f274 147c 077c 0a7c 027c 107c 117c 0c83  .t.|.|.|.|.|.|..
+000003e0: 0601 0074 1564 0783 0101 0067 007d 1274  ...t.d.....g.}.t
+000003f0: 167c 0d83 0144 005d 847d 137c 006a 177c  .|...D.].}.|.j.|
+00000400: 056a 187c 1319 0074 196a 1a6a 0a19 007c  .j.|...t.j.j...|
+00000410: 056a 187c 1319 007c 006a 1b19 007c 056a  .j.|...|.j...|.j
+00000420: 187c 1319 0074 196a 1c6a 0a19 0064 088d  .|...t.j.j...d..
+00000430: 037d 1474 1da0 1e7c 14a1 015c 027d 157d  .}.t...|...\.}.}
+00000440: 167c 006a 0e6a 187c 1619 007c 006a 1b19  .|.j.j.|...|.j..
+00000450: 007d 177c 12a0 1f7c 157c 177c 017c 027c  .}.|...|.|.|.|.|
+00000460: 006a 207c 037c 107c 117c 077c 0b7c 047c  .j |.|.|.|.|.|.|
+00000470: 087c 167c 0666 0ea1 0101 0071 fe7c 0964  .|.|.f.....q.|.d
+00000480: 096b 0490 0172 9264 056e 0264 0a7d 187c  .k...r.d.n.d.}.|
+00000490: 1890 0172 e264 0b64 0c6c 216d 227d 1901  ...r.d.d.l!m"}..
+000004a0: 0064 0b64 046c 237d 1a7c 1964 0d64 0e84  .d.d.l#}.|.d.d..
+000004b0: 0083 0189 0087 0066 0164 0f64 1084 087c  .......f.d.d...|
+000004c0: 1244 0083 017d 1b7c 1a6a 247c 1b64 117c  .D...}.|.j$|.d.|
+000004d0: 0964 129c 028e 017d 1c6e 1c74 257c 127c  .d.....}.n.t%|.|
+000004e0: 0d64 138d 0244 005d 0e7d 1d74 267c 1d8e  .d...D.].}.t&|..
+000004f0: 0001 0090 0171 ee64 0453 0029 1461 da03  .....q.d.S.).a..
+00000500: 0000 0a20 2020 2047 656e 6572 6174 6520  ...    Generate 
+00000510: 636f 756e 7465 7266 6163 7475 616c 7320  counterfactuals 
+00000520: 666f 7220 7468 6520 6461 7461 7365 742e  for the dataset.
+00000530: 0a0a 2020 2020 4172 6773 3a0a 2020 2020  ..    Args:.    
+00000540: 2020 2020 6461 7461 7365 7420 2853 7061      dataset (Spa
+00000550: 7469 616c 4461 7461 7365 7429 3a20 4461  tialDataset): Da
+00000560: 7461 7365 7420 746f 2067 656e 6572 6174  taset to generat
+00000570: 6520 636f 756e 7465 7266 6163 7475 616c  e counterfactual
+00000580: 7320 666f 722e 0a20 2020 2020 2020 2074  s for..        t
+00000590: 6172 6765 745f 636c 6173 7320 2869 6e74  arget_class (int
+000005a0: 293a 2054 6172 6765 7420 636c 6173 7320  ): Target class 
+000005b0: 666f 7220 7468 6520 636f 756e 7465 7266  for the counterf
+000005c0: 6163 7475 616c 732e 0a20 2020 2020 2020  actuals..       
+000005d0: 206d 6f64 656c 2028 746f 7263 682e 6e6e   model (torch.nn
+000005e0: 2e4d 6f64 756c 6529 3a20 4d6f 6465 6c20  .Module): Model 
+000005f0: 746f 2067 656e 6572 6174 6520 636f 756e  to generate coun
+00000600: 7465 7266 6163 7475 616c 7320 666f 722e  terfactuals for.
+00000610: 0a20 2020 2020 2020 2063 6861 6e6e 656c  .        channel
+00000620: 5f74 6f5f 7065 7274 7572 6220 286c 6973  _to_perturb (lis
+00000630: 7429 3a20 4c69 7374 206f 6620 6368 616e  t): List of chan
+00000640: 6e65 6c73 2074 6f20 7065 7274 7572 622e  nels to perturb.
+00000650: 0a20 2020 2020 2020 206f 7074 696d 697a  .        optimiz
+00000660: 6174 696f 6e5f 7061 7261 6d73 2028 6469  ation_params (di
+00000670: 6374 293a 2044 6963 7469 6f6e 6172 7920  ct): Dictionary 
+00000680: 636f 6e74 6169 6e69 6e67 2074 6865 2070  containing the p
+00000690: 6172 616d 6574 6572 7320 666f 7220 7468  arameters for th
+000006a0: 6520 6f70 7469 6d69 7a61 7469 6f6e 2e0a  e optimization..
+000006b0: 2020 2020 2020 2020 696d 6167 6573 2028          images (
+000006c0: 7064 2e44 6174 6146 7261 6d65 2c20 6f70  pd.DataFrame, op
+000006d0: 7469 6f6e 616c 293a 2049 6d61 6765 7320  tional): Images 
+000006e0: 746f 2067 656e 6572 6174 6520 636f 756e  to generate coun
+000006f0: 7465 7266 6163 7475 616c 7320 666f 722e  terfactuals for.
+00000700: 2044 6566 6175 6c74 7320 746f 204e 6f6e   Defaults to Non
+00000710: 652e 0a20 2020 2020 2020 2074 6872 6573  e..        thres
+00000720: 686f 6c64 2028 666c 6f61 742c 206f 7074  hold (float, opt
+00000730: 696f 6e61 6c29 3a20 5468 7265 7368 6f6c  ional): Threshol
+00000740: 6420 666f 7220 7468 6520 7072 6564 6963  d for the predic
+00000750: 7469 6f6e 2070 726f 6261 6269 6c69 7479  tion probability
+00000760: 2e20 4465 6661 756c 7473 2074 6f20 302e  . Defaults to 0.
+00000770: 352e 0a20 2020 2020 2020 206b 6474 7265  5..        kdtre
+00000780: 655f 7061 7468 2028 7374 722c 206f 7074  e_path (str, opt
+00000790: 696f 6e61 6c29 3a20 5061 7468 2074 6f20  ional): Path to 
+000007a0: 7468 6520 6b64 7472 6565 2066 696c 652e  the kdtree file.
+000007b0: 2044 6566 6175 6c74 7320 746f 204e 6f6e   Defaults to Non
+000007c0: 652e 0a20 2020 2020 2020 2073 6176 655f  e..        save_
+000007d0: 6469 7220 2873 7472 2c20 6f70 7469 6f6e  dir (str, option
+000007e0: 616c 293a 2044 6972 6563 746f 7279 2077  al): Directory w
+000007f0: 6865 7265 206f 7574 7075 7420 7769 6c6c  here output will
+00000800: 2062 6520 7361 7665 642e 2044 6566 6175   be saved. Defau
+00000810: 6c74 7320 746f 204e 6f6e 652e 0a20 2020  lts to None..   
+00000820: 2020 2020 206e 756d 5f77 6f72 6b65 7273       num_workers
+00000830: 2028 626f 6f6c 2c20 6f70 7469 6f6e 616c   (bool, optional
+00000840: 293a 204e 756d 6265 7220 6f66 2077 6f72  ): Number of wor
+00000850: 6b65 7273 2074 6f20 7573 6520 666f 7220  kers to use for 
+00000860: 7061 7261 6c6c 656c 2070 726f 6365 7373  parallel process
+00000870: 696e 672e 2044 6566 6175 6c74 7320 746f  ing. Defaults to
+00000880: 204e 6f6e 652e 0a20 2020 2020 2020 2074   None..        t
+00000890: 7261 696e 5f64 6174 6120 2873 7472 2c20  rain_data (str, 
+000008a0: 6f70 7469 6f6e 616c 293a 2050 6174 6820  optional): Path 
+000008b0: 746f 2074 6865 2074 7261 696e 696e 6720  to the training 
+000008c0: 6461 7461 2e20 4465 6661 756c 7473 2074  data. Defaults t
+000008d0: 6f20 4e6f 6e65 2e0a 2020 2020 7a19 6e6f  o None..    z.no
+000008e0: 726d 616c 697a 6174 696f 6e5f 7061 7261  rmalization_para
+000008f0: 6d73 2e6a 736f 6eda 046d 6561 6eda 0573  ms.json..mean..s
+00000900: 7464 6576 4e54 a901 da08 6578 6973 745f  tdevNT....exist_
+00000910: 6f6b 7a0c 6b64 7472 6565 2073 6176 6564  okz.kdtree saved
+00000920: 2903 da08 7061 7463 685f 6964 da05 6c61  )...patch_id..la
+00000930: 6265 6cda 0573 706c 6974 7206 0000 0046  bel..splitr....F
+00000940: 7201 0000 0029 01da 0764 656c 6179 6564  r....)...delayed
+00000950: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
+00000960: 0002 0000 0053 0000 0073 0800 0000 7400  .....S...s....t.
+00000970: 7c00 8e00 5300 a901 4e29 01da 0f67 656e  |...S...N)...gen
+00000980: 6572 6174 655f 6f6e 655f 6366 2901 da04  erate_one_cf)...
+00000990: 6172 6773 a900 7228 0000 00fa 562f 6365  args..r(....V/ce
+000009a0: 6e74 7261 6c2f 686f 6d65 2f7a 7761 6e67  ntral/home/zwang
+000009b0: 322f 6d6f 7270 6865 7573 2d73 7061 7469  2/morpheus-spati
+000009c0: 616c 2f6d 6f72 7068 6575 732f 7372 632f  al/morpheus/src/
+000009d0: 6d6f 7270 6865 7573 2f63 6f75 6e74 6572  morpheus/counter
+000009e0: 6661 6374 7561 6c2f 6765 6e65 7261 7465  factual/generate
+000009f0: 2e70 79da 1767 656e 6572 6174 655f 6f6e  .py..generate_on
+00000a00: 655f 6366 5f64 656c 6179 6564 7c00 0000  e_cf_delayed|...
+00000a10: 7302 0000 0000 027a 3367 6574 5f63 6f75  s......z3get_cou
+00000a20: 6e74 6572 6661 6374 7561 6c2e 3c6c 6f63  nterfactual.<loc
+00000a30: 616c 733e 2e67 656e 6572 6174 655f 6f6e  als>.generate_on
+00000a40: 655f 6366 5f64 656c 6179 6564 6301 0000  e_cf_delayedc...
+00000a50: 0000 0000 0000 0000 0002 0000 0004 0000  ................
+00000a60: 0013 0000 0073 1400 0000 6700 7c00 5d0c  .....s....g.|.].
+00000a70: 7d01 8800 7c01 8301 9102 7104 5300 7228  }...|.....q.S.r(
+00000a80: 0000 0072 2800 0000 2902 da02 2e30 7227  ...r(...)....0r'
+00000a90: 0000 00a9 0172 2a00 0000 7228 0000 0072  .....r*...r(...r
+00000aa0: 2900 0000 da0a 3c6c 6973 7463 6f6d 703e  ).....<listcomp>
+00000ab0: 8000 0000 f300 0000 007a 2667 6574 5f63  .........z&get_c
+00000ac0: 6f75 6e74 6572 6661 6374 7561 6c2e 3c6c  ounterfactual.<l
+00000ad0: 6f63 616c 733e 2e3c 6c69 7374 636f 6d70  ocals>.<listcomp
+00000ae0: 3eda 0970 726f 6365 7373 6573 2902 da09  >..processes)...
+00000af0: 7363 6865 6475 6c65 7272 1900 0000 2901  schedulerr....).
+00000b00: da05 746f 7461 6c29 27da 036c 656e da04  ..total)'..len..
+00000b10: 6f70 656e da02 6f73 da04 7061 7468 da04  open..os..path..
+00000b20: 6a6f 696e da09 7370 6c69 745f 6469 72da  join..split_dir.
+00000b30: 046a 736f 6eda 046c 6f61 6472 0900 0000  .json..loadr....
+00000b40: da05 7472 6169 6eda 0576 616c 7565 da08  ..train..value..
+00000b50: 726f 6f74 5f64 6972 720c 0000 00da 066b  root_dirr......k
+00000b60: 6474 7265 65da 086d 6574 6164 6174 6172  dtree..metadatar
+00000b70: 0b00 0000 da0e 636f 756e 7465 7266 6163  ......counterfac
+00000b80: 7475 616c da08 6d61 6b65 6469 7273 da06  tual..makedirs..
+00000b90: 6366 5f64 6972 da06 6578 6973 7473 da0c  cf_dir..exists..
+00000ba0: 6275 696c 645f 6b64 7472 6565 da05 7072  build_kdtree..pr
+00000bb0: 696e 74da 0572 616e 6765 da13 6765 6e65  int..range..gene
+00000bc0: 7261 7465 5f70 6174 6368 5f70 6174 68da  rate_patch_path.
+00000bd0: 0469 6c6f 6372 0a00 0000 7221 0000 00da  .ilocr....r!....
+00000be0: 0a6c 6162 656c 5f6e 616d 65da 0673 706c  .label_name..spl
+00000bf0: 6974 7372 0500 0000 da11 6c6f 6164 5f73  itsr......load_s
+00000c00: 696e 676c 655f 696d 6167 65da 0661 7070  ingle_image..app
+00000c10: 656e 64da 0d63 6861 6e6e 656c 5f6e 616d  end..channel_nam
+00000c20: 6573 da04 6461 736b 7224 0000 005a 1464  es..daskr$...Z.d
+00000c30: 6173 6b2e 6d75 6c74 6970 726f 6365 7373  ask.multiprocess
+00000c40: 696e 67da 0763 6f6d 7075 7465 7203 0000  ing..computer...
+00000c50: 0072 2600 0000 291e 7210 0000 0072 1100  .r&...).r....r..
+00000c60: 0000 7212 0000 0072 1300 0000 7214 0000  ..r....r....r...
+00000c70: 0072 1500 0000 7216 0000 0072 1700 0000  .r....r....r....
+00000c80: 7218 0000 0072 1900 0000 721a 0000 0072  r....r....r....r
+00000c90: 1b00 0000 721c 0000 00da 0a6e 756d 5f69  ....r......num_i
+00000ca0: 6d61 6765 735a 096a 736f 6e5f 6669 6c65  magesZ.json_file
+00000cb0: da14 6e6f 726d 616c 697a 6174 696f 6e5f  ..normalization_
+00000cc0: 7061 7261 6d73 da02 6d75 721e 0000 005a  params..mur....Z
+00000cd0: 1467 656e 6572 6174 655f 6f6e 655f 6366  .generate_one_cf
+00000ce0: 5f61 7267 73da 0169 da08 696d 675f 7061  _args..i..img_pa
+00000cf0: 7468 da03 696d 6772 2100 0000 7222 0000  th..imgr!...r"..
+00000d00: 00da 0870 6172 616c 6c65 6c72 2400 0000  ...parallelr$...
+00000d10: 724d 0000 005a 0a64 6173 6b5f 7461 736b  rM...Z.dask_task
+00000d20: 73da 015f 7227 0000 0072 2800 0000 722c  s.._r'...r(...r,
+00000d30: 0000 0072 2900 0000 da12 6765 745f 636f  ...r).....get_co
+00000d40: 756e 7465 7266 6163 7475 616c 1b00 0000  unterfactual....
+00000d50: 7376 0000 0000 1f08 0302 010e ff04 0202  sv..............
+00000d60: 010a 0108 0126 0308 0114 0108 0114 0108  .....&..........
+00000d70: 0106 0308 0106 010a ff04 030e 0106 030c  ................
+00000d80: 0112 0108 0304 010c 0104 0110 010e 0110  ................
+00000d90: fd06 050e 0112 0104 0202 0102 0102 0102  ................
+00000da0: 0104 0102 0102 0102 0102 0102 0102 0102  ................
+00000db0: 0102 0102 f202 ff06 1412 0106 010c 0108  ................
+00000dc0: 0202 010a 0312 0114 0210 0172 5700 0000  ...........rW...
+00000dd0: 290f da0e 6f72 6967 696e 616c 5f70 6174  )...original_pat
+00000de0: 6368 da0e 6f72 6967 696e 616c 5f63 6c61  ch..original_cla
+00000df0: 7373 7211 0000 0072 1200 0000 da07 6368  ssr....r......ch
+00000e00: 616e 6e65 6c72 1300 0000 7251 0000 0072  annelr....rQ...r
+00000e10: 1e00 0000 7217 0000 0072 1b00 0000 7214  ....r....r....r.
+00000e20: 0000 0072 1800 0000 7221 0000 0072 1600  ...r....r!...r..
+00000e30: 0000 da06 7265 7475 726e 630e 0000 0000  ....returnc.....
+00000e40: 0000 0000 0000 0022 0000 0007 0000 0003  ......."........
+00000e50: 0000 0073 3403 0000 7400 a001 8804 a101  ...s4...t.......
+00000e60: a002 a100 7400 a001 8803 a101 a002 a100  ....t...........
+00000e70: 0200 8904 8903 7c00 6a03 5c03 7d0e 7d0f  ......|.j.\.}.}.
+00000e80: 7d10 7400 a004 7c00 a101 a002 a100 8803  }.t...|.........
+00000e90: 1800 8804 1b00 7d00 7400 6a01 7c01 6701  ......}.t.j.|.g.
+00000ea0: 7400 6a05 6401 8d02 7d01 7400 6a06 7c00  t.j.d...}.t.j.|.
+00000eb0: 6402 6403 8d02 7d11 8802 6a07 6404 6b02  d.d...}...j.d.k.
+00000ec0: 726e 7c11 7d00 7c11 8804 1400 8803 1700  rn|.}.|.........
+00000ed0: 8905 8802 6a07 6404 6b02 729a 8702 6601  ....j.d.k.r...f.
+00000ee0: 6405 6406 8408 8900 6407 6406 8400 7d12  d.d.....d.d...}.
+00000ef0: 6e38 7c00 6408 6408 6408 8502 6602 1900  n8|.d.d.d...f...
+00000f00: 8804 1400 8803 1700 8906 8703 8704 8705  ................
+00000f10: 8706 6604 6409 6406 8408 7d13 7408 7c13  ..f.d.d...}.t.|.
+00000f20: 8802 8302 5c02 8900 7d12 7409 a00a 8701  ....\...}.t.....
+00000f30: 6601 640a 640b 8408 7c04 4400 8301 a101  f.d.d...|.D.....
+00000f40: 7d14 7400 a00b 8803 0b00 8804 1b00 7400  }.t...........t.
+00000f50: a00c 7c10 a101 640c 1400 a102 7400 a00c  ..|...d.....t...
+00000f60: 7c10 a101 640d 1400 6602 7d15 7c11 7c14  |...d...f.}.|.|.
+00000f70: 0f00 1900 740d 1800 7c15 640e 1900 7c14  ....t...|.d...|.
+00000f80: 0f00 3c00 7c11 7c14 0f00 1900 740d 1700  ..<.|.|.....t...
+00000f90: 7c15 640f 1900 7c14 0f00 3c00 8700 6601  |.d...|...<...f.
+00000fa0: 6410 6406 8408 7d16 7c16 7c11 6408 6408  d.d...}.|.|.d.d.
+00000fb0: 6408 8502 6602 1900 8301 a00e a100 a00f  d...f...........
+00000fc0: a100 a010 a100 7d17 7c09 9001 7284 7411  ......}.|...r.t.
+00000fd0: 6411 7c17 9b00 9d02 8301 0100 7c17 6402  d.|.........|.d.
+00000fe0: 1900 7c0d 6b04 7d18 7c18 7c02 6b02 9001  ..|.k.}.|.|.k...
+00000ff0: 72a6 7411 6412 8301 0100 6408 5300 6413  r.t.d.....d.S.d.
+00001000: 7c00 6a03 1700 7d19 7412 7c16 7c12 7c19  |.j...}.t.|.|.|.
+00001010: 6603 7c15 7c08 7c09 6414 9c03 7c0a a401  f.|.|.|.d...|...
+00001020: 8e01 7d1a 7c1a a013 a100 0100 7c1a 6a14  ..}.|.......|.j.
+00001030: 7c11 6408 6408 6408 8502 6602 1900 7c01  |.d.d.d...f...|.
+00001040: 6408 6408 6408 8502 6602 1900 7c02 6701  d.d.d...f...|.g.
+00001050: 6415 8d03 7d1b 7c1b 6a15 6408 7501 9003  d...}.|.j.d.u...
+00001060: 7230 7c1b 6a15 6416 1900 640e 1900 7d1c  r0|.j.d...d...}.
+00001070: 7c1b 6a15 6417 1900 640e 1900 7d1a 7c12  |.j.d...d...}.|.
+00001080: 7400 a004 7c1a 6408 6408 6408 8502 6602  t...|.d.d.d...f.
+00001090: 1900 a101 8301 7d1a 8802 6a07 6404 6b02  ......}...j.d.k.
+000010a0: 9002 7254 8800 7c1a 8301 6e06 8802 7c1a  ..rT..|...n...|.
+000010b0: 8301 7d1d 8802 6a07 6404 6b03 9002 7274  ..}...j.d.k...rt
+000010c0: 7400 a016 7c1a 6418 a102 7d1a 7411 6419  t...|.d...}.t.d.
+000010d0: 7c1d 9b00 9d02 8301 0100 7417 7c1a 8804  |.........t.|...
+000010e0: 1400 8803 1700 7c1a 6a18 640f 1800 641a  ......|.j.d...d.
+000010f0: 8d02 7d1e 7c11 8804 1400 8803 1700 7d00  ..}.|.........}.
+00001100: 7c1e 7c00 1800 7c00 1b00 641b 1400 7d1f  |.|...|...d...}.
+00001110: 7419 741a 7409 a00a 7c04 a101 7c14 1900  t.t.t...|...|...
+00001120: 7c1f 7c14 1900 a010 a100 8302 8301 7d20  |.|...........} 
+00001130: 7411 641c 7c20 9b00 9d02 8301 0100 7c0b  t.d.| ........|.
+00001140: 6408 7501 9003 7230 741b 6a1c 7c0b 641d  d.u...r0t.j.|.d.
+00001150: 641e 8d02 0100 741b 6a1d a01e 7c0b 641f  d.....t.j...|.d.
+00001160: 7c0c 9b00 6420 9d03 a102 7d21 7409 6a1f  |...d ....}!t.j.
+00001170: 7c21 7c1b 7c20 7409 a00a 7c04 a101 7c14  |!|.| t...|...|.
+00001180: 1900 6421 8d04 0100 7c1b 5300 2922 619a  ..d!....|.S.)"a.
+00001190: 0300 000a 2020 2020 4765 6e65 7261 7465  ....    Generate
+000011a0: 2063 6f75 6e74 6572 6661 6374 7561 6c73   counterfactuals
+000011b0: 2066 6f72 2061 2067 6976 656e 2069 6d61   for a given ima
+000011c0: 6765 2070 6174 6368 2e0a 0a20 2020 2041  ge patch...    A
+000011d0: 7267 733a 0a20 2020 2020 2020 2020 6f72  rgs:.         or
+000011e0: 6967 696e 616c 5f70 6174 6368 2028 6e70  iginal_patch (np
+000011f0: 2e6e 6461 7272 6179 293a 204f 7269 6769  .ndarray): Origi
+00001200: 6e61 6c20 7061 7463 6820 746f 2062 6520  nal patch to be 
+00001210: 6578 706c 6169 6e65 642e 0a20 2020 2020  explained..     
+00001220: 2020 2020 6f72 6967 696e 616c 5f63 6c61      original_cla
+00001230: 7373 2028 6e70 2e6e 6461 7272 6179 293a  ss (np.ndarray):
+00001240: 204f 7269 6769 6e61 6c20 6c61 6265 6c20   Original label 
+00001250: 6f66 2074 6865 2070 6174 6368 2e0a 2020  of the patch..  
+00001260: 2020 2020 2020 206d 6f64 656c 2028 746f         model (to
+00001270: 7263 682e 6e6e 2e4d 6f64 756c 6529 3a20  rch.nn.Module): 
+00001280: 4d6f 6465 6c20 746f 2062 6520 6578 706c  Model to be expl
+00001290: 6169 6e65 642e 0a20 2020 2020 2020 2020  ained..         
+000012a0: 6368 616e 6e65 6c5f 746f 5f70 6572 7475  channel_to_pertu
+000012b0: 7262 2028 6c69 7374 293a 204c 6973 7420  rb (list): List 
+000012c0: 6f66 2063 6861 6e6e 656c 7320 746f 2070  of channels to p
+000012d0: 6572 7475 7262 2e0a 2020 2020 2020 2020  erturb..        
+000012e0: 206e 6f72 6d61 6c69 7a61 7469 6f6e 5f70   normalization_p
+000012f0: 6172 616d 7320 2864 6963 7429 3a20 4469  arams (dict): Di
+00001300: 6374 696f 6e61 7279 2063 6f6e 7461 696e  ctionary contain
+00001310: 696e 6720 7468 6520 6d65 616e 2061 6e64  ing the mean and
+00001320: 2073 7461 6e64 6172 6420 6465 7669 6174   standard deviat
+00001330: 696f 6e20 6f66 2065 6163 6820 6368 616e  ion of each chan
+00001340: 6e65 6c2e 0a20 2020 2020 2020 2020 7472  nel..         tr
+00001350: 6169 6e5f 6461 7461 2028 7374 722c 206f  ain_data (str, o
+00001360: 7074 696f 6e61 6c29 3a20 5061 7468 2074  ptional): Path t
+00001370: 6f20 7468 6520 7472 6169 6e69 6e67 2064  o the training d
+00001380: 6174 612e 2044 6566 6175 6c74 7320 746f  ata. Defaults to
+00001390: 204e 6f6e 652e 0a20 2020 2020 2020 2020   None..         
+000013a0: 6f70 7469 6d69 7a61 7469 6f6e 5f70 6172  optimization_par
+000013b0: 616d 7320 2864 6963 742c 206f 7074 696f  ams (dict, optio
+000013c0: 6e61 6c29 3a20 4469 6374 696f 6e61 7279  nal): Dictionary
+000013d0: 2063 6f6e 7461 696e 696e 6720 7468 6520   containing the 
+000013e0: 7061 7261 6d65 7465 7273 2066 6f72 2074  parameters for t
+000013f0: 6865 206f 7074 696d 697a 6174 696f 6e2e  he optimization.
+00001400: 2044 6566 6175 6c74 7320 746f 207b 7d2e   Defaults to {}.
+00001410: 0a20 2020 2020 2020 2020 7361 7665 5f64  .         save_d
+00001420: 6972 2028 7374 722c 206f 7074 696f 6e61  ir (str, optiona
+00001430: 6c29 3a20 4469 7265 6374 6f72 7920 7768  l): Directory wh
+00001440: 6572 6520 6f75 7470 7574 2077 696c 6c20  ere output will 
+00001450: 6265 2073 6176 6564 2e20 4465 6661 756c  be saved. Defaul
+00001460: 7473 2074 6f20 4e6f 6e65 2e0a 2020 2020  ts to None..    
+00001470: 2020 2020 2070 6174 6368 5f69 6420 2869       patch_id (i
+00001480: 6e74 2c20 6f70 7469 6f6e 616c 293a 2050  nt, optional): P
+00001490: 6174 6368 2049 442e 2044 6566 6175 6c74  atch ID. Default
+000014a0: 7320 746f 204e 6f6e 652e 0a20 2020 2020  s to None..     
+000014b0: 2020 2020 7468 7265 7368 6f6c 6420 2866      threshold (f
+000014c0: 6c6f 6174 2c20 6f70 7469 6f6e 616c 293a  loat, optional):
+000014d0: 2054 6872 6573 686f 6c64 2066 6f72 2074   Threshold for t
+000014e0: 6865 2070 7265 6469 6374 696f 6e20 7072  he prediction pr
+000014f0: 6f62 6162 696c 6974 792e 2044 6566 6175  obability. Defau
+00001500: 6c74 7320 746f 2030 2e35 2e0a 0a20 2020  lts to 0.5...   
+00001510: 2020 5265 7475 726e 733a 0a20 2020 2020    Returns:.     
+00001520: 2020 2020 4e6f 6e65 0a20 2020 2072 0d00      None.    r..
+00001530: 0000 2902 7201 0000 0072 0600 0000 a901  ..).r....r......
+00001540: da03 6469 6dda 036d 6c70 6301 0000 0000  ..dim..mlpc.....
+00001550: 0000 0000 0000 0001 0000 0004 0000 0013  ................
+00001560: 0000 0073 1600 0000 7400 6a01 6a02 6a03  ...s....t.j.j.j.
+00001570: 8800 7c00 8301 6401 6402 8d02 5300 2903  ..|...d.d...S.).
+00001580: 4e72 0600 0000 725c 0000 0029 04da 0574  Nr....r\...)...t
+00001590: 6f72 6368 da02 6e6e da0a 6675 6e63 7469  orch..nn..functi
+000015a0: 6f6e 616c da07 736f 6674 6d61 78a9 01da  onal..softmax...
+000015b0: 0178 2901 7212 0000 0072 2800 0000 7229  .x).r....r(...r)
+000015c0: 0000 00da 083c 6c61 6d62 6461 3eb9 0000  .....<lambda>...
+000015d0: 0072 2e00 0000 7a21 6765 6e65 7261 7465  .r....z!generate
+000015e0: 5f6f 6e65 5f63 662e 3c6c 6f63 616c 733e  _one_cf.<locals>
+000015f0: 2e3c 6c61 6d62 6461 3e63 0100 0000 0000  .<lambda>c......
+00001600: 0000 0000 0000 0100 0000 0100 0000 5300  ..............S.
+00001610: 0000 7304 0000 007c 0053 0072 2500 0000  ..s....|.S.r%...
+00001620: 7228 0000 0072 6300 0000 7228 0000 0072  r(...rc...r(...r
+00001630: 2800 0000 7229 0000 0072 6500 0000 ba00  (...r)...re.....
+00001640: 0000 722e 0000 004e 6301 0000 0000 0000  ..r....Nc.......
+00001650: 0000 0000 0001 0000 0006 0000 0013 0000  ................
+00001660: 0073 1000 0000 7400 7c00 8803 8800 8801  .s....t.|.......
+00001670: 8802 8305 5300 7225 0000 0029 01da 0b61  ....S.r%...)...a
+00001680: 6c74 6572 5f69 6d61 6765 2901 da01 7929  lter_image)...y)
+00001690: 0472 5100 0000 721e 0000 00da 0d75 6e6e  .rQ...r......unn
+000016a0: 6f72 6d65 645f 6d65 616e da0e 756e 6e6f  ormed_mean..unno
+000016b0: 726d 6564 5f70 6174 6368 7228 0000 0072  rmed_patchr(...r
+000016c0: 2900 0000 7265 0000 00bd 0000 0072 2e00  )...re.......r..
+000016d0: 0000 6301 0000 0000 0000 0000 0000 0002  ..c.............
+000016e0: 0000 0004 0000 0013 0000 0073 1c00 0000  ...........s....
+000016f0: 6700 7c00 5d14 7d01 7c01 8800 7600 7214  g.|.].}.|...v.r.
+00001700: 6400 6e02 6401 9102 7104 5300 2902 5446  d.n.d...q.S.).TF
+00001710: 7228 0000 0029 0272 2b00 0000 da04 6e61  r(...).r+.....na
+00001720: 6d65 2901 7213 0000 0072 2800 0000 7229  me).r....r(...r)
+00001730: 0000 0072 2d00 0000 c200 0000 722e 0000  ...r-.......r...
+00001740: 007a 2367 656e 6572 6174 655f 6f6e 655f  .z#generate_one_
+00001750: 6366 2e3c 6c6f 6361 6c73 3e2e 3c6c 6973  cf.<locals>.<lis
+00001760: 7463 6f6d 703e e9fc ffff ffe9 0400 0000  tcomp>..........
+00001770: 7201 0000 0072 0600 0000 6301 0000 0000  r....r....c.....
+00001780: 0000 0000 0000 0001 0000 0002 0000 0013  ................
+00001790: 0000 0073 0800 0000 8800 7c00 8301 5300  ...s......|...S.
+000017a0: 7225 0000 0072 2800 0000 7263 0000 0029  r%...r(...rc...)
+000017b0: 01da 0d61 6c74 6572 6564 5f6d 6f64 656c  ...altered_model
+000017c0: 7228 0000 0072 2900 0000 7265 0000 00c9  r(...r)...re....
+000017d0: 0000 0072 2e00 0000 7a15 496e 6974 6961  ...r....z.Initia
+000017e0: 6c20 7072 6f62 6162 696c 6974 793a 207a  l probability: z
+000017f0: 4549 6e73 7461 6e63 6520 616c 7265 6164  EInstance alread
+00001800: 7920 636c 6173 7369 6669 6564 2061 7320  y classified as 
+00001810: 7461 7267 6574 2063 6c61 7373 2c20 6e6f  target class, no
+00001820: 2063 6f75 6e74 6572 6661 6374 7561 6c20   counterfactual 
+00001830: 6e65 6564 6564 2901 7206 0000 0029 03da  needed).r....)..
+00001840: 0d66 6561 7475 7265 5f72 616e 6765 5a0a  .feature_rangeZ.
+00001850: 7472 7573 7473 636f 7265 721b 0000 0029  trustscorer....)
+00001860: 03da 0158 da01 5972 1100 0000 5a05 7072  ...X..Yr....Z.pr
+00001870: 6f62 6172 6f00 0000 2904 7201 0000 0072  obaro...).r....r
+00001880: 0400 0000 e903 0000 0072 0600 0000 7a1c  .........r....z.
+00001890: 436f 756e 7465 7266 6163 7475 616c 2070  Counterfactual p
+000018a0: 726f 6261 6269 6c69 7479 3a20 a901 da0c  robability: ....
+000018b0: 7072 6573 6572 7665 4178 6973 e964 0000  preserveAxis.d..
+000018c0: 007a 0e63 6620 7065 7274 7572 6265 643a  .z.cf perturbed:
+000018d0: 2054 721f 0000 005a 0670 6174 6368 5f7a   Tr....Z.patch_z
+000018e0: 042e 6e70 7a29 03da 0b65 7870 6c61 6e61  ..npz)...explana
+000018f0: 7469 6f6e da0c 6366 5f70 6572 7475 7262  tion..cf_perturb
+00001900: 6564 7213 0000 0029 2072 5f00 0000 da06  edr....) r_.....
+00001910: 7465 6e73 6f72 da05 666c 6f61 74da 0573  tensor..float..s
+00001920: 6861 7065 da0a 6672 6f6d 5f6e 756d 7079  hape..from_numpy
+00001930: da05 696e 7436 3472 1d00 0000 da04 6172  ..int64r......ar
+00001940: 6368 da0e 6164 645f 696e 6974 5f6c 6179  ch..add_init_lay
+00001950: 6572 da02 6e70 da05 6172 7261 79da 076d  er..np..array..m
+00001960: 6178 696d 756d da04 6f6e 6573 da07 4550  aximum..ones..EP
+00001970: 5349 4c4f 4eda 0664 6574 6163 68da 0363  SILON..detach..c
+00001980: 7075 da05 6e75 6d70 7972 4400 0000 7207  pu..numpyrD...r.
+00001990: 0000 00da 0366 6974 da07 6578 706c 6169  .....fit..explai
+000019a0: 6eda 0263 66da 0770 6572 6d75 7465 da18  n..cf..permute..
+000019b0: 6d65 616e 5f70 7265 7365 7276 655f 6469  mean_preserve_di
+000019c0: 6d65 6e73 696f 6e73 da04 6e64 696d da04  mensions..ndim..
+000019d0: 6469 6374 da03 7a69 7072 3400 0000 7240  dict..zipr4...r@
+000019e0: 0000 0072 3500 0000 7236 0000 00da 0573  ...r5...r6.....s
+000019f0: 6176 657a 2922 7258 0000 0072 5900 0000  avez)"rX...rY...
+00001a00: 7211 0000 0072 1200 0000 725a 0000 0072  r....r....rZ...r
+00001a10: 1300 0000 7251 0000 0072 1e00 0000 7217  ....rQ...r....r.
+00001a20: 0000 0072 1b00 0000 7214 0000 0072 1800  ...r....r....r..
+00001a30: 0000 7221 0000 0072 1600 0000 da01 4872  ..r!...r......Hr
+00001a40: 5600 0000 da01 435a 0658 5f6d 6561 6eda  V.....CZ.X_mean.
+00001a50: 0f69 6e70 7574 5f74 7261 6e73 666f 726d  .input_transform
+00001a60: da08 696e 6974 5f66 756e 5a0c 6973 5f70  ..init_funZ.is_p
+00001a70: 6572 7475 7262 6564 726e 0000 005a 0a70  erturbedrn...Z.p
+00001a80: 7265 6469 6374 5f66 6e5a 0a6f 7269 675f  redict_fnZ.orig_
+00001a90: 7072 6f62 61da 0470 7265 6472 7900 0000  proba..predry...
+00001aa0: 7288 0000 0072 7500 0000 5a07 6366 5f70  r....ru...Z.cf_p
+00001ab0: 726f 625a 1c63 6f75 6e74 6572 6661 6374  robZ.counterfact
+00001ac0: 7561 6c5f 7072 6f62 6162 696c 6974 6965  ual_probabilitie
+00001ad0: 735a 0b58 5f70 6572 7475 7262 6564 5a08  sZ.X_perturbedZ.
+00001ae0: 6366 5f64 656c 7461 7276 0000 005a 0a73  cf_deltarv...Z.s
+00001af0: 6176 6564 5f66 696c 6572 2800 0000 2907  aved_filer(...).
+00001b00: 726d 0000 0072 1300 0000 7212 0000 0072  rm...r....r....r
+00001b10: 5100 0000 721e 0000 0072 6800 0000 7269  Q...r....rh...ri
+00001b20: 0000 0072 2900 0000 7226 0000 0087 0000  ...r)...r&......
+00001b30: 0073 9a00 0000 0024 0c01 0cfe 0604 0c01  .s.....$........
+00001b40: 1601 1201 0e02 0a01 0403 0c01 0a01 0c01  ................
+00001b50: 0a02 1801 1201 0e03 0401 10ff 0403 2a01  ..............*.
+00001b60: 1801 1803 0c03 2001 0601 0e01 0c01 0a01  ...... .........
+00001b70: 0801 0403 0a01 0201 0201 0201 02fd 0204  ................
+00001b80: 0201 0201 02fa 0407 02f9 0609 0803 0401  ................
+00001b90: 20ff 0604 0c01 0e01 0e03 1a02 1aff 0203   ...............
+00001ba0: 0c01 0c02 0e01 0201 12ff 0603 0c01 1001  ................
+00001bb0: 0201 0201 0c01 0afe 02ff 0406 0e02 0a01  ................
+00001bc0: 0e01 1601 0401 0201 0201 0201 0cfc 0606  ................
+00001bd0: 7226 0000 0029 0572 1a00 0000 7212 0000  r&...).r....r...
+00001be0: 0072 5100 0000 721e 0000 0072 1c00 0000  .rQ...r....r....
+00001bf0: 6306 0000 0000 0000 0000 0000 000b 0000  c...............
+00001c00: 0006 0000 0043 0000 0073 b400 0000 7400  .....C...s....t.
+00001c10: 7c01 8301 7d06 7401 a002 7c06 7403 a004  |...}.t...|.t...
+00001c20: 7c03 a101 1800 7403 a004 7c04 a101 1b00  |.....t...|.....
+00001c30: a101 a005 a100 7d06 7c02 6a06 6401 6b02  ......}.|.j.d.k.
+00001c40: 7242 7401 a007 7c06 6402 a102 7d07 6e0c  rBt...|.d...}.n.
+00001c50: 7401 a008 7c06 6403 a102 7d07 7c02 7c07  t...|.d...}.|.|.
+00001c60: 8301 a009 a100 a00a a100 7d08 7403 6a0b  ..........}.t.j.
+00001c70: 7c08 6404 6405 8d02 7d09 7c05 6400 7501  |.d.d...}.|.d.u.
+00001c80: 7284 740c 6600 6900 7c05 a401 8e01 7d0a  r.t.f.i.|.....}.
+00001c90: 6e06 740c 8300 7d0a 7401 a007 7c06 6402  n.t...}.t...|.d.
+00001ca0: a102 7d06 7c0a 6a0d 7c06 7c09 6406 6407  ..}.|.j.|.|.d.d.
+00001cb0: 8d03 0100 740e 7c0a 7c00 8302 0100 6400  ....t.|.|.....d.
+00001cc0: 5300 2908 4e72 5e00 0000 2902 7206 0000  S.).Nr^...).r...
+00001cd0: 0072 0400 0000 a904 7201 0000 0072 7100  .r......r....rq.
+00001ce0: 0000 7206 0000 0072 0400 0000 7206 0000  ..r....r....r...
+00001cf0: 00a9 01da 0461 7869 7372 0400 0000 2901  .....axisr....).
+00001d00: da07 636c 6173 7365 7329 0fda 176c 6f61  ..classes)...loa
+00001d10: 645f 6e70 795f 6669 6c65 735f 746f 5f61  d_npy_files_to_a
+00001d20: 7272 6179 725f 0000 0072 7a00 0000 727e  rrayr_...rz...r~
+00001d30: 0000 0072 7f00 0000 7278 0000 0072 7c00  ...r....rx...r|.
+00001d40: 0000 721d 0000 0072 8900 0000 7283 0000  ..r....r....r...
+00001d50: 0072 8500 0000 da06 6172 676d 6178 7208  .r......argmaxr.
+00001d60: 0000 0072 8600 0000 da0b 7361 7665 5f6f  ...r......save_o
+00001d70: 626a 6563 7429 0b72 1700 0000 721a 0000  bject).r....r...
+00001d80: 0072 1200 0000 7251 0000 0072 1e00 0000  .r....rQ...r....
+00001d90: 721c 0000 005a 0b74 7261 696e 5f70 6174  r....Z.train_pat
+00001da0: 6368 5a03 585f 745a 096d 6f64 656c 5f6f  chZ.X_tZ.model_o
+00001db0: 7574 da05 7072 6564 73da 0274 7372 2800  ut..preds..tsr(.
+00001dc0: 0000 7228 0000 0072 2900 0000 7243 0000  ..r(...r)...rC..
+00001dd0: 000c 0100 0073 1e00 0000 0008 0801 0401  .....s..........
+00001de0: 16ff 0803 0a01 0e02 0c02 1001 0e02 0801  ................
+00001df0: 1002 0601 0c01 1001 7243 0000 0063 0100  ........rC...c..
+00001e00: 0000 0000 0000 0000 0000 0900 0000 0600  ................
+00001e10: 0000 4300 0000 7372 0000 0067 007d 0164  ..C...sr...g.}.d
+00001e20: 0164 0267 027d 027c 0244 005d 4e7d 0374  .d.g.}.|.D.]N}.t
+00001e30: 006a 01a0 027c 007c 03a1 027d 0474 00a0  .j...|.|...}.t..
+00001e40: 037c 04a1 0144 005d 307d 057c 05a0 0464  .|...D.]0}.|...d
+00001e50: 03a1 0172 2c74 006a 01a0 027c 047c 05a1  ...r,t.j...|.|..
+00001e60: 027d 0674 05a0 067c 06a1 017d 077c 01a0  .}.t...|...}.|..
+00001e70: 077c 07a1 0101 0071 2c71 1074 056a 087c  .|.....q,q.t.j.|
+00001e80: 0164 0464 058d 027d 087c 0853 0029 064e  .d.d...}.|.S.).N
+00001e90: da01 30da 0131 7a04 2e6e 7079 7201 0000  ..0..1z..npyr...
+00001ea0: 0072 9500 0000 2909 7234 0000 0072 3500  .r....).r4...r5.
+00001eb0: 0000 7236 0000 00da 076c 6973 7464 6972  ..r6.....listdir
+00001ec0: da08 656e 6473 7769 7468 727e 0000 0072  ..endswithr~...r
+00001ed0: 3900 0000 724b 0000 00da 0573 7461 636b  9...rK.....stack
+00001ee0: 2909 da08 6261 7365 5f64 6972 da06 6172  )...base_dir..ar
+00001ef0: 7261 7973 5a08 7375 625f 6469 7273 da07  raysZ.sub_dirs..
+00001f00: 7375 625f 6469 725a 0c73 7562 5f64 6972  sub_dirZ.sub_dir
+00001f10: 5f70 6174 68da 0466 696c 65da 0966 696c  _path..file..fil
+00001f20: 655f 7061 7468 727f 0000 005a 0b66 696e  e_pathr....Z.fin
+00001f30: 616c 5f61 7272 6179 7228 0000 0072 2800  al_arrayr(...r(.
+00001f40: 0000 7229 0000 0072 9800 0000 2901 0000  ..r)...r....)...
+00001f50: 7316 0000 0000 0104 0108 0208 010e 010e  s...............
+00001f60: 010a 010e 010a 010e 030e 0172 9800 0000  ...........r....
+00001f70: 6305 0000 0000 0000 0000 0000 0007 0000  c...............
+00001f80: 0007 0000 0043 0000 0073 3800 0000 7c00  .....C...s8...|.
+00001f90: 7c03 1400 7c02 1700 7d05 7c01 7c05 7c04  |...|...}.|.|.|.
+00001fa0: 1b00 6400 6400 8502 6400 6400 6400 6400  ..d.d...d.d.d.d.
+00001fb0: 8502 6604 1900 1400 7d06 7c06 7c02 1800  ..f.....}.|.|...
+00001fc0: 7c03 1b00 5300 7225 0000 0072 2800 0000  |...S.r%...r(...
+00001fd0: 2907 7267 0000 0072 6900 0000 7251 0000  ).rg...ri...rQ..
+00001fe0: 0072 1e00 0000 7268 0000 005a 0a75 6e6e  .r....rh...Z.unn
+00001ff0: 6f72 6d65 645f 795a 096e 6577 5f70 6174  ormed_yZ.new_pat
+00002000: 6368 7228 0000 0072 2800 0000 7229 0000  chr(...r(...r)..
+00002010: 0072 6600 0000 3a01 0000 7306 0000 0000  .rf...:...s.....
+00002020: 010c 0120 0172 6600 0000 6302 0000 0000  ... .rf...c.....
+00002030: 0000 0000 0000 0005 0000 0004 0000 0003  ................
+00002040: 0000 0073 3400 0000 4700 8700 6601 6401  ...s4...G...f.d.
+00002050: 6402 8408 6402 7400 6a01 6a02 8303 7d02  d...d.t.j.j...}.
+00002060: 7c02 8300 7d03 7400 6a01 a003 7c03 7c01  |...}.t.j...|.|.
+00002070: a102 7d04 7c04 7c03 6602 5300 2903 6116  ..}.|.|.f.S.).a.
+00002080: 0100 000a 2020 2020 4164 6420 616e 2069  ....    Add an i
+00002090: 6e69 7469 616c 697a 6174 696f 6e20 6c61  nitialization la
+000020a0: 7965 7220 746f 2074 6865 206d 6f64 656c  yer to the model
+000020b0: 2e0a 0a20 2020 2041 7267 733a 0a20 2020  ...    Args:.   
+000020c0: 2020 2020 2069 6e69 745f 6675 6e20 2863       init_fun (c
+000020d0: 616c 6c61 626c 6529 3a20 496e 6974 6961  allable): Initia
+000020e0: 6c69 7a61 7469 6f6e 2066 756e 6374 696f  lization functio
+000020f0: 6e2e 0a20 2020 2020 2020 206d 6f64 656c  n..        model
+00002100: 2028 746f 7263 682e 6e6e 2e4d 6f64 756c   (torch.nn.Modul
+00002110: 6529 3a20 4f72 6967 696e 616c 206d 6f64  e): Original mod
+00002120: 656c 2e0a 0a20 2020 2052 6574 7572 6e73  el...    Returns
+00002130: 3a0a 2020 2020 2020 2020 7475 706c 653a  :.        tuple:
+00002140: 2028 746f 7263 682e 6e6e 2e4d 6f64 756c   (torch.nn.Modul
+00002150: 652c 2074 6f72 6368 2e6e 6e2e 4d6f 6475  e, torch.nn.Modu
+00002160: 6c65 2920 2d20 4d6f 6469 6669 6564 206d  le) - Modified m
+00002170: 6f64 656c 2061 6e64 2069 6e70 7574 2074  odel and input t
+00002180: 7261 6e73 666f 726d 6174 696f 6e20 6c61  ransformation la
+00002190: 7965 722e 0a20 2020 2063 0000 0000 0000  yer..    c......
+000021a0: 0000 0000 0000 0000 0000 0300 0000 0000  ................
+000021b0: 0000 7318 0000 0065 005a 0164 005a 0287  ..s....e.Z.d.Z..
+000021c0: 0066 0164 0164 0284 085a 0364 0353 0029  .f.d.d...Z.d.S.)
+000021d0: 047a 2061 6464 5f69 6e69 745f 6c61 7965  .z add_init_laye
+000021e0: 722e 3c6c 6f63 616c 733e 2e49 6e70 7574  r.<locals>.Input
+000021f0: 4675 6e63 0200 0000 0000 0000 0000 0000  Func............
+00002200: 0200 0000 0400 0000 1300 0000 7314 0000  ............s...
+00002210: 0074 00a0 0188 007c 0183 0164 01a1 02a0  .t.....|...d....
+00002220: 02a1 0053 0029 024e 7294 0000 0029 0372  ...S.).Nr....).r
+00002230: 5f00 0000 7289 0000 0072 7800 0000 2902  _...r....rx...).
+00002240: da04 7365 6c66 da05 696e 7075 74a9 0172  ..self..input..r
+00002250: 9200 0000 7228 0000 0072 2900 0000 da07  ....r(...r).....
+00002260: 666f 7277 6172 644d 0100 0073 0200 0000  forwardM...s....
+00002270: 0001 7a28 6164 645f 696e 6974 5f6c 6179  ..z(add_init_lay
+00002280: 6572 2e3c 6c6f 6361 6c73 3e2e 496e 7075  er.<locals>.Inpu
+00002290: 7446 756e 2e66 6f72 7761 7264 4e29 04da  tFun.forwardN)..
+000022a0: 085f 5f6e 616d 655f 5fda 0a5f 5f6d 6f64  .__name__..__mod
+000022b0: 756c 655f 5fda 0c5f 5f71 7561 6c6e 616d  ule__..__qualnam
+000022c0: 655f 5f72 aa00 0000 7228 0000 0072 a900  e__r....r(...r..
+000022d0: 0000 7228 0000 0072 2900 0000 da08 496e  ..r(...r).....In
+000022e0: 7075 7446 756e 4c01 0000 7302 0000 0008  putFunL...s.....
+000022f0: 0172 ae00 0000 2904 725f 0000 0072 6000  .r....).r_...r`.
+00002300: 0000 da06 4d6f 6475 6c65 da0a 5365 7175  ....Module..Sequ
+00002310: 656e 7469 616c 2905 7292 0000 0072 1200  ential).r....r..
+00002320: 0000 72ae 0000 0072 9100 0000 5a0e 636f  ..r....r....Z.co
+00002330: 6d70 6c65 7465 5f6d 6f64 656c 7228 0000  mplete_modelr(..
+00002340: 0072 a900 0000 7229 0000 0072 7d00 0000  .r....r)...r}...
+00002350: 4001 0000 7308 0000 0000 0c18 0406 010e  @...s...........
+00002360: 0172 7d00 0000 2903 7277 0000 0072 7300  .r}...).rw...rs.
+00002370: 0000 725b 0000 0063 0200 0000 0000 0000  ..r[...c........
+00002380: 0000 0000 0400 0000 0300 0000 0300 0000  ................
+00002390: 7338 0000 0074 0088 0074 0183 0272 1088  s8...t...t...r..
+000023a0: 0066 0189 0087 0066 0164 0164 0284 0874  .f.....f.d.d...t
+000023b0: 027c 006a 0383 0144 0083 017d 027c 006a  .|.j...D...}.|.j
+000023c0: 047c 0264 038d 017d 037c 0353 0029 0461  .|.d...}.|.S.).a
+000023d0: 2701 0000 0a20 2020 2043 6f6d 7075 7465  '....    Compute
+000023e0: 2074 6865 206d 6561 6e20 616c 6f6e 6720   the mean along 
+000023f0: 616c 6c20 6469 6d65 6e73 696f 6e73 2065  all dimensions e
+00002400: 7863 6570 7420 7468 6f73 6520 7370 6563  xcept those spec
+00002410: 6966 6965 6420 696e 2070 7265 7365 7276  ified in preserv
+00002420: 6541 7869 732e 0a0a 2020 2020 4172 6773  eAxis...    Args
+00002430: 3a0a 2020 2020 2020 2020 7465 6e73 6f72  :.        tensor
+00002440: 2028 746f 7263 682e 5465 6e73 6f72 293a   (torch.Tensor):
+00002450: 2049 6e70 7574 2074 656e 736f 722e 0a20   Input tensor.. 
+00002460: 2020 2020 2020 2070 7265 7365 7276 6541         preserveA
+00002470: 7869 7320 2874 7570 6c65 2c20 6f70 7469  xis (tuple, opti
+00002480: 6f6e 616c 293a 2044 696d 656e 7369 6f6e  onal): Dimension
+00002490: 7320 746f 2070 7265 7365 7276 652e 2044  s to preserve. D
+000024a0: 6566 6175 6c74 7320 746f 204e 6f6e 652e  efaults to None.
+000024b0: 0a0a 2020 2020 5265 7475 726e 733a 0a20  ..    Returns:. 
+000024c0: 2020 2020 2020 2074 6f72 6368 2e54 656e         torch.Ten
+000024d0: 736f 723a 2054 656e 736f 7220 7769 7468  sor: Tensor with
+000024e0: 2070 7265 7365 7276 6564 2064 696d 656e   preserved dimen
+000024f0: 7369 6f6e 732e 0a20 2020 2063 0100 0000  sions..    c....
+00002500: 0000 0000 0000 0000 0200 0000 0400 0000  ................
+00002510: 1300 0000 7318 0000 0067 007c 005d 107d  ....s....g.|.].}
+00002520: 017c 0188 0076 0172 047c 0191 0271 0453  .|...v.r.|...q.S
+00002530: 0072 2800 0000 7228 0000 0029 0272 2b00  .r(...r(...).r+.
+00002540: 0000 7252 0000 0072 7200 0000 7228 0000  ..rR...rr...r(..
+00002550: 0072 2900 0000 722d 0000 0065 0100 0072  .r)...r-...e...r
+00002560: 2e00 0000 7a2c 6d65 616e 5f70 7265 7365  ....z,mean_prese
+00002570: 7276 655f 6469 6d65 6e73 696f 6e73 2e3c  rve_dimensions.<
+00002580: 6c6f 6361 6c73 3e2e 3c6c 6973 7463 6f6d  locals>.<listcom
+00002590: 703e 725c 0000 0029 05da 0a69 7369 6e73  p>r\...)...isins
+000025a0: 7461 6e63 65da 0369 6e74 7245 0000 0072  tance..intrE...r
+000025b0: 8b00 0000 721d 0000 0029 0472 7700 0000  ....r....).rw...
+000025c0: 7273 0000 005a 0e64 696d 735f 746f 5f72  rs...Z.dims_to_r
+000025d0: 6564 7563 65da 0672 6573 756c 7472 2800  educe..resultr(.
+000025e0: 0000 7272 0000 0072 2900 0000 728a 0000  ..rr...r)...r...
+000025f0: 0055 0100 0073 0a00 0000 000d 0a01 0602  .U...s..........
+00002600: 1801 0c01 728a 0000 0063 0200 0000 0000  ....r....c......
+00002610: 0000 0000 0000 0300 0000 0800 0000 4300  ..............C.
+00002620: 0000 733c 0000 0074 007c 0164 0183 028f  ..s<...t.|.d....
+00002630: 1e7d 0274 01a0 027c 007c 0264 02a1 0301  .}.t...|.|.d....
+00002640: 0057 0064 0004 0004 0083 0301 006e 1031  .W.d.........n.1
+00002650: 0073 2e30 0001 0001 0001 0059 0001 0064  .s.0.......Y...d
+00002660: 0053 0029 034e da02 7762 e9ff ffff ff29  .S.).N..wb.....)
+00002670: 0372 3300 0000 da06 7069 636b 6c65 da04  .r3.....pickle..
+00002680: 6475 6d70 2903 da03 6f62 6ada 0866 696c  dump)...obj..fil
+00002690: 656e 616d 655a 046f 7574 7072 2800 0000  enameZ.outpr(...
+000026a0: 7228 0000 0072 2900 0000 729a 0000 006a  r(...r)...r....j
+000026b0: 0100 0073 0400 0000 0001 0c01 729a 0000  ...s........r...
+000026c0: 0029 084e 720f 0000 004e 4e72 0600 0000  .).Nr....NNr....
+000026d0: 4e46 4e29 0546 4e4e 4e72 0f00 0000 2901  NFN).FNNNr....).
+000026e0: 4e29 014e 292e 7234 0000 0072 3800 0000  N).N).r4...r8...
+000026f0: da07 5f70 6963 6b6c 6572 b600 0000 7285  .._pickler....r.
+00002700: 0000 0072 7e00 0000 da06 7061 6e64 6173  ...r~.....pandas
+00002710: da02 7064 da06 7479 7069 6e67 7202 0000  ..pd..typingr...
+00002720: 0072 5f00 0000 7203 0000 00da 0864 6174  .r_...r......dat
+00002730: 6173 6574 7372 0500 0000 7288 0000 0072  asetsr....r....r
+00002740: 0700 0000 da0a 636f 6e66 6964 656e 6365  ......confidence
+00002750: 7208 0000 00da 0d63 6f6e 6669 6775 7261  r......configura
+00002760: 7469 6f6e 7209 0000 0072 0a00 0000 720b  tionr....r....r.
+00002770: 0000 0072 0c00 0000 7277 0000 00da 0766  ...r....rw.....f
+00002780: 6c6f 6174 3332 7282 0000 0072 b200 0000  loat32r....r....
+00002790: 7260 0000 0072 af00 0000 da04 6c69 7374  r`...r......list
+000027a0: 728c 0000 00da 0944 6174 6146 7261 6d65  r......DataFrame
+000027b0: 7278 0000 00da 0373 7472 da04 626f 6f6c  rx.....str..bool
+000027c0: 7257 0000 00da 076e 6461 7272 6179 7226  rW.....ndarrayr&
+000027d0: 0000 0072 4300 0000 7298 0000 0072 6600  ...rC...r....rf.
+000027e0: 0000 727d 0000 00da 0654 656e 736f 72da  ..r}.....Tensor.
+000027f0: 0574 7570 6c65 728a 0000 0072 9a00 0000  .tupler....r....
+00002800: 7228 0000 0072 2800 0000 7228 0000 0072  r(...r(...r(...r
+00002810: 2900 0000 da08 3c6d 6f64 756c 653e 0100  ).....<module>..
+00002820: 0000 7396 0000 0008 0108 0108 0108 0108  ..s.............
+00002830: 010c 0108 020c 050c 010c 010c 0118 0710  ................
+00002840: 0900 0100 0100 0100 0100 0100 0100 0100  ................
+00002850: f302 0102 0102 0106 0102 0102 0104 0102  ................
+00002860: 0102 0102 0102 0102 0102 0106 f30c 7600  ..............v.
+00002870: 0100 0100 0100 0100 f202 0104 0104 0102  ................
+00002880: 0106 0102 0102 0104 0104 0102 0102 0102  ................
+00002890: 0102 0102 0102 0102 f10c 7f00 0c00 fa02  ................
+000028a0: 0202 0106 0102 0102 0106 fa0c 1d08 1108  ................
+000028b0: 0608 1600 ff02 0106 0104 fe0c 15         .............
```

### Comparing `morpheus_spatial-0.3.0/src/morpheus/counterfactual/cf.py` & `morpheus_spatial-0.4.0/src/morpheus/counterfactual/cf_in_progress.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 import torch
 import torch.optim as optim
 
 from ..api.defaults import DEFAULT_DATA, DEFAULT_META
 from ..api.interfaces import Explainer, Explanation, FitMixin
 
 
-
 class Counterfactual(Explainer, FitMixin):
     def __init__(
         self,
         predict: Union[Callable[[np.ndarray], np.ndarray], torch.nn.Module],
         input_transform: Union[Callable[[np.ndarray], np.ndarray], torch.nn.Module],
         shape: tuple,
         kappa: float = 0.0,
```

### Comparing `morpheus_spatial-0.3.0/src/morpheus/counterfactual/generate.py` & `morpheus_spatial-0.4.0/src/morpheus/counterfactual/generate.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 import _pickle as pickle
 import numpy as np
 import pandas as pd
 from typing import Optional
 import torch
 
 from tqdm import tqdm
-from multiprocessing import Pool
 
 # import multiprocessing
 
 
 from ..datasets import SpatialDataset
 from .cf import Counterfactual
 from ..confidence import TrustScore
@@ -236,33 +235,36 @@
         cf = input_transform(torch.from_numpy(cf[None, :]))
         counterfactual_probabilities = (
             altered_model(cf) if model.arch == "mlp" else model(cf)
         )
         if model.arch != "mlp":
             cf = torch.permute(cf, (0, 2, 3, 1))
 
-        print(f"Counterfactual probability: {cf_prob}")
-        print(f"Computed probability: {counterfactual_probabilities}")
+        print(f"Counterfactual probability: {counterfactual_probabilities}")
         X_perturbed = mean_preserve_dimensions(
             cf * stdev + mu, preserveAxis=cf.ndim - 1
         )
         original_patch = X_mean * stdev + mu
         cf_delta = (X_perturbed - original_patch) / original_patch * 100
-        print(f"cf delta: {cf_delta}")
-        cf_perturbed = dict(zip(channel[is_perturbed], cf_delta[is_perturbed].numpy()))
+        cf_perturbed = dict(
+            zip(
+                np.array(channel)[is_perturbed],
+                cf_delta[is_perturbed].numpy(),
+            )
+        )
         print(f"cf perturbed: {cf_perturbed}")
 
         if save_dir is not None:
             os.makedirs(save_dir, exist_ok=True)
             saved_file = os.path.join(save_dir, f"patch_{patch_id}.npz")
             np.savez(
                 saved_file,
                 explanation=explanation,
                 cf_perturbed=cf_perturbed,
-                channel_to_perturb=channel[is_perturbed],
+                channel_to_perturb=np.array(channel)[is_perturbed],
             )
     return explanation
 
 
 def build_kdtree(
     kdtree_path,
     train_data: str,
```

### Comparing `morpheus_spatial-0.3.0/src/morpheus/datasets/__pycache__/spatial_dataset.cpython-39.pyc` & `morpheus_spatial-0.4.0/src/morpheus/datasets/__pycache__/spatial_dataset.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `morpheus_spatial-0.3.0/src/morpheus/datasets/__pycache__/torch_dataset.cpython-39.pyc` & `morpheus_spatial-0.4.0/src/morpheus/datasets/__pycache__/torch_dataset.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `morpheus_spatial-0.3.0/src/morpheus/datasets/spatial_dataset.py` & `morpheus_spatial-0.4.0/src/morpheus/datasets/spatial_dataset.py`

 * *Files identical despite different names*

### Comparing `morpheus_spatial-0.3.0/src/morpheus/datasets/torch_dataset.py` & `morpheus_spatial-0.4.0/src/morpheus/datasets/torch_dataset.py`

 * *Files identical despite different names*

### Comparing `morpheus_spatial-0.3.0/src/morpheus/utils/__pycache__/saving.cpython-39.pyc` & `morpheus_spatial-0.4.0/src/morpheus/utils/__pycache__/saving.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `morpheus_spatial-0.3.0/src/morpheus/utils/patchify.py` & `morpheus_spatial-0.4.0/src/morpheus/utils/patchify.py`

 * *Files identical despite different names*

### Comparing `morpheus_spatial-0.3.0/src/morpheus/utils/saving.py` & `morpheus_spatial-0.4.0/src/morpheus/utils/saving.py`

 * *Files identical despite different names*

### Comparing `morpheus_spatial-0.3.0/PKG-INFO` & `morpheus_spatial-0.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: morpheus-spatial
-Version: 0.3.0
+Version: 0.4.0
 Summary: 
 Author: neonine2
 Author-email: jerry.wang95@yahoo.ca
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.9,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: dill (>=0.3.8,<0.4.0)
 Requires-Dist: h5py (>=3.10.0,<4.0.0)
-Requires-Dist: lightning (>=2.2.0.post0,<3.0.0)
+Requires-Dist: lightning (>=2.0.0,<3.0.0)
 Requires-Dist: pandas (>=2.2.1,<3.0.0)
 Requires-Dist: scikit-learn (>=1.4.1.post1,<2.0.0)
-Requires-Dist: torchvision (>=0.17.1,<0.18.0)
+Requires-Dist: tensorflow (==2.11.1)
+Requires-Dist: torch (==2.0.0)
+Requires-Dist: torchvision (>=0.15.1,<0.16.0)
 Description-Content-Type: text/markdown
 
 # Morpheus: Generating Therapeutic Strategies using Spatial Omics
 
 ## Introduction
 
 Morpheus is an integrated deep learning framework that takes large scale spatial omics profiles of patient tumors, and combines a formulation of T-cell infiltration prediction as a self-supervised machine learning problem with a counterfactual optimization strategy to generate minimal tumor perturbations predicted to boost T-cell infiltration.
```

