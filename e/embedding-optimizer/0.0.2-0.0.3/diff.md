# Comparing `tmp/embedding_optimizer-0.0.2.tar.gz` & `tmp/embedding_optimizer-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "embedding_optimizer-0.0.2.tar", last modified: Sat Apr  6 11:43:08 2024, max compression
+gzip compressed data, was "embedding_optimizer-0.0.3.tar", last modified: Sat Apr  6 11:45:41 2024, max compression
```

## Comparing `embedding_optimizer-0.0.2.tar` & `embedding_optimizer-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-06 11:43:08.831998 embedding_optimizer-0.0.2/
--rw-rw-rw-   0        0        0     1066 2024-04-06 10:20:26.000000 embedding_optimizer-0.0.2/LICENCE
--rw-rw-rw-   0        0        0     3541 2024-04-06 11:43:08.830998 embedding_optimizer-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     3039 2024-04-06 11:42:32.000000 embedding_optimizer-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-06 11:43:08.792378 embedding_optimizer-0.0.2/embedding_optimizer/
--rw-rw-rw-   0        0        0      574 2024-04-06 11:42:47.000000 embedding_optimizer-0.0.2/embedding_optimizer/__init__.py
--rw-rw-rw-   0        0        0     5987 2024-04-06 10:50:32.000000 embedding_optimizer-0.0.2/embedding_optimizer/optimizer.py
-drwxrwxrwx   0        0        0        0 2024-04-06 11:43:08.827747 embedding_optimizer-0.0.2/embedding_optimizer.egg-info/
--rw-rw-rw-   0        0        0     3541 2024-04-06 11:43:08.000000 embedding_optimizer-0.0.2/embedding_optimizer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      263 2024-04-06 11:43:08.000000 embedding_optimizer-0.0.2/embedding_optimizer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-06 11:43:08.000000 embedding_optimizer-0.0.2/embedding_optimizer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2024-04-06 11:43:08.000000 embedding_optimizer-0.0.2/embedding_optimizer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-06 11:43:08.832998 embedding_optimizer-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1001 2024-04-06 11:34:19.000000 embedding_optimizer-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-06 11:45:41.639819 embedding_optimizer-0.0.3/
+-rw-rw-rw-   0        0        0     1066 2024-04-06 10:20:26.000000 embedding_optimizer-0.0.3/LICENCE
+-rw-rw-rw-   0        0        0     3535 2024-04-06 11:45:41.638409 embedding_optimizer-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3034 2024-04-06 11:44:49.000000 embedding_optimizer-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-06 11:45:41.595877 embedding_optimizer-0.0.3/embedding_optimizer/
+-rw-rw-rw-   0        0        0      574 2024-04-06 11:45:03.000000 embedding_optimizer-0.0.3/embedding_optimizer/__init__.py
+-rw-rw-rw-   0        0        0     5987 2024-04-06 10:50:32.000000 embedding_optimizer-0.0.3/embedding_optimizer/optimizer.py
+drwxrwxrwx   0        0        0        0 2024-04-06 11:45:41.632860 embedding_optimizer-0.0.3/embedding_optimizer.egg-info/
+-rw-rw-rw-   0        0        0     3535 2024-04-06 11:45:41.000000 embedding_optimizer-0.0.3/embedding_optimizer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      263 2024-04-06 11:45:41.000000 embedding_optimizer-0.0.3/embedding_optimizer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-06 11:45:41.000000 embedding_optimizer-0.0.3/embedding_optimizer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2024-04-06 11:45:41.000000 embedding_optimizer-0.0.3/embedding_optimizer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-06 11:45:41.640819 embedding_optimizer-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1001 2024-04-06 11:34:19.000000 embedding_optimizer-0.0.3/setup.py
```

### Comparing `embedding_optimizer-0.0.2/LICENCE` & `embedding_optimizer-0.0.3/LICENCE`

 * *Files identical despite different names*

### Comparing `embedding_optimizer-0.0.2/PKG-INFO` & `embedding_optimizer-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: embedding_optimizer
-Version: 0.0.2
+Version: 0.0.3
 Summary: Strategies for Efficient Data Embedding: Creating Embeddings Optimized for Accuracy - Creating Embeddings Optimized for Storage
 Home-page: https://github.com/taherfattahi/embedding-optimizer
 Author: Taher Fattahi
 Author-email: taherfattahi11@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENCE
@@ -71,15 +71,14 @@
 $ pip install embedding-optimizer
 ```
 Also can be found on [pypi](https://pypi.org/project/embedding-optimizer)
 
 ### How can I use it?
   - Install the package by pip package manager.
   - After installing, you can use it and call the library.
-  - 
 
 ### Issues
 Feel free to submit issues and enhancement requests.
 
 ### Contributing
 Please refer to each project's style and contribution guidelines for submitting patches and additions. In general, we follow the "fork-and-pull" Git workflow.
```

### Comparing `embedding_optimizer-0.0.2/README.md` & `embedding_optimizer-0.0.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -60,15 +60,14 @@
 $ pip install embedding-optimizer
 ```
 Also can be found on [pypi](https://pypi.org/project/embedding-optimizer)
 
 ### How can I use it?
   - Install the package by pip package manager.
   - After installing, you can use it and call the library.
-  - 
 
 ### Issues
 Feel free to submit issues and enhancement requests.
 
 ### Contributing
 Please refer to each project's style and contribution guidelines for submitting patches and additions. In general, we follow the "fork-and-pull" Git workflow.
```

### Comparing `embedding_optimizer-0.0.2/embedding_optimizer/__init__.py` & `embedding_optimizer-0.0.3/embedding_optimizer/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 Embedding Optimizer.
 
 Strategies for Efficient Data Embedding: Creating Embeddings Optimized for Accuracy - Creating Embeddings Optimized for Storage --- python library for OpenAI
 """
 from .optimizer import EmbeddingOptimizer
 
-__version__ = "0.0.2"
+__version__ = "0.0.3"
 __author__ = 'Taher Fattahi'
 __author_email__ = "taherfattahi11@gmail.com"
 __license__ = "MIT"
 __url__ = "https://github.com/taherfattahi/embedding-optimizer"
 
 PYPI_SIMPLE_ENDPOINT: str = "https://pypi.org/project/embedding-optimizer"
```

### Comparing `embedding_optimizer-0.0.2/embedding_optimizer/optimizer.py` & `embedding_optimizer-0.0.3/embedding_optimizer/optimizer.py`

 * *Files identical despite different names*

### Comparing `embedding_optimizer-0.0.2/embedding_optimizer.egg-info/PKG-INFO` & `embedding_optimizer-0.0.3/embedding_optimizer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: embedding-optimizer
-Version: 0.0.2
+Version: 0.0.3
 Summary: Strategies for Efficient Data Embedding: Creating Embeddings Optimized for Accuracy - Creating Embeddings Optimized for Storage
 Home-page: https://github.com/taherfattahi/embedding-optimizer
 Author: Taher Fattahi
 Author-email: taherfattahi11@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENCE
@@ -71,15 +71,14 @@
 $ pip install embedding-optimizer
 ```
 Also can be found on [pypi](https://pypi.org/project/embedding-optimizer)
 
 ### How can I use it?
   - Install the package by pip package manager.
   - After installing, you can use it and call the library.
-  - 
 
 ### Issues
 Feel free to submit issues and enhancement requests.
 
 ### Contributing
 Please refer to each project's style and contribution guidelines for submitting patches and additions. In general, we follow the "fork-and-pull" Git workflow.
```

### Comparing `embedding_optimizer-0.0.2/setup.py` & `embedding_optimizer-0.0.3/setup.py`

 * *Files identical despite different names*

