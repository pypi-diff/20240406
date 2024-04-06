# Comparing `tmp/adbclone-0.0.3.tar.gz` & `tmp/adbclone-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adbclone-0.0.3.tar", last modified: Sun Mar 17 13:37:46 2024, max compression
+gzip compressed data, was "adbclone-0.0.4.tar", last modified: Sat Apr  6 09:00:17 2024, max compression
```

## Comparing `adbclone-0.0.3.tar` & `adbclone-0.0.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-03-17 13:37:46.031598 adbclone-0.0.3/
--rw-rw-rw-   0        0        0    11560 2024-03-17 08:58:08.000000 adbclone-0.0.3/LICENSE
--rw-rw-rw-   0        0        0    21419 2024-03-17 13:37:46.028478 adbclone-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     7974 2024-03-17 13:29:04.000000 adbclone-0.0.3/README.md
--rw-rw-rw-   0        0        0      498 2024-03-17 11:45:11.000000 adbclone-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-17 13:37:46.032599 adbclone-0.0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-03-17 13:37:45.940908 adbclone-0.0.3/src/
-drwxrwxrwx   0        0        0        0 2024-03-17 13:37:45.959391 adbclone-0.0.3/src/BetterADBSync/
-drwxrwxrwx   0        0        0        0 2024-03-17 13:37:45.971387 adbclone-0.0.3/src/BetterADBSync/FileSystems/
--rw-rw-rw-   0        0        0    10546 2024-03-17 11:47:03.000000 adbclone-0.0.3/src/BetterADBSync/FileSystems/Android.py
--rw-rw-rw-   0        0        0     8983 2024-03-17 11:47:16.000000 adbclone-0.0.3/src/BetterADBSync/FileSystems/Base.py
--rw-rw-rw-   0        0        0     2979 2024-03-17 11:47:27.000000 adbclone-0.0.3/src/BetterADBSync/FileSystems/Local.py
--rw-rw-rw-   0        0        0        0 2024-03-17 08:58:08.000000 adbclone-0.0.3/src/BetterADBSync/FileSystems/__init__.py
--rw-rw-rw-   0        0        0     8879 2024-03-17 11:46:44.000000 adbclone-0.0.3/src/BetterADBSync/SAOLogging.py
--rw-rw-rw-   0        0        0    28996 2024-03-17 13:37:05.000000 adbclone-0.0.3/src/BetterADBSync/__init__.py
--rw-rw-rw-   0        0        0     6794 2024-03-17 11:46:29.000000 adbclone-0.0.3/src/BetterADBSync/argparsing.py
-drwxrwxrwx   0        0        0        0 2024-03-17 13:37:46.024371 adbclone-0.0.3/src/adbclone.egg-info/
--rw-rw-rw-   0        0        0    21419 2024-03-17 13:37:45.000000 adbclone-0.0.3/src/adbclone.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      504 2024-03-17 13:37:45.000000 adbclone-0.0.3/src/adbclone.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-17 13:37:45.000000 adbclone-0.0.3/src/adbclone.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2024-03-17 13:37:45.000000 adbclone-0.0.3/src/adbclone.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        5 2024-03-17 13:37:45.000000 adbclone-0.0.3/src/adbclone.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-03-17 13:37:45.000000 adbclone-0.0.3/src/adbclone.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-06 09:00:17.309590 adbclone-0.0.4/
+-rw-rw-rw-   0        0        0    11560 2024-03-17 08:58:08.000000 adbclone-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0    21885 2024-04-06 09:00:17.307584 adbclone-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     8440 2024-04-06 08:48:04.000000 adbclone-0.0.4/README.md
+-rw-rw-rw-   0        0        0      498 2024-03-17 13:44:42.000000 adbclone-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-06 09:00:17.309590 adbclone-0.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-06 09:00:17.243160 adbclone-0.0.4/src/
+drwxrwxrwx   0        0        0        0 2024-04-06 09:00:17.254846 adbclone-0.0.4/src/BetterADBSync/
+drwxrwxrwx   0        0        0        0 2024-04-06 09:00:17.263220 adbclone-0.0.4/src/BetterADBSync/FileSystems/
+-rw-rw-rw-   0        0        0    10560 2024-04-06 07:06:00.000000 adbclone-0.0.4/src/BetterADBSync/FileSystems/Android.py
+-rw-rw-rw-   0        0        0     8983 2024-04-06 08:26:31.000000 adbclone-0.0.4/src/BetterADBSync/FileSystems/Base.py
+-rw-rw-rw-   0        0        0     3142 2024-04-06 08:25:30.000000 adbclone-0.0.4/src/BetterADBSync/FileSystems/Local.py
+-rw-rw-rw-   0        0        0        0 2024-03-17 08:58:08.000000 adbclone-0.0.4/src/BetterADBSync/FileSystems/__init__.py
+-rw-rw-rw-   0        0        0     8879 2024-04-06 08:26:55.000000 adbclone-0.0.4/src/BetterADBSync/SAOLogging.py
+-rw-rw-rw-   0        0        0    30257 2024-04-06 08:58:02.000000 adbclone-0.0.4/src/BetterADBSync/__init__.py
+-rw-rw-rw-   0        0        0     7091 2024-04-06 08:22:14.000000 adbclone-0.0.4/src/BetterADBSync/argparsing.py
+drwxrwxrwx   0        0        0        0 2024-04-06 09:00:17.305059 adbclone-0.0.4/src/adbclone.egg-info/
+-rw-rw-rw-   0        0        0    21885 2024-04-06 09:00:17.000000 adbclone-0.0.4/src/adbclone.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      504 2024-04-06 09:00:17.000000 adbclone-0.0.4/src/adbclone.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-06 09:00:17.000000 adbclone-0.0.4/src/adbclone.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2024-04-06 09:00:17.000000 adbclone-0.0.4/src/adbclone.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        5 2024-04-06 09:00:17.000000 adbclone-0.0.4/src/adbclone.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-06 09:00:17.000000 adbclone-0.0.4/src/adbclone.egg-info/top_level.txt
```

### Comparing `adbclone-0.0.3/LICENSE` & `adbclone-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `adbclone-0.0.3/PKG-INFO` & `adbclone-0.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adbclone
-Version: 0.0.3
+Version: 0.0.4
 Summary: Better version of adb-sync for Python3
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -210,52 +210,59 @@
 License-File: LICENSE
 Requires-Dist: rich
 
 # ⚡adbclone [![Hits](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2Fgautamajay52%2Fadbclone&count_bg=%2379C83D&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=hits&edge_flat=false)](https://github.com/gautamajay52/adbclone)
 
 > A [rclone](https://rclone.org/) like program to copy files between a computer and an Android device
 
+![adbclone GIF](https://raw.githubusercontent.com/gautamajay52/filestore/main/adbclone.gif)
+
+## ⚡Benefits:
+`adbclone` offers significantly faster and more reliable file transfers for larger files compared to traditional `MTP (Media Transfer Protocol)`
+
 ## ⚡Installation:
 
 Available on [PyPI](https://pypi.org/project/adbclone/)
 
 ```
 pip install adbclone
 ```
 
 ## ⚡Usage:
 
 To push from your computer to your phone use
 
 ```
