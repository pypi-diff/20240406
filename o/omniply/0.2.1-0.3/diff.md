# Comparing `tmp/omniply-0.2.1.tar.gz` & `tmp/omniply-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omniply-0.2.1.tar", last modified: Tue Feb 13 13:40:56 2024, max compression
+gzip compressed data, was "omniply-0.3.tar", last modified: Sat Apr  6 12:19:43 2024, max compression
```

## Comparing `omniply-0.2.1.tar` & `omniply-0.3.tar`

### file list

```diff
@@ -1,123 +1,47 @@
-drwxr-xr-x   0 fleeb     (7343) is        (1040)        0 2024-02-13 13:40:56.210778 omniply-0.2.1/
--rwxr-xr-x   0 fleeb     (7343) is        (1040)     1067 2023-08-30 14:47:46.000000 omniply-0.2.1/LICENSE
--rw-r--r--   0 fleeb     (7343) is        (1040)      517 2024-02-13 13:40:56.210778 omniply-0.2.1/PKG-INFO
--rwxr-xr-x   0 fleeb     (7343) is        (1040)      216 2023-08-31 12:56:39.000000 omniply-0.2.1/README.md
-drwxr-xr-x   0 fleeb     (7343) is        (1040)        0 2024-02-13 13:40:56.202778 omniply-0.2.1/omniply/
--rwxr-xr-x   0 fleeb     (7343) is        (1040)      334 2024-02-13 13:40:46.000000 omniply-0.2.1/omniply/__init__.py
-drwxr-xr-x   0 fleeb     (7343) is        (1040)        0 2024-02-13 13:40:56.202778 omniply-0.2.1/omniply/_future/
--rwxr-xr-x   0 fleeb     (7343) is        (1040)        0 2023-08-30 14:47:46.000000 omniply-0.2.1/omniply/_future/__init__.py
--rwxr-xr-x   0 fleeb     (7343) is        (1040)     2501 2023-08-30 14:47:46.000000 omniply-0.2.1/omniply/_future/common.py
--rwxr-xr-x   0 fleeb     (7343) is        (1040)     4287 2023-08-30 14:47:46.000000 omniply-0.2.1/omniply/_future/specification.py
--rwxr-xr-x   0 fleeb     (7343) is        (1040)     3749 2023-08-30 14:47:46.000000 omniply-0.2.1/omniply/_future/wrappers.py
-drwxr-xr-x   0 fleeb     (7343) is        (1040)        0 2024-02-13 13:40:56.202778 omniply-0.2.1/omniply/core/
--rwxr-xr-x   0 fleeb     (7343) is        (1040)      172 2023-11-18 13:26:58.000000 omniply-0.2.1/omniply/core/__init__.py
--rwxr-xr-x   0 fleeb     (7343) is        (1040)    10118 2024-01-16 12:05:27.000000 omniply-0.2.1/omniply/core/abstract.py
--rwxr-xr-x   0 fleeb     (7343) is        (1040)     2050 2023-11-18 13:36:36.000000 omniply-0.2.1/omniply/core/errors.py
--rwxr-xr-x   0 fleeb     (7343) is        (1040)     6092 2024-01-16 12:05:27.000000 omniply-0.2.1/omniply/core/gadgets.py
--rwxr-xr-x   0 fleeb     (7343) is        (1040)     9363 2024-01-16 12:05:27.000000 omniply-0.2.1/omniply/core/gaggles.py
--rwxr-xr-x   0 fleeb     (7343) is        (1040)     4255 2024-01-16 12:05:27.000000 omniply-0.2.1/omniply/core/gangs.py
--rwxr-xr-x   0 fleeb     (7343) is        (1040)     6889 2024-01-16 12:05:27.000000 omniply-0.2.1/omniply/core/gigs.py
--rwxr-xr-x   0 fleeb     (7343) is        (1040)     1353 2023-11-28 09:46:19.000000 omniply-0.2.1/omniply/core/gizmos.py
--rwxr-xr-x   0 fleeb     (7343) is        (1040)     8363 2024-01-16 12:13:31.000000 omniply-0.2.1/omniply/core/groups.py
--rwxr-xr-x   0 fleeb     (7343) is        (1040)     6843 2023-11-28 09:46:19.000000 omniply-0.2.1/omniply/core/tools.py
--rwxr-xr-x   0 fleeb     (7343) is        (1040)     5001 2024-01-16 12:09:12.000000 omniply-0.2.1/omniply/core/top.py
--rwxr-xr-x   0 fleeb     (7343) is        (1040)    24516 2024-01-16 12:05:27.000000 omniply-0.2.1/omniply/core/unit_test.py
-drwxr-xr-x   0 fleeb     (7343) is        (1040)        0 2024-02-13 13:40:56.206778 omniply-0.2.1/omniply/data/
--rwxr-xr-x   0 fleeb     (7343) is        (1040)      734 2023-08-30 14:47:46.000000 omniply-0.2.1/omniply/data/__init__.py
--rwxr-xr-x   0 fleeb     (7343) is        (1040)     7220 2023-08-30 14:47:46.000000 omniply-0.2.1/omniply/data/abstract.py
--rwxr-xr-x   0 fleeb     (7343) is        (1040)     4110 2023-08-30 14:47:46.000000 omniply-0.2.1/omniply/data/batches.py
--rwxr-xr-x   0 fleeb     (7343) is        (1040)    14259 2023-08-30 14:47:46.000000 omniply-0.2.1/omniply/data/budgeting.py
--rwxr-xr-x   0 fleeb     (7343) is        (1040)      426 2023-08-30 14:47:46.000000 omniply-0.2.1/omniply/data/errors.py
--rwxr-xr-x   0 fleeb     (7343) is        (1040)     7391 2023-08-30 14:47:46.000000 omniply-0.2.1/omniply/data/flavors.py
--rwxr-xr-x   0 fleeb     (7343) is        (1040)     5446 2023-08-30 14:47:46.000000 omniply-0.2.1/omniply/data/progression.py
--rwxr-xr-x   0 fleeb     (7343) is        (1040)     7197 2023-08-30 14:47:46.000000 omniply-0.2.1/omniply/data/routers.py
--rwxr-xr-x   0 fleeb     (7343) is        (1040)    14018 2023-08-30 14:47:46.000000 omniply-0.2.1/omniply/data/sources.py
--rwxr-xr-x   0 fleeb     (7343) is        (1040)     2348 2023-08-30 14:47:46.000000 omniply-0.2.1/omniply/data/top.py
-drwxr-xr-x   0 fleeb     (7343) is        (1040)        0 2024-02-13 13:40:56.206778 omniply-0.2.1/omniply/data/toy/
--rwxr-xr-x   0 fleeb     (7343) is        (1040)       78 2023-08-30 14:47:46.000000 omniply-0.2.1/omniply/data/toy/__init__.py
--rwxr-xr-x   0 fleeb     (7343) is        (1040)     4938 2023-08-30 14:47:46.000000 omniply-0.2.1/omniply/data/toy/manifolds.py
--rwxr-xr-x   0 fleeb     (7343) is        (1040)     3499 2023-08-30 14:47:46.000000 omniply-0.2.1/omniply/data/views.py
-drwxr-xr-x   0 fleeb     (7343) is        (1040)        0 2024-02-13 13:40:56.206778 omniply-0.2.1/omniply/features/
--rwxr-xr-x   0 fleeb     (7343) is        (1040)      304 2023-08-30 14:47:46.000000 omniply-0.2.1/omniply/features/__init__.py
--rwxr-xr-x   0 fleeb     (7343) is        (1040)     2439 2023-08-30 14:47:46.000000 omniply-0.2.1/omniply/features/containers.py
--rwxr-xr-x   0 fleeb     (7343) is        (1040)       41 2023-08-30 14:47:46.000000 omniply-0.2.1/omniply/features/errors.py
--rwxr-xr-x   0 fleeb     (7343) is        (1040)     1600 2023-08-30 14:47:46.000000 omniply-0.2.1/omniply/features/hardware.py
--rwxr-xr-x   0 fleeb     (7343) is        (1040)     8305 2023-08-30 14:47:46.000000 omniply-0.2.1/omniply/features/random.py
--rwxr-xr-x   0 fleeb     (7343) is        (1040)     1599 2023-08-30 14:47:46.000000 omniply-0.2.1/omniply/features/simple.py
-drwxr-xr-x   0 fleeb     (7343) is        (1040)        0 2024-02-13 13:40:56.206778 omniply-0.2.1/omniply/modules/
--rwxr-xr-x   0 fleeb     (7343) is        (1040)      361 2023-08-30 14:47:46.000000 omniply-0.2.1/omniply/modules/__init__.py
--rwxr-xr-x   0 fleeb     (7343) is        (1040)     1065 2023-08-30 14:47:46.000000 omniply-0.2.1/omniply/modules/abstract.py
--rwxr-xr-x   0 fleeb     (7343) is        (1040)     2349 2023-08-30 14:47:46.000000 omniply-0.2.1/omniply/modules/iterative.py
--rwxr-xr-x   0 fleeb     (7343) is        (1040)     6021 2023-08-30 14:47:46.000000 omniply-0.2.1/omniply/modules/loading.py
--rwxr-xr-x   0 fleeb     (7343) is        (1040)     3773 2023-08-30 14:47:46.000000 omniply-0.2.1/omniply/modules/machines.py
--rwxr-xr-x   0 fleeb     (7343) is        (1040)     1121 2023-08-30 14:47:46.000000 omniply-0.2.1/omniply/modules/simple.py
-drwxr-xr-x   0 fleeb     (7343) is        (1040)        0 2024-02-13 13:40:56.206778 omniply-0.2.1/omniply/novo/
--rwxr-xr-x   0 fleeb     (7343) is        (1040)        0 2023-08-30 14:47:46.000000 omniply-0.2.1/omniply/novo/__init__.py
--rwxr-xr-x   0 fleeb     (7343) is        (1040)     1344 2023-08-30 14:47:46.000000 omniply-0.2.1/omniply/novo/artists.py
--rwxr-xr-x   0 fleeb     (7343) is        (1040)     4957 2023-11-18 13:26:58.000000 omniply-0.2.1/omniply/novo/behaviors-tulip.py
--rwxr-xr-x   0 fleeb     (7343) is        (1040)     5139 2023-11-18 13:26:58.000000 omniply-0.2.1/omniply/novo/behaviors.py
--rwxr-xr-x   0 fleeb     (7343) is        (1040)     3574 2023-11-18 13:26:58.000000 omniply-0.2.1/omniply/novo/contexts-tulip.py
--rwxr-xr-x   0 fleeb     (7343) is        (1040)     3703 2023-11-18 13:26:58.000000 omniply-0.2.1/omniply/novo/contexts.py
--rwxr-xr-x   0 fleeb     (7343) is        (1040)     2379 2023-11-18 13:26:58.000000 omniply-0.2.1/omniply/novo/errors.py
--rwxr-xr-x   0 fleeb     (7343) is        (1040)      573 2023-08-30 14:47:46.000000 omniply-0.2.1/omniply/novo/imports.py
--rwxr-xr-x   0 fleeb     (7343) is        (1040)     4015 2023-08-31 13:37:56.000000 omniply-0.2.1/omniply/novo/kits.py
--rwxr-xr-x   0 fleeb     (7343) is        (1040)     7418 2024-01-16 12:05:27.000000 omniply-0.2.1/omniply/novo/oldtest_novo.py
--rwxr-xr-x   0 fleeb     (7343) is        (1040)      374 2023-11-18 13:26:58.000000 omniply-0.2.1/omniply/novo/patterns.py
--rwxr-xr-x   0 fleeb     (7343) is        (1040)     9636 2023-08-30 14:47:46.000000 omniply-0.2.1/omniply/novo/quirks.py
--rwxr-xr-x   0 fleeb     (7343) is        (1040)     3925 2023-08-30 14:47:46.000000 omniply-0.2.1/omniply/novo/quirky.py
--rwxr-xr-x   0 fleeb     (7343) is        (1040)      473 2023-08-31 13:18:00.000000 omniply-0.2.1/omniply/novo/spaced.py
--rwxr-xr-x   0 fleeb     (7343) is        (1040)     3325 2023-08-31 13:18:00.000000 omniply-0.2.1/omniply/novo/spawning.py
--rwxr-xr-x   0 fleeb     (7343) is        (1040)     4598 2023-08-31 13:37:56.000000 omniply-0.2.1/omniply/novo/tools.py
-drwxr-xr-x   0 fleeb     (7343) is        (1040)        0 2024-02-13 13:40:56.210778 omniply-0.2.1/omniply/parameters/
--rwxr-xr-x   0 fleeb     (7343) is        (1040)      433 2023-08-30 14:47:46.000000 omniply-0.2.1/omniply/parameters/__init__.py
--rwxr-xr-x   0 fleeb     (7343) is        (1040)     5091 2023-08-30 14:47:46.000000 omniply-0.2.1/omniply/parameters/abstract.py
--rwxr-xr-x   0 fleeb     (7343) is        (1040)    22369 2023-11-18 13:26:58.000000 omniply-0.2.1/omniply/parameters/building.py
--rwxr-xr-x   0 fleeb     (7343) is        (1040)      432 2023-08-30 14:47:46.000000 omniply-0.2.1/omniply/parameters/errors.py
--rwxr-xr-x   0 fleeb     (7343) is        (1040)     5834 2023-08-30 14:47:46.000000 omniply-0.2.1/omniply/parameters/hyperparameters.py
--rwxr-xr-x   0 fleeb     (7343) is        (1040)     5707 2023-08-30 14:47:46.000000 omniply-0.2.1/omniply/parameters/parameterized.py
--rwxr-xr-x   0 fleeb     (7343) is        (1040)    12607 2023-08-30 14:47:46.000000 omniply-0.2.1/omniply/parameters/spec.py
--rwxr-xr-x   0 fleeb     (7343) is        (1040)     8852 2023-08-30 14:47:46.000000 omniply-0.2.1/omniply/parameters/submodules.py
--rwxr-xr-x   0 fleeb     (7343) is        (1040)     4146 2023-08-30 14:47:46.000000 omniply-0.2.1/omniply/parameters/top.py
-drwxr-xr-x   0 fleeb     (7343) is        (1040)        0 2024-02-13 13:40:56.210778 omniply-0.2.1/omniply/persistent/
--rwxr-xr-x   0 fleeb     (7343) is        (1040)      196 2023-08-30 14:47:46.000000 omniply-0.2.1/omniply/persistent/__init__.py
--rwxr-xr-x   0 fleeb     (7343) is        (1040)      210 2023-08-30 14:47:46.000000 omniply-0.2.1/omniply/persistent/errors.py
--rwxr-xr-x   0 fleeb     (7343) is        (1040)     4701 2023-08-30 14:47:46.000000 omniply-0.2.1/omniply/persistent/exporting.py
--rwxr-xr-x   0 fleeb     (7343) is        (1040)      444 2023-08-30 14:47:46.000000 omniply-0.2.1/omniply/persistent/filesystem.py
--rwxr-xr-x   0 fleeb     (7343) is        (1040)     3762 2023-08-30 14:47:46.000000 omniply-0.2.1/omniply/persistent/fingerprinting.py
-drwxr-xr-x   0 fleeb     (7343) is        (1040)        0 2024-02-13 13:40:56.210778 omniply-0.2.1/omniply/quirks/
--rwxr-xr-x   0 fleeb     (7343) is        (1040)        0 2024-01-16 12:05:27.000000 omniply-0.2.1/omniply/quirks/__init__.py
--rwxr-xr-x   0 fleeb     (7343) is        (1040)     1158 2024-01-16 12:05:27.000000 omniply-0.2.1/omniply/quirks/abstract.py
--rwxr-xr-x   0 fleeb     (7343) is        (1040)      115 2024-01-16 12:05:27.000000 omniply-0.2.1/omniply/quirks/imports.py
--rwxr-xr-x   0 fleeb     (7343) is        (1040)     2367 2024-01-16 12:05:27.000000 omniply-0.2.1/omniply/quirks/simple.py
-drwxr-xr-x   0 fleeb     (7343) is        (1040)        0 2024-02-13 13:40:56.210778 omniply-0.2.1/omniply/structure/
--rwxr-xr-x   0 fleeb     (7343) is        (1040)      387 2023-08-30 14:47:46.000000 omniply-0.2.1/omniply/structure/__init__.py
--rwxr-xr-x   0 fleeb     (7343) is        (1040)     6021 2023-08-30 14:47:46.000000 omniply-0.2.1/omniply/structure/distributions.py
--rwxr-xr-x   0 fleeb     (7343) is        (1040)      987 2023-08-30 14:47:46.000000 omniply-0.2.1/omniply/structure/functions.py
--rwxr-xr-x   0 fleeb     (7343) is        (1040)      791 2023-08-30 14:47:46.000000 omniply-0.2.1/omniply/structure/metrics.py
--rwxr-xr-x   0 fleeb     (7343) is        (1040)     2439 2023-08-30 14:47:46.000000 omniply-0.2.1/omniply/structure/operations.py
--rwxr-xr-x   0 fleeb     (7343) is        (1040)    22820 2023-08-30 14:47:46.000000 omniply-0.2.1/omniply/structure/spaces.py
-drwxr-xr-x   0 fleeb     (7343) is        (1040)        0 2024-02-13 13:40:56.210778 omniply-0.2.1/omniply/tools/
--rwxr-xr-x   0 fleeb     (7343) is        (1040)      239 2023-08-30 14:47:46.000000 omniply-0.2.1/omniply/tools/__init__.py
--rwxr-xr-x   0 fleeb     (7343) is        (1040)     6932 2023-08-30 14:47:46.000000 omniply-0.2.1/omniply/tools/abstract.py
--rwxr-xr-x   0 fleeb     (7343) is        (1040)     2795 2023-08-30 14:47:46.000000 omniply-0.2.1/omniply/tools/assessments.py
--rwxr-xr-x   0 fleeb     (7343) is        (1040)     6469 2023-08-30 14:47:46.000000 omniply-0.2.1/omniply/tools/context.py
--rwxr-xr-x   0 fleeb     (7343) is        (1040)    19265 2023-08-30 14:47:46.000000 omniply-0.2.1/omniply/tools/crafts.py
--rwxr-xr-x   0 fleeb     (7343) is        (1040)      727 2023-08-30 14:47:46.000000 omniply-0.2.1/omniply/tools/errors.py
--rwxr-xr-x   0 fleeb     (7343) is        (1040)     8057 2023-08-30 14:47:46.000000 omniply-0.2.1/omniply/tools/kits.py
--rwxr-xr-x   0 fleeb     (7343) is        (1040)     6214 2023-08-30 14:47:46.000000 omniply-0.2.1/omniply/tools/moguls.py
--rwxr-xr-x   0 fleeb     (7343) is        (1040)     1965 2023-08-30 14:47:46.000000 omniply-0.2.1/omniply/tools/top.py
-drwxr-xr-x   0 fleeb     (7343) is        (1040)        0 2024-02-13 13:40:56.210778 omniply-0.2.1/omniply/util/
--rwxr-xr-x   0 fleeb     (7343) is        (1040)      199 2023-08-30 14:47:46.000000 omniply-0.2.1/omniply/util/__init__.py
--rwxr-xr-x   0 fleeb     (7343) is        (1040)      541 2023-08-30 14:47:46.000000 omniply-0.2.1/omniply/util/data.py
--rwxr-xr-x   0 fleeb     (7343) is        (1040)      716 2023-08-30 14:47:46.000000 omniply-0.2.1/omniply/util/math.py
--rwxr-xr-x   0 fleeb     (7343) is        (1040)      987 2023-08-30 14:47:46.000000 omniply-0.2.1/omniply/util/misc.py
--rwxr-xr-x   0 fleeb     (7343) is        (1040)      855 2023-08-30 14:47:46.000000 omniply-0.2.1/omniply/util/tensors.py
--rwxr-xr-x   0 fleeb     (7343) is        (1040)      358 2023-08-30 14:47:46.000000 omniply-0.2.1/omniply/util/viz.py
-drwxr-xr-x   0 fleeb     (7343) is        (1040)        0 2024-02-13 13:40:56.202778 omniply-0.2.1/omniply.egg-info/
--rw-r--r--   0 fleeb     (7343) is        (1040)      517 2024-02-13 13:40:56.000000 omniply-0.2.1/omniply.egg-info/PKG-INFO
--rw-r--r--   0 fleeb     (7343) is        (1040)     2751 2024-02-13 13:40:56.000000 omniply-0.2.1/omniply.egg-info/SOURCES.txt
--rw-r--r--   0 fleeb     (7343) is        (1040)        1 2024-02-13 13:40:56.000000 omniply-0.2.1/omniply.egg-info/dependency_links.txt
--rw-r--r--   0 fleeb     (7343) is        (1040)       15 2024-02-13 13:40:56.000000 omniply-0.2.1/omniply.egg-info/requires.txt
--rw-r--r--   0 fleeb     (7343) is        (1040)        8 2024-02-13 13:40:56.000000 omniply-0.2.1/omniply.egg-info/top_level.txt
--rwxr-xr-x   0 fleeb     (7343) is        (1040)      427 2024-02-13 13:40:56.214778 omniply-0.2.1/setup.cfg
--rwxr-xr-x   0 fleeb     (7343) is        (1040)       38 2023-08-30 14:47:46.000000 omniply-0.2.1/setup.py
+drwxr-xr-x   0 fleeb     (7343) is        (1040)        0 2024-04-06 12:19:43.529205 omniply-0.3/
+-rw-r--r--   0 fleeb     (7343) is        (1040)     1067 2024-02-14 16:25:24.000000 omniply-0.3/LICENSE
+-rw-r--r--   0 fleeb     (7343) is        (1040)      516 2024-04-06 12:19:43.529205 omniply-0.3/PKG-INFO
+-rw-r--r--   0 fleeb     (7343) is        (1040)      216 2024-02-14 16:25:24.000000 omniply-0.3/README.md
+drwxr-xr-x   0 fleeb     (7343) is        (1040)        0 2024-04-06 12:19:43.525205 omniply-0.3/omniply/
+-rw-r--r--   0 fleeb     (7343) is        (1040)       60 2024-04-06 12:17:07.000000 omniply-0.3/omniply/__init__.py
+drwxr-xr-x   0 fleeb     (7343) is        (1040)        0 2024-04-06 12:19:43.525205 omniply-0.3/omniply/_future/
+-rw-r--r--   0 fleeb     (7343) is        (1040)        0 2024-02-14 16:25:24.000000 omniply-0.3/omniply/_future/__init__.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)     2501 2024-02-14 16:25:24.000000 omniply-0.3/omniply/_future/common.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)     4287 2024-02-14 16:25:24.000000 omniply-0.3/omniply/_future/specification.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)     3749 2024-02-14 16:25:24.000000 omniply-0.3/omniply/_future/wrappers.py
+drwxr-xr-x   0 fleeb     (7343) is        (1040)        0 2024-04-06 12:19:43.525205 omniply-0.3/omniply/apps/
+-rw-r--r--   0 fleeb     (7343) is        (1040)      159 2024-03-27 17:40:13.000000 omniply-0.3/omniply/apps/__init__.py
+drwxr-xr-x   0 fleeb     (7343) is        (1040)        0 2024-04-06 12:19:43.529205 omniply-0.3/omniply/apps/iterative/
+-rw-r--r--   0 fleeb     (7343) is        (1040)       25 2024-03-29 16:54:35.000000 omniply-0.3/omniply/apps/iterative/__init__.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)     1580 2024-03-29 17:08:38.000000 omniply-0.3/omniply/apps/iterative/abstract.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)      671 2024-03-29 16:54:35.000000 omniply-0.3/omniply/apps/iterative/guru.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)      188 2024-03-17 13:15:20.000000 omniply-0.3/omniply/apps/iterative/imports.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)      723 2024-03-29 16:47:20.000000 omniply-0.3/omniply/apps/iterative/innovators.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)     1343 2024-03-29 16:54:35.000000 omniply-0.3/omniply/apps/iterative/moguls.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)     3654 2024-03-29 16:05:33.000000 omniply-0.3/omniply/apps/simple.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)     1360 2024-03-29 15:44:11.000000 omniply-0.3/omniply/apps/staging.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)     1384 2024-03-15 14:29:45.000000 omniply-0.3/omniply/apps/templating.py
+drwxr-xr-x   0 fleeb     (7343) is        (1040)        0 2024-04-06 12:19:43.529205 omniply-0.3/omniply/core/
+-rw-r--r--   0 fleeb     (7343) is        (1040)      171 2024-03-14 13:44:31.000000 omniply-0.3/omniply/core/__init__.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)     8643 2024-03-28 15:53:05.000000 omniply-0.3/omniply/core/abstract.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)     2050 2024-02-14 16:25:24.000000 omniply-0.3/omniply/core/errors.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)     6732 2024-03-24 15:18:18.000000 omniply-0.3/omniply/core/gadgets.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)    11322 2024-03-24 16:04:01.000000 omniply-0.3/omniply/core/gaggles.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)     8118 2024-03-24 14:49:06.000000 omniply-0.3/omniply/core/gangs.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)     8762 2024-03-29 16:12:01.000000 omniply-0.3/omniply/core/genetics.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)    10998 2024-03-24 14:47:29.000000 omniply-0.3/omniply/core/gigs.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)     1353 2024-02-14 16:25:24.000000 omniply-0.3/omniply/core/gizmos.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)     5275 2024-03-28 17:28:50.000000 omniply-0.3/omniply/core/op.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)     7135 2024-03-29 16:12:01.000000 omniply-0.3/omniply/core/tools.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)    27493 2024-03-28 17:26:39.000000 omniply-0.3/omniply/core/unit_test.py
+drwxr-xr-x   0 fleeb     (7343) is        (1040)        0 2024-04-06 12:19:43.529205 omniply-0.3/omniply/spaces/
+-rw-r--r--   0 fleeb     (7343) is        (1040)        0 2024-03-24 13:57:26.000000 omniply-0.3/omniply/spaces/__init__.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)        0 2024-03-24 13:58:04.000000 omniply-0.3/omniply/spaces/imports.py
+drwxr-xr-x   0 fleeb     (7343) is        (1040)        0 2024-04-06 12:19:43.525205 omniply-0.3/omniply.egg-info/
+-rw-r--r--   0 fleeb     (7343) is        (1040)      516 2024-04-06 12:19:43.000000 omniply-0.3/omniply.egg-info/PKG-INFO
+-rw-r--r--   0 fleeb     (7343) is        (1040)      961 2024-04-06 12:19:43.000000 omniply-0.3/omniply.egg-info/SOURCES.txt
+-rw-r--r--   0 fleeb     (7343) is        (1040)        1 2024-04-06 12:19:43.000000 omniply-0.3/omniply.egg-info/dependency_links.txt
+-rw-r--r--   0 fleeb     (7343) is        (1040)       15 2024-04-06 12:19:43.000000 omniply-0.3/omniply.egg-info/requires.txt
+-rw-r--r--   0 fleeb     (7343) is        (1040)        8 2024-04-06 12:19:43.000000 omniply-0.3/omniply.egg-info/top_level.txt
+-rw-r--r--   0 fleeb     (7343) is        (1040)      428 2024-04-06 12:19:43.529205 omniply-0.3/setup.cfg
+-rw-r--r--   0 fleeb     (7343) is        (1040)       38 2024-02-14 16:25:24.000000 omniply-0.3/setup.py
```

### Comparing `omniply-0.2.1/LICENSE` & `omniply-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `omniply-0.2.1/PKG-INFO` & `omniply-0.3/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: omniply
-Version: 0.2.1
+Version: 0.3
 Summary: "Omni-ply Versatile Data Management for Rapid AI Prototyping and Research"
 Author: Felix Leeb
 License: MIT
-Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 # omni-ply
 
 > Before your code complexity multiplies, use omniply.
```

