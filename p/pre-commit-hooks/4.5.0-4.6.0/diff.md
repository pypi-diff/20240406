# Comparing `tmp/pre_commit_hooks-4.5.0.tar.gz` & `tmp/pre_commit_hooks-4.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pre_commit_hooks-4.5.0.tar", last modified: Sat Oct  7 18:04:58 2023, max compression
+gzip compressed data, was "pre_commit_hooks-4.6.0.tar", last modified: Sat Apr  6 18:24:46 2024, max compression
```

## Comparing `pre_commit_hooks-4.5.0.tar` & `pre_commit_hooks-4.6.0.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-10-07 18:04:58.511832 pre_commit_hooks-4.5.0/
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1092 2022-04-30 16:59:41.000000 pre_commit_hooks-4.5.0/LICENSE
--rw-r--r--   0 asottile  (1000) asottile  (1000)     9834 2023-10-07 18:04:58.511832 pre_commit_hooks-4.5.0/PKG-INFO
--rw-r--r--   0 asottile  (1000) asottile  (1000)     9213 2023-10-07 18:04:06.000000 pre_commit_hooks-4.5.0/README.md
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-10-07 18:04:58.511832 pre_commit_hooks-4.5.0/pre_commit_hooks/
--rw-r--r--   0 asottile  (1000) asottile  (1000)        0 2022-04-30 16:59:41.000000 pre_commit_hooks-4.5.0/pre_commit_hooks/__init__.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     2156 2023-10-07 17:41:55.000000 pre_commit_hooks-4.5.0/pre_commit_hooks/check_added_large_files.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      874 2022-04-30 16:59:41.000000 pre_commit_hooks-4.5.0/pre_commit_hooks/check_ast.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     2920 2022-04-30 16:59:41.000000 pre_commit_hooks-4.5.0/pre_commit_hooks/check_builtin_literals.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      581 2022-04-30 16:59:41.000000 pre_commit_hooks-4.5.0/pre_commit_hooks/check_byte_order_marker.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     2047 2022-04-30 16:59:41.000000 pre_commit_hooks-4.5.0/pre_commit_hooks/check_case_conflict.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1930 2022-04-30 16:59:41.000000 pre_commit_hooks-4.5.0/pre_commit_hooks/check_docstring_first.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     2427 2022-11-23 19:32:33.000000 pre_commit_hooks-4.5.0/pre_commit_hooks/check_executables_have_shebangs.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      974 2022-04-30 16:59:41.000000 pre_commit_hooks-4.5.0/pre_commit_hooks/check_json.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1537 2022-04-30 16:59:41.000000 pre_commit_hooks-4.5.0/pre_commit_hooks/check_merge_conflict.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1791 2022-11-23 19:32:33.000000 pre_commit_hooks-4.5.0/pre_commit_hooks/check_shebang_scripts_are_executable.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      696 2022-04-30 16:59:41.000000 pre_commit_hooks-4.5.0/pre_commit_hooks/check_symlinks.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      762 2022-11-23 19:32:33.000000 pre_commit_hooks-4.5.0/pre_commit_hooks/check_toml.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1556 2022-04-30 16:59:41.000000 pre_commit_hooks-4.5.0/pre_commit_hooks/check_vcs_permalinks.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      728 2022-04-30 16:59:41.000000 pre_commit_hooks-4.5.0/pre_commit_hooks/check_xml.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1916 2023-10-07 17:41:55.000000 pre_commit_hooks-4.5.0/pre_commit_hooks/check_yaml.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     2209 2023-10-07 17:41:55.000000 pre_commit_hooks-4.5.0/pre_commit_hooks/debug_statement_hook.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     3561 2023-10-07 17:41:55.000000 pre_commit_hooks-4.5.0/pre_commit_hooks/destroyed_symlinks.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     4547 2022-04-30 16:59:41.000000 pre_commit_hooks-4.5.0/pre_commit_hooks/detect_aws_credentials.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1114 2022-04-30 16:59:41.000000 pre_commit_hooks-4.5.0/pre_commit_hooks/detect_private_key.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     2154 2022-04-30 16:59:41.000000 pre_commit_hooks-4.5.0/pre_commit_hooks/end_of_file_fixer.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     2239 2023-10-07 17:41:55.000000 pre_commit_hooks-4.5.0/pre_commit_hooks/file_contents_sorter.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      814 2022-04-30 16:59:41.000000 pre_commit_hooks-4.5.0/pre_commit_hooks/fix_byte_order_marker.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     3959 2022-04-30 16:59:41.000000 pre_commit_hooks-4.5.0/pre_commit_hooks/fix_encoding_pragma.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1302 2022-04-30 16:59:41.000000 pre_commit_hooks-4.5.0/pre_commit_hooks/forbid_new_submodules.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     2641 2022-04-30 16:59:41.000000 pre_commit_hooks-4.5.0/pre_commit_hooks/mixed_line_ending.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1353 2022-04-30 16:59:41.000000 pre_commit_hooks-4.5.0/pre_commit_hooks/no_commit_to_branch.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     3819 2022-04-30 16:59:41.000000 pre_commit_hooks-4.5.0/pre_commit_hooks/pretty_format_json.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      381 2022-04-30 16:59:41.000000 pre_commit_hooks-4.5.0/pre_commit_hooks/removed.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     4278 2022-04-30 16:59:41.000000 pre_commit_hooks-4.5.0/pre_commit_hooks/requirements_txt_fixer.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     3283 2022-04-30 16:59:41.000000 pre_commit_hooks-4.5.0/pre_commit_hooks/sort_simple_yaml.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     2693 2023-10-07 17:56:00.000000 pre_commit_hooks-4.5.0/pre_commit_hooks/string_fixer.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1399 2022-11-23 19:32:33.000000 pre_commit_hooks-4.5.0/pre_commit_hooks/tests_should_end_in_test.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     3160 2022-04-30 16:59:41.000000 pre_commit_hooks-4.5.0/pre_commit_hooks/trailing_whitespace_fixer.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      846 2022-04-30 16:59:41.000000 pre_commit_hooks-4.5.0/pre_commit_hooks/util.py
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-10-07 18:04:58.511832 pre_commit_hooks-4.5.0/pre_commit_hooks.egg-info/
--rw-r--r--   0 asottile  (1000) asottile  (1000)     9834 2023-10-07 18:04:58.000000 pre_commit_hooks-4.5.0/pre_commit_hooks.egg-info/PKG-INFO
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1677 2023-10-07 18:04:58.000000 pre_commit_hooks-4.5.0/pre_commit_hooks.egg-info/SOURCES.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)        1 2023-10-07 18:04:58.000000 pre_commit_hooks-4.5.0/pre_commit_hooks.egg-info/dependency_links.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)     2123 2023-10-07 18:04:58.000000 pre_commit_hooks-4.5.0/pre_commit_hooks.egg-info/entry_points.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)       59 2023-10-07 18:04:58.000000 pre_commit_hooks-4.5.0/pre_commit_hooks.egg-info/requires.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)       17 2023-10-07 18:04:58.000000 pre_commit_hooks-4.5.0/pre_commit_hooks.egg-info/top_level.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)     3338 2023-10-07 18:04:58.511832 pre_commit_hooks-4.5.0/setup.cfg
--rw-r--r--   0 asottile  (1000) asottile  (1000)       73 2022-04-30 16:59:41.000000 pre_commit_hooks-4.5.0/setup.py
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-10-07 18:04:58.511832 pre_commit_hooks-4.5.0/tests/
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1192 2022-11-23 19:32:33.000000 pre_commit_hooks-4.5.0/tests/tests_should_end_in_test_test.py
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2024-04-06 18:24:46.052145 pre_commit_hooks-4.6.0/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1092 2024-04-06 18:09:39.000000 pre_commit_hooks-4.6.0/LICENSE
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     9932 2024-04-06 18:24:46.052145 pre_commit_hooks-4.6.0/PKG-INFO
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     9311 2024-04-06 18:24:28.000000 pre_commit_hooks-4.6.0/README.md
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2024-04-06 18:24:46.052145 pre_commit_hooks-4.6.0/pre_commit_hooks/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)        0 2024-04-06 18:09:39.000000 pre_commit_hooks-4.6.0/pre_commit_hooks/__init__.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     2156 2024-04-06 18:09:39.000000 pre_commit_hooks-4.6.0/pre_commit_hooks/check_added_large_files.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      874 2024-04-06 18:09:39.000000 pre_commit_hooks-4.6.0/pre_commit_hooks/check_ast.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     2920 2024-04-06 18:09:39.000000 pre_commit_hooks-4.6.0/pre_commit_hooks/check_builtin_literals.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      581 2024-04-06 18:09:39.000000 pre_commit_hooks-4.6.0/pre_commit_hooks/check_byte_order_marker.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     2047 2024-04-06 18:09:39.000000 pre_commit_hooks-4.6.0/pre_commit_hooks/check_case_conflict.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1930 2024-04-06 18:09:39.000000 pre_commit_hooks-4.6.0/pre_commit_hooks/check_docstring_first.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     2427 2024-04-06 18:09:39.000000 pre_commit_hooks-4.6.0/pre_commit_hooks/check_executables_have_shebangs.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      974 2024-04-06 18:09:39.000000 pre_commit_hooks-4.6.0/pre_commit_hooks/check_json.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1537 2024-04-06 18:09:39.000000 pre_commit_hooks-4.6.0/pre_commit_hooks/check_merge_conflict.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1791 2024-04-06 18:09:39.000000 pre_commit_hooks-4.6.0/pre_commit_hooks/check_shebang_scripts_are_executable.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      696 2024-04-06 18:09:39.000000 pre_commit_hooks-4.6.0/pre_commit_hooks/check_symlinks.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      762 2024-04-06 18:09:39.000000 pre_commit_hooks-4.6.0/pre_commit_hooks/check_toml.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1556 2024-04-06 18:09:39.000000 pre_commit_hooks-4.6.0/pre_commit_hooks/check_vcs_permalinks.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      728 2024-04-06 18:09:39.000000 pre_commit_hooks-4.6.0/pre_commit_hooks/check_xml.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1916 2024-04-06 18:09:39.000000 pre_commit_hooks-4.6.0/pre_commit_hooks/check_yaml.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     2209 2024-04-06 18:09:39.000000 pre_commit_hooks-4.6.0/pre_commit_hooks/debug_statement_hook.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     3561 2024-04-06 18:09:39.000000 pre_commit_hooks-4.6.0/pre_commit_hooks/destroyed_symlinks.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     4547 2024-04-06 18:09:39.000000 pre_commit_hooks-4.6.0/pre_commit_hooks/detect_aws_credentials.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1114 2024-04-06 18:09:39.000000 pre_commit_hooks-4.6.0/pre_commit_hooks/detect_private_key.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     2154 2024-04-06 18:09:39.000000 pre_commit_hooks-4.6.0/pre_commit_hooks/end_of_file_fixer.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     2239 2024-04-06 18:09:39.000000 pre_commit_hooks-4.6.0/pre_commit_hooks/file_contents_sorter.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      814 2024-04-06 18:09:39.000000 pre_commit_hooks-4.6.0/pre_commit_hooks/fix_byte_order_marker.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     4190 2024-04-06 18:20:20.000000 pre_commit_hooks-4.6.0/pre_commit_hooks/fix_encoding_pragma.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1302 2024-04-06 18:09:39.000000 pre_commit_hooks-4.6.0/pre_commit_hooks/forbid_new_submodules.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     2641 2024-04-06 18:09:39.000000 pre_commit_hooks-4.6.0/pre_commit_hooks/mixed_line_ending.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1353 2024-04-06 18:09:39.000000 pre_commit_hooks-4.6.0/pre_commit_hooks/no_commit_to_branch.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     3819 2024-04-06 18:09:39.000000 pre_commit_hooks-4.6.0/pre_commit_hooks/pretty_format_json.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      381 2024-04-06 18:09:39.000000 pre_commit_hooks-4.6.0/pre_commit_hooks/removed.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     4743 2024-04-06 18:09:39.000000 pre_commit_hooks-4.6.0/pre_commit_hooks/requirements_txt_fixer.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     3283 2024-04-06 18:09:39.000000 pre_commit_hooks-4.6.0/pre_commit_hooks/sort_simple_yaml.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     2693 2024-04-06 18:09:39.000000 pre_commit_hooks-4.6.0/pre_commit_hooks/string_fixer.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1399 2024-04-06 18:09:39.000000 pre_commit_hooks-4.6.0/pre_commit_hooks/tests_should_end_in_test.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     3160 2024-04-06 18:09:39.000000 pre_commit_hooks-4.6.0/pre_commit_hooks/trailing_whitespace_fixer.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      846 2024-04-06 18:09:39.000000 pre_commit_hooks-4.6.0/pre_commit_hooks/util.py
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2024-04-06 18:24:46.052145 pre_commit_hooks-4.6.0/pre_commit_hooks.egg-info/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     9932 2024-04-06 18:24:45.000000 pre_commit_hooks-4.6.0/pre_commit_hooks.egg-info/PKG-INFO
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1677 2024-04-06 18:24:45.000000 pre_commit_hooks-4.6.0/pre_commit_hooks.egg-info/SOURCES.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)        1 2024-04-06 18:24:45.000000 pre_commit_hooks-4.6.0/pre_commit_hooks.egg-info/dependency_links.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     2123 2024-04-06 18:24:45.000000 pre_commit_hooks-4.6.0/pre_commit_hooks.egg-info/entry_points.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       59 2024-04-06 18:24:45.000000 pre_commit_hooks-4.6.0/pre_commit_hooks.egg-info/requires.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       17 2024-04-06 18:24:45.000000 pre_commit_hooks-4.6.0/pre_commit_hooks.egg-info/top_level.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     3338 2024-04-06 18:24:46.052145 pre_commit_hooks-4.6.0/setup.cfg
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       73 2024-04-06 18:09:39.000000 pre_commit_hooks-4.6.0/setup.py
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2024-04-06 18:24:46.052145 pre_commit_hooks-4.6.0/tests/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1192 2024-04-06 18:09:39.000000 pre_commit_hooks-4.6.0/tests/tests_should_end_in_test_test.py
```

### Comparing `pre_commit_hooks-4.5.0/LICENSE` & `pre_commit_hooks-4.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pre_commit_hooks-4.5.0/PKG-INFO` & `pre_commit_hooks-4.6.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,7 @@
-Metadata-Version: 2.1
-Name: pre_commit_hooks
-Version: 4.5.0
-Summary: Some out-of-the-box hooks for pre-commit.
-Home-page: https://github.com/pre-commit/pre-commit-hooks
-Author: Anthony Sottile
-Author-email: asottile@umich.edu
-License: MIT
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 [![build status](https://github.com/pre-commit/pre-commit-hooks/actions/workflows/main.yml/badge.svg)](https://github.com/pre-commit/pre-commit-hooks/actions/workflows/main.yml)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/pre-commit/pre-commit-hooks/main.svg)](https://results.pre-commit.ci/latest/github/pre-commit/pre-commit-hooks/main)
 
 pre-commit-hooks
 ================
 
 Some out-of-the-box hooks for pre-commit.
@@ -28,15 +11,15 @@
 
 ### Using pre-commit-hooks with pre-commit
 
 Add this to your `.pre-commit-config.yaml`
 
 ```yaml
 -   repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.5.0  # Use the ref you want to point at
+    rev: v4.6.0  # Use the ref you want to point at
     hooks:
     -   id: trailing-whitespace
     # -   id: ...
 ```
 
 ### Hooks available
 
@@ -140,14 +123,17 @@
 - `--ignore-case` - fold lower case to upper case characters.
 - `--unique` - ensure each line is unique.
 
 #### `fix-byte-order-marker`
 removes UTF-8 byte order marker
 
 #### `fix-encoding-pragma`
+
+_Deprecated since py2 is EOL - use [pyupgrade](https://github.com/asottile/pyupgrade) instead._
+
 Add `# -*- coding: utf-8 -*-` to the top of python files.
   - To remove the coding pragma pass `--remove` (useful in a python3-only codebase)
 
 #### `forbid-new-submodules`
 Prevent addition of new git submodules.
 
 This is intended as a helper to migrate away from submodules.  If you want to
```

### Comparing `pre_commit_hooks-4.5.0/README.md` & `pre_commit_hooks-4.6.0/pre_commit_hooks.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+Metadata-Version: 2.1
+Name: pre-commit-hooks
+Version: 4.6.0
+Summary: Some out-of-the-box hooks for pre-commit.
+Home-page: https://github.com/pre-commit/pre-commit-hooks
+Author: Anthony Sottile
+Author-email: asottile@umich.edu
+License: MIT
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: Implementation :: PyPy
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 [![build status](https://github.com/pre-commit/pre-commit-hooks/actions/workflows/main.yml/badge.svg)](https://github.com/pre-commit/pre-commit-hooks/actions/workflows/main.yml)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/pre-commit/pre-commit-hooks/main.svg)](https://results.pre-commit.ci/latest/github/pre-commit/pre-commit-hooks/main)
 
 pre-commit-hooks
 ================
 
 Some out-of-the-box hooks for pre-commit.
@@ -11,15 +28,15 @@
 
 ### Using pre-commit-hooks with pre-commit
 
 Add this to your `.pre-commit-config.yaml`
 
 ```yaml
 -   repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.5.0  # Use the ref you want to point at
+    rev: v4.6.0  # Use the ref you want to point at
     hooks:
     -   id: trailing-whitespace
     # -   id: ...
 ```
 
 ### Hooks available
 
@@ -123,14 +140,17 @@
 - `--ignore-case` - fold lower case to upper case characters.
 - `--unique` - ensure each line is unique.
 
 #### `fix-byte-order-marker`
 removes UTF-8 byte order marker
 
 #### `fix-encoding-pragma`
+
+_Deprecated since py2 is EOL - use [pyupgrade](https://github.com/asottile/pyupgrade) instead._
+
 Add `# -*- coding: utf-8 -*-` to the top of python files.
   - To remove the coding pragma pass `--remove` (useful in a python3-only codebase)
 
 #### `forbid-new-submodules`
 Prevent addition of new git submodules.
 
 This is intended as a helper to migrate away from submodules.  If you want to
```

### Comparing `pre_commit_hooks-4.5.0/pre_commit_hooks/check_added_large_files.py` & `pre_commit_hooks-4.6.0/pre_commit_hooks/check_added_large_files.py`

 * *Files identical despite different names*

### Comparing `pre_commit_hooks-4.5.0/pre_commit_hooks/check_ast.py` & `pre_commit_hooks-4.6.0/pre_commit_hooks/check_ast.py`

 * *Files identical despite different names*

### Comparing `pre_commit_hooks-4.5.0/pre_commit_hooks/check_builtin_literals.py` & `pre_commit_hooks-4.6.0/pre_commit_hooks/check_builtin_literals.py`

 * *Files identical despite different names*

### Comparing `pre_commit_hooks-4.5.0/pre_commit_hooks/check_byte_order_marker.py` & `pre_commit_hooks-4.6.0/pre_commit_hooks/check_byte_order_marker.py`

 * *Files identical despite different names*

### Comparing `pre_commit_hooks-4.5.0/pre_commit_hooks/check_case_conflict.py` & `pre_commit_hooks-4.6.0/pre_commit_hooks/check_case_conflict.py`

 * *Files identical despite different names*

### Comparing `pre_commit_hooks-4.5.0/pre_commit_hooks/check_docstring_first.py` & `pre_commit_hooks-4.6.0/pre_commit_hooks/check_docstring_first.py`

 * *Files identical despite different names*

### Comparing `pre_commit_hooks-4.5.0/pre_commit_hooks/check_executables_have_shebangs.py` & `pre_commit_hooks-4.6.0/pre_commit_hooks/check_executables_have_shebangs.py`

 * *Files identical despite different names*

### Comparing `pre_commit_hooks-4.5.0/pre_commit_hooks/check_json.py` & `pre_commit_hooks-4.6.0/pre_commit_hooks/check_json.py`

 * *Files identical despite different names*

### Comparing `pre_commit_hooks-4.5.0/pre_commit_hooks/check_merge_conflict.py` & `pre_commit_hooks-4.6.0/pre_commit_hooks/check_merge_conflict.py`

 * *Files identical despite different names*

### Comparing `pre_commit_hooks-4.5.0/pre_commit_hooks/check_shebang_scripts_are_executable.py` & `pre_commit_hooks-4.6.0/pre_commit_hooks/check_shebang_scripts_are_executable.py`

 * *Files identical despite different names*

### Comparing `pre_commit_hooks-4.5.0/pre_commit_hooks/check_symlinks.py` & `pre_commit_hooks-4.6.0/pre_commit_hooks/check_symlinks.py`

 * *Files identical despite different names*

### Comparing `pre_commit_hooks-4.5.0/pre_commit_hooks/check_toml.py` & `pre_commit_hooks-4.6.0/pre_commit_hooks/check_toml.py`

 * *Files identical despite different names*

### Comparing `pre_commit_hooks-4.5.0/pre_commit_hooks/check_vcs_permalinks.py` & `pre_commit_hooks-4.6.0/pre_commit_hooks/check_vcs_permalinks.py`

 * *Files identical despite different names*

### Comparing `pre_commit_hooks-4.5.0/pre_commit_hooks/check_xml.py` & `pre_commit_hooks-4.6.0/pre_commit_hooks/check_xml.py`

 * *Files identical despite different names*

### Comparing `pre_commit_hooks-4.5.0/pre_commit_hooks/check_yaml.py` & `pre_commit_hooks-4.6.0/pre_commit_hooks/check_yaml.py`

 * *Files identical despite different names*

### Comparing `pre_commit_hooks-4.5.0/pre_commit_hooks/debug_statement_hook.py` & `pre_commit_hooks-4.6.0/pre_commit_hooks/debug_statement_hook.py`

 * *Files identical despite different names*

### Comparing `pre_commit_hooks-4.5.0/pre_commit_hooks/destroyed_symlinks.py` & `pre_commit_hooks-4.6.0/pre_commit_hooks/destroyed_symlinks.py`

 * *Files identical despite different names*

### Comparing `pre_commit_hooks-4.5.0/pre_commit_hooks/detect_aws_credentials.py` & `pre_commit_hooks-4.6.0/pre_commit_hooks/detect_aws_credentials.py`

 * *Files identical despite different names*

### Comparing `pre_commit_hooks-4.5.0/pre_commit_hooks/detect_private_key.py` & `pre_commit_hooks-4.6.0/pre_commit_hooks/detect_private_key.py`

 * *Files identical despite different names*

### Comparing `pre_commit_hooks-4.5.0/pre_commit_hooks/end_of_file_fixer.py` & `pre_commit_hooks-4.6.0/pre_commit_hooks/end_of_file_fixer.py`

 * *Files identical despite different names*

### Comparing `pre_commit_hooks-4.5.0/pre_commit_hooks/file_contents_sorter.py` & `pre_commit_hooks-4.6.0/pre_commit_hooks/file_contents_sorter.py`

 * *Files identical despite different names*

### Comparing `pre_commit_hooks-4.5.0/pre_commit_hooks/fix_byte_order_marker.py` & `pre_commit_hooks-4.6.0/pre_commit_hooks/fix_byte_order_marker.py`

 * *Files identical despite different names*

### Comparing `pre_commit_hooks-4.5.0/pre_commit_hooks/fix_encoding_pragma.py` & `pre_commit_hooks-4.6.0/pre_commit_hooks/fix_encoding_pragma.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 
 import argparse
+import sys
 from typing import IO
 from typing import NamedTuple
 from typing import Sequence
 
 DEFAULT_PRAGMA = b'# -*- coding: utf-8 -*-'
 
 
@@ -103,14 +104,21 @@
 
 
 def _normalize_pragma(pragma: str) -> bytes:
     return pragma.encode().rstrip()
 
 
 def main(argv: Sequence[str] | None = None) -> int:
+    print(
+        'warning: this hook is deprecated and will be removed in a future '
+        'release because py2 is EOL. instead, use '
+        'https://github.com/asottile/pyupgrade',
+        file=sys.stderr,
+    )
+
     parser = argparse.ArgumentParser(
         'Fixes the encoding pragma of python files',
     )
     parser.add_argument('filenames', nargs='*', help='Filenames to fix')
     parser.add_argument(
         '--pragma', default=DEFAULT_PRAGMA, type=_normalize_pragma,
         help=(
```

### Comparing `pre_commit_hooks-4.5.0/pre_commit_hooks/forbid_new_submodules.py` & `pre_commit_hooks-4.6.0/pre_commit_hooks/forbid_new_submodules.py`

 * *Files identical despite different names*

### Comparing `pre_commit_hooks-4.5.0/pre_commit_hooks/mixed_line_ending.py` & `pre_commit_hooks-4.6.0/pre_commit_hooks/mixed_line_ending.py`

 * *Files identical despite different names*

### Comparing `pre_commit_hooks-4.5.0/pre_commit_hooks/no_commit_to_branch.py` & `pre_commit_hooks-4.6.0/pre_commit_hooks/no_commit_to_branch.py`

 * *Files identical despite different names*

### Comparing `pre_commit_hooks-4.5.0/pre_commit_hooks/pretty_format_json.py` & `pre_commit_hooks-4.6.0/pre_commit_hooks/pretty_format_json.py`

 * *Files identical despite different names*

### Comparing `pre_commit_hooks-4.5.0/pre_commit_hooks/requirements_txt_fixer.py` & `pre_commit_hooks-4.6.0/pre_commit_hooks/requirements_txt_fixer.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,14 +41,19 @@
         # otherwise just do a string comparison with value.
         assert self.value is not None, self.value
         if self.value == b'\n':
             return True
         elif requirement.value == b'\n':
             return False
         else:
+            # if 2 requirements have the same name, the one with comments
+            # needs to go first (so that when removing duplicates, the one
+            # with comments is kept)
+            if self.name == requirement.name:
+                return bool(self.comments) > bool(requirement.comments)
             return self.name < requirement.name
 
     def is_complete(self) -> bool:
         return (
             self.value is not None and
             not self.value.rstrip(b'\r\n').endswith(b'\\')
         )
@@ -109,18 +114,22 @@
     # find and remove pkg-resources==0.0.0
     # which is automatically added by broken pip package under Debian
     requirements = [
         req for req in requirements
         if req.value != b'pkg-resources==0.0.0\n'
     ]
 
+    # sort the requirements and remove duplicates
+    prev = None
     for requirement in sorted(requirements):
         after.extend(requirement.comments)
         assert requirement.value, requirement.value
-        after.append(requirement.value)
+        if prev is None or requirement.value != prev.value:
+            after.append(requirement.value)
+            prev = requirement
     after.extend(rest)
 
     after_string = b''.join(after)
 
     if before_string == after_string:
         return PASS
     else:
```

### Comparing `pre_commit_hooks-4.5.0/pre_commit_hooks/sort_simple_yaml.py` & `pre_commit_hooks-4.6.0/pre_commit_hooks/sort_simple_yaml.py`

 * *Files identical despite different names*

### Comparing `pre_commit_hooks-4.5.0/pre_commit_hooks/string_fixer.py` & `pre_commit_hooks-4.6.0/pre_commit_hooks/string_fixer.py`

 * *Files identical despite different names*

### Comparing `pre_commit_hooks-4.5.0/pre_commit_hooks/tests_should_end_in_test.py` & `pre_commit_hooks-4.6.0/pre_commit_hooks/tests_should_end_in_test.py`

 * *Files identical despite different names*

### Comparing `pre_commit_hooks-4.5.0/pre_commit_hooks/trailing_whitespace_fixer.py` & `pre_commit_hooks-4.6.0/pre_commit_hooks/trailing_whitespace_fixer.py`

 * *Files identical despite different names*

### Comparing `pre_commit_hooks-4.5.0/pre_commit_hooks/util.py` & `pre_commit_hooks-4.6.0/pre_commit_hooks/util.py`

 * *Files identical despite different names*

### Comparing `pre_commit_hooks-4.5.0/pre_commit_hooks.egg-info/PKG-INFO` & `pre_commit_hooks-4.6.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pre-commit-hooks
-Version: 4.5.0
+Name: pre_commit_hooks
+Version: 4.6.0
 Summary: Some out-of-the-box hooks for pre-commit.
 Home-page: https://github.com/pre-commit/pre-commit-hooks
 Author: Anthony Sottile
 Author-email: asottile@umich.edu
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -28,15 +28,15 @@
 
 ### Using pre-commit-hooks with pre-commit
 
 Add this to your `.pre-commit-config.yaml`
 
 ```yaml
 -   repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.5.0  # Use the ref you want to point at
+    rev: v4.6.0  # Use the ref you want to point at
     hooks:
     -   id: trailing-whitespace
     # -   id: ...
 ```
 
 ### Hooks available
 
@@ -140,14 +140,17 @@
 - `--ignore-case` - fold lower case to upper case characters.
 - `--unique` - ensure each line is unique.
 
 #### `fix-byte-order-marker`
 removes UTF-8 byte order marker
 
 #### `fix-encoding-pragma`
+
+_Deprecated since py2 is EOL - use [pyupgrade](https://github.com/asottile/pyupgrade) instead._
+
 Add `# -*- coding: utf-8 -*-` to the top of python files.
   - To remove the coding pragma pass `--remove` (useful in a python3-only codebase)
 
 #### `forbid-new-submodules`
 Prevent addition of new git submodules.
 
 This is intended as a helper to migrate away from submodules.  If you want to
```

### Comparing `pre_commit_hooks-4.5.0/pre_commit_hooks.egg-info/SOURCES.txt` & `pre_commit_hooks-4.6.0/pre_commit_hooks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pre_commit_hooks-4.5.0/pre_commit_hooks.egg-info/entry_points.txt` & `pre_commit_hooks-4.6.0/pre_commit_hooks.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `pre_commit_hooks-4.5.0/setup.cfg` & `pre_commit_hooks-4.6.0/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pre_commit_hooks
-version = 4.5.0
+version = 4.6.0
 description = Some out-of-the-box hooks for pre-commit.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/pre-commit/pre-commit-hooks
 author = Anthony Sottile
 author_email = asottile@umich.edu
 license = MIT
```

### Comparing `pre_commit_hooks-4.5.0/tests/tests_should_end_in_test_test.py` & `pre_commit_hooks-4.6.0/tests/tests_should_end_in_test_test.py`

 * *Files identical despite different names*

