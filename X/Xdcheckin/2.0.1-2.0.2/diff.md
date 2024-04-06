# Comparing `tmp/Xdcheckin-2.0.1.tar.gz` & `tmp/Xdcheckin-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Xdcheckin-2.0.1.tar", last modified: Fri Apr  5 14:44:29 2024, max compression
+gzip compressed data, was "Xdcheckin-2.0.2.tar", last modified: Sat Apr  6 04:04:23 2024, max compression
```

## Comparing `Xdcheckin-2.0.1.tar` & `Xdcheckin-2.0.2.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:44:29.738143 Xdcheckin-2.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-05 14:44:22.000000 Xdcheckin-2.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-04-05 14:44:29.738143 Xdcheckin-2.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-04-05 14:44:22.000000 Xdcheckin-2.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     5830 2024-04-05 14:44:22.000000 Xdcheckin-2.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 14:44:29.738143 Xdcheckin-2.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:44:29.730143 Xdcheckin-2.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:44:29.734143 Xdcheckin-2.0.1/src/Xdcheckin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-04-05 14:44:29.000000 Xdcheckin-2.0.1/src/Xdcheckin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-05 14:44:29.000000 Xdcheckin-2.0.1/src/Xdcheckin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 14:44:29.000000 Xdcheckin-2.0.1/src/Xdcheckin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-05 14:44:29.000000 Xdcheckin-2.0.1/src/Xdcheckin.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-05 14:44:29.000000 Xdcheckin-2.0.1/src/Xdcheckin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-05 14:44:29.000000 Xdcheckin-2.0.1/src/Xdcheckin.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:44:29.730143 Xdcheckin-2.0.1/src/xdcheckin/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 14:44:22.000000 Xdcheckin-2.0.1/src/xdcheckin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-05 14:44:22.000000 Xdcheckin-2.0.1/src/xdcheckin/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:44:29.734143 Xdcheckin-2.0.1/src/xdcheckin/core/
--rw-r--r--   0 runner    (1001) docker     (127)        2 2024-04-05 14:44:22.000000 Xdcheckin-2.0.1/src/xdcheckin/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    33265 2024-04-05 14:44:22.000000 Xdcheckin-2.0.1/src/xdcheckin/core/chaoxing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3845 2024-04-05 14:44:22.000000 Xdcheckin-2.0.1/src/xdcheckin/core/locations.py
--rw-r--r--   0 runner    (1001) docker     (127)     8862 2024-04-05 14:44:22.000000 Xdcheckin-2.0.1/src/xdcheckin/core/xidian.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:44:29.734143 Xdcheckin-2.0.1/src/xdcheckin/server/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 14:44:22.000000 Xdcheckin-2.0.1/src/xdcheckin/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11811 2024-04-05 14:44:22.000000 Xdcheckin-2.0.1/src/xdcheckin/server/server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:44:29.734143 Xdcheckin-2.0.1/src/xdcheckin/server/static/
--rw-r--r--   0 runner    (1001) docker     (127)     5183 2024-04-05 14:44:22.000000 Xdcheckin-2.0.1/src/xdcheckin/server/static/activity.js
--rw-r--r--   0 runner    (1001) docker     (127)     2798 2024-04-05 14:44:22.000000 Xdcheckin-2.0.1/src/xdcheckin/server/static/classroom.js
--rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-04-05 14:44:22.000000 Xdcheckin-2.0.1/src/xdcheckin/server/static/curriculum.js
--rw-r--r--   0 runner    (1001) docker     (127)   249304 2024-04-05 14:44:22.000000 Xdcheckin-2.0.1/src/xdcheckin/server/static/g_classroom_urls.js
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-05 14:44:22.000000 Xdcheckin-2.0.1/src/xdcheckin/server/static/global.js
--rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-04-05 14:44:22.000000 Xdcheckin-2.0.1/src/xdcheckin/server/static/location.js
--rw-r--r--   0 runner    (1001) docker     (127)     5707 2024-04-05 14:44:22.000000 Xdcheckin-2.0.1/src/xdcheckin/server/static/login.js
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-04-05 14:44:22.000000 Xdcheckin-2.0.1/src/xdcheckin/server/static/misc.js
--rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-04-05 14:44:22.000000 Xdcheckin-2.0.1/src/xdcheckin/server/static/player.js
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-05 14:44:22.000000 Xdcheckin-2.0.1/src/xdcheckin/server/static/style.css
--rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-04-05 14:44:22.000000 Xdcheckin-2.0.1/src/xdcheckin/server/static/util.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:44:29.734143 Xdcheckin-2.0.1/src/xdcheckin/server/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     7943 2024-04-05 14:44:22.000000 Xdcheckin-2.0.1/src/xdcheckin/server/templates/index.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:44:29.734143 Xdcheckin-2.0.1/src/xdcheckin/util/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 14:44:22.000000 Xdcheckin-2.0.1/src/xdcheckin/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5469 2024-04-05 14:44:22.000000 Xdcheckin-2.0.1/src/xdcheckin/util/chaoxing_captcha.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 04:04:23.183033 Xdcheckin-2.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-06 04:04:16.000000 Xdcheckin-2.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-04-06 04:04:23.183033 Xdcheckin-2.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-04-06 04:04:16.000000 Xdcheckin-2.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5830 2024-04-06 04:04:16.000000 Xdcheckin-2.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 04:04:23.183033 Xdcheckin-2.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 04:04:23.175032 Xdcheckin-2.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 04:04:23.183033 Xdcheckin-2.0.2/src/Xdcheckin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-04-06 04:04:23.000000 Xdcheckin-2.0.2/src/Xdcheckin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-06 04:04:23.000000 Xdcheckin-2.0.2/src/Xdcheckin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 04:04:23.000000 Xdcheckin-2.0.2/src/Xdcheckin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-06 04:04:23.000000 Xdcheckin-2.0.2/src/Xdcheckin.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-06 04:04:23.000000 Xdcheckin-2.0.2/src/Xdcheckin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-06 04:04:23.000000 Xdcheckin-2.0.2/src/Xdcheckin.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 04:04:23.179033 Xdcheckin-2.0.2/src/xdcheckin/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 04:04:16.000000 Xdcheckin-2.0.2/src/xdcheckin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-06 04:04:16.000000 Xdcheckin-2.0.2/src/xdcheckin/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 04:04:23.179033 Xdcheckin-2.0.2/src/xdcheckin/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-04-06 04:04:16.000000 Xdcheckin-2.0.2/src/xdcheckin/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33316 2024-04-06 04:04:16.000000 Xdcheckin-2.0.2/src/xdcheckin/core/chaoxing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3845 2024-04-06 04:04:16.000000 Xdcheckin-2.0.2/src/xdcheckin/core/locations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9392 2024-04-06 04:04:16.000000 Xdcheckin-2.0.2/src/xdcheckin/core/xidian.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 04:04:23.179033 Xdcheckin-2.0.2/src/xdcheckin/server/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 04:04:16.000000 Xdcheckin-2.0.2/src/xdcheckin/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11811 2024-04-06 04:04:16.000000 Xdcheckin-2.0.2/src/xdcheckin/server/server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 04:04:23.183033 Xdcheckin-2.0.2/src/xdcheckin/server/static/
+-rw-r--r--   0 runner    (1001) docker     (127)     5183 2024-04-06 04:04:16.000000 Xdcheckin-2.0.2/src/xdcheckin/server/static/activity.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2798 2024-04-06 04:04:16.000000 Xdcheckin-2.0.2/src/xdcheckin/server/static/classroom.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-04-06 04:04:16.000000 Xdcheckin-2.0.2/src/xdcheckin/server/static/curriculum.js
+-rw-r--r--   0 runner    (1001) docker     (127)   249304 2024-04-06 04:04:16.000000 Xdcheckin-2.0.2/src/xdcheckin/server/static/g_classroom_urls.js
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-06 04:04:16.000000 Xdcheckin-2.0.2/src/xdcheckin/server/static/global.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-04-06 04:04:16.000000 Xdcheckin-2.0.2/src/xdcheckin/server/static/location.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5707 2024-04-06 04:04:16.000000 Xdcheckin-2.0.2/src/xdcheckin/server/static/login.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-04-06 04:04:16.000000 Xdcheckin-2.0.2/src/xdcheckin/server/static/misc.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-04-06 04:04:16.000000 Xdcheckin-2.0.2/src/xdcheckin/server/static/player.js
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-06 04:04:16.000000 Xdcheckin-2.0.2/src/xdcheckin/server/static/style.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-04-06 04:04:16.000000 Xdcheckin-2.0.2/src/xdcheckin/server/static/util.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 04:04:23.183033 Xdcheckin-2.0.2/src/xdcheckin/server/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     7943 2024-04-06 04:04:16.000000 Xdcheckin-2.0.2/src/xdcheckin/server/templates/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 04:04:23.183033 Xdcheckin-2.0.2/src/xdcheckin/util/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 04:04:16.000000 Xdcheckin-2.0.2/src/xdcheckin/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5469 2024-04-06 04:04:16.000000 Xdcheckin-2.0.2/src/xdcheckin/util/chaoxing_captcha.py
```

### Comparing `Xdcheckin-2.0.1/LICENSE` & `Xdcheckin-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `Xdcheckin-2.0.1/PKG-INFO` & `Xdcheckin-2.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Xdcheckin
-Version: 2.0.1
+Version: 2.0.2
 Summary: Chaoxing Checkin Tool for XDU.
 Author-email: Pairman <pairmanxlr@gmail.com>
 License: GNU General Public License v3 (GPLv3)
 Project-URL: Homepage, https://github.com/Pairman/Xdcheckin
 Project-URL: Changelog, https://github.com/Pairman/Xdcheckin/blob/main/CHANGELOG.md
 Keywords: xdu,xidian,chaoxing,livestream
 Classifier: Framework :: Flask
```

