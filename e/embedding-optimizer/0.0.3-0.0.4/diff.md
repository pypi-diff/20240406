# Comparing `tmp/embedding_optimizer-0.0.3.tar.gz` & `tmp/embedding_optimizer-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "embedding_optimizer-0.0.3.tar", last modified: Sat Apr  6 11:45:41 2024, max compression
+gzip compressed data, was "embedding_optimizer-0.0.4.tar", last modified: Sat Apr  6 11:54:35 2024, max compression
```

## Comparing `embedding_optimizer-0.0.3.tar` & `embedding_optimizer-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-06 11:45:41.639819 embedding_optimizer-0.0.3/
--rw-rw-rw-   0        0        0     1066 2024-04-06 10:20:26.000000 embedding_optimizer-0.0.3/LICENCE
--rw-rw-rw-   0        0        0     3535 2024-04-06 11:45:41.638409 embedding_optimizer-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     3034 2024-04-06 11:44:49.000000 embedding_optimizer-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-06 11:45:41.595877 embedding_optimizer-0.0.3/embedding_optimizer/
--rw-rw-rw-   0        0        0      574 2024-04-06 11:45:03.000000 embedding_optimizer-0.0.3/embedding_optimizer/__init__.py
--rw-rw-rw-   0        0        0     5987 2024-04-06 10:50:32.000000 embedding_optimizer-0.0.3/embedding_optimizer/optimizer.py
-drwxrwxrwx   0        0        0        0 2024-04-06 11:45:41.632860 embedding_optimizer-0.0.3/embedding_optimizer.egg-info/
--rw-rw-rw-   0        0        0     3535 2024-04-06 11:45:41.000000 embedding_optimizer-0.0.3/embedding_optimizer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      263 2024-04-06 11:45:41.000000 embedding_optimizer-0.0.3/embedding_optimizer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-06 11:45:41.000000 embedding_optimizer-0.0.3/embedding_optimizer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2024-04-06 11:45:41.000000 embedding_optimizer-0.0.3/embedding_optimizer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-06 11:45:41.640819 embedding_optimizer-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1001 2024-04-06 11:34:19.000000 embedding_optimizer-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-06 11:54:35.135286 embedding_optimizer-0.0.4/
+-rw-rw-rw-   0        0        0     1066 2024-04-06 10:20:26.000000 embedding_optimizer-0.0.4/LICENCE
+-rw-rw-rw-   0        0        0     3748 2024-04-06 11:54:35.134290 embedding_optimizer-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     3245 2024-04-06 11:53:57.000000 embedding_optimizer-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2024-04-06 11:54:35.083773 embedding_optimizer-0.0.4/embedding_optimizer/
+-rw-rw-rw-   0        0        0      574 2024-04-06 11:54:04.000000 embedding_optimizer-0.0.4/embedding_optimizer/__init__.py
+-rw-rw-rw-   0        0        0     5987 2024-04-06 10:50:32.000000 embedding_optimizer-0.0.4/embedding_optimizer/optimizer.py
+drwxrwxrwx   0        0        0        0 2024-04-06 11:54:35.130514 embedding_optimizer-0.0.4/embedding_optimizer.egg-info/
+-rw-rw-rw-   0        0        0     3748 2024-04-06 11:54:34.000000 embedding_optimizer-0.0.4/embedding_optimizer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      263 2024-04-06 11:54:34.000000 embedding_optimizer-0.0.4/embedding_optimizer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-06 11:54:34.000000 embedding_optimizer-0.0.4/embedding_optimizer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2024-04-06 11:54:34.000000 embedding_optimizer-0.0.4/embedding_optimizer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-06 11:54:35.136311 embedding_optimizer-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1001 2024-04-06 11:34:19.000000 embedding_optimizer-0.0.4/setup.py
```

### Comparing `embedding_optimizer-0.0.3/LICENCE` & `embedding_optimizer-0.0.4/LICENCE`

 * *Files identical despite different names*

### Comparing `embedding_optimizer-0.0.3/PKG-INFO` & `embedding_optimizer-0.0.4/embedding_optimizer.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
-Name: embedding_optimizer
-Version: 0.0.3
+Name: embedding-optimizer
+Version: 0.0.4
 Summary: Strategies for Efficient Data Embedding: Creating Embeddings Optimized for Accuracy - Creating Embeddings Optimized for Storage
 Home-page: https://github.com/taherfattahi/embedding-optimizer
 Author: Taher Fattahi
 Author-email: taherfattahi11@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENCE
 
 # Strategies for Efficient Data Embedding
