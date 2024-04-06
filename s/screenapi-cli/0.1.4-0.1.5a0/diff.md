# Comparing `tmp/screenapi_cli-0.1.4.tar.gz` & `tmp/screenapi_cli-0.1.5a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "screenapi_cli-0.1.4.tar", max compression
+gzip compressed data, was "screenapi_cli-0.1.5a0.tar", max compression
```

## Comparing `screenapi_cli-0.1.4.tar` & `screenapi_cli-0.1.5a0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1092 2024-03-23 16:06:49.120124 screenapi_cli-0.1.4/LICENSE
--rw-r--r--   0        0        0     1381 2024-03-25 19:41:34.179648 screenapi_cli-0.1.4/README.md
--rw-r--r--   0        0        0        0 2024-03-26 06:15:38.237432 screenapi_cli-0.1.4/app/__init__.py
--rw-r--r--   0        0        0     9231 2024-03-31 18:24:26.956298 screenapi_cli-0.1.4/app/__main__.py
--rw-r--r--   0        0        0     1360 2024-03-29 17:33:20.645434 screenapi_cli-0.1.4/app/common.py
--rw-r--r--   0        0        0        0 2024-03-24 18:09:29.678307 screenapi_cli-0.1.4/app/export/__init__.py
--rw-r--r--   0        0        0     1435 2024-03-26 08:34:32.751466 screenapi_cli-0.1.4/app/export/cli.py
--rw-r--r--   0        0        0       97 2024-03-24 17:32:30.550768 screenapi_cli-0.1.4/app/scrape/__init__.py
--rw-r--r--   0        0        0     5737 2024-03-29 09:45:40.583647 screenapi_cli-0.1.4/app/scrape/cli.py
--rw-r--r--   0        0        0     6056 2024-03-25 18:55:58.756247 screenapi_cli-0.1.4/app/scrape/deprecated_cli.py
--rw-r--r--   0        0        0        0 2024-03-24 14:33:45.903715 screenapi_cli-0.1.4/app/setup/__init__.py
--rw-r--r--   0        0        0     1083 2024-03-25 19:15:41.722738 screenapi_cli-0.1.4/app/setup/utils.py
--rw-r--r--   0        0        0        0 2024-03-27 04:52:19.596215 screenapi_cli-0.1.4/app/update/__init__.py
--rw-r--r--   0        0        0     9981 2024-03-31 19:06:36.168898 screenapi_cli-0.1.4/app/update/main.py
--rw-r--r--   0        0        0      766 2024-03-31 18:28:58.370548 screenapi_cli-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     2042 1970-01-01 00:00:00.000000 screenapi_cli-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1092 2024-03-23 16:06:49.120124 screenapi_cli-0.1.5a0/LICENSE
+-rw-r--r--   0        0        0     1381 2024-03-25 19:41:34.179648 screenapi_cli-0.1.5a0/README.md
+-rw-r--r--   0        0        0        0 2024-03-26 06:15:38.237432 screenapi_cli-0.1.5a0/app/__init__.py
+-rw-r--r--   0        0        0     9224 2024-04-01 07:33:00.588714 screenapi_cli-0.1.5a0/app/__main__.py
+-rw-r--r--   0        0        0     1360 2024-04-01 07:33:03.304661 screenapi_cli-0.1.5a0/app/common.py
+-rw-r--r--   0        0        0        0 2024-03-24 18:09:29.678307 screenapi_cli-0.1.5a0/app/export/__init__.py
+-rw-r--r--   0        0        0     1435 2024-03-26 08:34:32.751466 screenapi_cli-0.1.5a0/app/export/cli.py
+-rw-r--r--   0        0        0        0 2024-03-24 14:33:45.903715 screenapi_cli-0.1.5a0/app/setup/__init__.py
+-rw-r--r--   0        0        0     1083 2024-03-25 19:15:41.722738 screenapi_cli-0.1.5a0/app/setup/utils.py
+-rw-r--r--   0        0        0       97 2024-03-24 17:32:30.550768 screenapi_cli-0.1.5a0/app/txt/__init__.py
+-rw-r--r--   0        0        0     5737 2024-03-29 09:45:40.583647 screenapi_cli-0.1.5a0/app/txt/cli.py
+-rw-r--r--   0        0        0     6056 2024-03-25 18:55:58.756247 screenapi_cli-0.1.5a0/app/txt/deprecated_cli.py
+-rw-r--r--   0        0        0        0 2024-03-27 04:52:19.596215 screenapi_cli-0.1.5a0/app/xlsx/__init__.py
+-rw-r--r--   0        0        0     9969 2024-04-01 07:33:16.992395 screenapi_cli-0.1.5a0/app/xlsx/main.py
+-rw-r--r--   0        0        0      767 2024-04-01 04:14:18.662394 screenapi_cli-0.1.5a0/pyproject.toml
+-rw-r--r--   0        0        0     2044 1970-01-01 00:00:00.000000 screenapi_cli-0.1.5a0/PKG-INFO
```

### Comparing `screenapi_cli-0.1.4/LICENSE` & `screenapi_cli-0.1.5a0/LICENSE`

 * *Files identical despite different names*

### Comparing `screenapi_cli-0.1.4/README.md` & `screenapi_cli-0.1.5a0/README.md`

 * *Files identical despite different names*

### Comparing `screenapi_cli-0.1.4/app/__main__.py` & `screenapi_cli-0.1.5a0/app/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 import random
 import re
 import sys
 
 from httpx import request
 
