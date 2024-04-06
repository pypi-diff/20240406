# Comparing `tmp/unicodedata-reader-0.1.7.tar.gz` & `tmp/unicodedata_reader-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unicodedata-reader-0.1.7.tar", max compression
+gzip compressed data, was "unicodedata_reader-0.2.0.tar", max compression
```

## Comparing `unicodedata-reader-0.1.7.tar` & `unicodedata_reader-0.2.0.tar`

### file list

```diff
@@ -1,16 +1,17 @@
--rw-r--r--   0        0        0    11357 2021-12-05 10:27:55.632115 unicodedata-reader-0.1.7/LICENSE
--rw-r--r--   0        0        0     3120 2021-12-05 10:27:55.632115 unicodedata-reader-0.1.7/README.md
--rw-r--r--   0        0        0      674 2021-12-05 10:27:55.632115 unicodedata-reader-0.1.7/pyproject.toml
--rw-r--r--   0        0        0       88 2021-12-05 10:27:55.632115 unicodedata-reader-0.1.7/unicodedata_reader/__init__.py
--rw-r--r--   0        0        0      988 2021-12-05 10:27:55.632115 unicodedata-reader-0.1.7/unicodedata_reader/__main__.py
--rwxr-xr-x   0        0        0     1310 2021-12-05 10:27:55.632115 unicodedata-reader-0.1.7/unicodedata_reader/bidi_brackets.py
--rw-r--r--   0        0        0     4674 2021-12-05 10:27:55.632115 unicodedata-reader-0.1.7/unicodedata_reader/cli.py
--rwxr-xr-x   0        0        0     4359 2021-12-05 10:27:55.632115 unicodedata-reader-0.1.7/unicodedata_reader/compressor.py
--rwxr-xr-x   0        0        0     1219 2021-12-05 10:27:55.632115 unicodedata-reader-0.1.7/unicodedata_reader/emoji.py
--rw-r--r--   0        0        0    13425 2021-12-05 10:27:55.632115 unicodedata-reader-0.1.7/unicodedata_reader/entry.py
--rwxr-xr-x   0        0        0      557 2021-12-05 10:27:55.632115 unicodedata-reader-0.1.7/unicodedata_reader/general_category.py
--rwxr-xr-x   0        0        0      670 2021-12-05 10:27:55.632115 unicodedata-reader-0.1.7/unicodedata_reader/line_break.py
--rw-r--r--   0        0        0     3623 2021-12-05 10:27:55.632115 unicodedata-reader-0.1.7/unicodedata_reader/reader.py
--rwxr-xr-x   0        0        0      995 2021-12-05 10:27:55.632115 unicodedata-reader-0.1.7/unicodedata_reader/vertical_orientation.py
--rw-r--r--   0        0        0     3978 2021-12-05 10:28:17.803963 unicodedata-reader-0.1.7/setup.py
--rw-r--r--   0        0        0     3766 2021-12-05 10:28:17.804319 unicodedata-reader-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-06 18:07:10.880042 unicodedata_reader-0.2.0/LICENSE
+-rw-r--r--   0        0        0     3120 2024-04-06 18:07:10.880042 unicodedata_reader-0.2.0/README.md
+-rw-r--r--   0        0        0      678 2024-04-06 18:07:10.880042 unicodedata_reader-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      107 2024-04-06 18:07:10.880042 unicodedata_reader-0.2.0/unicodedata_reader/__init__.py
+-rw-r--r--   0        0        0     1101 2024-04-06 18:07:10.880042 unicodedata_reader-0.2.0/unicodedata_reader/__main__.py
+-rwxr-xr-x   0        0        0     1310 2024-04-06 18:07:10.880042 unicodedata_reader-0.2.0/unicodedata_reader/bidi_brackets.py
+-rw-r--r--   0        0        0     4675 2024-04-06 18:07:10.880042 unicodedata_reader-0.2.0/unicodedata_reader/cli.py
+-rwxr-xr-x   0        0        0     4360 2024-04-06 18:07:10.880042 unicodedata_reader-0.2.0/unicodedata_reader/compressor.py
+-rw-r--r--   0        0        0      982 2024-04-06 18:07:10.880042 unicodedata_reader-0.2.0/unicodedata_reader/east_asian_width.py
+-rwxr-xr-x   0        0        0     1220 2024-04-06 18:07:10.880042 unicodedata_reader-0.2.0/unicodedata_reader/emoji.py
+-rw-r--r--   0        0        0    13464 2024-04-06 18:07:10.880042 unicodedata_reader-0.2.0/unicodedata_reader/entry.py
+-rwxr-xr-x   0        0        0      558 2024-04-06 18:07:10.880042 unicodedata_reader-0.2.0/unicodedata_reader/general_category.py
+-rwxr-xr-x   0        0        0      671 2024-04-06 18:07:10.880042 unicodedata_reader-0.2.0/unicodedata_reader/line_break.py
+-rw-r--r--   0        0        0     3806 2024-04-06 18:07:10.880042 unicodedata_reader-0.2.0/unicodedata_reader/reader.py
+-rw-r--r--   0        0        0     2141 2024-04-06 18:07:10.884042 unicodedata_reader-0.2.0/unicodedata_reader/set.py
+-rwxr-xr-x   0        0        0      996 2024-04-06 18:07:10.884042 unicodedata_reader-0.2.0/unicodedata_reader/vertical_orientation.py
+-rw-r--r--   0        0        0     3864 1970-01-01 00:00:00.000000 unicodedata_reader-0.2.0/PKG-INFO
```

### Comparing `unicodedata-reader-0.1.7/LICENSE` & `unicodedata_reader-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `unicodedata-reader-0.1.7/README.md` & `unicodedata_reader-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `unicodedata-reader-0.1.7/pyproject.toml` & `unicodedata_reader-0.2.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "unicodedata-reader"
-version = "0.1.7"
+version = "0.2.0"
 description = ""
 authors = ["Koji Ishii <kojii@chromium.org>"]
 readme = "README.md"
 repository = "https://github.com/kojiishi/unicodedata-reader"
 license = "Apache-2.0"
 
 [tool.poetry.dependencies]
 python = ">=3.8"
