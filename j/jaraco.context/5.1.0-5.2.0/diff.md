# Comparing `tmp/jaraco.context-5.1.0.tar.gz` & `tmp/jaraco.context-5.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaraco.context-5.1.0.tar", last modified: Thu Apr  4 23:20:45 2024, max compression
+gzip compressed data, was "jaraco.context-5.2.0.tar", last modified: Sat Apr  6 14:48:41 2024, max compression
```

## Comparing `jaraco.context-5.1.0.tar` & `jaraco.context-5.2.0.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:20:45.660750 jaraco.context-5.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-04 23:20:29.000000 jaraco.context-5.1.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-04 23:20:29.000000 jaraco.context-5.1.0/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:20:45.656750 jaraco.context-5.1.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-04 23:20:29.000000 jaraco.context-5.1.0/.github/FUNDING.yml
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-04 23:20:29.000000 jaraco.context-5.1.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:20:45.656750 jaraco.context-5.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-04-04 23:20:29.000000 jaraco.context-5.1.0/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-04 23:20:29.000000 jaraco.context-5.1.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-04 23:20:29.000000 jaraco.context-5.1.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-04-04 23:20:29.000000 jaraco.context-5.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-04-04 23:20:29.000000 jaraco.context-5.1.0/NEWS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3897 2024-04-04 23:20:45.660750 jaraco.context-5.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-04-04 23:20:29.000000 jaraco.context-5.1.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-04 23:20:29.000000 jaraco.context-5.1.0/SECURITY.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:20:45.656750 jaraco.context-5.1.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-04-04 23:20:29.000000 jaraco.context-5.1.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-04 23:20:29.000000 jaraco.context-5.1.0/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-04-04 23:20:29.000000 jaraco.context-5.1.0/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:20:45.656750 jaraco.context-5.1.0/jaraco/
--rw-r--r--   0 runner    (1001) docker     (127)     8927 2024-04-04 23:20:29.000000 jaraco.context-5.1.0/jaraco/context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:20:45.660750 jaraco.context-5.1.0/jaraco.context.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3897 2024-04-04 23:20:45.000000 jaraco.context-5.1.0/jaraco.context.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      507 2024-04-04 23:20:45.000000 jaraco.context-5.1.0/jaraco.context.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 23:20:45.000000 jaraco.context-5.1.0/jaraco.context.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-04 23:20:45.000000 jaraco.context-5.1.0/jaraco.context.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-04 23:20:45.000000 jaraco.context-5.1.0/jaraco.context.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-04 23:20:29.000000 jaraco.context-5.1.0/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-04 23:20:29.000000 jaraco.context-5.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      659 2024-04-04 23:20:29.000000 jaraco.context-5.1.0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-04 23:20:29.000000 jaraco.context-5.1.0/ruff.toml
--rw-r--r--   0 runner    (1001) docker     (127)      854 2024-04-04 23:20:45.660750 jaraco.context-5.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-04 23:20:29.000000 jaraco.context-5.1.0/towncrier.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-04-04 23:20:29.000000 jaraco.context-5.1.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:48:41.841425 jaraco.context-5.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-06 14:48:27.000000 jaraco.context-5.2.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-06 14:48:27.000000 jaraco.context-5.2.0/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:48:41.837425 jaraco.context-5.2.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-06 14:48:27.000000 jaraco.context-5.2.0/.github/FUNDING.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-06 14:48:27.000000 jaraco.context-5.2.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:48:41.837425 jaraco.context-5.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-04-06 14:48:27.000000 jaraco.context-5.2.0/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-06 14:48:27.000000 jaraco.context-5.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-06 14:48:27.000000 jaraco.context-5.2.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-04-06 14:48:27.000000 jaraco.context-5.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-04-06 14:48:27.000000 jaraco.context-5.2.0/NEWS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3998 2024-04-06 14:48:41.841425 jaraco.context-5.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-04-06 14:48:27.000000 jaraco.context-5.2.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-06 14:48:27.000000 jaraco.context-5.2.0/SECURITY.md
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-04-06 14:48:27.000000 jaraco.context-5.2.0/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:48:41.837425 jaraco.context-5.2.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-04-06 14:48:27.000000 jaraco.context-5.2.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-06 14:48:27.000000 jaraco.context-5.2.0/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-04-06 14:48:27.000000 jaraco.context-5.2.0/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:48:41.837425 jaraco.context-5.2.0/jaraco/
+-rw-r--r--   0 runner    (1001) docker     (127)     9381 2024-04-06 14:48:27.000000 jaraco.context-5.2.0/jaraco/context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:48:41.837425 jaraco.context-5.2.0/jaraco.context.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3998 2024-04-06 14:48:41.000000 jaraco.context-5.2.0/jaraco.context.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-06 14:48:41.000000 jaraco.context-5.2.0/jaraco.context.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 14:48:41.000000 jaraco.context-5.2.0/jaraco.context.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-06 14:48:41.000000 jaraco.context-5.2.0/jaraco.context.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-06 14:48:41.000000 jaraco.context-5.2.0/jaraco.context.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-06 14:48:27.000000 jaraco.context-5.2.0/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-06 14:48:27.000000 jaraco.context-5.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-04-06 14:48:27.000000 jaraco.context-5.2.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-06 14:48:27.000000 jaraco.context-5.2.0/ruff.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      909 2024-04-06 14:48:41.841425 jaraco.context-5.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-06 14:48:27.000000 jaraco.context-5.2.0/towncrier.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-04-06 14:48:27.000000 jaraco.context-5.2.0/tox.ini
```

### Comparing `jaraco.context-5.1.0/.github/workflows/main.yml` & `jaraco.context-5.2.0/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `jaraco.context-5.1.0/LICENSE` & `jaraco.context-5.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jaraco.context-5.1.0/NEWS.rst` & `jaraco.context-5.2.0/NEWS.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+v5.2.0
+======
+
+Features
+--------
+
+- Implemented tarfile using native functionality and avoiding subprocessing, making it portable. (#5)
+
+
 v5.1.0
 ======
 
 Features
 --------
 
 - Implement experimental _compose for composing context managers. If you wish to use this function, please comment in the issue regarding your thoughts on the ordering. (#6)
```

