# Comparing `tmp/sdss_hal-1.1.4.tar.gz` & `tmp/sdss_hal-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdss_hal-1.1.4.tar", max compression
+gzip compressed data, was "sdss_hal-1.1.5.tar", max compression
```

## Comparing `sdss_hal-1.1.4.tar` & `sdss_hal-1.1.5.tar`

### file list

```diff
@@ -1,46 +1,46 @@
--rw-r--r--   0        0        0     1504 2024-04-05 21:33:19.332700 sdss_hal-1.1.4/LICENSE.md
--rw-r--r--   0        0        0      816 2024-04-05 21:33:19.332700 sdss_hal-1.1.4/README.md
--rw-r--r--   0        0        0     2644 2024-04-05 21:33:19.336700 sdss_hal-1.1.4/pyproject.toml
--rw-r--r--   0        0        0      483 2024-04-05 21:33:19.336700 sdss_hal-1.1.4/src/hal/__init__.py
--rw-r--r--   0        0        0     1761 2024-04-05 21:33:19.336700 sdss_hal-1.1.4/src/hal/__main__.py
--rw-r--r--   0        0        0      356 2024-04-05 21:33:19.336700 sdss_hal-1.1.4/src/hal/actor/__init__.py
--rw-r--r--   0        0        0     3070 2024-04-05 21:33:19.336700 sdss_hal-1.1.4/src/hal/actor/actor.py
--rw-r--r--   0        0        0     2939 2024-04-05 21:33:19.336700 sdss_hal-1.1.4/src/hal/actor/commands/__init__.py
--rw-r--r--   0        0        0     3761 2024-04-05 21:33:19.336700 sdss_hal-1.1.4/src/hal/actor/commands/auto.py
--rw-r--r--   0        0        0     1593 2024-04-05 21:33:19.336700 sdss_hal-1.1.4/src/hal/actor/commands/bypass.py
--rw-r--r--   0        0        0      844 2024-04-05 21:33:19.336700 sdss_hal-1.1.4/src/hal/actor/commands/calibrations.py
--rw-r--r--   0        0        0     7973 2024-04-05 21:33:19.336700 sdss_hal-1.1.4/src/hal/actor/commands/expose.py
--rw-r--r--   0        0        0     1669 2024-04-05 21:33:19.336700 sdss_hal-1.1.4/src/hal/actor/commands/goto.py
--rw-r--r--   0        0        0     4370 2024-04-05 21:33:19.336700 sdss_hal-1.1.4/src/hal/actor/commands/goto_field.py
--rw-r--r--   0        0        0     2455 2024-04-05 21:33:19.336700 sdss_hal-1.1.4/src/hal/actor/commands/script.py
--rw-r--r--   0        0        0     1419 2024-04-05 21:33:19.336700 sdss_hal-1.1.4/src/hal/actor/commands/status.py
--rw-r--r--   0        0        0      687 2024-04-05 21:33:19.336700 sdss_hal-1.1.4/src/hal/actor/commands/test.py
--rw-r--r--   0        0        0     3092 2024-04-05 21:33:19.336700 sdss_hal-1.1.4/src/hal/etc/hal.yml
--rw-r--r--   0        0        0     2189 2024-04-05 21:33:19.336700 sdss_hal-1.1.4/src/hal/etc/schema.json
--rw-r--r--   0        0        0      346 2024-04-05 21:33:19.336700 sdss_hal-1.1.4/src/hal/etc/scripts/apo/cartchange.inp
--rw-r--r--   0        0        0     1161 2024-04-05 21:33:19.336700 sdss_hal-1.1.4/src/hal/etc/scripts/apo/eveningcals.inp
--rw-r--r--   0        0        0      161 2024-04-05 21:33:19.336700 sdss_hal-1.1.4/src/hal/etc/scripts/apo/example.inp
--rw-r--r--   0        0        0     1616 2024-04-05 21:33:19.336700 sdss_hal-1.1.4/src/hal/etc/scripts/apo/morningcals.inp
--rw-r--r--   0        0        0       35 2024-04-05 21:33:19.336700 sdss_hal-1.1.4/src/hal/etc/scripts/apo/test.inp
--rw-r--r--   0        0        0      346 2024-04-05 21:33:19.336700 sdss_hal-1.1.4/src/hal/etc/scripts/lco/cartchange.inp
--rw-r--r--   0        0        0     1056 2024-04-05 21:33:19.336700 sdss_hal-1.1.4/src/hal/etc/scripts/lco/eveningcals.inp
--rw-r--r--   0        0        0     1450 2024-04-05 21:33:19.336700 sdss_hal-1.1.4/src/hal/etc/scripts/lco/morningcals.inp
--rw-r--r--   0        0        0     1180 2024-04-05 21:33:19.336700 sdss_hal-1.1.4/src/hal/exceptions.py
--rw-r--r--   0        0        0     2373 2024-04-05 21:33:19.336700 sdss_hal-1.1.4/src/hal/helpers/__init__.py
--rw-r--r--   0        0        0    10224 2024-04-05 21:33:19.336700 sdss_hal-1.1.4/src/hal/helpers/apogee.py
--rw-r--r--   0        0        0     6825 2024-04-05 21:33:19.336700 sdss_hal-1.1.4/src/hal/helpers/boss.py
--rw-r--r--   0        0        0     5011 2024-04-05 21:33:19.336700 sdss_hal-1.1.4/src/hal/helpers/cherno.py
--rw-r--r--   0        0        0     1769 2024-04-05 21:33:19.336700 sdss_hal-1.1.4/src/hal/helpers/ffs.py
--rw-r--r--   0        0        0     6710 2024-04-05 21:33:19.336700 sdss_hal-1.1.4/src/hal/helpers/jaeger.py
--rw-r--r--   0        0        0    10429 2024-04-05 21:33:19.336700 sdss_hal-1.1.4/src/hal/helpers/lamps.py
--rw-r--r--   0        0        0     4732 2024-04-05 21:33:19.336700 sdss_hal-1.1.4/src/hal/helpers/overhead.py
--rw-r--r--   0        0        0     4671 2024-04-05 21:33:19.340700 sdss_hal-1.1.4/src/hal/helpers/scripts.py
--rw-r--r--   0        0        0    13441 2024-04-05 21:33:19.340700 sdss_hal-1.1.4/src/hal/helpers/tcc.py
--rw-r--r--   0        0        0     1385 2024-04-05 21:33:19.340700 sdss_hal-1.1.4/src/hal/macros/__init__.py
--rw-r--r--   0        0        0     3844 2024-04-05 21:33:19.340700 sdss_hal-1.1.4/src/hal/macros/apogee_dome_flat.py
--rw-r--r--   0        0        0     7601 2024-04-05 21:33:19.340700 sdss_hal-1.1.4/src/hal/macros/auto.py
--rw-r--r--   0        0        0    21007 2024-04-05 21:33:19.340700 sdss_hal-1.1.4/src/hal/macros/expose.py
--rw-r--r--   0        0        0    23236 2024-04-05 21:33:19.340700 sdss_hal-1.1.4/src/hal/macros/goto_field.py
--rw-r--r--   0        0        0    18518 2024-04-05 21:33:19.340700 sdss_hal-1.1.4/src/hal/macros/macro.py
--rw-r--r--   0        0        0     1263 2024-04-05 21:33:19.340700 sdss_hal-1.1.4/src/hal/macros/test_macro.py
--rw-r--r--   0        0        0     2168 1970-01-01 00:00:00.000000 sdss_hal-1.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1504 2024-04-06 17:06:12.659793 sdss_hal-1.1.5/LICENSE.md
+-rw-r--r--   0        0        0      816 2024-04-06 17:06:12.663793 sdss_hal-1.1.5/README.md
+-rw-r--r--   0        0        0     2644 2024-04-06 17:06:12.663793 sdss_hal-1.1.5/pyproject.toml
+-rw-r--r--   0        0        0      483 2024-04-06 17:06:12.667793 sdss_hal-1.1.5/src/hal/__init__.py
+-rw-r--r--   0        0        0     1761 2024-04-06 17:06:12.667793 sdss_hal-1.1.5/src/hal/__main__.py
+-rw-r--r--   0        0        0      356 2024-04-06 17:06:12.667793 sdss_hal-1.1.5/src/hal/actor/__init__.py
+-rw-r--r--   0        0        0     3070 2024-04-06 17:06:12.667793 sdss_hal-1.1.5/src/hal/actor/actor.py
+-rw-r--r--   0        0        0     2939 2024-04-06 17:06:12.667793 sdss_hal-1.1.5/src/hal/actor/commands/__init__.py
+-rw-r--r--   0        0        0     3761 2024-04-06 17:06:12.667793 sdss_hal-1.1.5/src/hal/actor/commands/auto.py
+-rw-r--r--   0        0        0     1593 2024-04-06 17:06:12.667793 sdss_hal-1.1.5/src/hal/actor/commands/bypass.py
+-rw-r--r--   0        0        0      844 2024-04-06 17:06:12.667793 sdss_hal-1.1.5/src/hal/actor/commands/calibrations.py
+-rw-r--r--   0        0        0     7973 2024-04-06 17:06:12.667793 sdss_hal-1.1.5/src/hal/actor/commands/expose.py
+-rw-r--r--   0        0        0     1669 2024-04-06 17:06:12.667793 sdss_hal-1.1.5/src/hal/actor/commands/goto.py
+-rw-r--r--   0        0        0     4434 2024-04-06 17:06:12.667793 sdss_hal-1.1.5/src/hal/actor/commands/goto_field.py
+-rw-r--r--   0        0        0     2455 2024-04-06 17:06:12.667793 sdss_hal-1.1.5/src/hal/actor/commands/script.py
+-rw-r--r--   0        0        0     1419 2024-04-06 17:06:12.667793 sdss_hal-1.1.5/src/hal/actor/commands/status.py
+-rw-r--r--   0        0        0      687 2024-04-06 17:06:12.667793 sdss_hal-1.1.5/src/hal/actor/commands/test.py
+-rw-r--r--   0        0        0     3092 2024-04-06 17:06:12.667793 sdss_hal-1.1.5/src/hal/etc/hal.yml
+-rw-r--r--   0        0        0     2189 2024-04-06 17:06:12.667793 sdss_hal-1.1.5/src/hal/etc/schema.json
+-rw-r--r--   0        0        0      346 2024-04-06 17:06:12.667793 sdss_hal-1.1.5/src/hal/etc/scripts/apo/cartchange.inp
+-rw-r--r--   0        0        0     1161 2024-04-06 17:06:12.667793 sdss_hal-1.1.5/src/hal/etc/scripts/apo/eveningcals.inp
+-rw-r--r--   0        0        0      161 2024-04-06 17:06:12.667793 sdss_hal-1.1.5/src/hal/etc/scripts/apo/example.inp
+-rw-r--r--   0        0        0     1616 2024-04-06 17:06:12.667793 sdss_hal-1.1.5/src/hal/etc/scripts/apo/morningcals.inp
+-rw-r--r--   0        0        0       35 2024-04-06 17:06:12.667793 sdss_hal-1.1.5/src/hal/etc/scripts/apo/test.inp
+-rw-r--r--   0        0        0      346 2024-04-06 17:06:12.667793 sdss_hal-1.1.5/src/hal/etc/scripts/lco/cartchange.inp
+-rw-r--r--   0        0        0     1056 2024-04-06 17:06:12.667793 sdss_hal-1.1.5/src/hal/etc/scripts/lco/eveningcals.inp
+-rw-r--r--   0        0        0     1450 2024-04-06 17:06:12.667793 sdss_hal-1.1.5/src/hal/etc/scripts/lco/morningcals.inp
+-rw-r--r--   0        0        0     1180 2024-04-06 17:06:12.667793 sdss_hal-1.1.5/src/hal/exceptions.py
+-rw-r--r--   0        0        0     2373 2024-04-06 17:06:12.667793 sdss_hal-1.1.5/src/hal/helpers/__init__.py
+-rw-r--r--   0        0        0    10224 2024-04-06 17:06:12.667793 sdss_hal-1.1.5/src/hal/helpers/apogee.py
+-rw-r--r--   0        0        0     6825 2024-04-06 17:06:12.667793 sdss_hal-1.1.5/src/hal/helpers/boss.py
+-rw-r--r--   0        0        0     5011 2024-04-06 17:06:12.667793 sdss_hal-1.1.5/src/hal/helpers/cherno.py
+-rw-r--r--   0        0        0     1769 2024-04-06 17:06:12.667793 sdss_hal-1.1.5/src/hal/helpers/ffs.py
+-rw-r--r--   0        0        0     6710 2024-04-06 17:06:12.667793 sdss_hal-1.1.5/src/hal/helpers/jaeger.py
+-rw-r--r--   0        0        0    10429 2024-04-06 17:06:12.667793 sdss_hal-1.1.5/src/hal/helpers/lamps.py
+-rw-r--r--   0        0        0     4732 2024-04-06 17:06:12.667793 sdss_hal-1.1.5/src/hal/helpers/overhead.py
+-rw-r--r--   0        0        0     4671 2024-04-06 17:06:12.667793 sdss_hal-1.1.5/src/hal/helpers/scripts.py
+-rw-r--r--   0        0        0    13441 2024-04-06 17:06:12.667793 sdss_hal-1.1.5/src/hal/helpers/tcc.py
+-rw-r--r--   0        0        0     1385 2024-04-06 17:06:12.667793 sdss_hal-1.1.5/src/hal/macros/__init__.py
+-rw-r--r--   0        0        0     3844 2024-04-06 17:06:12.667793 sdss_hal-1.1.5/src/hal/macros/apogee_dome_flat.py
+-rw-r--r--   0        0        0     7601 2024-04-06 17:06:12.667793 sdss_hal-1.1.5/src/hal/macros/auto.py
+-rw-r--r--   0        0        0    21007 2024-04-06 17:06:12.667793 sdss_hal-1.1.5/src/hal/macros/expose.py
+-rw-r--r--   0        0        0    23236 2024-04-06 17:06:12.667793 sdss_hal-1.1.5/src/hal/macros/goto_field.py
+-rw-r--r--   0        0        0    18518 2024-04-06 17:06:12.667793 sdss_hal-1.1.5/src/hal/macros/macro.py
+-rw-r--r--   0        0        0     1263 2024-04-06 17:06:12.667793 sdss_hal-1.1.5/src/hal/macros/test_macro.py
+-rw-r--r--   0        0        0     2168 1970-01-01 00:00:00.000000 sdss_hal-1.1.5/PKG-INFO
```

### Comparing `sdss_hal-1.1.4/LICENSE.md` & `sdss_hal-1.1.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.1.4/README.md` & `sdss_hal-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.1.4/pyproject.toml` & `sdss_hal-1.1.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sdss-hal"
-version = "1.1.4"
+version = "1.1.5"
 description = "High-level observing tool for SDSS-V (replaces SOP)"
 authors = ["José Sánchez-Gallego <gallegoj@uw.edu>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 homepage = "https://github.com/sdss/hal"
 repository = "https://github.com/sdss/hal"
 documentation = "https://sdss-hal.readthedocs.org"
```

### Comparing `sdss_hal-1.1.4/src/hal/__main__.py` & `sdss_hal-1.1.5/src/hal/__main__.py`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.1.4/src/hal/actor/actor.py` & `sdss_hal-1.1.5/src/hal/actor/actor.py`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.1.4/src/hal/actor/commands/__init__.py` & `sdss_hal-1.1.5/src/hal/actor/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.1.4/src/hal/actor/commands/auto.py` & `sdss_hal-1.1.5/src/hal/actor/commands/auto.py`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.1.4/src/hal/actor/commands/bypass.py` & `sdss_hal-1.1.5/src/hal/actor/commands/bypass.py`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.1.4/src/hal/actor/commands/calibrations.py` & `sdss_hal-1.1.5/src/hal/actor/commands/calibrations.py`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.1.4/src/hal/actor/commands/expose.py` & `sdss_hal-1.1.5/src/hal/actor/commands/expose.py`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.1.4/src/hal/actor/commands/goto.py` & `sdss_hal-1.1.5/src/hal/actor/commands/goto.py`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.1.4/src/hal/actor/commands/goto_field.py` & `sdss_hal-1.1.5/src/hal/actor/commands/goto_field.py`

 * *Files 1% similar despite different names*

```diff
@@ -122,14 +122,16 @@
             stages = auto_mode_stages["rm_field_stages"][observatory]
         else:
             stages = auto_mode_stages["new_field_stages"][observatory]
 
     if stages is not None and len(stages) == 0:
         return command.finish("No stages to run.")
 
+    stages = stages[:]  # Prevent modifying the original list.
+
     if with_hartmann and stages is not None and "boss_hartmann" not in stages:
         # Can be added at the end. Macro.reset() will order it.
         stages.append("boss_hartmann")
 
     macro.reset(
         command,
         stages,
```

### Comparing `sdss_hal-1.1.4/src/hal/actor/commands/script.py` & `sdss_hal-1.1.5/src/hal/actor/commands/script.py`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.1.4/src/hal/actor/commands/status.py` & `sdss_hal-1.1.5/src/hal/actor/commands/status.py`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.1.4/src/hal/actor/commands/test.py` & `sdss_hal-1.1.5/src/hal/actor/commands/test.py`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.1.4/src/hal/etc/hal.yml` & `sdss_hal-1.1.5/src/hal/etc/hal.yml`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.1.4/src/hal/etc/schema.json` & `sdss_hal-1.1.5/src/hal/etc/schema.json`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.1.4/src/hal/etc/scripts/apo/eveningcals.inp` & `sdss_hal-1.1.5/src/hal/etc/scripts/apo/eveningcals.inp`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.1.4/src/hal/etc/scripts/apo/morningcals.inp` & `sdss_hal-1.1.5/src/hal/etc/scripts/apo/morningcals.inp`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.1.4/src/hal/etc/scripts/lco/eveningcals.inp` & `sdss_hal-1.1.5/src/hal/etc/scripts/lco/eveningcals.inp`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.1.4/src/hal/etc/scripts/lco/morningcals.inp` & `sdss_hal-1.1.5/src/hal/etc/scripts/lco/morningcals.inp`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.1.4/src/hal/exceptions.py` & `sdss_hal-1.1.5/src/hal/exceptions.py`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.1.4/src/hal/helpers/__init__.py` & `sdss_hal-1.1.5/src/hal/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.1.4/src/hal/helpers/apogee.py` & `sdss_hal-1.1.5/src/hal/helpers/apogee.py`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.1.4/src/hal/helpers/boss.py` & `sdss_hal-1.1.5/src/hal/helpers/boss.py`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.1.4/src/hal/helpers/cherno.py` & `sdss_hal-1.1.5/src/hal/helpers/cherno.py`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.1.4/src/hal/helpers/ffs.py` & `sdss_hal-1.1.5/src/hal/helpers/ffs.py`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.1.4/src/hal/helpers/jaeger.py` & `sdss_hal-1.1.5/src/hal/helpers/jaeger.py`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.1.4/src/hal/helpers/lamps.py` & `sdss_hal-1.1.5/src/hal/helpers/lamps.py`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.1.4/src/hal/helpers/overhead.py` & `sdss_hal-1.1.5/src/hal/helpers/overhead.py`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.1.4/src/hal/helpers/scripts.py` & `sdss_hal-1.1.5/src/hal/helpers/scripts.py`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.1.4/src/hal/helpers/tcc.py` & `sdss_hal-1.1.5/src/hal/helpers/tcc.py`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.1.4/src/hal/macros/__init__.py` & `sdss_hal-1.1.5/src/hal/macros/__init__.py`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.1.4/src/hal/macros/apogee_dome_flat.py` & `sdss_hal-1.1.5/src/hal/macros/apogee_dome_flat.py`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.1.4/src/hal/macros/auto.py` & `sdss_hal-1.1.5/src/hal/macros/auto.py`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.1.4/src/hal/macros/expose.py` & `sdss_hal-1.1.5/src/hal/macros/expose.py`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.1.4/src/hal/macros/goto_field.py` & `sdss_hal-1.1.5/src/hal/macros/goto_field.py`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.1.4/src/hal/macros/macro.py` & `sdss_hal-1.1.5/src/hal/macros/macro.py`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.1.4/src/hal/macros/test_macro.py` & `sdss_hal-1.1.5/src/hal/macros/test_macro.py`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.1.4/PKG-INFO` & `sdss_hal-1.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdss-hal
-Version: 1.1.4
+Version: 1.1.5
 Summary: High-level observing tool for SDSS-V (replaces SOP)
 Home-page: https://github.com/sdss/hal
 License: BSD-3-Clause
 Keywords: astronomy,software
 Author: José Sánchez-Gallego
 Author-email: gallegoj@uw.edu
 Requires-Python: >=3.10,<4.0
```

