# Comparing `tmp/django_lookup_property-0.1.1.tar.gz` & `tmp/django_lookup_property-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_lookup_property-0.1.1.tar", max compression
+gzip compressed data, was "django_lookup_property-0.1.2.tar", max compression
```

## Comparing `django_lookup_property-0.1.1.tar` & `django_lookup_property-0.1.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1064 2024-02-18 08:11:26.784473 django_lookup_property-0.1.1/LICENSE
--rw-r--r--   0        0        0     2745 2024-02-18 08:11:26.784473 django_lookup_property-0.1.1/README.md
--rw-r--r--   0        0        0      305 2024-02-18 08:11:26.784473 django_lookup_property-0.1.1/lookup_property/__init__.py
--rw-r--r--   0        0        0      689 2024-02-18 08:11:26.784473 django_lookup_property-0.1.1/lookup_property/converters/__init__.py
--rw-r--r--   0        0        0     2383 2024-02-18 08:11:26.784473 django_lookup_property-0.1.1/lookup_property/converters/aggregates.py
--rw-r--r--   0        0        0     4255 2024-02-18 08:11:26.788473 django_lookup_property-0.1.1/lookup_property/converters/cast.py
--rw-r--r--   0        0        0     1915 2024-02-18 08:11:26.788473 django_lookup_property-0.1.1/lookup_property/converters/conditions.py
--rw-r--r--   0        0        0    10299 2024-02-18 08:11:26.788473 django_lookup_property-0.1.1/lookup_property/converters/datetime.py
--rw-r--r--   0        0        0     3382 2024-02-18 08:11:26.788473 django_lookup_property-0.1.1/lookup_property/converters/expressions.py
--rw-r--r--   0        0        0     4311 2024-02-18 08:11:26.788473 django_lookup_property-0.1.1/lookup_property/converters/functions.py
--rw-r--r--   0        0        0    11160 2024-02-18 08:11:26.788473 django_lookup_property-0.1.1/lookup_property/converters/lookups.py
--rw-r--r--   0        0        0     2341 2024-02-18 08:11:26.788473 django_lookup_property-0.1.1/lookup_property/converters/main.py
--rw-r--r--   0        0        0     6043 2024-02-18 08:11:26.788473 django_lookup_property-0.1.1/lookup_property/converters/math.py
--rw-r--r--   0        0        0      433 2024-02-18 08:11:26.788473 django_lookup_property-0.1.1/lookup_property/converters/number.py
--rw-r--r--   0        0        0     9155 2024-02-18 08:11:26.788473 django_lookup_property-0.1.1/lookup_property/converters/string.py
--rw-r--r--   0        0        0     2081 2024-02-18 08:11:26.788473 django_lookup_property-0.1.1/lookup_property/converters/utils.py
--rw-r--r--   0        0        0     4052 2024-02-18 08:11:26.788473 django_lookup_property-0.1.1/lookup_property/decorator.py
--rw-r--r--   0        0        0     1284 2024-02-18 08:11:26.788473 django_lookup_property-0.1.1/lookup_property/dispatch.py
--rw-r--r--   0        0        0    12847 2024-02-18 08:11:26.788473 django_lookup_property-0.1.1/lookup_property/expressions.py
--rw-r--r--   0        0        0     3438 2024-02-18 08:11:26.788473 django_lookup_property-0.1.1/lookup_property/field.py
--rw-r--r--   0        0        0        0 2024-02-18 08:11:26.788473 django_lookup_property-0.1.1/lookup_property/py.typed
--rw-r--r--   0        0        0     1721 2024-02-18 08:11:26.788473 django_lookup_property-0.1.1/lookup_property/typing.py
--rw-r--r--   0        0        0     5477 2024-02-18 08:11:26.788473 django_lookup_property-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     3887 1970-01-01 00:00:00.000000 django_lookup_property-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-04-06 14:38:59.358452 django_lookup_property-0.1.2/LICENSE
+-rw-r--r--   0        0        0     2745 2024-04-06 14:38:59.358452 django_lookup_property-0.1.2/README.md
+-rw-r--r--   0        0        0      305 2024-04-06 14:38:59.358452 django_lookup_property-0.1.2/lookup_property/__init__.py
+-rw-r--r--   0        0        0      689 2024-04-06 14:38:59.358452 django_lookup_property-0.1.2/lookup_property/converters/__init__.py
+-rw-r--r--   0        0        0     2383 2024-04-06 14:38:59.358452 django_lookup_property-0.1.2/lookup_property/converters/aggregates.py
+-rw-r--r--   0        0        0     4255 2024-04-06 14:38:59.358452 django_lookup_property-0.1.2/lookup_property/converters/cast.py
+-rw-r--r--   0        0        0     1915 2024-04-06 14:38:59.358452 django_lookup_property-0.1.2/lookup_property/converters/conditions.py
+-rw-r--r--   0        0        0    10299 2024-04-06 14:38:59.358452 django_lookup_property-0.1.2/lookup_property/converters/datetime.py
+-rw-r--r--   0        0        0     3382 2024-04-06 14:38:59.358452 django_lookup_property-0.1.2/lookup_property/converters/expressions.py
+-rw-r--r--   0        0        0     4311 2024-04-06 14:38:59.358452 django_lookup_property-0.1.2/lookup_property/converters/functions.py
+-rw-r--r--   0        0        0    11160 2024-04-06 14:38:59.362452 django_lookup_property-0.1.2/lookup_property/converters/lookups.py
+-rw-r--r--   0        0        0     2361 2024-04-06 14:38:59.362452 django_lookup_property-0.1.2/lookup_property/converters/main.py
+-rw-r--r--   0        0        0     6043 2024-04-06 14:38:59.362452 django_lookup_property-0.1.2/lookup_property/converters/math.py
+-rw-r--r--   0        0        0      433 2024-04-06 14:38:59.362452 django_lookup_property-0.1.2/lookup_property/converters/number.py
+-rw-r--r--   0        0        0     9155 2024-04-06 14:38:59.362452 django_lookup_property-0.1.2/lookup_property/converters/string.py
+-rw-r--r--   0        0        0     2081 2024-04-06 14:38:59.362452 django_lookup_property-0.1.2/lookup_property/converters/utils.py
+-rw-r--r--   0        0        0     4052 2024-04-06 14:38:59.362452 django_lookup_property-0.1.2/lookup_property/decorator.py
+-rw-r--r--   0        0        0     1284 2024-04-06 14:38:59.362452 django_lookup_property-0.1.2/lookup_property/dispatch.py
+-rw-r--r--   0        0        0    13960 2024-04-06 14:38:59.362452 django_lookup_property-0.1.2/lookup_property/expressions.py
+-rw-r--r--   0        0        0     3438 2024-04-06 14:38:59.362452 django_lookup_property-0.1.2/lookup_property/field.py
+-rw-r--r--   0        0        0        0 2024-04-06 14:38:59.362452 django_lookup_property-0.1.2/lookup_property/py.typed
+-rw-r--r--   0        0        0     2155 2024-04-06 14:38:59.362452 django_lookup_property-0.1.2/lookup_property/typing.py
+-rw-r--r--   0        0        0     5479 2024-04-06 14:38:59.362452 django_lookup_property-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3887 1970-01-01 00:00:00.000000 django_lookup_property-0.1.2/PKG-INFO
```

### Comparing `django_lookup_property-0.1.1/LICENSE` & `django_lookup_property-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django_lookup_property-0.1.1/README.md` & `django_lookup_property-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `django_lookup_property-0.1.1/lookup_property/converters/__init__.py` & `django_lookup_property-0.1.2/lookup_property/converters/__init__.py`

 * *Files identical despite different names*