### Comparing `Xdcheckin-2.0.1/README.md` & `Xdcheckin-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `Xdcheckin-2.0.1/pyproject.toml` & `Xdcheckin-2.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 00000010: 7265 7175 6972 6573 203d 205b 2273 6574  requires = ["set
 00000020: 7570 746f 6f6c 7322 2c20 2277 6865 656c  uptools", "wheel
 00000030: 225d 0d0a 6275 696c 642d 6261 636b 656e  "]..build-backen
 00000040: 6420 3d20 2273 6574 7570 746f 6f6c 732e  d = "setuptools.
 00000050: 6275 696c 645f 6d65 7461 220d 0a0d 0a5b  build_meta"....[
 00000060: 7072 6f6a 6563 745d 0d0a 6e61 6d65 203d  project]..name =
 00000070: 2022 5864 6368 6563 6b69 6e22 0d0a 7665   "Xdcheckin"..ve
-00000080: 7273 696f 6e20 3d20 2232 2e30 2e31 220d  rsion = "2.0.1".
+00000080: 7273 696f 6e20 3d20 2232 2e30 2e32 220d  rsion = "2.0.2".
 00000090: 0a61 7574 686f 7273 203d 205b 0d0a 097b  .authors = [...{
 000000a0: 6e61 6d65 203d 2022 5061 6972 6d61 6e22  name = "Pairman"
 000000b0: 2c20 656d 6169 6c20 3d20 2270 6169 726d  , email = "pairm
 000000c0: 616e 786c 7240 676d 6169 6c2e 636f 6d22  anxlr@gmail.com"
 000000d0: 7d0d 0a5d 0d0a 7265 6164 6d65 203d 2022  }..]..readme = "
 000000e0: 5245 4144 4d45 2e6d 6422 0d0a 6465 7363  README.md"..desc
 000000f0: 7269 7074 696f 6e20 3d20 2243 6861 6f78  ription = "Chaox
