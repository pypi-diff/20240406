# Comparing `tmp/flasky_cli-0.1.7.tar.gz` & `tmp/flasky_cli-0.1.9.tar.gz`

## Comparing `flasky_cli-0.1.7.tar` & `flasky_cli-0.1.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 flasky_cli-0.1.7/.python-version
--rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 flasky_cli-0.1.7/requirements-dev.lock
--rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 flasky_cli-0.1.7/requirements.lock
--rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 flasky_cli-0.1.7/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 flasky_cli-0.1.7/src/flask_cli/__init__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 flasky_cli-0.1.7/src/flask_cli/__version__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 flasky_cli-0.1.7/src/flask_cli/cli/__init__.py
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 flasky_cli-0.1.7/src/flask_cli/cli/main.py
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 flasky_cli-0.1.7/src/flask_cli/common/__init__.py
--rw-r--r--   0        0        0     5028 2020-02-02 00:00:00.000000 flasky_cli-0.1.7/src/flask_cli/common/cookiemod.py
--rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 flasky_cli-0.1.7/src/flask_cli/common/prompts.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 flasky_cli-0.1.7/src/flask_cli/create/__init__.py
--rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 flasky_cli-0.1.7/src/flask_cli/create/cli.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 flasky_cli-0.1.7/src/flask_cli/templates/__init__.py
--rw-r--r--   0        0        0     3976 2020-02-02 00:00:00.000000 flasky_cli-0.1.7/src/flask_cli/templates/cli.py
--rw-r--r--   0        0        0     2995 2020-02-02 00:00:00.000000 flasky_cli-0.1.7/src/flask_cli/templates/domain.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 flasky_cli-0.1.7/src/flask_cli/templates/data/__init__.py
--rw-r--r--   0        0        0     4819 2020-02-02 00:00:00.000000 flasky_cli-0.1.7/src/flask_cli/templates/data/default.py
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 flasky_cli-0.1.7/.gitignore
--rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 flasky_cli-0.1.7/README.md
--rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 flasky_cli-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     2144 2020-02-02 00:00:00.000000 flasky_cli-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 flasky_cli-0.1.9/.python-version
+-rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 flasky_cli-0.1.9/requirements-dev.lock
+-rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 flasky_cli-0.1.9/requirements.lock
+-rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 flasky_cli-0.1.9/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 flasky_cli-0.1.9/src/flask_cli/__init__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 flasky_cli-0.1.9/src/flask_cli/__version__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 flasky_cli-0.1.9/src/flask_cli/cli/__init__.py
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 flasky_cli-0.1.9/src/flask_cli/cli/main.py
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 flasky_cli-0.1.9/src/flask_cli/common/__init__.py
+-rw-r--r--   0        0        0     5028 2020-02-02 00:00:00.000000 flasky_cli-0.1.9/src/flask_cli/common/cookiemod.py
+-rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 flasky_cli-0.1.9/src/flask_cli/common/prompts.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 flasky_cli-0.1.9/src/flask_cli/create/__init__.py
+-rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 flasky_cli-0.1.9/src/flask_cli/create/cli.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 flasky_cli-0.1.9/src/flask_cli/templates/__init__.py
+-rw-r--r--   0        0        0     3976 2020-02-02 00:00:00.000000 flasky_cli-0.1.9/src/flask_cli/templates/cli.py
+-rw-r--r--   0        0        0     2995 2020-02-02 00:00:00.000000 flasky_cli-0.1.9/src/flask_cli/templates/domain.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 flasky_cli-0.1.9/src/flask_cli/templates/data/__init__.py
+-rw-r--r--   0        0        0     5099 2020-02-02 00:00:00.000000 flasky_cli-0.1.9/src/flask_cli/templates/data/default.py
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 flasky_cli-0.1.9/.gitignore
+-rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 flasky_cli-0.1.9/README.md
+-rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 flasky_cli-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     2200 2020-02-02 00:00:00.000000 flasky_cli-0.1.9/PKG-INFO
```

### Comparing `flasky_cli-0.1.7/requirements-dev.lock` & `flasky_cli-0.1.9/requirements-dev.lock`

 * *Files identical despite different names*

### Comparing `flasky_cli-0.1.7/requirements.lock` & `flasky_cli-0.1.9/requirements.lock`

 * *Files identical despite different names*

### Comparing `flasky_cli-0.1.7/.github/workflows/python-publish.yml` & `flasky_cli-0.1.9/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `flasky_cli-0.1.7/src/flask_cli/common/cookiemod.py` & `flasky_cli-0.1.9/src/flask_cli/common/cookiemod.py`

 * *Files identical despite different names*

