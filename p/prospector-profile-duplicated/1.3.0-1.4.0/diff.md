# Comparing `tmp/prospector_profile_duplicated-1.3.0.tar.gz` & `tmp/prospector_profile_duplicated-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prospector_profile_duplicated-1.3.0.tar", max compression
+gzip compressed data, was "prospector_profile_duplicated-1.4.0.tar", max compression
```

## Comparing `prospector_profile_duplicated-1.3.0.tar` & `prospector_profile_duplicated-1.4.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1303 2024-04-03 16:15:07.576513 prospector_profile_duplicated-1.3.0/LICENSE
--rw-r--r--   0        0        0      693 2024-04-03 16:15:07.576513 prospector_profile_duplicated-1.3.0/README.md
--rw-r--r--   0        0        0        0 2024-04-03 16:15:07.576513 prospector_profile_duplicated-1.3.0/prospector_profile_duplicated/__init__.py
--rw-r--r--   0        0        0       55 2024-04-03 16:15:07.576513 prospector_profile_duplicated-1.3.0/prospector_profile_duplicated/autoflake.yaml
--rw-r--r--   0        0        0     1794 2024-04-03 16:15:07.576513 prospector_profile_duplicated-1.3.0/prospector_profile_duplicated/black.yaml
--rw-r--r--   0        0        0      186 2024-04-03 16:15:07.576513 prospector_profile_duplicated-1.3.0/prospector_profile_duplicated/docformatter.yaml
--rw-r--r--   0        0        0      173 2024-04-03 16:15:07.576513 prospector_profile_duplicated-1.3.0/prospector_profile_duplicated/isort.yaml
--rw-r--r--   0        0        0      178 2024-04-03 16:15:07.576513 prospector_profile_duplicated-1.3.0/prospector_profile_duplicated/prospector.yaml
--rw-r--r--   0        0        0      119 2024-04-03 16:15:07.576513 prospector_profile_duplicated-1.3.0/prospector_profile_duplicated/pydocstyle.yaml
--rw-r--r--   0        0        0      917 2024-04-03 16:15:07.576513 prospector_profile_duplicated-1.3.0/prospector_profile_duplicated/pylint.yaml
--rw-r--r--   0        0        0      776 2024-04-03 16:15:07.576513 prospector_profile_duplicated-1.3.0/prospector_profile_duplicated/pyupgrade.yaml
--rw-r--r--   0        0        0     1778 2024-04-03 16:15:55.148842 prospector_profile_duplicated-1.3.0/pyproject.toml
--rw-r--r--   0        0        0     2002 1970-01-01 00:00:00.000000 prospector_profile_duplicated-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1303 2024-04-06 19:04:24.024551 prospector_profile_duplicated-1.4.0/LICENSE
+-rw-r--r--   0        0        0      693 2024-04-06 19:04:24.024551 prospector_profile_duplicated-1.4.0/README.md
+-rw-r--r--   0        0        0        0 2024-04-06 19:04:24.024551 prospector_profile_duplicated-1.4.0/prospector_profile_duplicated/__init__.py
+-rw-r--r--   0        0        0       55 2024-04-06 19:04:24.024551 prospector_profile_duplicated-1.4.0/prospector_profile_duplicated/autoflake.yaml
+-rw-r--r--   0        0        0     1794 2024-04-06 19:04:24.024551 prospector_profile_duplicated-1.4.0/prospector_profile_duplicated/black.yaml
+-rw-r--r--   0        0        0      186 2024-04-06 19:04:24.024551 prospector_profile_duplicated-1.4.0/prospector_profile_duplicated/docformatter.yaml
+-rw-r--r--   0        0        0      173 2024-04-06 19:04:24.024551 prospector_profile_duplicated-1.4.0/prospector_profile_duplicated/isort.yaml
+-rw-r--r--   0        0        0      178 2024-04-06 19:04:24.024551 prospector_profile_duplicated-1.4.0/prospector_profile_duplicated/prospector.yaml
+-rw-r--r--   0        0        0      119 2024-04-06 19:04:24.024551 prospector_profile_duplicated-1.4.0/prospector_profile_duplicated/pydocstyle.yaml
+-rw-r--r--   0        0        0      984 2024-04-06 19:04:24.024551 prospector_profile_duplicated-1.4.0/prospector_profile_duplicated/pylint.yaml
+-rw-r--r--   0        0        0      776 2024-04-06 19:04:24.024551 prospector_profile_duplicated-1.4.0/prospector_profile_duplicated/pyupgrade.yaml
+-rw-r--r--   0        0        0     1778 2024-04-06 19:05:14.496526 prospector_profile_duplicated-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0     2002 1970-01-01 00:00:00.000000 prospector_profile_duplicated-1.4.0/PKG-INFO
```

### Comparing `prospector_profile_duplicated-1.3.0/LICENSE` & `prospector_profile_duplicated-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `prospector_profile_duplicated-1.3.0/README.md` & `prospector_profile_duplicated-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `prospector_profile_duplicated-1.3.0/prospector_profile_duplicated/black.yaml` & `prospector_profile_duplicated-1.4.0/prospector_profile_duplicated/black.yaml`

 * *Files identical despite different names*

### Comparing `prospector_profile_duplicated-1.3.0/prospector_profile_duplicated/pylint.yaml` & `prospector_profile_duplicated-1.4.0/prospector_profile_duplicated/pylint.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -8,14 +8,15 @@
     - D103 # Missing docstring in public function, with: missing-function-docstring
 
 pycodestyle:
   disable:
     - E112 # expected an indented block, with: syntax-error
     - E722 # do not use bare 'except', with: bare-except
     - E901 # IndentationError: unindent does not match any outer indentation level, with: syntax-error
+    - N802 # function name should be lowercase, with: invalid-name
     - N806 # Variable in function should be lowercase, with: invalid-name
 
 pyflakes:
   disable:
     - F401 # unused import, with: unused-import
     - F811 # redefinition of unused, with: redefined-outer-name
     - F841 # local variable is assigned to but never used, with unused-variable
```

### Comparing `prospector_profile_duplicated-1.3.0/prospector_profile_duplicated/pyupgrade.yaml` & `prospector_profile_duplicated-1.4.0/prospector_profile_duplicated/pyupgrade.yaml`

 * *Files identical despite different names*

### Comparing `prospector_profile_duplicated-1.3.0/pyproject.toml` & `prospector_profile_duplicated-1.4.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 strict = true
 
 [tool.pytest.ini_options]
 pytest_plugins = ["pytest_profiling"]
 
 [tool.poetry]
 name = "prospector-profile-duplicated"
-version = "1.3.0"
+version = "1.4.0"
 description = "Profile that can be used to disable the duplicated or conflict rules between Prospector and other tools"
 readme = "README.md"
 authors = ["Stéphane Brunner <stephane.brunner@gmail.com>"]
 homepage = "https://github.com/sbrunner/prospector-profile-duplicated"
 repository = "https://github.com/sbrunner/prospector-profile-duplicated"
 license = "BSD-2-Clause"
 classifiers = [
```

### Comparing `prospector_profile_duplicated-1.3.0/PKG-INFO` & `prospector_profile_duplicated-1.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prospector-profile-duplicated
-Version: 1.3.0
+Version: 1.4.0
 Summary: Profile that can be used to disable the duplicated or conflict rules between Prospector and other tools
 Home-page: https://github.com/sbrunner/prospector-profile-duplicated
 License: BSD-2-Clause
 Author: Stéphane Brunner
 Author-email: stephane.brunner@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

