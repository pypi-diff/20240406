# Comparing `tmp/nbdocs-0.2.2.tar.gz` & `tmp/nbdocs-0.3.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nbdocs-0.2.2.tar", last modified: Wed May 24 10:52:15 2023, max compression
+gzip compressed data, was "nbdocs-0.3.dev0.tar", last modified: Sat Apr  6 12:33:53 2024, max compression
```

## Comparing `nbdocs-0.2.2.tar` & `nbdocs-0.3.dev0.tar`

### file list

```diff
@@ -1,45 +1,50 @@
-drwxrwxr-x   0 aya       (1000) aya       (1000)        0 2023-05-24 10:52:15.247217 nbdocs-0.2.2/
--rw-rw-r--   0 aya       (1000) aya       (1000)    11348 2022-05-11 12:40:15.000000 nbdocs-0.2.2/LICENSE
--rw-rw-r--   0 aya       (1000) aya       (1000)      518 2023-05-24 10:52:15.247217 nbdocs-0.2.2/PKG-INFO
--rw-rw-r--   0 aya       (1000) aya       (1000)       45 2022-02-09 06:21:26.000000 nbdocs-0.2.2/README.md
--rw-rw-r--   0 aya       (1000) aya       (1000)      229 2022-05-30 14:55:48.000000 nbdocs-0.2.2/pyproject.toml
--rw-rw-r--   0 aya       (1000) aya       (1000)      871 2023-05-24 10:52:15.247217 nbdocs-0.2.2/setup.cfg
--rw-rw-r--   0 aya       (1000) aya       (1000)      597 2022-05-27 11:09:38.000000 nbdocs-0.2.2/setup.py
-drwxrwxr-x   0 aya       (1000) aya       (1000)        0 2023-05-24 10:52:15.239217 nbdocs-0.2.2/src/
-drwxrwxr-x   0 aya       (1000) aya       (1000)        0 2023-05-24 10:52:15.243217 nbdocs-0.2.2/src/nbdocs/
--rw-rw-r--   0 aya       (1000) aya       (1000)       39 2022-05-27 11:09:38.000000 nbdocs-0.2.2/src/nbdocs/__init__.py
--rw-rw-r--   0 aya       (1000) aya       (1000)       48 2023-05-23 08:14:45.000000 nbdocs-0.2.2/src/nbdocs/__main__.py
-drwxrwxr-x   0 aya       (1000) aya       (1000)        0 2023-05-24 10:52:15.247217 nbdocs-0.2.2/src/nbdocs/apps/
--rw-rw-r--   0 aya       (1000) aya       (1000)        0 2022-05-11 12:40:15.000000 nbdocs-0.2.2/src/nbdocs/apps/__init__.py
--rw-rw-r--   0 aya       (1000) aya       (1000)     2737 2023-05-24 10:48:02.000000 nbdocs-0.2.2/src/nbdocs/apps/app_nb2md.py
--rw-rw-r--   0 aya       (1000) aya       (1000)     1434 2023-05-24 10:48:02.000000 nbdocs-0.2.2/src/nbdocs/apps/app_nbclean.py
--rw-rw-r--   0 aya       (1000) aya       (1000)     3224 2023-05-24 10:48:02.000000 nbdocs-0.2.2/src/nbdocs/apps/app_nbdocs.py
--rw-rw-r--   0 aya       (1000) aya       (1000)     2697 2023-05-24 10:48:02.000000 nbdocs-0.2.2/src/nbdocs/cfg_tools.py
--rw-rw-r--   0 aya       (1000) aya       (1000)     5077 2023-05-17 15:24:05.000000 nbdocs-0.2.2/src/nbdocs/clean.py
--rw-rw-r--   0 aya       (1000) aya       (1000)     4520 2023-05-24 10:48:02.000000 nbdocs-0.2.2/src/nbdocs/convert.py
--rw-rw-r--   0 aya       (1000) aya       (1000)     2014 2023-05-23 08:14:45.000000 nbdocs-0.2.2/src/nbdocs/core.py
--rw-rw-r--   0 aya       (1000) aya       (1000)     1188 2023-05-24 10:48:02.000000 nbdocs-0.2.2/src/nbdocs/default_settings.py
--rw-rw-r--   0 aya       (1000) aya       (1000)    11541 2023-05-24 10:48:02.000000 nbdocs-0.2.2/src/nbdocs/process.py
-drwxrwxr-x   0 aya       (1000) aya       (1000)        0 2023-05-24 10:52:15.247217 nbdocs-0.2.2/src/nbdocs/tests/
--rw-rw-r--   0 aya       (1000) aya       (1000)        0 2022-05-29 14:45:46.000000 nbdocs-0.2.2/src/nbdocs/tests/__init__.py
--rw-rw-r--   0 aya       (1000) aya       (1000)     4066 2023-05-22 08:43:58.000000 nbdocs-0.2.2/src/nbdocs/tests/base.py
--rw-rw-r--   0 aya       (1000) aya       (1000)     2746 2023-05-22 08:43:58.000000 nbdocs-0.2.2/src/nbdocs/typing.py
--rw-rw-r--   0 aya       (1000) aya       (1000)       22 2023-05-24 10:50:59.000000 nbdocs-0.2.2/src/nbdocs/version.py
-drwxrwxr-x   0 aya       (1000) aya       (1000)        0 2023-05-24 10:52:15.243217 nbdocs-0.2.2/src/nbdocs.egg-info/
--rw-rw-r--   0 aya       (1000) aya       (1000)      518 2023-05-24 10:52:15.000000 nbdocs-0.2.2/src/nbdocs.egg-info/PKG-INFO
--rw-rw-r--   0 aya       (1000) aya       (1000)      889 2023-05-24 10:52:15.000000 nbdocs-0.2.2/src/nbdocs.egg-info/SOURCES.txt
--rw-rw-r--   0 aya       (1000) aya       (1000)        1 2023-05-24 10:52:15.000000 nbdocs-0.2.2/src/nbdocs.egg-info/dependency_links.txt
--rw-rw-r--   0 aya       (1000) aya       (1000)      252 2023-05-24 10:52:15.000000 nbdocs-0.2.2/src/nbdocs.egg-info/entry_points.txt
--rw-rw-r--   0 aya       (1000) aya       (1000)       88 2023-05-24 10:52:15.000000 nbdocs-0.2.2/src/nbdocs.egg-info/requires.txt
--rw-rw-r--   0 aya       (1000) aya       (1000)        7 2023-05-24 10:52:15.000000 nbdocs-0.2.2/src/nbdocs.egg-info/top_level.txt
-drwxrwxr-x   0 aya       (1000) aya       (1000)        0 2023-05-24 10:52:15.247217 nbdocs-0.2.2/tests/
--rw-rw-r--   0 aya       (1000) aya       (1000)     3332 2023-05-23 08:14:45.000000 nbdocs-0.2.2/tests/test_apps.py
--rw-rw-r--   0 aya       (1000) aya       (1000)     3108 2023-05-22 08:43:36.000000 nbdocs-0.2.2/tests/test_base.py
--rw-rw-r--   0 aya       (1000) aya       (1000)     1499 2023-05-22 08:43:36.000000 nbdocs-0.2.2/tests/test_clean.py
--rw-rw-r--   0 aya       (1000) aya       (1000)     3697 2023-05-24 10:48:02.000000 nbdocs-0.2.2/tests/test_convert.py
--rw-rw-r--   0 aya       (1000) aya       (1000)     2123 2023-05-24 10:48:02.000000 nbdocs-0.2.2/tests/test_core.py
--rw-rw-r--   0 aya       (1000) aya       (1000)     1665 2023-05-03 13:42:07.000000 nbdocs-0.2.2/tests/test_process_collapse.py
--rw-rw-r--   0 aya       (1000) aya       (1000)     2433 2023-05-03 13:42:07.000000 nbdocs-0.2.2/tests/test_process_hide.py
--rw-rw-r--   0 aya       (1000) aya       (1000)     4577 2023-05-24 10:48:02.000000 nbdocs-0.2.2/tests/test_process_links.py
--rw-rw-r--   0 aya       (1000) aya       (1000)     1053 2023-05-03 08:06:54.000000 nbdocs-0.2.2/tests/test_process_re.py
--rw-rw-r--   0 aya       (1000) aya       (1000)     2102 2023-05-24 10:48:02.000000 nbdocs-0.2.2/tests/test_settings.py
+drwxrwxr-x   0 aya       (1000) aya       (1000)        0 2024-04-06 12:33:53.194941 nbdocs-0.3.dev0/
+-rw-rw-r--   0 aya       (1000) aya       (1000)    11348 2022-05-11 12:40:15.000000 nbdocs-0.3.dev0/LICENSE
+-rw-r--r--   0 aya       (1000) aya       (1000)     1063 2024-04-06 12:33:53.194941 nbdocs-0.3.dev0/PKG-INFO
+-rw-rw-r--   0 aya       (1000) aya       (1000)       45 2023-05-25 08:34:09.000000 nbdocs-0.3.dev0/README.md
+-rw-rw-r--   0 aya       (1000) aya       (1000)     1311 2024-03-25 08:25:06.000000 nbdocs-0.3.dev0/pyproject.toml
+-rw-rw-r--   0 aya       (1000) aya       (1000)     1036 2024-04-06 12:33:53.194941 nbdocs-0.3.dev0/setup.cfg
+-rw-rw-r--   0 aya       (1000) aya       (1000)      852 2024-03-25 08:25:06.000000 nbdocs-0.3.dev0/setup.py
+drwxrwxr-x   0 aya       (1000) aya       (1000)        0 2024-04-06 12:33:53.190941 nbdocs-0.3.dev0/src/
+drwxrwxr-x   0 aya       (1000) aya       (1000)        0 2024-04-06 12:33:53.190941 nbdocs-0.3.dev0/src/nbdocs/
+-rw-rw-r--   0 aya       (1000) aya       (1000)       39 2022-05-27 11:09:38.000000 nbdocs-0.3.dev0/src/nbdocs/__init__.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)       46 2024-03-25 08:25:06.000000 nbdocs-0.3.dev0/src/nbdocs/__main__.py
+drwxrwxr-x   0 aya       (1000) aya       (1000)        0 2024-04-06 12:33:53.190941 nbdocs-0.3.dev0/src/nbdocs/apps/
+-rw-rw-r--   0 aya       (1000) aya       (1000)        0 2022-05-11 12:40:15.000000 nbdocs-0.3.dev0/src/nbdocs/apps/__init__.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)     2527 2024-03-25 08:25:06.000000 nbdocs-0.3.dev0/src/nbdocs/apps/app_nb2md.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)     1530 2024-03-25 08:25:06.000000 nbdocs-0.3.dev0/src/nbdocs/apps/app_nbclean.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)     2871 2024-03-25 08:25:06.000000 nbdocs-0.3.dev0/src/nbdocs/apps/app_nbdocs.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)     2675 2024-03-25 08:25:06.000000 nbdocs-0.3.dev0/src/nbdocs/cfg_tools.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)     5209 2024-03-25 08:25:06.000000 nbdocs-0.3.dev0/src/nbdocs/clean.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)     4552 2024-03-26 15:38:32.000000 nbdocs-0.3.dev0/src/nbdocs/convert.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)     2562 2024-03-25 08:25:06.000000 nbdocs-0.3.dev0/src/nbdocs/core.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)     1188 2023-05-24 10:48:02.000000 nbdocs-0.3.dev0/src/nbdocs/default_settings.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)      698 2024-03-27 12:20:42.000000 nbdocs-0.3.dev0/src/nbdocs/flags.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)      983 2024-03-25 08:25:06.000000 nbdocs-0.3.dev0/src/nbdocs/helpers.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)     1169 2024-03-26 08:02:11.000000 nbdocs-0.3.dev0/src/nbdocs/process_cell.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)     2280 2024-03-27 08:54:38.000000 nbdocs-0.3.dev0/src/nbdocs/process_md.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)     1570 2024-03-27 09:07:57.000000 nbdocs-0.3.dev0/src/nbdocs/re_tools.py
+drwxrwxr-x   0 aya       (1000) aya       (1000)        0 2024-04-06 12:33:53.190941 nbdocs-0.3.dev0/src/nbdocs/tests/
+-rw-rw-r--   0 aya       (1000) aya       (1000)        0 2022-05-29 14:45:46.000000 nbdocs-0.3.dev0/src/nbdocs/tests/__init__.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)     4066 2023-05-22 08:43:58.000000 nbdocs-0.3.dev0/src/nbdocs/tests/base.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)     2732 2024-03-25 08:25:06.000000 nbdocs-0.3.dev0/src/nbdocs/typing.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)       24 2024-03-25 08:25:06.000000 nbdocs-0.3.dev0/src/nbdocs/version.py
+drwxrwxr-x   0 aya       (1000) aya       (1000)        0 2024-04-06 12:33:53.194941 nbdocs-0.3.dev0/src/nbdocs.egg-info/
+-rw-r--r--   0 aya       (1000) aya       (1000)     1063 2024-04-06 12:33:53.000000 nbdocs-0.3.dev0/src/nbdocs.egg-info/PKG-INFO
+-rw-rw-r--   0 aya       (1000) aya       (1000)     1004 2024-04-06 12:33:53.000000 nbdocs-0.3.dev0/src/nbdocs.egg-info/SOURCES.txt
+-rw-rw-r--   0 aya       (1000) aya       (1000)        1 2024-04-06 12:33:53.000000 nbdocs-0.3.dev0/src/nbdocs.egg-info/dependency_links.txt
+-rw-rw-r--   0 aya       (1000) aya       (1000)      256 2024-04-06 12:33:53.000000 nbdocs-0.3.dev0/src/nbdocs.egg-info/entry_points.txt
+-rw-rw-r--   0 aya       (1000) aya       (1000)      112 2024-04-06 12:33:53.000000 nbdocs-0.3.dev0/src/nbdocs.egg-info/requires.txt
+-rw-rw-r--   0 aya       (1000) aya       (1000)        7 2024-04-06 12:33:53.000000 nbdocs-0.3.dev0/src/nbdocs.egg-info/top_level.txt
+drwxrwxr-x   0 aya       (1000) aya       (1000)        0 2024-04-06 12:33:53.194941 nbdocs-0.3.dev0/tests/
+-rw-rw-r--   0 aya       (1000) aya       (1000)     3346 2024-03-25 08:25:06.000000 nbdocs-0.3.dev0/tests/test_apps.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)     3147 2024-03-25 08:25:06.000000 nbdocs-0.3.dev0/tests/test_base.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)     1499 2023-05-22 08:43:36.000000 nbdocs-0.3.dev0/tests/test_clean.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)     3748 2024-03-26 14:52:43.000000 nbdocs-0.3.dev0/tests/test_convert.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)      892 2024-03-26 11:26:11.000000 nbdocs-0.3.dev0/tests/test_convert_base.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)     2625 2024-03-25 08:25:06.000000 nbdocs-0.3.dev0/tests/test_core.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)     1131 2024-03-27 09:01:04.000000 nbdocs-0.3.dev0/tests/test_process_base.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)     1650 2024-03-26 11:53:33.000000 nbdocs-0.3.dev0/tests/test_process_cell.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)     4121 2024-03-27 08:55:18.000000 nbdocs-0.3.dev0/tests/test_process_md.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)     2481 2024-03-26 14:34:37.000000 nbdocs-0.3.dev0/tests/test_process_re.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)     2102 2023-05-24 10:48:02.000000 nbdocs-0.3.dev0/tests/test_settings.py
```

### Comparing `nbdocs-0.2.2/LICENSE` & `nbdocs-0.3.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `nbdocs-0.2.2/setup.cfg` & `nbdocs-0.3.dev0/setup.cfg`

 * *Files 23% similar despite different names*

