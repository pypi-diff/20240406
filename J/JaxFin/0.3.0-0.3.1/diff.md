# Comparing `tmp/JaxFin-0.3.0.tar.gz` & `tmp/JaxFin-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "JaxFin-0.3.0.tar", last modified: Wed Apr  3 16:01:42 2024, max compression
+gzip compressed data, was "JaxFin-0.3.1.tar", last modified: Sat Apr  6 09:48:20 2024, max compression
```

## Comparing `JaxFin-0.3.0.tar` & `JaxFin-0.3.1.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxrwxrwx   0        0        0        0 2024-04-03 16:01:42.317427 JaxFin-0.3.0/
-drwxrwxrwx   0        0        0        0 2024-04-03 16:01:42.046569 JaxFin-0.3.0/.github/
-drwxrwxrwx   0        0        0        0 2024-04-03 16:01:42.106186 JaxFin-0.3.0/.github/workflows/
--rw-rw-rw-   0        0        0      597 2024-03-17 17:34:48.000000 JaxFin-0.3.0/.github/workflows/linting.yml
--rw-rw-rw-   0        0        0      617 2024-02-20 14:16:18.000000 JaxFin-0.3.0/.github/workflows/pytest.yml
--rw-rw-rw-   0        0        0      822 2024-03-05 14:09:37.000000 JaxFin-0.3.0/.github/workflows/quality_check.yml
--rw-rw-rw-   0        0        0      497 2024-03-17 17:29:55.000000 JaxFin-0.3.0/.gitignore
-drwxrwxrwx   0        0        0        0 2024-04-03 16:01:42.126677 JaxFin-0.3.0/.idea/
--rw-rw-rw-   0        0        0      184 2023-11-27 18:39:40.000000 JaxFin-0.3.0/.idea/.gitignore
--rw-rw-rw-   0        0        0      435 2024-03-05 13:42:17.000000 JaxFin-0.3.0/.idea/aws.xml
-drwxrwxrwx   0        0        0        0 2024-04-03 16:01:42.129477 JaxFin-0.3.0/.idea/inspectionProfiles/
--rw-rw-rw-   0        0        0      179 2023-11-27 18:39:40.000000 JaxFin-0.3.0/.idea/inspectionProfiles/profiles_settings.xml
--rw-rw-rw-   0        0        0      434 2024-02-20 14:21:44.000000 JaxFin-0.3.0/.idea/misc.xml
--rw-rw-rw-   0        0        0      283 2023-11-27 18:39:40.000000 JaxFin-0.3.0/.idea/modules.xml
--rw-rw-rw-   0        0        0      191 2023-12-15 20:40:10.000000 JaxFin-0.3.0/.idea/other.xml
--rw-rw-rw-   0        0        0      409 2024-02-20 14:21:44.000000 JaxFin-0.3.0/.idea/py-exopricer.iml
--rw-rw-rw-   0        0        0      172 2023-11-27 18:39:40.000000 JaxFin-0.3.0/.idea/vcs.xml
--rw-rw-rw-   0        0        0     2418 2024-02-16 14:21:51.000000 JaxFin-0.3.0/CONTRIBUTING.md
-drwxrwxrwx   0        0        0        0 2024-04-03 16:01:42.311379 JaxFin-0.3.0/JaxFin.egg-info/
--rw-rw-rw-   0        0        0     7516 2024-04-03 16:01:41.000000 JaxFin-0.3.0/JaxFin.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1608 2024-04-03 16:01:42.000000 JaxFin-0.3.0/JaxFin.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-03 16:01:41.000000 JaxFin-0.3.0/JaxFin.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2024-04-03 16:01:41.000000 JaxFin-0.3.0/JaxFin.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-03 16:01:41.000000 JaxFin-0.3.0/JaxFin.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1098 2024-02-10 17:05:30.000000 JaxFin-0.3.0/LICENSE
--rw-rw-rw-   0        0        0      637 2024-04-03 15:58:34.000000 JaxFin-0.3.0/Makefile
--rw-rw-rw-   0        0        0     7516 2024-04-03 16:01:42.313856 JaxFin-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     6632 2024-04-03 15:58:34.000000 JaxFin-0.3.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-03 16:01:42.187832 JaxFin-0.3.0/jaxfin/
--rw-rw-rw-   0        0        0        0 2024-02-17 09:50:48.000000 JaxFin-0.3.0/jaxfin/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-03 16:01:42.194131 JaxFin-0.3.0/jaxfin/models/
--rw-rw-rw-   0        0        0      211 2024-02-17 10:10:13.000000 JaxFin-0.3.0/jaxfin/models/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-03 16:01:42.199669 JaxFin-0.3.0/jaxfin/models/gbm/
--rw-rw-rw-   0        0        0      230 2024-02-20 14:21:44.000000 JaxFin-0.3.0/jaxfin/models/gbm/__init__.py
--rw-rw-rw-   0        0        0     7604 2024-03-07 14:43:03.000000 JaxFin-0.3.0/jaxfin/models/gbm/gbm.py
-drwxrwxrwx   0        0        0        0 2024-04-03 16:01:42.207091 JaxFin-0.3.0/jaxfin/models/heston/
--rw-rw-rw-   0        0        0      159 2024-03-07 14:43:03.000000 JaxFin-0.3.0/jaxfin/models/heston/__init__.py
--rw-rw-rw-   0        0        0    12759 2024-03-07 14:43:03.000000 JaxFin-0.3.0/jaxfin/models/heston/heston.py
--rw-rw-rw-   0        0        0      381 2024-03-07 14:43:03.000000 JaxFin-0.3.0/jaxfin/models/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-03 16:01:42.209728 JaxFin-0.3.0/jaxfin/price_engine/
--rw-rw-rw-   0        0        0        0 2024-02-17 09:50:48.000000 JaxFin-0.3.0/jaxfin/price_engine/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-03 16:01:42.215098 JaxFin-0.3.0/jaxfin/price_engine/black/
--rw-rw-rw-   0        0        0      249 2024-02-20 14:16:18.000000 JaxFin-0.3.0/jaxfin/price_engine/black/__init__.py
--rw-rw-rw-   0        0        0     4809 2024-03-05 14:09:37.000000 JaxFin-0.3.0/jaxfin/price_engine/black/black_model.py
-drwxrwxrwx   0        0        0        0 2024-04-03 16:01:42.221477 JaxFin-0.3.0/jaxfin/price_engine/black_scholes/
--rw-rw-rw-   0        0        0      423 2024-03-04 19:28:01.000000 JaxFin-0.3.0/jaxfin/price_engine/black_scholes/__init__.py
--rw-rw-rw-   0        0        0     8033 2024-03-05 14:09:37.000000 JaxFin-0.3.0/jaxfin/price_engine/black_scholes/vanilla_options.py
-drwxrwxrwx   0        0        0        0 2024-04-03 16:01:42.227259 JaxFin-0.3.0/jaxfin/price_engine/fft/
--rw-rw-rw-   0        0        0      290 2024-04-03 15:58:34.000000 JaxFin-0.3.0/jaxfin/price_engine/fft/__init__.py
--rw-rw-rw-   0        0        0     5916 2024-04-03 15:58:34.000000 JaxFin-0.3.0/jaxfin/price_engine/fft/vanilla_options.py
-drwxrwxrwx   0        0        0        0 2024-04-03 16:01:42.234534 JaxFin-0.3.0/jaxfin/price_engine/math/
--rw-rw-rw-   0        0        0        0 2024-03-05 14:09:37.000000 JaxFin-0.3.0/jaxfin/price_engine/math/__init__.py
--rw-rw-rw-   0        0        0     2609 2024-03-05 14:09:37.000000 JaxFin-0.3.0/jaxfin/price_engine/math/bs_common.py
--rw-rw-rw-   0        0        0      640 2024-03-05 14:09:37.000000 JaxFin-0.3.0/jaxfin/price_engine/math/norm.py
-drwxrwxrwx   0        0        0        0 2024-04-03 16:01:42.245290 JaxFin-0.3.0/jaxfin/price_engine/utils/
--rw-rw-rw-   0        0        0        0 2024-03-05 14:09:37.000000 JaxFin-0.3.0/jaxfin/price_engine/utils/__init__.py
--rw-rw-rw-   0        0        0      920 2024-03-05 14:09:37.000000 JaxFin-0.3.0/jaxfin/price_engine/utils/arrays.py
--rw-rw-rw-   0        0        0     2788 2024-03-05 14:09:37.000000 JaxFin-0.3.0/jaxfin/price_engine/utils/vect.py
--rw-rw-rw-   0        0        0      175 2024-02-10 14:03:34.000000 JaxFin-0.3.0/noxfile.py
--rw-rw-rw-   0        0        0    23014 2024-03-23 15:48:12.000000 JaxFin-0.3.0/pyproject.toml
-drwxrwxrwx   0        0        0        0 2024-04-03 16:01:42.251698 JaxFin-0.3.0/requirements/
--rw-rw-rw-   0        0        0      505 2024-03-17 17:32:57.000000 JaxFin-0.3.0/requirements/build.txt
--rw-rw-rw-   0        0        0     2528 2024-03-17 17:26:30.000000 JaxFin-0.3.0/requirements/dev.txt
-drwxrwxrwx   0        0        0        0 2024-04-03 16:01:42.284511 JaxFin-0.3.0/scripts/
--rwxrwxrwx   0        0        0       61 2023-12-19 18:23:50.000000 JaxFin-0.3.0/scripts/basedir.bat
--rwxrwxrwx   0        0        0       68 2024-02-10 16:19:46.000000 JaxFin-0.3.0/scripts/black-reformat.bat
--rwxrwxrwx   0        0        0       76 2024-02-10 16:19:46.000000 JaxFin-0.3.0/scripts/check-black.bat
--rwxrwxrwx   0        0        0      376 2024-02-17 11:13:18.000000 JaxFin-0.3.0/scripts/configure-python.bat
--rwxrwxrwx   0        0        0      720 2024-02-17 11:22:03.000000 JaxFin-0.3.0/scripts/create-new-version.bat
--rwxrwxrwx   0        0        0      102 2024-02-20 14:16:18.000000 JaxFin-0.3.0/scripts/get-tests-cov.bat
--rwxrwxrwx   0        0        0       96 2024-03-17 17:31:24.000000 JaxFin-0.3.0/scripts/run-linter.bat
--rwxrwxrwx   0        0        0       69 2024-02-10 17:00:41.000000 JaxFin-0.3.0/scripts/run-mypy.bat
--rwxrwxrwx   0        0        0      126 2024-02-10 16:58:40.000000 JaxFin-0.3.0/scripts/run-tests.bat
--rw-rw-rw-   0        0        0       42 2024-04-03 16:01:42.317427 JaxFin-0.3.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-03 16:01:42.291126 JaxFin-0.3.0/tests/
--rw-rw-rw-   0        0        0        0 2023-11-27 18:43:58.000000 JaxFin-0.3.0/tests/.gitkeep
-drwxrwxrwx   0        0        0        0 2024-04-03 16:01:42.295482 JaxFin-0.3.0/tests/models/
--rw-rw-rw-   0        0        0     1760 2024-04-03 15:58:34.000000 JaxFin-0.3.0/tests/models/test_gbm.py
--rw-rw-rw-   0        0        0     3177 2024-04-03 15:58:34.000000 JaxFin-0.3.0/tests/models/test_heston.py
-drwxrwxrwx   0        0        0        0 2024-04-03 16:01:42.307829 JaxFin-0.3.0/tests/price_engine/
--rw-rw-rw-   0        0        0     6518 2024-04-03 15:58:34.000000 JaxFin-0.3.0/tests/price_engine/test_black.py
--rw-rw-rw-   0        0        0    11089 2024-04-03 15:58:34.000000 JaxFin-0.3.0/tests/price_engine/test_bs.py
--rw-rw-rw-   0        0        0     3335 2024-04-03 15:58:34.000000 JaxFin-0.3.0/tests/price_engine/test_fft.py
+drwxrwxrwx   0        0        0        0 2024-04-06 09:48:20.829982 JaxFin-0.3.1/
+drwxrwxrwx   0        0        0        0 2024-04-06 09:48:20.562607 JaxFin-0.3.1/.github/
+drwxrwxrwx   0        0        0        0 2024-04-06 09:48:20.615667 JaxFin-0.3.1/.github/workflows/
+-rw-rw-rw-   0        0        0      597 2024-03-17 17:34:48.000000 JaxFin-0.3.1/.github/workflows/linting.yml
+-rw-rw-rw-   0        0        0      617 2024-02-20 14:16:18.000000 JaxFin-0.3.1/.github/workflows/pytest.yml
+-rw-rw-rw-   0        0        0      822 2024-03-05 14:09:37.000000 JaxFin-0.3.1/.github/workflows/quality_check.yml
+-rw-rw-rw-   0        0        0      497 2024-03-17 17:29:55.000000 JaxFin-0.3.1/.gitignore
+drwxrwxrwx   0        0        0        0 2024-04-06 09:48:20.635396 JaxFin-0.3.1/.idea/
+-rw-rw-rw-   0        0        0      184 2023-11-27 18:39:40.000000 JaxFin-0.3.1/.idea/.gitignore
+-rw-rw-rw-   0        0        0      435 2024-03-05 13:42:17.000000 JaxFin-0.3.1/.idea/aws.xml
+drwxrwxrwx   0        0        0        0 2024-04-06 09:48:20.639024 JaxFin-0.3.1/.idea/inspectionProfiles/
+-rw-rw-rw-   0        0        0      179 2023-11-27 18:39:40.000000 JaxFin-0.3.1/.idea/inspectionProfiles/profiles_settings.xml
+-rw-rw-rw-   0        0        0      434 2024-02-20 14:21:44.000000 JaxFin-0.3.1/.idea/misc.xml
+-rw-rw-rw-   0        0        0      283 2023-11-27 18:39:40.000000 JaxFin-0.3.1/.idea/modules.xml
+-rw-rw-rw-   0        0        0      191 2023-12-15 20:40:10.000000 JaxFin-0.3.1/.idea/other.xml
+-rw-rw-rw-   0        0        0      409 2024-02-20 14:21:44.000000 JaxFin-0.3.1/.idea/py-exopricer.iml
+-rw-rw-rw-   0        0        0      172 2023-11-27 18:39:40.000000 JaxFin-0.3.1/.idea/vcs.xml
+-rw-rw-rw-   0        0        0     2418 2024-02-16 14:21:51.000000 JaxFin-0.3.1/CONTRIBUTING.md
+drwxrwxrwx   0        0        0        0 2024-04-06 09:48:20.824372 JaxFin-0.3.1/JaxFin.egg-info/
+-rw-rw-rw-   0        0        0     7516 2024-04-06 09:48:20.000000 JaxFin-0.3.1/JaxFin.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1608 2024-04-06 09:48:20.000000 JaxFin-0.3.1/JaxFin.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-06 09:48:20.000000 JaxFin-0.3.1/JaxFin.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2024-04-06 09:48:20.000000 JaxFin-0.3.1/JaxFin.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-06 09:48:20.000000 JaxFin-0.3.1/JaxFin.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1098 2024-02-10 17:05:30.000000 JaxFin-0.3.1/LICENSE
+-rw-rw-rw-   0        0        0      637 2024-04-03 15:58:34.000000 JaxFin-0.3.1/Makefile
+-rw-rw-rw-   0        0        0     7516 2024-04-06 09:48:20.824889 JaxFin-0.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0     6632 2024-04-03 15:58:34.000000 JaxFin-0.3.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-06 09:48:20.688881 JaxFin-0.3.1/jaxfin/
+-rw-rw-rw-   0        0        0        0 2024-02-17 09:50:48.000000 JaxFin-0.3.1/jaxfin/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-06 09:48:20.697180 JaxFin-0.3.1/jaxfin/models/
+-rw-rw-rw-   0        0        0      211 2024-02-17 10:10:13.000000 JaxFin-0.3.1/jaxfin/models/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-06 09:48:20.704643 JaxFin-0.3.1/jaxfin/models/gbm/
+-rw-rw-rw-   0        0        0      230 2024-02-20 14:21:44.000000 JaxFin-0.3.1/jaxfin/models/gbm/__init__.py
+-rw-rw-rw-   0        0        0     7604 2024-03-07 14:43:03.000000 JaxFin-0.3.1/jaxfin/models/gbm/gbm.py
+drwxrwxrwx   0        0        0        0 2024-04-06 09:48:20.708969 JaxFin-0.3.1/jaxfin/models/heston/
+-rw-rw-rw-   0        0        0      159 2024-03-07 14:43:03.000000 JaxFin-0.3.1/jaxfin/models/heston/__init__.py
+-rw-rw-rw-   0        0        0    13095 2024-04-06 09:45:45.000000 JaxFin-0.3.1/jaxfin/models/heston/heston.py
+-rw-rw-rw-   0        0        0      381 2024-03-07 14:43:03.000000 JaxFin-0.3.1/jaxfin/models/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-06 09:48:20.714704 JaxFin-0.3.1/jaxfin/price_engine/
+-rw-rw-rw-   0        0        0        0 2024-02-17 09:50:48.000000 JaxFin-0.3.1/jaxfin/price_engine/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-06 09:48:20.721935 JaxFin-0.3.1/jaxfin/price_engine/black/
+-rw-rw-rw-   0        0        0      249 2024-02-20 14:16:18.000000 JaxFin-0.3.1/jaxfin/price_engine/black/__init__.py
+-rw-rw-rw-   0        0        0     4809 2024-03-05 14:09:37.000000 JaxFin-0.3.1/jaxfin/price_engine/black/black_model.py
+drwxrwxrwx   0        0        0        0 2024-04-06 09:48:20.727440 JaxFin-0.3.1/jaxfin/price_engine/black_scholes/
+-rw-rw-rw-   0        0        0      423 2024-03-04 19:28:01.000000 JaxFin-0.3.1/jaxfin/price_engine/black_scholes/__init__.py
+-rw-rw-rw-   0        0        0     8033 2024-03-05 14:09:37.000000 JaxFin-0.3.1/jaxfin/price_engine/black_scholes/vanilla_options.py
+drwxrwxrwx   0        0        0        0 2024-04-06 09:48:20.733550 JaxFin-0.3.1/jaxfin/price_engine/fft/
+-rw-rw-rw-   0        0        0      290 2024-04-03 15:58:34.000000 JaxFin-0.3.1/jaxfin/price_engine/fft/__init__.py
+-rw-rw-rw-   0        0        0     5916 2024-04-03 15:58:34.000000 JaxFin-0.3.1/jaxfin/price_engine/fft/vanilla_options.py
+drwxrwxrwx   0        0        0        0 2024-04-06 09:48:20.746681 JaxFin-0.3.1/jaxfin/price_engine/math/
+-rw-rw-rw-   0        0        0        0 2024-03-05 14:09:37.000000 JaxFin-0.3.1/jaxfin/price_engine/math/__init__.py
+-rw-rw-rw-   0        0        0     2609 2024-03-05 14:09:37.000000 JaxFin-0.3.1/jaxfin/price_engine/math/bs_common.py
+-rw-rw-rw-   0        0        0      640 2024-03-05 14:09:37.000000 JaxFin-0.3.1/jaxfin/price_engine/math/norm.py
+drwxrwxrwx   0        0        0        0 2024-04-06 09:48:20.750194 JaxFin-0.3.1/jaxfin/price_engine/utils/
+-rw-rw-rw-   0        0        0        0 2024-03-05 14:09:37.000000 JaxFin-0.3.1/jaxfin/price_engine/utils/__init__.py
+-rw-rw-rw-   0        0        0      920 2024-03-05 14:09:37.000000 JaxFin-0.3.1/jaxfin/price_engine/utils/arrays.py
+-rw-rw-rw-   0        0        0     2788 2024-03-05 14:09:37.000000 JaxFin-0.3.1/jaxfin/price_engine/utils/vect.py
+-rw-rw-rw-   0        0        0      175 2024-02-10 14:03:34.000000 JaxFin-0.3.1/noxfile.py
+-rw-rw-rw-   0        0        0    23014 2024-03-23 15:48:12.000000 JaxFin-0.3.1/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-04-06 09:48:20.763558 JaxFin-0.3.1/requirements/
+-rw-rw-rw-   0        0        0      505 2024-03-17 17:32:57.000000 JaxFin-0.3.1/requirements/build.txt
+-rw-rw-rw-   0        0        0     2528 2024-03-17 17:26:30.000000 JaxFin-0.3.1/requirements/dev.txt
+drwxrwxrwx   0        0        0        0 2024-04-06 09:48:20.798155 JaxFin-0.3.1/scripts/
+-rwxrwxrwx   0        0        0       61 2023-12-19 18:23:50.000000 JaxFin-0.3.1/scripts/basedir.bat
+-rwxrwxrwx   0        0        0       68 2024-02-10 16:19:46.000000 JaxFin-0.3.1/scripts/black-reformat.bat
+-rwxrwxrwx   0        0        0       76 2024-02-10 16:19:46.000000 JaxFin-0.3.1/scripts/check-black.bat
+-rwxrwxrwx   0        0        0      376 2024-02-17 11:13:18.000000 JaxFin-0.3.1/scripts/configure-python.bat
+-rwxrwxrwx   0        0        0      720 2024-02-17 11:22:03.000000 JaxFin-0.3.1/scripts/create-new-version.bat
+-rwxrwxrwx   0        0        0      102 2024-02-20 14:16:18.000000 JaxFin-0.3.1/scripts/get-tests-cov.bat
+-rwxrwxrwx   0        0        0       96 2024-03-17 17:31:24.000000 JaxFin-0.3.1/scripts/run-linter.bat
+-rwxrwxrwx   0        0        0       69 2024-02-10 17:00:41.000000 JaxFin-0.3.1/scripts/run-mypy.bat
+-rwxrwxrwx   0        0        0      126 2024-02-10 16:58:40.000000 JaxFin-0.3.1/scripts/run-tests.bat
+-rw-rw-rw-   0        0        0       42 2024-04-06 09:48:20.831192 JaxFin-0.3.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-06 09:48:20.800184 JaxFin-0.3.1/tests/
+-rw-rw-rw-   0        0        0        0 2023-11-27 18:43:58.000000 JaxFin-0.3.1/tests/.gitkeep
+drwxrwxrwx   0        0        0        0 2024-04-06 09:48:20.800184 JaxFin-0.3.1/tests/models/
+-rw-rw-rw-   0        0        0     1760 2024-04-03 15:58:34.000000 JaxFin-0.3.1/tests/models/test_gbm.py
+-rw-rw-rw-   0        0        0     3374 2024-04-06 09:45:45.000000 JaxFin-0.3.1/tests/models/test_heston.py
+drwxrwxrwx   0        0        0        0 2024-04-06 09:48:20.818668 JaxFin-0.3.1/tests/price_engine/
+-rw-rw-rw-   0        0        0     6518 2024-04-03 15:58:34.000000 JaxFin-0.3.1/tests/price_engine/test_black.py
+-rw-rw-rw-   0        0        0    11089 2024-04-03 15:58:34.000000 JaxFin-0.3.1/tests/price_engine/test_bs.py
+-rw-rw-rw-   0        0        0     3335 2024-04-03 15:58:34.000000 JaxFin-0.3.1/tests/price_engine/test_fft.py
```

### Comparing `JaxFin-0.3.0/.github/workflows/linting.yml` & `JaxFin-0.3.1/.github/workflows/linting.yml`

 * *Files identical despite different names*

### Comparing `JaxFin-0.3.0/.github/workflows/pytest.yml` & `JaxFin-0.3.1/.github/workflows/pytest.yml`

 * *Files identical despite different names*

### Comparing `JaxFin-0.3.0/.github/workflows/quality_check.yml` & `JaxFin-0.3.1/.github/workflows/quality_check.yml`

 * *Files identical despite different names*

### Comparing `JaxFin-0.3.0/CONTRIBUTING.md` & `JaxFin-0.3.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `JaxFin-0.3.0/JaxFin.egg-info/PKG-INFO` & `JaxFin-0.3.1/JaxFin.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JaxFin
-Version: 0.3.0
+Version: 0.3.1
 Summary: JaxFin is a powerful and versatile Python library designed for pricing exotic options using a range of advanced financial techniques.
 Author-email: Paolo D'Elia <paolo.delia99@gmail.com>, Samuele D'Elia <delia.samuele00@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `JaxFin-0.3.0/JaxFin.egg-info/SOURCES.txt` & `JaxFin-0.3.1/JaxFin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `JaxFin-0.3.0/LICENSE` & `JaxFin-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `JaxFin-0.3.0/Makefile` & `JaxFin-0.3.1/Makefile`

 * *Files identical despite different names*

### Comparing `JaxFin-0.3.0/PKG-INFO` & `JaxFin-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JaxFin
-Version: 0.3.0
+Version: 0.3.1
 Summary: JaxFin is a powerful and versatile Python library designed for pricing exotic options using a range of advanced financial techniques.
 Author-email: Paolo D'Elia <paolo.delia99@gmail.com>, Samuele D'Elia <delia.samuele00@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `JaxFin-0.3.0/README.md` & `JaxFin-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `JaxFin-0.3.0/jaxfin/models/gbm/gbm.py` & `JaxFin-0.3.1/jaxfin/models/gbm/gbm.py`

 * *Files identical despite different names*

### Comparing `JaxFin-0.3.0/jaxfin/models/heston/heston.py` & `JaxFin-0.3.1/jaxfin/models/heston/heston.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 Heston model class implementation
 """
-from typing import Optional, Union
+from typing import Optional, Tuple, Union
 
 import jax
 import jax.numpy as jnp
 from jax import jit, random
 
 from ..utils import check_symmetric
 
@@ -131,23 +131,28 @@
         """Returns the underlying dtype of the Heston model
 
         Returns:
             jax.numpy.dtype: The underlying dtype of the Heston model
         """
         return self._dtype
 
-    def sample_paths(self, seed: int, maturity: float, n: int, n_sim: int):
+    def sample_paths(
+        self, seed: int, maturity: float, n: int, n_sim: int
+    ) -> Tuple[jax.Array, jax.Array]:
         """
         Sample of paths from the Univariate Heston model
 
         Args:
             seed (int): the seed for the random number generator
             maturity (float): The time in years
             n (int): Number of steps (discretization points)
             n_sim (int): The number of simulations
