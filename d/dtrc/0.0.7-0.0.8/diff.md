# Comparing `tmp/dtrc-0.0.7.tar.gz` & `tmp/dtrc-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dtrc-0.0.7.tar", last modified: Wed Apr  3 11:43:36 2024, max compression
+gzip compressed data, was "dtrc-0.0.8.tar", last modified: Sat Apr  6 19:33:13 2024, max compression
```

## Comparing `dtrc-0.0.7.tar` & `dtrc-0.0.8.tar`

### file list

```diff
@@ -1,28 +1,30 @@
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2024-04-03 11:43:36.551129 dtrc-0.0.7/
--rw-r--r--   0 solst      (501) staff       (20)    11337 2023-11-17 13:08:05.000000 dtrc-0.0.7/LICENSE
--rw-r--r--   0 solst      (501) staff       (20)      111 2023-11-17 13:08:05.000000 dtrc-0.0.7/MANIFEST.in
--rw-r--r--   0 solst      (501) staff       (20)     3853 2024-04-03 11:43:36.550914 dtrc-0.0.7/PKG-INFO
--rw-r--r--   0 solst      (501) staff       (20)     2720 2023-12-22 19:25:54.000000 dtrc-0.0.7/README.md
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2024-04-03 11:43:36.549393 dtrc-0.0.7/dtrc/
--rw-r--r--   0 solst      (501) staff       (20)      579 2024-04-03 11:43:20.000000 dtrc-0.0.7/dtrc/__init__.py
--rw-r--r--   0 solst      (501) staff       (20)     2976 2024-04-03 11:43:20.000000 dtrc-0.0.7/dtrc/_modidx.py
--rw-r--r--   0 solst      (501) staff       (20)      626 2024-04-03 11:43:20.000000 dtrc-0.0.7/dtrc/atyp.py
--rw-r--r--   0 solst      (501) staff       (20)     2893 2024-04-03 11:43:20.000000 dtrc-0.0.7/dtrc/cats.py
--rw-r--r--   0 solst      (501) staff       (20)      375 2024-04-03 11:43:20.000000 dtrc-0.0.7/dtrc/cons.py
--rw-r--r--   0 solst      (501) staff       (20)     4674 2024-04-03 11:43:20.000000 dtrc-0.0.7/dtrc/data.py
--rw-r--r--   0 solst      (501) staff       (20)      498 2024-04-03 11:43:20.000000 dtrc-0.0.7/dtrc/enum.py
--rw-r--r--   0 solst      (501) staff       (20)    16565 2024-04-03 11:43:20.000000 dtrc-0.0.7/dtrc/make.py
--rw-r--r--   0 solst      (501) staff       (20)     4791 2024-04-03 11:43:20.000000 dtrc-0.0.7/dtrc/poly.py
--rw-r--r--   0 solst      (501) staff       (20)     5350 2024-04-03 11:43:20.000000 dtrc-0.0.7/dtrc/trig.py
--rw-r--r--   0 solst      (501) staff       (20)      498 2024-04-03 11:43:20.000000 dtrc-0.0.7/dtrc/util.py
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2024-04-03 11:43:36.550445 dtrc-0.0.7/dtrc.egg-info/
--rw-r--r--   0 solst      (501) staff       (20)     3853 2024-04-03 11:43:36.000000 dtrc-0.0.7/dtrc.egg-info/PKG-INFO
--rw-r--r--   0 solst      (501) staff       (20)      398 2024-04-03 11:43:36.000000 dtrc-0.0.7/dtrc.egg-info/SOURCES.txt
--rw-r--r--   0 solst      (501) staff       (20)        1 2024-04-03 11:43:36.000000 dtrc-0.0.7/dtrc.egg-info/dependency_links.txt
--rw-r--r--   0 solst      (501) staff       (20)       30 2024-04-03 11:43:36.000000 dtrc-0.0.7/dtrc.egg-info/entry_points.txt
--rw-r--r--   0 solst      (501) staff       (20)        1 2024-03-24 17:50:00.000000 dtrc-0.0.7/dtrc.egg-info/not-zip-safe
--rw-r--r--   0 solst      (501) staff       (20)      142 2024-04-03 11:43:36.000000 dtrc-0.0.7/dtrc.egg-info/requires.txt
--rw-r--r--   0 solst      (501) staff       (20)        5 2024-04-03 11:43:36.000000 dtrc-0.0.7/dtrc.egg-info/top_level.txt
--rw-r--r--   0 solst      (501) staff       (20)      917 2024-04-03 11:43:17.000000 dtrc-0.0.7/settings.ini
--rw-r--r--   0 solst      (501) staff       (20)       38 2024-04-03 11:43:36.551173 dtrc-0.0.7/setup.cfg
--rw-r--r--   0 solst      (501) staff       (20)     2585 2023-11-17 13:08:05.000000 dtrc-0.0.7/setup.py
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2024-04-06 19:33:13.478735 dtrc-0.0.8/
+-rw-r--r--   0 solst      (501) staff       (20)    11337 2023-11-17 13:08:05.000000 dtrc-0.0.8/LICENSE
+-rw-r--r--   0 solst      (501) staff       (20)      111 2023-11-17 13:08:05.000000 dtrc-0.0.8/MANIFEST.in
+-rw-r--r--   0 solst      (501) staff       (20)     3895 2024-04-06 19:33:13.478489 dtrc-0.0.8/PKG-INFO
+-rw-r--r--   0 solst      (501) staff       (20)     2720 2023-12-22 19:25:54.000000 dtrc-0.0.8/README.md
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2024-04-06 19:33:13.476136 dtrc-0.0.8/dtrc/
+-rw-r--r--   0 solst      (501) staff       (20)      641 2024-04-06 19:33:05.000000 dtrc-0.0.8/dtrc/__init__.py
+-rw-r--r--   0 solst      (501) staff       (20)     8241 2024-04-06 19:33:05.000000 dtrc-0.0.8/dtrc/_modidx.py
+-rw-r--r--   0 solst      (501) staff       (20)      626 2024-04-06 19:33:05.000000 dtrc-0.0.8/dtrc/atyp.py
+-rw-r--r--   0 solst      (501) staff       (20)     3885 2024-04-06 19:33:05.000000 dtrc-0.0.8/dtrc/cats.py
+-rw-r--r--   0 solst      (501) staff       (20)      589 2024-04-06 19:33:05.000000 dtrc-0.0.8/dtrc/cons.py
+-rw-r--r--   0 solst      (501) staff       (20)     4674 2024-04-06 19:33:05.000000 dtrc-0.0.8/dtrc/data.py
+-rw-r--r--   0 solst      (501) staff       (20)     6105 2024-04-06 19:33:05.000000 dtrc-0.0.8/dtrc/dmod.py
+-rw-r--r--   0 solst      (501) staff       (20)     3889 2024-04-06 19:33:05.000000 dtrc-0.0.8/dtrc/dset.py
+-rw-r--r--   0 solst      (501) staff       (20)      498 2024-04-06 19:33:05.000000 dtrc-0.0.8/dtrc/enum.py
+-rw-r--r--   0 solst      (501) staff       (20)    16565 2024-04-06 19:33:05.000000 dtrc-0.0.8/dtrc/make.py
+-rw-r--r--   0 solst      (501) staff       (20)     4791 2024-04-06 19:33:05.000000 dtrc-0.0.8/dtrc/poly.py
+-rw-r--r--   0 solst      (501) staff       (20)     5350 2024-04-06 19:33:05.000000 dtrc-0.0.8/dtrc/trig.py
+-rw-r--r--   0 solst      (501) staff       (20)     2548 2024-04-06 19:33:05.000000 dtrc-0.0.8/dtrc/util.py
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2024-04-06 19:33:13.477471 dtrc-0.0.8/dtrc.egg-info/
+-rw-r--r--   0 solst      (501) staff       (20)     3895 2024-04-06 19:33:13.000000 dtrc-0.0.8/dtrc.egg-info/PKG-INFO
+-rw-r--r--   0 solst      (501) staff       (20)      424 2024-04-06 19:33:13.000000 dtrc-0.0.8/dtrc.egg-info/SOURCES.txt
+-rw-r--r--   0 solst      (501) staff       (20)        1 2024-04-06 19:33:13.000000 dtrc-0.0.8/dtrc.egg-info/dependency_links.txt
+-rw-r--r--   0 solst      (501) staff       (20)       30 2024-04-06 19:33:13.000000 dtrc-0.0.8/dtrc.egg-info/entry_points.txt
+-rw-r--r--   0 solst      (501) staff       (20)        1 2024-03-24 17:50:00.000000 dtrc-0.0.8/dtrc.egg-info/not-zip-safe
+-rw-r--r--   0 solst      (501) staff       (20)      154 2024-04-06 19:33:13.000000 dtrc-0.0.8/dtrc.egg-info/requires.txt
+-rw-r--r--   0 solst      (501) staff       (20)        5 2024-04-06 19:33:13.000000 dtrc-0.0.8/dtrc.egg-info/top_level.txt
+-rw-r--r--   0 solst      (501) staff       (20)      929 2024-04-06 19:33:03.000000 dtrc-0.0.8/settings.ini
+-rw-r--r--   0 solst      (501) staff       (20)       38 2024-04-06 19:33:13.478774 dtrc-0.0.8/setup.cfg
+-rw-r--r--   0 solst      (501) staff       (20)     2585 2023-11-17 13:08:05.000000 dtrc-0.0.8/setup.py
```

### Comparing `dtrc-0.0.7/LICENSE` & `dtrc-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `dtrc-0.0.7/PKG-INFO` & `dtrc-0.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dtrc
-Version: 0.0.7
+Version: 0.0.8
 Summary: data torch
 Home-page: https://github.com/dsm-72/dtrc
 Author: dsm-72
 Author-email: sumner.magruder@yale.edu
 License: Apache Software License 2.0
 Keywords: dtrc data pytorch torch trc
 Classifier: Development Status :: 4 - Beta
@@ -26,14 +26,16 @@
 Requires-Dist: uscr
 Requires-Dist: etrc
 Requires-Dist: slcs
 Requires-Dist: lmsg
 Requires-Dist: dtyp
 Requires-Dist: utrc
 Requires-Dist: zipr
+Requires-Dist: pcts
+Requires-Dist: seeder
 Provides-Extra: dev
 Requires-Dist: numpy; extra == "dev"
 Requires-Dist: pandas; extra == "dev"
 Requires-Dist: matplotlib; extra == "dev"
 Requires-Dist: torch; extra == "dev"
 Requires-Dist: pytorch_lightning; extra == "dev"
 Requires-Dist: torchvision; extra == "dev"
```

