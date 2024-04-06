# Comparing `tmp/legal_citation_parser-0.1.1.tar.gz` & `tmp/legal_citation_parser-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "legal_citation_parser-0.1.1.tar", last modified: Sat Apr  6 20:45:17 2024, max compression
+gzip compressed data, was "legal_citation_parser-0.1.2.tar", last modified: Sat Apr  6 21:10:24 2024, max compression
```

## Comparing `legal_citation_parser-0.1.1.tar` & `legal_citation_parser-0.1.2.tar`

### file list

```diff
@@ -1,12 +1,18 @@
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-06 20:45:17.778287 legal_citation_parser-0.1.1/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)    35149 2024-03-22 00:07:43.000000 legal_citation_parser-0.1.1/LICENSE
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      205 2024-04-06 20:45:17.778287 legal_citation_parser-0.1.1/PKG-INFO
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     2019 2024-04-06 19:14:15.000000 legal_citation_parser-0.1.1/README.md
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-06 20:45:17.778287 legal_citation_parser-0.1.1/legal_citation_parser.egg-info/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      205 2024-04-06 20:45:17.000000 legal_citation_parser-0.1.1/legal_citation_parser.egg-info/PKG-INFO
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      250 2024-04-06 20:45:17.000000 legal_citation_parser-0.1.1/legal_citation_parser.egg-info/SOURCES.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        1 2024-04-06 20:45:17.000000 legal_citation_parser-0.1.1/legal_citation_parser.egg-info/dependency_links.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        9 2024-04-06 20:45:17.000000 legal_citation_parser-0.1.1/legal_citation_parser.egg-info/requires.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        1 2024-04-06 20:45:17.000000 legal_citation_parser-0.1.1/legal_citation_parser.egg-info/top_level.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       38 2024-04-06 20:45:17.778287 legal_citation_parser-0.1.1/setup.cfg
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      299 2024-04-06 20:41:02.000000 legal_citation_parser-0.1.1/setup.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-06 21:10:24.038391 legal_citation_parser-0.1.2/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)    35149 2024-03-22 00:07:43.000000 legal_citation_parser-0.1.2/LICENSE
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      205 2024-04-06 21:10:24.038391 legal_citation_parser-0.1.2/PKG-INFO
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     2019 2024-04-06 19:14:15.000000 legal_citation_parser-0.1.2/README.md
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-06 21:10:24.038391 legal_citation_parser-0.1.2/legal_citation_parser/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2024-04-06 20:51:57.000000 legal_citation_parser-0.1.2/legal_citation_parser/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)    32460 2024-04-06 18:41:34.000000 legal_citation_parser-0.1.2/legal_citation_parser/canlii_constants.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     6244 2024-04-06 20:36:18.000000 legal_citation_parser-0.1.2/legal_citation_parser/canlii_rules.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      958 2024-04-06 20:39:48.000000 legal_citation_parser-0.1.2/legal_citation_parser/citation_parser.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      537 2024-04-06 20:05:11.000000 legal_citation_parser-0.1.2/legal_citation_parser/utils.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-06 21:10:24.038391 legal_citation_parser-0.1.2/legal_citation_parser.egg-info/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      205 2024-04-06 21:10:24.000000 legal_citation_parser-0.1.2/legal_citation_parser.egg-info/PKG-INFO
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      436 2024-04-06 21:10:24.000000 legal_citation_parser-0.1.2/legal_citation_parser.egg-info/SOURCES.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        1 2024-04-06 21:10:24.000000 legal_citation_parser-0.1.2/legal_citation_parser.egg-info/dependency_links.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        9 2024-04-06 21:10:24.000000 legal_citation_parser-0.1.2/legal_citation_parser.egg-info/requires.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       22 2024-04-06 21:10:24.000000 legal_citation_parser-0.1.2/legal_citation_parser.egg-info/top_level.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       38 2024-04-06 21:10:24.038391 legal_citation_parser-0.1.2/setup.cfg
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      299 2024-04-06 21:09:57.000000 legal_citation_parser-0.1.2/setup.py
```

### Comparing `legal_citation_parser-0.1.1/LICENSE` & `legal_citation_parser-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `legal_citation_parser-0.1.1/README.md` & `legal_citation_parser-0.1.2/README.md`

 * *Files identical despite different names*

