# Comparing `tmp/mdpython-0.0.1.tar.gz` & `tmp/mdpython-0.0.2.tar.gz`

## Comparing `mdpython-0.0.1.tar` & `mdpython-0.0.2.tar`

### file list

```diff
@@ -1,5 +1,10 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mdpython-0.0.1/src/mdpython/__init__.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 mdpython-0.0.1/src/mdpython/example.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 mdpython-0.0.1/README.md
--rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 mdpython-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 mdpython-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 mdpython-0.0.2/hello_world.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mdpython-0.0.2/src/mdpython/__init__.py
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 mdpython-0.0.2/src/mdpython/example.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mdpython-0.0.2/src/mdpython/fileutils/__init__.py
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 mdpython-0.0.2/src/mdpython/fileutils/compare.py
+-rw-r--r--   0        0        0     4887 2020-02-02 00:00:00.000000 mdpython-0.0.2/src/mdpython/fileutils/compare_dir.py
+-rw-r--r--   0        0        0     1493 2020-02-02 00:00:00.000000 mdpython-0.0.2/src/mdpython/fileutils/html_template.py
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 mdpython-0.0.2/README.md
+-rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 mdpython-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 mdpython-0.0.2/PKG-INFO
```

### Comparing `mdpython-0.0.1/pyproject.toml` & `mdpython-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "mdpython"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Dhaval", email="seedhaval@gmail.com" },
 ]
 description = "MD Python Library"
 readme = "README.md"
 requires-python = ">=3.0"
 classifiers = [
```

