# Comparing `tmp/xls_updater-0.1.6.tar.gz` & `tmp/xls_updater-0.1.7.tar.gz`

## Comparing `xls_updater-0.1.6.tar` & `xls_updater-0.1.7.tar`

### file list

```diff
@@ -1,30 +1,31 @@
--rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 xls_updater-0.1.6/.pre-commit-config.yaml
--rw-r--r--   0        0        0    21341 2020-02-02 00:00:00.000000 xls_updater-0.1.6/.pylintrc
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 xls_updater-0.1.6/CONTRIBUTING.md
--rw-r--r--   0        0        0     1134 2020-02-02 00:00:00.000000 xls_updater-0.1.6/Makefile
--rw-r--r--   0        0        0     2256 2020-02-02 00:00:00.000000 xls_updater-0.1.6/requirements-dev.txt
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 xls_updater-0.1.6/requirements.txt
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 xls_updater-0.1.6/.github/actions/prepare-environment/action.yaml
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 xls_updater-0.1.6/.github/workflows/black.yml
--rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 xls_updater-0.1.6/.github/workflows/coverage.yml
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 xls_updater-0.1.6/.github/workflows/isort.yml
--rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 xls_updater-0.1.6/.github/workflows/mypy.yml
--rw-r--r--   0        0        0     2038 2020-02-02 00:00:00.000000 xls_updater-0.1.6/.github/workflows/publish.yml
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 xls_updater-0.1.6/.github/workflows/pylint.yml
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 xls_updater-0.1.6/.github/workflows/pytest.yml
--rw-r--r--   0        0        0     2553 2020-02-02 00:00:00.000000 xls_updater-0.1.6/.github/workflows/validation.yaml
--rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 xls_updater-0.1.6/tests/test_app.py
--rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 xls_updater-0.1.6/tests/test_big.py
--rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 xls_updater-0.1.6/tests/test_cli.py
--rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 xls_updater-0.1.6/tests/test_samples.py
--rw-r--r--   0        0        0    30208 2020-02-02 00:00:00.000000 xls_updater-0.1.6/tests/samples/sample1.xls
--rw-r--r--   0        0        0    39424 2020-02-02 00:00:00.000000 xls_updater-0.1.6/tests/samples/sample2.xls
--rw-r--r--   0        0        0    16384 2020-02-02 00:00:00.000000 xls_updater-0.1.6/tests/samples/sample3.xls
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xls_updater-0.1.6/xls_updater/__init__.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 xls_updater-0.1.6/xls_updater/__main__.py
--rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 xls_updater-0.1.6/xls_updater/app.py
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 xls_updater-0.1.6/xls_updater/cli.py
--rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 xls_updater-0.1.6/.gitignore
--rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 xls_updater-0.1.6/README.md
--rw-r--r--   0        0        0     2653 2020-02-02 00:00:00.000000 xls_updater-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     2880 2020-02-02 00:00:00.000000 xls_updater-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 xls_updater-0.1.7/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    21341 2020-02-02 00:00:00.000000 xls_updater-0.1.7/.pylintrc
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 xls_updater-0.1.7/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 xls_updater-0.1.7/Makefile
+-rw-r--r--   0        0        0     1530 2020-02-02 00:00:00.000000 xls_updater-0.1.7/requirements-dev.txt
+-rw-r--r--   0        0        0     1296 2020-02-02 00:00:00.000000 xls_updater-0.1.7/requirements-test.txt
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 xls_updater-0.1.7/requirements.txt
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 xls_updater-0.1.7/.github/actions/prepare-environment/action.yaml
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 xls_updater-0.1.7/.github/workflows/black.yml
+-rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 xls_updater-0.1.7/.github/workflows/coverage.yml
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 xls_updater-0.1.7/.github/workflows/isort.yml
+-rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 xls_updater-0.1.7/.github/workflows/mypy.yml
+-rw-r--r--   0        0        0     2038 2020-02-02 00:00:00.000000 xls_updater-0.1.7/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 xls_updater-0.1.7/.github/workflows/pylint.yml
+-rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 xls_updater-0.1.7/.github/workflows/pytest.yml
+-rw-r--r--   0        0        0     2553 2020-02-02 00:00:00.000000 xls_updater-0.1.7/.github/workflows/validation.yaml
+-rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 xls_updater-0.1.7/tests/test_app.py
+-rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 xls_updater-0.1.7/tests/test_big.py
+-rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 xls_updater-0.1.7/tests/test_cli.py
+-rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 xls_updater-0.1.7/tests/test_samples.py
+-rw-r--r--   0        0        0    30208 2020-02-02 00:00:00.000000 xls_updater-0.1.7/tests/samples/sample1.xls
+-rw-r--r--   0        0        0    39424 2020-02-02 00:00:00.000000 xls_updater-0.1.7/tests/samples/sample2.xls
+-rw-r--r--   0        0        0    16384 2020-02-02 00:00:00.000000 xls_updater-0.1.7/tests/samples/sample3.xls
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xls_updater-0.1.7/xls_updater/__init__.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 xls_updater-0.1.7/xls_updater/__main__.py
+-rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 xls_updater-0.1.7/xls_updater/app.py
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 xls_updater-0.1.7/xls_updater/cli.py
+-rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 xls_updater-0.1.7/.gitignore
+-rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 xls_updater-0.1.7/README.md
+-rw-r--r--   0        0        0     2757 2020-02-02 00:00:00.000000 xls_updater-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     3010 2020-02-02 00:00:00.000000 xls_updater-0.1.7/PKG-INFO
```

