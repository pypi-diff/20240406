# Comparing `tmp/install-preserve-0.0.1.tar.gz` & `tmp/install-preserve-0.0.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "install-preserve-0.0.1.tar", last modified: Sat Apr  6 18:29:21 2024, max compression
+gzip compressed data, was "install-preserve-0.0.11.tar", last modified: Sat Apr  6 18:50:55 2024, max compression
```

## Comparing `install-preserve-0.0.1.tar` & `install-preserve-0.0.11.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:29:21.113463 install-preserve-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-06 18:29:14.000000 install-preserve-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-04-06 18:29:21.113463 install-preserve-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-04-06 18:29:14.000000 install-preserve-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:29:21.113463 install-preserve-0.0.1/install_preserve/
--rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-04-06 18:29:14.000000 install-preserve-0.0.1/install_preserve/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:29:21.113463 install-preserve-0.0.1/install_preserve.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-04-06 18:29:21.000000 install-preserve-0.0.1/install_preserve.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-06 18:29:21.000000 install-preserve-0.0.1/install_preserve.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 18:29:21.000000 install-preserve-0.0.1/install_preserve.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-06 18:29:21.000000 install-preserve-0.0.1/install_preserve.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 18:29:21.113463 install-preserve-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-06 18:29:14.000000 install-preserve-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:50:55.233461 install-preserve-0.0.11/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-06 18:50:52.000000 install-preserve-0.0.11/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-04-06 18:50:55.233461 install-preserve-0.0.11/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-04-06 18:50:52.000000 install-preserve-0.0.11/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:50:55.233461 install-preserve-0.0.11/install_preserve/
+-rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-04-06 18:50:52.000000 install-preserve-0.0.11/install_preserve/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:50:55.233461 install-preserve-0.0.11/install_preserve.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-04-06 18:50:55.000000 install-preserve-0.0.11/install_preserve.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-06 18:50:55.000000 install-preserve-0.0.11/install_preserve.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 18:50:55.000000 install-preserve-0.0.11/install_preserve.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-06 18:50:55.000000 install-preserve-0.0.11/install_preserve.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 18:50:55.233461 install-preserve-0.0.11/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-06 18:50:52.000000 install-preserve-0.0.11/setup.py
```

### Comparing `install-preserve-0.0.1/LICENSE` & `install-preserve-0.0.11/LICENSE`

 * *Files identical despite different names*

### Comparing `install-preserve-0.0.1/PKG-INFO` & `install-preserve-0.0.11/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: install-preserve
-Version: 0.0.1
+Version: 0.0.11
 Summary: A Python library that helps prevent accidental overwrites of hand-compiled libraries
 Home-page: https://github.com/manbehindthemadness/install-preserve
 Author: Manbehindthemadness
 Author-email: manbehindthemadness@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `install-preserve-0.0.1/README.md` & `install-preserve-0.0.11/README.md`

 * *Files identical despite different names*

### Comparing `install-preserve-0.0.1/install_preserve/__init__.py` & `install-preserve-0.0.11/install_preserve/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 """
 Lets init some stuff!
 """
-import importlib.util  # noqa
+import re
+import importlib.util
 
 
 def preserve(requirements: list[str], criteria: list[str], verbose: bool = False) -> list:
     """
     Preserve packages listed in the criteria argument if they are already installed.
     """
     package_names = list()
     for requirement in requirements:
-        package_names.append(requirement.split('=')[0])
+        package_names.append(re.sub(r'[^a-zA-Z0-9]+$', '', requirement.split('=')[0]))
     for item in criteria:
         alias = name = item
         if ':' in item:
             name, alias = item.split(':')
         if importlib.util.find_spec(alias) is not None:
             if verbose:
                 print(f'excluding package {name} as it is already installed')
@@ -40,16 +41,16 @@
         'pandas',
         'albumentations==0.5.2',
         'hydra-core==1.1.0',
         'tabulate',
         'webdataset',
         'packaging',
         'wldhx.yadisk-direct',
-        'opencv-python',
-        'pytorch==2.0.0'
+        'opencv-python>=3.4.2.17',
+        'pytorch>=2.0.0'
     ]
 
     excludes = [
         'tqdm',
         'opencv-python:cv2',
         'pytorch:torch'
     ]
```

### Comparing `install-preserve-0.0.1/install_preserve.egg-info/PKG-INFO` & `install-preserve-0.0.11/install_preserve.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: install-preserve
-Version: 0.0.1
+Version: 0.0.11
 Summary: A Python library that helps prevent accidental overwrites of hand-compiled libraries
 Home-page: https://github.com/manbehindthemadness/install-preserve
 Author: Manbehindthemadness
 Author-email: manbehindthemadness@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `install-preserve-0.0.1/setup.py` & `install-preserve-0.0.11/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setup(
     name='install-preserve',
-    version='0.0.1',
+    version='0.0.11',
     packages=find_packages(),
     entry_points={
         'console_scripts': [
         ],
     },
     author='Manbehindthemadness',
     author_email='manbehindthemadness@gmail.com',
```

