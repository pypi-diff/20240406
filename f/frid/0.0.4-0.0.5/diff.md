# Comparing `tmp/frid-0.0.4.tar.gz` & `tmp/frid-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frid-0.0.4.tar", last modified: Thu Apr  4 22:01:05 2024, max compression
+gzip compressed data, was "frid-0.0.5.tar", last modified: Sat Apr  6 00:53:53 2024, max compression
```

## Comparing `frid-0.0.4.tar` & `frid-0.0.5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 hanhua    (1000) hanhua    (1000)        0 2024-04-04 22:01:05.546019 frid-0.0.4/
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)     1077 2024-03-19 21:36:16.000000 frid-0.0.4/LICENSE
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)     1764 2024-04-04 22:01:05.546019 frid-0.0.4/PKG-INFO
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)     1235 2024-03-30 02:09:52.000000 frid-0.0.4/README.md
-drwxr-xr-x   0 hanhua    (1000) hanhua    (1000)        0 2024-04-04 22:01:05.546019 frid-0.0.4/frid/
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)      473 2024-04-04 14:54:45.000000 frid-0.0.4/frid/__init__.py
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)    23981 2024-03-29 23:28:02.000000 frid-0.0.4/frid/__main__.py
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)     1516 2024-04-04 18:04:22.000000 frid-0.0.4/frid/autils.py
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)     3828 2024-03-29 23:28:02.000000 frid-0.0.4/frid/chrono.py
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)    12841 2024-03-29 23:28:02.000000 frid-0.0.4/frid/dumper.py
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)     2597 2024-04-02 02:49:42.000000 frid-0.0.4/frid/errors.py
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)     7762 2024-04-03 22:34:38.000000 frid-0.0.4/frid/guards.py
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)     8503 2024-04-02 17:42:49.000000 frid-0.0.4/frid/helper.py
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)    21302 2024-04-01 15:36:11.000000 frid-0.0.4/frid/loader.py
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)     1514 2024-03-29 23:28:02.000000 frid-0.0.4/frid/pretty.py
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)    10833 2024-03-29 23:28:02.000000 frid-0.0.4/frid/strops.py
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)     2082 2024-04-01 15:53:05.000000 frid-0.0.4/frid/typing.py
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)    11661 2024-04-04 21:30:27.000000 frid-0.0.4/frid/webapp.py
-drwxr-xr-x   0 hanhua    (1000) hanhua    (1000)        0 2024-04-04 22:01:05.546019 frid-0.0.4/frid.egg-info/
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)     1764 2024-04-04 22:01:05.000000 frid-0.0.4/frid.egg-info/PKG-INFO
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)      343 2024-04-04 22:01:05.000000 frid-0.0.4/frid.egg-info/SOURCES.txt
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)        1 2024-04-04 22:01:05.000000 frid-0.0.4/frid.egg-info/dependency_links.txt
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)        5 2024-04-04 22:01:05.000000 frid-0.0.4/frid.egg-info/top_level.txt
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)      599 2024-04-04 21:56:55.000000 frid-0.0.4/pyproject.toml
--rw-r--r--   0 hanhua    (1000) hanhua    (1000)       38 2024-04-04 22:01:05.546019 frid-0.0.4/setup.cfg
+drwxr-xr-x   0 hanhua    (1000) hanhua    (1000)        0 2024-04-06 00:53:52.998498 frid-0.0.5/
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)     1077 2024-03-19 21:36:16.000000 frid-0.0.5/LICENSE
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)     1764 2024-04-06 00:53:52.998498 frid-0.0.5/PKG-INFO
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)     1235 2024-03-30 02:09:52.000000 frid-0.0.5/README.md
+drwxr-xr-x   0 hanhua    (1000) hanhua    (1000)        0 2024-04-06 00:53:52.998498 frid-0.0.5/frid/
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)      627 2024-04-05 23:01:29.000000 frid-0.0.5/frid/__init__.py
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)    24357 2024-04-05 19:29:01.000000 frid-0.0.5/frid/__main__.py
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)     1516 2024-04-04 18:04:22.000000 frid-0.0.5/frid/autils.py
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)     3828 2024-03-29 23:28:02.000000 frid-0.0.5/frid/chrono.py
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)    16063 2024-04-05 19:05:09.000000 frid-0.0.5/frid/dumper.py
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)     2597 2024-04-02 02:49:42.000000 frid-0.0.5/frid/errors.py
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)     8489 2024-04-06 00:48:32.000000 frid-0.0.5/frid/guards.py
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)     8627 2024-04-05 18:00:29.000000 frid-0.0.5/frid/helper.py
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)    22617 2024-04-05 19:23:00.000000 frid-0.0.5/frid/loader.py
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)     1514 2024-03-29 23:28:02.000000 frid-0.0.5/frid/pretty.py
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)    10833 2024-03-29 23:28:02.000000 frid-0.0.5/frid/strops.py
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)     2288 2024-04-05 19:32:20.000000 frid-0.0.5/frid/typing.py
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)    11661 2024-04-04 21:30:27.000000 frid-0.0.5/frid/webapp.py
+drwxr-xr-x   0 hanhua    (1000) hanhua    (1000)        0 2024-04-06 00:53:52.998498 frid-0.0.5/frid.egg-info/
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)     1764 2024-04-06 00:53:52.000000 frid-0.0.5/frid.egg-info/PKG-INFO
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)      343 2024-04-06 00:53:52.000000 frid-0.0.5/frid.egg-info/SOURCES.txt
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)        1 2024-04-06 00:53:52.000000 frid-0.0.5/frid.egg-info/dependency_links.txt
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)        5 2024-04-06 00:53:52.000000 frid-0.0.5/frid.egg-info/top_level.txt
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)      599 2024-04-06 00:53:35.000000 frid-0.0.5/pyproject.toml
+-rw-r--r--   0 hanhua    (1000) hanhua    (1000)       38 2024-04-06 00:53:52.998498 frid-0.0.5/setup.cfg
```

### Comparing `frid-0.0.4/LICENSE` & `frid-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `frid-0.0.4/PKG-INFO` & `frid-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frid
-Version: 0.0.4
+Version: 0.0.5
 Summary: Flexibly Represented Interactive Data
 Author-email: Hanhua Feng <han.hua.feng@askherefirst.com>
 Project-URL: Homepage, https://github.com/Ask-Here-First/ahf-generic
 Project-URL: Issues, https://github.com/Ask-Here-First/ahf-generic/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `frid-0.0.4/README.md` & `frid-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `frid-0.0.4/frid/__main__.py` & `frid-0.0.5/frid/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -299,15 +299,19 @@
         "..YQ..": b"a", "..YWI.": b"ab",    "..YWJj": b"abc",
         # List
         "[3, [4, 6], abc, [\"\"], [[[]]]]": [3,[4,6],"abc",[''],[[[]]]],
         "[3, [4, 6], abc , [,], [[[]]],  ] ": [3,[4,6],"abc",[''],[[[]]]],
         # Dict
         "{a.b: c, _: \"[]\", d+e-f: g@h}": {'a.b': "c", '_': "[]", 'd+e-f': "g@h"},
         "{a.b: c, _: '[]', d+e-f: g@h  , }": {'a.b': "c", '_': "[]", 'd+e-f': "g@h"},
-        # "{a}": {'a':"a"}, # TODO: decide what to do for set-like
+        "{: \"\"}": {'': ''}, "{:}": {'': ''}, "{: a}": {'': "a"}, "{:a}": {'': "a"},
+        # Set: Python caveats: True == 1 and False == 0; also
+        "{a}": {'a'}, "{3}": {3}, "{+}": {True}, "{-}": {False}, "{.}": {None},
+        # Can't set multi value set, since set is not following insert ordering
+        "{0,1,2,.}": (lambda x: x == {0, 1, 2, None}),
 
         # "()": (''), "(a>3)": LionExprStub('a>3'),
         # "(([{()}]))": LionExprStub("([{()}])"),
         # "(x in [a,b,c])": LionExprStub("x in [a,b,c]"),
         # "(x in '([{\\'\"\\\"')": LionExprStub("x in '([{\\'\"\\\"'"),
         # TODO: do we support non-string keys"{.:+}": {None: True}
     }
@@ -316,14 +320,15 @@
         for i, (s, t) in enumerate(cases.items()):
             try:
                 v = load_from_str(s, json_level=json_level)
                 if callable(t):
                     self.assertTrue(t(v), f"[{i}] {s} ==> {t} ({json_level=})")
                     continue
                 self.assertEqual(t, v, f"[{i}] {s} ==> {t} ({json_level=})")
+                assert t is not ...
                 if t == prev_value:
                     continue
                 self.assertEqual(s, dump_into_str(t, json_level=json_level),
                                 f"[{i}] {s} <== {t} ({json_level=})")
             except Exception:
                 print(f"\nError @ [{i}] {s} <=> {t} ({json_level=})", file=sys.stderr)
                 raise
@@ -471,14 +476,16 @@
         "I'm here", "back`ticks`", "a\\ b ", " c(d)", "Come, here",
         "'No ending quote", "'''Mismatched end quote' '", "'wrong quotes`",
         "'\\", "'\\x2", "'\\x3'", "'\\x9k'", "'\\u37'", "'\\xyz'", "'\\U03'",
         # List
         "[1,", "[}",
         # Dict
         "{,}", "{a:3,,}", "{)", "{a:1, a:2}", "{3a:3}", "{3: 4}",
