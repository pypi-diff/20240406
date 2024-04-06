# Comparing `tmp/speedtools-0.8.0.tar.gz` & `tmp/speedtools-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "speedtools-0.8.0.tar", last modified: Mon Sep 11 19:32:18 2023, max compression
+gzip compressed data, was "speedtools-0.9.0.tar", last modified: Tue Sep 12 21:57:50 2023, max compression
```

## Comparing `speedtools-0.8.0.tar` & `speedtools-0.9.0.tar`

### file list

```diff
@@ -1,37 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-11 19:32:18.933642 speedtools-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2023-09-11 19:32:04.000000 speedtools-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3102 2023-09-11 19:32:18.933642 speedtools-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2168 2023-09-11 19:32:04.000000 speedtools-0.8.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3007 2023-09-11 19:32:04.000000 speedtools-0.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-11 19:32:18.933642 speedtools-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2156 2023-09-11 19:32:04.000000 speedtools-0.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-11 19:32:18.933642 speedtools-0.8.0/speedtools/
--rw-r--r--   0 runner    (1001) docker     (127)      419 2023-09-11 19:32:04.000000 speedtools-0.8.0/speedtools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-11 19:32:18.933642 speedtools-0.8.0/speedtools/blender/
--rw-r--r--   0 runner    (1001) docker     (127)    20419 2023-09-11 19:32:04.000000 speedtools-0.8.0/speedtools/blender/io_nfs4_import.py
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2023-09-11 19:32:04.000000 speedtools-0.8.0/speedtools/can_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    10279 2023-09-11 19:32:04.000000 speedtools-0.8.0/speedtools/frd_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3558 2023-09-11 19:32:04.000000 speedtools-0.8.0/speedtools/fsh_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-11 19:32:18.933642 speedtools-0.8.0/speedtools/parsers/
--rw-r--r--   0 runner    (1001) docker     (127)      461 2023-09-11 19:32:04.000000 speedtools-0.8.0/speedtools/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3492 2023-09-11 19:32:04.000000 speedtools-0.8.0/speedtools/refpack.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-11 19:32:18.933642 speedtools-0.8.0/speedtools/specs/
--rw-r--r--   0 runner    (1001) docker     (127)      857 2023-09-11 19:32:04.000000 speedtools-0.8.0/speedtools/specs/can.ksy
--rw-r--r--   0 runner    (1001) docker     (127)     6015 2023-09-11 19:32:04.000000 speedtools-0.8.0/speedtools/specs/fce.ksy
--rw-r--r--   0 runner    (1001) docker     (127)    13941 2023-09-11 19:32:04.000000 speedtools-0.8.0/speedtools/specs/frd.ksy
--rw-r--r--   0 runner    (1001) docker     (127)     4084 2023-09-11 19:32:04.000000 speedtools-0.8.0/speedtools/specs/fsh.ksy
--rw-r--r--   0 runner    (1001) docker     (127)      417 2023-09-11 19:32:04.000000 speedtools-0.8.0/speedtools/specs/qfs.ksy
--rw-r--r--   0 runner    (1001) docker     (127)      919 2023-09-11 19:32:04.000000 speedtools-0.8.0/speedtools/specs/viv.ksy
--rw-r--r--   0 runner    (1001) docker     (127)      960 2023-09-11 19:32:04.000000 speedtools-0.8.0/speedtools/speedtool.py
--rw-r--r--   0 runner    (1001) docker     (127)     2333 2023-09-11 19:32:04.000000 speedtools-0.8.0/speedtools/tr_ini.py
--rw-r--r--   0 runner    (1001) docker     (127)     6801 2023-09-11 19:32:04.000000 speedtools-0.8.0/speedtools/track_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     5218 2023-09-11 19:32:04.000000 speedtools-0.8.0/speedtools/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     2475 2023-09-11 19:32:04.000000 speedtools-0.8.0/speedtools/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7399 2023-09-11 19:32:04.000000 speedtools-0.8.0/speedtools/viv_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-11 19:32:18.933642 speedtools-0.8.0/speedtools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3102 2023-09-11 19:32:18.000000 speedtools-0.8.0/speedtools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      712 2023-09-11 19:32:18.000000 speedtools-0.8.0/speedtools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-11 19:32:18.000000 speedtools-0.8.0/speedtools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2023-09-11 19:32:18.000000 speedtools-0.8.0/speedtools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2023-09-11 19:32:18.000000 speedtools-0.8.0/speedtools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2023-09-11 19:32:18.000000 speedtools-0.8.0/speedtools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-12 21:57:50.459526 speedtools-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2023-09-12 21:57:35.000000 speedtools-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3102 2023-09-12 21:57:50.459526 speedtools-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2168 2023-09-12 21:57:35.000000 speedtools-0.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3007 2023-09-12 21:57:35.000000 speedtools-0.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-12 21:57:50.459526 speedtools-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2133 2023-09-12 21:57:35.000000 speedtools-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-12 21:57:50.455525 speedtools-0.9.0/speedtools/
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2023-09-12 21:57:35.000000 speedtools-0.9.0/speedtools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-12 21:57:50.455525 speedtools-0.9.0/speedtools/blender/
+-rw-r--r--   0 runner    (1001) docker     (127)    21825 2023-09-12 21:57:35.000000 speedtools-0.9.0/speedtools/blender/io_nfs4_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1345 2023-09-12 21:57:35.000000 speedtools-0.9.0/speedtools/cam_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1227 2023-09-12 21:57:35.000000 speedtools-0.9.0/speedtools/can_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10256 2023-09-12 21:57:35.000000 speedtools-0.9.0/speedtools/frd_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3535 2023-09-12 21:57:35.000000 speedtools-0.9.0/speedtools/fsh_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-12 21:57:50.459526 speedtools-0.9.0/speedtools/parsers/
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2023-09-12 21:57:35.000000 speedtools-0.9.0/speedtools/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3469 2023-09-12 21:57:35.000000 speedtools-0.9.0/speedtools/refpack.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-12 21:57:50.459526 speedtools-0.9.0/speedtools/specs/
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2023-09-12 21:57:35.000000 speedtools-0.9.0/speedtools/specs/cam.ksy
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2023-09-12 21:57:35.000000 speedtools-0.9.0/speedtools/specs/can.ksy
+-rw-r--r--   0 runner    (1001) docker     (127)     6015 2023-09-12 21:57:35.000000 speedtools-0.9.0/speedtools/specs/fce.ksy
+-rw-r--r--   0 runner    (1001) docker     (127)    13941 2023-09-12 21:57:35.000000 speedtools-0.9.0/speedtools/specs/frd.ksy
+-rw-r--r--   0 runner    (1001) docker     (127)     4084 2023-09-12 21:57:35.000000 speedtools-0.9.0/speedtools/specs/fsh.ksy
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2023-09-12 21:57:35.000000 speedtools-0.9.0/speedtools/specs/qfs.ksy
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2023-09-12 21:57:35.000000 speedtools-0.9.0/speedtools/specs/viv.ksy
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2023-09-12 21:57:35.000000 speedtools-0.9.0/speedtools/speedtool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2333 2023-09-12 21:57:35.000000 speedtools-0.9.0/speedtools/tr_ini.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7186 2023-09-12 21:57:35.000000 speedtools-0.9.0/speedtools/track_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5283 2023-09-12 21:57:35.000000 speedtools-0.9.0/speedtools/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2452 2023-09-12 21:57:35.000000 speedtools-0.9.0/speedtools/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7376 2023-09-12 21:57:35.000000 speedtools-0.9.0/speedtools/viv_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-12 21:57:50.455525 speedtools-0.9.0/speedtools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3102 2023-09-12 21:57:50.000000 speedtools-0.9.0/speedtools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2023-09-12 21:57:50.000000 speedtools-0.9.0/speedtools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-12 21:57:50.000000 speedtools-0.9.0/speedtools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2023-09-12 21:57:50.000000 speedtools-0.9.0/speedtools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2023-09-12 21:57:50.000000 speedtools-0.9.0/speedtools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2023-09-12 21:57:50.000000 speedtools-0.9.0/speedtools.egg-info/top_level.txt
```

### Comparing `speedtools-0.8.0/LICENSE` & `speedtools-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `speedtools-0.8.0/PKG-INFO` & `speedtools-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: speedtools
-Version: 0.8.0
+Version: 0.9.0
 Summary: NFS4 HS (PC) resource utilities
 Author: Rafał Kuźnia
 Author-email: rafal.kuznia@protonmail.com
 License: GPL-3.0-or-later
 Project-URL: homepage, https://github.com/e-rk/speedtools
 Project-URL: repository, https://github.com/e-rk/speedtools
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

### Comparing `speedtools-0.8.0/README.md` & `speedtools-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `speedtools-0.8.0/pyproject.toml` & `speedtools-0.9.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "speedtools"
-version = "0.8.0"
+version = "0.9.0"
 description = "NFS4 HS (PC) resource utilities"
 authors = [{ name = "Rafał Kuźnia" }, { email = "rafal.kuznia@protonmail.com" }]
 readme = { file = 'README.md', content-type = 'text/markdown' }
 dependencies = ["kaitaistruct", "pillow", "click", "more-itertools", "parse"]
 license = { text = "GPL-3.0-or-later" }
 classifiers = [
     'License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)',
```

