# Comparing `tmp/py_ballisticcalc-2.0.0b3.tar.gz` & `tmp/py_ballisticcalc-2.0.0b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_ballisticcalc-2.0.0b3.tar", last modified: Thu Apr  4 18:32:36 2024, max compression
+gzip compressed data, was "py_ballisticcalc-2.0.0b4.tar", last modified: Sat Apr  6 18:22:49 2024, max compression
```

## Comparing `py_ballisticcalc-2.0.0b3.tar` & `py_ballisticcalc-2.0.0b4.tar`

### file list

```diff
@@ -1,36 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:32:36.717611 py_ballisticcalc-2.0.0b3/
--rw-r--r--   0 runner    (1001) docker     (127)     7817 2024-04-04 18:32:26.000000 py_ballisticcalc-2.0.0b3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    22793 2024-04-04 18:32:36.717611 py_ballisticcalc-2.0.0b3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12494 2024-04-04 18:32:26.000000 py_ballisticcalc-2.0.0b3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:32:36.713611 py_ballisticcalc-2.0.0b3/py_ballisticcalc/
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-04 18:32:26.000000 py_ballisticcalc-2.0.0b3/py_ballisticcalc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-04 18:32:26.000000 py_ballisticcalc-2.0.0b3/py_ballisticcalc/backend.py
--rw-r--r--   0 runner    (1001) docker     (127)    11322 2024-04-04 18:32:26.000000 py_ballisticcalc-2.0.0b3/py_ballisticcalc/conditions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6568 2024-04-04 18:32:26.000000 py_ballisticcalc-2.0.0b3/py_ballisticcalc/drag_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    22078 2024-04-04 18:32:26.000000 py_ballisticcalc-2.0.0b3/py_ballisticcalc/drag_tables.py
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-04 18:32:26.000000 py_ballisticcalc-2.0.0b3/py_ballisticcalc/example.py
--rw-r--r--   0 runner    (1001) docker     (127)     3281 2024-04-04 18:32:26.000000 py_ballisticcalc-2.0.0b3/py_ballisticcalc/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-04 18:32:26.000000 py_ballisticcalc-2.0.0b3/py_ballisticcalc/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     3608 2024-04-04 18:32:26.000000 py_ballisticcalc-2.0.0b3/py_ballisticcalc/munition.py
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-04-04 18:32:26.000000 py_ballisticcalc-2.0.0b3/py_ballisticcalc/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)    21137 2024-04-04 18:32:26.000000 py_ballisticcalc-2.0.0b3/py_ballisticcalc/trajectory_calc.py
--rw-r--r--   0 runner    (1001) docker     (127)    15701 2024-04-04 18:32:26.000000 py_ballisticcalc-2.0.0b3/py_ballisticcalc/trajectory_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    24075 2024-04-04 18:32:26.000000 py_ballisticcalc-2.0.0b3/py_ballisticcalc/unit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:32:36.717611 py_ballisticcalc-2.0.0b3/py_ballisticcalc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    22793 2024-04-04 18:32:36.000000 py_ballisticcalc-2.0.0b3/py_ballisticcalc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-04 18:32:36.000000 py_ballisticcalc-2.0.0b3/py_ballisticcalc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 18:32:36.000000 py_ballisticcalc-2.0.0b3/py_ballisticcalc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-04 18:32:36.000000 py_ballisticcalc-2.0.0b3/py_ballisticcalc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-04 18:32:36.000000 py_ballisticcalc-2.0.0b3/py_ballisticcalc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-04-04 18:32:26.000000 py_ballisticcalc-2.0.0b3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 18:32:36.717611 py_ballisticcalc-2.0.0b3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-04 18:32:26.000000 py_ballisticcalc-2.0.0b3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:32:36.717611 py_ballisticcalc-2.0.0b3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-04 18:32:26.000000 py_ballisticcalc-2.0.0b3/tests/test_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1796 2024-04-04 18:32:26.000000 py_ballisticcalc-2.0.0b3/tests/test_atmosphere.py
--rw-r--r--   0 runner    (1001) docker     (127)    10023 2024-04-04 18:32:26.000000 py_ballisticcalc-2.0.0b3/tests/test_computer.py
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-04-04 18:32:26.000000 py_ballisticcalc-2.0.0b3/tests/test_config_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-04-04 18:32:26.000000 py_ballisticcalc-2.0.0b3/tests/test_danger_space.py
--rw-r--r--   0 runner    (1001) docker     (127)     3999 2024-04-04 18:32:26.000000 py_ballisticcalc-2.0.0b3/tests/test_mbc.py
--rw-r--r--   0 runner    (1001) docker     (127)     5699 2024-04-04 18:32:26.000000 py_ballisticcalc-2.0.0b3/tests/test_trajectory.py
--rw-r--r--   0 runner    (1001) docker     (127)     6130 2024-04-04 18:32:26.000000 py_ballisticcalc-2.0.0b3/tests/test_units.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:22:49.968570 py_ballisticcalc-2.0.0b4/
+-rw-r--r--   0 runner    (1001) docker     (127)     7817 2024-04-06 18:22:40.000000 py_ballisticcalc-2.0.0b4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    22793 2024-04-06 18:22:49.964570 py_ballisticcalc-2.0.0b4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12494 2024-04-06 18:22:40.000000 py_ballisticcalc-2.0.0b4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:22:49.964570 py_ballisticcalc-2.0.0b4/py_ballisticcalc/
+-rw-r--r--   0 runner    (1001) docker     (127)     4981 2024-04-06 18:22:40.000000 py_ballisticcalc-2.0.0b4/py_ballisticcalc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-04-06 18:22:40.000000 py_ballisticcalc-2.0.0b4/py_ballisticcalc/backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11322 2024-04-06 18:22:40.000000 py_ballisticcalc-2.0.0b4/py_ballisticcalc/conditions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6568 2024-04-06 18:22:40.000000 py_ballisticcalc-2.0.0b4/py_ballisticcalc/drag_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22145 2024-04-06 18:22:40.000000 py_ballisticcalc-2.0.0b4/py_ballisticcalc/drag_tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-04-06 18:22:40.000000 py_ballisticcalc-2.0.0b4/py_ballisticcalc/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3281 2024-04-06 18:22:40.000000 py_ballisticcalc-2.0.0b4/py_ballisticcalc/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-06 18:22:40.000000 py_ballisticcalc-2.0.0b4/py_ballisticcalc/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3608 2024-04-06 18:22:40.000000 py_ballisticcalc-2.0.0b4/py_ballisticcalc/munition.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22327 2024-04-06 18:22:40.000000 py_ballisticcalc-2.0.0b4/py_ballisticcalc/trajectory_calc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15701 2024-04-06 18:22:40.000000 py_ballisticcalc-2.0.0b4/py_ballisticcalc/trajectory_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22572 2024-04-06 18:22:40.000000 py_ballisticcalc-2.0.0b4/py_ballisticcalc/unit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:22:49.964570 py_ballisticcalc-2.0.0b4/py_ballisticcalc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    22793 2024-04-06 18:22:49.000000 py_ballisticcalc-2.0.0b4/py_ballisticcalc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-06 18:22:49.000000 py_ballisticcalc-2.0.0b4/py_ballisticcalc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 18:22:49.000000 py_ballisticcalc-2.0.0b4/py_ballisticcalc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-06 18:22:49.000000 py_ballisticcalc-2.0.0b4/py_ballisticcalc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-06 18:22:49.000000 py_ballisticcalc-2.0.0b4/py_ballisticcalc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-04-06 18:22:40.000000 py_ballisticcalc-2.0.0b4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 18:22:49.968570 py_ballisticcalc-2.0.0b4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-06 18:22:40.000000 py_ballisticcalc-2.0.0b4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:22:49.964570 py_ballisticcalc-2.0.0b4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-06 18:22:40.000000 py_ballisticcalc-2.0.0b4/tests/test_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1796 2024-04-06 18:22:40.000000 py_ballisticcalc-2.0.0b4/tests/test_atmosphere.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10087 2024-04-06 18:22:40.000000 py_ballisticcalc-2.0.0b4/tests/test_computer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-04-06 18:22:40.000000 py_ballisticcalc-2.0.0b4/tests/test_config_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-04-06 18:22:40.000000 py_ballisticcalc-2.0.0b4/tests/test_danger_space.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3999 2024-04-06 18:22:40.000000 py_ballisticcalc-2.0.0b4/tests/test_mbc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5699 2024-04-06 18:22:40.000000 py_ballisticcalc-2.0.0b4/tests/test_trajectory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6054 2024-04-06 18:22:40.000000 py_ballisticcalc-2.0.0b4/tests/test_units.py
```

### Comparing `py_ballisticcalc-2.0.0b3/LICENSE` & `py_ballisticcalc-2.0.0b4/LICENSE`

 * *Files identical despite different names*

### Comparing `py_ballisticcalc-2.0.0b3/PKG-INFO` & `py_ballisticcalc-2.0.0b4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py_ballisticcalc
-Version: 2.0.0b3
+Version: 2.0.0b4
 Summary: LGPL library for small arms ballistic calculations (Python 3)
 Author-email: o-murphy <thehelixpg@gmail.com>, dbookstaber <bookstaber@gmail.com>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -186,15 +186,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: tomli; python_version < "3.11"
 Provides-Extra: exts
