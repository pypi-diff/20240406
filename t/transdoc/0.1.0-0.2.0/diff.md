# Comparing `tmp/transdoc-0.1.0.tar.gz` & `tmp/transdoc-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "transdoc-0.1.0.tar", max compression
+gzip compressed data, was "transdoc-0.2.0.tar", max compression
```

## Comparing `transdoc-0.1.0.tar` & `transdoc-0.2.0.tar`

### file list

```diff
@@ -1,7 +1,18 @@
--rw-r--r--   0        0        0     1073 2024-01-29 13:24:47.893260 transdoc-0.1.0/LICENSE
--rw-r--r--   0        0        0     2715 2024-01-29 13:24:47.893260 transdoc-0.1.0/README.md
--rw-r--r--   0        0        0      687 2024-01-29 13:24:47.893260 transdoc-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      173 2024-01-29 13:24:47.893260 transdoc-0.1.0/transdoc/__init__.py
--rw-r--r--   0        0        0      228 2024-01-29 13:24:47.893260 transdoc-0.1.0/transdoc/__rule.py
--rw-r--r--   0        0        0     5241 2024-01-29 13:24:47.893260 transdoc-0.1.0/transdoc/__transformer.py
--rw-r--r--   0        0        0     3311 1970-01-01 00:00:00.000000 transdoc-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-04-06 12:30:46.705493 transdoc-0.2.0/LICENSE
+-rw-r--r--   0        0        0     3931 2024-04-06 12:30:46.705493 transdoc-0.2.0/README.md
+-rw-r--r--   0        0        0     1463 2024-04-06 12:30:46.705493 transdoc-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     6006 2024-04-06 12:30:46.705493 transdoc-0.2.0/transdoc/__cli/__init__.py
+-rw-r--r--   0        0        0     1277 2024-04-06 12:30:46.705493 transdoc-0.2.0/transdoc/__cli/mutex.py
+-rw-r--r--   0        0        0      648 2024-04-06 12:30:46.705493 transdoc-0.2.0/transdoc/__collect_rules.py
+-rw-r--r--   0        0        0       74 2024-04-06 12:30:46.705493 transdoc-0.2.0/transdoc/__consts.py
+-rw-r--r--   0        0        0      337 2024-04-06 12:30:46.705493 transdoc-0.2.0/transdoc/__init__.py
+-rw-r--r--   0        0        0      201 2024-04-06 12:30:46.705493 transdoc-0.2.0/transdoc/__main__.py
+-rw-r--r--   0        0        0      228 2024-04-06 12:30:46.705493 transdoc-0.2.0/transdoc/__rule.py
+-rw-r--r--   0        0        0    10125 2024-04-06 12:30:46.705493 transdoc-0.2.0/transdoc/__transformer.py
+-rw-r--r--   0        0        0      888 2024-04-06 12:30:46.705493 transdoc-0.2.0/transdoc/errors.py
+-rw-r--r--   0        0        0        0 2024-04-06 12:30:46.705493 transdoc-0.2.0/transdoc/py.typed
+-rw-r--r--   0        0        0     4661 2024-04-06 12:30:46.705493 transdoc-0.2.0/transdoc/rules/__attributes.py
+-rw-r--r--   0        0        0      387 2024-04-06 12:30:46.705493 transdoc-0.2.0/transdoc/rules/__file_contents.py
+-rw-r--r--   0        0        0      381 2024-04-06 12:30:46.705493 transdoc-0.2.0/transdoc/rules/__init__.py
+-rw-r--r--   0        0        0     1294 2024-04-06 12:30:46.705493 transdoc-0.2.0/transdoc/rules/__markdown_docs_link.py
+-rw-r--r--   0        0        0     5068 1970-01-01 00:00:00.000000 transdoc-0.2.0/PKG-INFO
```

### Comparing `transdoc-0.1.0/LICENSE` & `transdoc-0.2.0/LICENSE`

 * *Files identical despite different names*