### Comparing `speedtools-0.8.0/setup.py` & `speedtools-0.9.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-#!/usr/bin/env python3
 #
 # Copyright (c) 2023 Rafał Kuźnia <rafal.kuznia@protonmail.com>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 #
 
 from pathlib import Path
```

### Comparing `speedtools-0.8.0/speedtools/blender/io_nfs4_import.py` & `speedtools-0.9.0/speedtools/blender/io_nfs4_import.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,27 +8,29 @@
 
 import logging
 from abc import ABCMeta, abstractmethod
 from collections.abc import Callable, Iterable
 from dataclasses import dataclass
 from functools import total_ordering
 from itertools import chain, groupby
+from math import pi
 from pathlib import Path
 from typing import Any
 
 import bpy
 import mathutils
 from bpy.props import BoolProperty, EnumProperty, StringProperty
 from more_itertools import collapse, duplicates_everseen, unique_everseen
 
 from speedtools import TrackData, VivData
 from speedtools.types import (
     Action,
     AnimationAction,
     BaseMesh,
+    Camera,
     DirectionalLight,
     DrawableMesh,
     Light,
     Matrix3x3,
     Part,
     Polygon,
     Resource,
@@ -177,17 +179,26 @@
         points = chain.from_iterable(fcurve.keyframe_points for fcurve in bpy_action.fcurves)
         for point in points:
             point.interpolation = "LINEAR"
         bpy_action.name = f"{obj.name}-action-{action.action}"
         track = anim_data.nla_tracks.new()
         track.strips.new(name=bpy_action.name, start=0, action=bpy_action)
 
-    def set_object_rotation(self, obj: bpy.types.Object, transform: Matrix3x3) -> None:
+    def set_object_rotation(
+        self,
+        obj: bpy.types.Object,
+        transform: Matrix3x3,
+        offset: mathutils.Euler | None = None,
+    ) -> None:
         mu_matrix = mathutils.Matrix(transform)
-        mu_euler = mu_matrix.to_euler("XYZ")  # type: ignore # pylint: disable=all
+        if offset:
+            mu_euler = offset
+            mu_euler.rotate(mu_matrix.to_euler("XYZ"))  # type: ignore # pylint: disable=all
+        else:
+            mu_euler = mu_matrix.to_euler("XYZ")  # type: ignore # pylint: disable=all
         obj.rotation_mode = "XYZ"
         obj.rotation_euler = mu_euler  # type: ignore[assignment]
 
     def make_drawable_object(
         self, name: str, mesh: DrawableMesh, import_shading: bool = False
     ) -> bpy.types.Object:
         bpy_mesh = self.make_base_mesh(name=name, mesh=mesh)
@@ -237,34 +248,44 @@
         bpy_sun = bpy.data.lights.new(name=name, type="SUN")
         bpy_obj = bpy.data.objects.new(name=name, object_data=bpy_sun)
         mu_euler = mathutils.Euler(light.euler_xyz)
         bpy_obj.rotation_mode = "XYZ"
         bpy_obj.rotation_euler = mu_euler  # type: ignore[assignment]
         return bpy_obj
 
+    def make_camera_object(self, name: str, camera: Camera) -> bpy.types.Object:
+        bpy_camera = bpy.data.cameras.new(name=name)
+        bpy_obj = bpy.data.objects.new(name=name, object_data=bpy_camera)
+        offset = mathutils.Euler((pi / 2, 0, 0))
+        self.set_object_location(obj=bpy_obj, location=camera.location)
+        self.set_object_rotation(obj=bpy_obj, transform=camera.transform, offset=offset)
+        return bpy_obj
+
 
 class TrackImportStrategy(metaclass=ABCMeta):
     @abstractmethod
     def import_track(
         self,
         track: TrackData,
         import_collision: bool = False,
         import_shading: bool = False,
         import_actions: bool = False,
+        import_cameras: bool = False,
     ) -> None:
         pass
 
 
 class TrackImportGLTF(TrackImportStrategy, BaseImporter):
     def import_track(
         self,
         track: TrackData,
         import_collision: bool = False,
         import_shading: bool = False,
         import_actions: bool = False,
+        import_cameras: bool = False,
     ) -> None:
         bpy.context.scene.render.fps = track.ANIMATION_FPS
         track_collection = bpy.data.collections.new("Track segments")
         bpy.context.scene.collection.children.link(track_collection)
         for index, segment in enumerate(track.track_segments):
             name = f"Segment {index}"
             segment_collection = bpy.data.collections.new(name=name)
@@ -307,14 +328,20 @@
             name = f"Light {index}"
             bpy_obj = self.make_light_object(name=name, light=light)
             light_collection.objects.link(bpy_obj)
         directional_light = track.directional_light
         if directional_light:
             bpy_obj = self.make_directional_light_object(name="sun", light=directional_light)
             light_collection.objects.link(bpy_obj)
+        if import_cameras:
+            camera_collection = bpy.data.collections.new("Cameras")
+            bpy.context.scene.collection.children.link(camera_collection)
+            for index, camera in enumerate(track.cameras):
+                bpy_obj = self.make_camera_object(name=f"Camera {index}", camera=camera)
+                camera_collection.objects.link(bpy_obj)
 
 
 class TrackImportBlender(TrackImportGLTF):
     def _link_texture_to_shader(
         self, node_tree: bpy.types.NodeTree, texture: bpy.types.Node, shader: bpy.types.Node
     ) -> None:
         color_attributes = node_tree.nodes.new("ShaderNodeAttribute")
@@ -398,14 +425,19 @@
         default=False,
     )
     import_actions: BoolProperty(  # type: ignore[valid-type]
         name="Import animation actions (experimental)",
         description="Import track animation actions from CAN files, such as object destruction animation",
         default=False,
     )
