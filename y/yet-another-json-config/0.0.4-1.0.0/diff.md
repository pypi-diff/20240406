# Comparing `tmp/yet-another-json-config-0.0.4.tar.gz` & `tmp/yet-another-json-config-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yet-another-json-config-0.0.4.tar", last modified: Fri Jun 16 02:54:36 2023, max compression
+gzip compressed data, was "yet-another-json-config-1.0.0.tar", last modified: Sat Apr  6 18:04:41 2024, max compression
```

## Comparing `yet-another-json-config-0.0.4.tar` & `yet-another-json-config-1.0.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-16 02:54:36.682004 yet-another-json-config-0.0.4/
--rw-rw-rw-   0        0        0     1087 2023-03-14 02:31:51.000000 yet-another-json-config-0.0.4/LICENSE
--rw-rw-rw-   0        0        0     5024 2023-06-16 02:54:36.682004 yet-another-json-config-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     4408 2023-03-14 03:17:31.000000 yet-another-json-config-0.0.4/README.md
--rw-rw-rw-   0        0        0      692 2023-06-16 02:53:04.000000 yet-another-json-config-0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-16 02:54:36.682004 yet-another-json-config-0.0.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-16 02:54:36.651382 yet-another-json-config-0.0.4/src/
-drwxrwxrwx   0        0        0        0 2023-06-16 02:54:36.666804 yet-another-json-config-0.0.4/src/yet_another_json_config/
--rw-rw-rw-   0        0        0       43 2023-03-14 02:31:51.000000 yet-another-json-config-0.0.4/src/yet_another_json_config/__init__.py
--rw-rw-rw-   0        0        0     6185 2023-06-16 02:52:51.000000 yet-another-json-config-0.0.4/src/yet_another_json_config/yet_another_json_config.py
-drwxrwxrwx   0        0        0        0 2023-06-16 02:54:36.680003 yet-another-json-config-0.0.4/src/yet_another_json_config.egg-info/
--rw-rw-rw-   0        0        0     5024 2023-06-16 02:54:36.000000 yet-another-json-config-0.0.4/src/yet_another_json_config.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      352 2023-06-16 02:54:36.000000 yet-another-json-config-0.0.4/src/yet_another_json_config.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-16 02:54:36.000000 yet-another-json-config-0.0.4/src/yet_another_json_config.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-06-16 02:54:36.000000 yet-another-json-config-0.0.4/src/yet_another_json_config.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-16 02:54:36.681005 yet-another-json-config-0.0.4/tests/
--rw-rw-rw-   0        0        0     4939 2023-03-14 02:39:28.000000 yet-another-json-config-0.0.4/tests/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:04:41.673148 yet-another-json-config-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-06 18:04:37.000000 yet-another-json-config-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4838 2024-04-06 18:04:41.673148 yet-another-json-config-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4237 2024-04-06 18:04:37.000000 yet-another-json-config-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-06 18:04:37.000000 yet-another-json-config-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 18:04:41.673148 yet-another-json-config-1.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:04:41.669149 yet-another-json-config-1.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:04:41.669149 yet-another-json-config-1.0.0/src/yet_another_json_config/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-06 18:04:37.000000 yet-another-json-config-1.0.0/src/yet_another_json_config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7312 2024-04-06 18:04:37.000000 yet-another-json-config-1.0.0/src/yet_another_json_config/yet_another_json_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:04:41.673148 yet-another-json-config-1.0.0/src/yet_another_json_config.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4838 2024-04-06 18:04:41.000000 yet-another-json-config-1.0.0/src/yet_another_json_config.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-06 18:04:41.000000 yet-another-json-config-1.0.0/src/yet_another_json_config.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 18:04:41.000000 yet-another-json-config-1.0.0/src/yet_another_json_config.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-06 18:04:41.000000 yet-another-json-config-1.0.0/src/yet_another_json_config.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:04:41.673148 yet-another-json-config-1.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4814 2024-04-06 18:04:37.000000 yet-another-json-config-1.0.0/tests/test_config.py
```

### Comparing `yet-another-json-config-0.0.4/PKG-INFO` & `yet-another-json-config-1.0.0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,186 +1,172 @@
-Metadata-Version: 2.1
-Name: yet-another-json-config
-Version: 0.0.4
-Summary: Reads and write json files as a configuration file, supports nested json values.
-Author-email: engmtcdrm <gabif54409@rolenot.com>
-Project-URL: Homepage, https://github.com/engmtcdrm/yet-another-json-config
-Project-URL: Bug Tracker, https://github.com/engmtcdrm/yet-another-json-config/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# yet-another-json-config
-Python class to reads and write json files as a configuration file, supports nested json values.
-
-# Examples
-
-## Initializing `Config` Class
-```py
-from yet_another_json_config import Config
-
-c = Config('./tests/test.json')
-```
-
-## Listing Settings
-```py
-from yet_another_json_config import Config
-
-c = Config('./tests/test.json')
-
-print(c.settings)
-```
-
-### Output
-```json
-{
-    "test": "test",
-    "varUserTest": "test_$user$",
-    "nestedTest": {
-        "test": "test"
-    },
-    "nestedTest2": {
-        "nested": {
-            "test": "test"
-        }
-    },
-    "get": "test"
-}
-```
-
-## Get Setting
-Settings can be obtained two ways through the method `get`
-
-### Class Method `get`
-```py
-# setting a basic setting
-c.get('test')
-
-# setting a nested setting via list of strings
-c.get('nestedTest2', 'nested', 'test')
-
-# setting a nested setting via tuple
-c.get(('nestedTest2', 'nested', 'test'))
-```
-
-### `key` Method
-```py
-# setting a basic setting
-print(c['test'])
-
-# setting a nested setting
-print(c['nestedTest2']['nested']['test'])
-```
-
-## Set Setting
-Settings can be both created and modified using the same methods. If a setting does not exist and one of the following methods is used, it will be created. If the setting already exists, it will be updated.
-
-### Class Method `set`
-This method supports *args for defining the keys for a setting. This means that a list of strings (not type of list) or a tuple can be passed to set the value.
-
-```py
-# setting a basic setting
-c.set('test', value='test2')
-
-# setting a nested setting via list of strings
-c.set('nestedTest2', 'nested', 'test', value='test2')
-
-# setting a nested setting via tuple
-c.set(('nestedTest2', 'nested', 'test'), value='test2')
-```
-
-### `key` Method
-```py
-# setting a basic setting
-c['test'] = 'test2'
-
-# setting a nested setting
-c['nestedTest2']['nested']['test'] = 'test2'
-```
-
-## Delete Setting
-Settings can be deleted two ways through the method `delete` and the `del` statement. As well, nested settings can also be deleted. Below are an example of each.
-
-### Class Method `delete`
-```py
-# deleting a basic setting
-c.delete('test')
-
-# deleting a nested setting
-c.delete(('nestedTest2', 'nested', 'test'))
-```
-
-### `del` Statement Method
-```py
-# deleting a basic setting
-del c['test']
-
-# deleting a nested setting
-del c['nestedTest2']['nested']['test']
-```
-
-## Custom Config Class
-Below is an example of a custom config class that is derived off the `Config` class. In this example it allows for the variable `$user$` to be replaced at run time with the user id that is currently running the code. This could be expanded further as well as potential validation of the configuration file after loading via the `validate` method.
-
-```py
-import getpass
-from yet_another_json_config import Config
-
-class CustomConfig(Config):
-    def _load(self):
-        super()._load()
-
-        user = getpass.getuser()
-
-        if 'varUserTest' in self._settings:
-            # replace special character in filename with the username
-            self.set('varUserTest', value=self.get('varUserTest').replace('$user$', user))
-
-        print(self._settings)
-
-        self.validate()
-
-    def validate(self):
-        pass
-
-
-conf = CustomConfig('./tests/test.json')
-
-print(conf.settings())
-```
-
-# API Reference
-> ```py
-> class Config(config_file_path, file_must_exist=False)
-> ```
-
-Create an instance of a configuration file.
-
-## Arguments
-
-- **`config_file_path`** (`str`) - The path to the configuration file.
-- **`file_must_exist`** (`bool, Optional`) - Raises a `FileNotFoundError` exception if file does not exist. Default value is `False`.
-
-> ```py
-> get(*keys: str)
-> ```
-
-Returns the value of the keys specified.
-
-- **`*keys`** - (`str`) - List of `str` or Tuple of `str` traversing the settings and return a value if the setting exists. If the setting does not exist, a `KeyError` exception is raised.
-
-> ```py
-> set(*keys: str, value)
-> ```
-
-Sets the keys to the value specified.
-
-- **`*keys`** - (`str`) - List of `str` or Tuple of `str` traversing the settings to set the specified key to the specified value. If the setting does not exist, the setting is created.
-
-> ```py
-> settings()
-> ```
-
-Returns all settings in the configuration.
+# yet-another-json-config
+Python class to reads and write json files as a configuration file, supports nested json values.
+
+# Examples
+
+## Initializing `Config` Class
+```py
+from yet_another_json_config import Config
+
+c = Config('./tests/test.json')
+```
+
+## Listing Settings
+```py
+from yet_another_json_config import Config
+
+c = Config('./tests/test.json')
+
+print(c.settings)
+```
+
+### Output
+```json
+{
+    "test": "test",
+    "varUserTest": "test_$user$",
+    "nestedTest": {
+        "test": "test"
+    },
+    "nestedTest2": {
+        "nested": {
+            "test": "test"
+        }
+    },
+    "get": "test"
+}
+```
+
+## Get Setting
+Settings can be obtained two ways through the method `get`
+
+### Class Method `get`
+```py
+# setting a basic setting
+c.get('test')
+
+# setting a nested setting via list of strings
+c.get('nestedTest2', 'nested', 'test')
+
+# setting a nested setting via tuple
+c.get(('nestedTest2', 'nested', 'test'))
+```
+
+### `key` Method
+```py
+# setting a basic setting
+print(c['test'])
+
+# setting a nested setting
+print(c['nestedTest2']['nested']['test'])
+```
+
+## Set Setting
+Settings can be both created and modified using the same methods. If a setting does not exist and one of the following methods is used, it will be created. If the setting already exists, it will be updated.
+
+### Class Method `set`
+This method supports *args for defining the keys for a setting. This means that a list of strings (not type of list) or a tuple can be passed to set the value.
+
+```py
+# setting a basic setting
+c.set('test', value='test2')
+
+# setting a nested setting via list of strings
+c.set('nestedTest2', 'nested', 'test', value='test2')
+
+# setting a nested setting via tuple
+c.set(('nestedTest2', 'nested', 'test'), value='test2')
+```
+
+### `key` Method
+```py
+# setting a basic setting
+c['test'] = 'test2'
+
+# setting a nested setting
+c['nestedTest2']['nested']['test'] = 'test2'
+```
+
+## Delete Setting
+Settings can be deleted two ways through the method `delete` and the `del` statement. As well, nested settings can also be deleted. Below are an example of each.
+
+### Class Method `delete`
+```py
+# deleting a basic setting
+c.delete('test')
+
+# deleting a nested setting
+c.delete(('nestedTest2', 'nested', 'test'))
+```
+
+### `del` Statement Method
+```py
+# deleting a basic setting
+del c['test']
+
+# deleting a nested setting
+del c['nestedTest2']['nested']['test']
+```
+
+## Custom Config Class
+Below is an example of a custom config class that is derived off the `Config` class. In this example it allows for the variable `$user$` to be replaced at run time with the user id that is currently running the code. This could be expanded further as well as potential validation of the configuration file after loading via the `validate` method.
+
+```py
+import getpass
+from yet_another_json_config import Config
+
+class CustomConfig(Config):
+    def _load(self):
+        super()._load()
+
+        user = getpass.getuser()
+
+        if 'varUserTest' in self._settings:
+            # replace special character in filename with the username
+            self.set('varUserTest', value=self.get('varUserTest').replace('$user$', user))
+
+        print(self._settings)
+
+        self.validate()
+
+    def validate(self):
+        pass
+
+
+conf = CustomConfig('./tests/test.json')
+
+print(conf.settings())
+```
+
+# API Reference
+> ```py
+> class Config(config_file_path, file_must_exist=False)
+> ```
+
+Create an instance of a configuration file.
+
+## Arguments
+
+- **`config_file_path`** (`str`) - The path to the configuration file.
+- **`file_must_exist`** (`bool, Optional`) - Raises a `FileNotFoundError` exception if file does not exist. Default value is `False`.
+
+> ```py
+> get(*keys: str)
+> ```
+
+Returns the value of the keys specified.
+
+- **`*keys`** - (`str`) - List of `str` or Tuple of `str` traversing the settings and return a value if the setting exists. If the setting does not exist, a `KeyError` exception is raised.
+
+> ```py
+> set(*keys: str, value)
+> ```
+
+Sets the keys to the value specified.
+
+- **`*keys`** - (`str`) - List of `str` or Tuple of `str` traversing the settings to set the specified key to the specified value. If the setting does not exist, the setting is created.
+
+> ```py
+> settings()
+> ```
+
+Returns all settings in the configuration.
```

### Comparing `yet-another-json-config-0.0.4/README.md` & `yet-another-json-config-1.0.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,172 +1,186 @@
-# yet-another-json-config
-Python class to reads and write json files as a configuration file, supports nested json values.
-
-# Examples
-
-## Initializing `Config` Class
-```py
-from yet_another_json_config import Config
-
-c = Config('./tests/test.json')
-```
-
-## Listing Settings
-```py
-from yet_another_json_config import Config
-
-c = Config('./tests/test.json')
-
-print(c.settings)
-```
-
-### Output
-```json
-{
-    "test": "test",
-    "varUserTest": "test_$user$",
-    "nestedTest": {
-        "test": "test"
-    },
-    "nestedTest2": {
-        "nested": {
-            "test": "test"
-        }
-    },
-    "get": "test"
-}
-```
-
-## Get Setting
-Settings can be obtained two ways through the method `get`
-
-### Class Method `get`
-```py
-# setting a basic setting
-c.get('test')
-
-# setting a nested setting via list of strings
-c.get('nestedTest2', 'nested', 'test')
-
-# setting a nested setting via tuple
-c.get(('nestedTest2', 'nested', 'test'))
-```
-
-### `key` Method
-```py
-# setting a basic setting
-print(c['test'])
-
-# setting a nested setting
-print(c['nestedTest2']['nested']['test'])
-```
-
-## Set Setting
-Settings can be both created and modified using the same methods. If a setting does not exist and one of the following methods is used, it will be created. If the setting already exists, it will be updated.
-
-### Class Method `set`
-This method supports *args for defining the keys for a setting. This means that a list of strings (not type of list) or a tuple can be passed to set the value.
-
-```py
-# setting a basic setting
-c.set('test', value='test2')
-
-# setting a nested setting via list of strings
-c.set('nestedTest2', 'nested', 'test', value='test2')
-
-# setting a nested setting via tuple
-c.set(('nestedTest2', 'nested', 'test'), value='test2')
-```
-
-### `key` Method
-```py
-# setting a basic setting
-c['test'] = 'test2'
-
-# setting a nested setting
-c['nestedTest2']['nested']['test'] = 'test2'
-```
-
-## Delete Setting
-Settings can be deleted two ways through the method `delete` and the `del` statement. As well, nested settings can also be deleted. Below are an example of each.
-
-### Class Method `delete`
-```py
-# deleting a basic setting
-c.delete('test')
-
-# deleting a nested setting
-c.delete(('nestedTest2', 'nested', 'test'))
-```
-
-### `del` Statement Method
-```py
-# deleting a basic setting
-del c['test']
-
-# deleting a nested setting
-del c['nestedTest2']['nested']['test']
-```
-
-## Custom Config Class
-Below is an example of a custom config class that is derived off the `Config` class. In this example it allows for the variable `$user$` to be replaced at run time with the user id that is currently running the code. This could be expanded further as well as potential validation of the configuration file after loading via the `validate` method.
-
-```py
-import getpass
-from yet_another_json_config import Config
-
-class CustomConfig(Config):
-    def _load(self):
-        super()._load()
-
-        user = getpass.getuser()
-
-        if 'varUserTest' in self._settings:
-            # replace special character in filename with the username
-            self.set('varUserTest', value=self.get('varUserTest').replace('$user$', user))
-
-        print(self._settings)
-
-        self.validate()
-
-    def validate(self):
-        pass
-
-
-conf = CustomConfig('./tests/test.json')
-
-print(conf.settings())
-```
-
-# API Reference
-> ```py
-> class Config(config_file_path, file_must_exist=False)
-> ```
-
-Create an instance of a configuration file.
-
-## Arguments
-
-- **`config_file_path`** (`str`) - The path to the configuration file.
-- **`file_must_exist`** (`bool, Optional`) - Raises a `FileNotFoundError` exception if file does not exist. Default value is `False`.
-
-> ```py
-> get(*keys: str)
-> ```
-
-Returns the value of the keys specified.
-
-- **`*keys`** - (`str`) - List of `str` or Tuple of `str` traversing the settings and return a value if the setting exists. If the setting does not exist, a `KeyError` exception is raised.
-
-> ```py
-> set(*keys: str, value)
-> ```
-
-Sets the keys to the value specified.
-
-- **`*keys`** - (`str`) - List of `str` or Tuple of `str` traversing the settings to set the specified key to the specified value. If the setting does not exist, the setting is created.
-
-> ```py
-> settings()
-> ```
-
-Returns all settings in the configuration.
+Metadata-Version: 2.1
+Name: yet-another-json-config
+Version: 1.0.0
+Summary: Reads and write json files as a configuration file, supports nested json values.
+Author-email: engmtcdrm <gabif54409@rolenot.com>
+Project-URL: Homepage, https://github.com/engmtcdrm/yet-another-json-config
+Project-URL: Bug Tracker, https://github.com/engmtcdrm/yet-another-json-config/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# yet-another-json-config
+Python class to reads and write json files as a configuration file, supports nested json values.
+
+# Examples
+
+## Initializing `Config` Class
+```py
+from yet_another_json_config import Config
+
+c = Config('./tests/test.json')
+```
+
+## Listing Settings
+```py
+from yet_another_json_config import Config
+
+c = Config('./tests/test.json')
+
+print(c.settings)
+```
+
+### Output
+```json
+{
+    "test": "test",
+    "varUserTest": "test_$user$",
+    "nestedTest": {
+        "test": "test"
+    },
+    "nestedTest2": {
+        "nested": {
+            "test": "test"
+        }
+    },
+    "get": "test"
+}
+```
+
+## Get Setting
+Settings can be obtained two ways through the method `get`
+
+### Class Method `get`
+```py
+# setting a basic setting
+c.get('test')
+
+# setting a nested setting via list of strings
+c.get('nestedTest2', 'nested', 'test')
+
+# setting a nested setting via tuple
+c.get(('nestedTest2', 'nested', 'test'))
+```
+
+### `key` Method
+```py
+# setting a basic setting
+print(c['test'])
+
+# setting a nested setting
+print(c['nestedTest2']['nested']['test'])
+```
+
+## Set Setting
+Settings can be both created and modified using the same methods. If a setting does not exist and one of the following methods is used, it will be created. If the setting already exists, it will be updated.
+
+### Class Method `set`
+This method supports *args for defining the keys for a setting. This means that a list of strings (not type of list) or a tuple can be passed to set the value.
+
+```py
+# setting a basic setting
+c.set('test', value='test2')
+
+# setting a nested setting via list of strings
+c.set('nestedTest2', 'nested', 'test', value='test2')
+
+# setting a nested setting via tuple
+c.set(('nestedTest2', 'nested', 'test'), value='test2')
+```
+
+### `key` Method
+```py
+# setting a basic setting
+c['test'] = 'test2'
+
+# setting a nested setting
+c['nestedTest2']['nested']['test'] = 'test2'
+```
+
+## Delete Setting
+Settings can be deleted two ways through the method `delete` and the `del` statement. As well, nested settings can also be deleted. Below are an example of each.
+
+### Class Method `delete`
+```py
+# deleting a basic setting
+c.delete('test')
+
+# deleting a nested setting
+c.delete(('nestedTest2', 'nested', 'test'))
+```
+
+### `del` Statement Method
+```py
+# deleting a basic setting
+del c['test']
+
+# deleting a nested setting
+del c['nestedTest2']['nested']['test']
+```
+
+## Custom Config Class
+Below is an example of a custom config class that is derived off the `Config` class. In this example it allows for the variable `$user$` to be replaced at run time with the user id that is currently running the code. This could be expanded further as well as potential validation of the configuration file after loading via the `validate` method.
+
+```py
+import getpass
+from yet_another_json_config import Config
+
+class CustomConfig(Config):
+    def _load(self):
+        super()._load()
+
+        user = getpass.getuser()
+
+        if 'varUserTest' in self._settings:
+            # replace special character in filename with the username
+            self.set('varUserTest', value=self.get('varUserTest').replace('$user$', user))
+
+        print(self._settings)
+
+        self.validate()
+
+    def validate(self):
+        pass
+
+
+conf = CustomConfig('./tests/test.json')
+
+print(conf.settings())
+```
+
+# API Reference
+> ```py
+> class Config(config_file_path, file_must_exist=False)
+> ```
+
+Create an instance of a configuration file.
+
+## Arguments
+
+- **`config_file_path`** (`str`) - The path to the configuration file.
+- **`file_must_exist`** (`bool, Optional`) - Raises a `FileNotFoundError` exception if file does not exist. Default value is `False`.
+
+> ```py
+> get(*keys: str)
+> ```
+
+Returns the value of the keys specified.
+
+- **`*keys`** - (`str`) - List of `str` or Tuple of `str` traversing the settings and return a value if the setting exists. If the setting does not exist, a `KeyError` exception is raised.
+
+> ```py
+> set(*keys: str, value)
+> ```
+
+Sets the keys to the value specified.
+
+- **`*keys`** - (`str`) - List of `str` or Tuple of `str` traversing the settings to set the specified key to the specified value. If the setting does not exist, the setting is created.
+
+> ```py
+> settings()
+> ```
+
+Returns all settings in the configuration.
```

### Comparing `yet-another-json-config-0.0.4/src/yet_another_json_config.egg-info/PKG-INFO` & `yet-another-json-config-1.0.0/src/yet_another_json_config.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,186 +1,186 @@
-Metadata-Version: 2.1
-Name: yet-another-json-config
-Version: 0.0.4
-Summary: Reads and write json files as a configuration file, supports nested json values.
-Author-email: engmtcdrm <gabif54409@rolenot.com>
-Project-URL: Homepage, https://github.com/engmtcdrm/yet-another-json-config
-Project-URL: Bug Tracker, https://github.com/engmtcdrm/yet-another-json-config/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# yet-another-json-config
-Python class to reads and write json files as a configuration file, supports nested json values.
-
-# Examples
-
-## Initializing `Config` Class
-```py
-from yet_another_json_config import Config
-
-c = Config('./tests/test.json')
-```
-
-## Listing Settings
-```py
-from yet_another_json_config import Config
-
-c = Config('./tests/test.json')
-
-print(c.settings)
-```
-
-### Output
-```json
-{
-    "test": "test",
-    "varUserTest": "test_$user$",
-    "nestedTest": {
-        "test": "test"
-    },
-    "nestedTest2": {
-        "nested": {
-            "test": "test"
-        }
-    },
-    "get": "test"
-}
-```
-
-## Get Setting
-Settings can be obtained two ways through the method `get`
-
-### Class Method `get`
-```py
-# setting a basic setting
-c.get('test')
-
-# setting a nested setting via list of strings
-c.get('nestedTest2', 'nested', 'test')
-
-# setting a nested setting via tuple
-c.get(('nestedTest2', 'nested', 'test'))
-```
-
-### `key` Method
-```py
-# setting a basic setting
-print(c['test'])
-
-# setting a nested setting
-print(c['nestedTest2']['nested']['test'])
-```
-
-## Set Setting
-Settings can be both created and modified using the same methods. If a setting does not exist and one of the following methods is used, it will be created. If the setting already exists, it will be updated.
-
-### Class Method `set`
-This method supports *args for defining the keys for a setting. This means that a list of strings (not type of list) or a tuple can be passed to set the value.
-
-```py
-# setting a basic setting
-c.set('test', value='test2')
-
-# setting a nested setting via list of strings
-c.set('nestedTest2', 'nested', 'test', value='test2')
-
-# setting a nested setting via tuple
-c.set(('nestedTest2', 'nested', 'test'), value='test2')
-```
-
-### `key` Method
-```py
-# setting a basic setting
-c['test'] = 'test2'
-
-# setting a nested setting
-c['nestedTest2']['nested']['test'] = 'test2'
-```
-
-## Delete Setting
-Settings can be deleted two ways through the method `delete` and the `del` statement. As well, nested settings can also be deleted. Below are an example of each.
-
-### Class Method `delete`
-```py
-# deleting a basic setting
-c.delete('test')
-
-# deleting a nested setting
-c.delete(('nestedTest2', 'nested', 'test'))
-```
-
-### `del` Statement Method
-```py
-# deleting a basic setting
-del c['test']
-
-# deleting a nested setting
-del c['nestedTest2']['nested']['test']
-```
-
-## Custom Config Class
-Below is an example of a custom config class that is derived off the `Config` class. In this example it allows for the variable `$user$` to be replaced at run time with the user id that is currently running the code. This could be expanded further as well as potential validation of the configuration file after loading via the `validate` method.
-
-```py
-import getpass
-from yet_another_json_config import Config
-
-class CustomConfig(Config):
-    def _load(self):
-        super()._load()
-
-        user = getpass.getuser()
-
-        if 'varUserTest' in self._settings:
-            # replace special character in filename with the username
-            self.set('varUserTest', value=self.get('varUserTest').replace('$user$', user))
-
-        print(self._settings)
-
-        self.validate()
-
-    def validate(self):
-        pass
-
-
-conf = CustomConfig('./tests/test.json')
-
-print(conf.settings())
-```
-
-# API Reference
-> ```py
-> class Config(config_file_path, file_must_exist=False)
-> ```
-
-Create an instance of a configuration file.
-
-## Arguments
-
-- **`config_file_path`** (`str`) - The path to the configuration file.
-- **`file_must_exist`** (`bool, Optional`) - Raises a `FileNotFoundError` exception if file does not exist. Default value is `False`.
-
-> ```py
-> get(*keys: str)
-> ```
-
-Returns the value of the keys specified.
-
-- **`*keys`** - (`str`) - List of `str` or Tuple of `str` traversing the settings and return a value if the setting exists. If the setting does not exist, a `KeyError` exception is raised.
-
-> ```py
-> set(*keys: str, value)
-> ```
-
-Sets the keys to the value specified.
-
-- **`*keys`** - (`str`) - List of `str` or Tuple of `str` traversing the settings to set the specified key to the specified value. If the setting does not exist, the setting is created.
-
-> ```py
-> settings()
-> ```
-
-Returns all settings in the configuration.
+Metadata-Version: 2.1
+Name: yet-another-json-config
+Version: 1.0.0
+Summary: Reads and write json files as a configuration file, supports nested json values.
+Author-email: engmtcdrm <gabif54409@rolenot.com>
+Project-URL: Homepage, https://github.com/engmtcdrm/yet-another-json-config
+Project-URL: Bug Tracker, https://github.com/engmtcdrm/yet-another-json-config/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# yet-another-json-config
+Python class to reads and write json files as a configuration file, supports nested json values.
+
+# Examples
+
+## Initializing `Config` Class
+```py
+from yet_another_json_config import Config
+
+c = Config('./tests/test.json')
+```
+
+## Listing Settings
+```py
+from yet_another_json_config import Config
+
+c = Config('./tests/test.json')
+
+print(c.settings)
+```
+
+### Output
+```json
+{
+    "test": "test",
+    "varUserTest": "test_$user$",
+    "nestedTest": {
+        "test": "test"
+    },
+    "nestedTest2": {
+        "nested": {
+            "test": "test"
+        }
+    },
+    "get": "test"
+}
+```
+
+## Get Setting
+Settings can be obtained two ways through the method `get`
+
+### Class Method `get`
+```py
+# setting a basic setting
+c.get('test')
+
+# setting a nested setting via list of strings
+c.get('nestedTest2', 'nested', 'test')
+
+# setting a nested setting via tuple
+c.get(('nestedTest2', 'nested', 'test'))
+```
+
+### `key` Method
+```py
+# setting a basic setting
+print(c['test'])
+
+# setting a nested setting
+print(c['nestedTest2']['nested']['test'])
+```
+
+## Set Setting
+Settings can be both created and modified using the same methods. If a setting does not exist and one of the following methods is used, it will be created. If the setting already exists, it will be updated.
+
+### Class Method `set`
+This method supports *args for defining the keys for a setting. This means that a list of strings (not type of list) or a tuple can be passed to set the value.
+
+```py
+# setting a basic setting
+c.set('test', value='test2')
+
+# setting a nested setting via list of strings
+c.set('nestedTest2', 'nested', 'test', value='test2')
+
+# setting a nested setting via tuple
+c.set(('nestedTest2', 'nested', 'test'), value='test2')
+```
+
+### `key` Method
+```py
+# setting a basic setting
+c['test'] = 'test2'
+
+# setting a nested setting
+c['nestedTest2']['nested']['test'] = 'test2'
+```
+
+## Delete Setting
+Settings can be deleted two ways through the method `delete` and the `del` statement. As well, nested settings can also be deleted. Below are an example of each.
+
+### Class Method `delete`
+```py
+# deleting a basic setting
+c.delete('test')
+
+# deleting a nested setting
+c.delete(('nestedTest2', 'nested', 'test'))
+```
+
+### `del` Statement Method
+```py
+# deleting a basic setting
+del c['test']
+
+# deleting a nested setting
+del c['nestedTest2']['nested']['test']
+```
+
+## Custom Config Class
+Below is an example of a custom config class that is derived off the `Config` class. In this example it allows for the variable `$user$` to be replaced at run time with the user id that is currently running the code. This could be expanded further as well as potential validation of the configuration file after loading via the `validate` method.
+
+```py
+import getpass
+from yet_another_json_config import Config
+
+class CustomConfig(Config):
+    def _load(self):
+        super()._load()
+
+        user = getpass.getuser()
+
+        if 'varUserTest' in self._settings:
+            # replace special character in filename with the username
+            self.set('varUserTest', value=self.get('varUserTest').replace('$user$', user))
+
+        print(self._settings)
+
+        self.validate()
+
+    def validate(self):
+        pass
+
+
+conf = CustomConfig('./tests/test.json')
+
+print(conf.settings())
+```
+
+# API Reference
+> ```py
+> class Config(config_file_path, file_must_exist=False)
+> ```
+
+Create an instance of a configuration file.
+
+## Arguments
+
+- **`config_file_path`** (`str`) - The path to the configuration file.
+- **`file_must_exist`** (`bool, Optional`) - Raises a `FileNotFoundError` exception if file does not exist. Default value is `False`.
+
+> ```py
+> get(*keys: str)
+> ```
+
+Returns the value of the keys specified.
+
+- **`*keys`** - (`str`) - List of `str` or Tuple of `str` traversing the settings and return a value if the setting exists. If the setting does not exist, a `KeyError` exception is raised.
+
+> ```py
+> set(*keys: str, value)
+> ```
+
+Sets the keys to the value specified.
+
+- **`*keys`** - (`str`) - List of `str` or Tuple of `str` traversing the settings to set the specified key to the specified value. If the setting does not exist, the setting is created.
+
+> ```py
+> settings()
+> ```
+
+Returns all settings in the configuration.
```

### Comparing `yet-another-json-config-0.0.4/tests/test_config.py` & `yet-another-json-config-1.0.0/tests/test_config.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,178 +1,181 @@
-import pytest
-from json import JSONDecodeError
-from contextlib import nullcontext as does_not_raise
-from src.yet_another_json_config.yet_another_json_config import Config
-import os
-
-@pytest.fixture
-def valid_config():
-    conf = Config('./tests/test.json')
-    return conf
-
-@pytest.fixture()
-def invalid_test_file(tmp_path):
-    return os.path.join(tmp_path, './tests/invalid_test_file?/:|.\\json')
-
-@pytest.fixture()
-def new_test_file(tmp_path):
-    return os.path.join(tmp_path, 'new_config_test.json')
-
-@pytest.fixture()
-def malformed_test_file():
-    return './tests/malformed_test.json'
-
-
-## Initialization tests
-
-def test_load(valid_config):
-    assert valid_config != {}
-
-def test_invalid_config_name(invalid_test_file):
-    with pytest.raises(OSError):
-        Config(invalid_test_file)
-
-def test_new_config(new_test_file):
-    c = Config(new_test_file)
-
-    assert c.settings() == {}
-
-def test_file_must_exist_config(new_test_file):
-    with pytest.raises(FileNotFoundError):
-        Config(new_test_file, True)
-
-def test_malformed_load(malformed_test_file):
-    with pytest.raises(JSONDecodeError):
-        Config(malformed_test_file)
-
-
-
-
-## SET tests
-
-### FUNC tests
-
-@pytest.mark.parametrize('keys, orig_val, expected_val, expected_except', [
-    ('test', 'test', 'test2', does_not_raise()),
-    (('nestedTest', 'test'), 'test', 'test2', does_not_raise()),
-    ('get', 'test', 'test2', does_not_raise()),
-    ('badNestedTest', 'test', 'test2', pytest.raises(KeyError)),
-    (None, None, None, pytest.raises(KeyError)),
-    ((), None, None, pytest.raises(KeyError)),
-    ([], None, None, pytest.raises(KeyError))
-])
-
-def test_set_by_func(valid_config, keys, orig_val, expected_val, expected_except):
-    with expected_except:
-        v = valid_config.get(keys)
-        valid_config.set(keys, value=expected_val)
-
-        assert v == orig_val and valid_config.get(keys) != orig_val and valid_config.get(keys) == expected_val
-
-### KEY tests
-
-def test_key_set(valid_config):
-    v = valid_config['test']
-    valid_config['test'] = 'test2'
-
-    assert v == 'test' and valid_config['test'] != 'test' and valid_config['test'] == 'test2'
-
-
-
-
-## GET tests
-
-### FUNC tests
-
-@pytest.mark.parametrize('keys, expected_result, expected_except', [
-    ('test', 'test', does_not_raise()),
-    ('nestedTest', { 'test': 'test' }, does_not_raise()),
-    (('nestedTest', 'test'), 'test', does_not_raise()),
-    (('nestedTest2', 'nested', 'test'), 'test', does_not_raise()),
-    ('get', 'test', does_not_raise()),
-    (None, None, pytest.raises(KeyError)),
-    ((), None, pytest.raises(KeyError)),
-    ([], None, pytest.raises(KeyError))
-])
-
-def test_get_by_func(valid_config, keys, expected_result, expected_except):
-    with expected_except:
-        v = valid_config.get(keys)
-
-        assert v == expected_result
-
-### KEY tests
-
-@pytest.mark.parametrize('keys, expected_result, expected_except', [
-    ('test', 'test', does_not_raise()),
-    ('nestedTest', { 'test': 'test' }, does_not_raise()),
-    (('nestedTest', 'test'), 'test', does_not_raise()),
-    (('nestedTest2', 'nested', 'test'), 'test', does_not_raise()),
-    ('get', 'test', does_not_raise()),
-    (None, None, pytest.raises(KeyError)),
-    ((), None, pytest.raises(KeyError)),
-    ([], None, pytest.raises(KeyError))
-])
-
-def test_get_by_key(valid_config, keys, expected_result, expected_except):
-    with expected_except:
-        if type(keys) == str or type(keys) == type(None):
-            v = valid_config[keys]
-        elif type(keys) == tuple:
-            fk = ()
-
-            if len(keys) > 0:
-                fk = keys[0]
-
-            v = valid_config[fk]
-
-            for k in keys[1:]:
-                v = v[k]
-        elif type(keys) == list:
-            fk = []
-
-            if len(keys) > 0:
-                fk = keys[0]
-
-            v = valid_config[fk]
-
-            for k in keys[1:]:
-                v = v[k]
-        else:
-            assert 1 == 2
-
-        assert v == expected_result
-
-
-
-
-## DELETE tests
-
-### FUNC tests
-
-@pytest.mark.parametrize('keys, expected_except', [
-    ('test', does_not_raise()),
-    (('nestedTest', 'test'), does_not_raise()),
-    (('nestedTest2', 'nested', 'test'), does_not_raise()),
-    ('badDelete', pytest.raises(KeyError)),
-    (None, pytest.raises(KeyError)),
-    ((), pytest.raises(KeyError)),
-    ([], pytest.raises(KeyError))
-])
-
-def test_delete_by_func(valid_config, keys, expected_except):
-    with expected_except:
-        valid_config.delete(keys)
-
-        assert keys not in valid_config
-
-### KEY tests
-
-def test_key_delete(valid_config):
-    del valid_config['test']
-
-    assert 'test' not in valid_config
-
-def test_key_nested_delete(valid_config):
-    del valid_config['nestedTest']['test']
-
+from contextlib import nullcontext as does_not_raise
+from json import JSONDecodeError
+import os
+
+import pytest
+from src.yet_another_json_config.yet_another_json_config import Config
+
+
+@pytest.fixture
+def valid_config():
+    conf = Config('./tests/test.json')
+    return conf
+
+@pytest.fixture()
+def invalid_test_file(tmp_path):
+    return os.path.join(tmp_path, './tests/invalid_test_file?/:|.\\json')
+
+@pytest.fixture()
+def new_test_file(tmp_path):
+    return os.path.join(tmp_path, 'new_config_test.json')
+
+@pytest.fixture()
+def malformed_test_file():
+    return './tests/malformed_test.json'
+
+
+## Initialization tests
+
+def test_load(valid_config):
+    assert valid_config != {}
+
+def test_invalid_config_name(invalid_test_file):
+    with pytest.raises(OSError):
+        Config(invalid_test_file)
+
+def test_new_config(new_test_file):
+    c = Config(new_test_file)
+
+    assert os.path.isfile(new_test_file) == False
+    assert c.settings() == {}
+
+def test_file_must_exist_config(new_test_file):
+    with pytest.raises(FileNotFoundError):
+        Config(new_test_file, True)
+
+def test_malformed_load(malformed_test_file):
+    with pytest.raises(JSONDecodeError):
+        Config(malformed_test_file)
+
+
+
+
+## SET tests
+
+### FUNC tests
+
+@pytest.mark.parametrize('keys, orig_val, expected_val, expected_except', [
+    ('test', 'test', 'test2', does_not_raise()),
+    (('nestedTest', 'test'), 'test', 'test2', does_not_raise()),
+    ('get', 'test', 'test2', does_not_raise()),
+    ('badNestedTest', 'test', 'test2', pytest.raises(KeyError)),
+    (None, None, None, pytest.raises(KeyError)),
+    ((), None, None, pytest.raises(KeyError)),
+    ([], None, None, pytest.raises(KeyError))
+])
+
+def test_set_by_func(valid_config, keys, orig_val, expected_val, expected_except):
+    with expected_except:
+        v = valid_config.get(keys)
+        valid_config.set(keys, value=expected_val)
+
+        assert v == orig_val and valid_config.get(keys) != orig_val and valid_config.get(keys) == expected_val
+
+### KEY tests
+
+def test_key_set(valid_config):
+    v = valid_config['test']
+    valid_config['test'] = 'test2'
+
+    assert v == 'test' and valid_config['test'] != 'test' and valid_config['test'] == 'test2'
+
+
+
+
+## GET tests
+
+### FUNC tests
+
+@pytest.mark.parametrize('keys, expected_result, expected_except', [
+    ('test', 'test', does_not_raise()),
+    ('nestedTest', { 'test': 'test' }, does_not_raise()),
+    (('nestedTest', 'test'), 'test', does_not_raise()),
+    (('nestedTest2', 'nested', 'test'), 'test', does_not_raise()),
+    ('get', 'test', does_not_raise()),
+    (None, None, pytest.raises(KeyError)),
+    ((), None, pytest.raises(KeyError)),
+    ([], None, pytest.raises(KeyError))
+])
+
+def test_get_by_func(valid_config, keys, expected_result, expected_except):
+    with expected_except:
+        v = valid_config.get(keys)
+
+        assert v == expected_result
+
+### KEY tests
+
+@pytest.mark.parametrize('keys, expected_result, expected_except', [
+    ('test', 'test', does_not_raise()),
+    ('nestedTest', { 'test': 'test' }, does_not_raise()),
+    (('nestedTest', 'test'), 'test', does_not_raise()),
+    (('nestedTest2', 'nested', 'test'), 'test', does_not_raise()),
+    ('get', 'test', does_not_raise()),
+    (None, None, pytest.raises(KeyError)),
+    ((), None, pytest.raises(KeyError)),
+    ([], None, pytest.raises(KeyError))
+])
+
+def test_get_by_key(valid_config, keys, expected_result, expected_except):
+    with expected_except:
+        if type(keys) == str or type(keys) == type(None):
+            v = valid_config[keys]
+        elif type(keys) == tuple:
+            fk = ()
+
+            if len(keys) > 0:
+                fk = keys[0]
+
+            v = valid_config[fk]
+
+            for k in keys[1:]:
+                v = v[k]
+        elif type(keys) == list:
+            fk = []
+
+            if len(keys) > 0:
+                fk = keys[0]
+
+            v = valid_config[fk]
+
+            for k in keys[1:]:
+                v = v[k]
+        else:
+            assert 1 == 2
+
+        assert v == expected_result
+
+
+
+
+## DELETE tests
+
+### FUNC tests
+
+@pytest.mark.parametrize('keys, expected_except', [
+    ('test', does_not_raise()),
+    (('nestedTest', 'test'), does_not_raise()),
+    (('nestedTest2', 'nested', 'test'), does_not_raise()),
+    ('badDelete', pytest.raises(KeyError)),
+    (None, pytest.raises(KeyError)),
+    ((), pytest.raises(KeyError)),
+    ([], pytest.raises(KeyError))
+])
+
+def test_delete_by_func(valid_config, keys, expected_except):
+    with expected_except:
+        valid_config.delete(keys)
+
+        assert keys not in valid_config
+
+### KEY tests
+
+def test_key_delete(valid_config):
+    del valid_config['test']
+
+    assert 'test' not in valid_config
+
+def test_key_nested_delete(valid_config):
+    del valid_config['nestedTest']['test']
+
     assert 'test' not in valid_config['nestedTest']
```

