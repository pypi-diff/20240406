# Comparing `tmp/mat3ra-fixtures-2024.3.21.post2.tar.gz` & `tmp/mat3ra-fixtures-2024.4.6.post0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mat3ra-fixtures-2024.3.21.post2.tar", last modified: Thu Mar 21 21:36:53 2024, max compression
+gzip compressed data, was "mat3ra-fixtures-2024.4.6.post0.tar", last modified: Sat Apr  6 03:23:59 2024, max compression
```

## Comparing `mat3ra-fixtures-2024.3.21.post2.tar` & `mat3ra-fixtures-2024.4.6.post0.tar`

### file list

```diff
@@ -1,46 +1,243 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 21:36:53.420641 mat3ra-fixtures-2024.3.21.post2/
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-03-21 21:36:36.000000 mat3ra-fixtures-2024.3.21.post2/.babelrc
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-21 21:36:36.000000 mat3ra-fixtures-2024.3.21.post2/.eslintrc.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 21:36:53.412640 mat3ra-fixtures-2024.3.21.post2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 21:36:53.416640 mat3ra-fixtures-2024.3.21.post2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     3800 2024-03-21 21:36:36.000000 mat3ra-fixtures-2024.3.21.post2/.github/workflows/cicd.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3222 2024-03-21 21:36:36.000000 mat3ra-fixtures-2024.3.21.post2/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 21:36:53.416640 mat3ra-fixtures-2024.3.21.post2/.husky/
--rwxr-xr-x   0 runner    (1001) docker     (127)      457 2024-03-21 21:36:36.000000 mat3ra-fixtures-2024.3.21.post2/.husky/pre-commit
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-03-21 21:36:36.000000 mat3ra-fixtures-2024.3.21.post2/.mocharc.json
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-03-21 21:36:36.000000 mat3ra-fixtures-2024.3.21.post2/.npmignore
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-03-21 21:36:36.000000 mat3ra-fixtures-2024.3.21.post2/.nycrc
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-03-21 21:36:36.000000 mat3ra-fixtures-2024.3.21.post2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-03-21 21:36:36.000000 mat3ra-fixtures-2024.3.21.post2/.prettierrc
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-03-21 21:36:36.000000 mat3ra-fixtures-2024.3.21.post2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-03-21 21:36:53.420641 mat3ra-fixtures-2024.3.21.post2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-03-21 21:36:36.000000 mat3ra-fixtures-2024.3.21.post2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)   307578 2024-03-21 21:36:36.000000 mat3ra-fixtures-2024.3.21.post2/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (127)     2469 2024-03-21 21:36:36.000000 mat3ra-fixtures-2024.3.21.post2/package.json
--rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-03-21 21:36:36.000000 mat3ra-fixtures-2024.3.21.post2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-21 21:36:53.420641 mat3ra-fixtures-2024.3.21.post2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 21:36:53.412640 mat3ra-fixtures-2024.3.21.post2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 21:36:53.416640 mat3ra-fixtures-2024.3.21.post2/src/js/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-03-21 21:36:36.000000 mat3ra-fixtures-2024.3.21.post2/src/js/index.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 21:36:53.416640 mat3ra-fixtures-2024.3.21.post2/src/py/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 21:36:36.000000 mat3ra-fixtures-2024.3.21.post2/src/py/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 21:36:53.420641 mat3ra-fixtures-2024.3.21.post2/src/py/mat3ra/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 21:36:36.000000 mat3ra-fixtures-2024.3.21.post2/src/py/mat3ra/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 21:36:53.420641 mat3ra-fixtures-2024.3.21.post2/src/py/mat3ra/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-03-21 21:36:36.000000 mat3ra-fixtures-2024.3.21.post2/src/py/mat3ra/fixtures/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 21:36:53.420641 mat3ra-fixtures-2024.3.21.post2/src/py/mat3ra_fixtures.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-03-21 21:36:53.000000 mat3ra-fixtures-2024.3.21.post2/src/py/mat3ra_fixtures.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-03-21 21:36:53.000000 mat3ra-fixtures-2024.3.21.post2/src/py/mat3ra_fixtures.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-21 21:36:53.000000 mat3ra-fixtures-2024.3.21.post2/src/py/mat3ra_fixtures.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-03-21 21:36:53.000000 mat3ra-fixtures-2024.3.21.post2/src/py/mat3ra_fixtures.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-21 21:36:53.000000 mat3ra-fixtures-2024.3.21.post2/src/py/mat3ra_fixtures.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 21:36:53.416640 mat3ra-fixtures-2024.3.21.post2/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 21:36:53.420641 mat3ra-fixtures-2024.3.21.post2/tests/js/
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-03-21 21:36:36.000000 mat3ra-fixtures-2024.3.21.post2/tests/js/babel-register.js
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-03-21 21:36:36.000000 mat3ra-fixtures-2024.3.21.post2/tests/js/greeting.test.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 21:36:53.420641 mat3ra-fixtures-2024.3.21.post2/tests/py/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 21:36:36.000000 mat3ra-fixtures-2024.3.21.post2/tests/py/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 21:36:53.420641 mat3ra-fixtures-2024.3.21.post2/tests/py/unit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 21:36:36.000000 mat3ra-fixtures-2024.3.21.post2/tests/py/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-03-21 21:36:36.000000 mat3ra-fixtures-2024.3.21.post2/tests/py/unit/test_sample.py
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-03-21 21:36:36.000000 mat3ra-fixtures-2024.3.21.post2/tsconfig.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 03:23:59.123716 mat3ra-fixtures-2024.4.6.post0/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/.babelrc
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/.eslintrc.json
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 03:23:59.051716 mat3ra-fixtures-2024.4.6.post0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 03:23:59.063716 mat3ra-fixtures-2024.4.6.post0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3800 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/.github/workflows/cicd.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3232 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 03:23:59.063716 mat3ra-fixtures-2024.4.6.post0/.husky/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      351 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/.husky/post-checkout
+-rwxr-xr-x   0 runner    (1001) docker     (127)      347 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/.husky/post-commit
+-rwxr-xr-x   0 runner    (1001) docker     (127)      345 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/.husky/post-merge
+-rwxr-xr-x   0 runner    (1001) docker     (127)      457 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/.husky/pre-commit
+-rwxr-xr-x   0 runner    (1001) docker     (127)      341 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/.husky/pre-push
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/.mocharc.json
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/.npmignore
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/.nycrc
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/.prettierrc
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3135 2024-04-06 03:23:59.123716 mat3ra-fixtures-2024.4.6.post0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 03:23:59.051716 mat3ra-fixtures-2024.4.6.post0/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 03:23:59.051716 mat3ra-fixtures-2024.4.6.post0/data/applications/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 03:23:59.051716 mat3ra-fixtures-2024.4.6.post0/data/applications/espresso/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 03:23:59.063716 mat3ra-fixtures-2024.4.6.post0/data/applications/espresso/5.4.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 03:23:59.063716 mat3ra-fixtures-2024.4.6.post0/data/applications/espresso/5.4.0/case-001/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 03:23:59.051716 mat3ra-fixtures-2024.4.6.post0/data/applications/espresso/5.4.0/case-001/outdir/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 03:23:59.067716 mat3ra-fixtures-2024.4.6.post0/data/applications/espresso/5.4.0/case-001/outdir/__prefix__.save/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 03:23:59.067716 mat3ra-fixtures-2024.4.6.post0/data/applications/espresso/5.4.0/case-001/outdir/__prefix__.save/K00001/
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/data/applications/espresso/5.4.0/case-001/outdir/__prefix__.save/K00001/eigenval.xml
+-rw-r--r--   0 runner    (1001) docker     (127)   160469 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/data/applications/espresso/5.4.0/case-001/outdir/__prefix__.save/K00001/evc.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    21019 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/data/applications/espresso/5.4.0/case-001/outdir/__prefix__.save/K00001/gkvectors.dat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 03:23:59.067716 mat3ra-fixtures-2024.4.6.post0/data/applications/espresso/5.4.0/case-001/outdir/__prefix__.save/K00002/
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/data/applications/espresso/5.4.0/case-001/outdir/__prefix__.save/K00002/eigenval.xml
+-rw-r--r--   0 runner    (1001) docker     (127)   151125 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/data/applications/espresso/5.4.0/case-001/outdir/__prefix__.save/K00002/evc.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    19851 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/data/applications/espresso/5.4.0/case-001/outdir/__prefix__.save/K00002/gkvectors.dat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 03:23:59.071716 mat3ra-fixtures-2024.4.6.post0/data/applications/espresso/5.4.0/case-001/outdir/__prefix__.save/K00003/
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/data/applications/espresso/5.4.0/case-001/outdir/__prefix__.save/K00003/eigenval.xml
+-rw-r--r--   0 runner    (1001) docker     (127)   151125 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/data/applications/espresso/5.4.0/case-001/outdir/__prefix__.save/K00003/evc.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    19851 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/data/applications/espresso/5.4.0/case-001/outdir/__prefix__.save/K00003/gkvectors.dat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 03:23:59.071716 mat3ra-fixtures-2024.4.6.post0/data/applications/espresso/5.4.0/case-001/outdir/__prefix__.save/K00004/
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/data/applications/espresso/5.4.0/case-001/outdir/__prefix__.save/K00004/eigenval.xml
+-rw-r--r--   0 runner    (1001) docker     (127)   150101 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/data/applications/espresso/5.4.0/case-001/outdir/__prefix__.save/K00004/evc.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    19723 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/data/applications/espresso/5.4.0/case-001/outdir/__prefix__.save/K00004/gkvectors.dat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 03:23:59.071716 mat3ra-fixtures-2024.4.6.post0/data/applications/espresso/5.4.0/case-001/outdir/__prefix__.save/K00005/
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/data/applications/espresso/5.4.0/case-001/outdir/__prefix__.save/K00005/eigenval.xml
+-rw-r--r--   0 runner    (1001) docker     (127)   151125 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/data/applications/espresso/5.4.0/case-001/outdir/__prefix__.save/K00005/evc.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    19851 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/data/applications/espresso/5.4.0/case-001/outdir/__prefix__.save/K00005/gkvectors.dat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 03:23:59.071716 mat3ra-fixtures-2024.4.6.post0/data/applications/espresso/5.4.0/case-001/outdir/__prefix__.save/K00006/
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/data/applications/espresso/5.4.0/case-001/outdir/__prefix__.save/K00006/eigenval.xml
+-rw-r--r--   0 runner    (1001) docker     (127)   150101 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/data/applications/espresso/5.4.0/case-001/outdir/__prefix__.save/K00006/evc.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    19723 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/data/applications/espresso/5.4.0/case-001/outdir/__prefix__.save/K00006/gkvectors.dat
+-rw-r--r--   0 runner    (1001) docker     (127)   377892 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/data/applications/espresso/5.4.0/case-001/outdir/__prefix__.save/charge-density.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    17304 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/data/applications/espresso/5.4.0/case-001/outdir/__prefix__.save/data-file.xml
+-rw-r--r--   0 runner    (1001) docker     (127)   160388 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/data/applications/espresso/5.4.0/case-001/outdir/__prefix__.save/gvectors.dat
+-rw-r--r--   0 runner    (1001) docker     (127)   577640 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/data/applications/espresso/5.4.0/case-001/outdir/__prefix__.save/si_pbe_gbrv_1.0.upf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 03:23:59.071716 mat3ra-fixtures-2024.4.6.post0/data/applications/espresso/5.4.0/case-001/pseudo/
+-rw-r--r--   0 runner    (1001) docker     (127)   577640 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/data/applications/espresso/5.4.0/case-001/pseudo/si_pbe_gbrv_1.0.upf
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/data/applications/espresso/5.4.0/case-001/pw-scf.in
+-rw-r--r--   0 runner    (1001) docker     (127)    11469 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/data/applications/espresso/5.4.0/case-001/pw-scf.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)      105 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/data/applications/espresso/5.4.0/case-001/run.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 03:23:59.075716 mat3ra-fixtures-2024.4.6.post0/data/applications/espresso/5.4.0/case-002/
+-rw-r--r--   0 runner    (1001) docker     (127)  2241092 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/data/applications/espresso/5.4.0/case-002/pw-vc-relax.out
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 03:23:59.079716 mat3ra-fixtures-2024.4.6.post0/data/applications/espresso/5.4.0/case-003/
+-rw-r--r--   0 runner    (1001) docker     (127)    13619 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/data/applications/espresso/5.4.0/case-003/__prefix__.pdos_atm#1(Si)_wfc#1(s)
+-rw-r--r--   0 runner    (1001) docker     (127)    23607 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/data/applications/espresso/5.4.0/case-003/__prefix__.pdos_atm#1(Si)_wfc#2(p)
+-rw-r--r--   0 runner    (1001) docker     (127)    13619 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/data/applications/espresso/5.4.0/case-003/__prefix__.pdos_atm#2(Si)_wfc#1(s)
+-rw-r--r--   0 runner    (1001) docker     (127)    23607 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/data/applications/espresso/5.4.0/case-003/__prefix__.pdos_atm#2(Si)_wfc#2(p)
+-rw-r--r--   0 runner    (1001) docker     (127)    13618 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/data/applications/espresso/5.4.0/case-003/__prefix__.pdos_tot
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/data/applications/espresso/5.4.0/case-003/bands.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/data/applications/espresso/5.4.0/case-003/bands.dat.gnu
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/data/applications/espresso/5.4.0/case-003/bands.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/data/applications/espresso/5.4.0/case-003/bands.out
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 03:23:59.079716 mat3ra-fixtures-2024.4.6.post0/data/applications/espresso/5.4.0/case-003/outdir/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 03:23:59.083716 mat3ra-fixtures-2024.4.6.post0/data/applications/espresso/5.4.0/case-003/outdir/__prefix__.save/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 03:23:59.087716 mat3ra-fixtures-2024.4.6.post0/data/applications/espresso/5.4.0/case-003/outdir/__prefix__.save/K00001/
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/data/applications/espresso/5.4.0/case-003/outdir/__prefix__.save/K00001/eigenval.xml
+-rw-r--r--   0 runner    (1001) docker     (127)   160469 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/data/applications/espresso/5.4.0/case-003/outdir/__prefix__.save/K00001/evc.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    21019 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/data/applications/espresso/5.4.0/case-003/outdir/__prefix__.save/K00001/gkvectors.dat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 03:23:59.087716 mat3ra-fixtures-2024.4.6.post0/data/applications/espresso/5.4.0/case-003/outdir/__prefix__.save/K00002/
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/data/applications/espresso/5.4.0/case-003/outdir/__prefix__.save/K00002/eigenval.xml
+-rw-r--r--   0 runner    (1001) docker     (127)   151125 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/data/applications/espresso/5.4.0/case-003/outdir/__prefix__.save/K00002/evc.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    19851 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/data/applications/espresso/5.4.0/case-003/outdir/__prefix__.save/K00002/gkvectors.dat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 03:23:59.087716 mat3ra-fixtures-2024.4.6.post0/data/applications/espresso/5.4.0/case-003/outdir/__prefix__.save/K00003/
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/data/applications/espresso/5.4.0/case-003/outdir/__prefix__.save/K00003/eigenval.xml
+-rw-r--r--   0 runner    (1001) docker     (127)   151125 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/data/applications/espresso/5.4.0/case-003/outdir/__prefix__.save/K00003/evc.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    19851 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/data/applications/espresso/5.4.0/case-003/outdir/__prefix__.save/K00003/gkvectors.dat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 03:23:59.087716 mat3ra-fixtures-2024.4.6.post0/data/applications/espresso/5.4.0/case-003/outdir/__prefix__.save/K00004/
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/data/applications/espresso/5.4.0/case-003/outdir/__prefix__.save/K00004/eigenval.xml
+-rw-r--r--   0 runner    (1001) docker     (127)   150101 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/data/applications/espresso/5.4.0/case-003/outdir/__prefix__.save/K00004/evc.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    19723 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/data/applications/espresso/5.4.0/case-003/outdir/__prefix__.save/K00004/gkvectors.dat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 03:23:59.091716 mat3ra-fixtures-2024.4.6.post0/data/applications/espresso/5.4.0/case-003/outdir/__prefix__.save/K00005/
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/data/applications/espresso/5.4.0/case-003/outdir/__prefix__.save/K00005/eigenval.xml
+-rw-r--r--   0 runner    (1001) docker     (127)   151125 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/data/applications/espresso/5.4.0/case-003/outdir/__prefix__.save/K00005/evc.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    19851 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/data/applications/espresso/5.4.0/case-003/outdir/__prefix__.save/K00005/gkvectors.dat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 03:23:59.091716 mat3ra-fixtures-2024.4.6.post0/data/applications/espresso/5.4.0/case-003/outdir/__prefix__.save/K00006/
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/data/applications/espresso/5.4.0/case-003/outdir/__prefix__.save/K00006/eigenval.xml
+-rw-r--r--   0 runner    (1001) docker     (127)   150101 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/data/applications/espresso/5.4.0/case-003/outdir/__prefix__.save/K00006/evc.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    19723 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/data/applications/espresso/5.4.0/case-003/outdir/__prefix__.save/K00006/gkvectors.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    24766 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/data/applications/espresso/5.4.0/case-003/outdir/__prefix__.save/atomic_proj.xml
+-rw-r--r--   0 runner    (1001) docker     (127)   377892 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/data/applications/espresso/5.4.0/case-003/outdir/__prefix__.save/charge-density.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    17043 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/data/applications/espresso/5.4.0/case-003/outdir/__prefix__.save/data-file.xml
+-rw-r--r--   0 runner    (1001) docker     (127)   160388 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/data/applications/espresso/5.4.0/case-003/outdir/__prefix__.save/gvectors.dat
+-rw-r--r--   0 runner    (1001) docker     (127)   577640 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/data/applications/espresso/5.4.0/case-003/outdir/__prefix__.save/si_pbe_gbrv_1.0.upf
+-rw-r--r--   0 runner    (1001) docker     (127)   954624 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/data/applications/espresso/5.4.0/case-003/outdir/__prefix__.wfc
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/data/applications/espresso/5.4.0/case-003/projwfc.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9428 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/data/applications/espresso/5.4.0/case-003/projwfc.out
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 03:23:59.091716 mat3ra-fixtures-2024.4.6.post0/data/applications/espresso/5.4.0/case-003/pseudo/
+-rw-r--r--   0 runner    (1001) docker     (127)   577640 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/data/applications/espresso/5.4.0/case-003/pseudo/si_pbe_gbrv_1.0.upf
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/data/applications/espresso/5.4.0/case-003/pw-bands.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7959 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/data/applications/espresso/5.4.0/case-003/pw-bands.out
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/data/applications/espresso/5.4.0/case-003/pw-nscf.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7998 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/data/applications/espresso/5.4.0/case-003/pw-nscf.out
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/data/applications/espresso/5.4.0/case-003/pw-scf.in
+-rw-r--r--   0 runner    (1001) docker     (127)    11553 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/data/applications/espresso/5.4.0/case-003/pw-scf.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)      301 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/data/applications/espresso/5.4.0/case-003/run.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/data/applications/espresso/5.4.0/manifest.yml
+-rw-r--r--   0 runner    (1001) docker     (127)   307578 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2469 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/package.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 03:23:59.123716 mat3ra-fixtures-2024.4.6.post0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 03:23:59.055716 mat3ra-fixtures-2024.4.6.post0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 03:23:59.091716 mat3ra-fixtures-2024.4.6.post0/src/js/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/src/js/index.ts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 03:23:59.091716 mat3ra-fixtures-2024.4.6.post0/src/py/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/src/py/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 03:23:59.091716 mat3ra-fixtures-2024.4.6.post0/src/py/mat3ra/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/src/py/mat3ra/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 03:23:59.091716 mat3ra-fixtures-2024.4.6.post0/src/py/mat3ra/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/src/py/mat3ra/fixtures/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 03:23:59.055716 mat3ra-fixtures-2024.4.6.post0/src/py/mat3ra/fixtures/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 03:23:59.055716 mat3ra-fixtures-2024.4.6.post0/src/py/mat3ra/fixtures/data/applications/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 03:23:59.055716 mat3ra-fixtures-2024.4.6.post0/src/py/mat3ra/fixtures/data/applications/espresso/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 03:23:59.091716 mat3ra-fixtures-2024.4.6.post0/src/py/mat3ra/fixtures/data/applications/espresso/5.4.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 03:23:59.091716 mat3ra-fixtures-2024.4.6.post0/src/py/mat3ra/fixtures/data/applications/espresso/5.4.0/case-001/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 03:23:59.055716 mat3ra-fixtures-2024.4.6.post0/src/py/mat3ra/fixtures/data/applications/espresso/5.4.0/case-001/outdir/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 03:23:59.095716 mat3ra-fixtures-2024.4.6.post0/src/py/mat3ra/fixtures/data/applications/espresso/5.4.0/case-001/outdir/__prefix__.save/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 03:23:59.095716 mat3ra-fixtures-2024.4.6.post0/src/py/mat3ra/fixtures/data/applications/espresso/5.4.0/case-001/outdir/__prefix__.save/K00001/
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/src/py/mat3ra/fixtures/data/applications/espresso/5.4.0/case-001/outdir/__prefix__.save/K00001/eigenval.xml
+-rw-r--r--   0 runner    (1001) docker     (127)   160469 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/src/py/mat3ra/fixtures/data/applications/espresso/5.4.0/case-001/outdir/__prefix__.save/K00001/evc.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    21019 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/src/py/mat3ra/fixtures/data/applications/espresso/5.4.0/case-001/outdir/__prefix__.save/K00001/gkvectors.dat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 03:23:59.099716 mat3ra-fixtures-2024.4.6.post0/src/py/mat3ra/fixtures/data/applications/espresso/5.4.0/case-001/outdir/__prefix__.save/K00002/
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/src/py/mat3ra/fixtures/data/applications/espresso/5.4.0/case-001/outdir/__prefix__.save/K00002/eigenval.xml
+-rw-r--r--   0 runner    (1001) docker     (127)   151125 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/src/py/mat3ra/fixtures/data/applications/espresso/5.4.0/case-001/outdir/__prefix__.save/K00002/evc.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    19851 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/src/py/mat3ra/fixtures/data/applications/espresso/5.4.0/case-001/outdir/__prefix__.save/K00002/gkvectors.dat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 03:23:59.099716 mat3ra-fixtures-2024.4.6.post0/src/py/mat3ra/fixtures/data/applications/espresso/5.4.0/case-001/outdir/__prefix__.save/K00003/
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/src/py/mat3ra/fixtures/data/applications/espresso/5.4.0/case-001/outdir/__prefix__.save/K00003/eigenval.xml
+-rw-r--r--   0 runner    (1001) docker     (127)   151125 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/src/py/mat3ra/fixtures/data/applications/espresso/5.4.0/case-001/outdir/__prefix__.save/K00003/evc.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    19851 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/src/py/mat3ra/fixtures/data/applications/espresso/5.4.0/case-001/outdir/__prefix__.save/K00003/gkvectors.dat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 03:23:59.099716 mat3ra-fixtures-2024.4.6.post0/src/py/mat3ra/fixtures/data/applications/espresso/5.4.0/case-001/outdir/__prefix__.save/K00004/
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/src/py/mat3ra/fixtures/data/applications/espresso/5.4.0/case-001/outdir/__prefix__.save/K00004/eigenval.xml
+-rw-r--r--   0 runner    (1001) docker     (127)   150101 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/src/py/mat3ra/fixtures/data/applications/espresso/5.4.0/case-001/outdir/__prefix__.save/K00004/evc.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    19723 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/src/py/mat3ra/fixtures/data/applications/espresso/5.4.0/case-001/outdir/__prefix__.save/K00004/gkvectors.dat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 03:23:59.099716 mat3ra-fixtures-2024.4.6.post0/src/py/mat3ra/fixtures/data/applications/espresso/5.4.0/case-001/outdir/__prefix__.save/K00005/
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/src/py/mat3ra/fixtures/data/applications/espresso/5.4.0/case-001/outdir/__prefix__.save/K00005/eigenval.xml
+-rw-r--r--   0 runner    (1001) docker     (127)   151125 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/src/py/mat3ra/fixtures/data/applications/espresso/5.4.0/case-001/outdir/__prefix__.save/K00005/evc.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    19851 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/src/py/mat3ra/fixtures/data/applications/espresso/5.4.0/case-001/outdir/__prefix__.save/K00005/gkvectors.dat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 03:23:59.099716 mat3ra-fixtures-2024.4.6.post0/src/py/mat3ra/fixtures/data/applications/espresso/5.4.0/case-001/outdir/__prefix__.save/K00006/
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/src/py/mat3ra/fixtures/data/applications/espresso/5.4.0/case-001/outdir/__prefix__.save/K00006/eigenval.xml
+-rw-r--r--   0 runner    (1001) docker     (127)   150101 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/src/py/mat3ra/fixtures/data/applications/espresso/5.4.0/case-001/outdir/__prefix__.save/K00006/evc.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    19723 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/src/py/mat3ra/fixtures/data/applications/espresso/5.4.0/case-001/outdir/__prefix__.save/K00006/gkvectors.dat
+-rw-r--r--   0 runner    (1001) docker     (127)   377892 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/src/py/mat3ra/fixtures/data/applications/espresso/5.4.0/case-001/outdir/__prefix__.save/charge-density.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    17304 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/src/py/mat3ra/fixtures/data/applications/espresso/5.4.0/case-001/outdir/__prefix__.save/data-file.xml
+-rw-r--r--   0 runner    (1001) docker     (127)   160388 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/src/py/mat3ra/fixtures/data/applications/espresso/5.4.0/case-001/outdir/__prefix__.save/gvectors.dat
+-rw-r--r--   0 runner    (1001) docker     (127)   577640 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/src/py/mat3ra/fixtures/data/applications/espresso/5.4.0/case-001/outdir/__prefix__.save/si_pbe_gbrv_1.0.upf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 03:23:59.099716 mat3ra-fixtures-2024.4.6.post0/src/py/mat3ra/fixtures/data/applications/espresso/5.4.0/case-001/pseudo/
+-rw-r--r--   0 runner    (1001) docker     (127)   577640 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/src/py/mat3ra/fixtures/data/applications/espresso/5.4.0/case-001/pseudo/si_pbe_gbrv_1.0.upf
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/src/py/mat3ra/fixtures/data/applications/espresso/5.4.0/case-001/pw-scf.in
+-rw-r--r--   0 runner    (1001) docker     (127)    11469 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/src/py/mat3ra/fixtures/data/applications/espresso/5.4.0/case-001/pw-scf.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)      105 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/src/py/mat3ra/fixtures/data/applications/espresso/5.4.0/case-001/run.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 03:23:59.103716 mat3ra-fixtures-2024.4.6.post0/src/py/mat3ra/fixtures/data/applications/espresso/5.4.0/case-002/
+-rw-r--r--   0 runner    (1001) docker     (127)  2241092 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/src/py/mat3ra/fixtures/data/applications/espresso/5.4.0/case-002/pw-vc-relax.out
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 03:23:59.107716 mat3ra-fixtures-2024.4.6.post0/src/py/mat3ra/fixtures/data/applications/espresso/5.4.0/case-003/
+-rw-r--r--   0 runner    (1001) docker     (127)    13619 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/src/py/mat3ra/fixtures/data/applications/espresso/5.4.0/case-003/__prefix__.pdos_atm#1(Si)_wfc#1(s)
+-rw-r--r--   0 runner    (1001) docker     (127)    23607 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/src/py/mat3ra/fixtures/data/applications/espresso/5.4.0/case-003/__prefix__.pdos_atm#1(Si)_wfc#2(p)
+-rw-r--r--   0 runner    (1001) docker     (127)    13619 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/src/py/mat3ra/fixtures/data/applications/espresso/5.4.0/case-003/__prefix__.pdos_atm#2(Si)_wfc#1(s)
+-rw-r--r--   0 runner    (1001) docker     (127)    23607 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/src/py/mat3ra/fixtures/data/applications/espresso/5.4.0/case-003/__prefix__.pdos_atm#2(Si)_wfc#2(p)
+-rw-r--r--   0 runner    (1001) docker     (127)    13618 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/src/py/mat3ra/fixtures/data/applications/espresso/5.4.0/case-003/__prefix__.pdos_tot
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/src/py/mat3ra/fixtures/data/applications/espresso/5.4.0/case-003/bands.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/src/py/mat3ra/fixtures/data/applications/espresso/5.4.0/case-003/bands.dat.gnu
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/src/py/mat3ra/fixtures/data/applications/espresso/5.4.0/case-003/bands.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/src/py/mat3ra/fixtures/data/applications/espresso/5.4.0/case-003/bands.out
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 03:23:59.111716 mat3ra-fixtures-2024.4.6.post0/src/py/mat3ra/fixtures/data/applications/espresso/5.4.0/case-003/outdir/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 03:23:59.111716 mat3ra-fixtures-2024.4.6.post0/src/py/mat3ra/fixtures/data/applications/espresso/5.4.0/case-003/outdir/__prefix__.save/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 03:23:59.115716 mat3ra-fixtures-2024.4.6.post0/src/py/mat3ra/fixtures/data/applications/espresso/5.4.0/case-003/outdir/__prefix__.save/K00001/
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/src/py/mat3ra/fixtures/data/applications/espresso/5.4.0/case-003/outdir/__prefix__.save/K00001/eigenval.xml
+-rw-r--r--   0 runner    (1001) docker     (127)   160469 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/src/py/mat3ra/fixtures/data/applications/espresso/5.4.0/case-003/outdir/__prefix__.save/K00001/evc.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    21019 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/src/py/mat3ra/fixtures/data/applications/espresso/5.4.0/case-003/outdir/__prefix__.save/K00001/gkvectors.dat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 03:23:59.115716 mat3ra-fixtures-2024.4.6.post0/src/py/mat3ra/fixtures/data/applications/espresso/5.4.0/case-003/outdir/__prefix__.save/K00002/
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/src/py/mat3ra/fixtures/data/applications/espresso/5.4.0/case-003/outdir/__prefix__.save/K00002/eigenval.xml
+-rw-r--r--   0 runner    (1001) docker     (127)   151125 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/src/py/mat3ra/fixtures/data/applications/espresso/5.4.0/case-003/outdir/__prefix__.save/K00002/evc.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    19851 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/src/py/mat3ra/fixtures/data/applications/espresso/5.4.0/case-003/outdir/__prefix__.save/K00002/gkvectors.dat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 03:23:59.115716 mat3ra-fixtures-2024.4.6.post0/src/py/mat3ra/fixtures/data/applications/espresso/5.4.0/case-003/outdir/__prefix__.save/K00003/
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/src/py/mat3ra/fixtures/data/applications/espresso/5.4.0/case-003/outdir/__prefix__.save/K00003/eigenval.xml
+-rw-r--r--   0 runner    (1001) docker     (127)   151125 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/src/py/mat3ra/fixtures/data/applications/espresso/5.4.0/case-003/outdir/__prefix__.save/K00003/evc.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    19851 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/src/py/mat3ra/fixtures/data/applications/espresso/5.4.0/case-003/outdir/__prefix__.save/K00003/gkvectors.dat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 03:23:59.115716 mat3ra-fixtures-2024.4.6.post0/src/py/mat3ra/fixtures/data/applications/espresso/5.4.0/case-003/outdir/__prefix__.save/K00004/
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/src/py/mat3ra/fixtures/data/applications/espresso/5.4.0/case-003/outdir/__prefix__.save/K00004/eigenval.xml
+-rw-r--r--   0 runner    (1001) docker     (127)   150101 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/src/py/mat3ra/fixtures/data/applications/espresso/5.4.0/case-003/outdir/__prefix__.save/K00004/evc.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    19723 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/src/py/mat3ra/fixtures/data/applications/espresso/5.4.0/case-003/outdir/__prefix__.save/K00004/gkvectors.dat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 03:23:59.119716 mat3ra-fixtures-2024.4.6.post0/src/py/mat3ra/fixtures/data/applications/espresso/5.4.0/case-003/outdir/__prefix__.save/K00005/
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/src/py/mat3ra/fixtures/data/applications/espresso/5.4.0/case-003/outdir/__prefix__.save/K00005/eigenval.xml
+-rw-r--r--   0 runner    (1001) docker     (127)   151125 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/src/py/mat3ra/fixtures/data/applications/espresso/5.4.0/case-003/outdir/__prefix__.save/K00005/evc.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    19851 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/src/py/mat3ra/fixtures/data/applications/espresso/5.4.0/case-003/outdir/__prefix__.save/K00005/gkvectors.dat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 03:23:59.119716 mat3ra-fixtures-2024.4.6.post0/src/py/mat3ra/fixtures/data/applications/espresso/5.4.0/case-003/outdir/__prefix__.save/K00006/
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/src/py/mat3ra/fixtures/data/applications/espresso/5.4.0/case-003/outdir/__prefix__.save/K00006/eigenval.xml
+-rw-r--r--   0 runner    (1001) docker     (127)   150101 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/src/py/mat3ra/fixtures/data/applications/espresso/5.4.0/case-003/outdir/__prefix__.save/K00006/evc.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    19723 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/src/py/mat3ra/fixtures/data/applications/espresso/5.4.0/case-003/outdir/__prefix__.save/K00006/gkvectors.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    24766 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/src/py/mat3ra/fixtures/data/applications/espresso/5.4.0/case-003/outdir/__prefix__.save/atomic_proj.xml
+-rw-r--r--   0 runner    (1001) docker     (127)   377892 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/src/py/mat3ra/fixtures/data/applications/espresso/5.4.0/case-003/outdir/__prefix__.save/charge-density.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    17043 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/src/py/mat3ra/fixtures/data/applications/espresso/5.4.0/case-003/outdir/__prefix__.save/data-file.xml
+-rw-r--r--   0 runner    (1001) docker     (127)   160388 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/src/py/mat3ra/fixtures/data/applications/espresso/5.4.0/case-003/outdir/__prefix__.save/gvectors.dat
+-rw-r--r--   0 runner    (1001) docker     (127)   577640 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/src/py/mat3ra/fixtures/data/applications/espresso/5.4.0/case-003/outdir/__prefix__.save/si_pbe_gbrv_1.0.upf
+-rw-r--r--   0 runner    (1001) docker     (127)   954624 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/src/py/mat3ra/fixtures/data/applications/espresso/5.4.0/case-003/outdir/__prefix__.wfc
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/src/py/mat3ra/fixtures/data/applications/espresso/5.4.0/case-003/projwfc.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9428 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/src/py/mat3ra/fixtures/data/applications/espresso/5.4.0/case-003/projwfc.out
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 03:23:59.119716 mat3ra-fixtures-2024.4.6.post0/src/py/mat3ra/fixtures/data/applications/espresso/5.4.0/case-003/pseudo/
+-rw-r--r--   0 runner    (1001) docker     (127)   577640 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/src/py/mat3ra/fixtures/data/applications/espresso/5.4.0/case-003/pseudo/si_pbe_gbrv_1.0.upf
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/src/py/mat3ra/fixtures/data/applications/espresso/5.4.0/case-003/pw-bands.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7959 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/src/py/mat3ra/fixtures/data/applications/espresso/5.4.0/case-003/pw-bands.out
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/src/py/mat3ra/fixtures/data/applications/espresso/5.4.0/case-003/pw-nscf.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7998 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/src/py/mat3ra/fixtures/data/applications/espresso/5.4.0/case-003/pw-nscf.out
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/src/py/mat3ra/fixtures/data/applications/espresso/5.4.0/case-003/pw-scf.in
+-rw-r--r--   0 runner    (1001) docker     (127)    11553 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/src/py/mat3ra/fixtures/data/applications/espresso/5.4.0/case-003/pw-scf.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)      301 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/src/py/mat3ra/fixtures/data/applications/espresso/5.4.0/case-003/run.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/src/py/mat3ra/fixtures/data/applications/espresso/5.4.0/manifest.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/src/py/mat3ra/fixtures/manifest.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 03:23:59.123716 mat3ra-fixtures-2024.4.6.post0/src/py/mat3ra_fixtures.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3135 2024-04-06 03:23:58.000000 mat3ra-fixtures-2024.4.6.post0/src/py/mat3ra_fixtures.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12984 2024-04-06 03:23:59.000000 mat3ra-fixtures-2024.4.6.post0/src/py/mat3ra_fixtures.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 03:23:58.000000 mat3ra-fixtures-2024.4.6.post0/src/py/mat3ra_fixtures.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-06 03:23:58.000000 mat3ra-fixtures-2024.4.6.post0/src/py/mat3ra_fixtures.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-06 03:23:58.000000 mat3ra-fixtures-2024.4.6.post0/src/py/mat3ra_fixtures.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 03:23:59.059716 mat3ra-fixtures-2024.4.6.post0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 03:23:59.119716 mat3ra-fixtures-2024.4.6.post0/tests/js/
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/tests/js/babel-register.js
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/tests/js/greeting.test.ts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 03:23:59.059716 mat3ra-fixtures-2024.4.6.post0/tests/py/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 03:23:59.123716 mat3ra-fixtures-2024.4.6.post0/tests/py/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/tests/py/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/tests/py/unit/test_get_from_manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-06 03:23:36.000000 mat3ra-fixtures-2024.4.6.post0/tsconfig.json
```

### Comparing `mat3ra-fixtures-2024.3.21.post2/.github/workflows/cicd.yml` & `mat3ra-fixtures-2024.4.6.post0/.github/workflows/cicd.yml`

 * *Files identical despite different names*

### Comparing `mat3ra-fixtures-2024.3.21.post2/.gitignore` & `mat3ra-fixtures-2024.4.6.post0/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+.husky/_
+
 # Byte-compiled / optimized / DLL files
 __pycache__/
 *.py[cod]
 *$py.class
 
 # C extensions
 *.so