```diff
@@ -5,34 +5,38 @@
 author_email = a.yasyrev@gmail.com
 description = Docs from jupyter notebooks.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/ayasyrev/nbdocs
 license = apache2
 classifiers = 
-	Programming Language :: Python :: 3
+	Programming Language :: Python :: 3.8
+	Programming Language :: Python :: 3.9
+	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
+	Programming Language :: Python :: 3.12
 	License :: OSI Approved :: Apache Software License
 	Operating System :: OS Independent
 
 [options]
 package_dir = 
 	= src
 packages = find:
 python_requires = >=3.8
 
 [options.packages.find]
 where = src
 
 [options.entry_points]
 console_scripts = 
-	nbdocs=nbdocs.apps.app_nbdocs:main
-	nb2md=nbdocs.apps.app_nb2md:main
+	nbdocs=nbdocs.apps.app_nbdocs:app
+	nb2md=nbdocs.apps.app_nb2md:convert
 	nbclean=nbdocs.apps.app_nbclean:main
 pipx.run = 
-	nbdocs=nbdocs.apps.app_nbdocs:main
-	nb2md=nbdocs.apps.app_nb2md:main
+	nbdocs=nbdocs.apps.app_nbdocs:app
+	nb2md=nbdocs.apps.app_nb2md:convert
 	nbclean=nbdocs.apps.app_nbclean:main
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `nbdocs-0.2.2/setup.py` & `nbdocs-0.3.dev0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from setuptools import setup
 
 
-REQUIREMENTS_FILENAME = 'requirements.txt'
-REQUIREMENTS_TEST_FILENAME = 'requirements_test.txt'
+REQUIREMENTS_FILENAME = "requirements.txt"
+REQUIREMENTS_TEST_FILENAME = "requirements_test.txt"
+REQUIREMENTS_DOCS_FILENAME = "requirements_docs.txt"
 
 
 # Requirements
 try:
     with open(REQUIREMENTS_FILENAME, encoding="utf-8") as fh:
         REQUIRED = fh.read().split("\n")
 except FileNotFoundError:
@@ -14,15 +15,24 @@
 
 try:
     with open(REQUIREMENTS_TEST_FILENAME, encoding="utf-8") as fh:
         TEST_REQUIRED = fh.read().split("\n")
 except FileNotFoundError:
     TEST_REQUIRED = []
 
+try:
+    with open(REQUIREMENTS_DOCS_FILENAME, encoding="utf-8") as fh:
+        DOCS_REQUIRED = fh.read().split("\n")
+except FileNotFoundError:
+    DOCS_REQUIRED = []
+
 # What packages are optional?
-EXTRAS = {"test": TEST_REQUIRED}
+EXTRAS = {
+    "test": TEST_REQUIRED,
+    "docs": DOCS_REQUIRED,
+}
 
 
 setup(
     install_requires=REQUIRED,
     extras_require=EXTRAS,
 )
```

### Comparing `nbdocs-0.2.2/src/nbdocs/apps/app_nb2md.py` & `nbdocs-0.3.dev0/src/nbdocs/apps/app_nb2md.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,18 @@
+import sys
 from dataclasses import dataclass
 from pathlib import Path
-import sys
-from typing import Optional, Sequence
 
-from argparsecfg import ArgumentParserCfg, field_argument, parse_args
+from argparsecfg import field_argument
+from argparsecfg.app import app
 from rich import print as rprint
 
