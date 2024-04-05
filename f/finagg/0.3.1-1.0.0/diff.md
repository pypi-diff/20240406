# Comparing `tmp/finagg-0.3.1.tar.gz` & `tmp/finagg-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finagg-0.3.1.tar", last modified: Sat Sep 23 01:36:06 2023, max compression
+gzip compressed data, was "finagg-1.0.0.tar", last modified: Fri Apr  5 23:04:20 2024, max compression
```

## Comparing `finagg-0.3.1.tar` & `finagg-1.0.0.tar`

### file list

```diff
@@ -1,127 +1,128 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-23 01:36:06.760758 finagg-0.3.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-23 01:36:06.740758 finagg-0.3.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-23 01:36:06.744758 finagg-0.3.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      916 2023-09-23 01:35:48.000000 finagg-0.3.1/.github/workflows/build-docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      737 2023-09-23 01:35:48.000000 finagg-0.3.1/.github/workflows/test-and-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      894 2023-09-23 01:35:48.000000 finagg-0.3.1/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1896 2023-09-23 01:35:48.000000 finagg-0.3.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      694 2023-09-23 01:35:48.000000 finagg-0.3.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2023-09-23 01:35:48.000000 finagg-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    27775 2023-09-23 01:36:06.760758 finagg-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13086 2023-09-23 01:35:48.000000 finagg-0.3.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-23 01:36:06.748758 finagg-0.3.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-23 01:35:48.000000 finagg-0.3.1/docs/.nojekyll
--rw-r--r--   0 runner    (1001) docker     (127)      635 2023-09-23 01:35:48.000000 finagg-0.3.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-23 01:36:06.748758 finagg-0.3.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)      480 2023-09-23 01:35:48.000000 finagg-0.3.1/docs/_static/custom.css
--rw-r--r--   0 runner    (1001) docker     (127)      639 2023-09-23 01:35:48.000000 finagg-0.3.1/docs/cli.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4239 2023-09-23 01:35:48.000000 finagg-0.3.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2134 2023-09-23 01:35:48.000000 finagg-0.3.1/docs/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (127)     9830 2023-09-23 01:35:48.000000 finagg-0.3.1/docs/conventions.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1895 2023-09-23 01:35:48.000000 finagg-0.3.1/docs/faq.rst
--rw-r--r--   0 runner    (1001) docker     (127)       71 2023-09-23 01:35:48.000000 finagg-0.3.1/docs/index.html
--rw-r--r--   0 runner    (1001) docker     (127)     8615 2023-09-23 01:35:48.000000 finagg-0.3.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1255 2023-09-23 01:35:48.000000 finagg-0.3.1/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)      799 2023-09-23 01:35:48.000000 finagg-0.3.1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)     1842 2023-09-23 01:35:48.000000 finagg-0.3.1/docs/references.rst
--rw-r--r--   0 runner    (1001) docker     (127)       87 2023-09-23 01:35:48.000000 finagg-0.3.1/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)    16306 2023-09-23 01:35:48.000000 finagg-0.3.1/docs/walkthroughs.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4193 2023-09-23 01:35:48.000000 finagg-0.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-23 01:36:06.760758 finagg-0.3.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-23 01:36:06.740758 finagg-0.3.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-23 01:36:06.748758 finagg-0.3.1/src/finagg/
--rw-r--r--   0 runner    (1001) docker     (127)      301 2023-09-23 01:35:48.000000 finagg-0.3.1/src/finagg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7791 2023-09-23 01:35:48.000000 finagg-0.3.1/src/finagg/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2256 2023-09-23 01:35:48.000000 finagg-0.3.1/src/finagg/backend.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-23 01:36:06.748758 finagg-0.3.1/src/finagg/bea/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2023-09-23 01:35:48.000000 finagg-0.3.1/src/finagg/bea/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1046 2023-09-23 01:35:48.000000 finagg-0.3.1/src/finagg/bea/_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    21084 2023-09-23 01:35:48.000000 finagg-0.3.1/src/finagg/bea/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2459 2023-09-23 01:35:48.000000 finagg-0.3.1/src/finagg/bea/sql.py
--rw-r--r--   0 runner    (1001) docker     (127)     6691 2023-09-23 01:35:48.000000 finagg-0.3.1/src/finagg/frame.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-23 01:36:06.748758 finagg-0.3.1/src/finagg/fred/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2023-09-23 01:35:48.000000 finagg-0.3.1/src/finagg/fred/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5490 2023-09-23 01:35:48.000000 finagg-0.3.1/src/finagg/fred/_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-23 01:36:06.752758 finagg-0.3.1/src/finagg/fred/api/
--rw-r--r--   0 runner    (1001) docker     (127)     3592 2023-09-23 01:35:48.000000 finagg-0.3.1/src/finagg/fred/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2772 2023-09-23 01:35:48.000000 finagg-0.3.1/src/finagg/fred/api/_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    18380 2023-09-23 01:35:48.000000 finagg-0.3.1/src/finagg/fred/api/_category.py
--rw-r--r--   0 runner    (1001) docker     (127)    22359 2023-09-23 01:35:48.000000 finagg-0.3.1/src/finagg/fred/api/_release.py
--rw-r--r--   0 runner    (1001) docker     (127)    40143 2023-09-23 01:35:48.000000 finagg-0.3.1/src/finagg/fred/api/_series.py
--rw-r--r--   0 runner    (1001) docker     (127)     8459 2023-09-23 01:35:48.000000 finagg-0.3.1/src/finagg/fred/api/_source.py
--rw-r--r--   0 runner    (1001) docker     (127)    11198 2023-09-23 01:35:48.000000 finagg-0.3.1/src/finagg/fred/api/_tags.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-23 01:36:06.752758 finagg-0.3.1/src/finagg/fred/feat/
--rw-r--r--   0 runner    (1001) docker     (127)      400 2023-09-23 01:35:48.000000 finagg-0.3.1/src/finagg/fred/feat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6696 2023-09-23 01:35:48.000000 finagg-0.3.1/src/finagg/fred/feat/_raw.py
--rw-r--r--   0 runner    (1001) docker     (127)    10806 2023-09-23 01:35:48.000000 finagg-0.3.1/src/finagg/fred/feat/_refined.py
--rw-r--r--   0 runner    (1001) docker     (127)     3935 2023-09-23 01:35:48.000000 finagg-0.3.1/src/finagg/fred/sql.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-23 01:36:06.752758 finagg-0.3.1/src/finagg/fundam/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2023-09-23 01:35:48.000000 finagg-0.3.1/src/finagg/fundam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3224 2023-09-23 01:35:48.000000 finagg-0.3.1/src/finagg/fundam/_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    35214 2023-09-23 01:35:48.000000 finagg-0.3.1/src/finagg/fundam/feat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2142 2023-09-23 01:35:48.000000 finagg-0.3.1/src/finagg/fundam/sql.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-23 01:36:06.752758 finagg-0.3.1/src/finagg/indices/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2023-09-23 01:35:48.000000 finagg-0.3.1/src/finagg/indices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2992 2023-09-23 01:35:48.000000 finagg-0.3.1/src/finagg/indices/_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     8168 2023-09-23 01:35:48.000000 finagg-0.3.1/src/finagg/indices/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3056 2023-09-23 01:35:48.000000 finagg-0.3.1/src/finagg/indices/sql.py
--rw-r--r--   0 runner    (1001) docker     (127)    14388 2023-09-23 01:35:48.000000 finagg-0.3.1/src/finagg/portfolio.py
--rw-r--r--   0 runner    (1001) docker     (127)     9160 2023-09-23 01:35:48.000000 finagg-0.3.1/src/finagg/ratelimit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-23 01:36:06.752758 finagg-0.3.1/src/finagg/sec/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2023-09-23 01:35:48.000000 finagg-0.3.1/src/finagg/sec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8372 2023-09-23 01:35:48.000000 finagg-0.3.1/src/finagg/sec/_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    38280 2023-09-23 01:35:48.000000 finagg-0.3.1/src/finagg/sec/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-23 01:36:06.752758 finagg-0.3.1/src/finagg/sec/feat/
--rw-r--r--   0 runner    (1001) docker     (127)      920 2023-09-23 01:35:48.000000 finagg-0.3.1/src/finagg/sec/feat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25769 2023-09-23 01:35:48.000000 finagg-0.3.1/src/finagg/sec/feat/_raw.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-23 01:36:06.752758 finagg-0.3.1/src/finagg/sec/feat/_refined/
--rw-r--r--   0 runner    (1001) docker     (127)      201 2023-09-23 01:35:48.000000 finagg-0.3.1/src/finagg/sec/feat/_refined/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    39780 2023-09-23 01:35:48.000000 finagg-0.3.1/src/finagg/sec/feat/_refined/annual.py
--rw-r--r--   0 runner    (1001) docker     (127)    40926 2023-09-23 01:35:48.000000 finagg-0.3.1/src/finagg/sec/feat/_refined/quarterly.py
--rw-r--r--   0 runner    (1001) docker     (127)    25535 2023-09-23 01:35:48.000000 finagg-0.3.1/src/finagg/sec/sql.py
--rw-r--r--   0 runner    (1001) docker     (127)     1800 2023-09-23 01:35:48.000000 finagg-0.3.1/src/finagg/testing.py
--rw-r--r--   0 runner    (1001) docker     (127)    12787 2023-09-23 01:35:48.000000 finagg-0.3.1/src/finagg/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-23 01:36:06.756758 finagg-0.3.1/src/finagg/yfinance/
--rw-r--r--   0 runner    (1001) docker     (127)       72 2023-09-23 01:35:48.000000 finagg-0.3.1/src/finagg/yfinance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5724 2023-09-23 01:35:48.000000 finagg-0.3.1/src/finagg/yfinance/_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2109 2023-09-23 01:35:48.000000 finagg-0.3.1/src/finagg/yfinance/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-23 01:36:06.756758 finagg-0.3.1/src/finagg/yfinance/feat/
--rw-r--r--   0 runner    (1001) docker     (127)      381 2023-09-23 01:35:48.000000 finagg-0.3.1/src/finagg/yfinance/feat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8629 2023-09-23 01:35:48.000000 finagg-0.3.1/src/finagg/yfinance/feat/_raw.py
--rw-r--r--   0 runner    (1001) docker     (127)    14234 2023-09-23 01:35:48.000000 finagg-0.3.1/src/finagg/yfinance/feat/_refined.py
--rw-r--r--   0 runner    (1001) docker     (127)     3173 2023-09-23 01:35:48.000000 finagg-0.3.1/src/finagg/yfinance/sql.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-23 01:36:06.748758 finagg-0.3.1/src/finagg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    27775 2023-09-23 01:36:06.000000 finagg-0.3.1/src/finagg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2586 2023-09-23 01:36:06.000000 finagg-0.3.1/src/finagg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-23 01:36:06.000000 finagg-0.3.1/src/finagg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2023-09-23 01:36:06.000000 finagg-0.3.1/src/finagg.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      314 2023-09-23 01:36:06.000000 finagg-0.3.1/src/finagg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2023-09-23 01:36:06.000000 finagg-0.3.1/src/finagg.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-23 01:36:06.756758 finagg-0.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-23 01:35:48.000000 finagg-0.3.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-23 01:36:06.756758 finagg-0.3.1/tests/test_bea/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-23 01:35:48.000000 finagg-0.3.1/tests/test_bea/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      432 2023-09-23 01:35:48.000000 finagg-0.3.1/tests/test_bea/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     4023 2023-09-23 01:35:48.000000 finagg-0.3.1/tests/test_frame.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-23 01:36:06.756758 finagg-0.3.1/tests/test_fred/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-23 01:35:48.000000 finagg-0.3.1/tests/test_fred/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      480 2023-09-23 01:35:48.000000 finagg-0.3.1/tests/test_fred/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2023-09-23 01:35:48.000000 finagg-0.3.1/tests/test_fred/test_feat.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-23 01:36:06.756758 finagg-0.3.1/tests/test_fundam/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-23 01:35:48.000000 finagg-0.3.1/tests/test_fundam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2103 2023-09-23 01:35:48.000000 finagg-0.3.1/tests/test_fundam/test_feat.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-23 01:36:06.756758 finagg-0.3.1/tests/test_indices/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-23 01:35:48.000000 finagg-0.3.1/tests/test_indices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      298 2023-09-23 01:35:48.000000 finagg-0.3.1/tests/test_indices/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3278 2023-09-23 01:35:48.000000 finagg-0.3.1/tests/test_portfolio.py
--rw-r--r--   0 runner    (1001) docker     (127)     2559 2023-09-23 01:35:48.000000 finagg-0.3.1/tests/test_ratelimit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-23 01:36:06.756758 finagg-0.3.1/tests/test_sec/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-23 01:35:48.000000 finagg-0.3.1/tests/test_sec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      351 2023-09-23 01:35:48.000000 finagg-0.3.1/tests/test_sec/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     4494 2023-09-23 01:35:48.000000 finagg-0.3.1/tests/test_sec/test_feat.py
--rw-r--r--   0 runner    (1001) docker     (127)     1285 2023-09-23 01:35:48.000000 finagg-0.3.1/tests/test_sec/test_sql.py
--rw-r--r--   0 runner    (1001) docker     (127)     2965 2023-09-23 01:35:48.000000 finagg-0.3.1/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-23 01:36:06.756758 finagg-0.3.1/tests/test_yfinance/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-23 01:35:48.000000 finagg-0.3.1/tests/test_yfinance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       76 2023-09-23 01:35:48.000000 finagg-0.3.1/tests/test_yfinance/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2382 2023-09-23 01:35:48.000000 finagg-0.3.1/tests/test_yfinance/test_feat.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 23:04:20.961888 finagg-1.0.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 23:04:20.933888 finagg-1.0.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 23:04:20.937888 finagg-1.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      916 2024-04-05 23:04:12.000000 finagg-1.0.0/.github/workflows/build-docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-05 23:04:12.000000 finagg-1.0.0/.github/workflows/test-and-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-05 23:04:12.000000 finagg-1.0.0/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-04-05 23:04:12.000000 finagg-1.0.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-05 23:04:12.000000 finagg-1.0.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-05 23:04:12.000000 finagg-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    27173 2024-04-05 23:04:20.957888 finagg-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12481 2024-04-05 23:04:12.000000 finagg-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 23:04:20.941888 finagg-1.0.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 23:04:12.000000 finagg-1.0.0/docs/.nojekyll
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-04-05 23:04:12.000000 finagg-1.0.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 23:04:20.941888 finagg-1.0.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-05 23:04:12.000000 finagg-1.0.0/docs/_static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-05 23:04:12.000000 finagg-1.0.0/docs/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4239 2024-04-05 23:04:12.000000 finagg-1.0.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-04-05 23:04:12.000000 finagg-1.0.0/docs/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9636 2024-04-05 23:04:12.000000 finagg-1.0.0/docs/conventions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1895 2024-04-05 23:04:12.000000 finagg-1.0.0/docs/faq.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-05 23:04:12.000000 finagg-1.0.0/docs/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     8648 2024-04-05 23:04:12.000000 finagg-1.0.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-04-05 23:04:12.000000 finagg-1.0.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-04-05 23:04:12.000000 finagg-1.0.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-04-05 23:04:12.000000 finagg-1.0.0/docs/references.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-04-05 23:04:12.000000 finagg-1.0.0/docs/release_notes.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-05 23:04:12.000000 finagg-1.0.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    16494 2024-04-05 23:04:12.000000 finagg-1.0.0/docs/walkthroughs.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4192 2024-04-05 23:04:12.000000 finagg-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 23:04:20.961888 finagg-1.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 23:04:20.933888 finagg-1.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 23:04:20.945888 finagg-1.0.0/src/finagg/
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-05 23:04:12.000000 finagg-1.0.0/src/finagg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7791 2024-04-05 23:04:12.000000 finagg-1.0.0/src/finagg/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2256 2024-04-05 23:04:12.000000 finagg-1.0.0/src/finagg/backend.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 23:04:20.945888 finagg-1.0.0/src/finagg/bea/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-05 23:04:12.000000 finagg-1.0.0/src/finagg/bea/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-04-05 23:04:12.000000 finagg-1.0.0/src/finagg/bea/_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21084 2024-04-05 23:04:12.000000 finagg-1.0.0/src/finagg/bea/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-04-05 23:04:12.000000 finagg-1.0.0/src/finagg/bea/sql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6696 2024-04-05 23:04:12.000000 finagg-1.0.0/src/finagg/frame.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 23:04:20.945888 finagg-1.0.0/src/finagg/fred/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-05 23:04:12.000000 finagg-1.0.0/src/finagg/fred/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5486 2024-04-05 23:04:12.000000 finagg-1.0.0/src/finagg/fred/_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 23:04:20.949888 finagg-1.0.0/src/finagg/fred/api/
+-rw-r--r--   0 runner    (1001) docker     (127)     3592 2024-04-05 23:04:12.000000 finagg-1.0.0/src/finagg/fred/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3803 2024-04-05 23:04:12.000000 finagg-1.0.0/src/finagg/fred/api/_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18869 2024-04-05 23:04:12.000000 finagg-1.0.0/src/finagg/fred/api/_category.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23337 2024-04-05 23:04:12.000000 finagg-1.0.0/src/finagg/fred/api/_release.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41472 2024-04-05 23:04:12.000000 finagg-1.0.0/src/finagg/fred/api/_series.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8785 2024-04-05 23:04:12.000000 finagg-1.0.0/src/finagg/fred/api/_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11656 2024-04-05 23:04:12.000000 finagg-1.0.0/src/finagg/fred/api/_tags.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 23:04:20.949888 finagg-1.0.0/src/finagg/fred/feat/
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-05 23:04:12.000000 finagg-1.0.0/src/finagg/fred/feat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6696 2024-04-05 23:04:12.000000 finagg-1.0.0/src/finagg/fred/feat/_raw.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10791 2024-04-05 23:04:12.000000 finagg-1.0.0/src/finagg/fred/feat/_refined.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3935 2024-04-05 23:04:12.000000 finagg-1.0.0/src/finagg/fred/sql.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 23:04:20.949888 finagg-1.0.0/src/finagg/fundam/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-05 23:04:12.000000 finagg-1.0.0/src/finagg/fundam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3220 2024-04-05 23:04:12.000000 finagg-1.0.0/src/finagg/fundam/_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35182 2024-04-05 23:04:12.000000 finagg-1.0.0/src/finagg/fundam/feat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-04-05 23:04:12.000000 finagg-1.0.0/src/finagg/fundam/sql.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 23:04:20.949888 finagg-1.0.0/src/finagg/indices/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-05 23:04:12.000000 finagg-1.0.0/src/finagg/indices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2992 2024-04-05 23:04:12.000000 finagg-1.0.0/src/finagg/indices/_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8289 2024-04-05 23:04:12.000000 finagg-1.0.0/src/finagg/indices/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3056 2024-04-05 23:04:12.000000 finagg-1.0.0/src/finagg/indices/sql.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14390 2024-04-05 23:04:12.000000 finagg-1.0.0/src/finagg/portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9160 2024-04-05 23:04:12.000000 finagg-1.0.0/src/finagg/ratelimit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 23:04:20.949888 finagg-1.0.0/src/finagg/sec/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-05 23:04:12.000000 finagg-1.0.0/src/finagg/sec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8368 2024-04-05 23:04:12.000000 finagg-1.0.0/src/finagg/sec/_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39411 2024-04-05 23:04:12.000000 finagg-1.0.0/src/finagg/sec/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 23:04:20.949888 finagg-1.0.0/src/finagg/sec/feat/
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-04-05 23:04:12.000000 finagg-1.0.0/src/finagg/sec/feat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25931 2024-04-05 23:04:12.000000 finagg-1.0.0/src/finagg/sec/feat/_raw.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 23:04:20.953888 finagg-1.0.0/src/finagg/sec/feat/_refined/
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-05 23:04:12.000000 finagg-1.0.0/src/finagg/sec/feat/_refined/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39834 2024-04-05 23:04:12.000000 finagg-1.0.0/src/finagg/sec/feat/_refined/annual.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40980 2024-04-05 23:04:12.000000 finagg-1.0.0/src/finagg/sec/feat/_refined/quarterly.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25535 2024-04-05 23:04:12.000000 finagg-1.0.0/src/finagg/sec/sql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-04-05 23:04:12.000000 finagg-1.0.0/src/finagg/testing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12757 2024-04-05 23:04:12.000000 finagg-1.0.0/src/finagg/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 23:04:20.953888 finagg-1.0.0/src/finagg/yfinance/
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-05 23:04:12.000000 finagg-1.0.0/src/finagg/yfinance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9013 2024-04-05 23:04:12.000000 finagg-1.0.0/src/finagg/yfinance/_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2472 2024-04-05 23:04:12.000000 finagg-1.0.0/src/finagg/yfinance/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 23:04:20.953888 finagg-1.0.0/src/finagg/yfinance/feat/
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-05 23:04:12.000000 finagg-1.0.0/src/finagg/yfinance/feat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11503 2024-04-05 23:04:12.000000 finagg-1.0.0/src/finagg/yfinance/feat/_raw.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16476 2024-04-05 23:04:12.000000 finagg-1.0.0/src/finagg/yfinance/feat/_refined.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3175 2024-04-05 23:04:12.000000 finagg-1.0.0/src/finagg/yfinance/sql.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 23:04:20.957888 finagg-1.0.0/src/finagg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    27173 2024-04-05 23:04:20.000000 finagg-1.0.0/src/finagg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2608 2024-04-05 23:04:20.000000 finagg-1.0.0/src/finagg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 23:04:20.000000 finagg-1.0.0/src/finagg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-05 23:04:20.000000 finagg-1.0.0/src/finagg.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-05 23:04:20.000000 finagg-1.0.0/src/finagg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-05 23:04:20.000000 finagg-1.0.0/src/finagg.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 23:04:20.953888 finagg-1.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 23:04:12.000000 finagg-1.0.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 23:04:20.953888 finagg-1.0.0/tests/test_bea/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 23:04:12.000000 finagg-1.0.0/tests/test_bea/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-05 23:04:12.000000 finagg-1.0.0/tests/test_bea/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4023 2024-04-05 23:04:12.000000 finagg-1.0.0/tests/test_frame.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 23:04:20.957888 finagg-1.0.0/tests/test_fred/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 23:04:12.000000 finagg-1.0.0/tests/test_fred/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-05 23:04:12.000000 finagg-1.0.0/tests/test_fred/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-04-05 23:04:12.000000 finagg-1.0.0/tests/test_fred/test_feat.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 23:04:20.957888 finagg-1.0.0/tests/test_fundam/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 23:04:12.000000 finagg-1.0.0/tests/test_fundam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-04-05 23:04:12.000000 finagg-1.0.0/tests/test_fundam/test_feat.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 23:04:20.957888 finagg-1.0.0/tests/test_indices/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 23:04:12.000000 finagg-1.0.0/tests/test_indices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-05 23:04:12.000000 finagg-1.0.0/tests/test_indices/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3278 2024-04-05 23:04:12.000000 finagg-1.0.0/tests/test_portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2559 2024-04-05 23:04:12.000000 finagg-1.0.0/tests/test_ratelimit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 23:04:20.957888 finagg-1.0.0/tests/test_sec/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 23:04:12.000000 finagg-1.0.0/tests/test_sec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-05 23:04:12.000000 finagg-1.0.0/tests/test_sec/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4494 2024-04-05 23:04:12.000000 finagg-1.0.0/tests/test_sec/test_feat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-04-05 23:04:12.000000 finagg-1.0.0/tests/test_sec/test_sql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2965 2024-04-05 23:04:12.000000 finagg-1.0.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 23:04:20.957888 finagg-1.0.0/tests/test_yfinance/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 23:04:12.000000 finagg-1.0.0/tests/test_yfinance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-05 23:04:12.000000 finagg-1.0.0/tests/test_yfinance/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3868 2024-04-05 23:04:12.000000 finagg-1.0.0/tests/test_yfinance/test_feat.py
```

### Comparing `finagg-0.3.1/.github/workflows/build-docs.yml` & `finagg-1.0.0/.github/workflows/build-docs.yml`

 * *Files identical despite different names*

### Comparing `finagg-0.3.1/.github/workflows/test-and-publish.yml` & `finagg-1.0.0/.github/workflows/test-and-publish.yml`

 * *Files identical despite different names*

### Comparing `finagg-0.3.1/.github/workflows/test.yml` & `finagg-1.0.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `finagg-0.3.1/.gitignore` & `finagg-1.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `finagg-0.3.1/.pre-commit-config.yaml` & `finagg-1.0.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `finagg-0.3.1/LICENSE` & `finagg-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `finagg-0.3.1/PKG-INFO` & `finagg-1.0.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finagg
-Version: 0.3.1
+Version: 1.0.0
 Summary: Data aggregation with popular and free financial APIs.
 Author: Andrew B.
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -216,20 +216,20 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Office/Business :: Financial :: Investment
 Classifier: Topic :: Software Development
 Classifier: Topic :: Scientific/Engineering
 Classifier: Typing :: Typed
 Requires-Python: >=3.10
-Description-Content-Type: text/x-rst
+Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: beautifulsoup4==4.*
 Requires-Dist: click==8.*
-Requires-Dist: pandas==1.*
-Requires-Dist: pandas-stubs==1.*
+Requires-Dist: pandas==2.*
+Requires-Dist: pandas-stubs==2.*
 Requires-Dist: python-dotenv==0.21.*
 Requires-Dist: requests==2.*
 Requires-Dist: requests-cache==0.9.*
 Requires-Dist: SQLAlchemy==2.*
 Requires-Dist: tqdm==4.*
 Requires-Dist: types-requests==2.*
 Requires-Dist: typing-extensions==4.*
@@ -242,304 +242,306 @@
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: pytest-xdist; extra == "dev"
 Requires-Dist: pytest-randomly; extra == "dev"
 Requires-Dist: sphinx; extra == "dev"
 Requires-Dist: tox; extra == "dev"
 Requires-Dist: virtualenv; extra == "dev"
 
-finagg: Financial Aggregation for Python
-========================================
+# finagg: Financial Aggregation for Python
 
 **finagg** is a Python package that provides implementations of popular and free
 financial APIs, tools for aggregating historical data from those APIs into SQL
 databases, and tools for transforming aggregated data into features useful for
 analysis and AI/ML.
 
 * **Documentation**: https://theogognf.github.io/finagg/
 * **PyPI**: https://pypi.org/project/finagg/
 * **Repository**: https://github.com/theOGognf/finagg
 
