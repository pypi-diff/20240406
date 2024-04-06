# Comparing `tmp/yaml-to-markdown-0.1.1712379388.tar.gz` & `tmp/yaml-to-markdown-0.1.1712381225.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yaml-to-markdown-0.1.1712379388.tar", last modified: Sat Apr  6 04:56:29 2024, max compression
+gzip compressed data, was "yaml-to-markdown-0.1.1712381225.tar", last modified: Sat Apr  6 05:27:06 2024, max compression
```

## Comparing `yaml-to-markdown-0.1.1712379388.tar` & `yaml-to-markdown-0.1.1712381225.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 nevis     (1000) nevis     (1000)        0 2024-04-06 04:56:29.350352 yaml-to-markdown-0.1.1712379388/
--rw-rw-r--   0 nevis     (1000) nevis     (1000)     1069 2024-04-05 00:30:02.000000 yaml-to-markdown-0.1.1712379388/LICENSE
--rw-r--r--   0 nevis     (1000) nevis     (1000)     1562 2024-04-06 04:56:29.350352 yaml-to-markdown-0.1.1712379388/PKG-INFO
--rw-rw-r--   0 nevis     (1000) nevis     (1000)     1249 2024-04-06 04:53:36.000000 yaml-to-markdown-0.1.1712379388/README.md
--rw-rw-r--   0 nevis     (1000) nevis     (1000)      127 2024-04-06 04:56:29.350352 yaml-to-markdown-0.1.1712379388/setup.cfg
--rw-rw-r--   0 nevis     (1000) nevis     (1000)      751 2024-04-06 04:54:41.000000 yaml-to-markdown-0.1.1712379388/setup.py
-drwxrwxr-x   0 nevis     (1000) nevis     (1000)        0 2024-04-06 04:56:29.318352 yaml-to-markdown-0.1.1712379388/src/
-drwxrwxr-x   0 nevis     (1000) nevis     (1000)        0 2024-04-06 04:56:29.334352 yaml-to-markdown-0.1.1712379388/src/yaml_to_markdown/
--rw-rw-r--   0 nevis     (1000) nevis     (1000)        0 2024-04-05 00:33:57.000000 yaml-to-markdown-0.1.1712379388/src/yaml_to_markdown/__init__.py
--rw-rw-r--   0 nevis     (1000) nevis     (1000)     2391 2024-04-06 04:37:43.000000 yaml-to-markdown-0.1.1712379388/src/yaml_to_markdown/convert.py
--rw-rw-r--   0 nevis     (1000) nevis     (1000)     1269 2024-04-05 02:28:11.000000 yaml-to-markdown-0.1.1712379388/src/yaml_to_markdown/convert_test.py
--rw-rw-r--   0 nevis     (1000) nevis     (1000)     5578 2024-04-06 01:46:47.000000 yaml-to-markdown-0.1.1712379388/src/yaml_to_markdown/md_converter.py
--rw-rw-r--   0 nevis     (1000) nevis     (1000)     7294 2024-04-05 03:27:25.000000 yaml-to-markdown-0.1.1712379388/src/yaml_to_markdown/md_converter_test.py
--rw-rw-r--   0 nevis     (1000) nevis     (1000)       92 2024-04-05 00:35:31.000000 yaml-to-markdown-0.1.1712379388/src/yaml_to_markdown/utils.py
--rw-rw-r--   0 nevis     (1000) nevis     (1000)      183 2024-04-05 00:47:06.000000 yaml-to-markdown-0.1.1712379388/src/yaml_to_markdown/utils_test.py
-drwxrwxr-x   0 nevis     (1000) nevis     (1000)        0 2024-04-06 04:56:29.346352 yaml-to-markdown-0.1.1712379388/src/yaml_to_markdown.egg-info/
--rw-r--r--   0 nevis     (1000) nevis     (1000)     1562 2024-04-06 04:56:29.000000 yaml-to-markdown-0.1.1712379388/src/yaml_to_markdown.egg-info/PKG-INFO
--rw-rw-r--   0 nevis     (1000) nevis     (1000)      548 2024-04-06 04:56:29.000000 yaml-to-markdown-0.1.1712379388/src/yaml_to_markdown.egg-info/SOURCES.txt
--rw-rw-r--   0 nevis     (1000) nevis     (1000)        1 2024-04-06 04:56:29.000000 yaml-to-markdown-0.1.1712379388/src/yaml_to_markdown.egg-info/dependency_links.txt
--rw-rw-r--   0 nevis     (1000) nevis     (1000)       67 2024-04-06 04:56:29.000000 yaml-to-markdown-0.1.1712379388/src/yaml_to_markdown.egg-info/entry_points.txt
--rw-rw-r--   0 nevis     (1000) nevis     (1000)       54 2024-04-06 04:56:29.000000 yaml-to-markdown-0.1.1712379388/src/yaml_to_markdown.egg-info/requires.txt
--rw-rw-r--   0 nevis     (1000) nevis     (1000)       17 2024-04-06 04:56:29.000000 yaml-to-markdown-0.1.1712379388/src/yaml_to_markdown.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 05:27:06.179115 yaml-to-markdown-0.1.1712381225/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-06 05:26:08.000000 yaml-to-markdown-0.1.1712381225/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-04-06 05:27:06.179115 yaml-to-markdown-0.1.1712381225/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-04-06 05:26:08.000000 yaml-to-markdown-0.1.1712381225/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-06 05:27:06.179115 yaml-to-markdown-0.1.1712381225/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-04-06 05:26:08.000000 yaml-to-markdown-0.1.1712381225/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 05:27:06.175115 yaml-to-markdown-0.1.1712381225/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 05:27:06.179115 yaml-to-markdown-0.1.1712381225/src/yaml_to_markdown/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 05:26:08.000000 yaml-to-markdown-0.1.1712381225/src/yaml_to_markdown/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-04-06 05:26:08.000000 yaml-to-markdown-0.1.1712381225/src/yaml_to_markdown/convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-04-06 05:26:08.000000 yaml-to-markdown-0.1.1712381225/src/yaml_to_markdown/convert_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5578 2024-04-06 05:26:08.000000 yaml-to-markdown-0.1.1712381225/src/yaml_to_markdown/md_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7294 2024-04-06 05:26:08.000000 yaml-to-markdown-0.1.1712381225/src/yaml_to_markdown/md_converter_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-06 05:26:08.000000 yaml-to-markdown-0.1.1712381225/src/yaml_to_markdown/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-06 05:26:08.000000 yaml-to-markdown-0.1.1712381225/src/yaml_to_markdown/utils_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 05:27:06.179115 yaml-to-markdown-0.1.1712381225/src/yaml_to_markdown.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-04-06 05:27:06.000000 yaml-to-markdown-0.1.1712381225/src/yaml_to_markdown.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-06 05:27:06.000000 yaml-to-markdown-0.1.1712381225/src/yaml_to_markdown.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 05:27:06.000000 yaml-to-markdown-0.1.1712381225/src/yaml_to_markdown.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-06 05:27:06.000000 yaml-to-markdown-0.1.1712381225/src/yaml_to_markdown.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-06 05:27:06.000000 yaml-to-markdown-0.1.1712381225/src/yaml_to_markdown.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-06 05:27:06.000000 yaml-to-markdown-0.1.1712381225/src/yaml_to_markdown.egg-info/top_level.txt
```

### Comparing `yaml-to-markdown-0.1.1712379388/LICENSE` & `yaml-to-markdown-0.1.1712381225/LICENSE`

 * *Files identical despite different names*

### Comparing `yaml-to-markdown-0.1.1712379388/PKG-INFO` & `yaml-to-markdown-0.1.1712381225/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: yaml-to-markdown
-Version: 0.1.1712379388
+Version: 0.1.1712381225
 Home-page: https://anevis.github.io/yaml-to-markdown/
 Author: anevis
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: click==8.1.7
 Requires-Dist: jsonschema[format]==4.21.1
 Requires-Dist: pyyaml==6.0.1
 