+from nbdocs.cfg_tools import get_config
 from nbdocs.convert import convert2md, filter_changed
 from nbdocs.core import get_nb_names
-from nbdocs.cfg_tools import get_config
-
-
-parser_cfg = ArgumentParserCfg(description="Nb2Md. Convert notebooks to Markdown.")
 
 
 @dataclass
 class AppConfig:
     nb_path: str = field_argument(
         "nb_path",
         help="Path to NB or folder with Nbs to convert",
@@ -39,14 +36,17 @@
         "-s",
         default=False,
         action="store_true",
         help="Run in silent mode.",
     )
 
 
+@app(
+    description="Nb2Md. Convert notebooks to Markdown.",
+)
 def convert(
     app_cfg: AppConfig,
 ) -> None:
     """Nb2Md. Convert notebooks to Markdown."""
     nb_names = get_nb_names(app_cfg.nb_path)
     nbs_number = len(nb_names)
     if nbs_number == 0:
@@ -78,21 +78,14 @@
         rprint("No files with changes to convert!")
         sys.exit()
 
     if not app_cfg.silent_mode:
         print(f"Files to convert from {nb_names[0].parent}:")
         for fn in nb_names:
             print(f"    {fn.name}")
-        print(
-            f"Destination directory: {app_cfg.dest_path},\nImage directory: {cfg.images_path}"
-        )
+        print(f"Destination directory: {app_cfg.dest_path},\nImage directory: {cfg.images_path}")
 
     convert2md(nb_names, cfg)
 
 
-def main(args: Optional[Sequence[str]] = None) -> None:
-    app_cfg = parse_args(AppConfig, parser_cfg, args)
-    convert(app_cfg)
-
-
 if __name__ == "__main__":  # pragma: no cover
-    main()
+    convert()
```

### Comparing `nbdocs-0.2.2/src/nbdocs/apps/app_nbclean.py` & `nbdocs-0.3.dev0/src/nbdocs/apps/app_nbclean.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,54 +1,56 @@
 import sys
 from dataclasses import dataclass
-from typing import Optional, Sequence
 
-from argparsecfg import field_argument, parse_args, ArgumentParserCfg
+from argparsecfg import field_argument
+from argparsecfg.app import app
 from rich import print as rprint
 
+from nbdocs.cfg_tools import get_config
 from nbdocs.clean import clean_nb_file
 from nbdocs.core import get_nb_names