+        # Set
+        "{3, a:}", "{b:3, +}"
         # Expr
         "(", "([})", "((())",
     ]
     def test_negative_load(self):
         # print(f"Running {len(positive_testcases)} negative testcases...")
         for i, k in enumerate(self.negative_load_cases):
             with self.assertRaises(ParseError, msg=f"[{i}]: {k}"):
```

### Comparing `frid-0.0.4/frid/autils.py` & `frid-0.0.5/frid/autils.py`

 * *Files identical despite different names*

### Comparing `frid-0.0.4/frid/chrono.py` & `frid-0.0.5/frid/chrono.py`

 * *Files identical despite different names*

### Comparing `frid-0.0.4/frid/dumper.py` & `frid-0.0.5/frid/dumper.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import math, base64
-from collections.abc import Callable, Iterable, Mapping
+from collections.abc import Callable, Iterable, Mapping, Sequence, Set
 from typing import Any, Literal, TextIO
 
 from .typing import BlobTypes, FridMixin, FridValue, StrKeyMap
-from .chrono import DateTypes, strfr_datetime
-from .guards import is_frid_identifier, is_frid_quote_free
+from .chrono import DateTypes, strfr_datetime, timeonly, datetime, dateonly
+from .guards import is_frid_identifier, is_frid_quote_free, is_list_like
 from .pretty import PPToTextIOMixin, PrettyPrint, PPTokenType, PPToStringMixin
 from .strops import StringEscapeEncode
 
 JSON_QUOTED_KEYSET = (
     'true', 'false', 'null',
 )
 JSON1_ESCAPE_PAIRS = "\nn\tt\rr\ff\vv\bb"
