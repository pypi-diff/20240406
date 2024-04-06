# Comparing `tmp/iog-randomizer-4.7.2.1.tar.gz` & `tmp/iog-randomizer-4.7.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "../../dist/randomizer/iog-randomizer-4.7.2.1.tar", last modified: Fri Apr  5 22:58:57 2024, max compression
+gzip compressed data, was "iog-randomizer-4.7.2.2.tar", last modified: Sat Apr  6 18:59:47 2024, max compression
```

## Comparing `iog-randomizer-4.7.2.1.tar` & `iog-randomizer-4.7.2.2.tar`

### file list

```diff
@@ -1,53 +1,54 @@
-drwxrwxrwx   0        0        0        0 2024-04-05 22:58:57.790593 iog-randomizer-4.7.2.1/
--rw-rw-rw-   0        0        0      244 2024-04-05 22:58:57.789595 iog-randomizer-4.7.2.1/PKG-INFO
--rw-rw-rw-   0        0        0    16459 2024-04-05 22:44:04.000000 iog-randomizer-4.7.2.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-05 22:58:57.685503 iog-randomizer-4.7.2.1/iog_randomizer.egg-info/
--rw-rw-rw-   0        0        0      244 2024-04-05 22:58:57.000000 iog-randomizer-4.7.2.1/iog_randomizer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1377 2024-04-05 22:58:57.000000 iog-randomizer-4.7.2.1/iog_randomizer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 22:58:57.000000 iog-randomizer-4.7.2.1/iog_randomizer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-04-05 22:58:57.000000 iog-randomizer-4.7.2.1/iog_randomizer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-05 22:58:57.000000 iog-randomizer-4.7.2.1/iog_randomizer.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-05 22:58:57.778591 iog-randomizer-4.7.2.1/randomizer/
--rw-rw-rw-   0        0        0      834 2024-04-05 22:44:04.000000 iog-randomizer-4.7.2.1/randomizer/ATlMpMuSEWaterHighSub_Tilemap1_comp.bin
--rw-rw-rw-   0        0        0      511 2024-04-05 22:44:04.000000 iog-randomizer-4.7.2.1/randomizer/ATlMpMuSWWaterHighSub_Tilemap1_comp.bin
--rw-rw-rw-   0        0        0     2341 2024-04-05 22:44:04.000000 iog-randomizer-4.7.2.1/randomizer/ATlMpSpecInvBg_comp.bin
--rw-rw-rw-   0        0        0     4437 2024-04-05 22:44:04.000000 iog-randomizer-4.7.2.1/randomizer/ConfigValueArray.asr
--rw-rw-rw-   0        0        0     1257 2024-04-05 22:44:04.000000 iog-randomizer-4.7.2.1/randomizer/Tilemap6D.bin
--rw-rw-rw-   0        0        0      486 2024-04-05 22:44:04.000000 iog-randomizer-4.7.2.1/randomizer/TilemapMuPassage.bin
--rw-rw-rw-   0        0        0       25 2024-04-05 22:44:04.000000 iog-randomizer-4.7.2.1/randomizer/__init__.py
--rw-rw-rw-   0        0        0    72688 2024-04-05 22:44:04.000000 iog-randomizer-4.7.2.1/randomizer/apocalypse_gaia_1.asr
--rw-rw-rw-   0        0        0    20962 2024-04-05 22:44:04.000000 iog-randomizer-4.7.2.1/randomizer/apocalypse_gaia_2.asr
--rw-rw-rw-   0        0        0   489472 2024-04-05 22:44:04.000000 iog-randomizer-4.7.2.1/randomizer/asar-x64.dll
--rw-rw-rw-   0        0        0   330280 2024-04-05 22:44:04.000000 iog-randomizer-4.7.2.1/randomizer/asar-x64.so
--rw-rw-rw-   0        0        0   344576 2024-04-05 22:44:04.000000 iog-randomizer-4.7.2.1/randomizer/asar-x86.dll
--rw-rw-rw-   0        0        0    14569 2024-04-05 22:44:04.000000 iog-randomizer-4.7.2.1/randomizer/asar.py
-drwxrwxrwx   0        0        0        0 2024-04-05 22:58:57.779585 iog-randomizer-4.7.2.1/randomizer/bin/
--rw-rw-rw-   0        0        0        0 2024-04-05 22:44:04.000000 iog-randomizer-4.7.2.1/randomizer/bin/__init__.py
--rw-rw-rw-   0        0        0   422504 2024-04-05 22:44:04.000000 iog-randomizer-4.7.2.1/randomizer/classes.py
--rw-rw-rw-   0        0        0      191 2024-04-05 22:44:04.000000 iog-randomizer-4.7.2.1/randomizer/errors.py
--rw-rw-rw-   0        0        0   247876 2024-04-05 22:44:04.000000 iog-randomizer-4.7.2.1/randomizer/iogr.asr
--rw-rw-rw-   0        0        0    38030 2024-04-05 22:44:04.000000 iog-randomizer-4.7.2.1/randomizer/iogr_81_exit_table.asr
--rw-rw-rw-   0        0        0   218181 2024-04-05 22:44:04.000000 iog-randomizer-4.7.2.1/randomizer/iogr_8C_actor_table.asr
--rw-rw-rw-   0        0        0    71930 2024-04-05 22:44:04.000000 iog-randomizer-4.7.2.1/randomizer/iogr_8D_asset_table.asr
--rw-rw-rw-   0        0        0    12873 2024-04-05 22:44:04.000000 iog-randomizer-4.7.2.1/randomizer/iogr_asset_ledger.asr
--rw-rw-rw-   0        0        0    75385 2024-04-05 22:44:04.000000 iog-randomizer-4.7.2.1/randomizer/iogr_code_overflow.asr
--rw-rw-rw-   0        0        0    29315 2024-04-05 22:44:04.000000 iog-randomizer-4.7.2.1/randomizer/iogr_dialogue_overflow.asr
--rw-rw-rw-   0        0        0    52543 2024-04-05 22:44:04.000000 iog-randomizer-4.7.2.1/randomizer/iogr_exit_ledger.asr
--rw-rw-rw-   0        0        0      112 2024-04-05 22:44:04.000000 iog-randomizer-4.7.2.1/randomizer/iogr_fluteless_melody_anim.bin
--rw-rw-rw-   0        0        0    12140 2024-04-05 22:44:04.000000 iog-randomizer-4.7.2.1/randomizer/iogr_misc_defines.asr
--rw-rw-rw-   0        0        0   436119 2024-04-05 22:44:04.000000 iog-randomizer-4.7.2.1/randomizer/iogr_monster_defaults.asr
--rw-rw-rw-   0        0        0    57365 2024-04-05 22:57:21.000000 iog-randomizer-4.7.2.1/randomizer/iogr_rom.py
-drwxrwxrwx   0        0        0        0 2024-04-05 22:58:57.783374 iog-randomizer-4.7.2.1/randomizer/models/
--rw-rw-rw-   0        0        0        0 2024-04-05 22:44:04.000000 iog-randomizer-4.7.2.1/randomizer/models/__init__.py
--rw-rw-rw-   0        0        0     1452 2024-04-05 22:44:04.000000 iog-randomizer-4.7.2.1/randomizer/models/enums.py
--rw-rw-rw-   0        0        0     3164 2024-04-05 22:44:04.000000 iog-randomizer-4.7.2.1/randomizer/models/randomizer_data.py
--rw-rw-rw-   0        0        0      818 2024-04-05 22:44:04.000000 iog-randomizer-4.7.2.1/randomizer/patch.py
--rw-rw-rw-   0        0        0     4190 2024-04-05 22:44:04.000000 iog-randomizer-4.7.2.1/randomizer/quintet_comp.py
--rw-rw-rw-   0        0        0    18409 2024-04-05 22:44:04.000000 iog-randomizer-4.7.2.1/randomizer/quintet_text.py
--rw-rw-rw-   0        0        0      544 2024-04-05 22:44:04.000000 iog-randomizer-4.7.2.1/randomizer/table_dialogue.txt
--rw-rw-rw-   0        0        0      520 2024-04-05 22:44:04.000000 iog-randomizer-4.7.2.1/randomizer/table_invtext.txt
-drwxrwxrwx   0        0        0        0 2024-04-05 22:58:57.788595 iog-randomizer-4.7.2.1/randomizer/tests/
--rw-rw-rw-   0        0        0        0 2024-04-05 22:44:04.000000 iog-randomizer-4.7.2.1/randomizer/tests/__init__.py
--rw-rw-rw-   0        0        0      407 2024-04-05 22:44:04.000000 iog-randomizer-4.7.2.1/randomizer/tests/test_generate_filename.py
--rw-rw-rw-   0        0        0       42 2024-04-05 22:58:57.790593 iog-randomizer-4.7.2.1/setup.cfg
--rw-rw-rw-   0        0        0      553 2024-04-05 22:57:38.000000 iog-randomizer-4.7.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-06 18:59:47.115169 iog-randomizer-4.7.2.2/
+-rw-rw-rw-   0        0        0     1233 2020-01-25 15:57:27.000000 iog-randomizer-4.7.2.2/LICENSE
+-rw-rw-rw-   0        0        0      235 2024-04-06 18:59:47.114168 iog-randomizer-4.7.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0    16459 2020-01-25 15:57:27.000000 iog-randomizer-4.7.2.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-06 18:59:47.113168 iog-randomizer-4.7.2.2/iog_randomizer.egg-info/
+-rw-rw-rw-   0        0        0      235 2024-04-06 18:59:47.000000 iog-randomizer-4.7.2.2/iog_randomizer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1385 2024-04-06 18:59:47.000000 iog-randomizer-4.7.2.2/iog_randomizer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-06 18:59:47.000000 iog-randomizer-4.7.2.2/iog_randomizer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-04-06 18:59:47.000000 iog-randomizer-4.7.2.2/iog_randomizer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-06 18:59:47.000000 iog-randomizer-4.7.2.2/iog_randomizer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-06 18:59:47.109170 iog-randomizer-4.7.2.2/randomizer/
+-rw-rw-rw-   0        0        0      834 2024-04-06 18:53:32.000000 iog-randomizer-4.7.2.2/randomizer/ATlMpMuSEWaterHighSub_Tilemap1_comp.bin
+-rw-rw-rw-   0        0        0      511 2024-04-06 18:53:32.000000 iog-randomizer-4.7.2.2/randomizer/ATlMpMuSWWaterHighSub_Tilemap1_comp.bin
+-rw-rw-rw-   0        0        0     2341 2024-04-06 18:53:32.000000 iog-randomizer-4.7.2.2/randomizer/ATlMpSpecInvBg_comp.bin
+-rw-rw-rw-   0        0        0     4437 2024-04-06 18:53:32.000000 iog-randomizer-4.7.2.2/randomizer/ConfigValueArray.asr
+-rw-rw-rw-   0        0        0     1257 2024-04-06 18:53:32.000000 iog-randomizer-4.7.2.2/randomizer/Tilemap6D.bin
+-rw-rw-rw-   0        0        0      486 2024-04-06 18:53:32.000000 iog-randomizer-4.7.2.2/randomizer/TilemapMuPassage.bin
+-rw-rw-rw-   0        0        0       25 2020-01-25 15:57:27.000000 iog-randomizer-4.7.2.2/randomizer/__init__.py
+-rw-rw-rw-   0        0        0    72688 2024-04-06 18:53:32.000000 iog-randomizer-4.7.2.2/randomizer/apocalypse_gaia_1.asr
+-rw-rw-rw-   0        0        0    20962 2024-04-06 18:53:32.000000 iog-randomizer-4.7.2.2/randomizer/apocalypse_gaia_2.asr
+-rw-rw-rw-   0        0        0   489472 2024-04-06 18:53:32.000000 iog-randomizer-4.7.2.2/randomizer/asar-x64.dll
+-rw-rw-rw-   0        0        0   330280 2024-04-06 18:53:32.000000 iog-randomizer-4.7.2.2/randomizer/asar-x64.so
+-rw-rw-rw-   0        0        0   344576 2024-04-06 18:53:32.000000 iog-randomizer-4.7.2.2/randomizer/asar-x86.dll
+-rw-rw-rw-   0        0        0    14569 2024-04-06 18:53:32.000000 iog-randomizer-4.7.2.2/randomizer/asar.py
+drwxrwxrwx   0        0        0        0 2024-04-06 18:59:47.109170 iog-randomizer-4.7.2.2/randomizer/bin/
+-rw-rw-rw-   0        0        0        0 2020-01-25 15:57:27.000000 iog-randomizer-4.7.2.2/randomizer/bin/__init__.py
+-rw-rw-rw-   0        0        0   422504 2024-04-06 18:53:32.000000 iog-randomizer-4.7.2.2/randomizer/classes.py
+-rw-rw-rw-   0        0        0      191 2020-01-25 15:57:27.000000 iog-randomizer-4.7.2.2/randomizer/errors.py
+-rw-rw-rw-   0        0        0   247876 2024-04-06 18:53:32.000000 iog-randomizer-4.7.2.2/randomizer/iogr.asr
+-rw-rw-rw-   0        0        0    38030 2024-04-06 18:53:32.000000 iog-randomizer-4.7.2.2/randomizer/iogr_81_exit_table.asr
+-rw-rw-rw-   0        0        0   218181 2024-04-06 18:53:32.000000 iog-randomizer-4.7.2.2/randomizer/iogr_8C_actor_table.asr
+-rw-rw-rw-   0        0        0    71930 2024-04-06 18:53:32.000000 iog-randomizer-4.7.2.2/randomizer/iogr_8D_asset_table.asr
+-rw-rw-rw-   0        0        0    12872 2024-04-06 18:55:39.000000 iog-randomizer-4.7.2.2/randomizer/iogr_asset_ledger.asr
+-rw-rw-rw-   0        0        0    75385 2024-04-06 18:53:32.000000 iog-randomizer-4.7.2.2/randomizer/iogr_code_overflow.asr
+-rw-rw-rw-   0        0        0    29315 2024-04-06 18:53:32.000000 iog-randomizer-4.7.2.2/randomizer/iogr_dialogue_overflow.asr
+-rw-rw-rw-   0        0        0    52543 2024-04-06 18:53:32.000000 iog-randomizer-4.7.2.2/randomizer/iogr_exit_ledger.asr
+-rw-rw-rw-   0        0        0      112 2024-04-06 18:53:32.000000 iog-randomizer-4.7.2.2/randomizer/iogr_fluteless_melody_anim.bin
+-rw-rw-rw-   0        0        0    12140 2024-04-06 18:53:32.000000 iog-randomizer-4.7.2.2/randomizer/iogr_misc_defines.asr
+-rw-rw-rw-   0        0        0   436119 2024-04-06 18:53:32.000000 iog-randomizer-4.7.2.2/randomizer/iogr_monster_defaults.asr
+-rw-rw-rw-   0        0        0    57365 2024-04-06 18:58:48.000000 iog-randomizer-4.7.2.2/randomizer/iogr_rom.py
+drwxrwxrwx   0        0        0        0 2024-04-06 18:59:47.111168 iog-randomizer-4.7.2.2/randomizer/models/
+-rw-rw-rw-   0        0        0        0 2020-01-25 15:57:27.000000 iog-randomizer-4.7.2.2/randomizer/models/__init__.py
+-rw-rw-rw-   0        0        0     1452 2024-04-06 18:53:32.000000 iog-randomizer-4.7.2.2/randomizer/models/enums.py
+-rw-rw-rw-   0        0        0     3164 2024-04-06 18:53:32.000000 iog-randomizer-4.7.2.2/randomizer/models/randomizer_data.py
+-rw-rw-rw-   0        0        0      818 2023-02-24 03:45:40.000000 iog-randomizer-4.7.2.2/randomizer/patch.py
+-rw-rw-rw-   0        0        0     4190 2020-01-25 15:57:27.000000 iog-randomizer-4.7.2.2/randomizer/quintet_comp.py
+-rw-rw-rw-   0        0        0    18409 2020-01-25 15:57:27.000000 iog-randomizer-4.7.2.2/randomizer/quintet_text.py
+-rw-rw-rw-   0        0        0      544 2024-04-06 18:53:32.000000 iog-randomizer-4.7.2.2/randomizer/table_dialogue.txt
+-rw-rw-rw-   0        0        0      520 2024-04-06 18:53:32.000000 iog-randomizer-4.7.2.2/randomizer/table_invtext.txt
+drwxrwxrwx   0        0        0        0 2024-04-06 18:59:47.112168 iog-randomizer-4.7.2.2/randomizer/tests/
+-rw-rw-rw-   0        0        0        0 2020-01-25 15:57:27.000000 iog-randomizer-4.7.2.2/randomizer/tests/__init__.py
+-rw-rw-rw-   0        0        0      407 2020-01-25 15:57:27.000000 iog-randomizer-4.7.2.2/randomizer/tests/test_generate_filename.py
+-rw-rw-rw-   0        0        0       42 2024-04-06 18:59:47.115169 iog-randomizer-4.7.2.2/setup.cfg
+-rw-rw-rw-   0        0        0      553 2024-04-06 18:59:06.000000 iog-randomizer-4.7.2.2/setup.py
```

### Comparing `iog-randomizer-4.7.2.1/README.md` & `iog-randomizer-4.7.2.2/README.md`

 * *Files identical despite different names*

### Comparing `iog-randomizer-4.7.2.1/iog_randomizer.egg-info/SOURCES.txt` & `iog-randomizer-4.7.2.2/iog_randomizer.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 setup.py
 iog_randomizer.egg-info/PKG-INFO
 iog_randomizer.egg-info/SOURCES.txt
 iog_randomizer.egg-info/dependency_links.txt
 iog_randomizer.egg-info/requires.txt
 iog_randomizer.egg-info/top_level.txt
