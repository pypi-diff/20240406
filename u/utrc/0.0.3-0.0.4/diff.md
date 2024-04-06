# Comparing `tmp/utrc-0.0.3.tar.gz` & `tmp/utrc-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "utrc-0.0.3.tar", last modified: Thu Apr  4 12:39:58 2024, max compression
+gzip compressed data, was "utrc-0.0.4.tar", last modified: Sat Apr  6 14:45:17 2024, max compression
```

## Comparing `utrc-0.0.3.tar` & `utrc-0.0.4.tar`

### file list

```diff
@@ -1,36 +1,39 @@
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2024-04-04 12:39:58.181978 utrc-0.0.3/
--rw-r--r--   0 solst      (501) staff       (20)    11337 2024-02-26 19:42:52.000000 utrc-0.0.3/LICENSE
--rw-r--r--   0 solst      (501) staff       (20)      111 2024-02-26 19:42:52.000000 utrc-0.0.3/MANIFEST.in
--rw-r--r--   0 solst      (501) staff       (20)     3841 2024-04-04 12:39:58.181769 utrc-0.0.3/PKG-INFO
--rw-r--r--   0 solst      (501) staff       (20)     2720 2024-03-14 20:37:52.000000 utrc-0.0.3/README.md
--rw-r--r--   0 solst      (501) staff       (20)      920 2024-04-02 17:48:34.000000 utrc-0.0.3/settings.ini
--rw-r--r--   0 solst      (501) staff       (20)       38 2024-04-04 12:39:58.182012 utrc-0.0.3/setup.cfg
--rw-r--r--   0 solst      (501) staff       (20)     2585 2024-02-26 19:42:52.000000 utrc-0.0.3/setup.py
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2024-04-04 12:39:58.179904 utrc-0.0.3/utrc/
--rw-r--r--   0 solst      (501) staff       (20)      936 2024-04-04 12:39:47.000000 utrc-0.0.3/utrc/__init__.py
--rw-r--r--   0 solst      (501) staff       (20)    20577 2024-04-04 12:39:47.000000 utrc-0.0.3/utrc/_modidx.py
--rw-r--r--   0 solst      (501) staff       (20)     2561 2024-04-04 12:39:47.000000 utrc-0.0.3/utrc/attr.py
--rw-r--r--   0 solst      (501) staff       (20)     7771 2024-04-04 12:39:47.000000 utrc-0.0.3/utrc/atyp.py
--rw-r--r--   0 solst      (501) staff       (20)     3481 2024-04-04 12:39:47.000000 utrc-0.0.3/utrc/bend.py
--rw-r--r--   0 solst      (501) staff       (20)     1360 2024-04-04 12:39:47.000000 utrc-0.0.3/utrc/cons.py
--rw-r--r--   0 solst      (501) staff       (20)     1384 2024-04-04 12:39:47.000000 utrc-0.0.3/utrc/data.py
--rw-r--r--   0 solst      (501) staff       (20)     8477 2024-04-04 12:39:47.000000 utrc-0.0.3/utrc/diff.py
--rw-r--r--   0 solst      (501) staff       (20)    13575 2024-04-04 12:39:47.000000 utrc-0.0.3/utrc/dims.py
--rw-r--r--   0 solst      (501) staff       (20)     7586 2024-04-04 12:39:47.000000 utrc-0.0.3/utrc/init.py
--rw-r--r--   0 solst      (501) staff       (20)    32638 2024-04-04 12:39:47.000000 utrc-0.0.3/utrc/kwds.py
--rw-r--r--   0 solst      (501) staff       (20)     1226 2024-04-04 12:39:47.000000 utrc-0.0.3/utrc/logs.py
--rw-r--r--   0 solst      (501) staff       (20)     6563 2024-04-04 12:39:47.000000 utrc-0.0.3/utrc/loss.py
--rw-r--r--   0 solst      (501) staff       (20)     5409 2024-04-04 12:39:47.000000 utrc-0.0.3/utrc/misc.py
--rw-r--r--   0 solst      (501) staff       (20)     6391 2024-04-04 12:39:47.000000 utrc-0.0.3/utrc/perc.py
--rw-r--r--   0 solst      (501) staff       (20)     3327 2024-04-04 12:39:47.000000 utrc-0.0.3/utrc/seed.py
--rw-r--r--   0 solst      (501) staff       (20)     5313 2024-04-04 12:39:47.000000 utrc-0.0.3/utrc/smpl.py
--rw-r--r--   0 solst      (501) staff       (20)     1084 2024-04-04 12:39:47.000000 utrc-0.0.3/utrc/strs.py
--rw-r--r--   0 solst      (501) staff       (20)     9168 2024-04-04 12:39:47.000000 utrc-0.0.3/utrc/tens.py
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2024-04-04 12:39:58.181281 utrc-0.0.3/utrc.egg-info/
--rw-r--r--   0 solst      (501) staff       (20)     3841 2024-04-04 12:39:58.000000 utrc-0.0.3/utrc.egg-info/PKG-INFO
--rw-r--r--   0 solst      (501) staff       (20)      502 2024-04-04 12:39:58.000000 utrc-0.0.3/utrc.egg-info/SOURCES.txt
--rw-r--r--   0 solst      (501) staff       (20)        1 2024-04-04 12:39:58.000000 utrc-0.0.3/utrc.egg-info/dependency_links.txt
--rw-r--r--   0 solst      (501) staff       (20)       30 2024-04-04 12:39:58.000000 utrc-0.0.3/utrc.egg-info/entry_points.txt
--rw-r--r--   0 solst      (501) staff       (20)        1 2024-03-08 15:51:50.000000 utrc-0.0.3/utrc.egg-info/not-zip-safe
--rw-r--r--   0 solst      (501) staff       (20)      137 2024-04-04 12:39:58.000000 utrc-0.0.3/utrc.egg-info/requires.txt
--rw-r--r--   0 solst      (501) staff       (20)        5 2024-04-04 12:39:58.000000 utrc-0.0.3/utrc.egg-info/top_level.txt
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2024-04-06 14:45:17.975528 utrc-0.0.4/
+-rw-r--r--   0 solst      (501) staff       (20)    11337 2024-02-26 19:42:52.000000 utrc-0.0.4/LICENSE
+-rw-r--r--   0 solst      (501) staff       (20)      111 2024-02-26 19:42:52.000000 utrc-0.0.4/MANIFEST.in
+-rw-r--r--   0 solst      (501) staff       (20)     3841 2024-04-06 14:45:17.975290 utrc-0.0.4/PKG-INFO
+-rw-r--r--   0 solst      (501) staff       (20)     2720 2024-03-14 20:37:52.000000 utrc-0.0.4/README.md
+-rw-r--r--   0 solst      (501) staff       (20)      920 2024-04-04 12:40:42.000000 utrc-0.0.4/settings.ini
+-rw-r--r--   0 solst      (501) staff       (20)       38 2024-04-06 14:45:17.975588 utrc-0.0.4/setup.cfg
+-rw-r--r--   0 solst      (501) staff       (20)     2585 2024-02-26 19:42:52.000000 utrc-0.0.4/setup.py
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2024-04-06 14:45:17.972595 utrc-0.0.4/utrc/
+-rw-r--r--   0 solst      (501) staff       (20)      980 2024-04-06 14:45:08.000000 utrc-0.0.4/utrc/__init__.py
+-rw-r--r--   0 solst      (501) staff       (20)    23626 2024-04-06 14:45:08.000000 utrc-0.0.4/utrc/_modidx.py
+-rw-r--r--   0 solst      (501) staff       (20)     3146 2024-04-06 14:45:08.000000 utrc-0.0.4/utrc/attr.py
+-rw-r--r--   0 solst      (501) staff       (20)     7771 2024-04-06 14:45:08.000000 utrc-0.0.4/utrc/atyp.py
+-rw-r--r--   0 solst      (501) staff       (20)     3481 2024-04-06 14:45:08.000000 utrc-0.0.4/utrc/bend.py
+-rw-r--r--   0 solst      (501) staff       (20)    10268 2024-04-04 17:50:33.000000 utrc-0.0.4/utrc/cols.py
+-rw-r--r--   0 solst      (501) staff       (20)     1360 2024-04-06 14:45:08.000000 utrc-0.0.4/utrc/cons.py
+-rw-r--r--   0 solst      (501) staff       (20)     1279 2024-04-06 14:45:08.000000 utrc-0.0.4/utrc/data.py
+-rw-r--r--   0 solst      (501) staff       (20)     8477 2024-04-06 14:45:08.000000 utrc-0.0.4/utrc/diff.py
+-rw-r--r--   0 solst      (501) staff       (20)    13575 2024-04-06 14:45:08.000000 utrc-0.0.4/utrc/dims.py
+-rw-r--r--   0 solst      (501) staff       (20)     7586 2024-04-06 14:45:08.000000 utrc-0.0.4/utrc/init.py
+-rw-r--r--   0 solst      (501) staff       (20)    32638 2024-04-06 14:45:08.000000 utrc-0.0.4/utrc/kwds.py
+-rw-r--r--   0 solst      (501) staff       (20)     1226 2024-04-06 14:45:08.000000 utrc-0.0.4/utrc/logs.py
+-rw-r--r--   0 solst      (501) staff       (20)     6563 2024-04-06 14:45:08.000000 utrc-0.0.4/utrc/loss.py
+-rw-r--r--   0 solst      (501) staff       (20)     7568 2024-04-06 14:45:08.000000 utrc-0.0.4/utrc/misc.py
+-rw-r--r--   0 solst      (501) staff       (20)    12556 2024-04-04 19:18:05.000000 utrc-0.0.4/utrc/pand.py
+-rw-r--r--   0 solst      (501) staff       (20)     6391 2024-04-06 14:04:05.000000 utrc-0.0.4/utrc/perc.py
+-rw-r--r--   0 solst      (501) staff       (20)     2198 2024-04-06 14:04:05.000000 utrc-0.0.4/utrc/seed.py
+-rw-r--r--   0 solst      (501) staff       (20)     6712 2024-04-06 14:45:08.000000 utrc-0.0.4/utrc/smpl.py
+-rw-r--r--   0 solst      (501) staff       (20)     2449 2024-04-06 14:45:08.000000 utrc-0.0.4/utrc/strs.py
+-rw-r--r--   0 solst      (501) staff       (20)     9168 2024-04-06 14:45:08.000000 utrc-0.0.4/utrc/tens.py
+-rw-r--r--   0 solst      (501) staff       (20)     1087 2024-04-06 14:45:08.000000 utrc-0.0.4/utrc/util.py
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2024-04-06 14:45:17.974189 utrc-0.0.4/utrc.egg-info/
+-rw-r--r--   0 solst      (501) staff       (20)     3841 2024-04-06 14:45:17.000000 utrc-0.0.4/utrc.egg-info/PKG-INFO
+-rw-r--r--   0 solst      (501) staff       (20)      541 2024-04-06 14:45:17.000000 utrc-0.0.4/utrc.egg-info/SOURCES.txt
+-rw-r--r--   0 solst      (501) staff       (20)        1 2024-04-06 14:45:17.000000 utrc-0.0.4/utrc.egg-info/dependency_links.txt
+-rw-r--r--   0 solst      (501) staff       (20)       30 2024-04-06 14:45:17.000000 utrc-0.0.4/utrc.egg-info/entry_points.txt
+-rw-r--r--   0 solst      (501) staff       (20)        1 2024-03-08 15:51:50.000000 utrc-0.0.4/utrc.egg-info/not-zip-safe
+-rw-r--r--   0 solst      (501) staff       (20)      137 2024-04-06 14:45:17.000000 utrc-0.0.4/utrc.egg-info/requires.txt
+-rw-r--r--   0 solst      (501) staff       (20)        5 2024-04-06 14:45:17.000000 utrc-0.0.4/utrc.egg-info/top_level.txt
```

### Comparing `utrc-0.0.3/LICENSE` & `utrc-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `utrc-0.0.3/PKG-INFO` & `utrc-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utrc
-Version: 0.0.3
+Version: 0.0.4
 Summary: util torch
 Home-page: https://github.com/dsm-72/utrc
 Author: dsm-72
 Author-email: sumner.magruder@yale.edu
 License: Apache Software License 2.0
 Keywords: utility for pytorch torch util utrc
 Classifier: Development Status :: 4 - Beta
```