-Quick Start
-===========
+# Quick Start
 
-Installation
-------------
+## Installation
 
-Install with pip for the latest (stable) version.
+Install with pip for the latest stable version.
 
-.. code:: console
+```console
+pip install finagg
+```
 
-  pip install finagg
+Install from GitHub for the latest unstable version.
 
-Install from GitHub for the latest (unstable) version.
-
-.. code:: console
-
-    git clone https://github.com/theOGognf/finagg.git
-    pip install ./finagg/
+```console
+git clone https://github.com/theOGognf/finagg.git
+pip install ./finagg/
+```
 
 Optionally install the recommended datasets (economic data, company
 financials, stock histories, etc.) from 3rd party APIs into a local SQL
 database.
 
-.. code:: console
-
-    finagg install -ss economic -ts indices -z -r
+```console
+finagg install -ss economic -ts indices -z -r
+```
 
 The installation will point you where to get free API keys for each API that
 requires one and will write those API keys to a local ``.env`` file for storage.
 Run ``finagg install --help`` for more installation options and details.
 
-Basic Usage
------------
+## Basic Usage
 
-These are just **finagg** usage samples. See the `documentation`_ for all the
+These are just **finagg** usage samples. See the [documentation][4] for all the
 supported APIs and features.
 
-Explore the APIs directly
-^^^^^^^^^^^^^^^^^^^^^^^^^
+### Explore the APIs directly
 
 *These methods require internet access and API keys/user agent declarations.*
 
 Get Bureau of Economic Analysis (BEA) data.
 
+```pycon
 >>> finagg.bea.api.gdp_by_industry.get(year=[2019]).head(5)
    table_id freq  year quarter industry                         industry_description ...
 0         1    Q  2019       1       11  Agriculture, forestry, fishing, and hunting ...
 1         1    Q  2019       1    111CA                                        Farms ...
 2         1    Q  2019       1    113FF    Forestry, fishing, and related activities ...
 3         1    Q  2019       1       21                                       Mining ...
 4         1    Q  2019       1      211                       Oil and gas extraction ...
+```
 
 Get Federal Reserve Economic Data (FRED).
 
+```pycon
 >>> finagg.fred.api.series.observations.get(
 ...   "CPIAUCNS",
 ...   realtime_start=0,
 ...   realtime_end=-1,
 ...   output_type=4
 ... ).head(5)
   realtime_start realtime_end        date  value series_id
 0     1949-04-22   1953-02-26  1949-03-01  169.5  CPIAUCNS
 1     1949-05-23   1953-02-26  1949-04-01  169.7  CPIAUCNS
 2     1949-06-24   1953-02-26  1949-05-01  169.2  CPIAUCNS
 3     1949-07-22   1953-02-26  1949-06-01  169.6  CPIAUCNS
 4     1949-08-26   1953-02-26  1949-07-01  168.5  CPIAUCNS
+```
 
 Get Securities and Exchange Commission (SEC) filings.
 
+```pycon
 >>> finagg.sec.api.company_facts.get(ticker="AAPL").head(5)
           end        value                  accn    fy  fp    form       filed ...
 0  2009-06-27  895816758.0  0001193125-09-153165  2009  Q3    10-Q  2009-07-22 ...
 1  2009-10-16  900678473.0  0001193125-09-214859  2009  FY    10-K  2009-10-27 ...
 2  2009-10-16  900678473.0  0001193125-10-012091  2009  FY  10-K/A  2010-01-25 ...
 3  2010-01-15  906794589.0  0001193125-10-012085  2010  Q1    10-Q  2010-01-25 ...
 4  2010-04-09  909938383.0  0001193125-10-088957  2010  Q2    10-Q  2010-04-21 ...
+```
 
-Use installed raw data for exploring the most popular features
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+### Use installed raw data for exploring the most popular features
 
 *These methods require internet access, API keys/user agent declarations, and
 downloading and installing raw data through the* ``finagg install`` *or*
 ``finagg <api/subpackage> install`` *commands.*
 
 Get the most popular FRED features all in one dataframe.
 
+```pycon
 >>> finagg.fred.feat.economic.from_raw().head(5)
             CIVPART  LOG_CHANGE(CPIAUCNS)  LOG_CHANGE(CSUSHPINSA)  FEDFUNDS ...
 date                                                                        ...
 2014-10-06     62.8                   0.0                     0.0      0.09 ...
 2014-10-08     62.8                   0.0                     0.0      0.09 ...
 2014-10-13     62.8                   0.0                     0.0      0.09 ...
 2014-10-15     62.8                   0.0                     0.0      0.09 ...
 2014-10-20     62.8                   0.0                     0.0      0.09 ...
+```
 
 Get quarterly report features from SEC data.
 
+```pycon
 >>> finagg.sec.feat.quarterly.from_raw("AAPL").head(5)
                     LOG_CHANGE(Assets)  LOG_CHANGE(AssetsCurrent) ...
 fy   fp filed                                                     ...
 2010 Q1 2010-01-25            0.182629                  -0.023676 ...
      Q2 2010-04-21            0.000000                   0.000000 ...
      Q3 2010-07-21            0.000000                   0.000000 ...
 2011 Q1 2011-01-19            0.459174                   0.278241 ...
      Q2 2011-04-21            0.000000                   0.000000 ...
+```
 
 Get an aggregation of quarterly and daily features for a particular ticker.
 
+```pycon
 >>> finagg.fundam.feat.fundam.from_raw("AAPL").head(5)
             PriceBookRatio  PriceEarningsRatio
 date
 2010-01-25        0.175061            2.423509
 2010-01-26        0.178035            2.464678
 2010-01-27        0.178813            2.475448
 2010-01-28        0.177154            2.452471
 2010-01-29        0.173825            2.406396
+```
 
-Use installed features for exploring refined aggregations of raw data
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+### Use installed features for exploring refined aggregations of raw data
 
 *These methods require installing refined data through the* ``finagg install``
 *or* ``finagg <api/subpackage> install`` *commands.*
 
 Get a ticker's industry's averaged quarterly report features.
 
+```pycon
 >>> finagg.sec.feat.quarterly.industry.from_refined(ticker="AAPL").head(5)
                                  mean                           ...
 name               AssetCoverageRatio BookRatio DebtEquityRatio ...
 fy   fp filed                                                   ...
 2014 Q1 2014-05-15          10.731301  9.448954        0.158318 ...
      Q2 2014-08-14          10.731301  9.448954        0.158318 ...
      Q3 2014-11-14          10.731301  9.448954        0.158318 ...
 2015 Q1 2015-05-15          16.738972  9.269250        0.294238 ...
      Q2 2015-08-13          16.738972  9.269250        0.294238 ...
+```
 
 Get a ticker's industry-averaged quarterly report features.
 
+```pycon
 >>> finagg.sec.feat.quarterly.normalized.from_refined("AAPL").head(5)
                     NORM(LOG_CHANGE(Assets))  NORM(LOG_CHANGE(AssetsCurrent)) ...
 fy   fp filed                                                                 ...
 2010 Q2 2010-04-21                  0.000000                         0.000000 ...
      Q3 2010-07-21                  0.000000                         0.000000 ...
 2011 Q1 2011-01-19                  0.978816                         0.074032 ...
      Q2 2011-04-21                  0.000000                         0.000000 ...
      Q3 2011-07-20                 -0.353553                        -0.353553 ...
+```
 
 Get tickers sorted by an industry-averaged quarterly report feature.
 
+```pycon
 >>> finagg.sec.feat.quarterly.normalized.get_tickers_sorted_by(
 ...   "NORM(EarningsPerShareBasic)",
 ...   year=2019
 ... )[:5]
 ['XRAY', 'TSLA', 'SYY', 'WHR', 'KMB']
+```
 
 Get tickers sorted by an industry-averaged fundamental feature.
 
+```pycon
 >>> finagg.fundam.feat.fundam.normalized.get_tickers_sorted_by(
 ...   "NORM(PriceEarningsRatio)",
 ...   date="2019-01-04"
 ... )[:5]
 ['AMD', 'TRGP', 'HPE', 'CZR', 'TSLA']
+```
 
-Configuration
-=============
+# Configuration
 
-API Keys and User Agents
-------------------------
+## API Keys and User Agents
 
 API keys and user agent declarations are required for most of the APIs.
 You can set environment variables to expose your API keys and user agents
 to **finagg**, or you can pass your API keys and user agents to the implemented
 APIs programmatically. The following environment variables are used for
 configuring API keys and user agents:
 
 * ``BEA_API_KEY`` is for the Bureau of Economic Analysis's API key. You can get
-  a free API key from the `BEA API site`_.
+  a free API key from the [BEA API site][3].
 * ``FRED_API_KEY`` is for the Federal Reserve Economic Data API key. You can get
-  a free API key from the `FRED API site`_.
+  a free API key from the [FRED API site][8].
 * ``INDICES_API_USER_AGENT`` is for scraping popular indices' compositions from
   Wikipedia and should be equivalent to a browser's user agent declaration.
   This defaults to a hardcoded value, but it may not always work.
 * ``SEC_API_USER_AGENT`` is for the Securities and Exchange Commission's API. This
   should be of the format ``FIRST_NAME LAST_NAME E_MAIL``.
 
-Data Locations
---------------
+## Data Locations
 
 **finagg**'s root path, HTTP cache path, and database path are all configurable
 through environment variables. By default, all data related to **finagg** is put
 in a ``./findata`` directory relative to a root directory. You can change these
 locations by modifying the respective environment variables:
 
 * ``FINAGG_ROOT_PATH`` points to the parent directory of the ``./findata`` directory.
   Defaults to your current working directory.
 * ``FINAGG_HTTP_CACHE_PATH`` points to the HTTP requests cache SQLite storage.
   Defaults to ``./findata/http_cache.sqlite``.
 * ``FINAGG_DATABASE_URL`` points to the **finagg** data storage. Defaults to
   ``./findata/finagg.sqlite``.
 
-Dependencies
-============
+# Dependencies
 
-* `pandas`_ for fast, flexible, and expressive representations of relational data.
-* `requests`_ for HTTP requests to 3rd party APIs.
-* `requests-cache`_ for caching HTTP requests to avoid getting throttled by 3rd
+* [pandas][11] for fast, flexible, and expressive representations of relational data.
+* [requests][12] for HTTP requests to 3rd party APIs.
+* [requests-cache][13] for caching HTTP requests to avoid getting throttled by 3rd
   party API servers.
-* `SQLAlchemy`_ for a SQL Python interface.
-* `yfinance`_ for historical stock data from Yahoo! Finance.
+* [SQLAlchemy][17] for a SQL Python interface.
+* [yfinance][18] for historical stock data from Yahoo! Finance.
 
-API References
-==============
+# API References
 
-* The `BEA API`_ and the `BEA API key registration link`_.
-* The `FRED API`_ and the `FRED API key registration link`_.
-* The `SEC API`_.
+* The [BEA API][1] and the [BEA API key registration link][2].
+* The [FRED API][6] and the [FRED API key registration link][7].
+* The [SEC API][14].
 
-Related Projects
-================
+# Related Projects
 
-* `FinRL`_ is a collection of financial reinforcement learning environments
+* [FinRL][5] is a collection of financial reinforcement learning environments
   and tools.
-* `fredapi`_ is an implementation of the FRED API.
-* `OpenBBTerminal`_ is an open-source version of the Bloomberg Terminal.
-* `sec-edgar`_ is an implementation of a file-based SEC EDGAR parser.
-* `sec-edgar-api`_ is an implementation of the SEC EDGAR REST API.
+* [fredapi][9] is an implementation of the FRED API.
+* [OpenBBTerminal][10] is an open-source version of the Bloomberg Terminal.
+* [sec-edgar][15] is an implementation of a file-based SEC EDGAR parser.
+* [sec-edgar-api][16] is an implementation of the SEC EDGAR REST API.
 
-Frequently Asked Questions
-==========================
+# Frequently Asked Questions
 
-Where should I start?
----------------------
+## Where should I start?
 
 Aggregate some data, create some analysis notebooks, or create some RL
 environments using the implemented data features and SQL tables. This
 project was originally created to make RL environments for financial
 applications but has since focused its purpose to just aggregating financial
 data and features. That being said, all the implemented features are
 defined in such a way to make it very easy to develop financial AI/ML,
 so we encourage you to do just that!
 
-Why aren't features being installed for a specific ticker or economic data series?
-----------------------------------------------------------------------------------
+## Why aren't features being installed for a specific ticker or economic data series?
 
 Implemented APIs may be relatively new and simply may not provide data for a
 particular ticker or economic data series. For example, earnings per share may
 not be accessible for all companies through the SEC EDGAR API. In some cases,
 APIs may raise an HTTP error, causing installations to skip the ticker or
 series. Additionally, not all tickers and economic data series contain
 sufficient data for feature normalization. If a ticker or series only has one
 data point, that data point could be dropped when computing a feature (such as
 percent change), causing no data to be installed.
 
-What Python versions are supported?
------------------------------------
+## What Python versions are supported?
 
 Python 3.10 and up are supported. We don't plan on supporting lower versions
 because 3.10 introduces some nice quality of life updates that are used
 throughout the package.
 
-What operating systems are supported?
--------------------------------------
+## What operating systems are supported?
 
 The package is developed and tested on both Linux and Windows, but we recommend
 using Linux or WSL in practice. The package performs a good amount of I/O and
 interprocess operations that could result in a noticeable performance
 degradation on Windows.
 
-.. _`BEA API`: https://apps.bea.gov/api/signup/
-.. _`BEA API key registration link`: https://apps.bea.gov/API/signup/
-.. _`BEA API site`: https://apps.bea.gov/API/signup/
-.. _`documentation`: https://theogognf.github.io/finagg/
-.. _`FinRL`: https://github.com/AI4Finance-Foundation/FinRL
-.. _`FRED API`: https://fred.stlouisfed.org/docs/api/fred/
-.. _`FRED API key registration link`: https://fredaccount.stlouisfed.org/login/secure/
-.. _`FRED API site`: https://fredaccount.stlouisfed.org/login/secure/
-.. _`fredapi`: https://github.com/mortada/fredapi
-.. _`OpenBBTerminal`: https://github.com/OpenBB-finance/OpenBBTerminal
-.. _`pandas`: https://pandas.pydata.org/
-.. _`requests`: https://requests.readthedocs.io/en/latest/
-.. _`requests-cache`: https://requests-cache.readthedocs.io/en/stable/
-.. _`SEC API`: https://www.sec.gov/edgar/sec-api-documentation
-.. _`sec-edgar`: https://github.com/sec-edgar/sec-edgar
-.. _`sec-edgar-api`: https://github.com/jadchaar/sec-edgar-api
-.. _`SQLAlchemy`: https://www.sqlalchemy.org/
-.. _`yfinance`: https://github.com/ranaroussi/yfinance
+[1]: https://apps.bea.gov/api/signup/
+[2]: https://apps.bea.gov/API/signup/
+[3]: https://apps.bea.gov/API/signup/
+[4]: https://theogognf.github.io/finagg/
+[5]: https://github.com/AI4Finance-Foundation/FinRL
+[6]: https://fred.stlouisfed.org/docs/api/fred/
+[7]: https://fredaccount.stlouisfed.org/login/secure/
+[8]: https://fredaccount.stlouisfed.org/login/secure/
+[9]: https://github.com/mortada/fredapi
+[10]: https://github.com/OpenBB-finance/OpenBBTerminal
+[11]: https://pandas.pydata.org/
+[12]: https://requests.readthedocs.io/en/latest/
+[13]: https://requests-cache.readthedocs.io/en/stable/
+[14]: https://www.sec.gov/edgar/sec-api-documentation
+[15]: https://github.com/sec-edgar/sec-edgar
+[16]: https://github.com/jadchaar/sec-edgar-api
+[17]: https://www.sqlalchemy.org/
+[18]: https://github.com/ranaroussi/yfinance
```

### Comparing `finagg-0.3.1/README.rst` & `finagg-1.0.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,297 +1,299 @@
-finagg: Financial Aggregation for Python
-========================================
+# finagg: Financial Aggregation for Python
 
 **finagg** is a Python package that provides implementations of popular and free
 financial APIs, tools for aggregating historical data from those APIs into SQL
 databases, and tools for transforming aggregated data into features useful for
 analysis and AI/ML.
 
 * **Documentation**: https://theogognf.github.io/finagg/
 * **PyPI**: https://pypi.org/project/finagg/
 * **Repository**: https://github.com/theOGognf/finagg
 
-Quick Start
-===========
+# Quick Start
 
-Installation
-------------
+## Installation
 
-Install with pip for the latest (stable) version.
+Install with pip for the latest stable version.
 
-.. code:: console
+```console
+pip install finagg
+```
 
-  pip install finagg
+Install from GitHub for the latest unstable version.
 
-Install from GitHub for the latest (unstable) version.
-
-.. code:: console
-
-    git clone https://github.com/theOGognf/finagg.git
-    pip install ./finagg/
+```console
+git clone https://github.com/theOGognf/finagg.git
+pip install ./finagg/
+```
 
 Optionally install the recommended datasets (economic data, company
 financials, stock histories, etc.) from 3rd party APIs into a local SQL
 database.
 
-.. code:: console
-
-    finagg install -ss economic -ts indices -z -r
+```console
+finagg install -ss economic -ts indices -z -r
+```
 
 The installation will point you where to get free API keys for each API that
 requires one and will write those API keys to a local ``.env`` file for storage.
 Run ``finagg install --help`` for more installation options and details.
 
-Basic Usage
------------
+## Basic Usage
 
-These are just **finagg** usage samples. See the `documentation`_ for all the
+These are just **finagg** usage samples. See the [documentation][4] for all the
 supported APIs and features.
 
-Explore the APIs directly
-^^^^^^^^^^^^^^^^^^^^^^^^^
+### Explore the APIs directly
 
 *These methods require internet access and API keys/user agent declarations.*
 
 Get Bureau of Economic Analysis (BEA) data.
 
+```pycon
 >>> finagg.bea.api.gdp_by_industry.get(year=[2019]).head(5)
    table_id freq  year quarter industry                         industry_description ...
 0         1    Q  2019       1       11  Agriculture, forestry, fishing, and hunting ...
 1         1    Q  2019       1    111CA                                        Farms ...
 2         1    Q  2019       1    113FF    Forestry, fishing, and related activities ...
 3         1    Q  2019       1       21                                       Mining ...
 4         1    Q  2019       1      211                       Oil and gas extraction ...
+```
 
 Get Federal Reserve Economic Data (FRED).
 
+```pycon
 >>> finagg.fred.api.series.observations.get(
 ...   "CPIAUCNS",
 ...   realtime_start=0,
 ...   realtime_end=-1,
 ...   output_type=4
 ... ).head(5)
   realtime_start realtime_end        date  value series_id
 0     1949-04-22   1953-02-26  1949-03-01  169.5  CPIAUCNS
 1     1949-05-23   1953-02-26  1949-04-01  169.7  CPIAUCNS
 2     1949-06-24   1953-02-26  1949-05-01  169.2  CPIAUCNS
 3     1949-07-22   1953-02-26  1949-06-01  169.6  CPIAUCNS
 4     1949-08-26   1953-02-26  1949-07-01  168.5  CPIAUCNS
+```
 
 Get Securities and Exchange Commission (SEC) filings.
 
+```pycon
 >>> finagg.sec.api.company_facts.get(ticker="AAPL").head(5)
           end        value                  accn    fy  fp    form       filed ...
 0  2009-06-27  895816758.0  0001193125-09-153165  2009  Q3    10-Q  2009-07-22 ...
 1  2009-10-16  900678473.0  0001193125-09-214859  2009  FY    10-K  2009-10-27 ...
 2  2009-10-16  900678473.0  0001193125-10-012091  2009  FY  10-K/A  2010-01-25 ...
 3  2010-01-15  906794589.0  0001193125-10-012085  2010  Q1    10-Q  2010-01-25 ...
 4  2010-04-09  909938383.0  0001193125-10-088957  2010  Q2    10-Q  2010-04-21 ...
+```
 
-Use installed raw data for exploring the most popular features
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+### Use installed raw data for exploring the most popular features
 
 *These methods require internet access, API keys/user agent declarations, and
 downloading and installing raw data through the* ``finagg install`` *or*
 ``finagg <api/subpackage> install`` *commands.*
 
 Get the most popular FRED features all in one dataframe.
 
+```pycon
 >>> finagg.fred.feat.economic.from_raw().head(5)
             CIVPART  LOG_CHANGE(CPIAUCNS)  LOG_CHANGE(CSUSHPINSA)  FEDFUNDS ...
 date                                                                        ...
 2014-10-06     62.8                   0.0                     0.0      0.09 ...
 2014-10-08     62.8                   0.0                     0.0      0.09 ...
 2014-10-13     62.8                   0.0                     0.0      0.09 ...
 2014-10-15     62.8                   0.0                     0.0      0.09 ...
 2014-10-20     62.8                   0.0                     0.0      0.09 ...
+```
 
 Get quarterly report features from SEC data.
 
+```pycon
 >>> finagg.sec.feat.quarterly.from_raw("AAPL").head(5)
                     LOG_CHANGE(Assets)  LOG_CHANGE(AssetsCurrent) ...
 fy   fp filed                                                     ...
 2010 Q1 2010-01-25            0.182629                  -0.023676 ...
      Q2 2010-04-21            0.000000                   0.000000 ...
      Q3 2010-07-21            0.000000                   0.000000 ...
 2011 Q1 2011-01-19            0.459174                   0.278241 ...
      Q2 2011-04-21            0.000000                   0.000000 ...
+```
 
 Get an aggregation of quarterly and daily features for a particular ticker.
 
+```pycon
 >>> finagg.fundam.feat.fundam.from_raw("AAPL").head(5)
             PriceBookRatio  PriceEarningsRatio
 date
 2010-01-25        0.175061            2.423509
 2010-01-26        0.178035            2.464678
 2010-01-27        0.178813            2.475448
 2010-01-28        0.177154            2.452471
 2010-01-29        0.173825            2.406396
+```
 
-Use installed features for exploring refined aggregations of raw data
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+### Use installed features for exploring refined aggregations of raw data
 
 *These methods require installing refined data through the* ``finagg install``
 *or* ``finagg <api/subpackage> install`` *commands.*
 
 Get a ticker's industry's averaged quarterly report features.
 
+```pycon
 >>> finagg.sec.feat.quarterly.industry.from_refined(ticker="AAPL").head(5)
                                  mean                           ...
 name               AssetCoverageRatio BookRatio DebtEquityRatio ...
 fy   fp filed                                                   ...
 2014 Q1 2014-05-15          10.731301  9.448954        0.158318 ...
      Q2 2014-08-14          10.731301  9.448954        0.158318 ...
      Q3 2014-11-14          10.731301  9.448954        0.158318 ...
 2015 Q1 2015-05-15          16.738972  9.269250        0.294238 ...
      Q2 2015-08-13          16.738972  9.269250        0.294238 ...
+```
 
 Get a ticker's industry-averaged quarterly report features.
 
+```pycon
 >>> finagg.sec.feat.quarterly.normalized.from_refined("AAPL").head(5)
                     NORM(LOG_CHANGE(Assets))  NORM(LOG_CHANGE(AssetsCurrent)) ...
 fy   fp filed                                                                 ...
 2010 Q2 2010-04-21                  0.000000                         0.000000 ...
      Q3 2010-07-21                  0.000000                         0.000000 ...
 2011 Q1 2011-01-19                  0.978816                         0.074032 ...
      Q2 2011-04-21                  0.000000                         0.000000 ...
      Q3 2011-07-20                 -0.353553                        -0.353553 ...
+```
 
 Get tickers sorted by an industry-averaged quarterly report feature.
 
+```pycon
 >>> finagg.sec.feat.quarterly.normalized.get_tickers_sorted_by(
 ...   "NORM(EarningsPerShareBasic)",
 ...   year=2019
 ... )[:5]
 ['XRAY', 'TSLA', 'SYY', 'WHR', 'KMB']
+```
 
 Get tickers sorted by an industry-averaged fundamental feature.
 
+```pycon
 >>> finagg.fundam.feat.fundam.normalized.get_tickers_sorted_by(
 ...   "NORM(PriceEarningsRatio)",
 ...   date="2019-01-04"
 ... )[:5]
 ['AMD', 'TRGP', 'HPE', 'CZR', 'TSLA']
+```
 
-Configuration
-=============
+# Configuration
 
-API Keys and User Agents
-------------------------
+## API Keys and User Agents
 
 API keys and user agent declarations are required for most of the APIs.
 You can set environment variables to expose your API keys and user agents
 to **finagg**, or you can pass your API keys and user agents to the implemented
 APIs programmatically. The following environment variables are used for
 configuring API keys and user agents:
 
 * ``BEA_API_KEY`` is for the Bureau of Economic Analysis's API key. You can get
-  a free API key from the `BEA API site`_.
+  a free API key from the [BEA API site][3].
 * ``FRED_API_KEY`` is for the Federal Reserve Economic Data API key. You can get
-  a free API key from the `FRED API site`_.
+  a free API key from the [FRED API site][8].
 * ``INDICES_API_USER_AGENT`` is for scraping popular indices' compositions from
   Wikipedia and should be equivalent to a browser's user agent declaration.
   This defaults to a hardcoded value, but it may not always work.
 * ``SEC_API_USER_AGENT`` is for the Securities and Exchange Commission's API. This
   should be of the format ``FIRST_NAME LAST_NAME E_MAIL``.
 
-Data Locations
---------------
+## Data Locations
 
 **finagg**'s root path, HTTP cache path, and database path are all configurable
 through environment variables. By default, all data related to **finagg** is put
 in a ``./findata`` directory relative to a root directory. You can change these
 locations by modifying the respective environment variables:
 
 * ``FINAGG_ROOT_PATH`` points to the parent directory of the ``./findata`` directory.
   Defaults to your current working directory.
 * ``FINAGG_HTTP_CACHE_PATH`` points to the HTTP requests cache SQLite storage.
   Defaults to ``./findata/http_cache.sqlite``.
 * ``FINAGG_DATABASE_URL`` points to the **finagg** data storage. Defaults to
   ``./findata/finagg.sqlite``.
 
-Dependencies
-============
+# Dependencies
 
-* `pandas`_ for fast, flexible, and expressive representations of relational data.
-* `requests`_ for HTTP requests to 3rd party APIs.
-* `requests-cache`_ for caching HTTP requests to avoid getting throttled by 3rd
+* [pandas][11] for fast, flexible, and expressive representations of relational data.
+* [requests][12] for HTTP requests to 3rd party APIs.
+* [requests-cache][13] for caching HTTP requests to avoid getting throttled by 3rd
   party API servers.
