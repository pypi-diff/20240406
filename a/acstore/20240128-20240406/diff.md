# Comparing `tmp/acstore-20240128.tar.gz` & `tmp/acstore-20240406.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acstore-20240128.tar", last modified: Tue Jan 30 05:40:58 2024, max compression
+gzip compressed data, was "acstore-20240406.tar", last modified: Sat Apr  6 04:12:34 2024, max compression
```

## Comparing `acstore-20240128.tar` & `acstore-20240406.tar`

### file list

```diff
@@ -1,98 +1,98 @@
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-30 05:40:58.957429 acstore-20240128/
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-30 05:40:58.942429 acstore-20240128/.github/
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-30 05:40:58.948429 acstore-20240128/.github/workflows/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2629 2024-01-28 17:50:00.000000 acstore-20240128/.github/workflows/test_docker.yml
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1355 2024-01-28 19:47:48.000000 acstore-20240128/.github/workflows/test_docs.yml
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4126 2024-01-28 19:47:58.000000 acstore-20240128/.github/workflows/test_tox.yml
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23143 2024-01-28 20:28:03.000000 acstore-20240128/.pylintrc
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      322 2024-01-28 16:37:59.000000 acstore-20240128/.readthedocs.yaml
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      149 2023-12-03 09:37:37.000000 acstore-20240128/.yamllint.yaml
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      575 2023-12-03 09:37:37.000000 acstore-20240128/ACKNOWLEDGEMENTS
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      368 2023-12-03 09:37:37.000000 acstore-20240128/AUTHORS
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11358 2023-12-03 09:37:37.000000 acstore-20240128/LICENSE
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      494 2023-12-03 09:37:37.000000 acstore-20240128/MANIFEST.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      663 2024-01-30 05:40:58.957429 acstore-20240128/PKG-INFO
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      249 2023-12-03 09:37:37.000000 acstore-20240128/README
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-30 05:40:58.948429 acstore-20240128/acstore/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      215 2024-01-28 20:28:35.000000 acstore-20240128/acstore/__init__.py
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-30 05:40:58.950429 acstore-20240128/acstore/containers/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       24 2023-12-03 09:38:01.000000 acstore-20240128/acstore/containers/__init__.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6615 2024-01-28 16:37:59.000000 acstore-20240128/acstore/containers/interface.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3816 2024-01-28 16:37:59.000000 acstore-20240128/acstore/containers/manager.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      175 2023-12-03 09:38:00.000000 acstore-20240128/acstore/errors.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6465 2024-01-28 16:37:59.000000 acstore-20240128/acstore/fake_store.py
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-30 05:40:58.950429 acstore-20240128/acstore/helpers/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       24 2023-12-03 09:38:00.000000 acstore-20240128/acstore/helpers/__init__.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3296 2024-01-28 16:37:59.000000 acstore-20240128/acstore/helpers/json_serializer.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2242 2023-12-03 09:38:00.000000 acstore-20240128/acstore/helpers/schema.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4598 2023-12-03 09:38:00.000000 acstore-20240128/acstore/helpers/yaml_definitions_file.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7840 2024-01-28 16:37:59.000000 acstore-20240128/acstore/interface.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3999 2023-12-03 09:38:00.000000 acstore-20240128/acstore/profilers.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35340 2024-01-28 20:20:48.000000 acstore-20240128/acstore/sqlite_store.py
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-30 05:40:58.949429 acstore-20240128/acstore.egg-info/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      663 2024-01-30 05:40:58.000000 acstore-20240128/acstore.egg-info/PKG-INFO
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1784 2024-01-30 05:40:58.000000 acstore-20240128/acstore.egg-info/SOURCES.txt
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        1 2024-01-30 05:40:58.000000 acstore-20240128/acstore.egg-info/dependency_links.txt
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       13 2024-01-30 05:40:58.000000 acstore-20240128/acstore.egg-info/requires.txt
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        8 2024-01-30 05:40:58.000000 acstore-20240128/acstore.egg-info/top_level.txt
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      411 2023-12-03 09:37:37.000000 acstore-20240128/acstore.ini
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1757 2024-01-28 16:37:59.000000 acstore-20240128/appveyor.yml
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-30 05:40:58.943429 acstore-20240128/config/
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-30 05:40:58.951429 acstore-20240128/config/appveyor/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      804 2024-01-28 20:28:03.000000 acstore-20240128/config/appveyor/install.ps1
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)      125 2024-01-28 16:37:59.000000 acstore-20240128/config/appveyor/install.sh
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)      620 2024-01-28 16:37:59.000000 acstore-20240128/config/appveyor/runtests.sh
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-30 05:40:58.951429 acstore-20240128/config/dpkg/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      170 2024-01-28 20:29:10.000000 acstore-20240128/config/dpkg/changelog
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       20 2023-12-03 09:37:37.000000 acstore-20240128/config/dpkg/clean
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        2 2024-01-28 13:31:08.000000 acstore-20240128/config/dpkg/compat
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      583 2024-01-28 20:28:03.000000 acstore-20240128/config/dpkg/control
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      962 2023-12-03 09:37:37.000000 acstore-20240128/config/dpkg/copyright
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)      122 2024-01-28 13:31:08.000000 acstore-20240128/config/dpkg/rules
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-30 05:40:58.952429 acstore-20240128/config/dpkg/source/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       12 2023-12-03 09:37:37.000000 acstore-20240128/config/dpkg/source/format
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      151 2024-01-28 20:28:03.000000 acstore-20240128/dependencies.ini
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-30 05:40:58.952429 acstore-20240128/docs/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5091 2024-01-28 16:37:59.000000 acstore-20240128/docs/conf.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      511 2023-12-03 09:38:02.000000 acstore-20240128/docs/index.rst
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      118 2024-01-28 16:37:59.000000 acstore-20240128/docs/requirements.txt
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-30 05:40:58.943429 acstore-20240128/docs/sources/
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-30 05:40:58.953429 acstore-20240128/docs/sources/api/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      540 2023-12-03 09:38:02.000000 acstore-20240128/docs/sources/api/acstore.containers.rst
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      734 2024-01-28 16:37:59.000000 acstore-20240128/docs/sources/api/acstore.helpers.rst
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      971 2023-12-03 09:38:02.000000 acstore-20240128/docs/sources/api/acstore.rst
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       58 2023-12-03 09:38:02.000000 acstore-20240128/docs/sources/api/modules.rst
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-30 05:40:58.953429 acstore-20240128/docs/sources/user/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1619 2023-12-03 09:38:02.000000 acstore-20240128/docs/sources/user/Installation-instructions.md
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      286 2023-12-03 09:38:02.000000 acstore-20240128/docs/sources/user/index.rst
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      261 2024-01-28 16:37:59.000000 acstore-20240128/pyproject.toml
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       15 2024-01-28 20:28:03.000000 acstore-20240128/requirements.txt
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)      929 2023-12-03 09:37:37.000000 acstore-20240128/run_tests.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1120 2024-01-30 05:40:58.957429 acstore-20240128/setup.cfg
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)      128 2024-01-28 13:31:08.000000 acstore-20240128/setup.py
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-30 05:40:58.953429 acstore-20240128/test_data/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      161 2023-12-03 09:37:37.000000 acstore-20240128/test_data/definitions.yaml
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        0 2023-12-03 09:37:37.000000 acstore-20240128/test_dependencies.ini
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-28 13:31:08.000000 acstore-20240128/test_requirements.txt
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-30 05:40:58.955429 acstore-20240128/tests/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       24 2023-12-03 09:37:37.000000 acstore-20240128/tests/__init__.py
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-30 05:40:58.955429 acstore-20240128/tests/containers/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       24 2023-12-03 09:37:37.000000 acstore-20240128/tests/containers/__init__.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5724 2024-01-28 16:37:59.000000 acstore-20240128/tests/containers/interface.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2838 2024-01-28 16:37:59.000000 acstore-20240128/tests/containers/manager.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8446 2023-12-03 09:37:37.000000 acstore-20240128/tests/fake_store.py
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-30 05:40:58.956429 acstore-20240128/tests/helpers/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       24 2023-12-03 09:37:38.000000 acstore-20240128/tests/helpers/__init__.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1874 2024-01-28 16:37:59.000000 acstore-20240128/tests/helpers/json_serializer.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1779 2023-12-03 09:37:38.000000 acstore-20240128/tests/helpers/schema.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3052 2023-12-03 09:37:38.000000 acstore-20240128/tests/helpers/yaml_definitions_file.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3332 2024-01-28 16:37:59.000000 acstore-20240128/tests/interface.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1649 2023-12-03 09:37:37.000000 acstore-20240128/tests/profilers.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20058 2024-01-28 16:37:59.000000 acstore-20240128/tests/sqlite_store.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2375 2024-01-21 17:37:54.000000 acstore-20240128/tests/test_lib.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1363 2024-01-28 16:38:14.000000 acstore-20240128/tox.ini
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-30 05:40:58.957429 acstore-20240128/utils/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       24 2023-12-03 09:38:01.000000 acstore-20240128/utils/__init__.py
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)      422 2024-01-28 13:31:08.000000 acstore-20240128/utils/check_dependencies.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11583 2024-01-28 13:31:08.000000 acstore-20240128/utils/dependencies.py
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)      773 2024-01-28 16:37:59.000000 acstore-20240128/utils/update_release.sh
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-06 04:12:34.366788 acstore-20240406/
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-06 04:12:34.354789 acstore-20240406/.github/
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-06 04:12:34.360789 acstore-20240406/.github/workflows/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2441 2024-04-06 04:12:17.000000 acstore-20240406/.github/workflows/test_docker.yml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1355 2024-04-06 03:53:55.000000 acstore-20240406/.github/workflows/test_docs.yml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4063 2024-04-06 03:54:09.000000 acstore-20240406/.github/workflows/test_tox.yml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23143 2024-04-06 03:53:46.000000 acstore-20240406/.pylintrc
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      322 2024-04-06 03:53:46.000000 acstore-20240406/.readthedocs.yaml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      149 2023-12-03 09:37:37.000000 acstore-20240406/.yamllint.yaml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      575 2023-12-03 09:37:37.000000 acstore-20240406/ACKNOWLEDGEMENTS
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      368 2023-12-03 09:37:37.000000 acstore-20240406/AUTHORS
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11358 2023-12-03 09:37:37.000000 acstore-20240406/LICENSE
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      494 2023-12-03 09:37:37.000000 acstore-20240406/MANIFEST.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      691 2024-04-06 04:12:34.366788 acstore-20240406/PKG-INFO
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      249 2023-12-03 09:37:37.000000 acstore-20240406/README
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-06 04:12:34.360789 acstore-20240406/acstore/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      215 2024-04-06 04:12:17.000000 acstore-20240406/acstore/__init__.py
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-06 04:12:34.361789 acstore-20240406/acstore/containers/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       24 2023-12-03 09:38:01.000000 acstore-20240406/acstore/containers/__init__.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6615 2024-03-30 05:07:58.000000 acstore-20240406/acstore/containers/interface.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3816 2024-03-30 05:07:58.000000 acstore-20240406/acstore/containers/manager.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      175 2023-12-03 09:38:00.000000 acstore-20240406/acstore/errors.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6465 2024-03-30 05:07:58.000000 acstore-20240406/acstore/fake_store.py
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-06 04:12:34.362789 acstore-20240406/acstore/helpers/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       24 2023-12-03 09:38:00.000000 acstore-20240406/acstore/helpers/__init__.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3656 2024-04-06 04:12:17.000000 acstore-20240406/acstore/helpers/json_serializer.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2242 2023-12-03 09:38:00.000000 acstore-20240406/acstore/helpers/schema.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4598 2023-12-03 09:38:00.000000 acstore-20240406/acstore/helpers/yaml_definitions_file.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7840 2024-03-30 05:07:58.000000 acstore-20240406/acstore/interface.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3999 2023-12-03 09:38:00.000000 acstore-20240406/acstore/profilers.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35352 2024-04-06 04:12:17.000000 acstore-20240406/acstore/sqlite_store.py
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-06 04:12:34.366788 acstore-20240406/acstore.egg-info/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      691 2024-04-06 04:12:34.000000 acstore-20240406/acstore.egg-info/PKG-INFO
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1784 2024-04-06 04:12:34.000000 acstore-20240406/acstore.egg-info/SOURCES.txt
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        1 2024-04-06 04:12:34.000000 acstore-20240406/acstore.egg-info/dependency_links.txt
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       13 2024-04-06 04:12:34.000000 acstore-20240406/acstore.egg-info/requires.txt
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        8 2024-04-06 04:12:34.000000 acstore-20240406/acstore.egg-info/top_level.txt
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      411 2023-12-03 09:37:37.000000 acstore-20240406/acstore.ini
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1757 2024-04-06 03:53:46.000000 acstore-20240406/appveyor.yml
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-06 04:12:34.355789 acstore-20240406/config/
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-06 04:12:34.362789 acstore-20240406/config/appveyor/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      804 2024-04-06 03:53:46.000000 acstore-20240406/config/appveyor/install.ps1
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)      125 2024-04-06 03:53:46.000000 acstore-20240406/config/appveyor/install.sh
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)      620 2024-04-06 03:53:46.000000 acstore-20240406/config/appveyor/runtests.sh
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-06 04:12:34.363788 acstore-20240406/config/dpkg/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      170 2024-04-06 04:12:17.000000 acstore-20240406/config/dpkg/changelog
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       20 2023-12-03 09:37:37.000000 acstore-20240406/config/dpkg/clean
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        2 2024-04-06 03:53:46.000000 acstore-20240406/config/dpkg/compat
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      583 2024-04-06 03:53:46.000000 acstore-20240406/config/dpkg/control
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      962 2023-12-03 09:37:37.000000 acstore-20240406/config/dpkg/copyright
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)      122 2024-04-06 03:53:46.000000 acstore-20240406/config/dpkg/rules
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-06 04:12:34.363788 acstore-20240406/config/dpkg/source/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       12 2023-12-03 09:37:37.000000 acstore-20240406/config/dpkg/source/format
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      151 2024-04-06 03:53:34.000000 acstore-20240406/dependencies.ini
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-06 04:12:34.364789 acstore-20240406/docs/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5091 2024-04-06 03:53:46.000000 acstore-20240406/docs/conf.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      511 2023-12-03 09:38:02.000000 acstore-20240406/docs/index.rst
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      118 2024-04-06 03:53:46.000000 acstore-20240406/docs/requirements.txt
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-06 04:12:34.356789 acstore-20240406/docs/sources/
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-06 04:12:34.364789 acstore-20240406/docs/sources/api/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      540 2023-12-03 09:38:02.000000 acstore-20240406/docs/sources/api/acstore.containers.rst
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      734 2024-03-30 05:07:58.000000 acstore-20240406/docs/sources/api/acstore.helpers.rst
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      971 2024-04-06 03:54:38.000000 acstore-20240406/docs/sources/api/acstore.rst
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       58 2023-12-03 09:38:02.000000 acstore-20240406/docs/sources/api/modules.rst
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-06 04:12:34.364789 acstore-20240406/docs/sources/user/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-03-30 05:08:02.000000 acstore-20240406/docs/sources/user/Installation-instructions.md
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      286 2023-12-03 09:38:02.000000 acstore-20240406/docs/sources/user/index.rst
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      296 2024-04-06 03:53:46.000000 acstore-20240406/pyproject.toml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       15 2024-04-06 03:53:46.000000 acstore-20240406/requirements.txt
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)      929 2023-12-03 09:37:37.000000 acstore-20240406/run_tests.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      886 2024-04-06 04:12:34.367788 acstore-20240406/setup.cfg
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)      128 2024-04-06 03:53:46.000000 acstore-20240406/setup.py
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-06 04:12:34.364789 acstore-20240406/test_data/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      161 2023-12-03 09:37:37.000000 acstore-20240406/test_data/definitions.yaml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        0 2023-12-03 09:37:37.000000 acstore-20240406/test_dependencies.ini
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-06 03:53:46.000000 acstore-20240406/test_requirements.txt
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-06 04:12:34.365789 acstore-20240406/tests/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       24 2023-12-03 09:37:37.000000 acstore-20240406/tests/__init__.py
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-06 04:12:34.365789 acstore-20240406/tests/containers/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       24 2023-12-03 09:37:37.000000 acstore-20240406/tests/containers/__init__.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5724 2024-03-30 05:07:58.000000 acstore-20240406/tests/containers/interface.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2838 2024-03-30 05:07:58.000000 acstore-20240406/tests/containers/manager.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8446 2023-12-03 09:37:37.000000 acstore-20240406/tests/fake_store.py
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-06 04:12:34.365789 acstore-20240406/tests/helpers/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       24 2023-12-03 09:37:38.000000 acstore-20240406/tests/helpers/__init__.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1874 2024-03-30 05:07:58.000000 acstore-20240406/tests/helpers/json_serializer.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1779 2023-12-03 09:37:38.000000 acstore-20240406/tests/helpers/schema.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3052 2023-12-03 09:37:38.000000 acstore-20240406/tests/helpers/yaml_definitions_file.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3332 2024-03-30 05:07:58.000000 acstore-20240406/tests/interface.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1649 2023-12-03 09:37:37.000000 acstore-20240406/tests/profilers.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20058 2024-03-30 05:07:58.000000 acstore-20240406/tests/sqlite_store.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2375 2024-01-21 17:37:54.000000 acstore-20240406/tests/test_lib.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1359 2024-04-06 03:53:46.000000 acstore-20240406/tox.ini
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-06 04:12:34.366788 acstore-20240406/utils/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       24 2023-12-03 09:38:01.000000 acstore-20240406/utils/__init__.py
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)      422 2024-04-06 03:53:46.000000 acstore-20240406/utils/check_dependencies.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11583 2024-04-06 03:53:46.000000 acstore-20240406/utils/dependencies.py
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)      773 2024-03-30 05:07:58.000000 acstore-20240406/utils/update_release.sh
```

### Comparing `acstore-20240128/.github/workflows/test_docker.yml` & `acstore-20240406/.github/workflows/test_docker.yml`

 * *Files 14% similar despite different names*

```diff
@@ -3,49 +3,45 @@
 on: [push]
 permissions: read-all
 jobs:
   test_fedora:
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        version: ['38']
+        version: ['39', '40']
     container:
       image: registry.fedoraproject.org/fedora:${{ matrix.version }}
     steps:
     - uses: actions/checkout@v3
     - name: Set up container
       run: |
         dnf install -y dnf-plugins-core langpacks-en
     - name: Install dependencies
       run: |
         dnf copr -y enable @gift/dev
