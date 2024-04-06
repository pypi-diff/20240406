# Comparing `tmp/mocker_db-0.0.6.tar.gz` & `tmp/mocker_db-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mocker_db-0.0.6.tar", last modified: Tue Mar 19 00:25:40 2024, max compression
+gzip compressed data, was "mocker_db-0.0.7.tar", last modified: Sat Apr  6 02:02:00 2024, max compression
```

## Comparing `mocker_db-0.0.6.tar` & `mocker_db-0.0.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 00:25:40.865634 mocker_db-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-03-19 00:22:25.000000 mocker_db-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8016 2024-03-19 00:25:40.865634 mocker_db-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4534 2024-03-19 00:22:25.000000 mocker_db-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 00:25:40.865634 mocker_db-0.0.6/mocker_db/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-03-19 00:25:24.000000 mocker_db-0.0.6/mocker_db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26554 2024-03-19 00:25:24.000000 mocker_db-0.0.6/mocker_db/mocker_db.py
--rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-03-19 00:25:40.000000 mocker_db-0.0.6/mocker_db/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 00:25:40.865634 mocker_db-0.0.6/mocker_db.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8016 2024-03-19 00:25:40.000000 mocker_db-0.0.6/mocker_db.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-03-19 00:25:40.000000 mocker_db-0.0.6/mocker_db.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-19 00:25:40.000000 mocker_db-0.0.6/mocker_db.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-03-19 00:25:40.000000 mocker_db-0.0.6/mocker_db.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-19 00:25:40.000000 mocker_db-0.0.6/mocker_db.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-19 00:25:40.865634 mocker_db-0.0.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 02:02:00.909648 mocker_db-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-06 01:58:29.000000 mocker_db-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8086 2024-04-06 02:02:00.909648 mocker_db-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4534 2024-04-06 01:58:29.000000 mocker_db-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 02:02:00.905648 mocker_db-0.0.7/mocker_db/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-06 02:01:37.000000 mocker_db-0.0.7/mocker_db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26611 2024-04-06 02:01:37.000000 mocker_db-0.0.7/mocker_db/mocker_db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-04-06 02:02:00.000000 mocker_db-0.0.7/mocker_db/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 02:02:00.905648 mocker_db-0.0.7/mocker_db.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8086 2024-04-06 02:02:00.000000 mocker_db-0.0.7/mocker_db.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-06 02:02:00.000000 mocker_db-0.0.7/mocker_db.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 02:02:00.000000 mocker_db-0.0.7/mocker_db.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-06 02:02:00.000000 mocker_db-0.0.7/mocker_db.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-06 02:02:00.000000 mocker_db-0.0.7/mocker_db.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 02:02:00.909648 mocker_db-0.0.7/setup.cfg
```

### Comparing `mocker_db-0.0.6/LICENSE` & `mocker_db-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `mocker_db-0.0.6/PKG-INFO` & `mocker_db-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mocker_db
-Version: 0.0.6
+Version: 0.0.7
 Summary: A mock handler for simulating a vector database.
 Author: Kyrylo Mordan
 Author-email: parachute.repo@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
@@ -79,15 +79,15 @@
 handler.search_database_keys(query='text')
 results = handler.get_dict_results(return_keys_list=["text"])
 print(results)
 
 ```
 
 
-    .gitattributes:   0%|          | 0.00/690 [00:00<?, ?B/s]
+    .gitattributes:   0%|          | 0.00/744 [00:00<?, ?B/s]
 
 
 
     1_Pooling/config.json:   0%|          | 0.00/190 [00:00<?, ?B/s]
 
 
 
@@ -99,14 +99,18 @@
 
 
 
     config_sentence_transformers.json:   0%|          | 0.00/122 [00:00<?, ?B/s]
 
 
 
+    model.safetensors:   0%|          | 0.00/1.11G [00:00<?, ?B/s]
+
+
+
     pytorch_model.bin:   0%|          | 0.00/1.11G [00:00<?, ?B/s]
 
 
 
     sentence_bert_config.json:   0%|          | 0.00/53.0 [00:00<?, ?B/s]
