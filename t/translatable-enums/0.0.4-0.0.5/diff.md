# Comparing `tmp/translatable_enums-0.0.4.tar.gz` & `tmp/translatable_enums-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "translatable_enums-0.0.4.tar", max compression
+gzip compressed data, was "translatable_enums-0.0.5.tar", max compression
```

## Comparing `translatable_enums-0.0.4.tar` & `translatable_enums-0.0.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0      539 2024-02-11 14:43:02.567345 translatable_enums-0.0.4/i18n/__init__.py
--rw-r--r--   0        0        0     2022 2024-02-11 15:20:36.424772 translatable_enums-0.0.4/i18n/__main__.py
--rw-r--r--   0        0        0      484 2024-02-11 18:24:31.975786 translatable_enums-0.0.4/i18n/enums.py
--rw-r--r--   0        0        0      218 2024-02-12 11:26:03.772662 translatable_enums-0.0.4/i18n/settings.py
--rw-r--r--   0        0        0      338 2024-02-11 12:08:21.511566 translatable_enums-0.0.4/i18n/tools.py
--rw-r--r--   0        0        0      169 2024-02-12 13:48:08.322619 translatable_enums-0.0.4/i18n/types.py
--rw-r--r--   0        0        0        0 2024-02-10 10:52:36.822551 translatable_enums-0.0.4/i18n/utils/__init__.py
--rw-r--r--   0        0        0       94 2024-02-11 10:25:57.928146 translatable_enums-0.0.4/i18n/utils/clsutils/__init__.py
--rw-r--r--   0        0        0      391 2024-02-11 10:25:57.917138 translatable_enums-0.0.4/i18n/utils/clsutils/generators.py
--rw-r--r--   0        0        0      222 2024-02-11 14:13:35.378888 translatable_enums-0.0.4/i18n/utils/gettext/__init__.py
--rw-r--r--   0        0        0      292 2024-02-11 14:13:35.390105 translatable_enums-0.0.4/i18n/utils/gettext/contexts.py
--rw-r--r--   0        0        0      421 2024-04-04 18:32:32.879535 translatable_enums-0.0.4/i18n/utils/gettext/shortcuts.py
--rw-r--r--   0        0        0       73 2024-02-11 15:08:51.918492 translatable_enums-0.0.4/i18n/utils/imputils/__init__.py
--rw-r--r--   0        0        0      842 2024-03-28 11:02:20.867491 translatable_enums-0.0.4/i18n/utils/imputils/utils.py
--rw-r--r--   0        0        0      115 2024-02-11 11:46:47.265559 translatable_enums-0.0.4/i18n/utils/potfile/__init__.py
--rw-r--r--   0        0        0      353 2024-02-11 11:33:58.286670 translatable_enums-0.0.4/i18n/utils/potfile/constants.py
--rw-r--r--   0        0        0     2030 2024-02-12 13:39:33.781025 translatable_enums-0.0.4/i18n/utils/potfile/potfile.py
--rw-r--r--   0        0        0      103 2024-02-12 11:26:03.765660 translatable_enums-0.0.4/i18n/utils/potfile/types.py
--rw-r--r--   0        0        0     1090 2024-02-10 10:48:35.222832 translatable_enums-0.0.4/LICENSE
--rw-r--r--   0        0        0      781 2024-04-04 18:36:39.836085 translatable_enums-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     2591 2024-02-12 14:07:25.708666 translatable_enums-0.0.4/README.md
--rw-r--r--   0        0        0     3279 1970-01-01 00:00:00.000000 translatable_enums-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      485 2024-04-06 13:09:19.657292 translatable_enums-0.0.5/i18n/__init__.py
+-rw-r--r--   0        0        0     1916 2024-04-06 13:09:19.835977 translatable_enums-0.0.5/i18n/__main__.py
+-rw-r--r--   0        0        0      442 2024-04-06 13:09:19.740810 translatable_enums-0.0.5/i18n/enums.py
+-rw-r--r--   0        0        0      215 2024-04-06 13:14:45.304159 translatable_enums-0.0.5/i18n/settings.py
+-rw-r--r--   0        0        0      404 2024-04-06 13:09:19.760304 translatable_enums-0.0.5/i18n/tools.py
+-rw-r--r--   0        0        0      282 2024-04-06 12:57:01.911526 translatable_enums-0.0.5/i18n/types.py
+-rw-r--r--   0        0        0        0 2024-02-10 10:52:36.822551 translatable_enums-0.0.5/i18n/utils/__init__.py
+-rw-r--r--   0        0        0       94 2024-04-06 13:09:19.874235 translatable_enums-0.0.5/i18n/utils/clsutils/__init__.py
+-rw-r--r--   0        0        0      391 2024-02-11 10:25:57.917138 translatable_enums-0.0.5/i18n/utils/clsutils/generators.py
+-rw-r--r--   0        0        0      248 2024-04-06 13:09:19.948795 translatable_enums-0.0.5/i18n/utils/gettext/__init__.py
+-rw-r--r--   0        0        0      277 2024-04-06 13:09:19.982037 translatable_enums-0.0.5/i18n/utils/gettext/contexts.py
+-rw-r--r--   0        0        0      495 2024-04-06 13:09:19.698542 translatable_enums-0.0.5/i18n/utils/gettext/shortcuts.py
+-rw-r--r--   0        0        0       65 2024-04-06 13:09:19.709541 translatable_enums-0.0.5/i18n/utils/imputils/__init__.py
+-rw-r--r--   0        0        0      842 2024-04-06 13:16:05.556430 translatable_enums-0.0.5/i18n/utils/imputils/utils.py
+-rw-r--r--   0        0        0      102 2024-04-06 13:09:19.754693 translatable_enums-0.0.5/i18n/utils/potfile/__init__.py
+-rw-r--r--   0        0        0      353 2024-04-06 13:09:19.769710 translatable_enums-0.0.5/i18n/utils/potfile/constants.py
+-rw-r--r--   0        0        0     2021 2024-04-06 13:09:19.864235 translatable_enums-0.0.5/i18n/utils/potfile/potfile.py
+-rw-r--r--   0        0        0      103 2024-04-06 13:09:19.778730 translatable_enums-0.0.5/i18n/utils/potfile/types.py
+-rw-r--r--   0        0        0     1090 2024-02-10 10:48:35.222832 translatable_enums-0.0.5/LICENSE
+-rw-r--r--   0        0        0      800 2024-04-06 13:08:10.690546 translatable_enums-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     2795 2024-04-06 13:19:21.424481 translatable_enums-0.0.5/README.md
+-rw-r--r--   0        0        0     3478 1970-01-01 00:00:00.000000 translatable_enums-0.0.5/PKG-INFO
```

### Comparing `translatable_enums-0.0.4/i18n/utils/imputils/utils.py` & `translatable_enums-0.0.5/i18n/utils/imputils/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,23 +4,23 @@
 from functools import cache
 from types import ModuleType
 
 
 @cache
 def import_module(path: str) -> ModuleType:
     if os.path.isdir(path):
