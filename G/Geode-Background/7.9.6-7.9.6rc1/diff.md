# Comparing `tmp/Geode_Background-7.9.6-cp39-cp39-manylinux2014_x86_64.whl.zip` & `tmp/Geode_Background-7.9.6rc1-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 3222015 bytes, number of entries: 16
--rw-r--r--  2.0 unx      110 b- defN 24-Apr-06 06:48 geode_background/__init__.py
--rw-r--r--  2.0 unx      191 b- defN 24-Apr-06 06:48 geode_background/brep.py
--rw-r--r--  2.0 unx      192 b- defN 24-Apr-06 06:48 geode_background/solid.py
--rw-r--r--  2.0 unx      196 b- defN 24-Apr-06 06:48 geode_background/surface.py
--rwxr-xr-x  2.0 unx   122264 b- defN 24-Apr-06 06:48 geode_background/lib64/geode_background_py_brep.cpython-39-x86_64-linux-gnu.so
--rwxr-xr-x  2.0 unx   122264 b- defN 24-Apr-06 06:48 geode_background/lib64/geode_background_py_common.cpython-39-x86_64-linux-gnu.so
--rwxr-xr-x  2.0 unx   122264 b- defN 24-Apr-06 06:48 geode_background/lib64/geode_background_py_solid.cpython-39-x86_64-linux-gnu.so
--rwxr-xr-x  2.0 unx   122264 b- defN 24-Apr-06 06:48 geode_background/lib64/geode_background_py_surface.cpython-39-x86_64-linux-gnu.so
--rwxr-xr-x  2.0 unx   155192 b- defN 24-Apr-06 06:48 geode_background/lib64/libGeode-Background_brep.so
--rwxr-xr-x  2.0 unx   109008 b- defN 24-Apr-06 06:48 geode_background/lib64/libGeode-Background_common.so
--rwxr-xr-x  2.0 unx  3420848 b- defN 24-Apr-06 06:48 geode_background/lib64/libGeode-Background_solid.so
--rwxr-xr-x  2.0 unx  3235312 b- defN 24-Apr-06 06:48 geode_background/lib64/libGeode-Background_surface.so
--rw-r--r--  2.0 unx     1057 b- defN 24-Apr-06 06:48 Geode_Background-7.9.6.dist-info/METADATA
--rw-r--r--  2.0 unx      103 b- defN 24-Apr-06 06:48 Geode_Background-7.9.6.dist-info/WHEEL
--rw-r--r--  2.0 unx       17 b- defN 24-Apr-06 06:48 Geode_Background-7.9.6.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1661 b- defN 24-Apr-06 06:48 Geode_Background-7.9.6.dist-info/RECORD
-16 files, 7412943 bytes uncompressed, 3219193 bytes compressed:  56.6%
+Zip file size: 4726940 bytes, number of entries: 16
+-rw-rw-rw-  2.0 fat      216 b- defN 24-Apr-05 16:31 geode_background/__init__.py
+-rw-rw-rw-  2.0 fat      199 b- defN 24-Apr-05 16:31 geode_background/brep.py
+-rw-rw-rw-  2.0 fat      199 b- defN 24-Apr-05 16:31 geode_background/solid.py
+-rw-rw-rw-  2.0 fat      203 b- defN 24-Apr-05 16:31 geode_background/surface.py
+-rw-rw-rw-  2.0 fat  3767808 b- defN 24-Apr-05 16:32 geode_background/bin/Geode-Background_brep.dll
+-rw-rw-rw-  2.0 fat    54272 b- defN 24-Apr-05 16:32 geode_background/bin/Geode-Background_common.dll
+-rw-rw-rw-  2.0 fat  3963904 b- defN 24-Apr-05 16:32 geode_background/bin/Geode-Background_solid.dll
+-rw-rw-rw-  2.0 fat  3812352 b- defN 24-Apr-05 16:32 geode_background/bin/Geode-Background_surface.dll
+-rw-rw-rw-  2.0 fat   125440 b- defN 24-Apr-05 16:32 geode_background/bin/geode_background_py_brep.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat   125440 b- defN 24-Apr-05 16:32 geode_background/bin/geode_background_py_common.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat   125440 b- defN 24-Apr-05 16:32 geode_background/bin/geode_background_py_solid.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat   125440 b- defN 24-Apr-05 16:32 geode_background/bin/geode_background_py_surface.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat     1104 b- defN 24-Apr-05 16:32 Geode_Background-7.9.6rc1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      100 b- defN 24-Apr-05 16:32 Geode_Background-7.9.6rc1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       17 b- defN 24-Apr-05 16:32 Geode_Background-7.9.6rc1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1601 b- defN 24-Apr-05 16:32 Geode_Background-7.9.6rc1.dist-info/RECORD
+16 files, 12103735 bytes uncompressed, 4724238 bytes compressed:  61.0%
```

## zipnote {}

```diff
@@ -6,44 +6,44 @@
 
 Filename: geode_background/solid.py
 Comment: 
 
 Filename: geode_background/surface.py
 Comment: 
 
