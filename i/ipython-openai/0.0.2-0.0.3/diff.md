# Comparing `tmp/ipython_openai-0.0.2.tar.gz` & `tmp/ipython_openai-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipython_openai-0.0.2.tar", last modified: Sat Apr  6 00:13:54 2024, max compression
+gzip compressed data, was "ipython_openai-0.0.3.tar", last modified: Sat Apr  6 00:37:48 2024, max compression
```

## Comparing `ipython_openai-0.0.2.tar` & `ipython_openai-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 jordan     (501) staff       (20)        0 2024-04-06 00:13:54.768849 ipython_openai-0.0.2/
--rw-r--r--   0 jordan     (501) staff       (20)     1060 2024-04-05 22:49:53.000000 ipython_openai-0.0.2/LICENSE
--rw-r--r--   0 jordan     (501) staff       (20)     1875 2024-04-06 00:13:54.768738 ipython_openai-0.0.2/PKG-INFO
-drwxr-xr-x   0 jordan     (501) staff       (20)        0 2024-04-06 00:13:54.767824 ipython_openai-0.0.2/ipython_openai/
--rw-r--r--   0 jordan     (501) staff       (20)      116 2024-04-05 20:25:04.000000 ipython_openai-0.0.2/ipython_openai/__init__.py
--rw-r--r--   0 jordan     (501) staff       (20)     3860 2024-04-05 22:04:38.000000 ipython_openai-0.0.2/ipython_openai/gpt.py
-drwxr-xr-x   0 jordan     (501) staff       (20)        0 2024-04-06 00:13:54.768600 ipython_openai-0.0.2/ipython_openai.egg-info/
--rw-r--r--   0 jordan     (501) staff       (20)     1875 2024-04-06 00:13:54.000000 ipython_openai-0.0.2/ipython_openai.egg-info/PKG-INFO
--rw-r--r--   0 jordan     (501) staff       (20)      295 2024-04-06 00:13:54.000000 ipython_openai-0.0.2/ipython_openai.egg-info/SOURCES.txt
--rw-r--r--   0 jordan     (501) staff       (20)        1 2024-04-06 00:13:54.000000 ipython_openai-0.0.2/ipython_openai.egg-info/dependency_links.txt
--rw-r--r--   0 jordan     (501) staff       (20)       77 2024-04-06 00:13:54.000000 ipython_openai-0.0.2/ipython_openai.egg-info/entry_points.txt
--rw-r--r--   0 jordan     (501) staff       (20)       51 2024-04-06 00:13:54.000000 ipython_openai-0.0.2/ipython_openai.egg-info/requires.txt
--rw-r--r--   0 jordan     (501) staff       (20)       15 2024-04-06 00:13:54.000000 ipython_openai-0.0.2/ipython_openai.egg-info/top_level.txt
--rw-r--r--   0 jordan     (501) staff       (20)       38 2024-04-06 00:13:54.768891 ipython_openai-0.0.2/setup.cfg
--rw-r--r--   0 jordan     (501) staff       (20)      930 2024-04-05 23:31:49.000000 ipython_openai-0.0.2/setup.py
+drwxr-xr-x   0 jordan     (501) staff       (20)        0 2024-04-06 00:37:48.187293 ipython_openai-0.0.3/
+-rw-r--r--   0 jordan     (501) staff       (20)     1060 2024-04-05 22:49:53.000000 ipython_openai-0.0.3/LICENSE
+-rw-r--r--   0 jordan     (501) staff       (20)     2151 2024-04-06 00:37:48.187186 ipython_openai-0.0.3/PKG-INFO
+drwxr-xr-x   0 jordan     (501) staff       (20)        0 2024-04-06 00:37:48.186380 ipython_openai-0.0.3/ipython_openai/
+-rw-r--r--   0 jordan     (501) staff       (20)      116 2024-04-05 20:25:04.000000 ipython_openai-0.0.3/ipython_openai/__init__.py
+-rw-r--r--   0 jordan     (501) staff       (20)     3860 2024-04-05 22:04:38.000000 ipython_openai-0.0.3/ipython_openai/gpt.py
+drwxr-xr-x   0 jordan     (501) staff       (20)        0 2024-04-06 00:37:48.187050 ipython_openai-0.0.3/ipython_openai.egg-info/
+-rw-r--r--   0 jordan     (501) staff       (20)     2151 2024-04-06 00:37:48.000000 ipython_openai-0.0.3/ipython_openai.egg-info/PKG-INFO
+-rw-r--r--   0 jordan     (501) staff       (20)      295 2024-04-06 00:37:48.000000 ipython_openai-0.0.3/ipython_openai.egg-info/SOURCES.txt
+-rw-r--r--   0 jordan     (501) staff       (20)        1 2024-04-06 00:37:48.000000 ipython_openai-0.0.3/ipython_openai.egg-info/dependency_links.txt
+-rw-r--r--   0 jordan     (501) staff       (20)       77 2024-04-06 00:37:48.000000 ipython_openai-0.0.3/ipython_openai.egg-info/entry_points.txt
+-rw-r--r--   0 jordan     (501) staff       (20)       51 2024-04-06 00:37:48.000000 ipython_openai-0.0.3/ipython_openai.egg-info/requires.txt
+-rw-r--r--   0 jordan     (501) staff       (20)       15 2024-04-06 00:37:48.000000 ipython_openai-0.0.3/ipython_openai.egg-info/top_level.txt
+-rw-r--r--   0 jordan     (501) staff       (20)       38 2024-04-06 00:37:48.187338 ipython_openai-0.0.3/setup.cfg
+-rw-r--r--   0 jordan     (501) staff       (20)      930 2024-04-06 00:34:47.000000 ipython_openai-0.0.3/setup.py
```

### Comparing `ipython_openai-0.0.2/LICENSE` & `ipython_openai-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ipython_openai-0.0.2/ipython_openai/gpt.py` & `ipython_openai-0.0.3/ipython_openai/gpt.py`

 * *Files identical despite different names*

### Comparing `ipython_openai-0.0.2/setup.py` & `ipython_openai-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="ipython_openai",
-    version="0.0.2",
+    version="0.0.3",
     author="Jordan Sitkin",
     author_email="jordan@fiftyfootfoghorn.com",
     description="An IPython extension for interacting with OpenAI's models",
     long_description=open('readme.md').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/dustmason/ipython_openai",
     packages=find_packages(),
```

