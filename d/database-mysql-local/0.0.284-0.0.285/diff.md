# Comparing `tmp/database-mysql-local-0.0.284.tar.gz` & `tmp/database-mysql-local-0.0.285.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "database-mysql-local-0.0.284.tar", last modified: Thu Apr  4 20:00:35 2024, max compression
+gzip compressed data, was "database-mysql-local-0.0.285.tar", last modified: Sat Apr  6 17:18:19 2024, max compression
```

## Comparing `database-mysql-local-0.0.284.tar` & `database-mysql-local-0.0.285.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:00:35.802778 database-mysql-local-0.0.284/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 19:59:35.000000 database-mysql-local-0.0.284/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-04 20:00:35.802778 database-mysql-local-0.0.284/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3519 2024-04-04 19:59:35.000000 database-mysql-local-0.0.284/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:00:35.794778 database-mysql-local-0.0.284/database_mysql_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:00:35.798778 database-mysql-local-0.0.284/database_mysql_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 19:59:35.000000 database-mysql-local-0.0.284/database_mysql_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4686 2024-04-04 19:59:35.000000 database-mysql-local-0.0.284/database_mysql_local/src/connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     2895 2024-04-04 19:59:35.000000 database-mysql-local-0.0.284/database_mysql_local/src/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-04-04 19:59:35.000000 database-mysql-local-0.0.284/database_mysql_local/src/cursor.py
--rw-r--r--   0 runner    (1001) docker     (127)    38968 2024-04-04 19:59:35.000000 database-mysql-local-0.0.284/database_mysql_local/src/generic_crud.py
--rw-r--r--   0 runner    (1001) docker     (127)    31706 2024-04-04 19:59:35.000000 database-mysql-local-0.0.284/database_mysql_local/src/generic_crud_ml.py
--rw-r--r--   0 runner    (1001) docker     (127)     6406 2024-04-04 19:59:35.000000 database-mysql-local-0.0.284/database_mysql_local/src/generic_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-04 19:59:35.000000 database-mysql-local-0.0.284/database_mysql_local/src/point.py
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-04-04 19:59:35.000000 database-mysql-local-0.0.284/database_mysql_local/src/polygon.py
--rw-r--r--   0 runner    (1001) docker     (127)   595483 2024-04-04 20:00:01.000000 database-mysql-local-0.0.284/database_mysql_local/src/table_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-04-04 19:59:35.000000 database-mysql-local-0.0.284/database_mysql_local/src/to_sql_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-04-04 19:59:35.000000 database-mysql-local-0.0.284/database_mysql_local/src/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:00:35.802778 database-mysql-local-0.0.284/database_mysql_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-04 20:00:35.000000 database-mysql-local-0.0.284/database_mysql_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-04 20:00:35.000000 database-mysql-local-0.0.284/database_mysql_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 20:00:35.000000 database-mysql-local-0.0.284/database_mysql_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-04 20:00:35.000000 database-mysql-local-0.0.284/database_mysql_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-04 20:00:35.000000 database-mysql-local-0.0.284/database_mysql_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-04 19:59:35.000000 database-mysql-local-0.0.284/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 20:00:35.802778 database-mysql-local-0.0.284/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-04-04 19:59:35.000000 database-mysql-local-0.0.284/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:18:19.019203 database-mysql-local-0.0.285/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 17:17:18.000000 database-mysql-local-0.0.285/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-06 17:18:19.019203 database-mysql-local-0.0.285/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3519 2024-04-06 17:17:18.000000 database-mysql-local-0.0.285/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:18:19.011203 database-mysql-local-0.0.285/database_mysql_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:18:19.015203 database-mysql-local-0.0.285/database_mysql_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 17:17:18.000000 database-mysql-local-0.0.285/database_mysql_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4686 2024-04-06 17:17:18.000000 database-mysql-local-0.0.285/database_mysql_local/src/connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2895 2024-04-06 17:17:18.000000 database-mysql-local-0.0.285/database_mysql_local/src/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-04-06 17:17:18.000000 database-mysql-local-0.0.285/database_mysql_local/src/cursor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38968 2024-04-06 17:17:18.000000 database-mysql-local-0.0.285/database_mysql_local/src/generic_crud.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31705 2024-04-06 17:17:46.000000 database-mysql-local-0.0.285/database_mysql_local/src/generic_crud_ml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6406 2024-04-06 17:17:18.000000 database-mysql-local-0.0.285/database_mysql_local/src/generic_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-06 17:17:18.000000 database-mysql-local-0.0.285/database_mysql_local/src/point.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-04-06 17:17:18.000000 database-mysql-local-0.0.285/database_mysql_local/src/polygon.py
+-rw-r--r--   0 runner    (1001) docker     (127)   595483 2024-04-06 17:17:43.000000 database-mysql-local-0.0.285/database_mysql_local/src/table_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-04-06 17:17:18.000000 database-mysql-local-0.0.285/database_mysql_local/src/to_sql_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-04-06 17:17:18.000000 database-mysql-local-0.0.285/database_mysql_local/src/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:18:19.015203 database-mysql-local-0.0.285/database_mysql_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-06 17:18:19.000000 database-mysql-local-0.0.285/database_mysql_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-06 17:18:19.000000 database-mysql-local-0.0.285/database_mysql_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 17:18:19.000000 database-mysql-local-0.0.285/database_mysql_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-06 17:18:19.000000 database-mysql-local-0.0.285/database_mysql_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-06 17:18:19.000000 database-mysql-local-0.0.285/database_mysql_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-06 17:17:18.000000 database-mysql-local-0.0.285/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 17:18:19.019203 database-mysql-local-0.0.285/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-04-06 17:17:18.000000 database-mysql-local-0.0.285/setup.py
```

### Comparing `database-mysql-local-0.0.284/PKG-INFO` & `database-mysql-local-0.0.285/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: database-mysql-local
-Version: 0.0.284
+Version: 0.0.285
 Home-page: https://github.com/circles-zone/database-mysql-local-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `database-mysql-local-0.0.284/README.md` & `database-mysql-local-0.0.285/README.md`

 * *Files identical despite different names*

