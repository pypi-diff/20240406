# Comparing `tmp/octobase-0.9.0.tar.gz` & `tmp/octobase-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "octobase-0.9.0.tar", last modified: Sun Mar 31 18:54:02 2024, max compression
+gzip compressed data, was "octobase-0.9.1.tar", last modified: Fri Apr  5 21:59:49 2024, max compression
```

## Comparing `octobase-0.9.0.tar` & `octobase-0.9.1.tar`

### file list

```diff
@@ -1,51 +1,52 @@
-drwxr-xr-x   0 wyvern     (501) staff       (20)        0 2024-03-31 18:54:02.459530 octobase-0.9.0/
--rw-r--r--   0 wyvern     (501) staff       (20)      552 2021-01-02 03:16:54.000000 octobase-0.9.0/LICENSE
--rw-r--r--   0 wyvern     (501) staff       (20)      694 2024-03-31 18:54:02.459263 octobase-0.9.0/PKG-INFO
--rw-r--r--   0 wyvern     (501) staff       (20)      145 2024-03-01 16:24:41.000000 octobase-0.9.0/README.md
-drwxr-xr-x   0 wyvern     (501) staff       (20)        0 2024-03-31 18:54:02.450619 octobase-0.9.0/base/
--rw-r--r--   0 wyvern     (501) staff       (20)     1358 2024-03-21 14:50:19.000000 octobase-0.9.0/base/__init__.py
--rw-r--r--   0 wyvern     (501) staff       (20)    29202 2024-02-28 19:12:30.000000 octobase-0.9.0/base/commonera.py
--rw-r--r--   0 wyvern     (501) staff       (20)     1817 2023-08-22 21:19:14.000000 octobase-0.9.0/base/consts.py
--rw-r--r--   0 wyvern     (501) staff       (20)     6971 2023-10-02 18:29:07.000000 octobase-0.9.0/base/controllers.py
--rw-r--r--   0 wyvern     (501) staff       (20)    21386 2024-03-03 21:08:01.000000 octobase-0.9.0/base/enums.py
--rwxr-xr-x   0 wyvern     (501) staff       (20)     2764 2023-08-30 16:33:23.000000 octobase-0.9.0/base/errors.py
--rwxr-xr-x   0 wyvern     (501) staff       (20)     6740 2023-12-26 20:01:59.000000 octobase-0.9.0/base/filetypes.py
--rwxr-xr-x   0 wyvern     (501) staff       (20)     8812 2024-02-09 18:03:32.000000 octobase-0.9.0/base/regexp.py
--rwxr-xr-x   0 wyvern     (501) staff       (20)     5011 2023-10-01 20:33:55.000000 octobase-0.9.0/base/registry.py
-drwxr-xr-x   0 wyvern     (501) staff       (20)        0 2024-03-31 18:54:02.453946 octobase-0.9.0/base/rightdown/
--rw-r--r--   0 wyvern     (501) staff       (20)      646 2024-03-21 20:30:19.000000 octobase-0.9.0/base/rightdown/__init__.py
--rw-r--r--   0 wyvern     (501) staff       (20)    33599 2024-03-30 21:32:14.000000 octobase-0.9.0/base/rightdown/blocks.py
--rw-r--r--   0 wyvern     (501) staff       (20)     6712 2024-02-29 17:37:34.000000 octobase-0.9.0/base/rightdown/commandline.py
--rwxr-xr-x   0 wyvern     (501) staff       (20)     6922 2024-03-30 19:26:09.000000 octobase-0.9.0/base/rightdown/enums.py
--rw-r--r--   0 wyvern     (501) staff       (20)     1724 2024-03-23 17:53:30.000000 octobase-0.9.0/base/rightdown/errors.py
--rw-r--r--   0 wyvern     (501) staff       (20)    17854 2024-03-30 18:52:06.000000 octobase-0.9.0/base/rightdown/parser.py
--rwxr-xr-x   0 wyvern     (501) staff       (20)    12461 2024-03-30 21:02:05.000000 octobase-0.9.0/base/rightdown/patterns.py
--rw-r--r--   0 wyvern     (501) staff       (20)    10897 2024-03-23 18:47:27.000000 octobase-0.9.0/base/rightdown/printers.py
--rw-r--r--   0 wyvern     (501) staff       (20)     2363 2024-03-21 19:39:07.000000 octobase-0.9.0/base/rightdown/rightdown.py
--rwxr-xr-x   0 wyvern     (501) staff       (20)     9191 2024-03-07 15:12:08.000000 octobase-0.9.0/base/rightdown/tests.py
--rw-r--r--   0 wyvern     (501) staff       (20)    12395 2024-03-30 18:53:22.000000 octobase-0.9.0/base/rightdown/tokens.py
--rwxr-xr-x   0 wyvern     (501) staff       (20)    11039 2024-03-21 14:59:39.000000 octobase-0.9.0/base/testing.py
--rwxr-xr-x   0 wyvern     (501) staff       (20)     2714 2024-01-21 19:30:10.000000 octobase-0.9.0/base/things.py
-drwxr-xr-x   0 wyvern     (501) staff       (20)        0 2024-03-31 18:54:02.457908 octobase-0.9.0/base/utils/
--rw-r--r--   0 wyvern     (501) staff       (20)      511 2023-12-12 19:38:02.000000 octobase-0.9.0/base/utils/__init__.py
--rw-r--r--   0 wyvern     (501) staff       (20)     2942 2023-08-22 21:18:51.000000 octobase-0.9.0/base/utils/decorators.py
--rw-r--r--   0 wyvern     (501) staff       (20)     4947 2023-12-18 03:41:37.000000 octobase-0.9.0/base/utils/django.py
--rw-r--r--   0 wyvern     (501) staff       (20)     6710 2024-03-21 14:48:22.000000 octobase-0.9.0/base/utils/environment.py
--rw-r--r--   0 wyvern     (501) staff       (20)     3239 2023-08-22 21:18:40.000000 octobase-0.9.0/base/utils/fuzzy.py
--rw-r--r--   0 wyvern     (501) staff       (20)     2711 2023-12-14 19:24:44.000000 octobase-0.9.0/base/utils/interactive.py
--rw-r--r--   0 wyvern     (501) staff       (20)     3337 2024-01-04 23:07:35.000000 octobase-0.9.0/base/utils/iterables.py
--rw-r--r--   0 wyvern     (501) staff       (20)     4498 2023-12-21 17:57:58.000000 octobase-0.9.0/base/utils/logging.py
--rw-r--r--   0 wyvern     (501) staff       (20)     1169 2023-08-22 21:18:32.000000 octobase-0.9.0/base/utils/metaclasses.py
--rw-r--r--   0 wyvern     (501) staff       (20)     2513 2024-01-26 19:34:02.000000 octobase-0.9.0/base/utils/misc.py
--rw-r--r--   0 wyvern     (501) staff       (20)     7003 2024-01-26 19:32:36.000000 octobase-0.9.0/base/utils/strings.py
--rwxr-xr-x   0 wyvern     (501) staff       (20)     1248 2024-03-21 15:05:33.000000 octobase-0.9.0/base/utils/tests.py
--rwxr-xr-x   0 wyvern     (501) staff       (20)     1452 2024-03-21 14:53:14.000000 octobase-0.9.0/base/utils/threadstacks.py
--rw-r--r--   0 wyvern     (501) staff       (20)     7945 2024-02-28 19:12:20.000000 octobase-0.9.0/base/utils/time.py
--rw-r--r--   0 wyvern     (501) staff       (20)     7835 2024-02-28 17:17:50.000000 octobase-0.9.0/base/whens.py
-drwxr-xr-x   0 wyvern     (501) staff       (20)        0 2024-03-31 18:54:02.458923 octobase-0.9.0/octobase.egg-info/
--rw-r--r--   0 wyvern     (501) staff       (20)      694 2024-03-31 18:54:02.000000 octobase-0.9.0/octobase.egg-info/PKG-INFO
--rw-r--r--   0 wyvern     (501) staff       (20)      955 2024-03-31 18:54:02.000000 octobase-0.9.0/octobase.egg-info/SOURCES.txt
--rw-r--r--   0 wyvern     (501) staff       (20)        1 2024-03-31 18:54:02.000000 octobase-0.9.0/octobase.egg-info/dependency_links.txt
--rw-r--r--   0 wyvern     (501) staff       (20)        5 2024-03-31 18:54:02.000000 octobase-0.9.0/octobase.egg-info/top_level.txt
--rw-r--r--   0 wyvern     (501) staff       (20)       38 2024-03-31 18:54:02.459609 octobase-0.9.0/setup.cfg
--rwxr-xr-x   0 wyvern     (501) staff       (20)     1002 2024-01-04 23:12:15.000000 octobase-0.9.0/setup.py
+drwxr-xr-x   0 wyvern     (501) staff       (20)        0 2024-04-05 21:59:49.254343 octobase-0.9.1/
+-rw-r--r--   0 wyvern     (501) staff       (20)      552 2021-01-02 03:16:54.000000 octobase-0.9.1/LICENSE
+-rw-r--r--   0 wyvern     (501) staff       (20)      694 2024-04-05 21:59:49.254088 octobase-0.9.1/PKG-INFO
+-rw-r--r--   0 wyvern     (501) staff       (20)      145 2024-03-01 16:24:41.000000 octobase-0.9.1/README.md
+drwxr-xr-x   0 wyvern     (501) staff       (20)        0 2024-04-05 21:59:49.246624 octobase-0.9.1/base/
+-rw-r--r--   0 wyvern     (501) staff       (20)     1358 2024-04-05 21:58:49.000000 octobase-0.9.1/base/__init__.py
+-rw-r--r--   0 wyvern     (501) staff       (20)    29202 2024-02-28 19:12:30.000000 octobase-0.9.1/base/commonera.py
+-rw-r--r--   0 wyvern     (501) staff       (20)     1817 2023-08-22 21:19:14.000000 octobase-0.9.1/base/consts.py
+-rw-r--r--   0 wyvern     (501) staff       (20)     6971 2023-10-02 18:29:07.000000 octobase-0.9.1/base/controllers.py
+-rw-r--r--   0 wyvern     (501) staff       (20)    21386 2024-03-03 21:08:01.000000 octobase-0.9.1/base/enums.py
+-rwxr-xr-x   0 wyvern     (501) staff       (20)     2764 2023-08-30 16:33:23.000000 octobase-0.9.1/base/errors.py
+-rwxr-xr-x   0 wyvern     (501) staff       (20)     6740 2023-12-26 20:01:59.000000 octobase-0.9.1/base/filetypes.py
+-rwxr-xr-x   0 wyvern     (501) staff       (20)     8822 2024-04-05 16:55:50.000000 octobase-0.9.1/base/regexp.py
+-rwxr-xr-x   0 wyvern     (501) staff       (20)     5011 2023-10-01 20:33:55.000000 octobase-0.9.1/base/registry.py
+drwxr-xr-x   0 wyvern     (501) staff       (20)        0 2024-04-05 21:59:49.249584 octobase-0.9.1/base/rightdown/
+-rw-r--r--   0 wyvern     (501) staff       (20)      683 2024-04-05 17:39:43.000000 octobase-0.9.1/base/rightdown/__init__.py
+-rwxr--r--   0 wyvern     (501) staff       (20)    25277 2024-04-05 19:59:57.000000 octobase-0.9.1/base/rightdown/blocks.py
+-rw-r--r--   0 wyvern     (501) staff       (20)     6639 2024-04-05 14:04:45.000000 octobase-0.9.1/base/rightdown/commandline.py
+-rwxr-xr-x   0 wyvern     (501) staff       (20)     7584 2024-04-05 19:04:30.000000 octobase-0.9.1/base/rightdown/enums.py
+-rw-r--r--   0 wyvern     (501) staff       (20)     1724 2024-03-23 17:53:30.000000 octobase-0.9.1/base/rightdown/errors.py
+-rw-r--r--   0 wyvern     (501) staff       (20)    17570 2024-04-05 17:40:25.000000 octobase-0.9.1/base/rightdown/parser.py
+-rwxr-xr-x   0 wyvern     (501) staff       (20)    11736 2024-04-05 19:09:11.000000 octobase-0.9.1/base/rightdown/patterns.py
+-rw-r--r--   0 wyvern     (501) staff       (20)    13304 2024-04-05 20:12:22.000000 octobase-0.9.1/base/rightdown/printers.py
+-rw-r--r--   0 wyvern     (501) staff       (20)     2371 2024-04-05 14:05:07.000000 octobase-0.9.1/base/rightdown/rightdown.py
+-rwxr-xr-x   0 wyvern     (501) staff       (20)     9118 2024-04-05 14:04:21.000000 octobase-0.9.1/base/rightdown/tests.py
+-rwxr--r--   0 wyvern     (501) staff       (20)    15910 2024-04-05 21:04:52.000000 octobase-0.9.1/base/rightdown/textblock.py
+-rw-r--r--   0 wyvern     (501) staff       (20)    13494 2024-04-05 20:22:35.000000 octobase-0.9.1/base/rightdown/tokens.py
+-rwxr-xr-x   0 wyvern     (501) staff       (20)    11039 2024-03-21 14:59:39.000000 octobase-0.9.1/base/testing.py
+-rwxr-xr-x   0 wyvern     (501) staff       (20)     2714 2024-01-21 19:30:10.000000 octobase-0.9.1/base/things.py
+drwxr-xr-x   0 wyvern     (501) staff       (20)        0 2024-04-05 21:59:49.252807 octobase-0.9.1/base/utils/
+-rw-r--r--   0 wyvern     (501) staff       (20)      511 2023-12-12 19:38:02.000000 octobase-0.9.1/base/utils/__init__.py
+-rw-r--r--   0 wyvern     (501) staff       (20)     2942 2023-08-22 21:18:51.000000 octobase-0.9.1/base/utils/decorators.py
+-rw-r--r--   0 wyvern     (501) staff       (20)     4947 2023-12-18 03:41:37.000000 octobase-0.9.1/base/utils/django.py
+-rw-r--r--   0 wyvern     (501) staff       (20)     6710 2024-03-21 14:48:22.000000 octobase-0.9.1/base/utils/environment.py
+-rw-r--r--   0 wyvern     (501) staff       (20)     3239 2023-08-22 21:18:40.000000 octobase-0.9.1/base/utils/fuzzy.py
+-rw-r--r--   0 wyvern     (501) staff       (20)     2711 2023-12-14 19:24:44.000000 octobase-0.9.1/base/utils/interactive.py
+-rw-r--r--   0 wyvern     (501) staff       (20)     3337 2024-01-04 23:07:35.000000 octobase-0.9.1/base/utils/iterables.py
+-rw-r--r--   0 wyvern     (501) staff       (20)     4498 2023-12-21 17:57:58.000000 octobase-0.9.1/base/utils/logging.py
+-rw-r--r--   0 wyvern     (501) staff       (20)     1169 2023-08-22 21:18:32.000000 octobase-0.9.1/base/utils/metaclasses.py
+-rw-r--r--   0 wyvern     (501) staff       (20)     2513 2024-01-26 19:34:02.000000 octobase-0.9.1/base/utils/misc.py
+-rw-r--r--   0 wyvern     (501) staff       (20)     7003 2024-01-26 19:32:36.000000 octobase-0.9.1/base/utils/strings.py
+-rwxr-xr-x   0 wyvern     (501) staff       (20)     1248 2024-03-21 15:05:33.000000 octobase-0.9.1/base/utils/tests.py
+-rwxr-xr-x   0 wyvern     (501) staff       (20)     1452 2024-03-21 14:53:14.000000 octobase-0.9.1/base/utils/threadstacks.py
+-rw-r--r--   0 wyvern     (501) staff       (20)     7945 2024-02-28 19:12:20.000000 octobase-0.9.1/base/utils/time.py
+-rw-r--r--   0 wyvern     (501) staff       (20)     7835 2024-02-28 17:17:50.000000 octobase-0.9.1/base/whens.py
+drwxr-xr-x   0 wyvern     (501) staff       (20)        0 2024-04-05 21:59:49.253759 octobase-0.9.1/octobase.egg-info/
+-rw-r--r--   0 wyvern     (501) staff       (20)      694 2024-04-05 21:59:49.000000 octobase-0.9.1/octobase.egg-info/PKG-INFO
+-rw-r--r--   0 wyvern     (501) staff       (20)      983 2024-04-05 21:59:49.000000 octobase-0.9.1/octobase.egg-info/SOURCES.txt
+-rw-r--r--   0 wyvern     (501) staff       (20)        1 2024-04-05 21:59:49.000000 octobase-0.9.1/octobase.egg-info/dependency_links.txt
+-rw-r--r--   0 wyvern     (501) staff       (20)        5 2024-04-05 21:59:49.000000 octobase-0.9.1/octobase.egg-info/top_level.txt
+-rw-r--r--   0 wyvern     (501) staff       (20)       38 2024-04-05 21:59:49.254413 octobase-0.9.1/setup.cfg
+-rwxr-xr-x   0 wyvern     (501) staff       (20)     1002 2024-01-04 23:12:15.000000 octobase-0.9.1/setup.py
```

### Comparing `octobase-0.9.0/LICENSE` & `octobase-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `octobase-0.9.0/PKG-INFO` & `octobase-0.9.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: octobase
-Version: 0.9.0
+Version: 0.9.1
 Summary: The First Building Block For Any Python Project
 Home-page: https://bitbucket.org/octoboxy/octobase/
 Author: Octoboxy
 Author-email: office@octoboxy.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `octobase-0.9.0/base/__init__.py` & `octobase-0.9.1/base/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     Licensed under the Apache License, Version 2.0
     http://www.apache.org/licenses/LICENSE-2.0
 
     Created and maintained by Octoboxy
     https://octoboxy.com/octobase/
 '''
 
-VERSION             = '0.9.0'
+VERSION             = '0.9.1'
 
 
 # Any exceptions we raise should be defined here
 from .              import errors
 
 # Massive library of helper functions
 from .              import utils
```

### Comparing `octobase-0.9.0/base/commonera.py` & `octobase-0.9.1/base/commonera.py`

 * *Files identical despite different names*

### Comparing `octobase-0.9.0/base/consts.py` & `octobase-0.9.1/base/consts.py`

 * *Files identical despite different names*

### Comparing `octobase-0.9.0/base/controllers.py` & `octobase-0.9.1/base/controllers.py`

 * *Files identical despite different names*

### Comparing `octobase-0.9.0/base/enums.py` & `octobase-0.9.1/base/enums.py`

 * *Files identical despite different names*

### Comparing `octobase-0.9.0/base/errors.py` & `octobase-0.9.1/base/errors.py`

 * *Files identical despite different names*

### Comparing `octobase-0.9.0/base/filetypes.py` & `octobase-0.9.1/base/filetypes.py`

 * *Files identical despite different names*

### Comparing `octobase-0.9.0/base/regexp.py` & `octobase-0.9.1/base/regexp.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,16 +93,16 @@
 ###
 ## smarter things
 #
 
 
 class Grouper:
   ''' class you init with a pattern, then acts like a function to turn strings into a dictionary