-adbclone push LOCAL ANDROID
+adbclone --show-progress push LOCAL ANDROID
 ```
 
 To pull from your phone to your computer use
 
 ```
-adbclone pull ANDROID LOCAL
+adbclone --show-progress pull ANDROID LOCAL
 ```
 
 Full help is available with `$ adbclone --help`
 
 ## ⚡Flags:
+- `--show-progress` Show progress of transferring files
+- `--copy-to-new-folder`  updated files will be copied to a new folder to work on later and can be merged
 - `--show-tree` Show tree of source and destination
 - `--del` will delete files and folders on the destination end that are not present on the source end. This does not include exluded files.
 - `--delete-excluded` will delete excluded files and folders on the destination end.
 - `--exclude` can be used many times. Each should be a `fnmatch` pattern relative to the source. These patterns will be ignored unless `--delete-excluded` is specified.
 - `--exclude-from` can be used many times. Each should be a filename of a file containing `fnmatch` patterns relative to the source.
 
 ## ⚡ToDos:
 - [x] Add Progress
 - [ ] Multiple Transfers
 - [ ] Add more ToDos
 
-# ⚡Demo:
-![adbclone GIF](https://raw.githubusercontent.com/gautamajay52/filestore/main/adbclone.gif)
+<!-- ## ⚡Demo:
+![adbclone GIF](https://raw.githubusercontent.com/gautamajay52/filestore/main/adbclone.gif) -->
 
 ## ⚡Credits:
 * [GautamKumar(me)](https://github.com/gautamajay52) for [Something](https://github.com/gautamajay52/adbclone)
 * [adb-sync](https://github.com/jb2170/better-adb-sync) for all the hard-work.
 
 #
 <details>
```

