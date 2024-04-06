# Comparing `tmp/filetrack-0.0.2.tar.gz` & `tmp/filetrack-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "filetrack-0.0.2.tar", last modified: Sat Apr  6 14:17:33 2024, max compression
+gzip compressed data, was "filetrack-0.0.3.tar", last modified: Sat Apr  6 14:29:55 2024, max compression
```

## Comparing `filetrack-0.0.2.tar` & `filetrack-0.0.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-04-06 14:17:33.924438 filetrack-0.0.2/
--rw-rw-rw-   0        0        0     1519 2024-04-03 13:43:42.000000 filetrack-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     4137 2024-04-06 14:17:33.923436 filetrack-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1306 2024-04-06 12:02:19.000000 filetrack-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-06 14:17:33.893298 filetrack-0.0.2/filetrack/
--rw-rw-rw-   0        0        0     6680 2024-04-06 11:56:01.000000 filetrack-0.0.2/filetrack/Trackfile.py
--rw-rw-rw-   0        0        0     5003 2024-04-06 11:57:29.000000 filetrack-0.0.2/filetrack/__init__.py
--rw-rw-rw-   0        0        0       83 2024-04-03 13:43:42.000000 filetrack-0.0.2/filetrack/__main__.py
--rw-rw-rw-   0        0        0      680 2024-04-06 12:05:03.000000 filetrack-0.0.2/filetrack/command_line.py
-drwxrwxrwx   0        0        0        0 2024-04-06 14:17:33.922435 filetrack-0.0.2/filetrack.egg-info/
--rw-rw-rw-   0        0        0     4137 2024-04-06 14:17:33.000000 filetrack-0.0.2/filetrack.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      435 2024-04-06 14:17:33.000000 filetrack-0.0.2/filetrack.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-06 14:17:33.000000 filetrack-0.0.2/filetrack.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2024-04-06 14:17:33.000000 filetrack-0.0.2/filetrack.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       77 2024-04-06 14:17:33.000000 filetrack-0.0.2/filetrack.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-04-06 14:17:33.000000 filetrack-0.0.2/filetrack.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1393 2024-04-06 07:21:50.000000 filetrack-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       14 2024-04-03 13:43:42.000000 filetrack-0.0.2/requirements-dev.txt
--rw-rw-rw-   0        0        0        9 2024-04-06 07:21:29.000000 filetrack-0.0.2/requirements-opt.txt
--rw-rw-rw-   0        0        0       46 2024-04-06 07:21:08.000000 filetrack-0.0.2/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-04-06 14:17:33.925434 filetrack-0.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-06 14:17:33.920433 filetrack-0.0.2/tests/
--rw-rw-rw-   0        0        0     1246 2024-04-03 13:43:42.000000 filetrack-0.0.2/tests/test_command_line.py
--rw-rw-rw-   0        0        0     1191 2024-04-03 13:43:42.000000 filetrack-0.0.2/tests/test_filetrack.py
+drwxrwxrwx   0        0        0        0 2024-04-06 14:29:55.902827 filetrack-0.0.3/
+-rw-rw-rw-   0        0        0     1519 2024-04-03 13:43:42.000000 filetrack-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     4137 2024-04-06 14:29:55.901825 filetrack-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1306 2024-04-06 12:02:19.000000 filetrack-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-06 14:29:55.873560 filetrack-0.0.3/filetrack/
+-rw-rw-rw-   0        0        0     6680 2024-04-06 11:56:01.000000 filetrack-0.0.3/filetrack/Trackfile.py
+-rw-rw-rw-   0        0        0     5260 2024-04-06 14:29:21.000000 filetrack-0.0.3/filetrack/__init__.py
+-rw-rw-rw-   0        0        0       83 2024-04-03 13:43:42.000000 filetrack-0.0.3/filetrack/__main__.py
+-rw-rw-rw-   0        0        0      680 2024-04-06 12:05:03.000000 filetrack-0.0.3/filetrack/command_line.py
+drwxrwxrwx   0        0        0        0 2024-04-06 14:29:55.900823 filetrack-0.0.3/filetrack.egg-info/
+-rw-rw-rw-   0        0        0     4137 2024-04-06 14:29:55.000000 filetrack-0.0.3/filetrack.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      435 2024-04-06 14:29:55.000000 filetrack-0.0.3/filetrack.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-06 14:29:55.000000 filetrack-0.0.3/filetrack.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2024-04-06 14:29:55.000000 filetrack-0.0.3/filetrack.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       77 2024-04-06 14:29:55.000000 filetrack-0.0.3/filetrack.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-04-06 14:29:55.000000 filetrack-0.0.3/filetrack.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1393 2024-04-06 07:21:50.000000 filetrack-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       14 2024-04-03 13:43:42.000000 filetrack-0.0.3/requirements-dev.txt
+-rw-rw-rw-   0        0        0        9 2024-04-06 07:21:29.000000 filetrack-0.0.3/requirements-opt.txt
+-rw-rw-rw-   0        0        0       46 2024-04-06 07:21:08.000000 filetrack-0.0.3/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-04-06 14:29:55.902827 filetrack-0.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-06 14:29:55.898826 filetrack-0.0.3/tests/
+-rw-rw-rw-   0        0        0     1246 2024-04-03 13:43:42.000000 filetrack-0.0.3/tests/test_command_line.py
+-rw-rw-rw-   0        0        0     1191 2024-04-03 13:43:42.000000 filetrack-0.0.3/tests/test_filetrack.py
```

### Comparing `filetrack-0.0.2/LICENSE` & `filetrack-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `filetrack-0.0.2/PKG-INFO` & `filetrack-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: filetrack
-Version: 0.0.2
+Version: 0.0.3
 Summary: Tracking file changes according to the record file.
 Author-email: Kyan <kai@kyan001.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2024, Kyan
         
         Redistribution and use in source and binary forms, with or without
```