-Requires-Dist: py_ballisticcalc.exts==2.0.0b3; extra == "exts"
+Requires-Dist: py_ballisticcalc.exts==2.0.0b4; extra == "exts"
 Provides-Extra: lint
 Requires-Dist: pylint; extra == "lint"
 Requires-Dist: flake8; extra == "lint"
 Provides-Extra: charts
 Requires-Dist: matplotlib; extra == "charts"
 Requires-Dist: pandas; extra == "charts"
```

### Comparing `py_ballisticcalc-2.0.0b3/README.md` & `py_ballisticcalc-2.0.0b4/README.md`

 * *Files identical despite different names*

### Comparing `py_ballisticcalc-2.0.0b3/py_ballisticcalc/conditions.py` & `py_ballisticcalc-2.0.0b4/py_ballisticcalc/conditions.py`

 * *Files identical despite different names*

### Comparing `py_ballisticcalc-2.0.0b3/py_ballisticcalc/drag_model.py` & `py_ballisticcalc-2.0.0b4/py_ballisticcalc/drag_model.py`

 * *Files identical despite different names*

### Comparing `py_ballisticcalc-2.0.0b3/py_ballisticcalc/drag_tables.py` & `py_ballisticcalc-2.0.0b4/py_ballisticcalc/drag_tables.py`

 * *Files 0% similar despite different names*

```diff
@@ -663,7 +663,10 @@
     {'Mach': 3.75, 'CD': 0.9355},
     {'Mach': 3.80, 'CD': 0.9340},
     {'Mach': 3.85, 'CD': 0.9325},
     {'Mach': 3.90, 'CD': 0.9310},
     {'Mach': 3.95, 'CD': 0.9295},
     {'Mach': 4.00, 'CD': 0.9280},
 ]