```

### Comparing `mocker_db-0.0.6/README.md` & `mocker_db-0.0.7/README.md`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -14,49 +14,43 @@
 - contains __package_metadata__ (won't package without it)
 - falls under common license
 
 The ones that were not packages, could still be used as packages with [this instruction](https://github.com/Kiril-Mordan/reusables/blob/main/docs/module_from_raw_file.md).
 
 ## Content:
  
+[module](python_modules/google_drive_support.py) - Google Drive API Utilities Module
+
+This module provides a set of functions for interacting with the Google Drive API.
+It allows you to authenticate with the API, upload, download, and manage files and folders in Google Drive.
+
 [module](python_modules/comparisonframe.py) | [usage](docs/comparisonframe.md) | [plantuml](docs/comparisonframe_plantuml.png) - Comparison Frame
 
 Designed to automate and streamline the process of comparing textual data, particularly focusing on various metrics
 such as character and word count, punctuation usage, and semantic similarity.
 It's particularly useful for scenarios where consistent text analysis is required,
 such as evaluating the performance of natural language processing models, monitoring content quality,
 or tracking changes in textual data over time using manual evaluation.
 
-[module](python_modules/shouterlog.py) | [usage](docs/shouterlog.md) | [![PyPiVersion](https://img.shields.io/pypi/v/shouterlog)](https://pypi.org/project/shouterlog/) - Shouter Log
-
-This class uses the logging module to create and manage a logger for displaying formatted messages.
-It provides a method to output various types of lines and headers, with customizable message and line lengths.
-The purpose is to be integrated into other classes that also use logger.
-
 [module](python_modules/mocker_db.py) | [usage](docs/mocker_db.md) | [drawio: -flow](docs/mocker_db-flow.png) | [release notes](release_notes/mocker_db.md) | [![PyPiVersion](https://img.shields.io/pypi/v/mocker-db)](https://pypi.org/project/mocker-db/) - MockerDB
 
 A python module that contains mock vector database like solution built around
 dictionary data type. It contains methods necessary to interact with this 'database',
 embed, search and persist.
 
+[module](python_modules/gridlooper.py) | [usage](docs/gridlooper.md) | [drawio: -flow](docs/gridlooper-flow.png) - Grid Looper
+
+A tool to run experiments based on defined grid and function with single iteration.
+
 [module](python_modules/search_based_extractor.py) | [usage](docs/search_based_extractor.md) - Search Based Extractor
 
 Utility to simplify webscraping by taking advantave of search and assumptions about html structure.
 Extractor allows to find parent html element that contains searched term, record path to it in a file
 and reuse that to scrape data with same html structure.
 
-[module](python_modules/google_drive_support.py) - Google Drive API Utilities Module
-
-This module provides a set of functions for interacting with the Google Drive API.
-It allows you to authenticate with the API, upload, download, and manage files and folders in Google Drive.
-
-[module](python_modules/gridlooper.py) | [usage](docs/gridlooper.md) | [drawio: -flow](docs/gridlooper-flow.png) - Grid Looper
-
-A tool to run experiments based on defined grid and function with single iteration.
-
 [module](python_modules/retriever_tunner.py) | [usage](docs/retriever_tunner.md) - Retriever tunner
 
 A simple tool to compare and tune retriever performance, given a desired ranking to strive for.
 The goal is to provide a simple metric to measure how a given retriver is close to the 'ideal', generated for example
 with a use of more expensive, slower or simply no-existant method.
 
 [module](python_modules/package_auto_assembler.py) | [usage](docs/package_auto_assembler.md) | [drawio: -flow](docs/package_auto_assembler-flow.png) | [![PyPiVersion](https://img.shields.io/pypi/v/package-auto-assembler)](https://pypi.org/project/package-auto-assembler/) - Package Auto Assembler
@@ -64,7 +58,13 @@
 This tool is meant to streamline creation of single module packages.
 Its purpose is to automate as many aspects of python package creation as possible,
 to shorten a development cycle of reusable components, maintain certain standard of quality
 for reusable code. It provides tool to simplify the process of package creatrion
 to a point that it can be triggered automatically within ci/cd pipelines,
 with minimal preparations and requirements for new modules.
 
+[module](python_modules/shouterlog.py) | [usage](docs/shouterlog.md) | [![PyPiVersion](https://img.shields.io/pypi/v/shouterlog)](https://pypi.org/project/shouterlog/) - Shouter Log
+
+This class uses the logging module to create and manage a logger for displaying formatted messages.
+It provides a method to output various types of lines and headers, with customizable message and line lengths.
+The purpose is to be integrated into other classes that also use logger.
+
```

### Comparing `mocker_db-0.0.6/mocker_db/mocker_db.py` & `mocker_db-0.0.7/mocker_db/mocker_db.py`

 * *Files 0% similar despite different names*