### Comparing `jaraco.context-5.1.0/PKG-INFO` & `jaraco.context-5.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 Metadata-Version: 2.1
 Name: jaraco.context
-Version: 5.1.0
+Version: 5.2.0
 Summary: Useful decorators and context managers
 Home-page: https://github.com/jaraco/jaraco.context
 Author: Jason R. Coombs
 Author-email: jaraco@jaraco.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.8
 License-File: LICENSE
+Requires-Dist: backports.tarfile; python_version < "3.12"
 Provides-Extra: testing
 Requires-Dist: pytest!=8.1.1,>=6; extra == "testing"
 Requires-Dist: pytest-checkdocs>=2.4; extra == "testing"
 Requires-Dist: pytest-cov; extra == "testing"
 Requires-Dist: pytest-mypy; extra == "testing"
 Requires-Dist: pytest-enabler>=2.2; extra == "testing"
 Requires-Dist: pytest-ruff>=0.2.1; extra == "testing"
+Requires-Dist: portend; extra == "testing"
 Provides-Extra: docs
 Requires-Dist: sphinx>=3.5; extra == "docs"
 Requires-Dist: jaraco.packaging>=9.3; extra == "docs"
 Requires-Dist: rst.linker>=1.9; extra == "docs"
 Requires-Dist: furo; extra == "docs"
 Requires-Dist: sphinx-lint; extra == "docs"
 Requires-Dist: jaraco.tidelift>=1.4; extra == "docs"
```

### Comparing `jaraco.context-5.1.0/README.rst` & `jaraco.context-5.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `jaraco.context-5.1.0/docs/conf.py` & `jaraco.context-5.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `jaraco.context-5.1.0/jaraco/context.py` & `jaraco.context-5.2.0/jaraco/context.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,19 +2,27 @@
 
 import contextlib
 import functools
 import operator
 import os
 import shutil
 import subprocess
+import sys
 import tempfile
+import urllib.request
 import warnings
 from typing import Iterator
 
 
+if sys.version_info < (3, 12):
+    from backports import tarfile
+else:
+    import tarfile
+
+
 @contextlib.contextmanager
 def pushd(dir: str | os.PathLike) -> Iterator[str | os.PathLike]:
     """
     >>> tmp_path = getfixture('tmp_path')
     >>> with pushd(tmp_path):
     ...     assert os.getcwd() == os.fspath(tmp_path)
     >>> assert os.getcwd() != os.fspath(tmp_path)
@@ -30,31 +38,46 @@
 
 @contextlib.contextmanager
 def tarball(
     url, target_dir: str | os.PathLike | None = None
 ) -> Iterator[str | os.PathLike]:
     """
     Get a tarball, extract it, yield, then clean up.