+
+
+__all__ = ["TableG%s" % n for n in (1, 7, 2, 5, 6, 8, 'I', 'S')]
```

### Comparing `py_ballisticcalc-2.0.0b3/py_ballisticcalc/example.py` & `py_ballisticcalc-2.0.0b4/py_ballisticcalc/example.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 """Example of library usage"""
 
 # pylint: disable=wildcard-import,unused-wildcard-import
 from py_ballisticcalc import *
-from py_ballisticcalc import Settings as Set
+
 
 # Modify default prefer_units
 PreferredUnits.velocity = Velocity.FPS
 PreferredUnits.temperature = Temperature.Celsius
 PreferredUnits.distance = Distance.Meter
 PreferredUnits.sight_height = Distance.Centimeter
 
-Set.USE_POWDER_SENSITIVITY = True  # Correct muzzle velocity for powder temperature
+set_global_use_powder_sensitivity(True)  # Correct muzzle velocity for powder temperature
 
 # Define ammunition parameters
 weight, diameter = 168, 0.308  # Numbers will be assumed to use default Settings.Units
 length = Distance.Inch(1.282)  # Or declare prefer_units explicitly
 dm = DragModel(0.223, TableG7, weight, diameter, length)
 ammo = Ammo(dm, 2750, 15)
 ammo.calc_powder_sens(2723, 0)