-        path = os.path.join(path, '__main__.py')
+        path = os.path.join(path, "__main__.py")
 
     directory = os.path.dirname(path)
     sys.path.append(directory)
     try:
         if not os.path.exists(path):
-            raise ImportError(f'Module not found at: {path}')
+            raise ImportError(f"Module not found at: {path}")
         *_, filename = os.path.split(path)
-        spec = importlib.util.spec_from_file_location(filename.replace('.py', ''), path)
+        spec = importlib.util.spec_from_file_location(filename.replace(".py", ""), path)
         imported_module = importlib.util.module_from_spec(spec)
         spec.loader.exec_module(imported_module)
         return imported_module
     except Exception:
-        raise ImportError(f'Failed to import module: {path}')
+        raise ImportError(f"Failed to import module: {path}")
     finally:
         sys.path.remove(directory)
```

### Comparing `translatable_enums-0.0.4/i18n/utils/potfile/potfile.py` & `translatable_enums-0.0.5/i18n/utils/potfile/potfile.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,63 +1,59 @@
+from io import TextIOWrapper
 from typing import TextIO
 
-from .types import (
-    TextFileMode
-)
-from .constants import (
-    TEMPLATES,
-    MSGID_REGEX
-)
+from .types import TextFileMode
+from .constants import MSGID_REGEX
 
 
 class POTFile:
     def __init__(
-            self,
-            file: str | TextIO,
-            mode: TextFileMode = 'r',
-            template: str | None = None,
-            encoding: str | None = None
+        self,
+        file: str | TextIO,
+        mode: TextFileMode = "r",
+        template: str | None = None,
+        encoding: str | None = None,
     ):
         self._mode = mode
         self._encoding = encoding
         self._template = template
         self._file: TextIO = self._open_file(file)
         self._cached_keys = set()
 
-        if self._mode == 'w':
+        if self._mode == "w":
             self._write_template()
 