### Comparing `omniply-0.2.1/omniply/_future/common.py` & `omniply-0.3/omniply/_future/common.py`

 * *Files identical despite different names*

### Comparing `omniply-0.2.1/omniply/_future/specification.py` & `omniply-0.3/omniply/_future/specification.py`

 * *Files identical despite different names*

### Comparing `omniply-0.2.1/omniply/_future/wrappers.py` & `omniply-0.3/omniply/_future/wrappers.py`

 * *Files identical despite different names*

### Comparing `omniply-0.2.1/omniply/core/abstract.py` & `omniply-0.3/omniply/core/abstract.py`

 * *Files 14% similar despite different names*

```diff
@@ -104,15 +104,15 @@
 			Any: The specified output gizmo.
 
 		Raises:
 			ToolFailedError: If the gizmo cannot be grabbed (possibly because a necessary input gizmo is missing).
 		"""
 		raise NotImplementedError
 
-	def grabable(self, gizmo: str) -> bool:
+	def gives(self, gizmo: str) -> bool:
 		"""
 		Checks if this tool can produce the given gizmo.
 
 		Args:
 			gizmo (str): The gizmo to check.
 
 		Returns:
@@ -172,59 +172,19 @@
 
 		Returns:
 			Iterator[AbstractGadget]: An iterator over the known gadgets that can directly produce the given gizmo.
 		"""
 		raise NotImplementedError
 
 
-class AbstractMultiGadget(AbstractGaggle):
-	"""
-	AbstractMultiGadget is a special kind of gaggle that hides all sub-gadgets from being accessed through `gadgets()`
-	and `vendors()`. Instead, it presents itself as a gadget that can produce all the products of the sub-gadgets.
-
-	Generally, if you know before runtime what gizmos a gadget can produce, then it should just be a gadget, however,
-	if you want to be able to dynamically add sub-gadgets, while still preventing delegation, then you can use this.
-
-	"""
-
-	def gadgets(self, gizmo: Optional[str] = None) -> Iterator[AbstractGadget]:
-		"""
-		Lists all known gadgets under this multi-gadget that can produce the given gizmo.
-		Since this is a multi-gadget, it doesn't delegate to sub-gadgets, and instead yields itself.
-
-		Args:
-			gizmo (Optional[str]): If specified, yields only the gadgets that can produce this gizmo. In this case, it
-			has no effect.
-
-		Returns:
-			Iterator[AbstractGadget]: An iterator over the known gadgets in this multi-gadget that can produce the
-			specified gizmo. Since this is a multi-gadget, it yields only itself.
-		"""
-		yield self
-
-	def vendors(self, gizmo: Optional[str] = None) -> Iterator[AbstractGadget]:
-		"""
-		Lists all known sub-gadgets and sub-gaggles in this multi-gadget that can produce the given gizmo.
-		Since this is a multi-gadget, it doesn't delegate to sub-gadgets, and instead yields itself.
-
-		Args:
-			gizmo (Optional[str]): If specified, yields only the gadgets that can produce this gizmo. In this case, it
-			checks if this multi-gadget can produce the gizmo.
-
-		Returns:
-			Iterator[AbstractGadget]: An iterator over the known gadgets that can directly produce the given gizmo. Since
-			this is a multi-gadget, it yields itself.
-		"""
-		yield self
-
-
 _unique_gig_default_value = object()
 
 
-class AbstractGig(AbstractMultiGadget):
+
+class AbstractGig(AbstractGaggle):
 	"""
 	Gigs are usually the top-level interface for users to use the inference engine of `omni-ply`. Gigs are a special
 	kind of gaggle that takes ownership of a `grab_from()` call, rather than (usually silently) delegating to an
 	appropriate gadget to produce the specified gizmo. This also means gigs are responsible providing the current
 	context for gadgets (which often includes caching existing gizmos).
 	"""
 
@@ -286,9 +246,29 @@
 		Returns:
 			str: The external gizmo name.
 		"""
 		raise NotImplementedError
 
 
 
-# Moguls -> Guru
+### exotic animals
+
+
+
+
+class AbstractConsistentGig(AbstractGig):
+	def is_unchanged(self, gizmo: str):
+		raise NotImplementedError
+
+
+	def update_gadget_cache(self, gadget: AbstractGadget, cache: dict[str,Any] = None):
+		raise NotImplementedError
+
+
+	def check_gadget_cache(self, gadget: AbstractGadget):
+		raise NotImplementedError
+
+
+
+
+
```