```

### Comparing `py_ballisticcalc-2.0.0b3/py_ballisticcalc/interface.py` & `py_ballisticcalc-2.0.0b4/py_ballisticcalc/interface.py`

 * *Files identical despite different names*

### Comparing `py_ballisticcalc-2.0.0b3/py_ballisticcalc/munition.py` & `py_ballisticcalc-2.0.0b4/py_ballisticcalc/munition.py`

 * *Files identical despite different names*

### Comparing `py_ballisticcalc-2.0.0b3/py_ballisticcalc/trajectory_calc.py` & `py_ballisticcalc-2.0.0b4/py_ballisticcalc/trajectory_calc.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,26 +5,63 @@
 import math
 from dataclasses import dataclass
 from typing import NamedTuple
 
 from .drag_model import DragDataPoint
 from .conditions import Atmo, Shot, Wind
 from .munition import Ammo
-from .settings import Settings
 from .trajectory_data import TrajectoryData, TrajFlag
-from .unit import Distance, Angular, Velocity, Weight, Energy, Pressure, Temperature
+from .unit import Distance, Angular, Velocity, Weight, Energy, Pressure, Temperature, PreferredUnits
 
-__all__ = ('TrajectoryCalc',)
+__all__ = (
+    'TrajectoryCalc',
+    'get_global_max_calc_step_size',
+    'get_global_use_powder_sensitivity',
+    'set_global_max_calc_step_size',
+    'set_global_use_powder_sensitivity',
+    'reset_globals'
+)
 
 cZeroFindingAccuracy = 0.000005
 cMinimumVelocity = 50.0
 cMaximumDrop = -15000
 cMaxIterations = 20
 cGravityConstant = -32.17405
 
+_globalUsePowderSensitivity = False
+_globalMaxCalcStepSize = Distance.Foot(0.5)
+
+
+def get_global_max_calc_step_size() -> Distance:
+    return _globalMaxCalcStepSize
+
+
+def get_global_use_powder_sensitivity() -> bool:
+    return _globalUsePowderSensitivity
+
+
+def reset_globals() -> None:
+    global _globalUsePowderSensitivity, _globalMaxCalcStepSize
+    _globalUsePowderSensitivity = False
+    _globalMaxCalcStepSize = Distance.Foot(0.5)
+
+
+def set_global_max_calc_step_size(value: [float, Distance]) -> None:
+    global _globalMaxCalcStepSize
+    if (_value := PreferredUnits.distance(value)).raw_value <= 0:
+        raise ValueError("_globalMaxCalcStepSize have to be > 0")
+    _globalMaxCalcStepSize = PreferredUnits.distance(value)
+
+
+def set_global_use_powder_sensitivity(value: bool) -> None:
+    global _globalUsePowderSensitivity
+    if not isinstance(value, bool):
+        raise TypeError(f"set_global_use_powder_sensitivity {value=} is not a boolean")
+    _globalUsePowderSensitivity = value
+
 
 class CurvePoint(NamedTuple):
     """Coefficients for quadratic interpolation"""
     a: float
     b: float
     c: float
 
@@ -106,17 +143,18 @@
 
     @staticmethod
     def get_calc_step(step: float = 0):
         """Keep step under max_calc_step_size
         :param step: proposed step size
         :return: step size for calculations (in feet)
         """
+        preferred_step = _globalMaxCalcStepSize >> Distance.Foot
         if step == 0:
-            return Settings.get_max_calc_step_size() / 2.0
-        return min(step, Settings.get_max_calc_step_size()) / 2.0
+            return preferred_step / 2.0
+        return min(step, preferred_step) / 2.0
 
     def trajectory(self, shot_info: Shot, max_range: Distance, dist_step: Distance,
                    extra_data: bool = False):
         filter_flags = TrajFlag.RANGE
 
         if extra_data:
             dist_step = Distance.Foot(0.2)
@@ -134,15 +172,15 @@
         self.barrel_elevation = shot_info.barrel_elevation >> Angular.Radian
         self.barrel_azimuth = shot_info.barrel_azimuth >> Angular.Radian
         self.sight_height = shot_info.weapon.sight_height >> Distance.Foot
         self.cant_cosine = math.cos(shot_info.cant_angle >> Angular.Radian)
         self.cant_sine = math.sin(shot_info.cant_angle >> Angular.Radian)
         self.alt0 = shot_info.atmo.altitude >> Distance.Foot
         self.calc_step = self.get_calc_step()
