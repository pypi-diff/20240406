# Comparing `tmp/vectara_cli-0.1.2.tar.gz` & `tmp/vectara-cli-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vectara_cli-0.1.2.tar", last modified: Sat Apr  6 15:15:09 2024, max compression
+gzip compressed data, was "vectara-cli-0.1.3.tar", last modified: Sat Apr  6 15:25:28 2024, max compression
```

## Comparing `vectara_cli-0.1.2.tar` & `vectara-cli-0.1.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-06 15:15:09.382781 vectara_cli-0.1.2/
--rw-rw-rw-   0        0        0     1026 2024-04-05 13:30:44.000000 vectara_cli-0.1.2/LICENSE.md
--rw-rw-rw-   0        0        0    18405 2024-04-06 15:15:09.381192 vectara_cli-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0    17239 2024-04-06 15:00:57.000000 vectara_cli-0.1.2/README.md
--rw-rw-rw-   0        0        0       42 2024-04-06 15:15:09.383291 vectara_cli-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1440 2024-04-06 15:10:59.000000 vectara_cli-0.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-06 15:15:09.364124 vectara_cli-0.1.2/vectara-cli/
--rw-rw-rw-   0        0        0        0 2024-04-05 09:13:47.000000 vectara_cli-0.1.2/vectara-cli/__init__.py
--rw-rw-rw-   0        0        0    17117 2024-04-05 10:27:08.000000 vectara_cli-0.1.2/vectara-cli/core.py
--rw-rw-rw-   0        0        0     6100 2024-04-06 14:12:04.000000 vectara_cli-0.1.2/vectara-cli/main.py
-drwxrwxrwx   0        0        0        0 2024-04-06 15:15:09.378708 vectara_cli-0.1.2/vectara_cli.egg-info/
--rw-rw-rw-   0        0        0    18405 2024-04-06 15:15:08.000000 vectara_cli-0.1.2/vectara_cli.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      305 2024-04-06 15:15:09.000000 vectara_cli-0.1.2/vectara_cli.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-06 15:15:08.000000 vectara_cli-0.1.2/vectara_cli.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2024-04-06 15:15:08.000000 vectara_cli-0.1.2/vectara_cli.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       83 2024-04-06 15:15:08.000000 vectara_cli-0.1.2/vectara_cli.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-06 15:15:08.000000 vectara_cli-0.1.2/vectara_cli.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-06 15:25:28.590633 vectara-cli-0.1.3/
+-rw-rw-rw-   0        0        0     1026 2024-04-05 13:30:44.000000 vectara-cli-0.1.3/LICENSE.md
+-rw-rw-rw-   0        0        0    18405 2024-04-06 15:25:28.588577 vectara-cli-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0    17239 2024-04-06 15:00:57.000000 vectara-cli-0.1.3/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-06 15:25:28.590633 vectara-cli-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1440 2024-04-06 15:25:19.000000 vectara-cli-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-06 15:25:28.577530 vectara-cli-0.1.3/vectara-cli/
+-rw-rw-rw-   0        0        0        0 2024-04-05 09:13:47.000000 vectara-cli-0.1.3/vectara-cli/__init__.py
+-rw-rw-rw-   0        0        0    17117 2024-04-05 10:27:08.000000 vectara-cli-0.1.3/vectara-cli/core.py
+-rw-rw-rw-   0        0        0     6100 2024-04-06 14:12:04.000000 vectara-cli-0.1.3/vectara-cli/main.py
+drwxrwxrwx   0        0        0        0 2024-04-06 15:25:28.586574 vectara-cli-0.1.3/vectara_cli.egg-info/
+-rw-rw-rw-   0        0        0    18405 2024-04-06 15:25:27.000000 vectara-cli-0.1.3/vectara_cli.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      305 2024-04-06 15:25:28.000000 vectara-cli-0.1.3/vectara_cli.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-06 15:25:27.000000 vectara-cli-0.1.3/vectara_cli.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2024-04-06 15:25:27.000000 vectara-cli-0.1.3/vectara_cli.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       83 2024-04-06 15:25:27.000000 vectara-cli-0.1.3/vectara_cli.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-06 15:25:27.000000 vectara-cli-0.1.3/vectara_cli.egg-info/top_level.txt
```

### Comparing `vectara_cli-0.1.2/LICENSE.md` & `vectara-cli-0.1.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `vectara_cli-0.1.2/PKG-INFO` & `vectara-cli-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: vectara_cli
-Version: 0.1.2
+Name: vectara-cli
+Version: 0.1.3
 Summary: A CLI tool for interacting with the Vectara platform, including advanced text processing and indexing features.
 Home-page: https://git.tonic-ai.com/releases/vectara-cli
 Author: Tonic-AI
 Author-email: team@tonic-ai.com
 License: MIT
 Keywords: vectara search-engine document-indexing text-analysis information-retrieval natural-language-processing cli-tool data-science machine-learning text-processing
 Classifier: Programming Language :: Python :: 3
```

### Comparing `vectara_cli-0.1.2/README.md` & `vectara-cli-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `vectara_cli-0.1.2/setup.py` & `vectara-cli-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
  # ./setup.py
 
 from setuptools import setup, find_packages
 
 setup(
-    name="vectara_cli",
-    version="0.1.2",
+    name="vectara-cli",
+    version="0.1.3",
     author="Tonic-AI",
     author_email="team@tonic-ai.com",
     description="A CLI tool for interacting with the Vectara platform, including advanced text processing and indexing features.",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     url="https://git.tonic-ai.com/releases/vectara-cli",
     packages=find_packages(),
@@ -22,15 +22,15 @@
             "transformers>=4.5.0",
             "span_marker",
             "spacy",
         ],
     },
     entry_points={
         'console_scripts': [
-            'vectara-cli=vectara_cli.core:VectaraClient',
+            'vectara_cli=vectara_cli.core:VectaraClient',
         ],
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Intended Audience :: Developers",
```

### Comparing `vectara_cli-0.1.2/vectara-cli/core.py` & `vectara-cli-0.1.3/vectara-cli/core.py`

 * *Files identical despite different names*

### Comparing `vectara_cli-0.1.2/vectara-cli/main.py` & `vectara-cli-0.1.3/vectara-cli/main.py`

 * *Files identical despite different names*

### Comparing `vectara_cli-0.1.2/vectara_cli.egg-info/PKG-INFO` & `vectara-cli-0.1.3/vectara_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: vectara_cli
-Version: 0.1.2
+Name: vectara-cli
+Version: 0.1.3
 Summary: A CLI tool for interacting with the Vectara platform, including advanced text processing and indexing features.
 Home-page: https://git.tonic-ai.com/releases/vectara-cli
 Author: Tonic-AI
 Author-email: team@tonic-ai.com
 License: MIT
 Keywords: vectara search-engine document-indexing text-analysis information-retrieval natural-language-processing cli-tool data-science machine-learning text-processing
 Classifier: Programming Language :: Python :: 3
```