### Comparing `database-mysql-local-0.0.284/database_mysql_local/src/connector.py` & `database-mysql-local-0.0.285/database_mysql_local/src/connector.py`

 * *Files identical despite different names*

### Comparing `database-mysql-local-0.0.284/database_mysql_local/src/constants.py` & `database-mysql-local-0.0.285/database_mysql_local/src/constants.py`

 * *Files identical despite different names*

### Comparing `database-mysql-local-0.0.284/database_mysql_local/src/cursor.py` & `database-mysql-local-0.0.285/database_mysql_local/src/cursor.py`

 * *Files identical despite different names*

### Comparing `database-mysql-local-0.0.284/database_mysql_local/src/generic_crud.py` & `database-mysql-local-0.0.285/database_mysql_local/src/generic_crud.py`

 * *Files identical despite different names*

### Comparing `database-mysql-local-0.0.284/database_mysql_local/src/generic_crud_ml.py` & `database-mysql-local-0.0.285/database_mysql_local/src/generic_crud_ml.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -523,8 +523,8 @@
         self.logger.warning("this method is deprecated, use select_multi_tuple_by_id instead")
         """Selects a column from the table based on a WHERE clause and returns it as a list of dictionaries."""
         result = self.select_multi_tuple_by_value_with_none_option(condition_column_name, condition_column_value,
 
                                                                    view_table_name=view_table_name,
                                                                    select_clause_value=select_clause_value,
                                                                    limit=limit, order_by=order_by)
-        return [self.convert_to_dict(row, select_clause_value) for row in result]
+        return [self.convert_to_dict(row, select_clause_value) for row in result]
```

### Comparing `database-mysql-local-0.0.284/database_mysql_local/src/generic_mapping.py` & `database-mysql-local-0.0.285/database_mysql_local/src/generic_mapping.py`

 * *Files identical despite different names*

### Comparing `database-mysql-local-0.0.284/database_mysql_local/src/point.py` & `database-mysql-local-0.0.285/database_mysql_local/src/point.py`

 * *Files identical despite different names*

### Comparing `database-mysql-local-0.0.284/database_mysql_local/src/polygon.py` & `database-mysql-local-0.0.285/database_mysql_local/src/polygon.py`

 * *Files identical despite different names*

### Comparing `database-mysql-local-0.0.284/database_mysql_local/src/table_definition.py` & `database-mysql-local-0.0.285/database_mysql_local/src/table_definition.py`

 * *Files identical despite different names*

### Comparing `database-mysql-local-0.0.284/database_mysql_local/src/to_sql_interface.py` & `database-mysql-local-0.0.285/database_mysql_local/src/to_sql_interface.py`

 * *Files identical despite different names*

### Comparing `database-mysql-local-0.0.284/database_mysql_local/src/utils.py` & `database-mysql-local-0.0.285/database_mysql_local/src/utils.py`

 * *Files identical despite different names*

### Comparing `database-mysql-local-0.0.284/database_mysql_local.egg-info/PKG-INFO` & `database-mysql-local-0.0.285/database_mysql_local.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: database-mysql-local
-Version: 0.0.284
+Version: 0.0.285
 Home-page: https://github.com/circles-zone/database-mysql-local-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `database-mysql-local-0.0.284/database_mysql_local.egg-info/SOURCES.txt` & `database-mysql-local-0.0.285/database_mysql_local.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `database-mysql-local-0.0.284/pyproject.toml` & `database-mysql-local-0.0.285/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [tool.poetry]
 name = "database-mysql-local"
-version = "0.0.284" # https://pypi.org/project/database-mysql-local
+version = "0.0.285" # https://pypi.org/project/database-mysql-local
 description = "database-mysql-local Python Package"
 readme = "README.md"
 authors = [
     "Circlez.ai <info@circlez.ai>",
 ]
 
 # dephell deps convert --from pyproject.toml --from-format poetry --to setup.py --to-format setuppy
```

### Comparing `database-mysql-local-0.0.284/setup.py` & `database-mysql-local-0.0.285/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 package_dir = PACKAGE_NAME.replace("-", "_")
 # TODO: we are migrating from circles_local_database_python to database_mysql_local
 #  but in the meantime we want to keep both names
 old_name = "circles_local_database_python"
 
 setuptools.setup(
     name=PACKAGE_NAME,  # https://pypi.org/project/database-mysql-local
-    version='0.0.284',
+    version='0.0.285',
     author="Circles",
     author_email="info@circles.life",
     url=f"https://github.com/circles-zone/{PACKAGE_NAME}-python-package",
     packages=[package_dir, old_name],
     package_dir={package_dir: f'{package_dir}/src', old_name: f'{package_dir}/src'},
     package_data={package_dir: ['*.py']},
     long_description="Database MySQL Local",
```

