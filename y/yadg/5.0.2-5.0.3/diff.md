# Comparing `tmp/yadg-5.0.2.tar.gz` & `tmp/yadg-5.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yadg-5.0.2.tar", last modified: Wed Dec 13 17:47:33 2023, max compression
+gzip compressed data, was "yadg-5.0.3.tar", last modified: Sat Apr  6 10:38:28 2024, max compression
```

## Comparing `yadg-5.0.2.tar` & `yadg-5.0.3.tar`

### file list

```diff
@@ -1,116 +1,116 @@
-drwxr-xr-x   0 kraus     (1000) kraus     (1000)        0 2023-12-13 17:47:33.362087 yadg-5.0.2/
--rw-r--r--   0 kraus     (1000) kraus     (1000)    35149 2023-09-01 17:04:55.000000 yadg-5.0.2/LICENSE
--rw-r--r--   0 kraus     (1000) kraus     (1000)       51 2023-09-01 17:04:55.000000 yadg-5.0.2/MANIFEST.in
--rw-r--r--   0 kraus     (1000) kraus     (1000)     4574 2023-12-13 17:47:33.362087 yadg-5.0.2/PKG-INFO
--rw-r--r--   0 kraus     (1000) kraus     (1000)     3281 2023-12-13 17:42:48.000000 yadg-5.0.2/README.md
--rw-r--r--   0 kraus     (1000) kraus     (1000)      199 2023-12-13 17:47:33.362087 yadg-5.0.2/setup.cfg
--rw-r--r--   0 kraus     (1000) kraus     (1000)     1704 2023-12-13 17:42:48.000000 yadg-5.0.2/setup.py
-drwxr-xr-x   0 kraus     (1000) kraus     (1000)        0 2023-12-13 17:47:33.332087 yadg-5.0.2/src/
-drwxr-xr-x   0 kraus     (1000) kraus     (1000)        0 2023-12-13 17:47:33.362087 yadg-5.0.2/src/yadg/
--rw-r--r--   0 kraus     (1000) kraus     (1000)      196 2023-09-01 17:04:55.000000 yadg-5.0.2/src/yadg/__init__.py
--rw-r--r--   0 kraus     (1000) kraus     (1000)      497 2023-12-13 17:47:33.362087 yadg-5.0.2/src/yadg/_version.py
-drwxr-xr-x   0 kraus     (1000) kraus     (1000)        0 2023-12-13 17:47:33.338754 yadg-5.0.2/src/yadg/core/
--rw-r--r--   0 kraus     (1000) kraus     (1000)     7116 2023-09-01 17:04:55.000000 yadg-5.0.2/src/yadg/core/__init__.py
-drwxr-xr-x   0 kraus     (1000) kraus     (1000)        0 2023-12-13 17:47:33.342087 yadg-5.0.2/src/yadg/dgutils/
--rw-r--r--   0 kraus     (1000) kraus     (1000)      472 2023-09-01 17:04:55.000000 yadg-5.0.2/src/yadg/dgutils/__init__.py
--rw-r--r--   0 kraus     (1000) kraus     (1000)     2198 2023-12-13 17:42:48.000000 yadg-5.0.2/src/yadg/dgutils/btools.py
--rw-r--r--   0 kraus     (1000) kraus     (1000)    13263 2023-09-01 17:04:55.000000 yadg-5.0.2/src/yadg/dgutils/dateutils.py
--rw-r--r--   0 kraus     (1000) kraus     (1000)      651 2023-09-01 17:04:55.000000 yadg-5.0.2/src/yadg/dgutils/helpers.py
--rw-r--r--   0 kraus     (1000) kraus     (1000)     2218 2023-09-01 17:04:55.000000 yadg-5.0.2/src/yadg/dgutils/pintutils.py
--rw-r--r--   0 kraus     (1000) kraus     (1000)     5897 2023-09-01 17:04:55.000000 yadg-5.0.2/src/yadg/dgutils/utils.py
-drwxr-xr-x   0 kraus     (1000) kraus     (1000)        0 2023-12-13 17:47:33.342087 yadg-5.0.2/src/yadg/extractors/
--rw-r--r--   0 kraus     (1000) kraus     (1000)     2814 2023-12-13 17:42:48.000000 yadg-5.0.2/src/yadg/extractors/__init__.py
-drwxr-xr-x   0 kraus     (1000) kraus     (1000)        0 2023-12-13 17:47:33.342087 yadg-5.0.2/src/yadg/extractors/agilentch/
--rw-r--r--   0 kraus     (1000) kraus     (1000)      158 2023-09-01 17:04:55.000000 yadg-5.0.2/src/yadg/extractors/agilentch/__init__.py
-drwxr-xr-x   0 kraus     (1000) kraus     (1000)        0 2023-12-13 17:47:33.342087 yadg-5.0.2/src/yadg/extractors/agilentdx/
--rw-r--r--   0 kraus     (1000) kraus     (1000)      158 2023-09-01 17:04:55.000000 yadg-5.0.2/src/yadg/extractors/agilentdx/__init__.py
-drwxr-xr-x   0 kraus     (1000) kraus     (1000)        0 2023-12-13 17:47:33.342087 yadg-5.0.2/src/yadg/extractors/eclabmpr/
--rw-r--r--   0 kraus     (1000) kraus     (1000)      159 2023-09-01 17:04:55.000000 yadg-5.0.2/src/yadg/extractors/eclabmpr/__init__.py
-drwxr-xr-x   0 kraus     (1000) kraus     (1000)        0 2023-12-13 17:47:33.342087 yadg-5.0.2/src/yadg/extractors/eclabmpt/
--rw-r--r--   0 kraus     (1000) kraus     (1000)      159 2023-09-01 17:04:55.000000 yadg-5.0.2/src/yadg/extractors/eclabmpt/__init__.py
-drwxr-xr-x   0 kraus     (1000) kraus     (1000)        0 2023-12-13 17:47:33.342087 yadg-5.0.2/src/yadg/extractors/panalyticalxrdml/
--rw-r--r--   0 kraus     (1000) kraus     (1000)      177 2023-09-01 17:04:55.000000 yadg-5.0.2/src/yadg/extractors/panalyticalxrdml/__init__.py
-drwxr-xr-x   0 kraus     (1000) kraus     (1000)        0 2023-12-13 17:47:33.342087 yadg-5.0.2/src/yadg/extractors/phispe/
--rw-r--r--   0 kraus     (1000) kraus     (1000)      147 2023-09-01 17:04:55.000000 yadg-5.0.2/src/yadg/extractors/phispe/__init__.py
--rw-r--r--   0 kraus     (1000) kraus     (1000)     6017 2023-12-13 17:42:48.000000 yadg-5.0.2/src/yadg/main.py
-drwxr-xr-x   0 kraus     (1000) kraus     (1000)        0 2023-12-13 17:47:33.345421 yadg-5.0.2/src/yadg/parsers/
--rw-r--r--   0 kraus     (1000) kraus     (1000)        0 2023-09-01 17:04:55.000000 yadg-5.0.2/src/yadg/parsers/__init__.py
-drwxr-xr-x   0 kraus     (1000) kraus     (1000)        0 2023-12-13 17:47:33.345421 yadg-5.0.2/src/yadg/parsers/basiccsv/
--rw-r--r--   0 kraus     (1000) kraus     (1000)     1521 2023-12-13 17:42:48.000000 yadg-5.0.2/src/yadg/parsers/basiccsv/__init__.py
--rw-r--r--   0 kraus     (1000) kraus     (1000)     6781 2023-12-13 17:42:48.000000 yadg-5.0.2/src/yadg/parsers/basiccsv/main.py
-drwxr-xr-x   0 kraus     (1000) kraus     (1000)        0 2023-12-13 17:47:33.345421 yadg-5.0.2/src/yadg/parsers/chromdata/
--rw-r--r--   0 kraus     (1000) kraus     (1000)     2658 2023-12-13 17:42:48.000000 yadg-5.0.2/src/yadg/parsers/chromdata/__init__.py
--rw-r--r--   0 kraus     (1000) kraus     (1000)     7782 2023-12-13 17:42:48.000000 yadg-5.0.2/src/yadg/parsers/chromdata/empalccsv.py
--rw-r--r--   0 kraus     (1000) kraus     (1000)     7630 2023-12-13 17:42:48.000000 yadg-5.0.2/src/yadg/parsers/chromdata/empalcxlsx.py
--rw-r--r--   0 kraus     (1000) kraus     (1000)     4254 2023-12-13 17:42:48.000000 yadg-5.0.2/src/yadg/parsers/chromdata/fusioncsv.py
--rw-r--r--   0 kraus     (1000) kraus     (1000)     4769 2023-12-13 17:42:48.000000 yadg-5.0.2/src/yadg/parsers/chromdata/fusionjson.py
--rw-r--r--   0 kraus     (1000) kraus     (1000)     2307 2023-12-13 17:42:48.000000 yadg-5.0.2/src/yadg/parsers/chromdata/fusionzip.py
-drwxr-xr-x   0 kraus     (1000) kraus     (1000)        0 2023-12-13 17:47:33.348754 yadg-5.0.2/src/yadg/parsers/chromtrace/
--rw-r--r--   0 kraus     (1000) kraus     (1000)     3470 2023-12-13 17:42:48.000000 yadg-5.0.2/src/yadg/parsers/chromtrace/__init__.py
--rw-r--r--   0 kraus     (1000) kraus     (1000)     4677 2023-12-13 17:42:48.000000 yadg-5.0.2/src/yadg/parsers/chromtrace/agilentch.py
--rw-r--r--   0 kraus     (1000) kraus     (1000)     6274 2023-12-13 17:42:48.000000 yadg-5.0.2/src/yadg/parsers/chromtrace/agilentcsv.py
--rw-r--r--   0 kraus     (1000) kraus     (1000)     3223 2023-12-13 17:42:48.000000 yadg-5.0.2/src/yadg/parsers/chromtrace/agilentdx.py
--rw-r--r--   0 kraus     (1000) kraus     (1000)     5998 2023-12-13 17:42:48.000000 yadg-5.0.2/src/yadg/parsers/chromtrace/ezchromasc.py
--rw-r--r--   0 kraus     (1000) kraus     (1000)     3549 2023-12-13 17:42:48.000000 yadg-5.0.2/src/yadg/parsers/chromtrace/fusionjson.py
--rw-r--r--   0 kraus     (1000) kraus     (1000)     2510 2023-12-13 17:42:48.000000 yadg-5.0.2/src/yadg/parsers/chromtrace/fusionzip.py
-drwxr-xr-x   0 kraus     (1000) kraus     (1000)        0 2023-12-13 17:47:33.348754 yadg-5.0.2/src/yadg/parsers/dummy/
--rw-r--r--   0 kraus     (1000) kraus     (1000)     2551 2023-12-13 17:42:48.000000 yadg-5.0.2/src/yadg/parsers/dummy/__init__.py
-drwxr-xr-x   0 kraus     (1000) kraus     (1000)        0 2023-12-13 17:47:33.348754 yadg-5.0.2/src/yadg/parsers/electrochem/
--rw-r--r--   0 kraus     (1000) kraus     (1000)     2585 2023-12-13 17:42:48.000000 yadg-5.0.2/src/yadg/parsers/electrochem/__init__.py
-drwxr-xr-x   0 kraus     (1000) kraus     (1000)        0 2023-12-13 17:47:33.348754 yadg-5.0.2/src/yadg/parsers/electrochem/eclabcommon/
--rw-r--r--   0 kraus     (1000) kraus     (1000)        0 2023-09-01 17:04:55.000000 yadg-5.0.2/src/yadg/parsers/electrochem/eclabcommon/__init__.py
--rw-r--r--   0 kraus     (1000) kraus     (1000)     6904 2023-09-01 17:04:55.000000 yadg-5.0.2/src/yadg/parsers/electrochem/eclabcommon/mpr_columns.py
--rw-r--r--   0 kraus     (1000) kraus     (1000)     3252 2023-09-01 17:04:55.000000 yadg-5.0.2/src/yadg/parsers/electrochem/eclabcommon/mpt_columns.py
--rw-r--r--   0 kraus     (1000) kraus     (1000)    33969 2023-12-13 17:43:31.000000 yadg-5.0.2/src/yadg/parsers/electrochem/eclabcommon/techniques.py
--rw-r--r--   0 kraus     (1000) kraus     (1000)    21452 2023-12-13 17:42:48.000000 yadg-5.0.2/src/yadg/parsers/electrochem/eclabmpr.py
--rw-r--r--   0 kraus     (1000) kraus     (1000)     9455 2023-12-13 17:42:48.000000 yadg-5.0.2/src/yadg/parsers/electrochem/eclabmpt.py
--rw-r--r--   0 kraus     (1000) kraus     (1000)     4411 2023-09-01 17:04:55.000000 yadg-5.0.2/src/yadg/parsers/electrochem/tomatojson.py
-drwxr-xr-x   0 kraus     (1000) kraus     (1000)        0 2023-12-13 17:47:33.348754 yadg-5.0.2/src/yadg/parsers/flowdata/
--rw-r--r--   0 kraus     (1000) kraus     (1000)      988 2023-09-01 17:04:55.000000 yadg-5.0.2/src/yadg/parsers/flowdata/__init__.py
--rw-r--r--   0 kraus     (1000) kraus     (1000)     6627 2023-12-13 17:42:48.000000 yadg-5.0.2/src/yadg/parsers/flowdata/drycal.py
--rw-r--r--   0 kraus     (1000) kraus     (1000)     1781 2023-12-13 17:42:48.000000 yadg-5.0.2/src/yadg/parsers/flowdata/main.py
-drwxr-xr-x   0 kraus     (1000) kraus     (1000)        0 2023-12-13 17:47:33.352087 yadg-5.0.2/src/yadg/parsers/masstrace/
--rw-r--r--   0 kraus     (1000) kraus     (1000)     2586 2023-12-13 17:42:48.000000 yadg-5.0.2/src/yadg/parsers/masstrace/__init__.py
--rw-r--r--   0 kraus     (1000) kraus     (1000)     9181 2023-12-13 17:42:48.000000 yadg-5.0.2/src/yadg/parsers/masstrace/quadstarsac.py
-drwxr-xr-x   0 kraus     (1000) kraus     (1000)        0 2023-12-13 17:47:33.352087 yadg-5.0.2/src/yadg/parsers/meascsv/
--rw-r--r--   0 kraus     (1000) kraus     (1000)     3317 2023-12-13 17:42:48.000000 yadg-5.0.2/src/yadg/parsers/meascsv/__init__.py
-drwxr-xr-x   0 kraus     (1000) kraus     (1000)        0 2023-12-13 17:47:33.352087 yadg-5.0.2/src/yadg/parsers/qftrace/
--rw-r--r--   0 kraus     (1000) kraus     (1000)     1833 2023-09-01 17:04:55.000000 yadg-5.0.2/src/yadg/parsers/qftrace/__init__.py
--rw-r--r--   0 kraus     (1000) kraus     (1000)     3851 2023-12-13 17:42:48.000000 yadg-5.0.2/src/yadg/parsers/qftrace/labviewcsv.py
-drwxr-xr-x   0 kraus     (1000) kraus     (1000)        0 2023-12-13 17:47:33.352087 yadg-5.0.2/src/yadg/parsers/xpstrace/
--rw-r--r--   0 kraus     (1000) kraus     (1000)     1627 2023-09-01 17:04:55.000000 yadg-5.0.2/src/yadg/parsers/xpstrace/__init__.py
--rw-r--r--   0 kraus     (1000) kraus     (1000)    11662 2023-12-13 17:42:48.000000 yadg-5.0.2/src/yadg/parsers/xpstrace/phispe.py
-drwxr-xr-x   0 kraus     (1000) kraus     (1000)        0 2023-12-13 17:47:33.352087 yadg-5.0.2/src/yadg/parsers/xrdtrace/
--rw-r--r--   0 kraus     (1000) kraus     (1000)     2034 2023-12-13 17:42:48.000000 yadg-5.0.2/src/yadg/parsers/xrdtrace/__init__.py
--rw-r--r--   0 kraus     (1000) kraus     (1000)     1900 2023-09-01 17:04:55.000000 yadg-5.0.2/src/yadg/parsers/xrdtrace/common.py
--rw-r--r--   0 kraus     (1000) kraus     (1000)     4928 2023-12-13 17:42:48.000000 yadg-5.0.2/src/yadg/parsers/xrdtrace/panalyticalcsv.py
--rw-r--r--   0 kraus     (1000) kraus     (1000)     8497 2023-12-13 17:42:48.000000 yadg-5.0.2/src/yadg/parsers/xrdtrace/panalyticalxrdml.py
--rw-r--r--   0 kraus     (1000) kraus     (1000)     2426 2023-12-13 17:42:48.000000 yadg-5.0.2/src/yadg/parsers/xrdtrace/panalyticalxy.py
--rw-r--r--   0 kraus     (1000) kraus     (1000)     7544 2023-12-13 17:42:48.000000 yadg-5.0.2/src/yadg/subcommands.py
-drwxr-xr-x   0 kraus     (1000) kraus     (1000)        0 2023-12-13 17:47:33.358754 yadg-5.0.2/src/yadg.egg-info/
--rw-r--r--   0 kraus     (1000) kraus     (1000)     4574 2023-12-13 17:47:33.000000 yadg-5.0.2/src/yadg.egg-info/PKG-INFO
--rw-r--r--   0 kraus     (1000) kraus     (1000)     2866 2023-12-13 17:47:33.000000 yadg-5.0.2/src/yadg.egg-info/SOURCES.txt
--rw-r--r--   0 kraus     (1000) kraus     (1000)        1 2023-12-13 17:47:33.000000 yadg-5.0.2/src/yadg.egg-info/dependency_links.txt
--rw-r--r--   0 kraus     (1000) kraus     (1000)       49 2023-12-13 17:47:33.000000 yadg-5.0.2/src/yadg.egg-info/entry_points.txt
--rw-r--r--   0 kraus     (1000) kraus     (1000)      288 2023-12-13 17:47:33.000000 yadg-5.0.2/src/yadg.egg-info/requires.txt
--rw-r--r--   0 kraus     (1000) kraus     (1000)        5 2023-12-13 17:47:33.000000 yadg-5.0.2/src/yadg.egg-info/top_level.txt
-drwxr-xr-x   0 kraus     (1000) kraus     (1000)        0 2023-12-13 17:47:33.358754 yadg-5.0.2/tests/
--rw-r--r--   0 kraus     (1000) kraus     (1000)     9557 2023-09-01 17:04:55.000000 yadg-5.0.2/tests/test_basiccsv.py
--rw-r--r--   0 kraus     (1000) kraus     (1000)     8734 2023-12-13 17:42:48.000000 yadg-5.0.2/tests/test_chromdata.py
--rw-r--r--   0 kraus     (1000) kraus     (1000)     6767 2023-09-01 17:04:55.000000 yadg-5.0.2/tests/test_chromtrace.py
--rw-r--r--   0 kraus     (1000) kraus     (1000)     3894 2023-12-13 17:42:48.000000 yadg-5.0.2/tests/test_drycal.py
--rw-r--r--   0 kraus     (1000) kraus     (1000)     3891 2023-09-01 17:04:55.000000 yadg-5.0.2/tests/test_dummy.py
--rw-r--r--   0 kraus     (1000) kraus     (1000)    18511 2023-12-13 17:43:31.000000 yadg-5.0.2/tests/test_electrochem.py
--rw-r--r--   0 kraus     (1000) kraus     (1000)     1216 2023-09-01 17:04:55.000000 yadg-5.0.2/tests/test_encoding.py
--rw-r--r--   0 kraus     (1000) kraus     (1000)     4728 2023-09-01 17:04:55.000000 yadg-5.0.2/tests/test_externaldate.py
--rw-r--r--   0 kraus     (1000) kraus     (1000)      826 2023-09-01 17:04:55.000000 yadg-5.0.2/tests/test_extract.py
--rw-r--r--   0 kraus     (1000) kraus     (1000)     1582 2023-12-13 17:42:48.000000 yadg-5.0.2/tests/test_locale.py
--rw-r--r--   0 kraus     (1000) kraus     (1000)     1652 2023-09-01 17:04:56.000000 yadg-5.0.2/tests/test_masstrace.py
--rw-r--r--   0 kraus     (1000) kraus     (1000)      678 2023-09-01 17:04:56.000000 yadg-5.0.2/tests/test_meascsv.py
--rw-r--r--   0 kraus     (1000) kraus     (1000)      730 2023-09-01 17:04:56.000000 yadg-5.0.2/tests/test_preset.py
--rw-r--r--   0 kraus     (1000) kraus     (1000)     2013 2023-09-01 17:04:56.000000 yadg-5.0.2/tests/test_qftrace.py
--rw-r--r--   0 kraus     (1000) kraus     (1000)     2058 2023-09-01 17:04:56.000000 yadg-5.0.2/tests/test_timezones.py
--rw-r--r--   0 kraus     (1000) kraus     (1000)     1623 2023-09-01 17:04:56.000000 yadg-5.0.2/tests/test_xpstrace.py
--rw-r--r--   0 kraus     (1000) kraus     (1000)     1293 2023-09-01 17:04:56.000000 yadg-5.0.2/tests/test_xrdtrace.py
--rw-r--r--   0 kraus     (1000) kraus     (1000)     6999 2023-12-13 17:42:48.000000 yadg-5.0.2/tests/test_yadg.py
--rw-r--r--   0 kraus     (1000) kraus     (1000)    81176 2023-09-01 17:04:56.000000 yadg-5.0.2/versioneer.py
+drwxr-xr-x   0 kraus     (1000) kraus     (1000)        0 2024-04-06 10:38:28.014293 yadg-5.0.3/
+-rw-r--r--   0 kraus     (1000) kraus     (1000)    35149 2024-03-27 19:00:02.000000 yadg-5.0.3/LICENSE
+-rw-r--r--   0 kraus     (1000) kraus     (1000)       51 2024-04-06 09:27:51.000000 yadg-5.0.3/MANIFEST.in
+-rw-r--r--   0 kraus     (1000) kraus     (1000)     4574 2024-04-06 10:38:28.014293 yadg-5.0.3/PKG-INFO
+-rw-r--r--   0 kraus     (1000) kraus     (1000)     3281 2024-04-06 09:30:35.000000 yadg-5.0.3/README.md
+-rw-r--r--   0 kraus     (1000) kraus     (1000)      199 2024-04-06 10:38:28.014293 yadg-5.0.3/setup.cfg
+-rw-r--r--   0 kraus     (1000) kraus     (1000)     1704 2024-04-06 09:30:35.000000 yadg-5.0.3/setup.py
+drwxr-xr-x   0 kraus     (1000) kraus     (1000)        0 2024-04-06 10:38:27.990962 yadg-5.0.3/src/
+drwxr-xr-x   0 kraus     (1000) kraus     (1000)        0 2024-04-06 10:38:28.014293 yadg-5.0.3/src/yadg/
+-rw-r--r--   0 kraus     (1000) kraus     (1000)      196 2024-04-06 09:30:35.000000 yadg-5.0.3/src/yadg/__init__.py
+-rw-r--r--   0 kraus     (1000) kraus     (1000)      497 2024-04-06 10:38:28.014293 yadg-5.0.3/src/yadg/_version.py
+drwxr-xr-x   0 kraus     (1000) kraus     (1000)        0 2024-04-06 10:38:27.997628 yadg-5.0.3/src/yadg/core/
+-rw-r--r--   0 kraus     (1000) kraus     (1000)     7299 2024-04-06 10:27:42.000000 yadg-5.0.3/src/yadg/core/__init__.py
+drwxr-xr-x   0 kraus     (1000) kraus     (1000)        0 2024-04-06 10:38:27.997628 yadg-5.0.3/src/yadg/dgutils/
+-rw-r--r--   0 kraus     (1000) kraus     (1000)      472 2024-04-06 09:30:35.000000 yadg-5.0.3/src/yadg/dgutils/__init__.py
+-rw-r--r--   0 kraus     (1000) kraus     (1000)     2198 2024-04-06 09:30:35.000000 yadg-5.0.3/src/yadg/dgutils/btools.py
+-rw-r--r--   0 kraus     (1000) kraus     (1000)    13263 2024-04-06 09:30:35.000000 yadg-5.0.3/src/yadg/dgutils/dateutils.py
+-rw-r--r--   0 kraus     (1000) kraus     (1000)      651 2024-04-06 09:30:35.000000 yadg-5.0.3/src/yadg/dgutils/helpers.py
+-rw-r--r--   0 kraus     (1000) kraus     (1000)     2220 2024-04-06 10:29:39.000000 yadg-5.0.3/src/yadg/dgutils/pintutils.py
+-rw-r--r--   0 kraus     (1000) kraus     (1000)     5897 2024-04-06 09:30:35.000000 yadg-5.0.3/src/yadg/dgutils/utils.py
+drwxr-xr-x   0 kraus     (1000) kraus     (1000)        0 2024-04-06 10:38:27.997628 yadg-5.0.3/src/yadg/extractors/
+-rw-r--r--   0 kraus     (1000) kraus     (1000)     2814 2024-04-06 09:30:35.000000 yadg-5.0.3/src/yadg/extractors/__init__.py
+drwxr-xr-x   0 kraus     (1000) kraus     (1000)        0 2024-04-06 10:38:28.000961 yadg-5.0.3/src/yadg/extractors/agilentch/
+-rw-r--r--   0 kraus     (1000) kraus     (1000)      158 2024-04-06 09:30:35.000000 yadg-5.0.3/src/yadg/extractors/agilentch/__init__.py
+drwxr-xr-x   0 kraus     (1000) kraus     (1000)        0 2024-04-06 10:38:28.000961 yadg-5.0.3/src/yadg/extractors/agilentdx/
+-rw-r--r--   0 kraus     (1000) kraus     (1000)      158 2024-04-06 09:30:35.000000 yadg-5.0.3/src/yadg/extractors/agilentdx/__init__.py
+drwxr-xr-x   0 kraus     (1000) kraus     (1000)        0 2024-04-06 10:38:28.000961 yadg-5.0.3/src/yadg/extractors/eclabmpr/
+-rw-r--r--   0 kraus     (1000) kraus     (1000)      159 2024-04-06 09:30:35.000000 yadg-5.0.3/src/yadg/extractors/eclabmpr/__init__.py
+drwxr-xr-x   0 kraus     (1000) kraus     (1000)        0 2024-04-06 10:38:28.000961 yadg-5.0.3/src/yadg/extractors/eclabmpt/
+-rw-r--r--   0 kraus     (1000) kraus     (1000)      159 2024-04-06 09:30:35.000000 yadg-5.0.3/src/yadg/extractors/eclabmpt/__init__.py
+drwxr-xr-x   0 kraus     (1000) kraus     (1000)        0 2024-04-06 10:38:28.000961 yadg-5.0.3/src/yadg/extractors/panalyticalxrdml/
+-rw-r--r--   0 kraus     (1000) kraus     (1000)      177 2024-04-06 09:30:35.000000 yadg-5.0.3/src/yadg/extractors/panalyticalxrdml/__init__.py
+drwxr-xr-x   0 kraus     (1000) kraus     (1000)        0 2024-04-06 10:38:28.000961 yadg-5.0.3/src/yadg/extractors/phispe/
+-rw-r--r--   0 kraus     (1000) kraus     (1000)      147 2024-04-06 09:30:35.000000 yadg-5.0.3/src/yadg/extractors/phispe/__init__.py
+-rw-r--r--   0 kraus     (1000) kraus     (1000)     6017 2024-04-06 09:30:35.000000 yadg-5.0.3/src/yadg/main.py
+drwxr-xr-x   0 kraus     (1000) kraus     (1000)        0 2024-04-06 10:38:28.000961 yadg-5.0.3/src/yadg/parsers/
+-rw-r--r--   0 kraus     (1000) kraus     (1000)        0 2024-04-06 09:27:51.000000 yadg-5.0.3/src/yadg/parsers/__init__.py
+drwxr-xr-x   0 kraus     (1000) kraus     (1000)        0 2024-04-06 10:38:28.000961 yadg-5.0.3/src/yadg/parsers/basiccsv/
+-rw-r--r--   0 kraus     (1000) kraus     (1000)     1521 2024-04-06 09:30:35.000000 yadg-5.0.3/src/yadg/parsers/basiccsv/__init__.py
+-rw-r--r--   0 kraus     (1000) kraus     (1000)     6766 2024-04-06 09:52:08.000000 yadg-5.0.3/src/yadg/parsers/basiccsv/main.py
+drwxr-xr-x   0 kraus     (1000) kraus     (1000)        0 2024-04-06 10:38:28.004294 yadg-5.0.3/src/yadg/parsers/chromdata/
+-rw-r--r--   0 kraus     (1000) kraus     (1000)     2659 2024-04-06 10:29:29.000000 yadg-5.0.3/src/yadg/parsers/chromdata/__init__.py
+-rw-r--r--   0 kraus     (1000) kraus     (1000)     7783 2024-04-06 10:29:30.000000 yadg-5.0.3/src/yadg/parsers/chromdata/empalccsv.py
+-rw-r--r--   0 kraus     (1000) kraus     (1000)     7631 2024-04-06 10:29:30.000000 yadg-5.0.3/src/yadg/parsers/chromdata/empalcxlsx.py
+-rw-r--r--   0 kraus     (1000) kraus     (1000)     4255 2024-04-06 10:29:29.000000 yadg-5.0.3/src/yadg/parsers/chromdata/fusioncsv.py
+-rw-r--r--   0 kraus     (1000) kraus     (1000)     4770 2024-04-06 10:29:29.000000 yadg-5.0.3/src/yadg/parsers/chromdata/fusionjson.py
+-rw-r--r--   0 kraus     (1000) kraus     (1000)     2308 2024-04-06 10:29:29.000000 yadg-5.0.3/src/yadg/parsers/chromdata/fusionzip.py
+drwxr-xr-x   0 kraus     (1000) kraus     (1000)        0 2024-04-06 10:38:28.004294 yadg-5.0.3/src/yadg/parsers/chromtrace/
+-rw-r--r--   0 kraus     (1000) kraus     (1000)     3470 2024-04-06 09:30:35.000000 yadg-5.0.3/src/yadg/parsers/chromtrace/__init__.py
+-rw-r--r--   0 kraus     (1000) kraus     (1000)     4678 2024-04-06 10:29:29.000000 yadg-5.0.3/src/yadg/parsers/chromtrace/agilentch.py
+-rw-r--r--   0 kraus     (1000) kraus     (1000)     6275 2024-04-06 10:29:30.000000 yadg-5.0.3/src/yadg/parsers/chromtrace/agilentcsv.py
+-rw-r--r--   0 kraus     (1000) kraus     (1000)     3224 2024-04-06 10:29:29.000000 yadg-5.0.3/src/yadg/parsers/chromtrace/agilentdx.py
+-rw-r--r--   0 kraus     (1000) kraus     (1000)     5999 2024-04-06 10:29:30.000000 yadg-5.0.3/src/yadg/parsers/chromtrace/ezchromasc.py
+-rw-r--r--   0 kraus     (1000) kraus     (1000)     3550 2024-04-06 10:29:29.000000 yadg-5.0.3/src/yadg/parsers/chromtrace/fusionjson.py
+-rw-r--r--   0 kraus     (1000) kraus     (1000)     2511 2024-04-06 10:29:30.000000 yadg-5.0.3/src/yadg/parsers/chromtrace/fusionzip.py
+drwxr-xr-x   0 kraus     (1000) kraus     (1000)        0 2024-04-06 10:38:28.004294 yadg-5.0.3/src/yadg/parsers/dummy/
+-rw-r--r--   0 kraus     (1000) kraus     (1000)     2552 2024-04-06 10:29:30.000000 yadg-5.0.3/src/yadg/parsers/dummy/__init__.py
+drwxr-xr-x   0 kraus     (1000) kraus     (1000)        0 2024-04-06 10:38:28.004294 yadg-5.0.3/src/yadg/parsers/electrochem/
+-rw-r--r--   0 kraus     (1000) kraus     (1000)     2586 2024-04-06 10:29:29.000000 yadg-5.0.3/src/yadg/parsers/electrochem/__init__.py
+drwxr-xr-x   0 kraus     (1000) kraus     (1000)        0 2024-04-06 10:38:28.007627 yadg-5.0.3/src/yadg/parsers/electrochem/eclabcommon/
+-rw-r--r--   0 kraus     (1000) kraus     (1000)        0 2024-04-06 09:30:35.000000 yadg-5.0.3/src/yadg/parsers/electrochem/eclabcommon/__init__.py
+-rw-r--r--   0 kraus     (1000) kraus     (1000)     6904 2024-04-06 09:30:35.000000 yadg-5.0.3/src/yadg/parsers/electrochem/eclabcommon/mpr_columns.py
+-rw-r--r--   0 kraus     (1000) kraus     (1000)     3252 2024-04-06 09:30:35.000000 yadg-5.0.3/src/yadg/parsers/electrochem/eclabcommon/mpt_columns.py
+-rw-r--r--   0 kraus     (1000) kraus     (1000)    33970 2024-04-06 10:29:31.000000 yadg-5.0.3/src/yadg/parsers/electrochem/eclabcommon/techniques.py
+-rw-r--r--   0 kraus     (1000) kraus     (1000)    21453 2024-04-06 10:29:30.000000 yadg-5.0.3/src/yadg/parsers/electrochem/eclabmpr.py
+-rw-r--r--   0 kraus     (1000) kraus     (1000)     9456 2024-04-06 10:29:30.000000 yadg-5.0.3/src/yadg/parsers/electrochem/eclabmpt.py
+-rw-r--r--   0 kraus     (1000) kraus     (1000)     4411 2024-04-06 09:30:35.000000 yadg-5.0.3/src/yadg/parsers/electrochem/tomatojson.py
+drwxr-xr-x   0 kraus     (1000) kraus     (1000)        0 2024-04-06 10:38:28.007627 yadg-5.0.3/src/yadg/parsers/flowdata/
+-rw-r--r--   0 kraus     (1000) kraus     (1000)      989 2024-04-06 10:29:30.000000 yadg-5.0.3/src/yadg/parsers/flowdata/__init__.py
+-rw-r--r--   0 kraus     (1000) kraus     (1000)     6628 2024-04-06 10:29:30.000000 yadg-5.0.3/src/yadg/parsers/flowdata/drycal.py
+-rw-r--r--   0 kraus     (1000) kraus     (1000)     1780 2024-04-06 10:29:39.000000 yadg-5.0.3/src/yadg/parsers/flowdata/main.py
+drwxr-xr-x   0 kraus     (1000) kraus     (1000)        0 2024-04-06 10:38:28.007627 yadg-5.0.3/src/yadg/parsers/masstrace/
+-rw-r--r--   0 kraus     (1000) kraus     (1000)     2587 2024-04-06 10:29:30.000000 yadg-5.0.3/src/yadg/parsers/masstrace/__init__.py
+-rw-r--r--   0 kraus     (1000) kraus     (1000)     9182 2024-04-06 10:29:30.000000 yadg-5.0.3/src/yadg/parsers/masstrace/quadstarsac.py
+drwxr-xr-x   0 kraus     (1000) kraus     (1000)        0 2024-04-06 10:38:28.007627 yadg-5.0.3/src/yadg/parsers/meascsv/
+-rw-r--r--   0 kraus     (1000) kraus     (1000)     3317 2024-04-06 09:30:35.000000 yadg-5.0.3/src/yadg/parsers/meascsv/__init__.py
+drwxr-xr-x   0 kraus     (1000) kraus     (1000)        0 2024-04-06 10:38:28.007627 yadg-5.0.3/src/yadg/parsers/qftrace/
+-rw-r--r--   0 kraus     (1000) kraus     (1000)     1834 2024-04-06 10:29:30.000000 yadg-5.0.3/src/yadg/parsers/qftrace/__init__.py
+-rw-r--r--   0 kraus     (1000) kraus     (1000)     3851 2024-04-06 09:30:35.000000 yadg-5.0.3/src/yadg/parsers/qftrace/labviewcsv.py
+drwxr-xr-x   0 kraus     (1000) kraus     (1000)        0 2024-04-06 10:38:28.007627 yadg-5.0.3/src/yadg/parsers/xpstrace/
+-rw-r--r--   0 kraus     (1000) kraus     (1000)     1628 2024-04-06 10:29:30.000000 yadg-5.0.3/src/yadg/parsers/xpstrace/__init__.py
+-rw-r--r--   0 kraus     (1000) kraus     (1000)    11662 2024-04-06 09:30:35.000000 yadg-5.0.3/src/yadg/parsers/xpstrace/phispe.py
+drwxr-xr-x   0 kraus     (1000) kraus     (1000)        0 2024-04-06 10:38:28.007627 yadg-5.0.3/src/yadg/parsers/xrdtrace/
+-rw-r--r--   0 kraus     (1000) kraus     (1000)     2035 2024-04-06 10:29:30.000000 yadg-5.0.3/src/yadg/parsers/xrdtrace/__init__.py
+-rw-r--r--   0 kraus     (1000) kraus     (1000)     1900 2024-04-06 09:27:51.000000 yadg-5.0.3/src/yadg/parsers/xrdtrace/common.py
+-rw-r--r--   0 kraus     (1000) kraus     (1000)     4928 2024-04-06 09:30:35.000000 yadg-5.0.3/src/yadg/parsers/xrdtrace/panalyticalcsv.py
+-rw-r--r--   0 kraus     (1000) kraus     (1000)     8497 2024-04-06 09:30:35.000000 yadg-5.0.3/src/yadg/parsers/xrdtrace/panalyticalxrdml.py
+-rw-r--r--   0 kraus     (1000) kraus     (1000)     2426 2024-04-06 09:30:35.000000 yadg-5.0.3/src/yadg/parsers/xrdtrace/panalyticalxy.py
+-rw-r--r--   0 kraus     (1000) kraus     (1000)     7703 2024-04-06 10:29:21.000000 yadg-5.0.3/src/yadg/subcommands.py
+drwxr-xr-x   0 kraus     (1000) kraus     (1000)        0 2024-04-06 10:38:28.014293 yadg-5.0.3/src/yadg.egg-info/
+-rw-r--r--   0 kraus     (1000) kraus     (1000)     4574 2024-04-06 10:38:27.000000 yadg-5.0.3/src/yadg.egg-info/PKG-INFO
+-rw-r--r--   0 kraus     (1000) kraus     (1000)     2866 2024-04-06 10:38:27.000000 yadg-5.0.3/src/yadg.egg-info/SOURCES.txt
+-rw-r--r--   0 kraus     (1000) kraus     (1000)        1 2024-04-06 10:38:27.000000 yadg-5.0.3/src/yadg.egg-info/dependency_links.txt
+-rw-r--r--   0 kraus     (1000) kraus     (1000)       49 2024-04-06 10:38:27.000000 yadg-5.0.3/src/yadg.egg-info/entry_points.txt
+-rw-r--r--   0 kraus     (1000) kraus     (1000)      288 2024-04-06 10:38:27.000000 yadg-5.0.3/src/yadg.egg-info/requires.txt
+-rw-r--r--   0 kraus     (1000) kraus     (1000)        5 2024-04-06 10:38:27.000000 yadg-5.0.3/src/yadg.egg-info/top_level.txt
+drwxr-xr-x   0 kraus     (1000) kraus     (1000)        0 2024-04-06 10:38:28.014293 yadg-5.0.3/tests/
+-rw-r--r--   0 kraus     (1000) kraus     (1000)    10184 2024-04-06 10:29:30.000000 yadg-5.0.3/tests/test_basiccsv.py
+-rw-r--r--   0 kraus     (1000) kraus     (1000)     8734 2024-04-06 09:30:35.000000 yadg-5.0.3/tests/test_chromdata.py
+-rw-r--r--   0 kraus     (1000) kraus     (1000)     6767 2024-04-06 09:30:35.000000 yadg-5.0.3/tests/test_chromtrace.py
+-rw-r--r--   0 kraus     (1000) kraus     (1000)     3894 2024-04-06 09:52:45.000000 yadg-5.0.3/tests/test_drycal.py
+-rw-r--r--   0 kraus     (1000) kraus     (1000)     3891 2024-04-06 09:30:35.000000 yadg-5.0.3/tests/test_dummy.py
+-rw-r--r--   0 kraus     (1000) kraus     (1000)    18511 2024-04-06 09:30:35.000000 yadg-5.0.3/tests/test_electrochem.py
+-rw-r--r--   0 kraus     (1000) kraus     (1000)     1216 2024-03-27 19:00:02.000000 yadg-5.0.3/tests/test_encoding.py
+-rw-r--r--   0 kraus     (1000) kraus     (1000)     4728 2024-03-27 19:00:02.000000 yadg-5.0.3/tests/test_externaldate.py
+-rw-r--r--   0 kraus     (1000) kraus     (1000)      826 2024-04-06 09:30:35.000000 yadg-5.0.3/tests/test_extract.py
+-rw-r--r--   0 kraus     (1000) kraus     (1000)     1582 2024-04-06 09:30:36.000000 yadg-5.0.3/tests/test_locale.py
+-rw-r--r--   0 kraus     (1000) kraus     (1000)     1652 2024-04-06 09:30:36.000000 yadg-5.0.3/tests/test_masstrace.py
+-rw-r--r--   0 kraus     (1000) kraus     (1000)      678 2024-04-06 09:30:36.000000 yadg-5.0.3/tests/test_meascsv.py
+-rw-r--r--   0 kraus     (1000) kraus     (1000)      730 2024-04-06 09:30:36.000000 yadg-5.0.3/tests/test_preset.py
+-rw-r--r--   0 kraus     (1000) kraus     (1000)     2013 2024-04-06 09:30:36.000000 yadg-5.0.3/tests/test_qftrace.py
+-rw-r--r--   0 kraus     (1000) kraus     (1000)     2058 2024-04-06 09:30:36.000000 yadg-5.0.3/tests/test_timezones.py
+-rw-r--r--   0 kraus     (1000) kraus     (1000)     1623 2024-04-06 09:30:36.000000 yadg-5.0.3/tests/test_xpstrace.py
+-rw-r--r--   0 kraus     (1000) kraus     (1000)     1293 2024-04-06 09:30:36.000000 yadg-5.0.3/tests/test_xrdtrace.py
+-rw-r--r--   0 kraus     (1000) kraus     (1000)     6999 2024-04-06 09:30:36.000000 yadg-5.0.3/tests/test_yadg.py
+-rw-r--r--   0 kraus     (1000) kraus     (1000)    81170 2024-04-06 10:29:39.000000 yadg-5.0.3/versioneer.py
```

### Comparing `yadg-5.0.2/LICENSE` & `yadg-5.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `yadg-5.0.2/PKG-INFO` & `yadg-5.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yadg
-Version: 5.0.2
+Version: 5.0.3
 Summary: yet another datagram
 Home-page: https://github.com/dgbowl/yadg
 Author: Peter Kraus
 Author-email: peter@tondon.de
 Project-URL: Bug Tracker, https://github.com/dgbowl/yadg/issues
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `yadg-5.0.2/README.md` & `yadg-5.0.3/README.md`

 * *Files identical despite different names*

### Comparing `yadg-5.0.2/setup.py` & `yadg-5.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `yadg-5.0.2/src/yadg/core/__init__.py` & `yadg-5.0.3/src/yadg/core/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,14 +72,18 @@
         "input_schema": dataschema.json(),
         "datagram_version": core.datagram_version,
     }
     root.attrs.update(dgutils.get_yadg_metadata())
 
     while hasattr(dataschema, "update"):
         dataschema = dataschema.update()
+        if hasattr(dataschema, "metadata"):
+            if hasattr(dataschema.metadata, "version"):
+                if dataschema.metadata.version == "5.0":
+                    break
 
     for si, step in enumerate(dataschema.steps):
         logger.info("Processing step %d:", si)
 
         # Backfill default timezone, locale, encoding.
         if step.extractor.timezone is None:
             tz = ZoneInfo(dataschema.step_defaults.timezone)
```

