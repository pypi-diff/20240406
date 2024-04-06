# Comparing `tmp/pyvidplayer2-0.9.8.tar.gz` & `tmp/pyvidplayer2-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyvidplayer2-0.9.8.tar", last modified: Thu Aug 24 03:26:42 2023, max compression
+gzip compressed data, was "pyvidplayer2-0.9.9.tar", last modified: Thu Aug 24 03:30:32 2023, max compression
```

## Comparing `pyvidplayer2-0.9.8.tar` & `pyvidplayer2-0.9.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-08-24 03:26:42.532276 pyvidplayer2-0.9.8/
--rw-rw-rw-   0        0        0     1085 2023-07-19 21:30:21.000000 pyvidplayer2-0.9.8/LICENSE
--rw-rw-rw-   0        0        0     2844 2023-08-24 03:26:42.532276 pyvidplayer2-0.9.8/PKG-INFO
--rw-rw-rw-   0        0        0     2511 2023-08-24 03:18:39.000000 pyvidplayer2-0.9.8/README.md
-drwxrwxrwx   0        0        0        0 2023-08-24 03:26:42.518768 pyvidplayer2-0.9.8/pyvidplayer2/
--rw-rw-rw-   0        0        0     1074 2023-08-24 03:19:03.000000 pyvidplayer2-0.9.8/pyvidplayer2/__init__.py
--rw-rw-rw-   0        0        0       47 2023-08-20 01:10:59.000000 pyvidplayer2-0.9.8/pyvidplayer2/error.py
--rw-rw-rw-   0        0        0     1220 2023-08-19 22:50:44.000000 pyvidplayer2-0.9.8/pyvidplayer2/mixer_handler.py
--rw-rw-rw-   0        0        0     1339 2023-07-30 13:44:08.000000 pyvidplayer2-0.9.8/pyvidplayer2/post_processing.py
--rw-rw-rw-   0        0        0     2957 2023-08-19 22:50:44.000000 pyvidplayer2-0.9.8/pyvidplayer2/pyaudio_handler.py
--rw-rw-rw-   0        0        0     2459 2023-08-19 22:50:44.000000 pyvidplayer2-0.9.8/pyvidplayer2/subtitles.py
--rw-rw-rw-   0        0        0     8750 2023-08-22 02:28:02.000000 pyvidplayer2-0.9.8/pyvidplayer2/video.py
--rw-rw-rw-   0        0        0    10550 2023-08-19 22:50:44.000000 pyvidplayer2-0.9.8/pyvidplayer2/video_player.py
--rw-rw-rw-   0        0        0     1347 2023-08-20 00:54:18.000000 pyvidplayer2-0.9.8/pyvidplayer2/video_pygame.py
--rw-rw-rw-   0        0        0     1540 2023-08-19 22:50:44.000000 pyvidplayer2-0.9.8/pyvidplayer2/video_pyglet.py
--rw-rw-rw-   0        0        0     1690 2023-08-05 01:14:06.000000 pyvidplayer2-0.9.8/pyvidplayer2/video_pyqt.py
--rw-rw-rw-   0        0        0     1528 2023-08-05 01:14:06.000000 pyvidplayer2-0.9.8/pyvidplayer2/video_tkinter.py
--rw-rw-rw-   0        0        0     3380 2023-08-20 01:11:08.000000 pyvidplayer2-0.9.8/pyvidplayer2/webcam.py
-drwxrwxrwx   0        0        0        0 2023-08-24 03:26:42.531276 pyvidplayer2-0.9.8/pyvidplayer2.egg-info/
--rw-rw-rw-   0        0        0     2844 2023-08-24 03:26:42.000000 pyvidplayer2-0.9.8/pyvidplayer2.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      561 2023-08-24 03:26:42.000000 pyvidplayer2-0.9.8/pyvidplayer2.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-24 03:26:42.000000 pyvidplayer2-0.9.8/pyvidplayer2.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-08-24 03:26:42.000000 pyvidplayer2-0.9.8/pyvidplayer2.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-08-24 03:26:42.000000 pyvidplayer2-0.9.8/pyvidplayer2.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-24 03:26:42.533277 pyvidplayer2-0.9.8/setup.cfg
--rw-rw-rw-   0        0        0      742 2023-08-24 03:25:10.000000 pyvidplayer2-0.9.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-24 03:30:32.461729 pyvidplayer2-0.9.9/
+-rw-rw-rw-   0        0        0     1085 2023-07-19 21:30:21.000000 pyvidplayer2-0.9.9/LICENSE
+-rw-rw-rw-   0        0        0     2844 2023-08-24 03:30:32.461729 pyvidplayer2-0.9.9/PKG-INFO
+-rw-rw-rw-   0        0        0     2511 2023-08-24 03:18:39.000000 pyvidplayer2-0.9.9/README.md
+drwxrwxrwx   0        0        0        0 2023-08-24 03:30:32.449717 pyvidplayer2-0.9.9/pyvidplayer2/
+-rw-rw-rw-   0        0        0     1065 2023-08-24 03:30:14.000000 pyvidplayer2-0.9.9/pyvidplayer2/__init__.py
+-rw-rw-rw-   0        0        0       47 2023-08-20 01:10:59.000000 pyvidplayer2-0.9.9/pyvidplayer2/error.py
+-rw-rw-rw-   0        0        0     1220 2023-08-19 22:50:44.000000 pyvidplayer2-0.9.9/pyvidplayer2/mixer_handler.py
+-rw-rw-rw-   0        0        0     1339 2023-07-30 13:44:08.000000 pyvidplayer2-0.9.9/pyvidplayer2/post_processing.py
+-rw-rw-rw-   0        0        0     2957 2023-08-19 22:50:44.000000 pyvidplayer2-0.9.9/pyvidplayer2/pyaudio_handler.py
+-rw-rw-rw-   0        0        0     2459 2023-08-19 22:50:44.000000 pyvidplayer2-0.9.9/pyvidplayer2/subtitles.py
+-rw-rw-rw-   0        0        0     8750 2023-08-22 02:28:02.000000 pyvidplayer2-0.9.9/pyvidplayer2/video.py
+-rw-rw-rw-   0        0        0    10550 2023-08-19 22:50:44.000000 pyvidplayer2-0.9.9/pyvidplayer2/video_player.py
+-rw-rw-rw-   0        0        0     1347 2023-08-20 00:54:18.000000 pyvidplayer2-0.9.9/pyvidplayer2/video_pygame.py
+-rw-rw-rw-   0        0        0     1540 2023-08-19 22:50:44.000000 pyvidplayer2-0.9.9/pyvidplayer2/video_pyglet.py
+-rw-rw-rw-   0        0        0     1690 2023-08-05 01:14:06.000000 pyvidplayer2-0.9.9/pyvidplayer2/video_pyqt.py
+-rw-rw-rw-   0        0        0     1528 2023-08-05 01:14:06.000000 pyvidplayer2-0.9.9/pyvidplayer2/video_tkinter.py
+-rw-rw-rw-   0        0        0     3380 2023-08-20 01:11:08.000000 pyvidplayer2-0.9.9/pyvidplayer2/webcam.py
+drwxrwxrwx   0        0        0        0 2023-08-24 03:30:32.460729 pyvidplayer2-0.9.9/pyvidplayer2.egg-info/
+-rw-rw-rw-   0        0        0     2844 2023-08-24 03:30:32.000000 pyvidplayer2-0.9.9/pyvidplayer2.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      561 2023-08-24 03:30:32.000000 pyvidplayer2-0.9.9/pyvidplayer2.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-24 03:30:32.000000 pyvidplayer2-0.9.9/pyvidplayer2.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-08-24 03:30:32.000000 pyvidplayer2-0.9.9/pyvidplayer2.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-08-24 03:30:32.000000 pyvidplayer2-0.9.9/pyvidplayer2.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-24 03:30:32.462729 pyvidplayer2-0.9.9/setup.cfg
+-rw-rw-rw-   0        0        0      742 2023-08-24 03:25:10.000000 pyvidplayer2-0.9.9/setup.py
```

### Comparing `pyvidplayer2-0.9.8/LICENSE` & `pyvidplayer2-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyvidplayer2-0.9.8/PKG-INFO` & `pyvidplayer2-0.9.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvidplayer2
-Version: 0.9.8
+Version: 0.9.9
 Summary: Video playback in Python
 Home-page: https://github.com/ree1261/pyvidplayer2
 Author: Anray Liu
 Author-email: anrayliu@gmail.com
 License: MIT
 Keywords: pygame,video,playback
 Platform: windows