-        if Settings.USE_POWDER_SENSITIVITY:
+        if _globalUsePowderSensitivity:
             self.muzzle_velocity = shot_info.ammo.get_velocity_for_temp(shot_info.atmo.temperature) >> Velocity.FPS
         else:
             self.muzzle_velocity = shot_info.ammo.mv >> Velocity.FPS
         self.stability_coefficient = self.calc_stability_coefficient(shot_info.atmo)
 
     def zero_angle(self, shot_info: Shot, distance: Distance) -> Angular:
         """Iterative algorithm to find barrel elevation needed for a particular zero
```

### Comparing `py_ballisticcalc-2.0.0b3/py_ballisticcalc/trajectory_data.py` & `py_ballisticcalc-2.0.0b4/py_ballisticcalc/trajectory_data.py`

 * *Files identical despite different names*

### Comparing `py_ballisticcalc-2.0.0b3/py_ballisticcalc/unit.py` & `py_ballisticcalc-2.0.0b4/py_ballisticcalc/unit.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,25 @@
 """
 Useful types for prefer_units of measurement conversion for ballistics calculations
 """
-import os
+
 import sys
 from abc import ABC, abstractmethod
 from dataclasses import dataclass, MISSING, Field
 from enum import IntEnum
 from math import pi, atan, tan
 from typing import NamedTuple, Union, TypeVar
 
 from py_ballisticcalc.logger import logger
 
-try:
-    import tomllib
-except ImportError:
-    import tomli as tomllib
 
-__all__ = ('Unit', 'AbstractUnit', 'UnitProps', 'UnitPropsDict', 'Distance',
+__all__ = ('Unit', 'AbstractUnit', 'AbstractUnitType', 'UnitProps',
+           'UnitPropsDict', 'Distance',
            'Velocity', 'Angular', 'Temperature', 'Pressure',
-           'Energy', 'Weight', 'Dimension', 'PreferredUnits', 'basicConfig')
+           'Energy', 'Weight', 'Dimension', 'PreferredUnits')
 
 
 AbstractUnitType = TypeVar('AbstractUnitType', bound='AbstractUnit')
 
 
 # pylint: disable=invalid-name
 class Unit(IntEnum):
@@ -668,80 +665,50 @@
                         value = PreferredUnits.__dict__[units](value)
                     else:
                         raise TypeError(f"Unsupported unit or dimension use one of {PreferredUnits}")
 
             super().__setattr__(key, value)
 
     @classmethod
+    def defaults(self):
+        """resets preferred units to defaults"""
+        self.angular = Unit.Degree
+        self.distance = Unit.Yard
+        self.velocity = Unit.FPS
+        self.pressure = Unit.InHg
+        self.temperature = Unit.Fahrenheit
+        self.diameter = Unit.Inch
+        self.length = Unit.Inch
+        self.weight = Unit.Grain
+        self.adjustment = Unit.Mil
+        self.drop = Unit.Inch
+        self.energy = Unit.FootPound
+        self.ogw = Unit.Pound
+        self.sight_height = Unit.Inch
+        self.target_height = Unit.Inch
+        self.twist = Unit.Inch
+
+    @classmethod
     def set(cls, **kwargs):
         """set preferred units from Mapping"""
         for attribute, value in kwargs.items():
-            try:
-                if hasattr(PreferredUnits, attribute):
-                    setattr(PreferredUnits, attribute, Unit[value])
-                else:
-                    logger.warning(f"{attribute=} not found in preferred_units")
-            except KeyError:
-                logger.warning(f"{value=} not found in preferred_units")
 
-    @classmethod
-    def _load_config(cls, filepath=None):
-
-        def find_pybc_toml(start_dir=os.path.dirname(__file__)):
-            """
-            Search for the pyproject.toml file starting from the specified directory.
-            :param start_dir: (str) The directory to start searching from. Default is the current working directory.
-            :return: str: The absolute path to the pyproject.toml file if found, otherwise None.
-            """
-            current_dir = os.path.abspath(start_dir)
-            while True:
-                # Check if pybc.toml or .pybc.toml exists in the current directory
-                pybc_paths = [
-                    os.path.join(current_dir, '.pybc.toml'),
-                    os.path.join(current_dir, 'pybc.toml'),
-                ]
-                for pypc_path in pybc_paths:
-                    if os.path.exists(pypc_path):
-                        return os.path.abspath(pypc_path)
-
-                # Move to the parent directory
-                parent_dir = os.path.dirname(current_dir)
-
-                # If we have reached the root directory, stop searching
-                if parent_dir == current_dir:
-                    return None
-
-                current_dir = parent_dir
-
-        if filepath is None:
-            filepath = find_pybc_toml()
-
-        with open(filepath, "rb") as fp:
-            _config = tomllib.load(fp)
-
-            if _pybc := _config.get('pybc'):
-                if preferred_units := _pybc.get('preferred_units'):
-                    cls.set(**preferred_units)
+            if hasattr(PreferredUnits, attribute):
+                if isinstance(value, Unit):
+                    setattr(PreferredUnits, attribute, value)
+                elif isinstance(value, str):
+                    try:
+                        setattr(PreferredUnits, attribute, Unit[value])
+                    except KeyError:
+                        logger.warning(f"{value=} not a member of Unit")
                 else:
-                    logger.warning("Config has not `pybc.preferred_units` section")
+                    logger.warning(f"type of {value=} have not been converted to a member of Unit")
             else:
-                logger.warning("Config has not `pybc` section")
+                logger.warning(f"{attribute=} not found in preferred_units")
 
-    @classmethod
-    def basic_config(cls, filename=None, **preferred_units):
-        """
-        Method to load preferred units from file or Mapping
-        """
-        if filename and preferred_units:
-            raise ValueError("Can't use preferred_units and config file at same time")
-        if preferred_units:
-            cls.set(**preferred_units)
-        else:
-            # trying to load definitions from pybc.toml
-            cls._load_config(filename)
 
 
 # pylint: disable=redefined-builtin,too-few-public-methods,too-many-arguments
 class Dimension(Field):
     """
     Definition of measure units specified field for
     PreferredUnits.Mixin based dataclasses