-Two approaches to generating optimized embeddings.
+Two approaches to generating optimized embeddings in the Retrieval-Augmented Generation (RAG) Pattern
+
+[![EmbeddingOptimizer](https://raw.github.com/taherfattahi/embedding-optimizer/master/images/RAG-pattern.webp)](https://pypi.org/project/embedding-optimizer/)
 
 1) Creating Embeddings Optimized for Accuracy
   If youâ€™re optimizing for accuracy, a good practice is to first summarize the entire document, then store the summary text and the embedding together. For the rest of the document, you can simply create overlapping chunks and store the embedding and the chunk text together.
 
 ![EmbeddingOptimizerAccuracy](https://raw.github.com/taherfattahi/embedding-optimizer/master/images/optimize-accuracy.webp
 )
```

### Comparing `embedding_optimizer-0.0.3/README.md` & `embedding_optimizer-0.0.4/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # Strategies for Efficient Data Embedding
-Two approaches to generating optimized embeddings.
+Two approaches to generating optimized embeddings in the Retrieval-Augmented Generation (RAG) Pattern
+
+[![EmbeddingOptimizer](https://raw.github.com/taherfattahi/embedding-optimizer/master/images/RAG-pattern.webp)](https://pypi.org/project/embedding-optimizer/)
 
 1) Creating Embeddings Optimized for Accuracy
   If you’re optimizing for accuracy, a good practice is to first summarize the entire document, then store the summary text and the embedding together. For the rest of the document, you can simply create overlapping chunks and store the embedding and the chunk text together.
 
 ![EmbeddingOptimizerAccuracy](https://raw.github.com/taherfattahi/embedding-optimizer/master/images/optimize-accuracy.webp
 )
```

### Comparing `embedding_optimizer-0.0.3/embedding_optimizer/__init__.py` & `embedding_optimizer-0.0.4/embedding_optimizer/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 Embedding Optimizer.
 
 Strategies for Efficient Data Embedding: Creating Embeddings Optimized for Accuracy - Creating Embeddings Optimized for Storage --- python library for OpenAI
 """
 from .optimizer import EmbeddingOptimizer
 
-__version__ = "0.0.3"
+__version__ = "0.0.4"
 __author__ = 'Taher Fattahi'
 __author_email__ = "taherfattahi11@gmail.com"
 __license__ = "MIT"
 __url__ = "https://github.com/taherfattahi/embedding-optimizer"
 
 PYPI_SIMPLE_ENDPOINT: str = "https://pypi.org/project/embedding-optimizer"
```

### Comparing `embedding_optimizer-0.0.3/embedding_optimizer/optimizer.py` & `embedding_optimizer-0.0.4/embedding_optimizer/optimizer.py`

 * *Files identical despite different names*

### Comparing `embedding_optimizer-0.0.3/embedding_optimizer.egg-info/PKG-INFO` & `embedding_optimizer-0.0.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
-Name: embedding-optimizer
-Version: 0.0.3
+Name: embedding_optimizer
+Version: 0.0.4
 Summary: Strategies for Efficient Data Embedding: Creating Embeddings Optimized for Accuracy - Creating Embeddings Optimized for Storage
 Home-page: https://github.com/taherfattahi/embedding-optimizer
 Author: Taher Fattahi
 Author-email: taherfattahi11@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENCE
 
 # Strategies for Efficient Data Embedding
-Two approaches to generating optimized embeddings.
+Two approaches to generating optimized embeddings in the Retrieval-Augmented Generation (RAG) Pattern
+
+[![EmbeddingOptimizer](https://raw.github.com/taherfattahi/embedding-optimizer/master/images/RAG-pattern.webp)](https://pypi.org/project/embedding-optimizer/)
 
 1) Creating Embeddings Optimized for Accuracy
   If youâ€™re optimizing for accuracy, a good practice is to first summarize the entire document, then store the summary text and the embedding together. For the rest of the document, you can simply create overlapping chunks and store the embedding and the chunk text together.
 
 ![EmbeddingOptimizerAccuracy](https://raw.github.com/taherfattahi/embedding-optimizer/master/images/optimize-accuracy.webp
 )
```

### Comparing `embedding_optimizer-0.0.3/setup.py` & `embedding_optimizer-0.0.4/setup.py`

 * *Files identical despite different names*