```

### Comparing `pyvidplayer2-0.9.8/README.md` & `pyvidplayer2-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `pyvidplayer2-0.9.8/pyvidplayer2/__init__.py` & `pyvidplayer2-0.9.9/pyvidplayer2/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import subprocess 
 
 from .post_processing import PostProcessing 
-from .video_tkinter import VideoTkinter as Video
+from .video_tkinter import VideoTkinter
 
 try:
     import PyQt6
 except ImportError:
     pass 
 else:
     from .video_pyqt import VideoPyQT
@@ -26,15 +26,15 @@
     import pyglet
 except ImportError:
     pass 
 else:
     from .video_pyglet import VideoPyglet
 
 
-_VERSION = "0.9.8"
+_VERSION = "0.9.9"
 
 
 def get_version_info() -> dict:
     try:
         pygame_ver = pygame.version.ver
     except NameError:
         pygame_ver = "not installed"
```

### Comparing `pyvidplayer2-0.9.8/pyvidplayer2/mixer_handler.py` & `pyvidplayer2-0.9.9/pyvidplayer2/mixer_handler.py`

 * *Files identical despite different names*

### Comparing `pyvidplayer2-0.9.8/pyvidplayer2/post_processing.py` & `pyvidplayer2-0.9.9/pyvidplayer2/post_processing.py`

 * *Files identical despite different names*