@@ -60,19 +60,19 @@
             self.se_encoder = StringEscapeEncode(pairs, '\\')
         else:
             self.se_encoder = StringEscapeEncode(pairs, '\\', hex_prefix)
 
     def print(self, token: str, ttype: PPTokenType, /):
         """Default token print behavior:
         - Do not show optional separator.
-        - Add a space after the required separator.
+        - Add a space after the required seqarator ',:'.
         """
         if ttype not in (PPTokenType.OPT_0, PPTokenType.OPT_1):
             self._print(token)
-        if ttype in (PPTokenType.SEP_0, PPTokenType.SEP_1):
+        if ttype in (PPTokenType.SEP_0, PPTokenType.SEP_1) and token in ':,':
             self._print(' ')
 
     def real_to_str(self, data: int|float, path: str, /) -> str:
         """Convert an integer or real number to string."""
         if isinstance(data, int):
             return str(data)
         if self.json_level == 5:
@@ -183,15 +183,18 @@
 
     def print_naked_list(self, data: Iterable[FridValue], path: str="", /, sep: str=','):
         """Prints a list/array to the stream without opening and closing delimiters."""
         non_empty = False  # Use this flag in case bool(data) data not work
         for i, x in enumerate(data):
             if i > 0:
                 self.print(sep[0], PPTokenType.SEP_0)
-            self.print_frid_value(x, path + '[' + str(i) + ']')
+            if x == '':
+                self.print('""', PPTokenType.ENTRY)  # Force quoted string in list
+            else:
+                self.print_frid_value(x, path + '[' + str(i) + ']')
             non_empty = True
         if non_empty and self.json_level in (0, 5):
             self.print(sep[0], PPTokenType.OPT_0)
 
     def _is_unquoted_key(self, key: str):
         """Checks if the key does not need to be quoted"""
         if self.ascii_only and not key.isascii():
@@ -210,26 +213,29 @@
     def print_naked_dict(self, data: StrKeyMap, path: str="", /, sep: str=',:'):
         """Prints a map to the stream without opening and closing delimiters."""
         for i, (k, v) in enumerate(data.items()):
             if i > 0:
                 self.print(sep[0], PPTokenType.SEP_0)
             if not isinstance(k, str):
                 raise ValueError(f"Key is not a string: {k}")
