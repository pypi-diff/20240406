# Comparing `tmp/vectara-cli-0.1.4.tar.gz` & `tmp/vectara-cli-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vectara-cli-0.1.4.tar", last modified: Sat Apr  6 16:17:50 2024, max compression
+gzip compressed data, was "vectara-cli-0.1.5.tar", last modified: Sat Apr  6 18:14:29 2024, max compression
```

## Comparing `vectara-cli-0.1.4.tar` & `vectara-cli-0.1.5.tar`

### file list

```diff
@@ -1,17 +1,40 @@
-drwxrwxrwx   0        0        0        0 2024-04-06 16:17:50.599243 vectara-cli-0.1.4/
--rw-rw-rw-   0        0        0     1026 2024-04-05 13:30:44.000000 vectara-cli-0.1.4/LICENSE.md
--rw-rw-rw-   0        0        0    20274 2024-04-06 16:17:50.597238 vectara-cli-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0    19108 2024-04-06 16:09:23.000000 vectara-cli-0.1.4/README.md
--rw-rw-rw-   0        0        0       42 2024-04-06 16:17:50.599739 vectara-cli-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0     1427 2024-04-06 15:48:13.000000 vectara-cli-0.1.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-06 16:17:50.580196 vectara-cli-0.1.4/vectara_cli/
--rw-rw-rw-   0        0        0        0 2024-04-05 09:13:47.000000 vectara-cli-0.1.4/vectara_cli/__init__.py
--rw-rw-rw-   0        0        0    17802 2024-04-06 16:04:27.000000 vectara-cli-0.1.4/vectara_cli/core.py
--rw-rw-rw-   0        0        0     6335 2024-04-06 16:04:09.000000 vectara-cli-0.1.4/vectara_cli/main.py
-drwxrwxrwx   0        0        0        0 2024-04-06 16:17:50.594240 vectara-cli-0.1.4/vectara_cli.egg-info/
--rw-rw-rw-   0        0        0    20274 2024-04-06 16:17:49.000000 vectara-cli-0.1.4/vectara_cli.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      305 2024-04-06 16:17:50.000000 vectara-cli-0.1.4/vectara_cli.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-06 16:17:49.000000 vectara-cli-0.1.4/vectara_cli.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2024-04-06 16:17:49.000000 vectara-cli-0.1.4/vectara_cli.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       83 2024-04-06 16:17:49.000000 vectara-cli-0.1.4/vectara_cli.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-06 16:17:49.000000 vectara-cli-0.1.4/vectara_cli.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-06 18:14:29.890507 vectara-cli-0.1.5/
+-rw-rw-rw-   0        0        0    33954 2024-04-06 18:07:05.000000 vectara-cli-0.1.5/LICENSE.md
+-rw-rw-rw-   0        0        0    22346 2024-04-06 18:14:29.888025 vectara-cli-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0    21180 2024-04-06 18:07:05.000000 vectara-cli-0.1.5/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-06 18:14:29.891015 vectara-cli-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1427 2024-04-06 18:07:05.000000 vectara-cli-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-06 18:14:29.834889 vectara-cli-0.1.5/vectara_cli/
+-rw-rw-rw-   0        0        0        0 2024-04-05 09:13:47.000000 vectara-cli-0.1.5/vectara_cli/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-06 18:14:29.849896 vectara-cli-0.1.5/vectara_cli/advanced/
+-rw-rw-rw-   0        0        0        0 2024-04-06 18:07:05.000000 vectara-cli-0.1.5/vectara_cli/advanced/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-06 18:14:29.852395 vectara-cli-0.1.5/vectara_cli/advanced/commercial/
+-rw-rw-rw-   0        0        0        0 2024-04-06 18:07:05.000000 vectara-cli-0.1.5/vectara_cli/advanced/commercial/__init__.py
+-rw-rw-rw-   0        0        0     7379 2024-04-06 14:04:07.000000 vectara-cli-0.1.5/vectara_cli/advanced/commercial/enterprise.py
+drwxrwxrwx   0        0        0        0 2024-04-06 18:14:29.857987 vectara-cli-0.1.5/vectara_cli/advanced/noncommercial/
+-rw-rw-rw-   0        0        0        0 2024-04-05 09:13:47.000000 vectara-cli-0.1.5/vectara_cli/advanced/noncommercial/__init__.py
+-rw-rw-rw-   0        0        0     6061 2024-04-06 18:07:05.000000 vectara-cli-0.1.5/vectara_cli/advanced/noncommercial/nerdspan.py
+-rw-rw-rw-   0        0        0     8476 2024-04-06 18:07:05.000000 vectara-cli-0.1.5/vectara_cli/advanced/noncommercial/rebel.py
+drwxrwxrwx   0        0        0        0 2024-04-06 18:14:29.883015 vectara-cli-0.1.5/vectara_cli/commands/
+-rw-rw-rw-   0        0        0        0 2024-04-06 18:07:05.000000 vectara-cli-0.1.5/vectara_cli/commands/__init__.py
+-rw-rw-rw-   0        0        0      719 2024-04-06 18:07:05.000000 vectara-cli-0.1.5/vectara_cli/commands/create_corpus.py
+-rw-rw-rw-   0        0        0      752 2024-04-06 18:07:05.000000 vectara-cli-0.1.5/vectara_cli/commands/delete_corpus.py
+-rw-rw-rw-   0        0        0     1027 2024-04-06 18:07:05.000000 vectara-cli-0.1.5/vectara_cli/commands/index_document.py
+-rw-rw-rw-   0        0        0     1034 2024-04-06 18:07:05.000000 vectara-cli-0.1.5/vectara_cli/commands/nerdspan_upsert_folder.py
+-rw-rw-rw-   0        0        0      683 2024-04-06 18:07:05.000000 vectara-cli-0.1.5/vectara_cli/commands/query.py
+-rw-rw-rw-   0        0        0     1055 2024-04-06 18:07:05.000000 vectara-cli-0.1.5/vectara_cli/commands/rebel_upsert_folder.py
+-rw-rw-rw-   0        0        0      419 2024-04-06 18:07:05.000000 vectara-cli-0.1.5/vectara_cli/commands/set_api_keys.py
+-rw-rw-rw-   0        0        0      773 2024-04-06 18:07:05.000000 vectara-cli-0.1.5/vectara_cli/commands/span-text.py
+-rw-rw-rw-   0        0        0     1119 2024-04-06 18:07:05.000000 vectara-cli-0.1.5/vectara_cli/commands/span_enhance_folder.py
+-rw-rw-rw-   0        0        0      983 2024-04-06 18:07:05.000000 vectara-cli-0.1.5/vectara_cli/commands/upload_document.py
+-rw-rw-rw-   0        0        0      932 2024-04-06 18:07:05.000000 vectara-cli-0.1.5/vectara_cli/commands/upload_enriched_text.py
+-rw-rw-rw-   0        0        0      719 2024-04-06 18:07:05.000000 vectara-cli-0.1.5/vectara_cli/config_manager.py
+-rw-rw-rw-   0        0        0    17117 2024-04-06 18:07:05.000000 vectara-cli-0.1.5/vectara_cli/core.py
+-rw-rw-rw-   0        0        0     2933 2024-04-06 18:07:05.000000 vectara-cli-0.1.5/vectara_cli/main.py
+drwxrwxrwx   0        0        0        0 2024-04-06 18:14:29.885505 vectara-cli-0.1.5/vectara_cli.egg-info/
+-rw-rw-rw-   0        0        0    22346 2024-04-06 18:14:29.000000 vectara-cli-0.1.5/vectara_cli.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1065 2024-04-06 18:14:29.000000 vectara-cli-0.1.5/vectara_cli.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-06 18:14:29.000000 vectara-cli-0.1.5/vectara_cli.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2024-04-06 18:14:29.000000 vectara-cli-0.1.5/vectara_cli.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       83 2024-04-06 18:14:29.000000 vectara-cli-0.1.5/vectara_cli.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-06 18:14:29.000000 vectara-cli-0.1.5/vectara_cli.egg-info/top_level.txt
```

### Comparing `vectara-cli-0.1.4/PKG-INFO` & `vectara-cli-0.1.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vectara-cli
-Version: 0.1.4
+Version: 0.1.5
 Summary: A CLI tool for interacting with the Vectara platform, including advanced text processing and indexing features.
 Home-page: https://git.tonic-ai.com/releases/vectara-cli
 Author: Tonic-AI
 Author-email: team@tonic-ai.com
 License: MIT
 Keywords: vectara search-engine document-indexing text-analysis information-retrieval natural-language-processing cli-tool data-science machine-learning text-processing
 Classifier: Programming Language :: Python :: 3