### Comparing `adbclone-0.0.3/README.md` & `adbclone-0.0.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,49 +1,56 @@
 # ⚡adbclone [![Hits](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2Fgautamajay52%2Fadbclone&count_bg=%2379C83D&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=hits&edge_flat=false)](https://github.com/gautamajay52/adbclone)
 
 > A [rclone](https://rclone.org/) like program to copy files between a computer and an Android device
 
+![adbclone GIF](https://raw.githubusercontent.com/gautamajay52/filestore/main/adbclone.gif)
+
+## ⚡Benefits:
+`adbclone` offers significantly faster and more reliable file transfers for larger files compared to traditional `MTP (Media Transfer Protocol)`
+
 ## ⚡Installation:
 
 Available on [PyPI](https://pypi.org/project/adbclone/)
 
 ```
 pip install adbclone
 ```
 
 ## ⚡Usage:
 
 To push from your computer to your phone use
 
 ```
-adbclone push LOCAL ANDROID
+adbclone --show-progress push LOCAL ANDROID
 ```
 
 To pull from your phone to your computer use
 
 ```
-adbclone pull ANDROID LOCAL
+adbclone --show-progress pull ANDROID LOCAL
 ```
 
 Full help is available with `$ adbclone --help`
 
 ## ⚡Flags:
+- `--show-progress` Show progress of transferring files
+- `--copy-to-new-folder`  updated files will be copied to a new folder to work on later and can be merged
 - `--show-tree` Show tree of source and destination
 - `--del` will delete files and folders on the destination end that are not present on the source end. This does not include exluded files.
 - `--delete-excluded` will delete excluded files and folders on the destination end.
 - `--exclude` can be used many times. Each should be a `fnmatch` pattern relative to the source. These patterns will be ignored unless `--delete-excluded` is specified.
 - `--exclude-from` can be used many times. Each should be a filename of a file containing `fnmatch` patterns relative to the source.
 
 ## ⚡ToDos:
 - [x] Add Progress
 - [ ] Multiple Transfers
 - [ ] Add more ToDos
 
-# ⚡Demo:
-![adbclone GIF](https://raw.githubusercontent.com/gautamajay52/filestore/main/adbclone.gif)
+<!-- ## ⚡Demo:
+![adbclone GIF](https://raw.githubusercontent.com/gautamajay52/filestore/main/adbclone.gif) -->
 
 ## ⚡Credits:
 * [GautamKumar(me)](https://github.com/gautamajay52) for [Something](https://github.com/gautamajay52/adbclone)
 * [adb-sync](https://github.com/jb2170/better-adb-sync) for all the hard-work.
 
 #
 <details>
```

### Comparing `adbclone-0.0.3/src/BetterADBSync/FileSystems/Android.py` & `adbclone-0.0.4/src/BetterADBSync/FileSystems/Android.py`

 * *Files 1% similar despite different names*

```diff
@@ -248,15 +248,15 @@
     def normpath(self, path: str) -> str:
         return os.path.normpath(path).replace("\\", "/")
 
     def push_file_here(
         self, source_path, destination_path, file_task_id, cur_file_size
     ):
         adb_process = subprocess.Popen(
-            ["adb", "push", source_path, destination_path],
+            self.adb_arguments + ["push", source_path, destination_path],
             stdout=subprocess.DEVNULL,
             stderr=subprocess.DEVNULL,
         )
         self.process = adb_process
         old_file_size = 0
         file_exists = False
```

### Comparing `adbclone-0.0.3/src/BetterADBSync/FileSystems/Base.py` & `adbclone-0.0.4/src/BetterADBSync/FileSystems/Base.py`

 * *Files identical despite different names*

### Comparing `adbclone-0.0.3/src/BetterADBSync/FileSystems/Local.py` & `adbclone-0.0.4/src/BetterADBSync/FileSystems/Local.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,30 +41,34 @@
 
     def split(self, path: str) -> Tuple[str, str]:
         return os.path.split(path)
 
     def normpath(self, path: str) -> str:
         return os.path.normpath(path)
 
+    def exists(self, path: str) -> bool:
+        return os.path.exists(path)
+
     def push_file_here(
         self, source_path, destination_path, file_task_id, cur_file_size
     ):
+        os.makedirs(os.path.dirname(destination_path), exist_ok=True)
         adb_process = subprocess.Popen(
-            ["adb", "pull", source_path, destination_path],
+            self.adb_arguments + ["pull", source_path, destination_path],
             stdout=subprocess.DEVNULL,
             stderr=subprocess.DEVNULL,
         )
         self.process = adb_process
         old_file_size = 0
         file_exists = False
         if cur_file_size > 30 * 1024 * 1024:
             time.sleep(1)
             while adb_process.poll() is None:
                 if not file_exists:
-                    file_exists = os.path.exists(destination_path)
+                    file_exists = self.exists(destination_path)
                     continue
 
                 current_file_size = self.lstat(
                     destination_path
                 ).st_size  # expensive much?
                 file_name_progress.update(file_task_id, completed=current_file_size)
                 overall_progress.update(
```

### Comparing `adbclone-0.0.3/src/BetterADBSync/SAOLogging.py` & `adbclone-0.0.4/src/BetterADBSync/SAOLogging.py`

 * *Files identical despite different names*

### Comparing `adbclone-0.0.3/src/BetterADBSync/__init__.py` & `adbclone-0.0.4/src/BetterADBSync/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,41 @@
 #!/usr/bin/env python3
 
 """Sync files between a computer and an Android device"""
 
-__version__ = "0.0.3"
+__version__ = "0.0.4"
 
 import fnmatch
 import logging
 import os
 import stat
 import time
 from collections import deque
+from datetime import datetime
 from typing import List, Tuple, Union
 
 from rich import print
 from rich.text import Text
 from rich.tree import Tree
 
 from .argparsing import get_cli_args
 from .FileSystems.Android import AndroidFileSystem
 from .FileSystems.Base import FileSystem
 from .FileSystems.Local import LocalFileSystem
 from .SAOLogging import (
     FATAL,
     destination_counting_progress,
+    live,
     log_tree,
     logging_fatal,
     overall_progress,
     perror,
     setup_root_logger,
     source_counting_progress,
     truncate_path,
-    live,
 )
 
 
 class FileSyncer:
     @classmethod
     def diff_trees(
         cls,
@@ -427,22 +428,22 @@
         fs_android.test_connection()
     except BrokenPipeError:
         logging_fatal("Connection test failed")
 
     live.start()
 
     if args.direction == "push":
-        path_source = args.direction_push_local
+        path_source = args.direction_push_local.rstrip("/")
         fs_source = fs_local
-        path_destination = args.direction_push_android
+        path_destination = args.direction_push_android.rstrip("/")
         fs_destination = fs_android
     else:
-        path_source = args.direction_pull_android
+        path_source = args.direction_pull_android.rstrip("/")
         fs_source = fs_android
-        path_destination = args.direction_pull_local
+        path_destination = args.direction_pull_local.rstrip("/")
         fs_destination = fs_local
 
     path_source, path_destination = FileSyncer.paths_to_fixed_destination_paths(
         path_source, fs_source, path_destination, fs_destination
     )
 
     path_source = fs_source.normpath(path_source)
@@ -524,14 +525,40 @@
         path_destination,
         excludePatterns,
         fs_source.join,
         fs_destination.join,
         folder_file_overwrite_error=not args.dry_run and not args.force,
     )
 
+    if args.copy_to_new_folder:
+        if path_destination != "." and fs_destination.exists(path_destination):
+            path_destination = (
+                f'{path_destination}_{datetime.now().strftime("%Y_%m_%d")}'
+            )
+            if fs_destination.exists(path_destination):  # recheck the new dest path
+                files_tree_destination = fs_destination.get_files_tree(
+                    path_destination, follow_links=args.copy_links
+                )
+                (
+                    tree_delete,
+                    tree_copy,
+                    tree_excluded_source,
+                    tree_unaccounted_destination,
+                    tree_excluded_destination,
+                ) = FileSyncer.diff_trees(
+                    tree_copy,
+                    files_tree_destination,
+                    path_source,
+                    path_destination,
+                    excludePatterns,
+                    fs_source.join,
+                    fs_destination.join,
+                    folder_file_overwrite_error=not args.dry_run and not args.force,
+                )
+
     tree_delete = FileSyncer.prune_tree(tree_delete)
     tree_copy = FileSyncer.prune_tree(tree_copy)
     tree_excluded_source = FileSyncer.prune_tree(tree_excluded_source)
     tree_unaccounted_destination = FileSyncer.prune_tree(tree_unaccounted_destination)
     tree_excluded_destination = FileSyncer.prune_tree(tree_excluded_destination)
 
     tree_delete = FileSyncer.sort_tree(tree_delete)
@@ -663,14 +690,15 @@
         else:
             overall_progress.console.print(
                 "Empty non-excluded-supporting destination unaccounted tree"
             )
         overall_progress.console.print("")
 
     if tree_copy is not None:
+        fs_destination.makedirs(path_destination)
         copy_files, copy_size = FileSyncer.about_tree(tree_copy)
         overall_progress.console.print("Copying files:")
         prog_title = f"[bold red]{args.direction}ing [bold violet]{truncate_path(path_source,4)} [/bold violet]to [bold violet]{truncate_path(path_destination,4)}"
 
         fields = f"[0/{copy_files}]"
         prog_id = overall_progress.add_task(
             prog_title,
```

### Comparing `adbclone-0.0.3/src/BetterADBSync/argparsing.py` & `adbclone-0.0.4/src/BetterADBSync/argparsing.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     exclude: List[str]
     exclude_from: List[Path]
     delete: bool
     delete_excluded: bool
     force: bool
     show_progress: bool
     show_tree: bool
+    copy_to_new_folder: bool
     adb_encoding: str
 
     adb_bin: str
     adb_flags: List[str]
     adb_options: List[List[str]]
 
     direction: str
@@ -121,14 +122,22 @@
     )
     parser.add_argument(
         "--show-tree",
         help="Show tree of source and destination",
         action="store_true",
         dest="show_tree",
     )
+
+    parser.add_argument(
+        "--copy-to-new-folder",
+        help="updated files will be copied to a new folder to work on later and can be merged",
+        action="store_true",
+        dest="copy_to_new_folder",
+    )
+
     parser.add_argument(
         "--adb-encoding",
         help="Which encoding to use when talking to adb. Defaults to UTF-8. Relevant to GitHub issue #22",
         dest="adb_encoding",
         default="UTF-8",
     )
 
@@ -210,14 +219,15 @@
         args.exclude,
         args.exclude_from,
         args.delete,
         args.delete_excluded,
         args.force,
         args.show_progress,
         args.show_tree,
+        args.copy_to_new_folder,
         args.adb_encoding,
         args.adb_bin,
         args.adb_flags,
         args.adb_options,
         args.direction,
         *args_direction_
     )
```

### Comparing `adbclone-0.0.3/src/adbclone.egg-info/PKG-INFO` & `adbclone-0.0.4/src/adbclone.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adbclone
-Version: 0.0.3
+Version: 0.0.4
 Summary: Better version of adb-sync for Python3
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -210,52 +210,59 @@
 License-File: LICENSE
 Requires-Dist: rich
 
 # ⚡adbclone [![Hits](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2Fgautamajay52%2Fadbclone&count_bg=%2379C83D&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=hits&edge_flat=false)](https://github.com/gautamajay52/adbclone)
 
 > A [rclone](https://rclone.org/) like program to copy files between a computer and an Android device
 
+![adbclone GIF](https://raw.githubusercontent.com/gautamajay52/filestore/main/adbclone.gif)
+
+## ⚡Benefits:
+`adbclone` offers significantly faster and more reliable file transfers for larger files compared to traditional `MTP (Media Transfer Protocol)`
+
 ## ⚡Installation:
 
 Available on [PyPI](https://pypi.org/project/adbclone/)
 
 ```
 pip install adbclone
 ```
 
 ## ⚡Usage:
 
 To push from your computer to your phone use
 
 ```
-adbclone push LOCAL ANDROID
+adbclone --show-progress push LOCAL ANDROID
 ```
 
 To pull from your phone to your computer use
 
 ```
-adbclone pull ANDROID LOCAL
+adbclone --show-progress pull ANDROID LOCAL
 ```
 
 Full help is available with `$ adbclone --help`
 
 ## ⚡Flags:
+- `--show-progress` Show progress of transferring files
+- `--copy-to-new-folder`  updated files will be copied to a new folder to work on later and can be merged
 - `--show-tree` Show tree of source and destination
 - `--del` will delete files and folders on the destination end that are not present on the source end. This does not include exluded files.
 - `--delete-excluded` will delete excluded files and folders on the destination end.
 - `--exclude` can be used many times. Each should be a `fnmatch` pattern relative to the source. These patterns will be ignored unless `--delete-excluded` is specified.
 - `--exclude-from` can be used many times. Each should be a filename of a file containing `fnmatch` patterns relative to the source.
 
 ## ⚡ToDos:
 - [x] Add Progress
 - [ ] Multiple Transfers
 - [ ] Add more ToDos
 
-# ⚡Demo:
-![adbclone GIF](https://raw.githubusercontent.com/gautamajay52/filestore/main/adbclone.gif)
+<!-- ## ⚡Demo:
+![adbclone GIF](https://raw.githubusercontent.com/gautamajay52/filestore/main/adbclone.gif) -->
 
 ## ⚡Credits:
 * [GautamKumar(me)](https://github.com/gautamajay52) for [Something](https://github.com/gautamajay52/adbclone)
 * [adb-sync](https://github.com/jb2170/better-adb-sync) for all the hard-work.
 
 #
 <details>
```