### Comparing `yadg-5.0.2/src/yadg/dgutils/btools.py` & `yadg-5.0.3/src/yadg/dgutils/btools.py`

 * *Files identical despite different names*

### Comparing `yadg-5.0.2/src/yadg/dgutils/dateutils.py` & `yadg-5.0.3/src/yadg/dgutils/dateutils.py`

 * *Files identical despite different names*

### Comparing `yadg-5.0.2/src/yadg/dgutils/helpers.py` & `yadg-5.0.3/src/yadg/dgutils/helpers.py`

 * *Files identical despite different names*

### Comparing `yadg-5.0.2/src/yadg/dgutils/pintutils.py` & `yadg-5.0.3/src/yadg/dgutils/pintutils.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 This package defines ``ureg``, a :class:`pint.UnitRegistry` used for validation of
 `datagrams` in **yadg**. The default SI :class:`pint.UnitRegistry` is extended
 by definitions of fractional quantities (%, ppm, etc.), standard volumetric
 quantities (smL/min, sccm), and other dimensionless "units" present in several
 file types.
 """
+
 import logging
 from typing import Union
 import pint
 
 logger = logging.getLogger(__name__)
 
 ureg = pint.UnitRegistry(
@@ -44,15 +45,15 @@
     if unit in ["deg C", "Deg C"]:
         return "degC"
     else:
         return unit
 
 
 def sanitize_units(
-    units: Union[str, dict[str, str], list[str]]
+    units: Union[str, dict[str, str], list[str]],
 ) -> Union[str, dict[str, str], list[str]]:
     """
     Unit sanitizer.
 
     This sanitizer should be used where user-supplied units are likely to occur,
     such as in the parsers :mod:`yadg.parsers.basiccsv`. Currently, only two
     replacements are done:
```

### Comparing `yadg-5.0.2/src/yadg/dgutils/utils.py` & `yadg-5.0.3/src/yadg/dgutils/utils.py`

 * *Files identical despite different names*

### Comparing `yadg-5.0.2/src/yadg/extractors/__init__.py` & `yadg-5.0.3/src/yadg/extractors/__init__.py`

 * *Files identical despite different names*

### Comparing `yadg-5.0.2/src/yadg/main.py` & `yadg-5.0.3/src/yadg/main.py`

 * *Files identical despite different names*

### Comparing `yadg-5.0.2/src/yadg/parsers/basiccsv/__init__.py` & `yadg-5.0.3/src/yadg/parsers/basiccsv/__init__.py`

 * *Files identical despite different names*

### Comparing `yadg-5.0.2/src/yadg/parsers/basiccsv/main.py` & `yadg-5.0.3/src/yadg/parsers/basiccsv/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,27 +102,32 @@
 def dicts_to_dataset(
     data: dict[str, list[Any]],
     meta: dict[str, list[Any]],
     units: dict[str, str] = dict(),
     fulldate: bool = True,
 ) -> xr.Dataset:
     darrs = {}
-    for k, v in data.items():
+    for key, val in data.items():
         attrs = {}
-        u = units.get(k, None)
+        u = units.get(key, None)
         if u is not None:
             attrs["units"] = u