### Comparing `dtrc-0.0.7/README.md` & `dtrc-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `dtrc-0.0.7/dtrc/__init__.py` & `dtrc-0.0.8/dtrc/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,23 +1,25 @@
-__version__ = "0.0.7"
+__version__ = "0.0.8"
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/00__init__.ipynb.
 
 # %% auto 0
 __all__ = []
 
 # %% ../nbs/00__init__.ipynb 3
 from itertools import chain
-from . import (cons, atyp, enum, util, trig, cats, data, poly, make, )
+from . import (cons, atyp, enum, util, trig, cats, data, poly, make, dset, dmod)
 from .cons import *
 from .atyp import *
 from .enum import *
 from .util import *
 from .trig import *
 from .cats import *
 from .data import *
 from .poly import *
 from .make import *
+from .dset import *
+from .dmod import *
 
 # %% ../nbs/00__init__.ipynb 4
 __all__ = sorted(set(chain(*[
-    mod.__all__ for mod in (cons, atyp, enum, util, trig, cats, data, poly, make, )
+    mod.__all__ for mod in (cons, atyp, enum, util, trig, cats, data, poly, make, dset, dmod, )
 ])))
```

### Comparing `dtrc-0.0.7/dtrc/atyp.py` & `dtrc-0.0.8/dtrc/atyp.py`

 * *Files identical despite different names*

### Comparing `dtrc-0.0.7/dtrc/data.py` & `dtrc-0.0.8/dtrc/data.py`

 * *Files identical despite different names*

### Comparing `dtrc-0.0.7/dtrc/make.py` & `dtrc-0.0.8/dtrc/make.py`

 * *Files identical despite different names*

### Comparing `dtrc-0.0.7/dtrc/poly.py` & `dtrc-0.0.8/dtrc/poly.py`

 * *Files identical despite different names*

### Comparing `dtrc-0.0.7/dtrc/trig.py` & `dtrc-0.0.8/dtrc/trig.py`

 * *Files identical despite different names*

### Comparing `dtrc-0.0.7/dtrc.egg-info/PKG-INFO` & `dtrc-0.0.8/dtrc.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dtrc
-Version: 0.0.7
+Version: 0.0.8
 Summary: data torch
 Home-page: https://github.com/dsm-72/dtrc
 Author: dsm-72
 Author-email: sumner.magruder@yale.edu
 License: Apache Software License 2.0
 Keywords: dtrc data pytorch torch trc
 Classifier: Development Status :: 4 - Beta