-* `SQLAlchemy`_ for a SQL Python interface.
-* `yfinance`_ for historical stock data from Yahoo! Finance.
+* [SQLAlchemy][17] for a SQL Python interface.
+* [yfinance][18] for historical stock data from Yahoo! Finance.
 
-API References
-==============
+# API References
 
-* The `BEA API`_ and the `BEA API key registration link`_.
-* The `FRED API`_ and the `FRED API key registration link`_.
-* The `SEC API`_.
+* The [BEA API][1] and the [BEA API key registration link][2].
+* The [FRED API][6] and the [FRED API key registration link][7].
+* The [SEC API][14].
 
-Related Projects
-================
+# Related Projects
 
-* `FinRL`_ is a collection of financial reinforcement learning environments
+* [FinRL][5] is a collection of financial reinforcement learning environments
   and tools.
-* `fredapi`_ is an implementation of the FRED API.
-* `OpenBBTerminal`_ is an open-source version of the Bloomberg Terminal.
-* `sec-edgar`_ is an implementation of a file-based SEC EDGAR parser.
-* `sec-edgar-api`_ is an implementation of the SEC EDGAR REST API.
+* [fredapi][9] is an implementation of the FRED API.
+* [OpenBBTerminal][10] is an open-source version of the Bloomberg Terminal.
+* [sec-edgar][15] is an implementation of a file-based SEC EDGAR parser.
+* [sec-edgar-api][16] is an implementation of the SEC EDGAR REST API.
 
-Frequently Asked Questions
-==========================
+# Frequently Asked Questions
 
-Where should I start?
----------------------
+## Where should I start?
 
 Aggregate some data, create some analysis notebooks, or create some RL
 environments using the implemented data features and SQL tables. This
 project was originally created to make RL environments for financial
 applications but has since focused its purpose to just aggregating financial
 data and features. That being said, all the implemented features are
 defined in such a way to make it very easy to develop financial AI/ML,
 so we encourage you to do just that!
 
-Why aren't features being installed for a specific ticker or economic data series?
-----------------------------------------------------------------------------------
+## Why aren't features being installed for a specific ticker or economic data series?
 
 Implemented APIs may be relatively new and simply may not provide data for a
 particular ticker or economic data series. For example, earnings per share may
 not be accessible for all companies through the SEC EDGAR API. In some cases,
 APIs may raise an HTTP error, causing installations to skip the ticker or
 series. Additionally, not all tickers and economic data series contain
 sufficient data for feature normalization. If a ticker or series only has one
 data point, that data point could be dropped when computing a feature (such as
 percent change), causing no data to be installed.
 
-What Python versions are supported?
------------------------------------
+## What Python versions are supported?
 
 Python 3.10 and up are supported. We don't plan on supporting lower versions
 because 3.10 introduces some nice quality of life updates that are used
 throughout the package.
 
-What operating systems are supported?
--------------------------------------
+## What operating systems are supported?
 
 The package is developed and tested on both Linux and Windows, but we recommend
 using Linux or WSL in practice. The package performs a good amount of I/O and
 interprocess operations that could result in a noticeable performance
 degradation on Windows.
 
-.. _`BEA API`: https://apps.bea.gov/api/signup/
-.. _`BEA API key registration link`: https://apps.bea.gov/API/signup/
-.. _`BEA API site`: https://apps.bea.gov/API/signup/
-.. _`documentation`: https://theogognf.github.io/finagg/
-.. _`FinRL`: https://github.com/AI4Finance-Foundation/FinRL
-.. _`FRED API`: https://fred.stlouisfed.org/docs/api/fred/
-.. _`FRED API key registration link`: https://fredaccount.stlouisfed.org/login/secure/
-.. _`FRED API site`: https://fredaccount.stlouisfed.org/login/secure/
-.. _`fredapi`: https://github.com/mortada/fredapi
-.. _`OpenBBTerminal`: https://github.com/OpenBB-finance/OpenBBTerminal
-.. _`pandas`: https://pandas.pydata.org/
-.. _`requests`: https://requests.readthedocs.io/en/latest/
-.. _`requests-cache`: https://requests-cache.readthedocs.io/en/stable/
-.. _`SEC API`: https://www.sec.gov/edgar/sec-api-documentation
-.. _`sec-edgar`: https://github.com/sec-edgar/sec-edgar
-.. _`sec-edgar-api`: https://github.com/jadchaar/sec-edgar-api
-.. _`SQLAlchemy`: https://www.sqlalchemy.org/
-.. _`yfinance`: https://github.com/ranaroussi/yfinance
+[1]: https://apps.bea.gov/api/signup/
+[2]: https://apps.bea.gov/API/signup/
+[3]: https://apps.bea.gov/API/signup/
+[4]: https://theogognf.github.io/finagg/
+[5]: https://github.com/AI4Finance-Foundation/FinRL
+[6]: https://fred.stlouisfed.org/docs/api/fred/
+[7]: https://fredaccount.stlouisfed.org/login/secure/
+[8]: https://fredaccount.stlouisfed.org/login/secure/
+[9]: https://github.com/mortada/fredapi
+[10]: https://github.com/OpenBB-finance/OpenBBTerminal
+[11]: https://pandas.pydata.org/
+[12]: https://requests.readthedocs.io/en/latest/
+[13]: https://requests-cache.readthedocs.io/en/stable/
+[14]: https://www.sec.gov/edgar/sec-api-documentation
+[15]: https://github.com/sec-edgar/sec-edgar
+[16]: https://github.com/jadchaar/sec-edgar-api
+[17]: https://www.sqlalchemy.org/
+[18]: https://github.com/ranaroussi/yfinance
```

### Comparing `finagg-0.3.1/docs/Makefile` & `finagg-1.0.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `finagg-0.3.1/docs/cli.rst` & `finagg-1.0.0/docs/cli.rst`

 * *Files 14% similar despite different names*

```diff
@@ -30,11 +30,13 @@
 .. program-output:: finagg sec install --help
 
 Yahoo! Finance
 --------------
 
 .. program-output:: finagg yfinance install --help
 
+.. program-output:: finagg yfinance update --help
+
 Fundamental Features
 --------------------
 
 .. program-output:: finagg fundam install --help
```

### Comparing `finagg-0.3.1/docs/conf.py` & `finagg-1.0.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `finagg-0.3.1/docs/configuration.rst` & `finagg-1.0.0/docs/configuration.rst`

 * *Files identical despite different names*

### Comparing `finagg-0.3.1/docs/conventions.rst` & `finagg-1.0.0/docs/conventions.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Conventions
 ===========
 
 **finagg** has a number of conventions around package organization,
 data organization, and data normalization. Understanding these conventions
 makes **finagg** a bit more ergonomic. This page covers those conventions.
 
-Import conventions
+Import Conventions
 ------------------
 
 Following **finagg**'s import conventions guarantees updates to **finagg**
 won't break your code. Although definitions may shift around during or
 **finagg**'s organization may change slightly, your code won't be affected
 so long as you follow the import conventions. On top of this benefit,
 **finagg**'s import conventions just simplify **finagg**'s usage.
@@ -27,15 +27,15 @@
 
 It's also common for subpackages to be imported using their name as an alias:
 
 >>> import finagg.bea as bea
 >>> import finagg.fred as fred
 >>> import finagg.sec as sec
 
-Package organization
+Package Organization
 --------------------
 
 **finagg** is organized according to API implementations, SQL table
 definitions, and feature definitions. As such, each subpackage has up to
 three submodules within it:
 
 * an ``api`` module that implements the subpackage's API (if one exists)
@@ -59,15 +59,15 @@
 However, not all subpackages contain all three submodules. As another example,
 the :mod:`finagg.indices` subpackage only contains ``api`` and ``sql``
 submodules. No ``feat`` submodule is necessary for :mod:`finagg.indices`
 because there is no use for further transforming or normalizing the data
 available through :mod:`finagg.indices.api` or defined by
 :mod:`finagg.indices.sql`.
 
-API implementations
+API Implementations
 -------------------
 
 APIs are implemented as singleton class instances within ``api`` submodules
 Each singleton has a ``get`` method for accessing data from API endpoints.
 Some API implementations include class attributes that define API metadata
 (such as URLs or endpoint names), while other API implementations include
 helper methods for navigating the APIs. The design of each API implementation
@@ -99,55 +99,52 @@
 3   7  Components of Value Added by Industry as a Per...
 4   8  Chain-Type Quantity Indexes for Value Added by...
 
 Other implemented APIs, such as the SEC EDGAR API implemented by
 :mod:`finagg.sec.api`, don't have as many helper methods and are barebone
 implementations.
 
-Almost everything is a dataframe
+Almost Everything is a Dataframe
 --------------------------------
 
 Dataframes are just too convenient to not use as the fundamental type within
 **finagg**. Almost all objects returned by APIs and features are dataframes.
 
-Helper methods for inspecting available data
+Helper Methods for Inspecting Available Data
 --------------------------------------------
 
 Most submodules and singletons contain helper methods for getting sets of
 IDs available through other methods. These methods are useful for verifying
 if data has been installed properly or for selecting a subset of data for
 further refinement. Examples of these methods include:
 
 * :meth:`finagg.fred.feat.Series.get_id_set` returns installed economic data
   series IDs
 * :meth:`finagg.sec.api.get_ticker_set` returns all the tickers that have
   at least *some* data available through the SEC EDGAR API
 * :meth:`finagg.sec.feat.Quarterly.get_ticker_set` returns all the tickers
   that have quarterly features available
 
-Data organization
+Data Organization
 -----------------
 
 There are only a handful of conventions regarding data organization:
 
 * Data returned by API implementations that're used by features typically have
   their own SQL table definitions. This is convenient for querying API data
   offline and for customizing features without having to repeatedly get data
   from APIs.
-* Feature SQL tables are typically "melted" and do not have a SQL table column
-  per feature dataframe column. This makes it so features can be changed without
-  breaking the SQL table schemas.
 * Classes within ``feat`` submodules and SQL tables within ``sql`` submodules are
   named similarly to indicate their relationship.
 * Unaltered data from APIs are typically referred to as "raw" data while
   features are referred to as "refined" data. Refined data SQL tables typically
   have foreign key constraints on raw data SQL tables such that refined rows
   are deleted when raw rows are deleted with the same primary key.
 
-Data normalization
+Data Normalization
 ------------------
 
 Data returned by API implementations is not normalized or standardized
 beyond type casting and column renaming. However, data returned by feature
 implementations is normalized depending on the nature of the data. The general
 rules implemented for data normalization are as follows:
 
@@ -163,15 +160,15 @@
   as the previous bullet.
 * Dataframe indices are always based on some time unit. When an index has
   multiple levels (e.g., features returned by
   :data:`finagg.sec.feat.quarterly`), the levels are ordered from least
   granular to most granular (e.g., year -> quarter -> date). Indices
   are always sorted.
 
-Feature method naming
+Feature Method Naming
 ---------------------
 
 Features are aggregations or collections of raw and/or refined data that're
 ready for ingestion by another process. Features can be aggregated from
 APIs, local SQL tables, or combinations of both. Features generally can be
 aggregated by more than one method, and a method's name determines where the
 feature is aggregated from. The feature's aggregation source(s) implies
```

### Comparing `finagg-0.3.1/docs/faq.rst` & `finagg-1.0.0/docs/faq.rst`

 * *Files identical despite different names*

### Comparing `finagg-0.3.1/docs/index.rst` & `finagg-1.0.0/docs/index.rst`

 * *Files 2% similar despite different names*

```diff
@@ -158,22 +158,23 @@
 ... )[:5]  # doctest: +SKIP
 ['AMD', 'TRGP', 'HPE', 'CZR', 'TSLA']
 
 .. toctree::
    :maxdepth: 2
    :caption: Contents
 
-   Conventions <conventions>
-   Walkthroughs <walkthroughs>
    Installation <installation>
    Configuration <configuration>
-   CLI <cli>
+   Conventions <conventions>
+   Walkthroughs <walkthroughs>
    API <api/modules>
-   References <references>
+   CLI <cli>
    FAQ <faq>
+   References <references>
+   Release Notes <release_notes>
 
 :ref:`genindex`
 ---------------
 
 Alphabetically-ordered index of all package members.
 
 .. _`(BEA) API`: https://apps.bea.gov/api/signup/
```

### Comparing `finagg-0.3.1/docs/make.bat` & `finagg-1.0.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `finagg-0.3.1/docs/references.rst` & `finagg-1.0.0/docs/references.rst`

 * *Files identical despite different names*

### Comparing `finagg-0.3.1/docs/walkthroughs.rst` & `finagg-1.0.0/docs/walkthroughs.rst`

 * *Files 6% similar despite different names*

```diff
@@ -16,14 +16,17 @@
 variables to enable using the respective APIs. See the
 :doc:`configuration docs <configuration>` for more info on configuring your
 environment.
 
 Using the FRED API Subpackages
 ------------------------------
 
+Searching for economic data
+^^^^^^^^^^^^^^^^^^^^^^^^^^^
+
 Let's say we're interested in finding economic data series corresponding
 to various US treasuries. The FRED series search API is a good place to start.
 The FRED series search API allows us to search through economic data series
 that're provided by the FRED series observations API (the main API used for
 retrieving economic data). We can search for economic data series using search
 terms/words with :attr:`finagg.fred.api.Series.search` (the FRED series
 search API implementation):
@@ -46,14 +49,17 @@
 * the ``id`` column indicates the economic data series ID corresponding to
   each returned series (IDs are args for other FRED series API methods)
 * the ``title`` column indicates the series name (useful for verifying the
   series are relevant)
 * the ``observation_start`` column indicates the oldest date with data for
   each series (we may want to ignore series that don't have as much history)
 
+Retrieving economic data
+^^^^^^^^^^^^^^^^^^^^^^^^
+
 Let's assume we're only interested in the economic data series corresponding
 to economic series ID ``"DGS10"`` under the ``id`` column. We can get the
 economic data series observations through the FRED series observations API
 (implemented by :attr:`finagg.fred.api.Series.observations`):
 
 >>> finagg.fred.api.series.observations.get(
 ...     "DGS10",
@@ -81,14 +87,17 @@
 
 However, the ``"DGS10"`` economic data series does not support retrieving
 initial release observations. To successfully retrieve data for the ``"DGS10"``
 series (and most treasury yield series), the ``realtime_start`` and
 ``realtime_end`` parameters must be today's date (the default) and the
 ``output_type`` parameter must be ``1`` (also the default).
 
+Installing economic data
+^^^^^^^^^^^^^^^^^^^^^^^^
+
 So now we have an economic data series we're interested in and can retrieve
 observation values for. We can download and store (or install) the economic
 data series observation values in our own SQL table to reduce the number of
 requests to the FRED API (so we don't get throttled), and to get a slight
 speed boost when performing offline analysis (it'll be slightly faster to
 get data that's on our own machine rather than some server).
 
@@ -176,14 +185,17 @@
 .. code:: console
 
     finagg fred install --raw series --refined economic -ss economic
 
 Using the SEC API Subpackages
 -----------------------------
 
+Retrieving company financial data
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+
 Let's say we're interested in a specific company. The SEC EDGAR API is a good
 place to start accessing a company's financials. However, not all companies
 have all their financial data accessible through the SEC EDGAR API. The best
 way to start out and see what financials are available for a particular
 company is to look at a company's facts through
 :data:`finagg.sec.api.company_facts`.
 
@@ -222,46 +234,50 @@
         start         end  value                  accn    fy  fp  form       filed ...
 0  2007-07-01  2007-09-30   0.46  0001193125-10-171791  2010  FY  10-K  2010-07-30 ...
 1  2007-10-01  2007-12-31   0.50  0001193125-10-171791  2010  FY  10-K  2010-07-30 ...
 2  2008-01-01  2008-03-31   0.47  0001193125-10-171791  2010  FY  10-K  2010-07-30 ...
 3  2007-07-01  2008-06-30   1.90  0001193125-10-171791  2010  FY  10-K  2010-07-30 ...
 4  2008-04-01  2008-06-30   0.46  0001193125-10-171791  2010  FY  10-K  2010-07-30 ...
 
+Filtering company financial data
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+
 However, the SEC EDGAR company concept API implementation returns all the
-earnings per share publications for Microsft, including amendments. We may
+earnings per share publications for Microsoft, including amendments. We may
 not necessarily care about amendments because we may be building strategies
 or models that use *current* data and not *future* data. Fortunately, **finagg**
-provides :meth:`finagg.sec.api.get_unique_filings` to further select
+provides :meth:`finagg.sec.api.filter_original_filings` to further select
 original financial publication data from specific forms:
 
->>> finagg.sec.api.get_unique_filings(df, form="10-Q").head(5)  # doctest: +SKIP
+>>> finagg.sec.api.filter_original_filings(df, form="10-Q").head(5)  # doctest: +SKIP
      fy  fp                    tag       start         end  value ...
 0  2010  Q1  EarningsPerShareBasic  2008-07-01  2008-09-30   0.48 ...
 1  2010  Q2  EarningsPerShareBasic  2008-07-01  2008-12-31   0.95 ...
 2  2010  Q3  EarningsPerShareBasic  2008-07-01  2009-03-31   1.29 ...
 3  2011  Q1  EarningsPerShareBasic  2009-07-01  2009-09-30   0.40 ...
 4  2011  Q2  EarningsPerShareBasic  2009-07-01  2009-12-31   1.15 ...
 
 Unfortunately, the SEC EDGAR API is still relatively new and a lot of the
 financial data publications are unaudited, so not all financials are available
 for all companies through the SEC EDGAR API. I.e., a workflow for retrieving
 Microsoft's financial data may not work for retrieving another company's
-financial data. It requires some trial-and-error to find a set of tags that
+financial data.
+
+It requires some trial-and-error to find a set of tags that
 are popular and available for the majority of companies. In addition, the
 workflow for exploring these tags and filtering forms can be cumbersome.
+However, **finagg** provides :data:`finagg.sec.api.popular_concepts` for listing
+company concepts (combinations of financial data tags and other parameters)
+that're popular and widely available for companies.
 
-Fortunately again, **finagg** exists for a reason besides implementing these
-useful APIs. **finagg** provides additional conveniences that makes these
-common workflows even easier.
+Installing company financial data
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
-First, **finagg** provides :data:`finagg.sec.api.popular_concepts` for listing
-company concepts (combinations of financial data tags and other parameters)
-that're popular and widely available for companies. Second, it's extremely
-straightforward to filter and install widely popular and available quarterly
-financial data for a set of companies using the :mod:`finagg.sec.feat`
+It's extremely straightforward to filter and install widely popular and available
+quarterly financial data for a set of companies using the :mod:`finagg.sec.feat`
 subpackage and :data:`finagg.sec.feat.quarterly` member. The
 :data:`finagg.sec.feat.quarterly` member also goes a step further by somewhat
 normalizing the installed financial data (e.g., total asset value is converted
 to percent change of total asset value on a quarter-over-quarter basis), making
 the process for aggregating company financial data and comparing company
 financial data painless.
```

### Comparing `finagg-0.3.1/pyproject.toml` & `finagg-1.0.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -22,28 +22,28 @@
     "Topic :: Software Development",
     "Topic :: Scientific/Engineering",
     "Typing :: Typed"
 ]
 dependencies = [
     "beautifulsoup4==4.*",
     "click==8.*",
-    "pandas==1.*",
-    "pandas-stubs==1.*",
+    "pandas==2.*",
+    "pandas-stubs==2.*",
     "python-dotenv==0.21.*",
     "requests==2.*",
     "requests-cache==0.9.*",
     "SQLAlchemy==2.*",
     "tqdm==4.*",
     "types-requests==2.*",
     "typing-extensions==4.*",
     "yfinance<0.2.29"
 ]
 dynamic = ["version"]
 license = {file = "LICENSE"}
-readme = "README.rst"
+readme = "README.md"
 requires-python = ">=3.10"
 
 [project.scripts]
 finagg = "finagg.__main__:main"
 
 [project.urls]
 Repository = "https://github.com/theOGognf/finagg"
```

### Comparing `finagg-0.3.1/src/finagg/__main__.py` & `finagg-1.0.0/src/finagg/__main__.py`

 * *Files identical despite different names*

### Comparing `finagg-0.3.1/src/finagg/backend.py` & `finagg-1.0.0/src/finagg/backend.py`

 * *Files identical despite different names*

### Comparing `finagg-0.3.1/src/finagg/bea/_cli.py` & `finagg-1.0.0/src/finagg/bea/_cli.py`

 * *Files identical despite different names*

### Comparing `finagg-0.3.1/src/finagg/bea/api.py` & `finagg-1.0.0/src/finagg/bea/api.py`

 * *Files identical despite different names*

### Comparing `finagg-0.3.1/src/finagg/bea/sql.py` & `finagg-1.0.0/src/finagg/bea/sql.py`

 * *Files identical despite different names*

### Comparing `finagg-0.3.1/src/finagg/frame.py` & `finagg-1.0.0/src/finagg/frame.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,15 +112,15 @@
         FiscalFrame(year=1997, quarter=3)
 
         Getting quarter differences between frames and determining if the sequence
         is a valid, ordered quarterly sequence.
 
         >>> from finagg.frame import FiscalFrame, is_valid_fiscal_seq
         >>> df = finagg.sec.api.company_concept.get("AssetsCurrent", ticker="AAPL")
-        >>> df = finagg.sec.api.get_unique_filings(df, form="10-Q", units="USD")
+        >>> df = finagg.sec.api.filter_original_filings(df, form="10-Q", units="USD")
         >>> frames: pd.Series = df["fy"].astype(int).astype(str) + df["fp"].astype(str)
         >>> frames = frames.apply(lambda row: FiscalFrame.fromstr(row))
         >>> frames = frames.diff(periods=1).dropna().astype(int)
         >>> is_valid_fiscal_seq(frames.tolist())
         True
 
     """
```

### Comparing `finagg-0.3.1/src/finagg/fred/_cli.py` & `finagg-1.0.0/src/finagg/fred/_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -165,15 +165,15 @@
 
     if all_ or all_refined or all_raw:
         if total_rows:
             logger.info(f"{total_rows} total rows inserted for {__package__}")
         else:
             logger.warning(
                 f"No rows were inserted for {__package__}. This could be an error if"
-                " installations were not skipped. Set the verbose flag with the"
+                " installations were skipped. Set the verbose flag with the"
                 " `--verbose/-v` option to enable debug logging."
             )
     else:
         logger.info(
             f"Skipping {__package__} installation because no installation "
             "options are provided"
         )
```

### Comparing `finagg-0.3.1/src/finagg/fred/api/__init__.py` & `finagg-1.0.0/src/finagg/fred/api/__init__.py`

 * *Files identical despite different names*

### Comparing `finagg-0.3.1/src/finagg/fred/api/_category.py` & `finagg-1.0.0/src/finagg/fred/api/_category.py`

 * *Files 5% similar despite different names*

```diff
@@ -150,14 +150,15 @@
         offset: None | int = 0,
         order_by: None | str = None,
         sort_order: None | str = None,
         filter_variable: None | str = None,
         filter_value: None | str = None,
         tag_names: None | str | list[str] = None,
         exclude_tag_names: None | str | list[str] = None,
+        paginate: bool = False,
         api_key: None | str = None,
     ) -> pd.DataFrame:
         """Get series within a category.
 
         See the related FRED API documentation at:
 
             https://fred.stlouisfed.org/docs/api/fred/category_series.html
@@ -188,14 +189,16 @@
                 - "units"
                 - "seasonal_adjustment"
 
             filter_value: The value of `filter_variable` to filter results
                 by.
             tag_names: Find tags related to these tags.
             exclude_tag_names: Exclude tags related to these tags.
+            paginate: Whether to manage `offset` automatically, making multiple
+                API calls until all results are returned.
             api_key: Your FRED API key. Defaults to the ``FRED_API_KEY``
                 environment variable.
 
         Returns:
             A dataframe containing data for a category's series
             according to the given parameters.
 
@@ -204,31 +207,31 @@
                       id realtime_start realtime_end                                              title ...
             0   FFHTHIGH     2023-03-15   2023-03-15  High Value of the Federal Funds Rate for the I... ...
             1    FFHTLOW     2023-03-15   2023-03-15  Low Value of the Federal Funds Rate for the In... ...
             2  FFWSJHIGH     2023-03-15   2023-03-15  High Value of the Federal Funds Rate for the I... ...
             3   FFWSJLOW     2023-03-15   2023-03-15  Low Value of the Federal Funds Rate for the In... ...
 
         """
-        data = _api.get(
+        return _api.maybe_paginate(
+            "seriess",
             cls.url,
             category_id=category_id,
             realtime_start=realtime_start,
             realtime_end=realtime_end,
             limit=limit,
             offset=offset,
             order_by=order_by,
             sort_order=sort_order,
             filter_variable=filter_variable,
             filter_value=filter_value,
             tag_names=tag_names,
             exclude_tag_names=exclude_tag_names,
+            paginate=paginate,
             api_key=api_key,
-        ).json()
-        data = data["seriess"]
-        return pd.DataFrame(data)
+        )
 
 
 class CategoryTags(_api.API):
     """Get FRED category's tags.
 
     The class variable :attr:`finagg.fred.api.Category.tags` is an instance
     of this API implementation and is the most popular interface for calling
@@ -249,14 +252,15 @@
         tag_names: None | str | list[str] = None,
         tag_group_id: None | str = None,
         search_text: None | str | list[str] = None,
         limit: None | int = 1000,
         offset: None | int = 0,
         order_by: None | str = None,
         sort_order: None | str = None,
+        paginate: bool = False,
         api_key: None | str = None,
     ) -> pd.DataFrame:
         """Get a FRED category's tags.
 
         See the related FRED API documentation at:
 
             https://fred.stlouisfed.org/docs/api/fred/category_tags.html
@@ -288,14 +292,16 @@
                 - "popularity"
                 - "created"
                 - "name"
                 - "group_id"
 
             sort_order: Sort results in ascending ("asc") or
                 descending ("desc") order.
+            paginate: Whether to manage `offset` automatically, making multiple
+                API calls until all results are returned.
             api_key: Your FRED API key. Defaults to the ``FRED_API_KEY``
                 environment variable.
 
         Returns:
             A dataframe containing data for a category's tags
             according to the given parameters.
 
@@ -305,30 +311,30 @@
             0   anbil, sriya      src        2020-07-03 11:52:33-05          16             8
             1  carlson, mark      src        2020-07-03 11:53:20-05          16             8
             2          daily     freq        2012-02-27 10:18:19-06          71             8
             3        federal      gen        2012-02-27 10:18:19-06          60             8
             4          funds      gen  None  2020-05-11 13:13:02-05          28             8
 
         """
