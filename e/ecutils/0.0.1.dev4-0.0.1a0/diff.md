# Comparing `tmp/ecutils-0.0.1.dev4.tar.gz` & `tmp/ecutils-0.0.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecutils-0.0.1.dev4.tar", last modified: Wed Oct  4 03:22:23 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `ecutils-0.0.1.dev4.tar` & `ecutils-0.0.1a0.tar`

### file list

```diff
@@ -1,21 +1,30 @@
-drwxr-xr-x   0 upy       (1000) upy       (1000)        0 2023-10-04 03:22:23.111471 ecutils-0.0.1.dev4/
--rwxrwxrwx   0 upy       (1000) upy       (1000)     1068 2023-10-01 22:16:37.000000 ecutils-0.0.1.dev4/LICENSE.md
--rwxrwxrwx   0 upy       (1000) upy       (1000)       51 2023-10-01 22:16:37.000000 ecutils-0.0.1.dev4/MANIFEST.in
--rw-r--r--   0 upy       (1000) upy       (1000)     7816 2023-10-04 03:22:23.111471 ecutils-0.0.1.dev4/PKG-INFO
--rwxrwxrwx   0 upy       (1000) upy       (1000)     7025 2023-10-01 22:52:33.000000 ecutils-0.0.1.dev4/README.md
--rwxrwxrwx   0 upy       (1000) upy       (1000)       77 2023-10-04 03:22:23.112471 ecutils-0.0.1.dev4/setup.cfg
--rwxr-xr-x   0 upy       (1000) upy       (1000)     1177 2023-10-04 03:20:48.000000 ecutils-0.0.1.dev4/setup.py
--rwxrwxrwx   0 upy       (1000) upy       (1000)       82 2023-10-01 22:16:37.000000 ecutils-0.0.1.dev4/setup.toml
-drwxr-xr-x   0 upy       (1000) upy       (1000)        0 2023-10-04 03:22:23.110471 ecutils-0.0.1.dev4/src/
-drwxr-xr-x   0 upy       (1000) upy       (1000)        0 2023-10-04 03:22:23.111471 ecutils-0.0.1.dev4/src/ecutils/
--rwxrwxrwx   0 upy       (1000) upy       (1000)      196 2023-10-01 22:20:38.000000 ecutils-0.0.1.dev4/src/ecutils/__init__.py
--rwxrwxrwx   0 upy       (1000) upy       (1000)    11015 2023-10-04 03:18:38.000000 ecutils-0.0.1.dev4/src/ecutils/ec.py
--rwxrwxrwx   0 upy       (1000) upy       (1000)     1142 2023-10-01 22:21:20.000000 ecutils-0.0.1.dev4/src/ecutils/ecdh.py
--rwxrwxrwx   0 upy       (1000) upy       (1000)     1980 2023-10-04 02:02:11.000000 ecutils-0.0.1.dev4/src/ecutils/ecdsa.py
--rwxrwxrwx   0 upy       (1000) upy       (1000)     1786 2023-10-01 22:21:13.000000 ecutils-0.0.1.dev4/src/ecutils/eck.py
--rwxrwxrwx   0 upy       (1000) upy       (1000)     1467 2023-10-01 22:54:03.000000 ecutils-0.0.1.dev4/src/ecutils/ecmo.py
-drwxr-xr-x   0 upy       (1000) upy       (1000)        0 2023-10-04 03:22:23.111471 ecutils-0.0.1.dev4/src/ecutils.egg-info/
--rw-r--r--   0 upy       (1000) upy       (1000)     7816 2023-10-04 03:22:23.000000 ecutils-0.0.1.dev4/src/ecutils.egg-info/PKG-INFO
--rw-r--r--   0 upy       (1000) upy       (1000)      324 2023-10-04 03:22:23.000000 ecutils-0.0.1.dev4/src/ecutils.egg-info/SOURCES.txt
--rw-r--r--   0 upy       (1000) upy       (1000)        1 2023-10-04 03:22:23.000000 ecutils-0.0.1.dev4/src/ecutils.egg-info/dependency_links.txt
--rw-r--r--   0 upy       (1000) upy       (1000)        8 2023-10-04 03:22:23.000000 ecutils-0.0.1.dev4/src/ecutils.egg-info/top_level.txt
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 ecutils-0.0.1a0/.readthedocs.yaml
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 ecutils-0.0.1a0/CHANGELOG.md
+-rw-r--r--   0        0        0     1808 2020-02-02 00:00:00.000000 ecutils-0.0.1a0/mkdocs.yml
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 ecutils-0.0.1a0/requirements-docs.txt
+-rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 ecutils-0.0.1a0/docs/index.md
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 ecutils-0.0.1a0/docs/installation.md
+-rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 ecutils-0.0.1a0/docs/usage.md
+-rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 ecutils-0.0.1a0/docs/algorithms/digital_signature.md
+-rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 ecutils-0.0.1a0/docs/algorithms/koblitz.md
+-rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 ecutils-0.0.1a0/docs/core/elliptic_curve.md
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 ecutils-0.0.1a0/docs/core/point.md
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 ecutils-0.0.1a0/docs/protocols/diffie_hellman.md
+-rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 ecutils-0.0.1a0/docs/protocols/massey_omura.md
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 ecutils-0.0.1a0/docs/reference/curves.md
+-rwxr-xr-x   0        0        0       25 2020-02-02 00:00:00.000000 ecutils-0.0.1a0/src/ecutils/__init__.py
+-rw-r--r--   0        0        0     7437 2020-02-02 00:00:00.000000 ecutils-0.0.1a0/src/ecutils/algorithms.py
+-rwxr-xr-x   0        0        0     4100 2020-02-02 00:00:00.000000 ecutils-0.0.1a0/src/ecutils/core.py
+-rw-r--r--   0        0        0     5269 2020-02-02 00:00:00.000000 ecutils-0.0.1a0/src/ecutils/curves.py
+-rw-r--r--   0        0        0     3037 2020-02-02 00:00:00.000000 ecutils-0.0.1a0/src/ecutils/protocols.py
+-rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 ecutils-0.0.1a0/tests/test_diffie_hellman.py
+-rw-r--r--   0        0        0     1339 2020-02-02 00:00:00.000000 ecutils-0.0.1a0/tests/test_digital_signature.py
+-rw-r--r--   0        0        0     8614 2020-02-02 00:00:00.000000 ecutils-0.0.1a0/tests/test_elliptic_curve_operations.py
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 ecutils-0.0.1a0/tests/test_get_curve.py
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 ecutils-0.0.1a0/tests/test_koblitz.py
+-rw-r--r--   0        0        0     1397 2020-02-02 00:00:00.000000 ecutils-0.0.1a0/tests/test_massey_omura.py
+-rwxr-xr-x   0        0        0       93 2020-02-02 00:00:00.000000 ecutils-0.0.1a0/.gitignore
+-rwxr-xr-x   0        0        0     1089 2020-02-02 00:00:00.000000 ecutils-0.0.1a0/LICENSE.md
+-rwxr-xr-x   0        0        0     3321 2020-02-02 00:00:00.000000 ecutils-0.0.1a0/README.md
+-rw-r--r--   0        0        0     1309 2020-02-02 00:00:00.000000 ecutils-0.0.1a0/pyproject.toml
+-rw-r--r--   0        0        0     5596 2020-02-02 00:00:00.000000 ecutils-0.0.1a0/PKG-INFO
```

### Comparing `ecutils-0.0.1.dev4/LICENSE.md` & `ecutils-0.0.1a0/LICENSE.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 
-Copyright (c) 2022 Isak Ruas
+Copyright (c) 2022-2023 Isak Ruas, Celimar Paiva.
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

