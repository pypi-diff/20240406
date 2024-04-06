# Comparing `tmp/blocklint-0.2.4.tar.gz` & `tmp/blocklint-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blocklint-0.2.4.tar", last modified: Mon Feb 13 18:39:49 2023, max compression
+gzip compressed data, was "blocklint-0.2.5.tar", last modified: Sat Apr  6 09:46:15 2024, max compression
```

## Comparing `blocklint-0.2.4.tar` & `blocklint-0.2.5.tar`

### file list

```diff
@@ -1,74 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 18:39:49.975567 blocklint-0.2.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 18:39:49.967567 blocklint-0.2.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 18:39:49.971567 blocklint-0.2.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-02-13 18:39:33.000000 blocklint-0.2.4/.github/workflows/cd.yml
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-02-13 18:39:33.000000 blocklint-0.2.4/.github/workflows/pre-commit.yml
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-02-13 18:39:33.000000 blocklint-0.2.4/.github/workflows/tox.yml
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-02-13 18:39:33.000000 blocklint-0.2.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-02-13 18:39:33.000000 blocklint-0.2.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-02-13 18:39:33.000000 blocklint-0.2.4/.pre-commit-hooks.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-02-13 18:39:33.000000 blocklint-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-02-13 18:39:33.000000 blocklint-0.2.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6701 2023-02-13 18:39:49.975567 blocklint-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5615 2023-02-13 18:39:33.000000 blocklint-0.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 18:39:49.971567 blocklint-0.2.4/blocklint/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-02-13 18:39:33.000000 blocklint-0.2.4/blocklint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-02-13 18:39:33.000000 blocklint-0.2.4/blocklint/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7610 2023-02-13 18:39:33.000000 blocklint-0.2.4/blocklint/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-02-13 18:39:49.000000 blocklint-0.2.4/blocklint/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 18:39:49.971567 blocklint-0.2.4/blocklint.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6701 2023-02-13 18:39:49.000000 blocklint-0.2.4/blocklint.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-02-13 18:39:49.000000 blocklint-0.2.4/blocklint.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-13 18:39:49.000000 blocklint-0.2.4/blocklint.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-02-13 18:39:49.000000 blocklint-0.2.4/blocklint.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-02-13 18:39:49.000000 blocklint-0.2.4/blocklint.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-02-13 18:39:49.000000 blocklint-0.2.4/blocklint.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 18:39:49.967567 blocklint-0.2.4/integration/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 18:39:49.971567 blocklint-0.2.4/integration/vim/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-02-13 18:39:33.000000 blocklint-0.2.4/integration/vim/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 18:39:49.975567 blocklint-0.2.4/integration/vim/autoload/
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-02-13 18:39:33.000000 blocklint-0.2.4/integration/vim/autoload/blocklint.vim
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 18:39:49.975567 blocklint-0.2.4/integration/vim/doc/
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-02-13 18:39:33.000000 blocklint-0.2.4/integration/vim/doc/blocklint.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 18:39:49.975567 blocklint-0.2.4/integration/vim/plugin/
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-02-13 18:39:33.000000 blocklint-0.2.4/integration/vim/plugin/blocklint.vim
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-02-13 18:39:33.000000 blocklint-0.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-02-13 18:39:49.979567 blocklint-0.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-02-13 18:39:33.000000 blocklint-0.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 18:39:49.975567 blocklint-0.2.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-02-13 18:39:33.000000 blocklint-0.2.4/tests/.blocklint
--rwxr-xr-x   0 runner    (1001) docker     (123)     1303 2023-02-13 18:39:33.000000 blocklint-0.2.4/tests/acceptance_test.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 18:39:49.971567 blocklint-0.2.4/tests/config_tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 18:39:49.975567 blocklint-0.2.4/tests/config_tests/flag_and_list/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-02-13 18:39:33.000000 blocklint-0.2.4/tests/config_tests/flag_and_list/tox.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 18:39:49.975567 blocklint-0.2.4/tests/config_tests/setup/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-02-13 18:39:33.000000 blocklint-0.2.4/tests/config_tests/setup/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 18:39:49.975567 blocklint-0.2.4/tests/config_tests/setup_blocklint/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-02-13 18:39:33.000000 blocklint-0.2.4/tests/config_tests/setup_blocklint/.blocklint
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-02-13 18:39:33.000000 blocklint-0.2.4/tests/config_tests/setup_blocklint/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 18:39:49.975567 blocklint-0.2.4/tests/config_tests/skip_files/
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-02-13 18:39:33.000000 blocklint-0.2.4/tests/config_tests/skip_files/tox.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 18:39:49.975567 blocklint-0.2.4/tests/config_tests/tox/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-02-13 18:39:33.000000 blocklint-0.2.4/tests/config_tests/tox/tox.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 18:39:49.975567 blocklint-0.2.4/tests/config_tests/tox_setup/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-02-13 18:39:33.000000 blocklint-0.2.4/tests/config_tests/tox_setup/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-02-13 18:39:33.000000 blocklint-0.2.4/tests/config_tests/tox_setup/tox.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 18:39:49.975567 blocklint-0.2.4/tests/sample_files/
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-02-13 18:39:33.000000 blocklint-0.2.4/tests/sample_files/blocklist.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-02-13 18:39:33.000000 blocklint-0.2.4/tests/sample_files/default.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-02-13 18:39:33.000000 blocklint-0.2.4/tests/sample_files/end.txt
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-02-13 18:39:33.000000 blocklint-0.2.4/tests/sample_files/exactlist.txt
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-02-13 18:39:33.000000 blocklint-0.2.4/tests/sample_files/pragma.txt
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-02-13 18:39:33.000000 blocklint-0.2.4/tests/sample_files/stdin.txt
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-02-13 18:39:33.000000 blocklint-0.2.4/tests/sample_files/stdin_wordlist.txt
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-02-13 18:39:33.000000 blocklint-0.2.4/tests/sample_files/test.cc
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-02-13 18:39:33.000000 blocklint-0.2.4/tests/sample_files/test.py
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-02-13 18:39:33.000000 blocklint-0.2.4/tests/sample_files/test.txt
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-02-13 18:39:33.000000 blocklint-0.2.4/tests/sample_files/test_pragma.cc
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-02-13 18:39:33.000000 blocklint-0.2.4/tests/sample_files/test_pragma.py
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-02-13 18:39:33.000000 blocklint-0.2.4/tests/sample_files/test_pragma.txt
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-02-13 18:39:33.000000 blocklint-0.2.4/tests/sample_files/wordlist.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     1734 2023-02-13 18:39:33.000000 blocklint-0.2.4/tests/test_configfiles.sh
--rw-r--r--   0 runner    (1001) docker     (123)     8349 2023-02-13 18:39:33.000000 blocklint-0.2.4/tests/test_main.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      725 2023-02-13 18:39:33.000000 blocklint-0.2.4/tests/test_max_issue_threshold.sh
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-02-13 18:39:33.000000 blocklint-0.2.4/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 09:46:15.648987 blocklint-0.2.5/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 09:46:15.636987 blocklint-0.2.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 09:46:15.640987 blocklint-0.2.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-04-06 09:46:06.000000 blocklint-0.2.5/.github/workflows/cd.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-06 09:46:06.000000 blocklint-0.2.5/.github/workflows/pre-commit.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-06 09:46:06.000000 blocklint-0.2.5/.github/workflows/tox.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-06 09:46:06.000000 blocklint-0.2.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-06 09:46:06.000000 blocklint-0.2.5/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-06 09:46:06.000000 blocklint-0.2.5/.pre-commit-hooks.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-06 09:46:06.000000 blocklint-0.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-06 09:46:06.000000 blocklint-0.2.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6820 2024-04-06 09:46:15.648987 blocklint-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5615 2024-04-06 09:46:06.000000 blocklint-0.2.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 09:46:15.640987 blocklint-0.2.5/blocklint/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-06 09:46:06.000000 blocklint-0.2.5/blocklint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-06 09:46:06.000000 blocklint-0.2.5/blocklint/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8590 2024-04-06 09:46:06.000000 blocklint-0.2.5/blocklint/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-06 09:46:15.000000 blocklint-0.2.5/blocklint/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 09:46:15.648987 blocklint-0.2.5/blocklint.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6820 2024-04-06 09:46:15.000000 blocklint-0.2.5/blocklint.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1674 2024-04-06 09:46:15.000000 blocklint-0.2.5/blocklint.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 09:46:15.000000 blocklint-0.2.5/blocklint.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-06 09:46:15.000000 blocklint-0.2.5/blocklint.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-06 09:46:15.000000 blocklint-0.2.5/blocklint.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-06 09:46:15.000000 blocklint-0.2.5/blocklint.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 09:46:15.636987 blocklint-0.2.5/integration/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 09:46:15.640987 blocklint-0.2.5/integration/vim/
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-04-06 09:46:06.000000 blocklint-0.2.5/integration/vim/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 09:46:15.640987 blocklint-0.2.5/integration/vim/autoload/
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-04-06 09:46:06.000000 blocklint-0.2.5/integration/vim/autoload/blocklint.vim
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 09:46:15.640987 blocklint-0.2.5/integration/vim/doc/
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-06 09:46:06.000000 blocklint-0.2.5/integration/vim/doc/blocklint.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 09:46:15.640987 blocklint-0.2.5/integration/vim/plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-06 09:46:06.000000 blocklint-0.2.5/integration/vim/plugin/blocklint.vim
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-06 09:46:06.000000 blocklint-0.2.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-04-06 09:46:15.648987 blocklint-0.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-06 09:46:06.000000 blocklint-0.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 09:46:15.644987 blocklint-0.2.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-06 09:46:06.000000 blocklint-0.2.5/tests/.blocklint
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1303 2024-04-06 09:46:06.000000 blocklint-0.2.5/tests/acceptance_test.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 09:46:15.636987 blocklint-0.2.5/tests/config_tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 09:46:15.644987 blocklint-0.2.5/tests/config_tests/flag_and_list/
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-06 09:46:06.000000 blocklint-0.2.5/tests/config_tests/flag_and_list/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 09:46:15.644987 blocklint-0.2.5/tests/config_tests/setup/
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-06 09:46:06.000000 blocklint-0.2.5/tests/config_tests/setup/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 09:46:15.644987 blocklint-0.2.5/tests/config_tests/setup_blocklint/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-06 09:46:06.000000 blocklint-0.2.5/tests/config_tests/setup_blocklint/.blocklint
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-06 09:46:06.000000 blocklint-0.2.5/tests/config_tests/setup_blocklint/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 09:46:15.644987 blocklint-0.2.5/tests/config_tests/skip_files/
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-06 09:46:06.000000 blocklint-0.2.5/tests/config_tests/skip_files/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 09:46:15.644987 blocklint-0.2.5/tests/config_tests/tox/
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-06 09:46:06.000000 blocklint-0.2.5/tests/config_tests/tox/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 09:46:15.644987 blocklint-0.2.5/tests/config_tests/tox_setup/
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-06 09:46:06.000000 blocklint-0.2.5/tests/config_tests/tox_setup/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-06 09:46:06.000000 blocklint-0.2.5/tests/config_tests/tox_setup/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 09:46:15.644987 blocklint-0.2.5/tests/docstring_tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 09:46:15.644987 blocklint-0.2.5/tests/docstring_tests/sample_files/
+-rw-r--r--   0 runner    (1001) docker     (127)     2803 2024-04-06 09:46:06.000000 blocklint-0.2.5/tests/docstring_tests/sample_files/docstring_test_file_1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-04-06 09:46:06.000000 blocklint-0.2.5/tests/docstring_tests/sample_files/docstring_test_file_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2348 2024-04-06 09:46:06.000000 blocklint-0.2.5/tests/docstring_tests/test_docstring_processing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 09:46:15.648987 blocklint-0.2.5/tests/sample_files/
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-04-06 09:46:06.000000 blocklint-0.2.5/tests/sample_files/blocklist.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-04-06 09:46:06.000000 blocklint-0.2.5/tests/sample_files/default.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-04-06 09:46:06.000000 blocklint-0.2.5/tests/sample_files/end.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-06 09:46:06.000000 blocklint-0.2.5/tests/sample_files/exactlist.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-06 09:46:06.000000 blocklint-0.2.5/tests/sample_files/pragma.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-04-06 09:46:06.000000 blocklint-0.2.5/tests/sample_files/stdin.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-06 09:46:06.000000 blocklint-0.2.5/tests/sample_files/stdin_wordlist.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-06 09:46:06.000000 blocklint-0.2.5/tests/sample_files/test.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-06 09:46:06.000000 blocklint-0.2.5/tests/sample_files/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-06 09:46:06.000000 blocklint-0.2.5/tests/sample_files/test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-06 09:46:06.000000 blocklint-0.2.5/tests/sample_files/test_pragma.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-04-06 09:46:06.000000 blocklint-0.2.5/tests/sample_files/test_pragma.py
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-06 09:46:06.000000 blocklint-0.2.5/tests/sample_files/test_pragma.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-04-06 09:46:06.000000 blocklint-0.2.5/tests/sample_files/wordlist.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1734 2024-04-06 09:46:06.000000 blocklint-0.2.5/tests/test_configfiles.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     8349 2024-04-06 09:46:06.000000 blocklint-0.2.5/tests/test_main.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      725 2024-04-06 09:46:06.000000 blocklint-0.2.5/tests/test_max_issue_threshold.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-06 09:46:06.000000 blocklint-0.2.5/tox.ini
```

### Comparing `blocklint-0.2.4/.github/workflows/cd.yml` & `blocklint-0.2.5/.github/workflows/cd.yml`

 * *Files identical despite different names*

### Comparing `blocklint-0.2.4/.github/workflows/tox.yml` & `blocklint-0.2.5/.github/workflows/tox.yml`

 * *Files identical despite different names*

### Comparing `blocklint-0.2.4/LICENSE` & `blocklint-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `blocklint-0.2.4/PKG-INFO` & `blocklint-0.2.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blocklint
-Version: 0.2.4
+Version: 0.2.5
 Summary: Lint for blocklisted words.
 Home-page: https://github.com/PrincetonUniversity/blocklint
 Author: Troy Comi
 Author-email: tcomi@princeton.edu
 License: MIT License
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -20,16 +20,19 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Software Development
 Classifier: Topic :: Utilities
 Requires-Python: !=3.0,!=3.1,!=3.2,!=3.3,!=3.4,>=2.7
 Description-Content-Type: text/markdown
-Provides-Extra: test
 License-File: LICENSE
+Provides-Extra: test
+Requires-Dist: tox; extra == "test"
+Requires-Dist: pytest; extra == "test"
+Requires-Dist: pytest-mock; extra == "test"
 
 # blocklint
 [![PyPI version](https://badge.fury.io/py/blocklint.svg)](https://badge.fury.io/py/blocklint)
 [![GitHub Actions (Tests)](https://github.com/PrincetonUniversity/blocklint/workflows/ToxTests/badge.svg)](https://github.com/PrincetonUniversity/blocklint)
 [![GitHub Actions (pre-commit)](https://github.com/PrincetonUniversity/blocklint/workflows/pre-commit/badge.svg)](https://github.com/PrincetonUniversity/blocklint)
 [![GitHub license](https://img.shields.io/github/license/PrincetonUniversity/blocklint)](https://github.com/PrincetonUniversity/blocklint/blob/master/LICENSE)
```