-Filename: geode_background/lib64/geode_background_py_brep.cpython-39-x86_64-linux-gnu.so
+Filename: geode_background/bin/Geode-Background_brep.dll
 Comment: 
 
-Filename: geode_background/lib64/geode_background_py_common.cpython-39-x86_64-linux-gnu.so
+Filename: geode_background/bin/Geode-Background_common.dll
 Comment: 
 
-Filename: geode_background/lib64/geode_background_py_solid.cpython-39-x86_64-linux-gnu.so
+Filename: geode_background/bin/Geode-Background_solid.dll
 Comment: 
 
-Filename: geode_background/lib64/geode_background_py_surface.cpython-39-x86_64-linux-gnu.so
+Filename: geode_background/bin/Geode-Background_surface.dll
 Comment: 
 
-Filename: geode_background/lib64/libGeode-Background_brep.so
+Filename: geode_background/bin/geode_background_py_brep.cp39-win_amd64.pyd
 Comment: 
 
-Filename: geode_background/lib64/libGeode-Background_common.so
+Filename: geode_background/bin/geode_background_py_common.cp39-win_amd64.pyd
 Comment: 
 
-Filename: geode_background/lib64/libGeode-Background_solid.so
+Filename: geode_background/bin/geode_background_py_solid.cp39-win_amd64.pyd
 Comment: 
 
-Filename: geode_background/lib64/libGeode-Background_surface.so
+Filename: geode_background/bin/geode_background_py_surface.cp39-win_amd64.pyd
 Comment: 
 
-Filename: Geode_Background-7.9.6.dist-info/METADATA
+Filename: Geode_Background-7.9.6rc1.dist-info/METADATA
 Comment: 
 
-Filename: Geode_Background-7.9.6.dist-info/WHEEL
+Filename: Geode_Background-7.9.6rc1.dist-info/WHEEL
 Comment: 
 
-Filename: Geode_Background-7.9.6.dist-info/top_level.txt
+Filename: Geode_Background-7.9.6rc1.dist-info/top_level.txt
 Comment: 
 
-Filename: Geode_Background-7.9.6.dist-info/RECORD
+Filename: Geode_Background-7.9.6rc1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## geode_background/__init__.py

```diff
@@ -1,5 +1,8 @@
-## Copyright (c) 2019 - 2024 Geode-solutions
-
-from .surface import *
-from .solid import *
-from .brep import *
+## Copyright (c) 2019 - 2024 Geode-solutions
+
+import os, pathlib
+os.add_dll_directory(pathlib.Path(__file__).parent.resolve().joinpath('bin'))
+
+from .surface import *
+from .solid import *
+from .brep import *
```

## geode_background/brep.py

```diff
@@ -1,10 +1,10 @@
-#
-# Copyright (c) 2019 - 2024 Geode-solutions. All rights reserved.
-#
-
-import opengeode
-import geode_common
-
-from .lib64.geode_background_py_brep import *
-
-BackgroundBRepLibrary.initialize()
+#
+# Copyright (c) 2019 - 2024 Geode-solutions. All rights reserved.
+#
+
+import opengeode
+import geode_common
+
+from .bin.geode_background_py_brep import *
+
+BackgroundBRepLibrary.initialize()
```

## geode_background/solid.py

```diff
@@ -1,9 +1,9 @@
-#
-# Copyright (c) 2019 - 2024 Geode-solutions. All rights reserved.
-#
-
-import opengeode
-import geode_common
-
-from .lib64.geode_background_py_solid import *
-BackgroundSolidLibrary.initialize()
+#
+# Copyright (c) 2019 - 2024 Geode-solutions. All rights reserved.
+#
+
+import opengeode
+import geode_common
+
+from .bin.geode_background_py_solid import *
+BackgroundSolidLibrary.initialize()
```

## geode_background/surface.py

