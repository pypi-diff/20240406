# Comparing `tmp/pulsectl-23.5.2.tar.gz` & `tmp/pulsectl-24.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulsectl-23.5.2.tar", last modified: Mon May 22 20:49:27 2023, max compression
+gzip compressed data, was "pulsectl-24.4.0.tar", last modified: Sat Apr  6 14:06:38 2024, max compression
```

## Comparing `pulsectl-23.5.2.tar` & `pulsectl-24.4.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 fraggod   (1000) fraggod   (1000)        0 2023-05-22 20:49:27.479202 pulsectl-23.5.2/
--rw-r--r--   0 fraggod   (1000) fraggod   (1000)     2179 2023-05-22 20:48:38.000000 pulsectl-23.5.2/CHANGES.rst
--rw-r--r--   0 fraggod   (1000) fraggod   (1000)     1123 2017-07-13 10:23:26.000000 pulsectl-23.5.2/COPYING
--rw-r--r--   0 fraggod   (1000) fraggod   (1000)       39 2021-02-25 10:54:47.000000 pulsectl-23.5.2/MANIFEST.in
--rw-r--r--   0 fraggod   (1000) fraggod   (1000)    17416 2023-05-22 20:49:27.479202 pulsectl-23.5.2/PKG-INFO
--rw-r--r--   0 fraggod   (1000) fraggod   (1000)    16561 2023-05-05 23:05:28.000000 pulsectl-23.5.2/README.rst
-drwxr-xr-x   0 fraggod   (1000) fraggod   (1000)        0 2023-05-22 20:49:27.478202 pulsectl-23.5.2/pulsectl/
--rw-r--r--   0 fraggod   (1000) fraggod   (1000)      665 2022-01-22 20:05:43.000000 pulsectl-23.5.2/pulsectl/__init__.py
--rw-r--r--   0 fraggod   (1000) fraggod   (1000)    22570 2023-05-22 20:45:39.000000 pulsectl-23.5.2/pulsectl/_pulsectl.py
--rw-r--r--   0 fraggod   (1000) fraggod   (1000)     4385 2018-04-23 16:48:50.000000 pulsectl-23.5.2/pulsectl/lookup.py
--rw-r--r--   0 fraggod   (1000) fraggod   (1000)    41085 2023-05-05 23:00:23.000000 pulsectl-23.5.2/pulsectl/pulsectl.py
-drwxr-xr-x   0 fraggod   (1000) fraggod   (1000)        0 2023-05-22 20:49:27.479202 pulsectl-23.5.2/pulsectl/tests/
--rw-r--r--   0 fraggod   (1000) fraggod   (1000)        0 2017-07-13 10:23:26.000000 pulsectl-23.5.2/pulsectl/tests/__init__.py
--rw-r--r--   0 fraggod   (1000) fraggod   (1000)    25645 2022-04-09 14:42:09.000000 pulsectl-23.5.2/pulsectl/tests/test_with_dummy_instance.py
-drwxr-xr-x   0 fraggod   (1000) fraggod   (1000)        0 2023-05-22 20:49:27.478202 pulsectl-23.5.2/pulsectl.egg-info/
--rw-r--r--   0 fraggod   (1000) fraggod   (1000)    17416 2023-05-22 20:49:27.000000 pulsectl-23.5.2/pulsectl.egg-info/PKG-INFO
--rw-r--r--   0 fraggod   (1000) fraggod   (1000)      342 2023-05-22 20:49:27.000000 pulsectl-23.5.2/pulsectl.egg-info/SOURCES.txt
--rw-r--r--   0 fraggod   (1000) fraggod   (1000)        1 2023-05-22 20:49:27.000000 pulsectl-23.5.2/pulsectl.egg-info/dependency_links.txt
--rw-r--r--   0 fraggod   (1000) fraggod   (1000)        9 2023-05-22 20:49:27.000000 pulsectl-23.5.2/pulsectl.egg-info/top_level.txt
--rw-r--r--   0 fraggod   (1000) fraggod   (1000)       67 2023-05-22 20:49:27.479202 pulsectl-23.5.2/setup.cfg
--rw-------   0 fraggod   (1000) fraggod   (1000)     1247 2023-05-22 20:48:14.000000 pulsectl-23.5.2/setup.py
+drwxr-xr-x   0 fraggod   (1000) fraggod   (1000)        0 2024-04-06 14:06:38.397456 pulsectl-24.4.0/
+-rw-r--r--   0 fraggod   (1000) fraggod   (1000)     2179 2023-05-22 20:48:38.000000 pulsectl-24.4.0/CHANGES.rst
+-rw-r--r--   0 fraggod   (1000) fraggod   (1000)     1123 2017-07-13 10:23:26.000000 pulsectl-24.4.0/COPYING
+-rw-r--r--   0 fraggod   (1000) fraggod   (1000)       39 2021-02-25 10:54:47.000000 pulsectl-24.4.0/MANIFEST.in
+-rw-r--r--   0 fraggod   (1000) fraggod   (1000)    17416 2024-04-06 14:06:38.397456 pulsectl-24.4.0/PKG-INFO
+-rw-r--r--   0 fraggod   (1000) fraggod   (1000)    16561 2023-05-05 23:05:28.000000 pulsectl-24.4.0/README.rst
+drwxr-xr-x   0 fraggod   (1000) fraggod   (1000)        0 2024-04-06 14:06:38.396456 pulsectl-24.4.0/pulsectl/
+-rw-r--r--   0 fraggod   (1000) fraggod   (1000)      665 2022-01-22 20:05:43.000000 pulsectl-24.4.0/pulsectl/__init__.py
+-rw-r--r--   0 fraggod   (1000) fraggod   (1000)    22570 2024-04-06 13:49:19.000000 pulsectl-24.4.0/pulsectl/_pulsectl.py
+-rw-r--r--   0 fraggod   (1000) fraggod   (1000)     4385 2018-04-23 16:48:50.000000 pulsectl-24.4.0/pulsectl/lookup.py
+-rw-r--r--   0 fraggod   (1000) fraggod   (1000)    41446 2024-04-06 14:03:03.000000 pulsectl-24.4.0/pulsectl/pulsectl.py
+drwxr-xr-x   0 fraggod   (1000) fraggod   (1000)        0 2024-04-06 14:06:38.397456 pulsectl-24.4.0/pulsectl/tests/
+-rw-r--r--   0 fraggod   (1000) fraggod   (1000)        0 2017-07-13 10:23:26.000000 pulsectl-24.4.0/pulsectl/tests/__init__.py
+-rw-r--r--   0 fraggod   (1000) fraggod   (1000)    25645 2022-04-09 14:42:09.000000 pulsectl-24.4.0/pulsectl/tests/test_with_dummy_instance.py
+drwxr-xr-x   0 fraggod   (1000) fraggod   (1000)        0 2024-04-06 14:06:38.397456 pulsectl-24.4.0/pulsectl.egg-info/
+-rw-r--r--   0 fraggod   (1000) fraggod   (1000)    17416 2024-04-06 14:06:38.000000 pulsectl-24.4.0/pulsectl.egg-info/PKG-INFO
+-rw-r--r--   0 fraggod   (1000) fraggod   (1000)      342 2024-04-06 14:06:38.000000 pulsectl-24.4.0/pulsectl.egg-info/SOURCES.txt
+-rw-r--r--   0 fraggod   (1000) fraggod   (1000)        1 2024-04-06 14:06:38.000000 pulsectl-24.4.0/pulsectl.egg-info/dependency_links.txt
+-rw-r--r--   0 fraggod   (1000) fraggod   (1000)        9 2024-04-06 14:06:38.000000 pulsectl-24.4.0/pulsectl.egg-info/top_level.txt
+-rw-r--r--   0 fraggod   (1000) fraggod   (1000)       67 2024-04-06 14:06:38.397456 pulsectl-24.4.0/setup.cfg
+-rw-------   0 fraggod   (1000) fraggod   (1000)     1198 2024-04-06 14:05:56.000000 pulsectl-24.4.0/setup.py
```

### Comparing `pulsectl-23.5.2/CHANGES.rst` & `pulsectl-24.4.0/CHANGES.rst`

 * *Files identical despite different names*

### Comparing `pulsectl-23.5.2/COPYING` & `pulsectl-24.4.0/COPYING`

 * *Files identical despite different names*

### Comparing `pulsectl-23.5.2/PKG-INFO` & `pulsectl-24.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulsectl
-Version: 23.5.2
+Version: 24.4.0
 Summary: Python high-level interface and ctypes-based bindings for PulseAudio (libpulse)
 Home-page: http://github.com/mk-fg/python-pulse-control
 Author: George Filipkin, Mike Kazantsev
 Author-email: mk.fraggod@gmail.com
 License: MIT
 Keywords: pulseaudio,libpulse,pulse,pa,bindings,sound,audio,ctypes,control,mixer,volume,mute,source,sink
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pulsectl-23.5.2/README.rst` & `pulsectl-24.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `pulsectl-23.5.2/pulsectl/__init__.py` & `pulsectl-24.4.0/pulsectl/__init__.py`

 * *Files identical despite different names*