### Comparing `django_lookup_property-0.1.1/lookup_property/converters/aggregates.py` & `django_lookup_property-0.1.2/lookup_property/converters/aggregates.py`

 * *Files identical despite different names*

### Comparing `django_lookup_property-0.1.1/lookup_property/converters/cast.py` & `django_lookup_property-0.1.2/lookup_property/converters/cast.py`

 * *Files identical despite different names*

### Comparing `django_lookup_property-0.1.1/lookup_property/converters/conditions.py` & `django_lookup_property-0.1.2/lookup_property/converters/conditions.py`

 * *Files identical despite different names*

### Comparing `django_lookup_property-0.1.1/lookup_property/converters/datetime.py` & `django_lookup_property-0.1.2/lookup_property/converters/datetime.py`

 * *Files identical despite different names*

### Comparing `django_lookup_property-0.1.1/lookup_property/converters/expressions.py` & `django_lookup_property-0.1.2/lookup_property/converters/expressions.py`

 * *Files identical despite different names*

### Comparing `django_lookup_property-0.1.1/lookup_property/converters/functions.py` & `django_lookup_property-0.1.2/lookup_property/converters/functions.py`

 * *Files identical despite different names*

### Comparing `django_lookup_property-0.1.1/lookup_property/converters/lookups.py` & `django_lookup_property-0.1.2/lookup_property/converters/lookups.py`

 * *Files identical despite different names*

