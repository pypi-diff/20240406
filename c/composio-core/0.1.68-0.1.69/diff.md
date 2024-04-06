# Comparing `tmp/composio_core-0.1.68.tar.gz` & `tmp/composio_core-0.1.69.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "composio_core-0.1.68.tar", last modified: Thu Apr  4 17:50:59 2024, max compression
+gzip compressed data, was "composio_core-0.1.69.tar", last modified: Sat Apr  6 12:53:46 2024, max compression
```

## Comparing `composio_core-0.1.68.tar` & `composio_core-0.1.69.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-04 17:50:59.718788 composio_core-0.1.68/
--rw-r--r--   0 utkarsh    (501) staff       (20)       48 2024-03-15 13:37:31.000000 composio_core-0.1.68/MANIFEST.in
--rw-r--r--   0 utkarsh    (501) staff       (20)      771 2024-04-04 17:50:59.718586 composio_core-0.1.68/PKG-INFO
--rw-r--r--   0 utkarsh    (501) staff       (20)      102 2024-03-16 10:06:01.000000 composio_core-0.1.68/README.md
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-04 17:50:59.716649 composio_core-0.1.68/composio/
--rw-r--r--   0 utkarsh    (501) staff       (20)      176 2024-03-27 14:52:24.000000 composio_core-0.1.68/composio/__init__.py
--rwxr-xr-x   0 utkarsh    (501) staff       (20)    10396 2024-04-04 17:45:13.000000 composio_core-0.1.68/composio/composio_cli.py
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-04 17:50:59.717597 composio_core-0.1.68/composio/sdk/
--rw-r--r--   0 utkarsh    (501) staff       (20)       85 2024-03-27 14:52:24.000000 composio_core-0.1.68/composio/sdk/__init__.py
--rw-r--r--   0 utkarsh    (501) staff       (20)     5036 2024-04-04 17:45:13.000000 composio_core-0.1.68/composio/sdk/core.py
--rw-r--r--   0 utkarsh    (501) staff       (20)     7414 2024-04-04 17:45:19.000000 composio_core-0.1.68/composio/sdk/enums.py
--rw-r--r--   0 utkarsh    (501) staff       (20)    16213 2024-04-04 17:45:13.000000 composio_core-0.1.68/composio/sdk/sdk.py
--rw-r--r--   0 utkarsh    (501) staff       (20)     1264 2024-03-16 12:05:30.000000 composio_core-0.1.68/composio/sdk/storage.py
--rw-r--r--   0 utkarsh    (501) staff       (20)     2812 2024-04-04 17:45:13.000000 composio_core-0.1.68/composio/sdk/utils.py
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-04 17:50:59.718371 composio_core-0.1.68/composio_core.egg-info/
--rw-r--r--   0 utkarsh    (501) staff       (20)      771 2024-04-04 17:50:59.000000 composio_core-0.1.68/composio_core.egg-info/PKG-INFO
--rw-r--r--   0 utkarsh    (501) staff       (20)      466 2024-04-04 17:50:59.000000 composio_core-0.1.68/composio_core.egg-info/SOURCES.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)        1 2024-04-04 17:50:59.000000 composio_core-0.1.68/composio_core.egg-info/dependency_links.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)       60 2024-04-04 17:50:59.000000 composio_core-0.1.68/composio_core.egg-info/entry_points.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)       92 2024-04-04 17:50:59.000000 composio_core-0.1.68/composio_core.egg-info/requires.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)        9 2024-04-04 17:50:59.000000 composio_core-0.1.68/composio_core.egg-info/top_level.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)      510 2024-03-23 19:08:16.000000 composio_core-0.1.68/pyproject.toml
--rw-r--r--   0 utkarsh    (501) staff       (20)       90 2024-03-23 19:08:10.000000 composio_core-0.1.68/requirements.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)       38 2024-04-04 17:50:59.718828 composio_core-0.1.68/setup.cfg
--rw-r--r--   0 utkarsh    (501) staff       (20)     1134 2024-04-04 17:50:54.000000 composio_core-0.1.68/setup.py
+drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-06 12:53:46.046623 composio_core-0.1.69/
+-rw-r--r--   0 utkarsh    (501) staff       (20)       48 2024-03-15 13:37:31.000000 composio_core-0.1.69/MANIFEST.in
+-rw-r--r--   0 utkarsh    (501) staff       (20)      771 2024-04-06 12:53:46.046283 composio_core-0.1.69/PKG-INFO
+-rw-r--r--   0 utkarsh    (501) staff       (20)      102 2024-03-16 10:06:01.000000 composio_core-0.1.69/README.md
+drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-06 12:53:46.043448 composio_core-0.1.69/composio/
+-rw-r--r--   0 utkarsh    (501) staff       (20)      176 2024-03-27 14:52:24.000000 composio_core-0.1.69/composio/__init__.py
+-rwxr-xr-x   0 utkarsh    (501) staff       (20)    11902 2024-04-06 12:52:24.000000 composio_core-0.1.69/composio/composio_cli.py
+drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-06 12:53:46.044738 composio_core-0.1.69/composio/sdk/
+-rw-r--r--   0 utkarsh    (501) staff       (20)       85 2024-03-27 14:52:24.000000 composio_core-0.1.69/composio/sdk/__init__.py
+-rw-r--r--   0 utkarsh    (501) staff       (20)     5542 2024-04-06 12:52:11.000000 composio_core-0.1.69/composio/sdk/core.py
+-rw-r--r--   0 utkarsh    (501) staff       (20)     7414 2024-04-04 17:45:19.000000 composio_core-0.1.69/composio/sdk/enums.py
+-rw-r--r--   0 utkarsh    (501) staff       (20)    16227 2024-04-06 12:36:58.000000 composio_core-0.1.69/composio/sdk/sdk.py
+-rw-r--r--   0 utkarsh    (501) staff       (20)     2210 2024-04-06 12:48:31.000000 composio_core-0.1.69/composio/sdk/storage.py
+-rw-r--r--   0 utkarsh    (501) staff       (20)     2861 2024-04-06 12:48:50.000000 composio_core-0.1.69/composio/sdk/utils.py
+drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-06 12:53:46.045985 composio_core-0.1.69/composio_core.egg-info/
+-rw-r--r--   0 utkarsh    (501) staff       (20)      771 2024-04-06 12:53:46.000000 composio_core-0.1.69/composio_core.egg-info/PKG-INFO
+-rw-r--r--   0 utkarsh    (501) staff       (20)      466 2024-04-06 12:53:46.000000 composio_core-0.1.69/composio_core.egg-info/SOURCES.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)        1 2024-04-06 12:53:46.000000 composio_core-0.1.69/composio_core.egg-info/dependency_links.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)       60 2024-04-06 12:53:46.000000 composio_core-0.1.69/composio_core.egg-info/entry_points.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)       92 2024-04-06 12:53:46.000000 composio_core-0.1.69/composio_core.egg-info/requires.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)        9 2024-04-06 12:53:46.000000 composio_core-0.1.69/composio_core.egg-info/top_level.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)      510 2024-03-23 19:08:16.000000 composio_core-0.1.69/pyproject.toml
+-rw-r--r--   0 utkarsh    (501) staff       (20)       90 2024-03-23 19:08:10.000000 composio_core-0.1.69/requirements.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)       38 2024-04-06 12:53:46.046695 composio_core-0.1.69/setup.cfg
+-rw-r--r--   0 utkarsh    (501) staff       (20)     1134 2024-04-06 12:53:03.000000 composio_core-0.1.69/setup.py
```

### Comparing `composio_core-0.1.68/PKG-INFO` & `composio_core-0.1.69/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: composio_core
-Version: 0.1.68
+Version: 0.1.69
 Summary: Core package to act as a bridge between composio platform and other services.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Utkarsh
 Author-email: utkarsh@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `composio_core-0.1.68/composio/composio_cli.py` & `composio_core-0.1.69/composio/composio_cli.py`

 * *Files 9% similar despite different names*