-      of groups matched in those strings.  if the pattern contains no groups, we return True on
-      match instead
+      of groups matched in those strings.  if the pattern contains no name groups, we return the
+      re.match object instead
   '''
 
   def __init__(self, pattern, groupermode=GROUPERMODE_SEARCH):
     self.mode       = GrouperModes(groupermode)
     self.pattern    = re.compile(pattern)
 
   def __repr__(self):
@@ -114,15 +114,15 @@
   def __eq__(self, other):
     return hash(self) == hash(other)
 
   def __call__(self, s):
     ''' returns captured groups, True if we matched but didn't capture any groups, or None if we did not match '''
     rem             = self.Match(s)
     if rem:
-      return rem.groupdict() or True
+      return rem.groupdict() or rem
 
   def Match(self, s):
     ''' returns a re.match if our pattern matches the string '''
     rem             = None
     if self.mode == GROUPERMODE_SEARCH:
       rem           = self.pattern.search(s)
     elif self.mode == GROUPERMODE_START:
```

### Comparing `octobase-0.9.0/base/registry.py` & `octobase-0.9.1/base/registry.py`

 * *Files identical despite different names*

### Comparing `octobase-0.9.0/base/rightdown/commandline.py` & `octobase-0.9.1/base/rightdown/commandline.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 #!/opt/local/bin/python
 
 import argparse
 import base
 import os
 import sys
 
