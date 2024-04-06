# Comparing `tmp/starrailcard-2.1.0.tar.gz` & `tmp/starrailcard-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starrailcard-2.1.0.tar", max compression
+gzip compressed data, was "starrailcard-2.1.1.tar", max compression
```

## Comparing `starrailcard-2.1.0.tar` & `starrailcard-2.1.1.tar`

### file list

```diff
@@ -1,48 +1,48 @@
--rw-r--r--   0        0        0     1721 2024-03-20 15:38:40.776791 starrailcard-2.1.0/LICENSE
--rw-r--r--   0        0        0     1147 2024-04-02 12:01:24.476671 starrailcard-2.1.0/pyproject.toml
--rw-r--r--   0        0        0     3642 2024-03-18 20:36:48.857949 starrailcard-2.1.0/README.md
--rw-r--r--   0        0        0       75 2024-03-15 20:07:42.107466 starrailcard-2.1.0/starrailcard/__init__.py
--rw-r--r--   0        0        0     9736 2024-04-02 12:01:15.004451 starrailcard-2.1.0/starrailcard/client.py
--rw-r--r--   0        0        0      106 2024-03-20 15:35:34.777763 starrailcard-2.1.0/starrailcard/requirements.txt
--rw-r--r--   0        0        0      969 2024-03-28 17:11:10.264563 starrailcard-2.1.0/starrailcard/src/api/api.py
--rw-r--r--   0        0        0   201292 2023-10-12 08:13:59.547042 starrailcard-2.1.0/starrailcard/src/assets/font/font_hsr.ttf
--rw-r--r--   0        0        0     1751 2024-03-28 18:26:38.347683 starrailcard-2.1.0/starrailcard/src/data/avatar.json
--rw-r--r--   0        0        0      252 2024-03-28 18:26:38.460098 starrailcard-2.1.0/starrailcard/src/data/element.json
--rw-r--r--   0        0        0       70 2024-03-28 18:26:38.462097 starrailcard-2.1.0/starrailcard/src/data/keys.json
--rw-r--r--   0        0        0      293 2024-03-28 18:26:38.423267 starrailcard-2.1.0/starrailcard/src/data/paths.json
--rw-r--r--   0        0        0     1915 2024-03-28 18:26:38.386139 starrailcard-2.1.0/starrailcard/src/data/relict_sets.json
--rw-r--r--   0        0        0     4947 2024-03-28 18:26:38.266305 starrailcard-2.1.0/starrailcard/src/data/stats.json
--rw-r--r--   0        0        0     4738 2024-03-28 18:26:38.308097 starrailcard-2.1.0/starrailcard/src/data/weapons.json
--rw-r--r--   0        0        0     6680 2024-03-16 23:04:12.294325 starrailcard-2.1.0/starrailcard/src/generator/style_profile_phone.py
--rw-r--r--   0        0        0    23968 2024-03-24 23:40:49.094126 starrailcard-2.1.0/starrailcard/src/generator/style_relict_score.py
--rw-r--r--   0        0        0    29840 2024-03-28 18:58:01.974256 starrailcard-2.1.0/starrailcard/src/generator/style_ticket.py
--rw-r--r--   0        0        0     8410 2024-03-13 13:47:49.948737 starrailcard-2.1.0/starrailcard/src/model/api_mihomo.py
--rw-r--r--   0        0        0     4757 2024-03-27 19:18:51.084890 starrailcard-2.1.0/starrailcard/src/model/StarRailCard.py
--rw-r--r--   0        0        0     4065 2024-03-13 13:47:58.864230 starrailcard-2.1.0/starrailcard/src/model/style.py
--rw-r--r--   0        0        0      493 2024-03-13 13:48:02.345029 starrailcard-2.1.0/starrailcard/src/model/ukrainization_model.py
--rw-r--r--   0        0        0      845 2024-03-13 13:48:07.469416 starrailcard-2.1.0/starrailcard/src/model/utils_model.py
--rw-r--r--   0        0        0      373 2024-03-28 19:05:12.724879 starrailcard-2.1.0/starrailcard/src/tools/calculator/src/assets/max.json
--rw-r--r--   0        0        0       49 2024-03-28 19:05:13.041062 starrailcard-2.1.0/starrailcard/src/tools/calculator/src/assets/relic_id.json
--rw-r--r--   0        0        0     3434 2024-03-28 19:05:13.341867 starrailcard-2.1.0/starrailcard/src/tools/calculator/src/assets/rolls.json
--rw-r--r--   0        0        0    87319 2024-03-28 19:05:13.882857 starrailcard-2.1.0/starrailcard/src/tools/calculator/src/assets/score.json
--rw-r--r--   0        0        0     1959 2024-03-13 13:47:21.923389 starrailcard-2.1.0/starrailcard/src/tools/calculator/src/utils.py
--rw-r--r--   0        0        0     5747 2024-04-01 14:16:17.689304 starrailcard-2.1.0/starrailcard/src/tools/calculator/stats.py
--rw-r--r--   0        0        0     2526 2024-02-22 12:56:12.220916 starrailcard-2.1.0/starrailcard/src/tools/cashe.py
--rw-r--r--   0        0        0      563 2024-03-28 16:30:39.886551 starrailcard-2.1.0/starrailcard/src/tools/enums.py
--rw-r--r--   0        0        0    10136 2024-02-23 21:20:24.125982 starrailcard-2.1.0/starrailcard/src/tools/git.py
--rw-r--r--   0        0        0     6100 2024-03-28 17:26:04.740937 starrailcard-2.1.0/starrailcard/src/tools/http.py
--rw-r--r--   0        0        0      940 2024-03-28 18:26:46.684860 starrailcard-2.1.0/starrailcard/src/tools/json_data.py
--rw-r--r--   0        0        0     6122 2024-02-25 12:22:45.869423 starrailcard-2.1.0/starrailcard/src/tools/options.py
--rw-r--r--   0        0        0      199 2024-02-18 13:46:16.566296 starrailcard-2.1.0/starrailcard/src/tools/pill/__init__.py
--rw-r--r--   0        0        0     3854 2024-02-22 12:55:07.451038 starrailcard-2.1.0/starrailcard/src/tools/pill/color.py
--rw-r--r--   0        0        0     2330 2024-02-22 13:03:49.291296 starrailcard-2.1.0/starrailcard/src/tools/pill/color_controle.py
--rw-r--r--   0        0        0     5518 2024-02-25 12:31:53.901150 starrailcard-2.1.0/starrailcard/src/tools/pill/grandiend_v2.py
--rw-r--r--   0        0        0     3284 2024-02-22 12:55:28.873148 starrailcard-2.1.0/starrailcard/src/tools/pill/grandient_v1.py
--rw-r--r--   0        0        0     3833 2024-03-17 12:15:47.665776 starrailcard-2.1.0/starrailcard/src/tools/pill/image_controle.py
--rw-r--r--   0        0        0     5106 2024-02-22 12:55:59.845148 starrailcard-2.1.0/starrailcard/src/tools/pill/style_editor.py
--rw-r--r--   0        0        0     2116 2024-02-22 13:01:14.697378 starrailcard-2.1.0/starrailcard/src/tools/pill/text_controle.py
--rw-r--r--   0        0        0     2360 2024-03-13 13:31:40.291343 starrailcard-2.1.0/starrailcard/src/tools/translator.py
--rw-r--r--   0        0        0     6585 2024-02-22 12:57:06.983609 starrailcard-2.1.0/starrailcard/src/tools/treePaths.py
--rw-r--r--   0        0        0     1748 2024-03-28 18:26:54.868269 starrailcard-2.1.0/starrailcard/src/tools/ukrainization.py
--rw-r--r--   0        0        0     6884 2024-03-18 20:19:11.991157 starrailcard-2.1.0/starrailcard/utils.py
--rw-r--r--   0        0        0     4999 1970-01-01 00:00:00.000000 starrailcard-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1721 2024-03-20 15:38:40.776791 starrailcard-2.1.1/LICENSE
+-rw-r--r--   0        0        0     1147 2024-04-06 18:58:14.199853 starrailcard-2.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3642 2024-03-18 20:36:48.857949 starrailcard-2.1.1/README.md
+-rw-r--r--   0        0        0       75 2024-03-15 20:07:42.107466 starrailcard-2.1.1/starrailcard/__init__.py
+-rw-r--r--   0        0        0     9736 2024-04-02 12:01:15.004451 starrailcard-2.1.1/starrailcard/client.py
+-rw-r--r--   0        0        0      106 2024-03-20 15:35:34.777763 starrailcard-2.1.1/starrailcard/requirements.txt
+-rw-r--r--   0        0        0     1049 2024-04-06 18:57:38.219761 starrailcard-2.1.1/starrailcard/src/api/api.py
+-rw-r--r--   0        0        0   201292 2023-10-12 08:13:59.547042 starrailcard-2.1.1/starrailcard/src/assets/font/font_hsr.ttf
+-rw-r--r--   0        0        0     1751 2024-03-28 18:26:38.347683 starrailcard-2.1.1/starrailcard/src/data/avatar.json
+-rw-r--r--   0        0        0      252 2024-03-28 18:26:38.460098 starrailcard-2.1.1/starrailcard/src/data/element.json
+-rw-r--r--   0        0        0       70 2024-03-28 18:26:38.462097 starrailcard-2.1.1/starrailcard/src/data/keys.json
+-rw-r--r--   0        0        0      293 2024-03-28 18:26:38.423267 starrailcard-2.1.1/starrailcard/src/data/paths.json
+-rw-r--r--   0        0        0     1915 2024-03-28 18:26:38.386139 starrailcard-2.1.1/starrailcard/src/data/relict_sets.json
+-rw-r--r--   0        0        0     4947 2024-03-28 18:26:38.266305 starrailcard-2.1.1/starrailcard/src/data/stats.json
+-rw-r--r--   0        0        0     4738 2024-03-28 18:26:38.308097 starrailcard-2.1.1/starrailcard/src/data/weapons.json
+-rw-r--r--   0        0        0     6696 2024-04-06 18:31:53.629800 starrailcard-2.1.1/starrailcard/src/generator/style_profile_phone.py
+-rw-r--r--   0        0        0    23968 2024-03-24 23:40:49.094126 starrailcard-2.1.1/starrailcard/src/generator/style_relict_score.py
+-rw-r--r--   0        0        0    29840 2024-03-28 18:58:01.974256 starrailcard-2.1.1/starrailcard/src/generator/style_ticket.py
+-rw-r--r--   0        0        0     8410 2024-03-13 13:47:49.948737 starrailcard-2.1.1/starrailcard/src/model/api_mihomo.py
+-rw-r--r--   0        0        0     4757 2024-03-27 19:18:51.084890 starrailcard-2.1.1/starrailcard/src/model/StarRailCard.py
+-rw-r--r--   0        0        0     4065 2024-03-13 13:47:58.864230 starrailcard-2.1.1/starrailcard/src/model/style.py
+-rw-r--r--   0        0        0      493 2024-03-13 13:48:02.345029 starrailcard-2.1.1/starrailcard/src/model/ukrainization_model.py
+-rw-r--r--   0        0        0      845 2024-03-13 13:48:07.469416 starrailcard-2.1.1/starrailcard/src/model/utils_model.py
+-rw-r--r--   0        0        0      373 2024-04-06 18:51:59.632223 starrailcard-2.1.1/starrailcard/src/tools/calculator/src/assets/max.json
+-rw-r--r--   0        0        0       49 2024-04-06 18:52:00.222443 starrailcard-2.1.1/starrailcard/src/tools/calculator/src/assets/relic_id.json
+-rw-r--r--   0        0        0     3434 2024-04-06 18:52:00.479448 starrailcard-2.1.1/starrailcard/src/tools/calculator/src/assets/rolls.json
+-rw-r--r--   0        0        0    92881 2024-04-06 18:52:01.246844 starrailcard-2.1.1/starrailcard/src/tools/calculator/src/assets/score.json
+-rw-r--r--   0        0        0     1959 2024-03-13 13:47:21.923389 starrailcard-2.1.1/starrailcard/src/tools/calculator/src/utils.py
+-rw-r--r--   0        0        0     5747 2024-04-01 14:16:17.689304 starrailcard-2.1.1/starrailcard/src/tools/calculator/stats.py
+-rw-r--r--   0        0        0     2526 2024-02-22 12:56:12.220916 starrailcard-2.1.1/starrailcard/src/tools/cashe.py
+-rw-r--r--   0        0        0      563 2024-03-28 16:30:39.886551 starrailcard-2.1.1/starrailcard/src/tools/enums.py
+-rw-r--r--   0        0        0    10136 2024-02-23 21:20:24.125982 starrailcard-2.1.1/starrailcard/src/tools/git.py
+-rw-r--r--   0        0        0     6100 2024-03-28 17:26:04.740937 starrailcard-2.1.1/starrailcard/src/tools/http.py
+-rw-r--r--   0        0        0      940 2024-03-28 18:26:46.684860 starrailcard-2.1.1/starrailcard/src/tools/json_data.py
+-rw-r--r--   0        0        0     6345 2024-04-06 18:55:54.476858 starrailcard-2.1.1/starrailcard/src/tools/options.py
+-rw-r--r--   0        0        0      199 2024-02-18 13:46:16.566296 starrailcard-2.1.1/starrailcard/src/tools/pill/__init__.py
+-rw-r--r--   0        0        0     3854 2024-02-22 12:55:07.451038 starrailcard-2.1.1/starrailcard/src/tools/pill/color.py
+-rw-r--r--   0        0        0     2330 2024-02-22 13:03:49.291296 starrailcard-2.1.1/starrailcard/src/tools/pill/color_controle.py
+-rw-r--r--   0        0        0     5518 2024-02-25 12:31:53.901150 starrailcard-2.1.1/starrailcard/src/tools/pill/grandiend_v2.py
+-rw-r--r--   0        0        0     3284 2024-02-22 12:55:28.873148 starrailcard-2.1.1/starrailcard/src/tools/pill/grandient_v1.py
+-rw-r--r--   0        0        0     3833 2024-04-06 18:31:03.220838 starrailcard-2.1.1/starrailcard/src/tools/pill/image_controle.py
+-rw-r--r--   0        0        0     5106 2024-02-22 12:55:59.845148 starrailcard-2.1.1/starrailcard/src/tools/pill/style_editor.py
+-rw-r--r--   0        0        0     2116 2024-02-22 13:01:14.697378 starrailcard-2.1.1/starrailcard/src/tools/pill/text_controle.py
+-rw-r--r--   0        0        0     2360 2024-03-13 13:31:40.291343 starrailcard-2.1.1/starrailcard/src/tools/translator.py
+-rw-r--r--   0        0        0     6585 2024-02-22 12:57:06.983609 starrailcard-2.1.1/starrailcard/src/tools/treePaths.py
+-rw-r--r--   0        0        0     1748 2024-03-28 18:26:54.868269 starrailcard-2.1.1/starrailcard/src/tools/ukrainization.py
+-rw-r--r--   0        0        0     6884 2024-03-18 20:19:11.991157 starrailcard-2.1.1/starrailcard/utils.py
+-rw-r--r--   0        0        0     4999 1970-01-01 00:00:00.000000 starrailcard-2.1.1/PKG-INFO
```

### Comparing `starrailcard-2.1.0/LICENSE` & `starrailcard-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.0/pyproject.toml` & `starrailcard-2.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "starrailcard"
-version = "2.1.0"
+version = "2.1.1"
 description = "This Python module provides the ability to create captivating character cards based on player data from Honkai Star Rail, obtained through their unique user identifiers (UIDs). StarRailCard streamlines the process of generating personalized character assembly cards, relying on the information provided by players."
 authors = ["DEViantUA <deviantapi@gmail.com>"]
 license = "MIT License with Additional Restrictions"
 
 readme = 'README.md'  # Markdown files are supported
 
 repository = "https://github.com/DEViantUA/StarRailCard"
