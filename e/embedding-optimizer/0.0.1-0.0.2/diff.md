# Comparing `tmp/embedding_optimizer-0.0.1.tar.gz` & `tmp/embedding_optimizer-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "embedding_optimizer-0.0.1.tar", last modified: Sat Apr  6 11:34:29 2024, max compression
+gzip compressed data, was "embedding_optimizer-0.0.2.tar", last modified: Sat Apr  6 11:43:08 2024, max compression
```

## Comparing `embedding_optimizer-0.0.1.tar` & `embedding_optimizer-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-06 11:34:29.030058 embedding_optimizer-0.0.1/
--rw-rw-rw-   0        0        0     1066 2024-04-06 10:20:26.000000 embedding_optimizer-0.0.1/LICENCE
--rw-rw-rw-   0        0        0     2798 2024-04-06 11:34:29.021685 embedding_optimizer-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2316 2024-04-06 11:30:02.000000 embedding_optimizer-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-06 11:34:28.961059 embedding_optimizer-0.0.1/embedding_optimizer/
--rw-rw-rw-   0        0        0      574 2024-04-06 10:18:25.000000 embedding_optimizer-0.0.1/embedding_optimizer/__init__.py
--rw-rw-rw-   0        0        0     5987 2024-04-06 10:50:32.000000 embedding_optimizer-0.0.1/embedding_optimizer/optimizer.py
-drwxrwxrwx   0        0        0        0 2024-04-06 11:34:29.012917 embedding_optimizer-0.0.1/embedding_optimizer.egg-info/
--rw-rw-rw-   0        0        0     2798 2024-04-06 11:34:28.000000 embedding_optimizer-0.0.1/embedding_optimizer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      263 2024-04-06 11:34:28.000000 embedding_optimizer-0.0.1/embedding_optimizer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-06 11:34:28.000000 embedding_optimizer-0.0.1/embedding_optimizer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2024-04-06 11:34:28.000000 embedding_optimizer-0.0.1/embedding_optimizer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-06 11:34:29.030058 embedding_optimizer-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1001 2024-04-06 11:34:19.000000 embedding_optimizer-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-06 11:43:08.831998 embedding_optimizer-0.0.2/
+-rw-rw-rw-   0        0        0     1066 2024-04-06 10:20:26.000000 embedding_optimizer-0.0.2/LICENCE
+-rw-rw-rw-   0        0        0     3541 2024-04-06 11:43:08.830998 embedding_optimizer-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3039 2024-04-06 11:42:32.000000 embedding_optimizer-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-06 11:43:08.792378 embedding_optimizer-0.0.2/embedding_optimizer/
+-rw-rw-rw-   0        0        0      574 2024-04-06 11:42:47.000000 embedding_optimizer-0.0.2/embedding_optimizer/__init__.py
+-rw-rw-rw-   0        0        0     5987 2024-04-06 10:50:32.000000 embedding_optimizer-0.0.2/embedding_optimizer/optimizer.py
+drwxrwxrwx   0        0        0        0 2024-04-06 11:43:08.827747 embedding_optimizer-0.0.2/embedding_optimizer.egg-info/
+-rw-rw-rw-   0        0        0     3541 2024-04-06 11:43:08.000000 embedding_optimizer-0.0.2/embedding_optimizer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      263 2024-04-06 11:43:08.000000 embedding_optimizer-0.0.2/embedding_optimizer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-06 11:43:08.000000 embedding_optimizer-0.0.2/embedding_optimizer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2024-04-06 11:43:08.000000 embedding_optimizer-0.0.2/embedding_optimizer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-06 11:43:08.832998 embedding_optimizer-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1001 2024-04-06 11:34:19.000000 embedding_optimizer-0.0.2/setup.py
```

### Comparing `embedding_optimizer-0.0.1/LICENCE` & `embedding_optimizer-0.0.2/LICENCE`

 * *Files identical despite different names*

### Comparing `embedding_optimizer-0.0.1/PKG-INFO` & `embedding_optimizer-0.0.2/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,71 +1,80 @@
-Metadata-Version: 2.1
-Name: embedding_optimizer
-Version: 0.0.1
-Summary: Strategies for Efficient Data Embedding: Creating Embeddings Optimized for Accuracy - Creating Embeddings Optimized for Storage
-Home-page: https://github.com/taherfattahi/embedding-optimizer
-Author: Taher Fattahi
-Author-email: taherfattahi11@gmail.com
-License: MIT
-Description-Content-Type: text/markdown
-License-File: LICENCE
-
-# Strategies for Efficient Data Embedding
-Two approaches to generating optimized embeddings.
-
-1) Creating Embeddings Optimized for Accuracy
-  If youâ€™re optimizing for accuracy, a good practice is to first summarize the entire document, then store the summary text and the embedding together. For the rest of the document, you can simply create overlapping chunks and store the embedding and the chunk text together.
-
-![EmbeddingOptimizerAccuracy](https://raw.github.com/taherfattahi/embedding-optimizer/master/images/optimize-accuracy.webp
-)
-
-2) Creating Embeddings Optimized for Storage
-  If youâ€™re optimizing for space, you can chunk the data, summarize each chunk, concatenate all the summarizations, then create an embedding for the final summary.
-
-![EmbeddingOptimizerStorage](https://raw.github.com/taherfattahi/embedding-optimizer/master/images/optimize-storage.webp
-)
-
-
-## Example
-```python
-import os
-
-from langchain_community.document_loaders import TextLoader
-from langchain_openai import OpenAIEmbeddings
-from langchain_text_splitters import CharacterTextSplitter
-from langchain.docstore.document import Document
-from langchain_community.vectorstores import FAISS
-from openai import OpenAI
-
-from embedding_optimizer.optimizer import EmbeddingOptimizer
-
-# Set your OpenAI API Key
-os.environ['OPENAI_API_KEY'] = ''
-
-# Load your document
-raw_document = TextLoader('test_data.txt').load()
-
-# If your document is long, you might want to split it into chunks
-text_splitter = CharacterTextSplitter(separator=".", chunk_size=1000, chunk_overlap=0)
-documents = text_splitter.split_documents(raw_document)
-
-embedding_optimizer = EmbeddingOptimizer(openai_api_key='')
-
-# documents_optimizer = embedding_optimizer.optimized_documents_for_storage(raw_document[0].page_content, documents)
-documents_optimizer = embedding_optimizer.optimized_documents_for_accuracy(raw_document[0].page_content, documents)
-
-# Embed the document chunks and the summary
-embedding_model = OpenAIEmbeddings(openai_api_key=os.environ["OPENAI_API_KEY"])
-
-db = FAISS.from_documents(documents_optimizer, embedding_model)
-
-# query it
-query = "What motivated Alex to create the Function of Everything (FoE)?"
-docs = db.similarity_search(query)
-
-print(docs[0].page_content)
-
-```
-
-
-### Issues
-Feel free to submit issues and enhancement requests.
+# Strategies for Efficient Data Embedding
+Two approaches to generating optimized embeddings.
+
+1) Creating Embeddings Optimized for Accuracy
+  If you’re optimizing for accuracy, a good practice is to first summarize the entire document, then store the summary text and the embedding together. For the rest of the document, you can simply create overlapping chunks and store the embedding and the chunk text together.
+
+![EmbeddingOptimizerAccuracy](https://raw.github.com/taherfattahi/embedding-optimizer/master/images/optimize-accuracy.webp
+)
+
+2) Creating Embeddings Optimized for Storage
+  If you’re optimizing for space, you can chunk the data, summarize each chunk, concatenate all the summarizations, then create an embedding for the final summary.
+
+![EmbeddingOptimizerStorage](https://raw.github.com/taherfattahi/embedding-optimizer/master/images/optimize-storage.webp
+)
+
+
+## Example
+```python
+import os
+
+from langchain_community.document_loaders import TextLoader
+from langchain_openai import OpenAIEmbeddings
+from langchain_text_splitters import CharacterTextSplitter
+from langchain.docstore.document import Document
+from langchain_community.vectorstores import FAISS
+from openai import OpenAI
+
+from embedding_optimizer.optimizer import EmbeddingOptimizer
+
+# Set your OpenAI API Key
+os.environ['OPENAI_API_KEY'] = ''
+
+# Load your document
+raw_document = TextLoader('test_data.txt').load()
+
+# If your document is long, you might want to split it into chunks
+text_splitter = CharacterTextSplitter(separator=".", chunk_size=1000, chunk_overlap=0)
+documents = text_splitter.split_documents(raw_document)
+
+embedding_optimizer = EmbeddingOptimizer(openai_api_key='')
+
+# documents_optimizer = embedding_optimizer.optimized_documents_for_storage(raw_document[0].page_content, documents)
+documents_optimizer = embedding_optimizer.optimized_documents_for_accuracy(raw_document[0].page_content, documents)
+
+# Embed the document chunks and the summary
+embedding_model = OpenAIEmbeddings(openai_api_key=os.environ["OPENAI_API_KEY"])
+
+db = FAISS.from_documents(documents_optimizer, embedding_model)
+
+# query it
+query = "What motivated Alex to create the Function of Everything (FoE)?"
+docs = db.similarity_search(query)
+
+print(docs[0].page_content)
+
+```
+### Installation
+
+```sh
+$ pip install embedding-optimizer
+```
+Also can be found on [pypi](https://pypi.org/project/embedding-optimizer)
+
+### How can I use it?
+  - Install the package by pip package manager.
+  - After installing, you can use it and call the library.
+  - 
+
+### Issues
+Feel free to submit issues and enhancement requests.
+
+### Contributing
+Please refer to each project's style and contribution guidelines for submitting patches and additions. In general, we follow the "fork-and-pull" Git workflow.
+
+ 1. **Fork** the repo on GitHub
+ 2. **Clone** the project to your own machine
+ 3. **Update the Version** inside __init__.py
+ 4. **Commit** changes to your own branch
+ 5. **Push** your work back up to your fork
+ 6. Submit a **Pull request** so that we can review your changes
```

### Comparing `embedding_optimizer-0.0.1/embedding_optimizer/__init__.py` & `embedding_optimizer-0.0.2/embedding_optimizer/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 Embedding Optimizer.
 
 Strategies for Efficient Data Embedding: Creating Embeddings Optimized for Accuracy - Creating Embeddings Optimized for Storage --- python library for OpenAI
 """
 from .optimizer import EmbeddingOptimizer
 
-__version__ = "0.0.1"
+__version__ = "0.0.2"
 __author__ = 'Taher Fattahi'
 __author_email__ = "taherfattahi11@gmail.com"
 __license__ = "MIT"
 __url__ = "https://github.com/taherfattahi/embedding-optimizer"
 
 PYPI_SIMPLE_ENDPOINT: str = "https://pypi.org/project/embedding-optimizer"
```

### Comparing `embedding_optimizer-0.0.1/embedding_optimizer/optimizer.py` & `embedding_optimizer-0.0.2/embedding_optimizer/optimizer.py`

 * *Files identical despite different names*

### Comparing `embedding_optimizer-0.0.1/setup.py` & `embedding_optimizer-0.0.2/setup.py`

 * *Files identical despite different names*