-        dnf install -y @development-tools python3 python3-devel python3-pyyaml python3-setuptools
+        dnf install -y @development-tools python3 python3-build python3-devel python3-pyyaml python3-setuptools python3-wheel
     - name: Run tests
       env:
         LANG: C.utf8
       run: |
         python3 ./run_tests.py
     - name: Run end-to-end tests
       run: |
         if test -f tests/end-to-end.py; then PYTHONPATH=. python3 ./tests/end-to-end.py --debug -c config/end-to-end.ini; fi
-    - name: Build source distribution
+    - name: Build source distribution (sdist)
       run: |
-        python3 ./setup.py sdist
-    - name: Build binary distribution
+        python3 -m build --no-isolation --sdist
+    - name: Build binary distribution (wheel)
       run: |
-        python3 ./setup.py bdist
-    - name: Run build and install test
-      run: |
-        python3 ./setup.py build
-        python3 ./setup.py install
+        python3 -m build --no-isolation --wheel
   test_ubuntu:
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        version: ['22.04']
+        version: ['24.04']
     container:
       image: ubuntu:${{ matrix.version }}
     steps:
     - uses: actions/checkout@v3
     - name: Set up container
       env:
         DEBIAN_FRONTEND: noninteractive
@@ -54,31 +50,24 @@
         apt-get install -y libterm-readline-gnu-perl locales software-properties-common
         locale-gen en_US.UTF-8
         ln -f -s /usr/share/zoneinfo/UTC /etc/localtime
     - name: Install dependencies
       run: |
         add-apt-repository -y ppa:gift/dev
         apt-get update -q