-from nbdocs.cfg_tools import get_config
-
-
-parser_cfg = ArgumentParserCfg(
-    description="Clean Nb or notebooks at `nb_path` - metadata and execution counts from nbs."
-)
 
 
 @dataclass
 class AppConfig:
     """Config for `app_nbclean`."""
 
     nb_path: str = field_argument(
-        "nb_path", help="Path to NB or folder with Nbs to clean"
+        "-p",
+        flag="--path",
+        default=None,
+        help="Path to NB or folder with Nbs to clean. If no path - from cfg.",
     )
     clear_execution_count: bool = field_argument(
         flag="--no-ec",
         default=True,
         action="store_false",
-        help="Clean execution counts.",
+        help="Dont clean execution counts.",
     )
 
 
+# @app(
+#     description="Clean Nb or notebooks at `nb_path` - metadata and execution counts from nbs."
+# )
 def nbclean(app_cfg: AppConfig) -> None:
     """Clean Nb or notebooks at `nb_path` - metadata and execution counts from nbs."""
     cfg = get_config(notebooks_path=app_cfg.nb_path)
 
     nb_names = get_nb_names(cfg.notebooks_path)
 
     if (num_nbs := len(nb_names)) == 0:
         rprint("No files to clean!")
         sys.exit()
 
     rprint(f"Clean: {cfg.notebooks_path}, found {num_nbs} notebooks.")
 
-    clean_nb_file(nb_names, app_cfg.clear_execution_count)
+    cleaned = clean_nb_file(nb_names, app_cfg.clear_execution_count)
+    if len(cleaned) == 0:
+        rprint("All notebooks were clean.")
 
 
-def main(args: Optional[Sequence[str]] = None) -> None:
-    app_cfg = parse_args(AppConfig, parser_cfg, args)
-    nbclean(app_cfg)
+main = app(description="Clean Nb or notebooks at `nb_path` - metadata and execution counts from nbs.")(nbclean)
 
 
 if __name__ == "__main__":  # pragma: no cover
+    # nbclean()
     main()
```

### Comparing `nbdocs-0.2.2/src/nbdocs/apps/app_nbdocs.py` & `nbdocs-0.3.dev0/src/nbdocs/apps/app_nbdocs.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,50 +1,47 @@
-from pathlib import Path
 import sys
 from dataclasses import dataclass
-from typing import Optional, Sequence
+from pathlib import Path
 
-from argparsecfg import (
-    ArgumentParserCfg,
-    add_args_from_dc,
-    create_dc_obj,
-    create_parser,
-    field_argument,
-)
+from argparsecfg import field_argument
+from argparsecfg.app import App
 from rich import print as rprint
 
-from nbdocs.convert import convert2md, filter_changed
-from nbdocs.core import get_nb_names
+from nbdocs.apps.app_nbclean import nbclean
 from nbdocs.cfg_tools import get_config
+from nbdocs.convert import convert2md, filter_changed
+from nbdocs.core import get_nb_names, get_readme_fn, process_readme
 from nbdocs.default_settings import (
-    NBDOCS_SETTINGS,
-    MKDOCS_BASE,
-    MATERIAL_BASE,
     FOOTER_HTML,
+    MATERIAL_BASE,
+    MKDOCS_BASE,
+    NBDOCS_SETTINGS,
 )
 
-parser_cfg = ArgumentParserCfg(
-    description="NbDocs. Convert notebooks to docs. Default to .md"
-)
+
+app = App(description="NbDocs. Convert notebooks to docs. Default to .md")
 
 
 @dataclass
 class AppConfig:
     force: bool = field_argument(
         "-F",
         default=False,
+        action="store_true",
         help="Force convert all notebooks.",
     )
 
 
+@app.main
 def nbdocs(
     app_cfg: AppConfig,
 ) -> None:
     """NbDocs. Convert notebooks to docs. Default to .md"""
     cfg = get_config()
+    # todo - add warning if no cfg
     nb_names = get_nb_names(cfg.notebooks_path)
     nbs_number = len(nb_names)
     if nbs_number == 0:
         rprint("No files to convert!")
         sys.exit()
     rprint(f"Found {nbs_number} notebooks.")
     if not app_cfg.force:
@@ -56,26 +53,34 @@
 
     if len(nb_names) == 0:
         rprint("No files to convert!")
         sys.exit()
 
     rprint(f"To convert: {len(nb_names)} notebooks.")
     convert2md(nb_names, cfg)
+    readme_nb = get_readme_fn(nb_names)
+    if readme_nb is not None:
+        with open(f"{cfg.docs_path}/README.md", "r", encoding="utf-8") as fh:
+            readme = fh.read()
+        with open(f"{cfg.cfg_path}/README.md", "w", encoding="utf-8") as fh:
+            fh.write(process_readme(readme))
+        rprint("Readme updated.")
 
 
 @dataclass
 class SetupCfg:
     clean: bool = field_argument(
         "-c",
         default=False,
         action="store_true",
         help="Clean MkDocs setup.",
     )
 
 
+@app.command
 def setup(cfg: SetupCfg) -> None:
     """Initialize config."""
     rprint("Settings up NbDocs.")
     # create nbdocs config - nbdocs.ini
     with open("nbdocs.ini", "w", encoding="utf-8") as f:
         f.write(NBDOCS_SETTINGS)
     # create mkdocs config - mkdocs.yaml
@@ -88,28 +93,12 @@
         with open(filename, "w", encoding="utf-8") as f:
             f.write(FOOTER_HTML)
     with open("mkdocs.yaml", "w", encoding="utf-8") as f:
         f.write(mkdocs_setup)
     rprint("Done.")
 
 