-        data = _api.get(
+        return _api.maybe_paginate(
+            "tags",
             cls.url,
             category_id=category_id,
             realtime_start=realtime_start,
             realtime_end=realtime_end,
             limit=limit,
             offset=offset,
             order_by=order_by,
             sort_order=sort_order,
             tag_names=tag_names,
             tag_group_id=tag_group_id,
             search_text=search_text,
+            paginate=paginate,
             api_key=api_key,
-        ).json()
-        data = data["tags"]
-        return pd.DataFrame(data)
+        )
 
 
 class CategoryRelatedTags(_api.API):
     """Get FRED category's related tags.
 
     The class variable :attr:`finagg.fred.api.Category.related_tags` is an
     instance of this API implementation and is the most popular interface for
@@ -350,14 +356,15 @@
         exclude_tag_names: None | str | list[str] = None,
         tag_group_id: None | str = None,
         search_text: None | str | list[str] = None,
         limit: None | int = 1000,
         offset: None | int = 0,
         order_by: None | str = None,
         sort_order: None | str = None,
+        paginate: bool = False,
         api_key: None | str = None,
     ) -> pd.DataFrame:
         """Get data for tags related to a category.
 
         See the related FRED API documentation at:
 
             https://fred.stlouisfed.org/docs/api/fred/category_related_tags.html
@@ -390,14 +397,16 @@
                 - "popularity"
                 - "created"
                 - "name"
                 - "group_id"
 
             sort_order: Sort results in ascending ("asc") or
                 descending ("desc") order.
+            paginate: Whether to manage `offset` automatically, making multiple
+                API calls until all results are returned.
             api_key: Your FRED API key. Defaults to the ``FRED_API_KEY``
                 environment variable.
 
         Returns:
             A dataframe containing data for tags related to a category
             according to the given parameters.
 
@@ -416,31 +425,31 @@
             9   public domain: citation requested       cc                      None ...
             10                               rate      gen                           ...
             11                                usa      geo  United States of America ...
             12                  wheelock, david c      src                           ...
             13                                wsj      rls       Wall Street Journal ...
 
         """
-        data = _api.get(
+        return _api.maybe_paginate(
+            "tags",
             cls.url,
             category_id=category_id,
             realtime_start=realtime_start,
             realtime_end=realtime_end,
             tag_names=tag_names,
             exclude_tag_names=exclude_tag_names,
             tag_group_id=tag_group_id,
             search_text=search_text,
             limit=limit,
             offset=offset,
             order_by=order_by,
             sort_order=sort_order,
+            paginate=paginate,
             api_key=api_key,
-        ).json()
-        data = data["tags"]
-        return pd.DataFrame(data)
+        )
 
 
 class Category(_api.API):
     """Collection of "fred/category" APIs.
 
     The class variable :data:`finagg.fred.api.category` is an
     instance of this API implementation and is the most popular interface for
```

### Comparing `finagg-0.3.1/src/finagg/fred/api/_release.py` & `finagg-1.0.0/src/finagg/fred/api/_release.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,14 +29,15 @@
         realtime_start: None | int | str = None,
         realtime_end: None | int | str = None,
         limit: None | int = 1000,
         offset: None | int = 0,
         order_by: None | str = "release_date",
         sort_order: None | str = "desc",
         include_release_dates_with_no_data: None | bool = False,
+        paginate: bool = False,
         api_key: None | str = None,
     ) -> pd.DataFrame:
         """Get all release dates of economic data.
 
         See the related FRED API documentation at:
 
             https://fred.stlouisfed.org/docs/api/fred/releases_dates.html
@@ -54,35 +55,37 @@
                 - "release_id"
                 - "release_name"
 
             sort_order: Sort results in ascending ("asc") or
                 descending ("desc") order.
             include_release_dates_with_no_data: Whether to return release
                 dates that don't contain any data.
+            paginate: Whether to manage `offset` automatically, making multiple
+                API calls until all results are returned.
             api_key: Your FRED API key. Defaults to the ``FRED_API_KEY``
                 environment variable.
 
         Returns:
             A dataframe containing data on release dates for all
             releases of economic data.
 
         """
-        data = _api.get(
+        return _api.maybe_paginate(
+            "release_dates",
             cls.url,
             realtime_start=realtime_start,
             realtime_end=realtime_end,
             limit=limit,
             offset=offset,
             order_by=order_by,
             sort_order=sort_order,
             include_release_dates_with_no_data=include_release_dates_with_no_data,
+            paginate=paginate,
             api_key=api_key,
-        ).json()
-        data = data["release_dates"]
-        return pd.DataFrame(data)
+        )
 
 
 class Releases(_api.API):
     """Get all releases of economic data."""
 
     dates = ReleasesDates()
     """"releases/dates" FRED API. Get dates for releases of economic data.
@@ -100,14 +103,15 @@
         *,
         realtime_start: None | int | str = None,
         realtime_end: None | int | str = None,
         limit: None | int = 1000,
         offset: None | int = 0,
         order_by: None | str = None,
         sort_order: None | str = None,
+        paginate: bool = False,
         api_key: None | str = None,
     ) -> pd.DataFrame:
         """Get all releases of economic data.
 
         See the related FRED API documentation at:
 
             https://fred.stlouisfed.org/docs/api/fred/releases.html
@@ -125,34 +129,36 @@
                 - "name"
                 - "press_release"
                 - "realtime_start"
                 - "realtime_end"
 
             sort_order: Sort results in ascending ("asc") or
                 descending ("desc") order.
+            paginate: Whether to manage `offset` automatically, making multiple
+                API calls until all results are returned.
             api_key: Your FRED API key. Defaults to the ``FRED_API_KEY``
                 environment variable.
 
         Returns:
             A dataframe containing data on all releases of economic
             data.
 
         """
-        data = _api.get(
+        return _api.maybe_paginate(
+            "releases",
             cls.url,
             realtime_start=realtime_start,
             realtime_end=realtime_end,
             limit=limit,
             offset=offset,
             order_by=order_by,
             sort_order=sort_order,
+            paginate=paginate,
             api_key=api_key,
-        ).json()
-        data = data["releases"]
-        return pd.DataFrame(data)
+        )
 
 
 class ReleaseDates(_api.API):
     """Get dates associated with an economic release.
 
     The class variable :attr:`finagg.fred.api.Release.dates` is an
     instance of this API implementation and is the most popular interface for
@@ -170,14 +176,15 @@
         *,
         realtime_start: None | int | str = None,
         realtime_end: None | int | str = None,
         limit: None | int = 10000,
         offset: None | int = 0,
         sort_order: None | str = None,
         include_release_dates_with_no_data: None | bool = False,
+        paginate: bool = False,
         api_key: None | str = None,
     ) -> pd.DataFrame:
         """Get data on release dates for a particular release of economic data.
 
         See the related FRED API documentation at:
 
             https://fred.stlouisfed.org/docs/api/fred/release_dates.html
@@ -190,34 +197,36 @@
                 to their publication date.
             limit: Maximum number of results to return.
             offset: Result start offset.
             sort_order: Sort results in ascending ("asc") or
                 descending ("desc") order.
             include_release_dates_with_no_data: Whether to return release
                 dates that don't contain any data.
+            paginate: Whether to manage `offset` automatically, making multiple
+                API calls until all results are returned.
             api_key: Your FRED API key. Defaults to the ``FRED_API_KEY``
                 environment variable.
 
         Returns:
             A dataframe containing data for an economic data release's release dates.
 
         """
-        data = _api.get(
+        return _api.maybe_paginate(
+            "release_dates",
             cls.url,
             release_id=release_id,
             realtime_start=realtime_start,
             realtime_end=realtime_end,
             limit=limit,
             offset=offset,
             sort_order=sort_order,
             include_release_dates_with_no_data=include_release_dates_with_no_data,
+            paginate=paginate,
             api_key=api_key,
-        ).json()
-        data = data["release_dates"]
-        return pd.DataFrame(data)
+        )
 
 
 class ReleaseSeries(_api.API):
     """Get series associated with an economic release.
 
     The class variable :attr:`finagg.fred.api.Release.series` is an
     instance of this API implementation and is the most popular interface for
@@ -239,14 +248,15 @@
         offset: None | int = 0,
         order_by: None | str = None,
         sort_order: None | str = None,
         filter_variable: None | str = None,
         filter_value: None | str = None,
         tag_names: None | str | list[str] = None,
         exclude_tag_names: None | str | list[str] = None,
+        paginate: bool = False,
         api_key: None | str = None,
     ) -> pd.DataFrame:
         """Get data on the series related to a release of economic data.
 
         See the related FRED API documentation at:
 
             https://fred.stlouisfed.org/docs/api/fred/release_series.html
@@ -283,38 +293,40 @@
                 - "units"
                 - "seasonal_adjustment"
 
             filter_value: The value of `filter_variable` to filter results
                 by.
             tag_names: Find tags related to these tags.
             exclude_tag_names: Exclude tags related to these tags.
+            paginate: Whether to manage `offset` automatically, making multiple
+                API calls until all results are returned.
             api_key: Your FRED API key. Defaults to the ``FRED_API_KEY``
                 environment variable.
 
         Returns:
             A dataframe containing series data for a release.
 
         """
-        data = _api.get(
+        return _api.maybe_paginate(
+            "seriess",
             cls.url,
             release_id=release_id,
             realtime_start=realtime_start,
             realtime_end=realtime_end,
             limit=limit,
             offset=offset,
             order_by=order_by,
             sort_order=sort_order,
             filter_variable=filter_variable,
             filter_value=filter_value,
             tag_names=tag_names,
             exclude_tag_names=exclude_tag_names,
+            paginate=paginate,
             api_key=api_key,
-        ).json()
-        data = data["seriess"]
-        return pd.DataFrame(data)
+        )
 
 
 class ReleaseSources(_api.API):
     """Get sources associated with an economic release.
 
     The class variable :attr:`finagg.fred.api.Release.sources` is an
     instance of this API implementation and is the most popular interface for
@@ -386,14 +398,15 @@
         tag_names: None | str | list[str] = None,
         tag_group_id: None | str = None,
         search_text: None | str | list[str] = None,
         limit: None | int = 1000,
         offset: None | int = 0,
         order_by: None | str = None,
         sort_order: None | str = None,
+        paginate: bool = False,
         api_key: None | str = None,
     ) -> pd.DataFrame:
         """Get tags for an economic release.
 
         See the related FRED API documentation at:
 
             https://fred.stlouisfed.org/docs/api/fred/release_tags.html
@@ -424,38 +437,40 @@
                 - "popularity"
                 - "created"
                 - "name"
                 - "group_id"
 
             sort_order: Sort results in ascending ("asc") or
                 descending ("desc") order.
+            paginate: Whether to manage `offset` automatically, making multiple
+                API calls until all results are returned.
             api_key: Your FRED API key. Defaults to the ``FRED_API_KEY``
                 environment variable.
 
         Returns:
             A dataframe containing data for an economic release's tags
             according to the given parameters.
 
         """
-        data = _api.get(
+        return _api.maybe_paginate(
+            "tags",
             cls.url,
             release_id=release_id,
             realtime_start=realtime_start,
             realtime_end=realtime_end,
             tag_names=tag_names,
             tag_group_id=tag_group_id,
             search_text=search_text,
             limit=limit,
             offset=offset,
             order_by=order_by,
             sort_order=sort_order,
+            paginate=paginate,
             api_key=api_key,
-        ).json()
-        data = data["tags"]
-        return pd.DataFrame(data)
+        )
 
 
 class ReleaseRelatedTags(_api.API):
     """Get tags related to an economic release.
 
     The class variable :attr:`finagg.fred.api.Release.related_tags` is an
     instance of this API implementation and is the most popular interface for
@@ -477,14 +492,15 @@
         exclude_tag_names: None | str | list[str] = None,
         tag_group_id: None | str = None,
         search_text: None | str | list[str] = None,
         limit: None | int = 1000,
         offset: None | int = 0,
         order_by: None | str = None,
         sort_order: None | str = None,
+        paginate: bool = False,
         api_key: None | str = None,
     ) -> pd.DataFrame:
         """Get data for tags related to an economic release.
 
         See the related FRED API documentation at:
 
             https://fred.stlouisfed.org/docs/api/fred/release_related_tags.html
@@ -516,39 +532,41 @@
                 - "popularity"
                 - "created"
                 - "name"
                 - "group_id"
 
             sort_order: Sort results in ascending ("asc") or
                 descending ("desc") order.
+            paginate: Whether to manage `offset` automatically, making multiple
+                API calls until all results are returned.
             api_key: Your FRED API key. Defaults to the ``FRED_API_KEY``
                 environment variable.
 
         Returns:
             A dataframe containing data for tags related to an economic
             release according to the given parameters.
 
         """
-        data = _api.get(
+        return _api.maybe_paginate(
+            "tags",
             cls.url,
             release_id=release_id,
             realtime_start=realtime_start,
             realtime_end=realtime_end,
             tag_names=tag_names,
             exclude_tag_names=exclude_tag_names,
             tag_group_id=tag_group_id,
             search_text=search_text,
             limit=limit,
             offset=offset,
             order_by=order_by,
             sort_order=sort_order,
+            paginate=paginate,
             api_key=api_key,
-        ).json()
-        data = data["tags"]
-        return pd.DataFrame(data)
+        )
 
 
 class ReleaseTables(_api.API):
     """Get tables associated with an economic release.
 
     The class variable :attr:`finagg.fred.api.Release.tables` is an instance of
     this API implementation and is the most popular interface for calling this
```

### Comparing `finagg-0.3.1/src/finagg/fred/api/_series.py` & `finagg-1.0.0/src/finagg/fred/api/_series.py`

 * *Files 3% similar despite different names*

```diff
@@ -99,14 +99,15 @@
         observation_start: None | int | str = None,
         observation_end: None | int | str = None,
         units: None | str = "lin",
         frequency: None | str = None,
         aggregation_method: None | str = "avg",
         output_type: None | int = 1,
         vintage_dates: None | str | list[str] = None,
+        paginate: bool = False,
         api_key: None | str = None,
     ) -> pd.DataFrame:
         """Get the observations or data values for an economic data series.
 
         See the related FRED API documentation at:
 
             https://fred.stlouisfed.org/docs/api/fred/series_observations.html
@@ -173,14 +174,16 @@
                     - 2 = all observations by vintage dates
                     - 3 = new and revised observations only
                     - 4 = initial release observations only
 
             vintage_dates: Vintage dates used to download data as it existed on these
                 specified dates in history. Vintage dates can be specified instead of
                 realtime periods.
+            paginate: Whether to manage `offset` automatically, making multiple
+                API calls until all results are returned.
             api_key: Your FRED API key. Defaults to the ``FRED_API_KEY``
                 environment variable.
 
         Returns:
             A dataframe containing economic data series observations/values according to
             the given parameters.
 
@@ -195,33 +198,33 @@
             0     1949-04-22   1953-02-26  1949-03-01  169.5  CPIAUCNS
             1     1949-05-23   1953-02-26  1949-04-01  169.7  CPIAUCNS
             2     1949-06-24   1953-02-26  1949-05-01  169.2  CPIAUCNS
             3     1949-07-22   1953-02-26  1949-06-01  169.6  CPIAUCNS
             4     1949-08-26   1953-02-26  1949-07-01  168.5  CPIAUCNS
 
         """
-        data = _api.get(
+        df = _api.maybe_paginate(
+            "observations",
             cls.url,
             series_id=series_id,
             realtime_start=realtime_start,
             realtime_end=realtime_end,
             limit=limit,
             offset=offset,
             sort_order=sort_order,
             observation_start=observation_start,
             observation_end=observation_end,
             units=units,
             frequency=frequency,
             aggregation_method=aggregation_method,
             output_type=output_type,
             vintage_dates=vintage_dates,
+            paginate=paginate,
             api_key=api_key,
-        ).json()
-        data = data["observations"]
-        df = pd.DataFrame(data)
+        )
         df["series_id"] = series_id
         df["value"] = pd.to_numeric(df["value"], errors="coerce")
         return df
 
     @classmethod
     def get_first_observations(
         cls,
@@ -232,14 +235,15 @@
         offset: None | int = 0,
         sort_order: None | str = None,
         observation_start: None | int | str = None,
         observation_end: None | int | str = None,
         units: None | str = "lin",
         frequency: None | str = None,
         aggregation_method: None | str = "avg",
+        paginate: bool = False,
         api_key: None | str = None,
     ) -> pd.DataFrame:
         """Get only the initial releases/observations for an
         economic data series.
 
         Similar to :meth:`SeriesObservations.get`, but tries to get initial
         releases/observations only.
@@ -290,14 +294,16 @@
             aggregation_method: A key that indicates the aggregation method used
                 for frequency aggregation. Options include:
 
                     - "avg" = average
                     - "sum" = sum
                     - "eop" = end of period
 
+            paginate: Whether to manage `offset` automatically, making multiple
+                API calls until all results are returned.
             api_key: Your FRED API key. Defaults to the ``FRED_API_KEY``
                 environment variable.
 
         Returns:
             A dataframe containing economic data series observations/values according to
             the given parameters.
 
@@ -323,27 +329,29 @@
                 sort_order=sort_order,
                 observation_start=observation_start,
                 observation_end=observation_end,
                 units=units,
                 frequency=frequency,
                 aggregation_method=aggregation_method,
                 output_type=4,
+                paginate=paginate,
                 api_key=api_key,
             )
         except HTTPError:
             return cls.get(
                 series_id,
                 limit=limit,
                 offset=offset,
                 sort_order=sort_order,
                 observation_start=observation_start,
                 observation_end=observation_end,
                 units=units,
                 frequency=frequency,
                 aggregation_method=aggregation_method,
+                paginate=paginate,
                 api_key=api_key,
             )
 
 
 class SeriesRelease(_api.API):
     """Get the latest release for an economic data seris.
 
@@ -418,14 +426,15 @@
         exclude_tag_names: None | str | list[str] = None,
         tag_group_id: None | str = None,
         tag_search_text: None | str | list[str] = None,
         limit: None | int = 1000,
         offset: None | int = 0,
         order_by: None | str = None,
         sort_order: None | str = None,
+        paginate: bool = False,
         api_key: None | str = None,
     ) -> pd.DataFrame:
         """Get the related tags for a series search.
 
         See the related FRED API documentation at:
 
             https://fred.stlouisfed.org/docs/api/fred/series_search_tags.html
@@ -458,14 +467,16 @@
                     - "popularity"
                     - "created"
                     - "name"
                     - "group_id"
 
             sort_order: Sort results in ascending ("asc") or descending ("desc")
                 order for the attribute values specified by `order_by`.
+            paginate: Whether to manage `offset` automatically, making multiple
+                API calls until all results are returned.
             api_key: Your FRED API key. Defaults to the ``FRED_API_KEY``
                 environment variable.
 
         Returns:
             A dataframe containing related FRED tags for a series search.
             The dataframe can have results optionally filtered by the FRED
             servers according to the method's args.
@@ -476,31 +487,31 @@
             0                                nsa     seas  Not Seasonally Adjusted  2012-02-27 10:18:19-06 ...
             1                            indexes      gen                           2012-02-27 10:18:19-06 ...
             2                        price index      gen                           2012-02-27 10:18:19-06 ...
             3                            monthly     freq                           2012-02-27 10:18:19-06 ...
             4  public domain: citation requested       cc                     None  2018-12-17 23:33:13-06 ...
 
         """
-        data = _api.get(
+        return _api.maybe_paginate(
+            "tags",
             cls.url,
             series_search_text=series_search_text,
             realtime_start=realtime_start,
             realtime_end=realtime_end,
             tag_names=tag_names,
             exclude_tag_names=exclude_tag_names,
             tag_group_id=tag_group_id,
             tag_search_text=tag_search_text,
             limit=limit,
             offset=offset,
             order_by=order_by,
             sort_order=sort_order,
+            paginate=paginate,
             api_key=api_key,
-        ).json()
-        data = data["tags"]
-        return pd.DataFrame(data)
+        )
 
 
 class SeriesSearchTags(_api.API):
     """Get FRED series tags.
 
     The class variable :attr:`finagg.fred.api.SeriesSearch.tags` is an
     instance of this API implementation and is the most popular interface for
@@ -521,14 +532,15 @@
         tag_names: None | str | list[str] = None,
         tag_group_id: None | str = None,
         tag_search_text: None | str | list[str] = None,
         limit: None | int = 1000,
         offset: None | int = 0,
         order_by: None | str = None,
         sort_order: None | str = None,
+        paginate: bool = False,
         api_key: None | str = None,
     ) -> pd.DataFrame:
         """Get the tags for a series search.
 
         See the related FRED API documentation at:
 
             https://fred.stlouisfed.org/docs/api/fred/series_search_tags.html
@@ -560,14 +572,16 @@
                     - "popularity"
                     - "created"
                     - "name"
                     - "group_id"
 
             sort_order: Sort results in ascending ("asc") or descending ("desc")
                 order for the attribute values specified by `order_by`.
+            paginate: Whether to manage `offset` automatically, making multiple
+                API calls until all results are returned.
             api_key: Your FRED API key. Defaults to the ``FRED_API_KEY``
                 environment variable.
 
         Returns:
             A dataframe containing FRED tags for a series search.
             The dataframe can have results optionally filtered by the FRED
             servers according to the method's args.
@@ -578,30 +592,30 @@
             0                                nsa     seas  Not Seasonally Adjusted ...
             1                              price      gen                          ...
             2                            indexes      gen                          ...
             3                        price index      gen                          ...
             4  public domain: citation requested       cc                     None ...
 
         """
-        data = _api.get(
+        return _api.maybe_paginate(
+            "tags",
             cls.url,
             series_search_text=series_search_text,
             realtime_start=realtime_start,
             realtime_end=realtime_end,
             tag_names=tag_names,
             tag_group_id=tag_group_id,
             tag_search_text=tag_search_text,
             limit=limit,
             offset=offset,
             order_by=order_by,
             sort_order=sort_order,
+            paginate=paginate,
             api_key=api_key,
-        ).json()
-        data = data["tags"]
-        return pd.DataFrame(data)
+        )
 
 
 class SeriesSearch(_api.API):
     """Get economic data series that match search text.
 
     The class variable :attr:`finagg.fred.api.Series.search` is an
     instance of this API implementation and is the most popular interface for
@@ -640,14 +654,15 @@
         offset: None | int = 0,
         order_by: None | str = None,
         sort_order: None | str = None,
         filter_variable: None | str = None,
         filter_value: None | str = None,
         tag_names: None | str | list[str] = None,
         exclude_tag_names: None | str | list[str] = None,
+        paginate: bool = False,
         api_key: None | str = None,
     ) -> pd.DataFrame:
         """Get economic data series that match search text.
 
         See the related FRED API documentation at:
 
             https://fred.stlouisfed.org/docs/api/fred/series_search.html
@@ -691,14 +706,16 @@
                 - "units"
                 - "seasonal_adjustment"
 
             filter_value: The value of the `filter_variable` attribute to filter
                 results by.
             tag_names: List of tag names that series match all of.
             exclude_tag_names: List of tag names that series match none of.
+            paginate: Whether to manage `offset` automatically, making multiple
+                API calls until all results are returned.
             api_key: Your FRED API key. Defaults to the ``FRED_API_KEY``
                 environment variable.
 
         Returns:
             A dataframe containing data on series matching the search.
 
         Examples:
@@ -707,32 +724,32 @@
             0     CPIAUCSL     2023-03-16   2023-03-16  Consumer Price Index for All Urban Consumers: ... ...
             1     CPIAUCNS     2023-03-16   2023-03-16  Consumer Price Index for All Urban Consumers: ... ...
             2  CUUS0000SA0     2023-03-16   2023-03-16  Consumer Price Index for All Urban Consumers: ... ...
             3   CSUSHPINSA     2023-03-16   2023-03-16    S&P/Case-Shiller U.S. National Home Price Index ...
             4    CSUSHPISA     2023-03-16   2023-03-16    S&P/Case-Shiller U.S. National Home Price Index ...
 
         """
-        data = _api.get(
+        return _api.maybe_paginate(
+            "seriess",
             cls.url,
             search_text=search_text,
             search_type=search_type,
             realtime_start=realtime_start,
             realtime_end=realtime_end,
             limit=limit,
             offset=offset,
             order_by=order_by,
             sort_order=sort_order,
             filter_variable=filter_variable,
             filter_value=filter_value,
             tag_names=tag_names,
             exclude_tag_names=exclude_tag_names,
+            paginate=paginate,
             api_key=api_key,
-        ).json()
-        data = data["seriess"]
-        return pd.DataFrame(data)
+        )
 
 
 class SeriesTags(_api.API):
     """Get FRED tags for an economic data series.
 
     The class variable :attr:`finagg.fred.api.Series.tags` is an
     instance of this API implementation and is the most popular interface for
@@ -824,14 +841,15 @@
         realtime_start: None | int | str = None,
         realtime_end: None | int | str = None,
         limit: None | int = 1000,
         offset: None | int = 0,
         filter_value: None | str = None,
         start_time: None | str = None,
         end_time: None | str = None,
+        paginate: bool = False,
         api_key: None | str = None,
     ) -> pd.DataFrame:
         """Get economic data series sorted by when observations
         were updated on the FRED server.
 
         Results are limited to series updated within the last two
         weeks.
@@ -854,35 +872,37 @@
                     - "regional" = limit results to series for parts of the US
                     - "all" = does not filter results
 
             start_time: Start time for limiting results for a time range.
                 Can filter down to minutes. Expects format "YYYMMDDHhmm".
             end_time: Start time for limiting results for a time range.
                 Can filter down to minutes. Expects format "YYYMMDDHhmm".
+            paginate: Whether to manage `offset` automatically, making multiple
+                API calls until all results are returned.
             api_key: Your FRED API key. Defaults to the ``FRED_API_KEY``
                 environment variable.
 
         Returns:
             A dataframe containing info on recently updated economic
             data series.
 
         """
-        data = _api.get(
+        return _api.maybe_paginate(
+            "seriess",
             cls.url,
             realtime_start=realtime_start,
             realtime_end=realtime_end,
             limit=limit,
             offset=offset,
             filter_value=filter_value,
             start_time=start_time,
             end_time=end_time,
+            paginate=paginate,
             api_key=api_key,
-        ).json()
-        data = data["seriess"]
-        return pd.DataFrame(data)
+        )
 
 
 class SeriesVintageDates(_api.API):
     """Get FRED series revision dates.
 
     The class variable :attr:`finagg.fred.api.Series.vintage_dates` is an
     instance of this API implementation and is the most popular interface for