-platformdirs = "^2.2.0"
+platformdirs = ">=2.2,<5.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "*"
 pytype = {version = "*", python = "<3.10"}
-tox = "^3.24.4"
-yapf = "^0.31.0"
+tox = "^4.14.2"
+yapf = "^0.40.2"
 
 [tool.poetry.scripts]
 unicodedata-reader = 'unicodedata_reader.__main__:main'
 
 [tool.pytest.ini_options]
 testpaths = "tests"
```

### Comparing `unicodedata-reader-0.1.7/unicodedata_reader/__main__.py` & `unicodedata_reader-0.2.0/unicodedata_reader/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 import pathlib
 import sys
 
 import unicodedata_reader.bidi_brackets as bidi_brackets
+import unicodedata_reader.east_asian_width as ea
 import unicodedata_reader.emoji as emoji
 import unicodedata_reader.general_category as gc
 import unicodedata_reader.line_break as lb
 import unicodedata_reader.vertical_orientation as vo
 
 
 def main():
     args = sys.argv
     sub_commands = {
         'bidi': lambda: bidi_brackets.dump_bidi_brackets(),
+        'ea': lambda: ea.UnicodeEastAsianWidthDataCli().main(),
         'emoji': lambda: emoji.UnicodeEmojiDataCli().main(),
         'gc': lambda: gc.UnicodeGeneralCategoryDataCli().main(),
         'lb': lambda: lb.UnicodeLineBreakDataCli().main(),
         'vo': lambda: vo.UnicodeVerticalOrientationDataCli().main(),
     }
     if len(args) > 1:
         func = sub_commands.get(args[1])
```

### Comparing `unicodedata-reader-0.1.7/unicodedata_reader/bidi_brackets.py` & `unicodedata_reader-0.2.0/unicodedata_reader/bidi_brackets.py`

 * *Files identical despite different names*

### Comparing `unicodedata-reader-0.1.7/unicodedata_reader/cli.py` & `unicodedata_reader-0.2.0/unicodedata_reader/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,14 +69,15 @@
     if verbose <= 1:
         logging.basicConfig(level=logging.INFO)
         return
     logging.basicConfig(level=logging.DEBUG)
 
 
 class UnicodeDataCli(object):