### Comparing `utrc-0.0.3/README.md` & `utrc-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `utrc-0.0.3/settings.ini` & `utrc-0.0.4/settings.ini`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = utrc
 lib_name = utrc
-version = 0.0.3
+version = 0.0.4
 min_python = 3.11
 license = apache2
 black_formatting = False
 doc_path = _docs
 lib_path = utrc
 nbs_path = nbs
 recursive = True
```

### Comparing `utrc-0.0.3/setup.py` & `utrc-0.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `utrc-0.0.3/utrc/__init__.py` & `utrc-0.0.4/utrc/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,36 +1,37 @@
-__version__ = "0.0.3"
+__version__ = "0.0.4"
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/00__init__.ipynb.
 
 # %% auto 0
 __all__ = []
 
 # %% ../nbs/00__init__.ipynb 3
 from itertools import chain
 from utrc import (
     cons, atyp, 
     kwds, 
-    logs, attr, seed, bend, 
-    perc, strs, misc, smpl, 
+    logs, attr, bend, 
+    util, strs, misc, smpl, 
     data, dims, tens, init, 
     diff, loss, 
 )
 
 from .cons import *
 from .atyp import *
 from .kwds import *
 
 from .logs import *
 
 from .attr import *
 
-from .seed import *
+# from utrc.seed import *
 from .bend import *
+from .util import *
 
-from .perc import *
+# from utrc.perc import *
 from .strs import *
 from .misc import *
 
 from .smpl import *
 from .data import *
 
 from .dims import *
@@ -41,13 +42,14 @@
 from .loss import *
 
 # %% ../nbs/00__init__.ipynb 4
 __all__ = sorted(set(chain(*[
     mod.__all__ for mod in (
         cons, atyp, 
         kwds, 
-        logs, attr, seed, bend, 
-        perc, strs, misc, smpl, 
+        logs, attr, # seed, 
+        bend, util, # perc,
+        strs, misc, smpl, 
         data, dims, tens, init, 
         diff, loss, 
     )
 ])))
```

