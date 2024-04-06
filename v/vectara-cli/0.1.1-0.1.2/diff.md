# Comparing `tmp/vectara-cli-0.1.1.tar.gz` & `tmp/vectara_cli-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vectara-cli-0.1.1.tar", last modified: Sat Apr  6 14:26:42 2024, max compression
+gzip compressed data, was "vectara_cli-0.1.2.tar", last modified: Sat Apr  6 15:15:09 2024, max compression
```

## Comparing `vectara-cli-0.1.1.tar` & `vectara_cli-0.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-06 14:26:42.562899 vectara-cli-0.1.1/
--rw-rw-rw-   0        0        0     1026 2024-04-05 13:30:44.000000 vectara-cli-0.1.1/LICENSE.md
--rw-rw-rw-   0        0        0    18570 2024-04-06 14:26:42.560897 vectara-cli-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0    17403 2024-04-06 14:23:07.000000 vectara-cli-0.1.1/README.md
--rw-rw-rw-   0        0        0       42 2024-04-06 14:26:42.563898 vectara-cli-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1441 2024-04-06 00:03:58.000000 vectara-cli-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-06 14:26:42.540794 vectara-cli-0.1.1/vectara-cli/
--rw-rw-rw-   0        0        0        0 2024-04-05 09:13:47.000000 vectara-cli-0.1.1/vectara-cli/__init__.py
--rw-rw-rw-   0        0        0    17117 2024-04-05 10:27:08.000000 vectara-cli-0.1.1/vectara-cli/core.py
--rw-rw-rw-   0        0        0     6100 2024-04-06 14:12:04.000000 vectara-cli-0.1.1/vectara-cli/main.py
-drwxrwxrwx   0        0        0        0 2024-04-06 14:26:42.558384 vectara-cli-0.1.1/vectara_cli.egg-info/
--rw-rw-rw-   0        0        0    18570 2024-04-06 14:26:41.000000 vectara-cli-0.1.1/vectara_cli.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      305 2024-04-06 14:26:42.000000 vectara-cli-0.1.1/vectara_cli.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-06 14:26:41.000000 vectara-cli-0.1.1/vectara_cli.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2024-04-06 14:26:41.000000 vectara-cli-0.1.1/vectara_cli.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       84 2024-04-06 14:26:41.000000 vectara-cli-0.1.1/vectara_cli.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-06 14:26:41.000000 vectara-cli-0.1.1/vectara_cli.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-06 15:15:09.382781 vectara_cli-0.1.2/
+-rw-rw-rw-   0        0        0     1026 2024-04-05 13:30:44.000000 vectara_cli-0.1.2/LICENSE.md
+-rw-rw-rw-   0        0        0    18405 2024-04-06 15:15:09.381192 vectara_cli-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0    17239 2024-04-06 15:00:57.000000 vectara_cli-0.1.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-06 15:15:09.383291 vectara_cli-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1440 2024-04-06 15:10:59.000000 vectara_cli-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-06 15:15:09.364124 vectara_cli-0.1.2/vectara-cli/
+-rw-rw-rw-   0        0        0        0 2024-04-05 09:13:47.000000 vectara_cli-0.1.2/vectara-cli/__init__.py
+-rw-rw-rw-   0        0        0    17117 2024-04-05 10:27:08.000000 vectara_cli-0.1.2/vectara-cli/core.py
+-rw-rw-rw-   0        0        0     6100 2024-04-06 14:12:04.000000 vectara_cli-0.1.2/vectara-cli/main.py
+drwxrwxrwx   0        0        0        0 2024-04-06 15:15:09.378708 vectara_cli-0.1.2/vectara_cli.egg-info/
+-rw-rw-rw-   0        0        0    18405 2024-04-06 15:15:08.000000 vectara_cli-0.1.2/vectara_cli.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      305 2024-04-06 15:15:09.000000 vectara_cli-0.1.2/vectara_cli.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-06 15:15:08.000000 vectara_cli-0.1.2/vectara_cli.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2024-04-06 15:15:08.000000 vectara_cli-0.1.2/vectara_cli.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       83 2024-04-06 15:15:08.000000 vectara_cli-0.1.2/vectara_cli.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-06 15:15:08.000000 vectara_cli-0.1.2/vectara_cli.egg-info/top_level.txt
```

### Comparing `vectara-cli-0.1.1/LICENSE.md` & `vectara_cli-0.1.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `vectara-cli-0.1.1/PKG-INFO` & `vectara_cli-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: vectara-cli
-Version: 0.1.1
+Name: vectara_cli
+Version: 0.1.2
 Summary: A CLI tool for interacting with the Vectara platform, including advanced text processing and indexing features.
 Home-page: https://git.tonic-ai.com/releases/vectara-cli
 Author: Tonic-AI
 Author-email: team@tonic-ai.com
 License: MIT
 Keywords: vectara search-engine document-indexing text-analysis information-retrieval natural-language-processing cli-tool data-science machine-learning text-processing
 Classifier: Programming Language :: Python :: 3
@@ -18,27 +18,31 @@
 License-File: LICENSE.md
 Requires-Dist: requests
 Provides-Extra: advanced
 Requires-Dist: accelerate; extra == "advanced"
 Requires-Dist: torch>=1.8.0; extra == "advanced"
 Requires-Dist: transformers>=4.5.0; extra == "advanced"
 Requires-Dist: span_marker; extra == "advanced"
-Requires-Dist: spacey; extra == "advanced"
+Requires-Dist: spacy; extra == "advanced"
 
 # vectara-cli
 
 `vectara-cli` is a Python package designed to interact with the Vectara platform, providing a command-line interface (CLI) and a set of APIs for indexing and querying documents, managing corpora, and performing advanced text analysis and processing tasks. This package is particularly useful for developers and data scientists working on search and information retrieval applications.
 
 ## Features
 
 - Indexing text and documents into Vectara corpora.
 - Querying indexed documents.
 - Creating and deleting corpora.
 - Advanced text processing and analysis using pre-trained models (optional advanced package).
 
+## QuickStart
+
+get started with the [example_notebooks here](https://git.tonic-ai.com/releases/vectara-cli/examples/examples.ipynb) by downloading them and running them locally on any laptop.
+
 ## Installation
 
 ### Basic Installation
 
 The basic installation includes the core functionality for interacting with the Vectara platform.
 
 ```bash