-# JSON to Markdown Converter
+# YAML to Markdown Converter
 
 A Python utility to take a JSON / YAML file or a python dict / list and create a Markdown file.
 
 ## Usage
 
 ### In Python Code example:
```

### Comparing `yaml-to-markdown-0.1.1712379388/README.md` & `yaml-to-markdown-0.1.1712381225/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# JSON to Markdown Converter
+# YAML to Markdown Converter
 
 A Python utility to take a JSON / YAML file or a python dict / list and create a Markdown file.
 
 ## Usage
 
 ### In Python Code example:
```

### Comparing `yaml-to-markdown-0.1.1712379388/setup.py` & `yaml-to-markdown-0.1.1712381225/setup.py`

 * *Files identical despite different names*

### Comparing `yaml-to-markdown-0.1.1712379388/src/yaml_to_markdown/convert.py` & `yaml-to-markdown-0.1.1712381225/src/yaml_to_markdown/convert.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import io
 import json
 from typing import Dict, Any, Optional
 
 import click
 import yaml
 
-from json_to_markdown.md_converter import MDConverter
+from yaml_to_markdown.md_converter import MDConverter
 
 
 def _get_json_data(json_file: str) -> Dict[str, Any]:
     with io.open(json_file, "r", encoding="utf-8") as j_file:
         return json.load(j_file)
 
 