```

### Comparing `mat3ra-fixtures-2024.3.21.post2/LICENSE.md` & `mat3ra-fixtures-2024.4.6.post0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mat3ra-fixtures-2024.3.21.post2/package-lock.json` & `mat3ra-fixtures-2024.4.6.post0/package-lock.json`

 * *Files identical despite different names*

### Comparing `mat3ra-fixtures-2024.3.21.post2/package.json` & `mat3ra-fixtures-2024.4.6.post0/package.json`

 * *Files identical despite different names*

### Comparing `mat3ra-fixtures-2024.3.21.post2/pyproject.toml` & `mat3ra-fixtures-2024.4.6.post0/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -11,27 +11,29 @@
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Development Status :: 3 - Alpha",
     "Topic :: Software Development",
 ]
 dependencies = [
-    # add requirements here
-    "numpy"
+    "pyyaml",
+    "mat3ra-utils",
 ]
 
 [project.optional-dependencies]
 tests = [
     "coverage[toml]>=5.3",
     "pre-commit",
     "black",
     "ruff",
     "isort",
     "mypy",
-    "pip-tools"
+    "pip-tools",
+    "pytest",
+    "types-PyYAML",
 ]
 all = ["mat3ra-fixtures[tests]"]
 
 # Entrypoint scripts can be defined here, see examples below.
 [project.scripts]
 # my-script = "my_package.my_module:my_function"
 
@@ -45,14 +47,27 @@
 
 [tool.setuptools_scm]
 git_describe_command = "git describe --tags --long"
 
 [tool.setuptools.packages.find]
 where = ["src/py"]
 
+[tool.setuptools.package-data]
+"*" = [
+    "*.yml",
+    "data/**"
+]
+
+[tool.setuptools.exclude-package-data]
+"*" = [
+    # Since data inside `src/py` is a link, exclusion is needed
+    # to avoid `doesn't exist or not a regular file` error
+    "data"
+]
+
 [tool.black]
 line-length = 120
 target-version = ['py38']
 # 'extend-exclude' excludes files or directories in addition to the defaults
 extend-exclude = '''
 (
     examples\/.*\/.*\.py
@@ -71,7 +86,12 @@
 [tool.ruff.per-file-ignores]
 "__init__.py" = ["F401"]
 
 [tool.isort]
 profile = "black"
 multi_line_output = 3
 include_trailing_comma = true
+
+# Per https://github.com/python/mypy/issues/10632
+[[tool.mypy.overrides]]
+module = "yaml"
+ignore_missing_imports = true
```