### Comparing `pulsectl-23.5.2/pulsectl/_pulsectl.py` & `pulsectl-24.4.0/pulsectl/_pulsectl.py`

 * *Files identical despite different names*

### Comparing `pulsectl-23.5.2/pulsectl/lookup.py` & `pulsectl-24.4.0/pulsectl/lookup.py`

 * *Files identical despite different names*

### Comparing `pulsectl-23.5.2/pulsectl/pulsectl.py` & `pulsectl-24.4.0/pulsectl/pulsectl.py`

 * *Files 1% similar despite different names*

```diff
@@ -748,14 +748,21 @@
 		assert_pulse_object(obj)
 		method = {
 			PulseSinkInfo: self.sink_default_set,
 			PulseSourceInfo: self.source_default_set }.get(type(obj))
 		if not method: raise NotImplementedError(type(obj))
 		method(obj)
 
+	def sink_default_get(self):
+		'Wrapper around server_info() to return sink for default_sink_name there.'
+		return self.get_sink_by_name(self.server_info().default_sink_name)
+	def source_default_get(self):
+		'Wrapper around server_info() to return source for default_source_name there.'
+		return self.get_source_by_name(self.server_info().default_source_name)
+
 	def mute(self, obj, mute=True):
 		assert_pulse_object(obj)
 		method = {
 			PulseSinkInfo: self.sink_mute,
 			PulseSinkInputInfo: self.sink_input_mute,
 			PulseSourceInfo: self.source_mute,
 			PulseSourceOutputInfo: self.source_output_mute }.get(type(obj))
```