### Comparing `xls_updater-0.1.6/.pre-commit-config.yaml` & `xls_updater-0.1.7/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `xls_updater-0.1.6/.pylintrc` & `xls_updater-0.1.7/.pylintrc`

 * *Files identical despite different names*

### Comparing `xls_updater-0.1.6/CONTRIBUTING.md` & `xls_updater-0.1.7/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `xls_updater-0.1.6/Makefile` & `xls_updater-0.1.7/Makefile`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,17 @@
 
 setup:
 	python3 -m pip install .
 
 setup-dev:
 	python3 -m pip install --editable '.[dev]'
 
+setup-test:
+	python3 -m pip install --editable '.[test]'
+
 pip-clean:
 	python3 -m pip uninstall -y -r <(pip freeze)
 
 clean:
 	rm -rf **/__pycache__ .pytest_cache/ dist/ .mypy_cache/ .coverage *.egg-info build
 
 check-black:
@@ -44,14 +47,15 @@
 check-mypy:
 	python3 -m mypy -p xls_updater
 
 compile:
 	python3 -m pip install --upgrade pip-tools
 	python3 -m piptools compile -o requirements.txt pyproject.toml
 	python3 -m piptools compile -o requirements-dev.txt --extra dev pyproject.toml
+	python3 -m piptools compile -o requirements-test.txt --extra test pyproject.toml
 
 build:
 	python3 -m pip install --upgrade build
 	python3 -m build
 
 publish:
 	python3 -m pip install --upgrade twine
```

### Comparing `xls_updater-0.1.6/requirements-dev.txt` & `xls_updater-0.1.7/requirements-dev.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,46 +1,32 @@
 about-time==4.2.1         # via alive-progress
 alive-progress==3.1.5     # via xls-updater (pyproject.toml)
 astroid==3.0.1            # via pylint
 black==23.10.1            # via xls-updater (pyproject.toml)
 cfgv==3.4.0               # via pre-commit
 click==8.1.7              # via black, xls-updater (pyproject.toml)
-coverage==7.3.4           # via pytest-cov
 dill==0.3.7               # via pylint
 distlib==0.3.7            # via virtualenv
 et-xmlfile==1.1.0         # via openpyxl
 filelock==3.12.4          # via virtualenv
 grapheme==0.6.0           # via alive-progress
-humanize==4.9.0           # via xls-updater (pyproject.toml)
 identify==2.5.30          # via pre-commit