```diff
@@ -1,9 +1,9 @@
-#
-# Copyright (c) 2019 - 2024 Geode-solutions. All rights reserved.
-#
-
-import opengeode
-import geode_common
-
-from .lib64.geode_background_py_surface import *
-BackgroundSurfaceLibrary.initialize()
+#
+# Copyright (c) 2019 - 2024 Geode-solutions. All rights reserved.
+#
+
+import opengeode
+import geode_common
+
+from .bin.geode_background_py_surface import *
+BackgroundSurfaceLibrary.initialize()
```

## Comparing `Geode_Background-7.9.6.dist-info/METADATA` & `Geode_Background-7.9.6rc1.dist-info/METADATA`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,24 @@
-Metadata-Version: 2.1
-Name: Geode-Background
-Version: 7.9.6
-Summary: Geode-solutions OpenGeode module for building background meshes
-Home-page: https://github.com/Geode-solutions/Geode-Background
-Author: Geode-solutions
-Author-email: contact@geode-solutions.com
-License: Proprietary
-Description-Content-Type: text/markdown
-Requires-Dist: geode-common ==31.*,>=31.0.5
-Requires-Dist: opengeode-core ==14.*,>=14.18.1
-
-<h1 align="center">Background<sup><i>by Geode-solutions</i></sup></h1>
-<h3 align="center">Module to generate background meshes and background models for OpenGeode</h3>
-
-<p align="center">
-  <img src="https://github.com/Geode-solutions/Background_private/workflows/CI/badge.svg" alt="Build Status">
-  <img src="https://github.com/Geode-solutions/Background_private/workflows/CD/badge.svg" alt="Deploy Status">
-  <img src="https://codecov.io/gh/Geode-solutions/Background_private/branch/master/graph/badge.svg" alt="Coverage Status">
-  <img src="https://img.shields.io/github/release/Geode-solutions/Background_private.svg" alt="Version">
-</p>
+Metadata-Version: 2.1
+Name: Geode-Background
+Version: 7.9.6rc1
+Summary: Geode-solutions OpenGeode module for building background meshes
+Home-page: https://github.com/Geode-solutions/Geode-Background
+Author: Geode-solutions
+Author-email: contact@geode-solutions.com
+License: Proprietary
+Platform: UNKNOWN
+Description-Content-Type: text/markdown
+Requires-Dist: geode-common ==31.*,>=31.0.5
+Requires-Dist: opengeode-core ==14.*,>=14.18.1
+
+<h1 align="center">Background<sup><i>by Geode-solutions</i></sup></h1>
+<h3 align="center">Module to generate background meshes and background models for OpenGeode</h3>
+
+<p align="center">
+  <img src="https://github.com/Geode-solutions/Background_private/workflows/CI/badge.svg" alt="Build Status">
+  <img src="https://github.com/Geode-solutions/Background_private/workflows/CD/badge.svg" alt="Deploy Status">
+  <img src="https://codecov.io/gh/Geode-solutions/Background_private/branch/master/graph/badge.svg" alt="Coverage Status">
+  <img src="https://img.shields.io/github/release/Geode-solutions/Background_private.svg" alt="Version">
+</p>
+
+
```

## Comparing `Geode_Background-7.9.6.dist-info/RECORD` & `Geode_Background-7.9.6rc1.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-geode_background/__init__.py,sha256=blPQYNF5G29FTzV7qPxTRuHFNAO7q4zkFMBd-AbHTnY,110
-geode_background/brep.py,sha256=CvXUH_pK1hYWw4q37x5Zc0jKhFSrRG0yQd7o7mPz5vM,191
-geode_background/solid.py,sha256=N0pBLglv9f58p0rmzx7H2kXI7UTDCxwLvojSDoA6oUg,192
-geode_background/surface.py,sha256=y1CRwP6BtWw-IJIJVbB8Ihg0qeL8cG7cB4WEj5ls1Aw,196
-geode_background/lib64/geode_background_py_brep.cpython-39-x86_64-linux-gnu.so,sha256=Fm3Me3ZDb3EV0_p-cwN__rRLI_2HuzbaqKWlwHkMUPc,122264
-geode_background/lib64/geode_background_py_common.cpython-39-x86_64-linux-gnu.so,sha256=SHMS9J00Gb1JN8KkyldH-80Zux6Jxqhp0m3WpjD5D5Q,122264
-geode_background/lib64/geode_background_py_solid.cpython-39-x86_64-linux-gnu.so,sha256=zTUqSnWck3d_NQS0ttT51S2LlP7RFnM5wQtOuBHYLFU,122264
-geode_background/lib64/geode_background_py_surface.cpython-39-x86_64-linux-gnu.so,sha256=FL-mb-dnX_Qg8mk0JboPG3b81K1icAqgcID-WN4TJFk,122264
-geode_background/lib64/libGeode-Background_brep.so,sha256=mcrG7ryUob6dBPeej8AszCrE3vola14bgeMiBa1R-oU,155192
-geode_background/lib64/libGeode-Background_common.so,sha256=Eg4N90RPkYH36qBbIggIZChM2QcfzoWcROoq5kI6VoI,109008
-geode_background/lib64/libGeode-Background_solid.so,sha256=_zbSfzRgY2C46S43hmBkn1R-qcU5cPP3tDA7gcB_f54,3420848
-geode_background/lib64/libGeode-Background_surface.so,sha256=Salnj-idiz54a2s6j_6NDoteCXlDGlF95E3FWyG0MCQ,3235312
-Geode_Background-7.9.6.dist-info/METADATA,sha256=wmmEaQsIQaawjpAl6gy3Irku2bIVSE9BEtFSL71skAU,1057
-Geode_Background-7.9.6.dist-info/WHEEL,sha256=cPiEulY4lHJMdGCxx29HxfDkwhV9C6172sJgZUA9dSs,103
-Geode_Background-7.9.6.dist-info/top_level.txt,sha256=Zrf1AIA63yPEiQFwdZwLsHzGAE3soNFO7AVs5NdN_r4,17
-Geode_Background-7.9.6.dist-info/RECORD,,
+geode_background/__init__.py,sha256=nrly-bKXLsgtI1cSxS2toM6MvcxIM8FMKiC07JhlV9U,216
+geode_background/brep.py,sha256=tYHPoFSpQe7DcP4UdByklZuv6cIhtVzy4AtC6FDmb5g,199
+geode_background/solid.py,sha256=XU7nXDgAjD_8fRTQOQteGvL812oy5pCNNxAPDjXg21c,199
+geode_background/surface.py,sha256=gYOsu70XBpFHsMsTG56V05oAa8xWQLPsZpDhdkPP7PY,203
+geode_background/bin/Geode-Background_brep.dll,sha256=e6MiThpHeZYQW1M4sivthDvcq9a_OCuc4mVKY6yt0c8,3767808
+geode_background/bin/Geode-Background_common.dll,sha256=vx4JOLHslXTRfJ26bETtZTAv72ut6uzGP_UYhlC3AJM,54272
+geode_background/bin/Geode-Background_solid.dll,sha256=SWLB_UXmINyNc3H6OseSMW2DOfZmqXEpKJFOavhzH5k,3963904
+geode_background/bin/Geode-Background_surface.dll,sha256=5q5IJYxAVAc69Q-DaN5lUlX6jc5BfPA6LpCGkf0PTNI,3812352
+geode_background/bin/geode_background_py_brep.cp39-win_amd64.pyd,sha256=zJ7xLDslXVc38j4p-l6Ae50buwCiNZ5k3-BQdTDI0ww,125440
+geode_background/bin/geode_background_py_common.cp39-win_amd64.pyd,sha256=FGt-oqPKCu5KtoWaaGkTb_nXsbP39a9RqwF5WP-cEMU,125440
+geode_background/bin/geode_background_py_solid.cp39-win_amd64.pyd,sha256=U9_NK106IU7KDkFIl_2Q2f3uBpKELK5ucC0QJuDkJrg,125440
+geode_background/bin/geode_background_py_surface.cp39-win_amd64.pyd,sha256=hIIFyWAdnoVj6yAAZMdgd8sUVabgPxlQO9QhSCdu0Qc,125440
+Geode_Background-7.9.6rc1.dist-info/METADATA,sha256=tZ-oi-KGUmhLtexPrRBCIA4o-12nYMxZI8WhtIFD0Mg,1104
+Geode_Background-7.9.6rc1.dist-info/WHEEL,sha256=Z6c-bE0pUM47a70GvqO_SvH_XXU0lm62gEAKtoNJ08A,100
+Geode_Background-7.9.6rc1.dist-info/top_level.txt,sha256=Zrf1AIA63yPEiQFwdZwLsHzGAE3soNFO7AVs5NdN_r4,17
+Geode_Background-7.9.6rc1.dist-info/RECORD,,
```