-        if self._mode in {'a', 'r'}:
+        if self._mode in {"a", "r"}:
             self._load_keys()
 
     def _open_file(self, file_or_path: str | TextIO) -> TextIO:
         if isinstance(file_or_path, str):
             return open(file_or_path, encoding=self._encoding, mode=self._mode)
-        elif isinstance(file_or_path, TextIO):
+        elif isinstance(file_or_path, TextIO | TextIOWrapper):
             return file_or_path
-        raise TypeError(f'Unsupported type of file parameter: {file_or_path}')
+        raise TypeError(f"Unsupported type of file parameter: {file_or_path}")
 
     def _write_template(self):
         if self._template:
             self._file.write(self._template)
 
     def _load_keys(self):
         for line in self._file:
             if MSGID_REGEX.match(line):
                 result = MSGID_REGEX.findall(line)[0]
                 self._cached_keys.add(result)
 
     def write(self, key: str, comment: str = None, check_key: bool = True):
         if check_key and key in self._cached_keys:
-            raise KeyError(f'Duplicate key: {key}')
+            raise KeyError(f"Duplicate key: {key}")
 
         self._cached_keys.add(key)
         text = f'msgid "{key}"\nmsgstr ""\n\n'
         if comment:
-            text = f'# {comment}\n{text}'
+            text = f"# {comment}\n{text}"
         self._file.write(text)
 
     @property
     def keys(self):
         yield from self
 
     def close(self):
```

### Comparing `translatable_enums-0.0.4/LICENSE` & `translatable_enums-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `translatable_enums-0.0.4/pyproject.toml` & `translatable_enums-0.0.5/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "translatable-enums"
-version = "0.0.4"
+version = "0.0.5"
 description = "Translatable-Enums is a i18n tool which uses built-in Enums as an convenient way to store translation keys."
 authors = ["CrazyProger1 <crazyproger1@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [
     { include = "i18n" },
 ]
@@ -17,12 +17,13 @@
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.0.0"
 ruff = "^0.2.1"
 mypy = "^1.8.0"
 coverage = "^7.4.1"
+black = "^24.3.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `translatable_enums-0.0.4/README.md` & `translatable_enums-0.0.5/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 <img src="https://github.com/CrazyProger1/Translatable-Enums/blob/master/resources/images/logo.png" alt="Lib logo">
 </p>
 
 <p align="center">
 <a href="https://github.com/CrazyProger1/Translatable-Enums/blob/master/LICENSE"><img alt="GitHub" src="https://img.shields.io/github/license/CrazyProger1/Translatable-Enums"></a>
 <a href="https://github.com/CrazyProger1/Translatable-Enums/releases/latest"><img alt="GitHub release (latest by date)" src="https://img.shields.io/github/v/release/CrazyProger1/Translatable-Enums"></a>
 <a href="https://pypi.org/project/translatable-enums/"><img alt="PyPI - Downloads" src="https://img.shields.io/pypi/dm/translatable-enums"></a>
-<img src="https://img.shields.io/badge/coverage-99%25-brightgreen" alt="Coverage"/>
+<img src="https://img.shields.io/badge/coverage-100%25-brightgreen" alt="Coverage"/>
+<a href="https://github.com/psf/black"><img src="https://img.shields.io/badge/code%20style-black-000000.svg" alt="Code Style"></a>
 </p>
 
 Translatable-Enums is an i18n tool which uses built-in Enums as a convenient way to store translation keys.
 
 ## Key-Features
 
 - No dependencies except the Python's standard library. Based on built-in enums & gettext
@@ -89,15 +90,19 @@
 msgid "Hello,"
 msgstr ""
 
 msgid "World!"
 msgstr ""
 ```
 
+### Examples
+
+See [/examples](examples/) for more examples.
+
 ## Status
 
-``0.0.3`` - RELEASED
+```0.0.5``` - **RELEASED**
 
 ## Licence
 
 Translatable-Enums is released under the MIT License. See the
 bundled [LICENSE](https://github.com/CrazyProger1/Translatable-Enums/blob/master/LICENSE) file for details.
```

#### html2text {}

