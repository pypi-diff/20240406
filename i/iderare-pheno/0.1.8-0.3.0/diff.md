# Comparing `tmp/iderare-pheno-0.1.8.tar.gz` & `tmp/iderare-pheno-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iderare-pheno-0.1.8.tar", last modified: Sat Apr  6 11:14:19 2024, max compression
+gzip compressed data, was "iderare-pheno-0.3.0.tar", last modified: Sat Apr  6 17:24:54 2024, max compression
```

## Comparing `iderare-pheno-0.1.8.tar` & `iderare-pheno-0.3.0.tar`

### file list

```diff
@@ -1,16 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:14:19.276228 iderare-pheno-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-04-06 11:14:06.000000 iderare-pheno-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7238 2024-04-06 11:14:19.276228 iderare-pheno-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3919 2024-04-06 11:14:06.000000 iderare-pheno-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:14:19.272228 iderare-pheno-0.1.8/iderare_pheno/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-06 11:14:06.000000 iderare-pheno-0.1.8/iderare_pheno/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 11:14:06.000000 iderare-pheno-0.1.8/iderare_pheno/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-06 11:14:06.000000 iderare-pheno-0.1.8/iderare_pheno/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:14:19.272228 iderare-pheno-0.1.8/iderare_pheno.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7238 2024-04-06 11:14:19.000000 iderare-pheno-0.1.8/iderare_pheno.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-06 11:14:19.000000 iderare-pheno-0.1.8/iderare_pheno.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 11:14:19.000000 iderare-pheno-0.1.8/iderare_pheno.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-06 11:14:19.000000 iderare-pheno-0.1.8/iderare_pheno.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-06 11:14:19.000000 iderare-pheno-0.1.8/iderare_pheno.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2632 2024-04-06 11:14:06.000000 iderare-pheno-0.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 11:14:19.276228 iderare-pheno-0.1.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:24:54.244353 iderare-pheno-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-04-06 17:24:01.000000 iderare-pheno-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7444 2024-04-06 17:24:54.244353 iderare-pheno-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3919 2024-04-06 17:24:01.000000 iderare-pheno-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:24:54.240353 iderare-pheno-0.3.0/iderare_pheno/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-06 17:24:01.000000 iderare-pheno-0.3.0/iderare_pheno/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11107 2024-04-06 17:24:01.000000 iderare-pheno-0.3.0/iderare_pheno/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 17:24:01.000000 iderare-pheno-0.3.0/iderare_pheno/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     6540 2024-04-06 17:24:01.000000 iderare-pheno-0.3.0/iderare_pheno/simrec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2016 2024-04-06 17:24:01.000000 iderare-pheno-0.3.0/iderare_pheno/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-06 17:24:01.000000 iderare-pheno-0.3.0/iderare_pheno/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:24:54.240353 iderare-pheno-0.3.0/iderare_pheno.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7444 2024-04-06 17:24:54.000000 iderare-pheno-0.3.0/iderare_pheno.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-06 17:24:54.000000 iderare-pheno-0.3.0/iderare_pheno.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 17:24:54.000000 iderare-pheno-0.3.0/iderare_pheno.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-06 17:24:54.000000 iderare-pheno-0.3.0/iderare_pheno.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-06 17:24:54.000000 iderare-pheno-0.3.0/iderare_pheno.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2764 2024-04-06 17:24:01.000000 iderare-pheno-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 17:24:54.244353 iderare-pheno-0.3.0/setup.cfg
```

### Comparing `iderare-pheno-0.1.8/LICENSE` & `iderare-pheno-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `iderare-pheno-0.1.8/PKG-INFO` & `iderare-pheno-0.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iderare-pheno
-Version: 0.1.8
+Version: 0.3.0
 Author-email: Ivan William Harsono <contact@ivanwilliammd.org>
 License: BSD 3-Clause License
         
         Copyright (c) 2024, Ivan William Harsono
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
@@ -38,18 +38,26 @@
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: pandas
+Requires-Dist: numpy
+Requires-Dist: matplotlib
+Requires-Dist: scipy
+Requires-Dist: hpo3
+Requires-Dist: scikit-learn
+Requires-Dist: pyyaml
 Provides-Extra: dev
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: mypy<1.10,>=1.0; extra == "dev"
 Requires-Dist: black<25.0,>=23.0; extra == "dev"
+Requires-Dist: black[jupyter]; extra == "dev"
 Requires-Dist: isort<5.14,>=5.12; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-sphinx; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: twine>=1.11.0; extra == "dev"
 Requires-Dist: build; extra == "dev"
 Requires-Dist: setuptools; extra == "dev"
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: iderare-pheno Version: 0.1.8 Author-email: Ivan
+Metadata-Version: 2.1 Name: iderare-pheno Version: 0.3.0 Author-email: Ivan
 William Harsono
 ivanwilliammd.org> License: BSD 3-Clause License Copyright (c) 2024, Ivan
 William Harsono Redistribution and use in source and binary forms, with or
 without modification, are permitted provided that the following conditions are
 met: 1. Redistributions of source code must retain the above copyright notice,
 this list of conditions and the following disclaimer. 2. Redistributions in
 binary form must reproduce the above copyright notice, this list of conditions
@@ -23,17 +23,20 @@
 URL: Homepage, https://github.com/ivanwilliammd/iderare-pheno Project-URL:
 Repository, https://github.com/ivanwilliammd/iderare-pheno Project-URL:
 Changelog, https://github.com/ivanwilliammd/iderare-pheno/blob/main/
 CHANGELOG.md Classifier: Intended Audience :: Science/Research Classifier:
 Development Status :: 3 - Alpha Classifier: License :: OSI Approved :: Apache
 Software License Classifier: Programming Language :: Python :: 3 Classifier:
 Topic :: Scientific/Engineering :: Artificial Intelligence Requires-Python:
->=3.8 Description-Content-Type: text/markdown License-File: LICENSE Provides-
-Extra: dev Requires-Dist: ruff; extra == "dev" Requires-Dist: mypy<1.10,>=1.0;
-extra == "dev" Requires-Dist: black<25.0,>=23.0; extra == "dev" Requires-Dist:
+>=3.8 Description-Content-Type: text/markdown License-File: LICENSE Requires-
+Dist: pandas Requires-Dist: numpy Requires-Dist: matplotlib Requires-Dist:
+scipy Requires-Dist: hpo3 Requires-Dist: scikit-learn Requires-Dist: pyyaml
+Provides-Extra: dev Requires-Dist: ruff; extra == "dev" Requires-Dist:
+mypy<1.10,>=1.0; extra == "dev" Requires-Dist: black<25.0,>=23.0; extra ==
+"dev" Requires-Dist: black[jupyter]; extra == "dev" Requires-Dist:
 isort<5.14,>=5.12; extra == "dev" Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-sphinx; extra == "dev" Requires-Dist: pytest-cov; extra
 == "dev" Requires-Dist: twine>=1.11.0; extra == "dev" Requires-Dist: build;
 extra == "dev" Requires-Dist: setuptools; extra == "dev" Requires-Dist: wheel;
 extra == "dev" Requires-Dist: Sphinx<7.3.0,>=4.3.0; extra == "dev" Requires-
 Dist: furo==2024.1.29; extra == "dev" Requires-Dist: myst-parser<2.1,>=1.0;
 extra == "dev" Requires-Dist: sphinx-copybutton==0.5.2; extra == "dev"
```

