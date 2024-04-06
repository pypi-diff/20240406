# Comparing `tmp/vectara-cli-0.1.3.tar.gz` & `tmp/vectara-cli-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vectara-cli-0.1.3.tar", last modified: Sat Apr  6 15:25:28 2024, max compression
+gzip compressed data, was "vectara-cli-0.1.4.tar", last modified: Sat Apr  6 16:17:50 2024, max compression
```

## Comparing `vectara-cli-0.1.3.tar` & `vectara-cli-0.1.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-06 15:25:28.590633 vectara-cli-0.1.3/
--rw-rw-rw-   0        0        0     1026 2024-04-05 13:30:44.000000 vectara-cli-0.1.3/LICENSE.md
--rw-rw-rw-   0        0        0    18405 2024-04-06 15:25:28.588577 vectara-cli-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0    17239 2024-04-06 15:00:57.000000 vectara-cli-0.1.3/README.md
--rw-rw-rw-   0        0        0       42 2024-04-06 15:25:28.590633 vectara-cli-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0     1440 2024-04-06 15:25:19.000000 vectara-cli-0.1.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-06 15:25:28.577530 vectara-cli-0.1.3/vectara-cli/
--rw-rw-rw-   0        0        0        0 2024-04-05 09:13:47.000000 vectara-cli-0.1.3/vectara-cli/__init__.py
--rw-rw-rw-   0        0        0    17117 2024-04-05 10:27:08.000000 vectara-cli-0.1.3/vectara-cli/core.py
--rw-rw-rw-   0        0        0     6100 2024-04-06 14:12:04.000000 vectara-cli-0.1.3/vectara-cli/main.py
-drwxrwxrwx   0        0        0        0 2024-04-06 15:25:28.586574 vectara-cli-0.1.3/vectara_cli.egg-info/
--rw-rw-rw-   0        0        0    18405 2024-04-06 15:25:27.000000 vectara-cli-0.1.3/vectara_cli.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      305 2024-04-06 15:25:28.000000 vectara-cli-0.1.3/vectara_cli.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-06 15:25:27.000000 vectara-cli-0.1.3/vectara_cli.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2024-04-06 15:25:27.000000 vectara-cli-0.1.3/vectara_cli.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       83 2024-04-06 15:25:27.000000 vectara-cli-0.1.3/vectara_cli.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-06 15:25:27.000000 vectara-cli-0.1.3/vectara_cli.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-06 16:17:50.599243 vectara-cli-0.1.4/
+-rw-rw-rw-   0        0        0     1026 2024-04-05 13:30:44.000000 vectara-cli-0.1.4/LICENSE.md
+-rw-rw-rw-   0        0        0    20274 2024-04-06 16:17:50.597238 vectara-cli-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0    19108 2024-04-06 16:09:23.000000 vectara-cli-0.1.4/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-06 16:17:50.599739 vectara-cli-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     1427 2024-04-06 15:48:13.000000 vectara-cli-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-06 16:17:50.580196 vectara-cli-0.1.4/vectara_cli/
+-rw-rw-rw-   0        0        0        0 2024-04-05 09:13:47.000000 vectara-cli-0.1.4/vectara_cli/__init__.py
+-rw-rw-rw-   0        0        0    17802 2024-04-06 16:04:27.000000 vectara-cli-0.1.4/vectara_cli/core.py
+-rw-rw-rw-   0        0        0     6335 2024-04-06 16:04:09.000000 vectara-cli-0.1.4/vectara_cli/main.py
+drwxrwxrwx   0        0        0        0 2024-04-06 16:17:50.594240 vectara-cli-0.1.4/vectara_cli.egg-info/
+-rw-rw-rw-   0        0        0    20274 2024-04-06 16:17:49.000000 vectara-cli-0.1.4/vectara_cli.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      305 2024-04-06 16:17:50.000000 vectara-cli-0.1.4/vectara_cli.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-06 16:17:49.000000 vectara-cli-0.1.4/vectara_cli.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2024-04-06 16:17:49.000000 vectara-cli-0.1.4/vectara_cli.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       83 2024-04-06 16:17:49.000000 vectara-cli-0.1.4/vectara_cli.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-06 16:17:49.000000 vectara-cli-0.1.4/vectara_cli.egg-info/top_level.txt
```

### Comparing `vectara-cli-0.1.3/LICENSE.md` & `vectara-cli-0.1.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `vectara-cli-0.1.3/PKG-INFO` & `vectara-cli-0.1.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,7 @@
-Metadata-Version: 2.1
-Name: vectara-cli
-Version: 0.1.3
-Summary: A CLI tool for interacting with the Vectara platform, including advanced text processing and indexing features.
-Home-page: https://git.tonic-ai.com/releases/vectara-cli
-Author: Tonic-AI
-Author-email: team@tonic-ai.com
-License: MIT
-Keywords: vectara search-engine document-indexing text-analysis information-retrieval natural-language-processing cli-tool data-science machine-learning text-processing
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Utilities
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-Requires-Dist: requests
-Provides-Extra: advanced
-Requires-Dist: accelerate; extra == "advanced"
-Requires-Dist: torch>=1.8.0; extra == "advanced"
-Requires-Dist: transformers>=4.5.0; extra == "advanced"
-Requires-Dist: span_marker; extra == "advanced"
-Requires-Dist: spacy; extra == "advanced"
-
 # vectara-cli
 
 `vectara-cli` is a Python package designed to interact with the Vectara platform, providing a command-line interface (CLI) and a set of APIs for indexing and querying documents, managing corpora, and performing advanced text analysis and processing tasks. This package is particularly useful for developers and data scientists working on search and information retrieval applications.
 
 ## Features
 
 - Indexing text and documents into Vectara corpora.
@@ -64,25 +38,69 @@
 The `vectara-cli` provides a powerful command line interface for interacting with the Vectara platform, enabling tasks such as document indexing, querying, corpus management, and advanced text processing directly from your terminal. This section will guide you through the basics of using the `vectara-cli`.
 
 ### Installation
 
 Before using the CLI, ensure you have the package installed. You can install it directly from PyPi using pip:
 
 ```bash