### Comparing `utrc-0.0.3/utrc/_modidx.py` & `utrc-0.0.4/utrc/_modidx.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 # Autogenerated by nbdev
 
 d = { 'settings': { 'branch': 'main',
                 'doc_baseurl': '/utrc',
                 'doc_host': 'https://dsm-72.github.io',
                 'git_url': 'https://github.com/dsm-72/utrc',
                 'lib_path': 'utrc'},
-  'syms': { 'utrc.attr': { 'utrc.attr._avail': ('attr.html#_avail', 'utrc/attr.py'),
+  'syms': { 'utrc.attr': { 'utrc.attr._astype': ('attr.html#_astype', 'utrc/attr.py'),
+                           'utrc.attr._avail': ('attr.html#_avail', 'utrc/attr.py'),
                            'utrc.attr._built': ('attr.html#_built', 'utrc/attr.py'),
+                           'utrc.attr._index': ('attr.html#_index', 'utrc/attr.py'),
+                           'utrc.attr._name': ('attr.html#_name', 'utrc/attr.py'),
                            'utrc.attr._ndim': ('attr.html#_ndim', 'utrc/attr.py'),
                            'utrc.attr._seeded': ('attr.html#_seeded', 'utrc/attr.py'),
                            'utrc.attr._shape': ('attr.html#_shape', 'utrc/attr.py'),
                            'utrc.attr.getattrs': ('attr.html#getattrs', 'utrc/attr.py'),
                            'utrc.attr.gets': ('attr.html#gets', 'utrc/attr.py'),
                            'utrc.attr.nested': ('attr.html#nested', 'utrc/attr.py'),
                            'utrc.attr.nested.__call__': ('attr.html#nested.__call__', 'utrc/attr.py'),
@@ -20,14 +23,24 @@
             'utrc.bend': { 'utrc.bend.backend': ('bend.html#backend', 'utrc/bend.py'),
                            'utrc.bend.getbackend': ('bend.html#getbackend', 'utrc/bend.py'),
                            'utrc.bend.hasbackend': ('bend.html#hasbackend', 'utrc/bend.py'),
                            'utrc.bend.hascuda': ('bend.html#hascuda', 'utrc/bend.py'),
                            'utrc.bend.hasmps': ('bend.html#hasmps', 'utrc/bend.py'),
                            'utrc.bend.isavail': ('bend.html#isavail', 'utrc/bend.py'),
                            'utrc.bend.isbuilt': ('bend.html#isbuilt', 'utrc/bend.py')},
+            'utrc.cols': { 'utrc.cols.LocReturn': ('cols.html#locreturn', 'utrc/cols.py'),
+                           'utrc.cols.as_categories': ('cols.html#as_categories', 'utrc/cols.py'),
+                           'utrc.cols.drop_column': ('cols.html#drop_column', 'utrc/cols.py'),
+                           'utrc.cols.drop_named_index': ('cols.html#drop_named_index', 'utrc/cols.py'),
+                           'utrc.cols.get_categorical_column': ('cols.html#get_categorical_column', 'utrc/cols.py'),
+                           'utrc.cols.get_categories': ('cols.html#get_categories', 'utrc/cols.py'),
+                           'utrc.cols.get_category_indexes': ('cols.html#get_category_indexes', 'utrc/cols.py'),
+                           'utrc.cols.get_group': ('cols.html#get_group', 'utrc/cols.py'),
+                           'utrc.cols.is_not_named': ('cols.html#is_not_named', 'utrc/cols.py'),
+                           'utrc.cols.is_unnamed': ('cols.html#is_unnamed', 'utrc/cols.py')},
             'utrc.cons': {},
             'utrc.data': { 'utrc.data.catdists': ('data.html#catdists', 'utrc/data.py'),
                            'utrc.data.datasplit': ('data.html#datasplit', 'utrc/data.py')},
             'utrc.diff': { 'utrc.diff.Diffusion': ('diff.html#diffusion', 'utrc/diff.py'),
                            'utrc.diff.Diffusion.__init__': ('diff.html#diffusion.__init__', 'utrc/diff.py'),
                            'utrc.diff.Diffusion._eigs_to_use': ('diff.html#diffusion._eigs_to_use', 'utrc/diff.py'),
                            'utrc.diff.Diffusion._pairwise_distances': ('diff.html#diffusion._pairwise_distances', 'utrc/diff.py'),
@@ -156,43 +169,59 @@
                            'utrc.loss.MMDLoss.__init__': ('loss.html#mmdloss.__init__', 'utrc/loss.py'),
                            'utrc.loss.MMDLoss.forward': ('loss.html#mmdloss.forward', 'utrc/loss.py'),
                            'utrc.loss.MMDLoss.guassian_kernel': ('loss.html#mmdloss.guassian_kernel', 'utrc/loss.py'),
                            'utrc.loss.OptimalTransportLoss': ('loss.html#optimaltransportloss', 'utrc/loss.py'),
                            'utrc.loss.OptimalTransportLoss.__call__': ('loss.html#optimaltransportloss.__call__', 'utrc/loss.py'),
                            'utrc.loss.OptimalTransportLoss.__init__': ('loss.html#optimaltransportloss.__init__', 'utrc/loss.py')},
             'utrc.misc': { 'utrc.misc.calcgrid': ('misc.html#calcgrid', 'utrc/misc.py'),
+                           'utrc.misc.drop_column': ('misc.html#drop_column', 'utrc/misc.py'),
+                           'utrc.misc.drop_named_index': ('misc.html#drop_named_index', 'utrc/misc.py'),
                            'utrc.misc.generate_steps': ('misc.html#generate_steps', 'utrc/misc.py'),
+                           'utrc.misc.get_categories': ('misc.html#get_categories', 'utrc/misc.py'),
                            'utrc.misc.grididx': ('misc.html#grididx', 'utrc/misc.py'),
+                           'utrc.misc.groupget': ('misc.html#groupget', 'utrc/misc.py'),
+                           'utrc.misc.grouplens': ('misc.html#grouplens', 'utrc/misc.py'),
                            'utrc.misc.increment_pairs': ('misc.html#increment_pairs', 'utrc/misc.py'),
                            'utrc.misc.pad4grid': ('misc.html#pad4grid', 'utrc/misc.py'),
                            'utrc.misc.pair': ('misc.html#pair', 'utrc/misc.py'),
                            'utrc.misc.steps': ('misc.html#steps', 'utrc/misc.py'),
                            'utrc.misc.takekeys': ('misc.html#takekeys', 'utrc/misc.py')},
+            'utrc.pand': { 'utrc.pand.as_categories': ('pand.html#as_categories', 'utrc/pand.py'),
+                           'utrc.pand.column_as_category': ('pand.html#column_as_category', 'utrc/pand.py'),
+                           'utrc.pand.drop_column': ('pand.html#drop_column', 'utrc/pand.py'),
+                           'utrc.pand.drop_named_index': ('pand.html#drop_named_index', 'utrc/pand.py'),
+                           'utrc.pand.extent': ('pand.html#extent', 'utrc/pand.py'),
+                           'utrc.pand.get_categories': ('pand.html#get_categories', 'utrc/pand.py'),
+                           'utrc.pand.get_category_indexes': ('pand.html#get_category_indexes', 'utrc/pand.py'),
+                           'utrc.pand.get_group': ('pand.html#get_group', 'utrc/pand.py'),
+                           'utrc.pand.is_not_named': ('pand.html#is_not_named', 'utrc/pand.py'),
+                           'utrc.pand.is_unnamed': ('pand.html#is_unnamed', 'utrc/pand.py'),
+                           'utrc.pand.numpy_labels': ('pand.html#numpy_labels', 'utrc/pand.py'),
+                           'utrc.pand.sample_categories': ('pand.html#sample_categories', 'utrc/pand.py'),
+                           'utrc.pand.sample_index': ('pand.html#sample_index', 'utrc/pand.py'),
+                           'utrc.pand.samples_per_category': ('pand.html#samples_per_category', 'utrc/pand.py')},
             'utrc.perc': { 'utrc.perc.accumulate_percents': ('perc.html#accumulate_percents', 'utrc/perc.py'),
                            'utrc.perc.apercents': ('perc.html#apercents', 'utrc/perc.py'),
                            'utrc.perc.idxstep': ('perc.html#idxstep', 'utrc/perc.py'),
                            'utrc.perc.integer_percent': ('perc.html#integer_percent', 'utrc/perc.py'),
                            'utrc.perc.integer_percents': ('perc.html#integer_percents', 'utrc/perc.py'),
                            'utrc.perc.ipercent': ('perc.html#ipercent', 'utrc/perc.py'),
                            'utrc.perc.ipercents': ('perc.html#ipercents', 'utrc/perc.py'),
                            'utrc.perc.perbounds': ('perc.html#perbounds', 'utrc/perc.py'),
                            'utrc.perc.percent': ('perc.html#percent', 'utrc/perc.py'),
                            'utrc.perc.range_percents': ('perc.html#range_percents', 'utrc/perc.py'),
                            'utrc.perc.rpercents': ('perc.html#rpercents', 'utrc/perc.py')},
-            'utrc.seed': { 'utrc.seed.npseed': ('seed.html#npseed', 'utrc/seed.py'),
-                           'utrc.seed.osseed': ('seed.html#osseed', 'utrc/seed.py'),
-                           'utrc.seed.plseed': ('seed.html#plseed', 'utrc/seed.py'),
-                           'utrc.seed.ptseed': ('seed.html#ptseed', 'utrc/seed.py'),
-                           'utrc.seed.seedall': ('seed.html#seedall', 'utrc/seed.py'),
-                           'utrc.seed.seedfn': ('seed.html#seedfn', 'utrc/seed.py')},
-            'utrc.smpl': { 'utrc.smpl.groupget': ('smpl.html#groupget', 'utrc/smpl.py'),
-                           'utrc.smpl.idxperm': ('smpl.html#idxperm', 'utrc/smpl.py'),
-                           'utrc.smpl.permute_indicies': ('smpl.html#permute_indicies', 'utrc/smpl.py'),
-                           'utrc.smpl.sample': ('smpl.html#sample', 'utrc/smpl.py')},
+            'utrc.seed': {'utrc.seed.seedall': ('seed.html#seedall', 'utrc/seed.py')},
+            'utrc.smpl': { 'utrc.smpl._categorical_labels': ('smpl.html#_categorical_labels', 'utrc/smpl.py'),
+                           'utrc.smpl._categorical_sample': ('smpl.html#_categorical_sample', 'utrc/smpl.py'),
+                           'utrc.smpl.categorical_sample': ('smpl.html#categorical_sample', 'utrc/smpl.py'),
+                           'utrc.smpl.sample': ('smpl.html#sample', 'utrc/smpl.py'),
+                           'utrc.smpl.sample_grouped': ('smpl.html#sample_grouped', 'utrc/smpl.py')},
             'utrc.strs': { 'utrc.strs.endpart': ('strs.html#endpart', 'utrc/strs.py'),
+                           'utrc.strs.is_not_named': ('strs.html#is_not_named', 'utrc/strs.py'),
                            'utrc.strs.midpart': ('strs.html#midpart', 'utrc/strs.py'),
                            'utrc.strs.prepart': ('strs.html#prepart', 'utrc/strs.py'),
                            'utrc.strs.snakecase': ('strs.html#snakecase', 'utrc/strs.py')},
             'utrc.tens': { 'utrc.tens.augment_zeros': ('tens.html#augment_zeros', 'utrc/tens.py'),
                            'utrc.tens.augzeros': ('tens.html#augzeros', 'utrc/tens.py'),
                            'utrc.tens.last': ('tens.html#last', 'utrc/tens.py'),
                            'utrc.tens.last_rn': ('tens.html#last_rn', 'utrc/tens.py'),
@@ -200,8 +229,9 @@
                            'utrc.tens.nonzerosfrom': ('tens.html#nonzerosfrom', 'utrc/tens.py'),
                            'utrc.tens.pack': ('tens.html#pack', 'utrc/tens.py'),
                            'utrc.tens.pack_padded': ('tens.html#pack_padded', 'utrc/tens.py'),
                            'utrc.tens.pad': ('tens.html#pad', 'utrc/tens.py'),
                            'utrc.tens.sort_sequences': ('tens.html#sort_sequences', 'utrc/tens.py'),
                            'utrc.tens.torchnans': ('tens.html#torchnans', 'utrc/tens.py'),
                            'utrc.tens.unpack': ('tens.html#unpack', 'utrc/tens.py'),
-                           'utrc.tens.unpadded_len': ('tens.html#unpadded_len', 'utrc/tens.py')}}}
+                           'utrc.tens.unpadded_len': ('tens.html#unpadded_len', 'utrc/tens.py')},
+            'utrc.util': {'utrc.util.extent': ('util.html#extent', 'utrc/util.py')}}}
```

### Comparing `utrc-0.0.3/utrc/atyp.py` & `utrc-0.0.4/utrc/atyp.py`

 * *Files identical despite different names*

### Comparing `utrc-0.0.3/utrc/bend.py` & `utrc-0.0.4/utrc/bend.py`

 * *Files identical despite different names*

### Comparing `utrc-0.0.3/utrc/cons.py` & `utrc-0.0.4/utrc/cons.py`

 * *Files identical despite different names*

### Comparing `utrc-0.0.3/utrc/data.py` & `utrc-0.0.4/utrc/data.py`

 * *Files 7% similar despite different names*

```diff
@@ -27,31 +27,28 @@
 # %% ../nbs/21_data.ipynb 17
 #| export
 
 
 # %% ../nbs/21_data.ipynb 19
 from quac import ints, array, tensor
 from nlit import DROP