@@ -899,14 +919,15 @@
         /,
         *,
         realtime_start: None | int | str = None,
         realtime_end: None | int | str = None,
         limit: None | int = 10000,
         offset: None | int = 0,
         sort_order: None | str = None,
+        paginate: bool = False,
         api_key: None | str = None,
     ) -> pd.DataFrame:
         """Get the dates in history when a series' data values were revised
         or new data values were released.
 
         Vintage dates are the release dates for a series excluding release dates
         when the data for the series did not change.
@@ -921,31 +942,35 @@
                 according to their publication date.
             realtime_end: End date for fetching results according
                 to their publication date.
             limit: Maximum number of results to return.
             offset: Result start offset.
             sort_order: Sort results in ascending ("asc") or descending ("desc")
                 vintage date order.
+            paginate: Whether to manage `offset` automatically, making multiple
+                API calls until all results are returned.
+            api_key: Your FRED API key. Defaults to the ``FRED_API_KEY``
+                environment variable.
 
         Returns:
             A dataframe containing dates on vintage release dates for a series.
 
         """
-        data = _api.get(
+        return _api.maybe_paginate(
+            "seriess",
             cls.url,
             series_id=series_id,
             realtime_start=realtime_start,
             realtime_end=realtime_end,
             limit=limit,
             offset=offset,
             sort_order=sort_order,
+            paginate=paginate,
             api_key=api_key,
-        ).json()
-        data = data["seriess"]
-        return pd.DataFrame(data)
+        )
 
 
 class Series(_api.API):
     """Get an economic data series.
 
     The class variable :data:`finagg.fred.api.series` is an instance of this
     API implementation and is the most popular interface for calling this API.
```

### Comparing `finagg-0.3.1/src/finagg/fred/api/_source.py` & `finagg-1.0.0/src/finagg/fred/api/_source.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,14 +30,15 @@
         *,
         realtime_start: None | int | str = None,
         realtime_end: None | int | str = None,
         limit: None | int = 1000,
         offset: None | int = 0,
         order_by: None | str = None,
         sort_order: None | str = None,
+        paginate: bool = False,
         api_key: None | str = None,
     ) -> pd.DataFrame:
         """Get all releases for a source of economic data.
 
         See the related FRED API documentation at:
 
             https://fred.stlouisfed.org/docs/api/fred/source_releases.html
@@ -56,14 +57,16 @@
                 - "name"
                 - "press_release"
                 - "realtime_start"
                 - "realtime_end"
 
             sort_order: Sort results in ascending ("asc") or
                 descending ("desc") order.
+            paginate: Whether to manage `offset` automatically, making multiple
+                API calls until all results are returned.
             api_key: Your FRED API key. Defaults to the ``FRED_API_KEY``
                 environment variable.
 
         Returns:
             A dataframe containing data on all releases for a
             source of economic data.
 
@@ -73,27 +76,27 @@
             0  13     2023-03-15   2023-03-15  G.17 Industrial Production and Capacity Utiliz...           True  http://www.federalreserve.gov/releases/g17/
             1  14     2023-03-15   2023-03-15                               G.19 Consumer Credit           True  http://www.federalreserve.gov/releases/g19/
             2  15     2023-03-15   2023-03-15                         G.5 Foreign Exchange Rates           True   http://www.federalreserve.gov/releases/g5/
             3  17     2023-03-15   2023-03-15                        H.10 Foreign Exchange Rates           True  http://www.federalreserve.gov/releases/h10/
             4  18     2023-03-15   2023-03-15                       H.15 Selected Interest Rates           True  http://www.federalreserve.gov/releases/h15/
 
         """
-        data = _api.get(
+        return _api.maybe_paginate(
+            "releases",
             cls.url,
             source_id=source_id,
             realtime_start=realtime_start,
             realtime_end=realtime_end,
             limit=limit,
             offset=offset,
             order_by=order_by,
             sort_order=sort_order,
+            paginate=paginate,
             api_key=api_key,
-        ).json()
-        data = data["releases"]
-        return pd.DataFrame(data)
+        )
 
 
 class Source(_api.API):
     """Get a source of economic data.
 
     The module variable :data:`finagg.fred.api.source` is an instance
     of this API implementation and is the most popular interface for calling
@@ -172,14 +175,15 @@
         cls,
         realtime_start: None | int | str = None,
         realtime_end: None | int | str = None,
         limit: None | int = 1000,
         offset: None | int = 0,
         order_by: None | str = None,
         sort_order: None | str = None,
+        paginate: bool = False,
         api_key: None | str = None,
     ) -> pd.DataFrame:
         """Get all sources of economic data.
 
         See the related FRED API documentation at:
 
             https://fred.stlouisfed.org/docs/api/fred/sources.html
@@ -197,14 +201,16 @@
                 - "name"
                 - "press_release"
                 - "realtime_start"
                 - "realtime_end"
 
             sort_order: Sort results in ascending ("asc") or
                 descending ("desc") order.
+            paginate: Whether to manage `offset` automatically, making multiple
+                API calls until all results are returned.
             api_key: Your FRED API key. Defaults to the ``FRED_API_KEY``
                 environment variable.
 
         Returns:
             A dataframe containing data on all sources of economic
             data.
 
@@ -214,19 +220,19 @@
             0   1     2023-03-15   2023-03-15  Board of Governors of the Federal Reserve Syst...    http://www.federalreserve.gov/
             1   3     2023-03-15   2023-03-15               Federal Reserve Bank of Philadelphia  https://www.philadelphiafed.org/
             2   4     2023-03-15   2023-03-15                  Federal Reserve Bank of St. Louis        http://www.stlouisfed.org/
             3   6     2023-03-15   2023-03-15  Federal Financial Institutions Examination Cou...             http://www.ffiec.gov/
             4  11     2023-03-15   2023-03-15                                Dow Jones & Company           http://www.dowjones.com
 
         """
-        data = _api.get(
+        return _api.maybe_paginate(
+            "sources",
             cls.url,
             realtime_start=realtime_start,
             realtime_end=realtime_end,
             limit=limit,
             offset=offset,
             order_by=order_by,
             sort_order=sort_order,
+            paginate=paginate,
             api_key=api_key,
-        ).json()
-        data = data["sources"]
-        return pd.DataFrame(data)
+        )
```

### Comparing `finagg-0.3.1/src/finagg/fred/api/_tags.py` & `finagg-1.0.0/src/finagg/fred/api/_tags.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,14 +32,15 @@
         exclude_tag_names: None | str | list[str] = None,
         tag_group_id: None | str = None,
         search_text: None | str | list[str] = None,
         limit: None | int = 1000,
         offset: None | int = 0,
         order_by: None | str = None,
         sort_order: None | str = None,
+        paginate: bool = False,
         api_key: None | str = None,
     ) -> pd.DataFrame:
         """Get data for tags related to an economic release.
 
         See the related FRED API documentation at:
 
             https://fred.stlouisfed.org/docs/api/fred/related_tags.html
@@ -70,14 +71,16 @@
                 - "popularity"
                 - "created"
                 - "name"
                 - "group_id"
 
             sort_order: Sort results in ascending ("asc") or
                 descending ("desc") order.
+            paginate: Whether to manage `offset` automatically, making multiple
+                API calls until all results are returned.
             api_key: Your FRED API key. Defaults to the ``FRED_API_KEY``
                 environment variable.
 
         Returns:
             A dataframe containing data for related FRED tags.
 
         Examples:
@@ -86,30 +89,30 @@
             0  public domain: citation requested       cc                      None  2018-12-17 23:33:13-06          99         78680
             1                                usa      geo  United States of America  2012-02-27 10:18:19-06         100         78434
             2                                nsa     seas   Not Seasonally Adjusted  2012-02-27 10:18:19-06          99         67720
             3                             annual     freq                            2012-02-27 10:18:19-06          88         66478
             4                                gdp      gen    Gross Domestic Product  2012-02-27 10:18:19-06          81         60040
 
         """
-        data = _api.get(
+        return _api.maybe_paginate(
+            "tags",
             cls.url,
             realtime_start=realtime_start,
             realtime_end=realtime_end,
             tag_names=tag_names,
             exclude_tag_names=exclude_tag_names,
             tag_group_id=tag_group_id,
             search_text=search_text,
             limit=limit,
             offset=offset,
             order_by=order_by,
             sort_order=sort_order,
+            paginate=paginate,
             api_key=api_key,
-        ).json()
-        data = data["tags"]
-        return pd.DataFrame(data)
+        )
 
 
 class Series(_api.API):
     """Get FRED series related to FRED tags.
 
     The class variable :data:`finagg.fred.api.tags.series` is an instance
     of this API implementation and is the most popular interface for calling
@@ -127,14 +130,15 @@
         exclude_tag_names: None | str | list[str] = None,
         realtime_start: None | int | str = None,
         realtime_end: None | int | str = None,
         limit: None | int = 1000,
         offset: None | int = 0,
         order_by: None | str = None,
         sort_order: None | str = None,
+        paginate: bool = False,
         api_key: None | str = None,
     ) -> pd.DataFrame:
         """Get the economic data series matching tags.
 
         See the related FRED API documentation at:
 
             https://fred.stlouisfed.org/docs/api/fred/tags_series.html
@@ -161,14 +165,16 @@
                 - "observation_start"
                 - "observation_end"
                 - "popularity"
                 - "group_popularity"
 
             sort_order: Sort results in ascending ("asc") or
                 descending ("desc") order.
+            paginate: Whether to manage `offset` automatically, making multiple
+                API calls until all results are returned.
             api_key: Your FRED API key. Defaults to the ``FRED_API_KEY``
                 environment variable.
 
         Returns:
             A dataframe containing series data for related tags.
 
         Examples:
@@ -177,28 +183,28 @@
             0  A001RD3A086NBEA     2023-03-15   2023-03-15  Gross national product (implicit price deflator) ...
             1  A001RG3A086NBEA     2023-03-15   2023-03-15   Gross national product (chain-type price index) ...
             2  A001RI1A225NBEA     2023-03-15   2023-03-15   Gross National Product: Implicit Price Deflator ...
             3  A001RI1Q225SBEA     2023-03-15   2023-03-15   Gross National Product: Implicit Price Deflator ...
             4  A001RL1A225NBEA     2023-03-15   2023-03-15                       Real Gross National Product ...
 
         """
-        data = _api.get(
+        return _api.maybe_paginate(
+            "seriess",
             cls.url,
             tag_names=tag_names,
             exclude_tag_names=exclude_tag_names,
             realtime_start=realtime_start,
             realtime_end=realtime_end,
             limit=limit,
             offset=offset,
             order_by=order_by,
             sort_order=sort_order,
+            paginate=paginate,
             api_key=api_key,
-        ).json()
-        data = data["seriess"]
-        return pd.DataFrame(data)
+        )
 
 
 class Tags(_api.API):
     """Get FRED tags.
 
     The module variable :data:`tags` is an instance of this API
     implementation and is the most popular interface for calling
@@ -224,14 +230,15 @@
         tag_names: None | str | list[str] = None,
         tag_group_id: None | str = None,
         search_text: None | str | list[str] = None,
         limit: None | int = 1000,
         offset: None | int = 0,
         order_by: None | str = None,
         sort_order: None | str = None,
+        paginate: bool = False,
         api_key: None | str = None,
     ) -> pd.DataFrame:
         """Get the FRED tags for a series.
 
         See the related FRED API documentation at:
 
             https://fred.stlouisfed.org/docs/api/fred/tags.html
@@ -262,14 +269,16 @@
                 - "popularity"
                 - "created"
                 - "name"
                 - "group_id"
 
             sort_order: Sort results in ascending ("asc") or
                 descending ("desc") order.
+            paginate: Whether to manage `offset` automatically, making multiple
+                API calls until all results are returned.
             api_key: Your FRED API key. Defaults to the ``FRED_API_KEY``
                 environment variable.
 
         Returns:
             A dataframe containing data for all FRED economic data tags.
 
         Examples:
@@ -278,22 +287,21 @@
             0       census      src                       Census  2012-02-27 10:18:19-06          79        237692
             1          bls      src   Bureau of Labor Statistics  2012-02-27 10:18:19-06          89        175376
             2  realtor.com      src                               2020-03-24 11:15:04-05          66         90632
             3          bea      src  Bureau of Economic Analysis  2012-02-27 10:18:19-06          78         78842
             4      frb stl      src                St. Louis Fed  2012-02-27 10:18:19-06          68         78442
 
         """
-        data = _api.get(
+        return _api.maybe_paginate(
+            "tags",
             cls.url,
             realtime_start=realtime_start,
             realtime_end=realtime_end,
             tag_names=tag_names,
             tag_group_id=tag_group_id,
             search_text=search_text,
             limit=limit,
             offset=offset,
             order_by=order_by,
             sort_order=sort_order,
             api_key=api_key,
-        ).json()
-        data = data["tags"]
-        return pd.DataFrame(data)
+        )
```

### Comparing `finagg-0.3.1/src/finagg/fred/feat/_raw.py` & `finagg-1.0.0/src/finagg/fred/feat/_raw.py`

 * *Files identical despite different names*

### Comparing `finagg-0.3.1/src/finagg/fred/feat/_refined.py` & `finagg-1.0.0/src/finagg/fred/feat/_refined.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     @classmethod
     def _normalize(cls, df: pd.DataFrame, /) -> pd.DataFrame:
         """Normalize economic features columns."""
         df = (
             df.pivot(index="date", values="value", columns="series_id")
             .sort_index()
             .astype(float)
-            .fillna(method="ffill")
+            .ffill()
             .dropna()
         )
         df = utils.resolve_func_cols(sql.economic, df, drop=True, inplace=True)
         df.columns = df.columns.rename(None)
         df = utils.resolve_col_order(sql.economic, df)
         return df.dropna()
```

### Comparing `finagg-0.3.1/src/finagg/fred/sql.py` & `finagg-1.0.0/src/finagg/fred/sql.py`

 * *Files identical despite different names*

### Comparing `finagg-0.3.1/src/finagg/fundam/_cli.py` & `finagg-1.0.0/src/finagg/fundam/_cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -106,15 +106,15 @@
 
     if all_ or all_refined:
         if total_rows:
             logger.info(f"{total_rows} total rows inserted for {__package__}")
         else:
             logger.warning(
                 f"No rows were inserted for {__package__}. This could be an error if"
-                " installations were not skipped. Set the verbose flag with the"
+                " installations were skipped. Set the verbose flag with the"
                 " `--verbose/-v` option to enable debug logging."
             )
     else:
         logger.info(
             f"Skipping {__package__} installation because no installation "
             "options are provided"
         )
```

### Comparing `finagg-0.3.1/src/finagg/fundam/feat.py` & `finagg-1.0.0/src/finagg/fundam/feat.py`

 * *Files 2% similar despite different names*

```diff
@@ -139,15 +139,15 @@
             )
         if not len(df.index):
             raise NoResultFound(f"No industry fundamental rows found for {code}.")
         df = df.drop(columns=["ticker"])
         df = df.melt(["date"], var_name="name", value_name="value").set_index("date")
         return (
             df.groupby(["date", "name"])  # type: ignore[return-value]
-            .agg([np.mean, np.std])
+            .agg(["mean", "std"])
             .reset_index()
             .pivot(index=["date"], columns="name")["value"]
             .sort_index()
             .dropna()
         )
 
 
@@ -228,15 +228,15 @@
         company_df["date"] = date
         company_df = (
             company_df.reset_index()
             .set_index("date")
             .rename(lambda x: f"NORM({x})", axis=1)
         )
         company_df = (
-            company_df.fillna(method="ffill")
+            company_df.ffill()
             .reset_index()
             .dropna()
             .drop_duplicates("date")
             .set_index("date")
             .sort_index()
         )
         company_df = utils.resolve_col_order(sql.normalized_fundam, company_df)
@@ -600,15 +600,15 @@
         cls,
         quarterly: pd.DataFrame,
         prices: pd.DataFrame,
         /,
     ) -> pd.DataFrame:
         """Normalize the feature columns."""
         df = pd.merge(quarterly, prices, how="outer", left_index=True, right_index=True)
-        df = df.replace([-np.inf, np.inf], np.nan).fillna(method="ffill")
+        df = df.replace([-np.inf, np.inf], np.nan).ffill()
         df["PriceBookRatio"] = df["close"] / df["BookRatio"]
         df["PriceEarningsRatio"] = df["close"] / df["EarningsPerShareBasic"]
         df.index.names = ["date"]
         df = utils.resolve_col_order(sql.fundam, df)
         return df.dropna()
 
     @classmethod
```

### Comparing `finagg-0.3.1/src/finagg/fundam/sql.py` & `finagg-1.0.0/src/finagg/fundam/sql.py`

 * *Files identical despite different names*

### Comparing `finagg-0.3.1/src/finagg/indices/_cli.py` & `finagg-1.0.0/src/finagg/indices/_cli.py`

 * *Files identical despite different names*

### Comparing `finagg-0.3.1/src/finagg/indices/api.py` & `finagg-1.0.0/src/finagg/indices/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Indices API (symbols in popular indices)."""
 
+import io
 import os
 from abc import ABC, abstractmethod
 from datetime import timedelta
 from functools import cache
 from typing import ClassVar
 
 import pandas as pd
@@ -61,15 +62,16 @@
             3             Apple   NASDAQ   AAPL  Information technology  2015-03-19  0.0284
             4            Boeing     NYSE     BA   Aerospace and defense  1987-03-12  0.0336
 
         """
         response = _get(cls.url, user_agent=user_agent)
         soup = BeautifulSoup(response.text, "html.parser")
         tbl = soup.find("table", {"class": "wikitable"})
-        (df,) = pd.read_html(str(tbl))
+        tbl_io = io.StringIO(str(tbl))
+        (df,) = pd.read_html(tbl_io)
         df = pd.DataFrame(df)
 
         def _percent_to_fraction(item: str) -> float:
             value, _ = item.split("%")
             return float(value) / 100
 
         df.drop("Notes", axis=1, inplace=True)
@@ -111,15 +113,16 @@
             3                       Airbnb   ABNB  Consumer Discretionary     Internet & Direct Marketing Retail
             4             Align Technology   ALGN             Health Care                   Health Care Supplies
 
         """
         response = _get(cls.url, user_agent=user_agent)
         soup = BeautifulSoup(response.text, "html.parser")
         tbl = soup.find_all("table", {"class": "wikitable"})[3]
-        (df,) = pd.read_html(str(tbl))
+        tbl_io = io.StringIO(str(tbl))
+        (df,) = pd.read_html(tbl_io)
         df = pd.DataFrame(df)
         return df.rename(
             columns={
                 "Company": "company",
                 "Ticker": "ticker",
                 "GICS Sector": "industry",
                 "GICS Sub-Industry": "sub_industry",
@@ -151,15 +154,16 @@
             3     ABBV                AbbVie             Health Care ...
             4      ACN             Accenture  Information Technology ...
 
         """
         response = _get(cls.url, user_agent=user_agent)
         soup = BeautifulSoup(response.text, "html.parser")
         tbl = soup.find("table", {"class": "wikitable"})