-            if self._is_unquoted_key(k):
-                self.print(k, PPTokenType.LABEL)
-            else:
-                self.print_quoted_str(k, path, as_key=True)
+            # Empty key with non-... value we can omit the key (i.e., unquoted)
+            if k != '' or v is ...:
+                if self._is_unquoted_key(k):
+                    self.print(k, PPTokenType.LABEL)
+                else:
+                    self.print_quoted_str(k, path, as_key=True)
+                if v is ...:  # If the value is ..., print only key without colon
+                    continue
             self.print(sep[1], PPTokenType.SEP_1)
             self.print_frid_value(v, path)
         if data and self.json_level in (0, 5):
             self.print(sep[0], PPTokenType.OPT_0)
 
-    def print_frid_mixin(self, data: FridMixin, path: str, /):
-        """Print any Frid mixin types."""
-        (name, args, kwas) = data.frid_repr()
+    def print_named_args(self, name: str, args: Sequence[FridValue],
+                         kwas: Mapping[str,FridValue], path: str, /):
         path = path + '(' + name + ')'
         if not self.json_level:
             assert is_frid_identifier(name)
             self.print(name, PPTokenType.ENTRY)
             self.print('(', PPTokenType.START)
             self.print_naked_list(args, path, ',')
             self.print(',', PPTokenType.SEP_0)
@@ -250,25 +256,35 @@
             self.print(']', PPTokenType.CLOSE)
         else:
             self.print_quoted_str(self.escape_seq + name, path)
         if kwas:
             self.print_naked_dict(kwas)
             self.print('}', PPTokenType.CLOSE)
 
+    def print_frid_mixin(self, data: FridMixin, path: str, /):
+        """Print any Frid mixin types."""
+        (name, args, kwas) = data.frid_repr()
+        self.print_named_args(name, args, kwas, path)
+
     def print_frid_value(self, data: FridValue, path: str='', /):
         """Print the any value that Frid supports to the stream."""
         s = self.prime_data_to_str(data, path)
         if s is not None:
             self.print(s, PPTokenType.ENTRY)
         elif isinstance(data, str):
             self.print_quoted_str(data, path)
         elif isinstance(data, Mapping):
             self.print('{', PPTokenType.START)
             self.print_naked_dict(data, path)
             self.print('}', PPTokenType.CLOSE)
+        elif isinstance(data, Set):
+            # We won't be able to load empty set back as set
+            self.print('{', PPTokenType.START)
+            self.print_naked_list(data, path)
+            self.print('}', PPTokenType.CLOSE)
         elif isinstance(data, Iterable):
             self.print('[', PPTokenType.START)
             self.print_naked_list(data, path)
             self.print(']', PPTokenType.CLOSE)
         elif isinstance(data, FridMixin):
             self.print_frid_mixin(data, path)
         elif self.print_user is not None and (out := self.print_user(data, path)) is not None:
@@ -278,16 +294,74 @@
 
 class FridStringDumper(PPToStringMixin, FridDumper):
     pass
 
 class FridTextIODumper(PPToTextIOMixin, FridDumper):
     pass
 
-def dump_into_str(data: FridValue, *args, **kwargs) -> str:
+def dump_into_str(data: FridValue, /, *args, **kwargs) -> str:
     dumper = FridStringDumper(*args, **kwargs)
     dumper.print_frid_value(data)
     return str(dumper)
 
-def dump_into_tio(data: FridValue, io: TextIO, *args, **kwargs) -> TextIO:
-    dumper = FridTextIODumper(io, *args, **kwargs)
+def dump_into_tio(data: FridValue, /, file: TextIO, *args, **kwargs) -> TextIO:
+    dumper = FridTextIODumper(file, *args, **kwargs)
     dumper.print_frid_value(data)