```

### Comparing `starrailcard-2.1.0/README.md` & `starrailcard-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.0/starrailcard/client.py` & `starrailcard-2.1.1/starrailcard/client.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.0/starrailcard/src/api/api.py` & `starrailcard-2.1.1/starrailcard/src/api/api.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,12 +14,15 @@
         self.uid = uid
         api_mihomo.UA_LANG = False
         if lang == "ua":
             api_mihomo.UA_LANG = True
         self.lang = translator.SUPPORTED_LANGUAGES.get(lang, "en")
     
     async def get(self):
-        data = await http.AioSession.get(_API_MIHOMO.format(uid = self.uid, lang = self.lang, force_update = self.force_update))
+        try:
+            data = await http.AioSession.get(_API_MIHOMO.format(uid = self.uid, lang = self.lang, force_update = self.force_update))
+        except:
+            raise TypeError("Error in UID")
         if api_mihomo.UA_LANG:
             await ukrainization.TranslateDataManager().load_translate_data()
             
         return api_mihomo.MiHoMoApi(**data)
```

### Comparing `starrailcard-2.1.0/starrailcard/src/assets/font/font_hsr.ttf` & `starrailcard-2.1.1/starrailcard/src/assets/font/font_hsr.ttf`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.0/starrailcard/src/data/avatar.json` & `starrailcard-2.1.1/starrailcard/src/data/avatar.json`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.0/starrailcard/src/data/relict_sets.json` & `starrailcard-2.1.1/starrailcard/src/data/relict_sets.json`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.0/starrailcard/src/data/stats.json` & `starrailcard-2.1.1/starrailcard/src/data/stats.json`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.0/starrailcard/src/data/weapons.json` & `starrailcard-2.1.1/starrailcard/src/data/weapons.json`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.0/starrailcard/src/generator/style_profile_phone.py` & `starrailcard-2.1.1/starrailcard/src/generator/style_profile_phone.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,30 +61,30 @@
         charter_profile.alpha_composite(name,(136,int(49-name.size[1]/2)))       
 
         max_level = options.max_lvl(key.promotion)
         level = f"{self.lang.lvl}: {key.level}/{max_level}"
         
         element_icon = await pill.get_dowload_img(key.element.icon, size=(28,28))
         path_icon = await pill.get_dowload_img(key.path.icon, size=(28,28))
-        starts = await options.get_stars(key.light_cone.rarity)
         
         charter_profile.alpha_composite(path_icon,(263,28))
         charter_profile.alpha_composite(element_icon,(293,28))
-        charter_profile.alpha_composite(starts.resize((85,18)),(224,114))
+        
         
         
         d = ImageDraw.Draw(charter_profile)
         d.text((19,7), level, font= self.font_charter, fill=(255,255,255,255))
         
         
         if not key.light_cone is None:
             icon = await pill.get_dowload_img(key.light_cone.icon, size = (66,66))
             charter_profile.alpha_composite(icon,(136,70))
             d.text((201,95), f"{self.lang.lvl}: {key.light_cone.level}/{options.max_lvl(key.light_cone.promotion)}", font=self.font_charter, fill=(255, 255, 255, 255))
-
+            starts = await options.get_stars(key.light_cone.rarity)
+            charter_profile.alpha_composite(starts.resize((85,18)),(224,114))
             
             background = await _of.light_cone_ups
             background = background.copy()
             
             d = ImageDraw.Draw(background)
             font_12 = await pill.get_font(12)
             up = options.ups(key.light_cone.rank)
```