-pip install your-package-name
+pip install vectara-cli
 ```
+### Configuration
 
-Replace `your-package-name` with the actual name of your package on PyPi.
+#### Setting Credentials via CLI Commands
 
-### Configuration
+The `vectara-cli` tool now supports a convenient feature for setting your Vectara customer ID and API key directly through the command line. This method utilizes a command specifically designed for securely storing your credentials, making it easier to manage your Vectara configuration without manually setting environment variables or directly embedding your credentials in your scripts.
+
+#### Using the `set-api-keys` Command
+
+To set your Vectara customer ID and API key using the `vectara-cli`, you can use the `set-api-keys` command. This command stores your credentials securely, allowing `vectara-cli` to automatically use them for authentication in future operations.
+
+- **Syntax:** The command follows this simple syntax:
 
-To use the CLI, you need to configure your Vectara customer ID and API key. These can be set as environment variables or directly within the CLI commands as shown in the examples below.
+```bash
+vectara-cli set-api-keys <customer_id> <api_key>
+```
+
+Replace `<customer_id>` with your Vectara customer ID and `<api_key>` with your Vectara API key.
+
+- **Example:**
+
+```bash
+vectara-cli set-api-keys 123456789 abcdefghijklmnopqrstuvwxyz
+```
+
+After executing this command, you will see a confirmation message indicating that your API keys have been set successfully.
+
+#### Windows
+
+For Windows users, you can also set environment variables through the Command Prompt or PowerShell, or via the System Properties window.
+
+- **Command Prompt:**
+
+```cmd
+setx VECTARA_CUSTOMER_ID "your_customer_id"
+setx VECTARA_API_KEY "your_api_key"
+```
+
+- **PowerShell:**
+
+```powershell
+[System.Environment]::SetEnvironmentVariable('VECTARA_CUSTOMER_ID', 'your_customer_id', [System.EnvironmentVariableTarget]::User)
+[System.Environment]::SetEnvironmentVariable('VECTARA_API_KEY', 'your_api_key', [System.EnvironmentVariableTarget]::User)
+```
+
+Note that changes made through the command line will only take effect in new instances of the terminal or command prompt.
+
+#### Using Credentials in `vectara-cli`
+
+Once you have set up your environment variables, `vectara-cli` will automatically use these credentials for authentication. There's no need to manually input your customer ID and API key each time you execute a command.
 
 ### Basic Commands
 
+
 #### Indexing a Document
 
 To index a document into a specific corpus:
 
 ```bash
 vectara-cli index-document <corpus_id> <document_id> "<title>" '<metadata_json>' "<section_text>"
 ```
@@ -464,8 +482,8 @@
 
 ## License
 
 `vectara-cli` is MIT licensed. See the [LICENSE](LICENSE.md) file for more details.
 
 ---
 
-This README provides a comprehensive guide for installing and using the `vectara-cli` package. For further information or assistance, please refer to the [Vectara documentation](https://docs.vectara.com) or submit an issue on the [GitLab repository](https://git.tonic-ai.com/releases/vectara-cli/).
+This README provides a comprehensive guide for installing and using the `vectara-cli` package. For further information or assistance, please refer to the [Vectara documentation](https://docs.vectara.com) or submit an issue on the [GitLab repository](https://git.tonic-ai.com/releases/vectara-cli/).
```