-    return io
+    return file
+
+def dump_args_into_str(name: str, opas: Sequence[FridValue], kwas: Mapping[str,FridValue],
+                       *args, **kwargs) -> str:
+    dumper = FridStringDumper(*args, **kwargs)
+    dumper.print_named_args(name, opas, kwas, '')
+    return str(dumper)
+
+def dump_args_into_tio(name: str, opas: Sequence[FridValue], kwas: Mapping[str,FridValue],
+                       /, file: TextIO, *args, **kwargs) -> TextIO:
+    dumper = FridTextIODumper(file, *args, **kwargs)
+    dumper.print_named_args(name, opas, kwas, '')
+    return file
+
+def frid_redact(data, depth: int=16) -> FridValue:
+    """Redacts the `data` of any type to a certain depth.
+    - Keeps null and boolean as is.
+    - Converts string to 's' + length.
+    - Converts bytes to 'b' + length.
+    - Converts integer to string 'i', float to string 'f', date/datetime to 'd', time to 't'.
+    - Converts mixins to its type name string.
+    - Recursively process the sequence and the mapping with decremented depth.
+    - Converts non-empty sequence to a single element of integer length if the depth is zero.
+    - Converts non-empty mapping to keys with no value if the depth reaches zero.
+    - Returns the redacted value.
+    This function is usually used before dump.
+    """
+    if data is None:
+        return None
+    if isinstance(data, bool):
+        return data
+    if isinstance(data, str):
+        return 's' + str(len(data))
+    if isinstance(data, BlobTypes):
+        return 'b' + str(len(data))
+    if isinstance(data, int):
+        return 'i'
+    if isinstance(data, float):
+        return 'f'
+    if isinstance(data, timeonly):
+        return 't'
+    if isinstance(data, datetime|dateonly):
+        return 'd'
+    if isinstance(data, FridMixin):
+        return data.frid_keys()[0]
+    if not data:
+        return data   # As is for empty mapping or sequence
+    if isinstance(data, Mapping):
+        if depth <= 0:
+            return {k: ... for k in data.keys()}
+        # Do not decrement the depth if value is a sequence; keep elipsis as is
+        return {k: v if v is ... else frid_redact(v, depth if is_list_like(v) else depth - 1)
+                for k, v in data.items()}
+    if isinstance(data, Sequence):
+        if depth <= 0:
+            return [len(data)]
+        return [frid_redact(x, depth-1) for x in data]
+    return "??"
+
```

### Comparing `frid-0.0.4/frid/errors.py` & `frid-0.0.5/frid/errors.py`

 * *Files identical despite different names*

### Comparing `frid-0.0.4/frid/guards.py` & `frid-0.0.5/frid/guards.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,23 +24,23 @@
 ) -> TypeGuard[Sequence]: ...
 @overload
 def is_list_like(
         data, /, etype: type[V], *, allow_none: Literal[False]=False
 ) -> TypeGuard[Sequence[V]]: ...
 @overload
 def is_list_like(
-        data, /, etype: type[V], *, allow_none: Literal[True]
+        data, /, etype: type[V], *, allow_none: Literal[True]|bool
 ) -> TypeGuard[Sequence[V|None]]: ...
 @overload
 def is_list_like(
         data, /, etype: Callable[[Any],TypeGuard[V]], *, allow_none: Literal[False]=False
 ) -> TypeGuard[Sequence[V]]: ...
 @overload
 def is_list_like(
-        data, /, etype: Callable[[Any],TypeGuard[V]], *, allow_none: Literal[True]
+        data, /, etype: Callable[[Any],TypeGuard[V]], *, allow_none: Literal[True]|bool
 ) -> TypeGuard[Sequence[V|None]]: ...
 def is_list_like(
         data, /, etype: Callable[[Any],bool]|type|None=None, *, allow_none: bool=False
 ) -> TypeGuard[Sequence]:
     """Type guard for a sequence type.
     Arguments:
     - `data`: the input data to be type-checked.
@@ -62,64 +62,81 @@
         if not allow_none:
             return all(etype(x) for x in data)
         return all(etype(x) or x is None for x in data)
     raise ValueError(f"Invalid etype specification: {etype}")
 
 @overload
 def is_dict_like(
-        data, vtypes: None=None, /, *, allow_none=False
+        data, /, vtype: None=None, *, allow_none=False
 ) -> TypeGuard[Mapping]: ...
 @overload
 def is_dict_like(
-        data, vtypes: type[V], ktypes: type[K]=str, *, allow_none: Literal[False]=False
+        data, /, vtype: type[V], ktype: type[K]=str, *, allow_none: Literal[False]=False
 ) -> TypeGuard[Mapping[K,V]]: ...
 @overload
 def is_dict_like(
-        data, vtypes: type[V], ktypes: type[K]=str, *, allow_none: Literal[True]
+        data, /, vtype: type[V], ktype: type[K]=str, *, allow_none: Literal[True]|bool
 ) -> TypeGuard[Mapping[K,V|None]]: ...
+@overload
+def is_dict_like(
+        data, /, vtype: Callable[[Any],TypeGuard[V]], ktype: type[K]=str,
+        *, allow_none: Literal[False]=False
+) -> TypeGuard[Mapping[K,V]]: ...
+@overload
 def is_dict_like(
-        data, vtypes: type|None=None, ktypes: type=str, *, allow_none=False
+        data, /, vtype: Callable[[Any],TypeGuard[V]], ktype: type[K]=str,
+        *, allow_none: Literal[True]|bool
+) -> TypeGuard[Mapping[K,V|None]]: ...
+def is_dict_like(
+        data, /, vtype: Callable[[Any],bool]|type|None=None,
+        ktype: type=str, *, allow_none=False
 ) -> TypeGuard[Mapping]:
     """Type guard for a map type.
     Arguments:
     - `data`: the input data to be type-checked.
     - `vtype`: the type for values (default: any).
     - `ktype`: the type for keys (default: `str`)
     - `allow_none`: if set to true, the element values is allowed to be None
       in addition to the `etype`.
     """
     if not isinstance(data, Mapping):
         return False
-    if ktypes is not None and not all(isinstance(x, ktypes) for x in data.keys()):
+    if ktype is not None and not all(isinstance(x, ktype) for x in data.keys()):
         return False
-    if vtypes is None:
+    if vtype is None:
         return True
-    if not allow_none:
-        return all(isinstance(x, ktypes) for x in data.values())
-    return all(isinstance(x, vtypes) or x is None for x in data.values())
+    if isinstance(vtype, type):
+        if not allow_none:
+            return all(isinstance(x, ktype) for x in data.values())
+        return all(isinstance(x, vtype) or x is None for x in data.values())
+    if callable(vtype):
+        if not allow_none:
+            return all(vtype(x) for x in data.values())
+        return all(vtype(x) or x is None for x in data.values())
+    raise ValueError(f"Invalid etype specification: {vtype}")
 
 
 @overload
 def as_type(dtype: type[V], data, /, allow_none: Literal[False]=False) -> V: ...
 @overload
-def as_type(dtype: type[V], data, /, allow_none: Literal[True]) -> V|None: ...
+def as_type(dtype: type[V], data, /, allow_none: Literal[True]|bool) -> V|None: ...
 def as_type(dtype: type[V], data, /, allow_none: bool=False) -> V|None:
     if data is None and allow_none:
         return None
     if not isinstance(data, dtype):
         raise ValueError(f"Expecting type {dtype}, got {type(data).__name__}")
     return data
 @overload
 def get_as_type(dtype: type[V], map: StrKeyMap, key: str,
                 /, allow_none: Literal[False]=False) -> V: ...
 @overload
 def get_as_type(dtype: type[V], map: StrKeyMap, key: str,
-                /, allow_none: Literal[True]) -> V|None: ...
+                /, allow_none: Literal[True]|bool) -> V|None: ...
 def get_as_type(dtype: type[V], map: StrKeyMap, key: str, /, allow_none: bool=False) -> V|None:
-    return as_type(dtype, map.get(key))
+    return as_type(dtype, map.get(key), allow_none=allow_none)
 
 def as_key_value_pair(
         data: Sequence[tuple[K,V]]|Mapping[K,V]|Iterable
 ) -> Sequence[tuple[K,V]]:
     """Converts the `data` to a sequence of key value pairs.
     - If the `data` is a map, convert it to a list of pairs.
     - If the `data` is already a sequence, return it as is.