+from pcts import permute_indicies
 
 # %% ../nbs/21_data.ipynb 21
 from .atyp import XYArray, LabelArray
-# from utrc.attr import _shape
-from .smpl import permute_indicies
 
 # %% ../nbs/21_data.ipynb 24
 def catdists(data: XYArray, n: int) -> LabelArray:
     '''Categorize data by distances from the origin into n classes.'''
     dist = np.linalg.norm(data, axis=1)
     return pd.qcut(dist, q=n, labels=False, duplicates=DROP)
 
 # %% ../nbs/21_data.ipynb 26
 def datasplit(data, splits: ints, retdfs: bool = False, seed: int = 3) -> tuple[Union[array, tensor], ...]:
     els = data.shape[0]
-    # els = _shape(data)[0]
-    # idx = idxperm(els, *splits, seed=seed)
     idx = permute_indicies(els, *splits, seed=seed)
     if retdfs: return tuple(data.iloc[i] for i in idx)
     try: return tuple(data[i] for i in idx)
     except: return idx
 
 # %% ../nbs/21_data.ipynb 28
 #| export
```

### Comparing `utrc-0.0.3/utrc/diff.py` & `utrc-0.0.4/utrc/diff.py`

 * *Files identical despite different names*

### Comparing `utrc-0.0.3/utrc/dims.py` & `utrc-0.0.4/utrc/dims.py`

 * *Files identical despite different names*

### Comparing `utrc-0.0.3/utrc/init.py` & `utrc-0.0.4/utrc/init.py`

 * *Files identical despite different names*

### Comparing `utrc-0.0.3/utrc/kwds.py` & `utrc-0.0.4/utrc/kwds.py`

 * *Files identical despite different names*

### Comparing `utrc-0.0.3/utrc/logs.py` & `utrc-0.0.4/utrc/logs.py`

 * *Files identical despite different names*

### Comparing `utrc-0.0.3/utrc/loss.py` & `utrc-0.0.4/utrc/loss.py`

 * *Files identical despite different names*

### Comparing `utrc-0.0.3/utrc/perc.py` & `utrc-0.0.4/utrc/perc.py`

 * *Files identical despite different names*

### Comparing `utrc-0.0.3/utrc/seed.py` & `utrc-0.0.4/utrc/seed.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/06_seed.ipynb.
 
 # %% auto 0
