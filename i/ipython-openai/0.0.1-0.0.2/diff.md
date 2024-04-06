# Comparing `tmp/ipython_openai-0.0.1.tar.gz` & `tmp/ipython_openai-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipython_openai-0.0.1.tar", last modified: Fri Apr  5 23:24:37 2024, max compression
+gzip compressed data, was "ipython_openai-0.0.2.tar", last modified: Sat Apr  6 00:13:54 2024, max compression
```

## Comparing `ipython_openai-0.0.1.tar` & `ipython_openai-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 jordan     (501) staff       (20)        0 2024-04-05 23:24:37.533366 ipython_openai-0.0.1/
--rw-r--r--   0 jordan     (501) staff       (20)     1060 2024-04-05 22:49:53.000000 ipython_openai-0.0.1/LICENSE
--rw-r--r--   0 jordan     (501) staff       (20)     1875 2024-04-05 23:24:37.533261 ipython_openai-0.0.1/PKG-INFO
-drwxr-xr-x   0 jordan     (501) staff       (20)        0 2024-04-05 23:24:37.532491 ipython_openai-0.0.1/ipython_openai/
--rw-r--r--   0 jordan     (501) staff       (20)      116 2024-04-05 20:25:04.000000 ipython_openai-0.0.1/ipython_openai/__init__.py
--rw-r--r--   0 jordan     (501) staff       (20)     3860 2024-04-05 22:04:38.000000 ipython_openai-0.0.1/ipython_openai/gpt.py
-drwxr-xr-x   0 jordan     (501) staff       (20)        0 2024-04-05 23:24:37.533127 ipython_openai-0.0.1/ipython_openai.egg-info/
--rw-r--r--   0 jordan     (501) staff       (20)     1875 2024-04-05 23:24:37.000000 ipython_openai-0.0.1/ipython_openai.egg-info/PKG-INFO
--rw-r--r--   0 jordan     (501) staff       (20)      295 2024-04-05 23:24:37.000000 ipython_openai-0.0.1/ipython_openai.egg-info/SOURCES.txt
--rw-r--r--   0 jordan     (501) staff       (20)        1 2024-04-05 23:24:37.000000 ipython_openai-0.0.1/ipython_openai.egg-info/dependency_links.txt
--rw-r--r--   0 jordan     (501) staff       (20)       77 2024-04-05 23:24:37.000000 ipython_openai-0.0.1/ipython_openai.egg-info/entry_points.txt
--rw-r--r--   0 jordan     (501) staff       (20)       13 2024-04-05 23:24:37.000000 ipython_openai-0.0.1/ipython_openai.egg-info/requires.txt
--rw-r--r--   0 jordan     (501) staff       (20)       15 2024-04-05 23:24:37.000000 ipython_openai-0.0.1/ipython_openai.egg-info/top_level.txt
--rw-r--r--   0 jordan     (501) staff       (20)       38 2024-04-05 23:24:37.533399 ipython_openai-0.0.1/setup.cfg
--rw-r--r--   0 jordan     (501) staff       (20)      859 2024-04-05 23:18:49.000000 ipython_openai-0.0.1/setup.py
+drwxr-xr-x   0 jordan     (501) staff       (20)        0 2024-04-06 00:13:54.768849 ipython_openai-0.0.2/
+-rw-r--r--   0 jordan     (501) staff       (20)     1060 2024-04-05 22:49:53.000000 ipython_openai-0.0.2/LICENSE
+-rw-r--r--   0 jordan     (501) staff       (20)     1875 2024-04-06 00:13:54.768738 ipython_openai-0.0.2/PKG-INFO
+drwxr-xr-x   0 jordan     (501) staff       (20)        0 2024-04-06 00:13:54.767824 ipython_openai-0.0.2/ipython_openai/
+-rw-r--r--   0 jordan     (501) staff       (20)      116 2024-04-05 20:25:04.000000 ipython_openai-0.0.2/ipython_openai/__init__.py
+-rw-r--r--   0 jordan     (501) staff       (20)     3860 2024-04-05 22:04:38.000000 ipython_openai-0.0.2/ipython_openai/gpt.py
+drwxr-xr-x   0 jordan     (501) staff       (20)        0 2024-04-06 00:13:54.768600 ipython_openai-0.0.2/ipython_openai.egg-info/
+-rw-r--r--   0 jordan     (501) staff       (20)     1875 2024-04-06 00:13:54.000000 ipython_openai-0.0.2/ipython_openai.egg-info/PKG-INFO
+-rw-r--r--   0 jordan     (501) staff       (20)      295 2024-04-06 00:13:54.000000 ipython_openai-0.0.2/ipython_openai.egg-info/SOURCES.txt
+-rw-r--r--   0 jordan     (501) staff       (20)        1 2024-04-06 00:13:54.000000 ipython_openai-0.0.2/ipython_openai.egg-info/dependency_links.txt
+-rw-r--r--   0 jordan     (501) staff       (20)       77 2024-04-06 00:13:54.000000 ipython_openai-0.0.2/ipython_openai.egg-info/entry_points.txt
+-rw-r--r--   0 jordan     (501) staff       (20)       51 2024-04-06 00:13:54.000000 ipython_openai-0.0.2/ipython_openai.egg-info/requires.txt
+-rw-r--r--   0 jordan     (501) staff       (20)       15 2024-04-06 00:13:54.000000 ipython_openai-0.0.2/ipython_openai.egg-info/top_level.txt
+-rw-r--r--   0 jordan     (501) staff       (20)       38 2024-04-06 00:13:54.768891 ipython_openai-0.0.2/setup.cfg
+-rw-r--r--   0 jordan     (501) staff       (20)      930 2024-04-05 23:31:49.000000 ipython_openai-0.0.2/setup.py
```

### Comparing `ipython_openai-0.0.1/LICENSE` & `ipython_openai-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ipython_openai-0.0.1/PKG-INFO` & `ipython_openai-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipython_openai
-Version: 0.0.1
+Version: 0.0.2
 Summary: An IPython extension for interacting with OpenAI's models
 Home-page: https://github.com/dustmason/ipython_openai
 Author: Jordan Sitkin
 Author-email: jordan@fiftyfootfoghorn.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ipython_openai-0.0.1/ipython_openai/gpt.py` & `ipython_openai-0.0.2/ipython_openai/gpt.py`

 * *Files identical despite different names*

### Comparing `ipython_openai-0.0.1/ipython_openai.egg-info/PKG-INFO` & `ipython_openai-0.0.2/ipython_openai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipython-openai
-Version: 0.0.1
+Version: 0.0.2
 Summary: An IPython extension for interacting with OpenAI's models
 Home-page: https://github.com/dustmason/ipython_openai
 Author: Jordan Sitkin
 Author-email: jordan@fiftyfootfoghorn.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ipython_openai-0.0.1/setup.py` & `ipython_openai-0.0.2/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="ipython_openai",
-    version="0.0.1",
+    version="0.0.2",
     author="Jordan Sitkin",
     author_email="jordan@fiftyfootfoghorn.com",
     description="An IPython extension for interacting with OpenAI's models",
     long_description=open('readme.md').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/dustmason/ipython_openai",
     packages=find_packages(),
@@ -14,15 +14,18 @@
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Framework :: IPython",
     ],
     python_requires='>=3.6',
     install_requires=[
+        "openai",
         "ipython>=7.0",
+        "prompt_toolkit>=2.0.0",
+        "pygments",
     ],
     entry_points={
         'ipython.extensions': [
             'ipython_openai = ipython_openai:load_ipython_extension',
         ],
     }
 )
```