@@ -138,15 +155,15 @@
 
 def is_frid_prime(data) -> TypeGuard[FridPrime]:
     return data is None or isinstance(data, str|BlobTypes|DateTypes|int|float|bool)
 def is_frid_array(data) -> TypeGuard[FridArray]:
     return isinstance(data, Sequence) and all(is_frid_value(x) for x in data)
 def is_frid_skmap(data) -> TypeGuard[StrKeyMap]:
     return isinstance(data, Mapping) and all(
-        isinstance(k, str) and is_frid_value(v) for k, v in data.items()
+        isinstance(k, str) and is_frid_value(v) or v is ... for k, v in data.items()
     )
 def is_frid_value(data) -> TypeGuard[FridValue]:
     return (is_frid_prime(data) or is_frid_array(data) or is_frid_skmap(data)
             or isinstance(data, FridMixin))
 
 def is_identifier_head(c: str) -> bool:
     """Returns if `c` can be first character of an indentifier."""
```

### Comparing `frid-0.0.4/frid/helper.py` & `frid-0.0.5/frid/helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from collections.abc import Callable, Mapping, Sequence
 from functools import partial
 from typing import Concatenate, Generic, ParamSpec, TypeVar, overload
 
-from .typing import BlobTypes, DateTypes, FridArray, FridValue, StrKeyMap
+from .typing import BlobTypes, DateTypes, FridArray, FridMapVT, FridSeqVT, FridValue, StrKeyMap
 from .guards import is_list_like
 from .strops import str_transform
 from .dumper import dump_into_str
 
 P = ParamSpec('P')
 T = TypeVar('T')
 CompareFunc = Callable[Concatenate[T,FridValue,P],bool]