### Comparing `blocklint-0.2.4/README.md` & `blocklint-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `blocklint-0.2.4/blocklint/main.py` & `blocklint-0.2.5/blocklint/main.py`

 * *Files 9% similar despite different names*

```diff
@@ -34,28 +34,55 @@
         total_issues += process_file(sys.stdin, 'stdin', word_checkers,
                                      args['end_pos'])
     else:
         for file in args['files']:
             with open(file, 'r') as handle:
                 total_issues += process_file(handle, file, word_checkers,
                                              args['end_pos'])
-
     if (args['max_issue_threshold'] is not None
             and args['max_issue_threshold'] <= total_issues):
         print(("Found {issues} issues, with maximum set to "
                "{max}!").format(
                    issues=total_issues,
                    max=args['max_issue_threshold']))
         sys.exit(1)
 
 
+def clean_ignored_docstrings(lines):
+    end_pattern = re.compile(r'(("""|\'\'\')\s*#\s*blocklint:.*pragma\s*$)')
+    lines_to_clear = []
+
+    for i, line in enumerate(lines):
+        match = end_pattern.search(line)
+        if match:
+            start_quote = match.group(1)[:3]  # This is either """ or '''
+
+            if start_quote in line[:-(len(match.group(1)))]:
+                # single line docstring
+                lines_to_clear.append((i, i+1))
+            else:
+                # multi line docstring - scan backwards from the current line
+                for j in range(i-1, -1, -1):
+                    if start_quote in lines[j]:
+                        lines_to_clear.append((j, i+1))
+                        break
+
+    for start_line, stop_line in lines_to_clear:
+        for ignored_line in range(start_line, stop_line):
+            lines[ignored_line] = ""
+
+    return lines
+
+
 def process_file(input_file, file_name, word_checkers, end_pos):
     num_matched = 0
     try:
-        for i, line in enumerate(input_file, 1):
+        lines = input_file.readlines()
+        lines = clean_ignored_docstrings(lines)
+        for i, line in enumerate(lines, 1):
             for match in check_line(line, word_checkers,
                                     file_name, i, end_pos):
                 num_matched += 1
                 print(match)
     except FileNotFoundError:
         pass
     except UnicodeDecodeError:
```