### Comparing `omniply-0.2.1/omniply/core/errors.py` & `omniply-0.3/omniply/core/errors.py`

 * *Files identical despite different names*

### Comparing `omniply-0.2.1/omniply/core/gadgets.py` & `omniply-0.3/omniply/core/gadgets.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from typing import Iterator, Optional, Any, Iterable, Callable
-from omnibelt import extract_function_signature
+from omnibelt import extract_function_signature, extract_missing_args
 from omnibelt.crafts import AbstractSkill, NestableCraft
 
 from .errors import GadgetFailure, MissingGadget
 from .abstract import AbstractGadget, AbstractGaggle, AbstractGig
 
 
 class GadgetBase(AbstractGadget):
@@ -15,14 +15,15 @@
 		_GadgetFailure: The general exception that is raised when a gadget fails.
 		_MissingGadgetError: The exception that is raised when a required gizmo is missing.
 	"""
 	_GadgetFailure = GadgetFailure
 	_MissingGadgetError = MissingGadget
 
 
+
 class SingleGadgetBase(GadgetBase):
 	"""
 	SingleGadgetBase is a simple bass class for gadgets that only produce a single gizmo, which is specified at init.
 
 	Attributes:
 		_gizmo (str): The gizmo that this gadget grabs.
 	"""
@@ -44,15 +45,47 @@
 
 		Returns:
 			Iterator[str]: An iterator over the gizmo that this gadget grabs.
 		"""
 		yield self._gizmo
 
 
-class FunctionGadget(SingleGadgetBase):
+	def _grab_from(self, ctx: AbstractGig):
+		"""
+		Grabs the gizmo from the given context. This method is called by grab_from.
+
+		Args:
+			ctx (AbstractGig): The context from which to grab the gizmo.
+
+		Returns:
+			Any: The grabbed gizmo.
+		"""
+		raise NotImplementedError
+
+
+	def grab_from(self, ctx: Optional[AbstractGig], gizmo: str) -> Any:
+		"""
+		Returns the given gizmo from this gadget, or raises MissingGadgetError if the gizmo cannot be grabbed.
+
+		Args:
+			ctx (Optional[AbstractGig]): The context from which to grab the gizmo.
+			gizmo (str): The gizmo to grab.
+
+		Returns:
+			Any: The grabbed gizmo.
+
+		Raises:
+			MissingGadgetError: If the wrong gizmo is requested.
+		"""
+		# if gizmo != self._gizmo: raise self._MissingGadgetError(gizmo) # would cause issues with MIMO gadgets
+		return self._grab_from(ctx)
+
+
+
+class SingleFunctionGadget(SingleGadgetBase):
 	"""
 	FunctionGadget is a subclass of SingleGadgetBase for gadgets that produce a single gizmo using a given function.
 	The function should take a single argument, the context (gig), and return the output gizmo.
 
 	Attributes:
 		_gizmo (str): The gizmo that this gadget grabs.
 		_fn (Callable[[AbstractGig], Any]): The function that this gadget uses to grab the gizmo.
@@ -102,45 +135,41 @@
 			owner: The owner of the instance.
 
 		Returns:
 			Callable[[AbstractGig], Any]: The function that this gadget uses to grab the gizmo.
 		"""
 		return self._fn.__get__(instance, owner)
 