@@ -26,14 +26,16 @@
 Requires-Dist: uscr
 Requires-Dist: etrc
 Requires-Dist: slcs
 Requires-Dist: lmsg
 Requires-Dist: dtyp
 Requires-Dist: utrc
 Requires-Dist: zipr
+Requires-Dist: pcts
+Requires-Dist: seeder
 Provides-Extra: dev
 Requires-Dist: numpy; extra == "dev"
 Requires-Dist: pandas; extra == "dev"
 Requires-Dist: matplotlib; extra == "dev"
 Requires-Dist: torch; extra == "dev"
 Requires-Dist: pytorch_lightning; extra == "dev"
 Requires-Dist: torchvision; extra == "dev"
```

### Comparing `dtrc-0.0.7/settings.ini` & `dtrc-0.0.8/settings.ini`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = dtrc
 lib_name = dtrc
-version = 0.0.7
+version = 0.0.8
 min_python = 3.11
 license = apache2
 black_formatting = False
 doc_path = _docs
 lib_path = dtrc
 nbs_path = nbs
 recursive = True
@@ -29,10 +29,10 @@
 conda_user = dsm-72
 jupyter_hooks = True
 clean_ids = True
 clear_all = False
 readme_nb = index.ipynb
 allowed_metadata_keys = 
 allowed_cell_metadata_keys = 
-requirements = astr atup chck dref lull nchr nlit quac uscr etrc slcs lmsg dtyp utrc zipr
+requirements = astr atup chck dref lull nchr nlit quac uscr etrc slcs lmsg dtyp utrc zipr pcts seeder
 dev_requirements = numpy pandas matplotlib torch pytorch_lightning torchvision
```

### Comparing `dtrc-0.0.7/setup.py` & `dtrc-0.0.8/setup.py`

 * *Files identical despite different names*