-        if k == "uts":
+        if key == "uts":
             continue
-        darrs[k] = xr.DataArray(data=v, dims=["uts"], attrs=attrs)
-        if k in meta and darrs[k].dtype.kind in {"i", "u", "f", "c", "m", "M"}:
+        if "/" in key:
+            logger.warning(f"Replacing '/' for '_' in column {key!r}.")
+            k = key.replace("/", "_")
+        else:
+            k = key
+        darrs[k] = xr.DataArray(data=val, dims=["uts"], attrs=attrs)
+        if key in meta and darrs[k].dtype.kind in {"i", "u", "f", "c", "m", "M"}:
             err = f"{k}_std_err"
             darrs[k].attrs["ancillary_variables"] = err
             attrs["standard_name"] = f"{k} standard error"
-            darrs[err] = xr.DataArray(data=meta[k], dims=["uts"], attrs=attrs)
+            darrs[err] = xr.DataArray(data=meta[key], dims=["uts"], attrs=attrs)
     if "uts" in data:
         coords = dict(uts=data.pop("uts"))
     else:
         coords = dict()
     if fulldate:
         attrs = dict()
     else:
@@ -178,19 +183,14 @@
     with open(fn, "r", encoding=encoding) as infile:
         # This decode/encode is done to account for some csv files that have a BOM
         # at the beginning of each line.
         lines = [i.encode().decode(encoding) for i in infile.readlines()]
     assert len(lines) >= 2
     headers = [h.strip().strip(strip) for h in lines[0].split(parameters.sep)]
 
