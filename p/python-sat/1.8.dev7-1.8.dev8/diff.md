# Comparing `tmp/python-sat-1.8.dev7.tar.gz` & `tmp/python-sat-1.8.dev8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-sat-1.8.dev7.tar", last modified: Sun Mar 31 04:52:51 2024, max compression
+gzip compressed data, was "python-sat-1.8.dev8.tar", last modified: Sat Apr  6 03:31:03 2024, max compression
```

## Comparing `python-sat-1.8.dev7.tar` & `python-sat-1.8.dev8.tar`

### file list

```diff
@@ -1,103 +1,103 @@
-drwxr-xr-x   0 aign0002 (892519254) 907548567        0 2024-03-31 04:52:51.601193 python-sat-1.8.dev7/
--rw-r--r--   0 aign0002 (892519254) 907548567     1109 2023-01-13 10:53:42.000000 python-sat-1.8.dev7/LICENSE.txt
--rw-r--r--   0 aign0002 (892519254) 907548567      217 2023-01-13 10:53:42.000000 python-sat-1.8.dev7/MANIFEST.in
--rw-r--r--   0 aign0002 (892519254) 907548567     1523 2024-03-31 04:52:51.601090 python-sat-1.8.dev7/PKG-INFO
--rw-r--r--   0 aign0002 (892519254) 907548567    14570 2024-03-16 05:05:09.000000 python-sat-1.8.dev7/README.rst
-drwxr-xr-x   0 aign0002 (892519254) 907548567        0 2024-03-31 04:52:51.563666 python-sat-1.8.dev7/allies/
--rw-------   0 aign0002 (892519254) 907548567        0 2023-04-14 00:41:27.000000 python-sat-1.8.dev7/allies/__init__.py
--rwxr-xr-x   0 aign0002 (892519254) 907548567    13551 2023-11-24 02:09:08.000000 python-sat-1.8.dev7/allies/approxmc.py
--rwxr-xr-x   0 aign0002 (892519254) 907548567    16698 2023-11-24 05:11:48.000000 python-sat-1.8.dev7/allies/unigen.py
-drwxr-xr-x   0 aign0002 (892519254) 907548567        0 2024-03-31 04:52:51.567145 python-sat-1.8.dev7/cardenc/
--rw-r--r--   0 aign0002 (892519254) 907548567     1375 2023-01-13 10:53:42.000000 python-sat-1.8.dev7/cardenc/bitwise.hh
--rw-r--r--   0 aign0002 (892519254) 907548567     2468 2023-03-02 05:23:11.000000 python-sat-1.8.dev7/cardenc/card.hh
--rw-r--r--   0 aign0002 (892519254) 907548567     1874 2023-01-13 10:53:42.000000 python-sat-1.8.dev7/cardenc/clset.hh
--rw-r--r--   0 aign0002 (892519254) 907548567     1303 2023-01-13 10:53:42.000000 python-sat-1.8.dev7/cardenc/common.hh
--rw-r--r--   0 aign0002 (892519254) 907548567     4646 2023-01-13 10:53:42.000000 python-sat-1.8.dev7/cardenc/itot.hh
--rw-r--r--   0 aign0002 (892519254) 907548567     2325 2023-01-13 10:53:42.000000 python-sat-1.8.dev7/cardenc/ladder.hh
--rw-r--r--   0 aign0002 (892519254) 907548567    11355 2023-01-13 10:53:42.000000 python-sat-1.8.dev7/cardenc/mto.hh
--rw-r--r--   0 aign0002 (892519254) 907548567     1008 2023-01-13 10:53:42.000000 python-sat-1.8.dev7/cardenc/pairwise.hh
--rw-r--r--   0 aign0002 (892519254) 907548567      918 2023-01-13 10:53:42.000000 python-sat-1.8.dev7/cardenc/ptypes.hh
--rw-r--r--   0 aign0002 (892519254) 907548567    15865 2023-01-13 10:53:42.000000 python-sat-1.8.dev7/cardenc/pycard.cc
--rw-r--r--   0 aign0002 (892519254) 907548567     4851 2023-01-13 10:53:42.000000 python-sat-1.8.dev7/cardenc/seqcounter.hh
--rw-r--r--   0 aign0002 (892519254) 907548567     8355 2023-01-13 10:53:42.000000 python-sat-1.8.dev7/cardenc/sortcard.hh
--rw-r--r--   0 aign0002 (892519254) 907548567     5117 2023-01-13 10:53:42.000000 python-sat-1.8.dev7/cardenc/utils.hh
-drwxr-xr-x   0 aign0002 (892519254) 907548567        0 2024-03-31 04:52:51.569637 python-sat-1.8.dev7/examples/
--rw-------   0 aign0002 (892519254) 907548567        0 2023-01-13 10:53:42.000000 python-sat-1.8.dev7/examples/__init__.py
--rwxr-xr-x   0 aign0002 (892519254) 907548567    17968 2023-01-13 10:53:42.000000 python-sat-1.8.dev7/examples/fm.py
--rwxr-xr-x   0 aign0002 (892519254) 907548567    18986 2024-02-23 12:49:50.000000 python-sat-1.8.dev7/examples/genhard.py
--rwxr-xr-x   0 aign0002 (892519254) 907548567    25406 2023-06-04 07:07:20.000000 python-sat-1.8.dev7/examples/hitman.py
--rwxr-xr-x   0 aign0002 (892519254) 907548567    21295 2023-01-13 10:53:42.000000 python-sat-1.8.dev7/examples/lbx.py
--rwxr-xr-x   0 aign0002 (892519254) 907548567    15523 2023-01-20 20:56:31.000000 python-sat-1.8.dev7/examples/lsu.py
--rwxr-xr-x   0 aign0002 (892519254) 907548567    20320 2023-01-13 10:53:42.000000 python-sat-1.8.dev7/examples/mcsls.py
--rwxr-xr-x   0 aign0002 (892519254) 907548567     5704 2023-11-17 01:15:24.000000 python-sat-1.8.dev7/examples/models.py
--rwxr-xr-x   0 aign0002 (892519254) 907548567    10563 2024-03-12 23:08:45.000000 python-sat-1.8.dev7/examples/musx.py
--rwxr-xr-x   0 aign0002 (892519254) 907548567    25636 2023-06-04 07:39:47.000000 python-sat-1.8.dev7/examples/optux.py
--rwxr-xr-x   0 aign0002 (892519254) 907548567    67270 2023-06-09 06:00:18.000000 python-sat-1.8.dev7/examples/rc2.py
--rwxr-xr-x   0 aign0002 (892519254) 907548567     2183 2023-01-13 10:53:42.000000 python-sat-1.8.dev7/examples/usage.py
-drwxr-xr-x   0 aign0002 (892519254) 907548567        0 2024-03-31 04:52:51.573071 python-sat-1.8.dev7/pysat/
--rw-r--r--   0 aign0002 (892519254) 907548567      669 2024-03-31 04:48:54.000000 python-sat-1.8.dev7/pysat/__init__.py
--rw-r--r--   0 aign0002 (892519254) 907548567     5814 2023-01-13 10:53:42.000000 python-sat-1.8.dev7/pysat/_fileio.py
--rw-r--r--   0 aign0002 (892519254) 907548567     1340 2023-01-13 10:53:42.000000 python-sat-1.8.dev7/pysat/_utils.py
--rw-r--r--   0 aign0002 (892519254) 907548567    30043 2023-01-13 10:53:42.000000 python-sat-1.8.dev7/pysat/card.py
--rw-r--r--   0 aign0002 (892519254) 907548567    45094 2024-03-18 05:43:24.000000 python-sat-1.8.dev7/pysat/engines.py
--rw-r--r--   0 aign0002 (892519254) 907548567   192658 2024-03-31 04:44:45.000000 python-sat-1.8.dev7/pysat/formula.py
--rw-r--r--   0 aign0002 (892519254) 907548567    16649 2024-03-16 04:25:34.000000 python-sat-1.8.dev7/pysat/pb.py
--rw-r--r--   0 aign0002 (892519254) 907548567    11968 2023-03-05 06:22:14.000000 python-sat-1.8.dev7/pysat/process.py
--rw-r--r--   0 aign0002 (892519254) 907548567   226003 2024-03-18 05:36:00.000000 python-sat-1.8.dev7/pysat/solvers.py
-drwxr-xr-x   0 aign0002 (892519254) 907548567        0 2024-03-31 04:52:51.600343 python-sat-1.8.dev7/python_sat.egg-info/
--rw-r--r--   0 aign0002 (892519254) 907548567     1523 2024-03-31 04:52:51.000000 python-sat-1.8.dev7/python_sat.egg-info/PKG-INFO
--rw-r--r--   0 aign0002 (892519254) 907548567     2090 2024-03-31 04:52:51.000000 python-sat-1.8.dev7/python_sat.egg-info/SOURCES.txt
--rw-r--r--   0 aign0002 (892519254) 907548567        1 2024-03-31 04:52:51.000000 python-sat-1.8.dev7/python_sat.egg-info/dependency_links.txt
--rw-r--r--   0 aign0002 (892519254) 907548567      148 2024-03-31 04:52:51.000000 python-sat-1.8.dev7/python_sat.egg-info/requires.txt
--rw-r--r--   0 aign0002 (892519254) 907548567       23 2024-03-31 04:52:51.000000 python-sat-1.8.dev7/python_sat.egg-info/top_level.txt
--rw-r--r--   0 aign0002 (892519254) 907548567       39 2023-01-13 10:53:42.000000 python-sat-1.8.dev7/requirements.txt
--rw-r--r--   0 aign0002 (892519254) 907548567      108 2024-03-31 04:52:51.601453 python-sat-1.8.dev7/setup.cfg
--rw-r--r--   0 aign0002 (892519254) 907548567     6664 2024-03-27 04:48:33.000000 python-sat-1.8.dev7/setup.py
-drwxr-xr-x   0 aign0002 (892519254) 907548567        0 2024-03-31 04:52:51.587108 python-sat-1.8.dev7/solvers/
--rw-r--r--   0 aign0002 (892519254) 907548567   547031 2023-03-02 05:10:30.000000 python-sat-1.8.dev7/solvers/cadical103.tar.gz
--rw-r--r--   0 aign0002 (892519254) 907548567   596433 2023-03-03 10:16:48.000000 python-sat-1.8.dev7/solvers/cadical153.tar.gz
--rw-r--r--   0 aign0002 (892519254) 907548567   644206 2023-08-25 01:25:36.000000 python-sat-1.8.dev7/solvers/cadical170.tar.gz
--rw-r--r--   0 aign0002 (892519254) 907548567   691268 2024-03-16 04:33:34.000000 python-sat-1.8.dev7/solvers/cadical195.tar.gz
--rw-r--r--   0 aign0002 (892519254) 907548567    50813 2023-01-13 10:53:42.000000 python-sat-1.8.dev7/solvers/glucose30.tar.gz
--rw-r--r--   0 aign0002 (892519254) 907548567    82779 2023-01-13 10:53:42.000000 python-sat-1.8.dev7/solvers/glucose41.tar.gz
--rw-r--r--   0 aign0002 (892519254) 907548567    88105 2023-07-11 23:37:13.000000 python-sat-1.8.dev7/solvers/glucose421.tar.gz
--rw-r--r--   0 aign0002 (892519254) 907548567   501731 2023-01-13 10:53:42.000000 python-sat-1.8.dev7/solvers/lingeling.tar.gz
--rw-r--r--   0 aign0002 (892519254) 907548567    82656 2023-01-13 10:53:42.000000 python-sat-1.8.dev7/solvers/maplechrono.zip
--rw-r--r--   0 aign0002 (892519254) 907548567    94949 2023-01-13 10:53:42.000000 python-sat-1.8.dev7/solvers/maplecm.zip
--rw-r--r--   0 aign0002 (892519254) 907548567    77088 2023-01-13 10:53:42.000000 python-sat-1.8.dev7/solvers/maplesat.zip
--rw-r--r--   0 aign0002 (892519254) 907548567   179223 2023-01-13 10:53:42.000000 python-sat-1.8.dev7/solvers/mergesat3.tar.gz
--rw-r--r--   0 aign0002 (892519254) 907548567  1529188 2023-01-13 10:53:42.000000 python-sat-1.8.dev7/solvers/minicard.tar.gz
--rw-r--r--   0 aign0002 (892519254) 907548567    43879 2023-01-13 10:53:42.000000 python-sat-1.8.dev7/solvers/minisat22.tar.gz
--rw-r--r--   0 aign0002 (892519254) 907548567    75209 2023-01-13 10:53:42.000000 python-sat-1.8.dev7/solvers/minisatgh.zip
-drwxr-xr-x   0 aign0002 (892519254) 907548567        0 2024-03-31 04:52:51.597665 python-sat-1.8.dev7/solvers/patches/
--rw-r--r--   0 aign0002 (892519254) 907548567    51588 2023-03-02 05:15:52.000000 python-sat-1.8.dev7/solvers/patches/cadical103.patch
--rw-r--r--   0 aign0002 (892519254) 907548567    69395 2024-03-17 07:15:43.000000 python-sat-1.8.dev7/solvers/patches/cadical153.patch
--rw-r--r--   0 aign0002 (892519254) 907548567    92210 2024-03-17 07:14:50.000000 python-sat-1.8.dev7/solvers/patches/cadical195.patch
--rw-r--r--   0 aign0002 (892519254) 907548567    93207 2023-01-13 10:53:42.000000 python-sat-1.8.dev7/solvers/patches/glucose30.patch
--rw-r--r--   0 aign0002 (892519254) 907548567    89206 2023-01-13 10:53:42.000000 python-sat-1.8.dev7/solvers/patches/glucose41.patch
--rw-r--r--   0 aign0002 (892519254) 907548567    68942 2023-07-15 01:30:10.000000 python-sat-1.8.dev7/solvers/patches/glucose421.patch
--rw-r--r--   0 aign0002 (892519254) 907548567   117955 2023-01-13 10:53:42.000000 python-sat-1.8.dev7/solvers/patches/gluecard30.patch
--rw-r--r--   0 aign0002 (892519254) 907548567   137342 2023-01-13 10:53:42.000000 python-sat-1.8.dev7/solvers/patches/gluecard41.patch
--rw-r--r--   0 aign0002 (892519254) 907548567    54848 2023-01-13 10:53:42.000000 python-sat-1.8.dev7/solvers/patches/lingeling.patch
--rw-r--r--   0 aign0002 (892519254) 907548567    90618 2023-01-14 22:24:35.000000 python-sat-1.8.dev7/solvers/patches/maplechrono.patch
--rw-r--r--   0 aign0002 (892519254) 907548567   114715 2023-01-14 21:29:08.000000 python-sat-1.8.dev7/solvers/patches/maplecm.patch
--rw-r--r--   0 aign0002 (892519254) 907548567    82379 2023-01-13 10:53:42.000000 python-sat-1.8.dev7/solvers/patches/maplesat.patch
--rw-r--r--   0 aign0002 (892519254) 907548567    88893 2023-01-14 22:24:31.000000 python-sat-1.8.dev7/solvers/patches/mergesat3.patch
--rw-r--r--   0 aign0002 (892519254) 907548567    51757 2023-01-13 10:53:42.000000 python-sat-1.8.dev7/solvers/patches/minicard.patch
--rw-r--r--   0 aign0002 (892519254) 907548567    42627 2023-01-13 10:53:42.000000 python-sat-1.8.dev7/solvers/patches/minisat22.patch
--rw-r--r--   0 aign0002 (892519254) 907548567    60626 2023-01-13 10:53:42.000000 python-sat-1.8.dev7/solvers/patches/minisatgh.patch
--rw-r--r--   0 aign0002 (892519254) 907548567    32315 2024-03-17 07:15:51.000000 python-sat-1.8.dev7/solvers/prepare.py
--rw-r--r--   0 aign0002 (892519254) 907548567   285751 2024-03-16 04:32:47.000000 python-sat-1.8.dev7/solvers/pysolvers.cc
-drwxr-xr-x   0 aign0002 (892519254) 907548567        0 2024-03-31 04:52:51.599682 python-sat-1.8.dev7/tests/
--rw-r--r--   0 aign0002 (892519254) 907548567      987 2023-07-12 00:04:49.000000 python-sat-1.8.dev7/tests/test_accum_stats.py
--rw-r--r--   0 aign0002 (892519254) 907548567      429 2023-01-13 10:53:42.000000 python-sat-1.8.dev7/tests/test_atmost.py
--rw-r--r--   0 aign0002 (892519254) 907548567      707 2023-01-13 10:53:42.000000 python-sat-1.8.dev7/tests/test_atmost1.py
--rw-r--r--   0 aign0002 (892519254) 907548567      998 2023-01-13 10:53:42.000000 python-sat-1.8.dev7/tests/test_atmostk.py
--rw-r--r--   0 aign0002 (892519254) 907548567     1299 2024-03-17 06:23:23.000000 python-sat-1.8.dev7/tests/test_boolengine.py
--rw-r--r--   0 aign0002 (892519254) 907548567     2432 2023-07-12 00:04:57.000000 python-sat-1.8.dev7/tests/test_cnfplus.py
--rw-r--r--   0 aign0002 (892519254) 907548567      784 2023-01-13 10:53:42.000000 python-sat-1.8.dev7/tests/test_equals1.py
--rw-r--r--   0 aign0002 (892519254) 907548567     1007 2023-03-05 06:31:37.000000 python-sat-1.8.dev7/tests/test_process.py
--rw-r--r--   0 aign0002 (892519254) 907548567     1260 2024-03-17 06:23:42.000000 python-sat-1.8.dev7/tests/test_propagate.py
--rw-r--r--   0 aign0002 (892519254) 907548567      890 2023-07-12 00:05:05.000000 python-sat-1.8.dev7/tests/test_unique_model.py
--rw-r--r--   0 aign0002 (892519254) 907548567      937 2023-01-13 10:53:42.000000 python-sat-1.8.dev7/tests/test_unique_mus.py
--rw-r--r--   0 aign0002 (892519254) 907548567      650 2023-07-12 00:05:10.000000 python-sat-1.8.dev7/tests/test_warmstart.py
+drwxr-xr-x   0 aign0002 (892519254) 907548567        0 2024-04-06 03:31:03.863770 python-sat-1.8.dev8/
+-rw-r--r--   0 aign0002 (892519254) 907548567     1109 2023-01-13 10:53:42.000000 python-sat-1.8.dev8/LICENSE.txt
+-rw-r--r--   0 aign0002 (892519254) 907548567      217 2023-01-13 10:53:42.000000 python-sat-1.8.dev8/MANIFEST.in
+-rw-r--r--   0 aign0002 (892519254) 907548567     1523 2024-04-06 03:31:03.863645 python-sat-1.8.dev8/PKG-INFO
+-rw-r--r--   0 aign0002 (892519254) 907548567    14570 2024-03-16 05:05:09.000000 python-sat-1.8.dev8/README.rst
+drwxr-xr-x   0 aign0002 (892519254) 907548567        0 2024-04-06 03:31:03.834119 python-sat-1.8.dev8/allies/
+-rw-------   0 aign0002 (892519254) 907548567        0 2023-04-14 00:41:27.000000 python-sat-1.8.dev8/allies/__init__.py
+-rwxr-xr-x   0 aign0002 (892519254) 907548567    13551 2023-11-24 02:09:08.000000 python-sat-1.8.dev8/allies/approxmc.py
+-rwxr-xr-x   0 aign0002 (892519254) 907548567    16698 2023-11-24 05:11:48.000000 python-sat-1.8.dev8/allies/unigen.py
+drwxr-xr-x   0 aign0002 (892519254) 907548567        0 2024-04-06 03:31:03.836878 python-sat-1.8.dev8/cardenc/
+-rw-r--r--   0 aign0002 (892519254) 907548567     1375 2023-01-13 10:53:42.000000 python-sat-1.8.dev8/cardenc/bitwise.hh
+-rw-r--r--   0 aign0002 (892519254) 907548567     2468 2023-03-02 05:23:11.000000 python-sat-1.8.dev8/cardenc/card.hh
+-rw-r--r--   0 aign0002 (892519254) 907548567     1874 2023-01-13 10:53:42.000000 python-sat-1.8.dev8/cardenc/clset.hh
+-rw-r--r--   0 aign0002 (892519254) 907548567     1303 2023-01-13 10:53:42.000000 python-sat-1.8.dev8/cardenc/common.hh
+-rw-r--r--   0 aign0002 (892519254) 907548567     4646 2023-01-13 10:53:42.000000 python-sat-1.8.dev8/cardenc/itot.hh
+-rw-r--r--   0 aign0002 (892519254) 907548567     2325 2023-01-13 10:53:42.000000 python-sat-1.8.dev8/cardenc/ladder.hh
+-rw-r--r--   0 aign0002 (892519254) 907548567    11355 2023-01-13 10:53:42.000000 python-sat-1.8.dev8/cardenc/mto.hh
+-rw-r--r--   0 aign0002 (892519254) 907548567     1008 2023-01-13 10:53:42.000000 python-sat-1.8.dev8/cardenc/pairwise.hh
+-rw-r--r--   0 aign0002 (892519254) 907548567      918 2023-01-13 10:53:42.000000 python-sat-1.8.dev8/cardenc/ptypes.hh
+-rw-r--r--   0 aign0002 (892519254) 907548567    15865 2023-01-13 10:53:42.000000 python-sat-1.8.dev8/cardenc/pycard.cc
+-rw-r--r--   0 aign0002 (892519254) 907548567     4851 2023-01-13 10:53:42.000000 python-sat-1.8.dev8/cardenc/seqcounter.hh
+-rw-r--r--   0 aign0002 (892519254) 907548567     8355 2023-01-13 10:53:42.000000 python-sat-1.8.dev8/cardenc/sortcard.hh
+-rw-r--r--   0 aign0002 (892519254) 907548567     5117 2023-01-13 10:53:42.000000 python-sat-1.8.dev8/cardenc/utils.hh
+drwxr-xr-x   0 aign0002 (892519254) 907548567        0 2024-04-06 03:31:03.839308 python-sat-1.8.dev8/examples/
+-rw-------   0 aign0002 (892519254) 907548567        0 2023-01-13 10:53:42.000000 python-sat-1.8.dev8/examples/__init__.py
+-rwxr-xr-x   0 aign0002 (892519254) 907548567    18174 2024-04-05 11:52:59.000000 python-sat-1.8.dev8/examples/fm.py
+-rwxr-xr-x   0 aign0002 (892519254) 907548567    18986 2024-02-23 12:49:50.000000 python-sat-1.8.dev8/examples/genhard.py
+-rwxr-xr-x   0 aign0002 (892519254) 907548567    25762 2024-04-05 10:59:25.000000 python-sat-1.8.dev8/examples/hitman.py
+-rwxr-xr-x   0 aign0002 (892519254) 907548567    21484 2024-04-05 11:52:23.000000 python-sat-1.8.dev8/examples/lbx.py
+-rwxr-xr-x   0 aign0002 (892519254) 907548567    16112 2024-04-05 12:04:10.000000 python-sat-1.8.dev8/examples/lsu.py
+-rwxr-xr-x   0 aign0002 (892519254) 907548567    20509 2024-04-05 11:53:17.000000 python-sat-1.8.dev8/examples/mcsls.py
+-rwxr-xr-x   0 aign0002 (892519254) 907548567     5741 2024-04-05 12:12:36.000000 python-sat-1.8.dev8/examples/models.py
+-rwxr-xr-x   0 aign0002 (892519254) 907548567    10747 2024-04-05 11:53:33.000000 python-sat-1.8.dev8/examples/musx.py
+-rwxr-xr-x   0 aign0002 (892519254) 907548567    25841 2024-04-05 11:50:00.000000 python-sat-1.8.dev8/examples/optux.py
+-rwxr-xr-x   0 aign0002 (892519254) 907548567    67511 2024-04-05 12:47:02.000000 python-sat-1.8.dev8/examples/rc2.py
+-rwxr-xr-x   0 aign0002 (892519254) 907548567     2183 2023-01-13 10:53:42.000000 python-sat-1.8.dev8/examples/usage.py
+drwxr-xr-x   0 aign0002 (892519254) 907548567        0 2024-04-06 03:31:03.841280 python-sat-1.8.dev8/pysat/
+-rw-r--r--   0 aign0002 (892519254) 907548567      669 2024-04-05 12:47:38.000000 python-sat-1.8.dev8/pysat/__init__.py
+-rw-r--r--   0 aign0002 (892519254) 907548567     5814 2023-01-13 10:53:42.000000 python-sat-1.8.dev8/pysat/_fileio.py
+-rw-r--r--   0 aign0002 (892519254) 907548567     1340 2023-01-13 10:53:42.000000 python-sat-1.8.dev8/pysat/_utils.py
+-rw-r--r--   0 aign0002 (892519254) 907548567    30043 2023-01-13 10:53:42.000000 python-sat-1.8.dev8/pysat/card.py
+-rw-r--r--   0 aign0002 (892519254) 907548567    45094 2024-03-18 05:43:24.000000 python-sat-1.8.dev8/pysat/engines.py
+-rw-r--r--   0 aign0002 (892519254) 907548567   192658 2024-03-31 04:44:45.000000 python-sat-1.8.dev8/pysat/formula.py
+-rw-r--r--   0 aign0002 (892519254) 907548567    16649 2024-03-16 04:25:34.000000 python-sat-1.8.dev8/pysat/pb.py
+-rw-r--r--   0 aign0002 (892519254) 907548567    11968 2023-03-05 06:22:14.000000 python-sat-1.8.dev8/pysat/process.py
+-rw-r--r--   0 aign0002 (892519254) 907548567   226003 2024-03-18 05:36:00.000000 python-sat-1.8.dev8/pysat/solvers.py
+drwxr-xr-x   0 aign0002 (892519254) 907548567        0 2024-04-06 03:31:03.862892 python-sat-1.8.dev8/python_sat.egg-info/
+-rw-r--r--   0 aign0002 (892519254) 907548567     1523 2024-04-06 03:31:03.000000 python-sat-1.8.dev8/python_sat.egg-info/PKG-INFO
+-rw-r--r--   0 aign0002 (892519254) 907548567     2090 2024-04-06 03:31:03.000000 python-sat-1.8.dev8/python_sat.egg-info/SOURCES.txt
+-rw-r--r--   0 aign0002 (892519254) 907548567        1 2024-04-06 03:31:03.000000 python-sat-1.8.dev8/python_sat.egg-info/dependency_links.txt
+-rw-r--r--   0 aign0002 (892519254) 907548567      148 2024-04-06 03:31:03.000000 python-sat-1.8.dev8/python_sat.egg-info/requires.txt
+-rw-r--r--   0 aign0002 (892519254) 907548567       23 2024-04-06 03:31:03.000000 python-sat-1.8.dev8/python_sat.egg-info/top_level.txt
+-rw-r--r--   0 aign0002 (892519254) 907548567       39 2023-01-13 10:53:42.000000 python-sat-1.8.dev8/requirements.txt
+-rw-r--r--   0 aign0002 (892519254) 907548567      108 2024-04-06 03:31:03.864042 python-sat-1.8.dev8/setup.cfg
+-rw-r--r--   0 aign0002 (892519254) 907548567     6664 2024-03-27 04:48:33.000000 python-sat-1.8.dev8/setup.py
+drwxr-xr-x   0 aign0002 (892519254) 907548567        0 2024-04-06 03:31:03.853219 python-sat-1.8.dev8/solvers/
+-rw-r--r--   0 aign0002 (892519254) 907548567   547031 2023-03-02 05:10:30.000000 python-sat-1.8.dev8/solvers/cadical103.tar.gz
+-rw-r--r--   0 aign0002 (892519254) 907548567   596433 2023-03-03 10:16:48.000000 python-sat-1.8.dev8/solvers/cadical153.tar.gz
+-rw-r--r--   0 aign0002 (892519254) 907548567   644206 2023-08-25 01:25:36.000000 python-sat-1.8.dev8/solvers/cadical170.tar.gz
+-rw-r--r--   0 aign0002 (892519254) 907548567   691268 2024-03-16 04:33:34.000000 python-sat-1.8.dev8/solvers/cadical195.tar.gz
+-rw-r--r--   0 aign0002 (892519254) 907548567    50813 2023-01-13 10:53:42.000000 python-sat-1.8.dev8/solvers/glucose30.tar.gz
+-rw-r--r--   0 aign0002 (892519254) 907548567    82779 2023-01-13 10:53:42.000000 python-sat-1.8.dev8/solvers/glucose41.tar.gz
+-rw-r--r--   0 aign0002 (892519254) 907548567    88105 2023-07-11 23:37:13.000000 python-sat-1.8.dev8/solvers/glucose421.tar.gz
+-rw-r--r--   0 aign0002 (892519254) 907548567   501731 2023-01-13 10:53:42.000000 python-sat-1.8.dev8/solvers/lingeling.tar.gz
+-rw-r--r--   0 aign0002 (892519254) 907548567    82656 2023-01-13 10:53:42.000000 python-sat-1.8.dev8/solvers/maplechrono.zip
+-rw-r--r--   0 aign0002 (892519254) 907548567    94949 2023-01-13 10:53:42.000000 python-sat-1.8.dev8/solvers/maplecm.zip
+-rw-r--r--   0 aign0002 (892519254) 907548567    77088 2023-01-13 10:53:42.000000 python-sat-1.8.dev8/solvers/maplesat.zip
+-rw-r--r--   0 aign0002 (892519254) 907548567   179223 2023-01-13 10:53:42.000000 python-sat-1.8.dev8/solvers/mergesat3.tar.gz
+-rw-r--r--   0 aign0002 (892519254) 907548567  1529188 2023-01-13 10:53:42.000000 python-sat-1.8.dev8/solvers/minicard.tar.gz
+-rw-r--r--   0 aign0002 (892519254) 907548567    43879 2023-01-13 10:53:42.000000 python-sat-1.8.dev8/solvers/minisat22.tar.gz
+-rw-r--r--   0 aign0002 (892519254) 907548567    75209 2023-01-13 10:53:42.000000 python-sat-1.8.dev8/solvers/minisatgh.zip
+drwxr-xr-x   0 aign0002 (892519254) 907548567        0 2024-04-06 03:31:03.857486 python-sat-1.8.dev8/solvers/patches/
+-rw-r--r--   0 aign0002 (892519254) 907548567    51588 2023-03-02 05:15:52.000000 python-sat-1.8.dev8/solvers/patches/cadical103.patch
+-rw-r--r--   0 aign0002 (892519254) 907548567    69395 2024-03-17 07:15:43.000000 python-sat-1.8.dev8/solvers/patches/cadical153.patch
+-rw-r--r--   0 aign0002 (892519254) 907548567    92210 2024-03-17 07:14:50.000000 python-sat-1.8.dev8/solvers/patches/cadical195.patch
+-rw-r--r--   0 aign0002 (892519254) 907548567    93207 2023-01-13 10:53:42.000000 python-sat-1.8.dev8/solvers/patches/glucose30.patch
+-rw-r--r--   0 aign0002 (892519254) 907548567    89206 2023-01-13 10:53:42.000000 python-sat-1.8.dev8/solvers/patches/glucose41.patch
+-rw-r--r--   0 aign0002 (892519254) 907548567    68942 2023-07-15 01:30:10.000000 python-sat-1.8.dev8/solvers/patches/glucose421.patch
+-rw-r--r--   0 aign0002 (892519254) 907548567   117955 2023-01-13 10:53:42.000000 python-sat-1.8.dev8/solvers/patches/gluecard30.patch
+-rw-r--r--   0 aign0002 (892519254) 907548567   137342 2023-01-13 10:53:42.000000 python-sat-1.8.dev8/solvers/patches/gluecard41.patch
+-rw-r--r--   0 aign0002 (892519254) 907548567    54848 2023-01-13 10:53:42.000000 python-sat-1.8.dev8/solvers/patches/lingeling.patch
+-rw-r--r--   0 aign0002 (892519254) 907548567    90618 2023-01-14 22:24:35.000000 python-sat-1.8.dev8/solvers/patches/maplechrono.patch
+-rw-r--r--   0 aign0002 (892519254) 907548567   114715 2023-01-14 21:29:08.000000 python-sat-1.8.dev8/solvers/patches/maplecm.patch
+-rw-r--r--   0 aign0002 (892519254) 907548567    82379 2023-01-13 10:53:42.000000 python-sat-1.8.dev8/solvers/patches/maplesat.patch
+-rw-r--r--   0 aign0002 (892519254) 907548567    88893 2023-01-14 22:24:31.000000 python-sat-1.8.dev8/solvers/patches/mergesat3.patch
+-rw-r--r--   0 aign0002 (892519254) 907548567    51757 2023-01-13 10:53:42.000000 python-sat-1.8.dev8/solvers/patches/minicard.patch
+-rw-r--r--   0 aign0002 (892519254) 907548567    42627 2023-01-13 10:53:42.000000 python-sat-1.8.dev8/solvers/patches/minisat22.patch
+-rw-r--r--   0 aign0002 (892519254) 907548567    60626 2023-01-13 10:53:42.000000 python-sat-1.8.dev8/solvers/patches/minisatgh.patch
+-rw-r--r--   0 aign0002 (892519254) 907548567    32315 2024-03-17 07:15:51.000000 python-sat-1.8.dev8/solvers/prepare.py
+-rw-r--r--   0 aign0002 (892519254) 907548567   285751 2024-03-16 04:32:47.000000 python-sat-1.8.dev8/solvers/pysolvers.cc
+drwxr-xr-x   0 aign0002 (892519254) 907548567        0 2024-04-06 03:31:03.862435 python-sat-1.8.dev8/tests/
+-rw-r--r--   0 aign0002 (892519254) 907548567      987 2023-07-12 00:04:49.000000 python-sat-1.8.dev8/tests/test_accum_stats.py
+-rw-r--r--   0 aign0002 (892519254) 907548567      429 2023-01-13 10:53:42.000000 python-sat-1.8.dev8/tests/test_atmost.py
+-rw-r--r--   0 aign0002 (892519254) 907548567      707 2023-01-13 10:53:42.000000 python-sat-1.8.dev8/tests/test_atmost1.py
+-rw-r--r--   0 aign0002 (892519254) 907548567      998 2023-01-13 10:53:42.000000 python-sat-1.8.dev8/tests/test_atmostk.py
+-rw-r--r--   0 aign0002 (892519254) 907548567     1299 2024-03-17 06:23:23.000000 python-sat-1.8.dev8/tests/test_boolengine.py
+-rw-r--r--   0 aign0002 (892519254) 907548567     2432 2023-07-12 00:04:57.000000 python-sat-1.8.dev8/tests/test_cnfplus.py
+-rw-r--r--   0 aign0002 (892519254) 907548567      784 2023-01-13 10:53:42.000000 python-sat-1.8.dev8/tests/test_equals1.py
+-rw-r--r--   0 aign0002 (892519254) 907548567     1007 2023-03-05 06:31:37.000000 python-sat-1.8.dev8/tests/test_process.py
+-rw-r--r--   0 aign0002 (892519254) 907548567     1260 2024-03-17 06:23:42.000000 python-sat-1.8.dev8/tests/test_propagate.py
+-rw-r--r--   0 aign0002 (892519254) 907548567      890 2023-07-12 00:05:05.000000 python-sat-1.8.dev8/tests/test_unique_model.py
+-rw-r--r--   0 aign0002 (892519254) 907548567      937 2023-01-13 10:53:42.000000 python-sat-1.8.dev8/tests/test_unique_mus.py
+-rw-r--r--   0 aign0002 (892519254) 907548567      650 2023-07-12 00:05:10.000000 python-sat-1.8.dev8/tests/test_warmstart.py
```

### Comparing `python-sat-1.8.dev7/LICENSE.txt` & `python-sat-1.8.dev8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev7/PKG-INFO` & `python-sat-1.8.dev8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-sat
-Version: 1.8.dev7
+Version: 1.8.dev8
 Summary: A Python library for prototyping with SAT oracles
 Home-page: https://github.com/pysathq/pysat
 Author: Alexey Ignatiev, Joao Marques-Silva, Antonio Morgado
 Author-email: alexey.ignatiev@monash.edu, joao.marques-silva@univ-toulouse.fr, ajrmorgado@gmail.com
 License: MIT
 Description-Content-Type: text/x-rst; charset=UTF-8
 License-File: LICENSE.txt