```

### Comparing `Xdcheckin-2.0.1/src/Xdcheckin.egg-info/PKG-INFO` & `Xdcheckin-2.0.2/src/Xdcheckin.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Xdcheckin
-Version: 2.0.1
+Version: 2.0.2
 Summary: Chaoxing Checkin Tool for XDU.
 Author-email: Pairman <pairmanxlr@gmail.com>
 License: GNU General Public License v3 (GPLv3)
 Project-URL: Homepage, https://github.com/Pairman/Xdcheckin
 Project-URL: Changelog, https://github.com/Pairman/Xdcheckin/blob/main/CHANGELOG.md
 Keywords: xdu,xidian,chaoxing,livestream
 Classifier: Framework :: Flask
```

### Comparing `Xdcheckin-2.0.1/src/Xdcheckin.egg-info/SOURCES.txt` & `Xdcheckin-2.0.2/src/Xdcheckin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Xdcheckin-2.0.1/src/xdcheckin/core/chaoxing.py` & `Xdcheckin-2.0.2/src/xdcheckin/core/chaoxing.py`

 * *Files 1% similar despite different names*

```diff
@@ -846,40 +846,44 @@
 				"params": params
 			}
 		except Exception as e:
 			if type(e) is AssertionError:
 				match = search(r"validate_([0-9A-Fa-f]{32})", str(e))
 				if match:
 					params["enc2"] = match.group(1)
