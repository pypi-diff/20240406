# Comparing `tmp/pyprland-2.2.0.tar.gz` & `tmp/pyprland-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyprland-2.2.0.tar", max compression
+gzip compressed data, was "pyprland-2.2.1.tar", max compression
```

## Comparing `pyprland-2.2.0.tar` & `pyprland-2.2.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     1070 2024-02-16 16:53:56.731771 pyprland-2.2.0/LICENSE
--rw-r--r--   0        0        0     5366 2024-04-03 21:58:48.932070 pyprland-2.2.0/README.md
--rw-r--r--   0        0        0        0 2024-03-03 01:47:24.891034 pyprland-2.2.0/pyprland/__init__.py
--rw-r--r--   0        0        0        0 2024-03-03 01:47:24.891034 pyprland-2.2.0/pyprland/adapters/__init__.py
--rw-r--r--   0        0        0      400 2024-04-05 20:13:47.397221 pyprland-2.2.0/pyprland/adapters/colors.py
--rw-r--r--   0        0        0     4377 2024-03-03 01:47:24.894367 pyprland-2.2.0/pyprland/adapters/menus.py
--rwxr-xr-x   0        0        0    15685 2024-04-05 21:22:04.241803 pyprland-2.2.0/pyprland/command.py
--rwxr-xr-x   0        0        0    15815 2024-04-05 21:08:59.846455 pyprland-2.2.0/pyprland/command.py.orig
--rw-r--r--   0        0        0     4133 2024-03-03 01:47:24.921035 pyprland-2.2.0/pyprland/common.py
--rw-r--r--   0        0        0     5948 2024-03-31 20:05:57.091220 pyprland-2.2.0/pyprland/ipc.py
--rw-r--r--   0        0        0       45 2024-03-03 01:47:24.897701 pyprland-2.2.0/pyprland/plugins/__init__.py
--rw-r--r--   0        0        0      106 2024-03-03 01:47:24.897701 pyprland-2.2.0/pyprland/plugins/experimental.py
--rw-r--r--   0        0        0     1647 2024-03-03 01:47:24.914368 pyprland-2.2.0/pyprland/plugins/expose.py
--rw-r--r--   0        0        0     1386 2024-03-30 16:09:04.631012 pyprland-2.2.0/pyprland/plugins/fetch_client_menu.py
--rw-r--r--   0        0        0     2601 2024-03-03 01:47:24.901034 pyprland-2.2.0/pyprland/plugins/interface.py
--rw-r--r--   0        0        0     7972 2024-03-03 01:47:24.917701 pyprland-2.2.0/pyprland/plugins/layout_center.py
--rw-r--r--   0        0        0     1677 2024-03-03 01:47:24.901034 pyprland-2.2.0/pyprland/plugins/lost_windows.py
--rw-r--r--   0        0        0     1239 2024-04-03 21:48:38.877707 pyprland-2.2.0/pyprland/plugins/magnify.py
--rw-r--r--   0        0        0     8684 2024-03-31 17:52:13.879696 pyprland-2.2.0/pyprland/plugins/monitors.py
--rw-r--r--   0        0        0     8720 2024-03-30 19:02:09.575863 pyprland-2.2.0/pyprland/plugins/monitors.py.orig
--rw-r--r--   0        0        0     3922 2024-03-03 01:47:24.904368 pyprland-2.2.0/pyprland/plugins/monitors_v0.py
--rw-r--r--   0        0        0        0 2024-04-04 16:21:22.101700 pyprland-2.2.0/pyprland/plugins/nohup.out
--rw-r--r--   0        0        0     1218 2024-03-03 01:47:24.907701 pyprland-2.2.0/pyprland/plugins/pyprland.py
--rw-r--r--   0        0        0    35284 2024-04-05 11:26:39.264749 pyprland-2.2.0/pyprland/plugins/scratchpads.py
--rw-r--r--   0        0        0     1058 2024-03-03 01:47:24.907701 pyprland-2.2.0/pyprland/plugins/shift_monitors.py
--rw-r--r--   0        0        0     4122 2024-03-03 01:47:24.917701 pyprland-2.2.0/pyprland/plugins/shortcuts_menu.py
--rw-r--r--   0        0        0     3983 2024-04-05 20:13:47.397221 pyprland-2.2.0/pyprland/plugins/system_notifier.py
--rw-r--r--   0        0        0      519 2024-03-03 01:47:24.911034 pyprland-2.2.0/pyprland/plugins/toggle_dpms.py
--rw-r--r--   0        0        0     1063 2024-03-03 01:47:24.917701 pyprland-2.2.0/pyprland/plugins/toggle_special.py
--rw-r--r--   0        0        0     3764 2024-04-05 20:13:47.397221 pyprland-2.2.0/pyprland/plugins/wallpapers.py
--rw-r--r--   0        0        0     2589 2024-03-03 01:47:24.911034 pyprland-2.2.0/pyprland/plugins/workspaces_follow_focus.py
--rw-r--r--   0        0        0      725 2024-04-05 21:21:12.163408 pyprland-2.2.0/pyproject.toml
--rw-r--r--   0        0        0     5905 1970-01-01 00:00:00.000000 pyprland-2.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-02-16 16:53:56.731771 pyprland-2.2.1/LICENSE
+-rw-r--r--   0        0        0     5425 2024-04-05 22:08:40.558921 pyprland-2.2.1/README.md
+-rw-r--r--   0        0        0        0 2024-03-03 01:47:24.891034 pyprland-2.2.1/pyprland/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-03 01:47:24.891034 pyprland-2.2.1/pyprland/adapters/__init__.py
+-rw-r--r--   0        0        0      400 2024-04-05 20:13:47.397221 pyprland-2.2.1/pyprland/adapters/colors.py
+-rw-r--r--   0        0        0     4377 2024-03-03 01:47:24.894367 pyprland-2.2.1/pyprland/adapters/menus.py
+-rwxr-xr-x   0        0        0    15682 2024-04-05 22:16:19.299301 pyprland-2.2.1/pyprland/command.py
+-rwxr-xr-x   0        0        0    15808 2024-04-05 22:08:40.562254 pyprland-2.2.1/pyprland/command.py.orig
+-rw-r--r--   0        0        0     4133 2024-03-03 01:47:24.921035 pyprland-2.2.1/pyprland/common.py
+-rw-r--r--   0        0        0     5948 2024-03-31 20:05:57.091220 pyprland-2.2.1/pyprland/ipc.py
+-rw-r--r--   0        0        0       45 2024-03-03 01:47:24.897701 pyprland-2.2.1/pyprland/plugins/__init__.py
+-rw-r--r--   0        0        0      106 2024-03-03 01:47:24.897701 pyprland-2.2.1/pyprland/plugins/experimental.py
+-rw-r--r--   0        0        0     1647 2024-03-03 01:47:24.914368 pyprland-2.2.1/pyprland/plugins/expose.py
+-rw-r--r--   0        0        0     1386 2024-03-30 16:09:04.631012 pyprland-2.2.1/pyprland/plugins/fetch_client_menu.py
+-rw-r--r--   0        0        0     2601 2024-03-03 01:47:24.901034 pyprland-2.2.1/pyprland/plugins/interface.py
+-rw-r--r--   0        0        0     7972 2024-03-03 01:47:24.917701 pyprland-2.2.1/pyprland/plugins/layout_center.py
+-rw-r--r--   0        0        0     1677 2024-03-03 01:47:24.901034 pyprland-2.2.1/pyprland/plugins/lost_windows.py
+-rw-r--r--   0        0        0     1239 2024-04-03 21:48:38.877707 pyprland-2.2.1/pyprland/plugins/magnify.py
+-rw-r--r--   0        0        0     8684 2024-03-31 17:52:13.879696 pyprland-2.2.1/pyprland/plugins/monitors.py
+-rw-r--r--   0        0        0     8720 2024-03-30 19:02:09.575863 pyprland-2.2.1/pyprland/plugins/monitors.py.orig
+-rw-r--r--   0        0        0     3922 2024-03-03 01:47:24.904368 pyprland-2.2.1/pyprland/plugins/monitors_v0.py
+-rw-r--r--   0        0        0        0 2024-04-04 16:21:22.101700 pyprland-2.2.1/pyprland/plugins/nohup.out
+-rw-r--r--   0        0        0     1218 2024-03-03 01:47:24.907701 pyprland-2.2.1/pyprland/plugins/pyprland.py
+-rw-r--r--   0        0        0    35284 2024-04-05 11:26:39.264749 pyprland-2.2.1/pyprland/plugins/scratchpads.py
+-rw-r--r--   0        0        0     1058 2024-03-03 01:47:24.907701 pyprland-2.2.1/pyprland/plugins/shift_monitors.py
+-rw-r--r--   0        0        0     4122 2024-03-03 01:47:24.917701 pyprland-2.2.1/pyprland/plugins/shortcuts_menu.py
+-rw-r--r--   0        0        0     3983 2024-04-05 20:13:47.397221 pyprland-2.2.1/pyprland/plugins/system_notifier.py
+-rw-r--r--   0        0        0      519 2024-03-03 01:47:24.911034 pyprland-2.2.1/pyprland/plugins/toggle_dpms.py
+-rw-r--r--   0        0        0     1063 2024-03-03 01:47:24.917701 pyprland-2.2.1/pyprland/plugins/toggle_special.py
+-rw-r--r--   0        0        0     3764 2024-04-05 20:13:47.397221 pyprland-2.2.1/pyprland/plugins/wallpapers.py
+-rw-r--r--   0        0        0     2589 2024-03-03 01:47:24.911034 pyprland-2.2.1/pyprland/plugins/workspaces_follow_focus.py
+-rw-r--r--   0        0        0      725 2024-04-05 22:26:50.548509 pyprland-2.2.1/pyproject.toml
+-rw-r--r--   0        0        0     5964 1970-01-01 00:00:00.000000 pyprland-2.2.1/PKG-INFO
```

### Comparing `pyprland-2.2.0/LICENSE` & `pyprland-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyprland-2.2.0/README.md` & `pyprland-2.2.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -34,14 +34,17 @@
 - **Python** >= 3.11
 - **aiofiles** python package (since Pyprland >= 2.0)
 
 ## Latest major changes
 
 Check the [Releases change log](https://github.com/hyprland-community/pyprland/releases) for more information
 
+### 2.2
+
+- Adds `wallpapers` and `system_notifier` plugins
 
 ### 2.1
 
 - Requires Hyprland >= 0.37
 - [monitors](https://github.com/hyprland-community/pyprland/wiki//monitors)
   - Drops the `wlr-randr` dependency (used in `monitors` plugin)
   - simplified the syntax, no need for `()` around a screen name (will try matching the exact name first, then partial description)
```

### Comparing `pyprland-2.2.0/pyprland/adapters/menus.py` & `pyprland-2.2.1/pyprland/adapters/menus.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.2.0/pyprland/command.py` & `pyprland-2.2.1/pyprland/command.py`

 * *Files 0% similar despite different names*

```diff
@@ -344,15 +344,15 @@
 
 
 async def run_client():
     "Runs the client (CLI)"
     manager = Pyprland()
 
     if sys.argv[1] == "version":
-        print("2.1.4-23")  # Automatically updated version
+        print("2.2.1")  # Automatically updated version
         return
 
     if sys.argv[1] in ("--help", "-h", "help"):
         await manager.load_config(init=False)
 
         def format_doc(txt):
             return txt.split("\n")[0]
```

### Comparing `pyprland-2.2.0/pyprland/command.py.orig` & `pyprland-2.2.1/pyprland/command.py.orig`

 * *Files 2% similar despite different names*

```diff
@@ -345,18 +345,18 @@
 
 async def run_client():
     "Runs the client (CLI)"
     manager = Pyprland()
 
     if sys.argv[1] == "version":
 <<<<<<< HEAD
-        print("2.2.0")  # Automatically updated version
+        print("2.1.4-21")  # Automatically updated version
 =======
         print("2.1.4-19")  # Automatically updated version
->>>>>>> fb8d25b (mitigate code complexity - release)
+>>>>>>> ee2fea0 (mitigate code complexity)
         return
 
     if sys.argv[1] in ("--help", "-h", "help"):
         await manager.load_config(init=False)
 
         def format_doc(txt):
             return txt.split("\n")[0]
```

### Comparing `pyprland-2.2.0/pyprland/common.py` & `pyprland-2.2.1/pyprland/common.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.2.0/pyprland/ipc.py` & `pyprland-2.2.1/pyprland/ipc.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.2.0/pyprland/plugins/expose.py` & `pyprland-2.2.1/pyprland/plugins/expose.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.2.0/pyprland/plugins/fetch_client_menu.py` & `pyprland-2.2.1/pyprland/plugins/fetch_client_menu.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.2.0/pyprland/plugins/interface.py` & `pyprland-2.2.1/pyprland/plugins/interface.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.2.0/pyprland/plugins/layout_center.py` & `pyprland-2.2.1/pyprland/plugins/layout_center.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.2.0/pyprland/plugins/lost_windows.py` & `pyprland-2.2.1/pyprland/plugins/lost_windows.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.2.0/pyprland/plugins/magnify.py` & `pyprland-2.2.1/pyprland/plugins/magnify.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.2.0/pyprland/plugins/monitors.py` & `pyprland-2.2.1/pyprland/plugins/monitors.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.2.0/pyprland/plugins/monitors.py.orig` & `pyprland-2.2.1/pyprland/plugins/monitors.py.orig`

 * *Files identical despite different names*

### Comparing `pyprland-2.2.0/pyprland/plugins/monitors_v0.py` & `pyprland-2.2.1/pyprland/plugins/monitors_v0.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.2.0/pyprland/plugins/pyprland.py` & `pyprland-2.2.1/pyprland/plugins/pyprland.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.2.0/pyprland/plugins/scratchpads.py` & `pyprland-2.2.1/pyprland/plugins/scratchpads.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.2.0/pyprland/plugins/shift_monitors.py` & `pyprland-2.2.1/pyprland/plugins/shift_monitors.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.2.0/pyprland/plugins/shortcuts_menu.py` & `pyprland-2.2.1/pyprland/plugins/shortcuts_menu.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.2.0/pyprland/plugins/system_notifier.py` & `pyprland-2.2.1/pyprland/plugins/system_notifier.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.2.0/pyprland/plugins/toggle_dpms.py` & `pyprland-2.2.1/pyprland/plugins/toggle_dpms.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.2.0/pyprland/plugins/toggle_special.py` & `pyprland-2.2.1/pyprland/plugins/toggle_special.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.2.0/pyprland/plugins/wallpapers.py` & `pyprland-2.2.1/pyprland/plugins/wallpapers.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.2.0/pyprland/plugins/workspaces_follow_focus.py` & `pyprland-2.2.1/pyprland/plugins/workspaces_follow_focus.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.2.0/pyproject.toml` & `pyprland-2.2.1/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyprland"
-version = "2.2.0"
+version = "2.2.1"
 description = "Hyperland plugin system - batteries included"
 authors = ["fdev31 <fdev31@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "pyprland"}]
 homepage = "https://github.com/hyprland-community/pyprland/"
```

### Comparing `pyprland-2.2.0/PKG-INFO` & `pyprland-2.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyprland
-Version: 2.2.0
+Version: 2.2.1
 Summary: Hyperland plugin system - batteries included
 Home-page: https://github.com/hyprland-community/pyprland/
 License: MIT
 Author: fdev31
 Author-email: fdev31@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -50,14 +50,17 @@
 - **Python** >= 3.11
 - **aiofiles** python package (since Pyprland >= 2.0)
 
 ## Latest major changes
 
 Check the [Releases change log](https://github.com/hyprland-community/pyprland/releases) for more information
 
+### 2.2
+
+- Adds `wallpapers` and `system_notifier` plugins
 
 ### 2.1
 
 - Requires Hyprland >= 0.37
 - [monitors](https://github.com/hyprland-community/pyprland/wiki//monitors)
   - Drops the `wlr-randr` dependency (used in `monitors` plugin)
   - simplified the syntax, no need for `()` around a screen name (will try matching the exact name first, then partial description)
```