-__all__ = ['osseed', 'npseed', 'ptseed', 'plseed', 'seedfn', 'seedall']
+__all__ = ['seedall']
 
 # %% ../nbs/06_seed.ipynb 6
-#| export
-
+from functools import wraps
 
 # %% ../nbs/06_seed.ipynb 8
 from types import FunctionType
 
 # %% ../nbs/06_seed.ipynb 11
 #| export
 
@@ -23,69 +22,31 @@
 
 # %% ../nbs/06_seed.ipynb 17
 #| export
 
 
 # %% ../nbs/06_seed.ipynb 19
 from lull import lull
+from seeder import seedall as _seedall
 
 # %% ../nbs/06_seed.ipynb 21
-from .cons import _SEEDED
-from .attr import _seeded
-
-# %% ../nbs/06_seed.ipynb 24
-def osseed(seed: int) -> int:
-    '''Set python random seed for reproducibility.'''
-    try: 
-        import random
-        random.seed(seed)
-    except ImportError: ...
-    return seed
-
-def npseed(seed: int) -> int:
-    '''Set numpy seed for reproducibility.'''
-    try: 
-        import numpy as np
-        np.random.seed(seed)
-    except ImportError: ...
-    return seed
-
-def ptseed(seed: int) -> int:
-    '''Set pytorch seed for reproducibility.'''
-    try: 
-        import torch
-        torch.manual_seed(seed)
-    except ImportError: ...
-    return seed
-
-
-def plseed(seed: int) -> int:
-    '''Set pytorch lightning seed for reproducibility.'''
-    try: 
-        import pytorch_lightning as pl
-        pl.seed_everything(seed)
-    except ImportError: ...
-    return seed
+#| export
 