+
     def __init__(self):
         self._parse_args()
 
     def _columns(self) -> Dict[str, Callable[[int, str], Any]]:
         columns = self._core_columns()
         columns = dict(
             itertools.chain({
```

### Comparing `unicodedata-reader-0.1.7/unicodedata_reader/compressor.py` & `unicodedata_reader-0.2.0/unicodedata_reader/compressor.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,14 +18,15 @@
         _logger.addHandler(handler)
         _logger.setLevel(logging.DEBUG if verbose else logging.INFO)
         return
     logging.basicConfig(level=logging.DEBUG)
 
 
 class UnicodeDataCompressor(object):
+
     def __init__(self, entries: UnicodeDataEntries):
         self._entries = entries
 
     @property
     def _bitsize(self) -> int:
         values_for_int = self._entries.values_for_int()
         assert values_for_int
```

### Comparing `unicodedata-reader-0.1.7/unicodedata_reader/emoji.py` & `unicodedata_reader-0.2.0/unicodedata_reader/emoji.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from typing import Callable
 from typing import Dict
 
 from unicodedata_reader import *
 
 
 class UnicodeEmojiDataCli(UnicodeDataCli):
+
     def __init__(self):
         super().__init__()
         self._entries = UnicodeDataReader.default.emoji()
 
     def _emoji_flag_func(self, mask: EmojiType):
         return lambda code, ch: 1 if self._entries.value(code) & mask else 0
```

### Comparing `unicodedata-reader-0.1.7/unicodedata_reader/entry.py` & `unicodedata_reader-0.2.0/unicodedata_reader/entry.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     code = 0
     for byte in c.encode(encoding, 'ignore'):
         code = code * 256 + byte
     return u_hex(code) if code else ''
 
 
 class BidiBrackets(object):
+
     def __init__(self, pair: int, type: str):
         self.pair = pair
         self.type = type
 
     @staticmethod
     def from_values(value):
         assert len(value) == 2
@@ -51,14 +52,17 @@
 
     This class consists of:
     * A range (min and max, inclusive) of Unicode code points.
     * A value for the range.
 
     [Unicode character database]: https://unicode.org/reports/tr44/
     """
+
+    max_code_point = 0x10FFFF
+
     def __init__(self, min: int, max: int, value):
         self.min = min
         self.max = max
         self.value = value
         self.assert_range()
 
     def __eq__(self, other):
@@ -162,14 +166,15 @@
 
 
 class UnicodeDataEntries(object):
     """Represents a [Unicode character database] file,
     or a list of `UnicodeDataEntry`.
     [Unicode character database]: https://unicode.org/reports/tr44/
     """
+
     def __init__(self,
                  entries: Optional[Union[Iterable[UnicodeDataEntry],
                                          Sequence[UnicodeDataEntry]]] = None,
                  name: Optional[str] = None,
                  lines: Optional[Iterable[str]] = None,
                  converter=None):
         self._missing_entries = self._default_missing_entries()
@@ -306,20 +311,22 @@
         for entry in self._entries:
             for code in entry.range():
                 dict[code] = entry.value
         return dict
 
 
 class UnicodeBidiBracketsDataEntries(UnicodeDataEntries):
+
     def _load_lines(self, lines: Iterable[str], converter=None):
         converter = converter or BidiBrackets.from_values
         super()._load_lines(lines, converter=converter)
 
 
 class UnicodeEmojiDataEntries(UnicodeDataEntries):
+
     def _load_lines(self, lines: Iterable[str], converter=None):
         converter = converter or (lambda v: EmojiType[v])
         super()._load_lines(lines, converter=converter)
 
         # `emoji-data.txt` has multiple Emoji properties as separate lists.
         # Unite them to `EmojiType` flags.
         dict = {}
@@ -336,14 +343,15 @@
         pass
 
     def missing_value(self, code: int):
         return EmojiType(0)
 
 
 class UnicodeLineBreakDataEntries(UnicodeDataEntries):
+
     def _load_comment(self, comment: str, start_index: int):
         # Load missing value entries. See the comments in:
         # https://www.unicode.org/Public/UNIDATA/LineBreak.txt
         if start_index == 0:
             m = re.search(r'\sdefault to "([A-Z]{2})":', comment)
             if m:
                 self._current_missing_value = m.group(1)
@@ -358,20 +366,22 @@
                 self._missing_entries.append(
                     UnicodeDataEntry(min, max, self._current_missing_value))
                 return
         super()._load_comment(comment, start_index)
 
 
 class UnicodeScriptExtensionsDataEntries(UnicodeDataEntries):
+
     def _load_lines(self, lines: Iterable[str], converter=None):
         converter = converter or (lambda v: v.split())
         super()._load_lines(lines, converter=converter)
 
 
 class UnicodeVerticalOrientationDataEntries(UnicodeDataEntries):
+
     def _load_comment(self, comment: str, start_index: int):
         # Load missing value entries. See the comments in:
         # https://www.unicode.org/Public/UNIDATA/VerticalOrientation.txt
         if start_index == 0:
             m = re.search(r'\sU\+([0-9A-F]+)(\.\.U\+([0-9A-F]+))?$', comment)
             if m:
                 _logger.debug('Missing entry: %s', comment)
```

### Comparing `unicodedata-reader-0.1.7/unicodedata_reader/general_category.py` & `unicodedata_reader-0.2.0/unicodedata_reader/general_category.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from typing import Callable
 from typing import Dict
 
 from unicodedata_reader import *
 
 
 class UnicodeGeneralCategoryDataCli(UnicodeDataCli):
+
     def __init__(self):
         super().__init__()
         self._entries = UnicodeDataReader.default.general_category()
 
     def _core_columns(self) -> Dict[str, Callable[[int, str], Any]]:
         return {
             'GC': lambda code, ch: self._entries.value(code),
```

### Comparing `unicodedata-reader-0.1.7/unicodedata_reader/line_break.py` & `unicodedata_reader-0.2.0/unicodedata_reader/line_break.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from typing import Callable
 from typing import Dict
 
 from unicodedata_reader import *
 
 
 class UnicodeLineBreakDataCli(UnicodeDataCli):
+
     def __init__(self):
         super().__init__()
         self._entries = UnicodeDataReader.default.line_break()
 
     def _core_columns(self) -> Dict[str, Callable[[int, str], Any]]:
         return {
             'LB': lambda code, ch: self._entries.value(code),
```

### Comparing `unicodedata-reader-0.1.7/unicodedata_reader/reader.py` & `unicodedata_reader-0.2.0/unicodedata_reader/reader.py`

 * *Files 7% similar despite different names*

```diff
@@ -29,14 +29,19 @@
         return UnicodeBidiBracketsDataEntries(name=name, lines=lines)
 
     def blocks(self) -> UnicodeDataEntries:
         name = 'Blocks'
         lines = self.read_lines(name)
         return UnicodeDataEntries(name=name, lines=lines)
 
+    def east_asian_width(self) -> UnicodeDataEntries:
+        name = 'EastAsianWidth'
+        lines = self.read_lines(name)
+        return UnicodeDataEntries(name=name, lines=lines)
+
     def emoji(self) -> UnicodeDataEntries:
         lines = self.read_lines('emoji/emoji-data')
         return UnicodeEmojiDataEntries(name='Emoji', lines=lines)
 
     def general_category(self) -> UnicodeDataEntries:
         lines = self.read_lines('extracted/DerivedGeneralCategory')
         entries = UnicodeDataEntries(name='GeneralCategory', lines=lines)
```

### Comparing `unicodedata-reader-0.1.7/unicodedata_reader/vertical_orientation.py` & `unicodedata_reader-0.2.0/unicodedata_reader/vertical_orientation.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from typing import Callable
 from typing import Dict
 
 from unicodedata_reader import *
 
 
 class UnicodeVerticalOrientationDataCli(UnicodeDataCli):
+
     def __init__(self):
         super().__init__()
         self._entries = UnicodeDataReader.default.vertical_orientation()
 
     def _core_columns(self) -> Dict[str, Callable[[int, str], Any]]:
         return {
             'VO': lambda code, ch: self._entries.value(code),
```

### Comparing `unicodedata-reader-0.1.7/PKG-INFO` & `unicodedata_reader-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: unicodedata-reader
-Version: 0.1.7
+Version: 0.2.0
 Summary: 
 Home-page: https://github.com/kojiishi/unicodedata-reader
 License: Apache-2.0
 Author: Koji Ishii
 Author-email: kojii@chromium.org
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: platformdirs (>=2.2.0,<3.0.0)
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: platformdirs (>=2.2,<5.0)
 Project-URL: Repository, https://github.com/kojiishi/unicodedata-reader
 Description-Content-Type: text/markdown
 
 [![CI](https://github.com/kojiishi/unicodedata-reader/actions/workflows/ci.yml/badge.svg)](https://github.com/kojiishi/unicodedata-reader/actions/workflows/ci.yml)
 [![PyPI](https://img.shields.io/pypi/v/unicodedata-reader.svg)](https://pypi.org/project/unicodedata-reader/)
 [![Dependencies](https://badgen.net/github/dependabot/kojiishi/unicodedata-reader)](https://github.com/kojiishi/unicodedata-reader/network/updates)
```