@@ -51,20 +55,14 @@
 
 ```bash
 pip install vectara-cli[advanced]
 ```
 
 Ensure you have an appropriate PyTorch version installed for your system, especially if you're installing on a machine with GPU support. Refer to the [official PyTorch installation guide](https://pytorch.org/get-started/locally/) for more details.
 
-## Usage
-
-To include a section in the README of your PyPi package that describes how to use the CLI tool you've developed, you should provide clear, concise instructions covering installation, basic setup, and usage examples for each command. Below is a template you can adapt to fit your package's README file.
-
----
-
 ## Command Line Interface (CLI) Usage
 
 The `vectara-cli` provides a powerful command line interface for interacting with the Vectara platform, enabling tasks such as document indexing, querying, corpus management, and advanced text processing directly from your terminal. This section will guide you through the basics of using the `vectara-cli`.
 
 ### Installation
 
 Before using the CLI, ensure you have the package installed. You can install it directly from PyPi using pip:
@@ -126,40 +124,14 @@
 vectara-cli delete-corpus <corpus_id>
 ```
 
 - `<corpus_id>`: The ID of the corpus to delete.
 
 ### Advanced Commands
 
-#### Span Text Processing
-
-To process text using the Span model:
-
-```bash
-vectara-cli span-text "<text>" "<model_name>" "<model_type>"
-```
-
-- `<text>`: The text to process.
-- `<model_name>`: The name of the Span model to use.
-- `<model_type>`: The type of the Span model.
-
-#### Enhanced Batch Processing with NerdSpan
-
-To process and upload documents from a folder:
-
-```bash
-vectara-cli nerdspan-upsert-folder "<folder_path>" "<model_name>" "<model_type>"
-```
-
-- `<folder_path>`: The path to the folder containing documents to process and upload.
-- `<model_name>`: The name of the model to use for processing.
-- `<model_type>`: The type of the model.
-
-For more advanced processing and upsert operations, including using the Rebel model for complex document analysis and upload, refer to the specific command documentation provided with the CLI.
-
 ### Basic Usage
 
 #### Setting Up a Vectara Client
 
 First, initialize the Vectara client with your customer ID and API key. This client will be used for all subsequent operations.
 
 ```python