@@ -770,13 +737,7 @@
     @abstractmethod
     def __rshift__(self, other):
         ...
 
     @abstractmethod
     def __lshift__(self, other):
         ...
-
-
-PreferredUnits.basic_config()  # init PreferredUnits
-
-# export method globally
-basicConfig = PreferredUnits.basic_config
```

### Comparing `py_ballisticcalc-2.0.0b3/py_ballisticcalc.egg-info/PKG-INFO` & `py_ballisticcalc-2.0.0b4/py_ballisticcalc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py_ballisticcalc
-Version: 2.0.0b3
+Version: 2.0.0b4
 Summary: LGPL library for small arms ballistic calculations (Python 3)
 Author-email: o-murphy <thehelixpg@gmail.com>, dbookstaber <bookstaber@gmail.com>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -186,15 +186,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: tomli; python_version < "3.11"
 Provides-Extra: exts
-Requires-Dist: py_ballisticcalc.exts==2.0.0b3; extra == "exts"
+Requires-Dist: py_ballisticcalc.exts==2.0.0b4; extra == "exts"
 Provides-Extra: lint
 Requires-Dist: pylint; extra == "lint"
 Requires-Dist: flake8; extra == "lint"
 Provides-Extra: charts
 Requires-Dist: matplotlib; extra == "charts"
 Requires-Dist: pandas; extra == "charts"
```

### Comparing `py_ballisticcalc-2.0.0b3/py_ballisticcalc.egg-info/SOURCES.txt` & `py_ballisticcalc-2.0.0b4/py_ballisticcalc.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 py_ballisticcalc/conditions.py
 py_ballisticcalc/drag_model.py
 py_ballisticcalc/drag_tables.py
 py_ballisticcalc/example.py
 py_ballisticcalc/interface.py
 py_ballisticcalc/logger.py
 py_ballisticcalc/munition.py