```diff
@@ -595,33 +595,14 @@
         similarity_params: dict = None,
         perform_similarity_search: bool = None):
 
         """
         Searches the mock database using embeddings and saves a list of entries that match the query.
         """
 
-        try:
-            model_name = self.embedder_params['model_name_or_path']
-            query_hash = self._make_embs_key(text = query, model = model_name)
-
-            if model_name in list(self.embs.keys()):
-
-                if query_hash not in list(self.embs[model_name].keys()):
-                    query_embedding = self.embedder.embed(query, processing_type='single')
-                else:
-                    query_embedding = self.embs[model_name][query_hash]
-            else:
-                self.embs[model_name] = {}
-                query_embedding = self.embedder.embed(query, processing_type='single')
-                self.embs[model_name][query_hash] = query_embedding
-
-
-        except Exception as e:
-            self.logger.error("Problem during embedding search query!", e)
-
 
         if search_results_n is None:
             search_results_n = self.search_results_n
 
         if similarity_search_type is None:
             similarity_search_type = self.similarity_search_type
 
@@ -635,14 +616,34 @@
             self.keys_list = [key for key in self.filtered_data]
 
         if perform_similarity_search is None:
             perform_similarity_search = True
 
         if perform_similarity_search:
 
+
+            try:
+                model_name = self.embedder_params['model_name_or_path']
+                query_hash = self._make_embs_key(text = query, model = model_name)
+
+                if model_name in list(self.embs.keys()):
+
+                    if query_hash not in list(self.embs[model_name].keys()):
+                        query_embedding = self.embedder.embed(query, processing_type='single')
+                    else:
+                        query_embedding = self.embs[model_name][query_hash]
+                else:
+                    self.embs[model_name] = {}
+                    query_embedding = self.embedder.embed(query, processing_type='single')
+                    self.embs[model_name][query_hash] = query_embedding
+
+
+            except Exception as e:
+                self.logger.error("Problem during embedding search query!", e)
+
             try:
                 data_embeddings = np.array([(self.filtered_data[d]['embedding']) for d in self.keys_list])
             except Exception as e:
                 self.logger.error("Problem during extracting search pool embeddings!", e)
 
             try:
```

### Comparing `mocker_db-0.0.6/mocker_db/setup.py` & `mocker_db-0.0.7/mocker_db/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,10 +14,10 @@
 setup(
     name="mocker_db",
     packages=["mocker_db"],
     install_requires=['### mocker_db.py', 'dill==0.3.7', 'numpy', 'sentence-transformers==2.2.2', 'hnswlib==0.8.0', 'attrs>=22.2.0'],
     classifiers=['Development Status :: 3 - Alpha', 'Intended Audience :: Developers', 'Intended Audience :: Science/Research', 'Programming Language :: Python :: 3', 'Programming Language :: Python :: 3.9', 'Programming Language :: Python :: 3.10', 'Programming Language :: Python :: 3.11', 'License :: OSI Approved :: MIT License', 'Topic :: Scientific/Engineering'],
     long_description=long_description,
     long_description_content_type='text/markdown',
-    author="Kyrylo Mordan", author_email="parachute.repo@gmail.com", description="A mock handler for simulating a vector database.", version="0.0.6"
+    author="Kyrylo Mordan", author_email="parachute.repo@gmail.com", description="A mock handler for simulating a vector database.", version="0.0.7"
 )
```

### Comparing `mocker_db-0.0.6/mocker_db.egg-info/PKG-INFO` & `mocker_db-0.0.7/mocker_db.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mocker-db
-Version: 0.0.6
+Version: 0.0.7
 Summary: A mock handler for simulating a vector database.
 Author: Kyrylo Mordan
 Author-email: parachute.repo@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
@@ -79,15 +79,15 @@
 handler.search_database_keys(query='text')
 results = handler.get_dict_results(return_keys_list=["text"])
 print(results)
 
 ```
 
 
-    .gitattributes:   0%|          | 0.00/690 [00:00<?, ?B/s]
+    .gitattributes:   0%|          | 0.00/744 [00:00<?, ?B/s]
 
 
 
     1_Pooling/config.json:   0%|          | 0.00/190 [00:00<?, ?B/s]
 
 
 
@@ -99,14 +99,18 @@
 
 
 
     config_sentence_transformers.json:   0%|          | 0.00/122 [00:00<?, ?B/s]
 
 
 
+    model.safetensors:   0%|          | 0.00/1.11G [00:00<?, ?B/s]
+
+
+
     pytorch_model.bin:   0%|          | 0.00/1.11G [00:00<?, ?B/s]
 
 
 
     sentence_bert_config.json:   0%|          | 0.00/53.0 [00:00<?, ?B/s]
```