### Comparing `vectara-cli-0.1.3/README.md` & `vectara-cli-0.1.4/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,33 @@
+Metadata-Version: 2.1
+Name: vectara-cli
+Version: 0.1.4
+Summary: A CLI tool for interacting with the Vectara platform, including advanced text processing and indexing features.
+Home-page: https://git.tonic-ai.com/releases/vectara-cli
+Author: Tonic-AI
+Author-email: team@tonic-ai.com
+License: MIT
+Keywords: vectara search-engine document-indexing text-analysis information-retrieval natural-language-processing cli-tool data-science machine-learning text-processing
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Utilities
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE.md
+Requires-Dist: requests
+Provides-Extra: advanced
+Requires-Dist: accelerate; extra == "advanced"
+Requires-Dist: torch>=1.8.0; extra == "advanced"
+Requires-Dist: transformers>=4.5.0; extra == "advanced"
+Requires-Dist: span_marker; extra == "advanced"
+Requires-Dist: spacy; extra == "advanced"
+
 # vectara-cli
 
 `vectara-cli` is a Python package designed to interact with the Vectara platform, providing a command-line interface (CLI) and a set of APIs for indexing and querying documents, managing corpora, and performing advanced text analysis and processing tasks. This package is particularly useful for developers and data scientists working on search and information retrieval applications.
 
 ## Features
 
 - Indexing text and documents into Vectara corpora.
@@ -38,25 +64,69 @@
 The `vectara-cli` provides a powerful command line interface for interacting with the Vectara platform, enabling tasks such as document indexing, querying, corpus management, and advanced text processing directly from your terminal. This section will guide you through the basics of using the `vectara-cli`.
 
 ### Installation
 
 Before using the CLI, ensure you have the package installed. You can install it directly from PyPi using pip:
 
 ```bash
-pip install your-package-name
+pip install vectara-cli
 ```
+### Configuration
 
-Replace `your-package-name` with the actual name of your package on PyPi.
+#### Setting Credentials via CLI Commands
 
-### Configuration
+The `vectara-cli` tool now supports a convenient feature for setting your Vectara customer ID and API key directly through the command line. This method utilizes a command specifically designed for securely storing your credentials, making it easier to manage your Vectara configuration without manually setting environment variables or directly embedding your credentials in your scripts.
+
+#### Using the `set-api-keys` Command
+
+To set your Vectara customer ID and API key using the `vectara-cli`, you can use the `set-api-keys` command. This command stores your credentials securely, allowing `vectara-cli` to automatically use them for authentication in future operations.
+
+- **Syntax:** The command follows this simple syntax:
 
-To use the CLI, you need to configure your Vectara customer ID and API key. These can be set as environment variables or directly within the CLI commands as shown in the examples below.
+```bash
+vectara-cli set-api-keys <customer_id> <api_key>
+```
+
+Replace `<customer_id>` with your Vectara customer ID and `<api_key>` with your Vectara API key.
+
+- **Example:**
+
+```bash
+vectara-cli set-api-keys 123456789 abcdefghijklmnopqrstuvwxyz
+```
+
+After executing this command, you will see a confirmation message indicating that your API keys have been set successfully.
+
+#### Windows
+
+For Windows users, you can also set environment variables through the Command Prompt or PowerShell, or via the System Properties window.
+
+- **Command Prompt:**
+
+```cmd
+setx VECTARA_CUSTOMER_ID "your_customer_id"
+setx VECTARA_API_KEY "your_api_key"
+```
+
+- **PowerShell:**
+
+```powershell
+[System.Environment]::SetEnvironmentVariable('VECTARA_CUSTOMER_ID', 'your_customer_id', [System.EnvironmentVariableTarget]::User)
+[System.Environment]::SetEnvironmentVariable('VECTARA_API_KEY', 'your_api_key', [System.EnvironmentVariableTarget]::User)
+```
+
+Note that changes made through the command line will only take effect in new instances of the terminal or command prompt.
+
+#### Using Credentials in `vectara-cli`
+
+Once you have set up your environment variables, `vectara-cli` will automatically use these credentials for authentication. There's no need to manually input your customer ID and API key each time you execute a command.
 
 ### Basic Commands
 