-        apt-get install -y build-essential python3 python3-dev python3-distutils python3-pip python3-setuptools python3-wheel python3-yaml
+        apt-get install -y build-essential python3 python3-build python3-dev python3-distutils python3-pip python3-setuptools python3-wheel python3-yaml
     - name: Run tests
       env:
         LANG: en_US.UTF-8
       run: |
         python3 ./run_tests.py
     - name: Run end-to-end tests
       env:
         LANG: en_US.UTF-8
       run: |
         if test -f tests/end-to-end.py; then PYTHONPATH=. python3 ./tests/end-to-end.py --debug -c config/end-to-end.ini; fi
-    - name: Update setuptools
-      run: |
-        python3 -m pip install -U setuptools
-    - name: Build source distribution
-      run: |
-        python3 ./setup.py sdist
-    - name: Build binary distribution
+    - name: Build source distribution (sdist)
       run: |
-        python3 ./setup.py bdist
-    - name: Run build and install test
+        python3 -m build --no-isolation --sdist
+    - name: Build binary distribution (wheel)
       run: |
-        python3 ./setup.py build
-        python3 ./setup.py install
+        python3 -m build --no-isolation --wheel
```

### Comparing `acstore-20240128/.github/workflows/test_docs.yml` & `acstore-20240406/.github/workflows/test_docs.yml`

 * *Files identical despite different names*

### Comparing `acstore-20240128/.github/workflows/test_tox.yml` & `acstore-20240406/.github/workflows/test_tox.yml`

 * *Files 4% similar despite different names*

```diff
@@ -10,16 +10,14 @@
 permissions: read-all
 jobs:
   build:
     runs-on: ubuntu-latest
     strategy:
       matrix:
         include:
-        - python-version: '3.7'
-          toxenv: 'py37,wheel'
         - python-version: '3.8'
           toxenv: 'py38,wheel'
         - python-version: '3.9'
           toxenv: 'py39,wheel'
         - python-version: '3.10'
           toxenv: 'py310,wheel'
         - python-version: '3.11'
```

### Comparing `acstore-20240128/.pylintrc` & `acstore-20240406/.pylintrc`

 * *Files identical despite different names*

### Comparing `acstore-20240128/ACKNOWLEDGEMENTS` & `acstore-20240406/ACKNOWLEDGEMENTS`

 * *Files identical despite different names*

### Comparing `acstore-20240128/LICENSE` & `acstore-20240406/LICENSE`

 * *Files identical despite different names*

### Comparing `acstore-20240128/PKG-INFO` & `acstore-20240406/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: acstore
-Version: 20240128
+Version: 20240406
 Summary: Attribute Container Storage (ACStore).
 Home-page: https://github.com/log2timeline/acstore
 Maintainer: Log2Timeline maintainers
 Maintainer-email: log2timeline-maintainers@googlegroups.com
 License: Apache License, Version 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/plain
 License-File: ACKNOWLEDGEMENTS
 License-File: AUTHORS
 License-File: LICENSE
 License-File: README