### Comparing `flasky_cli-0.1.7/src/flask_cli/common/prompts.py` & `flasky_cli-0.1.9/src/flask_cli/common/prompts.py`

 * *Files identical despite different names*

### Comparing `flasky_cli-0.1.7/src/flask_cli/create/cli.py` & `flasky_cli-0.1.9/src/flask_cli/create/cli.py`

 * *Files identical despite different names*

### Comparing `flasky_cli-0.1.7/src/flask_cli/templates/cli.py` & `flasky_cli-0.1.9/src/flask_cli/templates/cli.py`

 * *Files identical despite different names*

### Comparing `flasky_cli-0.1.7/src/flask_cli/templates/domain.py` & `flasky_cli-0.1.9/src/flask_cli/templates/domain.py`

 * *Files identical despite different names*

### Comparing `flasky_cli-0.1.7/src/flask_cli/templates/data/default.py` & `flasky_cli-0.1.9/src/flask_cli/templates/data/default.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,14 +39,21 @@
             },
             {
                 "id": "cookiecutter-flask-skeleton",
                 "source": "https://github.com/testdrivenio/cookiecutter-flask-skeleton",
                 "description": (
                     "Flask Starter Project"
                 )
+            },
+            {
+                "id": "Flask-API",
+                "source": "https://github.com/jennier0107/Flask-API",
+                "description": (
+                    "Cookiecutter template to create new flask application to build a Web API"
+                )
             }
         ]
     }
 
 
 class JSONTemplatesDataProvider(TemplatesDataProvider):
     """
```

### Comparing `flasky_cli-0.1.7/README.md` & `flasky_cli-0.1.9/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 
 ## Project templates
 
 - [cookiecutter-flask](https://github.com/cookiecutter-flask/cookiecutter-flask)
 - [cookiecutter-flask-minimal](https://github.com/candidtim/cookiecutter-flask-minimal)
 - [cookiecutter-flask-skeleton](https://github.com/testdrivenio/cookiecutter-flask-skeleton)
 - [cookiecutter-Flask-Foundation](https://github.com/JackStouffer/cookiecutter-Flask-Foundation)
+- [Flask-API](https://github.com/jennier0107/Flask-API)
 
 ## Creating a new project
 
 ```bash
 flask-cli create
 ```
```

### Comparing `flasky_cli-0.1.7/pyproject.toml` & `flasky_cli-0.1.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "flasky-cli"
-version = "0.1.7"
+version = "0.1.9"
 description = " CLI to start Flask projects"
 authors = [
     { name = "jennier0107", email = "mt3085570450@outlook.com" }
 ]
 dependencies = [
     "click>=8.1.7",
     "rich-click>=1.7.4",
```

### Comparing `flasky_cli-0.1.7/PKG-INFO` & `flasky_cli-0.1.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: flasky-cli
-Version: 0.1.7
+Version: 0.1.9
 Summary:  CLI to start Flask projects
 Project-URL: Homepage, https://github.com/jennier0107/flasky-cli
 Project-URL: Repository, https://github.com/jennier0107/flasky-cli
 Project-URL: Bug Tracker, https://github.com/jennier0107/flasky-cli/issues
 Author-email: jennier0107 <mt3085570450@outlook.com>
 Requires-Python: >=3.8
 Requires-Dist: click>=8.1.7
@@ -29,14 +29,15 @@
 
 ## Project templates
 
 - [cookiecutter-flask](https://github.com/cookiecutter-flask/cookiecutter-flask)
 - [cookiecutter-flask-minimal](https://github.com/candidtim/cookiecutter-flask-minimal)
 - [cookiecutter-flask-skeleton](https://github.com/testdrivenio/cookiecutter-flask-skeleton)
 - [cookiecutter-Flask-Foundation](https://github.com/JackStouffer/cookiecutter-Flask-Foundation)
+- [Flask-API](https://github.com/jennier0107/Flask-API)
 
 ## Creating a new project
 
 ```bash
 flask-cli create
 ```
```