@@ -17,30 +17,30 @@
     with io.open(yaml_file, "r", encoding="utf-8") as y_file:
         return yaml.safe_load(y_file)
 
 
 def _help() -> None:
     click.echo("Convert JSON or YAML to Markdown.")
     click.echo(
-        "Usage: json-to-markdown -o <output_file> [-y <yaml_file> | -j <json_file>]"
+        "Usage: yaml-to-markdown -o <output_file> [-y <yaml_file> | -j <json_file>]"
     )
     click.echo(
         "    -o, --output-file <output_file>: Path to the output file as a string [Mandatory]."
     )
     click.echo(
         "    -y, --yaml-file <yaml_file>: Path to the YAML file as a string [Optional]"
     )
     click.echo(
         "    -j, --json-file <json_file>: Path to the JSON file as a string [Optional]"
     )
     click.echo("    -h, --help: Show this message and exit.")
     click.echo(
         "Note: Either yaml_file or json_file is required along with output_file."
     )
-    click.echo("Example: json-to-markdown -o output.md -y data.yaml")
+    click.echo("Example: yaml-to-markdown -o output.md -y data.yaml")
 
 
 @click.command()
 @click.option("-o", "--output-file", "output_file", type=str)
 @click.option("-y", "--yaml-file", "yaml_file", type=str, default=None)
 @click.option("-j", "--json-file", "json_file", type=str, default=None)
 @click.option("-h", "--help", "show_help", default=False, is_flag=True)
```

### Comparing `yaml-to-markdown-0.1.1712379388/src/yaml_to_markdown/convert_test.py` & `yaml-to-markdown-0.1.1712381225/src/yaml_to_markdown/convert_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from io import StringIO
 from unittest.mock import mock_open, patch, Mock
 
 import pytest
 
-from json_to_markdown.convert import convert
+from yaml_to_markdown.convert import convert
 
 _JSON_DATA = '{"key": "value"}'
 
 
 def test_convert_with_no_file() -> None:
     # Execute
     with pytest.raises(
```

### Comparing `yaml-to-markdown-0.1.1712379388/src/yaml_to_markdown/md_converter.py` & `yaml-to-markdown-0.1.1712381225/src/yaml_to_markdown/md_converter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 from typing import Any, Dict, IO, List, Optional, Union, Callable
 
-from json_to_markdown.utils import convert_to_title_case
+from yaml_to_markdown.utils import convert_to_title_case
 
 
 class MDConverter:
     def __init__(self) -> None:
         """
         Converter to convert a JSON object into Markdown.
         """
```

### Comparing `yaml-to-markdown-0.1.1712379388/src/yaml_to_markdown/md_converter_test.py` & `yaml-to-markdown-0.1.1712381225/src/yaml_to_markdown/md_converter_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from copy import deepcopy
 from io import StringIO
 from typing import Dict, Any
 
 import pytest
 from mock import mock
 
-from json_to_markdown.md_converter import MDConverter
+from yaml_to_markdown.md_converter import MDConverter
 
 _TABLE_ITEMS = [
     {
         "col1": "R1C1",
         "col2": "R1C2",
     },
     {
```

### Comparing `yaml-to-markdown-0.1.1712379388/src/yaml_to_markdown.egg-info/PKG-INFO` & `yaml-to-markdown-0.1.1712381225/src/yaml_to_markdown.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: yaml-to-markdown
-Version: 0.1.1712379388
+Version: 0.1.1712381225
 Home-page: https://anevis.github.io/yaml-to-markdown/
 Author: anevis
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: click==8.1.7
 Requires-Dist: jsonschema[format]==4.21.1
 Requires-Dist: pyyaml==6.0.1
 
-# JSON to Markdown Converter
+# YAML to Markdown Converter
 
 A Python utility to take a JSON / YAML file or a python dict / list and create a Markdown file.
 
 ## Usage
 
 ### In Python Code example:
```

### Comparing `yaml-to-markdown-0.1.1712379388/src/yaml_to_markdown.egg-info/SOURCES.txt` & `yaml-to-markdown-0.1.1712381225/src/yaml_to_markdown.egg-info/SOURCES.txt`

 * *Files identical despite different names*