-iniconfig==2.0.0          # via pytest
 isort==5.12.0             # via pylint, xls-updater (pyproject.toml)
 mccabe==0.7.0             # via pylint
 mypy==1.8.0               # via xls-updater (pyproject.toml)
 mypy-extensions==1.0.0    # via black, mypy
 nodeenv==1.8.0            # via pre-commit
-numpy==1.26.3             # via pandas, pyarrow
 openpyxl==3.1.2           # via xls-updater (pyproject.toml)
-packaging==23.2           # via black, pytest
-pandas==2.1.4             # via xls-updater (pyproject.toml)
+packaging==23.2           # via black
 pathspec==0.11.2          # via black
 platformdirs==3.11.0      # via black, pylint, virtualenv
-pluggy==1.3.0             # via pytest
 pre-commit==3.5.0         # via xls-updater (pyproject.toml)
-pyarrow==15.0.0           # via xls-updater (pyproject.toml)
 pylint==3.0.2             # via xls-updater (pyproject.toml)
-pytest==7.4.3             # via pytest-cov, pytest-mock, xls-updater (pyproject.toml)
-pytest-cov==4.1.0         # via xls-updater (pyproject.toml)
-pytest-mock==3.12.0       # via xls-updater (pyproject.toml)
-python-dateutil==2.8.2    # via pandas
-pytz==2024.1              # via pandas
 pyyaml==6.0.1             # via pre-commit
-six==1.16.0               # via python-dateutil
+tomli==2.0.1              # via black, mypy, pylint
 tomlkit==0.12.1           # via pylint
-typing-extensions==4.9.0  # via mypy
-tzdata==2023.4            # via pandas
+typing-extensions==4.9.0  # via astroid, black, mypy
 virtualenv==20.24.6       # via pre-commit
 xlrd==2.0.1               # via xls-updater (pyproject.toml)
-xlwt==1.3.0               # via xls-updater (pyproject.toml)
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `xls_updater-0.1.6/.github/workflows/publish.yml` & `xls_updater-0.1.7/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `xls_updater-0.1.6/.github/workflows/validation.yaml` & `xls_updater-0.1.7/.github/workflows/validation.yaml`

 * *Files identical despite different names*

### Comparing `xls_updater-0.1.6/tests/test_app.py` & `xls_updater-0.1.7/tests/test_app.py`

 * *Files identical despite different names*

### Comparing `xls_updater-0.1.6/tests/test_big.py` & `xls_updater-0.1.7/tests/test_big.py`

 * *Files identical despite different names*

### Comparing `xls_updater-0.1.6/tests/test_cli.py` & `xls_updater-0.1.7/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `xls_updater-0.1.6/tests/test_samples.py` & `xls_updater-0.1.7/tests/test_samples.py`

 * *Files identical despite different names*

### Comparing `xls_updater-0.1.6/tests/samples/sample1.xls` & `xls_updater-0.1.7/tests/samples/sample1.xls`

 * *Files identical despite different names*

### Comparing `xls_updater-0.1.6/tests/samples/sample2.xls` & `xls_updater-0.1.7/tests/samples/sample2.xls`

 * *Files identical despite different names*

### Comparing `xls_updater-0.1.6/tests/samples/sample3.xls` & `xls_updater-0.1.7/tests/samples/sample3.xls`

 * *Files identical despite different names*

### Comparing `xls_updater-0.1.6/xls_updater/app.py` & `xls_updater-0.1.7/xls_updater/app.py`

 * *Files identical despite different names*

### Comparing `xls_updater-0.1.6/.gitignore` & `xls_updater-0.1.7/.gitignore`

 * *Files identical despite different names*

### Comparing `xls_updater-0.1.6/README.md` & `xls_updater-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `xls_updater-0.1.6/pyproject.toml` & `xls_updater-0.1.7/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [project]
 name = "xls-updater"
 description = "Convert legacy xls data to newer xlsx format."
 readme = "README.md"