```diff
@@ -50,20 +50,56 @@
     enable_trigger_parser.set_defaults(func=enable_trigger)
 
     # List triggers command
     list_triggers_parser = subparsers.add_parser('list-triggers', help='List all triggers for a given app')
     list_triggers_parser.add_argument('app_name', type=str, help='Name of the app to list triggers for')
     list_triggers_parser.set_defaults(func=list_triggers)
 
+    # Beta command group
+    beta_parser = subparsers.add_parser('beta', help='Beta features commands')
+    beta_subparsers = beta_parser.add_subparsers(help='beta commands', dest='beta_command')
+    beta_subparsers.required = True
+
+    # Update base_url command under beta
+    update_base_url_parser = beta_subparsers.add_parser('update-base-url', help='Update the base URL for API calls')
+    update_base_url_parser.add_argument('base_url', type=str, help='The new base URL to use for API calls')
+    update_base_url_parser.set_defaults(func=update_base_url)
+
+    # Logout command
+    logout_parser = subparsers.add_parser('logout', help='Logout from the current session')
+    logout_parser.set_defaults(func=logout)
+
     # Generate enums command
     generate_enums_parser = subparsers.add_parser('update', help='Update enums for apps and actions')
     generate_enums_parser.set_defaults(func=handle_update)
 
     return parser.parse_args()
 
+def logout(args):
+    client = ComposioCore()
+    console.print(f"\n[green]> Logging out...[/green]\n")
+    try:
+        client.logout()
+        console.print(f"\n[green]✔ Logged out successfully![/green]\n")
+    except Exception as e:
+        console.print(f"[red] Error occurred during logging out: {e}[/red]")
+        sys.exit(1)
+
+def update_base_url(args):
+    client = ComposioCore()
+    auth_user(client)
+    base_url = args.base_url
+    console.print(f"\n[green]> Updating base URL to: {base_url}...[/green]\n")
+    try:
+        client.set_base_url(base_url)
+        console.print(f"\n[green]✔ Base URL updated successfully![/green]\n")
+    except Exception as e:
+        console.print(f"[red] Error occurred during updating base URL: {e}[/red]")
+        sys.exit(1)
+
 def list_triggers(args):
     client = ComposioCore()
     auth_user(client)
     app_name = args.app_name
     console.print(f"\n[green]> Listing triggers for app: {app_name}...[/green]\n")
     try:
         triggers = client.list_triggers(app_name)
@@ -217,7 +253,9 @@
         console.print(f"[red]Error occurred during user identification: {e}[/red]")
         sys.exit(1)
 
     if hasattr(args, 'func'):
         args.func(args)
     else:
         console.print("[red]Error: No valid command provided. Use --help for more information.[/red]")
+
+main()
```