+    import_cameras: BoolProperty(  # type: ignore[valid-type]
+        name="Import cameras (experimental)",
+        description="Import track-specific replay cameras",
+        default=False,
+    )
 
     def invoke(self, context: bpy.types.Context, event: bpy.types.Event) -> set[int] | set[str]:
         wm = context.window_manager
         wm.fileselect_add(self)
         return {"RUNNING_MODAL"}
 
     def execute(self, context: bpy.types.Context) -> set[int] | set[str]:
@@ -429,14 +461,15 @@
         else:
             return {"CANCELLED"}
         import_strategy.import_track(
             track=track,
             import_collision=self.import_collision,
             import_shading=import_shading,
             import_actions=self.import_actions,
+            import_cameras=self.import_cameras,
         )
         return {"FINISHED"}
 
 
 class CarImporter(bpy.types.Operator):
     """Import NFS4 Car Operator"""
```

### Comparing `speedtools-0.8.0/speedtools/can_data.py` & `speedtools-0.9.0/speedtools/can_data.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-#!/usr/bin/env python3
 #
 # Copyright (c) 2023 Rafał Kuźnia <rafal.kuznia@protonmail.com>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 #
 
 from __future__ import annotations
```

### Comparing `speedtools-0.8.0/speedtools/frd_data.py` & `speedtools-0.9.0/speedtools/frd_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-#!/usr/bin/env python3
 #
 # Copyright (c) 2023 Rafał Kuźnia <rafal.kuznia@protonmail.com>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 #
 
 from __future__ import annotations