### Comparing `starrailcard-2.1.0/starrailcard/src/generator/style_relict_score.py` & `starrailcard-2.1.1/starrailcard/src/generator/style_relict_score.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.0/starrailcard/src/generator/style_ticket.py` & `starrailcard-2.1.1/starrailcard/src/generator/style_ticket.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.0/starrailcard/src/model/api_mihomo.py` & `starrailcard-2.1.1/starrailcard/src/model/api_mihomo.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.0/starrailcard/src/model/StarRailCard.py` & `starrailcard-2.1.1/starrailcard/src/model/StarRailCard.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.0/starrailcard/src/model/style.py` & `starrailcard-2.1.1/starrailcard/src/model/style.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.0/starrailcard/src/model/utils_model.py` & `starrailcard-2.1.1/starrailcard/src/model/utils_model.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.0/starrailcard/src/tools/calculator/src/assets/rolls.json` & `starrailcard-2.1.1/starrailcard/src/tools/calculator/src/assets/rolls.json`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.0/starrailcard/src/tools/calculator/src/assets/score.json` & `starrailcard-2.1.1/starrailcard/src/tools/calculator/src/assets/score.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9334503968253968%*

 * *Differences: {"'1107'": "{'main': {'4': {'SpeedDelta': 0}}, 'weight': {'SpeedDelta': 0}}",*

 * * "'1203'": "{'main': {'3': {'AttackAddedRatio': 1}, '4': {'AttackAddedRatio': 1}, '5': "*

 * *           "{'AttackAddedRatio': 1}, '6': {'AttackAddedRatio': 1}}, 'weight': {'AttackDelta': 0.5, "*

 * *           "'AttackAddedRatio': 1}}",*

 * * "'1301'": "OrderedDict([('main', OrderedDict([('1', OrderedDict([('HPDelta', 1)])), ('2', "*

 * *           "OrderedDict([('AttackDelta', 1)])), ('3', OrderedDict([('HPAddedRatio', 0.4), "*

 * *           "('AttackA […]*

```diff
@@ -901,15 +901,15 @@
                 "HealRatioBase": 0,
                 "StatusProbabilityBase": 0
             },
             "4": {
                 "AttackAddedRatio": 1,
                 "DefenceAddedRatio": 0,
                 "HPAddedRatio": 0,
-                "SpeedDelta": 0.8
+                "SpeedDelta": 0
             },
             "5": {
                 "AttackAddedRatio": 0.8,
                 "DefenceAddedRatio": 0,
                 "FireAddedRatio": 0,
                 "HPAddedRatio": 0,
                 "IceAddedRatio": 0,
@@ -934,15 +934,15 @@
             "BreakDamageAddedRatioBase": 0,
             "CriticalChanceBase": 1,
             "CriticalDamageBase": 1,
             "DefenceAddedRatio": 0,
             "DefenceDelta": 0,
             "HPAddedRatio": 0,
             "HPDelta": 0,
-            "SpeedDelta": 0.8,
+            "SpeedDelta": 0,
             "StatusProbabilityBase": 0,
             "StatusResistanceBase": 0
         }
     },
     "1108": {
         "main": {
             "1": {
@@ -1361,52 +1361,52 @@
             "1": {
                 "HPDelta": 1
             },
             "2": {
                 "AttackDelta": 1
             },
             "3": {
-                "AttackAddedRatio": 0,
+                "AttackAddedRatio": 1,
                 "CriticalChanceBase": 0,
                 "CriticalDamageBase": 0,
                 "DefenceAddedRatio": 0,
                 "HPAddedRatio": 0.8,
                 "HealRatioBase": 1,
                 "StatusProbabilityBase": 0
             },
             "4": {
-                "AttackAddedRatio": 0,
+                "AttackAddedRatio": 1,
                 "DefenceAddedRatio": 0,
                 "HPAddedRatio": 1,
                 "SpeedDelta": 1
             },
             "5": {
-                "AttackAddedRatio": 0,
+                "AttackAddedRatio": 1,
                 "DefenceAddedRatio": 0.5,
                 "FireAddedRatio": 0,
                 "HPAddedRatio": 1,
                 "IceAddedRatio": 0,
                 "ImaginaryAddedRatio": 0,
                 "PhysicalAddedRatio": 0,
                 "QuantumAddedRatio": 0,
                 "ThunderAddedRatio": 0,
                 "WindAddedRatio": 0
             },
             "6": {
-                "AttackAddedRatio": 0,
+                "AttackAddedRatio": 1,
                 "BreakDamageAddedRatioBase": 0,
                 "DefenceAddedRatio": 0,
                 "HPAddedRatio": 1,
                 "SPRatioBase": 0.5
             }
         },
         "max": 8.46,
         "weight": {
-            "AttackAddedRatio": 0,
-            "AttackDelta": 0,
+            "AttackAddedRatio": 1,
+            "AttackDelta": 0.5,
             "BreakDamageAddedRatioBase": 0,
             "CriticalChanceBase": 0,
             "CriticalDamageBase": 0,
             "DefenceAddedRatio": 0.5,
             "DefenceDelta": 0.2,
             "HPAddedRatio": 1,
             "HPDelta": 0.5,
@@ -2178,14 +2178,73 @@
             "HPAddedRatio": 1,
             "HPDelta": 0.5,
             "SpeedDelta": 1,
             "StatusProbabilityBase": 0,
             "StatusResistanceBase": 0.5
         }
     },
+    "1301": {
+        "main": {
+            "1": {
+                "HPDelta": 1
+            },
+            "2": {
+                "AttackDelta": 1
+            },
+            "3": {
+                "AttackAddedRatio": 0,
+                "CriticalChanceBase": 0,
+                "CriticalDamageBase": 0,
+                "DefenceAddedRatio": 0.4,
+                "HPAddedRatio": 0.4,
+                "HealRatioBase": 1,
+                "StatusProbabilityBase": 0
+            },
+            "4": {
+                "AttackAddedRatio": 0,
+                "DefenceAddedRatio": 0.4,
+                "HPAddedRatio": 0.4,
+                "SpeedDelta": 1
+            },
+            "5": {
+                "AttackAddedRatio": 0,
+                "DefenceAddedRatio": 1,
+                "FireAddedRatio": 0,
+                "HPAddedRatio": 1,
+                "IceAddedRatio": 0,
+                "ImaginaryAddedRatio": 0,
+                "PhysicalAddedRatio": 0,
+                "QuantumAddedRatio": 0,
+                "ThunderAddedRatio": 0,
+                "WindAddedRatio": 0
+            },
+            "6": {
+                "AttackAddedRatio": 0,
+                "BreakDamageAddedRatioBase": 1,
+                "DefenceAddedRatio": 0.4,
+                "HPAddedRatio": 0.4,
+                "SPRatioBase": 1
+            }
+        },
+        "max": 10.18,
+        "weight": {
+            "AttackAddedRatio": 0.8,
+            "AttackDelta": 0,
+            "BreakDamageAddedRatioBase": 1,
+            "CriticalChanceBase": 0,
+            "CriticalDamageBase": 0,
+            "DefenceAddedRatio": 0.4,
+            "DefenceDelta": 0.1,
+            "HPAddedRatio": 0.4,
+            "HPDelta": 0.1,
+            "SpeedDelta": 0.8,
+            "StatusProbabilityBase": 0,
+            "StatusResistanceBase": 0.6
+        }
+    },
     "1302": {
         "main": {
             "1": {
                 "HPDelta": 1
             },
             "2": {
                 "AttackDelta": 1
@@ -2296,25 +2355,84 @@
             "HPAddedRatio": 0.8,
             "HPDelta": 0.3,
             "SpeedDelta": 1,
             "StatusProbabilityBase": 0,
             "StatusResistanceBase": 0.5
         }
     },
+    "1304": {
+        "main": {
+            "1": {
+                "HPDelta": 1
+            },
+            "2": {
+                "AttackDelta": 1
+            },
+            "3": {
+                "AttackAddedRatio": 0,
+                "CriticalChanceBase": 0,
+                "CriticalDamageBase": 0,
+                "DefenceAddedRatio": 1,
+                "HPAddedRatio": 1,
+                "HealRatioBase": 0,
+                "StatusProbabilityBase": 0
+            },
+            "4": {
+                "AttackAddedRatio": 0,
+                "DefenceAddedRatio": 0.8,
+                "HPAddedRatio": 0.8,
+                "SpeedDelta": 1
+            },
+            "5": {
+                "AttackAddedRatio": 0,
+                "DefenceAddedRatio": 1,
+                "FireAddedRatio": 0,
+                "HPAddedRatio": 1,
+                "IceAddedRatio": 0,
+                "ImaginaryAddedRatio": 0,
+                "PhysicalAddedRatio": 0,
+                "QuantumAddedRatio": 0,
+                "ThunderAddedRatio": 0,
+                "WindAddedRatio": 0
+            },
+            "6": {
+                "AttackAddedRatio": 0,
+                "BreakDamageAddedRatioBase": 1,
+                "DefenceAddedRatio": 0.8,
+                "HPAddedRatio": 0.8,
+                "SPRatioBase": 1
+            }
+        },
+        "max": 10.0,
+        "weight": {
+            "AttackAddedRatio": 0,
+            "AttackDelta": 0,
+            "BreakDamageAddedRatioBase": 1,
+            "CriticalChanceBase": 0,
+            "CriticalDamageBase": 0,
+            "DefenceAddedRatio": 0.8,
+            "DefenceDelta": 0.3,
+            "HPAddedRatio": 0.8,
+            "HPDelta": 0.3,
+            "SpeedDelta": 1,
+            "StatusProbabilityBase": 0,
+            "StatusResistanceBase": 0.5
+        }
+    },
     "1305": {
         "main": {
             "1": {
                 "HPDelta": 1
             },
             "2": {
                 "AttackDelta": 1
             },
             "3": {
                 "AttackAddedRatio": 0.8,
-                "CriticalChanceBase": 0,
+                "CriticalChanceBase": 1,
                 "CriticalDamageBase": 1,
                 "DefenceAddedRatio": 0,
                 "HPAddedRatio": 0,
                 "HealRatioBase": 0,
                 "StatusProbabilityBase": 0
             },
             "4": {
@@ -2341,24 +2459,24 @@
                 "DefenceAddedRatio": 0,
                 "HPAddedRatio": 0,
                 "SPRatioBase": 0
             }
         },
         "max": 0.0,
         "weight": {
-            "AttackAddedRatio": 0,
-            "AttackDelta": 0,
+            "AttackAddedRatio": 0.6,
+            "AttackDelta": 0.1,
             "BreakDamageAddedRatioBase": 0,
-            "CriticalChanceBase": 0,
-            "CriticalDamageBase": 0,
+            "CriticalChanceBase": 1,
+            "CriticalDamageBase": 1,
             "DefenceAddedRatio": 0,
             "DefenceDelta": 0,
             "HPAddedRatio": 0,
             "HPDelta": 0,
-            "SpeedDelta": 0,
+            "SpeedDelta": 0.8,
             "StatusProbabilityBase": 0,
             "StatusResistanceBase": 0
         }
     },
     "1306": {
         "main": {
             "1": {
@@ -2367,59 +2485,59 @@
             "2": {
                 "AttackDelta": 1
             },
             "3": {
                 "AttackAddedRatio": 0,
                 "CriticalChanceBase": 0,
                 "CriticalDamageBase": 1,
-                "DefenceAddedRatio": 0.5,
-                "HPAddedRatio": 0.8,
+                "DefenceAddedRatio": 0.8,
+                "HPAddedRatio": 0,
                 "HealRatioBase": 0,
                 "StatusProbabilityBase": 0
             },
             "4": {
                 "AttackAddedRatio": 0,
-                "DefenceAddedRatio": 0,
-                "HPAddedRatio": 0.8,
+                "DefenceAddedRatio": 0.8,
+                "HPAddedRatio": 0,
                 "SpeedDelta": 1
             },
             "5": {
                 "AttackAddedRatio": 0,
-                "DefenceAddedRatio": 0.5,
+                "DefenceAddedRatio": 1,
                 "FireAddedRatio": 0,
                 "HPAddedRatio": 1,
                 "IceAddedRatio": 0,
-                "ImaginaryAddedRatio": 0,
+                "ImaginaryAddedRatio": 1,
                 "PhysicalAddedRatio": 0,
                 "QuantumAddedRatio": 0,
                 "ThunderAddedRatio": 0,
                 "WindAddedRatio": 0
             },
             "6": {
                 "AttackAddedRatio": 0,
                 "BreakDamageAddedRatioBase": 0,
-                "DefenceAddedRatio": 0.5,
-                "HPAddedRatio": 0.8,
+                "DefenceAddedRatio": 0,
+                "HPAddedRatio": 0,
                 "SPRatioBase": 1
             }
         },
-        "max": 10.06,
+        "max": 0.0,
         "weight": {
             "AttackAddedRatio": 0,
             "AttackDelta": 0,
             "BreakDamageAddedRatioBase": 0,
             "CriticalChanceBase": 0,
             "CriticalDamageBase": 1,
-            "DefenceAddedRatio": 0.5,
-            "DefenceDelta": 0.2,
-            "HPAddedRatio": 0.8,
-            "HPDelta": 0.3,
+            "DefenceAddedRatio": 0.8,
+            "DefenceDelta": 0.3,
+            "HPAddedRatio": 0,
+            "HPDelta": 0,
             "SpeedDelta": 1,
             "StatusProbabilityBase": 0,
-            "StatusResistanceBase": 0.8
+            "StatusResistanceBase": 0.6
         }
     },
     "1307": {
         "main": {
             "1": {
                 "HPDelta": 1
             },
@@ -2438,74 +2556,133 @@
             "4": {
                 "AttackAddedRatio": 1,
                 "DefenceAddedRatio": 0,
                 "HPAddedRatio": 0,
                 "SpeedDelta": 1
             },
             "5": {
-                "AttackAddedRatio": 0.8,
+                "AttackAddedRatio": 1,
                 "DefenceAddedRatio": 0,
                 "FireAddedRatio": 0,
                 "HPAddedRatio": 0,
                 "IceAddedRatio": 0,
-                "ImaginaryAddedRatio": 0,
+                "ImaginaryAddedRatio": 1,
                 "PhysicalAddedRatio": 0,
                 "QuantumAddedRatio": 0,
                 "ThunderAddedRatio": 0,
                 "WindAddedRatio": 1
             },
             "6": {
                 "AttackAddedRatio": 1,
                 "BreakDamageAddedRatioBase": 0,
                 "DefenceAddedRatio": 0,
                 "HPAddedRatio": 0,
-                "SPRatioBase": 1
+                "SPRatioBase": 0
             }
         },
-        "max": 9.84,
+        "max": 0.0,
         "weight": {
-            "AttackAddedRatio": 1,
-            "AttackDelta": 0.4,
+            "AttackAddedRatio": 0.8,
+            "AttackDelta": 0.3,
             "BreakDamageAddedRatioBase": 0,
-            "CriticalChanceBase": 0.4,
-            "CriticalDamageBase": 0.4,
+            "CriticalChanceBase": 0,
+            "CriticalDamageBase": 0,
             "DefenceAddedRatio": 0,
             "DefenceDelta": 0,
             "HPAddedRatio": 0,
             "HPDelta": 0,
-            "SpeedDelta": 1,
+            "SpeedDelta": 0.8,
             "StatusProbabilityBase": 1,
             "StatusResistanceBase": 0
         }
     },
-    "1312": {
+    "1308": {
         "main": {
             "1": {
                 "HPDelta": 1
             },
             "2": {
                 "AttackDelta": 1
             },
             "3": {
-                "AttackAddedRatio": 0.8,
+                "AttackAddedRatio": 0.7,
                 "CriticalChanceBase": 1,
                 "CriticalDamageBase": 1,
                 "DefenceAddedRatio": 0,
                 "HPAddedRatio": 0,
                 "HealRatioBase": 0,
                 "StatusProbabilityBase": 0
             },
             "4": {
                 "AttackAddedRatio": 1,
                 "DefenceAddedRatio": 0,
                 "HPAddedRatio": 0,
                 "SpeedDelta": 1
             },
             "5": {
+                "AttackAddedRatio": 1,
+                "DefenceAddedRatio": 0,
+                "FireAddedRatio": 0,
+                "HPAddedRatio": 0,
+                "IceAddedRatio": 0,
+                "ImaginaryAddedRatio": 0,
+                "PhysicalAddedRatio": 0,
+                "QuantumAddedRatio": 0,
+                "ThunderAddedRatio": 1,
+                "WindAddedRatio": 0
+            },
+            "6": {
+                "AttackAddedRatio": 1,
+                "BreakDamageAddedRatioBase": 0,
+                "DefenceAddedRatio": 0,
+                "HPAddedRatio": 0,
+                "SPRatioBase": 0
+            }
+        },
+        "max": 0.0,
+        "weight": {
+            "AttackAddedRatio": 0.7,
+            "AttackDelta": 0.3,
+            "BreakDamageAddedRatioBase": 0,
+            "CriticalChanceBase": 1,
+            "CriticalDamageBase": 0.9,
+            "DefenceAddedRatio": 0,
+            "DefenceDelta": 0,
+            "HPAddedRatio": 0,
+            "HPDelta": 0,
+            "SpeedDelta": 0.6,
+            "StatusProbabilityBase": 0,
+            "StatusResistanceBase": 0
+        }
+    },
+    "1312": {
+        "main": {
+            "1": {
+                "HPDelta": 1
+            },
+            "2": {
+                "AttackDelta": 1
+            },
+            "3": {
                 "AttackAddedRatio": 0.8,
+                "CriticalChanceBase": 1,
+                "CriticalDamageBase": 1,
+                "DefenceAddedRatio": 0,
+                "HPAddedRatio": 0,
+                "HealRatioBase": 0,
+                "StatusProbabilityBase": 0.6
+            },
+            "4": {
+                "AttackAddedRatio": 1,
+                "DefenceAddedRatio": 0,
+                "HPAddedRatio": 0,
+                "SpeedDelta": 1
+            },
+            "5": {
+                "AttackAddedRatio": 1,
                 "DefenceAddedRatio": 0,
                 "FireAddedRatio": 0,
                 "HPAddedRatio": 0,
                 "IceAddedRatio": 1,
                 "ImaginaryAddedRatio": 0,
                 "PhysicalAddedRatio": 0,
                 "QuantumAddedRatio": 0,
@@ -2513,30 +2690,30 @@
                 "WindAddedRatio": 0
             },
             "6": {
                 "AttackAddedRatio": 1,
                 "BreakDamageAddedRatioBase": 0,
                 "DefenceAddedRatio": 0,
                 "HPAddedRatio": 0,
-                "SPRatioBase": 1
+                "SPRatioBase": 0
             }
         },
-        "max": 10.16,
+        "max": 0.0,
         "weight": {
             "AttackAddedRatio": 0.8,
             "AttackDelta": 0.3,
             "BreakDamageAddedRatioBase": 0,
             "CriticalChanceBase": 1,
             "CriticalDamageBase": 1,
             "DefenceAddedRatio": 0,
             "DefenceDelta": 0,
             "HPAddedRatio": 0,
             "HPDelta": 0,
             "SpeedDelta": 0.8,
-            "StatusProbabilityBase": 0.5,
+            "StatusProbabilityBase": 0.6,
             "StatusResistanceBase": 0
         }
     },
     "8001": {
         "main": {
             "1": {
                 "HPDelta": 1
```

### Comparing `starrailcard-2.1.0/starrailcard/src/tools/calculator/src/utils.py` & `starrailcard-2.1.1/starrailcard/src/tools/calculator/src/utils.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.0/starrailcard/src/tools/calculator/stats.py` & `starrailcard-2.1.1/starrailcard/src/tools/calculator/stats.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.0/starrailcard/src/tools/cashe.py` & `starrailcard-2.1.1/starrailcard/src/tools/cashe.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.0/starrailcard/src/tools/enums.py` & `starrailcard-2.1.1/starrailcard/src/tools/enums.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.0/starrailcard/src/tools/git.py` & `starrailcard-2.1.1/starrailcard/src/tools/git.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.0/starrailcard/src/tools/http.py` & `starrailcard-2.1.1/starrailcard/src/tools/http.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.0/starrailcard/src/tools/json_data.py` & `starrailcard-2.1.1/starrailcard/src/tools/json_data.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.0/starrailcard/src/tools/options.py` & `starrailcard-2.1.1/starrailcard/src/tools/options.py`

 * *Files 4% similar despite different names*

```diff
@@ -198,15 +198,20 @@
         if key["k"] == str(charter_id):
             data = key.get("lb")
     
     if data != {} and data is not None:
         if type(data) == list:
             for key in data:
                 if "lb" in key:
-                    return key["lb"]["tutorial"]
+                    if "tutorial" in key["lb"]:
+                        return key["lb"]["tutorial"]
+                    else:
+                        '''for keys in key["lb"]:
+                            return key["lb"][keys]'''
+                        return None
         else:
             for key in data:
                 return data[key]
     else:
         return None
 
 async def save_card(uid, image_data, name):
```

### Comparing `starrailcard-2.1.0/starrailcard/src/tools/pill/color.py` & `starrailcard-2.1.1/starrailcard/src/tools/pill/color.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.0/starrailcard/src/tools/pill/color_controle.py` & `starrailcard-2.1.1/starrailcard/src/tools/pill/color_controle.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.0/starrailcard/src/tools/pill/grandiend_v2.py` & `starrailcard-2.1.1/starrailcard/src/tools/pill/grandiend_v2.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.0/starrailcard/src/tools/pill/grandient_v1.py` & `starrailcard-2.1.1/starrailcard/src/tools/pill/grandient_v1.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.0/starrailcard/src/tools/pill/image_controle.py` & `starrailcard-2.1.1/starrailcard/src/tools/pill/image_controle.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.0/starrailcard/src/tools/pill/style_editor.py` & `starrailcard-2.1.1/starrailcard/src/tools/pill/style_editor.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.0/starrailcard/src/tools/pill/text_controle.py` & `starrailcard-2.1.1/starrailcard/src/tools/pill/text_controle.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.0/starrailcard/src/tools/translator.py` & `starrailcard-2.1.1/starrailcard/src/tools/translator.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.0/starrailcard/src/tools/treePaths.py` & `starrailcard-2.1.1/starrailcard/src/tools/treePaths.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.0/starrailcard/src/tools/ukrainization.py` & `starrailcard-2.1.1/starrailcard/src/tools/ukrainization.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.0/starrailcard/utils.py` & `starrailcard-2.1.1/starrailcard/utils.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.0/PKG-INFO` & `starrailcard-2.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starrailcard
-Version: 2.1.0
+Version: 2.1.1
 Summary: This Python module provides the ability to create captivating character cards based on player data from Honkai Star Rail, obtained through their unique user identifiers (UIDs). StarRailCard streamlines the process of generating personalized character assembly cards, relying on the information provided by players.
 Home-page: https://github.com/DEViantUA/StarRailCard
 License: MIT License with Additional Restrictions
 Keywords: honkai,cards,generation,honkaistarraill,raill,starraill,builds,honkairail,honkai
 Author: DEViantUA
 Author-email: deviantapi@gmail.com
 Requires-Python: >=3.9,<4.0
```