### Comparing `iderare-pheno-0.1.8/README.md` & `iderare-pheno-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `iderare-pheno-0.1.8/iderare_pheno.egg-info/PKG-INFO` & `iderare-pheno-0.3.0/iderare_pheno.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iderare-pheno
-Version: 0.1.8
+Version: 0.3.0
 Author-email: Ivan William Harsono <contact@ivanwilliammd.org>
 License: BSD 3-Clause License
         
         Copyright (c) 2024, Ivan William Harsono
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
@@ -38,18 +38,26 @@
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: pandas
+Requires-Dist: numpy
+Requires-Dist: matplotlib
+Requires-Dist: scipy
+Requires-Dist: hpo3
+Requires-Dist: scikit-learn
+Requires-Dist: pyyaml
 Provides-Extra: dev
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: mypy<1.10,>=1.0; extra == "dev"
 Requires-Dist: black<25.0,>=23.0; extra == "dev"
+Requires-Dist: black[jupyter]; extra == "dev"
 Requires-Dist: isort<5.14,>=5.12; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-sphinx; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: twine>=1.11.0; extra == "dev"
 Requires-Dist: build; extra == "dev"
 Requires-Dist: setuptools; extra == "dev"
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: iderare-pheno Version: 0.1.8 Author-email: Ivan
+Metadata-Version: 2.1 Name: iderare-pheno Version: 0.3.0 Author-email: Ivan
 William Harsono
 ivanwilliammd.org> License: BSD 3-Clause License Copyright (c) 2024, Ivan
 William Harsono Redistribution and use in source and binary forms, with or
 without modification, are permitted provided that the following conditions are
 met: 1. Redistributions of source code must retain the above copyright notice,
 this list of conditions and the following disclaimer. 2. Redistributions in
 binary form must reproduce the above copyright notice, this list of conditions