```

### Comparing `speedtools-0.8.0/speedtools/fsh_data.py` & `speedtools-0.9.0/speedtools/fsh_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-#!/usr/bin/env python3
 #
 # Copyright (c) 2023 Rafał Kuźnia <rafal.kuznia@protonmail.com>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 #
 
 from __future__ import annotations
```

### Comparing `speedtools-0.8.0/speedtools/refpack.py` & `speedtools-0.9.0/speedtools/refpack.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-#!/usr/bin/env python3
 #
 # Copyright (c) 2023 Rafał Kuźnia <rafal.kuznia@protonmail.com>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 #
 
 import logging
```

### Comparing `speedtools-0.8.0/speedtools/specs/can.ksy` & `speedtools-0.9.0/speedtools/specs/can.ksy`

 * *Files identical despite different names*

### Comparing `speedtools-0.8.0/speedtools/specs/fce.ksy` & `speedtools-0.9.0/speedtools/specs/fce.ksy`

 * *Files identical despite different names*

### Comparing `speedtools-0.8.0/speedtools/specs/frd.ksy` & `speedtools-0.9.0/speedtools/specs/frd.ksy`

 * *Files identical despite different names*

### Comparing `speedtools-0.8.0/speedtools/specs/fsh.ksy` & `speedtools-0.9.0/speedtools/specs/fsh.ksy`

 * *Files identical despite different names*

### Comparing `speedtools-0.8.0/speedtools/specs/viv.ksy` & `speedtools-0.9.0/speedtools/specs/viv.ksy`

 * *Files identical despite different names*

### Comparing `speedtools-0.8.0/speedtools/speedtool.py` & `speedtools-0.9.0/speedtools/speedtool.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-#!/usr/bin/env python3
 #
 # Copyright (c) 2023 Rafał Kuźnia <rafal.kuznia@protonmail.com>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 #
 
 import logging
