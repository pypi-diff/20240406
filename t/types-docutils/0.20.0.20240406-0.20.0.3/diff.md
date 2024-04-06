# Comparing `tmp/types-docutils-0.20.0.20240406.tar.gz` & `tmp/types-docutils-0.20.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-docutils-0.20.0.20240406.tar", last modified: Sat Apr  6 02:13:13 2024, max compression
+gzip compressed data, was "types-docutils-0.20.0.3.tar", last modified: Wed Aug 16 09:13:29 2023, max compression
```

## Comparing `types-docutils-0.20.0.20240406.tar` & `types-docutils-0.20.0.3.tar`

### file list

```diff
@@ -1,64 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 02:13:13.958644 types-docutils-0.20.0.20240406/
--rw-r--r--   0 runner    (1001) docker     (127)     5629 2024-04-06 02:13:12.000000 types-docutils-0.20.0.20240406/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-06 02:13:12.000000 types-docutils-0.20.0.20240406/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-04-06 02:13:13.958644 types-docutils-0.20.0.20240406/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 02:13:13.950644 types-docutils-0.20.0.20240406/docutils-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-06 02:13:12.000000 types-docutils-0.20.0.20240406/docutils-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-04-06 02:12:57.000000 types-docutils-0.20.0.20240406/docutils-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-06 02:12:57.000000 types-docutils-0.20.0.20240406/docutils-stubs/core.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-06 02:12:57.000000 types-docutils-0.20.0.20240406/docutils-stubs/examples.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3689 2024-04-06 02:12:57.000000 types-docutils-0.20.0.20240406/docutils-stubs/frontend.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3347 2024-04-06 02:12:57.000000 types-docutils-0.20.0.20240406/docutils-stubs/io.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 02:13:13.950644 types-docutils-0.20.0.20240406/docutils-stubs/languages/
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-06 02:12:57.000000 types-docutils-0.20.0.20240406/docutils-stubs/languages/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    19320 2024-04-06 02:12:57.000000 types-docutils-0.20.0.20240406/docutils-stubs/nodes.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 02:13:13.950644 types-docutils-0.20.0.20240406/docutils-stubs/parsers/
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-06 02:12:57.000000 types-docutils-0.20.0.20240406/docutils-stubs/parsers/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-06 02:12:57.000000 types-docutils-0.20.0.20240406/docutils-stubs/parsers/null.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-06 02:12:57.000000 types-docutils-0.20.0.20240406/docutils-stubs/parsers/recommonmark_wrapper.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 02:13:13.950644 types-docutils-0.20.0.20240406/docutils-stubs/parsers/rst/
--rw-r--r--   0 runner    (1001) docker     (127)     2454 2024-04-06 02:12:57.000000 types-docutils-0.20.0.20240406/docutils-stubs/parsers/rst/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 02:13:13.954644 types-docutils-0.20.0.20240406/docutils-stubs/parsers/rst/directives/
--rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-04-06 02:12:57.000000 types-docutils-0.20.0.20240406/docutils-stubs/parsers/rst/directives/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-06 02:12:57.000000 types-docutils-0.20.0.20240406/docutils-stubs/parsers/rst/directives/admonitions.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-06 02:12:57.000000 types-docutils-0.20.0.20240406/docutils-stubs/parsers/rst/directives/body.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-06 02:12:57.000000 types-docutils-0.20.0.20240406/docutils-stubs/parsers/rst/directives/html.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-06 02:12:57.000000 types-docutils-0.20.0.20240406/docutils-stubs/parsers/rst/directives/images.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-06 02:12:57.000000 types-docutils-0.20.0.20240406/docutils-stubs/parsers/rst/directives/misc.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-06 02:12:57.000000 types-docutils-0.20.0.20240406/docutils-stubs/parsers/rst/directives/parts.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-06 02:12:57.000000 types-docutils-0.20.0.20240406/docutils-stubs/parsers/rst/directives/references.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-06 02:12:57.000000 types-docutils-0.20.0.20240406/docutils-stubs/parsers/rst/directives/tables.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3991 2024-04-06 02:12:57.000000 types-docutils-0.20.0.20240406/docutils-stubs/parsers/rst/roles.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4388 2024-04-06 02:12:57.000000 types-docutils-0.20.0.20240406/docutils-stubs/parsers/rst/states.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-04-06 02:12:57.000000 types-docutils-0.20.0.20240406/docutils-stubs/parsers/rst/tableparser.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-06 02:13:12.000000 types-docutils-0.20.0.20240406/docutils-stubs/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 02:13:13.954644 types-docutils-0.20.0.20240406/docutils-stubs/readers/
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-04-06 02:12:57.000000 types-docutils-0.20.0.20240406/docutils-stubs/readers/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-06 02:12:57.000000 types-docutils-0.20.0.20240406/docutils-stubs/readers/doctree.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-06 02:12:57.000000 types-docutils-0.20.0.20240406/docutils-stubs/readers/pep.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-06 02:12:57.000000 types-docutils-0.20.0.20240406/docutils-stubs/readers/standalone.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9550 2024-04-06 02:12:57.000000 types-docutils-0.20.0.20240406/docutils-stubs/statemachine.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 02:13:13.954644 types-docutils-0.20.0.20240406/docutils-stubs/transforms/
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-06 02:12:57.000000 types-docutils-0.20.0.20240406/docutils-stubs/transforms/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 02:13:13.954644 types-docutils-0.20.0.20240406/docutils-stubs/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     5360 2024-04-06 02:12:57.000000 types-docutils-0.20.0.20240406/docutils-stubs/utils/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 02:13:13.954644 types-docutils-0.20.0.20240406/docutils-stubs/writers/
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-06 02:12:57.000000 types-docutils-0.20.0.20240406/docutils-stubs/writers/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-06 02:12:57.000000 types-docutils-0.20.0.20240406/docutils-stubs/writers/docutils_xml.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-06 02:12:57.000000 types-docutils-0.20.0.20240406/docutils-stubs/writers/html4css1.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-06 02:12:57.000000 types-docutils-0.20.0.20240406/docutils-stubs/writers/html5_polyglot.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-06 02:12:57.000000 types-docutils-0.20.0.20240406/docutils-stubs/writers/latex2e.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-06 02:12:57.000000 types-docutils-0.20.0.20240406/docutils-stubs/writers/manpage.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-06 02:12:57.000000 types-docutils-0.20.0.20240406/docutils-stubs/writers/null.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-06 02:12:57.000000 types-docutils-0.20.0.20240406/docutils-stubs/writers/odf_odt.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-06 02:12:57.000000 types-docutils-0.20.0.20240406/docutils-stubs/writers/pep_html.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-06 02:12:57.000000 types-docutils-0.20.0.20240406/docutils-stubs/writers/pseudoxml.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-06 02:12:57.000000 types-docutils-0.20.0.20240406/docutils-stubs/writers/s5_html.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-06 02:12:57.000000 types-docutils-0.20.0.20240406/docutils-stubs/writers/xetex.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 02:13:13.958644 types-docutils-0.20.0.20240406/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3239 2024-04-06 02:13:12.000000 types-docutils-0.20.0.20240406/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 02:13:13.958644 types-docutils-0.20.0.20240406/types_docutils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-04-06 02:13:13.000000 types-docutils-0.20.0.20240406/types_docutils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-04-06 02:13:13.000000 types-docutils-0.20.0.20240406/types_docutils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 02:13:13.000000 types-docutils-0.20.0.20240406/types_docutils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-06 02:13:13.000000 types-docutils-0.20.0.20240406/types_docutils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-16 09:13:29.749210 types-docutils-0.20.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-08-16 09:13:27.000000 types-docutils-0.20.0.3/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-16 09:13:27.000000 types-docutils-0.20.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-08-16 09:13:29.749210 types-docutils-0.20.0.3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-16 09:13:29.741210 types-docutils-0.20.0.3/docutils-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-08-16 09:13:27.000000 types-docutils-0.20.0.3/docutils-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-08-16 09:13:13.000000 types-docutils-0.20.0.3/docutils-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-08-16 09:13:13.000000 types-docutils-0.20.0.3/docutils-stubs/core.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-08-16 09:13:13.000000 types-docutils-0.20.0.3/docutils-stubs/examples.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3689 2023-08-16 09:13:13.000000 types-docutils-0.20.0.3/docutils-stubs/frontend.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-08-16 09:13:13.000000 types-docutils-0.20.0.3/docutils-stubs/io.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-16 09:13:29.741210 types-docutils-0.20.0.3/docutils-stubs/languages/
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-08-16 09:13:13.000000 types-docutils-0.20.0.3/docutils-stubs/languages/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5811 2023-08-16 09:13:13.000000 types-docutils-0.20.0.3/docutils-stubs/nodes.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-16 09:13:29.741210 types-docutils-0.20.0.3/docutils-stubs/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-08-16 09:13:13.000000 types-docutils-0.20.0.3/docutils-stubs/parsers/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-16 09:13:13.000000 types-docutils-0.20.0.3/docutils-stubs/parsers/null.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-08-16 09:13:13.000000 types-docutils-0.20.0.3/docutils-stubs/parsers/recommonmark_wrapper.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-16 09:13:29.741210 types-docutils-0.20.0.3/docutils-stubs/parsers/rst/
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-08-16 09:13:13.000000 types-docutils-0.20.0.3/docutils-stubs/parsers/rst/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-16 09:13:29.741210 types-docutils-0.20.0.3/docutils-stubs/parsers/rst/directives/
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-08-16 09:13:13.000000 types-docutils-0.20.0.3/docutils-stubs/parsers/rst/directives/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-08-16 09:13:13.000000 types-docutils-0.20.0.3/docutils-stubs/parsers/rst/directives/admonitions.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-08-16 09:13:13.000000 types-docutils-0.20.0.3/docutils-stubs/parsers/rst/directives/body.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-08-16 09:13:13.000000 types-docutils-0.20.0.3/docutils-stubs/parsers/rst/directives/html.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-08-16 09:13:13.000000 types-docutils-0.20.0.3/docutils-stubs/parsers/rst/directives/images.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-08-16 09:13:13.000000 types-docutils-0.20.0.3/docutils-stubs/parsers/rst/directives/misc.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-08-16 09:13:13.000000 types-docutils-0.20.0.3/docutils-stubs/parsers/rst/directives/parts.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-08-16 09:13:13.000000 types-docutils-0.20.0.3/docutils-stubs/parsers/rst/directives/references.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-08-16 09:13:13.000000 types-docutils-0.20.0.3/docutils-stubs/parsers/rst/directives/tables.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-08-16 09:13:13.000000 types-docutils-0.20.0.3/docutils-stubs/parsers/rst/roles.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-08-16 09:13:13.000000 types-docutils-0.20.0.3/docutils-stubs/parsers/rst/states.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-16 09:13:29.745210 types-docutils-0.20.0.3/docutils-stubs/readers/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-08-16 09:13:13.000000 types-docutils-0.20.0.3/docutils-stubs/readers/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-08-16 09:13:13.000000 types-docutils-0.20.0.3/docutils-stubs/readers/doctree.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-08-16 09:13:13.000000 types-docutils-0.20.0.3/docutils-stubs/readers/pep.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-08-16 09:13:13.000000 types-docutils-0.20.0.3/docutils-stubs/readers/standalone.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-08-16 09:13:13.000000 types-docutils-0.20.0.3/docutils-stubs/statemachine.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-16 09:13:29.745210 types-docutils-0.20.0.3/docutils-stubs/transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-08-16 09:13:13.000000 types-docutils-0.20.0.3/docutils-stubs/transforms/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-16 09:13:29.745210 types-docutils-0.20.0.3/docutils-stubs/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-08-16 09:13:13.000000 types-docutils-0.20.0.3/docutils-stubs/utils/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-16 09:13:29.745210 types-docutils-0.20.0.3/docutils-stubs/writers/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-08-16 09:13:13.000000 types-docutils-0.20.0.3/docutils-stubs/writers/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-08-16 09:13:13.000000 types-docutils-0.20.0.3/docutils-stubs/writers/docutils_xml.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-08-16 09:13:13.000000 types-docutils-0.20.0.3/docutils-stubs/writers/html4css1.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-08-16 09:13:13.000000 types-docutils-0.20.0.3/docutils-stubs/writers/html5_polyglot.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-08-16 09:13:13.000000 types-docutils-0.20.0.3/docutils-stubs/writers/latex2e.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-08-16 09:13:13.000000 types-docutils-0.20.0.3/docutils-stubs/writers/manpage.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-08-16 09:13:13.000000 types-docutils-0.20.0.3/docutils-stubs/writers/null.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-08-16 09:13:13.000000 types-docutils-0.20.0.3/docutils-stubs/writers/odf_odt.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-08-16 09:13:13.000000 types-docutils-0.20.0.3/docutils-stubs/writers/pep_html.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-08-16 09:13:13.000000 types-docutils-0.20.0.3/docutils-stubs/writers/pseudoxml.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-08-16 09:13:13.000000 types-docutils-0.20.0.3/docutils-stubs/writers/s5_html.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-08-16 09:13:13.000000 types-docutils-0.20.0.3/docutils-stubs/writers/xetex.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-16 09:13:29.749210 types-docutils-0.20.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-08-16 09:13:27.000000 types-docutils-0.20.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-16 09:13:29.749210 types-docutils-0.20.0.3/types_docutils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-08-16 09:13:29.000000 types-docutils-0.20.0.3/types_docutils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-08-16 09:13:29.000000 types-docutils-0.20.0.3/types_docutils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-16 09:13:29.000000 types-docutils-0.20.0.3/types_docutils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-16 09:13:29.000000 types-docutils-0.20.0.3/types_docutils.egg-info/top_level.txt
```

### Comparing `types-docutils-0.20.0.20240406/PKG-INFO` & `types-docutils-0.20.0.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,41 +1,35 @@
 Metadata-Version: 2.1
 Name: types-docutils