-requires-python = ">=3.11"
+requires-python = ">=3.10"
 dynamic = ["version"]
 keywords = [
     "converter",
     "xls",
     "xlsx",
     "excel",
     "spreadsheet",
@@ -15,15 +15,17 @@
 authors = [
     {name = "Roy Moore", email="roy@moore.co.il"}
 ]
 classifiers = [
     "Development Status :: 4 - Beta",
     "License :: OSI Approved :: MIT License",
     "Natural Language :: English",
+    "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Topic :: Office/Business :: Financial :: Spreadsheet",
     "Topic :: File Formats",
 ]
 dependencies = [
     "click==8.1.7",
     "openpyxl==3.1.2",
     "xlrd==2.0.1",
@@ -31,22 +33,24 @@
 ]
 [project.optional-dependencies]
 dev = [
     "black",
     "isort",
     "pylint",
     "pre-commit",
-    "pytest",
-    "pytest-cov",
-    "pytest_mock",
     "mypy",
+]
+test = [
     "xlwt==1.*",
-    "pandas==2.*",
     "pyarrow==15.*",
-    "humanize"
+    "humanize",
+    "pandas==2.*",
+    "pytest",
+    "pytest-cov",
+    "pytest_mock",
 ]
 
 [project.scripts]
 xls-updater = "xls_updater.cli:cli"
 
 [project.urls]
 homepage = "https://github.com/Tranquility2/xls_updater"
```

### Comparing `xls_updater-0.1.6/PKG-INFO` & `xls_updater-0.1.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,39 +1,42 @@
 Metadata-Version: 2.3
 Name: xls-updater
-Version: 0.1.6
+Version: 0.1.7
 Summary: Convert legacy xls data to newer xlsx format.
 Project-URL: homepage, https://github.com/Tranquility2/xls_updater
 Project-URL: repository, https://github.com/Tranquility2/xls_updater
 Author-email: Roy Moore <roy@moore.co.il>
 Keywords: converter,excel,fileformat,spreadsheet,xls,xlsx
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: File Formats
 Classifier: Topic :: Office/Business :: Financial :: Spreadsheet
-Requires-Python: >=3.11
+Requires-Python: >=3.10
 Requires-Dist: alive-progress==3.1.5
 Requires-Dist: click==8.1.7
 Requires-Dist: openpyxl==3.1.2
 Requires-Dist: xlrd==2.0.1
 Provides-Extra: dev
 Requires-Dist: black; extra == 'dev'
-Requires-Dist: humanize; extra == 'dev'
 Requires-Dist: isort; extra == 'dev'
 Requires-Dist: mypy; extra == 'dev'
-Requires-Dist: pandas==2.*; extra == 'dev'
 Requires-Dist: pre-commit; extra == 'dev'
-Requires-Dist: pyarrow==15.*; extra == 'dev'
 Requires-Dist: pylint; extra == 'dev'
-Requires-Dist: pytest; extra == 'dev'
-Requires-Dist: pytest-cov; extra == 'dev'
-Requires-Dist: pytest-mock; extra == 'dev'
-Requires-Dist: xlwt==1.*; extra == 'dev'
+Provides-Extra: test
+Requires-Dist: humanize; extra == 'test'
+Requires-Dist: pandas==2.*; extra == 'test'
+Requires-Dist: pyarrow==15.*; extra == 'test'
+Requires-Dist: pytest; extra == 'test'
+Requires-Dist: pytest-cov; extra == 'test'
+Requires-Dist: pytest-mock; extra == 'test'
+Requires-Dist: xlwt==1.*; extra == 'test'
 Description-Content-Type: text/markdown
 
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/) [![linting: pylint](https://img.shields.io/badge/linting-pylint-yellowgreen)](https://github.com/pylint-dev/pylint) [![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)
 
 [![PyPI - Version](https://img.shields.io/pypi/v/xls-updater.svg?logo=pypi&label=PyPI&logoColor=gold)](https://pypi.org/project/xls-updater/) [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/xls-updater.svg?logo=python&label=Python&logoColor=gold)](https://pypi.org/project/xls-updater/) [![Coverage Status](https://coveralls.io/repos/github/Tranquility2/xls_updater/badge.svg?branch=master)](https://coveralls.io/github/Tranquility2/xls_updater?branch=master)
 
 # xls_updater
```