@@ -276,16 +248,39 @@
 
 To leverage the advanced text processing capabilities, ensure you have completed the advanced installation of `vectara-cli`. This includes the necessary dependencies for text analysis:
 
 ```bash
 pip install vectara-cli[advanced]
 ```
 
+#### Span Text Processing
+
+To process text using the Span model:
+
+```bash
+vectara-cli span-text "<text>" "<model_name>" "<model_type>"
+```
+
+- `<text>`: The text to process.
+- `<model_name>`: The name of the Span model to use.
+- `<model_type>`: The type of the Span model.
 
-### Commercial Advanced Useage
+#### Enhanced Batch Processing with NerdSpan
+
+To process and upload documents from a folder:
+
+```bash
+vectara-cli nerdspan-upsert-folder "<folder_path>" "<model_name>" "<model_type>"
+```
+
+- `<folder_path>`: The path to the folder containing documents to process and upload.
+- `<model_name>`: The name of the model to use for processing.
+- `<model_type>`: The type of the model.
+
+For more advanced processing and upsert operations, including using the Rebel model for complex document analysis and upload, refer to the specific command documentation provided with the CLI.
 
 ### Commercial Advanced Usage
 
 The commercial advanced features of `vectara-cli` enable users to leverage state-of-the-art text processing models for enriching document indexes with additional metadata. This enrichment process enhances the search and retrieval capabilities of the Vectara platform, providing more relevant and accurate results for complex queries.
 
 **Reference:** Aarsen, T. (2023). SpanMarker for Named Entity Recognition. Radboud University. Supervised by Prof. Dr. Fermin Moscoso del Prado Martin (fermin.moscoso-del-prado@ru.nl) and Dr. Daniel Vila Suero (daniel@argilla.io). Second assessor: Dr. Harrie Oosterhuis (harrie.oosterhuis@ru.nl).
 
@@ -301,15 +296,15 @@
 
   ```bash
   vectara-cli upload-enriched-text <corpus_id> <document_id> <model_name> "<text>"
   ```
 
   - `<corpus_id>`: The ID of the corpus where the document will be uploaded.
   - `<document_id>`: A unique identifier for the document.
-  - `<model_name>`: The name of the model used for text enrichment. `science` and `keyphrase`
+  - `<model_name>`: The name of the model used for text enrichment. `science` or `keyphrase`
   - `<text>`: The text content to be enriched and uploaded.
 
 - **Span Enhance Folder**
 
   To process and upload all documents within a folder, enhancing them using a specified model:
 
   ```bash
```

### Comparing `vectara-cli-0.1.1/README.md` & `vectara_cli-0.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,18 @@
 ## Features
 
 - Indexing text and documents into Vectara corpora.
 - Querying indexed documents.
 - Creating and deleting corpora.
 - Advanced text processing and analysis using pre-trained models (optional advanced package).
 