-    for hi, header in enumerate(headers):
-        if "/" in header:
-            logger.warning("Replacing '/' for '_' in header '%s'.", header)
-            headers[hi] = header.replace("/", "_")
-
     datecolumns, datefunc, fulldate = dgutils.infer_timestamp_from(
         headers=headers, spec=parameters.timestamp, timezone=timezone
     )
 
     # Populate units
     units = parameters.units
     if units is None:
```

### Comparing `yadg-5.0.2/src/yadg/parsers/chromdata/__init__.py` & `yadg-5.0.3/src/yadg/parsers/chromdata/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -50,14 +50,15 @@
       concentration:  (uts, species)        # Species concentration (mol/l)
       xout:           (uts, species)        # Species mole fraction (-)
 
 Module Functions
 ````````````````
 
 """
+
 import xarray as xr
 
 from . import (
     fusionjson,
     fusionzip,
     fusioncsv,
     empalccsv,
```

### Comparing `yadg-5.0.2/src/yadg/parsers/chromdata/empalccsv.py` & `yadg-5.0.3/src/yadg/parsers/chromdata/empalccsv.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
   - metadata section,
   - table containing sampling information,
   - table containing analysed chromatography data.
 
 .. codeauthor:: Peter Kraus
 """
+
 import logging
 import datetime
 from uncertainties.core import str_to_number_with_uncert as tuple_fromstr
 import xarray as xr
 import numpy as np
 
 logger = logging.getLogger(__name__)
