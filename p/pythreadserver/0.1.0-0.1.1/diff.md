# Comparing `tmp/pythreadserver-0.1.0.tar.gz` & `tmp/pythreadserver-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythreadserver-0.1.0.tar", last modified: Fri Apr  5 21:53:23 2024, max compression
+gzip compressed data, was "pythreadserver-0.1.1.tar", last modified: Fri Apr  5 22:02:40 2024, max compression
```

## Comparing `pythreadserver-0.1.0.tar` & `pythreadserver-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-05 21:53:23.132282 pythreadserver-0.1.0/
--rw-rw-rw-   0        0        0      524 2024-04-05 21:53:23.131281 pythreadserver-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      186 2024-04-05 13:30:40.000000 pythreadserver-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-05 21:53:23.109277 pythreadserver-0.1.0/pythreadserver/
--rw-rw-rw-   0        0        0       46 2024-04-05 20:52:10.000000 pythreadserver-0.1.0/pythreadserver/__init__.py
--rw-rw-rw-   0        0        0     3407 2024-04-05 20:40:27.000000 pythreadserver-0.1.0/pythreadserver/client.py
--rw-rw-rw-   0        0        0      141 2024-04-05 20:52:10.000000 pythreadserver-0.1.0/pythreadserver/constants.py
--rw-rw-rw-   0        0        0     5035 2024-04-05 21:06:34.000000 pythreadserver-0.1.0/pythreadserver/server.py
--rw-rw-rw-   0        0        0      465 2024-04-05 13:30:40.000000 pythreadserver-0.1.0/pythreadserver/textlog.py
-drwxrwxrwx   0        0        0        0 2024-04-05 21:53:23.130282 pythreadserver-0.1.0/pythreadserver.egg-info/
--rw-rw-rw-   0        0        0      524 2024-04-05 21:53:23.000000 pythreadserver-0.1.0/pythreadserver.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      338 2024-04-05 21:53:23.000000 pythreadserver-0.1.0/pythreadserver.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 21:53:23.000000 pythreadserver-0.1.0/pythreadserver.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-04-05 21:53:23.000000 pythreadserver-0.1.0/pythreadserver.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-04-05 21:53:23.000000 pythreadserver-0.1.0/pythreadserver.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-05 21:53:23.132282 pythreadserver-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1043 2024-04-05 21:51:36.000000 pythreadserver-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-05 22:02:40.682393 pythreadserver-0.1.1/
+-rw-rw-rw-   0        0        0      524 2024-04-05 22:02:40.681394 pythreadserver-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      186 2024-04-05 13:30:40.000000 pythreadserver-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-05 22:02:40.671391 pythreadserver-0.1.1/pythreadserver/
+-rw-rw-rw-   0        0        0       46 2024-04-05 20:52:10.000000 pythreadserver-0.1.1/pythreadserver/__init__.py
+-rw-rw-rw-   0        0        0     3407 2024-04-05 20:40:27.000000 pythreadserver-0.1.1/pythreadserver/client.py
+-rw-rw-rw-   0        0        0      141 2024-04-05 20:52:10.000000 pythreadserver-0.1.1/pythreadserver/constants.py
+-rw-rw-rw-   0        0        0     5035 2024-04-05 21:06:34.000000 pythreadserver-0.1.1/pythreadserver/server.py
+-rw-rw-rw-   0        0        0      465 2024-04-05 13:30:40.000000 pythreadserver-0.1.1/pythreadserver/textlog.py
+drwxrwxrwx   0        0        0        0 2024-04-05 22:02:40.680393 pythreadserver-0.1.1/pythreadserver.egg-info/
+-rw-rw-rw-   0        0        0      524 2024-04-05 22:02:40.000000 pythreadserver-0.1.1/pythreadserver.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      301 2024-04-05 22:02:40.000000 pythreadserver-0.1.1/pythreadserver.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 22:02:40.000000 pythreadserver-0.1.1/pythreadserver.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-04-05 22:02:40.000000 pythreadserver-0.1.1/pythreadserver.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-05 22:02:40.682393 pythreadserver-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      996 2024-04-05 22:02:31.000000 pythreadserver-0.1.1/setup.py
```

### Comparing `pythreadserver-0.1.0/PKG-INFO` & `pythreadserver-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythreadserver
-Version: 0.1.0
+Version: 0.1.1
 Summary: Simple multi-threaded server package
 Author: rain-1107
 Author-email: 
 Keywords: python,server,network,multi-threaded,sockets
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pythreadserver-0.1.0/pythreadserver/client.py` & `pythreadserver-0.1.1/pythreadserver/client.py`

 * *Files identical despite different names*

### Comparing `pythreadserver-0.1.0/pythreadserver/server.py` & `pythreadserver-0.1.1/pythreadserver/server.py`

 * *Files identical despite different names*

### Comparing `pythreadserver-0.1.0/pythreadserver.egg-info/PKG-INFO` & `pythreadserver-0.1.1/pythreadserver.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythreadserver
-Version: 0.1.0
+Version: 0.1.1
 Summary: Simple multi-threaded server package
 Author: rain-1107
 Author-email: 
 Keywords: python,server,network,multi-threaded,sockets
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pythreadserver-0.1.0/setup.py` & `pythreadserver-0.1.1/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,29 +3,28 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.1.0'
+VERSION = '0.1.1'
 DESCRIPTION = 'Simple multi-threaded server package'
 LONG_DESCRIPTION = ''
 
 # Setting up
 setup(
     name="pythreadserver",
     version=VERSION,
     author="rain-1107",
     author_email="",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=LONG_DESCRIPTION,
     packages=find_packages(),
-    install_requires=['threading', 'socket'],
     keywords=['python', 'server', 'network', 'multi-threaded', 'sockets'],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
```