+
+    >>> import urllib.request
+    >>> url = getfixture('tarfile_served')
+    >>> target = getfixture('tmp_path') / 'out'
+    >>> tb = tarball(url, target_dir=target)
+    >>> import pathlib
+    >>> with tb as extracted:
+    ...     contents = pathlib.Path(extracted, 'contents.txt').read_text()
+    >>> assert not os.path.exists(extracted)
     """
     if target_dir is None:
         target_dir = os.path.basename(url).replace('.tar.gz', '').replace('.tgz', '')
-    runner = functools.partial(subprocess.check_call, shell=True)
     # In the tar command, use --strip-components=1 to strip the first path and
     #  then
     #  use -C to cause the files to be extracted to {target_dir}. This ensures
     #  that we always know where the files were extracted.
-    runner('mkdir {target_dir}'.format(**vars()))
+    os.mkdir(target_dir)
     try:
-        getter = 'wget {url} -O -'
-        extract = 'tar x{compression} --strip-components=1 -C {target_dir}'
-        cmd = ' | '.join((getter, extract))
-        runner(cmd.format(compression=infer_compression(url), **vars()))
+        req = urllib.request.urlopen(url)
+        with tarfile.open(fileobj=req, mode='r|gz') as tf:
+            tf.extractall(path=target_dir, filter=strip_first_component)
         yield target_dir
     finally:
-        runner('rm -Rf {target_dir}'.format(**vars()))
+        shutil.rmtree(target_dir)
+
+
+def strip_first_component(
+    member: tarfile.TarInfo,
+    path,
+) -> tarfile.TarInfo:
+    _, member.name = member.name.split('/', 1)
+    return member
 
 
 def _compose(*cmgrs):
     """
     Compose any number of dependent context managers into a single one.
 
     The last, innermost context manager may take arbitrary arguments, but
```

### Comparing `jaraco.context-5.1.0/jaraco.context.egg-info/PKG-INFO` & `jaraco.context-5.2.0/jaraco.context.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 Metadata-Version: 2.1
 Name: jaraco.context
-Version: 5.1.0
+Version: 5.2.0
 Summary: Useful decorators and context managers
 Home-page: https://github.com/jaraco/jaraco.context
 Author: Jason R. Coombs
 Author-email: jaraco@jaraco.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.8
 License-File: LICENSE
+Requires-Dist: backports.tarfile; python_version < "3.12"
 Provides-Extra: testing
 Requires-Dist: pytest!=8.1.1,>=6; extra == "testing"
 Requires-Dist: pytest-checkdocs>=2.4; extra == "testing"
 Requires-Dist: pytest-cov; extra == "testing"
 Requires-Dist: pytest-mypy; extra == "testing"
 Requires-Dist: pytest-enabler>=2.2; extra == "testing"
 Requires-Dist: pytest-ruff>=0.2.1; extra == "testing"
+Requires-Dist: portend; extra == "testing"
 Provides-Extra: docs
 Requires-Dist: sphinx>=3.5; extra == "docs"
 Requires-Dist: jaraco.packaging>=9.3; extra == "docs"
 Requires-Dist: rst.linker>=1.9; extra == "docs"
 Requires-Dist: furo; extra == "docs"
 Requires-Dist: sphinx-lint; extra == "docs"
 Requires-Dist: jaraco.tidelift>=1.4; extra == "docs"
```

### Comparing `jaraco.context-5.1.0/pytest.ini` & `jaraco.context-5.2.0/pytest.ini`

 * *Files identical despite different names*

### Comparing `jaraco.context-5.1.0/setup.cfg` & `jaraco.context-5.2.0/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -12,23 +12,26 @@
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
 
 [options]
 include_package_data = true
 python_requires = >=3.8
 install_requires = 
+	backports.tarfile; python_version < "3.12"
 
 [options.extras_require]
 testing = 
 	pytest >= 6, != 8.1.1
 	pytest-checkdocs >= 2.4
 	pytest-cov
 	pytest-mypy
 	pytest-enabler >= 2.2
 	pytest-ruff >= 0.2.1
+	
+	portend
 docs = 
 	sphinx >= 3.5
 	jaraco.packaging >= 9.3
 	rst.linker >= 1.9
 	furo
 	sphinx-lint
```

### Comparing `jaraco.context-5.1.0/tox.ini` & `jaraco.context-5.2.0/tox.ini`

 * *Files identical despite different names*

