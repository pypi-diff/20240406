# Comparing `tmp/antoine-2.3.tar.gz` & `tmp/antoine-2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "antoine-2.3.tar", last modified: Fri Apr  5 10:44:37 2024, max compression
+gzip compressed data, was "antoine-2.4.tar", last modified: Fri Apr  5 10:49:08 2024, max compression
```

## Comparing `antoine-2.3.tar` & `antoine-2.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 antoinebertin   (501) staff       (20)        0 2024-04-05 10:44:37.344009 antoine-2.3/
--rw-r--r--   0 antoinebertin   (501) staff       (20)      206 2024-04-05 10:44:37.343799 antoine-2.3/PKG-INFO
--rw-r--r--   0 antoinebertin   (501) staff       (20)      261 2024-04-05 10:43:11.000000 antoine-2.3/README.md
-drwxr-xr-x   0 antoinebertin   (501) staff       (20)        0 2024-04-05 10:44:37.342919 antoine-2.3/antoine/
--rw-r--r--   0 antoinebertin   (501) staff       (20)       42 2024-04-04 12:03:26.000000 antoine-2.3/antoine/__init__.py
--rw-r--r--   0 antoinebertin   (501) staff       (20)     2425 2024-04-05 10:41:40.000000 antoine-2.3/antoine/app.py
-drwxr-xr-x   0 antoinebertin   (501) staff       (20)        0 2024-04-05 10:44:37.343578 antoine-2.3/antoine.egg-info/
--rw-r--r--   0 antoinebertin   (501) staff       (20)      206 2024-04-05 10:44:37.000000 antoine-2.3/antoine.egg-info/PKG-INFO
--rw-r--r--   0 antoinebertin   (501) staff       (20)      211 2024-04-05 10:44:37.000000 antoine-2.3/antoine.egg-info/SOURCES.txt
--rw-r--r--   0 antoinebertin   (501) staff       (20)        1 2024-04-05 10:44:37.000000 antoine-2.3/antoine.egg-info/dependency_links.txt
--rw-r--r--   0 antoinebertin   (501) staff       (20)       50 2024-04-05 10:44:37.000000 antoine-2.3/antoine.egg-info/entry_points.txt
--rw-r--r--   0 antoinebertin   (501) staff       (20)        8 2024-04-05 10:44:37.000000 antoine-2.3/antoine.egg-info/top_level.txt
--rw-r--r--   0 antoinebertin   (501) staff       (20)       38 2024-04-05 10:44:37.344050 antoine-2.3/setup.cfg
--rw-r--r--   0 antoinebertin   (501) staff       (20)      574 2024-04-05 09:43:39.000000 antoine-2.3/setup.py
+drwxr-xr-x   0 antoinebertin   (501) staff       (20)        0 2024-04-05 10:49:08.903540 antoine-2.4/
+-rw-r--r--   0 antoinebertin   (501) staff       (20)      206 2024-04-05 10:49:08.903340 antoine-2.4/PKG-INFO
+-rw-r--r--   0 antoinebertin   (501) staff       (20)      261 2024-04-05 10:43:11.000000 antoine-2.4/README.md
+drwxr-xr-x   0 antoinebertin   (501) staff       (20)        0 2024-04-05 10:49:08.902340 antoine-2.4/antoine/
+-rw-r--r--   0 antoinebertin   (501) staff       (20)       42 2024-04-04 12:03:26.000000 antoine-2.4/antoine/__init__.py
+-rw-r--r--   0 antoinebertin   (501) staff       (20)     2417 2024-04-05 10:48:28.000000 antoine-2.4/antoine/app.py
+drwxr-xr-x   0 antoinebertin   (501) staff       (20)        0 2024-04-05 10:49:08.903114 antoine-2.4/antoine.egg-info/
+-rw-r--r--   0 antoinebertin   (501) staff       (20)      206 2024-04-05 10:49:08.000000 antoine-2.4/antoine.egg-info/PKG-INFO
+-rw-r--r--   0 antoinebertin   (501) staff       (20)      211 2024-04-05 10:49:08.000000 antoine-2.4/antoine.egg-info/SOURCES.txt
+-rw-r--r--   0 antoinebertin   (501) staff       (20)        1 2024-04-05 10:49:08.000000 antoine-2.4/antoine.egg-info/dependency_links.txt
+-rw-r--r--   0 antoinebertin   (501) staff       (20)       50 2024-04-05 10:49:08.000000 antoine-2.4/antoine.egg-info/entry_points.txt
+-rw-r--r--   0 antoinebertin   (501) staff       (20)        8 2024-04-05 10:49:08.000000 antoine-2.4/antoine.egg-info/top_level.txt
+-rw-r--r--   0 antoinebertin   (501) staff       (20)       38 2024-04-05 10:49:08.903575 antoine-2.4/setup.cfg
+-rw-r--r--   0 antoinebertin   (501) staff       (20)      574 2024-04-05 10:48:21.000000 antoine-2.4/setup.py
```

### Comparing `antoine-2.3/antoine/app.py` & `antoine-2.4/antoine/app.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         print()  # Print a newline after fully revealing a line
 
 def main():
     email = "https://www.linkedin.com/in/antoinebertin35/"
     width = 60
     height = 10
     personal_text = """
-    Hey there! 👋 Antoine 2.3 here. 
+    Hey there! 👋 Antoine 2.4 here. 
     Sold my restaurant after 12 years and jumped into coding for about the same time. 
     Recently graduated from the top data scientist BootCamp in Europe! 🎓 
     There, I honed my skills in crafting, deploying, and monitoring ML/deep learning models. 
     I'm a computer tinkerer who enjoys slapping on 6 GPUs for fun, securing blockchain networks, 
     and crafting apps leveraging vector databases to help my lawyer friends with the civil code.
     Data's my jam, and I'm passionate about wine, blockchain, gymnastics, and kitesurfing. 
     On the lookout for a company 🕵️ that needs a reliable ally to grow their business. 
@@ -60,9 +60,7 @@
     4
     3
     2
     1
     Boom!
     """
     construct_rectangle(width, height, email, personal_text)
-
-main()
```

### Comparing `antoine-2.3/setup.py` & `antoine-2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='antoine',
-    version='2.3',
+    version='2.4',
     packages=['antoine'],  # 'antoine' is the name of the package
     author='Antoine Bertin',
     author_email='monolok35@gmail.com',
     description='Hiring Antoine is so much fun!',
     url='https://github.com/monolok/antoine/',
     license='MIT',
     entry_points={
```