+## QuickStart
+
+get started with the [example_notebooks here](https://git.tonic-ai.com/releases/vectara-cli/examples/examples.ipynb) by downloading them and running them locally on any laptop.
+
 ## Installation
 
 ### Basic Installation
 
 The basic installation includes the core functionality for interacting with the Vectara platform.
 
 ```bash
@@ -25,20 +29,14 @@
 
 ```bash
 pip install vectara-cli[advanced]
 ```
 
 Ensure you have an appropriate PyTorch version installed for your system, especially if you're installing on a machine with GPU support. Refer to the [official PyTorch installation guide](https://pytorch.org/get-started/locally/) for more details.
 
-## Usage
-
-To include a section in the README of your PyPi package that describes how to use the CLI tool you've developed, you should provide clear, concise instructions covering installation, basic setup, and usage examples for each command. Below is a template you can adapt to fit your package's README file.
-
----
-
 ## Command Line Interface (CLI) Usage
 
 The `vectara-cli` provides a powerful command line interface for interacting with the Vectara platform, enabling tasks such as document indexing, querying, corpus management, and advanced text processing directly from your terminal. This section will guide you through the basics of using the `vectara-cli`.
 
 ### Installation
 
 Before using the CLI, ensure you have the package installed. You can install it directly from PyPi using pip:
@@ -100,40 +98,14 @@
 vectara-cli delete-corpus <corpus_id>
 ```
 
 - `<corpus_id>`: The ID of the corpus to delete.
 
 ### Advanced Commands
 
-#### Span Text Processing
-
-To process text using the Span model:
-
-```bash
-vectara-cli span-text "<text>" "<model_name>" "<model_type>"
-```
-
-- `<text>`: The text to process.
-- `<model_name>`: The name of the Span model to use.
-- `<model_type>`: The type of the Span model.
-
-#### Enhanced Batch Processing with NerdSpan
-
-To process and upload documents from a folder:
-
-```bash
-vectara-cli nerdspan-upsert-folder "<folder_path>" "<model_name>" "<model_type>"
-```
-
-- `<folder_path>`: The path to the folder containing documents to process and upload.
-- `<model_name>`: The name of the model to use for processing.
-- `<model_type>`: The type of the model.
-
-For more advanced processing and upsert operations, including using the Rebel model for complex document analysis and upload, refer to the specific command documentation provided with the CLI.
-
 ### Basic Usage
 
 #### Setting Up a Vectara Client
 
 First, initialize the Vectara client with your customer ID and API key. This client will be used for all subsequent operations.
 
 ```python
@@ -250,16 +222,39 @@
 
 To leverage the advanced text processing capabilities, ensure you have completed the advanced installation of `vectara-cli`. This includes the necessary dependencies for text analysis:
 
 ```bash
 pip install vectara-cli[advanced]
 ```
 
+#### Span Text Processing
+
+To process text using the Span model:
+
+```bash
+vectara-cli span-text "<text>" "<model_name>" "<model_type>"
+```
+
+- `<text>`: The text to process.
+- `<model_name>`: The name of the Span model to use.
+- `<model_type>`: The type of the Span model.
 
-### Commercial Advanced Useage
+#### Enhanced Batch Processing with NerdSpan
+
+To process and upload documents from a folder:
+
+```bash
+vectara-cli nerdspan-upsert-folder "<folder_path>" "<model_name>" "<model_type>"
+```
+
+- `<folder_path>`: The path to the folder containing documents to process and upload.
+- `<model_name>`: The name of the model to use for processing.
+- `<model_type>`: The type of the model.
+
+For more advanced processing and upsert operations, including using the Rebel model for complex document analysis and upload, refer to the specific command documentation provided with the CLI.
 
 ### Commercial Advanced Usage
 
 The commercial advanced features of `vectara-cli` enable users to leverage state-of-the-art text processing models for enriching document indexes with additional metadata. This enrichment process enhances the search and retrieval capabilities of the Vectara platform, providing more relevant and accurate results for complex queries.
 
 **Reference:** Aarsen, T. (2023). SpanMarker for Named Entity Recognition. Radboud University. Supervised by Prof. Dr. Fermin Moscoso del Prado Martin (fermin.moscoso-del-prado@ru.nl) and Dr. Daniel Vila Suero (daniel@argilla.io). Second assessor: Dr. Harrie Oosterhuis (harrie.oosterhuis@ru.nl).
 
@@ -275,15 +270,15 @@
 
   ```bash
   vectara-cli upload-enriched-text <corpus_id> <document_id> <model_name> "<text>"
   ```
 
   - `<corpus_id>`: The ID of the corpus where the document will be uploaded.
   - `<document_id>`: A unique identifier for the document.
-  - `<model_name>`: The name of the model used for text enrichment. `science` and `keyphrase`
+  - `<model_name>`: The name of the model used for text enrichment. `science` or `keyphrase`
   - `<text>`: The text content to be enriched and uploaded.
 
 - **Span Enhance Folder**
 
   To process and upload all documents within a folder, enhancing them using a specified model:
 
   ```bash
```

### Comparing `vectara-cli-0.1.1/setup.py` & `vectara_cli-0.1.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
  # ./setup.py
 
 from setuptools import setup, find_packages
 
 setup(
-    name="vectara-cli",
-    version="0.1.1",
+    name="vectara_cli",
+    version="0.1.2",
     author="Tonic-AI",
     author_email="team@tonic-ai.com",
     description="A CLI tool for interacting with the Vectara platform, including advanced text processing and indexing features.",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     url="https://git.tonic-ai.com/releases/vectara-cli",
     packages=find_packages(),
@@ -17,15 +17,15 @@
     ],
     extras_require={
         "advanced": [
             "accelerate",
             "torch>=1.8.0",
             "transformers>=4.5.0",
             "span_marker",
-            "spacey",
+            "spacy",
         ],
     },
     entry_points={
         'console_scripts': [
             'vectara-cli=vectara_cli.core:VectaraClient',
         ],
     },
```

### Comparing `vectara-cli-0.1.1/vectara-cli/core.py` & `vectara_cli-0.1.2/vectara-cli/core.py`

 * *Files identical despite different names*

### Comparing `vectara-cli-0.1.1/vectara-cli/main.py` & `vectara_cli-0.1.2/vectara-cli/main.py`

 * *Files identical despite different names*

### Comparing `vectara-cli-0.1.1/vectara_cli.egg-info/PKG-INFO` & `vectara_cli-0.1.2/vectara_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: vectara-cli
-Version: 0.1.1
+Name: vectara_cli
+Version: 0.1.2
 Summary: A CLI tool for interacting with the Vectara platform, including advanced text processing and indexing features.
 Home-page: https://git.tonic-ai.com/releases/vectara-cli
 Author: Tonic-AI
 Author-email: team@tonic-ai.com
 License: MIT
 Keywords: vectara search-engine document-indexing text-analysis information-retrieval natural-language-processing cli-tool data-science machine-learning text-processing
 Classifier: Programming Language :: Python :: 3
@@ -18,27 +18,31 @@
 License-File: LICENSE.md
 Requires-Dist: requests
 Provides-Extra: advanced
 Requires-Dist: accelerate; extra == "advanced"
 Requires-Dist: torch>=1.8.0; extra == "advanced"
 Requires-Dist: transformers>=4.5.0; extra == "advanced"
 Requires-Dist: span_marker; extra == "advanced"
-Requires-Dist: spacey; extra == "advanced"
+Requires-Dist: spacy; extra == "advanced"
 
 # vectara-cli
 
 `vectara-cli` is a Python package designed to interact with the Vectara platform, providing a command-line interface (CLI) and a set of APIs for indexing and querying documents, managing corpora, and performing advanced text analysis and processing tasks. This package is particularly useful for developers and data scientists working on search and information retrieval applications.
 
 ## Features
 
 - Indexing text and documents into Vectara corpora.
 - Querying indexed documents.
 - Creating and deleting corpora.
 - Advanced text processing and analysis using pre-trained models (optional advanced package).
 
+## QuickStart
+
+get started with the [example_notebooks here](https://git.tonic-ai.com/releases/vectara-cli/examples/examples.ipynb) by downloading them and running them locally on any laptop.
+
 ## Installation
 
 ### Basic Installation
 
 The basic installation includes the core functionality for interacting with the Vectara platform.
 
 ```bash
@@ -51,20 +55,14 @@
 
 ```bash
 pip install vectara-cli[advanced]
 ```
 
 Ensure you have an appropriate PyTorch version installed for your system, especially if you're installing on a machine with GPU support. Refer to the [official PyTorch installation guide](https://pytorch.org/get-started/locally/) for more details.
 
-## Usage
-
-To include a section in the README of your PyPi package that describes how to use the CLI tool you've developed, you should provide clear, concise instructions covering installation, basic setup, and usage examples for each command. Below is a template you can adapt to fit your package's README file.
-
----
-
 ## Command Line Interface (CLI) Usage
 
 The `vectara-cli` provides a powerful command line interface for interacting with the Vectara platform, enabling tasks such as document indexing, querying, corpus management, and advanced text processing directly from your terminal. This section will guide you through the basics of using the `vectara-cli`.
 
 ### Installation
 
 Before using the CLI, ensure you have the package installed. You can install it directly from PyPi using pip:
@@ -126,40 +124,14 @@
 vectara-cli delete-corpus <corpus_id>
 ```
 
 - `<corpus_id>`: The ID of the corpus to delete.
 
 ### Advanced Commands
 
-#### Span Text Processing
-
-To process text using the Span model:
-
-```bash
-vectara-cli span-text "<text>" "<model_name>" "<model_type>"
-```
-
-- `<text>`: The text to process.
-- `<model_name>`: The name of the Span model to use.
-- `<model_type>`: The type of the Span model.
-
-#### Enhanced Batch Processing with NerdSpan
-
-To process and upload documents from a folder:
-
-```bash
-vectara-cli nerdspan-upsert-folder "<folder_path>" "<model_name>" "<model_type>"
-```
-
-- `<folder_path>`: The path to the folder containing documents to process and upload.
-- `<model_name>`: The name of the model to use for processing.
-- `<model_type>`: The type of the model.
-
-For more advanced processing and upsert operations, including using the Rebel model for complex document analysis and upload, refer to the specific command documentation provided with the CLI.
-
 ### Basic Usage
 
 #### Setting Up a Vectara Client
 
 First, initialize the Vectara client with your customer ID and API key. This client will be used for all subsequent operations.
 
 ```python
@@ -276,16 +248,39 @@
 
 To leverage the advanced text processing capabilities, ensure you have completed the advanced installation of `vectara-cli`. This includes the necessary dependencies for text analysis:
 
 ```bash
 pip install vectara-cli[advanced]
 ```
 
+#### Span Text Processing
+
+To process text using the Span model:
+
+```bash
+vectara-cli span-text "<text>" "<model_name>" "<model_type>"
+```
+
+- `<text>`: The text to process.
+- `<model_name>`: The name of the Span model to use.
+- `<model_type>`: The type of the Span model.
 
-### Commercial Advanced Useage
+#### Enhanced Batch Processing with NerdSpan
+
+To process and upload documents from a folder:
+
+```bash
+vectara-cli nerdspan-upsert-folder "<folder_path>" "<model_name>" "<model_type>"
+```
+
+- `<folder_path>`: The path to the folder containing documents to process and upload.
+- `<model_name>`: The name of the model to use for processing.
+- `<model_type>`: The type of the model.
+
+For more advanced processing and upsert operations, including using the Rebel model for complex document analysis and upload, refer to the specific command documentation provided with the CLI.
 
 ### Commercial Advanced Usage
 
 The commercial advanced features of `vectara-cli` enable users to leverage state-of-the-art text processing models for enriching document indexes with additional metadata. This enrichment process enhances the search and retrieval capabilities of the Vectara platform, providing more relevant and accurate results for complex queries.
 
 **Reference:** Aarsen, T. (2023). SpanMarker for Named Entity Recognition. Radboud University. Supervised by Prof. Dr. Fermin Moscoso del Prado Martin (fermin.moscoso-del-prado@ru.nl) and Dr. Daniel Vila Suero (daniel@argilla.io). Second assessor: Dr. Harrie Oosterhuis (harrie.oosterhuis@ru.nl).
 
@@ -301,15 +296,15 @@
 
   ```bash
   vectara-cli upload-enriched-text <corpus_id> <document_id> <model_name> "<text>"
   ```
 
   - `<corpus_id>`: The ID of the corpus where the document will be uploaded.
   - `<document_id>`: A unique identifier for the document.
-  - `<model_name>`: The name of the model used for text enrichment. `science` and `keyphrase`
+  - `<model_name>`: The name of the model used for text enrichment. `science` or `keyphrase`
   - `<text>`: The text content to be enriched and uploaded.
 
 - **Span Enhance Folder**
 
   To process and upload all documents within a folder, enhancing them using a specified model:
 
   ```bash
```

