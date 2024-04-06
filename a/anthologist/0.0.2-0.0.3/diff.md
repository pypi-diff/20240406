# Comparing `tmp/anthologist-0.0.2.tar.gz` & `tmp/anthologist-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anthologist-0.0.2.tar", max compression
+gzip compressed data, was "anthologist-0.0.3.tar", max compression
```

## Comparing `anthologist-0.0.2.tar` & `anthologist-0.0.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2024-03-24 19:54:14.250723 anthologist-0.0.2/anthologist/__init__.py
--rw-r--r--   0        0        0      547 2024-03-24 19:54:14.279716 anthologist-0.0.2/anthologist/helpers.py
--rw-r--r--   0        0        0     5405 2024-03-24 19:54:14.281713 anthologist-0.0.2/anthologist/main.py
--rw-r--r--   0        0        0      641 2024-03-24 20:06:36.828065 anthologist-0.0.2/pyproject.toml
--rw-r--r--   0        0        0       93 2024-03-24 19:56:17.668990 anthologist-0.0.2/README.md
--rw-r--r--   0        0        0      758 1970-01-01 00:00:00.000000 anthologist-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-03-24 19:54:14.250723 anthologist-0.0.3/anthologist/__init__.py
+-rw-r--r--   0        0        0      547 2024-03-24 19:54:14.279716 anthologist-0.0.3/anthologist/helpers.py
+-rw-r--r--   0        0        0     5362 2024-03-24 20:36:51.926072 anthologist-0.0.3/anthologist/main.py
+-rw-r--r--   0        0        0      704 2024-04-06 20:43:54.191427 anthologist-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0       93 2024-03-24 19:56:17.668990 anthologist-0.0.3/README.md
+-rw-r--r--   0        0        0      758 1970-01-01 00:00:00.000000 anthologist-0.0.3/PKG-INFO
```

### Comparing `anthologist-0.0.2/anthologist/helpers.py` & `anthologist-0.0.3/anthologist/helpers.py`

 * *Files identical despite different names*

### Comparing `anthologist-0.0.2/anthologist/main.py` & `anthologist-0.0.3/anthologist/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -182,11 +182,7 @@
         projects, label="Locking dependencies", length=len(projects)
     ) as bar:
         for project in bar:
             click.secho(
                 f"\nAnthologist locking dependencies for {project}:", fg="magenta"
             )
             subprocess.run(["poetry", "lock"], cwd=project, shell=True)
-
-
-if __name__ == "__main__":
-    cli()
```

### Comparing `anthologist-0.0.2/pyproject.toml` & `anthologist-0.0.3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "anthologist"
-version = "0.0.2"
+version = "0.0.3"
 description = "A CLI for managing multiple Poetry-managed Python projects simultaneously"
 authors = ["James Harrison <40500443+jharibo@users.noreply.github.com>"]
 readme = "README.md"
 homepage = "https://github.com/jharibo/anthologist"
 repository = "https://github.com/jharibo/anthologist"
 keywords = ["poetry", "packaging"]
 
@@ -17,7 +17,10 @@
 mypy = "^1.9.0"
 pre-commit = "^3.6.2"
 ruff = "^0.3.4"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
+
+[tool.poetry.scripts]
+anthologist = "anthologist.main:cli"
```

### Comparing `anthologist-0.0.2/PKG-INFO` & `anthologist-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anthologist
-Version: 0.0.2
+Version: 0.0.3
 Summary: A CLI for managing multiple Poetry-managed Python projects simultaneously
 Home-page: https://github.com/jharibo/anthologist
 Keywords: poetry,packaging
 Author: James Harrison
 Author-email: 40500443+jharibo@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
```

