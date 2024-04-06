# Comparing `tmp/lisaanalysistools-1.0.3.tar.gz` & `tmp/lisaanalysistools-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lisaanalysistools-1.0.3.tar", last modified: Fri Apr  5 07:54:53 2024, max compression
+gzip compressed data, was "lisaanalysistools-1.0.4.tar", last modified: Sat Apr  6 01:31:17 2024, max compression
```

## Comparing `lisaanalysistools-1.0.3.tar` & `lisaanalysistools-1.0.4.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 mlkatz1    (502) staff       (20)        0 2024-04-05 07:54:53.212034 lisaanalysistools-1.0.3/
--rw-r--r--   0 mlkatz1    (502) staff       (20)        0 2024-03-22 19:17:22.000000 lisaanalysistools-1.0.3/CHANGELOG
--rw-r--r--   0 mlkatz1    (502) staff       (20)    11357 2024-03-22 19:17:22.000000 lisaanalysistools-1.0.3/LICENSE
-drwxr-xr-x   0 mlkatz1    (502) staff       (20)        0 2024-04-05 07:54:53.209537 lisaanalysistools-1.0.3/LISAanalysistools.egg-info/
--rw-r--r--   0 mlkatz1    (502) staff       (20)     2753 2024-04-05 07:54:53.000000 lisaanalysistools-1.0.3/LISAanalysistools.egg-info/PKG-INFO
--rw-r--r--   0 mlkatz1    (502) staff       (20)     1802 2024-04-05 07:54:53.000000 lisaanalysistools-1.0.3/LISAanalysistools.egg-info/SOURCES.txt
--rw-r--r--   0 mlkatz1    (502) staff       (20)        1 2024-04-05 07:54:53.000000 lisaanalysistools-1.0.3/LISAanalysistools.egg-info/dependency_links.txt
--rw-r--r--   0 mlkatz1    (502) staff       (20)        1 2024-03-13 23:07:52.000000 lisaanalysistools-1.0.3/LISAanalysistools.egg-info/not-zip-safe
--rw-r--r--   0 mlkatz1    (502) staff       (20)       14 2024-04-05 07:54:53.000000 lisaanalysistools-1.0.3/LISAanalysistools.egg-info/top_level.txt
--rw-r--r--   0 mlkatz1    (502) staff       (20)      451 2024-03-22 19:17:22.000000 lisaanalysistools-1.0.3/MANIFEST.in
--rw-r--r--   0 mlkatz1    (502) staff       (20)     4756 2024-03-22 19:17:22.000000 lisaanalysistools-1.0.3/Makefile
--rw-r--r--   0 mlkatz1    (502) staff       (20)     2753 2024-04-05 07:54:53.210898 lisaanalysistools-1.0.3/PKG-INFO
--rw-r--r--   0 mlkatz1    (502) staff       (20)     2156 2024-04-05 07:51:03.000000 lisaanalysistools-1.0.3/README.md
-drwxr-xr-x   0 mlkatz1    (502) staff       (20)        0 2024-04-05 07:54:53.151281 lisaanalysistools-1.0.3/include/
--rw-r--r--   0 mlkatz1    (502) staff       (20)     1694 2024-03-22 19:17:23.000000 lisaanalysistools-1.0.3/include/Detector.hpp
-drwxr-xr-x   0 mlkatz1    (502) staff       (20)        0 2024-04-05 07:54:53.166318 lisaanalysistools-1.0.3/lisatools/
--rw-r--r--   0 mlkatz1    (502) staff       (20)        0 2023-05-16 15:40:56.000000 lisaanalysistools-1.0.3/lisatools/__init__.py
--rw-r--r--   0 mlkatz1    (502) staff       (20)      123 2024-04-05 07:54:53.000000 lisaanalysistools-1.0.3/lisatools/_version.py
--rw-r--r--   0 mlkatz1    (502) staff       (20)    15333 2024-04-04 00:21:39.000000 lisaanalysistools-1.0.3/lisatools/analysiscontainer.py
--rw-r--r--   0 mlkatz1    (502) staff       (20)     9224 2024-03-22 19:17:23.000000 lisaanalysistools-1.0.3/lisatools/datacontainer.py
--rw-r--r--   0 mlkatz1    (502) staff       (20)    13852 2024-04-02 17:24:55.000000 lisaanalysistools-1.0.3/lisatools/detector.py
--rw-r--r--   0 mlkatz1    (502) staff       (20)    34177 2024-03-22 19:17:23.000000 lisaanalysistools-1.0.3/lisatools/diagnostic.py
--rw-r--r--   0 mlkatz1    (502) staff       (20)     5154 2024-02-20 21:17:07.000000 lisaanalysistools-1.0.3/lisatools/glitch.py
-drwxr-xr-x   0 mlkatz1    (502) staff       (20)        0 2024-04-05 07:54:53.171704 lisaanalysistools-1.0.3/lisatools/sampling/
--rw-r--r--   0 mlkatz1    (502) staff       (20)        0 2023-05-16 15:40:56.000000 lisaanalysistools-1.0.3/lisatools/sampling/__init__.py
--rw-r--r--   0 mlkatz1    (502) staff       (20)    29585 2024-03-22 19:17:23.000000 lisaanalysistools-1.0.3/lisatools/sampling/likelihood.py
-drwxr-xr-x   0 mlkatz1    (502) staff       (20)        0 2024-04-05 07:54:53.182855 lisaanalysistools-1.0.3/lisatools/sampling/moves/
--rw-r--r--   0 mlkatz1    (502) staff       (20)        0 2023-05-16 15:40:56.000000 lisaanalysistools-1.0.3/lisatools/sampling/moves/__init__.py
--rw-r--r--   0 mlkatz1    (502) staff       (20)     1220 2023-06-08 00:14:36.000000 lisaanalysistools-1.0.3/lisatools/sampling/moves/gbgroupstretch.py
--rw-r--r--   0 mlkatz1    (502) staff       (20)    51802 2024-01-25 22:07:16.000000 lisaanalysistools-1.0.3/lisatools/sampling/moves/gbmultipletryrj.py
--rw-r--r--   0 mlkatz1    (502) staff       (20)    31152 2024-01-25 22:07:16.000000 lisaanalysistools-1.0.3/lisatools/sampling/moves/gbspecialgroupstretch.py
--rw-r--r--   0 mlkatz1    (502) staff       (20)    90189 2024-01-25 22:07:16.000000 lisaanalysistools-1.0.3/lisatools/sampling/moves/gbspecialstretch.py
--rw-r--r--   0 mlkatz1    (502) staff       (20)    14163 2023-10-25 21:01:10.000000 lisaanalysistools-1.0.3/lisatools/sampling/moves/mbhspecialmove.py
--rw-r--r--   0 mlkatz1    (502) staff       (20)      469 2023-06-08 00:14:36.000000 lisaanalysistools-1.0.3/lisatools/sampling/moves/placeholder.py
--rw-r--r--   0 mlkatz1    (502) staff       (20)     3348 2024-03-22 19:17:23.000000 lisaanalysistools-1.0.3/lisatools/sampling/moves/skymodehop.py
--rw-r--r--   0 mlkatz1    (502) staff       (20)    25092 2024-01-25 22:07:16.000000 lisaanalysistools-1.0.3/lisatools/sampling/moves/specialforegroundmove.py
--rw-r--r--   0 mlkatz1    (502) staff       (20)    18461 2024-03-22 19:17:23.000000 lisaanalysistools-1.0.3/lisatools/sampling/prior.py
--rw-r--r--   0 mlkatz1    (502) staff       (20)     9682 2024-03-22 19:17:23.000000 lisaanalysistools-1.0.3/lisatools/sampling/stopping.py
--rw-r--r--   0 mlkatz1    (502) staff       (20)    14340 2024-03-22 19:17:23.000000 lisaanalysistools-1.0.3/lisatools/sampling/utility.py
--rw-r--r--   0 mlkatz1    (502) staff       (20)    27236 2024-03-22 19:17:23.000000 lisaanalysistools-1.0.3/lisatools/sensitivity.py
-drwxr-xr-x   0 mlkatz1    (502) staff       (20)        0 2024-04-05 07:54:53.184698 lisaanalysistools-1.0.3/lisatools/sources/
--rw-r--r--   0 mlkatz1    (502) staff       (20)        0 2024-03-01 22:45:54.000000 lisaanalysistools-1.0.3/lisatools/sources/__init__.py
-drwxr-xr-x   0 mlkatz1    (502) staff       (20)        0 2024-04-05 07:54:53.186781 lisaanalysistools-1.0.3/lisatools/sources/emri/
--rw-r--r--   0 mlkatz1    (502) staff       (20)       41 2024-03-01 23:04:25.000000 lisaanalysistools-1.0.3/lisatools/sources/emri/__init__.py
--rw-r--r--   0 mlkatz1    (502) staff       (20)     2297 2024-03-05 21:50:21.000000 lisaanalysistools-1.0.3/lisatools/sources/emri/tdiwaveform.py
--rw-r--r--   0 mlkatz1    (502) staff       (20)     9440 2024-03-22 19:17:23.000000 lisaanalysistools-1.0.3/lisatools/stochastic.py
-drwxr-xr-x   0 mlkatz1    (502) staff       (20)        0 2024-04-05 07:54:53.193304 lisaanalysistools-1.0.3/lisatools/utils/
--rw-r--r--   0 mlkatz1    (502) staff       (20)        0 2023-05-16 15:40:56.000000 lisaanalysistools-1.0.3/lisatools/utils/__init__.py
--rw-r--r--   0 mlkatz1    (502) staff       (20)     1354 2024-03-22 19:17:23.000000 lisaanalysistools-1.0.3/lisatools/utils/constants.py
--rw-r--r--   0 mlkatz1    (502) staff       (20)    33765 2023-10-25 21:01:10.000000 lisaanalysistools-1.0.3/lisatools/utils/multigpudataholder.py
--rw-r--r--   0 mlkatz1    (502) staff       (20)     2995 2024-03-22 19:17:23.000000 lisaanalysistools-1.0.3/lisatools/utils/pointeradjust.py
--rw-r--r--   0 mlkatz1    (502) staff       (20)     6742 2024-03-22 19:17:23.000000 lisaanalysistools-1.0.3/lisatools/utils/utility.py
--rw-r--r--   0 mlkatz1    (502) staff       (20)      667 2024-04-05 07:51:18.000000 lisaanalysistools-1.0.3/pyproject.toml
--rw-r--r--   0 mlkatz1    (502) staff       (20)       30 2024-03-22 19:17:23.000000 lisaanalysistools-1.0.3/requirements-data.txt
--rw-r--r--   0 mlkatz1    (502) staff       (20)       15 2024-03-22 19:17:23.000000 lisaanalysistools-1.0.3/requirements-demo.txt
--rw-r--r--   0 mlkatz1    (502) staff       (20)      263 2024-03-22 19:17:23.000000 lisaanalysistools-1.0.3/requirements-dev.txt
--rw-r--r--   0 mlkatz1    (502) staff       (20)       33 2024-03-22 19:17:23.000000 lisaanalysistools-1.0.3/requirements-release.txt
--rw-r--r--   0 mlkatz1    (502) staff       (20)      143 2024-03-22 19:17:23.000000 lisaanalysistools-1.0.3/requirements.txt
-drwxr-xr-x   0 mlkatz1    (502) staff       (20)        0 2024-04-05 07:54:53.201184 lisaanalysistools-1.0.3/scripts/
--rw-r--r--   0 mlkatz1    (502) staff       (20)     1578 2024-03-22 19:17:23.000000 lisaanalysistools-1.0.3/scripts/data_download.py
--rwxr-xr-x   0 mlkatz1    (502) staff       (20)      819 2024-03-22 19:17:23.000000 lisaanalysistools-1.0.3/scripts/generate-changelog.bash
--rwxr-xr-x   0 mlkatz1    (502) staff       (20)      279 2024-03-22 19:17:23.000000 lisaanalysistools-1.0.3/scripts/install-hooks.bash
--rwxr-xr-x   0 mlkatz1    (502) staff       (20)       55 2024-03-22 19:17:23.000000 lisaanalysistools-1.0.3/scripts/post-commit.bash
--rwxr-xr-x   0 mlkatz1    (502) staff       (20)     1253 2024-03-22 19:17:23.000000 lisaanalysistools-1.0.3/scripts/run-tests.bash
--rwxr-xr-x   0 mlkatz1    (502) staff       (20)     1242 2024-03-22 19:17:23.000000 lisaanalysistools-1.0.3/scripts/to_conda.bash
--rw-r--r--   0 mlkatz1    (502) staff       (20)       38 2024-04-05 07:54:53.212303 lisaanalysistools-1.0.3/setup.cfg
--rw-r--r--   0 mlkatz1    (502) staff       (20)     2756 2024-03-27 20:31:21.000000 lisaanalysistools-1.0.3/setup.py
-drwxr-xr-x   0 mlkatz1    (502) staff       (20)        0 2024-04-05 07:54:53.207961 lisaanalysistools-1.0.3/src/
--rw-r--r--   0 mlkatz1    (502) staff       (20)     3857 2024-03-22 19:17:23.000000 lisaanalysistools-1.0.3/src/Detector.cpp
--rw-r--r--   0 mlkatz1    (502) staff       (20)   636410 2024-04-05 07:51:47.000000 lisaanalysistools-1.0.3/src/pycppdetector.cpp
--rw-r--r--   0 mlkatz1    (502) staff       (20)     5100 2024-03-22 19:17:23.000000 lisaanalysistools-1.0.3/src/pycppdetector.pyx
+drwxr-xr-x   0 mlkatz1    (502) staff       (20)        0 2024-04-06 01:31:17.627090 lisaanalysistools-1.0.4/
+-rw-r--r--   0 mlkatz1    (502) staff       (20)        0 2024-03-22 19:17:22.000000 lisaanalysistools-1.0.4/CHANGELOG
+-rw-r--r--   0 mlkatz1    (502) staff       (20)    11357 2024-03-22 19:17:22.000000 lisaanalysistools-1.0.4/LICENSE
+drwxr-xr-x   0 mlkatz1    (502) staff       (20)        0 2024-04-06 01:31:17.625256 lisaanalysistools-1.0.4/LISAanalysistools.egg-info/
+-rw-r--r--   0 mlkatz1    (502) staff       (20)     3380 2024-04-06 01:31:17.000000 lisaanalysistools-1.0.4/LISAanalysistools.egg-info/PKG-INFO
+-rw-r--r--   0 mlkatz1    (502) staff       (20)     1802 2024-04-06 01:31:17.000000 lisaanalysistools-1.0.4/LISAanalysistools.egg-info/SOURCES.txt
+-rw-r--r--   0 mlkatz1    (502) staff       (20)        1 2024-04-06 01:31:17.000000 lisaanalysistools-1.0.4/LISAanalysistools.egg-info/dependency_links.txt
+-rw-r--r--   0 mlkatz1    (502) staff       (20)        1 2024-03-13 23:07:52.000000 lisaanalysistools-1.0.4/LISAanalysistools.egg-info/not-zip-safe
+-rw-r--r--   0 mlkatz1    (502) staff       (20)       14 2024-04-06 01:31:17.000000 lisaanalysistools-1.0.4/LISAanalysistools.egg-info/top_level.txt
+-rw-r--r--   0 mlkatz1    (502) staff       (20)      451 2024-03-22 19:17:22.000000 lisaanalysistools-1.0.4/MANIFEST.in
+-rw-r--r--   0 mlkatz1    (502) staff       (20)     4756 2024-03-22 19:17:22.000000 lisaanalysistools-1.0.4/Makefile
+-rw-r--r--   0 mlkatz1    (502) staff       (20)     3380 2024-04-06 01:31:17.626357 lisaanalysistools-1.0.4/PKG-INFO
+-rw-r--r--   0 mlkatz1    (502) staff       (20)     2783 2024-04-06 01:10:31.000000 lisaanalysistools-1.0.4/README.md
+drwxr-xr-x   0 mlkatz1    (502) staff       (20)        0 2024-04-06 01:31:17.570677 lisaanalysistools-1.0.4/include/
+-rw-r--r--   0 mlkatz1    (502) staff       (20)     1694 2024-03-22 19:17:23.000000 lisaanalysistools-1.0.4/include/Detector.hpp
+drwxr-xr-x   0 mlkatz1    (502) staff       (20)        0 2024-04-06 01:31:17.581110 lisaanalysistools-1.0.4/lisatools/
+-rw-r--r--   0 mlkatz1    (502) staff       (20)        0 2023-05-16 15:40:56.000000 lisaanalysistools-1.0.4/lisatools/__init__.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)      123 2024-04-06 01:31:17.000000 lisaanalysistools-1.0.4/lisatools/_version.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)    15321 2024-04-06 01:04:36.000000 lisaanalysistools-1.0.4/lisatools/analysiscontainer.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)     9187 2024-04-06 01:14:58.000000 lisaanalysistools-1.0.4/lisatools/datacontainer.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)    13852 2024-04-02 17:24:55.000000 lisaanalysistools-1.0.4/lisatools/detector.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)    34174 2024-04-06 01:05:28.000000 lisaanalysistools-1.0.4/lisatools/diagnostic.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)     5154 2024-02-20 21:17:07.000000 lisaanalysistools-1.0.4/lisatools/glitch.py
+drwxr-xr-x   0 mlkatz1    (502) staff       (20)        0 2024-04-06 01:31:17.585071 lisaanalysistools-1.0.4/lisatools/sampling/
+-rw-r--r--   0 mlkatz1    (502) staff       (20)        0 2023-05-16 15:40:56.000000 lisaanalysistools-1.0.4/lisatools/sampling/__init__.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)    29585 2024-03-22 19:17:23.000000 lisaanalysistools-1.0.4/lisatools/sampling/likelihood.py
+drwxr-xr-x   0 mlkatz1    (502) staff       (20)        0 2024-04-06 01:31:17.598911 lisaanalysistools-1.0.4/lisatools/sampling/moves/
+-rw-r--r--   0 mlkatz1    (502) staff       (20)        0 2023-05-16 15:40:56.000000 lisaanalysistools-1.0.4/lisatools/sampling/moves/__init__.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)     1220 2023-06-08 00:14:36.000000 lisaanalysistools-1.0.4/lisatools/sampling/moves/gbgroupstretch.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)    51802 2024-01-25 22:07:16.000000 lisaanalysistools-1.0.4/lisatools/sampling/moves/gbmultipletryrj.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)    31152 2024-01-25 22:07:16.000000 lisaanalysistools-1.0.4/lisatools/sampling/moves/gbspecialgroupstretch.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)    90189 2024-01-25 22:07:16.000000 lisaanalysistools-1.0.4/lisatools/sampling/moves/gbspecialstretch.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)    14163 2023-10-25 21:01:10.000000 lisaanalysistools-1.0.4/lisatools/sampling/moves/mbhspecialmove.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)      469 2023-06-08 00:14:36.000000 lisaanalysistools-1.0.4/lisatools/sampling/moves/placeholder.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)     3348 2024-03-22 19:17:23.000000 lisaanalysistools-1.0.4/lisatools/sampling/moves/skymodehop.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)    25092 2024-01-25 22:07:16.000000 lisaanalysistools-1.0.4/lisatools/sampling/moves/specialforegroundmove.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)    21407 2024-04-06 01:06:43.000000 lisaanalysistools-1.0.4/lisatools/sampling/prior.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)     9682 2024-03-22 19:17:23.000000 lisaanalysistools-1.0.4/lisatools/sampling/stopping.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)    14340 2024-03-22 19:17:23.000000 lisaanalysistools-1.0.4/lisatools/sampling/utility.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)    27263 2024-04-06 01:17:33.000000 lisaanalysistools-1.0.4/lisatools/sensitivity.py
+drwxr-xr-x   0 mlkatz1    (502) staff       (20)        0 2024-04-06 01:31:17.600301 lisaanalysistools-1.0.4/lisatools/sources/
+-rw-r--r--   0 mlkatz1    (502) staff       (20)        0 2024-03-01 22:45:54.000000 lisaanalysistools-1.0.4/lisatools/sources/__init__.py
+drwxr-xr-x   0 mlkatz1    (502) staff       (20)        0 2024-04-06 01:31:17.602710 lisaanalysistools-1.0.4/lisatools/sources/emri/
+-rw-r--r--   0 mlkatz1    (502) staff       (20)       41 2024-03-01 23:04:25.000000 lisaanalysistools-1.0.4/lisatools/sources/emri/__init__.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)     2297 2024-03-05 21:50:21.000000 lisaanalysistools-1.0.4/lisatools/sources/emri/tdiwaveform.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)     9421 2024-04-06 01:09:31.000000 lisaanalysistools-1.0.4/lisatools/stochastic.py
+drwxr-xr-x   0 mlkatz1    (502) staff       (20)        0 2024-04-06 01:31:17.609850 lisaanalysistools-1.0.4/lisatools/utils/
+-rw-r--r--   0 mlkatz1    (502) staff       (20)        0 2023-05-16 15:40:56.000000 lisaanalysistools-1.0.4/lisatools/utils/__init__.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)     1354 2024-03-22 19:17:23.000000 lisaanalysistools-1.0.4/lisatools/utils/constants.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)    33765 2023-10-25 21:01:10.000000 lisaanalysistools-1.0.4/lisatools/utils/multigpudataholder.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)     2995 2024-03-22 19:17:23.000000 lisaanalysistools-1.0.4/lisatools/utils/pointeradjust.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)     6831 2024-04-06 00:53:22.000000 lisaanalysistools-1.0.4/lisatools/utils/utility.py
+-rw-r--r--   0 mlkatz1    (502) staff       (20)      667 2024-04-06 01:10:06.000000 lisaanalysistools-1.0.4/pyproject.toml
+-rw-r--r--   0 mlkatz1    (502) staff       (20)       30 2024-03-22 19:17:23.000000 lisaanalysistools-1.0.4/requirements-data.txt
+-rw-r--r--   0 mlkatz1    (502) staff       (20)       15 2024-03-22 19:17:23.000000 lisaanalysistools-1.0.4/requirements-demo.txt
+-rw-r--r--   0 mlkatz1    (502) staff       (20)      263 2024-03-22 19:17:23.000000 lisaanalysistools-1.0.4/requirements-dev.txt
+-rw-r--r--   0 mlkatz1    (502) staff       (20)       33 2024-03-22 19:17:23.000000 lisaanalysistools-1.0.4/requirements-release.txt
+-rw-r--r--   0 mlkatz1    (502) staff       (20)      143 2024-03-22 19:17:23.000000 lisaanalysistools-1.0.4/requirements.txt
+drwxr-xr-x   0 mlkatz1    (502) staff       (20)        0 2024-04-06 01:31:17.616210 lisaanalysistools-1.0.4/scripts/
+-rw-r--r--   0 mlkatz1    (502) staff       (20)     1578 2024-03-22 19:17:23.000000 lisaanalysistools-1.0.4/scripts/data_download.py
+-rwxr-xr-x   0 mlkatz1    (502) staff       (20)      819 2024-03-22 19:17:23.000000 lisaanalysistools-1.0.4/scripts/generate-changelog.bash
+-rwxr-xr-x   0 mlkatz1    (502) staff       (20)      279 2024-03-22 19:17:23.000000 lisaanalysistools-1.0.4/scripts/install-hooks.bash
+-rwxr-xr-x   0 mlkatz1    (502) staff       (20)       55 2024-03-22 19:17:23.000000 lisaanalysistools-1.0.4/scripts/post-commit.bash
+-rwxr-xr-x   0 mlkatz1    (502) staff       (20)     1253 2024-03-22 19:17:23.000000 lisaanalysistools-1.0.4/scripts/run-tests.bash
+-rwxr-xr-x   0 mlkatz1    (502) staff       (20)     1242 2024-03-22 19:17:23.000000 lisaanalysistools-1.0.4/scripts/to_conda.bash
+-rw-r--r--   0 mlkatz1    (502) staff       (20)       38 2024-04-06 01:31:17.627241 lisaanalysistools-1.0.4/setup.cfg
+-rw-r--r--   0 mlkatz1    (502) staff       (20)     2756 2024-03-27 20:31:21.000000 lisaanalysistools-1.0.4/setup.py
+drwxr-xr-x   0 mlkatz1    (502) staff       (20)        0 2024-04-06 01:31:17.623636 lisaanalysistools-1.0.4/src/
+-rw-r--r--   0 mlkatz1    (502) staff       (20)     3857 2024-03-22 19:17:23.000000 lisaanalysistools-1.0.4/src/Detector.cpp
+-rw-r--r--   0 mlkatz1    (502) staff       (20)   636410 2024-04-06 01:29:48.000000 lisaanalysistools-1.0.4/src/pycppdetector.cpp
+-rw-r--r--   0 mlkatz1    (502) staff       (20)     5100 2024-03-22 19:17:23.000000 lisaanalysistools-1.0.4/src/pycppdetector.pyx
```

### Comparing `lisaanalysistools-1.0.3/LICENSE` & `lisaanalysistools-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `lisaanalysistools-1.0.3/LISAanalysistools.egg-info/PKG-INFO` & `lisaanalysistools-1.0.4/LISAanalysistools.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lisaanalysistools
-Version: 1.0.3
+Version: 1.0.4
 Home-page: https://github.com/mikekatz04/lisa-on-gpu
 Author: Michael Katz
 Author-email: mikekatz04@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Environment :: GPU :: NVIDIA CUDA
 Classifier: Natural Language :: English
@@ -14,16 +14,17 @@
 Requires-Python: >=3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # LISA Analysis Tools
 
 [![Doc badge](https://img.shields.io/badge/Docs-master-brightgreen)](https://mikekatz04.github.io/LISAanalysistools)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.10930980.svg)](https://doi.org/10.5281/zenodo.10930980)
 
-LISA Analysis Tools is a package for performing LISA Data Analysis tasks, including building the LISA Global Fit. 
+LISA Analysis Tools is a package for performing LISA Data Analysis tasks, including building the LISA Global Fit.  
 
 ## 1 - Getting Started
 
 These instructions will get you a copy of the project up and running on your local machine,
 either for development and testing purposes or as an installed package.  For more information, see the documentation at https://mikekatz04.github.io/LISAanalysistools.
 
 # Installation
@@ -55,26 +56,40 @@
 
 Please read [CONTRIBUTING.md](CONTRIBUTING.md) for details on our code of conduct, and the process for submitting pull requests to us.
 
 ## Versioning
 
 We use [SemVer](http://semver.org/) for versioning. For the versions available, see the [tags on this repository](https://github.com/BlackHolePerturbationToolkit/FastEMRIWaveforms/tags).
 
-Current Version: 1.0.3
+Current Version: 1.0.4
 
 ## Authors/Developers
 
 * **Michael Katz**
-
-### Contibutors
-
 * Lorenzo Speri
 * Christian Chapman-Bird
+* Natalia Korsakova
+* Nikos Karnesis
 
 ## License
 
 This project is licensed under the Apache License - see the [LICENSE.md](LICENSE.md) file for details.
 
 ## Citation
 
-TODO.
+```
+@software{michael_katz_2024_10930980,
+  author       = {Michael Katz and
+                  CChapmanbird and
+                  Lorenzo Speri and
+                  Nikolaos Karnesis and
+                  Korsakova, Natalia},
+  title        = {mikekatz04/LISAanalysistools: First main release.},
+  month        = apr,
+  year         = 2024,
+  publisher    = {Zenodo},
+  version      = {v1.0.3},
+  doi          = {10.5281/zenodo.10930980},
+  url          = {https://doi.org/10.5281/zenodo.10930980}
+}
+```
```

### Comparing `lisaanalysistools-1.0.3/LISAanalysistools.egg-info/SOURCES.txt` & `lisaanalysistools-1.0.4/LISAanalysistools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lisaanalysistools-1.0.3/Makefile` & `lisaanalysistools-1.0.4/Makefile`

 * *Files identical despite different names*

### Comparing `lisaanalysistools-1.0.3/PKG-INFO` & `lisaanalysistools-1.0.4/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lisaanalysistools
-Version: 1.0.3
+Version: 1.0.4
 Home-page: https://github.com/mikekatz04/lisa-on-gpu
 Author: Michael Katz
 Author-email: mikekatz04@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Environment :: GPU :: NVIDIA CUDA
 Classifier: Natural Language :: English
@@ -14,16 +14,17 @@
 Requires-Python: >=3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # LISA Analysis Tools
 
 [![Doc badge](https://img.shields.io/badge/Docs-master-brightgreen)](https://mikekatz04.github.io/LISAanalysistools)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.10930980.svg)](https://doi.org/10.5281/zenodo.10930980)
 
-LISA Analysis Tools is a package for performing LISA Data Analysis tasks, including building the LISA Global Fit. 
+LISA Analysis Tools is a package for performing LISA Data Analysis tasks, including building the LISA Global Fit.  
 
 ## 1 - Getting Started
 
 These instructions will get you a copy of the project up and running on your local machine,
 either for development and testing purposes or as an installed package.  For more information, see the documentation at https://mikekatz04.github.io/LISAanalysistools.
 
 # Installation
@@ -55,26 +56,40 @@
 
 Please read [CONTRIBUTING.md](CONTRIBUTING.md) for details on our code of conduct, and the process for submitting pull requests to us.
 
 ## Versioning
 
 We use [SemVer](http://semver.org/) for versioning. For the versions available, see the [tags on this repository](https://github.com/BlackHolePerturbationToolkit/FastEMRIWaveforms/tags).
 
-Current Version: 1.0.3
+Current Version: 1.0.4
 
 ## Authors/Developers
 
 * **Michael Katz**
-
-### Contibutors
-
 * Lorenzo Speri
 * Christian Chapman-Bird
+* Natalia Korsakova
+* Nikos Karnesis
 
 ## License
 
 This project is licensed under the Apache License - see the [LICENSE.md](LICENSE.md) file for details.
 
 ## Citation
 
-TODO.
+```
+@software{michael_katz_2024_10930980,
+  author       = {Michael Katz and
+                  CChapmanbird and
+                  Lorenzo Speri and
+                  Nikolaos Karnesis and
+                  Korsakova, Natalia},
+  title        = {mikekatz04/LISAanalysistools: First main release.},
+  month        = apr,
+  year         = 2024,
+  publisher    = {Zenodo},
+  version      = {v1.0.3},
+  doi          = {10.5281/zenodo.10930980},
+  url          = {https://doi.org/10.5281/zenodo.10930980}
+}
+```
```

### Comparing `lisaanalysistools-1.0.3/README.md` & `lisaanalysistools-1.0.4/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # LISA Analysis Tools
 
 [![Doc badge](https://img.shields.io/badge/Docs-master-brightgreen)](https://mikekatz04.github.io/LISAanalysistools)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.10930980.svg)](https://doi.org/10.5281/zenodo.10930980)
 
-LISA Analysis Tools is a package for performing LISA Data Analysis tasks, including building the LISA Global Fit. 
+LISA Analysis Tools is a package for performing LISA Data Analysis tasks, including building the LISA Global Fit.  
 
 ## 1 - Getting Started
 
 These instructions will get you a copy of the project up and running on your local machine,
 either for development and testing purposes or as an installed package.  For more information, see the documentation at https://mikekatz04.github.io/LISAanalysistools.
 
 # Installation
@@ -38,26 +39,40 @@
 
 Please read [CONTRIBUTING.md](CONTRIBUTING.md) for details on our code of conduct, and the process for submitting pull requests to us.
 
 ## Versioning
 
 We use [SemVer](http://semver.org/) for versioning. For the versions available, see the [tags on this repository](https://github.com/BlackHolePerturbationToolkit/FastEMRIWaveforms/tags).
 
-Current Version: 1.0.3
+Current Version: 1.0.4
 
 ## Authors/Developers
 
 * **Michael Katz**
-
-### Contibutors
-
 * Lorenzo Speri
 * Christian Chapman-Bird
+* Natalia Korsakova
+* Nikos Karnesis
 
 ## License
 
 This project is licensed under the Apache License - see the [LICENSE.md](LICENSE.md) file for details.
 
 ## Citation
 
-TODO.
+```
+@software{michael_katz_2024_10930980,
+  author       = {Michael Katz and
+                  CChapmanbird and
+                  Lorenzo Speri and
+                  Nikolaos Karnesis and
+                  Korsakova, Natalia},
+  title        = {mikekatz04/LISAanalysistools: First main release.},
+  month        = apr,
+  year         = 2024,
+  publisher    = {Zenodo},
+  version      = {v1.0.3},
+  doi          = {10.5281/zenodo.10930980},
+  url          = {https://doi.org/10.5281/zenodo.10930980}
+}
+```
```

### Comparing `lisaanalysistools-1.0.3/include/Detector.hpp` & `lisaanalysistools-1.0.4/include/Detector.hpp`

 * *Files identical despite different names*

### Comparing `lisaanalysistools-1.0.3/lisatools/analysiscontainer.py` & `lisaanalysistools-1.0.4/lisatools/analysiscontainer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,21 @@
+from __future__ import annotations
+
+
 import warnings
 from abc import ABC
 from typing import Any, Tuple, Optional, List
 
 import math
 import numpy as np
-from numpy.typing import ArrayLike
+
 from scipy import interpolate
 import matplotlib.pyplot as plt
 
+
 try:
     import cupy as cp
 
 except (ModuleNotFoundError, ImportError):
     import numpy as cp
 
 from . import detector as lisa_models
@@ -205,15 +209,15 @@
         return (opt_snr, det_snr)
 
     def template_likelihood(
         self,
         template: DataResidualArray,
         include_psd_info: bool = False,
         phase_maximize: bool = False,
-        **kwargs: dict
+        **kwargs: dict,
     ) -> float:
         """Calculate the Likelihood of a template against the data.
 
         Args:
             template: Template signal.
             include_psd_info: If ``True``, add the PSD term to the Likelihood value.
             phase_maximize: If ``True``, maximize over an overall phase.
@@ -274,19 +278,19 @@
             return residual_full_source_and_noise_likelihood(
                 self.data_res_arr, self.sens_mat, **kwargs
             )
 
     def _calculate_signal_operation(
         self,
         calc: str,
-        *args: ArrayLike,
+        *args: Any,
         source_only: bool = False,
         waveform_kwargs: Optional[dict] = {},
         data_res_arr_kwargs: Optional[dict] = {},
-        **kwargs: dict
+        **kwargs: dict,
     ) -> float | complex:
         """Return the likelihood of a generated signal with the data.
 
         Args:
             calc: Type of calculation to do. Options are ``"likelihood"``, ``"inner_product"``, or ``"snr"``.
             *args: Arguments to waveform generating function. Must include parameters.
             source_only: If ``True`` return the source-only Likelihood (leave out noise part).
@@ -324,19 +328,19 @@
         elif calc == "snr":
             return self.template_snr(*args_2, **kwargs)
         else:
             raise ValueError("`calc` must be 'likelihood', 'inner_product', or 'snr'.")
 
     def calculate_signal_likelihood(
         self,
-        *args: ArrayLike,
+        *args: Any,
         source_only: bool = False,
         waveform_kwargs: Optional[dict] = {},
         data_res_arr_kwargs: Optional[dict] = {},
-        **kwargs: dict
+        **kwargs: dict,
     ) -> float | complex:
         """Return the likelihood of a generated signal with the data.
 
         Args:
             params: Arguments to waveform generating function. Must include parameters.
             source_only: If ``True`` return the source-only Likelihood (leave out noise part).
             waveform_kwargs: Keyword arguments to pass to waveform generator.
@@ -351,24 +355,24 @@
 
         return self._calculate_signal_operation(
             "likelihood",
             *args,
             source_only=source_only,
             waveform_kwargs=waveform_kwargs,
             data_res_arr_kwargs=data_res_arr_kwargs,
-            **kwargs
+            **kwargs,
         )
 
     def calculate_signal_inner_product(
         self,
-        *args: ArrayLike,
+        *args: Any,
         source_only: bool = False,
         waveform_kwargs: Optional[dict] = {},
         data_res_arr_kwargs: Optional[dict] = {},
-        **kwargs: dict
+        **kwargs: dict,
     ) -> float | complex:
         """Return the inner product of a generated signal with the data.
 
         Args:
             *args: Arguments to waveform generating function. Must include parameters.
             source_only: If ``True`` return the source-only Likelihood (leave out noise part).
             waveform_kwargs: Keyword arguments to pass to waveform generator.
@@ -383,24 +387,24 @@
 
         return self._calculate_signal_operation(
             "inner_product",
             *args,
             source_only=source_only,
             waveform_kwargs=waveform_kwargs,
             data_res_arr_kwargs=data_res_arr_kwargs,
-            **kwargs
+            **kwargs,
         )
 
     def calculate_signal_snr(
         self,
-        *args: ArrayLike,
+        *args: Any,
         source_only: bool = False,
         waveform_kwargs: Optional[dict] = {},
         data_res_arr_kwargs: Optional[dict] = {},
-        **kwargs: dict
+        **kwargs: dict,
     ) -> Tuple[float, float]:
         """Return the SNR of a generated signal with the data.
 
         Args:
             *args: Arguments to waveform generating function. Must include parameters.
             source_only: If ``True`` return the source-only Likelihood (leave out noise part).
             waveform_kwargs: Keyword arguments to pass to waveform generator.
@@ -415,15 +419,15 @@
 
         return self._calculate_signal_operation(
             "snr",
             *args,
             source_only=source_only,
             waveform_kwargs=waveform_kwargs,
             data_res_arr_kwargs=data_res_arr_kwargs,
-            **kwargs
+            **kwargs,
         )
 
     def eryn_likelihood_function(self, x, *args, **kwargs):
         if x.ndim == 1:
             input_vals = tuple(x) + tuple(args)
             return self.calculate_signal_likelihood(*input_vals, **kwargs)
         elif x.ndim == 2:
```

### Comparing `lisaanalysistools-1.0.3/lisatools/datacontainer.py` & `lisaanalysistools-1.0.4/lisatools/datacontainer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import warnings
 from abc import ABC
 from typing import Any, Tuple, Optional, List
 
 import math
 import numpy as np
-from numpy.typing import ArrayLike
 from scipy import interpolate
 import matplotlib.pyplot as plt
 
 try:
     import cupy as cp
 
 except (ModuleNotFoundError, ImportError):
@@ -32,15 +31,15 @@
     """Container to hold sensitivity information.
 
     Args:
         f: Frequency array.
         sens_mat: Input sensitivity list. The shape of the nested lists should represent the shape of the
             desired matrix. Each entry in the list must be an array, :class:`Sensitivity`-derived object,
             or a string corresponding to the :class:`Sensitivity` object.
-        **sens_kwargs: Keyword arguments to pass to :method:`Sensitivity.get_Sn`.
+        **sens_kwargs: Keyword arguments to pass to :func:`Sensitivity.get_Sn`.
 
     """
 
     def __init__(
         self,
         data_res_in: List[np.ndarray] | np.ndarray | DataResidualArray,
         dt: Optional[float] = None,
```

### Comparing `lisaanalysistools-1.0.3/lisatools/detector.py` & `lisaanalysistools-1.0.4/lisatools/detector.py`

 * *Files identical despite different names*

### Comparing `lisaanalysistools-1.0.3/lisatools/diagnostic.py` & `lisaanalysistools-1.0.4/lisatools/diagnostic.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import warnings
 from types import ModuleType, NoneType
 from typing import Optional, Any, Tuple, List
 
-from numpy.typing import ArrayLike
 import matplotlib.pyplot as plt
 
 from eryn.utils import TransformContainer
 
 import numpy as np
 
 try:
@@ -383,15 +382,15 @@
         det_snr = inner_product(sig1, data, *args, **kwargs).real / opt_snr
         return det_snr
 
 
 def h_var_p_eps(
     step: float,
     waveform_model: callable,
-    params: ArrayLike,
+    params: np.ndarray | list,
     index: int,
     parameter_transforms: Optional[TransformContainer] = None,
     waveform_args: Optional[tuple] = (),
     waveform_kwargs: Optional[dict] = {},
 ) -> np.ndarray:  # TODO: check this
     """Calculate the waveform with a perturbation step of the variable V[i]
 
@@ -495,16 +494,16 @@
 
     return dh_I
 
 
 def info_matrix(
     eps: float | np.ndarray,
     waveform_model: callable,
-    params: ArrayLike,
-    deriv_inds: Optional[ArrayLike] = None,
+    params: np.ndarray | list,
+    deriv_inds: Optional[np.ndarray | list] = None,
     inner_product_kwargs: Optional[dict] = {},
     return_derivs: Optional[bool] = False,
     **kwargs: dict,
 ) -> np.ndarray | Tuple[np.ndarray, list]:
     """Calculate Information Matrix.
 
     This calculates the information matrix for a given waveform model at a given set of parameters.
@@ -789,15 +788,15 @@
 def cutler_vallisneri_bias(
     waveform_model_true: callable,
     waveform_model_approx: callable,
     params: np.ndarray,
     eps: float | np.ndarray,
     input_diagnostics: Optional[dict] = None,
     info_mat: Optional[np.ndarray] = None,
-    deriv_inds: Optional[ArrayLike] = None,
+    deriv_inds: Optional[np.ndarray | list] = None,
     return_derivs: Optional[bool] = False,
     return_cov: Optional[bool] = False,
     parameter_transforms: Optional[TransformContainer] = None,
     waveform_true_args: Optional[tuple] = (),
     waveform_true_kwargs: Optional[dict] = {},
     waveform_approx_args: Optional[tuple] = (),
     waveform_approx_kwargs: Optional[dict] = {},
```

### Comparing `lisaanalysistools-1.0.3/lisatools/glitch.py` & `lisaanalysistools-1.0.4/lisatools/glitch.py`

 * *Files identical despite different names*

### Comparing `lisaanalysistools-1.0.3/lisatools/sampling/likelihood.py` & `lisaanalysistools-1.0.4/lisatools/sampling/likelihood.py`

 * *Files identical despite different names*

### Comparing `lisaanalysistools-1.0.3/lisatools/sampling/moves/gbgroupstretch.py` & `lisaanalysistools-1.0.4/lisatools/sampling/moves/gbgroupstretch.py`

 * *Files identical despite different names*

### Comparing `lisaanalysistools-1.0.3/lisatools/sampling/moves/gbmultipletryrj.py` & `lisaanalysistools-1.0.4/lisatools/sampling/moves/gbmultipletryrj.py`

 * *Files identical despite different names*

### Comparing `lisaanalysistools-1.0.3/lisatools/sampling/moves/gbspecialgroupstretch.py` & `lisaanalysistools-1.0.4/lisatools/sampling/moves/gbspecialgroupstretch.py`

 * *Files identical despite different names*

### Comparing `lisaanalysistools-1.0.3/lisatools/sampling/moves/gbspecialstretch.py` & `lisaanalysistools-1.0.4/lisatools/sampling/moves/gbspecialstretch.py`

 * *Files identical despite different names*

### Comparing `lisaanalysistools-1.0.3/lisatools/sampling/moves/mbhspecialmove.py` & `lisaanalysistools-1.0.4/lisatools/sampling/moves/mbhspecialmove.py`

 * *Files identical despite different names*

### Comparing `lisaanalysistools-1.0.3/lisatools/sampling/moves/skymodehop.py` & `lisaanalysistools-1.0.4/lisatools/sampling/moves/skymodehop.py`

 * *Files identical despite different names*

### Comparing `lisaanalysistools-1.0.3/lisatools/sampling/moves/specialforegroundmove.py` & `lisaanalysistools-1.0.4/lisatools/sampling/moves/specialforegroundmove.py`

 * *Files identical despite different names*

### Comparing `lisaanalysistools-1.0.3/lisatools/sampling/stopping.py` & `lisaanalysistools-1.0.4/lisatools/sampling/stopping.py`

 * *Files identical despite different names*

### Comparing `lisaanalysistools-1.0.3/lisatools/sampling/utility.py` & `lisaanalysistools-1.0.4/lisatools/sampling/utility.py`

 * *Files identical despite different names*

### Comparing `lisaanalysistools-1.0.3/lisatools/sensitivity.py` & `lisaanalysistools-1.0.4/lisatools/sensitivity.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import warnings
 from abc import ABC
 from typing import Any, Tuple, Optional, List
 from copy import deepcopy
 
 import math
 import numpy as np
-from numpy.typing import ArrayLike
 from scipy import interpolate
 import matplotlib.pyplot as plt
 
 try:
     import cupy as cp
 
 except (ModuleNotFoundError, ImportError):
@@ -523,25 +522,27 @@
     """Container to hold sensitivity information.
 
     Args:
         f: Frequency array.
         sens_mat: Input sensitivity list. The shape of the nested lists should represent the shape of the
             desired matrix. Each entry in the list must be an array, :class:`Sensitivity`-derived object,
             or a string corresponding to the :class:`Sensitivity` object.
-        **sens_kwargs: Keyword arguments to pass to :method:`Sensitivity.get_Sn`.
+        **sens_kwargs: Keyword arguments to pass to :func:`Sensitivity.get_Sn`.
 
     """
 
     def __init__(
         self,
         f: np.ndarray,
-        sens_mat: List[List[np.ndarray | Sensitivity]]
-        | List[np.ndarray | Sensitivity]
-        | np.ndarray
-        | Sensitivity,
+        sens_mat: (
+            List[List[np.ndarray | Sensitivity]]
+            | List[np.ndarray | Sensitivity]
+            | np.ndarray
+            | Sensitivity
+        ),
         *sens_args: tuple,
         **sens_kwargs: dict,
     ) -> None:
         self.frequency_arr = f
         self.data_length = len(self.frequency_arr)
         self.sens_args = sens_args
         self.sens_kwargs = sens_kwargs
@@ -594,18 +595,20 @@
     def sens_mat(self) -> np.ndarray:
         """Get sensitivity matrix."""
         return self._sens_mat
 
     @sens_mat.setter
     def sens_mat(
         self,
-        sens_mat: List[List[np.ndarray | Sensitivity]]
-        | List[np.ndarray | Sensitivity]
-        | np.ndarray
-        | Sensitivity,
+        sens_mat: (
+            List[List[np.ndarray | Sensitivity]]
+            | List[np.ndarray | Sensitivity]
+            | np.ndarray
+            | Sensitivity
+        ),
     ) -> None:
         """Set sensitivity matrix."""
         self.sens_mat_input = deepcopy(sens_mat)
         self._sens_mat = np.asarray(sens_mat, dtype=object)
 
         # not an
         new_out = np.full(len(self._sens_mat.flatten()), None, dtype=object)
@@ -725,15 +728,15 @@
 class XYZ1SensitivityMatrix(SensitivityMatrix):
     """Default sensitivity matrix for XYZ (TDI 1)
 
     This is 3x3 symmetric matrix.
 
     Args:
         f: Frequency array.
-        **sens_kwargs: Keyword arguments to pass to :method:`Sensitivity.get_Sn`.
+        **sens_kwargs: Keyword arguments to pass to :func:`Sensitivity.get_Sn`.
 
     """
 
     def __init__(self, f: np.ndarray, **sens_kwargs: dict) -> None:
         sens_mat = [
             [X1TDISens, XY1TDISens, ZX1TDISens],
             [XY1TDISens, Y1TDISens, YZ1TDISens],
@@ -745,44 +748,44 @@
 class AET1SensitivityMatrix(SensitivityMatrix):
     """Default sensitivity matrix for AET (TDI 1)
 
     This is just an array because no cross-terms.
 
     Args:
         f: Frequency array.
-        **sens_kwargs: Keyword arguments to pass to :method:`Sensitivity.get_Sn`.
+        **sens_kwargs: Keyword arguments to pass to :func:`Sensitivity.get_Sn`.
 
     """
 
     def __init__(self, f: np.ndarray, **sens_kwargs: dict) -> None:
         sens_mat = [A1TDISens, E1TDISens, T1TDISens]
         super().__init__(f, sens_mat, **sens_kwargs)
 
 
 class AE1SensitivityMatrix(SensitivityMatrix):
     """Default sensitivity matrix for AE (no T) (TDI 1)
 
     Args:
         f: Frequency array.
-        **sens_kwargs: Keyword arguments to pass to :method:`Sensitivity.get_Sn`.
+        **sens_kwargs: Keyword arguments to pass to :func:`Sensitivity.get_Sn`.
 
     """
 
     def __init__(self, f: np.ndarray, **sens_kwargs: dict) -> None:
         sens_mat = [A1TDISens, E1TDISens]
         super().__init__(f, sens_mat, **sens_kwargs)
 
 
 class LISASensSensitivityMatrix(SensitivityMatrix):
     """Default sensitivity matrix adding :class:`LISASens` for the specified number of channels.
 
     Args:
         f: Frequency array.
         nchannels: Number of channels.
-        **sens_kwargs: Keyword arguments to pass to :method:`Sensitivity.get_Sn`.
+        **sens_kwargs: Keyword arguments to pass to :func:`Sensitivity.get_Sn`.
 
     """
 
     def __init__(self, f: np.ndarray, nchannels: int, **sens_kwargs: dict) -> None:
         sens_mat = [LISASens for _ in range(nchannels)]
         super().__init__(f, sens_mat, **sens_kwargs)
```

### Comparing `lisaanalysistools-1.0.3/lisatools/sources/emri/tdiwaveform.py` & `lisaanalysistools-1.0.4/lisatools/sources/emri/tdiwaveform.py`

 * *Files identical despite different names*

### Comparing `lisaanalysistools-1.0.3/lisatools/stochastic.py` & `lisaanalysistools-1.0.4/lisatools/stochastic.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import warnings
 from abc import ABC
 from typing import Any, Tuple, Optional, List, Dict
 
 import math
 import numpy as np
-from numpy.typing import ArrayLike
 from scipy import interpolate
 
 try:
     import cupy as cp
 
 except (ModuleNotFoundError, ImportError):
     import numpy as cp
@@ -21,15 +20,15 @@
 class StochasticContribution(ABC):
     """Base Class for Stochastic Contributions to the PSD."""
 
     ndim = None
     added_stochastic_list = []
 
     @classmethod
-    def _check_ndim(cls, params: ArrayLike) -> None:
+    def _check_ndim(cls, params: np.ndarray | list) -> None:
         """Check the dimensionality of the parameters matches the model.
 
         Args:
             params: Parameters for stochastic model.
 
         """
         if cls.ndim is None:
@@ -38,15 +37,15 @@
             )
 
         if len(params) != cls.ndim:
             raise ValueError("length of parameters is not equivalent to class ndim.")
 
     @classmethod
     def get_Sh(
-        cls, f: float | np.ndarray, *params: ArrayLike, **kwargs: Any
+        cls, f: float | np.ndarray, *params: np.ndarray | list, **kwargs: Any
     ) -> float | np.ndarray:
         """Calculate the power spectral density of the stochastic contribution.
 
         Args:
             f: Frequency array.
             *params: Parameters for the stochastic model.
             **kwargs: Keyword arguments for the stochastic model.
```

### Comparing `lisaanalysistools-1.0.3/lisatools/utils/constants.py` & `lisaanalysistools-1.0.4/lisatools/utils/constants.py`

 * *Files identical despite different names*

### Comparing `lisaanalysistools-1.0.3/lisatools/utils/multigpudataholder.py` & `lisaanalysistools-1.0.4/lisatools/utils/multigpudataholder.py`

 * *Files identical despite different names*

### Comparing `lisaanalysistools-1.0.3/lisatools/utils/pointeradjust.py` & `lisaanalysistools-1.0.4/lisatools/utils/pointeradjust.py`

 * *Files identical despite different names*

### Comparing `lisaanalysistools-1.0.3/lisatools/utils/utility.py` & `lisaanalysistools-1.0.4/lisatools/utils/utility.py`

 * *Files 1% similar despite different names*

```diff
@@ -222,19 +222,25 @@
             * (band_indices_sorted.flatten()[keep] % num_groups_base == i)
             for i in range(num_groups_base)
         ]
     )
     groups_even_odd = xp.sum(groups_even_odd_tmp, axis=0)
 
     groups_out = -2 * xp.ones_like(f0, dtype=int)
-    groups_out[
-        (temp_inds, walker_inds, inds_band_indices.flatten()[keep])
-    ] = groups_even_odd
+    groups_out[(temp_inds, walker_inds, inds_band_indices.flatten()[keep])] = (
+        groups_even_odd
+    )
 
     groups_out[bad] = -1
 
     """if f0_2 is not None and not np.all(keep):
         fix = (temp_inds_remove, walker_inds_remove, inds_band_indices_remove)
         fix_2 = band_indices_2[fix]
         fix_1 = band_indices[fix]"""
 
     return groups_out
+
+
+autodoc_type_aliases = {
+    "Iterable": "Iterable",
+    "ArrayLike": "ArrayLike",
+}
```

### Comparing `lisaanalysistools-1.0.3/pyproject.toml` & `lisaanalysistools-1.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 [build-system]
 requires = ["setuptools", "wheel", "Cython",  "numpy"]
 build-backend = 'setuptools.build_meta'
 
 [tool.poetry]
 name = "lisaanalysistools"
-version = "1.0.3"
+version = "1.0.4"
 description = "A package for LISA Data Analysis"
 license = "Apache"
 classifiers = ["Programming Language :: Python :: 3", "Operating System :: OS Independent"]
 homepage = "https://github.com/mikekatz04/LISAanalysistools"
 authors = ["Michael L. Katz"]
 readme = "README.md"
```

### Comparing `lisaanalysistools-1.0.3/scripts/data_download.py` & `lisaanalysistools-1.0.4/scripts/data_download.py`

 * *Files identical despite different names*

### Comparing `lisaanalysistools-1.0.3/scripts/generate-changelog.bash` & `lisaanalysistools-1.0.4/scripts/generate-changelog.bash`

 * *Files identical despite different names*

### Comparing `lisaanalysistools-1.0.3/scripts/run-tests.bash` & `lisaanalysistools-1.0.4/scripts/run-tests.bash`

 * *Files identical despite different names*

### Comparing `lisaanalysistools-1.0.3/scripts/to_conda.bash` & `lisaanalysistools-1.0.4/scripts/to_conda.bash`

 * *Files identical despite different names*

### Comparing `lisaanalysistools-1.0.3/setup.py` & `lisaanalysistools-1.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `lisaanalysistools-1.0.3/src/Detector.cpp` & `lisaanalysistools-1.0.4/src/Detector.cpp`

 * *Files identical despite different names*

### Comparing `lisaanalysistools-1.0.3/src/pycppdetector.cpp` & `lisaanalysistools-1.0.4/src/pycppdetector.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 /* Generated by Cython 3.0.10 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "/private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/core/include/numpy/arrayobject.h",
-            "/private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/core/include/numpy/arrayscalars.h",
-            "/private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/core/include/numpy/ndarrayobject.h",
-            "/private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/core/include/numpy/ndarraytypes.h",
-            "/private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/core/include/numpy/ufuncobject.h",
+            "/private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/core/include/numpy/arrayobject.h",
+            "/private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/core/include/numpy/arrayscalars.h",
+            "/private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/core/include/numpy/ndarrayobject.h",
+            "/private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/core/include/numpy/ndarraytypes.h",
+            "/private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/core/include/numpy/ufuncobject.h",
             "include/Detector.hpp"
         ],
         "include_dirs": [
             "src",
             "./include",
-            "/private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/core/include"
+            "/private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/core/include"
         ],
         "language": "c++",
         "name": "lisatools.cutils.detector",
         "sources": [
             "src/pycppdetector.pyx",
             "src/Detector.cpp"
         ]
@@ -1553,177 +1553,177 @@
 /* ForceInitThreads.proto */
 #ifndef __PYX_FORCE_INIT_THREADS
   #define __PYX_FORCE_INIT_THREADS 0
 #endif
 
 /* #### Code section: numeric_typedefs ### */
 
-/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":730
+/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":730
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":731
+/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":731
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":732
+/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":732
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":733
+/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":733
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":737
+/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":737
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":738
+/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":738
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":739
+/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":739
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":740
+/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":740
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":744
+/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":744
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":745
+/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":745
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":754
+/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":754
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":755
+/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":755
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":757
+/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":757
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":758
+/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":758
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":760
+/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":760
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":761
+/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":761
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":763
+/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":763
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":764
+/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":764
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":765
+/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":765
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1753,42 +1753,42 @@
 static CYTHON_INLINE __pyx_t_double_complex __pyx_t_double_complex_from_parts(double, double);
 
 /* #### Code section: type_declarations ### */
 
 /*--- Type declarations ---*/
 struct __pyx_obj_9lisatools_6cutils_8detector_pycppDetector;
 
-/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":767
+/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":767
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":768
+/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":768
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":769
+/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":769
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":771
+/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":771
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -3506,261 +3506,261 @@
 #define __pyx_codeobj__21 __pyx_mstate_global->__pyx_codeobj__21
 #define __pyx_codeobj__23 __pyx_mstate_global->__pyx_codeobj__23
 #define __pyx_codeobj__25 __pyx_mstate_global->__pyx_codeobj__25
 #define __pyx_codeobj__27 __pyx_mstate_global->__pyx_codeobj__27
 #define __pyx_codeobj__29 __pyx_mstate_global->__pyx_codeobj__29
 /* #### Code section: module_code ### */
 
-/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":245
+/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":245
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_7ndarray_4base_base(PyArrayObject *__pyx_v_self) {
   PyObject *__pyx_r;
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":248
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":248
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  *             return PyArray_BASE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_BASE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":245
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":245
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":251
+/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":251
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
 static CYTHON_INLINE PyArray_Descr *__pyx_f_5numpy_7ndarray_5descr_descr(PyArrayObject *__pyx_v_self) {
   PyArray_Descr *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyArray_Descr *__pyx_t_1;
   __Pyx_RefNannySetupContext("descr", 1);
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":254
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":254
  *             """Returns an owned reference to the dtype of the array.
  *             """
  *             return <dtype>PyArray_DESCR(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __Pyx_XDECREF((PyObject *)__pyx_r);
   __pyx_t_1 = PyArray_DESCR(__pyx_v_self);
   __Pyx_INCREF((PyObject *)((PyArray_Descr *)__pyx_t_1));
   __pyx_r = ((PyArray_Descr *)__pyx_t_1);
   goto __pyx_L0;
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":251
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":251
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":257
+/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":257
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_7ndarray_4ndim_ndim(PyArrayObject *__pyx_v_self) {
   int __pyx_r;
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":260
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":260
  *             """Returns the number of dimensions in the array.
  *             """
  *             return PyArray_NDIM(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_NDIM(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":257
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":257
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":263
+/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":263
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_5shape_shape(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":268
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":268
  *             Can return NULL for 0-dimensional arrays.
  *             """
  *             return PyArray_DIMS(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_DIMS(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":263
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":263
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":271
+/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":271
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_7strides_strides(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":275
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":275
  *             The number of elements matches the number of dimensions of the array (ndim).
  *             """
  *             return PyArray_STRIDES(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_STRIDES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":271
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":271
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":278
+/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":278
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
 static CYTHON_INLINE npy_intp __pyx_f_5numpy_7ndarray_4size_size(PyArrayObject *__pyx_v_self) {
   npy_intp __pyx_r;
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":281
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":281
  *             """Returns the total size (in number of elements) of the array.
  *             """
  *             return PyArray_SIZE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_SIZE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":278
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":278
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":284
+/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":284
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
 static CYTHON_INLINE char *__pyx_f_5numpy_7ndarray_4data_data(PyArrayObject *__pyx_v_self) {
   char *__pyx_r;
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":290
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":290
  *             of `PyArray_DATA()` instead, which returns a 'void*'.
  *             """
  *             return PyArray_BYTES(self)             # <<<<<<<<<<<<<<
  * 
  *     ctypedef unsigned char      npy_bool
  */
   __pyx_r = PyArray_BYTES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":284
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":284
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":773
+/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":773
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -3769,29 +3769,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 1);
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":774
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":774
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 774, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":773
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":773
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -3802,15 +3802,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":776
+/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":776
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -3819,29 +3819,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 1);
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":777
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":777
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 777, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":776
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":776
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -3852,15 +3852,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":779
+/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":779
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -3869,29 +3869,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 1);
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":780
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":780
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 780, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":779
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":779
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -3902,15 +3902,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":782
+/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":782
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -3919,29 +3919,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 1);
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":783
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":783
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 783, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":782
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":782
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -3952,15 +3952,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":785
+/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":785
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -3969,29 +3969,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 1);
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":786
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":786
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 786, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":785
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":785
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -4002,217 +4002,217 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":788
+/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":788
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 1);
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":789
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":789
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = PyDataType_HASSUBARRAY(__pyx_v_d);
   if (__pyx_t_1) {
 
-    /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":790
+    /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":790
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":789
+    /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":789
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":792
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":792
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":788
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":788
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":968
+/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":968
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":969
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":969
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":970
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":970
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   __pyx_t_1 = PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(1, 970, __pyx_L1_error)
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":968
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":968
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_AddTraceback("numpy.set_array_base", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_L0:;
 }
 
-/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":972
+/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":972
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 1);
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":973
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":973
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":974
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":974
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = (__pyx_v_base == NULL);
   if (__pyx_t_1) {
 
-    /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":975
+    /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":975
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":974
+    /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":974
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":976
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":976
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":972
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":972
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":980
+/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":980
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -4228,15 +4228,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 1);
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":981
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":981
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -4244,68 +4244,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":982
+      /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":982
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 982, __pyx_L3_error)
 
-      /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":981
+      /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":981
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":983
+    /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":983
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 983, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":984
+      /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":984
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 984, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 984, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":981
+    /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":981
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -4313,15 +4313,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":980
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":980
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -4336,15 +4336,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":986
+/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":986
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4360,15 +4360,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 1);
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":987
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":987
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -4376,68 +4376,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":988
+      /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":988
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 988, __pyx_L3_error)
 
-      /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":987
+      /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":987
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":989
+    /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":989
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 989, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":990
+      /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":990
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 990, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 990, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":987
+    /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":987
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -4445,15 +4445,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":986
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":986
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4468,15 +4468,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":992
+/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":992
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4492,15 +4492,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 1);
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":993
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":993
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -4508,68 +4508,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":994
+      /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":994
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 994, __pyx_L3_error)
 
-      /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":993
+      /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":993
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":995
+    /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":995
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 995, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":996
+      /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":996
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * 
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 996, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 996, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":993
+    /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":993
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -4577,15 +4577,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":992
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":992
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4600,170 +4600,170 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":999
+/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":999
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1011
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1011
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":999
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":999
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1014
+/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1014
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1026
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1026
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1014
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1014
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1029
+/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1029
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1036
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1036
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1029
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1029
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1039
+/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1039
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1043
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1043
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1039
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1039
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1046
+/* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1046
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1050
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1050
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1046
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1046
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -8957,26 +8957,26 @@
 }
 /* #### Code section: cached_constants ### */
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":984
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":984
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_s_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple_)) __PYX_ERR(1, 984, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple_);
   __Pyx_GIVEREF(__pyx_tuple_);
 
-  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-gm9069mo/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":990
+  /* "../../../../private/var/folders/j0/bh276m5s531565_7zdy_t5m40000gp/T/pip-build-env-ctlxm5b3/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":990
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(1, 990, __pyx_L1_error)
```

### Comparing `lisaanalysistools-1.0.3/src/pycppdetector.pyx` & `lisaanalysistools-1.0.4/src/pycppdetector.pyx`

 * *Files identical despite different names*