-def main(args: Optional[Sequence[str]] = None) -> None:
-    parser = create_parser(parser_cfg)
-    add_args_from_dc(parser, AppConfig)
-    subparsers = parser.add_subparsers(title="Commands", help="Available commands.")
-    parser_init = subparsers.add_parser(
-        "init", help="Initialize config", description="Initialize NbDocs config"
-    )
-    parser_init.set_defaults(command="init")
-    add_args_from_dc(parser_init, SetupCfg)
-    parsed_args = parser.parse_args(args=args)
-    if hasattr(parsed_args, "command"):
-        if parsed_args.command == "init":
-            setup_cfg = create_dc_obj(SetupCfg, parsed_args)
-            setup(setup_cfg)
-    else:
-        app_cfg = create_dc_obj(AppConfig, parsed_args)
-        nbdocs(app_cfg)
+app.command(nbclean)
 
 
 if __name__ == "__main__":
-    main()
+    app()
```

### Comparing `nbdocs-0.2.2/src/nbdocs/cfg_tools.py` & `nbdocs-0.3.dev0/src/nbdocs/cfg_tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,17 +47,15 @@
 def read_ini_config(config_name: PathOrStr) -> configparser.SectionProxy:
     """return nbdocs config section from INI config."""
     cfg = ConfigParser()
     cfg.read(config_name)
     try:
         section = cfg[SECTION_NAME]
     except KeyError as exc:
-        raise KeyError(
-            f"No section {SECTION_NAME} at config file {config_name}"
-        ) from exc
+        raise KeyError(f"No section {SECTION_NAME} at config file {config_name}") from exc
     return section
 
 
 # def get_config_toml(config_name: PosixPath):
 #     """return nbdocs config section from TOML config."""
 #     cfg_tool = toml.load(config_name).get("tool", None)
 #     if cfg_tool is not None:
```

### Comparing `nbdocs-0.2.2/src/nbdocs/clean.py` & `nbdocs-0.3.dev0/src/nbdocs/clean.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,17 +24,15 @@
         All the code cells are returned with an empty metadata field.
         """
         if self.clear_cell_metadata:
             if cell.cell_type == "code":
                 # Remove metadata
                 if cell.metadata:
                     current_metadata = cell.metadata
-                    cell, resources = super().preprocess_cell(
-                        cell, resources, cell_index
-                    )
+                    cell, resources = super().preprocess_cell(cell, resources, cell_index)
                     if cell.metadata != current_metadata:
                         resources["changed"] = True
         return cell, resources
 
     def preprocess(self, nb: Nb, resources: ResourcesDict) -> NbAndResources:
         """
         Preprocessing to apply on each notebook.
@@ -88,20 +86,16 @@
 
 class MetadataCleaner:
     """Metadata cleaner.
     Wrapper for metadata and execution count preprocessors.
     """
 
     def __init__(self) -> None:
-        self.cleaner_metadata: TPreprocessor = ClearMetadataPreprocessorRes(
-            enabled=True
-        )
-        self.cleaner_execution_count: TPreprocessor = ClearExecutionCountPreprocessor(
-            enabled=True
-        )
+        self.cleaner_metadata: TPreprocessor = ClearMetadataPreprocessorRes(enabled=True)
+        self.cleaner_execution_count: TPreprocessor = ClearExecutionCountPreprocessor(enabled=True)
 
     def __call__(
         self,
         nb: Nb,
         resources: ResourcesDict | None = None,
         clear_execution_count: bool = True,
     ) -> NbAndResources:
@@ -124,24 +118,30 @@
     return cleaner(nb, clear_execution_count=clear_execution_count)
 
 
 def clean_nb_file(
     fn: PathOrStr | list[PathOrStr],
     clear_execution_count: bool = True,
     as_version: nbformat.Sentinel = nbformat.NO_CONVERT,
-) -> None:
+    silent: bool = False,
+) -> list[PathOrStr]:
     """Clean metadata and execution count from notebook.
 
     Args:
         fn (Union[str, PosixPath]): Notebook filename or list of names.
         as_version (int, optional): Nbformat version. Defaults to 4.
         clear_execution_count (bool, optional): Clean execution count. Defaults to True.
+        silent (bool, optional): Silent mode. Defaults to False.
     """
     cleaner = MetadataCleaner()
     if not isinstance(fn, list):
         fn = [fn]
+    cleaned: list[PathOrStr] = []
     for fn_item in track(fn, transient=True):
         nb = read_nb(fn_item, as_version)
         nb, resources = cleaner(nb, clear_execution_count=clear_execution_count)
         if resources["changed"]:
+            cleaned.append(fn_item)
             write_nb(nb, fn_item, as_version)
-            print(f"done: {fn_item}")
+            if not silent:
+                print(f"done: {fn_item}")
+    return cleaned
```

### Comparing `nbdocs-0.2.2/src/nbdocs/core.py` & `nbdocs-0.3.dev0/src/nbdocs/core.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     """Write notebook to file
 
     Args:
         nb (Notebook): Notebook to write
         fn (Union[str, PosixPath]): filename to write
         as_version (_type_, optional): Nbformat version. Defaults to nbformat.NO_CONVERT.
     Returns:
-        Path: Filename of writed Nb.
+        Path: Filename of written Nb.
     """
     filename = Path(fn)
     if filename.suffix != ".ipynb":
         filename = filename.with_suffix(".ipynb")
     with filename.open("w", encoding="utf-8") as fh:
         nbformat.write(nb, fh, version=as_version)  # type: ignore
     return filename
