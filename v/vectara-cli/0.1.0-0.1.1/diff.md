# Comparing `tmp/vectara-cli-0.1.0.tar.gz` & `tmp/vectara-cli-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vectara-cli-0.1.0.tar", last modified: Fri Apr  5 15:54:23 2024, max compression
+gzip compressed data, was "vectara-cli-0.1.1.tar", last modified: Sat Apr  6 14:26:42 2024, max compression
```

## Comparing `vectara-cli-0.1.0.tar` & `vectara-cli-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-05 15:54:23.575954 vectara-cli-0.1.0/
--rw-rw-rw-   0        0        0     1026 2024-04-05 13:30:44.000000 vectara-cli-0.1.0/LICENSE.md
--rw-rw-rw-   0        0        0     8179 2024-04-05 15:54:23.573449 vectara-cli-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     7275 2024-04-05 13:31:49.000000 vectara-cli-0.1.0/README.md
--rw-rw-rw-   0        0        0       42 2024-04-05 15:54:23.576454 vectara-cli-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1268 2024-04-05 13:20:46.000000 vectara-cli-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-05 15:54:23.557922 vectara-cli-0.1.0/vectara-cli/
--rw-rw-rw-   0        0        0        0 2024-04-05 09:13:47.000000 vectara-cli-0.1.0/vectara-cli/__init__.py
--rw-rw-rw-   0        0        0    17117 2024-04-05 10:27:08.000000 vectara-cli-0.1.0/vectara-cli/core.py
-drwxrwxrwx   0        0        0        0 2024-04-05 15:54:23.570934 vectara-cli-0.1.0/vectara_cli.egg-info/
--rw-rw-rw-   0        0        0     8179 2024-04-05 15:54:22.000000 vectara-cli-0.1.0/vectara_cli.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      285 2024-04-05 15:54:23.000000 vectara-cli-0.1.0/vectara_cli.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 15:54:22.000000 vectara-cli-0.1.0/vectara_cli.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2024-04-05 15:54:22.000000 vectara-cli-0.1.0/vectara_cli.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       65 2024-04-05 15:54:22.000000 vectara-cli-0.1.0/vectara_cli.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-05 15:54:22.000000 vectara-cli-0.1.0/vectara_cli.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-06 14:26:42.562899 vectara-cli-0.1.1/
+-rw-rw-rw-   0        0        0     1026 2024-04-05 13:30:44.000000 vectara-cli-0.1.1/LICENSE.md
+-rw-rw-rw-   0        0        0    18570 2024-04-06 14:26:42.560897 vectara-cli-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0    17403 2024-04-06 14:23:07.000000 vectara-cli-0.1.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-06 14:26:42.563898 vectara-cli-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1441 2024-04-06 00:03:58.000000 vectara-cli-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-06 14:26:42.540794 vectara-cli-0.1.1/vectara-cli/
+-rw-rw-rw-   0        0        0        0 2024-04-05 09:13:47.000000 vectara-cli-0.1.1/vectara-cli/__init__.py
+-rw-rw-rw-   0        0        0    17117 2024-04-05 10:27:08.000000 vectara-cli-0.1.1/vectara-cli/core.py
+-rw-rw-rw-   0        0        0     6100 2024-04-06 14:12:04.000000 vectara-cli-0.1.1/vectara-cli/main.py
+drwxrwxrwx   0        0        0        0 2024-04-06 14:26:42.558384 vectara-cli-0.1.1/vectara_cli.egg-info/
+-rw-rw-rw-   0        0        0    18570 2024-04-06 14:26:41.000000 vectara-cli-0.1.1/vectara_cli.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      305 2024-04-06 14:26:42.000000 vectara-cli-0.1.1/vectara_cli.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-06 14:26:41.000000 vectara-cli-0.1.1/vectara_cli.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2024-04-06 14:26:41.000000 vectara-cli-0.1.1/vectara_cli.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       84 2024-04-06 14:26:41.000000 vectara-cli-0.1.1/vectara_cli.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-06 14:26:41.000000 vectara-cli-0.1.1/vectara_cli.egg-info/top_level.txt
```

### Comparing `vectara-cli-0.1.0/LICENSE.md` & `vectara-cli-0.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `vectara-cli-0.1.0/setup.py` & `vectara-cli-0.1.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,14 @@
+ # ./setup.py
+
 from setuptools import setup, find_packages
 
 setup(
     name="vectara-cli",
-    version="0.1.0",
+    version="0.1.1",
     author="Tonic-AI",
     author_email="team@tonic-ai.com",
     description="A CLI tool for interacting with the Vectara platform, including advanced text processing and indexing features.",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     url="https://git.tonic-ai.com/releases/vectara-cli",
     packages=find_packages(),
@@ -14,25 +16,28 @@
         "requests",
     ],
     extras_require={
         "advanced": [
             "accelerate",
             "torch>=1.8.0",
             "transformers>=4.5.0",
+            "span_marker",
+            "spacey",
         ],
     },
     entry_points={
         'console_scripts': [
-            'vectara-cli=vectara_cli.main:main',  # Ensure you have a main.py with a main function in your vectara_cli package
+            'vectara-cli=vectara_cli.core:VectaraClient',
         ],
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Libraries :: Python Modules",
         "Topic :: Utilities",
     ],
     python_requires='>=3.6',
     license="MIT",
-)
+    keywords="vectara search-engine document-indexing text-analysis information-retrieval natural-language-processing cli-tool data-science machine-learning text-processing",
+)
```

### Comparing `vectara-cli-0.1.0/vectara-cli/core.py` & `vectara-cli-0.1.1/vectara-cli/core.py`

 * *Files identical despite different names*