@@ -100,21 +100,24 @@
         """Convert data to text in the case it is in the middle of a string.
         This method can be overridden by a derived class
         """
         if isinstance(data, str):
             return data
         return dump_into_str(data)
 
-    def evaluate(self, expr: str, values: StrKeyMap, default):
+    def evaluate(self, expr: str, values: StrKeyMap, default) -> FridValue:
         """Evaluate an expression against the values."""
         expr = expr.strip()
         if expr.endswith('*'):
             expr = expr[:-1]
             return {k[len(expr):]: v for k, v in values.items() if k.startswith(expr)}
-        return values.get(expr, default)
+        v = values.get(expr, default)
+        if v is ...:
+            return default
+        return v
 
     def sub_text(self, s: str, values: StrKeyMap|None, default) -> FridValue:
         """Return the string `s` with placeholder variable replaced with values.
         If a variable does not exist in `values`
         - Returns `...` (ellipsis)  if the template contains only a single variable;
         - Returns as is if template contains more than a single variable.
         """
@@ -131,31 +134,31 @@
                     raise IndexError(f"Search ends at {index}")
                 raise ValueError(f"Missing '}}' at {index}")
             expr = s[index:end]
             return (len(self.suffix) + end, self.textuate(self.evaluate(expr, values, default)))
         return str_transform(s, {self.prefix: _transform})[1]
     _T = TypeVar('_T', bound=FridValue)
     @overload
-    def sub(self, data: StrKeyMap, values: StrKeyMap|None=None) -> dict[str,FridValue]: ...
+    def sub(self, data: StrKeyMap, values: StrKeyMap|None=None) -> dict[str,FridMapVT]: ...
     @overload
-    def sub(self, data: FridArray, values: StrKeyMap|None=None) -> list[FridValue]: ...
+    def sub(self, data: FridArray, values: StrKeyMap|None=None) -> list[FridSeqVT]: ...
     @overload
     def sub(self, data: str, values: StrKeyMap|None=None) -> FridValue: ...
     @overload
     def sub(self, data: _T, values: StrKeyMap|None=None) -> _T: ...
     def sub(self, data: FridValue, values: StrKeyMap|None=None) -> FridValue:
         """Substitute the placeholders in data (only for its values).
-        The placeholders are escaped with `${...}` (only for string value).
-        The enclosed string `...` is used as the key to get the actual value
+        The placeholders are escaped with `${......}` (only for string value).
+        The enclosed string `......` is used as the key to get the actual value
         in `values`.
         """
         if isinstance(data, str):
             return self.sub_text(data, values, self.default)
         if isinstance(data, Mapping):
-            return {k: self.sub(v, values) for k, v in data.items()}
+            return {k: ... if v is ... else self.sub(v, values) for k, v in data.items()}
         if isinstance(data, Sequence):
             # Special handling for array: array return value do "splice"
             out = []
             for v in data:
                 r = self.sub(v, values)
                 if r is ...:
                     continue
```

### Comparing `frid-0.0.4/frid/loader.py` & `frid-0.0.5/frid/loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import math, base64
-from collections.abc import Callable, Iterator, Mapping
+from collections.abc import Callable, Iterator, Mapping, Set
 from typing import  Any, Literal, NoReturn, TextIO, TypeVar
 
 from .typing import BlobTypes, DateTypes, FridArray, FridMixin, FridPrime, FridValue, StrKeyMap
-from .guards import is_frid_identifier, is_frid_quote_free, is_quote_free_char
+from .guards import is_frid_identifier, is_frid_prime, is_frid_quote_free, is_quote_free_char
 from .errors import FridError
 from .strops import str_find_any, StringEscapeDecode
 from .chrono import parse_datetime
 from .dumper import EXTRA_ESCAPE_PAIRS
 
 NO_QUOTE_CHARS = "~!?@#$%^&*/"
 ALLOWED_QUOTES = "'`\""
@@ -17,14 +17,19 @@
 class ParseError(FridError):
     def __init__(self, s: str, index: int, *args, **kwargs):
         super().__init__(*args, **kwargs)
         note = s[(index-16):index] + '\u274e' + s[index:(index+16)]
         self.notes.append(note)
         self.input_string = s
         self.error_offset = index