```

### Comparing `python-sat-1.8.dev7/README.rst` & `python-sat-1.8.dev8/README.rst`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev7/allies/approxmc.py` & `python-sat-1.8.dev8/allies/approxmc.py`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev7/allies/unigen.py` & `python-sat-1.8.dev8/allies/unigen.py`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev7/cardenc/bitwise.hh` & `python-sat-1.8.dev8/cardenc/bitwise.hh`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev7/cardenc/card.hh` & `python-sat-1.8.dev8/cardenc/card.hh`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev7/cardenc/clset.hh` & `python-sat-1.8.dev8/cardenc/clset.hh`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev7/cardenc/common.hh` & `python-sat-1.8.dev8/cardenc/common.hh`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev7/cardenc/itot.hh` & `python-sat-1.8.dev8/cardenc/itot.hh`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev7/cardenc/ladder.hh` & `python-sat-1.8.dev8/cardenc/ladder.hh`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev7/cardenc/mto.hh` & `python-sat-1.8.dev8/cardenc/mto.hh`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev7/cardenc/pairwise.hh` & `python-sat-1.8.dev8/cardenc/pairwise.hh`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev7/cardenc/ptypes.hh` & `python-sat-1.8.dev8/cardenc/ptypes.hh`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev7/cardenc/pycard.cc` & `python-sat-1.8.dev8/cardenc/pycard.cc`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev7/cardenc/seqcounter.hh` & `python-sat-1.8.dev8/cardenc/seqcounter.hh`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev7/cardenc/sortcard.hh` & `python-sat-1.8.dev8/cardenc/sortcard.hh`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev7/cardenc/utils.hh` & `python-sat-1.8.dev8/cardenc/utils.hh`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev7/examples/fm.py` & `python-sat-1.8.dev8/examples/fm.py`

 * *Files 1% similar despite different names*

```diff
@@ -205,14 +205,18 @@
             :param with_soft: copy formula's soft clauses to the oracle or not
             :type with_soft: bool
         """
 
         self.oracle = Solver(name=self.solver, bootstrap_with=self.hard, use_timer=True)
 
         if self.atm1:  # this check is needed at the beggining (before iteration 1)
+            # we are using CaDiCaL195 and it can use external linear engine
+            if self.solver in SolverNames.cadical195:
+                self.oracle.activate_atmost()
+
             assert self.oracle.supports_atmost(), \
                     '{0} does not support native cardinality constraints. Make sure you use the right type of formula.'.format(solver_name)
 
             # self.atm1 is not empty only in case of minicard
             for am in self.atm1:
                 self.oracle.add_atmost(*am)
 
@@ -467,15 +471,16 @@
             verbose += 1
         else:
             assert False, 'Unhandled option: {0} {1}'.format(opt, arg)
 
     cardenc = encmap[cardenc]
 
     # using minicard's native implementation of AtMost1 constraints
-    if solver in SolverNames.minicard or solver in SolverNames.gluecard3 or solver in SolverNames.gluecard4:
+    if solver in SolverNames.minicard + SolverNames.gluecard3 + \
+            SolverNames.gluecard4 + SolverNames.cadical195:
         cardenc = encmap['native']
     else:
         assert cardenc != encmap['native'], 'Only Minicard can handle cardinality constraints natively'
 
     return solver, cardenc, verbose, args
 
 
@@ -487,15 +492,15 @@
 
     print('Usage:', os.path.basename(sys.argv[0]), '[options] dimacs-file')
     print('Options:')
     print('        -c, --cardenc    Cardinality encoding to use:')
     print('                         Available values: bw, cardn, kmtot, ladder, mtot, pw, seqc, sortn, tot (default = seqc)')
     print('        -h, --help')
     print('        -s, --solver     SAT solver to use')
-    print('                         Available values: g3, g4, lgl, mcb, mcm, mpl, m22, mc, mgh (default = m22)')
+    print('                         Available values: cd15, cd19, g3, g4, lgl, mcb, mcm, mpl, m22, mc, mgh (default = m22)')
     print('        -v, --verbose    Be verbose')
 
 
 #
 #==============================================================================
 if __name__ == '__main__':
     solver, cardenc, verbose, files = parse_options()
```

### Comparing `python-sat-1.8.dev7/examples/genhard.py` & `python-sat-1.8.dev8/examples/genhard.py`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev7/examples/hitman.py` & `python-sat-1.8.dev8/examples/hitman.py`

 * *Files 2% similar despite different names*

```diff
@@ -389,23 +389,29 @@
             self.oracle = LBX(formula, solver_name=self.solver,
                     use_cld=self.usecld)
         elif self.htype == 'mcsls':
             self.oracle = MCSls(formula, solver_name=self.solver,
                     use_cld=self.usecld)
         else:  # 'sat'
             assert self.solver in SolverNames.minisatgh + \
-                    SolverNames.lingeling + SolverNames.cadical153, \
-                    'Hard polarity setting is unsupported by {0}'.format(self.solver)
-
-            assert formula.atms == [], 'Native AtMostK constraints aren\'t' \
-            'supported by MinisatGH, Lingeling, or CaDiCaL 153'
+                    SolverNames.lingeling + SolverNames.cadical153 + \
+                    SolverNames.cadical195, 'Hard polarity setting is unsupported by {0}'.format(self.solver)
 
             # setting up a SAT solver, so that it supports the same interface
-            self.oracle = Solver(name=self.solver, bootstrap_with=formula.hard,
-                                 use_timer=True)
+            if formula.atms == []:
+                self.oracle = Solver(name=self.solver, bootstrap_with=formula.hard,
+                                    use_timer=True)
+            elif self.solver in SolverNames.cadical195:
+                self.oracle = Solver(name=self.solver, bootstrap_with=formula.hard,
+                                    use_timer=True, native_card=True)
+
+                for atm in formula.atms:
+                    self.oracle.add_atmost(*atm)
+            else:
+                assert 0, 'Native AtMostK constraints aren\'t supported by MinisatGH, Lingeling, or CaDiCaL 153'
 
             # MinisatGH supports warm start mode
             if self.solver in SolverNames.minisatgh:
                 self.oracle.start_mode(warm=True)
 
             # soft clauses are enforced by means of setting polarities
             self.oracle.set_phases(literals=[self.phase * cl[0] for cl in formula.soft])
```

### Comparing `python-sat-1.8.dev7/examples/lbx.py` & `python-sat-1.8.dev8/examples/lbx.py`

 * *Files 0% similar despite different names*

```diff
@@ -132,14 +132,18 @@
         self.oracle = Solver(name=solver_name, bootstrap_with=formula.hard,
                 use_timer=use_timer)
         self.solver = solver_name
 
         # adding native cardinality constraints (if any) as hard clauses
         # this can be done only if the Minicard solver is in use
         if isinstance(formula, WCNFPlus) and formula.atms:
+            # we are using CaDiCaL195 and it can use external linear engine
+            if solver_name in SolverNames.cadical195:
+                self.oracle.activate_atmost()
+
             assert self.oracle.supports_atmost(), \
                     '{0} does not support native cardinality constraints. Make sure you use the right type of formula.'.format(solver_name)
 
             for atm in formula.atms:
                 self.oracle.add_atmost(*atm)
 
         self.topv = formula.nv  # top variable id
@@ -556,15 +560,15 @@
     print('Usage:', os.path.basename(sys.argv[0]), '[options] file')
     print('Options:')
     print('        -d, --dcalls           Apply clause D calls')
     print('        -e, --enum=<string>    How many solutions to compute')
     print('                               Available values: [1 .. all] (default: 1)')
     print('        -h, --help')
     print('        -s, --solver           SAT solver to use')
-    print('                               Available values: g3, g4, lgl, mcb, mcm, mpl, m22, mc, mgh (default = m22)')
+    print('                               Available values: cd15, cd19, g3, g4, lgl, mcb, mcm, mpl, m22, mc, mgh (default = m22)')
     print('        -v, --verbose          Be verbose')
 
 
 #
 #==============================================================================
 if __name__ == '__main__':
     dcalls, to_enum, solver, verbose, files = parse_options()
```

### Comparing `python-sat-1.8.dev7/examples/lsu.py` & `python-sat-1.8.dev8/examples/lsu.py`

 * *Files 4% similar despite different names*

```diff
@@ -114,30 +114,33 @@
 
         The constructor receives an input :class:`.WCNF` formula, a name of the
         SAT solver to use (see :class:`.SolverNames` for details), and an
         integer verbosity level.
 
         :param formula: input MaxSAT formula
         :param solver: name of SAT solver
+        :param incr: enable incremental mode of Glucose
         :param expect_interrupt: whether or not an :meth:`interrupt` call is expected
         :param verbose: verbosity level
 
         :type formula: :class:`.WCNF`
         :type solver: str
+        :type incr: bool
         :type expect_interrupt: bool
         :type verbose: int
     """
 