```

### Comparing `iog-randomizer-4.7.2.1/randomizer/ATlMpMuSEWaterHighSub_Tilemap1_comp.bin` & `iog-randomizer-4.7.2.2/randomizer/ATlMpMuSEWaterHighSub_Tilemap1_comp.bin`

 * *Files identical despite different names*

### Comparing `iog-randomizer-4.7.2.1/randomizer/ATlMpSpecInvBg_comp.bin` & `iog-randomizer-4.7.2.2/randomizer/ATlMpSpecInvBg_comp.bin`

 * *Files identical despite different names*

### Comparing `iog-randomizer-4.7.2.1/randomizer/ConfigValueArray.asr` & `iog-randomizer-4.7.2.2/randomizer/ConfigValueArray.asr`

 * *Files identical despite different names*

### Comparing `iog-randomizer-4.7.2.1/randomizer/Tilemap6D.bin` & `iog-randomizer-4.7.2.2/randomizer/Tilemap6D.bin`

 * *Files identical despite different names*

### Comparing `iog-randomizer-4.7.2.1/randomizer/apocalypse_gaia_1.asr` & `iog-randomizer-4.7.2.2/randomizer/apocalypse_gaia_1.asr`

 * *Files identical despite different names*

### Comparing `iog-randomizer-4.7.2.1/randomizer/apocalypse_gaia_2.asr` & `iog-randomizer-4.7.2.2/randomizer/apocalypse_gaia_2.asr`

 * *Files identical despite different names*

### Comparing `iog-randomizer-4.7.2.1/randomizer/asar-x64.dll` & `iog-randomizer-4.7.2.2/randomizer/asar-x64.dll`

 * *Files identical despite different names*

### Comparing `iog-randomizer-4.7.2.1/randomizer/asar-x64.so` & `iog-randomizer-4.7.2.2/randomizer/asar-x64.so`

 * *Files identical despite different names*

### Comparing `iog-randomizer-4.7.2.1/randomizer/asar-x86.dll` & `iog-randomizer-4.7.2.2/randomizer/asar-x86.dll`

 * *Files identical despite different names*

### Comparing `iog-randomizer-4.7.2.1/randomizer/asar.py` & `iog-randomizer-4.7.2.2/randomizer/asar.py`

 * *Files identical despite different names*

### Comparing `iog-randomizer-4.7.2.1/randomizer/classes.py` & `iog-randomizer-4.7.2.2/randomizer/classes.py`

 * *Files identical despite different names*

### Comparing `iog-randomizer-4.7.2.1/randomizer/iogr.asr` & `iog-randomizer-4.7.2.2/randomizer/iogr.asr`

 * *Files identical despite different names*

### Comparing `iog-randomizer-4.7.2.1/randomizer/iogr_81_exit_table.asr` & `iog-randomizer-4.7.2.2/randomizer/iogr_81_exit_table.asr`

 * *Files identical despite different names*

### Comparing `iog-randomizer-4.7.2.1/randomizer/iogr_8C_actor_table.asr` & `iog-randomizer-4.7.2.2/randomizer/iogr_8C_actor_table.asr`

 * *Files identical despite different names*

### Comparing `iog-randomizer-4.7.2.1/randomizer/iogr_8D_asset_table.asr` & `iog-randomizer-4.7.2.2/randomizer/iogr_8D_asset_table.asr`

 * *Files identical despite different names*

### Comparing `iog-randomizer-4.7.2.1/randomizer/iogr_asset_ledger.asr` & `iog-randomizer-4.7.2.2/randomizer/iogr_asset_ledger.asr`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 !CardMusicCreditsB = $11,$13,$00,$93,$17,$D2
 !CardMusicCreditsA = $11,$14,$00,$66,$D2,$99
 !CardMusicRaft = $11,$15,$00,$8D,$5C,$DC
 !CardMusicDarkSpace = $11,$16,$00,$53,$35,$D6
 !CardMusicCityVariant = $11,$1C,$00,$9C,$F3,$95
 !CardMusicSilence = $11,$1b,$00,$1d,$2a,$df
 
-if !SettingDungeonShuffle == 2    ; Dungeon Chaos QOL to prevent chaotic music shifts.
+if !SettingDungeonShuffle > 0    ; Dungeon Chaos QOL to prevent chaotic music shifts.
 !CardMusicInca = !CardMusicMinorDungeon
 !CardMusicSkGn = !CardMusicMinorDungeon
 !CardMusicMu = !CardMusicMinorDungeon
 !CardMusicGtWl = !CardMusicMinorDungeon
 !CardMusicAnkr = !CardMusicMinorDungeon
 !CardMusicPymd = !CardMusicMinorDungeon
 endif
```