```

### Comparing `yadg-5.0.2/src/yadg/parsers/chromdata/empalcxlsx.py` & `yadg-5.0.3/src/yadg/parsers/chromdata/empalcxlsx.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,14 +8,15 @@
   - metadata section,
   - table containing sampling information,
   - table containing analysed chromatography data.
 
 
 .. codeauthor:: Peter Kraus
 """
+
 import logging
 import datetime
 import openpyxl
 from uncertainties.core import str_to_number_with_uncert as tuple_fromstr
 import xarray as xr
 import numpy as np
```

### Comparing `yadg-5.0.2/src/yadg/parsers/chromdata/fusioncsv.py` & `yadg-5.0.3/src/yadg/parsers/chromdata/fusioncsv.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
     As also mentioned in the ``csv`` files themselves, the use of this filetype
     is discouraged, and the ``json`` files (or a zipped archive of them) should
     be parsed instead.
 
 .. codeauthor:: Peter Kraus
 """
+
 import logging
 from zoneinfo import ZoneInfo
 from ...dgutils.dateutils import str_to_uts
 from uncertainties.core import str_to_number_with_uncert as tuple_fromstr
 import xarray as xr
 import numpy as np
```

### Comparing `yadg-5.0.2/src/yadg/parsers/chromdata/fusionjson.py` & `yadg-5.0.3/src/yadg/parsers/chromdata/fusionjson.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,14 +26,15 @@
       method:   !!str
       username: None
       version:  !!str
       datafile: !!str
 
 .. codeauthor:: Peter Kraus
 """
+
 import json
 import logging
 from zoneinfo import ZoneInfo
 from ...dgutils.dateutils import str_to_uts
 import xarray as xr
 import numpy as np
```

### Comparing `yadg-5.0.2/src/yadg/parsers/chromdata/fusionzip.py` & `yadg-5.0.3/src/yadg/parsers/chromdata/fusionzip.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 This is a wrapper parser which unzips the provided zip file, and then uses
 the :mod:`yadg.parsers.chromdata.fusionjson` parser to parse every data
 file present in the archive.
 
 .. codeauthor:: Peter Kraus
 """
+
 import zipfile
 import tempfile
 import os
 import xarray as xr
 
 from .fusionjson import process as processjson
```

### Comparing `yadg-5.0.2/src/yadg/parsers/chromtrace/__init__.py` & `yadg-5.0.3/src/yadg/parsers/chromtrace/__init__.py`

 * *Files identical despite different names*

### Comparing `yadg-5.0.2/src/yadg/parsers/chromtrace/agilentch.py` & `yadg-5.0.3/src/yadg/parsers/chromtrace/agilentch.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,14 +29,15 @@
     0x127c "y-axis slope"
 
 Data is stored in a consecutive set of ``<f8``, starting at the offset (calculated
 as ``offset =  ("data offset" - 1) * 512``) until the end of the file.
 
 .. codeauthor:: Peter Kraus
 """
+
 import numpy as np
 from zoneinfo import ZoneInfo
 from ... import dgutils
 from ...dgutils.dateutils import str_to_uts
 import xarray as xr
 from datatree import DataTree
```

### Comparing `yadg-5.0.2/src/yadg/parsers/chromtrace/agilentcsv.py` & `yadg-5.0.3/src/yadg/parsers/chromtrace/agilentcsv.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 
 .. warning ::
 
     Unfortunately, the chromatographic ``method`` is not exposed in this file format.
 
 .. codeauthor:: Peter Kraus
 """