-from base import rightdown
+from base                   import rightdown
+from base.rightdown.enums   import *
 
 
 class RightDownCommandLineTool:
   ''' implementation of a command-line tool to process rightdown documents '''
 
   @classmethod
   def Run(klass, timer=None):
@@ -54,18 +55,18 @@
     self.printed    = self.printer.Print(rd)
     timer.Lap('formatting output')
 
   def ConfigureThings(self):
     ''' sets up our parser and printer '''
     self.parser     = rightdown.parser.Parser()
     self.printer    = {
-        rightdown.enums.PRINTMODE_NAKED:  rightdown.printers.NakedPrinter(),
-        rightdown.enums.PRINTMODE_TEXT:   rightdown.printers.TextPrinter(),
-        rightdown.enums.PRINTMODE_HTML:   rightdown.printers.HtmlPrinter(),
-        rightdown.enums.PRINTMODE_DEBUG:  rightdown.printers.DebugPrinter(),
+        PRINTMODE_NAKED:  rightdown.printers.NakedPrinter(),
+        PRINTMODE_TEXT:   rightdown.printers.TextPrinter(),
+        PRINTMODE_HTML:   rightdown.printers.HtmlPrinter(),
+        PRINTMODE_DEBUG:  rightdown.printers.DebugPrinter(),
     }[self.output]
     for thing in (self.parser, self.printer):
       for attr, value in self.options.items():
         if hasattr(thing, attr):
           setattr(thing, attr, value)
 
   def ProcessArgs(self):
@@ -95,18 +96,18 @@
     # add our positional args
     args1.add_argument('filepath')
     args0.add_argument('filepath', metavar='FILEPATH',
         help='path to the file to read; use a single dash - to read stdin')
 
     args1.add_argument('output', nargs='?')
     args0.add_argument('output', nargs='?', metavar='OUTPUT',
-        default=rightdown.enums.PRINTMODE_HTML, type=rightdown.enums.PrintModes,
+        default=PRINTMODE_HTML, type=PrintModes,
         help=(
             'desired output format; ' +
-            self._HelpTextForEnum(rightdown.enums.PRINTMODE_HTML, rightdown.enums.PrintModes)))
+            self._HelpTextForEnum(PRINTMODE_HTML, PrintModes)))
 
     args1.add_argument('--time', action=argparse.BooleanOptionalAction)
     args0.add_argument('--time', action=argparse.BooleanOptionalAction, default=False,
         help='report how much wall time is taken by the tool')
 
     # add all the many parser and printer options
     seen            = set()
```

### Comparing `octobase-0.9.0/base/rightdown/enums.py` & `octobase-0.9.1/base/rightdown/enums.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,16 @@
     ('Early Metadata',        3),       # rd.metadata contains most metadata from fragment 0
     ('ReParsed',              4),       # if metadata is allowed to trigger a reparse, here's where it happens
     ('Metadata',              5),       # fragment 0 metadata is available
     ('Blocks',                6),       # all fragments broken down into blocks
     ('Inlines',               7),       # all text has been processed
     ('Parsed',                8),       # token tree has been validated
     ('Imprints',              9),       # (printing) tokens are serialized for the print settings
-    ('Done',                 10),       # (printing) done
+    ('Filtered',             10),       # (printing) last output filtering is applied
+    ('Done',                 11),       # (printing) done
 ))
 
 
 # text alignment
 base.Enum.Define(('ALIGN', 'Aligns'), (
     ('Default',             None),
     ('Left',                'left'),
@@ -149,26 +150,32 @@
     ('Table',               'tab,'),    # contains one or more Table Rows
     ('Text',                'txt,'),    # a formatted line of text
 ))
 
 
 base.Enum.Define(('SNIPTYPE', 'SnipTypes'), (
     ('code',                'cds,'),    # text that should be emitted in fixed-width typeface
-    ('comment',             'com,'),    # text that should not be emitted
+    ('comment',             'com,'),    # text that should not be emitted at all
     ('html',                'htm,'),    # snippet of HTML that was detected in the document
     ('icon',                'ico,'),    # icon reference
     ('plain',               'ezy,'),    # plain ol' text, ready to print
     ('template',            'tpl,'),    # template language markup that was detected in the document
+    ('format up',           'fup,',     'FORMAT_UP'),       # in-line formatting:  count goes up
+    ('format dn',           'fdn,',     'FORMAT_DOWN'),     # in-line formatting:  count goes down
+    ('format md',           'fmd,',     'FORMAT_MIDDLE'),   # in-line formatting:  count toggles
+    ('format lt',           'flt,',     'FORMAT_LEFT'),     # in-line formatting:  paragraph left
+    ('format rt',           'frt,',     'FORMAT_RIGHT'),    # in-line formatting:  paragraph right
 ))
 
 
 ###
 ## Imprints are not tokens, but are what the token tree serializes to during printing
 #
 
 
 base.Enum.Define(('IMPRINT', 'ImprintTypes'), (
     ('Markup',              'htm,'),    # markup language
     ('Formatting',          'frm,'),    # formatting text
     ('Narrative',           'txm,'),    # actual text content
+    ('Inert',               'nrt,'),    # pre-rendered and pre-escaped content
     ('Break',               'brk,'),    # indicates the end of a block
 ))
```

### Comparing `octobase-0.9.0/base/rightdown/errors.py` & `octobase-0.9.1/base/rightdown/errors.py`

 * *Files identical despite different names*

### Comparing `octobase-0.9.0/base/rightdown/parser.py` & `octobase-0.9.1/base/rightdown/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -381,36 +381,36 @@
 
 
 class TextMaker(metaclass=base.utils.Singleton):
   ''' refines a string into a text block '''
 
   def __init__(self):
     self.codesnippat  = Grouper(rightdown.patterns.CODE_SNIP_PATTERN)
-    self.blockpats    = [(x, Grouper(y)) for x,y in rightdown.patterns.TEXTBLOCK_PATTERNS]
     self.whackwhack   = Grouper(r'\\\\')
     self.whacktick    = Grouper(r'\\`')
     self.whackdot     = Grouper(r'\\.')
     self.whackspace   = (Grouper(rightdown.patterns.SIMPLE_PATTERN_NBSP[0]), rightdown.patterns.SIMPLE_PATTERN_NBSP)