-				msg = f"Checkin failure. {dumps(activity), dumps(location), dumps(params), str(e)}"
+				msg = f"Checkin failure. {dumps(params), str(e)}"
 			else:
 				msg = str(e)
 			return False, {
 				"msg": msg,
 				"params": params
 			}
 
 	def checkin_checkin_location(
 		self, activity: dict = {"active_id": ""},
 		location: dict = {"latitude": -1, "longitude": -1, "address": ""}
 	):
 		"""Location checkin.
 		:param activity: Activity ID in dictionary.
 		:param location: Address, latitude and longitude in dictionary. Overriden by server-side location if any.
-		:return: Checkin state (True on success), success / error message and payload (placeholder).
+		:return: Checkin state (True on success), message, params and captcha (placeholder if already checked-in or on failure).
 		"""
 		try:
 			thread_analysis = Thread(target = self.checkin_do_analysis, kwargs = {"activity": activity})
 			thread_analysis.start()
 			info = self.checkin_get_details(activity = activity)
 			assert info["status"] == 1 and not info["isDelete"], "Activity ended or deleted."
 			presign = self.checkin_do_presign(activity = activity, course = {"class_id": str(info["clazzId"])})
-			assert presign[0], f"Presign failure. {dumps(activity), dumps(location), dumps(presign)}"
+			assert presign[0], f"Presign failure. {dumps(activity), dumps(presign)}"
 			if presign[0] == 2:
-				return True, "Checkin success. (Already checked in.)"
+				return True, {
+					"msg": "Checkin success. (Already checked in.)",
+					"params": "",
+					"captcha": ""
+				}
 			location_new = {
 				**(self.checkin_format_location(location = location, location_new = presign[1]) if presign[1]["ranged"] else location),
 				"ranged": presign[1]["ranged"]
 			}
 			thread_analysis.join()
 			result = self.checkin_do_sign(activity = {**activity, "type": "4"}, location = location_new)
 			result[1]["captcha"] = presign[2]
@@ -911,24 +915,27 @@
 			thread_analysis.start()
 			info = self.checkin_get_details(activity = activity)
 			assert info["status"] == 1 and not info["isDelete"], "Activity ended or deleted."
 			course, location_new = {"class_id": str(info["clazzId"])}, {}
 			thread_location = Thread(target = _get_location)
 			thread_location.start()
 			presign = self.checkin_do_presign(activity = activity, course = course)
