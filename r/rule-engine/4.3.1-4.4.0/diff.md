# Comparing `tmp/rule-engine-4.3.1.tar.gz` & `tmp/rule-engine-4.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rule-engine-4.3.1.tar", last modified: Mon Jan 15 18:04:38 2024, max compression
+gzip compressed data, was "rule-engine-4.4.0.tar", last modified: Sat Apr  6 00:12:58 2024, max compression
```

## Comparing `rule-engine-4.3.1.tar` & `rule-engine-4.4.0.tar`

### file list

```diff
@@ -1,25 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 18:04:38.389888 rule-engine-4.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-01-15 18:04:13.000000 rule-engine-4.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5293 2024-01-15 18:04:38.389888 rule-engine-4.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4191 2024-01-15 18:04:13.000000 rule-engine-4.3.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 18:04:38.385888 rule-engine-4.3.1/lib/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 18:04:38.385888 rule-engine-4.3.1/lib/rule_engine/
--rw-r--r--   0 runner    (1001) docker     (127)     1989 2024-01-15 18:04:13.000000 rule-engine-4.3.1/lib/rule_engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-01-15 18:04:13.000000 rule-engine-4.3.1/lib/rule_engine/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    52628 2024-01-15 18:04:13.000000 rule-engine-4.3.1/lib/rule_engine/ast.py
--rw-r--r--   0 runner    (1001) docker     (127)     8465 2024-01-15 18:04:13.000000 rule-engine-4.3.1/lib/rule_engine/builtins.py
--rw-r--r--   0 runner    (1001) docker     (127)     2512 2024-01-15 18:04:13.000000 rule-engine-4.3.1/lib/rule_engine/debug_ast.py
--rw-r--r--   0 runner    (1001) docker     (127)     4707 2024-01-15 18:04:13.000000 rule-engine-4.3.1/lib/rule_engine/debug_repl.py
--rw-r--r--   0 runner    (1001) docker     (127)    25372 2024-01-15 18:04:13.000000 rule-engine-4.3.1/lib/rule_engine/engine.py
--rw-r--r--   0 runner    (1001) docker     (127)    11982 2024-01-15 18:04:13.000000 rule-engine-4.3.1/lib/rule_engine/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    18616 2024-01-15 18:04:13.000000 rule-engine-4.3.1/lib/rule_engine/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     3654 2024-01-15 18:04:13.000000 rule-engine-4.3.1/lib/rule_engine/suggestions.py
--rw-r--r--   0 runner    (1001) docker     (127)    22572 2024-01-15 18:04:13.000000 rule-engine-4.3.1/lib/rule_engine/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 18:04:38.385888 rule-engine-4.3.1/lib/rule_engine.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5293 2024-01-15 18:04:38.000000 rule-engine-4.3.1/lib/rule_engine.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-01-15 18:04:38.000000 rule-engine-4.3.1/lib/rule_engine.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-15 18:04:38.000000 rule-engine-4.3.1/lib/rule_engine.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-01-15 18:04:38.000000 rule-engine-4.3.1/lib/rule_engine.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-01-15 18:04:38.000000 rule-engine-4.3.1/lib/rule_engine.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-15 18:04:38.389888 rule-engine-4.3.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     3778 2024-01-15 18:04:13.000000 rule-engine-4.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 00:12:58.483672 rule-engine-4.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-04-06 00:12:35.000000 rule-engine-4.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5293 2024-04-06 00:12:58.483672 rule-engine-4.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4191 2024-04-06 00:12:35.000000 rule-engine-4.4.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 00:12:58.479672 rule-engine-4.4.0/lib/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 00:12:58.483672 rule-engine-4.4.0/lib/rule_engine/
+-rw-r--r--   0 runner    (1001) docker     (127)     1989 2024-04-06 00:12:35.000000 rule-engine-4.4.0/lib/rule_engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52638 2024-04-06 00:12:35.000000 rule-engine-4.4.0/lib/rule_engine/ast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9269 2024-04-06 00:12:35.000000 rule-engine-4.4.0/lib/rule_engine/builtins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2512 2024-04-06 00:12:35.000000 rule-engine-4.4.0/lib/rule_engine/debug_ast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4707 2024-04-06 00:12:35.000000 rule-engine-4.4.0/lib/rule_engine/debug_repl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25372 2024-04-06 00:12:35.000000 rule-engine-4.4.0/lib/rule_engine/engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11982 2024-04-06 00:12:35.000000 rule-engine-4.4.0/lib/rule_engine/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 00:12:58.483672 rule-engine-4.4.0/lib/rule_engine/parser/
+-rw-r--r--   0 runner    (1001) docker     (127)    16872 2024-04-06 00:12:35.000000 rule-engine-4.4.0/lib/rule_engine/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3367 2024-04-06 00:12:35.000000 rule-engine-4.4.0/lib/rule_engine/parser/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35017 2024-04-06 00:12:35.000000 rule-engine-4.4.0/lib/rule_engine/parser/parsetab.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3786 2024-04-06 00:12:35.000000 rule-engine-4.4.0/lib/rule_engine/parser/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3654 2024-04-06 00:12:35.000000 rule-engine-4.4.0/lib/rule_engine/suggestions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22572 2024-04-06 00:12:35.000000 rule-engine-4.4.0/lib/rule_engine/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 00:12:58.483672 rule-engine-4.4.0/lib/rule_engine.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5293 2024-04-06 00:12:58.000000 rule-engine-4.4.0/lib/rule_engine.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-06 00:12:58.000000 rule-engine-4.4.0/lib/rule_engine.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 00:12:58.000000 rule-engine-4.4.0/lib/rule_engine.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-06 00:12:58.000000 rule-engine-4.4.0/lib/rule_engine.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-06 00:12:58.000000 rule-engine-4.4.0/lib/rule_engine.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 00:12:58.483672 rule-engine-4.4.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3778 2024-04-06 00:12:35.000000 rule-engine-4.4.0/setup.py
```

### Comparing `rule-engine-4.3.1/LICENSE` & `rule-engine-4.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rule-engine-4.3.1/PKG-INFO` & `rule-engine-4.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rule-engine
-Version: 4.3.1
+Version: 4.4.0
 Summary: A lightweight, optionally typed expression language with a custom grammar for matching arbitrary Python objects.
 Home-page: https://github.com/zeroSteiner/rule-engine
 Author: Spencer McIntyre
 Author-email: zeroSteiner@gmail.com
 Maintainer: Spencer McIntyre
 Maintainer-email: zeroSteiner@gmail.com
 License: BSD