+    self.blockpats0   = [(x, Grouper(y)) for x,y in rightdown.patterns.TEXTBLOCK_PATTERNS0]
+    self.blockpats1   = [(x, Grouper(y)) for x,y in rightdown.patterns.TEXTBLOCK_PATTERNS1]
     self.simplesubs   = self._CompileSimpleSubs()   # [ ( grouper, patterntuple ) ]
-    self.comingles    = [(x.tag, Grouper(x.pattern)) for x in rightdown.patterns.CoMingles]
 
   def _CompileSimpleSubs(self):
     results           = []
     for submode, patternlist in rightdown.patterns.TEXT_SUBSTITUTIONS.items():
       for patterntuple in patternlist:
         pattern       = patterntuple[0]
         decorated     = rightdown.patterns.TEXT_SUB_DECORATORS[submode](pattern)
         results.append((Grouper(decorated), patterntuple))
     return results
 
   def __call__(self, s, parenttext, **kwargs):
     if not s:
       return
 
-    text              = parenttext and parenttext.Spawn(text=s) or rightdown.blocks.Text(text=s)
+    text              = parenttext and parenttext.Spawn(text=s) or rightdown.textblock.Text(text=s)
 
     # backslash backslash
     self.SubOut(text, self.whackwhack)
 
     # backslash backtick
     self.SubOut(text, self.whacktick)
 
@@ -420,25 +420,25 @@
     # backslash space
     self.Chunk(text, self.whackspace[0], self.whackspace[1])
 
     # backslashed other characters
     self.SubOut(text, self.whackdot)
 
     # blocks and snips
-    self.ChunkTokenAll(text, self.blockpats, **kwargs)
+    self.ChunkTokenAll(text, self.blockpats0, **kwargs)
 
     # simple substitutions
     for grouper, patterntuple in self.simplesubs:
       self.Chunk(text, grouper, stash=patterntuple)
 
-    # special co-mingled formatting tokens
-    comingled       = self.CoMingles(text, self.comingles)
+    # more snips
+    self.ChunkTokenAll(text, self.blockpats1, **kwargs)
 
     # if through all this we did nothing, just return a simple snip instead
-    if not comingled and not text.subdict:
+    if not text.subdict:
       return Snip(SNIPTYPE_PLAIN, text=text.text)
     return text
 
   def Chunk(self, text, pattern, stash=None, replace=None, strip=None):
     ''' match a pattern -- that may have unnamed groups -- and (usually) stash it for later '''
     howmany         = 0
     rem             = pattern.Match(text.text)
@@ -482,15 +482,7 @@
     ''' match all patterns and replace them with a Snip of the given type '''
     for blocktype, pattern in patternlist:
       self.ChunkToken(text, blocktype, pattern, **kwargs)
 
   def SubOut(self, text, pattern):
     ''' replace backslashed characters so they can't match our patterns '''
     self.Chunk(text, pattern, strip='\\')
-
-  def CoMingles(self, text, patternlist):
-    ''' detect the co-mingled formatting characters '''
-    howmany         = 0
-    for tag, pattern in patternlist:
-      howmany       += self.Chunk(text, pattern, replace=tag)
-    return howmany
-
```

### Comparing `octobase-0.9.0/base/rightdown/patterns.py` & `octobase-0.9.1/base/rightdown/patterns.py`

 * *Files 18% similar despite different names*

```diff
@@ -133,39 +133,86 @@
 
 ###
 ## Text patterns
 #
 
 ## pattern building helpers
 
-SPACE0              = Group(Or('^', r'[^\w]'))
-SPACE1              = Group(Or(r'[^\w]', '$'))
+SPACE               = r'\s'
 NOTSPACE            = r'[^\s]'
 
-LA_SPACE1           = Group(SPACE1, grouptype=GROUPTYPE_LOOK_AHEAD)
+LA_SPACE            = Group(Or('$', Group(SPACE, grouptype=GROUPTYPE_LOOK_AHEAD)))
+LB_SPACE            = Group(Or('^', Group(SPACE, grouptype=GROUPTYPE_LOOK_BEHIND)))
+
+LA_NOTSPACE         = Group(NOTSPACE, grouptype=GROUPTYPE_LOOK_AHEAD)
 LB_NOTSPACE         = Group(NOTSPACE, grouptype=GROUPTYPE_LOOK_BEHIND)
 
+# decorators that help in TEXT_SUBSTITUTIONS
+
+SPACISH             = r'[^\w]'
+SPACISH0            = Group(Or('^', SPACISH))
+SPACISH1            = Group(Or(SPACISH, '$'))
+
 TEXT_SUB_DECORATORS = {
     SUBMODE_ALL:      lambda x: Capture(x),
-    SUBMODE_SOLO:     lambda x: SPACE0 + Capture(x) + SPACE1,
-    SUBMODE_OPEN:     lambda x: SPACE0 + Capture(x),
-    SUBMODE_CLOSE:    lambda x: Capture(x) + SPACE1,
+    SUBMODE_SOLO:     lambda x: SPACISH0 + Capture(x) + SPACISH1,
+    SUBMODE_OPEN:     lambda x: SPACISH0 + Capture(x),
+    SUBMODE_CLOSE:    lambda x: Capture(x) + SPACISH1,
     SUBMODE_NOTOPEN:  lambda x: NOTSPACE + Capture(x)
-
 }
 
+# couple patterns we match early
+
+SIMPLE_PATTERN_NBSP = (r'\\ ', CHAR_NO_BREAK_SPACE)
+CODE_SNIP_PATTERN   = '`' + Capture('.*?', name='text') + '`'
+
+# pieces of a link
+
+IMAGE               = Capture('!?', name='image')
+FLAGS               = Capture('.*?', name='flags')
+TITLE               = Capture('.*?', name='text')
+URL                 = Capture('.*?', name='url')
+PROTOCOL            = Capture(Or('https?:/', 'mailto:'), name='protocol')
 
-## simple text substitutions
+# HTML
+
+HTMLATTR0           = '\\s*\\w+\\s*' + Optional('=' + '\\s*".*?"')
+HTMLATTR1           = '\\s*\\w+\\s*' + Optional('=' + "\\s*'.*?'")
+HTMLTAGOPEN         = '<\\w+' + Group(Or(HTMLATTR0, HTMLATTR1)) + '*\\s*/?>'
+HTMLTAGCLOSE        = '</\\w+\s*>'
+HTMLTAGCOMMENT      = '<!.*?>'
 
 HTML_TH             = '<sup><u>th</u></sup>'
 HTML_ST             = '<sup><u>st</u></sup>'
 HTML_ND             = '<sup><u>nd</u></sup>'
 HTML_RD             = '<sup><u>rd</u></sup>'
 
-SIMPLE_PATTERN_NBSP = (r'\\ ', CHAR_NO_BREAK_SPACE)
+## these patterns identify range-based parts of text
+
+TEXTBLOCK_PATTERNS0 = (
+    (BLOCKTYPE_LINK,            IMAGE + r'\[\[' + FLAGS + r'\]\]\(' + URL + r'\)'),
+    (BLOCKTYPE_LINK,            IMAGE + r'\['   + TITLE +   r'\]\(' + URL + r'\)'),
+    (BLOCKTYPE_LINK,            IMAGE + r'\[\(' + URL   + r'\)\]'),
+    (BLOCKTYPE_LINK,            LB_SPACE + PROTOCOL + URL + LA_SPACE),
+    (SNIPTYPE_ICON,             r'\(\(' + Capture('\w+\s?' + Group('\w+')) + '\)\)'),
+    (SNIPTYPE_TEMPLATE,         Capture(r'{%.*?%}', name='text')),
+    (SNIPTYPE_TEMPLATE,         Capture(r'{{.*?}}', name='text')),
+    (SNIPTYPE_COMMENT,          Capture(r'{#.*?#}', name='text')),
+    (SNIPTYPE_HTML,             Capture(HTMLTAGOPEN, name='text')),
+    (SNIPTYPE_HTML,             Capture(HTMLTAGCLOSE, name='text')),
+    (SNIPTYPE_COMMENT,          Capture(HTMLTAGCOMMENT, name='text')),
+    (BLOCKTYPE_SUBSCRIPT,       LB_NOTSPACE + '~' + r'\(' + Capture('.*?', name='text') + r'\)' + LA_SPACE),
+    (BLOCKTYPE_SUPERSCRIPT,     LB_NOTSPACE + '\\^' + r'\(' + Capture('.*?', name='text') + r'\)' + LA_SPACE),
+    (BLOCKTYPE_SUPERSCRIPT,     LB_NOTSPACE + '\\^' + Capture(r'.+?', name='text') + LA_SPACE),
+    # *DISABLED BY INTENTION*
+    #   because mid-word strikethrough is more useful
+    # (BLOCKTYPE_SUBSCRIPT,     NOTSPACE + '~' + Capture(r'\w+', name='sub') + SPACE),
+)
+
+## these simple substitutions apply after the text blocks have been found
 
 # tuples are:  (pattern, naked, text, html)
 #   if html is missing, naked will be used
 #   if text is missing, pattern will be used
 TEXT_SUBSTITUTIONS  = {
     SUBMODE_ALL:    (
         SIMPLE_PATTERN_NBSP,
@@ -173,14 +220,15 @@
         (r'\.\.\.',             CHAR_ELLIPSIS,          '...'),
         ('<-->',                CHAR_BI_ARROW),
         ('-->',                 CHAR_RIGHT_ARROW),
         ('<--',                 CHAR_LEFT_ARROW),
         ('---',                 CHAR_EMDASH),
         ('--',                  CHAR_ENDASH),
         (r'\+/-',               CHAR_PLUS_MINUS),
+        ('!=',                  CHAR_NOT_EQUAL),
         ('=/=',                 CHAR_NOT_EQUAL),
         ('~=',                  CHAR_ALMOST_EQUAL),
     ),
     SUBMODE_SOLO:   (
         ('1/2',                 CHAR_ONE_HALF),
         ('1/3',                 CHAR_ONE_THIRD),
         ('2/3',                 CHAR_TWO_THIRDS),
@@ -195,15 +243,15 @@
         ('1/8',                 CHAR_ONE_EIGHTH),
         ('3/8',                 CHAR_THREE_EIGHTHS),
         ('5/8',                 CHAR_FIVE_EIGTHS),
         ('7/8',                 CHAR_SEVEN_EIGHTS),
         (r'\(c\)',              CHAR_COPYRIGHT,         '(c)'),           # xyzzy: revisit
         (r'\(tm\)',             CHAR_TRADEMARK,         '(tm)'),
         (r'\(r\)',              CHAR_REGISTERED,        '(r)'),
-        ( '0' + Capture('st'),  HTML_ST),
+        ( '0' + Capture('st'),  'st',                   'st',             HTML_ST),
     ),
     SUBMODE_OPEN:   (
         ("'",                   CHAR_LEFT_TICK),
         ('"',                   CHAR_LEFT_QUOTE),
     ),
     SUBMODE_CLOSE:  (
         ('11' + Capture('th'),  'th',                   'th',             HTML_TH),
@@ -222,63 +270,20 @@
     ),
     SUBMODE_NOTOPEN:  (
         ("'",           CHAR_RIGHT_TICK),
         ('"',           CHAR_RIGHT_QUOTE),
     ),
 }
 