-py_ballisticcalc/settings.py
 py_ballisticcalc/trajectory_calc.py
 py_ballisticcalc/trajectory_data.py
 py_ballisticcalc/unit.py
 py_ballisticcalc.egg-info/PKG-INFO
 py_ballisticcalc.egg-info/SOURCES.txt
 py_ballisticcalc.egg-info/dependency_links.txt
 py_ballisticcalc.egg-info/requires.txt
```

### Comparing `py_ballisticcalc-2.0.0b3/pyproject.toml` & `py_ballisticcalc-2.0.0b4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "py_ballisticcalc"
-version = "2.0.0b3"
+version = "2.0.0b4"
 
 authors = [
     { name="o-murphy", email="thehelixpg@gmail.com" },
     { name="dbookstaber", email="bookstaber@gmail.com"}
 ]
 description = "LGPL library for small arms ballistic calculations (Python 3)"
 readme = "README.md"
@@ -50,10 +50,10 @@
 [tool.setuptools.packages.find]
 where = ["."]
 include = ["py_ballisticcalc*"]  # alternatively: `exclude = ["additional*"]`
 exclude = ["py_ballisticcalc_exts*"]
 
 
 [project.optional-dependencies]
-exts = ['py_ballisticcalc.exts==2.0.0b3']
+exts = ['py_ballisticcalc.exts==2.0.0b4']
 lint = ['pylint', 'flake8']
 charts = ['matplotlib', 'pandas']
```

### Comparing `py_ballisticcalc-2.0.0b3/tests/test_atmosphere.py` & `py_ballisticcalc-2.0.0b4/tests/test_atmosphere.py`

 * *Files identical despite different names*

### Comparing `py_ballisticcalc-2.0.0b3/tests/test_computer.py` & `py_ballisticcalc-2.0.0b4/tests/test_computer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 """Unittests for the py_ballisticcalc library"""
 
 import unittest
 import copy
-from py_ballisticcalc import DragModel, Ammo, Weapon, Calculator, Shot, Wind, Atmo, TableG7
-from py_ballisticcalc import Settings as Set
+from py_ballisticcalc import (
+    DragModel, Ammo, Weapon, Calculator, Shot, Wind, Atmo, TableG7,
+    get_global_use_powder_sensitivity, set_global_use_powder_sensitivity
+)
 from py_ballisticcalc.unit import *
 
+
 class TestComputer(unittest.TestCase):
     """Basic verifications that wind, spin, and cant values produce effects of correct sign and magnitude"""
 
     def setUp(self):
         """Baseline shot has barrel at zero elevation"""
         self.range = 1000
         self.step = 100
@@ -156,21 +159,21 @@
         tdm = DragModel(self.dm.BC, self.dm.drag_table)
         tammo = Ammo(tdm, mv=self.ammo.mv)
         shot = Shot(weapon=self.weapon, ammo=tammo, atmo=self.atmosphere)
         t = self.calc.fire(shot=shot, trajectory_range=self.range, trajectory_step=self.step)
         self.assertEqual(t.trajectory[5].height, self.baseline_trajectory[5].height)
 
     def test_powder_sensitivity(self):
-        """With USE_POWDER_SENSITIVITY: Reducing temperature should reduce muzzle velocity"""
-        previous = Set.USE_POWDER_SENSITIVITY
-        Set.USE_POWDER_SENSITIVITY = True
+        """With _globalUsePowderSensitivity: Reducing temperature should reduce muzzle velocity"""
+        previous = get_global_use_powder_sensitivity()
+        set_global_use_powder_sensitivity(True)
         self.ammo.calc_powder_sens(Velocity.FPS(2550), Temperature.Celsius(0))
         cold = Atmo(temperature=Temperature.Celsius(-5))
         shot = Shot(weapon=self.weapon, ammo=self.ammo, atmo=cold)
         t = self.calc.fire(shot=shot, trajectory_range=self.range, trajectory_step=self.step)
         self.assertLess(t.trajectory[0].velocity, self.baseline_trajectory[0].velocity)