-	def grab_from(self, ctx: Optional[AbstractGig], gizmo: str) -> Any:
+
+	def _grab_from(self, ctx: AbstractGig) -> Any:
 		"""
-		Returns the given gizmo from this gadget, or raises MissingGadgetError if the gizmo cannot be grabbed.
+		Grabs the gizmo from the given context. This method is called by grab_from.
 
 		Args:
-			ctx (Optional[AbstractGig]): The context from which to grab the gizmo.
-			gizmo (str): The gizmo to grab.
+			ctx (AbstractGig): The context from which to grab the gizmo.
 
 		Returns:
 			Any: The grabbed gizmo.
-
-		Raises:
-			MissingGadgetError: If the wrong gizmo is requested.
 		"""
-		if gizmo != self._gizmo:
-			raise self._MissingGadgetError(gizmo)
 		return self._fn(ctx)
 
 
-class AutoFunctionGadget(FunctionGadget):
+class AutoSingleFunctionGadget(SingleFunctionGadget):
 	"""
 	AutoFunctionGadget is a subclass of FunctionGadget that produces a single gizmo using a given function.
 	The function can take any number of arguments, and any arguments that are gizmos will be grabbed from
 	the gig and passed to the function automatically.
 	The gizmo and the function are specified at initialization.
 
 	Attributes:
 		_gizmo (str): The gizmo that this gadget grabs.
 		_fn (Callable[tuple, Any]): The function that this gadget uses to grab the gizmo.
 	"""
 
+
 	@staticmethod
 	def _extract_gizmo_args(fn: Callable, ctx: AbstractGig, *, args: Optional[tuple] = None,
 							kwargs: Optional[dict[str, Any]] = None) -> tuple[list[Any], dict[str, Any]]:
 		"""
 		Extracts the arguments for the function that this gadget uses to grab the gizmo. Any arguments that are gizmos
 		are grabbed from the gig.
 
@@ -152,29 +181,39 @@
 
 		Returns:
 			tuple[list[Any], dict[str, Any]]: A tuple containing a list of positional arguments and a dictionary
 			of keyword arguments.
 		"""
 		return extract_function_signature(fn, args=args, kwargs=kwargs, default_fn=ctx.grab)
 
-	def grab_from(self, ctx: Optional[AbstractGig], gizmo: str) -> Any:
+
+	def _grab_from(self, ctx: AbstractGig) -> Any:
 		"""
-		Returns the given gizmo from this gadget, or raises MissingGadgetError if the gizmo cannot be grabbed.
-		The function that this gadget uses to grab the gizmo is called with the arguments extracted by _extract_gizmo_args.
+		Grabs the gizmo from the given context. This method is called by grab_from.
 
 		Args:
-			ctx (Optional[AbstractGig]): The context from which to grab the gizmo.
-			gizmo (str): The gizmo to grab.
+			ctx (AbstractGig): The context from which to grab the gizmo.
 
 		Returns:
 			Any: The grabbed gizmo.
-
-		Raises:
-			MissingGadgetError: If the wrong gizmo is requested.
 		"""
-		if gizmo != self._gizmo:
-			raise self._MissingGadgetError(gizmo)
-
 		args, kwargs = self._extract_gizmo_args(self._fn, ctx)
 		return self._fn(*args, **kwargs)
 
 
+
+class FunctionGadget(SingleGadgetBase):
+	'''the function is expected to be MISO'''
+	def __init__(self, fn: Callable = None, **kwargs):
+		super().__init__(**kwargs)
+		self._fn = fn
+
+
+	def _grab_from(self, ctx: 'AbstractGig') -> Any:
+		return self._fn(ctx)
+
+
+	@property
+	def __call__(self):
+		return self._fn
+
+
```

### Comparing `omniply-0.2.1/omniply/core/gaggles.py` & `omniply-0.3/omniply/core/gaggles.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from itertools import chain
 from collections import OrderedDict
 from omnibelt import filter_duplicates
 from omnibelt.crafts import InheritableCrafty
 
 from .abstract import AbstractGadget, AbstractGaggle, AbstractGig
 from .errors import logger, GadgetFailure, MissingGadget, AssemblyError
-from .gadgets import GadgetBase, SingleGadgetBase, FunctionGadget, AutoFunctionGadget
+from .gadgets import GadgetBase, SingleGadgetBase, SingleFunctionGadget, AutoSingleFunctionGadget
 
 
 
 class GaggleBase(GadgetBase, AbstractGaggle):
 	"""
 	The GaggleBase class is a base class for creating custom gaggles. It uses a protected _gadgets_table dictionary to
 	keep track of all the subgadgets, and consequently implements the expected API for gaggles.
@@ -41,15 +41,15 @@
 
 	def gizmos(self) -> Iterator[str]:
 		"""
 		Iterates over all known gizmos that this gaggle can produce in order of oldest to newest.
 		"""
 		yield from self._gadgets_table.keys()
 
-	def grabable(self, gizmo: str) -> bool:
+	def gives(self, gizmo: str) -> bool:
 		"""
 		Checks if a gizmo is can be produced by this gaggle.
 
 		Args:
 			gizmo (str): The name of the gizmo to check.
 
 		Returns:
@@ -77,25 +77,25 @@
 		Args:
 			gizmo (Optional[str]): The name of the gizmo to check. If not provided, all gadgets are returned.
 
 		Returns:
 			Iterator[AbstractGadget]: An iterator over the gadgets that can produce the given gizmo.
 		"""
 		if gizmo is None:
-			for gadget in filter_duplicates(chain.from_iterable(map(reversed, self._gadgets_table.values()))):
+			for gadget in chain.from_iterable(map(reversed, self._gadgets_table.values())):
 				if isinstance(gadget, AbstractGaggle):
-					yield from gadget.gadgets(gizmo)
+					yield from gadget.vendors(gizmo)
 				else:
 					yield gadget
 		else:
 			if gizmo not in self._gadgets_table:
 				raise self._MissingGadgetError(gizmo)
-			for gadget in filter_duplicates(reversed(self._gadgets_table[gizmo])):
+			for gadget in reversed(self._gadgets_table[gizmo]):
 				if isinstance(gadget, AbstractGaggle):
-					yield from gadget.gadgets(gizmo)
+					yield from gadget.vendors(gizmo)
 				else:
 					yield gadget
 
 	_AssemblyFailedError = AssemblyError
 	def grab_from(self, ctx: AbstractGig, gizmo: str) -> Any:
 		"""
 		Tries to grab a gizmo using the subgadgets given the context.
@@ -120,14 +120,57 @@
 			except:
 				logger.debug(f'{gadget!r} failed while trying to produce {gizmo!r}')
 				raise
 		if failures:
 			raise self._AssemblyFailedError(failures)
 		raise self._MissingGadgetError(gizmo)
 