-## these patterns identify range-based parts of text
-
-IMAGE               = Capture('!?', name='image')
-FLAGS               = Capture('.*?', name='flags')
-TITLE               = Capture('.*?', name='text')
-URL                 = Capture('.*?', name='url')
-PROTOCOL            = Capture(Or('https?:/', 'mailto:'), name='protocol')
-
-CODE_SNIP_PATTERN   = '`' + Capture('.*?', name='text') + '`'
-
-HTMLATTR0           = '\\s*\\w+\\s*' + Optional('=' + '\\s*".*?"')
-HTMLATTR1           = '\\s*\\w+\\s*' + Optional('=' + "\\s*'.*?'")
-HTMLTAGOPEN         = '<\\w+' + Group(Or(HTMLATTR0, HTMLATTR1)) + '*\\s*/?>'
-HTMLTAGCLOSE        = '</\\w+\s*>'
-HTMLTAGCOMMENT      = '<!.*?>'
-
+## these patterns apply last
 
-TEXTBLOCK_PATTERNS  = (
-    (BLOCKTYPE_LINK,            IMAGE + r'\[\[' + FLAGS + r'\]\]\(' + URL + r'\)'),
-    (BLOCKTYPE_LINK,            IMAGE + r'\['   + TITLE +   r'\]\(' + URL + r'\)'),
-    (BLOCKTYPE_LINK,            IMAGE + r'\[\(' + URL   + r'\)\]'),
-    (BLOCKTYPE_LINK,            PROTOCOL + URL + SPACE1),
-    (SNIPTYPE_ICON,             r'\(\(' + Capture('\w+\s?' + Group('\w+')) + '\)\)'),
-    (SNIPTYPE_TEMPLATE,         Capture(r'{%.*?%}', name='text')),
-    (SNIPTYPE_TEMPLATE,         Capture(r'{{.*?}}', name='text')),
-    (SNIPTYPE_COMMENT,          Capture(r'{#.*?#}', name='text')),
-    (SNIPTYPE_HTML,             Capture(HTMLTAGOPEN, name='text')),
-    (SNIPTYPE_HTML,             Capture(HTMLTAGCLOSE, name='text')),
-    (SNIPTYPE_COMMENT,          Capture(HTMLTAGCOMMENT, name='text')),
-    (BLOCKTYPE_SUBSCRIPT,       LB_NOTSPACE + '~' + r'\(' + Capture('.*?', name='text') + r'\)' + LA_SPACE1),
-    (BLOCKTYPE_SUPERSCRIPT,     LB_NOTSPACE + '\\^' + r'\(' + Capture('.*?', name='text') + r'\)' + LA_SPACE1),
-    (BLOCKTYPE_SUPERSCRIPT,     LB_NOTSPACE + '\\^' + Capture(r'.+?', name='text') + LA_SPACE1),
-    # *DISABLED BY INTENTION*
-    #   because mid-word strikethrough is more useful
-    # (BLOCKTYPE_SUBSCRIPT,     NOTSPACE + '~' + Capture(r'\w+', name='sub') + SPACE),
+TEXTBLOCK_PATTERNS1 = (
+    (SNIPTYPE_FORMAT_UP,        LB_SPACE + Capture(Group(Or('~', '_', '=', '\\*')) + '+', name='text') + LA_NOTSPACE),
+    (SNIPTYPE_FORMAT_DOWN,      LB_NOTSPACE + Capture(Group(Or('~', '_', '=', '\\*')) + '+', name='text') + LA_SPACE),
+
+    (SNIPTYPE_FORMAT_MIDDLE,    Capture('~+', name='text')),
+
+    (SNIPTYPE_FORMAT_LEFT,      Capture(r'^<-', name='text') + LA_SPACE),
+    (SNIPTYPE_FORMAT_RIGHT,     Capture(r'^->', name='text') + LA_SPACE),
+    (SNIPTYPE_FORMAT_LEFT,      LB_SPACE + Capture(r'<-$', name='text')),
+    (SNIPTYPE_FORMAT_RIGHT,     LB_SPACE + Capture(r'->$', name='text')),
 )
-
-## these patterns relate to the formatting symbols we see co-mingled with each other
-
-comingle_char_gen   = rightdown.tokens.SpecialCharGen()
-base.Enum.Define(('COMINGLE', 'CoMingles'), (
-    {'name': 'Push Left',     'pattern': TEXT_SUB_DECORATORS[SUBMODE_SOLO](Or(r'^<-', r'<-$')), 'tag': comingle_char_gen()},
-    {'name': 'Push Right',    'pattern': TEXT_SUB_DECORATORS[SUBMODE_SOLO](Or(r'^->', r'->$')), 'tag': comingle_char_gen()},
-    {'name': 'Strike',        'pattern': TEXT_SUB_DECORATORS[SUBMODE_ALL]  ('~'),               'tag': comingle_char_gen()},
-    {'name': 'Under Up',      'pattern': TEXT_SUB_DECORATORS[SUBMODE_OPEN] ('_'),               'tag': comingle_char_gen()},
-    {'name': 'Under Down',    'pattern': TEXT_SUB_DECORATORS[SUBMODE_CLOSE]('_'),               'tag': comingle_char_gen()},
-    {'name': 'Light Up',      'pattern': TEXT_SUB_DECORATORS[SUBMODE_OPEN] ('='),               'tag': comingle_char_gen()},
-    {'name': 'Light Down',    'pattern': TEXT_SUB_DECORATORS[SUBMODE_CLOSE]('='),               'tag': comingle_char_gen()},
-    {'name': 'Star 3 Up',     'pattern': TEXT_SUB_DECORATORS[SUBMODE_OPEN] (r'\*\*\*'),         'tag': comingle_char_gen()},
-    {'name': 'Star 3 Down',   'pattern': TEXT_SUB_DECORATORS[SUBMODE_CLOSE](r'\*\*\*'),         'tag': comingle_char_gen()},
-    {'name': 'Star 2 Up',     'pattern': TEXT_SUB_DECORATORS[SUBMODE_OPEN] (r'\*\*'),           'tag': comingle_char_gen()},
-    {'name': 'Star 2 Down',   'pattern': TEXT_SUB_DECORATORS[SUBMODE_CLOSE](r'\*\*'),           'tag': comingle_char_gen()},
-    {'name': 'Star 1 Up',     'pattern': TEXT_SUB_DECORATORS[SUBMODE_OPEN] (r'\*'),             'tag': comingle_char_gen()},
-    {'name': 'Star 1 Down',   'pattern': TEXT_SUB_DECORATORS[SUBMODE_CLOSE](r'\*'),             'tag': comingle_char_gen()},
-))
-FIRST_SPECIAL_CHAR  = comingle_char_gen.AsInt()
```

### Comparing `octobase-0.9.0/base/rightdown/printers.py` & `octobase-0.9.1/base/rightdown/printers.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 #!/opt/local/bin/python
 
 import base
+import html
+
 from base                   import rightdown
+from base.regexp            import *
 from base.rightdown.enums   import *
+from base.rightdown.tokens  import *
 
 
 class Printer(base.Thing):
   ''' default options cause us to emit naked text with neither formatting nor markup '''
 
   # Copy()-ing a Printer means copying all our settings
   ATTRIBUTES        = [
@@ -35,15 +39,15 @@
   pass_comments               = False
   pass_templates              = False
 
   # should we force indented code blocks to turn into fenced code blocks?
   force_fence                 = False
 
   # should we emit blank lines between blocks?
-  double_space                = True
+  double_space                = False
 
   # How many spaces to indent nested blocks?
   block_indent                = 0
 
   # How many spaces to indent un-fenced code blocks?
   unfenced_indent             = 4
 
@@ -64,39 +68,63 @@
     if isinstance(rd, rightdown.tokens.Snip):
       imprints      = self._NormalizeImprints(rd.PrintOpen(self, None, None)) + self._NormalizeImprints(rd.PrintClose(self, None, None))
     elif isinstance(rd, rightdown.tokens.Block):
       imprints      = rd.Walk(self._WalkOpen, self._WalkClose) or []
     else:
       raise rightdown.errors.UnPrintable(rd)
 
-    if self.stop_after_stage == rightdown.enums.STAGE_IMPRINTS:
+    if self.stop_after_stage == STAGE_IMPRINTS:
       return ''.join(x.debug + '\n' for x in imprints).rstrip()
 
-    return self._MergeImprints(imprints).rstrip()
+    filtered        = self.FilterImprints(imprints)
+
+    if self.stop_after_stage == STAGE_FILTERED:
+      return ''.join(x.debug + '\n' for x in filtered).rstrip()
+
+    return self.MergeImprints(filtered).rstrip()
 
   ###
   ## callbacks
   #
 
-  def HandleToken(self, token, depth, first, last):
-    ''' allows subclasses to override the action on any token rendering '''
-
   def MuteUntilClose(self, token):
     ''' causes us to suppress all output until the given token is in the rear view mirror '''
     self._muted     = token
 
   def PrefixUntilClose(self, token, imprint):
     ''' the given imprint should precede any line of output until the given token is closing '''
     if self._stack[-1][0] != token:
       raise rightdown.errors.TreeWalkBroken(list(repr(x[0]) for x in self._stack), repr(token))
     if self._stack[-1][1]:
       raise rightdown.errors.OnePrefixPerToken(token)
     self._stack[-1] = (token, imprint)
 
   ###
+  ## child class hooks
+  #
+
+  def HandleToken(self, token, depth, first, last):
+    ''' allows subclasses to override the action on any token rendering '''
+
+  def FilterImprints(self, imprints):
+    ''' last chance to hack the imprint stream '''
+    return imprints
+
+  def MergeImprints(self, imprints):
+    ''' merge the imprints into a single string '''
+    NEWLINE         = '\n'
+    substrings      = []
+    for imprint in imprints:
+      if imprint.imprinttype == IMPRINT_BREAK:
+        substrings.append(NEWLINE)
+      if imprint.text:
+        substrings.append(imprint.text)
+    return ''.join(substrings)
+
+  ###
   ## mechanical
   #
 
   def __init__(self, **kwargs):
     base.utils.SetAttrs(self, **kwargs)
     self._muted     = None    # token
     self._stack     = []      # [ (token, prefix) ]
@@ -129,22 +157,23 @@
     # self._broken is assumed to be accurate to the point *before* our first imprint
     results           = []
     doublespace       = self.double_space and (prefixes + [breaker])
     maybies           = self._maybe and [x for x in self._maybe if x.depth <= depth]
     for imprint in imprints:
 
       # imprint is a break; pass it through, maybe double it
-      if imprint.imprinttype == rightdown.enums.IMPRINT_BREAK:
-        self._broken  = True
-        results.append(breaker)
-        if doublespace:
-          if imprint is imprints[-1] and prefixes:
-            self._maybe = prefixes
-          else:
-            results.extend(doublespace)
+      if imprint.imprinttype == IMPRINT_BREAK:
+        if not self._broken:
+          self._broken  = True
+          results.append(breaker)
+          if doublespace:
+            if imprint is imprints[-1] and prefixes:
+              self._maybe = prefixes
+            else:
+              results.extend(doublespace)
 
       # imprint is inline; we are now *not* broken
       elif imprint.inline:
         if self._broken:
           if self._maybe:
             results.extend(maybies)
             results.append(breaker)
@@ -220,62 +249,105 @@
       if self._muted == token:
         self._muted = None
       return
 
     # ask the token for its imprints
     prefixes        = self._CollectPrefixes(depth)
     imprints        = self._NormalizeImprints(token.PrintClose(self, first, last))
-    breaker         = rightdown.tokens.Imprint(IMPRINT_BREAK)
+    breaker         = Imprint(IMPRINT_BREAK)
 
     # break when exiting an inline context
     if not token.inline and self._inlining:
       self._inlining  = False
       if not self._broken:
         imprints.append(breaker)
 
     # fix up breaks
     imprints        = self._FixBreaks(imprints, breaker, prefixes, depth)
 
     return imprints or None
 
-  def _MergeImprints(self, imprints):
-    ''' merge the final list of imprints into a single string '''
-    NEWLINE         = '\n'
-    substrings      = []
-    for imprint in imprints:
-      if imprint.imprinttype == rightdown.enums.IMPRINT_BREAK:
-        substrings.append(NEWLINE)
-      if imprint.text:
-        substrings.append(imprint.text)
-    return ''.join(substrings)
-
 
 
 class TextPrinter(Printer):
   ''' this printer emits normalized rightdown text '''
 
   formatting                  = True
   metadata                    = True
   pass_html                   = True
   pass_comments               = True
   pass_templates              = True
+  double_space                = True
   _test_substitution_column   = 2
 
 
 
 class HtmlPrinter(Printer):
   ''' this printer emits HTML similar to any other markdown engine '''
 
   markup                      = True
   pass_html                   = True
   pass_templates              = True
   double_space                = False
   block_indent                = 2
   _test_substitution_column   = 3
 
+  REGEXP_CLOSING_WHITE        = Grouper(Group(r'[^\s]', grouptype=GROUPTYPE_LOOK_BEHIND) + Capture(r'\s+') + '$')
+  REGEXP_CLOSING_HTMLTAG      = Grouper(Capture(r'</\w+>'), groupermode=GROUPERMODE_START)
+
+  def FilterImprints(self, imprints):
+    imprints        = self._SwizleImprints(imprints)
+    imprints        = self._EscapeImprints(imprints)
+    return imprints
+
+  def _EscapeImprints(self, imprints):
+    for imprint in imprints:
+      if imprint.imprinttype == IMPRINT_NARRATIVE:
+        imprint.text  = html.escape(imprint.text)
+    return imprints
+
+  def _SwizleImprints(self, imprints):
+    ''' browsers do a stupid where "<i>yip </i><b>yap</b>" loses white space but "<i>yip</i> <b>yap</b>" is fine '''
+    results         = []
+    stash           = None
+    for imprint in imprints:
+      if stash and imprint.imprinttype == IMPRINT_MARKUP and stash.inline and imprint.inline:
+        remwhite    = self.REGEXP_CLOSING_WHITE(stash.text)
+        remtag      = self.REGEXP_CLOSING_HTMLTAG(imprint.text)
+        if remwhite and remtag:
+          results.extend(self._SwizleImprintsInner(stash, imprint, remwhite, remtag))
+          stash     = None
+          continue
+      if stash:
+        results.append(stash)
+      if imprint.imprinttype == IMPRINT_NARRATIVE:
+        stash       = imprint
+      else:
+        results.append(imprint)
+        stash       = None
+    if stash:
+      results.append(stash)
+    return results
+
+  def _SwizleImprintsInner(self, narrative, markup, remwhite, remtag):
+    poswhite        = remwhite.start()
+    if poswhite == 0:
+      return (narrative, markup)
+
+    white           = Imprint(IMPRINT_NARRATIVE, narrative.text[poswhite:], inline=True)
+    narrative.text  = narrative.text[:poswhite]
+
+    postag          = remtag.end()
+    if postag == len(markup.text):
+      return (narrative, markup, white)
+
+    second          = Imprint(IMPRINT_MARKUP, markup.text[postag:], inline=True)
+    markup.text     = markup.text[:postag]
+    return (narrative, markup, white, second)
+
 #   ATTRIBUTES        = Printer.ATTRIBUTES + ['dress', 'minimize']
 #
 #   # Normally we emit naked HTML, but let us know if you want <HTML>, <HEAD>, and <BODY> tags with that
 #   dress                       = False
 #
 #   # Should the HTML be compacted down to one line?
 #   minimize                    = False
@@ -299,15 +371,15 @@
   token_width                 = 24
 
   def Print(self, rd):
     ''' distills a RightDown instance to a single string '''
     return '\n'.join(rd.Walk(self._WalkOpen, self._WalkClose) or [])
 
   def _WalkOpen(self, token, depth, first, last):
-    tokensymbol     = token.tokentype.enum == rightdown.enums.LineTypes and '-' or ''
+    tokensymbol     = token.tokentype.enum == LineTypes and '-' or ''
     tokentag        = '  ' * depth + tokensymbol + token.tokentype.name
     tokentext       = token.debug
     if tokentext:
       content       = base.utils.PadString(tokentag, self.token_width) + token.debug_sep + ' ' + tokentext
     else:
       content       = tokentag
     if self.truncate_width and len(content) > self.truncate_width:
```

### Comparing `octobase-0.9.0/base/rightdown/rightdown.py` & `octobase-0.9.1/base/rightdown/rightdown.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 #!/opt/local/bin/python
 
 import base
-from base import rightdown
+
+from base                   import rightdown
+from base.rightdown.enums   import *
 
 
 class RightDown(rightdown.tokens.Block):
 
-  tokentype         = rightdown.enums.BLOCKTYPE_RIGHTDOWN
+  tokentype         = BLOCKTYPE_RIGHTDOWN
 
   metadata          = None    # dict of structured data extracted from the first document fragment
 
   children          = None    # list of fragments; collectively, the fully-parsed document tree
 
   # warnings that may be triggered during parsing (rare)
   has_illegal_chars = False   # reserved characters in input text
@@ -46,15 +48,15 @@
 
   def Html(self, **kwargs):
     ''' renders the document to a string of HTML '''
     return rightdown.printers.HtmlPrinter(**kwargs).Print(self) or ''
 
   def Links(self):
     ''' returns a list of all the Link tokens in the document '''
-    return self.All(rightdown.enums.BLOCKTYPE_LINK)
+    return self.All(BLOCKTYPE_LINK)
 
   def Save(self, filepath):
     ''' writes our normalized plain text content to the given filepath '''
     with open(filepath, 'wt') as file:
       file.write(self.Text())
 
   ###
@@ -64,10 +66,10 @@
   def __init__(self):
     self.metadata   = {}
     self.children   = []
 
   def Validate(self):
     ''' tests our structure for flaws; raises on finding any '''
     for child in self.children:
-      if not child.tokentype == rightdown.enums.BLOCKTYPE_FRAGMENT:
+      if not child.tokentype == BLOCKTYPE_FRAGMENT:
         raise rightdown.errors.InvalidChild(child)
       child.Validate()
```

### Comparing `octobase-0.9.0/base/rightdown/tests.py` & `octobase-0.9.1/base/rightdown/tests.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 #!/usr/bin/env python3
 
 import base
 import itertools
 import logging
 import os
 
-from base import rightdown
+from base                   import rightdown
+from base.rightdown.enums   import *
 
 
 ###
 ## test context and base class
 #
 
 
@@ -55,15 +56,15 @@
 
 
 class ReferenceDocumentTestCase(base.TestCase, skip=1):
   ''' common code for our tests that want to use reference files from our testdata '''
 
   COMMANDS          = ('Run', 'Compare', 'Write', 'Dump')
 
-  TEST_PRINTER      = rightdown.enums.PRINTMODE_DEBUG
+  TEST_PRINTER      = PRINTMODE_DEBUG
   TERMINUS          = None
 
   def Compare(self):
     return self.Run(command='compare')
 
   def Write(self):
     return self.Run(command='write')
@@ -161,36 +162,36 @@
     return rightdown.printers.HtmlPrinter(minimize=True).Print(rd)
 
 
 class TestParagraphs(ReferenceDocumentTestCase):
   ''' tests paragraphs and whitespace '''
 
   TEST_CONTEXT      = ReferenceDocumentContext(source='paragraphs.rd', expect='paragraphs.html')
-  TEST_PRINTER      = rightdown.enums.PRINTMODE_HTML
+  TEST_PRINTER      = PRINTMODE_HTML
 
 
 class TestFragmenting(ReferenceDocumentTestCase):
   ''' tests fragmenting, comments, and fenced code blocks '''
 
   TEST_CONTEXT      = ReferenceDocumentContext(source='fragmenting.rd', expect='fragmenting.txt')
-  TEST_PRINTER      = rightdown.enums.PRINTMODE_DEBUG
+  TEST_PRINTER      = PRINTMODE_DEBUG
 
 
 class TestSubblocks(ReferenceDocumentTestCase):
   ''' tests blocks that contain sub-blocks '''
 
   TEST_CONTEXT      = ReferenceDocumentContext(source='subblocks.rd', expect='subblocks.html')
-  TEST_PRINTER      = rightdown.enums.PRINTMODE_HTML
+  TEST_PRINTER      = PRINTMODE_HTML
 
 
 class TestInline(ReferenceDocumentTestCase):
   ''' tests inline formatting '''
 
   TEST_CONTEXT      = ReferenceDocumentContext(source='inline.rd', expect='inline.html')
-  TEST_PRINTER      = rightdown.enums.PRINTMODE_HTML
+  TEST_PRINTER      = PRINTMODE_HTML
 
 
 ###
 ## tests around extracting structured content
 #
 
 class TestMetadata(ReferenceDocumentTestCase):
@@ -222,17 +223,17 @@
 #
 
 
 class TestTokenTypes(base.TestCase):
   ''' ensures there's no overlaps between our tokentype enum tags '''
 
   def Run(self):
-    linetypes       = set(x.tag for x in rightdown.enums.LineTypes)
-    blocktypes      = set(x.tag for x in rightdown.enums.BlockTypes)
-    sniptypes       = set(x.tag for x in rightdown.enums.SnipTypes)
+    linetypes       = set(x.tag for x in LineTypes)
+    blocktypes      = set(x.tag for x in BlockTypes)
+    sniptypes       = set(x.tag for x in SnipTypes)
     overlaps        = (linetypes & blocktypes) | (blocktypes & sniptypes) | (linetypes & sniptypes)
     if overlaps:
       self.LogResult(False, 'overlapping tags: ' + ', '.join(overlaps))
     for tag in linetypes | blocktypes:
       L             = rightdown.parser.TokenList.TOKENLEN
       if len(tag) != L or tag[L-1] != ',' or ',' in tag[:L-1]:
         self.LogResult(False, 'bad tag: ' + tag)
```

### Comparing `octobase-0.9.0/base/rightdown/tokens.py` & `octobase-0.9.1/base/rightdown/tokens.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 #!/opt/local/bin/python
 
 import base
-from base import rightdown
+
+from base                   import rightdown
+from base.rightdown.enums   import *
 
 
 class Token(base.Thing):
   ''' base class for everything that ends up in the parse tree '''
 
   tokentype         = None
   text              = None      # narrative content from the document
@@ -38,15 +40,15 @@
     ''' return an Imprint or list of Imprints for this token's open text '''
 
   def PrintClose(self, printer, first, last):
     ''' return an Imprint or list of Imprints for this token's close text '''
 
   def Validate(self):
     ''' test our structure for flaws; raise on finding any '''
-    if not any(self.tokentype in x for x in (rightdown.enums.LineTypes, rightdown.enums.BlockTypes, rightdown.enums.SnipTypes)):
+    if not any(self.tokentype in x for x in (LineTypes, BlockTypes, SnipTypes)):
       raise rightdown.errors.BadTokenType(self.tokentype)
     if self.text and not self.text_after_inline:
       raise rightdown.errors.LingeringText(self, self.debug)
 
 
 ###
 ## Lines and Snips are only ever leaves of the tree
@@ -80,54 +82,90 @@
 
 
 class Snip(Token):
   ''' a fully-parsed snip of inert text '''
 
   text_after_inline = True
   inline            = True
+  snipprinter       = None
 
   def __init__(self, tokentype, **kwargs):
     self.tokentype  = tokentype
     base.utils.SetAttrs(self, **kwargs)
 
+  @property
+  def debug(self):
+    if not self.snipprinter:
+      return super().debug
+    return super().debug + ' (' + self.snipprinter.debug + ')'
+
   def ProcessText(self, parser, parenttext=None):
     return
 
-  def ToString(self, printer):
-    # this is called by text blocks to make a complete string of our contents
+  def ShouldSuppress(self, printer):
+    if self.tokentype == SNIPTYPE_COMMENT and not printer.pass_comments:
+      return True
+    if self.tokentype == SNIPTYPE_HTML and not printer.pass_html:
+      return True
+    if self.tokentype == SNIPTYPE_TEMPLATE and not printer.pass_templates:
+      return True
+
+    if self.tokentype in (
+        SNIPTYPE_FORMAT_UP,
+        SNIPTYPE_FORMAT_DOWN,
+        SNIPTYPE_FORMAT_LEFT,
+        SNIPTYPE_FORMAT_RIGHT,
+        SNIPTYPE_FORMAT_MIDDLE,
+      ) and not printer.formatting:
+      return True
+
+    return False
+
+  def Print(self, printer):
+    ''' this is called by Text blocks to render our contents.  any text we return is taken as
+        narrative.  alternately, we may return an imprint or list thereof
+    '''
+    if self.snipprinter:
+      return self.snipprinter.Print(self, printer)
 
-    if self.tokentype == rightdown.enums.SNIPTYPE_COMMENT and not printer.pass_comments:
-      return ''
-    if self.tokentype == rightdown.enums.SNIPTYPE_HTML and not printer.pass_html:
-      return ''
-    if self.tokentype == rightdown.enums.SNIPTYPE_TEMPLATE and not printer.pass_templates:
+    if self.ShouldSuppress(printer):
       return ''
 
-    if self.tokentype == rightdown.enums.SNIPTYPE_CODE:
-      return self.ToCodeString(printer)
+    if self.tokentype == SNIPTYPE_HTML:
+      return Imprint(IMPRINT_INERT, self.text, inline=True)
 
-    return self.text
+    if self.tokentype == SNIPTYPE_TEMPLATE:
+      return Imprint(IMPRINT_INERT, self.text, inline=True)
 
-  def PrintOpen(self, printer, first, last):
-    # the only sniptype this is called on is plain snips, because they are the only snips
-    # that don't live under a text block, and text always mutes through the end of itself
-    return Imprint(rightdown.enums.IMPRINT_NARRATIVE, self.text, inline=self.inline)
+    if self.tokentype == SNIPTYPE_CODE:
+      return self.PrintCode(printer)
+
+    return self.text
 
-  def ToCodeString(self, printer):
-    results         = ''
+  def PrintCode(self, printer):
+    imprints        = []
     if printer.markup:
-      results       += '<code>'
+      imprints.append(Imprint(IMPRINT_MARKUP, '<code>', inline=self.inline))
     if printer.formatting:
-      results       += '`'
-    results         += self.text
+      imprints.append(Imprint(IMPRINT_FORMATTING, '`', inline=self.inline))
+    imprints.append(Imprint(IMPRINT_NARRATIVE, self.text, inline=self.inline))
     if printer.formatting:
-      results       += '`'
+      imprints.append(Imprint(IMPRINT_FORMATTING, '`', inline=self.inline))
     if printer.markup:
-      results       += '</code>'
-    return results
+      imprints.append(Imprint(IMPRINT_MARKUP, '</code>', inline=self.inline))
+    return imprints
+
+  def PrintOpen(self, printer, first, last):
+    ''' this is called by the printer, usually only on plain snips or comment snips, because
+        they can live outside of text blocks.  most other snips only live in text blocks,
+        and text mutes its children
+    '''
+    if self.ShouldSuppress(printer):
+      return ''
+    return Imprint(IMPRINT_NARRATIVE, self.text, inline=self.inline)
 
   def Validate(self):
     super().Validate()
     if self.text:
       if SpecialCharGen.HasAnySpecialChars(self.text):
         raise rightdown.errors.SnipSubbedChars(self.text)
 
@@ -245,25 +283,25 @@
       cleantext     = SpecialCharGen.WipeSpecialChars(self.text, parser.barf_char, parser._TriggerBarf, unless)
       textblock     = parser.textmaker(cleantext, parenttext)
       self.children = [textblock] + self.children
       self.text     = None
 
     textblock       = parenttext
     for child in self.children:
-      if isinstance(child, rightdown.blocks.Text):
+      if isinstance(child, rightdown.textblock.Text):
         textblock   = child
       if isinstance(child, Block) and not child.processed:
         child.ProcessText(parser, parenttext=textblock)
 
   def Validate(self):
     ''' verify our final child list makes sense '''
     super().Validate()
     for child in self.children:
       # no longer should have any lines in the parse tree
-      if child.tokentype in rightdown.enums.LineTypes:
+      if child.tokentype in LineTypes:
         raise rightdown.errors.InvalidChild(child)
       child.Validate()
 
 
 class VerbatimBlock(Block):
   ''' shared implementation for block classes that just verbatim quote the lines they're given '''
 
@@ -274,15 +312,15 @@
   def DigestLines(self, parser):
     lines           = [x for x in list(self) if isinstance(x, Line)]
     self.children   = []
     if not lines:
       super().DigestLines(parser)
       return
     if len(lines) >= 2:
-      if lines[0].tokentype == rightdown.enums.LINETYPE_FENCE and lines[-1].tokentype == rightdown.enums.LINETYPE_FENCE:
+      if lines[0].tokentype == LINETYPE_FENCE and lines[-1].tokentype == LINETYPE_FENCE:
         self.fence  = True
         lines       = lines[1:-1]
     if lines:
       self.indent   = min(x.leading_space for x in lines)
     self.text       = '\n'.join(x.original[self.indent:].rstrip() for x in lines)
     super().DigestLines(parser)
 
@@ -365,15 +403,15 @@
     return self.ConsoleStr()
 
   @property
   def debug(self):
     typename        = self.imprinttype and self.imprinttype.name or base.utils.ClassName(self)
     text            = ''
     if self.text:
-      inline        = (self.inline and rightdown.enums.CHAR_BI_ARROW or ' ') + ' '
+      inline        = (self.inline and CHAR_BI_ARROW or ' ') + ' '
       text          = inline + self.ConsoleStr()
     if text:
       return base.utils.PadString(typename + ':', rightdown.printers.DebugPrinter.token_width) + text
     return typename
 
   def ConsoleStr(self):
     s               = self.text or ''
```

### Comparing `octobase-0.9.0/base/testing.py` & `octobase-0.9.1/base/testing.py`

 * *Files identical despite different names*

### Comparing `octobase-0.9.0/base/things.py` & `octobase-0.9.1/base/things.py`

 * *Files identical despite different names*

### Comparing `octobase-0.9.0/base/utils/decorators.py` & `octobase-0.9.1/base/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `octobase-0.9.0/base/utils/django.py` & `octobase-0.9.1/base/utils/django.py`

 * *Files identical despite different names*

### Comparing `octobase-0.9.0/base/utils/environment.py` & `octobase-0.9.1/base/utils/environment.py`

 * *Files identical despite different names*

### Comparing `octobase-0.9.0/base/utils/fuzzy.py` & `octobase-0.9.1/base/utils/fuzzy.py`

 * *Files identical despite different names*

### Comparing `octobase-0.9.0/base/utils/interactive.py` & `octobase-0.9.1/base/utils/interactive.py`

 * *Files identical despite different names*

### Comparing `octobase-0.9.0/base/utils/iterables.py` & `octobase-0.9.1/base/utils/iterables.py`

 * *Files identical despite different names*

### Comparing `octobase-0.9.0/base/utils/logging.py` & `octobase-0.9.1/base/utils/logging.py`

 * *Files identical despite different names*

### Comparing `octobase-0.9.0/base/utils/metaclasses.py` & `octobase-0.9.1/base/utils/metaclasses.py`

 * *Files identical despite different names*

### Comparing `octobase-0.9.0/base/utils/misc.py` & `octobase-0.9.1/base/utils/misc.py`

 * *Files identical despite different names*

### Comparing `octobase-0.9.0/base/utils/strings.py` & `octobase-0.9.1/base/utils/strings.py`

 * *Files identical despite different names*

### Comparing `octobase-0.9.0/base/utils/tests.py` & `octobase-0.9.1/base/utils/tests.py`

 * *Files identical despite different names*

### Comparing `octobase-0.9.0/base/utils/threadstacks.py` & `octobase-0.9.1/base/utils/threadstacks.py`

 * *Files identical despite different names*

### Comparing `octobase-0.9.0/base/utils/time.py` & `octobase-0.9.1/base/utils/time.py`

 * *Files identical despite different names*

### Comparing `octobase-0.9.0/base/whens.py` & `octobase-0.9.1/base/whens.py`

 * *Files identical despite different names*

### Comparing `octobase-0.9.0/octobase.egg-info/PKG-INFO` & `octobase-0.9.1/octobase.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: octobase
-Version: 0.9.0
+Version: 0.9.1
 Summary: The First Building Block For Any Python Project
 Home-page: https://bitbucket.org/octoboxy/octobase/
 Author: Octoboxy
 Author-email: office@octoboxy.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `octobase-0.9.0/octobase.egg-info/SOURCES.txt` & `octobase-0.9.1/octobase.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 base/rightdown/enums.py
 base/rightdown/errors.py
 base/rightdown/parser.py
 base/rightdown/patterns.py
 base/rightdown/printers.py
 base/rightdown/rightdown.py
 base/rightdown/tests.py
+base/rightdown/textblock.py
 base/rightdown/tokens.py
 base/utils/__init__.py
 base/utils/decorators.py
 base/utils/django.py
 base/utils/environment.py
 base/utils/fuzzy.py
 base/utils/interactive.py
```

### Comparing `octobase-0.9.0/setup.py` & `octobase-0.9.1/setup.py`

 * *Files identical despite different names*

