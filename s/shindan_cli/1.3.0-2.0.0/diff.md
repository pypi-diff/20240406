# Comparing `tmp/shindan_cli-1.3.0.tar.gz` & `tmp/shindan_cli-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shindan_cli-1.3.0.tar", max compression
+gzip compressed data, was "shindan_cli-2.0.0.tar", max compression
```

## Comparing `shindan_cli-1.3.0.tar` & `shindan_cli-2.0.0.tar`

### file list

```diff
@@ -1,8 +1,12 @@
--rw-r--r--   0        0        0     1066 2023-06-24 20:01:51.737832 shindan_cli-1.3.0/LICENSE
--rw-r--r--   0        0        0     3795 2023-06-24 20:01:51.737832 shindan_cli-1.3.0/README.md
--rw-r--r--   0        0        0     2037 2023-06-24 20:01:51.737832 shindan_cli-1.3.0/pyproject.toml
--rw-r--r--   0        0        0      210 2023-06-24 20:01:51.737832 shindan_cli-1.3.0/shindan_cli/__init__.py
--rw-r--r--   0        0        0     1832 2023-06-24 20:01:51.737832 shindan_cli-1.3.0/shindan_cli/main.py
--rw-r--r--   0        0        0        0 2023-06-24 20:01:51.737832 shindan_cli-1.3.0/shindan_cli/py.typed
--rw-r--r--   0        0        0     2562 2023-06-24 20:01:51.737832 shindan_cli-1.3.0/shindan_cli/shindan.py
--rw-r--r--   0        0        0     4761 1970-01-01 00:00:00.000000 shindan_cli-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-04-05 22:36:54.712486 shindan_cli-2.0.0/LICENSE
+-rw-r--r--   0        0        0     3795 2024-04-05 22:36:54.712486 shindan_cli-2.0.0/README.md
+-rw-r--r--   0        0        0     1931 2024-04-05 22:36:54.712486 shindan_cli-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0      211 2024-04-05 22:36:54.712486 shindan_cli-2.0.0/shindan_cli/__init__.py
+-rw-r--r--   0        0        0      646 2024-04-05 22:36:54.712486 shindan_cli-2.0.0/shindan_cli/constants.py
+-rw-r--r--   0        0        0     4957 2024-04-05 22:36:54.712486 shindan_cli-2.0.0/shindan_cli/get_results.py
+-rw-r--r--   0        0        0     5326 2024-04-05 22:36:54.712486 shindan_cli-2.0.0/shindan_cli/interactive.py
+-rw-r--r--   0        0        0     2107 2024-04-05 22:36:54.712486 shindan_cli-2.0.0/shindan_cli/main.py
+-rw-r--r--   0        0        0      938 2024-04-05 22:36:54.712486 shindan_cli-2.0.0/shindan_cli/models.py
+-rw-r--r--   0        0        0        0 2024-04-05 22:36:54.712486 shindan_cli-2.0.0/shindan_cli/py.typed
+-rw-r--r--   0        0        0     3277 2024-04-05 22:36:54.712486 shindan_cli-2.0.0/shindan_cli/shindan.py
+-rw-r--r--   0        0        0     4812 1970-01-01 00:00:00.000000 shindan_cli-2.0.0/PKG-INFO
```

### Comparing `shindan_cli-1.3.0/LICENSE` & `shindan_cli-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `shindan_cli-1.3.0/README.md` & `shindan_cli-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `shindan_cli-1.3.0/pyproject.toml` & `shindan_cli-2.0.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,46 +1,14 @@
-# poetry self add poetry-bumpversion
-
 [build-system]
 build-backend = "poetry.core.masonry.api"
 requires = [
   "poetry-core",
 ]
 
 [tool]