-        Set.USE_POWDER_SENSITIVITY = previous
+        set_global_use_powder_sensitivity(previous)
 
 #endregion Ammo
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `py_ballisticcalc-2.0.0b3/tests/test_config_loader.py` & `py_ballisticcalc-2.0.0b4/tests/test_config_loader.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,40 @@
 import os
 from unittest import TestCase
-from py_ballisticcalc import basicConfig, PreferredUnits, Unit
+from py_ballisticcalc import (basicConfig, PreferredUnits, Unit,
+                              get_global_max_calc_step_size, reset_globals)
+
+ASSETS_DIR = os.path.join(
+    os.path.dirname(
+        os.path.dirname(__file__)
+    ), 'assets')
 
 
 class TestConfigLoader(TestCase):
 
     def test_preferred_units_load(self):
-        basicConfig()
-        self.assertEqual(PreferredUnits.distance, Unit.Yard)
-
-    def test_custom_config_path(self):
-
-        assets_dir = os.path.join(
-            os.path.dirname(
-                os.path.dirname(__file__)
-            ), 'assets')
-
-        basicConfig(os.path.join(assets_dir, ".pybc-imperial.toml"))
-        self.assertEqual(PreferredUnits.distance, Unit.Foot)
-
-        basicConfig(os.path.join(assets_dir, ".pybc-metrics.toml"))
-        self.assertEqual(PreferredUnits.distance, Unit.Meter)
-
-        basicConfig(os.path.join(assets_dir, ".pybc-mixed.toml"))
-        self.assertEqual(PreferredUnits.velocity, Unit.MPS)
-
+        with self.subTest("env"):
+            basicConfig()
+            self.assertEqual(PreferredUnits.distance, Unit.Yard)
+
+        with self.subTest("manual"):
+            basicConfig(max_calc_step_size=Unit.Meter(0.3), preferred_units={
+                'distance': Unit.Meter
+            })
+            self.assertEqual(get_global_max_calc_step_size().units, Unit.Meter)
+            self.assertEqual(PreferredUnits.distance, Unit.Meter)
+
+        with self.subTest("imperial"):
+            basicConfig(os.path.join(ASSETS_DIR, ".pybc-imperial.toml"))
+            self.assertEqual(PreferredUnits.distance, Unit.Foot)
+
+        with self.subTest("mixed"):
+            basicConfig(os.path.join(ASSETS_DIR, ".pybc-metrics.toml"))
+            self.assertEqual(PreferredUnits.distance, Unit.Meter)
+
+        with self.subTest("mixed"):
+            basicConfig(os.path.join(ASSETS_DIR, ".pybc-mixed.toml"))
+            self.assertEqual(PreferredUnits.velocity, Unit.MPS)
 
+        basicConfig()
+        reset_globals()
+        PreferredUnits.defaults()
```

### Comparing `py_ballisticcalc-2.0.0b3/tests/test_danger_space.py` & `py_ballisticcalc-2.0.0b4/tests/test_danger_space.py`

 * *Files identical despite different names*

### Comparing `py_ballisticcalc-2.0.0b3/tests/test_mbc.py` & `py_ballisticcalc-2.0.0b4/tests/test_mbc.py`

 * *Files identical despite different names*

### Comparing `py_ballisticcalc-2.0.0b3/tests/test_trajectory.py` & `py_ballisticcalc-2.0.0b4/tests/test_trajectory.py`

 * *Files identical despite different names*

### Comparing `py_ballisticcalc-2.0.0b3/tests/test_units.py` & `py_ballisticcalc-2.0.0b4/tests/test_units.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,22 @@
-import typing
 import unittest
-import warnings
-from dataclasses import field, dataclass
+from dataclasses import dataclass
 
-from py_ballisticcalc import Settings
 from py_ballisticcalc.unit import *
 
 
 def back_n_forth(test, value, units):
     u = test.unit_class(value, units)
     v = u >> units
     test.assertAlmostEqual(v, value, 7, f'Read back failed for {units}')
 
 
 class TestPrefUnits(unittest.TestCase):
 
     def test_pref(self):
-
         @dataclass
         class TestClass(PreferredUnits.Mixin):
             as_metadata_str: [float, Distance] = Dimension(prefer_units='sight_height')
             as_metadata_unit: [float, Distance] = Dimension(prefer_units=Unit.Meter)
 
         tc1 = TestClass(1, 1)
         self.assertEqual(tc1.as_metadata_str.units, Unit.Inch)
```