+
+
+class MultiGadgetBase(AbstractGaggle):
+	"""
+	MultiGadgetBase is a special kind of gaggle that hides all sub-gadgets from being accessed through `gadgets()`
+	and `vendors()`. Instead, it presents itself as a gadget that can produce all the products of the sub-gadgets.
+
+	Generally, if you know before runtime what gizmos a gadget can produce, then it should just be a gadget, however,
+	if you want to be able to dynamically add sub-gadgets, while still preventing delegation, then you can use this.
+
+	"""
+	def gadgets(self, gizmo: Optional[str] = None) -> Iterator[AbstractGadget]:
+		"""
+		Lists all known gadgets under this multi-gadget that can produce the given gizmo.
+		Since this is a multi-gadget, it doesn't delegate to sub-gadgets, and instead yields itself.
+
+		Args:
+			gizmo (Optional[str]): If specified, yields only the gadgets that can produce this gizmo. In this case, it
+			has no effect.
+
+		Returns:
+			Iterator[AbstractGadget]: An iterator over the known gadgets in this multi-gadget that can produce the
+			specified gizmo. Since this is a multi-gadget, it yields only itself.
+		"""
+		yield self
+
+	def vendors(self, gizmo: Optional[str] = None) -> Iterator[AbstractGadget]:
+		"""
+		Lists all known sub-gadgets and sub-gaggles in this multi-gadget that can produce the given gizmo.
+		Since this is a multi-gadget, it doesn't delegate to sub-gadgets, and instead yields itself.
+
+		Args:
+			gizmo (Optional[str]): If specified, yields only the gadgets that can produce this gizmo. In this case, it
+			checks if this multi-gadget can produce the gizmo.
+
+		Returns:
+			Iterator[AbstractGadget]: An iterator over the known gadgets that can directly produce the given gizmo. Since
+			this is a multi-gadget, it yields itself.
+		"""
+		yield self
+
+
+
 class LoopyGaggle(GaggleBase):
 	"""
 	The LoopyGaggle class is mix-in for custom gaggles that allows multiple gadgets that produce the same gizmos to
 	recursively call each other. Specifically, if a subgadget requires the same gizmo as input as it produces, then the
 	next known subgadget of this gaggle is used after which the stack is resolved.
 
 	Attributes:
@@ -259,16 +302,21 @@
 		history = OrderedDict() # src<N-O> : craft<N-O>
 		for src, key, craft in self._emit_all_craft_items(): # craft<N-O>
 			history.setdefault(src, []).append(craft)
 
 		# convert crafts to skills and add in O-N (N-O) order to table
 		for crafts in reversed(history.values()): # O-N
 			gizmos = {}
-			for craft in reversed(crafts): # N-O (in order of presidence)
-				skill = craft.as_skill(self)
+			for craft in reversed(crafts): # N-O (in order of precedence)
+				skill = craft.as_skill(self) # TODO: convert as_skill to a generator to enable multiple skills per craft
 				if isinstance(skill, AbstractGadget):
 					for gizmo in skill.gizmos():
 						gizmos.setdefault(gizmo, []).append(skill)
+				else:
+					self._process_auxiliary_skill(skill)
 			for gizmo, skills in gizmos.items():
 				self._gadgets_table.setdefault(gizmo, []).extend(reversed(skills)) # O-N (in order of appearance)
 
 
+	def _process_auxiliary_skill(self, skill):
+		pass
+
```

### Comparing `omniply-0.2.1/omniply/core/gizmos.py` & `omniply-0.3/omniply/core/gizmos.py`

 * *Files identical despite different names*

### Comparing `omniply-0.2.1/omniply/core/groups.py` & `omniply-0.3/omniply/core/gangs.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,279 +1,279 @@
-from typing import Any, Optional, Iterator
-from collections import UserDict
-from omnibelt import filter_duplicates
-
-from .abstract import AbstractGang, AbstractGig
-from .errors import GadgetFailure, ApplicationAmbiguityError
-from .gaggles import GaggleBase
-from .gigs import GigBase, GroupCache
-
-
-class GroupBase(GaggleBase, AbstractGang):
-	"""
-	The GroupBase class is a subclass of GaggleBase and AbstractGroup. It provides methods to handle gizmo grabbing and packaging.
-
-	Attributes:
-		_current_context (Optional[AbstractGig]): The current context of the group.
-	"""
-
-	_current_context: Optional[AbstractGig]
-
-	def __init__(self, *args, gap: Optional[dict[str, str]] = None, **kwargs):
-		"""
-		Initializes a new instance of the GroupBase class.
-
-		Args:
-			args: Variable length argument list.
-			gap (Optional[dict[str, str]]): A dictionary of gizmo mappings. If not provided, an empty dictionary will be used.
-			kwargs: Arbitrary keyword arguments.
-		"""
-		if gap is None:
-			gap = {}
-		super().__init__(*args, **kwargs)
-		self._raw_gap = gap # internal gizmos -> external gizmos
-		self._raw_reverse_gap = None
-		self._gig_stack = []
-
-	def _gizmos(self) -> Iterator[str]:
-		"""
-		Lists gizmos produced by self using internal names.
-
-		Returns:
-			Iterator[str]: An iterator over the gizmos.
-		"""
-		yield from super().gizmos()
-
-	def gizmos(self) -> Iterator[str]:
-		"""
-		Lists gizmos produced by self using external names.
-
-		Returns:
-			Iterator[str]: An iterator over the gizmos.
-		"""
-		for gizmo in self._gizmos():
-			yield self.gizmo_to(gizmo)
-
-	@property
-	def internal2external(self) -> dict[str, str]:
-		"""
-		Getter for the internal to external gizmo mapping.
-
-		Returns:
-			dict[str, str]: The internal to external gizmo mapping.
-		"""
-		return self._raw_gap
-
-	@internal2external.setter
-	def internal2external(self, value: dict[str, str]):
-		"""
-		Setter for the internal to external gizmo mapping.
-
-		Args:
-			value (dict[str, str]): The new internal to external gizmo mapping.
-		"""
-		self._raw_gap = value
-		self._raw_reverse_gap = None
-
-	@property
-	def external2internal(self) -> dict[str, str]:
-		"""
-		Getter for the external to internal gizmo mapping.
-
-		Returns:
-			dict[str, str]: The external to internal gizmo mapping.
-		"""
-		if self._raw_reverse_gap is None:
-			self._raw_reverse_gap = self._infer_external2internal(self._raw_gap, self._gizmos())
-		return self._raw_reverse_gap
-
-	@staticmethod
-	def _infer_external2internal(raw: dict[str, str], products: Iterator[str]) -> dict[str, str]:
-		"""
-		Infers the external to internal gizmo mapping from the provided raw mapping and products.
-
-		Args:
-			raw (dict[str, str]): The raw gizmo mapping.
-			products (Iterator[str]): An iterator over the products.
-
-		Returns:
-			dict[str, str]: The inferred external to internal gizmo mapping.
-		"""
-		reverse = {}
-		for product in products:
-			if product in raw:
-				external = raw[product]
-				if external in reverse:
-					raise ApplicationAmbiguityError(product, [reverse[external], product])
-				reverse[external] = product
-		return reverse
-
-	def gizmo_from(self, gizmo: str) -> str:
-		"""
-		Converts an external gizmo to its internal representation.
-
-		Args:
-			gizmo (str): The external gizmo.
-
-		Returns:
-			str: The internal representation of the gizmo.
-		"""
-		return self.external2internal.get(gizmo, gizmo)
-
-	def gizmo_to(self, gizmo: str) -> str:
-		"""
-		Converts an internal gizmo to its external representation.
-
-		Args:
-			gizmo (str): The internal gizmo.
-
-		Returns:
-			str: The external representation of the gizmo.
-		"""
-		return self.internal2external.get(gizmo, gizmo)
-
-	def _grab(self, gizmo: str):
-		"""
-		Grabs a gizmo from self.
-
-		Args:
-			gizmo (str): The name of the gizmo to grab.
-
-		Returns:
-			Any: The grabbed gizmo.
-		"""
-		return super().grab_from(self, gizmo)
-
-	def grab_from(self, ctx: AbstractGig, gizmo: str) -> Any:
-		"""
-		Tries to grab a gizmo from the context.
-
-		Args:
-			ctx (Optional[AbstractGig]): The context from which to grab the gizmo.
-			gizmo (str): The name of the gizmo to grab.
-
-		Returns:
-			Any: The grabbed gizmo.
-		"""
-		if ctx is not None and ctx is not self:
-			self._gig_stack.append(ctx)
-			gizmo = self.gizmo_from(gizmo)  # convert to internal gizmo
-
-		try:
-			out = self._grab(gizmo)
-		except self._GadgetFailure:
-			if len(self._gig_stack) == 0 or ctx is self._gig_stack[-1]:
-				raise
-			# default to parent/s
-			out = self._gig_stack[-1].grab(self.gizmo_to(gizmo))
-
-		if len(self._gig_stack) and ctx is self._gig_stack[-1]:
-			self._gig_stack.pop()
-
-		return out
-
-	# def _grab_from_fallback(self, error: Exception, ctx: Optional[AbstractGig], gizmo: str) -> Any:
-	# 	assert ctx is self, f'{ctx} != {self}'
-	# 	if len(self._gig_stack):
-	# 		return super()._grab_from_fallback(error, self._gig_stack[-1], self.gizmo_to(gizmo))
-	# 	raise error from error
-	#
-	#
-	# def grab_from(self, ctx: Optional[AbstractGig], gizmo: str) -> Any:
-	# 	if ctx is not None and ctx is not self:
-	# 		self._gig_stack.append(ctx)
-	# 		gizmo = self.gizmo_from(gizmo) # convert to internal gizmo
-	# 	out = super().grab_from(self, gizmo)
-	# 	if len(self._gig_stack) and ctx is self._gig_stack[-1]:
-	# 		self._gig_stack.pop()
-	# 	return out
-
-
-class CachableGroup(GroupBase):
-	"""
-	The CachableGroup class is a subclass of GroupBase. It provides methods to handle gizmo grabbing with cache support.
-
-	Attributes:
-		_GroupCacheMiss (KeyError): The exception to be raised when a cache miss occurs.
-	"""
-
-	_GroupCacheMiss = KeyError
-
-	def _grab(self, gizmo: str) -> Any:
-		"""
-		Tries to grab a gizmo from the group. If the gizmo is not found in the group's cache, it checks the cache using
-		the external gizmo name. If it still can't be found in any cache, it grabs it from the group's gadgets.
-
-		Args:
-			gizmo (str): The name of the gizmo to grab.
-
-		Returns:
-			Any: The grabbed gizmo.
-		"""
-		if len(self._gig_stack):
-			# check cache (if one exists)
-			for parent in reversed(self._gig_stack):
-				if isinstance(parent, GroupCache):
-					try:
-						return parent.check_group_cache(self, gizmo)
-					except self._GroupCacheMiss:
-						pass
-
-			# if it can't be found in my cache, check the cache using the external gizmo name
-			ext = self.gizmo_to(gizmo)
-			for parent in reversed(self._gig_stack):
-				if isinstance(parent, GroupCache) and parent.is_cached(ext):
-					return parent.grab(ext)
-
-		# if it can't be found in any cache, grab it from my gadgets
-		out = super()._grab(gizmo)
-
-		# update my cache
-		if len(self._gig_stack):
-			for parent in reversed(self._gig_stack):
-				if isinstance(parent, GroupCache):
-					parent.update_group_cache(self, gizmo, out)
-					break
-
-		return out
-
-
-class SelectiveGroup(GroupBase):
-	"""
-	The SelectiveGroup class is a subclass of GroupBase. It provides methods to handle selective gizmo mapping.
-
-	Args:
-		args: Variable length argument list.
-		gap (dict[str, str] | list[str] | None): A dictionary or list of gizmo mappings. If not provided, an empty dictionary will be used.
-		kwargs: Arbitrary keyword arguments.
-	"""
-
-	def __init__(self, *args, gap: dict[str, str] | list[str] | None = None, **kwargs):
-		"""
-		Initializes a new instance of the SelectiveGroup class.
-
-		If the gap argument is a list, it is converted to a dictionary with the same keys and values.
-		If the gap argument is a dictionary, it is processed to ensure that all values are not None.
-
-		Args:
-			args: Variable length argument list.
-			gap (dict[str, str] | list[str] | None): A dictionary or list of gizmo mappings. If not provided, an empty dictionary will be used.
-			kwargs: Arbitrary keyword arguments.
-		"""
-		if isinstance(gap, list):
-			gap = {gizmo: gizmo for gizmo in gap}
-		if isinstance(gap, dict):
-			gap = {gizmo: gizmo if ext is None else ext for gizmo, ext in gap.items()}
-		super().__init__(*args, gap=gap, **kwargs)
-
-	def gizmos(self) -> Iterator[str]:
-		"""
-		Lists gizmos produced by self using external names.
-
-		Returns:
-			Iterator[str]: An iterator over the gizmos.
-		"""
-		for gizmo in self._gizmos():
-			if gizmo in self.internal2external:
-				yield self.gizmo_to(gizmo)
-
-
+from typing import Any, Optional, Iterator
+from collections import UserDict
+from omnibelt import filter_duplicates
+
+from .abstract import AbstractGang, AbstractGig
+from .errors import GadgetFailure, ApplicationAmbiguityError
+from .gaggles import GaggleBase, MultiGadgetBase
+from .gigs import GigBase, GroupCache
+
+
+class GroupBase(MultiGadgetBase, GaggleBase, AbstractGang):
+	"""
+	The GroupBase class is a subclass of GaggleBase and AbstractGroup. It provides methods to handle gizmo grabbing and packaging.
+
+	Attributes:
+		_current_context (Optional[AbstractGig]): The current context of the group.
+	"""
+
+	_current_context: Optional[AbstractGig]
+
+	def __init__(self, *args, gap: Optional[dict[str, str]] = None, **kwargs):
+		"""
+		Initializes a new instance of the GroupBase class.
+
+		Args:
+			args: Variable length argument list.
+			gap (Optional[dict[str, str]]): A dictionary of gizmo mappings. If not provided, an empty dictionary will be used.
+			kwargs: Arbitrary keyword arguments.
+		"""
+		if gap is None:
+			gap = {}
+		super().__init__(*args, **kwargs)
+		self._raw_gap = gap # internal gizmos -> external gizmos
+		self._raw_reverse_gap = None
+		self._gig_stack = []
+
+	def _gizmos(self) -> Iterator[str]:
+		"""
+		Lists gizmos produced by self using internal names.
+
+		Returns:
+			Iterator[str]: An iterator over the gizmos.
+		"""
+		yield from super().gizmos()
+
+	def gizmos(self) -> Iterator[str]:
+		"""
+		Lists gizmos produced by self using external names.
+
+		Returns:
+			Iterator[str]: An iterator over the gizmos.
+		"""
+		for gizmo in self._gizmos():
+			yield self.gizmo_to(gizmo)
+
+	@property
+	def internal2external(self) -> dict[str, str]:
+		"""
+		Getter for the internal to external gizmo mapping.
+
+		Returns:
+			dict[str, str]: The internal to external gizmo mapping.
+		"""
+		return self._raw_gap
+
+	@internal2external.setter
+	def internal2external(self, value: dict[str, str]):
+		"""
+		Setter for the internal to external gizmo mapping.
+
+		Args:
+			value (dict[str, str]): The new internal to external gizmo mapping.
+		"""
+		self._raw_gap = value
+		self._raw_reverse_gap = None
+
+	@property
+	def external2internal(self) -> dict[str, str]:
+		"""
+		Getter for the external to internal gizmo mapping.
+
+		Returns:
+			dict[str, str]: The external to internal gizmo mapping.
+		"""
+		if self._raw_reverse_gap is None:
+			self._raw_reverse_gap = self._infer_external2internal(self._raw_gap, self._gizmos())
+		return self._raw_reverse_gap
+
+	@staticmethod
+	def _infer_external2internal(raw: dict[str, str], products: Iterator[str]) -> dict[str, str]:
+		"""
+		Infers the external to internal gizmo mapping from the provided raw mapping and products.
+
+		Args:
+			raw (dict[str, str]): The raw gizmo mapping.
+			products (Iterator[str]): An iterator over the products.
+
+		Returns:
+			dict[str, str]: The inferred external to internal gizmo mapping.
+		"""
+		reverse = {}
+		for product in products:
+			if product in raw:
+				external = raw[product]
+				if external in reverse:
+					raise ApplicationAmbiguityError(product, [reverse[external], product])
+				reverse[external] = product
+		return reverse
+
+	def gizmo_from(self, gizmo: str) -> str:
+		"""
+		Converts an external gizmo to its internal representation.
+
+		Args:
+			gizmo (str): The external gizmo.
+
+		Returns:
+			str: The internal representation of the gizmo.
+		"""
+		return self.external2internal.get(gizmo, gizmo)
+
+	def gizmo_to(self, gizmo: str) -> str:
+		"""
+		Converts an internal gizmo to its external representation.
+
+		Args:
+			gizmo (str): The internal gizmo.
+
+		Returns:
+			str: The external representation of the gizmo.
+		"""
+		return self.internal2external.get(gizmo, gizmo)
+
+	def _grab(self, gizmo: str):
+		"""
+		Grabs a gizmo from self.
+
+		Args:
+			gizmo (str): The name of the gizmo to grab.
+
+		Returns:
+			Any: The grabbed gizmo.
+		"""
+		return super().grab_from(self, gizmo)
+
+	def grab_from(self, ctx: AbstractGig, gizmo: str) -> Any:
+		"""
+		Tries to grab a gizmo from the context.
+
+		Args:
+			ctx (Optional[AbstractGig]): The context from which to grab the gizmo.
+			gizmo (str): The name of the gizmo to grab.
+
+		Returns:
+			Any: The grabbed gizmo.
+		"""
+		if ctx is not None and ctx is not self:
+			self._gig_stack.append(ctx)
+			gizmo = self.gizmo_from(gizmo)  # convert to internal gizmo
+
+		try:
+			out = self._grab(gizmo)
+		except self._GadgetFailure:
+			if len(self._gig_stack) == 0 or ctx is self._gig_stack[-1]:
+				raise
+			# default to parent/s
+			out = self._gig_stack[-1].grab(self.gizmo_to(gizmo))
+
+		if len(self._gig_stack) and ctx is self._gig_stack[-1]:
+			self._gig_stack.pop()
+
+		return out
+
+	# def _grab_from_fallback(self, error: Exception, ctx: Optional[AbstractGig], gizmo: str) -> Any:
+	# 	assert ctx is self, f'{ctx} != {self}'
+	# 	if len(self._gig_stack):
+	# 		return super()._grab_from_fallback(error, self._gig_stack[-1], self.gizmo_to(gizmo))
+	# 	raise error from error
+	#
+	#
+	# def grab_from(self, ctx: Optional[AbstractGig], gizmo: str) -> Any:
+	# 	if ctx is not None and ctx is not self:
+	# 		self._gig_stack.append(ctx)
+	# 		gizmo = self.gizmo_from(gizmo) # convert to internal gizmo
+	# 	out = super().grab_from(self, gizmo)
+	# 	if len(self._gig_stack) and ctx is self._gig_stack[-1]:
+	# 		self._gig_stack.pop()
+	# 	return out
+
+
+class CachableGroup(GroupBase):
+	"""
+	The CachableGroup class is a subclass of GroupBase. It provides methods to handle gizmo grabbing with cache support.
+
+	Attributes:
+		_GroupCacheMiss (KeyError): The exception to be raised when a cache miss occurs.
+	"""
+
+	_GroupCacheMiss = KeyError
+
+	def _grab(self, gizmo: str) -> Any:
+		"""
+		Tries to grab a gizmo from the group. If the gizmo is not found in the group's cache, it checks the cache using
+		the external gizmo name. If it still can't be found in any cache, it grabs it from the group's gadgets.
+
+		Args:
+			gizmo (str): The name of the gizmo to grab.
+
+		Returns:
+			Any: The grabbed gizmo.
+		"""
+		if len(self._gig_stack):
+			# check cache (if one exists)
+			for parent in reversed(self._gig_stack):
+				if isinstance(parent, GroupCache):
+					try:
+						return parent.check_group_cache(self, gizmo)
+					except self._GroupCacheMiss:
+						pass
+
+			# if it can't be found in my cache, check the cache using the external gizmo name
+			ext = self.gizmo_to(gizmo)
+			for parent in reversed(self._gig_stack):
+				if isinstance(parent, GroupCache) and parent.is_cached(ext):
+					return parent.grab(ext)
+
+		# if it can't be found in any cache, grab it from my gadgets
+		out = super()._grab(gizmo)
+
+		# update my cache
+		if len(self._gig_stack):
+			for parent in reversed(self._gig_stack):
+				if isinstance(parent, GroupCache):
+					parent.update_group_cache(self, gizmo, out)
+					break
+
+		return out
+
+
+class SelectiveGroup(GroupBase):
+	"""
+	The SelectiveGroup class is a subclass of GroupBase. It provides methods to handle selective gizmo mapping.
+
+	Args:
+		args: Variable length argument list.
+		gap (dict[str, str] | list[str] | None): A dictionary or list of gizmo mappings. If not provided, an empty dictionary will be used.
+		kwargs: Arbitrary keyword arguments.
+	"""
+
+	def __init__(self, *args, gap: dict[str, str] | list[str] | None = None, **kwargs):
+		"""
+		Initializes a new instance of the SelectiveGroup class.
+
+		If the gap argument is a list, it is converted to a dictionary with the same keys and values.
+		If the gap argument is a dictionary, it is processed to ensure that all values are not None.
+
+		Args:
+			args: Variable length argument list.
+			gap (dict[str, str] | list[str] | None): A dictionary or list of gizmo mappings. If not provided, an empty dictionary will be used.
+			kwargs: Arbitrary keyword arguments.
+		"""
+		if isinstance(gap, list):
+			gap = {gizmo: gizmo for gizmo in gap}
+		if isinstance(gap, dict):
+			gap = {gizmo: gizmo if ext is None else ext for gizmo, ext in gap.items()}
+		super().__init__(*args, gap=gap, **kwargs)
+
+	def gizmos(self) -> Iterator[str]:
+		"""
+		Lists gizmos produced by self using external names.
+
+		Returns:
+			Iterator[str]: An iterator over the gizmos.
+		"""
+		for gizmo in self._gizmos():
+			if gizmo in self.internal2external:
+				yield self.gizmo_to(gizmo)
+
+
```

### Comparing `omniply-0.2.1/omniply/core/tools.py` & `omniply-0.3/omniply/core/tools.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,59 +1,30 @@
 from typing import Iterator, Optional, Any, Iterable, Callable
 from omnibelt.crafts import AbstractSkill, AbstractCraft, AbstractCrafty, NestableCraft
 
 from .abstract import AbstractGadget, AbstractGaggle, AbstractGig
-from .gadgets import GadgetBase, SingleGadgetBase, FunctionGadget, AutoFunctionGadget
+from .gadgets import GadgetBase, FunctionGadget
+from .genetics import AutoMIMOFunctionGadget, MIMOGadgetBase, Parentable, AbstractGenetic, Gene, ParentedSkill
 
 
-class ToolSkill(AbstractSkill):
-	"""
-	The ToolSkill class is a subclass of AbstractSkill. It provides methods to handle unbound functions and their bases.
-
-	Attributes:
-		_unbound_fn (Callable): The unbound function to be handled.
-		_base (Optional[AbstractCraft]): The base of the unbound function. Defaults to None.
-	"""
 
+class SkillBase(AbstractSkill):
 	def __init__(self, *, unbound_fn: Callable, base: Optional[AbstractCraft] = None, **kwargs):
-		"""
-		Initializes a new instance of the ToolSkill class.
-
-		Args:
-			unbound_fn (Callable): The unbound function to be handled.
-			base (Optional[AbstractCraft]): The base of the unbound function. If not provided, base will be None.
-			kwargs: Arbitrary keyword arguments.
-		"""
 		super().__init__(**kwargs)
 		self._unbound_fn = unbound_fn
 		self._base = base
 
-	def __get__(self, instance, owner):
-		"""
-		Returns the unbound function if the instance is None, otherwise it returns the bound method.
-
-		Args:
-			instance: The instance that the method is being accessed through, or None when the method is accessed through the owner.
-			owner: The owner class.
 