### Comparing `iog-randomizer-4.7.2.1/randomizer/iogr_code_overflow.asr` & `iog-randomizer-4.7.2.2/randomizer/iogr_code_overflow.asr`

 * *Files identical despite different names*

### Comparing `iog-randomizer-4.7.2.1/randomizer/iogr_dialogue_overflow.asr` & `iog-randomizer-4.7.2.2/randomizer/iogr_dialogue_overflow.asr`

 * *Files identical despite different names*

### Comparing `iog-randomizer-4.7.2.1/randomizer/iogr_exit_ledger.asr` & `iog-randomizer-4.7.2.2/randomizer/iogr_exit_ledger.asr`

 * *Files identical despite different names*

### Comparing `iog-randomizer-4.7.2.1/randomizer/iogr_misc_defines.asr` & `iog-randomizer-4.7.2.2/randomizer/iogr_misc_defines.asr`

 * *Files identical despite different names*

### Comparing `iog-randomizer-4.7.2.1/randomizer/iogr_monster_defaults.asr` & `iog-randomizer-4.7.2.2/randomizer/iogr_monster_defaults.asr`

 * *Files identical despite different names*

### Comparing `iog-randomizer-4.7.2.1/randomizer/iogr_rom.py` & `iog-randomizer-4.7.2.2/randomizer/iogr_rom.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #from .models.enums.enemizer import Enemizer
 #from .models.enums.flute import FluteOpt
 #from .models.enums.start_location import StartLocation
 from .models.enums import *
 
 from . import asar
 