### Comparing `filetrack-0.0.2/README.md` & `filetrack-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `filetrack-0.0.2/filetrack/Trackfile.py` & `filetrack-0.0.3/filetrack/Trackfile.py`

 * *Files identical despite different names*

### Comparing `filetrack-0.0.2/filetrack/__init__.py` & `filetrack-0.0.3/filetrack/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import fuzzyfinder
 import consolecmdtools as cct
 import consoleiotools as cit
 
 from . import Trackfile
 
 
-__version__ = '0.0.2'
+__version__ = '0.0.3'
 
 
 def get_configs(config_path: str = "filetrack.toml") -> dict:
     """Get configurations from the config file.
 
     Args:
         config_path (str, optional): The path or the file name of the config file. Defaults to "filetrack.toml".
@@ -63,33 +63,37 @@
             else:
                 cit.echo(f"{pres['delete']} {filename}")
     for filename in entries_added:
         cit.echo(f"{pres['add']} {filename}")
     return True
 
 
-def run_filetrack(config_path: str = "filetrack.toml", target_dir: str = os.getcwd(), target_exts: list[str] = ["mp3", "m4a"], trackfile_dir: str = os.getcwd(), trackfile_format: str = "json", hash_mode: str = "CRC32", group_by: str = ""):
+def run_filetrack(config_path: str = "filetrack.toml", target_dir: str = ".", target_exts: list[str] = ["mp3", "m4a"], trackfile_dir: str = ".", trackfile_format: str = "json", hash_mode: str = "CRC32", group_by: str = ""):
     """Run filetrack
 
     Args:
         config_path (str, optional): The path or the file name of the config file. Defaults to "filetrack.toml".
-        target_dir (str): The directory path of the files to be tracked. Default is the current working folder.
+        target_dir (str): The directory path of the files to be tracked. Default is config file's parent directory.
         target_exts (list[str], optional): The target extensions. Defaults to TARGET_EXTS.
-        trackfile_dir (str): The directory path of the trackfile. Default is the current working folder.
+        trackfile_dir (str): The directory path of the trackfile. Default is config file's parent directory.
         trackfile_format (str, optional): The output format. Defaults to "json". Options: "json", "toml".
         hash_mode (str, optional): The hash mode. Defaults to "CRC32". Options: "CRC32", "MD5", "NAME", "PATH", "MTIME".
         group_by (str, optional): Group by. Defaults to "". Options: "host", "os", "".
     """
     cit.rule("▶ [yellow]Run Filetrack")
     configs = get_configs(config_path)
     if target_configs := configs.get("target"):
         target_dir = target_configs.get("dir") or target_dir
+        if not os.path.isabs(target_dir):
+            target_dir = os.path.join(cct.get_path(config_path).parent, target_dir)
         target_exts = target_configs.get("exts") or target_exts
     if trackfile_configs := configs.get("trackfile"):
         trackfile_dir = trackfile_configs.get("dir") or trackfile_dir
+        if not os.path.isabs(trackfile_dir):
+            trackfile_dir = os.path.join(cct.get_path(config_path).parent, trackfile_dir)
         trackfile_format = trackfile_configs.get("format") or trackfile_format
         hash_mode = trackfile_configs.get("hash_mode") or hash_mode
         group_by = trackfile_configs.get("group_by") or group_by
         trackfile_prefix = trackfile_configs.get("prefix") or "FileTrack-"
     target_dir = cct.get_path(target_dir)
     trackfile_dir = cct.get_path(trackfile_dir)
     old_ft = Trackfile.Trackfile(trackfile_dir=trackfile_dir, prefix=trackfile_prefix, format=trackfile_format, group_by=group_by)
```

### Comparing `filetrack-0.0.2/filetrack/command_line.py` & `filetrack-0.0.3/filetrack/command_line.py`

 * *Files identical despite different names*

### Comparing `filetrack-0.0.2/filetrack.egg-info/PKG-INFO` & `filetrack-0.0.3/filetrack.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: filetrack
-Version: 0.0.2
+Version: 0.0.3
 Summary: Tracking file changes according to the record file.
 Author-email: Kyan <kai@kyan001.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2024, Kyan
         
         Redistribution and use in source and binary forms, with or without
```

### Comparing `filetrack-0.0.2/pyproject.toml` & `filetrack-0.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `filetrack-0.0.2/tests/test_command_line.py` & `filetrack-0.0.3/tests/test_command_line.py`

 * *Files identical despite different names*

### Comparing `filetrack-0.0.2/tests/test_filetrack.py` & `filetrack-0.0.3/tests/test_filetrack.py`

 * *Files identical despite different names*