```

### Comparing `rule-engine-4.3.1/README.rst` & `rule-engine-4.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `rule-engine-4.3.1/lib/rule_engine/__init__.py` & `rule-engine-4.4.0/lib/rule_engine/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 #  LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE,
 #  DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY
 #  THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
 #  (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 #  OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 #
 
-__version__ = '4.3.1'
+__version__ = '4.4.0'
 
 from .engine import resolve_attribute
 from .engine import resolve_item
 from .engine import type_resolver_from_dict
 from .engine import Context
 from .engine import Rule
```

### Comparing `rule-engine-4.3.1/lib/rule_engine/ast.py` & `rule-engine-4.4.0/lib/rule_engine/ast.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 import collections.abc
 import datetime
 import functools
 import operator
 import re
 
 from . import errors
-from ._utils import parse_datetime, parse_float, parse_timedelta
+from .parser.utilities import parse_datetime, parse_float, parse_timedelta
 from .suggestions import suggest_symbol
 from .types import *
 
 def _assert_is_integer_number(*values):
 	if not all(map(is_integer_number, values)):
 		raise errors.EvaluationError('data type mismatch (not an integer number)')
```

### Comparing `rule-engine-4.3.1/lib/rule_engine/builtins.py` & `rule-engine-4.4.0/lib/rule_engine/builtins.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,18 +34,18 @@
 import collections.abc
 import datetime
 import decimal
 import functools
 import math
 import random
 
-from ._utils import parse_datetime, parse_float, parse_timedelta
 from . import ast
 from . import errors
 from . import types
+from .parser.utilities import parse_datetime, parse_float, parse_timedelta
 
 import dateutil.tz
 
 def _builtin_filter(function, iterable):
 	return tuple(filter(function, iterable))
 
 def _builtin_map(function, iterable):
@@ -57,14 +57,27 @@
 def _builtin_random(boundary=None):
 	if boundary:
 		if not types.is_natural_number(boundary):
 			raise errors.FunctionCallError('argument #1 (boundary) must be a natural number')
 		return random.randint(0, int(boundary))
 	return random.random()
 
+def _builtin_range(start, stop=None, step=None):
+	if not types.is_integer_number(start):
+		raise errors.FunctionCallError('argument #1 (start) must be an integer number')
+	if stop:
+		if not types.is_integer_number(stop):
+			raise errors.FunctionCallError('argument #2 (stop) must be an integer number')
+		if step:
+			if not types.is_integer_number(step):
+				raise errors.FunctionCallError('argument #3 (step) must be an integer number')
+			return list(range(int(start), int(stop), int(step)))
+		return list(range(int(start), int(stop)))
+	return list(range(int(start)))
+
 def _builtins_split(string, sep=None, maxsplit=None):
 	if maxsplit is None:
 		maxsplit = -1
 	elif types.is_natural_number(maxsplit):
 		maxsplit = int(maxsplit)
 	else:
 		raise errors.FunctionCallError('argument #3 (maxsplit) must be a natural number')