+
 import numpy as np
 from zoneinfo import ZoneInfo
 from uncertainties.core import str_to_number_with_uncert as tuple_fromstr
 from ...dgutils.dateutils import str_to_uts
 import xarray as xr
 from datatree import DataTree
```

### Comparing `yadg-5.0.2/src/yadg/parsers/chromtrace/agilentdx.py` & `yadg-5.0.3/src/yadg/parsers/chromtrace/agilentdx.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 .. note::
 
    Currently the timesteps from multiple CH files (if present) are appended in the
    timesteps array without any further sorting.
 
 .. codeauthor:: Peter Kraus
 """
+
 import zipfile
 import tempfile
 import os
 from .agilentch import process as processch
 from datatree import DataTree
 import xarray as xr
```

### Comparing `yadg-5.0.2/src/yadg/parsers/chromtrace/ezchromasc.py` & `yadg-5.0.3/src/yadg/parsers/chromtrace/ezchromasc.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 This file format includes one timestep with multiple traces in each ASCII file. It
 contains a header section, and a sequence of Y datapoints (``signal``) for each detector.
 The X-axis (``elution_time``) is assumed to be uniform between traces, and its units have
 to be deduced from the header.
 
 .. codeauthor:: Peter Kraus
 """
+
 import numpy as np
 import logging
 from zoneinfo import ZoneInfo
 from uncertainties.core import str_to_number_with_uncert as tuple_fromstr
 from ...dgutils.dateutils import str_to_uts
 import xarray as xr
 from datatree import DataTree
```

### Comparing `yadg-5.0.2/src/yadg/parsers/chromtrace/fusionjson.py` & `yadg-5.0.3/src/yadg/parsers/chromtrace/fusionjson.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     method:   !!str
     sampleid: !!str
     version:  !!str
     datafile: !!str
 
 .. codeauthor:: Peter Kraus
 """
+
 import json
 from zoneinfo import ZoneInfo
 import numpy as np
 from ...dgutils.dateutils import str_to_uts
 import xarray as xr
 from datatree import DataTree
```

### Comparing `yadg-5.0.2/src/yadg/parsers/chromtrace/fusionzip.py` & `yadg-5.0.3/src/yadg/parsers/chromtrace/fusionzip.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     method:   !!str
     sampleid: !!str
     version:  !!str
     datafile: !!str
 
 .. codeauthor:: Peter Kraus
 """
+
 import zipfile
 import tempfile
 import os
 import xarray as xr
 from datatree import DataTree
 
 from .fusionjson import process as processjson
```

### Comparing `yadg-5.0.2/src/yadg/parsers/dummy/__init__.py` & `yadg-5.0.3/src/yadg/parsers/dummy/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 
 The value of every element of ``data`` is assigned a deviation of 0.0.
 
 Module Functions
 ````````````````
 
 """
+
 from pydantic import BaseModel
 import json
 from ... import dgutils
 from ..basiccsv.main import append_dicts, dicts_to_dataset
 from datatree import DataTree
```

### Comparing `yadg-5.0.2/src/yadg/parsers/electrochem/__init__.py` & `yadg-5.0.3/src/yadg/parsers/electrochem/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,14 +52,15 @@
   optionally transposed data from impedance spectroscopy, grouping the datapoints
   in each scan into a single "trace". This behaviour has been removed in ``yadg-5.0``.
 
 Module Functions
 ````````````````
 
 """