-			assert presign[0], f"Presign failure. {dumps(activity), dumps(location), dumps(presign)}"
+			assert presign[0], f"Presign failure. {dumps(activity), dumps(presign)}"
 			if presign[0] == 2:
-				return True, "Checkin success. (Already checked in.)"
+				return True, {
+					"msg": "Checkin success. (Already checked in.)",
+					"params": "",
+					"captcha": ""
+				}
 			location_new = {
 				**(thread_location.join() or self.checkin_format_location(location = location, location_new = location_new) if presign[1]["ranged"] else location),
 				"ranged": presign[1]["ranged"]
 			}
 			thread_analysis.join()
 			result = self.checkin_do_sign(activity = {**activity, "type": "2"}, location = location_new)
-			print(result)
 			result[1]["captcha"] = presign[2]
 			return result
 		except Exception as e:
 			return False, {
 				"msg": str(e),
 				"params": {},
 				"captcha": {}
@@ -940,15 +947,15 @@
 	):
 		"""Qrcode checkin.
 		:param url: URL from Qrcode.
 		:param location: Same as checkin_checkin_location().
 		:return: Same as checkin_checkin_location().
 		"""
 		try:
-			assert "mobilelearn.chaoxing.com/widget/sign/e" in url, f"Checkin failure. {'Invalid URL.', url, dumps(location)}"
+			assert "mobilelearn.chaoxing.com/widget/sign/e" in url, f"Checkin failure. {'Invalid URL.', url}"
 			match = search(r"id=(\d+).*?([0-9A-F]{32})", url)
 			return self.checkin_checkin_qrcode(activity = {
 				"active_id": match.group(1),
 				"enc": match.group(2)
 			}, location = location)
 		except Exception as e:
 			return False, {
```

### Comparing `Xdcheckin-2.0.1/src/xdcheckin/core/locations.py` & `Xdcheckin-2.0.2/src/xdcheckin/core/locations.py`

 * *Files identical despite different names*

### Comparing `Xdcheckin-2.0.1/src/xdcheckin/core/xidian.py` & `Xdcheckin-2.0.2/src/xdcheckin/core/xidian.py`

 * *Files 8% similar despite different names*

```diff
@@ -201,89 +201,100 @@
 		if self.logined or not chaoxing.logined or not chaoxing.cookies.get("fid") == "16820":
 			return
 		self.logined, self.chaoxing_session = True, chaoxing
 
 	def livestream_get_url(self, livestream: dict = {"live_id": ""}):
 		"""Get livestream URL.
 		:param livesteam: Live ID in dictionary.
-		:return: Livestream URL, live ID and device ID (placeholder). URL will fallback to replay URL for non-ongoing live IDs.
+		:return: Livestream URL, live ID, device ID and classroom location (placeholder). URL will fallback to replay URL for non-ongoing live IDs.
 		"""
 		url = "https://newesxidian.chaoxing.com/live/getViewUrlHls"
 		params = {
 			"liveId": livestream["live_id"]
 		}
 		res = self.chaoxing_session.get(url = url, params = params, expire_after = 86400)
 		return {
 			"url": res.text,
 			"live_id": livestream["live_id"],
-			"device": ""
+			"device": "",
+			"location": ""
 		}
 
 	def livestream_get_live_url(
-		self, livestream: dict = {"live_id": "", "device": ""}
+		self, livestream: dict = {"live_id": "", "device": "", "location": ""}
 	):
 		"""Get livestream URL.
-		:param livestream: Live ID (unused if device ID is present) or device ID in dictionary.
-		:return: Livestream URL, live ID (placeholder if not given) and device ID.
+		:param livestream: Live ID (unused if device ID is present), device ID, and location (in case device ID is not present) in dictionary.
+		:return: Livestream URL, live ID (placeholder if not given), device ID and classroom location (placeholder if device ID not given).
 		"""
 		url1 = "http://newesxidian.chaoxing.com/live/listSignleCourse"
 		params1 = {
 			"liveId": livestream.get("live_id") or ""
 		}
 		url2 = "http://newesxidian.chaoxing.com/live/getViewUrlNoCourseLive"
 		params2 = {
 			"deviceCode": livestream.get("device") or "",
 			"status": 1
 		}
+		location = livestream.get("location") or ""
 		if not livestream.get("device"):
 			res1 = self.chaoxing_session.get(url = url1, params = params1, expire_after = 86400)
 			data = res1.json() or []
 			for lesson in data:
 				if str(lesson["id"]) == livestream["live_id"]:
 					params2["deviceCode"] = lesson["deviceCode"]
+					location = lesson["schoolRoomName"].rstrip()
 					break
 		res2 = self.chaoxing_session.get(url = url2, params = params2, expire_after = 86400)
 		return {
 			"url": res2.text,
 			"live_id": params1["liveId"],
-			"device": params2["deviceCode"]
+			"device": params2["deviceCode"],
+			"location": location
 		}
 
-	def curriculum_get_curriculum(self):
-		"""Get curriculum with livestream URLs.
+	def curriculum_get_curriculum(self, week: str = ""):
+		"""Get curriculum with livestreams.
+		:param week: Week number. Defaulted to the current week.
 		:return: Chaoxing curriculum with livestreams for lessons.
 		"""
-		def _get_livestream_wrapper(class_id: str = "", live_id: str = ""):
+		def _get_livestream_wrapper(class_id: str = "", live_id: str = "", location: str = ""):
+			if not curriculum["lessons"].get(class_id):
+				return
 			if not curriculum["lessons"][class_id].get("livestreams"):
 				curriculum["lessons"][class_id]["livestreams"] = []
-			livestream = self.livestream_get_live_url(livestream = {"live_id": live_id})
+			livestream = self.livestream_get_live_url(livestream = {
+				"live_id": live_id,
+				"location": location
+			})
 			for ls in curriculum["lessons"][class_id]["livestreams"]:
-				if ls["url"] == livestream["url"]:
+				if ls["device"] == livestream["device"]:
 					return
 			curriculum["lessons"][class_id]["livestreams"].append(livestream)
 		url = "https://newesxidian.chaoxing.com/frontLive/listStudentCourseLivePage"
 		params = {
 			"fid": 16820,
 			"userId": self.chaoxing_session.cookies["UID"],
 			"termYear": 0,
 			"termId": 0,
-			"week": 0
+			"week": week or 0
 		}
-		curriculum = self.chaoxing_session.curriculum_get_curriculum()
+		curriculum = self.chaoxing_session.curriculum_get_curriculum(week = week)
 		params.update({
 			"termYear": curriculum["details"]["year"],
 			"termId": curriculum["details"]["semester"],
-			"week": curriculum["details"]["week"]
+			"week": week or curriculum["details"]["week"]
 		})
 		res = self.chaoxing_session.get(url = url, params = params, expire_after = 86400)
 		data = res.json() or []
 		threads = [
 			Thread(target = _get_livestream_wrapper, kwargs = {
 				"class_id": str(lesson["teachClazzId"]),
-				"live_id": str(lesson["id"])
+				"live_id": str(lesson["id"]),
+				"location": lesson["place"]
 			}) for lesson in data
 		]
 		for thread in threads:
 			thread.start()
 		for thread in threads:
 			thread.join()
 		return curriculum
```

### Comparing `Xdcheckin-2.0.1/src/xdcheckin/server/server.py` & `Xdcheckin-2.0.2/src/xdcheckin/server/server.py`

 * *Files identical despite different names*

### Comparing `Xdcheckin-2.0.1/src/xdcheckin/server/static/activity.js` & `Xdcheckin-2.0.2/src/xdcheckin/server/static/activity.js`

 * *Files identical despite different names*

### Comparing `Xdcheckin-2.0.1/src/xdcheckin/server/static/classroom.js` & `Xdcheckin-2.0.2/src/xdcheckin/server/static/classroom.js`

 * *Files identical despite different names*

### Comparing `Xdcheckin-2.0.1/src/xdcheckin/server/static/curriculum.js` & `Xdcheckin-2.0.2/src/xdcheckin/server/static/curriculum.js`

 * *Files 7% similar despite different names*

#### js-beautify {}

```diff
@@ -37,27 +37,27 @@
             let bgn = timetable[v.period_begin - 1].slice(0, 5);
             let end = timetable[v.period_end - 1].slice(6, 11);
             td.appendChild(document.createTextNode(`${v.day}  ` +
                 `${bgn}-${end}`));
 
         });
         td = tr.appendChild(newElement("td"));
-        lesson.locations.forEach((v, i) => {
-            if (i)
-                td.appendChild(newElement("br"));
-            td.appendChild(document.createTextNode(v));
-        });
         if (!with_live)
-            continue;
-        td = tr.appendChild(newElement("td"));
-        lesson.livestreams.forEach((v, i) => {
-            if (i)
-                td.appendChild(newElement("br"));
-            td.appendChild(newElement("button", {
-                innerText: v.live_id,
-                onclick: () => setClassroom(v.url, v.live_id)
-            }));
-        });
+            lesson.locations.forEach((v, i) => {
+                if (i)
+                    td.appendChild(newElement("br"));
+                td.appendChild(document.createTextNode(v));
+            });
+        else
+            lesson.livestreams.forEach((v, i) => {
+                if (i)
+                    td.appendChild(newElement("br"));
+                td.appendChild(newElement("button", {
+                    innerText: v.location,
+                    onclick: () => setClassroom(v.url,
+                        v.live_id)
+                }));
+            });
     }
     document.getElementById("curriculum-list-div").appendChild(table);
     getCurriculum.calling = false;
 }
```

### Comparing `Xdcheckin-2.0.1/src/xdcheckin/server/static/g_classroom_urls.js` & `Xdcheckin-2.0.2/src/xdcheckin/server/static/g_classroom_urls.js`

 * *Files identical despite different names*

### Comparing `Xdcheckin-2.0.1/src/xdcheckin/server/static/location.js` & `Xdcheckin-2.0.2/src/xdcheckin/server/static/location.js`

 * *Files identical despite different names*

### Comparing `Xdcheckin-2.0.1/src/xdcheckin/server/static/login.js` & `Xdcheckin-2.0.2/src/xdcheckin/server/static/login.js`

 * *Files identical despite different names*

### Comparing `Xdcheckin-2.0.1/src/xdcheckin/server/static/misc.js` & `Xdcheckin-2.0.2/src/xdcheckin/server/static/misc.js`

 * *Files identical despite different names*

### Comparing `Xdcheckin-2.0.1/src/xdcheckin/server/static/player.js` & `Xdcheckin-2.0.2/src/xdcheckin/server/static/player.js`

 * *Files identical despite different names*

### Comparing `Xdcheckin-2.0.1/src/xdcheckin/server/static/style.css` & `Xdcheckin-2.0.2/src/xdcheckin/server/static/style.css`

 * *Files identical despite different names*

### Comparing `Xdcheckin-2.0.1/src/xdcheckin/server/static/util.js` & `Xdcheckin-2.0.2/src/xdcheckin/server/static/util.js`

 * *Files identical despite different names*

### Comparing `Xdcheckin-2.0.1/src/xdcheckin/server/templates/index.html` & `Xdcheckin-2.0.2/src/xdcheckin/server/templates/index.html`

 * *Files identical despite different names*

### Comparing `Xdcheckin-2.0.1/src/xdcheckin/util/chaoxing_captcha.py` & `Xdcheckin-2.0.2/src/xdcheckin/util/chaoxing_captcha.py`

 * *Files identical despite different names*