+
+        Returns:
+            Tuple[jax.Array, jax.Array]: The simulated paths of the asset and the variance process
         """
         key = random.PRNGKey(seed)
 
         dt = maturity / n
 
         W = random.normal(key, shape=(n_sim, n)).T
         Z = (
@@ -284,25 +289,27 @@
         """Returns the underlying dtype of the Heston model
 
         Returns:
             jax.numpy.dtype: The underlying dtype of the Heston model
         """
         return self._dtype
 
-    def sample_paths(self, seed: int, maturity: float, n: int, n_sim: int) -> jax.Array:
+    def sample_paths(
+        self, seed: int, maturity: float, n: int, n_sim: int
+    ) -> Tuple[jax.Array, jax.Array]:
         """Sample paths from the Multivariate Heston model
 
         Args:
             seed (int): The seed for the random number generator
             maturity (float): The time in years
             n (int): The number of steps
             n_sim (int): The number of simulations
 
         Returns:
-            jax.Array: The simulated paths
+            Tuple[jax.Array, jax.Array]: The simulated paths and the variance processes of the assets
         """
         key = random.PRNGKey(seed)
 
         dt = maturity / n
 
         W = random.normal(key, shape=(n_sim, n * self._dim))
         Z = random.normal(key, shape=(n_sim, n * self._dim))
@@ -354,15 +361,15 @@
     kappa: jax.Array,
     theta: jax.Array,
     sigma: jax.Array,
     dt: jax.Array,
     W: jax.Array,
     Z: jax.Array,
     N: int,
-) -> jax.Array:
+) -> Tuple[jax.Array, jax.Array]:
     """Main function that simulate the path of the Heston model leveragin the
        jax.lax.while_loop function that allows to perform a loop in a jax makes
        it useful for reducing compilation times for jit-compiled functions,
        since native Python loop constructs in an @jit function are unrolled,
        leading to large XLA computations.
 
     Args:
@@ -374,15 +381,15 @@
         sigma (jax.Array): The volatility of the variance of the stock(s)
         dt (jax.Array): The time step
         W (jax.Array): The Weiner process of the stock(s)
         Z (jax.Array): The (correlated) Weiner process of the variance of the stock(s)
         N (int): The number of steps
 
     Returns:
-        jax.Array: The simulated paths of the stock(s)
+        Tuple[jax.Array, jax.Array]: The simulated paths of the stock(s), and the variance process(es)
     """
 
     def init_fn(W, Z):
         W_ = W
         Z_ = Z
 
         S = jnp.full_like(W_, s0)
@@ -404,10 +411,10 @@
             * jnp.exp((mean - 0.5 * v[i]) * dt + jnp.sqrt(v[i]) * jnp.sqrt(dt) * dW)
         )
 
         v = v.at[i + 1].set(_variance_process_step(v[i], kappa, theta, sigma, dt, dZ))
 
         return i + 1, S, v, W, Z
 
-    _, S, _, _, _ = jax.lax.while_loop(cond_fn, body_val, init_fn(W, Z))
+    _, S, v, _, _ = jax.lax.while_loop(cond_fn, body_val, init_fn(W, Z))
 
-    return S
+    return S, v
```

### Comparing `JaxFin-0.3.0/jaxfin/price_engine/black/black_model.py` & `JaxFin-0.3.1/jaxfin/price_engine/black/black_model.py`

 * *Files identical despite different names*

### Comparing `JaxFin-0.3.0/jaxfin/price_engine/black_scholes/vanilla_options.py` & `JaxFin-0.3.1/jaxfin/price_engine/black_scholes/vanilla_options.py`

 * *Files identical despite different names*

### Comparing `JaxFin-0.3.0/jaxfin/price_engine/fft/vanilla_options.py` & `JaxFin-0.3.1/jaxfin/price_engine/fft/vanilla_options.py`

 * *Files identical despite different names*

### Comparing `JaxFin-0.3.0/jaxfin/price_engine/math/bs_common.py` & `JaxFin-0.3.1/jaxfin/price_engine/math/bs_common.py`

 * *Files identical despite different names*

### Comparing `JaxFin-0.3.0/jaxfin/price_engine/math/norm.py` & `JaxFin-0.3.1/jaxfin/price_engine/math/norm.py`

 * *Files identical despite different names*

### Comparing `JaxFin-0.3.0/jaxfin/price_engine/utils/arrays.py` & `JaxFin-0.3.1/jaxfin/price_engine/utils/arrays.py`

 * *Files identical despite different names*

### Comparing `JaxFin-0.3.0/jaxfin/price_engine/utils/vect.py` & `JaxFin-0.3.1/jaxfin/price_engine/utils/vect.py`

 * *Files identical despite different names*

### Comparing `JaxFin-0.3.0/pyproject.toml` & `JaxFin-0.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `JaxFin-0.3.0/requirements/dev.txt` & `JaxFin-0.3.1/requirements/dev.txt`

 * *Files identical despite different names*

### Comparing `JaxFin-0.3.0/scripts/create-new-version.bat` & `JaxFin-0.3.1/scripts/create-new-version.bat`

 * *Files identical despite different names*

### Comparing `JaxFin-0.3.0/tests/models/test_gbm.py` & `JaxFin-0.3.1/tests/models/test_gbm.py`

 * *Files identical despite different names*

### Comparing `JaxFin-0.3.0/tests/models/test_heston.py` & `JaxFin-0.3.1/tests/models/test_heston.py`

 * *Files 12% similar despite different names*

```diff
@@ -37,17 +37,20 @@
         theta = jnp.array(0.25, dtype=jnp.float32)
         sigma = jnp.array(0.3, dtype=jnp.float32)
         rho = jnp.array(-0.7, dtype=jnp.float32)
 
         heston_model = UnivHestonModel(
             s0, v0, mean, kappa, theta, sigma, rho, dtype=jnp.float32
         )
-        paths = heston_model.sample_paths(seed=SEED, maturity=1.0, n=100, n_sim=100)
+        paths, variance_process = heston_model.sample_paths(
+            seed=SEED, maturity=1.0, n=100, n_sim=100
+        )
 
         assert paths.shape == (100, 100)
+        assert variance_process.shape == (100, 100)
 
 
 class TestMultiHestonModel:
     def test_init(self):
         s0 = jnp.array([100, 100], dtype=jnp.float32)
         v0 = jnp.array([0.2, 0.2], dtype=jnp.float32)
         mean = jnp.array([0.2, 0.2], dtype=jnp.float32)
@@ -78,10 +81,13 @@
         theta = jnp.array([0.25, 0.25], dtype=jnp.float32)
         sigma = jnp.array([0.3, 0.3], dtype=jnp.float32)
         corr = jnp.array([[1.0, 0.5], [0.5, 1.0]], dtype=jnp.float32)
 
         heston_model = MultiHestonModel(
             s0, v0, mean, kappa, theta, sigma, corr, dtype=jnp.float32
         )
-        paths = heston_model.sample_paths(seed=SEED, maturity=1.0, n=100, n_sim=100)
+        paths, variance_processes = heston_model.sample_paths(
+            seed=SEED, maturity=1.0, n=100, n_sim=100
+        )
 
         assert paths.shape == (100, 100, 2)
+        assert variance_processes.shape == (100, 100, 2)
```

### Comparing `JaxFin-0.3.0/tests/price_engine/test_black.py` & `JaxFin-0.3.1/tests/price_engine/test_black.py`

 * *Files identical despite different names*

### Comparing `JaxFin-0.3.0/tests/price_engine/test_bs.py` & `JaxFin-0.3.1/tests/price_engine/test_bs.py`

 * *Files identical despite different names*

### Comparing `JaxFin-0.3.0/tests/price_engine/test_fft.py` & `JaxFin-0.3.1/tests/price_engine/test_fft.py`

 * *Files identical despite different names*