@@ -161,14 +174,15 @@
 			'max': max,
 			'min': min,
 			'filter': _builtin_filter,
 			'parse_datetime': BuiltinValueGenerator(lambda builtins: functools.partial(_builtin_parse_datetime, builtins)),
 			'parse_float': parse_float,
 			'parse_timedelta': parse_timedelta,
 			'random': _builtin_random,
+			'range': _builtin_range,
 			'split': _builtins_split
 		}
 		default_values.update(values or {})
 		default_value_types = {
 			# mathematical constants
 			'e': ast.DataType.FLOAT,
 			'pi': ast.DataType.FLOAT,
@@ -184,14 +198,15 @@
 			'max': ast.DataType.FUNCTION('max', return_type=ast.DataType.FLOAT, argument_types=(ast.DataType.ARRAY(ast.DataType.FLOAT),)),
 			'min': ast.DataType.FUNCTION('min', return_type=ast.DataType.FLOAT, argument_types=(ast.DataType.ARRAY(ast.DataType.FLOAT),)),
 			'filter': ast.DataType.FUNCTION('filter', return_type=ast.DataType.ARRAY, argument_types=(ast.DataType.FUNCTION, ast.DataType.ARRAY)),
 			'parse_datetime': ast.DataType.FUNCTION('parse_datetime', return_type=ast.DataType.DATETIME, argument_types=(ast.DataType.STRING,)),
 			'parse_float': ast.DataType.FUNCTION('parse_float', return_type=ast.DataType.FLOAT, argument_types=(ast.DataType.STRING,)),
 			'parse_timedelta': ast.DataType.FUNCTION('parse_timedelta', return_type=ast.DataType.TIMEDELTA, argument_types=(ast.DataType.STRING,)),
 			'random': ast.DataType.FUNCTION('random', return_type=ast.DataType.FLOAT, argument_types=(ast.DataType.FLOAT,), minimum_arguments=0),
+			'range': ast.DataType.FUNCTION('range', return_type=ast.DataType.ARRAY(ast.DataType.FLOAT), argument_types=(ast.DataType.FLOAT, ast.DataType.FLOAT, ast.DataType.FLOAT,), minimum_arguments=1),
 			'split': ast.DataType.FUNCTION(
 				'split',
 				return_type=ast.DataType.ARRAY(ast.DataType.STRING),
 				argument_types=(ast.DataType.STRING, ast.DataType.STRING, ast.DataType.FLOAT),
 				minimum_arguments=1
 			)
 		}
```

### Comparing `rule-engine-4.3.1/lib/rule_engine/debug_ast.py` & `rule-engine-4.4.0/lib/rule_engine/debug_ast.py`

 * *Files identical despite different names*

### Comparing `rule-engine-4.3.1/lib/rule_engine/debug_repl.py` & `rule-engine-4.4.0/lib/rule_engine/debug_repl.py`

 * *Files identical despite different names*

### Comparing `rule-engine-4.3.1/lib/rule_engine/engine.py` & `rule-engine-4.4.0/lib/rule_engine/engine.py`

 * *Files identical despite different names*

### Comparing `rule-engine-4.3.1/lib/rule_engine/errors.py` & `rule-engine-4.4.0/lib/rule_engine/errors.py`

 * *Files identical despite different names*

### Comparing `rule-engine-4.3.1/lib/rule_engine/parser.py` & `rule-engine-4.4.0/lib/rule_engine/parser/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 #
-#  rule_engine/parser.py
+#  rule_engine/parser/__init__.py
 #
 #  Redistribution and use in source and binary forms, with or without
 #  modification, are permitted provided that the following conditions are
 #  met:
 #
 #  * Redistributions of source code must retain the above copyright
 #    notice, this list of conditions and the following disclaimer.
@@ -28,23 +28,20 @@
 #  THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
 #  (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 #  OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 #
 
 import ast as pyast
 import collections
-import threading
 import types as pytypes
 
-from . import ast
-from . import errors
-from ._utils import timedelta_regex
-
-import ply.lex as lex
-import ply.yacc as yacc
+from .. import ast
+from .. import errors
+from .base import ParserBase
+from .utilities import timedelta_regex
 
 literal_eval = pyast.literal_eval
 
 class _DeferredAstNode(object):
 	__slots__ = ('cls', 'args', 'kwargs', 'method')
 	def __init__(self, cls, *, args, kwargs=None, method='build'):
 		if not issubclass(cls, ast.ASTNodeBase):