### Comparing `blocklint-0.2.4/blocklint.egg-info/PKG-INFO` & `blocklint-0.2.5/blocklint.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blocklint
-Version: 0.2.4
+Version: 0.2.5
 Summary: Lint for blocklisted words.
 Home-page: https://github.com/PrincetonUniversity/blocklint
 Author: Troy Comi
 Author-email: tcomi@princeton.edu
 License: MIT License
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -20,16 +20,19 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Software Development
 Classifier: Topic :: Utilities
 Requires-Python: !=3.0,!=3.1,!=3.2,!=3.3,!=3.4,>=2.7
 Description-Content-Type: text/markdown
-Provides-Extra: test
 License-File: LICENSE
+Provides-Extra: test
+Requires-Dist: tox; extra == "test"
+Requires-Dist: pytest; extra == "test"
+Requires-Dist: pytest-mock; extra == "test"
 
 # blocklint
 [![PyPI version](https://badge.fury.io/py/blocklint.svg)](https://badge.fury.io/py/blocklint)
 [![GitHub Actions (Tests)](https://github.com/PrincetonUniversity/blocklint/workflows/ToxTests/badge.svg)](https://github.com/PrincetonUniversity/blocklint)
 [![GitHub Actions (pre-commit)](https://github.com/PrincetonUniversity/blocklint/workflows/pre-commit/badge.svg)](https://github.com/PrincetonUniversity/blocklint)
 [![GitHub license](https://img.shields.io/github/license/PrincetonUniversity/blocklint)](https://github.com/PrincetonUniversity/blocklint/blob/master/LICENSE)
```

### Comparing `blocklint-0.2.4/blocklint.egg-info/SOURCES.txt` & `blocklint-0.2.5/blocklint.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -34,14 +34,17 @@
 tests/config_tests/setup/setup.cfg
 tests/config_tests/setup_blocklint/.blocklint
 tests/config_tests/setup_blocklint/setup.cfg
 tests/config_tests/skip_files/tox.ini
 tests/config_tests/tox/tox.ini
 tests/config_tests/tox_setup/setup.cfg
 tests/config_tests/tox_setup/tox.ini
+tests/docstring_tests/test_docstring_processing.py
+tests/docstring_tests/sample_files/docstring_test_file_1.py
+tests/docstring_tests/sample_files/docstring_test_file_2.py
 tests/sample_files/blocklist.txt
 tests/sample_files/default.txt
 tests/sample_files/end.txt
 tests/sample_files/exactlist.txt
 tests/sample_files/pragma.txt
 tests/sample_files/stdin.txt
 tests/sample_files/stdin_wordlist.txt
```

### Comparing `blocklint-0.2.4/integration/vim/README.md` & `blocklint-0.2.5/integration/vim/README.md`

 * *Files identical despite different names*

### Comparing `blocklint-0.2.4/integration/vim/autoload/blocklint.vim` & `blocklint-0.2.5/integration/vim/autoload/blocklint.vim`

 * *Files identical despite different names*

### Comparing `blocklint-0.2.4/integration/vim/plugin/blocklint.vim` & `blocklint-0.2.5/integration/vim/plugin/blocklint.vim`

 * *Files identical despite different names*

### Comparing `blocklint-0.2.4/setup.cfg` & `blocklint-0.2.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `blocklint-0.2.4/tests/acceptance_test.sh` & `blocklint-0.2.5/tests/acceptance_test.sh`

 * *Files identical despite different names*

### Comparing `blocklint-0.2.4/tests/sample_files/blocklist.txt` & `blocklint-0.2.5/tests/sample_files/blocklist.txt`

 * *Files identical despite different names*

### Comparing `blocklint-0.2.4/tests/sample_files/default.txt` & `blocklint-0.2.5/tests/sample_files/default.txt`

 * *Files identical despite different names*

### Comparing `blocklint-0.2.4/tests/sample_files/end.txt` & `blocklint-0.2.5/tests/sample_files/end.txt`

 * *Files identical despite different names*

### Comparing `blocklint-0.2.4/tests/sample_files/stdin.txt` & `blocklint-0.2.5/tests/sample_files/stdin.txt`

 * *Files identical despite different names*

### Comparing `blocklint-0.2.4/tests/sample_files/wordlist.txt` & `blocklint-0.2.5/tests/sample_files/wordlist.txt`

 * *Files identical despite different names*

### Comparing `blocklint-0.2.4/tests/test_configfiles.sh` & `blocklint-0.2.5/tests/test_configfiles.sh`

 * *Files identical despite different names*

### Comparing `blocklint-0.2.4/tests/test_main.py` & `blocklint-0.2.5/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `blocklint-0.2.4/tests/test_max_issue_threshold.sh` & `blocklint-0.2.5/tests/test_max_issue_threshold.sh`

 * *Files identical despite different names*