-		Returns:
-			Callable: The unbound function if the instance is None, otherwise the bound method.
-		"""
+	def __get__(self, instance, owner):
 		if instance is None:
 			return self
 		return self._unbound_fn.__get__(instance, owner)
 
-class ToolCraft(FunctionGadget, NestableCraft):
-	"""
-	The ToolCraft class is a subclass of FunctionGadget and NestableCraft. It provides methods to handle gizmos and their associated functions.
-
-	Attributes:
-		_ToolSkill (FunctionGadget, ToolSkill): A nested class that inherits from FunctionGadget and ToolSkill.
-	"""
 
+class CraftBase(NestableCraft):
 	@property
 	def __call__(self):
 		"""
 		Calling a ToolCraft instance directly results in the wrapped function being called.
 
 		Returns:
 			Callable: The wrapped function.
@@ -80,59 +51,70 @@
 		Note: If you want the actual function, use _wrapped_content_leaf.
 
 		Returns:
 			Callable: The wrapped function.
 		"""
 		return self._fn
 
-	class _ToolSkill(FunctionGadget, ToolSkill):
-		"""
-		The _ToolSkill class is a nested class that inherits from FunctionGadget and ToolSkill.
-		"""
-		pass
 
-	def as_skill(self, owner: AbstractCrafty) -> ToolSkill:
+
+class ToolCraftBase(FunctionGadget, CraftBase):
+	"""
+	The ToolCraft class is a subclass of FunctionGadget and NestableCraft. It provides methods to handle gizmos and their associated functions.
+
+	Attributes:
+		_ToolSkill (FunctionGadget, ToolSkill): A nested class that inherits from FunctionGadget and ToolSkill.
+	"""
+
+	_ToolSkill = None
+	def as_skill(self, owner: AbstractCrafty) -> SkillBase:
 		"""
 		When an AbstractCrafty is instantiated (i.e., `owner`), any crafts accessible by the class (including inherited ones) can be converted to skills.
 
 		Args:
 			owner (AbstractCrafty): The owner of the craft.
 
 		Returns:
 			ToolSkill: The converted skill.
 		"""
 		unbound_fn = self._wrapped_content_leaf()
 		fn = unbound_fn.__get__(owner, type(owner))
-		return self._ToolSkill(self._gizmo, fn=fn, unbound_fn=unbound_fn, base=self)
+		return self._ToolSkill(fn=fn, gizmo=self._gizmo, unbound_fn=unbound_fn, base=self)
 
 
-class AutoToolCraft(AutoFunctionGadget, ToolCraft):
-	"""
-	The AutoToolCraft class is a subclass of AutoFunctionGadget and ToolCraft. It provides methods to handle automatic
-	function gadgets and tool crafts.
 
-	Attributes:
-		_ToolSkill (AutoFunctionGadget, ToolSkill): A nested class that inherits from AutoFunctionGadget and ToolSkill.
-	"""
-
-	class _ToolSkill(AutoFunctionGadget, ToolSkill):
+class ToolCraft(Parentable, ToolCraftBase, MIMOGadgetBase):
+	class _ToolSkill(ParentedSkill, MIMOGadgetBase, SkillBase):
 		"""
-		The _ToolSkill class is a nested class that inherits from AutoFunctionGadget and ToolSkill. It provides methods
-		to handle automatic function gadgets and tool skills.
+		The _ToolSkill class is a nested class that inherits from FunctionGadget and ToolSkill.
 		"""
+		_Gene = Gene
+		def genes(self, gizmo: str) -> Iterator['AbstractGene']:
+			siblings = list(self.gizmos())
+			if len(siblings) == 1:
+				siblings = None
+			else:
+				siblings = tuple(sibling if sibling != gizmo else None for sibling in self.gizmos())
+			yield self._Gene(gizmo, self, parents=self.get_parents(), siblings=siblings, endpoint=self._fn)
+
+
+class AutoToolCraft(AutoMIMOFunctionGadget, ToolCraftBase):
+	class _ToolSkill(AutoMIMOFunctionGadget, SkillBase):
 		pass
 
-class ToolDecorator(GadgetBase):
+
+
+class ToolDecoratorBase(GadgetBase):
 	"""
 	The ToolDecorator class is a subclass of GadgetBase. It provides methods to handle gizmo decoration.
 
 	Attributes:
 		_gizmo_type (None): The type of the gizmo. Defaults to None.
 		_gizmo (str): The gizmo to be handled.