```

### Comparing `speedtools-0.8.0/speedtools/tr_ini.py` & `speedtools-0.9.0/speedtools/tr_ini.py`

 * *Files identical despite different names*

### Comparing `speedtools-0.8.0/speedtools/track_data.py` & `speedtools-0.9.0/speedtools/track_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,30 @@
-#!/usr/bin/env python3
 #
 # Copyright (c) 2023 Rafał Kuźnia <rafal.kuznia@protonmail.com>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 #
 
 import logging
 from collections.abc import Callable, Iterable, Iterator, Sequence
 from contextlib import suppress
 from functools import partial
 from math import atan2, cos, tau
 from pathlib import Path
 from typing import TypeVar
 
+from speedtools.cam_data import CamData
 from speedtools.can_data import CanData
 from speedtools.frd_data import FrdData
 from speedtools.fsh_data import FshData
 from speedtools.tr_ini import TrackIni
 from speedtools.types import (
     Action,
     AnimationAction,
+    Camera,
     CollisionType,
     DirectionalLight,
     Light,
     LightAttributes,
     LightStub,
     Polygon,
     Resource,
@@ -86,14 +87,23 @@
             directory=directory,
             prefix="TR",
             postfix=".INI",
             mirrored=mirrored,
             night=night,
             weather=weather,
         )