-from app.update.main import read_mapping
+from app.xlsx.main import read_mapping
 
 sys.path.append(os.curdir)
 
 from importlib.metadata import version
 from rich import print
 import asyncio
 import typer
@@ -68,15 +68,15 @@
     urls_file: Path = typer.Argument(help="Path to the urls file", resolve_path=True),
     max_workers: Annotated[
         int, typer.Option("-w", help="number of workers")
     ] = configGet("default", "max_workers"),
     overwrite: Annotated[bool, typer.Option(help="overwrite existing data")] = False,
     skip_images: Annotated[bool, typer.Option(help="skip saving images")] = False,
 ):
-    from app.scrape.cli import main
+    from app.txt.cli import main
 
     print("Scraping...")
     print(f"Urls file: {urls_file}")
     print(f"Number of workers: {max_workers}")
     print(f"Overwrite existing data: {overwrite}")
     print(f"Skip saving images: {skip_images}")
 
@@ -195,15 +195,15 @@
     ] = None,
     max_workers: Annotated[
         int, typer.Option("-w", help="number of workers")
     ] = configGet("default", "max_workers"),
     overwrite: Annotated[bool, typer.Option(help="overwrite existing data")] = False,
     skip_images: Annotated[bool, typer.Option(help="skip saving images")] = False,
 ):
-    from app.update.main import main
+    from app.xlsx.main import main
 
     print(f"[bold]Updating sheet from {input_path}[/]")
     print(f"Number of workers: {max_workers}")
     print(f"Overwrite existing data: {overwrite}")
     print(f"Skip saving images: {skip_images}")
 
     main(
```

### Comparing `screenapi_cli-0.1.4/app/common.py` & `screenapi_cli-0.1.5a0/app/common.py`

 * *Files identical despite different names*

### Comparing `screenapi_cli-0.1.4/app/export/cli.py` & `screenapi_cli-0.1.5a0/app/export/cli.py`

 * *Files identical despite different names*

### Comparing `screenapi_cli-0.1.4/app/scrape/cli.py` & `screenapi_cli-0.1.5a0/app/txt/cli.py`

 * *Files identical despite different names*

### Comparing `screenapi_cli-0.1.4/app/scrape/deprecated_cli.py` & `screenapi_cli-0.1.5a0/app/txt/deprecated_cli.py`

 * *Files identical despite different names*

### Comparing `screenapi_cli-0.1.4/app/setup/utils.py` & `screenapi_cli-0.1.5a0/app/setup/utils.py`

 * *Files identical despite different names*

### Comparing `screenapi_cli-0.1.4/app/update/main.py` & `screenapi_cli-0.1.5a0/app/xlsx/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,24 +7,24 @@
 from click import echo
 from rich.progress import TaskID, Progress
 import pandas
 import configparser
 from rich import print
 from httpx import Client
 from app.common import providers_pattern, sheetType
-from app.scrape.cli import getId
+from app.txt.cli import getId
 from app.setup.utils import config_file
 
 # global output_dir
 config = configparser.ConfigParser()
 config.read(config_file())
 OUTPUT_DIR: Path = None
 
 
-def read_mapping(sitename: sheetType, swap: bool = False) -> dict:
+def read_mapping(sitename: str, swap: bool = False) -> dict:
     ecom = {
         "S.No.": "sl",
         "Image": "image",
         "URL": "url",
         "Title": "title",
         "MRP": "mrp",
         "Price": "price",
@@ -42,24 +42,25 @@
     social = {
         "S.No.": "sl",
         "Image": "image",
         "Heading": "description",
         "URL": "url",
     }
 
+
     match sitename:
         case "ecom":
             if swap:
-                return {value: key for key, value in ecom}
+                return {ecom[key]: key for key in ecom}
 
             return ecom
 
         case "social":
             if swap:
-                return {value: key for key, value in social}
+                return {social[key]: key for key in social}
             return social
 
 
 def convert_to_json(input_path: Path, site: sheetType, save: Optional[bool] = True):
     # setup input_path and output_file (excel to json)
 
     # read excel, rename column, fix date
```

### Comparing `screenapi_cli-0.1.4/pyproject.toml` & `screenapi_cli-0.1.5a0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "screenapi-cli"
-version = "0.1.4"
+version = "0.1.5a"
 description = "A cli interface to interact with screenapi"
 authors = ["RONY <iamrony777@pm.me>"]
 license = "MIT"
 readme = "README.md"
 packages = [
     { include = "app" },
 ]
 
 [project.urls]
-Homepage = "https://ffstudios.io"
-Repository = "https://github.com/FutureForge-Studios/screenapi-cli.git"
+homepage = "https://ffstudios.io"
+repository = "https://github.com/FutureForge-Studios/screenapi-cli.git"
 
 [tool.poetry.scripts]
 screenapi-cli = "app.__main__:app"
 sapi = "app.__main__:app"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `screenapi_cli-0.1.4/PKG-INFO` & `screenapi_cli-0.1.5a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: screenapi-cli
-Version: 0.1.4
+Version: 0.1.5a0
 Summary: A cli interface to interact with screenapi
 License: MIT
 Author: RONY
 Author-email: iamrony777@pm.me
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