-		_ToolCraft (ToolCraft): A nested class that inherits from ToolCraft.
+		_ToolCraft (ToolCraftBase): A nested class that inherits from ToolCraft.
 	"""
 
 	_gizmo_type = None
 
 	def __init__(self, gizmo: str, **kwargs):
 		"""
 		Initializes a new instance of the ToolDecorator class.
@@ -151,23 +133,23 @@
 		Lists gizmos produced by self.
 
 		Returns:
 			Iterator[str]: An iterator over the gizmos.
 		"""
 		yield self._gizmo
 
-	def grabable(self, gizmo: str) -> bool:
+	def gives(self, gizmo: str) -> bool:
 		"""
-		Checks if a gizmo is grabable.
+		Checks if a gizmo is can be produced by this gadget.
 
 		Args:
 			gizmo (str): The name of the gizmo to check.
 
 		Returns:
-			bool: True if the gizmo is grabable, False otherwise.
+			bool: True if the gizmo can be grabbed, False otherwise.
 		"""
 		return gizmo == self._gizmo
 
 	def grab_from(self, ctx: Optional[AbstractGig], gizmo: str) -> Any:
 		"""
 		Tries to grab a gizmo from the context.
 
@@ -177,44 +159,85 @@
 
 		Returns:
 			Any: The grabbed gizmo.
 
 		Raises:
 			_GadgetFailed: If the gizmo cannot be grabbed.
 		"""
-		raise self._GadgetFailed(gizmo)
-
-	_ToolCraft = ToolCraft
+		raise self._GadgetFailure(gizmo)
 
+	_ToolCraft = ToolCraftBase
 	def _actualize_tool(self, fn: Callable, **kwargs):
 		"""
 		Actualizes a tool by creating a ToolCraft instance with the gizmo and the function.
 
 		Args:
 			fn (Callable): The function to be actualized.
 			kwargs: Arbitrary keyword arguments.
 
 		Returns:
-			ToolCraft: The actualized tool.
+			ToolCraftBase: The actualized tool.
 		"""
-		return self._ToolCraft(self._gizmo, fn=fn, **kwargs)
+		return self._ToolCraft(gizmo=self._gizmo, fn=fn, **kwargs)
 
 	def __call__(self, fn):
 		"""
 		Calling a ToolDecorator instance directly results in the actualization of the function.
 
 		Args:
 			fn (Callable): The function to be actualized.
 
 		Returns:
-			ToolCraft: The actualized tool.
+			ToolCraftBase: The actualized tool.
 		"""
 		return self._actualize_tool(fn)
 
-class AutoToolDecorator(ToolDecorator):
+
+
+class MIMOToolDecorator(ToolDecoratorBase):
+	_ToolCraft = ToolCraft
+
+	def __init__(self, *gizmos: str, **kwargs):
+		"""
+		Important: a single gizmo is always interpretted as a MISO (not MIMO).
+
+		To use a MIMO with a single output gizmo you must pass a 1-element tuple/list (why would you do that though?)
+
+		"""
+		gizmo = None
+		if len(gizmos) == 1:
+			if isinstance(gizmos[0], str):
+				gizmo = gizmos[0]
+				gizmos = None
+			else:
+				assert len(gizmos[0]) == 1, f'Cannot interpret {gizmos[0]} as a single gizmo'
+
+		if gizmos is not None:
+			gizmos = tuple(self._gizmo_type(gizmo) if isinstance(gizmo, str) and self._gizmo_type is not None
+						   else gizmo for gizmo in gizmos)
+		super().__init__(gizmo=gizmo, **kwargs)
+		self._gizmos = gizmos
+
+
+		def gizmos(self) -> Iterator[str]:
+			"""
+			Lists gizmos produced by self.
+
+			Returns:
+				Iterator[str]: An iterator over the gizmos.
+			"""
+			yield from self._gizmos
+
+
+	def _actualize_tool(self, fn: Callable, **kwargs):
+		return super()._actualize_tool(fn, gizmos=self._gizmos, **kwargs)
+
+
+
+class AutoToolDecorator(MIMOToolDecorator):
 	"""
 	The AutoToolDecorator class is a subclass of ToolDecorator. It overrides the _ToolCraft attribute of the parent class
 	with AutoToolCraft. This means that when a tool is actualized, an instance of AutoToolCraft will be created instead
 	of ToolCraft.
 
 	Attributes:
 		_ToolCraft (AutoToolCraft): A nested class that inherits from AutoToolCraft.
@@ -222,7 +245,10 @@
 	_ToolCraft = AutoToolCraft
 
 
 
 
 
 
+
+
+
```

### Comparing `omniply-0.2.1/omniply/core/top.py` & `omniply-0.3/omniply/core/op.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,160 +1,169 @@
-from .abstract import AbstractGadget, AbstractGaggle, AbstractGig, AbstractGang
-from .errors import GadgetFailure, MissingGadget
-from .tools import ToolCraft, AutoToolCraft, ToolDecorator, AutoToolDecorator
-from .gizmos import DashGizmo
-from .gaggles import MutableGaggle, LoopyGaggle, CraftyGaggle
-from .gigs import CacheGig, GroupCache
-from .groups import GroupBase, CachableGroup, SelectiveGroup
-
-
-
-class tool(AutoToolDecorator):
-	"""
-	The tool class is a subclass of AutoToolDecorator. It provides a convenient way to create tool instances
-	with automatic function gadget capabilities. It does not specify a gizmo type, meaning it can handle any type of gizmo.
-
-	Attributes:
-		_gizmo_type (None): The type of the gizmo. Defaults to None.
-	"""
-
-	# _gizmo_type = DashGizmo
-
-	class from_context(ToolDecorator):
-		"""
-		The from_context class is a nested class within tool that inherits from ToolDecorator. It provides a way to create
-		tool instances that handle DashGizmo types specifically. This is useful when the gizmos being handled contain dashes.
-
-		Attributes:
-			_gizmo_type (DashGizmo): The type of the gizmo. Defaults to DashGizmo.
-		"""
-		# _gizmo_type = DashGizmo
-		pass
-
-
-class ToolKit(LoopyGaggle, MutableGaggle, CraftyGaggle):
-	"""
-	The ToolKit class is a subclass of LoopyGaggle, MutableGaggle, and CraftyGaggle. It provides methods to handle
-	tools in a kit.
-
-	Methods:
-		__init__(self, *args, **kwargs): Initializes a new instance of the ToolKit class.
-	"""
-
-	def __init__(self, *args, **kwargs):
-		"""
-		Initializes a new instance of the ToolKit class.
-
-		This method initializes the superclass with the provided arguments and processes the crafts in the tool kit.
-
-		Args:
-			args: Variable length argument list.
-			kwargs: Arbitrary keyword arguments.
-		"""
-		super().__init__(*args, **kwargs)
-		self._process_crafts()
-
-
-class Context(GroupCache, LoopyGaggle, MutableGaggle, AbstractGig):
-	"""
-	The Context class is a subclass of GroupCache, LoopyGaggle, MutableGaggle, and AbstractGig. It provides methods to handle
-	gadgets in a context.
-
-	Methods:
-		__init__(self, *gadgets: AbstractGadget, **kwargs): Initializes a new instance of the Context class.
-		__getitem__(self, item): Returns the grabbed item from the context.
-	"""
-
-	# _gizmo_type = DashGizmo # TODO
-
-	def __init__(self, *gadgets: AbstractGadget, **kwargs):
-		"""
-		Initializes a new instance of the Context class.
-
-		This method initializes the superclass with the provided arguments and includes the provided gadgets in the context.
-
-		Args:
-			gadgets (AbstractGadget): The gadgets to be included in the context.
-			kwargs: Arbitrary keyword arguments.
-		"""
-		super().__init__(**kwargs)
-		self.include(*gadgets)
-
-	def __getitem__(self, item):
-		"""
-		Returns the grabbed item from the context.
-
-		Args:
-			item: The item to be grabbed from the context.
-
-		Returns:
-			Any: The grabbed item from the context.
-		"""
-		return self.grab(item)
-
-
-class Scope(CachableGroup, LoopyGaggle, MutableGaggle, AbstractGang):
-	"""
-	The Scope class is a subclass of CachableGroup, LoopyGaggle, MutableGaggle, and AbstractGang. It provides methods
-	to handle gadgets in a scope.
-
-	Methods:
-		__init__(self, *gadgets: AbstractGadget, **kwargs): Initializes a new instance of the Scope class.
-	"""
-
-	def __init__(self, *gadgets: AbstractGadget, **kwargs):
-		"""
-		Initializes a new instance of the Scope class.
-
-		This method initializes the superclass with the provided arguments and includes the provided gadgets in the scope.
-
-		Args:
-			gadgets (AbstractGadget): The gadgets to be included in the scope.
-			kwargs: Arbitrary keyword arguments.
-		"""
-		super().__init__(**kwargs)
-		self.include(*gadgets)
-
-	def __getitem__(self, item):
-		"""
-		Returns the grabbed item from the context.
-
-		Args:
-			item: The item to be grabbed from the context.
-
-		Returns:
-			Any: The grabbed item from the context.
-		"""
-		return self.grab(item)
-
-class Selection(SelectiveGroup, Scope):
-	"""
-	The Selection class is a subclass of SelectiveGroup and Scope. It provides methods to handle selective gizmo mapping
-	within a scope.
-
-	Methods:
-		__init__(self, *gadgets: AbstractGadget, **kwargs): Initializes a new instance of the Selection class.
-	"""
-
-	def __init__(self, *gadgets: AbstractGadget, **kwargs):
-		"""
-		Initializes a new instance of the Selection class.
-
-		This method initializes the superclass with the provided arguments and includes the provided gadgets in the selection.
-
-		Args:
-			gadgets (AbstractGadget): The gadgets to be included in the selection.
-			kwargs: Arbitrary keyword arguments.
-		"""
-		super().__init__(*gadgets, **kwargs)
-
-	def __getitem__(self, item):
-		"""
-		Returns the grabbed item from the context.
-
-		Args:
-			item: The item to be grabbed from the context.
-
-		Returns:
-			Any: The grabbed item from the context.
-		"""
+from typing import Iterable, Callable
+from .abstract import AbstractGadget, AbstractGaggle, AbstractGig, AbstractGang
+from .errors import GadgetFailure, MissingGadget
+from .tools import ToolCraftBase, AutoToolCraft, MIMOToolDecorator, AutoToolDecorator
+from .gizmos import DashGizmo
+from .gaggles import MutableGaggle, LoopyGaggle, CraftyGaggle
+from .gigs import CacheGig, GroupCache, TraceGig, RollingGig, ConsistentGig
+from .gangs import GroupBase, CachableGroup, SelectiveGroup
+from .genetics import GeneticGaggle
+
+
+
+class tool(AutoToolDecorator):
+	"""
+	The tool class is a subclass of AutoToolDecorator. It provides a convenient way to create tool instances
+	with automatic function gadget capabilities. It does not specify a gizmo type, meaning it can handle any type of gizmo.
+
+	Attributes:
+		_gizmo_type (None): The type of the gizmo. Defaults to None.
+	"""
+
+	# _gizmo_type = DashGizmo
+
+	class from_context(MIMOToolDecorator):
+		"""
+		The from_context class is a nested class within tool that inherits from ToolDecorator. It provides a way to create
+		tool instances that handle DashGizmo types specifically. This is useful when the gizmos being handled contain dashes.
+
+		Attributes:
+			_gizmo_type (DashGizmo): The type of the gizmo. Defaults to DashGizmo.
+		"""
+		# _gizmo_type = DashGizmo
+		def __init__(self, *args, parents: Iterable[str] = None, **kwargs):
+			super().__init__(*args, **kwargs)
+			self._parents = parents
+
+
+		def _actualize_tool(self, fn: Callable, **kwargs):
+			return super()._actualize_tool(fn, parents=self._parents, **kwargs)
+
+
+
+class ToolKit(LoopyGaggle, MutableGaggle, CraftyGaggle, GeneticGaggle):
+	"""
+	The ToolKit class is a subclass of LoopyGaggle, MutableGaggle, and CraftyGaggle. It provides methods to handle
+	tools in a kit.
+
+	Methods:
+		__init__(self, *args, **kwargs): Initializes a new instance of the ToolKit class.
+	"""
+
+	def __init__(self, *args, **kwargs):
+		"""
+		Initializes a new instance of the ToolKit class.
+
+		This method initializes the superclass with the provided arguments and processes the crafts in the tool kit.
+
+		Args:
+			args: Variable length argument list.
+			kwargs: Arbitrary keyword arguments.
+		"""
+		super().__init__(*args, **kwargs)
+		self._process_crafts()
+
+
+class Context(GroupCache, ConsistentGig, RollingGig, LoopyGaggle, MutableGaggle, GeneticGaggle, AbstractGig):
+	"""
+	The Context class is a subclass of GroupCache, LoopyGaggle, MutableGaggle, and AbstractGig. It provides methods to handle
+	gadgets in a context.
+
+	Methods:
+		__init__(self, *gadgets: AbstractGadget, **kwargs): Initializes a new instance of the Context class.
+		__getitem__(self, item): Returns the grabbed item from the context.
+	"""
+
+	# _gizmo_type = DashGizmo # TODO
+
+	def __init__(self, *gadgets: AbstractGadget, **kwargs):
+		"""
+		Initializes a new instance of the Context class.
+
+		This method initializes the superclass with the provided arguments and includes the provided gadgets in the context.
+
+		Args:
+			gadgets (AbstractGadget): The gadgets to be included in the context.
+			kwargs: Arbitrary keyword arguments.
+		"""
+		super().__init__(**kwargs)
+		self.include(*gadgets)
+
+	def __getitem__(self, item):
+		"""
+		Returns the grabbed item from the context.
+
+		Args:
+			item: The item to be grabbed from the context.
+
+		Returns:
+			Any: The grabbed item from the context.
+		"""
+		return self.grab(item)
+
+
+class Scope(CachableGroup, LoopyGaggle, MutableGaggle, AbstractGang):
+	"""
+	The Scope class is a subclass of CachableGroup, LoopyGaggle, MutableGaggle, and AbstractGang. It provides methods
+	to handle gadgets in a scope.
+
+	Methods:
+		__init__(self, *gadgets: AbstractGadget, **kwargs): Initializes a new instance of the Scope class.
+	"""
+
+	def __init__(self, *gadgets: AbstractGadget, **kwargs):
+		"""
+		Initializes a new instance of the Scope class.
+
+		This method initializes the superclass with the provided arguments and includes the provided gadgets in the scope.
+
+		Args:
+			gadgets (AbstractGadget): The gadgets to be included in the scope.
+			kwargs: Arbitrary keyword arguments.
+		"""
+		super().__init__(**kwargs)
+		self.include(*gadgets)
+
+	def __getitem__(self, item):
+		"""
+		Returns the grabbed item from the context.
+
+		Args:
+			item: The item to be grabbed from the context.
+
+		Returns:
+			Any: The grabbed item from the context.
+		"""
+		return self.grab(item)
+
+class Selection(SelectiveGroup, Scope):
+	"""
+	The Selection class is a subclass of SelectiveGroup and Scope. It provides methods to handle selective gizmo mapping
+	within a scope.
+
+	Methods:
+		__init__(self, *gadgets: AbstractGadget, **kwargs): Initializes a new instance of the Selection class.
+	"""
+
+	def __init__(self, *gadgets: AbstractGadget, **kwargs):
+		"""
+		Initializes a new instance of the Selection class.
+
+		This method initializes the superclass with the provided arguments and includes the provided gadgets in the selection.
+
+		Args:
+			gadgets (AbstractGadget): The gadgets to be included in the selection.
+			kwargs: Arbitrary keyword arguments.
+		"""
+		super().__init__(*gadgets, **kwargs)
+
+	def __getitem__(self, item):
+		"""
+		Returns the grabbed item from the context.
+
+		Args:
+			item: The item to be grabbed from the context.
+
+		Returns:
+			Any: The grabbed item from the context.
+		"""
 		return self.grab(item)