+    def __str__(self):
+        s = super().__str__()
+        if not self.notes:
+            return s
+        return s + " => " + " | ".join(self.notes)
 
 class FridLoader:
     """This class loads data in buffer into Frid-allowed data structures.
 
     Constructor arguments (all optional):
     - `buffer`: the optional buffer for the (initial parts) of the data stream.
     - `length`: the upper limit of total length of the buffer if all text are
@@ -315,36 +320,58 @@
             out.append(value if value is not ... else '')
         # The last entry that is not an empty string will be added to the data.
         if value is not ...:
             out.append(value)
         return (index, out)
 
     def scan_naked_dict(self, index: int, path: str,
-                        /, stop: str='', sep: str=",:") -> tuple[int,StrKeyMap]:
+                        /, stop: str='', sep: str=",:") -> tuple[int,StrKeyMap|Set]:
         out = {}
         while True:
-            (index, key) = self.scan_frid_value(index, path, empty=...)
-            if key is ...:
-                break
-            if not isinstance(key, str):
+            (index, key) = self.scan_frid_value(index, path, empty='')
+            if not is_frid_prime(key):
                 self.error(index, f"Invalid key type {type(key).__name__} of a map: {path=}")
             if key in out:
                 self.error(index, f"Existing key '{key}' of a map: {path=}")
             index = self.skip_whitespace(index, path)
-            if self.peek_fixed_size(index, path, 1) != sep[1]:
+            c = self.peek_fixed_size(index, path, 1)
+            if c == sep[0]:
+                # Seeing item separator without key/value separator
+                if key == "":
+                    # Not allowing item separator with empty key and no key/value separator
+                    self.error(index, f"Missing data before '{sep[0]}'")
+                # Using value ... if key is non-empty
+                index = self.skip_fixed_size(index, path, len(c))
+                out[key] = ...
+                continue
+            if c in stop:
+                # If stops without key/value separator, add key=... only for non-empty key
+                if key != "":
+                    out[key] = ...
+                break
+            if c != sep[1]:
                 self.error(index, f"Expect '{sep[1]}' after key '{key}' of a map: {path=}")
+            # With value, key must be string
+            if not isinstance(key, str):
+                self.error(index, f"Invalid key type {type(key).__name__} of a map: {path=}")
             index = self.skip_fixed_size(index, path, 1)
             (index, value) = self.scan_frid_value(index, path + '/' + key)
             out[key] = value
             index = self.skip_whitespace(index, path)
             if (c := self.peek_fixed_size(index, path, 1)) in stop:  # Empty is also a sub-seq
                 break
             if c != sep[0]:
                 self.error(index, f"Expect '{sep[0]}' after the value for '{key}': {path=}")
             index = self.skip_fixed_size(index, path, len(c))
+        # Convert into a set if non-empty and all values are ...
+        if out:
+            if all(v is ... for v in out.values()):
+                out = set(out.keys())
+            elif any(not isinstance(k, str) for k in out.keys()):
+                self.error(index, f"Not a map but keys are not all string: {path=}")
         return (index, out)
 
     def scan_naked_args(
             self, index: int, path: str, /, stop: str='', sep: str=",="
     ) -> tuple[int,list[FridValue],dict[str,FridValue]]:
         args = []
         kwas = {}
```

### Comparing `frid-0.0.4/frid/pretty.py` & `frid-0.0.5/frid/pretty.py`

 * *Files identical despite different names*

### Comparing `frid-0.0.4/frid/strops.py` & `frid-0.0.5/frid/strops.py`

 * *Files identical despite different names*

### Comparing `frid-0.0.4/frid/webapp.py` & `frid-0.0.5/frid/webapp.py`

 * *Files identical despite different names*

### Comparing `frid-0.0.4/frid.egg-info/PKG-INFO` & `frid-0.0.5/frid.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frid
-Version: 0.0.4
+Version: 0.0.5
 Summary: Flexibly Represented Interactive Data
 Author-email: Hanhua Feng <han.hua.feng@askherefirst.com>
 Project-URL: Homepage, https://github.com/Ask-Here-First/ahf-generic
 Project-URL: Issues, https://github.com/Ask-Here-First/ahf-generic/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `frid-0.0.4/pyproject.toml` & `frid-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "frid"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Hanhua Feng", email="han.hua.feng@askherefirst.com" },
 ]
 description = "Flexibly Represented Interactive Data"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