-    def __init__(self, formula, solver='g4', expect_interrupt=False, verbose=0):
+    def __init__(self, formula, solver='g4', incr=False, expect_interrupt=False, verbose=0):
         """
             Constructor.
         """
 
         self.verbose = verbose
         self.solver = solver
+        self.incr = incr
         self.expect_interrupt = expect_interrupt
         self.formula = formula
         self.topv = formula.nv  # largest variable index
         self.sels = []          # soft clause selector variables
         self.tot = None         # totalizer encoder for the cardinality constraint
         self._init(formula)     # initiaize SAT oracle
 
@@ -150,15 +153,15 @@
             stored in variable ``self.sels``.
 
             :param formula: input MaxSAT formula
             :type formula: :class:`WCNF`
         """
 
         self.oracle = Solver(name=self.solver, bootstrap_with=formula.hard,
-                incr=True, use_timer=True)
+                incr=self.incr, use_timer=True)
 
         for i, cl in enumerate(formula.soft):
             # TODO: if clause is unit, use its literal as selector
             # (ITotalizer must be extended to support PB constraints first)
             self.topv += 1
             selv = self.topv
             cl.append(self.topv)
@@ -349,26 +352,31 @@
         :param verbose: verbosity level
 
         :type formula: :class:`.WCNFPlus`
         :type expect_interrupt: bool
         :type verbose: int
     """
 