@@ -54,60 +51,14 @@
 		self.kwargs = kwargs or {}
 		self.method = method
 
 	def build(self):
 		constructor = getattr(self.cls, self.method)
 		return constructor(*self.args, **self.kwargs)
 
-class ParserBase(object):
-	"""
-	A base class for parser objects to inherit from. This does not provide any
-	grammar related definitions.
-	"""
-	precedence = ()
-	"""The precedence for operators."""
-	tokens = ()
-	reserved_words = {}
-	"""
-	A mapping of literal words which are reserved to their corresponding grammar
-	names.
-	"""
-	__mutex = threading.Lock()
-	def __init__(self, debug=False):
-		"""
-		:param bool debug: Whether or not to enable debugging features when
-			using the ply API.
-		"""
-		self.debug = debug
-		self.context = None
-		# Build the lexer and parser
-		self._lexer = lex.lex(module=self, debug=self.debug)
-		self._parser = yacc.yacc(module=self, debug=self.debug, write_tables=self.debug)
-
-	def parse(self, text, context, **kwargs):
-		"""
-		Parse the specified text in an abstract syntax tree of nodes that can later be evaluated. This is done in two
-		phases. First, the syntax is parsed and a tree of deferred / uninitialized AST nodes are constructed. Next each
-		node is built recursively using it's respective :py:meth:`rule_engine.ast.ASTNodeBase.build`.
-
-		:param str text: The grammar text to parse into an AST.
-		:param context: A context for specifying parsing and evaluation options.
-		:type context: :py:class:`~rule_engine.engine.Context`
-		:return: The parsed AST statement.
-		:rtype: :py:class:`~rule_engine.ast.Statement`
-		"""
-		kwargs['lexer'] = kwargs.pop('lexer', self._lexer)
-		with self.__mutex:
-			self.context = context
-			# phase 1: parse the string into a tree of deferred nodes
-			result = self._parser.parse(text, **kwargs)
-			self.context = None
-		# phase 2: initialize each AST node recursively, providing them with an opportunity to define assignments
-		return result.build()
-
 class Parser(ParserBase):
 	"""
 	The parser class for the rule grammar. This class contains many ply specific
 	members to define the various components of the grammar allowing it to be
 	parsed and reduced into an abstract syntax tree (AST). Once the AST has been
 	constructed it can then be evaluated multiple times. To make the evaluation
 	more efficient, nodes within the AST that are able to be reduced are while
```

### Comparing `rule-engine-4.3.1/lib/rule_engine/suggestions.py` & `rule-engine-4.4.0/lib/rule_engine/suggestions.py`

 * *Files identical despite different names*

### Comparing `rule-engine-4.3.1/lib/rule_engine/types.py` & `rule-engine-4.4.0/lib/rule_engine/types.py`

 * *Files identical despite different names*

### Comparing `rule-engine-4.3.1/lib/rule_engine.egg-info/PKG-INFO` & `rule-engine-4.4.0/lib/rule_engine.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rule-engine
-Version: 4.3.1
+Version: 4.4.0
 Summary: A lightweight, optionally typed expression language with a custom grammar for matching arbitrary Python objects.
 Home-page: https://github.com/zeroSteiner/rule-engine
 Author: Spencer McIntyre
 Author-email: zeroSteiner@gmail.com
 Maintainer: Spencer McIntyre
 Maintainer-email: zeroSteiner@gmail.com
 License: BSD
```

### Comparing `rule-engine-4.3.1/lib/rule_engine.egg-info/SOURCES.txt` & `rule-engine-4.4.0/lib/rule_engine.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 LICENSE
 README.rst
 setup.py
 lib/rule_engine/__init__.py
-lib/rule_engine/_utils.py
 lib/rule_engine/ast.py
 lib/rule_engine/builtins.py
 lib/rule_engine/debug_ast.py
 lib/rule_engine/debug_repl.py
 lib/rule_engine/engine.py
 lib/rule_engine/errors.py
-lib/rule_engine/parser.py
 lib/rule_engine/suggestions.py
 lib/rule_engine/types.py
 lib/rule_engine.egg-info/PKG-INFO
 lib/rule_engine.egg-info/SOURCES.txt
 lib/rule_engine.egg-info/dependency_links.txt
 lib/rule_engine.egg-info/requires.txt
-lib/rule_engine.egg-info/top_level.txt
+lib/rule_engine.egg-info/top_level.txt
+lib/rule_engine/parser/__init__.py
+lib/rule_engine/parser/base.py
+lib/rule_engine/parser/parsetab.py
+lib/rule_engine/parser/utilities.py
```

### Comparing `rule-engine-4.3.1/setup.py` & `rule-engine-4.4.0/setup.py`

 * *Files identical despite different names*