@@ -68,7 +68,29 @@
         return list(path.glob("*.ipynb"))
 
     if path.suffix != ".ipynb":
         rprint(f"Nb extension must be .ipynb, but got: {path.suffix}")
         sys.exit()
 
     return [path]
+
+
+def get_readme_fn(nb_names: list[Path]) -> Path | None:
+    """Find notebook for readme. Return filename or None.
+
+    Args:
+        nb_names (List[Path]): List of notebooks.
+
+    Returns:
+        Path | None: Filename or None.
+    """
+    for nb_name in nb_names:
+        if nb_name.stem == "README":
+            return nb_name
+    return None
+
+
+def process_readme(text: str) -> str:
+    """Clear readme file - remove YAML Style Meta-Data."""
+    if text.startswith("---"):
+        text = "".join(text.split("---")[2:]).strip()
+    return text
```

### Comparing `nbdocs-0.2.2/src/nbdocs/default_settings.py` & `nbdocs-0.3.dev0/src/nbdocs/default_settings.py`

 * *Files identical despite different names*

### Comparing `nbdocs-0.2.2/src/nbdocs/tests/base.py` & `nbdocs-0.3.dev0/src/nbdocs/tests/base.py`

 * *Files identical despite different names*

### Comparing `nbdocs-0.2.2/src/nbdocs/typing.py` & `nbdocs-0.3.dev0/src/nbdocs/typing.py`

 * *Files 7% similar despite different names*

```diff
@@ -107,11 +107,9 @@
 
     def __call__(self, nb: Nb, resources: ResourcesDict) -> NbAndResources:
         return nb, resources  # pragma: no cover
 
     def preprocess(self, nb: Nb, resources: ResourcesDict) -> NbAndResources:
         return nb, resources  # pragma: no cover
 
-    def preprocess_cell(
-        self, cell: Cell, resources: ResourcesDict, index: int
-    ) -> CellAndResources:
+    def preprocess_cell(self, cell: Cell, resources: ResourcesDict, index: int) -> CellAndResources:
         return cell, resources  # pragma: no cover
```

### Comparing `nbdocs-0.2.2/src/nbdocs.egg-info/SOURCES.txt` & `nbdocs-0.3.dev0/src/nbdocs.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,19 @@
 src/nbdocs/__init__.py
 src/nbdocs/__main__.py
 src/nbdocs/cfg_tools.py
 src/nbdocs/clean.py
 src/nbdocs/convert.py
 src/nbdocs/core.py
 src/nbdocs/default_settings.py
-src/nbdocs/process.py
+src/nbdocs/flags.py
+src/nbdocs/helpers.py
+src/nbdocs/process_cell.py
+src/nbdocs/process_md.py
+src/nbdocs/re_tools.py
 src/nbdocs/typing.py
 src/nbdocs/version.py
 src/nbdocs.egg-info/PKG-INFO
 src/nbdocs.egg-info/SOURCES.txt
 src/nbdocs.egg-info/dependency_links.txt
 src/nbdocs.egg-info/entry_points.txt
 src/nbdocs.egg-info/requires.txt
@@ -25,13 +29,14 @@
 src/nbdocs/apps/app_nbdocs.py
 src/nbdocs/tests/__init__.py
 src/nbdocs/tests/base.py
 tests/test_apps.py
 tests/test_base.py
 tests/test_clean.py
 tests/test_convert.py
+tests/test_convert_base.py
 tests/test_core.py
-tests/test_process_collapse.py
-tests/test_process_hide.py
-tests/test_process_links.py
+tests/test_process_base.py
+tests/test_process_cell.py
+tests/test_process_md.py
 tests/test_process_re.py
 tests/test_settings.py
```

### Comparing `nbdocs-0.2.2/tests/test_apps.py` & `nbdocs-0.3.dev0/tests/test_apps.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,68 +1,68 @@
 from pathlib import Path
 from pytest import CaptureFixture
 
 from nbdocs.apps.app_nbclean import main as app_nbclean
 
-from nbdocs.apps.app_nb2md import main as app_nb2md
+from nbdocs.apps.app_nb2md import convert as app_nb2md
 
 
 def test_app_nbclean_def(capsys: CaptureFixture[str]):
     """Test default run"""
-    # result = runner.invoke(app_nbclean)
     # run without args
-    try:
-        app_nbclean([])
-    except SystemExit as e:
-        assert e.code == 2
+    # try:
+    app_nbclean([])
+    # except SystemExit as e:
+    #     assert e.code == 2
     captured = capsys.readouterr()
     out = captured.out
-    assert out == ""
+    assert "Clean: nbs, found 1 notebooks." in out
+    assert "All notebooks were clean." in out
     error_out = captured.err
-    assert "error: the following arguments are required: nb_path" in error_out
+    assert "" == error_out
 
 
 def test_app_nbclean_no_nb(capsys: CaptureFixture[str]):
-    """Test if no Nb at path aor path not exist"""
+    """Test if no Nb at path or path not exist"""
     try:
-        app_nbclean(["."])
+        app_nbclean(["-p", "."])
     except SystemExit as e:
         assert e.code is None
 
     captured = capsys.readouterr()
     out = captured.out
     assert "No files to clean!" in out
     err_out = captured.err
     assert err_out == ""
 
     try:
-        app_nbclean(["not_exist_path"])
+        app_nbclean(["-p", "not_exist_path"])
     except SystemExit as e:  # pragma: no cover
         assert e.code is None
     captured = capsys.readouterr()
     out = captured.out
     assert "not exists!" in out
     err_out = captured.err
     assert err_out == ""
 
 
 def test_app_nbclean(capsys: CaptureFixture[str]):
     """Test nb folder and file run"""
     try:
-        app_nbclean(["tests/test_nbs"])
+        app_nbclean(["--path", "tests/test_nbs"])
     except SystemExit as e:  # pragma: no cover
         assert e.code == 0
     captured = capsys.readouterr()
     out = captured.out
     assert "tests/test_nbs" in out
     err_out = captured.err
     assert err_out == ""
 
     try:
-        app_nbclean(["tests/test_nbs/code_hide_cells.ipynb"])
+        app_nbclean(["-p", "tests/test_nbs/code_hide_cells.ipynb"])
     except SystemExit as e:  # pragma: no cover
         assert e.code == 0
     captured = capsys.readouterr()
     out = captured.out
     assert "tests/test_nbs/code_hide_cells.ipynb" in out
     err_out = captured.err
     assert err_out == ""
@@ -98,15 +98,15 @@
     try:
         app_nb2md(["tests/test_nbs/", "--dest", f"{tmp_path}"])
     except SystemExit as e:  # pragma: no cover
         assert e.code is None
 
     captured = capsys.readouterr()
     out = captured.out
-    assert "Found 4 notebooks" in out
+    assert "Found 7 notebooks" in out
     err_out = captured.err
     assert err_out == ""
     # check for result
 
     # run again - no changes in nbs
     try:
         app_nb2md(["tests/test_nbs/", "--dest", f"{tmp_path}"])
```

### Comparing `nbdocs-0.2.2/tests/test_base.py` & `nbdocs-0.3.dev0/tests/test_base.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 from pathlib import Path
 
+from nbformat.notebooknode import NotebookNode
+
 from nbdocs.tests.base import (
     create_cell_metadata,
     create_nb,
-    create_test_nb,
     create_nb_metadata,
-    create_tmp_image_file,
-    create_test_metadata_nb,
     create_test_metadata_code,
+    create_test_metadata_nb,
+    create_test_nb,
+    create_tmp_image_file,
 )
-from nbdocs.typing import Nb
 
 
 def test_create_nb():
     """test for create_nb"""
     # empty nb
     nb = create_nb()
-    assert isinstance(nb, Nb)
+    assert isinstance(nb, NotebookNode)
     assert len(nb.cells) == 0
     # only code cell
     nb = create_nb("test code")
     assert len(nb.cells) == 1
     assert nb.cells[0].cell_type == "code"
     assert nb.cells[0].source == "test code"
     # only md cell
@@ -37,15 +38,15 @@
     assert nb.cells[1].source == "test md"
 
 
 def test_create_test_nb():
     """test for create_test_nb"""
     # empty nb
     nb = create_test_nb()
-    assert isinstance(nb, Nb)
+    assert isinstance(nb, NotebookNode)
     assert len(nb.cells) == 0
     # only code cell
     nb = create_test_nb("test code")
     assert len(nb.cells) == 1
     assert nb.cells[0].cell_type == "code"
     assert nb.cells[0].source == "test code"
     assert len(nb.cells[0].outputs) == 3
```

### Comparing `nbdocs-0.2.2/tests/test_clean.py` & `nbdocs-0.3.dev0/tests/test_clean.py`

 * *Files identical despite different names*

### Comparing `nbdocs-0.2.2/tests/test_convert.py` & `nbdocs-0.3.dev0/tests/test_convert.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,36 +9,38 @@
 
 
 def test_MdConverter():
     """test for MdConverter"""
     md_converter = MdConverter()
     # md cell
     nb = create_nb(md_source="test_md")
-    md, resources = md_converter.nb2md(nb)
-    assert md == "test_md\n"
+    md, resources = md_converter.from_nb(nb)
+    assert md == "<!-- cell #0 markdown -->\ntest_md\n"
     assert resources["output_extension"] == ".md"
     assert not resources["image_names"]
+
     # code cell
     nb = create_test_nb(code_source="test_code")
-    md, resources = md_converter.nb2md(nb)
+    md, resources = md_converter.from_nb(nb)
     assert "test_code" in md
-    assert "![png](output_0_2.png)" in md
-    assert resources["outputs"] == {"output_0_2.png": b"g"}
-    assert "output_0_2.png" in resources["image_names"]
+    # assert "![png](output_0_2.png)" in md
+    # assert resources["outputs"] == {"output_0_2.png": b"g"}
+    # assert "output_0_2.png" in resources["image_names"]
+
     # code and markdown, call()
     nb = create_test_nb(
         code_source="test_code",
         md_source="![cat](cat.jpg)",
     )
-    md, resources = md_converter(nb)
+    md, resources = md_converter.from_nb(nb)
     assert "test_code" in md
-    assert "![png](output_0_2.png)" in md
-    assert resources["outputs"] == {"output_0_2.png": b"g"}
-    assert "output_0_2.png" in resources["image_names"]
-    assert "cat.jpg" in resources["image_names"]
+    assert "![png](output_1_2.png)" in md
+    assert resources["outputs"] == {"output_1_2.png": b"g"}
+    # assert "output_0_1.png" in resources["image_names"]
+    # assert "cat.jpg" in resources["image_names"]
 
 
 def test_convert2md(tmp_path: Path, capsys: CaptureFixture[str]):
     """test convert2md"""
     cfg = NbDocsCfg()
     image_name = "t_1.png"
     create_tmp_image_file(tmp_path / image_name)
```

### Comparing `nbdocs-0.2.2/tests/test_settings.py` & `nbdocs-0.3.dev0/tests/test_settings.py`

 * *Files identical despite different names*

