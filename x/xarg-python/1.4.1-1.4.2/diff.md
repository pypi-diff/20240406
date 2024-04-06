# Comparing `tmp/xarg-python-1.4.1.tar.gz` & `tmp/xarg-python-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xarg-python-1.4.1.tar", last modified: Fri Apr  5 16:55:07 2024, max compression
+gzip compressed data, was "xarg-python-1.4.2.tar", last modified: Sat Apr  6 10:43:04 2024, max compression
```

## Comparing `xarg-python-1.4.1.tar` & `xarg-python-1.4.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 16:55:07.698812 xarg-python-1.4.1/
--rw-r--r--   0 root         (0) root         (0)     1093 2023-08-28 15:46:08.000000 xarg-python-1.4.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1320 2024-04-05 16:55:07.698812 xarg-python-1.4.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      656 2023-11-23 15:08:18.000000 xarg-python-1.4.1/README.md
--rw-r--r--   0 root         (0) root         (0)      579 2024-04-05 16:55:07.698812 xarg-python-1.4.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      779 2024-03-31 14:51:50.000000 xarg-python-1.4.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 16:55:07.698812 xarg-python-1.4.1/xarg/
--rw-r--r--   0 root         (0) root         (0)      463 2024-04-01 15:33:01.000000 xarg-python-1.4.1/xarg/__init__.py
--rw-r--r--   0 root         (0) root         (0)    22952 2024-04-02 15:42:25.000000 xarg-python-1.4.1/xarg/actuator.py
--rw-r--r--   0 root         (0) root         (0)      479 2024-04-05 16:53:41.000000 xarg-python-1.4.1/xarg/attribute.py
--rw-r--r--   0 root         (0) root         (0)     9216 2024-04-05 16:52:06.000000 xarg-python-1.4.1/xarg/colorful.py
--rw-r--r--   0 root         (0) root         (0)     8184 2024-03-31 14:53:08.000000 xarg-python-1.4.1/xarg/complete.py
--rw-r--r--   0 root         (0) root         (0)     8479 2024-03-31 14:51:50.000000 xarg-python-1.4.1/xarg/parser.py
--rw-r--r--   0 root         (0) root         (0)     2216 2024-03-31 14:25:54.000000 xarg-python-1.4.1/xarg/safefile.py
--rw-r--r--   0 root         (0) root         (0)     8482 2024-03-31 14:49:33.000000 xarg-python-1.4.1/xarg/scanner.py
--rw-r--r--   0 root         (0) root         (0)     1236 2024-03-31 15:00:43.000000 xarg-python-1.4.1/xarg/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 16:55:07.698812 xarg-python-1.4.1/xarg_python.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1320 2024-04-05 16:55:07.000000 xarg-python-1.4.1/xarg_python.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      425 2024-04-05 16:55:07.000000 xarg-python-1.4.1/xarg_python.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-05 16:55:07.000000 xarg-python-1.4.1/xarg_python.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       53 2024-04-05 16:55:07.000000 xarg-python-1.4.1/xarg_python.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       46 2024-04-05 16:55:07.000000 xarg-python-1.4.1/xarg_python.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2024-04-05 16:55:07.000000 xarg-python-1.4.1/xarg_python.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-05 16:55:07.000000 xarg-python-1.4.1/xarg_python.egg-info/zip-safe
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 10:43:04.735508 xarg-python-1.4.2/
+-rw-r--r--   0 root         (0) root         (0)     1093 2023-08-28 15:46:08.000000 xarg-python-1.4.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1320 2024-04-06 10:43:04.735508 xarg-python-1.4.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      656 2023-11-23 15:08:18.000000 xarg-python-1.4.2/README.md
+-rw-r--r--   0 root         (0) root         (0)      579 2024-04-06 10:43:04.735508 xarg-python-1.4.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      779 2024-03-31 14:51:50.000000 xarg-python-1.4.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 10:43:04.735508 xarg-python-1.4.2/xarg/
+-rw-r--r--   0 root         (0) root         (0)      490 2024-04-06 10:39:58.000000 xarg-python-1.4.2/xarg/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    22972 2024-04-06 10:36:59.000000 xarg-python-1.4.2/xarg/actuator.py
+-rw-r--r--   0 root         (0) root         (0)      479 2024-04-06 10:42:08.000000 xarg-python-1.4.2/xarg/attribute.py
+-rw-r--r--   0 root         (0) root         (0)     9216 2024-04-05 16:52:06.000000 xarg-python-1.4.2/xarg/colorful.py
+-rw-r--r--   0 root         (0) root         (0)     8184 2024-03-31 14:53:08.000000 xarg-python-1.4.2/xarg/complete.py
+-rw-r--r--   0 root         (0) root         (0)     8479 2024-03-31 14:51:50.000000 xarg-python-1.4.2/xarg/parser.py
+-rw-r--r--   0 root         (0) root         (0)     2216 2024-03-31 14:25:54.000000 xarg-python-1.4.2/xarg/safefile.py
+-rw-r--r--   0 root         (0) root         (0)     8482 2024-03-31 14:49:33.000000 xarg-python-1.4.2/xarg/scanner.py
+-rw-r--r--   0 root         (0) root         (0)     1236 2024-03-31 15:00:43.000000 xarg-python-1.4.2/xarg/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 10:43:04.735508 xarg-python-1.4.2/xarg_python.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1320 2024-04-06 10:43:04.000000 xarg-python-1.4.2/xarg_python.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      425 2024-04-06 10:43:04.000000 xarg-python-1.4.2/xarg_python.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-06 10:43:04.000000 xarg-python-1.4.2/xarg_python.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       53 2024-04-06 10:43:04.000000 xarg-python-1.4.2/xarg_python.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       46 2024-04-06 10:43:04.000000 xarg-python-1.4.2/xarg_python.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2024-04-06 10:43:04.000000 xarg-python-1.4.2/xarg_python.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-06 10:43:04.000000 xarg-python-1.4.2/xarg_python.egg-info/zip-safe
```

### Comparing `xarg-python-1.4.1/LICENSE` & `xarg-python-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `xarg-python-1.4.1/PKG-INFO` & `xarg-python-1.4.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xarg-python
-Version: 1.4.1
+Version: 1.4.2
 Summary: Simple command-line tool based on argparse.
 Home-page: https://github.com/bondbox/xarg-python/
 Author: Mingzhe Zou
 Author-email: zoumingzhe@outlook.com
 License: MIT
 Project-URL: Source Code, https://github.com/bondbox/xarg-python/
 Project-URL: Bug Tracker, https://github.com/bondbox/xarg-python/issues
```