-Version: 0.20.0.20240406
+Version: 0.20.0.3
 Summary: Typing stubs for docutils
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/docutils.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Typing :: Stubs Only
-Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 ## Typing stubs for docutils
 
-This is a [PEP 561](https://peps.python.org/pep-0561/)
-type stub package for the [`docutils`](https://sourceforge.net/p/docutils/code) package.
-It can be used by type-checking tools like
+This is a PEP 561 type stub package for the `docutils` package. It
+can be used by type-checking tools like
 [mypy](https://github.com/python/mypy/),
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
-`docutils`.
-
-This version of `types-docutils` aims to provide accurate annotations
-for `docutils==0.20.*`.
-The source for this package can be found at
+`docutils`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/docutils. All fixes for
 types and metadata should be contributed there.
 
 This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
 If you find that annotations are missing, feel free to contribute and help complete them.
 
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `a9d644b3ffd9e9a8bb9a01393674972573cd256b` and was tested
-with mypy 1.9.0, pyright 1.1.357, and
-pytype 2024.3.19.
+This package was generated from typeshed commit `7a7dba5e7a000bfbd3e642760e6374e3f5a4d618` and was tested
+with mypy 1.4.1, pyright 1.1.320, and
+pytype 2023.8.14.
```

### Comparing `types-docutils-0.20.0.20240406/docutils-stubs/__init__.pyi` & `types-docutils-0.20.0.3/docutils-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-docutils-0.20.0.20240406/docutils-stubs/frontend.pyi` & `types-docutils-0.20.0.3/docutils-stubs/frontend.pyi`

 * *Files identical despite different names*

### Comparing `types-docutils-0.20.0.20240406/docutils-stubs/io.pyi` & `types-docutils-0.20.0.3/docutils-stubs/io.pyi`

 * *Files 26% similar despite different names*

```diff
@@ -4,40 +4,31 @@
     OpenBinaryModeWriting,
     OpenTextModeReading,
     OpenTextModeWriting,
     SupportsWrite,
     Unused,
 )
 from re import Pattern
-from typing import IO, Any, ClassVar, Generic, Literal, TypeVar
+from typing import Any, ClassVar
+from typing_extensions import Literal
 
-from docutils import TransformSpec, nodes
+from docutils import TransformSpec
 
 __docformat__: str
 
 class InputError(OSError): ...
 class OutputError(OSError): ...
 
 def check_encoding(stream: Any, encoding: str) -> bool | None: ...
 def error_string(err: BaseException) -> str: ...
 
-_S = TypeVar("_S")
-
-class Input(TransformSpec, Generic[_S]):
+class Input(TransformSpec):
     component_type: ClassVar[str]
     default_source_path: ClassVar[str | None]
-    encoding: str | None
-    error_handler: str
-    source: _S | None
-    source_path: str | None
-    successful_encoding: str | None = None
-    def __init__(
-        self, source: _S | None = None, source_path: str | None = None, encoding: str | None = None, error_handler: str = "strict"
-    ) -> None: ...
-    def read(self) -> str: ...
+    def read(self) -> Any: ...
     def decode(self, data: str | bytes | bytearray) -> str: ...
     coding_slug: ClassVar[Pattern[bytes]]
     byte_order_marks: ClassVar[tuple[tuple[bytes, str], ...]]
     def determine_encoding_from_data(self, data: str | bytes | bytearray) -> str | None: ...
     def isatty(self) -> bool: ...
 
 class Output(TransformSpec):
@@ -61,15 +52,15 @@
         encoding_errors: str = "backslashreplace",
         decoding_errors: str = "replace",
     ) -> None: ...
     def write(self, data: str | bytes | Exception) -> None: ...
     def close(self) -> None: ...
     def isatty(self) -> bool: ...
 
-class FileInput(Input[IO[str]]):
+class FileInput(Input):
     def __init__(
         self,
         source: Incomplete | None = None,
         source_path: Incomplete | None = None,
         encoding: str | None = None,
         error_handler: str = "strict",
         autoclose: bool = True,
@@ -81,24 +72,24 @@
 
 class FileOutput(Output):
     mode: ClassVar[OpenTextModeWriting | OpenBinaryModeWriting]
     def __getattr__(self, name: str) -> Incomplete: ...
 
 class BinaryFileOutput(FileOutput): ...
 
-class StringInput(Input[str]):
+class StringInput(Input):
     default_source_path: ClassVar[str]
 
 class StringOutput(Output):
     default_destination_path: ClassVar[str]
     destination: str | bytes  # only defined after call to write()
 
-class NullInput(Input[Any]):
+class NullInput(Input):
     default_source_path: ClassVar[str]
     def read(self) -> str: ...
 
 class NullOutput(Output):
     default_destination_path: ClassVar[str]
     def write(self, data: Unused) -> None: ...
 
-class DocTreeInput(Input[nodes.document]):
+class DocTreeInput(Input):
     default_source_path: ClassVar[str]
```

### Comparing `types-docutils-0.20.0.20240406/docutils-stubs/parsers/__init__.pyi` & `types-docutils-0.20.0.3/docutils-stubs/parsers/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-docutils-0.20.0.20240406/setup.py` & `types-docutils-0.20.0.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,55 +1,49 @@
 from setuptools import setup
 
 name = "types-docutils"
 description = "Typing stubs for docutils"
 long_description = '''
 ## Typing stubs for docutils
 
-This is a [PEP 561](https://peps.python.org/pep-0561/)
-type stub package for the [`docutils`](https://sourceforge.net/p/docutils/code) package.
-It can be used by type-checking tools like
+This is a PEP 561 type stub package for the `docutils` package. It
+can be used by type-checking tools like
 [mypy](https://github.com/python/mypy/),
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
-`docutils`.
-
-This version of `types-docutils` aims to provide accurate annotations
-for `docutils==0.20.*`.
-The source for this package can be found at
+`docutils`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/docutils. All fixes for
 types and metadata should be contributed there.
 
 This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
 If you find that annotations are missing, feel free to contribute and help complete them.
 
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `a9d644b3ffd9e9a8bb9a01393674972573cd256b` and was tested
-with mypy 1.9.0, pyright 1.1.357, and
-pytype 2024.3.19.
+This package was generated from typeshed commit `7a7dba5e7a000bfbd3e642760e6374e3f5a4d618` and was tested
+with mypy 1.4.1, pyright 1.1.320, and
+pytype 2023.8.14.
 '''.lstrip()
 
 setup(name=name,
-      version="0.20.0.20240406",
+      version="0.20.0.3",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/docutils.md",
           "Issue tracker": "https://github.com/python/typeshed/issues",
           "Chat": "https://gitter.im/python/typing",
       },
       install_requires=[],
       packages=['docutils-stubs'],
-      package_data={'docutils-stubs': ['__init__.pyi', 'core.pyi', 'examples.pyi', 'frontend.pyi', 'io.pyi', 'languages/__init__.pyi', 'nodes.pyi', 'parsers/__init__.pyi', 'parsers/null.pyi', 'parsers/recommonmark_wrapper.pyi', 'parsers/rst/__init__.pyi', 'parsers/rst/directives/__init__.pyi', 'parsers/rst/directives/admonitions.pyi', 'parsers/rst/directives/body.pyi', 'parsers/rst/directives/html.pyi', 'parsers/rst/directives/images.pyi', 'parsers/rst/directives/misc.pyi', 'parsers/rst/directives/parts.pyi', 'parsers/rst/directives/references.pyi', 'parsers/rst/directives/tables.pyi', 'parsers/rst/roles.pyi', 'parsers/rst/states.pyi', 'parsers/rst/tableparser.pyi', 'readers/__init__.pyi', 'readers/doctree.pyi', 'readers/pep.pyi', 'readers/standalone.pyi', 'statemachine.pyi', 'transforms/__init__.pyi', 'utils/__init__.pyi', 'writers/__init__.pyi', 'writers/docutils_xml.pyi', 'writers/html4css1.pyi', 'writers/html5_polyglot.pyi', 'writers/latex2e.pyi', 'writers/manpage.pyi', 'writers/null.pyi', 'writers/odf_odt.pyi', 'writers/pep_html.pyi', 'writers/pseudoxml.pyi', 'writers/s5_html.pyi', 'writers/xetex.pyi', 'METADATA.toml', 'py.typed']},
+      package_data={'docutils-stubs': ['__init__.pyi', 'core.pyi', 'examples.pyi', 'frontend.pyi', 'io.pyi', 'languages/__init__.pyi', 'nodes.pyi', 'parsers/__init__.pyi', 'parsers/null.pyi', 'parsers/recommonmark_wrapper.pyi', 'parsers/rst/__init__.pyi', 'parsers/rst/directives/__init__.pyi', 'parsers/rst/directives/admonitions.pyi', 'parsers/rst/directives/body.pyi', 'parsers/rst/directives/html.pyi', 'parsers/rst/directives/images.pyi', 'parsers/rst/directives/misc.pyi', 'parsers/rst/directives/parts.pyi', 'parsers/rst/directives/references.pyi', 'parsers/rst/directives/tables.pyi', 'parsers/rst/roles.pyi', 'parsers/rst/states.pyi', 'readers/__init__.pyi', 'readers/doctree.pyi', 'readers/pep.pyi', 'readers/standalone.pyi', 'statemachine.pyi', 'transforms/__init__.pyi', 'utils/__init__.pyi', 'writers/__init__.pyi', 'writers/docutils_xml.pyi', 'writers/html4css1.pyi', 'writers/html5_polyglot.pyi', 'writers/latex2e.pyi', 'writers/manpage.pyi', 'writers/null.pyi', 'writers/odf_odt.pyi', 'writers/pep_html.pyi', 'writers/pseudoxml.pyi', 'writers/s5_html.pyi', 'writers/xetex.pyi', 'METADATA.toml', 'py.typed']},
       license="Apache-2.0 license",
-      python_requires=">=3.8",
       classifiers=[
           "License :: OSI Approved :: Apache Software License",
           "Programming Language :: Python :: 3",
           "Typing :: Stubs Only",
       ]
 )
```

### Comparing `types-docutils-0.20.0.20240406/types_docutils.egg-info/PKG-INFO` & `types-docutils-0.20.0.3/types_docutils.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,41 +1,35 @@
 Metadata-Version: 2.1
 Name: types-docutils
-Version: 0.20.0.20240406
+Version: 0.20.0.3
 Summary: Typing stubs for docutils
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/docutils.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Typing :: Stubs Only
-Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 ## Typing stubs for docutils
 
-This is a [PEP 561](https://peps.python.org/pep-0561/)
-type stub package for the [`docutils`](https://sourceforge.net/p/docutils/code) package.
-It can be used by type-checking tools like
+This is a PEP 561 type stub package for the `docutils` package. It
+can be used by type-checking tools like
 [mypy](https://github.com/python/mypy/),
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
-`docutils`.
-
-This version of `types-docutils` aims to provide accurate annotations
-for `docutils==0.20.*`.
-The source for this package can be found at
+`docutils`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/docutils. All fixes for
 types and metadata should be contributed there.
 
 This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
 If you find that annotations are missing, feel free to contribute and help complete them.
 
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `a9d644b3ffd9e9a8bb9a01393674972573cd256b` and was tested
-with mypy 1.9.0, pyright 1.1.357, and
-pytype 2024.3.19.
+This package was generated from typeshed commit `7a7dba5e7a000bfbd3e642760e6374e3f5a4d618` and was tested
+with mypy 1.4.1, pyright 1.1.320, and
+pytype 2023.8.14.
```

### Comparing `types-docutils-0.20.0.20240406/types_docutils.egg-info/SOURCES.txt` & `types-docutils-0.20.0.3/types_docutils.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -4,24 +4,22 @@
 docutils-stubs/METADATA.toml
 docutils-stubs/__init__.pyi
 docutils-stubs/core.pyi
 docutils-stubs/examples.pyi
 docutils-stubs/frontend.pyi
 docutils-stubs/io.pyi
 docutils-stubs/nodes.pyi
-docutils-stubs/py.typed
 docutils-stubs/statemachine.pyi
 docutils-stubs/languages/__init__.pyi
 docutils-stubs/parsers/__init__.pyi
 docutils-stubs/parsers/null.pyi
 docutils-stubs/parsers/recommonmark_wrapper.pyi
 docutils-stubs/parsers/rst/__init__.pyi
 docutils-stubs/parsers/rst/roles.pyi
 docutils-stubs/parsers/rst/states.pyi
-docutils-stubs/parsers/rst/tableparser.pyi
 docutils-stubs/parsers/rst/directives/__init__.pyi
 docutils-stubs/parsers/rst/directives/admonitions.pyi
 docutils-stubs/parsers/rst/directives/body.pyi
 docutils-stubs/parsers/rst/directives/html.pyi
 docutils-stubs/parsers/rst/directives/images.pyi
 docutils-stubs/parsers/rst/directives/misc.pyi
 docutils-stubs/parsers/rst/directives/parts.pyi
```