### Comparing `django_lookup_property-0.1.1/lookup_property/converters/main.py` & `django_lookup_property-0.1.2/lookup_property/converters/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 
 def ast_to_module(function_name: str, return_value: ast.AST, state: State) -> ast.Module:
     function_body: list[ast.Import | ast.Return | ast.If | ast.Try] = [
         ast.Import(names=[ast.alias(name=import_name)]) for import_name in state.imports
     ]
 
-    if isinstance(return_value, (ast.If, ast.Try)):
+    if isinstance(return_value, (ast.If, ast.Try)):  # pragma: no cover
         function_body.append(return_value)
     else:
         function_body.append(ast.Return(value=return_value))
 
     module = ast.Module(
         body=[
             ast.FunctionDef(
```

### Comparing `django_lookup_property-0.1.1/lookup_property/converters/math.py` & `django_lookup_property-0.1.2/lookup_property/converters/math.py`

 * *Files identical despite different names*

### Comparing `django_lookup_property-0.1.1/lookup_property/converters/string.py` & `django_lookup_property-0.1.2/lookup_property/converters/string.py`

 * *Files identical despite different names*

### Comparing `django_lookup_property-0.1.1/lookup_property/converters/utils.py` & `django_lookup_property-0.1.2/lookup_property/converters/utils.py`

 * *Files identical despite different names*

### Comparing `django_lookup_property-0.1.1/lookup_property/decorator.py` & `django_lookup_property-0.1.2/lookup_property/decorator.py`

 * *Files identical despite different names*

### Comparing `django_lookup_property-0.1.1/lookup_property/dispatch.py` & `django_lookup_property-0.1.2/lookup_property/dispatch.py`

 * *Files identical despite different names*

### Comparing `django_lookup_property-0.1.1/lookup_property/expressions.py` & `django_lookup_property-0.1.2/lookup_property/expressions.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,30 +3,31 @@
 from contextlib import suppress
 from copy import deepcopy
 from functools import cached_property
 from typing import TYPE_CHECKING, Iterator
 
 from django.core.exceptions import FieldDoesNotExist
 from django.db import models
-from django.db.models import sql
+from django.db.models import Q, sql
 from django.db.models.constants import LOOKUP_SEP
-from django.db.models.expressions import BaseExpression, ResolvedOuterRef
+from django.db.models.expressions import BaseExpression, Combinable, NegatedExpression, ResolvedOuterRef
 from django.db.models.sql import Query
 
+from .typing import Sentinel
+
 if TYPE_CHECKING:
     from django.db.backends.base.base import BaseDatabaseWrapper
     from django.db.models.expressions import Col
     from django.db.models.lookups import Lookup, Transform
     from django.db.models.sql.compiler import SQLCompiler
     from django.db.models.sql.datastructures import Join
     from django.db.models.sql.where import WhereNode
 
     from .field import LookupPropertyField
-    from .typing import Any, Callable, ConvertFunc, Expr
-
+    from .typing import Any, Callable, ConvertFunc, Expr, ExpressionKind
 
 __all__ = [
     "LookupPropertyCol",
     "L",
 ]
 
 
@@ -43,15 +44,15 @@
         return self.target.model
 
     @property
     def alias(self) -> str:  # pragma: no cover
         return self.target.model._meta.db_table
 
     @property
-    def expression(self) -> Expr:
+    def expression(self) -> ExpressionKind:
         return self.target.expression
 
     @cached_property
     def output_field(self) -> models.Field:
         if hasattr(self.expression, "output_field"):
             return self.expression.output_field
         return self.resolved_target_expression.output_field  # type: ignore[union-attr]
@@ -62,26 +63,26 @@
 
     def get_lookup(self, name: str) -> type[Lookup] | None:
         return self.target.get_lookup(name)
 
     def get_transform(self, name: str) -> type[Transform] | None:
         return self.target.get_transform(name)  # pragma: no cover
 
-    def _resolve_joined_lookup(self, query: sql.Query) -> Expr:
+    def _resolve_joined_lookup(self, query: sql.Query) -> ExpressionKind:
         try:
             join: Join = query.alias_map[self.model._meta.db_table]  # type: ignore[assignment]
         except KeyError:
             # Lookup property is referenced with an OuterRef in a Subquery.
             return self.resolved_target_expression  # type: ignore[return-value]
 
         table_name: str = join.join_field.name  # type: ignore[union-attr,attr-defined]
         return extend_expression_to_joined_table(self.expression, table_name)
 
     def as_sql(self, compiler: SQLCompiler, connection: BaseDatabaseWrapper) -> tuple[str, list[Any]]:
-        expression: Expr = self.expression
+        expression = self.expression
         if self.model != compiler.query.model:
             expression = self._resolve_joined_lookup(compiler.query)
 
         resolved: Col | WhereNode | BaseExpression
         resolved = expression.resolve_expression(compiler.query)  # type: ignore[assignment]
 
         vendor_impl: Callable[[SQLCompiler, BaseDatabaseWrapper], tuple[str, list[Any]]] | None
@@ -94,47 +95,51 @@
     @cached_property
     def convert_value(self) -> ConvertFunc:  # pragma: no cover
         if expression_has_output_field(self.expression) and hasattr(self.expression, "convert_value"):
             return self.expression.convert_value
         return super().convert_value
 
 
-class L:
+class L(Combinable):
     """
     Designate a lookup property as a filter condition or values selection.
 
     Examples:
 
-    >>> qs.values(full_name_alias=L("full_name"))
+    >>> qs.values(full_name=L("full_name"))
 
     >>> qs.values_list(L("full_name"), flat=True)
 
     >>> qs.filter(L(full_name__contains="foo"))
 
     >>> sq = qs_1.filter(name=OuterRef("full_name")).values("pk")
     >>> qs_2.filter(id__in=L(models.Subquery(sq)))
     """
 
     def __init__(self, __ref: str | models.Subquery = "", /, **kwargs: Any) -> None:
+        self.conditional = bool(kwargs)  # See. `django.db.models.sql.query.Query.build_filter`
+
         if __ref:  # pragma: no cover
             if kwargs:
                 msg = "Either one positional or keyword argument can be given."
                 raise ValueError(msg)
 
             self.lookup = __ref
 
-        elif len(kwargs) != 1:  # pragma: no cover
-            msg = "Exactly one keyword argument is required."
+        elif len(kwargs) > 1:  # pragma: no cover
+            msg = "Multiple keyword arguments are not supported."
+            raise ValueError(msg)
+
+        elif not kwargs:  # pragma: no cover
+            msg = "Either one positional or keyword argument must be given."
             raise ValueError(msg)
 
         else:
             self.lookup, self.value = kwargs.popitem()
 
-        self.conditional = True  # See. `django.db.models.sql.query.Query.build_filter`
-
     def __str__(self) -> str:
         if hasattr(self, "value"):
             return f"{self.__class__.__name__}({self.lookup}={self.value!r})"
         return f"{self.__class__.__name__}({self.lookup!r})"
 
     def __repr__(self) -> str:
         return str(self)
@@ -146,22 +151,47 @@
 
     def __len__(self) -> int:
         return len(list(iter(self)))
 
     def __getitem__(self, item: int) -> Any:
         return list(self)[item]
 
+    def __or__(self, other: L | Q) -> Q:
+        return Q(self) | Q(other)
+
+    def __and__(self, other: L | Q) -> Q:
+        return Q(self) & Q(other)
+
+    def __xor__(self, other: L | Q) -> Q:
+        return Q(self) ^ Q(other)
+
+    def __invert__(self) -> Q | NegatedExpression:
+        if self.conditional:
+            return ~Q(self)
+        return super().__invert__()
+
+    def __eq__(self, other: object) -> bool:
+        if not isinstance(other, L):
+            return False
+        return self.lookup == other.lookup and getattr(self, "value", Sentinel) == getattr(other, "value", Sentinel)
+
+    def __hash__(self) -> int:
+        value = getattr(self, "value", Sentinel)
+        if value is not Sentinel:
+            return hash((self.lookup, value))
+        return hash(self.lookup)
+
     def resolve_expression(  # noqa: PLR0913
         self,
         query: Query,
         allow_joins: bool,  # noqa: FBT001
         reuse: Any = None,
         summarize: bool = False,  # noqa: FBT001, FBT002
         for_save: bool = False,  # noqa: ARG002, FBT001, FBT002
-    ) -> Expr:
+    ) -> ExpressionKind:
         """Resolve lookup expression and either return it or build a lookup expression based on it."""
         field, lookup_parts, joined_tables = self.find_lookup_property_field(query)
         lookup_name = field.attname.removeprefix("_")
         expression = field.expression
         for table_name in reversed(joined_tables):
             expression = extend_expression_to_joined_table(expression, table_name)
 
@@ -234,38 +264,38 @@
                     query.join(query.base_table_class(table, table))
 
             break
 
         return field, lookup_parts, joined_tables
 
 
-def expression_has_output_field(expression: Expr) -> bool:  # pragma: no cover
+def expression_has_output_field(expression: ExpressionKind) -> bool:  # pragma: no cover
     # Check whether the 'output_field' of the expression can be resolved.
     # This might fail, and does fail for expressions like Trunc if the 'output_field'
     # is not explicitly given (e.g. 'Trunc(F("foo"))' will end up using 'BaseExpression.output_field',
     # which then uses 'BaseExpression.get_source_fields' while F does not have an '_output_field_or_none').
     with suppress(AttributeError):
         return expression.output_field is not None  # type: ignore[union-attr]
     return False
 
 
 def extend_expression_to_joined_table(expression: Expr, table_name: str) -> Expr:
-    """Rewrite the expression so that any containing F and Q expressions are referenced from the given table."""
+    """Rewrite an expression so that any containing expressions are referenced from the given table."""
     if isinstance(expression, models.F):
         expression = deepcopy(expression)
         expression.name = f"{table_name}{LOOKUP_SEP}{expression.name}"
         return expression
 
     if isinstance(expression, L):
         expression = deepcopy(expression)
         expression.lookup = f"{table_name}{LOOKUP_SEP}{expression.lookup}"
         if hasattr(expression, "value"):
             expression.value = (
                 extend_expression_to_joined_table(expression.value, table_name)
-                if isinstance(expression.value, (models.F, models.Q, BaseExpression))
+                if isinstance(expression.value, (models.F, models.Q, BaseExpression, L))
                 else expression.value
             )
         return expression
 
     if isinstance(expression, models.Q):
         expression = deepcopy(expression)
         children: list[tuple[str, Any] | models.Q | L] = expression.children  # type: ignore[assignment]
@@ -282,15 +312,15 @@
                 expression.children.append((f"{table_name}{LOOKUP_SEP}{child[0]}", value))
 
         return expression
 
     # For sub-queries, only OuterRefs are rewritten.
     if isinstance(expression, models.Subquery):
         expression = deepcopy(expression)
-        sub_expressions: list[Expr] = expression.query.where.children
+        sub_expressions: list[ExpressionKind] = expression.query.where.children  # type: ignore[assignment]
         expression.query.where.children = []
         for child in sub_expressions:
             expression.query.where.children.append(extend_subquery_to_joined_table(child, table_name))
         return expression
 
     expression = deepcopy(expression)
     expressions = [extend_expression_to_joined_table(expr, table_name) for expr in expression.get_source_expressions()]
```

### Comparing `django_lookup_property-0.1.1/lookup_property/field.py` & `django_lookup_property-0.1.2/lookup_property/field.py`

 * *Files identical despite different names*

### Comparing `django_lookup_property-0.1.1/lookup_property/typing.py` & `django_lookup_property-0.1.2/lookup_property/typing.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,15 @@
+from __future__ import annotations
+
 import random
 import string
 from dataclasses import dataclass, field
 from types import FunctionType
 from typing import (
+    TYPE_CHECKING,
     Any,
     Callable,
     Collection,
     Concatenate,
     Generator,
     Iterable,
     Literal,
@@ -16,15 +19,18 @@
     TypeVar,
     cast,
 )
 
 from django.conf import settings
 from django.db import models
 from django.db.backends.base.base import BaseDatabaseWrapper
-from django.db.models.expressions import BaseExpression
+from django.db.models.expressions import BaseExpression, Combinable
+
+if TYPE_CHECKING:
+    from django.db.models.sql import Query
 
 __all__ = [
     "Any",
     "Callable",
     "cast",
     "Collection",
     "Concatenate",
@@ -39,16 +45,30 @@
     "Protocol",
     "Self",
     "State",
     "TModel",
     "TypeVar",
 ]
 
+
 TModel = TypeVar("TModel", bound=models.Model)
-Expr = BaseExpression | models.F | models.Q
+Expr = BaseExpression | Combinable | models.Q
+
+
+class ExpressionKind(Protocol):
+    def resolve_expression(  # noqa: PLR0913
+        self,
+        query: Query,
+        allow_joins: bool,  # noqa: FBT001
+        reuse: set[str] | None,
+        summarize: bool,  # noqa: FBT001
+        for_save: bool,  # noqa: FBT001
+    ) -> ExpressionKind: ...
+
+
 ModelMethod = Callable[[TModel], Expr] | Callable[[], Expr]
 ConvertFunc = Callable[[Any, BaseExpression, BaseDatabaseWrapper], Any]
 
 Sentinel = object()
 
 
 def random_arg_name() -> str:
```

### Comparing `django_lookup_property-0.1.1/pyproject.toml` & `django_lookup_property-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-lookup-property"
-version = "0.1.1"
+version = "0.1.2"
 description = "Django model properties that are also lookup expressions."
 authors = [
     "Matti Lamppu <lamppu.matti.akseli@gmail.com>",
 ]
 packages = [
     { include = "lookup_property" },
 ]
@@ -45,31 +45,31 @@
 "Bug Tracker" = "https://github.com/MrThearMan/django-lookup-property/issues"
 
 [tool.poetry.dependencies]
 python = ">=3.11,<4"
 Django = ">=4.2"
 
 [tool.poetry.group.test.dependencies]
-pytest = "8.0.1"
-coverage = "7.4.1"
+pytest = "8.1.1"
+coverage = "7.4.4"
 pytest-django = "4.8.0"
 freezegun = "^1.2.2"
-pre-commit = "3.6.1"
-tox = "4.13.0"
+pre-commit = "3.7.0"
+tox = "4.14.2"
 tox-gh-actions = "3.2.0"
 factory-boy = "^3.3.0"
 django-shared-property = "^0.8.0"
 
 [tool.poetry.group.docs.dependencies]
 mkdocs = "1.5.3"
-pymdown-extensions = "10.7"
+pymdown-extensions = "10.7.1"
 mkdocs-mermaid2-plugin = "1.1.1"
 
 [tool.poetry.group.lint.dependencies]
-mypy = "1.8.0"
+mypy = "1.9.0"
 django-stubs = "4.2.7"
 
 [tool.ruff]
 fix = true
 line-length = 120
 extend-exclude = [
     "tests/*",
```

### Comparing `django_lookup_property-0.1.1/PKG-INFO` & `django_lookup_property-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-lookup-property
-Version: 0.1.1
+Version: 0.1.2
 Summary: Django model properties that are also lookup expressions.
 Home-page: https://mrthearman.github.io/django-lookup-property
 License: MIT
 Keywords: django,lookup,property,orm,model,extension
 Author: Matti Lamppu
 Author-email: lamppu.matti.akseli@gmail.com
 Requires-Python: >=3.11,<4
```