+
 import xarray as xr
 from . import eclabmpr, eclabmpt, tomatojson
 
 
 def process(
     *,
     filetype: str,
```

### Comparing `yadg-5.0.2/src/yadg/parsers/electrochem/eclabcommon/mpr_columns.py` & `yadg-5.0.3/src/yadg/parsers/electrochem/eclabcommon/mpr_columns.py`

 * *Files identical despite different names*

### Comparing `yadg-5.0.2/src/yadg/parsers/electrochem/eclabcommon/mpt_columns.py` & `yadg-5.0.3/src/yadg/parsers/electrochem/eclabcommon/mpt_columns.py`

 * *Files identical despite different names*

### Comparing `yadg-5.0.2/src/yadg/parsers/electrochem/eclabcommon/techniques.py` & `yadg-5.0.3/src/yadg/parsers/electrochem/eclabcommon/techniques.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     - WAIT - Wait
     - ZIR - IR compensation (PEIS)
 
 The module also implements resolution determination for parameters of techniques,
 in :func:`get_resolution`.
 
 """
+
 import re
 import numpy as np
 from typing import Union
 import bisect
 import logging
 
 logger = logging.getLogger(__name__)
```

### Comparing `yadg-5.0.2/src/yadg/parsers/electrochem/eclabmpr.py` & `yadg-5.0.3/src/yadg/parsers/electrochem/eclabmpr.py`

 * *Files 0% similar despite different names*

```diff
@@ -190,14 +190,15 @@
 
     If the ``.mpr`` file contains an ``ExtDev`` module (containing parameters
     of any external sensors plugged into the device), the ``log`` is usually
     not present and therefore the full timestamp cannot be calculated.
 
 .. codeauthor:: Nicolas Vetsch
 """
+
 import logging
 from zoneinfo import ZoneInfo
 import xarray as xr
 import numpy as np
 from ...dgutils.dateutils import ole_to_uts
 from ...dgutils.btools import read_value
 from .eclabcommon.techniques import (
```

### Comparing `yadg-5.0.2/src/yadg/parsers/electrochem/eclabmpt.py` & `yadg-5.0.3/src/yadg/parsers/electrochem/eclabmpt.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 .. note ::
 
     The mapping between metadata parameters between ``.mpr`` and ``.mpt`` files
     is not yet complete.
 
 .. codeauthor:: Nicolas Vetsch
 """
+
 import re
 import logging
 import locale as lc
 import xarray as xr
 from zoneinfo import ZoneInfo
 from ...dgutils.dateutils import str_to_uts
 from .eclabcommon.techniques import get_resolution, technique_params, param_from_key
```

### Comparing `yadg-5.0.2/src/yadg/parsers/electrochem/tomatojson.py` & `yadg-5.0.3/src/yadg/parsers/electrochem/tomatojson.py`

 * *Files identical despite different names*

### Comparing `yadg-5.0.2/src/yadg/parsers/flowdata/__init__.py` & `yadg-5.0.3/src/yadg/parsers/flowdata/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -29,10 +29,11 @@
 The parser is used to extract all tabular data in the input file. This parser processes
 additional calibration information analogously to :mod:`~yadg.parsers.basiccsv`.
 
 Module Functions
 ````````````````
 
 """
+
 from .main import process
 
 __all__ = ["process"]
```

### Comparing `yadg-5.0.2/src/yadg/parsers/flowdata/drycal.py` & `yadg-5.0.3/src/yadg/parsers/flowdata/drycal.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 The DryCal files only contain the timestamps of the datapoints, not the date. Therefore,
 the date has to be supplied either using the ``date`` argument in parameters, or is
 parsed from the prefix of the filename.
 
 .. codeauthor:: Peter Kraus
 """
+
 from striprtf.striprtf import rtf_to_text
 from ..basiccsv.main import process_row, append_dicts, dicts_to_dataset
 from ... import dgutils
 from pydantic import BaseModel
 from typing import Optional
 from datatree import DataTree
 from zoneinfo import ZoneInfo
```

### Comparing `yadg-5.0.2/src/yadg/parsers/flowdata/main.py` & `yadg-5.0.3/src/yadg/parsers/flowdata/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,14 @@
     Returns
     -------
     :class:`xarray.Dataset`
 
     """
 
     if filetype.startswith("drycal"):
-
         if filetype.endswith(".rtf") or fn.endswith("rtf"):
             vals = drycal.rtf(fn, encoding, timezone)
         elif filetype.endswith(".csv") or fn.endswith("csv"):
             vals = drycal.sep(fn, ",", encoding, timezone)
         elif filetype.endswith(".txt") or fn.endswith("txt"):
             vals = drycal.sep(fn, "\t", encoding, timezone)
```

### Comparing `yadg-5.0.2/src/yadg/parsers/masstrace/__init__.py` & `yadg-5.0.3/src/yadg/parsers/masstrace/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,14 +58,15 @@
     F.S.R. (e.g. 1e-9), and will then flip directly to the maximum value
     of a float32. These values are set to ``float("NaN")``.
 
 Module Functions
 ````````````````
 
 """
+
 import datatree
 from . import quadstarsac
 
 
 def process(
     *,
     filetype: str,
```

### Comparing `yadg-5.0.2/src/yadg/parsers/masstrace/quadstarsac.py` & `yadg-5.0.3/src/yadg/parsers/masstrace/quadstarsac.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,14 +60,15 @@
     # Datapoints. Read these 4 bytes (scan_width * values_per_mass)
     # times.
     data_position + (n * timestep_length) + 0x06 "datapoints"
     ...
 
 .. codeauthor:: Nicolas Vetsch
 """
+
 import numpy as np
 from datatree import DataTree
 import xarray as xr
 import yadg.dgutils as dgutils
 
 # The general header at the top of .sac files.
 general_header_dtype = np.dtype(
```

### Comparing `yadg-5.0.2/src/yadg/parsers/meascsv/__init__.py` & `yadg-5.0.3/src/yadg/parsers/meascsv/__init__.py`

 * *Files identical despite different names*

### Comparing `yadg-5.0.2/src/yadg/parsers/qftrace/__init__.py` & `yadg-5.0.3/src/yadg/parsers/qftrace/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,14 +39,15 @@
         average:    (uts)         # Number of scans averaged to form a single trace
         bandwidth:  (uts)         # Filter bandwidth (Hz)
 
 Module Functions
 ````````````````
 
 """
+
 from . import labviewcsv
 import datatree
 
 
 def process(
     *,
     filetype: str,
```

### Comparing `yadg-5.0.2/src/yadg/parsers/qftrace/labviewcsv.py` & `yadg-5.0.3/src/yadg/parsers/qftrace/labviewcsv.py`

 * *Files identical despite different names*

### Comparing `yadg-5.0.2/src/yadg/parsers/xpstrace/__init__.py` & `yadg-5.0.3/src/yadg/parsers/xpstrace/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,14 +36,15 @@
       data_vals:
         y:                (uts, E)     # signal
 
 Module Functions
 ````````````````
 
 """
+
 import datatree
 from . import phispe
 
 
 def process(
     *,
     filetype: str,
```

### Comparing `yadg-5.0.2/src/yadg/parsers/xpstrace/phispe.py` & `yadg-5.0.3/src/yadg/parsers/xpstrace/phispe.py`

 * *Files identical despite different names*

### Comparing `yadg-5.0.2/src/yadg/parsers/xrdtrace/__init__.py` & `yadg-5.0.3/src/yadg/parsers/xrdtrace/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,14 +36,15 @@
     coords:
       uts:         !!float
       angle:       !!float            # Diffraction angle (deg)
     data_vals:
       intensity:   (uts, angle)       # Detector intensity (counts)
 
 """
+
 import xarray as xr
 from . import panalyticalxrdml, panalyticalcsv, panalyticalxy
 
 
 def process(
     *,
     filetype: str,
```

### Comparing `yadg-5.0.2/src/yadg/parsers/xrdtrace/common.py` & `yadg-5.0.3/src/yadg/parsers/xrdtrace/common.py`

 * *Files identical despite different names*

### Comparing `yadg-5.0.2/src/yadg/parsers/xrdtrace/panalyticalcsv.py` & `yadg-5.0.3/src/yadg/parsers/xrdtrace/panalyticalcsv.py`

 * *Files identical despite different names*

### Comparing `yadg-5.0.2/src/yadg/parsers/xrdtrace/panalyticalxrdml.py` & `yadg-5.0.3/src/yadg/parsers/xrdtrace/panalyticalxrdml.py`

 * *Files identical despite different names*

### Comparing `yadg-5.0.2/src/yadg/parsers/xrdtrace/panalyticalxy.py` & `yadg-5.0.3/src/yadg/parsers/xrdtrace/panalyticalxy.py`

 * *Files identical despite different names*

### Comparing `yadg-5.0.2/src/yadg/subcommands.py` & `yadg-5.0.3/src/yadg/subcommands.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,14 +63,18 @@
 
     logger.info("Loading dataschema.")
     ds = to_dataschema(**schema)
     logger.info("Loaded dataschema version '%s'", ds.metadata.version)
 
     while hasattr(ds, "update"):
         ds = ds.update()
+        if hasattr(ds, "metadata"):
+            if hasattr(ds.metadata, "version"):
+                if ds.metadata.version == "5.0":
+                    break
 
     logger.debug("Processing schema")
     datagram = core.process_schema(ds, strict_merge=not args.ignore_merge_errors)
 
     logger.info("Saving datagram to '%s'.", args.outfile)
     datagram.to_netcdf(args.outfile, engine="h5netcdf")
     # with open(args.outfile, "w") as ofile:
```

### Comparing `yadg-5.0.2/src/yadg.egg-info/PKG-INFO` & `yadg-5.0.3/src/yadg.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yadg
-Version: 5.0.2
+Version: 5.0.3
 Summary: yet another datagram
 Home-page: https://github.com/dgbowl/yadg
 Author: Peter Kraus
 Author-email: peter@tondon.de
 Project-URL: Bug Tracker, https://github.com/dgbowl/yadg/issues
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `yadg-5.0.2/src/yadg.egg-info/SOURCES.txt` & `yadg-5.0.3/src/yadg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `yadg-5.0.2/tests/test_basiccsv.py` & `yadg-5.0.3/tests/test_basiccsv.py`

 * *Files 3% similar despite different names*

```diff
@@ -275,7 +275,28 @@
     ],
 )
 def test_datagram_from_basiccsv(input, ts, datadir):
     ver = input.pop("version", "4.0")
     ret = datagram_from_input(input, "basiccsv", datadir, version=ver)
     standard_datagram_test(ret, ts)
     pars_datagram_test(ret, ts)
+
+
+def test_issue_143(datadir):
+    input = {
+        "case": "flow_data.csv",
+        "version": "4.2",
+        "parameters": {
+            "sep": ",",
+            "timestamp": {"time": {"index": 5}},
+            "units": {
+                "DryCal smL/min": "smL/min",
+                "DryCal Avg. smL/min": "smL/min",
+                "Temp. Deg C": "degC",
+                "Pressure mBar": "mbar",
+            },
+        },
+    }
+    ver = input.pop("version", "4.0")
+    ret = datagram_from_input(input, "basiccsv", datadir, version=ver)
+    print(f"{ret=}")
+    assert ret["0"]["DryCal smL_min"].attrs["units"] == "smL/min"
```

### Comparing `yadg-5.0.2/tests/test_chromdata.py` & `yadg-5.0.3/tests/test_chromdata.py`

 * *Files identical despite different names*

### Comparing `yadg-5.0.2/tests/test_chromtrace.py` & `yadg-5.0.3/tests/test_chromtrace.py`

 * *Files identical despite different names*

### Comparing `yadg-5.0.2/tests/test_drycal.py` & `yadg-5.0.3/tests/test_drycal.py`

 * *Files identical despite different names*

### Comparing `yadg-5.0.2/tests/test_dummy.py` & `yadg-5.0.3/tests/test_dummy.py`

 * *Files identical despite different names*

### Comparing `yadg-5.0.2/tests/test_electrochem.py` & `yadg-5.0.3/tests/test_electrochem.py`

 * *Files identical despite different names*

### Comparing `yadg-5.0.2/tests/test_encoding.py` & `yadg-5.0.3/tests/test_encoding.py`

 * *Files identical despite different names*

### Comparing `yadg-5.0.2/tests/test_externaldate.py` & `yadg-5.0.3/tests/test_externaldate.py`

 * *Files identical despite different names*

### Comparing `yadg-5.0.2/tests/test_extract.py` & `yadg-5.0.3/tests/test_extract.py`

 * *Files identical despite different names*

### Comparing `yadg-5.0.2/tests/test_locale.py` & `yadg-5.0.3/tests/test_locale.py`

 * *Files identical despite different names*

### Comparing `yadg-5.0.2/tests/test_masstrace.py` & `yadg-5.0.3/tests/test_masstrace.py`

 * *Files identical despite different names*

### Comparing `yadg-5.0.2/tests/test_meascsv.py` & `yadg-5.0.3/tests/test_meascsv.py`

 * *Files identical despite different names*

### Comparing `yadg-5.0.2/tests/test_preset.py` & `yadg-5.0.3/tests/test_preset.py`

 * *Files identical despite different names*

### Comparing `yadg-5.0.2/tests/test_qftrace.py` & `yadg-5.0.3/tests/test_qftrace.py`

 * *Files identical despite different names*

### Comparing `yadg-5.0.2/tests/test_timezones.py` & `yadg-5.0.3/tests/test_timezones.py`

 * *Files identical despite different names*

### Comparing `yadg-5.0.2/tests/test_xpstrace.py` & `yadg-5.0.3/tests/test_xpstrace.py`

 * *Files identical despite different names*

### Comparing `yadg-5.0.2/tests/test_xrdtrace.py` & `yadg-5.0.3/tests/test_xrdtrace.py`

 * *Files identical despite different names*

### Comparing `yadg-5.0.2/tests/test_yadg.py` & `yadg-5.0.3/tests/test_yadg.py`

 * *Files identical despite different names*

### Comparing `yadg-5.0.2/versioneer.py` & `yadg-5.0.3/versioneer.py`

 * *Files 0% similar despite different names*

```diff
@@ -427,17 +427,15 @@
         if verbose:
             print("unable to run %s (error)" % dispcmd)
             print("stdout was %s" % stdout)
         return None, process.returncode
     return stdout, process.returncode
 
 
-LONG_VERSION_PY[
-    "git"
-] = r'''
+LONG_VERSION_PY["git"] = r'''
 # This file helps to compute a version number in source trees obtained from
 # git-archive tarball (such as those provided by githubs download-from-tag
 # feature). Distribution tarballs (built by setup.py sdist) and build
 # directories (produced by setup.py build) will contain a much shorter file
 # that just contains the computed version number.
 
 # This file is released into the public domain. Generated by
```