### Comparing `xarg-python-1.4.1/README.md` & `xarg-python-1.4.2/README.md`

 * *Files identical despite different names*

### Comparing `xarg-python-1.4.1/setup.cfg` & `xarg-python-1.4.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `xarg-python-1.4.1/setup.py` & `xarg-python-1.4.2/setup.py`

 * *Files identical despite different names*

### Comparing `xarg-python-1.4.1/xarg/actuator.py` & `xarg-python-1.4.2/xarg/actuator.py`

 * *Files 0% similar despite different names*

```diff
@@ -300,15 +300,15 @@
     For example:
 
     >>> from typing import Optional\n
     >>> from typing import Sequence\n
 
     >>> from xarg import add_command\n
     >>> from xarg import argp\n
-    >>> from xarg import commands\n
+    >>> from xarg import cmds\n
     >>> from xarg import end_command\n
     >>> from xarg import pre_command\n
     >>> from xarg import run_command\n
 
     >>> @add_command("example")\n
     >>> def cmd(_arg: argp):\n
     >>>     argp.add_opt_on("-t", "--test")\n
@@ -322,15 +322,15 @@
     >>>     return 0\n
 
     >>> @end_command(run)\n
     >>> def end(cmds: commands) -> int:\n
     >>>     return 0\n
 
     >>> def main(argv: Optional[Sequence[str]] = None) -> int:\n
-    >>>     return commands().run(\n
+    >>>     return cmds.run(\n
     >>>         root=cmd,\n
     >>>         argv=argv,\n
     >>>         prog="xarg-example",\n
     >>>         description="Simple command-line tool based on argparse.")\n
     '''
 
     LOGGER_ARGUMENT_GROUP = "logger options"
@@ -708,7 +708,10 @@
                 return ret
             return self.__run(args, root)
         except KeyboardInterrupt:
             return EINTR
         except BaseException:
             self.logger.exception("Something went wrong:")
             return 10000
+
+
+cmds: commands = commands()
```

### Comparing `xarg-python-1.4.1/xarg/colorful.py` & `xarg-python-1.4.2/xarg/colorful.py`

 * *Files identical despite different names*

### Comparing `xarg-python-1.4.1/xarg/complete.py` & `xarg-python-1.4.2/xarg/complete.py`

 * *Files identical despite different names*

### Comparing `xarg-python-1.4.1/xarg/parser.py` & `xarg-python-1.4.2/xarg/parser.py`

 * *Files identical despite different names*

### Comparing `xarg-python-1.4.1/xarg/safefile.py` & `xarg-python-1.4.2/xarg/safefile.py`

 * *Files identical despite different names*

### Comparing `xarg-python-1.4.1/xarg/scanner.py` & `xarg-python-1.4.2/xarg/scanner.py`

 * *Files identical despite different names*

### Comparing `xarg-python-1.4.1/xarg/util.py` & `xarg-python-1.4.2/xarg/util.py`

 * *Files identical despite different names*

### Comparing `xarg-python-1.4.1/xarg_python.egg-info/PKG-INFO` & `xarg-python-1.4.2/xarg_python.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xarg-python
-Version: 1.4.1
+Version: 1.4.2
 Summary: Simple command-line tool based on argparse.
 Home-page: https://github.com/bondbox/xarg-python/
 Author: Mingzhe Zou
 Author-email: zoumingzhe@outlook.com
 License: MIT
 Project-URL: Source Code, https://github.com/bondbox/xarg-python/
 Project-URL: Bug Tracker, https://github.com/bondbox/xarg-python/issues
```

