# Comparing `tmp/legal_citation_parser-0.1.tar.gz` & `tmp/legal_citation_parser-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "legal_citation_parser-0.1.tar", last modified: Sat Apr  6 20:21:29 2024, max compression
+gzip compressed data, was "legal_citation_parser-0.1.1.tar", last modified: Sat Apr  6 20:45:17 2024, max compression
```

## Comparing `legal_citation_parser-0.1.tar` & `legal_citation_parser-0.1.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-06 20:21:29.963556 legal_citation_parser-0.1/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)    35149 2024-03-22 00:07:43.000000 legal_citation_parser-0.1/LICENSE
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      203 2024-04-06 20:21:29.963556 legal_citation_parser-0.1/PKG-INFO
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     2019 2024-04-06 19:14:15.000000 legal_citation_parser-0.1/README.md
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-06 20:21:29.963556 legal_citation_parser-0.1/legal_citation_parser.egg-info/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      203 2024-04-06 20:21:29.000000 legal_citation_parser-0.1/legal_citation_parser.egg-info/PKG-INFO
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      250 2024-04-06 20:21:29.000000 legal_citation_parser-0.1/legal_citation_parser.egg-info/SOURCES.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        1 2024-04-06 20:21:29.000000 legal_citation_parser-0.1/legal_citation_parser.egg-info/dependency_links.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        9 2024-04-06 20:21:29.000000 legal_citation_parser-0.1/legal_citation_parser.egg-info/requires.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        1 2024-04-06 20:21:29.000000 legal_citation_parser-0.1/legal_citation_parser.egg-info/top_level.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       38 2024-04-06 20:21:29.963556 legal_citation_parser-0.1/setup.cfg
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      297 2024-04-06 20:18:50.000000 legal_citation_parser-0.1/setup.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-06 20:45:17.778287 legal_citation_parser-0.1.1/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)    35149 2024-03-22 00:07:43.000000 legal_citation_parser-0.1.1/LICENSE
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      205 2024-04-06 20:45:17.778287 legal_citation_parser-0.1.1/PKG-INFO
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     2019 2024-04-06 19:14:15.000000 legal_citation_parser-0.1.1/README.md
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-06 20:45:17.778287 legal_citation_parser-0.1.1/legal_citation_parser.egg-info/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      205 2024-04-06 20:45:17.000000 legal_citation_parser-0.1.1/legal_citation_parser.egg-info/PKG-INFO
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      250 2024-04-06 20:45:17.000000 legal_citation_parser-0.1.1/legal_citation_parser.egg-info/SOURCES.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        1 2024-04-06 20:45:17.000000 legal_citation_parser-0.1.1/legal_citation_parser.egg-info/dependency_links.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        9 2024-04-06 20:45:17.000000 legal_citation_parser-0.1.1/legal_citation_parser.egg-info/requires.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        1 2024-04-06 20:45:17.000000 legal_citation_parser-0.1.1/legal_citation_parser.egg-info/top_level.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       38 2024-04-06 20:45:17.778287 legal_citation_parser-0.1.1/setup.cfg
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      299 2024-04-06 20:41:02.000000 legal_citation_parser-0.1.1/setup.py
```

### Comparing `legal_citation_parser-0.1/LICENSE` & `legal_citation_parser-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `legal_citation_parser-0.1/README.md` & `legal_citation_parser-0.1.1/README.md`

 * *Files identical despite different names*