-# %% ../nbs/06_seed.ipynb 25
-def seedfn(fn: FunctionType, seed: int = 3, reseed: bool = True) -> int:
-    # seeded = getattr(fn, _SEEDED, False)
-    if not _seeded(fn) or reseed:
-        fn(seed)
-        _seeded.set(fn, True)
-        # setattr(fn, _SEEDED, True)
-    return seed
 
-# %% ../nbs/06_seed.ipynb 27
+# %% ../nbs/06_seed.ipynb 23
+@wraps(_seedall)
 def seedall(seed: int = 3, reseed: bool = False) -> int:
     '''Set seeds for reproducibility.
     
     Parameters
     ----------
     seed : int
+    
+    reseed : bool, default = False,
+        Whether or not to reinvoke each seed function if it was already called.
 
     Returns
     -------
     seed: int
         The seed used to set the random number generators.
 
     Notes
@@ -105,15 +66,12 @@
     .. _randomness: https://pytorch.org/docs/stable/notes/randomness.html
     .. _random.seed: https://docs.python.org/3/library/random.html#random.seed
     .. _np.random.seed: https://numpy.org/doc/stable/reference/random/generated/numpy.random.seed.html
     .. _torch.manual_seed: https://pytorch.org/docs/stable/generated/torch.manual_seed.html
     .. _pl.seed_everything: https://pytorch-lightning.readthedocs.io/en/latest/common/seed_everything.html
     '''    
     with lull():
-        seedfn(osseed, seed, reseed=reseed)
-        seedfn(npseed, seed, reseed=reseed)
-        seedfn(ptseed, seed, reseed=reseed)
-        seedfn(plseed, seed, reseed=reseed)  
+        _seedall(seed, reseed)
     return seed
 
-# %% ../nbs/06_seed.ipynb 29
+# %% ../nbs/06_seed.ipynb 25
 #| export
```

### Comparing `utrc-0.0.3/utrc/tens.py` & `utrc-0.0.4/utrc/tens.py`

 * *Files identical despite different names*

### Comparing `utrc-0.0.3/utrc.egg-info/PKG-INFO` & `utrc-0.0.4/utrc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utrc
-Version: 0.0.3
+Version: 0.0.4
 Summary: util torch
 Home-page: https://github.com/dsm-72/utrc
 Author: dsm-72
 Author-email: sumner.magruder@yale.edu
 License: Apache Software License 2.0
 Keywords: utility for pytorch torch util utrc
 Classifier: Development Status :: 4 - Beta
```