-[tool.black]
-line-length = 120
-target-version = ['py39']
-
-[tool.isort]
-profile = "black"
-
-[tool.mypy]
-pretty = true
-python_version = "3.9"
-show_error_codes = true
-strict = true
-
-[tool.ruff]
-ignore = [
-  "D203", # 1 blank line required before class docstring
-  "D213", # Multi-line docstring summary should start at the second line
-]
-line-length = 120
-select = ["ALL"]
-
-[tool.ruff.mccabe]
-max-complexity = 18
-
-[tool.ruff.per-file-ignores]
-"tests/*.py" = [
-  "D",
-  "S101", # Use of assert detected
-]
-
 [tool.poetry]
 authors = ["eggplants <w10776e8w@yahoo.co.jp>"]
 classifiers = [
   "Development Status :: 3 - Alpha",
   "License :: OSI Approved :: MIT License",
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3.7",
@@ -49,39 +17,65 @@
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3 :: Only",
 ]
 description = "ShindanMaker (https://shindanmaker.com) CLI"
 keywords = ["shindanmaker", "cli"]
 license = "MIT"
 name = "shindan_cli"
-packages = [{include = "shindan_cli"}]
+packages = [{ include = "shindan_cli" }]
 readme = "README.md"
 repository = "https://github.com/eggplants/shindan-cli"
-version = "1.3.0"
+version = "0"
 
 [tool.poetry.dependencies]
 beautifulsoup4 = "^4.11.2"
-lxml = "^4.9.2"
+lxml = ">=4.9.2,<6.0.0"
 python = ">=3.7,<4"
 requests = "^2.28.2"
 
 [tool.poetry.group.dev.dependencies]
-lxml-stubs = "^0.4.0"
-mypy = ">=0.991,<1.4"
+lxml-stubs = ">=0.4,<0.6"
+mypy = ">=0.991,<1.5"
 pre-commit = "^2.20.0"
 pytest = "^7.2.2"
 pytest-cov = "^4.0.0"
 taskipy = "^1.10.3"
 types-beautifulsoup4 = "^4.11.6.7"
 types-requests = "^2.28.11.14"
 
 [tool.poetry.scripts]
 shindan = "shindan_cli.main:main"
 
-[tool.poetry_bumpversion.file."shindan_cli/__init__.py"]
+[tool.black]
+target-version = ['py39']
+
+[tool.ruff.lint]
+ignore = [
+  "D203", # 1 blank line required before class docstring
+  "D213", # Multi-line docstring summary should start at the second line
+]
+select = ["ALL"]
+
+[tool.ruff.lint.per-file-ignores]
+"tests/*.py" = [
+  "D",
+  "S101", # Use of assert detected
+]
+
+[tool.isort]
+profile = "black"
+
+[tool.mypy]
+pretty = true
+python_version = "3.9"
+show_error_codes = true
+strict = true
+
+[tool.poetry-version-plugin]
+source = "init"
 
 [tool.taskipy.tasks]
 lint = "pre-commit run -a"
 profile = "python -m cProfile"
 setup = "poetry install && pre-commit install -t pre-commit -t pre-push"
 test = "pytest --cov=shindan_cli --cov-report=term"
 "test:ci" = "task test --cov-report=xml:cov.xml"
```

### Comparing `shindan_cli-1.3.0/PKG-INFO` & `shindan_cli-2.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: shindan-cli
-Version: 1.3.0
+Name: shindan_cli
+Version: 2.0.0
 Summary: ShindanMaker (https://shindanmaker.com) CLI
 Home-page: https://github.com/eggplants/shindan-cli
 License: MIT
 Keywords: shindanmaker,cli
 Author: eggplants
 Author-email: w10776e8w@yahoo.co.jp
 Requires-Python: >=3.7,<4
@@ -12,17 +12,18 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Dist: beautifulsoup4 (>=4.11.2,<5.0.0)
-Requires-Dist: lxml (>=4.9.2,<5.0.0)
+Requires-Dist: lxml (>=4.9.2,<6.0.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Project-URL: Repository, https://github.com/eggplants/shindan-cli
 Description-Content-Type: text/markdown
 
 # shindan-cli
 
 [![Release Package](
```