```diff
@@ -1,10 +1,11 @@
 # Translatable-Enums
                                   [Lib logo]
-     _[_G_i_t_H_u_b_]_[_G_i_t_H_u_b_ _r_e_l_e_a_s_e_ _(_l_a_t_e_s_t_ _b_y_ _d_a_t_e_)_]_[_P_y_P_I_ _-_ _D_o_w_n_l_o_a_d_s_][Coverage]
+  _[_G_i_t_H_u_b_]_[_G_i_t_H_u_b_ _r_e_l_e_a_s_e_ _(_l_a_t_e_s_t_ _b_y_ _d_a_t_e_)_]_[_P_y_P_I_ _-_ _D_o_w_n_l_o_a_d_s_][Coverage]_[_C_o_d_e
+                                    _S_t_y_l_e_]
 Translatable-Enums is an i18n tool which uses built-in Enums as a convenient
 way to store translation keys. ## Key-Features - No dependencies except the
 Python's standard library. Based on built-in enums & gettext - Powerful utility
 for extracting translation-keys - Easy-to-Use ## Installation You can use PIP:
 ```shell pip install translatable-enums ``` Or Poetry: ```shell poetry add
 translatable-enums ``` ## Getting-Started ```python from i18n import
 ( TranslatableEnum, set_domain, set_language ) class Messages
@@ -16,11 +17,12 @@
 (Messages.HELLO.language('uk'), Messages.WORLD.language('en')) # ÐÑÐ¸Ð²ÑÑ,
 World! ``` ### Extraction-Tools To extract the translation-keys from
 application: ```shell python -m i18n main.py application.pot ``` You will
 obtain a [.pot](https://pofile.net/) file like this: ```potfile msgid "" msgstr
 "" "Project-Id-Version: \n" "POT-Creation-Date: \n" "Last-Translator: \n"
 "Language-Team: \n" "Language: \n" "MIME-Version: \n" "Content-Type: text/
 plain; charset=utf-8\n" "Content-Transfer-Encoding: 8bit\n" msgid "Hello,"
-msgstr "" msgid "World!" msgstr "" ``` ## Status ``0.0.3`` - RELEASED ##
-Licence Translatable-Enums is released under the MIT License. See the bundled
-[LICENSE](https://github.com/CrazyProger1/Translatable-Enums/blob/master/
-LICENSE) file for details.
+msgstr "" msgid "World!" msgstr "" ``` ### Examples See [/examples](examples/
+) for more examples. ## Status ```0.0.5``` - **RELEASED** ## Licence
+Translatable-Enums is released under the MIT License. See the bundled [LICENSE]
+(https://github.com/CrazyProger1/Translatable-Enums/blob/master/LICENSE) file
+for details.
```

### Comparing `translatable_enums-0.0.4/PKG-INFO` & `translatable_enums-0.0.5/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: translatable-enums
-Version: 0.0.4
+Version: 0.0.5
 Summary: Translatable-Enums is a i18n tool which uses built-in Enums as an convenient way to store translation keys.
 Home-page: https://github.com/CrazyProger1/Translatable-Enums
 License: MIT
 Author: CrazyProger1
 Author-email: crazyproger1@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -22,15 +22,16 @@
 <img src="https://github.com/CrazyProger1/Translatable-Enums/blob/master/resources/images/logo.png" alt="Lib logo">
 </p>
 
 <p align="center">
 <a href="https://github.com/CrazyProger1/Translatable-Enums/blob/master/LICENSE"><img alt="GitHub" src="https://img.shields.io/github/license/CrazyProger1/Translatable-Enums"></a>
 <a href="https://github.com/CrazyProger1/Translatable-Enums/releases/latest"><img alt="GitHub release (latest by date)" src="https://img.shields.io/github/v/release/CrazyProger1/Translatable-Enums"></a>
 <a href="https://pypi.org/project/translatable-enums/"><img alt="PyPI - Downloads" src="https://img.shields.io/pypi/dm/translatable-enums"></a>
-<img src="https://img.shields.io/badge/coverage-99%25-brightgreen" alt="Coverage"/>
+<img src="https://img.shields.io/badge/coverage-100%25-brightgreen" alt="Coverage"/>
+<a href="https://github.com/psf/black"><img src="https://img.shields.io/badge/code%20style-black-000000.svg" alt="Code Style"></a>
 </p>
 
 Translatable-Enums is an i18n tool which uses built-in Enums as a convenient way to store translation keys.
 
 ## Key-Features
 
 - No dependencies except the Python's standard library. Based on built-in enums & gettext
@@ -107,15 +108,19 @@
 msgid "Hello,"
 msgstr ""
 
 msgid "World!"
 msgstr ""
 ```
 
+### Examples
+
+See [/examples](examples/) for more examples.
+
 ## Status
 
-``0.0.3`` - RELEASED
+```0.0.5``` - **RELEASED**
 
 ## Licence
 
 Translatable-Enums is released under the MIT License. See the
 bundled [LICENSE](https://github.com/CrazyProger1/Translatable-Enums/blob/master/LICENSE) file for details.
```