+        self.cam: CamData = self.tr_open(
+            constructor=CamData.from_file,
+            directory=directory,
+            prefix="TR",
+            postfix=".CAM",
+            mirrored=mirrored,
+            night=night,
+            weather=weather,
+        )
         self.sfx: FshData = FshData.from_file(Path(game_root, self.SFX_RESOURCE_FILE))
         self.can: Sequence[tuple[Action, CanData]] = self.tr_can_open(directory=directory)
         self.resources: dict[int, Resource] = {}
         self.sfx_resources: dict[str, Resource] = {}
         self.light_glows: dict[int, LightAttributes] = {}
         self.mirrored: bool = mirrored
         self.night: bool = night
@@ -199,7 +209,11 @@
         # The INI angleRho value is not really a spherical coordinate.
         # Some approximations are done here to convert to spherical coordinates.
         rho = sun.angle_rho * tau
         z = self.SUN_DISTANCE * cos(rho)
         phi = atan2(z, self.SUN_DISTANCE)
         theta = sun.angle_theta * tau
         return DirectionalLight(rho=phi, theta=theta, radius=sun.radius)
+
+    @property
+    def cameras(self) -> Iterable[Camera]:
+        return self.cam.cameras
```

### Comparing `speedtools-0.8.0/speedtools/types.py` & `speedtools-0.9.0/speedtools/types.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-#!/usr/bin/env python3
 #
 # Copyright (c) 2023 Rafał Kuźnia <rafal.kuznia@protonmail.com>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 #
 
 from __future__ import annotations
@@ -240,7 +239,13 @@
     radius: float
 
     @property
     def euler_xyz(self) -> Vector3d:
         z = pi / 2 - self.rho
         y = self.theta
         return Vector3d(x=0, y=y, z=z)
+
+
+@dataclass(frozen=True)
+class Camera:
+    location: Vector3d
+    transform: Matrix3x3
```

### Comparing `speedtools-0.8.0/speedtools/utils.py` & `speedtools-0.9.0/speedtools/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-#!/usr/bin/env python3
 #
 # Copyright (c) 2023 Rafał Kuźnia <rafal.kuznia@protonmail.com>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 #
 
 import logging
```

### Comparing `speedtools-0.8.0/speedtools/viv_data.py` & `speedtools-0.9.0/speedtools/viv_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-#!/usr/bin/env python3
 #
 # Copyright (c) 2023 Rafał Kuźnia <rafal.kuznia@protonmail.com>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 #
 
 from __future__ import annotations
```

### Comparing `speedtools-0.8.0/speedtools.egg-info/PKG-INFO` & `speedtools-0.9.0/speedtools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: speedtools
-Version: 0.8.0
+Version: 0.9.0
 Summary: NFS4 HS (PC) resource utilities
 Author: Rafał Kuźnia
 Author-email: rafal.kuznia@protonmail.com
 License: GPL-3.0-or-later
 Project-URL: homepage, https://github.com/e-rk/speedtools
 Project-URL: repository, https://github.com/e-rk/speedtools
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

### Comparing `speedtools-0.8.0/speedtools.egg-info/SOURCES.txt` & `speedtools-0.9.0/speedtools.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 LICENSE
 README.md
 pyproject.toml
 setup.py
 speedtools/__init__.py
+speedtools/cam_data.py
 speedtools/can_data.py
 speedtools/frd_data.py
 speedtools/fsh_data.py
 speedtools/refpack.py
 speedtools/speedtool.py
 speedtools/tr_ini.py
 speedtools/track_data.py
@@ -17,13 +18,14 @@
 speedtools.egg-info/SOURCES.txt
 speedtools.egg-info/dependency_links.txt
 speedtools.egg-info/entry_points.txt
 speedtools.egg-info/requires.txt
 speedtools.egg-info/top_level.txt
 speedtools/blender/io_nfs4_import.py
 speedtools/parsers/__init__.py
+speedtools/specs/cam.ksy
 speedtools/specs/can.ksy
 speedtools/specs/fce.ksy
 speedtools/specs/frd.ksy
 speedtools/specs/fsh.ksy
 speedtools/specs/qfs.ksy
 speedtools/specs/viv.ksy
```