-VERSION = "4.7.2.1"
+VERSION = "4.7.2.2"
 MAX_RANDO_RETRIES = 50
 OUTPUT_FOLDER: str = os.path.dirname(os.path.realpath(__file__)) + os.path.sep + ".." + os.path.sep + ".." + os.path.sep + "data" + os.path.sep + "output" + os.path.sep
 
 
 def generate_filename(settings: RandomizerData, extension: str):
     def getDifficulty(difficulty):
         if difficulty.value == Difficulty.EASY.value:
```

### Comparing `iog-randomizer-4.7.2.1/randomizer/models/enums.py` & `iog-randomizer-4.7.2.2/randomizer/models/enums.py`

 * *Files identical despite different names*

### Comparing `iog-randomizer-4.7.2.1/randomizer/models/randomizer_data.py` & `iog-randomizer-4.7.2.2/randomizer/models/randomizer_data.py`

 * *Files identical despite different names*

### Comparing `iog-randomizer-4.7.2.1/randomizer/patch.py` & `iog-randomizer-4.7.2.2/randomizer/patch.py`

 * *Files identical despite different names*

### Comparing `iog-randomizer-4.7.2.1/randomizer/quintet_comp.py` & `iog-randomizer-4.7.2.2/randomizer/quintet_comp.py`

 * *Files identical despite different names*

### Comparing `iog-randomizer-4.7.2.1/randomizer/quintet_text.py` & `iog-randomizer-4.7.2.2/randomizer/quintet_text.py`

 * *Files identical despite different names*

### Comparing `iog-randomizer-4.7.2.1/randomizer/table_dialogue.txt` & `iog-randomizer-4.7.2.2/randomizer/table_dialogue.txt`

 * *Files identical despite different names*

### Comparing `iog-randomizer-4.7.2.1/randomizer/table_invtext.txt` & `iog-randomizer-4.7.2.2/randomizer/table_invtext.txt`

 * *Files identical despite different names*

### Comparing `iog-randomizer-4.7.2.1/setup.py` & `iog-randomizer-4.7.2.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setuptools.setup(
     name='iog-randomizer',
-    version='4.7.2.1',
+    version='4.7.2.2',
     description='The Illusion of Gaia Randomizer',
     author='dontbagume,bryon_w,raeven0',
     packages=setuptools.find_packages(),
     package_data={'': [
         '*.bin',
         '*.asr',
         '*.txt',
```