-        (df,) = pd.read_html(str(tbl))
+        tbl_io = io.StringIO(str(tbl))
+        (df,) = pd.read_html(tbl_io)
         df = pd.DataFrame(df)
         df.drop("SEC filings", axis=1, inplace=True, errors="ignore")
         return df.rename(
             columns={
                 "Symbol": "ticker",
                 "Security": "company",
                 "GICS Sector": "industry",
```

### Comparing `finagg-0.3.1/src/finagg/indices/sql.py` & `finagg-1.0.0/src/finagg/indices/sql.py`

 * *Files identical despite different names*

### Comparing `finagg-0.3.1/src/finagg/portfolio.py` & `finagg-1.0.0/src/finagg/portfolio.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,25 +16,25 @@
         quantity: Number of shares held at ``cost``.
 
     """
 
     # Average dollar cost for each share in the position.
     _average_cost_basis: Decimal
 
-    # Total dollar cost for all shares in the position.
-    # The amount of dollars or cash invested in this security.
-    _cost_basis_total: Decimal
-
     # Current number of shares owned in the position.
     _quantity: Decimal
 
+    # Total dollar cost for all shares in the position.
+    # The amount of dollars or cash invested in this security.
+    _total_cost_basis: Decimal
+
     def __init__(self, cost: float, quantity: float, /) -> None:
         self._average_cost_basis = Decimal(cost)
         self._quantity = Decimal(quantity)
-        self._cost_basis_total = self._average_cost_basis * self._quantity
+        self._total_cost_basis = self._average_cost_basis * self._quantity
 
     def __eq__(self, __o: object) -> bool:
         """Compare the position's cost basis."""
         if not isinstance(__o, float | Position):
             raise TypeError(
                 "Can only compare "
                 f"{self.__class__.__name__} to [{float.__name__}, {Position.__name__}]"
@@ -59,22 +59,14 @@
         return self._average_cost_basis < __o
 
     @property
     def average_cost_basis(self) -> float:
         """Average dollar cost for each share in the position."""
         return float(self._average_cost_basis)
 
-    @property
-    def cost_basis_total(self) -> float:
-        """Total dollar cost for all shares in the position. The amount of
-        dollars or cash invested in this security.
-
-        """
-        return float(self._cost_basis_total)
-
     def buy(self, cost: float, quantity: float, /) -> float:
         """Buy ``quantity`` of the position for ``cost``.
 
         Args:
             cost: Cost to buy at.
             quantity: Number of shares to buy.
 
@@ -82,27 +74,27 @@
             Value of the bought position.
 
         Examples:
             >>> from finagg.portfolio import Position
             >>> pos = Position(100.0, 1)
             >>> pos.buy(50.0, 1)
             50.0
-            >>> pos.cost_basis_total
+            >>> pos.total_cost_basis
             150.0
             >>> pos.average_cost_basis
             75.0
             >>> pos.quantity
             2.0
 
         """
         exact_cost = Decimal(cost)
         exact_quantity = Decimal(quantity)
         self._quantity += exact_quantity
-        self._cost_basis_total = self._cost_basis_total + exact_cost * exact_quantity
-        self._average_cost_basis = self._cost_basis_total / self._quantity
+        self._total_cost_basis = self._total_cost_basis + exact_cost * exact_quantity
+        self._average_cost_basis = self._total_cost_basis / self._quantity
         return float(exact_cost * exact_quantity)
 
     @property
     def quantity(self) -> float:
         """Current number of shares owned in the position."""
         return float(self._quantity)
 
@@ -121,30 +113,38 @@
                 to sell in the position.
 
         Examples:
             >>> from finagg.portfolio import Position
             >>> pos = Position(100.0, 2)
             >>> pos.sell(50.0, 1)
             50.0
-            >>> pos.cost_basis_total
+            >>> pos.total_cost_basis
             100.0
             >>> pos.average_cost_basis
             100.0
             >>> pos.quantity
             1.0
 
         """
         exact_cost = Decimal(cost)
         exact_quantity = Decimal(quantity)
         if self._quantity < exact_quantity:
             raise ValueError("Invalid order - not enough shares.")
         self._quantity -= exact_quantity
-        self._cost_basis_total = self._average_cost_basis * self._quantity
+        self._total_cost_basis = self._average_cost_basis * self._quantity
         return float(exact_cost * exact_quantity)
 
+    @property
+    def total_cost_basis(self) -> float:
+        """Total dollar cost for all shares in the position. The amount of
+        dollars or cash invested in this security.
+
+        """
+        return float(self._total_cost_basis)
+
     def total_dollar_change(self, cost: float, /) -> float:
         """Compute the total dollar change relative to the average
         cost basis and the current value of the security.
 
         Args:
             cost: Current value of one share.
 
@@ -209,26 +209,26 @@
 
     """
 
     # Total liquid cash on-hand.
     _cash: Decimal
 
     # Total cash deposited since starting the portfolio.
-    _deposits_total: Decimal
+    _total_deposits: Decimal
+
+    # Total cash withdrawn since starting the portfolio.
+    _total_withdrawals: Decimal
 
     #: Existing positions for each security.
     positions: dict[str, Position]
 
-    # Total cash withdrawn since starting the portfolio.
-    _withdrawals_total: Decimal
-
     def __init__(self, cash: float, /) -> None:
         self._cash = Decimal(cash)
-        self._deposits_total = self._cash
-        self._withdrawals_total = Decimal(0)
+        self._total_deposits = self._cash
+        self._total_withdrawals = Decimal(0)
         self.positions = {}
 
     def __contains__(self, symbol: str) -> bool:
         """Return whether the portfolio contains a position
         in ``symbol``.
 
         """
@@ -264,15 +264,15 @@
 
         Examples:
             >>> from finagg.portfolio import Portfolio
             >>> port = Portfolio(1000.0)
             >>> port.buy("AAPL", 100.0, 1)
             100.0
             >>> pos = port["AAPL"]
-            >>> pos.cost_basis_total
+            >>> pos.total_cost_basis
             100.0
             >>> pos.average_cost_basis
             100.0
             >>> pos.quantity
             1.0
 
         """
@@ -294,22 +294,17 @@
 
         Returns:
             Total cash in the portfolio.
 
         """
         exact_cash = Decimal(cash)
         self._cash += exact_cash
-        self._deposits_total += exact_cash
+        self._total_deposits += exact_cash
         return float(self._cash)
 
-    @property
-    def deposits_total(self) -> float:
-        """Total cash deposited since starting the portfolio."""
-        return float(self._deposits_total)
-
     def sell(self, symbol: str, cost: float, quantity: float, /) -> float:
         """Sell ``quantity`` of security with `symbol` for ``cost``.
 
         Args:
             symbol: Security ticker.
             cost: Cost to sell the symbol at.
             quantity: Number of shares to sell.
@@ -322,28 +317,33 @@
             >>> from finagg.portfolio import Portfolio
             >>> port = Portfolio(1000.0)
             >>> port.buy("AAPL", 100.0, 2)
             200.0
             >>> port.sell("AAPL", 50.0, 1)
             50.0
             >>> pos = port["AAPL"]
-            >>> pos.cost_basis_total
+            >>> pos.total_cost_basis
             100.0
             >>> pos.average_cost_basis
             100.0
             >>> pos.quantity
             1.0
 
         """
         current_value = self.positions[symbol].sell(cost, quantity)
         if not self.positions[symbol]._quantity:
             self.positions.pop(symbol)
         self._cash += Decimal(cost) * Decimal(quantity)
         return float(current_value)
 
+    @property
+    def total_deposits(self) -> float:
+        """Total cash deposited since starting the portfolio."""
+        return float(self._total_deposits)
+
     def total_dollar_change(self, costs: dict[str, float], /) -> float:
         """Compute the total dollar change relative to the total
         deposits made into the portfolio.
 
         Args:
             costs: Mapping of symbol to its current value of one share.
 
@@ -355,15 +355,15 @@
             >>> port = Portfolio(1000.0)
             >>> port.buy("AAPL", 100.0, 1)
             100.0
             >>> port.total_dollar_change({"AAPL": 50.0})
             -50.0
 
         """
-        return float(Decimal(self.total_dollar_value(costs)) - self._deposits_total)
+        return float(Decimal(self.total_dollar_value(costs)) - self._total_deposits)
 
     def total_dollar_value(self, costs: dict[str, float], /) -> float:
         """Compute the total dollar value of the portfolio.
 
         Args:
             costs: Mapping of symbol to its current value of one share.
 
@@ -375,19 +375,19 @@
             >>> port = Portfolio(1000.0)
             >>> port.buy("AAPL", 100.0, 1)
             100.0
             >>> port.total_dollar_value({"AAPL": 50.0})
             950.0
 
         """
-        dollar_value_total = self._cash
+        total_dollar_value = self._cash
         for symbol, cost in costs.items():
             if symbol in self.positions:
-                dollar_value_total += Decimal(cost) * self.positions[symbol]._quantity
-        return float(dollar_value_total)
+                total_dollar_value += Decimal(cost) * self.positions[symbol]._quantity
+        return float(total_dollar_value)
 
     def total_log_change(self, costs: dict[str, float], /) -> float:
         """Compute the total log change relative to the total
         deposits made into the portfolio.
 
         Args:
             costs: Mapping of symbol to its current value of one share.
@@ -402,15 +402,15 @@
             >>> port.buy("AAPL", 100.0, 1)
             100.0
             >>> port.total_log_change({"AAPL": 50.0})
             -0.051293294387550536
 
         """
         return float(
-            Decimal(self.total_dollar_value(costs)).ln() - self._deposits_total.ln()
+            Decimal(self.total_dollar_value(costs)).ln() - self._total_deposits.ln()
         )
 
     def total_percent_change(self, costs: dict[str, float], /) -> float:
         """Compute the total percent change relative to the total
         deposits made into the portfolio.
 
         Args:
@@ -426,17 +426,22 @@
             >>> port.buy("AAPL", 100.0, 1)
             100.0
             >>> port.total_percent_change({"AAPL": 50.0})
             -0.05
 
         """
         return float(
-            (Decimal(self.total_dollar_value(costs)) / self._deposits_total) - 1
+            (Decimal(self.total_dollar_value(costs)) / self._total_deposits) - 1
         )
 
+    @property
+    def total_withdrawals(self) -> float:
+        """Total cash withdrawn since starting the portfolio."""
+        return float(self._total_withdrawals)
+
     def withdraw(self, cash: float, /) -> float:
         """Withdraw cash from the portfolio.
 
         Args:
             cash: Cash to withdraw.
 
         Returns:
@@ -453,14 +458,9 @@
             900.0
 
         """
         exact_cash = Decimal(cash)
         if self._cash < exact_cash:
             raise ValueError("Not enough cash to withdraw.")
         self._cash -= exact_cash
-        self._withdrawals_total += exact_cash
+        self._total_withdrawals += exact_cash
         return float(self._cash)
-
-    @property
-    def withdraws_total(self) -> float:
-        """Total cash withdrawn since starting the portfolio."""
-        return float(self._withdrawals_total)
```

### Comparing `finagg-0.3.1/src/finagg/ratelimit.py` & `finagg-1.0.0/src/finagg/ratelimit.py`

 * *Files identical despite different names*

### Comparing `finagg-0.3.1/src/finagg/sec/_cli.py` & `finagg-1.0.0/src/finagg/sec/_cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -240,15 +240,15 @@
 
     if all_ or all_refined or all_raw:
         if total_rows:
             logger.info(f"{total_rows} total rows inserted for {__package__}")
         else:
             logger.warning(
                 f"No rows were inserted for {__package__}. This could be an error if"
-                " installations were not skipped. Set the verbose flag with the"
+                " installations were skipped. Set the verbose flag with the"
                 " `--verbose/-v` option to enable debug logging."
             )
     else:
         logger.info(
             f"Skipping {__package__} installation because no installation "
             "options were provided"
         )
```

### Comparing `finagg-0.3.1/src/finagg/sec/api.py` & `finagg-1.0.0/src/finagg/sec/api.py`

 * *Files 5% similar despite different names*

```diff
@@ -190,59 +190,56 @@
         results = pd.concat(results_list)
         for k, v in content.items():
             results[k] = v
         results["cik"] = cik
         return results.rename(columns={"entityName": "entity", "val": "value"})
 
     @classmethod
-    def join_get(
+    def get_multiple_original(
         cls,
         concepts: list[Concept],
         *,
         cik: None | str = None,
         ticker: None | str = None,
-        form: str = "10-Q",
+        form: None | str = None,
         start: None | str = None,
         end: None | str = None,
         user_agent: None | str = None,
     ) -> pd.DataFrame:
-        """Return unique XBRL disclosures for a single company and filing
-        form from a set of company concepts.
-
-        Tags are also joined and pivoted such that each tag has its own
-        column. Gaps in reporting periods are forward-filled.
+        """Return original (not amended) XBRL disclosures for a single company
+        using a set of company concepts.
 
         Args:
             concepts: Company concepts to retrieve.
             cik: Company SEC CIK. Mutually exclusive with ``ticker``.
             ticker: Company ticker. Mutually exclusive with ``cik``.
             form: SEC filing form type to include. ``"10-Q"`` is for quarterly
-                filing forms and ``"10-K"`` is for annual filing forms.
+                filing forms and ``"10-K"`` is for annual filing forms. Ignored
+                if left ``None``.
             start: The start date of the observation period. Defaults to the
                 first recorded date.
             end: The end date of the observation period. Defaults to the
                 last recorded date.
             user_agent: Self-declared bot header. Defaults to the value
                 found in the ``SEC_API_USER_AGENT`` environment variable.
 
         Returns:
             Pivoted dataframe with a tag per column.
 
         Examples:
-            >>> finagg.sec.api.company_concept.join_get(
+            >>> finagg.sec.api.company_concept.get_multiple_original(
             ...     finagg.sec.api.popular_concepts,
             ...     ticker="AAPL",
             ... ).head(5)  # doctest: +SKIP
-                                      Assets  AssetsCurrent  CommonStockSharesOutstanding ...
-            fy   fp filed                                                                 ...
-            2009 Q3 2009-07-22  3.957200e+10   3.231100e+10                   888325973.0 ...
-            2010 Q1 2010-01-25  4.750100e+10   3.155500e+10                   899805500.0 ...
-                 Q2 2010-04-21  4.750100e+10   3.155500e+10                   899805500.0 ...
-                 Q3 2010-07-21  4.750100e+10   3.155500e+10                   899805500.0 ...
-            2011 Q1 2011-01-19  7.518300e+10   4.167800e+10                   915970050.0 ...
+                fy  fp     tag         end         value  ...
+            0  2009  Q3  Assets  2009-06-27  4.814000e+10 ...
+            1  2010  Q1  Assets  2009-12-26  5.392600e+10 ...
+            2  2010  Q2  Assets  2010-03-27  5.705700e+10 ...
+            3  2010  Q3  Assets  2010-06-26  6.472500e+10 ...
+            4  2011  Q1  Assets  2010-12-25  8.674200e+10 ...
 
         """
         start = start or "1776-07-04"
         end = end or utils.today
         dfs = []
         for concept in concepts:
             tag = concept["tag"]
@@ -252,19 +249,18 @@
                 tag,
                 cik=cik,
                 ticker=ticker,
                 taxonomy=taxonomy,
                 units=units,
                 user_agent=user_agent,
             )
-            df = get_unique_filings(df, form=form, units=units)
+            df = filter_original_filings(df, form=form, units=units)
             df = df[(df["filed"] >= start) & (df["filed"] <= end)]
             dfs.append(df)
         df = pd.concat(dfs)
-        df = join_filings(df, form=form)
         return df
 
 
 class CompanyFacts(API):
     """Get all XBRL disclosures for a single company.
 
     The module variable :data:`finagg.sec.api.company_facts` is an instance of
@@ -360,15 +356,15 @@
         if ticker:
             cik = str(get_cik(ticker))
 
         cik = str(cik).zfill(10)
         url = cls.url.format(cik=cik)
         response = _get(url, user_agent=user_agent)
         content = response.json()
-        df = _parse_facts(content)
+        df = _parse_company_facts(content)
         df["cik"] = cik
         return df
 
 
 class Exchanges(API):
     """SEC-registered ticker info with exchange data.
 
@@ -615,15 +611,15 @@
         response = _get(url, user_agent=user_agent)
         content = response.json()
         recent_filings = content.pop("filings")["recent"]
         df = pd.DataFrame(recent_filings)
         df.columns = map(utils.snake_case, df.columns)  # type: ignore
         df.rename(columns={"accession_number": "accn"})
         df["cik"] = cik
-        metadata = _parse_metadata(content)
+        metadata = _parse_submission_metadata(content)
         metadata["cik"] = cik
         metadata["ticker"] = str(ticker)
         return {"metadata": metadata, "filings": df}
 
 
 class Tickers(API):
     """SEC-registered ticker info.
@@ -823,14 +819,115 @@
         response = session.get(url, headers=headers, stream=stream)
     else:
         response = requests.get(url, headers=headers, stream=stream)
     response.raise_for_status()
     return response
 
 
+def compute_financial_ratios(df: pd.DataFrame, /) -> pd.DataFrame:
+    """Compute financial ratios in-place for a dataframe using XBRL financial
+    tags.
+
+    Args:
+        df: Dataframe with common XBRL financial tags (e.g., "Assets",
+            "Liabilities", etc.).
+
+    Returns:
+        ``df`` but with additional columns that're normalized financial ratios.
+
+    """
+    df["AssetCoverageRatio"] = (df["Assets"] - df["LiabilitiesCurrent"]) / df[
+        "Liabilities"
+    ]
+    df["BookRatio"] = (df["Assets"] - df["Liabilities"]) / df[
+        "CommonStockSharesOutstanding"
+    ]
+    df["DebtEquityRatio"] = df["Liabilities"] / df["StockholdersEquity"]
+    df["QuickRatio"] = (df["AssetsCurrent"] - df["InventoryNet"]) / df[
+        "LiabilitiesCurrent"
+    ]
+    df["ReturnOnAssets"] = df["NetIncomeLoss"] / df["Assets"]
+    df["ReturnOnEquity"] = df["NetIncomeLoss"] / df["StockholdersEquity"]
+    df["WorkingCapitalRatio"] = df["AssetsCurrent"] / df["LiabilitiesCurrent"]
+    return df
+
+
+def filter_original_filings(
+    df: pd.DataFrame, /, *, form: None | str = None, units: None | str = None
+) -> pd.DataFrame:
+    """Get all original filing rows as determined by the filing date and
+    tag for a period.
+
+    Args:
+        df: Dataframe without mixed original and amendment rows.
+        form: Only keep rows with form type ``form``. Most popular choices
+            include ``"10-K"`` for annual and ``"10-Q"`` for quarterly.
+            This parameter is ignored if left ``None``.
+        units: Only keep rows with units ``units`` if not ``None``.
+
+    Returns:
+        Dataframe with rows that only correspond to original filings.
+
+    Examples:
+        Only get a company's original quarterly earnings-per-share filings.
+
+        >>> df = finagg.sec.api.company_concept.get(
+        ...     "EarningsPerShareBasic",
+        ...     ticker="AAPL",
+        ...     taxonomy="us-gaap",
+        ...     units="USD/shares",
+        ... )
+        >>> finagg.sec.api.filter_original_filings(
+        ...     df,
+        ...     form="10-Q",
+        ...     units="USD/shares"
+        ... ).head(5)  # doctest: +SKIP
+             fy  fp  ...
+        0  2009  Q3  ...
+        1  2010  Q1  ...
+        2  2010  Q2  ...
+        3  2010  Q3  ...
+        4  2011  Q1  ...
+
+    """
+    end = pd.DatetimeIndex(df["end"])
+    filed = pd.DatetimeIndex(df["filed"])
+    filing_delay = filed - end
+    # Make sure filings occurs within 90 days of the reporting end date.
+    # Helps ensure each filing is the first filing and not an amendment.
+    mask = filing_delay.days <= 90
+    if form:
+        mask &= df["form"] == form
+        # Not all filings contain a start date, but it can be helpful to
+        # use the start date to ensure the filing corresponds to the time
+        # period we care about.
+        if "start" in df:
+            start: pd.DatetimeIndex = pd.DatetimeIndex(df["start"])
+            start_to_end = end - start
+        match form:
+            case "10-K":
+                mask &= df["fp"] == "FY"
+                # Make sure the reporting frame is close to a year.
+                if "start" in df:
+                    mask &= start.isna() | ((350 <= start_to_end.days) & (start_to_end.days <= 380))  # type: ignore[no-untyped-call]
+            case "10-Q":
+                mask &= df["fp"].str.startswith("Q")
+                # Make sure the reporting frame is close to a quarter.
+                if "start" in df:
+                    mask &= start.isna() | ((75 <= start_to_end.days) & (start_to_end.days <= 105))  # type: ignore[no-untyped-call]
+    if units:
+        mask &= df["units"] == units
+    df = df[mask]
+    return (
+        df.sort_values(["fy", "fp", "filed"])
+        .groupby(["fy", "fp", "tag"], as_index=False)
+        .first()
+    )
+
+
 def get_cik(ticker: str, /, *, user_agent: None | str = None) -> str:
     """Return a company's SEC CIK from its ticker.
 
     Args:
         ticker: A company's ticker symbol.
         user_agent: Self-declared SEC bot header. Defaults to the value
             found in the ``SEC_API_USER_AGENT`` environment variable.
@@ -851,42 +948,14 @@
         for _, items in content.items():
             normalized_cik = str(items["cik_str"]).zfill(10)
             _tickers_to_cik[items["ticker"]] = normalized_cik
             _cik_to_tickers[normalized_cik] = items["ticker"]
     return _tickers_to_cik[ticker.upper()]
 
 
-def get_financial_ratios(df: pd.DataFrame, /) -> pd.DataFrame:
-    """Compute financial ratios in-place for a dataframe using XBRL financial
-    tags.
-
-    Args:
-        df: Dataframe with common XBRL financial tags (e.g., "Assets",
-            "Liabilities", etc.).
-
-    Returns:
-        ``df`` but with additional columns that're normalized financial ratios.
-
-    """
-    df["AssetCoverageRatio"] = (df["Assets"] - df["LiabilitiesCurrent"]) / df[
-        "Liabilities"
-    ]
-    df["BookRatio"] = (df["Assets"] - df["Liabilities"]) / df[
-        "CommonStockSharesOutstanding"
-    ]
-    df["DebtEquityRatio"] = df["Liabilities"] / df["StockholdersEquity"]
-    df["QuickRatio"] = (df["AssetsCurrent"] - df["InventoryNet"]) / df[
-        "LiabilitiesCurrent"
-    ]
-    df["ReturnOnAssets"] = df["NetIncomeLoss"] / df["Assets"]
-    df["ReturnOnEquity"] = df["NetIncomeLoss"] / df["StockholdersEquity"]
-    df["WorkingCapitalRatio"] = df["AssetsCurrent"] / df["LiabilitiesCurrent"]
-    return df
-
-
 def get_ticker(cik: str, /, *, user_agent: None | str = None) -> str:
     """Return a company's ticker from its SEC CIK.
 
     Args:
         cik: A company's 10-character SEC CIK.
         user_agent: Self-declared SEC bot header. Defaults to the value
             found in the ``SEC_API_USER_AGENT`` environment variable.
@@ -961,102 +1030,55 @@
                     ticker = get_ticker(cik)
                 except KeyError:
                     continue
                 tickers.add(ticker)
     return tickers
 
 
-def get_unique_filings(
-    df: pd.DataFrame, /, *, form: str = "10-Q", units: None | str = None
+def group_and_pivot_filings(
+    df: pd.DataFrame, /, *, form: None | str = None
 ) -> pd.DataFrame:
-    """Get all unique rows as determined by the filing date and tag for a
-    period.
-
-    Args:
-        df: Dataframe without unique rows.
-        form: Only keep rows with form type ``form``. Most popular choices
-            include ``"10-K"`` for annual and ``"10-Q"`` for quarterly.
-        units: Only keep rows with units ``units`` if not ``None``.
-
-    Returns:
-        Dataframe with unique rows.
-
-    Examples:
-        Only get a company's original quarterly earnings-per-share filings.
-
-        >>> df = finagg.sec.api.company_concept.get(
-        ...     "EarningsPerShareBasic",
-        ...     ticker="AAPL",
-        ...     taxonomy="us-gaap",
-        ...     units="USD/shares",
-        ... )
-        >>> finagg.sec.api.get_unique_filings(
-        ...     df,
-        ...     form="10-Q",
-        ...     units="USD/shares"
-        ... ).head(5)  # doctest: +SKIP
-             fy  fp  ...
-        0  2009  Q3  ...
-        1  2010  Q1  ...
-        2  2010  Q2  ...
-        3  2010  Q3  ...
-        4  2011  Q1  ...
-
-    """
-    mask = df["form"] == form
-    match form:
-        case "10-K":
-            mask &= df["fp"] == "FY"
-        case "10-Q":
-            mask &= df["fp"].str.startswith("Q")
-    if units:
-        mask &= df["units"] == units
-    df = df[mask]
-    return (
-        df.sort_values(["fy", "fp", "filed"])
-        .groupby(["fy", "fp", "tag"], as_index=False)
-        .first()
-    )
-
-
-def join_filings(df: pd.DataFrame, /, *, form: str = "10-Q") -> pd.DataFrame:
-    """Helper for joining filings into a pivoted dataframe such that each
+    """Helper for grouping filings into a pivoted dataframe such that each
     tag has its own column.
 
-    Tags are joined according to fiscal year and fiscal period. The newest
+    Tags are grouped according to fiscal year and fiscal period. The newest
     filing date is used when tags have different filing dates for the same
     fiscal year and fiscal period. Tags are forward-filled to fill gaps
     in filings.
 
     Args:
         df: "Melted" dataframe where each filing is a row.
-        form: Type of form to join. ``"10-K"`` sets the index to the fiscal
+        form: Type of form to group. ``"10-K"`` sets the index to the fiscal
             year and filing date whereas ``"10-Q"`` sets the index to the
-            fiscal year, fiscal period, and filing date.
+            fiscal year, fiscal period, and filing date. If not provided,
+            the form type is chosen by inspecting the first element of the
+            ``"form"`` column.
 
     Returns:
         A pivoted dataframe where each column is a tag.
 
     Examples:
         Get all XBRL filings from a company, unintelligently select the first
-        unique filings for each XBRL tag, and then join all filings into
+        unique filings for each XBRL tag, and then group all filings into
         a pivoted table.
 
         >>> df = finagg.sec.api.company_facts.get(ticker="AAPL")
-        >>> df = finagg.sec.api.get_unique_filings(df, form="10-K")
-        >>> finagg.sec.api.join_filings(df, form="10-K")  # doctest: +SKIP
+        >>> df = finagg.sec.api.filter_original_filings(df, form="10-K")
+        >>> finagg.sec.api.group_and_pivot_filings(df, form="10-K")  # doctest: +SKIP
                          AccountsPayableCurrent  AccountsReceivableNetCurrent ...
         fy   filed                                                            ...
         2009 2009-10-27            5.520000e+09                  2.422000e+09 ...
         2010 2010-10-27            5.601000e+09                  3.361000e+09 ...
         2011 2011-10-26            1.201500e+10                  5.510000e+09 ...
         2012 2012-10-31            1.463200e+10                  5.369000e+09 ...
         2013 2013-10-30            2.117500e+10                  1.093000e+10 ...
 
     """
+    if form is None:
+        form = df.iloc[0]["form"]
     match form:
         case "10-K":
             df = df.drop(columns=["fp"]).set_index(["fy"]).sort_index()
             df["filed"] = df.groupby(["fy"])["filed"].max()
             df = df.reset_index().pivot(
                 index=["fy", "filed"],
                 columns="tag",
@@ -1070,15 +1092,15 @@
                 columns="tag",
                 values="value",
             )
     df.columns = df.columns.rename(None)
     return df
 
 
-def _parse_facts(content: dict[str, Any], /) -> pd.DataFrame:
+def _parse_company_facts(content: dict[str, Any], /) -> pd.DataFrame:
     """Helper for parsing company facts.
 
     This function is only defined to make parsing company
     facts easier and common between parsing from the REST
     API responses and the bulk zip file.
 
     Args:
@@ -1104,15 +1126,15 @@
     for k, v in content.items():
         results[k] = v
     return results.rename(
         columns={"entityName": "entity", "uom": "units", "val": "value"}
     )
 
 
-def _parse_metadata(content: dict[str, Any], /) -> dict[str, Any]:
+def _parse_submission_metadata(content: dict[str, Any], /) -> dict[str, Any]:
     """Helper for parsing submission metadata.
 
     This function is only defined to make parsing submission
     metadata easier and common between parsing from the REST
     API responses and the bulk zip file.
 
     Args:
```

### Comparing `finagg-0.3.1/src/finagg/sec/feat/__init__.py` & `finagg-1.0.0/src/finagg/sec/feat/__init__.py`

 * *Files identical despite different names*

### Comparing `finagg-0.3.1/src/finagg/sec/feat/_raw.py` & `finagg-1.0.0/src/finagg/sec/feat/_raw.py`

 * *Files 0% similar despite different names*

```diff
@@ -215,15 +215,15 @@
             leave=True,
         ):
             try:
                 cik = f[3:-5]
                 ticker = api.get_ticker(cik)
                 data = zipfile.read(f)
                 content = json.loads(data)
-                metadata = api._parse_metadata(content)
+                metadata = api._parse_submission_metadata(content)
                 metadata["cik"] = cik
                 metadata["ticker"] = ticker
                 df = pd.DataFrame(metadata, index=[0])
                 cls.to_raw(df, engine=engine)
                 total_rows += 1
                 logger.debug(f"Inserted row for {f}")
             except Exception as e:
@@ -279,26 +279,28 @@
         zip_filename, filename = args
         zipfile = ZipFile(zip_filename)
         dfs = []
         cik = filename[3:-5]
         data = zipfile.read(filename)
         content = json.loads(data)
         try:
-            df = api._parse_facts(content)
+            df = api._parse_company_facts(content)
         except:
             return filename, pd.DataFrame()
         df["cik"] = cik
         for concept in api.popular_concepts:
             try:
                 tag = concept["tag"]
                 taxonomy = concept["taxonomy"]
                 units = concept["units"]
                 df_tag = df[(df["tag"] == tag) & (df["taxonomy"] == taxonomy)]
                 for form in ("10-K", "10-Q"):
-                    df_unique = api.get_unique_filings(df_tag, form=form, units=units)
+                    df_unique = api.filter_original_filings(
+                        df_tag, form=form, units=units
+                    )
                     if len(df_unique.index):
                         dfs.append(df_unique)
             except:
                 continue
         if dfs:
             return filename, pd.concat(dfs)
         return filename, pd.DataFrame()
@@ -442,14 +444,102 @@
                 )
                 .scalars()
                 .all()
             )
         return set(tickers)
 
     @classmethod
+    def group_and_pivot_from_raw(
+        cls,
+        ticker: str,
+        tags: list[str],
+        /,
+        *,
+        form: str = "10-Q",
+        start: None | str = None,
+        end: None | str = None,
+        engine: None | Engine = None,
+    ) -> pd.DataFrame:
+        """Get one or more company concept tags from raw SEC data.
+
+        Joins all the tags into one table, pivoting the columns such that
+        each tag is in its own column. Tags are forward-filled to fill
+        gaps.
+
+        Args:
+            ticker: Company ticker.
+            tags: Company concept tags to retreive.
+            form: SEC filing form to retrieve rows for. Options include:
+
+                - "10-Q" = quarterly filings
+                - "10-K" = annual filings
+
+            start: The start date of the observation period. Defaults to the
+                first recorded date.
+            end: The end date of the observation period. Defaults to the
+                last recorded date.
+            engine: Feature store database engine. Defaults to the engine
+                at :data:`finagg.backend.engine`.
+
+        Returns:
+            A dataframe containing the company concept tag values
+            across the specified period.
+
+        Raises:
+            `NoResultFound`: If there are no rows for ``ticker`` or any of
+                the tags in ``tags`` for ``ticker`` in the raw SQL table.
+
+        Examples:
+            >>> finagg.sec.feat.tags.group_and_pivot_from_raw(
+            ...     "AAPL",
+            ...     ["Assets", "EarningsPerShareBasic"],
+            ...     form="10-Q"
+            ... ).head(5)  # doctest: +SKIP
+                                      Assets  EarningsPerShareBasic
+            fy   fp filed
+            2009 Q3 2009-07-22  3.957200e+10                   4.20
+            2010 Q1 2010-01-25  4.750100e+10                   2.54
+                 Q2 2010-04-21  4.750100e+10                   4.35
+                 Q3 2010-07-21  4.750100e+10                   6.40
+            2011 Q1 2011-01-19  7.518300e+10                   3.74
+
+        """
+        start = start or "1776-07-04"
+        end = end or utils.today
+        engine = engine or backend.engine
+        if not sa.inspect(engine).has_table(sql.submissions.name):
+            sql.submissions.create(engine)
+        if not sa.inspect(engine).has_table(sql.tags.name):
+            sql.tags.create(engine)
+        with engine.begin() as conn:
+            df = pd.DataFrame(
+                conn.execute(
+                    sql.tags.select()
+                    .join(
+                        sql.submissions,
+                        (sql.submissions.c.cik == sql.tags.c.cik)
+                        & (sql.submissions.c.ticker == ticker),
+                    )
+                    .where(
+                        sql.tags.c.tag.in_(tags),
+                        sql.tags.c.form == form,
+                        sql.tags.c.filed >= start,
+                        sql.tags.c.filed <= end,
+                    )
+                )
+            )
+        if not len(df.index):
+            raise NoResultFound(f"No rows found for {ticker}.")
+        df = api.group_and_pivot_filings(df, form=form)
+        for tag in tags:
+            if tag not in df.columns:
+                raise NoResultFound(f"No {tag} rows found for {ticker}.")
+        return df
+
+    @classmethod
     def install(
         cls,
         tickers: None | set[str] = None,
         *,
         engine: None | Engine = None,
         recreate_tables: bool = False,
     ) -> int:
@@ -492,15 +582,17 @@
                     df = api.company_concept.get(
                         tag,
                         ticker=ticker,
                         taxonomy=taxonomy,
                         units=units,
                     )
                     for form in ("10-K", "10-Q"):
-                        df_unique = api.get_unique_filings(df, form=form, units=units)
+                        df_unique = api.filter_original_filings(
+                            df, form=form, units=units
+                        )
                         rowcount = len(df_unique.index)
                         if rowcount:
                             cls.to_raw(df_unique, engine=engine)
                             total_rows += rowcount
                             logger.debug(
                                 f"{rowcount} rows inserted for"
                                 f" {ticker} {tag} {form} filings"
@@ -584,102 +676,14 @@
                     else:
                         logger.debug(f"Skipping {f} due to missing filings")
                 except Exception as e:
                     logger.debug(f"Skipping {f}", exc_info=e)
         return total_rows
 
     @classmethod
-    def join_from_raw(
-        cls,
-        ticker: str,
-        tags: list[str],
-        /,
-        *,
-        form: str = "10-Q",
-        start: None | str = None,
-        end: None | str = None,
-        engine: None | Engine = None,
-    ) -> pd.DataFrame:
-        """Get one or more company concept tags from raw SEC data.
-
-        Joins all the tags into one table, pivoting the columns such that
-        each tag is in its own column. Tags are forward-filled to fill
-        gaps.
-
-        Args:
-            ticker: Company ticker.
-            tags: Company concept tags to retreive.
-            form: SEC filing form to retrieve rows for. Options include:
-
-                - "10-Q" = quarterly filings
-                - "10-K" = annual filings
-
-            start: The start date of the observation period. Defaults to the
-                first recorded date.
-            end: The end date of the observation period. Defaults to the
-                last recorded date.
-            engine: Feature store database engine. Defaults to the engine
-                at :data:`finagg.backend.engine`.
-
-        Returns:
-            A dataframe containing the company concept tag values
-            across the specified period.
-
-        Raises:
-            `NoResultFound`: If there are no rows for ``ticker`` or any of
-                the tags in ``tags`` for ``ticker`` in the raw SQL table.
-
-        Examples:
-            >>> finagg.sec.feat.tags.join_from_raw(
-            ...     "AAPL",
-            ...     ["Assets", "EarningsPerShareBasic"],
-            ...     form="10-Q"
-            ... ).head(5)  # doctest: +SKIP
-                                      Assets  EarningsPerShareBasic
-            fy   fp filed
-            2009 Q3 2009-07-22  3.957200e+10                   4.20
-            2010 Q1 2010-01-25  4.750100e+10                   2.54
-                 Q2 2010-04-21  4.750100e+10                   4.35
-                 Q3 2010-07-21  4.750100e+10                   6.40
-            2011 Q1 2011-01-19  7.518300e+10                   3.74
-
-        """
-        start = start or "1776-07-04"
-        end = end or utils.today
-        engine = engine or backend.engine
-        if not sa.inspect(engine).has_table(sql.submissions.name):
-            sql.submissions.create(engine)
-        if not sa.inspect(engine).has_table(sql.tags.name):
-            sql.tags.create(engine)
-        with engine.begin() as conn:
-            df = pd.DataFrame(
-                conn.execute(
-                    sql.tags.select()
-                    .join(
-                        sql.submissions,
-                        (sql.submissions.c.cik == sql.tags.c.cik)
-                        & (sql.submissions.c.ticker == ticker),
-                    )
-                    .where(
-                        sql.tags.c.tag.in_(tags),
-                        sql.tags.c.form == form,
-                        sql.tags.c.filed >= start,
-                        sql.tags.c.filed <= end,
-                    )
-                )
-            )
-        if not len(df.index):
-            raise NoResultFound(f"No rows found for {ticker}.")
-        df = api.join_filings(df, form=form)
-        for tag in tags:
-            if tag not in df.columns:
-                raise NoResultFound(f"No {tag} rows found for {ticker}.")
-        return df
-
-    @classmethod
     def to_raw(cls, df: pd.DataFrame, /, *, engine: None | Engine = None) -> int:
         """Write the given dataframe to the raw feature table.
 
         Args:
             df: Dataframe to store as rows in a local SQL table
             engine: Feature store database engine. Defaults to the engine
                 at :data:`finagg.backend.engine`.
```

### Comparing `finagg-0.3.1/src/finagg/sec/feat/_refined/annual.py` & `finagg-1.0.0/src/finagg/sec/feat/_refined/annual.py`

 * *Files 0% similar despite different names*

```diff
@@ -145,15 +145,15 @@
             ["fy"]
         )
         df["filed"] = df.groupby(["fy"])["filed"].max()
         return (
             df.reset_index()  # type: ignore[return-value]
             .set_index(["fy", "filed"])
             .groupby(["fy", "filed", "name"])
-            .agg([np.mean, np.std])
+            .agg(["mean", "std"])
             .reset_index()
             .pivot(index=["fy", "filed"], columns="name")["value"]
             .sort_index()
             .dropna()
         )
 
 
@@ -236,15 +236,15 @@
         company_df[func_cols] = company_df[func_cols].fillna(value=0.0)
         company_df = (
             company_df.reset_index()
             .set_index(["fy", "filed"])
             .rename(lambda x: f"NORM({x})", axis=1)
         )
         company_df = (
-            company_df.fillna(method="ffill")
+            company_df.ffill()
             .dropna()
             .reset_index()
             .drop_duplicates("filed")
             .set_index(["fy", "filed"])
             .sort_index()
         )
         company_df = utils.resolve_col_order(
@@ -607,16 +607,16 @@
 
     :meta hide-value:
     """
 
     @classmethod
     def _normalize(cls, df: pd.DataFrame, /) -> pd.DataFrame:
         """Normalize annual features columns."""
-        df = api.get_financial_ratios(df)
-        df = df.replace([-np.inf, np.inf], np.nan).fillna(method="ffill")
+        df = api.compute_financial_ratios(df)
+        df = df.replace([-np.inf, np.inf], np.nan).ffill()
         df = utils.resolve_func_cols(sql.annual, df, drop=True, inplace=True)
         df.columns = df.columns.rename(None)
         df = utils.resolve_col_order(sql.annual, df, extra_ignore=["filed"])
         return df.dropna()
 
     @classmethod
     def from_api(
@@ -642,17 +642,18 @@
             2010 2010-10-27           -0.089864                  -0.023676                                  0.012840 ...
             2011 2011-10-26            0.272493                   0.278241                                  0.017805 ...
             2012 2012-10-31            0.896033                   0.076422                                  0.014423 ...
             2013 2013-10-30            0.414064                   0.248046                                  0.010630 ...
             2014 2014-10-27            0.161871                   0.239927                                  1.902394 ...
 
         """
-        df = api.company_concept.join_get(
+        df = api.company_concept.get_multiple_original(
             api.popular_concepts, ticker=ticker, form="10-K", start=start, end=end
         )
+        df = api.group_and_pivot_filings(df, form="10-K")
         return cls._normalize(df)
 
     @classmethod
     def from_raw(
         cls,
         ticker: str,
         /,
@@ -687,15 +688,15 @@
             2010 2010-10-27           -0.089864                  -0.023676                                  0.012840 ...
             2011 2011-10-26            0.272493                   0.278241                                  0.017805 ...
             2012 2012-10-31            0.896033                   0.076422                                  0.014423 ...
             2013 2013-10-30            0.414064                   0.248046                                  0.010630 ...
             2014 2014-10-27            0.161871                   0.239927                                  1.902394 ...
 
         """
-        df = _raw.Tags.join_from_raw(
+        df = _raw.Tags.group_and_pivot_from_raw(
             ticker,
             [concept["tag"] for concept in api.popular_concepts],
             form="10-K",
             start=start,
             end=end,
             engine=engine,
         )
```

### Comparing `finagg-0.3.1/src/finagg/sec/feat/_refined/quarterly.py` & `finagg-1.0.0/src/finagg/sec/feat/_refined/quarterly.py`

 * *Files 0% similar despite different names*

```diff
@@ -147,15 +147,15 @@
             ["fy", "fp", "filed"], var_name="name", value_name="value"
         ).set_index(["fy", "fp"])
         df["filed"] = df.groupby(["fy", "fp"])["filed"].max()
         return (
             df.reset_index()  # type: ignore[return-value]
             .set_index(["fy", "fp", "filed"])
             .groupby(["fy", "fp", "filed", "name"])
-            .agg([np.mean, np.std])
+            .agg(["mean", "std"])
             .reset_index()
             .pivot(index=["fy", "fp", "filed"], columns="name")["value"]
             .sort_index()
             .dropna()
         )
 
 
@@ -238,15 +238,15 @@
         company_df[func_cols] = company_df[func_cols].fillna(value=0.0)
         company_df = (
             company_df.reset_index()
             .set_index(["fy", "fp", "filed"])
             .rename(lambda x: f"NORM({x})", axis=1)
         )
         company_df = (
-            company_df.fillna(method="ffill")
+            company_df.ffill()
             .reset_index()
             .dropna()
             .drop_duplicates("filed")
             .set_index(["fy", "fp", "filed"])
             .sort_index()
         )
         company_df = utils.resolve_col_order(
@@ -620,16 +620,16 @@
 
     :meta hide-value:
     """
 
     @classmethod
     def _normalize(cls, df: pd.DataFrame, /) -> pd.DataFrame:
         """Normalize quarterly features columns."""
-        df = api.get_financial_ratios(df)
-        df = df.replace([-np.inf, np.inf], np.nan).fillna(method="ffill")
+        df = api.compute_financial_ratios(df)
+        df = df.replace([-np.inf, np.inf], np.nan).ffill()
         df = utils.resolve_func_cols(sql.quarterly, df, drop=True, inplace=True)
         df.columns = df.columns.rename(None)
         df = utils.resolve_col_order(sql.quarterly, df, extra_ignore=["filed"])
         return df.dropna()
 
     @classmethod
     def from_api(
@@ -659,17 +659,18 @@
             2010 Q1 2010-01-25            0.182629                  -0.023676                                  0.012840 ...
                  Q2 2010-04-21            0.000000                   0.000000                                  0.000000 ...
                  Q3 2010-07-21            0.000000                   0.000000                                  0.000000 ...
             2011 Q1 2011-01-19            0.459174                   0.278241                                  0.017805 ...
                  Q2 2011-04-21            0.000000                   0.000000                                  0.000000 ...
 
         """
-        df = api.company_concept.join_get(
+        df = api.company_concept.get_multiple_original(
             api.popular_concepts, ticker=ticker, form="10-Q", start=start, end=end
         )
+        df = api.group_and_pivot_filings(df, form="10-Q")
         return cls._normalize(df)
 
     @classmethod
     def from_raw(
         cls,
         ticker: str,
         /,
@@ -704,15 +705,15 @@
             2010 Q1 2010-01-25            0.182629                  -0.023676                                  0.012840 ...
                  Q2 2010-04-21            0.000000                   0.000000                                  0.000000 ...
                  Q3 2010-07-21            0.000000                   0.000000                                  0.000000 ...
             2011 Q1 2011-01-19            0.459174                   0.278241                                  0.017805 ...
                  Q2 2011-04-21            0.000000                   0.000000                                  0.000000 ...
 
         """
-        df = _raw.Tags.join_from_raw(
+        df = _raw.Tags.group_and_pivot_from_raw(
             ticker,
             [concept["tag"] for concept in api.popular_concepts],
             form="10-Q",
             start=start,
             end=end,
             engine=engine,
         )
```

### Comparing `finagg-0.3.1/src/finagg/sec/sql.py` & `finagg-1.0.0/src/finagg/sec/sql.py`

 * *Files identical despite different names*

### Comparing `finagg-0.3.1/src/finagg/testing.py` & `finagg-1.0.0/src/finagg/testing.py`

 * *Files identical despite different names*

### Comparing `finagg-0.3.1/src/finagg/utils.py` & `finagg-1.0.0/src/finagg/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -223,15 +223,15 @@
         A series representing percent changes of ``col``.
 
     """
     if other is None:
         other = series.shift(1)
 
     out = series.apply(np.log) - other.apply(np.log)
-    return out.replace([-np.inf, np.inf], np.nan).fillna(method="ffill")
+    return out.replace([-np.inf, np.inf], np.nan).ffill()
 
 
 def safe_pct_change(series: pd.Series, other: None | pd.Series = None) -> pd.Series:  # type: ignore[type-arg]
     """Safely compute percent change between two columns.
 
     Replaces ``Inf`` values with ``NaN`` and forward-fills.
     This function is meant to be used with ``pd.Series.apply``.
@@ -245,15 +245,15 @@
         A series representing percent changes of ``col``.
 
     """
     if other is None:
         other = series.shift(1)
 
     out = (series - other) / other
-    return out.replace([-np.inf, np.inf], np.nan).fillna(method="ffill")
+    return out.replace([-np.inf, np.inf], np.nan).ffill()
 
 
 def setenv(name: str, value: str, /, *, exist_ok: bool = False) -> pathlib.Path:
     """Set the value of the environment variable ``name`` to ``value``.
 
     The environment variable is permanently set in the environment
     and in the current process.
```

### Comparing `finagg-0.3.1/src/finagg/yfinance/_cli.py` & `finagg-1.0.0/src/finagg/yfinance/_cli.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,24 +11,21 @@
 
 logging.basicConfig(
     format="%(asctime)s | %(levelname)s | %(message)s", level=logging.INFO
 )
 logger = logging.getLogger(__name__)
 
 
-@click.group(help="Yahoo! finance tools.")
+@click.group(help="Yahoo! Finance tools.")
 def entry_point() -> None:
     ...
 
 
 @entry_point.command(
-    help=(
-        "Drop and recreate tables, and install the recommended "
-        "tables into the SQL database."
-    ),
+    help="Install Yahoo! Finance stock price and price feature data.",
 )
 @click.option(
     "--raw",
     type=click.Choice(["prices"]),
     multiple=True,
     help=(
         "Raw tables to install. `prices` indicates daily historical stock "
@@ -170,16 +167,132 @@
 
     if all_ or all_refined or all_raw:
         if total_rows:
             logger.info(f"{total_rows} total rows inserted for {__package__}")
         else:
             logger.warning(
                 f"No rows were inserted for {__package__}. This could be an error if"
-                " installations were not skipped. Set the verbose flag with the"
+                " installations were skipped. Set the verbose flag with the"
                 " `--verbose/-v` option to enable debug logging."
             )
     else:
         logger.info(
             f"Skipping {__package__} installation because no installation "
             "options are provided"
         )
     return total_rows
+
+
+@entry_point.command(
+    help="Update Yahoo! Finance stock price and price feature data.",
+)
+@click.option(
+    "--raw",
+    type=click.Choice(["prices"]),
+    multiple=True,
+    help=(
+        "Raw tables to update. `prices` indicates daily historical stock "
+        "price data. `prices` must be specified to enable updating refined "
+        "data using the `refined` flag."
+    ),
+)
+@click.option(
+    "--refined",
+    type=click.Choice(["daily"]),
+    multiple=True,
+    help=(
+        "Refined tables to update. This requires raw data to be "
+        "updated beforehand using the `--raw` flag or for the "
+        "`--raw` flag to be set when this option is provided."
+    ),
+)
+@click.option(
+    "--all",
+    "-a",
+    "all_",
+    is_flag=True,
+    default=False,
+    help="Whether to update all defined tables (including all refined tables).",
+)
+@click.option(
+    "--ticker",
+    "-t",
+    multiple=True,
+    help=(
+        "Ticker whose data is attempted to be downloaded and inserted into "
+        "the SQL tables. Multiple tickers can be specified by providing "
+        "multiple `ticker` options, by separating tickers with a comma (e.g., "
+        "`AAPL,MSFT,NVDA`), or by providing tickers in a CSV file by "
+        "specifying a file path (e.g., `bank_tickers.txt`). The CSV file "
+        "can be formatted such that there's one ticker per line or multiple "
+        "tickers per line (delimited by a comma)."
+    ),
+)
+@click.option(
+    "--processes",
+    "-n",
+    type=int,
+    default=mp.cpu_count() - 1,
+    help=(
+        "Number of backgruond processes to run in parallel when updating. Note,"
+        " not all tables support updates with multiprocessing."
+    ),
+)
+@click.option(
+    "--verbose",
+    "-v",
+    is_flag=True,
+    default=False,
+    help="Sets the log level to DEBUG to show update errors for each ticker.",
+)
+def update(
+    raw: list[Literal["prices"]] = [],
+    refined: list[Literal["daily"]] = [],
+    all_: bool = False,
+    ticker: list[str] = [],
+    processes: int = mp.cpu_count() - 1,
+    verbose: bool = False,
+) -> int:
+    if verbose:
+        logging.getLogger(__package__).setLevel(logging.DEBUG)
+
+    total_rows = 0
+    all_raw = set()
+    if all_:
+        all_raw = {"prices"}
+    elif raw:
+        all_raw = set(raw)
+
+    all_tickers = utils.expand_csv(ticker)
+    if all_raw:
+        if "prices" in all_raw:
+            total_rows += _feat.prices.update(
+                all_tickers,
+                processes=processes,
+            )
+
+    all_refined = set()
+    if all_:
+        all_refined = {"daily"}
+    elif refined:
+        all_refined = set(refined)
+
+    if "daily" in all_refined:
+        total_rows += _feat.daily.update(
+            tickers=all_tickers,
+            processes=processes,
+        )
+
+    if all_ or all_refined or all_raw:
+        if total_rows:
+            logger.info(f"{total_rows} total rows inserted for {__package__}")
+        else:
+            logger.warning(
+                f"No rows were inserted for {__package__}. This could be an error if"
+                " updates were skipped. Set the verbose flag with the"
+                " `--verbose/-v` option to enable debug logging."
+            )
+    else:
+        logger.info(
+            f"Skipping {__package__} update because no update options are provided"
+        )
+    return total_rows
```

### Comparing `finagg-0.3.1/src/finagg/yfinance/api.py` & `finagg-1.0.0/src/finagg/yfinance/api.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Simple wrappers for Yahoo! Finance."""
 
 import logging
+from datetime import datetime, timedelta
 
 import pandas as pd
 import yfinance as yf
 
 logging.getLogger("yfinance").setLevel(logging.CRITICAL)
 
 
@@ -42,14 +43,20 @@
         0  1980-12-12  0.0997  0.1002  0.0997  0.0997  469033600   AAPL
         1  1980-12-15  0.0950  0.0950  0.0945  0.0945  175884800   AAPL
         2  1980-12-16  0.0880  0.0880  0.0876  0.0876  105728000   AAPL
         3  1980-12-17  0.0897  0.0902  0.0897  0.0897   86441600   AAPL
         4  1980-12-18  0.0924  0.0928  0.0924  0.0924   73449600   AAPL
 
     """
+    # yfinance returns data exclusive of the end date if provided,
+    # so we add an extra day to be consistent across all other
+    # methods that're inclusive of the end date.
+    if end is not None:
+        end_plus_one = datetime.fromisoformat(end) + timedelta(days=1)
+        end = end_plus_one.strftime("%Y-%m-%d")
     stock = yf.Ticker(ticker)
     df = stock.history(
         period=period,
         interval=interval,
         start=start,
         end=end,
         auto_adjust=True,
```

### Comparing `finagg-0.3.1/src/finagg/yfinance/feat/_raw.py` & `finagg-1.0.0/src/finagg/yfinance/feat/_raw.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """Raw features from Yahoo! Finance sources."""
 
 import logging
 import multiprocessing as mp
+from datetime import datetime, timedelta
 
 import pandas as pd
 import sqlalchemy as sa
 from sqlalchemy.engine import Engine
-from sqlalchemy.exc import NoResultFound
+from sqlalchemy.exc import NoResultFound, NoSuchTableError
 from tqdm import tqdm
 
 from ... import backend, indices, utils
 from .. import api, sql
 
 logging.basicConfig(
     format="%(asctime)s | %(levelname)s | %(message)s", level=logging.INFO
@@ -25,21 +26,24 @@
     The module variable :data:`finagg.yfinance.feat.prices` is an instance of
     this feature set implementation and is the most popular interface for
     calling feature methods.
 
     """
 
     @classmethod
-    def _install_worker(cls, ticker: str) -> tuple[None | Exception, str, pd.DataFrame]:
+    def _install_worker(
+        cls, args: tuple[str, None | str]
+    ) -> tuple[None | Exception, str, pd.DataFrame]:
         """Helper for installing data from the Yahoo! Finance API using
         multiprocessing.
 
         """
+        ticker, start = args
         try:
-            df = api.get(ticker)
+            df = api.get(ticker, start=start)
         except Exception as e:
             return e, ticker, pd.DataFrame()
         return None, ticker, df
 
     @classmethod
     def from_raw(
         cls,
@@ -188,15 +192,17 @@
         if recreate_tables or not sa.inspect(engine).has_table(sql.prices.name):
             sql.prices.drop(engine, checkfirst=True)
             sql.prices.create(engine)
 
         total_rows = 0
         with mp.Pool(processes) as pool:
             for exc, ticker, df in tqdm(
-                pool.imap_unordered(cls._install_worker, tickers),
+                pool.imap_unordered(
+                    cls._install_worker, [(ticker, None) for ticker in tickers]
+                ),
                 desc="Installing raw Yahoo! Finance stock data",
                 total=len(tickers),
                 position=0,
                 leave=True,
             ):
                 if exc:
                     logger.debug(f"Skipping {ticker}", exc_info=exc)
@@ -228,7 +234,74 @@
         """
         engine = engine or backend.engine
         if not sa.inspect(engine).has_table(sql.prices.name):
             sql.prices.create(engine)
         with engine.begin() as conn:
             conn.execute(sql.prices.insert(), df.to_dict(orient="records"))  # type: ignore[arg-type]
         return len(df)
+
+    @classmethod
+    def update(
+        cls,
+        tickers: None | set[str] = None,
+        *,
+        processes: int = mp.cpu_count() - 1,
+        engine: None | Engine = None,
+    ) -> int:
+        """Update data associated with ``tickers`` by pulling data from the
+        API, and then writing the data to the raw prices SQL table.
+
+        Args:
+            tickers: Set of tickers to install features for. Defaults to all
+                the tickers from :meth:`finagg.yfinance.feat.Prices.get_ticker_set`.
+            processes: Number of background processes to use when installing
+                data.
+            engine: Feature store database engine. Defaults to the engine
+                at :data:`finagg.backend.engine`.
+
+        Returns:
+            Number of rows written to the feature's raw SQL table.
+
+        Raises:
+            `NoSuchTableError`: If the table associated with this feature
+                set update does not exist.
+
+        """
+        tickers = tickers or cls.get_ticker_set()
+        engine = engine or backend.engine
+        if not sa.inspect(engine).has_table(sql.prices.name):
+            raise NoSuchTableError(f"{sql.prices.name} table does not exist.")
+
+        with engine.begin() as conn:
+            result = conn.execute(
+                sa.select(sql.prices.c.ticker, sa.func.max(sql.prices.c.date))
+                .where(sql.prices.c.ticker.in_(tickers))
+                .group_by(sql.prices.c.ticker)
+            )
+        updates = []
+        for ticker, start in result:
+            start_plus_one = datetime.fromisoformat(start) + timedelta(days=1)
+            updates.append((ticker, start_plus_one.strftime("%Y-%m-%d")))
+
+        total_rows = 0
+        with mp.Pool(processes) as pool:
+            for exc, ticker, df in tqdm(
+                pool.imap_unordered(cls._install_worker, updates),
+                desc="Updating raw Yahoo! Finance stock data",
+                total=len(updates),
+                position=0,
+                leave=True,
+            ):
+                if exc:
+                    logger.debug(f"Skipping {ticker}", exc_info=exc)
+                    continue
+                try:
+                    rowcount = len(df.index)
+                    if rowcount:
+                        cls.to_raw(df, engine=engine)
+                        total_rows += rowcount
+                        logger.debug(f"{rowcount} rows inserted for {ticker}")
+                    else:
+                        logger.debug(f"Skipping {ticker} due to missing stock data")
+                except Exception as e:
+                    logger.debug(f"Skipping {ticker}", exc_info=e)
+        return total_rows
```

### Comparing `finagg-0.3.1/src/finagg/yfinance/feat/_refined.py` & `finagg-1.0.0/src/finagg/yfinance/feat/_refined.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import logging
 import multiprocessing as mp
 
 import numpy as np
 import pandas as pd
 import sqlalchemy as sa
 from sqlalchemy.engine import Engine
-from sqlalchemy.exc import NoResultFound
+from sqlalchemy.exc import NoResultFound, NoSuchTableError
 
 from ... import backend, utils
 from .. import api, sql
 from . import _raw
 
 logging.basicConfig(
     format="%(asctime)s | %(levelname)s | %(message)s", level=logging.INFO
@@ -35,18 +35,39 @@
         >>> df3 = finagg.yfinance.feat.daily.from_refined("AAPL").head(5)
         >>> pd.testing.assert_frame_equal(df1, df2, rtol=1e-4)
         >>> pd.testing.assert_frame_equal(df1, df3, rtol=1e-4)
 
     """
 
     @classmethod
+    def _from_raw_for_update(
+        cls,
+        ticker: str,
+        /,
+        *,
+        start: None | str = None,
+        end: None | str = None,
+        engine: None | Engine = None,
+    ) -> pd.DataFrame:
+        """Helper for getting raw features for the update method."""
+        engine = engine or backend.engine
+        if start is None:
+            with engine.begin() as conn:
+                (start,) = conn.execute(
+                    sa.select(sa.func.max(sql.daily.c.date)).where(
+                        sql.daily.c.ticker == ticker
+                    )
+                ).one()
+        return cls.from_raw(ticker, start=start, end=end, engine=engine)
+
+    @classmethod
     def _normalize(cls, df: pd.DataFrame, /) -> pd.DataFrame:
         """Normalize daily features columns."""
         df = df.drop(columns=["ticker"]).set_index("date").sort_index()
-        df = df.replace([-np.inf, np.inf], np.nan).fillna(method="ffill")
+        df = df.replace([-np.inf, np.inf], np.nan).ffill()
         df = utils.resolve_func_cols(sql.daily, df, drop=True, inplace=True)
         return df.dropna()
 
     @classmethod
     def from_api(
         cls, ticker: str, /, *, start: None | str = None, end: None | str = None
     ) -> pd.DataFrame:
@@ -363,7 +384,50 @@
         if not sa.inspect(engine).has_table(sql.daily.name):
             sql.daily.create(engine)
         df = df.reset_index("date")
         df["ticker"] = ticker
         with engine.begin() as conn:
             conn.execute(sql.daily.insert(), df.to_dict(orient="records"))  # type: ignore[arg-type]
         return len(df.index)
+
+    @classmethod
+    def update(
+        cls,
+        tickers: None | set[str] = None,
+        *,
+        processes: int = mp.cpu_count() - 1,
+        engine: None | Engine = None,
+    ) -> int:
+        """Update data associated with ``tickers`` by pulling data from the
+        raw SQL tables, transforming them into daily features, and then writing
+        to the refined daily SQL table.
+
+        Args:
+            tickers: Set of tickers to install features for. Defaults to all
+                the tickers from :meth:`finagg.yfinance.feat.Daily.get_ticker_set`.
+            processes: Number of background processes to run in parallel
+                when processing ``tickers``.
+            engine: Feature store database engine. Defaults to the engine
+                at :data:`finagg.backend.engine`.
+
+        Returns:
+            Number of rows written to the feature's refined SQL table.
+
+        Raises:
+            `NoSuchTableError`: If the table associated with this feature
+                set update does not exist.
+
+        """
+        tickers = tickers or cls.get_ticker_set()
+        engine = engine or backend.engine
+        if not sa.inspect(engine).has_table(sql.prices.name):
+            raise NoSuchTableError(f"{sql.daily.name} table does not exist.")
+
+        return utils._install(
+            cls._from_raw_for_update,
+            cls.to_refined,
+            logger,
+            list(tickers),
+            engine,
+            desc="Updating refined Yahoo! Finance daily data",
+            processes=processes,
+        )
```

### Comparing `finagg-0.3.1/src/finagg/yfinance/sql.py` & `finagg-1.0.0/src/finagg/yfinance/sql.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     metadata,
     sa.Column("ticker", sa.String, primary_key=True, doc="Unique company ticker."),
     sa.Column("date", sa.String, primary_key=True, doc="Stock price date."),
     sa.Column("open", sa.Float, doc="Stock price at market open."),
     sa.Column("high", sa.Float, doc="Stock price max during trading hours."),
     sa.Column("low", sa.Float, doc="Stock price min during trading hours."),
     sa.Column("close", sa.Float, doc="Stock price at market close."),
-    sa.Column("volume", sa.Float, doc="Units traded during trading hours."),
+    sa.Column("volume", sa.Integer, doc="Units traded during trading hours."),
 )
 """SQL table for storing raw data as managed by
 :data:`finagg.yfinance.feat.prices` (an alias for
 :class:`finagg.yfinance.feat.Prices`).
 
 :meta hide-value:
 """
```

### Comparing `finagg-0.3.1/src/finagg.egg-info/PKG-INFO` & `finagg-1.0.0/src/finagg.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finagg
-Version: 0.3.1
+Version: 1.0.0
 Summary: Data aggregation with popular and free financial APIs.
 Author: Andrew B.
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -216,20 +216,20 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Office/Business :: Financial :: Investment
 Classifier: Topic :: Software Development
 Classifier: Topic :: Scientific/Engineering
 Classifier: Typing :: Typed
 Requires-Python: >=3.10
-Description-Content-Type: text/x-rst
+Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: beautifulsoup4==4.*
 Requires-Dist: click==8.*
-Requires-Dist: pandas==1.*
-Requires-Dist: pandas-stubs==1.*
+Requires-Dist: pandas==2.*
+Requires-Dist: pandas-stubs==2.*
 Requires-Dist: python-dotenv==0.21.*
 Requires-Dist: requests==2.*
 Requires-Dist: requests-cache==0.9.*
 Requires-Dist: SQLAlchemy==2.*
 Requires-Dist: tqdm==4.*
 Requires-Dist: types-requests==2.*
 Requires-Dist: typing-extensions==4.*
@@ -242,304 +242,306 @@
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: pytest-xdist; extra == "dev"
 Requires-Dist: pytest-randomly; extra == "dev"
 Requires-Dist: sphinx; extra == "dev"
 Requires-Dist: tox; extra == "dev"
 Requires-Dist: virtualenv; extra == "dev"
 
-finagg: Financial Aggregation for Python
-========================================
+# finagg: Financial Aggregation for Python
 
 **finagg** is a Python package that provides implementations of popular and free
 financial APIs, tools for aggregating historical data from those APIs into SQL
 databases, and tools for transforming aggregated data into features useful for
 analysis and AI/ML.
 
 * **Documentation**: https://theogognf.github.io/finagg/
 * **PyPI**: https://pypi.org/project/finagg/
 * **Repository**: https://github.com/theOGognf/finagg
 
-Quick Start
-===========
+# Quick Start
 
-Installation
-------------
+## Installation
 
-Install with pip for the latest (stable) version.
+Install with pip for the latest stable version.
 
-.. code:: console
+```console
+pip install finagg
+```
 
-  pip install finagg
+Install from GitHub for the latest unstable version.
 
-Install from GitHub for the latest (unstable) version.
-
-.. code:: console
-
-    git clone https://github.com/theOGognf/finagg.git
-    pip install ./finagg/
+```console
+git clone https://github.com/theOGognf/finagg.git
+pip install ./finagg/
+```
 
 Optionally install the recommended datasets (economic data, company
 financials, stock histories, etc.) from 3rd party APIs into a local SQL
 database.
 
-.. code:: console
-
-    finagg install -ss economic -ts indices -z -r
+```console
+finagg install -ss economic -ts indices -z -r
+```
 
 The installation will point you where to get free API keys for each API that
 requires one and will write those API keys to a local ``.env`` file for storage.
 Run ``finagg install --help`` for more installation options and details.
 
-Basic Usage
------------
+## Basic Usage
 
-These are just **finagg** usage samples. See the `documentation`_ for all the
+These are just **finagg** usage samples. See the [documentation][4] for all the
 supported APIs and features.
 
-Explore the APIs directly
-^^^^^^^^^^^^^^^^^^^^^^^^^
+### Explore the APIs directly
 
 *These methods require internet access and API keys/user agent declarations.*
 
 Get Bureau of Economic Analysis (BEA) data.
 
+```pycon
 >>> finagg.bea.api.gdp_by_industry.get(year=[2019]).head(5)
    table_id freq  year quarter industry                         industry_description ...
 0         1    Q  2019       1       11  Agriculture, forestry, fishing, and hunting ...
 1         1    Q  2019       1    111CA                                        Farms ...
 2         1    Q  2019       1    113FF    Forestry, fishing, and related activities ...
 3         1    Q  2019       1       21                                       Mining ...
 4         1    Q  2019       1      211                       Oil and gas extraction ...
+```
 
 Get Federal Reserve Economic Data (FRED).
 
+```pycon
 >>> finagg.fred.api.series.observations.get(
 ...   "CPIAUCNS",
 ...   realtime_start=0,
 ...   realtime_end=-1,
 ...   output_type=4
 ... ).head(5)
   realtime_start realtime_end        date  value series_id
 0     1949-04-22   1953-02-26  1949-03-01  169.5  CPIAUCNS
 1     1949-05-23   1953-02-26  1949-04-01  169.7  CPIAUCNS
 2     1949-06-24   1953-02-26  1949-05-01  169.2  CPIAUCNS
 3     1949-07-22   1953-02-26  1949-06-01  169.6  CPIAUCNS
 4     1949-08-26   1953-02-26  1949-07-01  168.5  CPIAUCNS
+```
 
 Get Securities and Exchange Commission (SEC) filings.
 
+```pycon
 >>> finagg.sec.api.company_facts.get(ticker="AAPL").head(5)
           end        value                  accn    fy  fp    form       filed ...
 0  2009-06-27  895816758.0  0001193125-09-153165  2009  Q3    10-Q  2009-07-22 ...
 1  2009-10-16  900678473.0  0001193125-09-214859  2009  FY    10-K  2009-10-27 ...
 2  2009-10-16  900678473.0  0001193125-10-012091  2009  FY  10-K/A  2010-01-25 ...
 3  2010-01-15  906794589.0  0001193125-10-012085  2010  Q1    10-Q  2010-01-25 ...
 4  2010-04-09  909938383.0  0001193125-10-088957  2010  Q2    10-Q  2010-04-21 ...
+```
 
-Use installed raw data for exploring the most popular features
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+### Use installed raw data for exploring the most popular features
 
 *These methods require internet access, API keys/user agent declarations, and
 downloading and installing raw data through the* ``finagg install`` *or*
 ``finagg <api/subpackage> install`` *commands.*
 
 Get the most popular FRED features all in one dataframe.
 
+```pycon
 >>> finagg.fred.feat.economic.from_raw().head(5)
             CIVPART  LOG_CHANGE(CPIAUCNS)  LOG_CHANGE(CSUSHPINSA)  FEDFUNDS ...
 date                                                                        ...
 2014-10-06     62.8                   0.0                     0.0      0.09 ...
 2014-10-08     62.8                   0.0                     0.0      0.09 ...
 2014-10-13     62.8                   0.0                     0.0      0.09 ...
 2014-10-15     62.8                   0.0                     0.0      0.09 ...
 2014-10-20     62.8                   0.0                     0.0      0.09 ...
+```
 
 Get quarterly report features from SEC data.
 
+```pycon
 >>> finagg.sec.feat.quarterly.from_raw("AAPL").head(5)
                     LOG_CHANGE(Assets)  LOG_CHANGE(AssetsCurrent) ...
 fy   fp filed                                                     ...
 2010 Q1 2010-01-25            0.182629                  -0.023676 ...
      Q2 2010-04-21            0.000000                   0.000000 ...
      Q3 2010-07-21            0.000000                   0.000000 ...
 2011 Q1 2011-01-19            0.459174                   0.278241 ...
      Q2 2011-04-21            0.000000                   0.000000 ...
+```
 
 Get an aggregation of quarterly and daily features for a particular ticker.
 
+```pycon
 >>> finagg.fundam.feat.fundam.from_raw("AAPL").head(5)
             PriceBookRatio  PriceEarningsRatio
 date
 2010-01-25        0.175061            2.423509
 2010-01-26        0.178035            2.464678
 2010-01-27        0.178813            2.475448
 2010-01-28        0.177154            2.452471
 2010-01-29        0.173825            2.406396
+```
 
-Use installed features for exploring refined aggregations of raw data
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+### Use installed features for exploring refined aggregations of raw data
 
 *These methods require installing refined data through the* ``finagg install``
 *or* ``finagg <api/subpackage> install`` *commands.*
 
 Get a ticker's industry's averaged quarterly report features.
 
+```pycon
 >>> finagg.sec.feat.quarterly.industry.from_refined(ticker="AAPL").head(5)
                                  mean                           ...
 name               AssetCoverageRatio BookRatio DebtEquityRatio ...
 fy   fp filed                                                   ...
 2014 Q1 2014-05-15          10.731301  9.448954        0.158318 ...
      Q2 2014-08-14          10.731301  9.448954        0.158318 ...
      Q3 2014-11-14          10.731301  9.448954        0.158318 ...
 2015 Q1 2015-05-15          16.738972  9.269250        0.294238 ...
      Q2 2015-08-13          16.738972  9.269250        0.294238 ...
+```
 
 Get a ticker's industry-averaged quarterly report features.
 
+```pycon
 >>> finagg.sec.feat.quarterly.normalized.from_refined("AAPL").head(5)
                     NORM(LOG_CHANGE(Assets))  NORM(LOG_CHANGE(AssetsCurrent)) ...
 fy   fp filed                                                                 ...
 2010 Q2 2010-04-21                  0.000000                         0.000000 ...
      Q3 2010-07-21                  0.000000                         0.000000 ...
 2011 Q1 2011-01-19                  0.978816                         0.074032 ...
      Q2 2011-04-21                  0.000000                         0.000000 ...
      Q3 2011-07-20                 -0.353553                        -0.353553 ...
+```
 
 Get tickers sorted by an industry-averaged quarterly report feature.
 
+```pycon
 >>> finagg.sec.feat.quarterly.normalized.get_tickers_sorted_by(
 ...   "NORM(EarningsPerShareBasic)",
 ...   year=2019
 ... )[:5]
 ['XRAY', 'TSLA', 'SYY', 'WHR', 'KMB']
+```
 
 Get tickers sorted by an industry-averaged fundamental feature.
 
+```pycon
 >>> finagg.fundam.feat.fundam.normalized.get_tickers_sorted_by(
 ...   "NORM(PriceEarningsRatio)",
 ...   date="2019-01-04"
 ... )[:5]
 ['AMD', 'TRGP', 'HPE', 'CZR', 'TSLA']
+```
 
-Configuration
-=============
+# Configuration
 
-API Keys and User Agents
-------------------------
+## API Keys and User Agents
 
 API keys and user agent declarations are required for most of the APIs.
 You can set environment variables to expose your API keys and user agents
 to **finagg**, or you can pass your API keys and user agents to the implemented
 APIs programmatically. The following environment variables are used for
 configuring API keys and user agents:
 
 * ``BEA_API_KEY`` is for the Bureau of Economic Analysis's API key. You can get
-  a free API key from the `BEA API site`_.
+  a free API key from the [BEA API site][3].
 * ``FRED_API_KEY`` is for the Federal Reserve Economic Data API key. You can get
-  a free API key from the `FRED API site`_.
+  a free API key from the [FRED API site][8].
 * ``INDICES_API_USER_AGENT`` is for scraping popular indices' compositions from
   Wikipedia and should be equivalent to a browser's user agent declaration.
   This defaults to a hardcoded value, but it may not always work.
 * ``SEC_API_USER_AGENT`` is for the Securities and Exchange Commission's API. This
   should be of the format ``FIRST_NAME LAST_NAME E_MAIL``.
 
-Data Locations
---------------
+## Data Locations
 
 **finagg**'s root path, HTTP cache path, and database path are all configurable
 through environment variables. By default, all data related to **finagg** is put
 in a ``./findata`` directory relative to a root directory. You can change these
 locations by modifying the respective environment variables:
 
 * ``FINAGG_ROOT_PATH`` points to the parent directory of the ``./findata`` directory.
   Defaults to your current working directory.
 * ``FINAGG_HTTP_CACHE_PATH`` points to the HTTP requests cache SQLite storage.
   Defaults to ``./findata/http_cache.sqlite``.
 * ``FINAGG_DATABASE_URL`` points to the **finagg** data storage. Defaults to
   ``./findata/finagg.sqlite``.
 
-Dependencies
-============
+# Dependencies
 
-* `pandas`_ for fast, flexible, and expressive representations of relational data.
-* `requests`_ for HTTP requests to 3rd party APIs.
-* `requests-cache`_ for caching HTTP requests to avoid getting throttled by 3rd
+* [pandas][11] for fast, flexible, and expressive representations of relational data.
+* [requests][12] for HTTP requests to 3rd party APIs.
+* [requests-cache][13] for caching HTTP requests to avoid getting throttled by 3rd
   party API servers.
-* `SQLAlchemy`_ for a SQL Python interface.
-* `yfinance`_ for historical stock data from Yahoo! Finance.
+* [SQLAlchemy][17] for a SQL Python interface.
+* [yfinance][18] for historical stock data from Yahoo! Finance.
 
-API References
-==============
+# API References
 
-* The `BEA API`_ and the `BEA API key registration link`_.
-* The `FRED API`_ and the `FRED API key registration link`_.
-* The `SEC API`_.
+* The [BEA API][1] and the [BEA API key registration link][2].
+* The [FRED API][6] and the [FRED API key registration link][7].
+* The [SEC API][14].
 
-Related Projects
-================
+# Related Projects
 
-* `FinRL`_ is a collection of financial reinforcement learning environments
+* [FinRL][5] is a collection of financial reinforcement learning environments
   and tools.
-* `fredapi`_ is an implementation of the FRED API.
-* `OpenBBTerminal`_ is an open-source version of the Bloomberg Terminal.
-* `sec-edgar`_ is an implementation of a file-based SEC EDGAR parser.
-* `sec-edgar-api`_ is an implementation of the SEC EDGAR REST API.
+* [fredapi][9] is an implementation of the FRED API.
+* [OpenBBTerminal][10] is an open-source version of the Bloomberg Terminal.
+* [sec-edgar][15] is an implementation of a file-based SEC EDGAR parser.
+* [sec-edgar-api][16] is an implementation of the SEC EDGAR REST API.
 
-Frequently Asked Questions
-==========================
+# Frequently Asked Questions
 
-Where should I start?
----------------------
+## Where should I start?
 
 Aggregate some data, create some analysis notebooks, or create some RL
 environments using the implemented data features and SQL tables. This
 project was originally created to make RL environments for financial
 applications but has since focused its purpose to just aggregating financial
 data and features. That being said, all the implemented features are
 defined in such a way to make it very easy to develop financial AI/ML,
 so we encourage you to do just that!
 
-Why aren't features being installed for a specific ticker or economic data series?
-----------------------------------------------------------------------------------
+## Why aren't features being installed for a specific ticker or economic data series?
 
 Implemented APIs may be relatively new and simply may not provide data for a
 particular ticker or economic data series. For example, earnings per share may
 not be accessible for all companies through the SEC EDGAR API. In some cases,
 APIs may raise an HTTP error, causing installations to skip the ticker or
 series. Additionally, not all tickers and economic data series contain
 sufficient data for feature normalization. If a ticker or series only has one
 data point, that data point could be dropped when computing a feature (such as
 percent change), causing no data to be installed.
 
-What Python versions are supported?
------------------------------------
+## What Python versions are supported?
 
 Python 3.10 and up are supported. We don't plan on supporting lower versions
 because 3.10 introduces some nice quality of life updates that are used
 throughout the package.
 
-What operating systems are supported?
--------------------------------------
+## What operating systems are supported?
 
 The package is developed and tested on both Linux and Windows, but we recommend
 using Linux or WSL in practice. The package performs a good amount of I/O and
 interprocess operations that could result in a noticeable performance
 degradation on Windows.
 
-.. _`BEA API`: https://apps.bea.gov/api/signup/
-.. _`BEA API key registration link`: https://apps.bea.gov/API/signup/
-.. _`BEA API site`: https://apps.bea.gov/API/signup/
-.. _`documentation`: https://theogognf.github.io/finagg/
-.. _`FinRL`: https://github.com/AI4Finance-Foundation/FinRL
-.. _`FRED API`: https://fred.stlouisfed.org/docs/api/fred/
-.. _`FRED API key registration link`: https://fredaccount.stlouisfed.org/login/secure/
-.. _`FRED API site`: https://fredaccount.stlouisfed.org/login/secure/
-.. _`fredapi`: https://github.com/mortada/fredapi
-.. _`OpenBBTerminal`: https://github.com/OpenBB-finance/OpenBBTerminal
-.. _`pandas`: https://pandas.pydata.org/
-.. _`requests`: https://requests.readthedocs.io/en/latest/
-.. _`requests-cache`: https://requests-cache.readthedocs.io/en/stable/
-.. _`SEC API`: https://www.sec.gov/edgar/sec-api-documentation
-.. _`sec-edgar`: https://github.com/sec-edgar/sec-edgar
-.. _`sec-edgar-api`: https://github.com/jadchaar/sec-edgar-api
-.. _`SQLAlchemy`: https://www.sqlalchemy.org/
-.. _`yfinance`: https://github.com/ranaroussi/yfinance
+[1]: https://apps.bea.gov/api/signup/
+[2]: https://apps.bea.gov/API/signup/
+[3]: https://apps.bea.gov/API/signup/
+[4]: https://theogognf.github.io/finagg/
+[5]: https://github.com/AI4Finance-Foundation/FinRL
+[6]: https://fred.stlouisfed.org/docs/api/fred/
+[7]: https://fredaccount.stlouisfed.org/login/secure/
+[8]: https://fredaccount.stlouisfed.org/login/secure/
+[9]: https://github.com/mortada/fredapi
+[10]: https://github.com/OpenBB-finance/OpenBBTerminal
+[11]: https://pandas.pydata.org/
+[12]: https://requests.readthedocs.io/en/latest/
+[13]: https://requests-cache.readthedocs.io/en/stable/
+[14]: https://www.sec.gov/edgar/sec-api-documentation
+[15]: https://github.com/sec-edgar/sec-edgar
+[16]: https://github.com/jadchaar/sec-edgar-api
+[17]: https://www.sqlalchemy.org/
+[18]: https://github.com/ranaroussi/yfinance
```

### Comparing `finagg-0.3.1/src/finagg.egg-info/SOURCES.txt` & `finagg-1.0.0/src/finagg.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 .gitignore
 .pre-commit-config.yaml
 LICENSE
-README.rst
+README.md
 pyproject.toml
 .github/workflows/build-docs.yml
 .github/workflows/test-and-publish.yml
 .github/workflows/test.yml
 docs/.nojekyll
 docs/Makefile
 docs/cli.rst
@@ -14,14 +14,15 @@
 docs/conventions.rst
 docs/faq.rst
 docs/index.html
 docs/index.rst
 docs/installation.rst
 docs/make.bat
 docs/references.rst
+docs/release_notes.rst
 docs/requirements.txt
 docs/walkthroughs.rst
 docs/_static/custom.css
 src/finagg/__init__.py
 src/finagg/__main__.py
 src/finagg/backend.py
 src/finagg/frame.py
```

### Comparing `finagg-0.3.1/tests/test_frame.py` & `finagg-1.0.0/tests/test_frame.py`

 * *Files identical despite different names*

### Comparing `finagg-0.3.1/tests/test_fred/test_feat.py` & `finagg-1.0.0/tests/test_fred/test_feat.py`

 * *Files identical despite different names*

### Comparing `finagg-0.3.1/tests/test_fundam/test_feat.py` & `finagg-1.0.0/tests/test_fundam/test_feat.py`

 * *Files identical despite different names*

### Comparing `finagg-0.3.1/tests/test_portfolio.py` & `finagg-1.0.0/tests/test_portfolio.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     return Position(INITIAL_COST, INITIAL_QUANTITY)
 
 
 def test_portfolio_buy(portfolio: Portfolio, position: Position) -> None:
     portfolio.buy("TEST", INITIAL_COST, INITIAL_QUANTITY)
     assert portfolio.cash == (INITIAL_CASH - (INITIAL_COST * INITIAL_QUANTITY))
     assert portfolio["TEST"] == position
-    assert portfolio["TEST"].cost_basis_total == position.cost_basis_total
+    assert portfolio["TEST"].total_cost_basis == position.total_cost_basis
     assert portfolio["TEST"].quantity == position.quantity
 
 
 def test_portfolio_sell(portfolio: Portfolio) -> None:
     portfolio.buy("TEST", INITIAL_COST, INITIAL_QUANTITY)
     portfolio.sell("TEST", CHANGE_MULTIPLE * INITIAL_COST, INITIAL_QUANTITY)
     assert portfolio.cash == (
@@ -49,46 +49,46 @@
         portfolio.total_percent_change({"TEST": CHANGE_MULTIPLE * INITIAL_CASH}) == -0.5
     )
     assert portfolio.total_percent_change({"TEST": 0.0}) == -1
 
 
 def test_position_buy(position: Position) -> None:
     assert position.average_cost_basis == INITIAL_COST
-    assert position.cost_basis_total == (INITIAL_COST * INITIAL_QUANTITY)
+    assert position.total_cost_basis == (INITIAL_COST * INITIAL_QUANTITY)
     position.buy(CHANGE_MULTIPLE * INITIAL_COST, INITIAL_QUANTITY)
     assert position.average_cost_basis == (
         INITIAL_COST - INITIAL_COST * (CHANGE_MULTIPLE / 2)
     )
-    assert position.cost_basis_total == (
+    assert position.total_cost_basis == (
         (1 + CHANGE_MULTIPLE) * INITIAL_COST * INITIAL_QUANTITY
     )
 
 
 def test_position_sell(position: Position) -> None:
     assert position.average_cost_basis == INITIAL_COST
-    assert position.cost_basis_total == (INITIAL_COST * INITIAL_QUANTITY)
+    assert position.total_cost_basis == (INITIAL_COST * INITIAL_QUANTITY)
     position.sell(
         CHANGE_MULTIPLE * INITIAL_COST,
         CHANGE_MULTIPLE * INITIAL_QUANTITY,
     )
     assert position.average_cost_basis == INITIAL_COST
-    assert position.cost_basis_total == (
+    assert position.total_cost_basis == (
         (1 - CHANGE_MULTIPLE) * INITIAL_COST * INITIAL_QUANTITY
     )
 
 
 def test_position_total_dollar_change(position: Position) -> None:
     assert position.average_cost_basis == INITIAL_COST
-    assert position.cost_basis_total == (INITIAL_COST * INITIAL_QUANTITY)
+    assert position.total_cost_basis == (INITIAL_COST * INITIAL_QUANTITY)
     assert (
         position.total_dollar_change(CHANGE_MULTIPLE * INITIAL_COST)
         == -CHANGE_MULTIPLE * position.average_cost_basis * position.quantity
     )
 
 
 def test_position_total_percent_change(position: Position) -> None:
     assert position.average_cost_basis == INITIAL_COST
-    assert position.cost_basis_total == (INITIAL_COST * INITIAL_QUANTITY)
+    assert position.total_cost_basis == (INITIAL_COST * INITIAL_QUANTITY)
     assert (
         position.total_percent_change(CHANGE_MULTIPLE * INITIAL_COST)
         == -CHANGE_MULTIPLE
     )
```

### Comparing `finagg-0.3.1/tests/test_ratelimit.py` & `finagg-1.0.0/tests/test_ratelimit.py`

 * *Files identical despite different names*

### Comparing `finagg-0.3.1/tests/test_sec/test_feat.py` & `finagg-1.0.0/tests/test_sec/test_feat.py`

 * *Files identical despite different names*

### Comparing `finagg-0.3.1/tests/test_sec/test_sql.py` & `finagg-1.0.0/tests/test_sec/test_sql.py`

 * *Files identical despite different names*

### Comparing `finagg-0.3.1/tests/test_utils.py` & `finagg-1.0.0/tests/test_utils.py`

 * *Files identical despite different names*