@@ -23,17 +23,20 @@
 URL: Homepage, https://github.com/ivanwilliammd/iderare-pheno Project-URL:
 Repository, https://github.com/ivanwilliammd/iderare-pheno Project-URL:
 Changelog, https://github.com/ivanwilliammd/iderare-pheno/blob/main/
 CHANGELOG.md Classifier: Intended Audience :: Science/Research Classifier:
 Development Status :: 3 - Alpha Classifier: License :: OSI Approved :: Apache
 Software License Classifier: Programming Language :: Python :: 3 Classifier:
 Topic :: Scientific/Engineering :: Artificial Intelligence Requires-Python:
->=3.8 Description-Content-Type: text/markdown License-File: LICENSE Provides-
-Extra: dev Requires-Dist: ruff; extra == "dev" Requires-Dist: mypy<1.10,>=1.0;
-extra == "dev" Requires-Dist: black<25.0,>=23.0; extra == "dev" Requires-Dist:
+>=3.8 Description-Content-Type: text/markdown License-File: LICENSE Requires-
+Dist: pandas Requires-Dist: numpy Requires-Dist: matplotlib Requires-Dist:
+scipy Requires-Dist: hpo3 Requires-Dist: scikit-learn Requires-Dist: pyyaml
+Provides-Extra: dev Requires-Dist: ruff; extra == "dev" Requires-Dist:
+mypy<1.10,>=1.0; extra == "dev" Requires-Dist: black<25.0,>=23.0; extra ==
+"dev" Requires-Dist: black[jupyter]; extra == "dev" Requires-Dist:
 isort<5.14,>=5.12; extra == "dev" Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-sphinx; extra == "dev" Requires-Dist: pytest-cov; extra
 == "dev" Requires-Dist: twine>=1.11.0; extra == "dev" Requires-Dist: build;
 extra == "dev" Requires-Dist: setuptools; extra == "dev" Requires-Dist: wheel;
 extra == "dev" Requires-Dist: Sphinx<7.3.0,>=4.3.0; extra == "dev" Requires-
 Dist: furo==2024.1.29; extra == "dev" Requires-Dist: myst-parser<2.1,>=1.0;
 extra == "dev" Requires-Dist: sphinx-copybutton==0.5.2; extra == "dev"
```

### Comparing `iderare-pheno-0.1.8/pyproject.toml` & `iderare-pheno-0.3.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -15,29 +15,36 @@
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
 ]
 authors = [
     {name = "Ivan William Harsono", email = "contact@ivanwilliammd.org"}
 ]
 requires-python = ">=3.8"
 dependencies = [
-  # Add your own dependencies here
+  "pandas",
+  "numpy",
+  "matplotlib",
+  "scipy",
+  "hpo3",
+  "scikit-learn",
+  "pyyaml"
 ]
 license = {file = "LICENSE"}
 
 [project.urls]
 Homepage = "https://github.com/ivanwilliammd/iderare-pheno"
 Repository = "https://github.com/ivanwilliammd/iderare-pheno"
 Changelog = "https://github.com/ivanwilliammd/iderare-pheno/blob/main/CHANGELOG.md"
 # Documentation = "https://iderare-pheno.readthedocs.io/"
 
 [project.optional-dependencies]
 dev = [
     "ruff",
     "mypy>=1.0,<1.10",
     "black>=23.0,<25.0",
+    "black[jupyter]",
     "isort>=5.12,<5.14",
     "pytest",
     "pytest-sphinx",
     "pytest-cov",
     "twine>=1.11.0",
     "build",
     "setuptools",
@@ -56,14 +63,15 @@
     "*.tests",
     "*.tests.*",
     "tests.*",
     "tests",
     "docs*",
     "scripts*"
 ]
+include = ["iderare_pheno", "phenotype", "phenotype.*"]
 
 [tool.setuptools]
 include-package-data = true
 
 [tool.setuptools.package-data]
 iderare_pheno = ["py.typed"]
```