### Comparing `pyvidplayer2-0.9.8/pyvidplayer2/pyaudio_handler.py` & `pyvidplayer2-0.9.9/pyvidplayer2/pyaudio_handler.py`

 * *Files identical despite different names*

### Comparing `pyvidplayer2-0.9.8/pyvidplayer2/subtitles.py` & `pyvidplayer2-0.9.9/pyvidplayer2/subtitles.py`

 * *Files identical despite different names*

### Comparing `pyvidplayer2-0.9.8/pyvidplayer2/video.py` & `pyvidplayer2-0.9.9/pyvidplayer2/video.py`

 * *Files identical despite different names*

### Comparing `pyvidplayer2-0.9.8/pyvidplayer2/video_player.py` & `pyvidplayer2-0.9.9/pyvidplayer2/video_player.py`

 * *Files identical despite different names*

### Comparing `pyvidplayer2-0.9.8/pyvidplayer2/video_pygame.py` & `pyvidplayer2-0.9.9/pyvidplayer2/video_pygame.py`

 * *Files identical despite different names*

### Comparing `pyvidplayer2-0.9.8/pyvidplayer2/video_pyglet.py` & `pyvidplayer2-0.9.9/pyvidplayer2/video_pyglet.py`

 * *Files identical despite different names*

### Comparing `pyvidplayer2-0.9.8/pyvidplayer2/video_pyqt.py` & `pyvidplayer2-0.9.9/pyvidplayer2/video_pyqt.py`

 * *Files identical despite different names*

### Comparing `pyvidplayer2-0.9.8/pyvidplayer2/video_tkinter.py` & `pyvidplayer2-0.9.9/pyvidplayer2/video_tkinter.py`

 * *Files identical despite different names*

### Comparing `pyvidplayer2-0.9.8/pyvidplayer2/webcam.py` & `pyvidplayer2-0.9.9/pyvidplayer2/webcam.py`

 * *Files identical despite different names*

### Comparing `pyvidplayer2-0.9.8/pyvidplayer2.egg-info/PKG-INFO` & `pyvidplayer2-0.9.9/pyvidplayer2.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvidplayer2
-Version: 0.9.8
+Version: 0.9.9
 Summary: Video playback in Python
 Home-page: https://github.com/ree1261/pyvidplayer2
 Author: Anray Liu
 Author-email: anrayliu@gmail.com
 License: MIT
 Keywords: pygame,video,playback
 Platform: windows
```

### Comparing `pyvidplayer2-0.9.8/pyvidplayer2.egg-info/SOURCES.txt` & `pyvidplayer2-0.9.9/pyvidplayer2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyvidplayer2-0.9.8/setup.py` & `pyvidplayer2-0.9.9/setup.py`

 * *Files identical despite different names*