+Requires-Dist: PyYAML>=3.10
 
 ACStore, or Attribute Container Storage, provides a stand-alone implementation to read and write attribute container storage files.
```

### Comparing `acstore-20240128/acstore/containers/interface.py` & `acstore-20240406/acstore/containers/interface.py`

 * *Files identical despite different names*

### Comparing `acstore-20240128/acstore/containers/manager.py` & `acstore-20240406/acstore/containers/manager.py`

 * *Files identical despite different names*

### Comparing `acstore-20240128/acstore/fake_store.py` & `acstore-20240406/acstore/fake_store.py`

 * *Files identical despite different names*

### Comparing `acstore-20240128/acstore/helpers/json_serializer.py` & `acstore-20240406/acstore/helpers/json_serializer.py`

 * *Files 4% similar despite different names*

```diff
@@ -85,19 +85,31 @@
     """
     # Use __container_type__ to indicate the attribute container type.
     container_type = json_dict.get('__container_type__', None)
 
     attribute_container = cls._CONTAINERS_MANAGER.CreateAttributeContainer(
         container_type)
 
+    try:
+      schema = cls._CONTAINERS_MANAGER.GetSchema(container_type)
+    except ValueError:
+      schema = {}
+
     supported_attribute_names = attribute_container.GetAttributeNames()
     for attribute_name, attribute_value in json_dict.items():
       if attribute_name in ('__container_type__', '__type__'):
         continue
 
       # Be strict about which attributes to set.
       if attribute_name not in supported_attribute_names:
         continue
 
+      data_type = schema.get(attribute_name, None)
+      serializer = schema_helper.SchemaHelper.GetAttributeSerializer(
+          data_type, 'json')
+
+      if serializer:
+        attribute_value = serializer.DeserializeValue(attribute_value)
+
       setattr(attribute_container, attribute_name, attribute_value)
 
     return attribute_container
```

### Comparing `acstore-20240128/acstore/helpers/schema.py` & `acstore-20240406/acstore/helpers/schema.py`

 * *Files identical despite different names*

### Comparing `acstore-20240128/acstore/helpers/yaml_definitions_file.py` & `acstore-20240406/acstore/helpers/yaml_definitions_file.py`

 * *Files identical despite different names*

### Comparing `acstore-20240128/acstore/interface.py` & `acstore-20240406/acstore/interface.py`

 * *Files identical despite different names*

### Comparing `acstore-20240128/acstore/profilers.py` & `acstore-20240406/acstore/profilers.py`

 * *Files identical despite different names*

### Comparing `acstore-20240128/acstore/sqlite_store.py` & `acstore-20240406/acstore/sqlite_store.py`

 * *Files 1% similar despite different names*

```diff
@@ -662,39 +662,39 @@
 
     schema = self._GetAttributeContainerSchema(container.CONTAINER_TYPE)
     if not schema:
       raise IOError(
           f'Unsupported attribute container type: {container.CONTAINER_TYPE:s}')
 
     column_names = []
-    values = []
+    row_values = []
     for name, data_type in sorted(schema.items()):
       attribute_value = getattr(container, name, None)
       try:
         row_value = self._schema_helper.SerializeValue(
             data_type, attribute_value)
       except IOError:
         raise IOError((
             f'Unsupported attribute container type: '
             f'{container.CONTAINER_TYPE:s} attribute: {name:s} data type: '
             f'{data_type:s}'))
 
       column_names.append(f'{name:s} = ?')
-      values.append(row_value)
+      row_values.append(row_value)
 
     column_names_string = ', '.join(column_names)
 
     query = (f'UPDATE {container.CONTAINER_TYPE:s} SET {column_names_string:s} '
              f'WHERE _identifier = {identifier.sequence_number:d}')
 
     if self._storage_profiler:
       self._storage_profiler.StartTiming('write_existing')
 
     try:
-      self._cursor.execute(query, values)
+      self._cursor.execute(query, row_values)
 
     except (sqlite3.InterfaceError, sqlite3.OperationalError) as exception:
       raise IOError((
           f'Unable to query attribute container store with error: '
           f'{exception!s}'))
 
     finally:
```

### Comparing `acstore-20240128/acstore.egg-info/PKG-INFO` & `acstore-20240406/acstore.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: acstore
-Version: 20240128
+Version: 20240406
 Summary: Attribute Container Storage (ACStore).
 Home-page: https://github.com/log2timeline/acstore
 Maintainer: Log2Timeline maintainers
 Maintainer-email: log2timeline-maintainers@googlegroups.com
 License: Apache License, Version 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/plain
 License-File: ACKNOWLEDGEMENTS
 License-File: AUTHORS
 License-File: LICENSE
 License-File: README
+Requires-Dist: PyYAML>=3.10
 
 ACStore, or Attribute Container Storage, provides a stand-alone implementation to read and write attribute container storage files.
```

### Comparing `acstore-20240128/acstore.egg-info/SOURCES.txt` & `acstore-20240406/acstore.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `acstore-20240128/appveyor.yml` & `acstore-20240406/appveyor.yml`

 * *Files identical despite different names*

### Comparing `acstore-20240128/config/appveyor/install.ps1` & `acstore-20240406/config/appveyor/install.ps1`

 * *Files identical despite different names*

### Comparing `acstore-20240128/config/appveyor/runtests.sh` & `acstore-20240406/config/appveyor/runtests.sh`

 * *Files identical despite different names*

### Comparing `acstore-20240128/config/dpkg/control` & `acstore-20240406/config/dpkg/control`

 * *Files identical despite different names*

### Comparing `acstore-20240128/config/dpkg/copyright` & `acstore-20240406/config/dpkg/copyright`

 * *Files identical despite different names*

### Comparing `acstore-20240128/docs/conf.py` & `acstore-20240406/docs/conf.py`

 * *Files identical despite different names*

### Comparing `acstore-20240128/docs/sources/api/acstore.containers.rst` & `acstore-20240406/docs/sources/api/acstore.containers.rst`

 * *Files identical despite different names*

### Comparing `acstore-20240128/docs/sources/api/acstore.helpers.rst` & `acstore-20240406/docs/sources/api/acstore.helpers.rst`

 * *Files identical despite different names*

### Comparing `acstore-20240128/docs/sources/api/acstore.rst` & `acstore-20240406/docs/sources/api/acstore.rst`

 * *Files identical despite different names*

### Comparing `acstore-20240128/docs/sources/user/Installation-instructions.md` & `acstore-20240406/docs/sources/user/Installation-instructions.md`

 * *Files 15% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 To deactivate the virtualenv run:
 
 ```bash
 deactivate
 ```
 
-## Ubuntu 18.04 and 20.04 LTS
+## Ubuntu 22.04 LTS
 
 To install ACStore from the [GIFT Personal Package Archive (PPA)](https://launchpad.net/~gift):
 
 ```bash
 sudo add-apt-repository ppa:gift/stable
 ```
 
@@ -45,22 +45,22 @@
 ## Windows
 
 The [l2tbinaries](https://github.com/log2timeline/l2tbinaries) contains the
 necessary packages for running ACStore. l2tbinaries provides the following
 branches:
 
 * main; branch intended for the "packaged release" of ACStore and dependencies;
+* staging; branch intended for testing pre-releases of ACStore;
 * dev; branch intended for the "development release" of ACStore;
 * testing; branch intended for testing newly created packages.
 
 The l2tdevtools project provides [an update script](https://github.com/log2timeline/l2tdevtools/wiki/Update-script)
 to ease the process of keeping the dependencies up to date.
 
-The script requires [pywin32](https://github.com/mhammond/pywin32/releases) and
-[Python WMI](https://pypi.org/project/WMI).
+The script requires [pywin32](https://github.com/mhammond/pywin32/releases).
 
 To install the release versions of the dependencies run:
 
 ```
 set PYTHONPATH=.
 
 C:\Python3\python.exe tools\update.py --preset acstore
```

### Comparing `acstore-20240128/run_tests.py` & `acstore-20240406/run_tests.py`

 * *Files identical despite different names*

### Comparing `acstore-20240128/setup.cfg` & `acstore-20240406/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = acstore
-version = 20240128
+version = 20240406
 description = Attribute Container Storage (ACStore).
 long_description = ACStore, or Attribute Container Storage, provides a stand-alone implementation to read and write attribute container storage files.
 long_description_content_type = text/plain
 url = https://github.com/log2timeline/acstore
 maintainer = Log2Timeline maintainers
 maintainer_email = log2timeline-maintainers@googlegroups.com
 license = Apache License, Version 2.0
@@ -18,36 +18,24 @@
 	Programming Language :: Python
 
 [options]
 install_requires = file:requirements.txt
 package_dir = 
 	acstore = acstore
 packages = find:
-python_requires = >=3.7
+python_requires = >=3.8
 
 [options.packages.find]
 exclude = 
 	docs
 	tests
 	tests.*
 	utils
 where = .
 
-[bdist_rpm]
-release = 1
-packager = Log2Timeline maintainers <log2timeline-maintainers@googlegroups.com>
-doc_files = 
-	ACKNOWLEDGEMENTS
-	AUTHORS
-	LICENSE
-	README
-build_requires = python3-setuptools
-requires = 
-	python3-pyyaml >= 3.10
-
 [bdist_wheel]
 universal = 1
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `acstore-20240128/tests/containers/interface.py` & `acstore-20240406/tests/containers/interface.py`

 * *Files identical despite different names*

### Comparing `acstore-20240128/tests/containers/manager.py` & `acstore-20240406/tests/containers/manager.py`

 * *Files identical despite different names*

### Comparing `acstore-20240128/tests/fake_store.py` & `acstore-20240406/tests/fake_store.py`

 * *Files identical despite different names*

### Comparing `acstore-20240128/tests/helpers/json_serializer.py` & `acstore-20240406/tests/helpers/json_serializer.py`

 * *Files identical despite different names*

### Comparing `acstore-20240128/tests/helpers/schema.py` & `acstore-20240406/tests/helpers/schema.py`

 * *Files identical despite different names*

### Comparing `acstore-20240128/tests/helpers/yaml_definitions_file.py` & `acstore-20240406/tests/helpers/yaml_definitions_file.py`

 * *Files identical despite different names*

### Comparing `acstore-20240128/tests/interface.py` & `acstore-20240406/tests/interface.py`

 * *Files identical despite different names*

### Comparing `acstore-20240128/tests/profilers.py` & `acstore-20240406/tests/profilers.py`

 * *Files identical despite different names*

### Comparing `acstore-20240128/tests/sqlite_store.py` & `acstore-20240406/tests/sqlite_store.py`

 * *Files identical despite different names*

### Comparing `acstore-20240128/tests/test_lib.py` & `acstore-20240406/tests/test_lib.py`

 * *Files identical despite different names*

### Comparing `acstore-20240128/tox.ini` & `acstore-20240406/tox.ini`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [tox]
-envlist = py3{7,8,9,10,11,12},coverage,docformatter,docs,lint,wheel
+envlist = py3{8,9,10,11,12},coverage,docformatter,docs,lint,wheel
 
 [testenv]
 allowlist_externals = ./run_tests.py
 pip_pre = True
 passenv =
   CFLAGS
   CPPFLAGS
@@ -15,15 +15,15 @@
   -rtest_requirements.txt
   coverage: coverage
   wheel:
     build
     setuptools >= 65
     wheel
 commands =
-  py3{7,8,9,10,11,12}: ./run_tests.py
+  py3{8,9,10,11,12}: ./run_tests.py
   coverage: coverage erase
   coverage: coverage run --source=acstore --omit="*_test*,*__init__*,*test_lib*" run_tests.py
   coverage: coverage xml
   wheel: python -m build --no-isolation --wheel
 
 [testenv:docformatter]
 usedevelop = True
```

### Comparing `acstore-20240128/utils/dependencies.py` & `acstore-20240406/utils/dependencies.py`

 * *Files identical despite different names*

### Comparing `acstore-20240128/utils/update_release.sh` & `acstore-20240406/utils/update_release.sh`

 * *Files identical despite different names*