+
 #### Indexing a Document
 
 To index a document into a specific corpus:
 
 ```bash
 vectara-cli index-document <corpus_id> <document_id> "<title>" '<metadata_json>' "<section_text>"
 ```
@@ -438,8 +508,8 @@
 
 ## License
 
 `vectara-cli` is MIT licensed. See the [LICENSE](LICENSE.md) file for more details.
 
 ---
 
-This README provides a comprehensive guide for installing and using the `vectara-cli` package. For further information or assistance, please refer to the [Vectara documentation](https://docs.vectara.com) or submit an issue on the [GitLab repository](https://git.tonic-ai.com/releases/vectara-cli/).
+This README provides a comprehensive guide for installing and using the `vectara-cli` package. For further information or assistance, please refer to the [Vectara documentation](https://docs.vectara.com) or submit an issue on the [GitLab repository](https://git.tonic-ai.com/releases/vectara-cli/).
```

### Comparing `vectara-cli-0.1.3/setup.py` & `vectara-cli-0.1.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
  # ./setup.py
 
 from setuptools import setup, find_packages
 
 setup(
     name="vectara-cli",
-    version="0.1.3",
+    version="0.1.4",
     author="Tonic-AI",
     author_email="team@tonic-ai.com",
     description="A CLI tool for interacting with the Vectara platform, including advanced text processing and indexing features.",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     url="https://git.tonic-ai.com/releases/vectara-cli",
     packages=find_packages(),
@@ -22,22 +22,22 @@
             "transformers>=4.5.0",
             "span_marker",
             "spacy",
         ],
     },
     entry_points={
         'console_scripts': [
-            'vectara_cli=vectara_cli.core:VectaraClient',
+            'vectara=vectara_cli.main:main',
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
-    python_requires='>=3.6',
+    python_requires='>=3.9',
     license="MIT",
     keywords="vectara search-engine document-indexing text-analysis information-retrieval natural-language-processing cli-tool data-science machine-learning text-processing",
 )
```

### Comparing `vectara-cli-0.1.3/vectara-cli/core.py` & `vectara-cli-0.1.4/vectara_cli/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,30 @@
 # ./vectara-cli/core.py
 
 import requests
 import json
 import os
 import logging
 
+class ConfigManager:
+    @staticmethod
+    def set_api_keys(customer_id, api_key):
+        """Sets the customer ID and API key as environment variables."""
+        os.environ['VECTARA_CUSTOMER_ID'] = customer_id
+        os.environ['VECTARA_API_KEY'] = api_key
+
+    @staticmethod
+    def get_api_keys():
+        """Retrieves the customer ID and API key from environment variables."""
+        customer_id = os.getenv('VECTARA_CUSTOMER_ID')
+        api_key = os.getenv('VECTARA_API_KEY')
+        if not customer_id or not api_key:
+            raise ValueError("API keys are not set. Please set them using the 'set-api-keys' command.")
+        return customer_id, api_key
+
 class VectaraClient:
     def __init__(self, customer_id, api_key):
         self.base_url = "https://api.vectara.io"
         self.headers = {
             "Content-Type": "application/json",
             "Accept": "application/json",
             "customer-id": customer_id,
```

### Comparing `vectara-cli-0.1.3/vectara-cli/main.py` & `vectara-cli-0.1.4/vectara_cli/main.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,32 @@
 # ./vectara_cli/main.py
 
-from .core import VectaraClient
+from .core import VectaraClient , ConfigManager
 from .advanced.noncommercial.nerdspan import Span
 from .advanced.noncommercial.rebel import Rebel
 import json
 import sys
 import os
 
 def main():
-    args = sys.argv[1:]
-    if not args:
-        print("Usage: vectara-cli [command] [options]")
+    if command == "set-api-keys":
+        if len(args) != 3:
+            print("Usage: vectara-cli set-api-keys customer_id api_key")
+            return
+        customer_id = args[1]
+        api_key = args[2]
+        ConfigManager.set_api_keys(customer_id, api_key)
+        print("API keys set successfully.")
+        return
+    try:
+        customer_id, api_key = ConfigManager.get_api_keys()
+    except ValueError as e:
+        print(e)
         return
 
-    command = args[0]
-    customer_id = "your_customer_id"
-    api_key = "your_api_key"
     vectara_client = VectaraClient(customer_id, api_key)
 
     if command == "index-document":
         if len(args) < 6:
             print("Usage: vectara-cli index-document corpus_id document_id title metadata_json section_text")
             return
         corpus_id = args[1]
@@ -43,15 +50,14 @@
         print(response)
     elif command == "create-corpus":
         if len(args) < 3:
             print("Usage: vectara-cli create-corpus corpus_id name")
             return
         corpus_id = args[1]
         name = args[2]
-        # Simplified for demonstration; 
         response = vectara_client.create_corpus(corpus_id, name, "Description", 1234567890, True, False, False, False, False, "default", 10000, [], [])
         print(response)
     elif command == "delete-corpus":
         if len(args) < 2:
             print("Usage: vectara-cli delete-corpus corpus_id")
             return
         corpus_id = args[1]
```

### Comparing `vectara-cli-0.1.3/vectara_cli.egg-info/PKG-INFO` & `vectara-cli-0.1.4/vectara_cli.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: vectara-cli
-Version: 0.1.3
+Version: 0.1.4
 Summary: A CLI tool for interacting with the Vectara platform, including advanced text processing and indexing features.
 Home-page: https://git.tonic-ai.com/releases/vectara-cli
 Author: Tonic-AI
 Author-email: team@tonic-ai.com
 License: MIT
 Keywords: vectara search-engine document-indexing text-analysis information-retrieval natural-language-processing cli-tool data-science machine-learning text-processing
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
-Requires-Python: >=3.6
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: requests
 Provides-Extra: advanced
 Requires-Dist: accelerate; extra == "advanced"
 Requires-Dist: torch>=1.8.0; extra == "advanced"
 Requires-Dist: transformers>=4.5.0; extra == "advanced"
@@ -64,25 +64,69 @@
 The `vectara-cli` provides a powerful command line interface for interacting with the Vectara platform, enabling tasks such as document indexing, querying, corpus management, and advanced text processing directly from your terminal. This section will guide you through the basics of using the `vectara-cli`.
 
 ### Installation
 
 Before using the CLI, ensure you have the package installed. You can install it directly from PyPi using pip:
 
 ```bash
-pip install your-package-name
+pip install vectara-cli
 ```
+### Configuration
 
-Replace `your-package-name` with the actual name of your package on PyPi.
+#### Setting Credentials via CLI Commands
 
-### Configuration
+The `vectara-cli` tool now supports a convenient feature for setting your Vectara customer ID and API key directly through the command line. This method utilizes a command specifically designed for securely storing your credentials, making it easier to manage your Vectara configuration without manually setting environment variables or directly embedding your credentials in your scripts.
+
+#### Using the `set-api-keys` Command
+
+To set your Vectara customer ID and API key using the `vectara-cli`, you can use the `set-api-keys` command. This command stores your credentials securely, allowing `vectara-cli` to automatically use them for authentication in future operations.
+
+- **Syntax:** The command follows this simple syntax:
+
+```bash
+vectara-cli set-api-keys <customer_id> <api_key>
+```
+
+Replace `<customer_id>` with your Vectara customer ID and `<api_key>` with your Vectara API key.
+
+- **Example:**
+
+```bash
+vectara-cli set-api-keys 123456789 abcdefghijklmnopqrstuvwxyz
+```
+
+After executing this command, you will see a confirmation message indicating that your API keys have been set successfully.
+
+#### Windows
+
+For Windows users, you can also set environment variables through the Command Prompt or PowerShell, or via the System Properties window.
+
+- **Command Prompt:**
+
+```cmd
+setx VECTARA_CUSTOMER_ID "your_customer_id"
+setx VECTARA_API_KEY "your_api_key"
+```
 
-To use the CLI, you need to configure your Vectara customer ID and API key. These can be set as environment variables or directly within the CLI commands as shown in the examples below.
+- **PowerShell:**
+
+```powershell
+[System.Environment]::SetEnvironmentVariable('VECTARA_CUSTOMER_ID', 'your_customer_id', [System.EnvironmentVariableTarget]::User)
+[System.Environment]::SetEnvironmentVariable('VECTARA_API_KEY', 'your_api_key', [System.EnvironmentVariableTarget]::User)
+```
+
+Note that changes made through the command line will only take effect in new instances of the terminal or command prompt.
+
+#### Using Credentials in `vectara-cli`
+
+Once you have set up your environment variables, `vectara-cli` will automatically use these credentials for authentication. There's no need to manually input your customer ID and API key each time you execute a command.
 
 ### Basic Commands
 
+
 #### Indexing a Document
 
 To index a document into a specific corpus:
 
 ```bash
 vectara-cli index-document <corpus_id> <document_id> "<title>" '<metadata_json>' "<section_text>"
 ```
```