### Comparing `composio_core-0.1.68/composio/sdk/core.py` & `composio_core-0.1.69/composio/sdk/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from typing import Union
 import requests
 
 from .utils import get_git_user_info
 from .sdk import ConnectionRequest, ConnectedAccount
-from .storage import get_user_connection, get_api_key, save_api_key
+from .storage import delete_user_connections, get_base_url, get_user_connection, get_api_key, load_user_data, save_api_key, save_user_data, set_base_url
 from .sdk import Composio
 from .enums import TestIntegration, Action
 from enum import Enum
 
 class FrameworkEnum(Enum):
     AUTOGEN = "autogen"
     LANGCHAIN = "langchain"
 
 __IS_FIRST_TIME__ = True
 
 class ComposioCore:
     sdk: Composio = None
     framework: FrameworkEnum = None
 
-    def __init__(self, base_url = "https://backend.composio.dev/api", manage_auth = True, framework: FrameworkEnum = None):
+    def __init__(self, base_url = get_base_url(), manage_auth = True, framework: FrameworkEnum = None):
         global __IS_FIRST_TIME__
 
         self.base_url = base_url
         self.manage_auth = manage_auth
         self.http_client = requests.Session()
         self.framework = framework
         self.http_client.headers.update({
@@ -47,14 +47,28 @@
                                 "email": git_info.email
                             } if git_info.name and git_info.email else None
                         });
                         __IS_FIRST_TIME__ = False
                     except:
                         pass
 