@@ -66,14 +66,75 @@
 ### Installation
 
 Before using the CLI, ensure you have the package installed. You can install it directly from PyPi using pip:
 
 ```bash
 pip install vectara-cli
 ```
+
+### Optional: Conda Virtual Environment Setup
+
+Conda is an open-source package management system and environment management system that runs on Windows, macOS, and Linux. It allows you to install, run, and update packages and their dependencies. To set up this project using Conda, follow the steps below:
+
+#### Prerequisites
+
+- Ensure that you have Conda installed on your system. If you do not have Conda installed, you can download it from the [official Conda website](https://www.anaconda.com/products/distribution).
+
+#### Creating a Conda Environment
+
+1. Open your terminal (or Anaconda Prompt on Windows).
+2. Navigate to the project directory where the `environment.yml` file is located.
+3. Create a new Conda environment by running the following command:
+
+   ```bash
+   conda env create -f environment.yml
+   ```
+
+   This will create a new environment with the name specified in the `environment.yml` file and install all the required packages.
+
+#### Activating the Environment
+
+Once the environment is created, you can activate it using the following command:
+
+```bash
+conda activate <env_name>
+```
+
+Replace `<env_name>` with the name of your Conda environment.
+
+#### Deactivating the Environment
+
+When you are done working on the project, you can deactivate the Conda environment by running:
+
+```bash
+conda deactivate
+```
+
+#### Updating the Environment
+
+If you need to update the environment based on the `environment.yml` file, use the following command:
+
+```bash
+conda env update -f environment.yml --prune
+```
+
+This will update the environment with any new dependencies specified in the `environment.yml` file.
+
+#### Removing the Environment
+
+If you wish to remove the Conda environment, you can do so with the following command:
+
+```bash
+conda env remove -n <env_name>
+```
+
+Again, replace `<env_name>` with the name of your Conda environment.
+
+By following these steps, you can manage your project's dependencies in an isolated environment using Conda.
+
 ### Configuration
 
 #### Setting Credentials via CLI Commands
 
 The `vectara-cli` tool now supports a convenient feature for setting your Vectara customer ID and API key directly through the command line. This method utilizes a command specifically designed for securely storing your credentials, making it easier to manage your Vectara configuration without manually setting environment variables or directly embedding your credentials in your scripts.
 
 #### Using the `set-api-keys` Command
@@ -395,17 +456,16 @@
 
 This example showcases how to enrich text with additional metadata using the `EnterpriseSpan` class and upload it to a specified corpus in Vectara. By leveraging advanced models for text processing, users can significantly enhance the quality and relevance of their search and retrieval operations on the Vectara platform.
 
 ### Non-Commercial Advanced Usage
 
 The advanced features allow you to enrich your indexes with additional information automatically. This should produce better results for retrieval.
 
-![mRebel](<Screenshot 2024-04-05 112158.png>)
-
-![Span Models for Named Entity Recognition](image.png)
+![mRebel](/res/images/Screenshot_2024-04-05_112158.png)
+![Span Models for Named Entity Recognition](/res/images/Screenshot_2024-04-05_112142.png)
 
 ### Non-Commercial Advanced Usage Using Span Models
 
 The `vectara-cli` package extends its functionality through the advanced usage of Span Models, enabling users to perform sophisticated text analysis and entity recognition tasks. This feature is particularly beneficial for non-commercial applications that require deep understanding and processing of textual data.
 
 The `Span` class supports processing and indexing documents from a folder, enabling batch operations for efficiency. This feature allows for the automatic extraction of entities from multiple documents, which are then indexed into specified corpora with enriched metadata.
```

### Comparing `vectara-cli-0.1.4/README.md` & `vectara-cli-0.1.5/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -40,14 +40,75 @@
 ### Installation
 
 Before using the CLI, ensure you have the package installed. You can install it directly from PyPi using pip:
 
 ```bash
 pip install vectara-cli
 ```
+
+### Optional: Conda Virtual Environment Setup
+
+Conda is an open-source package management system and environment management system that runs on Windows, macOS, and Linux. It allows you to install, run, and update packages and their dependencies. To set up this project using Conda, follow the steps below:
+
+#### Prerequisites
+
+- Ensure that you have Conda installed on your system. If you do not have Conda installed, you can download it from the [official Conda website](https://www.anaconda.com/products/distribution).
+
+#### Creating a Conda Environment
+
+1. Open your terminal (or Anaconda Prompt on Windows).
+2. Navigate to the project directory where the `environment.yml` file is located.
+3. Create a new Conda environment by running the following command:
+
+   ```bash
+   conda env create -f environment.yml
+   ```
+
+   This will create a new environment with the name specified in the `environment.yml` file and install all the required packages.
+
+#### Activating the Environment
+
+Once the environment is created, you can activate it using the following command:
+
+```bash
+conda activate <env_name>
+```
+
+Replace `<env_name>` with the name of your Conda environment.
+
+#### Deactivating the Environment
+
+When you are done working on the project, you can deactivate the Conda environment by running:
+
+```bash
+conda deactivate
+```
+
+#### Updating the Environment
+
+If you need to update the environment based on the `environment.yml` file, use the following command:
+
+```bash
+conda env update -f environment.yml --prune
+```
+
+This will update the environment with any new dependencies specified in the `environment.yml` file.
+
+#### Removing the Environment
+
+If you wish to remove the Conda environment, you can do so with the following command:
+
+```bash
+conda env remove -n <env_name>
+```
+
+Again, replace `<env_name>` with the name of your Conda environment.
+
+By following these steps, you can manage your project's dependencies in an isolated environment using Conda.
+
 ### Configuration
 
 #### Setting Credentials via CLI Commands
 
 The `vectara-cli` tool now supports a convenient feature for setting your Vectara customer ID and API key directly through the command line. This method utilizes a command specifically designed for securely storing your credentials, making it easier to manage your Vectara configuration without manually setting environment variables or directly embedding your credentials in your scripts.
 
 #### Using the `set-api-keys` Command
@@ -369,17 +430,16 @@
 
 This example showcases how to enrich text with additional metadata using the `EnterpriseSpan` class and upload it to a specified corpus in Vectara. By leveraging advanced models for text processing, users can significantly enhance the quality and relevance of their search and retrieval operations on the Vectara platform.
 
 ### Non-Commercial Advanced Usage
 
 The advanced features allow you to enrich your indexes with additional information automatically. This should produce better results for retrieval.
 
-![mRebel](<Screenshot 2024-04-05 112158.png>)
-
-![Span Models for Named Entity Recognition](image.png)
+![mRebel](/res/images/Screenshot_2024-04-05_112158.png)
+![Span Models for Named Entity Recognition](/res/images/Screenshot_2024-04-05_112142.png)
 
 ### Non-Commercial Advanced Usage Using Span Models
 
 The `vectara-cli` package extends its functionality through the advanced usage of Span Models, enabling users to perform sophisticated text analysis and entity recognition tasks. This feature is particularly beneficial for non-commercial applications that require deep understanding and processing of textual data.
 
 The `Span` class supports processing and indexing documents from a folder, enabling batch operations for efficiency. This feature allows for the automatic extraction of entities from multiple documents, which are then indexed into specified corpora with enriched metadata.
```

### Comparing `vectara-cli-0.1.4/setup.py` & `vectara-cli-0.1.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
  # ./setup.py
 
 from setuptools import setup, find_packages
 
 setup(
     name="vectara-cli",
-    version="0.1.4",
+    version="0.1.5",
     author="Tonic-AI",
     author_email="team@tonic-ai.com",
     description="A CLI tool for interacting with the Vectara platform, including advanced text processing and indexing features.",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     url="https://git.tonic-ai.com/releases/vectara-cli",
     packages=find_packages(),
```

### Comparing `vectara-cli-0.1.4/vectara_cli/core.py` & `vectara-cli-0.1.5/vectara_cli/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,14 @@
 # ./vectara-cli/core.py
 
 import requests
 import json
 import os
 import logging
 
-class ConfigManager:
-    @staticmethod
-    def set_api_keys(customer_id, api_key):
-        """Sets the customer ID and API key as environment variables."""
-        os.environ['VECTARA_CUSTOMER_ID'] = customer_id
-        os.environ['VECTARA_API_KEY'] = api_key
-
-    @staticmethod
-    def get_api_keys():
-        """Retrieves the customer ID and API key from environment variables."""
-        customer_id = os.getenv('VECTARA_CUSTOMER_ID')
-        api_key = os.getenv('VECTARA_API_KEY')
-        if not customer_id or not api_key:
-            raise ValueError("API keys are not set. Please set them using the 'set-api-keys' command.")
-        return customer_id, api_key
-
 class VectaraClient:
     def __init__(self, customer_id, api_key):
         self.base_url = "https://api.vectara.io"
         self.headers = {
             "Content-Type": "application/json",
             "Accept": "application/json",
             "customer-id": customer_id,
```

### Comparing `vectara-cli-0.1.4/vectara_cli.egg-info/PKG-INFO` & `vectara-cli-0.1.5/vectara_cli.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vectara-cli
-Version: 0.1.4
+Version: 0.1.5
 Summary: A CLI tool for interacting with the Vectara platform, including advanced text processing and indexing features.
 Home-page: https://git.tonic-ai.com/releases/vectara-cli
 Author: Tonic-AI
 Author-email: team@tonic-ai.com
 License: MIT
 Keywords: vectara search-engine document-indexing text-analysis information-retrieval natural-language-processing cli-tool data-science machine-learning text-processing
 Classifier: Programming Language :: Python :: 3
@@ -66,14 +66,75 @@
 ### Installation
 
 Before using the CLI, ensure you have the package installed. You can install it directly from PyPi using pip:
 
 ```bash
 pip install vectara-cli
 ```
+
+### Optional: Conda Virtual Environment Setup
+
+Conda is an open-source package management system and environment management system that runs on Windows, macOS, and Linux. It allows you to install, run, and update packages and their dependencies. To set up this project using Conda, follow the steps below:
+
+#### Prerequisites
+
+- Ensure that you have Conda installed on your system. If you do not have Conda installed, you can download it from the [official Conda website](https://www.anaconda.com/products/distribution).
+
+#### Creating a Conda Environment
+
+1. Open your terminal (or Anaconda Prompt on Windows).
+2. Navigate to the project directory where the `environment.yml` file is located.
+3. Create a new Conda environment by running the following command:
+
+   ```bash
+   conda env create -f environment.yml
+   ```
+
+   This will create a new environment with the name specified in the `environment.yml` file and install all the required packages.
+
+#### Activating the Environment
+
+Once the environment is created, you can activate it using the following command:
+
+```bash
+conda activate <env_name>
+```
+
+Replace `<env_name>` with the name of your Conda environment.
+
+#### Deactivating the Environment
+
+When you are done working on the project, you can deactivate the Conda environment by running:
+
+```bash
+conda deactivate
+```
+
+#### Updating the Environment
+
+If you need to update the environment based on the `environment.yml` file, use the following command:
+
+```bash
+conda env update -f environment.yml --prune
+```
+
+This will update the environment with any new dependencies specified in the `environment.yml` file.
+
+#### Removing the Environment
+
+If you wish to remove the Conda environment, you can do so with the following command:
+
+```bash
+conda env remove -n <env_name>
+```
+
+Again, replace `<env_name>` with the name of your Conda environment.
+
+By following these steps, you can manage your project's dependencies in an isolated environment using Conda.
+
 ### Configuration
 
 #### Setting Credentials via CLI Commands
 
 The `vectara-cli` tool now supports a convenient feature for setting your Vectara customer ID and API key directly through the command line. This method utilizes a command specifically designed for securely storing your credentials, making it easier to manage your Vectara configuration without manually setting environment variables or directly embedding your credentials in your scripts.
 
 #### Using the `set-api-keys` Command
@@ -395,17 +456,16 @@
 
 This example showcases how to enrich text with additional metadata using the `EnterpriseSpan` class and upload it to a specified corpus in Vectara. By leveraging advanced models for text processing, users can significantly enhance the quality and relevance of their search and retrieval operations on the Vectara platform.
 
 ### Non-Commercial Advanced Usage
 
 The advanced features allow you to enrich your indexes with additional information automatically. This should produce better results for retrieval.
 
-![mRebel](<Screenshot 2024-04-05 112158.png>)
-
-![Span Models for Named Entity Recognition](image.png)
+![mRebel](/res/images/Screenshot_2024-04-05_112158.png)
+![Span Models for Named Entity Recognition](/res/images/Screenshot_2024-04-05_112142.png)
 
 ### Non-Commercial Advanced Usage Using Span Models
 
 The `vectara-cli` package extends its functionality through the advanced usage of Span Models, enabling users to perform sophisticated text analysis and entity recognition tasks. This feature is particularly beneficial for non-commercial applications that require deep understanding and processing of textual data.
 
 The `Span` class supports processing and indexing documents from a folder, enabling batch operations for efficiency. This feature allows for the automatic extraction of entities from multiple documents, which are then indexed into specified corpora with enriched metadata.
```