```

### Comparing `omniply-0.2.1/omniply/core/unit_test.py` & `omniply-0.3/omniply/core/unit_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from .top import tool, ToolKit, Context, Scope, Selection
+from .op import tool, ToolKit, Context, Scope, Selection
 
 
 def test_tool():
 	"""
 	This function tests the functionality of the 'tool' decorator and the 'gizmos' method.
 
 	The 'tool' decorator is used to define two functions, 'f' and 'g', with 'a' and 'b' as their respective gizmos.
@@ -411,14 +411,15 @@
 
 		Returns:
 			int: The input integer incremented by 10.
 		"""
 		return b + 10
 
 
+
 def test_nested_tools():
 	"""
 	This function tests the functionality of the '_Kit3' class and the 'Context' class.
 
 	The '_Kit3' class is instantiated and a context is created with the '_Kit3' instance as its tool kit.
 	The function asserts that the gizmos of the '_Kit3' instance are correctly identified and that the context correctly maps 'x' to 'y', 'z', 'w', and 'x'.
 	"""
@@ -553,16 +554,16 @@
 	assert counter == 1  # Asserts that the counter is correctly incremented.
 	assert 'a' in ctx.data  # Asserts that 'a' is in the context's data.
 	assert ctx['a'] == 1  # Asserts that the context correctly maps 'a' to 1.
 	assert counter == 1  # Asserts that the counter is not incremented.
 
 	ctx = Context(Scope(f, gap={'a': 'b'}))  # The 'Scope' class is used to create a scope with the function 'f' and a gizmo mapping from 'a' to 'b'.
 
-	assert not ctx.grabable('a')  # Asserts that 'a' is not grabable from the context.
-	assert ctx.grabable('b')  # Asserts that 'b' is grabable from the context.
+	assert not ctx.gives('a')  # Asserts that 'a' is not grabable from the context.
+	assert ctx.gives('b')  # Asserts that 'b' is grabable from the context.
 	assert ctx['b'] == 1  # Asserts that the context correctly maps 'b' to 1.
 	assert counter == 2  # Asserts that the counter is correctly incremented.
 	assert 'b' in ctx.data  # Asserts that 'b' is in the context's data.
 	assert ctx['b'] == 1  # Asserts that the context correctly maps 'b' to 1.
 	assert counter == 2  # Asserts that the counter is not incremented.
 
 	ctx.clear_cache()  # The context's cache is cleared.
@@ -630,11 +631,175 @@
 
 	ctx['a'] = 2  # The context maps 'a' to 2.
 	assert ctx['x'] == 20  # Asserts that the context correctly maps 'x' to 20.
 	assert counter == 7  # Asserts that the counter is not incremented.
 
 
 
+def test_simple_mimo():
+
+	_fuel = 1
+
+	@tool('x', 'y')
+	def f(a, b):
+		nonlocal _fuel
+		if _fuel == 0:
+			raise Exception('No fuel')
+		_fuel -= 1
+		return a + b, a * b
+
+	ctx = Context(f)
+	ctx['a'] = 2
+	ctx['b'] = 3
+
+	assert ctx['x'] == 5
+	assert ctx.is_cached('x')
+	assert not ctx.is_cached('y')
+	assert ctx['y'] == 6
+	assert ctx.is_cached('x')
+	assert ctx.is_cached('y')
+	assert ctx['x'] == 5
+
+
+	@tool('x', 'y')
+	def g(a):
+		return {'x': a + 1, 'y': a + 2}
+
+	@tool('a')
+	def h():
+		return 1
+
+	ctx = Context(g, h)
+
+	assert ctx['x'] == 2
+	assert ctx.is_cached('x')
+	assert not ctx.is_cached('y')
+	assert ctx['y'] == 3
+	assert ctx.is_cached('x')
+	assert ctx.is_cached('y')
+
+
+def test_simple_purge():
+
+	@tool('x')
+	def g(a):
+		return a + 1
+
+	@tool('a')
+	def h():
+		return 1
+
+	ctx = Context(g, h)
+
+	assert ctx['x'] == 2
+	assert ctx.is_cached('a') and ctx.is_cached('x')
+	ctx.purge('a')
+	assert not ctx.is_cached('a') and not ctx.is_cached('x')
+
+	assert ctx['x'] == 2
+	assert ctx.is_cached('a') and ctx.is_cached('x')
+	ctx['a'] = 10
+	assert ctx.is_cached('a') and not ctx.is_cached('x')
+	assert ctx['x'] == 11
+	assert ctx.is_cached('x')
+
+	# mimo
+
+	@tool('x', 'y')
+	def f(a):
+		return a + 1, a + 2
+
+	ctx = Context(f, h)
+
+	assert ctx['x'] == 2
+	assert ctx.is_cached('a') and ctx.is_cached('x') and not ctx.is_cached('y')
+
+	ctx['a'] = 10
+	assert ctx.is_cached('a') and not ctx.is_cached('x') and not ctx.is_cached('y')
+	assert ctx['y'] == 12
+	assert ctx.is_cached('a') and not ctx.is_cached('x') and ctx.is_cached('y')
+
+
+
+def test_genetics():
+	kit = _Kit3()
+
+	genome = next(kit.genes('a'))
+
+	assert genome.name == 'a'
+	assert genome.parents == ()
+	assert genome.siblings is None
+
+	genomes = list(kit.genes('c'))
+
+	assert len(genomes) == 2
+	assert genomes[1].name == 'c'
+	assert genomes[1].parents == ('b',)
+	assert genomes[1].siblings is None
+
+	genome = next(kit.genes('d'))
+
+	assert genome.name == 'd'
+	assert genome.parents == ('b',)
+	assert genome.siblings is None
+
+
+	@tool('x', 'y')
+	def f(a):
+		return a + 1, a + 2
+
+	genome = next(f.genes('x'))
+
+	assert genome.name == 'x'
+	assert genome.parents == ('a',)
+	assert genome.siblings == (None, 'y')
+
+	genome = next(f.genes('y'))
+
+	assert genome.name == 'y'
+	assert genome.parents == ('a',)
+	assert genome.siblings == ('x', None)
+	assert genome.endpoint == f._fn
+	assert genome.source == f
+
+
+
+def test_parents():
+	class MyKit(ToolKit):
+		@tool.from_context('a', 'b')
+		def f(self, ctx):
+			return ctx['x'] * ctx['y'], ctx['y']
+		@f.parents
+		def _f_parents(self):
+			return 'x', 'y'
+
+	kit = MyKit()
+
+	genome = next(kit.genes('a'))
+
+	assert genome.name == 'a'
+	assert genome.parents == ('x', 'y')
+	assert genome.siblings == (None, 'b')
+
+	ctx = Context(kit)
+
+	ctx['x'] = 10
+	ctx['y'] = 20
+
+	assert ctx['a'] == 200
+	assert not ctx.is_cached('b')
+	assert ctx['b'] == 20
+
+
+
+
+
+
+
+
+
+
+
```

### Comparing `omniply-0.2.1/omniply.egg-info/PKG-INFO` & `omniply-0.3/omniply.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: omniply
-Version: 0.2.1
+Version: 0.3
 Summary: "Omni-ply Versatile Data Management for Rapid AI Prototyping and Research"
 Author: Felix Leeb
 License: MIT
-Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 # omni-ply
 
 > Before your code complexity multiplies, use omniply.
```