+    def set_base_url(self, base_url: str):
+        self.base_url = base_url
+        set_base_url(base_url, force_reset=True)
+        self.http_client.headers.update({
+            'Content-Type': 'application/json'
+        })
+    
+    def logout(self):
+        self.http_client.headers.pop('x-api-key')
+        user_data = load_user_data()
+        user_data.pop('api_key')
+        delete_user_connections()
+        save_user_data(user_data)
+
     def authenticate(self, hash: str):
         resp = self.http_client.post(f"{self.base_url}/v1/client/auth/identify", json={
             "hash": hash,
         });
         if resp.status_code == 202:
             api_key = resp.json().get('apiKey')
             self.http_client.headers.update({
```

### Comparing `composio_core-0.1.68/composio/sdk/enums.py` & `composio_core-0.1.69/composio/sdk/enums.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.1.68/composio/sdk/sdk.py` & `composio_core-0.1.69/composio/sdk/sdk.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from enum import Enum
 import time
 from typing import Optional, Union, Tuple
 import requests
 from pydantic import BaseModel, ConfigDict
 
 from .enums import Action, App, TestIntegration
+from .storage import get_base_url
 from openai.types.chat.chat_completion import ChatCompletion
 from openai.types.beta.threads import run
 from openai import Client
 from openai.types.beta import thread
 import json
 
 
@@ -171,15 +172,15 @@
 
     def get_required_variables(self):
         return self.expectedInputFields
 
 
 class Composio:
     def __init__(
-        self, api_key: str = None, base_url="https://backend.composio.dev/api"
+        self, api_key: str = None, base_url=get_base_url()
     ):
         self.base_url = base_url
         self.api_key = api_key
         self.http_client = requests.Session()
         self.http_client.headers.update(
             {"Content-Type": "application/json", "x-api-key": self.api_key}
         )
```

### Comparing `composio_core-0.1.68/composio/sdk/utils.py` & `composio_core-0.1.69/composio/sdk/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,18 @@
+from .storage import get_base_account_api_key
 from .sdk import Composio
 import os
 from pydantic import BaseModel
 import subprocess
 
 def _get_enum_key(name):
     return name.upper().replace(' ', '_').replace('-', '_')
 
 def generate_enums():
-    sdk_client = Composio("yw1qb4ls4340z696zh7sa")
+    sdk_client = Composio(get_base_account_api_key())
     apps = sdk_client.get_list_of_apps()
     actions = sdk_client.get_list_of_actions()
     triggers = sdk_client.get_list_of_triggers()
 
     enum_content = 'from enum import Enum\n\n'
     enum_content += 'class App(Enum):\n'
     for app in apps["items"]:
```

### Comparing `composio_core-0.1.68/composio_core.egg-info/PKG-INFO` & `composio_core-0.1.69/composio_core.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: composio_core
-Version: 0.1.68
+Version: 0.1.69
 Summary: Core package to act as a bridge between composio platform and other services.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Utkarsh
 Author-email: utkarsh@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `composio_core-0.1.68/setup.py` & `composio_core-0.1.69/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
     def run(self):
         install.run(self)
 
 
 setup(
     name="composio_core",
-    version="0.1.68",
+    version="0.1.69",
     author="Utkarsh",
     author_email="utkarsh@composio.dev",
     description="Core package to act as a bridge between composio platform and other services.",
     long_description=open(readme_path).read(),
     long_description_content_type="text/markdown",
     url="https://github.com/SamparkAI/composio_sdk",
     classifiers=[
```