-    def __init__(self, formula, solver, expect_interrupt=False, verbose=0):
+    def __init__(self, formula, solver='g4', incr=False, expect_interrupt=False, verbose=0):
         """
             Constructor.
         """
 
         assert solver in SolverNames.gluecard3 or \
                 solver in SolverNames.gluecard4 or \
-                solver in SolverNames.minicard, '{0} does not support native cardinality constraints'.format(solver)
+                solver in SolverNames.minicard or \
+                solver in SolverNames.cadical195, '{0} does not support native cardinality constraints'.format(solver)
 
-        super(LSUPlus, self).__init__(formula, solver=solver,
+        super(LSUPlus, self).__init__(formula, solver=solver, incr=incr,
                 expect_interrupt=expect_interrupt, verbose=verbose)
 
+        # we are using CaDiCaL195 and it can use external linear engine
+        if solver in SolverNames.cadical195:
+            self.oracle.activate_atmost()
+
         # adding atmost constraints
         for am in formula.atms:
             self.oracle.add_atmost(*am)
 
     def _assert_lt(self, cost):
         """
             Overrides _assert_lt of :class:`.LSU` in order to use Minicard's
@@ -387,82 +395,86 @@
 #==============================================================================
 def parse_options():
     """
         Parses command-line options.
     """
 
     try:
-        opts, args = getopt.getopt(sys.argv[1:], 'hms:t:v', ['help', 'model', 'solver=', 'timeout=', 'verbose'])
+        opts, args = getopt.getopt(sys.argv[1:], 'hims:t:v', ['help', 'incr', 'model', 'solver=', 'timeout=', 'verbose'])
     except getopt.GetoptError as err:
         sys.stderr.write(str(err).capitalize())
         print_usage()
         sys.exit(1)
 
     solver = 'g4'
+    incr = False
     verbose = 1
     print_model = False
     timeout = None
 
     for opt, arg in opts:
         if opt in ('-h', '--help'):
             print_usage()
             sys.exit(0)
+        elif opt in ('-i', '--incr'):
+            incr = True
         elif opt in ('-m', '--model'):
             print_model = True
         elif opt in ('-s', '--solver'):
             solver = str(arg)
         elif opt in ('-t', '--timeout'):
             if str(arg) != 'none':
                 timeout = float(arg)
         elif opt in ('-v', '--verbose'):
             verbose += 1
         else:
             assert False, 'Unhandled option: {0} {1}'.format(opt, arg)
 
-    return print_model, solver, timeout, verbose, args
+    return incr, print_model, solver, timeout, verbose, args
 
 
 #
 #==============================================================================
 def print_usage():
     """
         Prints usage message.
     """
 
     print('Usage: ' + os.path.basename(sys.argv[0]) + ' [options] dimacs-file')
     print('Options:')
     print('        -h, --help               Show this message')
+    print('        -i, --incr               Enable incremental model (for Glucose only)')
     print('        -m, --model              Print model')
     print('        -s, --solver=<string>    SAT solver to use')
-    print('                                 Available values: g3, g4, mc, m22, mgh (default = g4)')
+    print('                                 Available values: cd15, cd19, g3, g4, mc, m22, mgh (default = g4)')
     print('        -t, --timeout=<float>    Set time limit for MaxSAT solver')
     print('                                 Available values: [0 .. FLOAT_MAX], none (default: none)')
     print('        -v, --verbose            Be verbose')
 
 
 #
 #==============================================================================
 if __name__ == '__main__':
-    print_model, solver, timeout, verbose, files = parse_options()
+    incr, print_model, solver, timeout, verbose, files = parse_options()
 
     if files:
         # reading standard CNF or WCNF
         if re.search('cnf(\.(gz|bz2|lzma|xz))?$', files[0]):
             if re.search('\.wcnf(\.(gz|bz2|lzma|xz))?$', files[0]):
                 formula = WCNF(from_file=files[0])
             else:  # expecting '*.cnf'
                 formula = CNF(from_file=files[0]).weighted()
 
-            lsu = LSU(formula, solver=solver,
+            lsu = LSU(formula, solver=solver, incr=incr,
                     expect_interrupt=(timeout != None), verbose=verbose)
 
         # reading WCNF+
         elif re.search('\.wcnf[p,+](\.(gz|bz2|lzma|xz))?$', files[0]):
             formula = WCNFPlus(from_file=files[0])
-            lsu = LSUPlus(formula, solver=solver,
+            lsu = LSUPlus(formula, solver=solver, incr=incr,
                     expect_interrupt=(timeout != None), verbose=verbose)
 
         # setting a timer if necessary
         if timeout is not None:
             if verbose > 1:
                 print('c timeout: {0}'.format(timeout))
```

### Comparing `python-sat-1.8.dev7/examples/mcsls.py` & `python-sat-1.8.dev8/examples/mcsls.py`

 * *Files 1% similar despite different names*

```diff
@@ -132,14 +132,18 @@
         self.oracle = Solver(name=solver_name, bootstrap_with=formula.hard,
                 use_timer=use_timer)
         self.solver = solver_name
 
         # adding native cardinality constraints (if any) as hard clauses
         # this can be done only if the Minicard solver is in use
         if isinstance(formula, WCNFPlus) and formula.atms:
+            # we are using CaDiCaL195 and it can use external linear engine
+            if solver_name in SolverNames.cadical195:
+                self.oracle.activate_atmost()
+
             assert self.oracle.supports_atmost(), \
                     '{0} does not support native cardinality constraints. Make sure you use the right type of formula.'.format(solver_name)
 
             for atm in formula.atms:
                 self.oracle.add_atmost(*atm)
 
         self.topv = formula.nv  # top variable id
@@ -531,15 +535,15 @@
     print('Usage:', os.path.basename(sys.argv[0]), '[options] file')
     print('Options:')
     print('        -d, --dcalls           Apply clause D calls')
     print('        -e, --enum=<string>    How many solutions to compute')
     print('                               Available values: [1 .. all] (default: 1)')
     print('        -h, --help')
     print('        -s, --solver           SAT solver to use')
-    print('                               Available values: g3, g4, lgl, mcb, mcm, mpl, m22, mc, mgh (default = m22)')
+    print('                               Available values: cd15, cd19, g3, g4, lgl, mcb, mcm, mpl, m22, mc, mgh (default = m22)')
     print('        -v, --verbose          Be verbose')
 
 
 #
 #==============================================================================
 if __name__ == '__main__':
     dcalls, to_enum, solver, verbose, files = parse_options()
```

### Comparing `python-sat-1.8.dev7/examples/models.py` & `python-sat-1.8.dev8/examples/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -83,17 +83,19 @@
         :type warm: bool
     """
 
     with Solver(name=solver, bootstrap_with=formula.clauses,
                 use_timer=True, warm_start=warm) as s:
         # adding native cardinality constraints if needed
         if formula.atmosts:
-            assert solver in SolverNames.minicard or \
-                    solver in SolverNames.gluecard3 or \
-                    solver in SolverNames.gluecard4, \
+            # we are using CaDiCaL195 and it can use external linear engine
+            if solver in SolverNames.cadical195:
+                s.activate_atmost()
+
+            assert s.supports_atmost(), \
                     '{0} does not support native cardinality constraints'.format(solver)
 
             for atm in formula.atmosts:
                 s.add_atmost(*atm)
 
         # model enumeration and printing is done here
         computed = 0
```

### Comparing `python-sat-1.8.dev7/examples/musx.py` & `python-sat-1.8.dev8/examples/musx.py`

 * *Files 1% similar despite different names*

```diff
@@ -141,14 +141,18 @@
         self.sels, self.vmap = [], {}
 
         # constructing the oracle
         self.oracle = Solver(name=solver, bootstrap_with=formula.hard,
                 use_timer=True)
 
         if isinstance(formula, WCNFPlus) and formula.atms:
+            # we are using CaDiCaL195 and it can use external linear engine
+            if solver in SolverNames.cadical195:
+                self.oracle.activate_atmost()
+
             assert self.oracle.supports_atmost(), \
                     '{0} does not support native cardinality constraints. Make sure you use the right type of formula.'.format(solver_name)
 
             for atm in formula.atms:
                 self.oracle.add_atmost(*atm)
 
         # relaxing soft clauses and adding them to the oracle
@@ -304,15 +308,15 @@
         Prints usage message.
         """
 
     print('Usage:', os.path.basename(sys.argv[0]), '[options] dimacs-file')
     print('Options:')
     print('        -h, --help')
     print('        -s, --solver     SAT solver to use')
-    print('                         Available values: g3, lgl, mcb, mcm, mpl, m22, mc, mgh (default: m22)')
+    print('                         Available values: cd15, cd19, g3, lgl, mcb, mcm, mpl, m22, mc, mgh (default: m22)')
     print('        -v, --verbose    Be verbose')
 
 
 #
 #==============================================================================
 if __name__ == '__main__':
     solver, verbose, files = parse_options()
```

### Comparing `python-sat-1.8.dev7/examples/optux.py` & `python-sat-1.8.dev8/examples/optux.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,15 +107,15 @@
 #==============================================================================
 from __future__ import print_function
 import getopt
 import os
 from pysat.examples.hitman import Atom, Hitman
 from pysat.examples.rc2 import RC2
 from pysat.formula import CNFPlus, WCNFPlus
-from pysat.solvers import Solver
+from pysat.solvers import Solver, SolverNames
 import re
 import sys
 
 
 #
 #==============================================================================
 class OptUx(object):
@@ -285,14 +285,18 @@
 
         # SAT oracle bootstrapped with the hard clauses; note that
         # clauses of the unit-size MCSes are enforced to be enabled
         self.oracle = Solver(name=solver, bootstrap_with=unweighted.hard +
                 [[mcs] for mcs in self.units])
 
         if unweighted.atms:
+            if solver in SolverNames.cadical195:
+                # we are using CaDiCaL195 and it can use external linear engine
+                self.oracle.activate_atmost()
+
             assert self.oracle.supports_atmost(), \
                     '{0} does not support native cardinality constraints. Make sure you use the right type of formula.'.format(self.solver)
 
             for atm in unweighted.atms:
                 self.oracle.add_atmost(*atm)
 
     def __del__(self):
@@ -554,15 +558,15 @@
 
     adapt = False
     cover = None
     dcalls = False
     exhaust = False
     minz = False
     to_enum = 1
-    solver = 'm22'
+    solver = 'g3'
     puresat = False
     unsorted = False
     trim = 0
     verbose = 1
 
     for opt, arg in opts:
         if opt in ('-a', '--adapt'):
@@ -615,18 +619,18 @@
     print('                                  Available values: any valid file path, none (default = none)')
     print('        -d, --dcalls              Apply clause D calls (in unsorted enumeration only)')
     print('        -e, --enum=<string>       Enumerate top-k solutions')
     print('                                  Available values: [1 .. INT_MAX], all (default: 1)')
     print('        -h, --help                Show this message')
     print('        -m, --minimize            Use a heuristic unsatisfiable core minimizer')
     print('        -p, --puresat=<string>    Use a pure SAT-based hitting set enumerator')
-    print('                                  Available values: cd15, lgl, mgh (default = mgh)')
+    print('                                  Available values: cd15, cd19, lgl, mgh (default = mgh)')
     print('                                  Requires: unsorted mode, i.e. \'-u\'')
     print('        -s, --solver              SAT solver to use')
-    print('                                  Available values: g3, g4, lgl, mcb, mcm, mpl, m22, mc, mgh (default = m22)')
+    print('                                  Available values: cd15, cd19, g3, g4, lgl, mcb, mcm, mpl, m22, mc, mgh (default = g3)')
     print('        -t, --trim=<int>          How many times to trim unsatisfiable cores')
     print('                                  Available values: [0 .. INT_MAX] (default = 0)')
     print('        -u, --unsorted            Enumerate MUSes in an unsorted way')
     print('        -v, --verbose             Be verbose')
     print('        -x, --exhaust             Exhaust new unsatisfiable cores')
```

### Comparing `python-sat-1.8.dev7/examples/rc2.py` & `python-sat-1.8.dev8/examples/rc2.py`

 * *Files 0% similar despite different names*

```diff
@@ -281,14 +281,18 @@
         self.oracle = Solver(name=self.solver, bootstrap_with=formula.hard,
                 incr=incr, use_timer=True)
 
         # adding native cardinality constraints (if any) as hard clauses
         # this can be done only if the Minicard solver is in use
         # this cannot be done if RC2 is run from the command line
         if isinstance(formula, WCNFPlus) and formula.atms:
+            # we are using CaDiCaL195 and it can use external linear engine
+            if self.solver in SolverNames.cadical195:
+                self.oracle.activate_atmost()
+
             assert self.oracle.supports_atmost(), \
                     '{0} does not support native cardinality constraints. Make sure you use the right type of formula.'.format(self.solver)
 
             for atm in formula.atms:
                 self.oracle.add_atmost(*atm)
 
         # adding soft clauses to oracle
@@ -385,15 +389,15 @@
                 self.oracle.add_clause(cl)
             else:
                 # this should be a native cardinality constraint,
                 # which can be used only together with Minicard
                 assert self.oracle.supports_atmost(), \
                         '{0} does not support native cardinality constraints. Make sure you use the right type of formula.'.format(self.solver)
 
-                self.oracle.add_atmost(cl, clause[1])
+                self.oracle.add_atmost(cl, clause[1], weights=clause[2] if len(clause) == 3 else [])
         else:
             # soft clauses should be augmented with a selector
             selv = cl[0]  # for a unit clause, no selector is needed
 
             if len(cl) > 1:
                 selv = self.pool.id()
 
@@ -416,15 +420,15 @@
     def delete(self):
         """
             Explicit destructor of the internal SAT oracle and all the
             totalizer objects creating during the solving process.
         """
 
         if self.oracle:
-            if not self.oracle.supports_atmost():  # for minicard, there is nothing to free
+            if not self.oracle.supports_atmost():  # for minicard-like, there is nothing to free
                 for t in six.itervalues(self.tobj):
                     t.delete()
 
             self.oracle.delete()
             self.oracle = None
 
     def compute(self):
@@ -1711,15 +1715,15 @@
     print('                                 Available values: [1 .. INT_MAX], all (default = 1)')
     print('        -h, --help               Show this message')
     print('        -i, --incr               Use SAT solver incrementally (only for g3 and g4)')
     print('        -l, --blo=<string>       Use BLO and stratification')
     print('                                 Available values: basic, div, cluster, none, full (default = none)')
     print('        -m, --minimize           Use a heuristic unsatisfiable core minimizer')
     print('        -s, --solver=<string>    SAT solver to use')
-    print('                                 Available values: g3, g4, lgl, mcb, mcm, mpl, m22, mc, mgh (default = g3)')
+    print('                                 Available values: cd15, cd19, g3, g4, lgl, mcb, mcm, mpl, m22, mc, mgh (default = g3)')
     print('        -t, --trim=<int>         How many times to trim unsatisfiable cores')
     print('                                 Available values: [0 .. INT_MAX] (default = 0)')
     print('        -v, --verbose            Be verbose')
     print('        --vnew                   Print v-line in the new format')
     print('        -x, --exhaust            Exhaust new unsatisfiable cores')
```

### Comparing `python-sat-1.8.dev7/examples/usage.py` & `python-sat-1.8.dev8/examples/usage.py`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev7/pysat/_fileio.py` & `python-sat-1.8.dev8/pysat/_fileio.py`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev7/pysat/_utils.py` & `python-sat-1.8.dev8/pysat/_utils.py`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev7/pysat/card.py` & `python-sat-1.8.dev8/pysat/card.py`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev7/pysat/engines.py` & `python-sat-1.8.dev8/pysat/engines.py`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev7/pysat/formula.py` & `python-sat-1.8.dev8/pysat/formula.py`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev7/pysat/pb.py` & `python-sat-1.8.dev8/pysat/pb.py`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev7/pysat/process.py` & `python-sat-1.8.dev8/pysat/process.py`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev7/pysat/solvers.py` & `python-sat-1.8.dev8/pysat/solvers.py`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev7/python_sat.egg-info/PKG-INFO` & `python-sat-1.8.dev8/python_sat.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-sat
-Version: 1.8.dev7
+Version: 1.8.dev8
 Summary: A Python library for prototyping with SAT oracles
 Home-page: https://github.com/pysathq/pysat
 Author: Alexey Ignatiev, Joao Marques-Silva, Antonio Morgado
 Author-email: alexey.ignatiev@monash.edu, joao.marques-silva@univ-toulouse.fr, ajrmorgado@gmail.com
 License: MIT
 Description-Content-Type: text/x-rst; charset=UTF-8
 License-File: LICENSE.txt
```

### Comparing `python-sat-1.8.dev7/python_sat.egg-info/SOURCES.txt` & `python-sat-1.8.dev8/python_sat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev7/setup.py` & `python-sat-1.8.dev8/setup.py`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev7/solvers/cadical103.tar.gz` & `python-sat-1.8.dev8/solvers/cadical103.tar.gz`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev7/solvers/cadical153.tar.gz` & `python-sat-1.8.dev8/solvers/cadical153.tar.gz`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev7/solvers/cadical170.tar.gz` & `python-sat-1.8.dev8/solvers/cadical170.tar.gz`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev7/solvers/cadical195.tar.gz` & `python-sat-1.8.dev8/solvers/cadical195.tar.gz`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev7/solvers/glucose30.tar.gz` & `python-sat-1.8.dev8/solvers/glucose30.tar.gz`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev7/solvers/glucose41.tar.gz` & `python-sat-1.8.dev8/solvers/glucose41.tar.gz`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev7/solvers/glucose421.tar.gz` & `python-sat-1.8.dev8/solvers/glucose421.tar.gz`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev7/solvers/lingeling.tar.gz` & `python-sat-1.8.dev8/solvers/lingeling.tar.gz`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev7/solvers/maplechrono.zip` & `python-sat-1.8.dev8/solvers/maplechrono.zip`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev7/solvers/maplecm.zip` & `python-sat-1.8.dev8/solvers/maplecm.zip`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev7/solvers/maplesat.zip` & `python-sat-1.8.dev8/solvers/maplesat.zip`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev7/solvers/mergesat3.tar.gz` & `python-sat-1.8.dev8/solvers/mergesat3.tar.gz`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev7/solvers/minicard.tar.gz` & `python-sat-1.8.dev8/solvers/minicard.tar.gz`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev7/solvers/minisat22.tar.gz` & `python-sat-1.8.dev8/solvers/minisat22.tar.gz`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev7/solvers/minisatgh.zip` & `python-sat-1.8.dev8/solvers/minisatgh.zip`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev7/solvers/patches/cadical103.patch` & `python-sat-1.8.dev8/solvers/patches/cadical103.patch`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev7/solvers/patches/cadical153.patch` & `python-sat-1.8.dev8/solvers/patches/cadical153.patch`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev7/solvers/patches/cadical195.patch` & `python-sat-1.8.dev8/solvers/patches/cadical195.patch`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev7/solvers/patches/glucose30.patch` & `python-sat-1.8.dev8/solvers/patches/glucose30.patch`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev7/solvers/patches/glucose41.patch` & `python-sat-1.8.dev8/solvers/patches/glucose41.patch`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev7/solvers/patches/glucose421.patch` & `python-sat-1.8.dev8/solvers/patches/glucose421.patch`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev7/solvers/patches/gluecard30.patch` & `python-sat-1.8.dev8/solvers/patches/gluecard30.patch`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev7/solvers/patches/gluecard41.patch` & `python-sat-1.8.dev8/solvers/patches/gluecard41.patch`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev7/solvers/patches/lingeling.patch` & `python-sat-1.8.dev8/solvers/patches/lingeling.patch`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev7/solvers/patches/maplechrono.patch` & `python-sat-1.8.dev8/solvers/patches/maplechrono.patch`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev7/solvers/patches/maplecm.patch` & `python-sat-1.8.dev8/solvers/patches/maplecm.patch`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev7/solvers/patches/maplesat.patch` & `python-sat-1.8.dev8/solvers/patches/maplesat.patch`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev7/solvers/patches/mergesat3.patch` & `python-sat-1.8.dev8/solvers/patches/mergesat3.patch`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev7/solvers/patches/minicard.patch` & `python-sat-1.8.dev8/solvers/patches/minicard.patch`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev7/solvers/patches/minisat22.patch` & `python-sat-1.8.dev8/solvers/patches/minisat22.patch`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev7/solvers/patches/minisatgh.patch` & `python-sat-1.8.dev8/solvers/patches/minisatgh.patch`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev7/solvers/prepare.py` & `python-sat-1.8.dev8/solvers/prepare.py`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev7/solvers/pysolvers.cc` & `python-sat-1.8.dev8/solvers/pysolvers.cc`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev7/tests/test_accum_stats.py` & `python-sat-1.8.dev8/tests/test_accum_stats.py`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev7/tests/test_atmost1.py` & `python-sat-1.8.dev8/tests/test_atmost1.py`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev7/tests/test_atmostk.py` & `python-sat-1.8.dev8/tests/test_atmostk.py`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev7/tests/test_boolengine.py` & `python-sat-1.8.dev8/tests/test_boolengine.py`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev7/tests/test_cnfplus.py` & `python-sat-1.8.dev8/tests/test_cnfplus.py`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev7/tests/test_equals1.py` & `python-sat-1.8.dev8/tests/test_equals1.py`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev7/tests/test_process.py` & `python-sat-1.8.dev8/tests/test_process.py`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev7/tests/test_propagate.py` & `python-sat-1.8.dev8/tests/test_propagate.py`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev7/tests/test_unique_model.py` & `python-sat-1.8.dev8/tests/test_unique_model.py`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev7/tests/test_unique_mus.py` & `python-sat-1.8.dev8/tests/test_unique_mus.py`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev7/tests/test_warmstart.py` & `python-sat-1.8.dev8/tests/test_warmstart.py`

 * *Files identical despite different names*