### Comparing `pulsectl-23.5.2/pulsectl/tests/test_with_dummy_instance.py` & `pulsectl-24.4.0/pulsectl/tests/test_with_dummy_instance.py`

 * *Files identical despite different names*

### Comparing `pulsectl-23.5.2/pulsectl.egg-info/PKG-INFO` & `pulsectl-24.4.0/pulsectl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulsectl
-Version: 23.5.2
+Version: 24.4.0
 Summary: Python high-level interface and ctypes-based bindings for PulseAudio (libpulse)
 Home-page: http://github.com/mk-fg/python-pulse-control
 Author: George Filipkin, Mike Kazantsev
 Author-email: mk.fraggod@gmail.com
 License: MIT
 Keywords: pulseaudio,libpulse,pulse,pa,bindings,sound,audio,ctypes,control,mixer,volume,mute,source,sink
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pulsectl-23.5.2/setup.py` & `pulsectl-24.4.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,25 @@
-#!/usr/bin/env python2
-#-*- coding: utf-8 -*-
-
 from setuptools import setup, find_packages
 import os, sys
 
 # Error-handling here is to allow package to be built w/o README included
 try:
 	readme = open(os.path.join(
 		os.path.dirname(__file__), 'README.rst' )).read()
 except IOError: readme = ''
 
 setup(
 
 	name = 'pulsectl',
-	version = '23.5.2',
+	version = '24.4.0',
 	author = 'George Filipkin, Mike Kazantsev',
 	author_email = 'mk.fraggod@gmail.com',
 	license = 'MIT',
 	keywords = [
-		'pulseaudio', 'libpulse', 'pulse', 'pa', 'bindings',
-		'sound', 'audio',
+		'pulseaudio', 'libpulse', 'pulse', 'pa', 'bindings', 'sound', 'audio',
 		'ctypes', 'control', 'mixer', 'volume', 'mute', 'source', 'sink' ],
 
 	url = 'http://github.com/mk-fg/python-pulse-control',
 
 	description = 'Python high-level interface'
 		' and ctypes-based bindings for PulseAudio (libpulse)',
 	long_description = readme,
```

