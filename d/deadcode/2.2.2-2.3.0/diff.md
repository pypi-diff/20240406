# Comparing `tmp/deadcode-2.2.2.tar.gz` & `tmp/deadcode-2.3.0.tar.gz`

## Comparing `deadcode-2.2.2.tar` & `deadcode-2.3.0.tar`

### file list

```diff
@@ -1,67 +1,342 @@
--rw-r--r--   0        0        0     5549 2020-02-02 00:00:00.000000 deadcode-2.2.2/call_arg_map_to_parameters_poc.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 deadcode-2.2.2/deadcode/__init__.py
--rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 deadcode-2.2.2/deadcode/cli.py
--rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 deadcode-2.2.2/deadcode/constants.py
--rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 deadcode-2.2.2/deadcode/data_types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 deadcode-2.2.2/deadcode/actions/__init__.py
--rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 deadcode-2.2.2/deadcode/actions/find_python_filenames.py
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 deadcode-2.2.2/deadcode/actions/find_unused_names.py
--rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 deadcode-2.2.2/deadcode/actions/fix_unused_code.py
--rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 deadcode-2.2.2/deadcode/actions/get_unused_names_error_message.py
--rw-r--r--   0        0        0     3222 2020-02-02 00:00:00.000000 deadcode-2.2.2/deadcode/actions/merge_overlaping_file_parts.py
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 deadcode-2.2.2/deadcode/actions/parse_abstract_syntax_tree.py
--rw-r--r--   0        0        0     6453 2020-02-02 00:00:00.000000 deadcode-2.2.2/deadcode/actions/parse_arguments.py
--rw-r--r--   0        0        0     5692 2020-02-02 00:00:00.000000 deadcode-2.2.2/deadcode/actions/remove_file_parts_from_content.py
--rw-r--r--   0        0        0     3369 2020-02-02 00:00:00.000000 deadcode-2.2.2/deadcode/tests/base.py
--rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 deadcode-2.2.2/deadcode/tests/test_accurate_usage_detection.py
--rw-r--r--   0        0        0     2720 2020-02-02 00:00:00.000000 deadcode-2.2.2/deadcode/tests/test_deadcode.py
--rw-r--r--   0        0        0     3842 2020-02-02 00:00:00.000000 deadcode-2.2.2/deadcode/tests/test_imports.py
--rw-r--r--   0        0        0     2519 2020-02-02 00:00:00.000000 deadcode-2.2.2/deadcode/tests/test_line_number_detection.py
--rw-r--r--   0        0        0     4251 2020-02-02 00:00:00.000000 deadcode-2.2.2/deadcode/tests/test_output.py
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 deadcode-2.2.2/deadcode/tests/test_variable_parsing_from_ast_dump.py
--rw-r--r--   0        0        0     1492 2020-02-02 00:00:00.000000 deadcode-2.2.2/deadcode/tests/actions/test_find_python_filenames.py
--rw-r--r--   0        0        0     2296 2020-02-02 00:00:00.000000 deadcode-2.2.2/deadcode/tests/actions/test_merge_overlaping_file_parts.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 deadcode-2.2.2/deadcode/tests/cli_args/test_count.py
--rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 deadcode-2.2.2/deadcode/tests/cli_args/test_exclude.py
--rw-r--r--   0        0        0    12172 2020-02-02 00:00:00.000000 deadcode-2.2.2/deadcode/tests/cli_args/test_fix.py
--rw-r--r--   0        0        0     1380 2020-02-02 00:00:00.000000 deadcode-2.2.2/deadcode/tests/cli_args/test_ignore_bodies_if_inherits_from.py
--rw-r--r--   0        0        0     3404 2020-02-02 00:00:00.000000 deadcode-2.2.2/deadcode/tests/cli_args/test_ignore_definitions.py
--rw-r--r--   0        0        0     3555 2020-02-02 00:00:00.000000 deadcode-2.2.2/deadcode/tests/cli_args/test_ignore_definitions_if_inherits_from.py
--rw-r--r--   0        0        0     2443 2020-02-02 00:00:00.000000 deadcode-2.2.2/deadcode/tests/cli_args/test_ignore_names.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 deadcode-2.2.2/deadcode/tests/cli_args/test_ignore_names_in_files.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 deadcode-2.2.2/deadcode/tests/cli_args/test_no_color.py
--rw-r--r--   0        0        0     2609 2020-02-02 00:00:00.000000 deadcode-2.2.2/deadcode/tests/cli_args/test_parsing.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 deadcode-2.2.2/deadcode/tests/cli_args/test_quiet.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 deadcode-2.2.2/deadcode/tests/cli_args/test_verbose.py
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 deadcode-2.2.2/deadcode/tests/code_item/test_code_item.py
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 deadcode-2.2.2/deadcode/tests/files/classes.py
--rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 deadcode-2.2.2/deadcode/tests/files/functions.py
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 deadcode-2.2.2/deadcode/tests/files/variables.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 deadcode-2.2.2/deadcode/tests/files/subdir/one_more_file.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 deadcode-2.2.2/deadcode/tests/files/subdir/another_subdir/__init__.py
--rw-r--r--   0        0        0     2361 2020-02-02 00:00:00.000000 deadcode-2.2.2/deadcode/tests/fix/test_assign.py
--rw-r--r--   0        0        0     2897 2020-02-02 00:00:00.000000 deadcode-2.2.2/deadcode/tests/fix/test_class_def.py
--rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 deadcode-2.2.2/deadcode/tests/fix/test_empty_files.py
--rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 deadcode-2.2.2/deadcode/tests/fix/test_method_def.py
--rw-r--r--   0        0        0     6307 2020-02-02 00:00:00.000000 deadcode-2.2.2/deadcode/tests/fix/test_scope.py
--rw-r--r--   0        0        0     2565 2020-02-02 00:00:00.000000 deadcode-2.2.2/deadcode/tests/fix/test_unreachable_code.py
--rw-r--r--   0        0        0     1948 2020-02-02 00:00:00.000000 deadcode-2.2.2/deadcode/tests/nested_scope/test_nested_scope.py
--rw-r--r--   0        0        0     8219 2020-02-02 00:00:00.000000 deadcode-2.2.2/deadcode/tests/noqa/test_noqa_comments.py
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 deadcode-2.2.2/deadcode/tests/utils/test_fix_indent.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 deadcode-2.2.2/deadcode/utils/__init__.py
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 deadcode-2.2.2/deadcode/utils/fix_indent.py
--rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 deadcode-2.2.2/deadcode/utils/flatten_lists.py
--rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 deadcode-2.2.2/deadcode/utils/nested_scopes.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 deadcode-2.2.2/deadcode/utils/print_ast.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 deadcode-2.2.2/deadcode/visitor/__init__.py
--rw-r--r--   0        0        0     4410 2020-02-02 00:00:00.000000 deadcode-2.2.2/deadcode/visitor/code_item.py
--rw-r--r--   0        0        0    25082 2020-02-02 00:00:00.000000 deadcode-2.2.2/deadcode/visitor/dead_code_visitor.py
--rw-r--r--   0        0        0     3191 2020-02-02 00:00:00.000000 deadcode-2.2.2/deadcode/visitor/ignore.py
--rw-r--r--   0        0        0     3241 2020-02-02 00:00:00.000000 deadcode-2.2.2/deadcode/visitor/lines.py
--rw-r--r--   0        0        0     1760 2020-02-02 00:00:00.000000 deadcode-2.2.2/deadcode/visitor/noqa.py
--rw-r--r--   0        0        0     2765 2020-02-02 00:00:00.000000 deadcode-2.2.2/deadcode/visitor/utils.py
--rw-r--r--   0        0        0     3106 2020-02-02 00:00:00.000000 deadcode-2.2.2/.gitignore
--rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 deadcode-2.2.2/LICENSE
--rw-r--r--   0        0        0     7072 2020-02-02 00:00:00.000000 deadcode-2.2.2/README.md
--rw-r--r--   0        0        0     1991 2020-02-02 00:00:00.000000 deadcode-2.2.2/pyproject.toml
--rw-r--r--   0        0        0     7903 2020-02-02 00:00:00.000000 deadcode-2.2.2/PKG-INFO
+-rw-r--r--   0        0        0     5546 2020-02-02 00:00:00.000000 deadcode-2.3.0/call_arg_map_to_parameters_poc.py
+-rw-r--r--   0        0        0     5373 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/action/main.py
+-rw-r--r--   0        0        0     6841 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/docs/conf.py
+-rwxr-xr-x   0        0        0     9105 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/gallery/gallery.py
+-rw-r--r--   0        0        0   215971 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/profiling/dict_big.py
+-rw-r--r--   0        0        0  1118824 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/profiling/dict_huge.py
+-rw-r--r--   0        0        0   159994 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/profiling/list_big.py
+-rw-r--r--   0        0        0   897234 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/profiling/list_huge.py
+-rw-r--r--   0        0        0   184224 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/profiling/mix_big.py
+-rw-r--r--   0        0        0  1406108 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/profiling/mix_huge.py
+-rw-r--r--   0        0        0    18306 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/profiling/mix_small.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/scripts/__init__.py
+-rw-r--r--   0        0        0     1863 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/scripts/check_pre_commit_rev_in_example.py
+-rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/scripts/check_version_in_basics_example.py
+-rw-r--r--   0        0        0     8987 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/scripts/diff_shades_gha_helper.py
+-rw-r--r--   0        0        0     3553 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/scripts/fuzz.py
+-rwxr-xr-x   0        0        0     2381 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/scripts/generate_schema.py
+-rw-r--r--   0        0        0     2358 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/scripts/make_width_table.py
+-rwxr-xr-x   0        0        0     2987 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/scripts/migrate-black.py
+-rwxr-xr-x   0        0        0     7496 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/scripts/release.py
+-rw-r--r--   0        0        0     2321 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/scripts/release_tests.py
+-rw-r--r--   0        0        0    51975 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/src/black/__init__.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/src/black/__main__.py
+-rw-r--r--   0        0        0    10761 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/src/black/_width_table.py
+-rw-r--r--   0        0        0    12426 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/src/black/brackets.py
+-rw-r--r--   0        0        0     4835 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/src/black/cache.py
+-rw-r--r--   0        0        0    15983 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/src/black/comments.py
+-rw-r--r--   0        0        0     6410 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/src/black/concurrency.py
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/src/black/const.py
+-rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/src/black/debug.py
+-rw-r--r--   0        0        0    14665 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/src/black/files.py
+-rw-r--r--   0        0        0    13364 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/src/black/handle_ipynb_magics.py
+-rw-r--r--   0        0        0    67512 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/src/black/linegen.py
+-rw-r--r--   0        0        0    39349 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/src/black/lines.py
+-rw-r--r--   0        0        0     8500 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/src/black/mode.py
+-rw-r--r--   0        0        0    28915 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/src/black/nodes.py
+-rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/src/black/numerics.py
+-rw-r--r--   0        0        0     3939 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/src/black/output.py
+-rw-r--r--   0        0        0     8428 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/src/black/parsing.py
+-rw-r--r--   0        0        0    19695 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/src/black/ranges.py
+-rw-r--r--   0        0        0     3452 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/src/black/report.py
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/src/black/rusty.py
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/src/black/schema.py
+-rw-r--r--   0        0        0    10933 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/src/black/strings.py
+-rw-r--r--   0        0        0    95476 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/src/black/trans.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/src/black/resources/__init__.py
+-rw-r--r--   0        0        0     8867 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/src/blackd/__init__.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/src/blackd/__main__.py
+-rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/src/blackd/middlewares.py
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/src/blib2to3/__init__.py
+-rw-r--r--   0        0        0     4810 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/src/blib2to3/pygram.py
+-rw-r--r--   0        0        0    32666 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/src/blib2to3/pytree.py
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/src/blib2to3/pgen2/__init__.py
+-rw-r--r--   0        0        0     9587 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/src/blib2to3/pgen2/conv.py
+-rw-r--r--   0        0        0    10631 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/src/blib2to3/pgen2/driver.py
+-rw-r--r--   0        0        0     6858 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/src/blib2to3/pgen2/grammar.py
+-rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/src/blib2to3/pgen2/literals.py
+-rw-r--r--   0        0        0    15658 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/src/blib2to3/pgen2/parse.py
+-rw-r--r--   0        0        0    15428 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/src/blib2to3/pgen2/pgen.py
+-rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/src/blib2to3/pgen2/token.py
+-rw-r--r--   0        0        0    23006 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/src/blib2to3/pgen2/tokenize.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/__init__.py
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/conftest.py
+-rw-r--r--   0        0        0     4530 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/optional.py
+-rw-r--r--   0        0        0   118890 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/test_black.py
+-rw-r--r--   0        0        0     9375 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/test_blackd.py
+-rw-r--r--   0        0        0     2531 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/test_docs.py
+-rw-r--r--   0        0        0     2683 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/test_format.py
+-rw-r--r--   0        0        0    16073 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/test_ipynb.py
+-rw-r--r--   0        0        0     1247 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/test_no_ipynb.py
+-rw-r--r--   0        0        0     4538 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/test_ranges.py
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/test_schema.py
+-rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/test_trans.py
+-rw-r--r--   0        0        0    12198 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/util.py
+-rw-r--r--   0        0        0     1794 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/allow_empty_first_line.py
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/async_stmts.py
+-rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/attribute_access_on_number_literals.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/beginning_backslash.py
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/bracketmatch.py
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/bytes_docstring.py
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/class_blank_parentheses.py
+-rw-r--r--   0        0        0     4318 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/class_methods_new_line.py
+-rw-r--r--   0        0        0     3294 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/collections.py
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/comment_after_escaped_newline.py
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/comment_type_hint.py
+-rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/comments.py
+-rw-r--r--   0        0        0     7640 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/comments2.py
+-rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/comments3.py
+-rw-r--r--   0        0        0     3532 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/comments4.py
+-rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/comments5.py
+-rw-r--r--   0        0        0     2479 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/comments6.py
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/comments8.py
+-rw-r--r--   0        0        0     5279 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/comments9.py
+-rw-r--r--   0        0        0     2150 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/comments_in_blocks.py
+-rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/comments_in_double_parens.py
+-rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/comments_non_breaking_space.py
+-rw-r--r--   0        0        0     5596 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/composition.py
+-rw-r--r--   0        0        0    11196 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/composition_no_trailing_comma.py
+-rw-r--r--   0        0        0     4910 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/conditional_expression.py
+-rw-r--r--   0        0        0     1171 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/context_managers_38.py
+-rw-r--r--   0        0        0     3392 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/context_managers_39.py
+-rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/context_managers_autodetect_310.py
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/context_managers_autodetect_311.py
+-rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/context_managers_autodetect_38.py
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/context_managers_autodetect_39.py
+-rw-r--r--   0        0        0     7978 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/docstring.py
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/docstring_newline_preview.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/docstring_no_extra_empty_line_before_eof.py
+-rw-r--r--   0        0        0     3638 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/docstring_no_string_normalization.py
+-rw-r--r--   0        0        0     3518 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/docstring_preview.py
+-rw-r--r--   0        0        0     2247 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/dummy_implementations.py
+-rw-r--r--   0        0        0     4597 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/empty_lines.py
+-rw-r--r--   0        0        0    18624 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/expression.py
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/f_docstring.py
+-rw-r--r--   0        0        0     9635 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/fmtonoff.py
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/fmtonoff2.py
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/fmtonoff3.py
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/fmtonoff4.py
+-rw-r--r--   0        0        0     3619 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/fmtonoff5.py
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/fmtpass_imports.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/fmtskip.py
+-rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/fmtskip2.py
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/fmtskip3.py
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/fmtskip4.py
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/fmtskip5.py
+-rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/fmtskip6.py
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/fmtskip7.py
+-rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/fmtskip8.py
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/fmtskip9.py
+-rw-r--r--   0        0        0     1932 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/form_feeds.py
+-rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/fstring.py
+-rw-r--r--   0        0        0     5786 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/funcdef_return_type_trailing_comma.py
+-rw-r--r--   0        0        0     6408 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/function.py
+-rw-r--r--   0        0        0     2419 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/function2.py
+-rw-r--r--   0        0        0     3605 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/function_trailing_comma.py
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/ignore_pyi.py
+-rw-r--r--   0        0        0     2542 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/import_spacing.py
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/is_simple_lookup_for_doublestar_expression.py
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/keep_newline_after_match.py
+-rw-r--r--   0        0        0     3519 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/line_ranges_basic.py
+-rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/line_ranges_diff_edge_case.py
+-rw-r--r--   0        0        0     1276 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/line_ranges_exceeding_end.py
+-rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/line_ranges_fmt_off.py
+-rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/line_ranges_fmt_off_decorator.py
+-rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/line_ranges_fmt_off_overlap.py
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/line_ranges_imports.py
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/line_ranges_indentation.py
+-rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/line_ranges_outside_source.py
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/line_ranges_two_passes.py
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/line_ranges_unwrapping.py
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/linelength6.py
+-rw-r--r--   0        0        0    11608 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/long_strings_flag_disabled.py
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/module_docstring_1.py
+-rw-r--r--   0        0        0     2252 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/module_docstring_2.py
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/module_docstring_3.py
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/module_docstring_4.py
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/module_docstring_followed_by_class.py
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/module_docstring_followed_by_function.py
+-rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/multiline_consecutive_open_parentheses_ignore.py
+-rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/nested_stub.py
+-rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/no_blank_line_before_docstring.py
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/numeric_literals.py
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/numeric_literals_skip_underscores.py
+-rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/one_element_subscript.py
+-rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/parenthesized_context_managers.py
+-rw-r--r--   0        0        0     2965 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/pattern_matching_complex.py
+-rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/pattern_matching_extras.py
+-rw-r--r--   0        0        0     3098 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/pattern_matching_generic.py
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/pattern_matching_long.py
+-rw-r--r--   0        0        0     2673 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/pattern_matching_simple.py
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/pattern_matching_style.py
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/pattern_matching_trailing_comma.py
+-rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/pattern_matching_with_if_stmt.py
+-rw-r--r--   0        0        0     4689 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/pep604_union_types_line_breaks.py
+-rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/pep_570.py
+-rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/pep_572.py
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/pep_572_do_not_remove_parens.py
+-rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/pep_572_py310.py
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/pep_572_py39.py
+-rw-r--r--   0        0        0     1919 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/pep_572_remove_parens.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/pep_572_slices.py
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/pep_604.py
+-rw-r--r--   0        0        0     2146 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/pep_646.py
+-rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/pep_654.py
+-rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/pep_654_style.py
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/percent_precedence.py
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/power_op_newline.py
+-rw-r--r--   0        0        0     3533 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/power_op_spacing.py
+-rw-r--r--   0        0        0     2500 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/power_op_spacing_long.py
+-rw-r--r--   0        0        0     3270 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/prefer_rhs_split.py
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/prefer_rhs_split_reformatted.py
+-rw-r--r--   0        0        0     3328 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/preview_cantfit.py
+-rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/preview_cantfit_string.py
+-rw-r--r--   0        0        0     8996 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/preview_comments7.py
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/preview_format_unicode_escape_seq.py
+-rw-r--r--   0        0        0     5823 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/preview_hug_parens_with_braces_and_square_brackets.py
+-rw-r--r--   0        0        0     4093 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/preview_hug_parens_with_braces_and_square_brackets_no_ll1.py
+-rw-r--r--   0        0        0     3982 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/preview_long_dict_values.py
+-rw-r--r--   0        0        0    36538 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/preview_long_strings.py
+-rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/preview_long_strings__east_asian_width.py
+-rw-r--r--   0        0        0     6556 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/preview_long_strings__edge_case.py
+-rw-r--r--   0        0        0    45834 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/preview_long_strings__regression.py
+-rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/preview_long_strings__type_annotations.py
+-rw-r--r--   0        0        0     7861 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/preview_multiline_strings.py
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/preview_return_annotation_brackets_string.py
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/py310_pep572.py
+-rw-r--r--   0        0        0     1178 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/python37.py
+-rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/python38.py
+-rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/python39.py
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/raw_docstring.py
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/raw_docstring_no_string_normalization.py
+-rw-r--r--   0        0        0     3538 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/remove_await_parens.py
+-rw-r--r--   0        0        0     2025 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/remove_except_parens.py
+-rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/remove_for_brackets.py
+-rw-r--r--   0        0        0     3218 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/remove_newline_after_code_block_open.py
+-rw-r--r--   0        0        0     3493 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/remove_parens.py
+-rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/remove_redundant_parens_in_case_guard.py
+-rw-r--r--   0        0        0     2606 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/remove_with_brackets.py
+-rw-r--r--   0        0        0     5207 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/return_annotation_brackets.py
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/single_line_format_skip_with_multiple_comments.py
+-rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/skip_magic_trailing_comma.py
+-rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/slices.py
+-rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/split_delimiter_comments.py
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/starred_for_target.py
+-rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/string_prefixes.py
+-rw-r--r--   0        0        0     2281 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/stub.py
+-rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/torture.py
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/trailing_comma.py
+-rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/trailing_comma_optional_parens1.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/trailing_comma_optional_parens2.py
+-rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/trailing_comma_optional_parens3.py
+-rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/trailing_commas_in_leading_parts.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/tricky_unicode_symbols.py
+-rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/tupleassign.py
+-rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/type_aliases.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/type_comment_syntax_error.py
+-rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/type_params.py
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/typed_params_trailing_comma.py
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/walrus_in_dict.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/cases/whitespace.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/gitignore_used_on_multiple_sources/dir1/a.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/gitignore_used_on_multiple_sources/dir1/b.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/gitignore_used_on_multiple_sources/dir2/a.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/gitignore_used_on_multiple_sources/dir2/b.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/ignore_subfolders_gitignore_tests/a.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/ignore_subfolders_gitignore_tests/subdir/b.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/ignore_subfolders_gitignore_tests/subdir/subdir/c.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/include_exclude_tests/b/.definitely_exclude/a.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/include_exclude_tests/b/dont_exclude/a.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/include_exclude_tests/b/exclude/a.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/invalid_gitignore_tests/a.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/invalid_nested_gitignore_tests/a.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/invalid_nested_gitignore_tests/a/a.py
+-rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/line_ranges_formatted/basic.py
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/line_ranges_formatted/pattern_matching.py
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/miscellaneous/async_as_identifier.py
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/miscellaneous/blackd_diff.py
+-rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/miscellaneous/debug_visitor.py
+-rw-r--r--   0        0        0     1774 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/miscellaneous/decorators.py
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/miscellaneous/force_py36.py
+-rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/miscellaneous/force_pyi.py
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/miscellaneous/invalid_header.py
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/miscellaneous/missing_final_newline.py
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/miscellaneous/pattern_matching_invalid.py
+-rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/miscellaneous/python2_detection.py
+-rw-r--r--   0        0        0     2363 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/miscellaneous/string_quotes.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/nested_gitignore_tests/x.py
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/nested_gitignore_tests/root/a.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/nested_gitignore_tests/root/b.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/nested_gitignore_tests/root/c.py
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/nested_gitignore_tests/root/child/a.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/nested_gitignore_tests/root/child/b.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 deadcode-2.3.0/black/tests/data/nested_gitignore_tests/root/child/c.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 deadcode-2.3.0/deadcode/__init__.py
+-rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 deadcode-2.3.0/deadcode/cli.py
+-rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 deadcode-2.3.0/deadcode/constants.py
+-rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 deadcode-2.3.0/deadcode/data_types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 deadcode-2.3.0/deadcode/actions/__init__.py
+-rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 deadcode-2.3.0/deadcode/actions/find_python_filenames.py
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 deadcode-2.3.0/deadcode/actions/find_unused_names.py
+-rw-r--r--   0        0        0     2577 2020-02-02 00:00:00.000000 deadcode-2.3.0/deadcode/actions/fix_or_show_unused_code.py
+-rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 deadcode-2.3.0/deadcode/actions/get_unused_names_error_message.py
+-rw-r--r--   0        0        0     3222 2020-02-02 00:00:00.000000 deadcode-2.3.0/deadcode/actions/merge_overlaping_file_parts.py
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 deadcode-2.3.0/deadcode/actions/parse_abstract_syntax_tree.py
+-rw-r--r--   0        0        0     6955 2020-02-02 00:00:00.000000 deadcode-2.3.0/deadcode/actions/parse_arguments.py
+-rw-r--r--   0        0        0     5692 2020-02-02 00:00:00.000000 deadcode-2.3.0/deadcode/actions/remove_file_parts_from_content.py
+-rw-r--r--   0        0        0     3385 2020-02-02 00:00:00.000000 deadcode-2.3.0/deadcode/tests/base.py
+-rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 deadcode-2.3.0/deadcode/tests/test_accurate_usage_detection.py
+-rw-r--r--   0        0        0     2709 2020-02-02 00:00:00.000000 deadcode-2.3.0/deadcode/tests/test_deadcode.py
+-rw-r--r--   0        0        0     3839 2020-02-02 00:00:00.000000 deadcode-2.3.0/deadcode/tests/test_imports.py
+-rw-r--r--   0        0        0     2519 2020-02-02 00:00:00.000000 deadcode-2.3.0/deadcode/tests/test_line_number_detection.py
+-rw-r--r--   0        0        0     4245 2020-02-02 00:00:00.000000 deadcode-2.3.0/deadcode/tests/test_output.py
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 deadcode-2.3.0/deadcode/tests/test_variable_parsing_from_ast_dump.py
+-rw-r--r--   0        0        0     1492 2020-02-02 00:00:00.000000 deadcode-2.3.0/deadcode/tests/actions/test_find_python_filenames.py
+-rw-r--r--   0        0        0     2296 2020-02-02 00:00:00.000000 deadcode-2.3.0/deadcode/tests/actions/test_merge_overlaping_file_parts.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 deadcode-2.3.0/deadcode/tests/cli_args/test_count.py
+-rw-r--r--   0        0        0     8865 2020-02-02 00:00:00.000000 deadcode-2.3.0/deadcode/tests/cli_args/test_dry.py
+-rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 deadcode-2.3.0/deadcode/tests/cli_args/test_exclude.py
+-rw-r--r--   0        0        0    12167 2020-02-02 00:00:00.000000 deadcode-2.3.0/deadcode/tests/cli_args/test_fix.py
+-rw-r--r--   0        0        0     1377 2020-02-02 00:00:00.000000 deadcode-2.3.0/deadcode/tests/cli_args/test_ignore_bodies_if_inherits_from.py
+-rw-r--r--   0        0        0     3403 2020-02-02 00:00:00.000000 deadcode-2.3.0/deadcode/tests/cli_args/test_ignore_definitions.py
+-rw-r--r--   0        0        0     3551 2020-02-02 00:00:00.000000 deadcode-2.3.0/deadcode/tests/cli_args/test_ignore_definitions_if_inherits_from.py
+-rw-r--r--   0        0        0     2440 2020-02-02 00:00:00.000000 deadcode-2.3.0/deadcode/tests/cli_args/test_ignore_names.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 deadcode-2.3.0/deadcode/tests/cli_args/test_ignore_names_in_files.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 deadcode-2.3.0/deadcode/tests/cli_args/test_no_color.py
+-rw-r--r--   0        0        0     4477 2020-02-02 00:00:00.000000 deadcode-2.3.0/deadcode/tests/cli_args/test_parsing.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 deadcode-2.3.0/deadcode/tests/cli_args/test_quiet.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 deadcode-2.3.0/deadcode/tests/cli_args/test_verbose.py
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 deadcode-2.3.0/deadcode/tests/code_item/test_code_item.py
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 deadcode-2.3.0/deadcode/tests/files/classes.py
+-rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 deadcode-2.3.0/deadcode/tests/files/functions.py
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 deadcode-2.3.0/deadcode/tests/files/variables.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 deadcode-2.3.0/deadcode/tests/files/subdir/one_more_file.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 deadcode-2.3.0/deadcode/tests/files/subdir/another_subdir/__init__.py
+-rw-r--r--   0        0        0     2359 2020-02-02 00:00:00.000000 deadcode-2.3.0/deadcode/tests/fix/test_assign.py
+-rw-r--r--   0        0        0     2893 2020-02-02 00:00:00.000000 deadcode-2.3.0/deadcode/tests/fix/test_class_def.py
+-rw-r--r--   0        0        0      933 2020-02-02 00:00:00.000000 deadcode-2.3.0/deadcode/tests/fix/test_empty_files.py
+-rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 deadcode-2.3.0/deadcode/tests/fix/test_method_def.py
+-rw-r--r--   0        0        0     6307 2020-02-02 00:00:00.000000 deadcode-2.3.0/deadcode/tests/fix/test_scope.py
+-rw-r--r--   0        0        0     2565 2020-02-02 00:00:00.000000 deadcode-2.3.0/deadcode/tests/fix/test_unreachable_code.py
+-rw-r--r--   0        0        0     4359 2020-02-02 00:00:00.000000 deadcode-2.3.0/deadcode/tests/nested_scope/test_nested_scope.py
+-rw-r--r--   0        0        0     8191 2020-02-02 00:00:00.000000 deadcode-2.3.0/deadcode/tests/noqa/test_noqa_comments.py
+-rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 deadcode-2.3.0/deadcode/tests/utils/test_add_colors_to_diff.py
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 deadcode-2.3.0/deadcode/tests/utils/test_fix_indent.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 deadcode-2.3.0/deadcode/utils/__init__.py
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 deadcode-2.3.0/deadcode/utils/add_colors_to_diff.py
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 deadcode-2.3.0/deadcode/utils/fix_indent.py
+-rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 deadcode-2.3.0/deadcode/utils/flatten_lists.py
+-rw-r--r--   0        0        0     3467 2020-02-02 00:00:00.000000 deadcode-2.3.0/deadcode/utils/nested_scopes.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 deadcode-2.3.0/deadcode/utils/print_ast.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 deadcode-2.3.0/deadcode/visitor/__init__.py
+-rw-r--r--   0        0        0     4514 2020-02-02 00:00:00.000000 deadcode-2.3.0/deadcode/visitor/code_item.py
+-rw-r--r--   0        0        0    21285 2020-02-02 00:00:00.000000 deadcode-2.3.0/deadcode/visitor/dead_code_visitor.py
+-rw-r--r--   0        0        0     3179 2020-02-02 00:00:00.000000 deadcode-2.3.0/deadcode/visitor/ignore.py
+-rw-r--r--   0        0        0     3241 2020-02-02 00:00:00.000000 deadcode-2.3.0/deadcode/visitor/lines.py
+-rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 deadcode-2.3.0/deadcode/visitor/noqa.py
+-rw-r--r--   0        0        0     2765 2020-02-02 00:00:00.000000 deadcode-2.3.0/deadcode/visitor/utils.py
+-rw-r--r--   0        0        0     3106 2020-02-02 00:00:00.000000 deadcode-2.3.0/.gitignore
+-rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 deadcode-2.3.0/LICENSE
+-rw-r--r--   0        0        0     9882 2020-02-02 00:00:00.000000 deadcode-2.3.0/README.md
+-rw-r--r--   0        0        0     2092 2020-02-02 00:00:00.000000 deadcode-2.3.0/pyproject.toml
+-rw-r--r--   0        0        0    10713 2020-02-02 00:00:00.000000 deadcode-2.3.0/PKG-INFO
```

### Comparing `deadcode-2.2.2/call_arg_map_to_parameters_poc.py` & `deadcode-2.3.0/call_arg_map_to_parameters_poc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 '''
-DeadCode PEP1:  Make usage tracking more precise. 
+DeadCode PEP1:  Make usage tracking more precise.
 
     Problem statement:
         A variable name has to be unique in a whole code base in order to make detect its usage properly.
         When the variable with the same name is defined several times a different approach has to be taken into account
         Variable definitoin scope has to be tracked.
         When the usage is being detected, the scope of the used variable has to be correctly identified.
 
@@ -21,15 +21,15 @@
 
         Feature request:
             Build local scopes of defined variables (available classes).
 
             During instantiation track the type of the variable and mark the usages of those classes.
 
         Feature request:
-            For invocation: resolve which arguments were converted into which parameters. 
+            For invocation: resolve which arguments were converted into which parameters.
 
         Feature request:
             When a variable value is being assigned, the type of value has to be tracked.
                 Which class usages have to registered, when instance attributes are being used?
 
         Insight:
             The data structure for storing used code items should be built by scope, instead of a common pool of names.
@@ -43,15 +43,15 @@
         for every invocation: compile mapping from invocation arguments to parameters map
             update invocation argument usage based on function parameter usage map.
 
 
 
         When an instance is being assigned: its type have to be assigned.
 
-        on instance creation: its type has to be assigned to 
+        on instance creation: its type has to be assigned to
 
 
 '''
 
 
 ### Parsed of ast:
 # Module(
```

### Comparing `deadcode-2.2.2/deadcode/cli.py` & `deadcode-2.3.0/deadcode/cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import List, Optional
 
 from deadcode.actions.find_python_filenames import find_python_filenames
 from deadcode.actions.find_unused_names import find_unused_names
-from deadcode.actions.fix_unused_code import fix_unused_code
+from deadcode.actions.fix_or_show_unused_code import fix_or_show_unused_code
 from deadcode.actions.parse_arguments import parse_arguments
 from deadcode.actions.get_unused_names_error_message import (
     get_unused_names_error_message,
 )
 
 
 def main(
@@ -15,19 +15,20 @@
     args = parse_arguments(command_line_args)
 
     filenames = find_python_filenames(args=args)
 
     # TODO: rename unused_names to unused_code_items
     unused_names = find_unused_names(filenames=filenames, args=args)
 
-    if args.fix and unused_names:
-        fix_unused_code(unused_names)
+    file_diff = None
+    if (args.fix or args.dry) and unused_names:
+        file_diff = fix_or_show_unused_code(unused_names, args=args)
 
     if (error_message := get_unused_names_error_message(unused_names, args=args)) is not None:
-        return error_message
+        return error_message + ("\n\n" + file_diff if file_diff else "")
 
     if not args.count and not args.quiet:
         print("\033[1mWell done!\033[0m ✨ 🚀 ✨")
     return None
 
 
 if __name__ == "__main__":
```

### Comparing `deadcode-2.2.2/deadcode/constants.py` & `deadcode-2.3.0/deadcode/constants.py`

 * *Files 19% similar despite different names*

```diff
@@ -14,36 +14,36 @@
     "unused_file",
     "commented_out_code",
     "ignore_expression",
 ]
 
 
 UnusedCodeErrorCode = Literal[
-    "DC001",
-    "DC002",
-    "DC003",
-    "DC004",
-    "DC005",
-    "DC006",
-    "DC007",
-    "DC008",
-    "DC009",
-    "DC011",
-    "DC012",
-    "DC013",
+    "DC01",
+    "DC02",
+    "DC03",
+    "DC04",
+    "DC05",
+    "DC06",
+    "DC07",
+    "DC08",
+    "DC09",
+    "DC11",
+    "DC12",
+    "DC13",
 ]
 
 
 ERROR_TYPE_TO_ERROR_CODE: Dict[UnusedCodeType, UnusedCodeErrorCode] = {
-    "variable": "DC001",
-    "function": "DC002",
-    "class": "DC003",
-    "method": "DC004",
-    "attribute": "DC005",
-    "name": "DC006",
-    "import": "DC007",
-    "property": "DC008",
-    "unreachable_code": "DC009",
-    "unused_file": "DC011",
-    "commented_out_code": "DC012",
-    "ignore_expression": "DC013",
+    "variable": "DC01",
+    "function": "DC02",
+    "class": "DC03",
+    "method": "DC04",
+    "attribute": "DC05",
+    "name": "DC06",
+    "import": "DC07",
+    "property": "DC08",
+    "unreachable_code": "DC09",
+    "unused_file": "DC11",
+    "commented_out_code": "DC12",
+    "ignore_expression": "DC13",
 }
```

### Comparing `deadcode-2.2.2/deadcode/data_types.py` & `deadcode-2.3.0/deadcode/data_types.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 Pathname = str  # Can contain wildewards
 
 
 @dataclass
 class Args:
     fix: bool = False
     verbose: bool = False
+    dry: Iterable[Pathname] = ()
     paths: Iterable[Pathname] = ()
     exclude: Iterable[Pathname] = ()
     ignore_definitions: Iterable[Pathname] = ()
     ignore_definitions_if_decorated_with: Iterable[Pathname] = ()
     ignore_definitions_if_inherits_from: Iterable[Pathname] = ()
     ignore_bodies_of: Iterable[Pathname] = ()
     ignore_bodies_if_decorated_with: Iterable[Pathname] = ()
```

### Comparing `deadcode-2.2.2/deadcode/actions/find_python_filenames.py` & `deadcode-2.3.0/deadcode/actions/find_python_filenames.py`

 * *Files identical despite different names*

### Comparing `deadcode-2.2.2/deadcode/actions/fix_unused_code.py` & `deadcode-2.3.0/deadcode/actions/fix_or_show_unused_code.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,43 +1,64 @@
 from collections import defaultdict
+from difflib import unified_diff
 from typing import Iterable
 import os
 
 from deadcode.actions.merge_overlaping_file_parts import merge_overlaping_file_parts
 from deadcode.actions.remove_file_parts_from_content import remove_file_parts_from_content
+from deadcode.data_types import Args
 from deadcode.visitor.code_item import CodeItem
 from deadcode.utils.flatten_lists import flatten_list
+from deadcode.utils.add_colors_to_diff import add_colors_to_diff
+from deadcode.visitor.ignore import _match
 
 
-def fix_unused_code(unused_items: Iterable[CodeItem]) -> None:
+def fix_or_show_unused_code(unused_items: Iterable[CodeItem], args: Args) -> str:
     # Reading and writing should be patched in this file.
 
     # Group unused_names by filenames
     # For each filename find file parts, which have to be fixed.
     # And fix those file parts.
     #
     # TODO: trailing commas, trailing white spaces and empty lines
 
     filename_to_unused_items = defaultdict(list)
     for unused_item in unused_items:
         filename_to_unused_items[str(unused_item.filename)].append(unused_item)
 
+    result = []
+
     for filename, unused_items in filename_to_unused_items.items():
         file_parts = flatten_list([item.code_parts for item in unused_items])
 
         unused_file_parts = merge_overlaping_file_parts(file_parts)
 
         with open(filename) as f:
             file_content_lines = f.readlines()
 
         updated_file_content_lines = remove_file_parts_from_content(file_content_lines, unused_file_parts)
         updated_file_content = "".join(updated_file_content_lines)
         if updated_file_content.strip():
-            with open(filename, "w") as f:
-                # TODO: is there a method writelines?
-                f.write(updated_file_content)
+            if args.dry and ("__all_files__" in args.dry or _match(filename, args.dry)):
+                with open(filename, "r") as f:
+                    diff = unified_diff(f.readlines(), updated_file_content_lines, fromfile=filename, tofile=filename)
+                    # TODO: consider printing result instantly to save memory
+                    diff_str = "".join(diff)
+                    if args.no_color:
+                        result.append(diff_str)
+                    else:
+                        result.append(add_colors_to_diff(diff_str))
+
+            elif args.fix:
+                with open(filename, "w") as f:
+                    # TODO: is there a method writelines?
+                    f.write(updated_file_content)
         else:
             os.remove(filename)
 
+    if result:
+        return "\n".join(result)
+    return ""
+
     # TODO: update this one: solution is to use read and write operations.
     #
     # Solution is to open file for reading and then for writing.
```

### Comparing `deadcode-2.2.2/deadcode/actions/get_unused_names_error_message.py` & `deadcode-2.3.0/deadcode/actions/get_unused_names_error_message.py`

 * *Files identical despite different names*

### Comparing `deadcode-2.2.2/deadcode/actions/merge_overlaping_file_parts.py` & `deadcode-2.3.0/deadcode/actions/merge_overlaping_file_parts.py`

 * *Files identical despite different names*

### Comparing `deadcode-2.2.2/deadcode/actions/parse_abstract_syntax_tree.py` & `deadcode-2.3.0/deadcode/actions/parse_abstract_syntax_tree.py`

 * *Files identical despite different names*

### Comparing `deadcode-2.2.2/deadcode/actions/parse_arguments.py` & `deadcode-2.3.0/deadcode/actions/parse_arguments.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,21 +29,21 @@
     parser.add_argument("paths", help="Paths where to search for python files", nargs="+")
     parser.add_argument(
         "--fix",
         help="Automatically remove detected unused code expressions from the code base.",
         action="store_true",
         default=False,
     )
-
     parser.add_argument(
-        "-v",
-        "--verbose",
-        help="Shows logs useful for debuging",
-        action="store_true",
-        default=False,
+        "--dry",
+        help="Show changes which would be made in files with --fix option.",
+        nargs="*",
+        action="append",
+        default=[["__all_files__"]],
+        type=str,
     )
     parser.add_argument(
         "--exclude",
         help="Filenames (or path expressions), which will be completely skipped without being analysed.",
         nargs="*",
         action="append",
         default=[],
@@ -156,44 +156,62 @@
         "--ignore-names-in-files",
         help="Ignores unused names in files, which filenames match provided path expressions.",
         nargs="*",
         action="append",
         default=[],
         type=str,
     )
+
     parser.add_argument(
         "--no-color",
         help="Turn off colors in the output",
         action="store_true",
         default=False,
     )
+
     parser.add_argument(
         "--quiet",
         help="Does not output anything. Makefile still fails with exit code 1 if unused names are found.",
         action="store_true",
         default=False,
     )
+
     parser.add_argument(
         "--count",
         help="Provides the count of the detected unused names instead of printing them all out.",
         action="store_true",
         default=False,
     )
+    parser.add_argument(
+        "-v",
+        "--verbose",
+        help="Shows logs useful for debuging",
+        action="store_true",
+        default=False,
+    )
 
     parsed_args = parser.parse_args(args).__dict__
 
     for arg_name, arg_value in parsed_args.items():
         if isinstance(arg_value, list) and arg_name != "paths":
             parsed_args[arg_name] = flatten_lists_of_comma_separated_values(parsed_args.get(arg_name))
 
     # Extend the Args with the values provided in the pyproject.toml
     for key, item in parse_pyproject_toml().items():
         if key in parsed_args:
             parsed_args[key].extend(item)
 
+    # Show changes for only provided files instead of all
+    if len(parsed_args["dry"]) > 1 or "--dry" not in args:
+        parsed_args["dry"].remove("__all_files__")
+
+    # Do not fix if dry option is provided:
+    if parsed_args["dry"]:
+        parsed_args["fix"] = False
+
     return Args(**parsed_args)
 
 
 def parse_pyproject_toml() -> Dict[str, Any]:
     """Parse a pyproject toml file, pulling out relevant parts for Black.
 
     If parsing fails, will raise a tomllib.TOMLDecodeError.
```

### Comparing `deadcode-2.2.2/deadcode/actions/remove_file_parts_from_content.py` & `deadcode-2.3.0/deadcode/actions/remove_file_parts_from_content.py`

 * *Files identical despite different names*

### Comparing `deadcode-2.2.2/deadcode/tests/base.py` & `deadcode-2.3.0/deadcode/tests/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,18 +39,18 @@
 
         self.find_python_filenames_mock = self.patch("deadcode.cli.find_python_filenames")
         self.find_python_filenames_mock.side_effect = self._get_filenames
 
         self.read_file_mock = self.patch("deadcode.visitor.dead_code_visitor.open")
         self.read_file_mock.side_effect = self._read_file_side_effect
 
-        self.fix_file_mock = self.patch("deadcode.actions.fix_unused_code.open")
+        self.fix_file_mock = self.patch("deadcode.actions.fix_or_show_unused_code.open")
         self.fix_file_mock.side_effect = self._read_file_side_effect
 
-        self.os_remove = self.patch("deadcode.actions.fix_unused_code.os.remove")
+        self.os_remove = self.patch("deadcode.actions.fix_or_show_unused_code.os.remove")
 
         self.args = Args()
 
     def assertFiles(self, files: Dict[str, str], removed: List[str] = None):
         expected_removed_files = removed
         expected_files = files
```

### Comparing `deadcode-2.2.2/deadcode/tests/test_accurate_usage_detection.py` & `deadcode-2.3.0/deadcode/tests/test_accurate_usage_detection.py`

 * *Files identical despite different names*

### Comparing `deadcode-2.2.2/deadcode/tests/test_deadcode.py` & `deadcode-2.3.0/deadcode/tests/test_deadcode.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,59 +7,59 @@
 class DeadCodeIntegrationTests(TestCase):
     def test_unused_variable_name_found_successfully(self):
         unused_names = main(["tests/files/variables.py", "--no-color"])
 
         self.assertEqual(
             unused_names,
             (
-                "tests/files/variables.py:1:0: DC001 Variable `unused_global_variable` is never used\n"
-                "tests/files/variables.py:3:0: DC001 Variable `ANOTHER_GLOBAL_VARIABLE` is never used\n"
-                "tests/files/variables.py:5:0: DC001 Variable `third_global_varialbe` is never used"
+                "tests/files/variables.py:1:0: DC01 Variable `unused_global_variable` is never used\n"
+                "tests/files/variables.py:3:0: DC01 Variable `ANOTHER_GLOBAL_VARIABLE` is never used\n"
+                "tests/files/variables.py:5:0: DC01 Variable `third_global_varialbe` is never used"
             ),
         )
 
     def test_unused_function_name_found(self):
         unused_names = main(["tests/files/functions.py", "--no-color"])
 
         self.assertEqual(
             unused_names,
             (
-                "tests/files/functions.py:1:0: DC002 Function `unused_function` is never used\n"
-                "tests/files/functions.py:13:0: DC002 Function `another_unused_function` is never used\n"
-                "tests/files/functions.py:14:4: DC002 Function `this_is_unused_closure` is never used"
+                "tests/files/functions.py:1:0: DC02 Function `unused_function` is never used\n"
+                "tests/files/functions.py:13:0: DC02 Function `another_unused_function` is never used\n"
+                "tests/files/functions.py:14:4: DC02 Function `this_is_unused_closure` is never used"
             ),
         )
 
     def test_unused_class_name_found(self):
         unused_names = main(["tests/files/classes.py", "--no-color"])
 
         # TODO: Scope of a variable in the output would be really helpful (class name, function)
         # - dotted notation would suite perfectly
         self.assertEqual(
             unused_names,
             (
-                "tests/files/classes.py:1:0: DC003 Class `UnusedClass` is never used\n"
-                "tests/files/classes.py:13:0: DC003 Class `AnotherUnusedClass` is never used"
+                "tests/files/classes.py:1:0: DC03 Class `UnusedClass` is never used\n"
+                "tests/files/classes.py:13:0: DC03 Class `AnotherUnusedClass` is never used"
             ),
         )
 
     def test_run_dead_code_finder_with_a_subprocess_in_a_right_directory_main(self):
         unused_names = main(
             [
                 "tests/files/variables.py",
                 "deadcode/tests/files/variables.py",
                 "--no-color",
             ]
         )
         self.assertEqual(
             unused_names,
             (
-                "tests/files/variables.py:1:0: DC001 Variable `unused_global_variable` is never used\n"
-                "tests/files/variables.py:3:0: DC001 Variable `ANOTHER_GLOBAL_VARIABLE` is never used\n"
-                "tests/files/variables.py:5:0: DC001 Variable `third_global_varialbe` is never used"
+                "tests/files/variables.py:1:0: DC01 Variable `unused_global_variable` is never used\n"
+                "tests/files/variables.py:3:0: DC01 Variable `ANOTHER_GLOBAL_VARIABLE` is never used\n"
+                "tests/files/variables.py:5:0: DC01 Variable `third_global_varialbe` is never used"
             ),
         )
 
 
 class DeadCodeTests(BaseTestCase):
     def test_invalid_python_file_found(self):
         self.files = {"tests/files/invalid_file.py": """This is invalid python file content."""}
```

### Comparing `deadcode-2.2.2/deadcode/tests/test_imports.py` & `deadcode-2.3.0/deadcode/tests/test_imports.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,39 +60,39 @@
         self.files = {"foo.py": "unused_var = None this is syntax error"}
         unused_names = main(["foo.py", "--no-color"])
         assert unused_names is None
 
         # The same check works without a Syntax error
         self.files = {"foo.py": "unused_var = None"}
         unused_names = main(["foo.py", "--no-color"])
-        assert unused_names == "foo.py:1:0: DC001 Variable `unused_var` is never used"
+        assert unused_names == "foo.py:1:0: DC01 Variable `unused_var` is never used"
 
     def test_ignore_variable_names_in_comments(self):
         self.files = {
             "foo.py": """
                 # unused_variable is empty
                 unused_var = None  # This is a comment about unused_var
                 # Another comment about unused variable
                 """
         }
         unused_names = main(["ignore_names_by_pattern.py", "--no-color"])
-        assert unused_names == "foo.py:2:0: DC001 Variable `unused_var` is never used"
+        assert unused_names == "foo.py:2:0: DC01 Variable `unused_var` is never used"
 
     def test_ignore_variable_names_in_strings(self):
         self.files = {
             "foo.py": """
                 '''
                 unused_var initial value is None - this a string about unused_variable
                 '''
                 unused_var = None
                 print("This is another string about unused_variable")
                 """
         }
         unused_names = main(["ignore_names_by_pattern.py", "--no-color"])
-        assert unused_names == "foo.py:4:0: DC001 Variable `unused_var` is never used"
+        assert unused_names == "foo.py:4:0: DC01 Variable `unused_var` is never used"
 
     # TODO:
     def test_unused_names_found_in_subdirectories(self):
         pass
 
     def test_exclude_option(self):
         pass
```

### Comparing `deadcode-2.2.2/deadcode/tests/test_line_number_detection.py` & `deadcode-2.3.0/deadcode/tests/test_line_number_detection.py`

 * *Files identical despite different names*

### Comparing `deadcode-2.2.2/deadcode/tests/test_output.py` & `deadcode-2.3.0/deadcode/tests/test_output.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,19 +103,19 @@
                 print(THIS_ONE_IS_USED)"""
         }
         unused_names = main(["tests/files/variables.py"])
 
         self.assertEqual(
             unused_names,
             (
-                "tests/files/variables.py:1:0: \x1b[91mDC001\x1b[0m Variable "
+                "tests/files/variables.py:1:0: \x1b[91mDC01\x1b[0m Variable "
                 "`\x1b[1munused_global_variable\x1b[0m` is never used\n"
-                "tests/files/variables.py:2:0: \x1b[91mDC001\x1b[0m Variable "
+                "tests/files/variables.py:2:0: \x1b[91mDC01\x1b[0m Variable "
                 "`\x1b[1mANOTHER_GLOBAL_VARIABLE\x1b[0m` is never used\n"
-                "tests/files/variables.py:3:0: \x1b[91mDC001\x1b[0m Variable "
+                "tests/files/variables.py:3:0: \x1b[91mDC01\x1b[0m Variable "
                 "`\x1b[1mthird_global_varialbe3\x1b[0m` is never used"
             ),
         )
 
     def test_no_color_option(self):
         self.files = {
             "tests/files/variables.py": """
@@ -126,12 +126,12 @@
                 print(THIS_ONE_IS_USED)"""
         }
         unused_names = main(["tests/files/variables.py", "--no-color"])
 
         self.assertEqual(
             unused_names,
             (
-                "tests/files/variables.py:1:0: DC001 Variable `unused_global_variable` is never used\n"
-                "tests/files/variables.py:2:0: DC001 Variable `ANOTHER_GLOBAL_VARIABLE` is never used\n"
-                "tests/files/variables.py:3:0: DC001 Variable `third_global_varialbe3` is never used"
+                "tests/files/variables.py:1:0: DC01 Variable `unused_global_variable` is never used\n"
+                "tests/files/variables.py:2:0: DC01 Variable `ANOTHER_GLOBAL_VARIABLE` is never used\n"
+                "tests/files/variables.py:3:0: DC01 Variable `third_global_varialbe3` is never used"
             ),
         )
```

### Comparing `deadcode-2.2.2/deadcode/tests/actions/test_find_python_filenames.py` & `deadcode-2.3.0/deadcode/tests/actions/test_find_python_filenames.py`

 * *Files identical despite different names*

### Comparing `deadcode-2.2.2/deadcode/tests/actions/test_merge_overlaping_file_parts.py` & `deadcode-2.3.0/deadcode/tests/actions/test_merge_overlaping_file_parts.py`

 * *Files identical despite different names*

### Comparing `deadcode-2.2.2/deadcode/tests/cli_args/test_exclude.py` & `deadcode-2.3.0/deadcode/tests/cli_args/test_exclude.py`

 * *Files identical despite different names*

### Comparing `deadcode-2.2.2/deadcode/tests/cli_args/test_fix.py` & `deadcode-2.3.0/deadcode/tests/cli_args/test_fix.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
                 """
         }
 
         unused_names = main(["ignore_names_by_pattern.py", "--no-color", "--fix"])
         self.assertEqual(
             unused_names,
             (
-                "ignore_names_by_pattern.py:1:0: DC003 Class `UnusedClass` is never used\n\n"
+                "ignore_names_by_pattern.py:1:0: DC03 Class `UnusedClass` is never used\n\n"
                 "Removed 1 unused code item!"
             ),
         )
 
         self.assertFiles(
             {
                 "ignore_names_by_pattern.py": """
@@ -41,15 +41,15 @@
                 print("Keep the file")
                 """
         }
 
         unused_names = main(["ignore_names_by_pattern.py", "--no-color", "--fix"])
         self.assertEqual(
             unused_names,
-            ("ignore_names_by_pattern.py:1:0: DC002 Function `foo` is never used\n\n" "Removed 1 unused code item!"),
+            ("ignore_names_by_pattern.py:1:0: DC02 Function `foo` is never used\n\n" "Removed 1 unused code item!"),
         )
 
         self.assertFiles(
             {
                 "ignore_names_by_pattern.py": """
                 print("Keep the file")
         """
@@ -70,15 +70,15 @@
                 print(spam, used_variable)
                 """
         }
 
         unused_names = main(["ignore_names_by_pattern.py", "--no-color", "--fix"])
         self.assertEqual(
             unused_names,
-            ("ignore_names_by_pattern.py:3:0: DC002 Function `foo` is never used\n\n" "Removed 1 unused code item!"),
+            ("ignore_names_by_pattern.py:3:0: DC02 Function `foo` is never used\n\n" "Removed 1 unused code item!"),
         )
 
         self.assertFiles(
             {
                 "ignore_names_by_pattern.py": """
                 used_variable = "one"
 
@@ -103,16 +103,16 @@
                 """
         }
 
         unused_names = main(["ignore_names_by_pattern.py", "--no-color", "--fix"])
         self.assertEqual(
             unused_names,
             (
-                "ignore_names_by_pattern.py:3:0: DC001 Variable `unused_variable` is never used\n"
-                "ignore_names_by_pattern.py:5:0: DC002 Function `unused_function` is never used\n\n"
+                "ignore_names_by_pattern.py:3:0: DC01 Variable `unused_variable` is never used\n"
+                "ignore_names_by_pattern.py:5:0: DC02 Function `unused_function` is never used\n\n"
                 "Removed 2 unused code items!"
             ),
         )
 
         self.assertFiles(
             {
                 "ignore_names_by_pattern.py": """
```

### Comparing `deadcode-2.2.2/deadcode/tests/cli_args/test_ignore_bodies_if_inherits_from.py` & `deadcode-2.3.0/deadcode/tests/cli_args/test_ignore_bodies_if_inherits_from.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,13 +34,13 @@
                     pass
                 """
             }
         )
 
         self.assertEqual(
             output,
-            "foo.py:5:0: DC003 Class `UnusedClass` is never used\n"
-            "foo.py:15:0: DC003 Class `AnotherUnusedClass` is never used\n"
-            "foo.py:16:4: DC001 Variable `another_unused_attribute` is never used\n"
+            "foo.py:5:0: DC03 Class `UnusedClass` is never used\n"
+            "foo.py:15:0: DC03 Class `AnotherUnusedClass` is never used\n"
+            "foo.py:16:4: DC01 Variable `another_unused_attribute` is never used\n"
             "\n"
             "Removed 3 unused code items!",
         )
```

### Comparing `deadcode-2.2.2/deadcode/tests/cli_args/test_ignore_definitions.py` & `deadcode-2.3.0/deadcode/tests/cli_args/test_ignore_definitions.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,15 @@
                     pass
                 """
         }
         unused_names = main(["ignore_names_by_pattern.py", "--no-color", "--ignore-definitions=UnusedClass", "--fix"])
 
         self.assertEqual(
             unused_names,
-            ("foo.py:10:0: DC003 Class `AnotherUnusedClass` is never used\n\nRemoved 1 unused code item!"),
+            ("foo.py:10:0: DC03 Class `AnotherUnusedClass` is never used\n\nRemoved 1 unused code item!"),
         )
 
         self.assertFiles(
             {
                 "foo.py": """
                 class UnusedClass:
                     unused_attribute = None
```

### Comparing `deadcode-2.2.2/deadcode/tests/cli_args/test_ignore_definitions_if_inherits_from.py` & `deadcode-2.3.0/deadcode/tests/cli_args/test_ignore_definitions_if_inherits_from.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,16 +48,16 @@
                         unused_class_attribute = ""
                 """
             }
         )
 
         self.assertEqual(
             output,
-            "foo.py:15:0: DC003 Class `AnotherUnusedClass` is never used\n"
-            "foo.py:16:4: DC001 Variable `another_unused_attribute` is never used\n"
+            "foo.py:15:0: DC03 Class `AnotherUnusedClass` is never used\n"
+            "foo.py:16:4: DC01 Variable `another_unused_attribute` is never used\n"
             "\n"
             "Removed 2 unused code items!",
         )
 
     @skip
     def test_ignore_class_definition_if_inherits_from_multiple_classes(self):
         # TODO:
@@ -114,12 +114,12 @@
                         unused_class_attribute = ""
                 """
             }
         )
 
         self.assertEqual(
             output,
-            "foo.py:15:0: DC003 Class `AnotherUnusedClass` is never used\n"
-            "foo.py:16:4: DC001 Variable `another_unused_attribute` is never used\n"
+            "foo.py:15:0: DC03 Class `AnotherUnusedClass` is never used\n"
+            "foo.py:16:4: DC01 Variable `another_unused_attribute` is never used\n"
             "\n"
             "Removed 2 unused code items!",
         )
```

### Comparing `deadcode-2.2.2/deadcode/tests/cli_args/test_ignore_names.py` & `deadcode-2.3.0/deadcode/tests/cli_args/test_ignore_names.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
                 """
         }
         # unused_names = main(["ignore_names_by_pattern.py", "--no-color", "--ignore-names=\\w*Model,.*[Ii]{1}gnore.*"])
         unused_names = main(["ignore_names_by_pattern.py", "--no-color", "--ignore-names=*Model,*[Ii]gnore*"])
 
         self.assertEqual(
             unused_names,
-            ("ignore_names_by_pattern.py:7:0: DC003 Class `Unused` is never used"),
+            ("ignore_names_by_pattern.py:7:0: DC03 Class `Unused` is never used"),
         )
 
     def test_ignore_names_matched_by_dot_regexp_pattern(self):
         # TODO: README has to be updated to not use .*, use * instead.
         # TODO: Ignoring does not work as expected: wild cards have to be used.
 
         self.files = {
@@ -46,15 +46,15 @@
                     pass
                 """
         }
         unused_names = main(["ignore_names_by_pattern.py", "--no-color", "--ignore-names=*Model,*Ignore*"])
 
         self.assertEqual(
             unused_names,
-            ("ignore_names_by_pattern.py:7:0: DC003 Class `Unused` is never used"),
+            ("ignore_names_by_pattern.py:7:0: DC03 Class `Unused` is never used"),
         )
 
     def test_ignore_names_matched_exactly(self):
         self.files = {
             "ignore_names_by_pattern.py": """
                 class MyModel:
                     pass
@@ -71,9 +71,9 @@
         }
         unused_names = main(
             ["ignore_names_by_pattern.py", "--no-color", "--ignore-names=MyModel,MyUserModel,ThisClassShouldBeIgnored"]
         )
 
         self.assertEqual(
             unused_names,
-            ("ignore_names_by_pattern.py:7:0: DC003 Class `Unused` is never used"),
+            ("ignore_names_by_pattern.py:7:0: DC03 Class `Unused` is never used"),
         )
```

### Comparing `deadcode-2.2.2/deadcode/tests/code_item/test_code_item.py` & `deadcode-2.3.0/deadcode/tests/code_item/test_code_item.py`

 * *Files identical despite different names*

### Comparing `deadcode-2.2.2/deadcode/tests/fix/test_assign.py` & `deadcode-2.3.0/deadcode/tests/fix/test_assign.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
                 print("Keep the file")
                 """
         }
 
         unused_names = main(["foo.py", "--no-color", "--fix"])
         self.assertEqual(
             unused_names,
-            ("foo.py:1:0: DC001 Variable `unused_variable` is never used\n\n" "Removed 1 unused code item!"),
+            ("foo.py:1:0: DC01 Variable `unused_variable` is never used\n\n" "Removed 1 unused code item!"),
         )
 
         self.assertFiles(
             {
                 "foo.py": """
                 print("Keep the file")
             """
@@ -38,15 +38,15 @@
             unused_variable: List[int] = [123]
         """
         }
 
         unused_names = main(["foo.py", "--no-color", "--fix"])
         self.assertEqual(
             unused_names,
-            ("foo.py:1:0: DC001 Variable `unused_variable` is never used\n\n" "Removed 1 unused code item!"),
+            ("foo.py:1:0: DC01 Variable `unused_variable` is never used\n\n" "Removed 1 unused code item!"),
         )
 
         self.assertFiles({"foo.py": """"""})
 
     @skip
     def test_unused_variable_in_multiple_inline_assignment_start(self):
         self.files = {
```

### Comparing `deadcode-2.2.2/deadcode/tests/fix/test_class_def.py` & `deadcode-2.3.0/deadcode/tests/fix/test_class_def.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,16 +45,16 @@
                 """,
         }
 
         unused_names = main(["foo.py", "--no-color", "--fix"])
         self.assertEqual(
             unused_names,
             (
-                "bar.py:1:0: DC003 Class `MyTest` is never used\n"
-                "foo.py:1:0: DC003 Class `MyTest` is never used\n\n"
+                "bar.py:1:0: DC03 Class `MyTest` is never used\n"
+                "foo.py:1:0: DC03 Class `MyTest` is never used\n\n"
                 "Removed 2 unused code items!"
             ),
         )
 
         self.assertFiles({})
 
     @skip
@@ -77,15 +77,15 @@
                 print(instance)
                 """,
         }
 
         unused_names = main(["foo.py", "--no-color", "--fix"])
         self.assertEqual(
             unused_names,
-            ("bar.py:1:0: DC003 Class `MyTest` is never used\n\n" "Removed 2 unused code items!"),
+            ("bar.py:1:0: DC03 Class `MyTest` is never used\n\n" "Removed 2 unused code items!"),
         )
 
         self.assertFiles({})
 
     @skip
     def test_methods_with_the_same_name(self):
         # TODO: this use case has to be solved by using scopes
@@ -106,11 +106,11 @@
                 print(bar.foo())
                 """
         }
 
         unused_names = main(["foo.py", "--no-color", "--fix"])
         self.assertEqual(
             unused_names,
-            ("foo.py:2:4: DC004 Method `foo` is never used\n\n" "Removed 1 unused code item!"),
+            ("foo.py:2:4: DC04 Method `foo` is never used\n\n" "Removed 1 unused code item!"),
         )
 
         self.assertFiles({})
```

### Comparing `deadcode-2.2.2/deadcode/tests/fix/test_empty_files.py` & `deadcode-2.3.0/deadcode/tests/fix/test_empty_files.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,25 +12,25 @@
             "foo.py": """
                 """
         }
 
         unused_names = main(["foo.py", "--no-color", "--fix"])
         self.assertEqual(
             unused_names,
-            ("foo.py DC011 Empty file\n\n" "Removed 1 unused code item!"),
+            ("foo.py DC11 Empty file\n\n" "Removed 1 unused code item!"),
         )
 
         self.assertFiles({}, removed=["foo.py"])
 
     def test_file_removal_from_subpath(self):
         self.files = {
             "bar/foo.py": """
                 """
         }
 
         unused_names = main(["bar/foo.py", "--no-color", "--fix"])
         self.assertEqual(
             unused_names,
-            ("bar/foo.py DC011 Empty file\n\n" "Removed 1 unused code item!"),
+            ("bar/foo.py DC11 Empty file\n\n" "Removed 1 unused code item!"),
         )
 
         self.assertFiles({}, removed=["bar/foo.py"])
```

### Comparing `deadcode-2.2.2/deadcode/tests/fix/test_method_def.py` & `deadcode-2.3.0/deadcode/tests/fix/test_method_def.py`

 * *Files identical despite different names*

### Comparing `deadcode-2.2.2/deadcode/tests/fix/test_scope.py` & `deadcode-2.3.0/deadcode/tests/fix/test_scope.py`

 * *Files identical despite different names*

### Comparing `deadcode-2.2.2/deadcode/tests/fix/test_unreachable_code.py` & `deadcode-2.3.0/deadcode/tests/fix/test_unreachable_code.py`

 * *Files identical despite different names*

### Comparing `deadcode-2.2.2/deadcode/tests/noqa/test_noqa_comments.py` & `deadcode-2.3.0/deadcode/tests/noqa/test_noqa_comments.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 from deadcode.tests.base import BaseTestCase
 
 
 class TestNoqaComments(BaseTestCase):
     def test_unused_class_is_unchanged_if_noqa_comment_is_provided(self):
         self.files = {
             "foo.py": """
-                class MyTest:  # noqa: DC003
+                class MyTest:  # noqa: DC03
                     pass
                 """
         }
 
         unused_names = main(["foo.py", "--no-color", "--fix"])
 
         self.assertFiles(
             {
                 "foo.py": """
-                class MyTest:  # noqa: DC003
+                class MyTest:  # noqa: DC03
                     pass
                 """
             }
         )
 
         self.assertEqual(unused_names, None)
 
@@ -44,191 +44,191 @@
         )
 
         self.assertEqual(unused_names, None)
 
     def test_unused_variable(self):
         self.files = {
             "foo.py": """
-                unused_variable = "Hello"  # noqa: DC001
+                unused_variable = "Hello"  # noqa: DC01
                     pass
                 """
         }
 
         unused_names = main(["foo.py", "--no-color", "--fix"])
         self.assertEqual(unused_names, None)
 
         self.assertFiles(
             {
                 "foo.py": """
-                unused_variable = "Hello"  # noqa: DC001
+                unused_variable = "Hello"  # noqa: DC01
                     pass
                 """
             }
         )
 
     def test_unused_variable_but_wrong_noqa_specified(self):
         self.files = {
             "foo.py": """
-                unused_variable = "Hello"  # noqa: DC002
+                unused_variable = "Hello"  # noqa: DC02
                 """
         }
 
         unused_names = main(["foo.py", "--no-color", "--fix"])
 
         self.assertFiles({})
         self.assertEqual(
             unused_names,
-            ("foo.py:1:0: DC001 Variable `unused_variable` is never used\n\n" "Removed 1 unused code item!"),
+            ("foo.py:1:0: DC01 Variable `unused_variable` is never used\n\n" "Removed 1 unused code item!"),
         )
 
     def test_unused_function(self):
         self.files = {
             "foo.py": """
-                def unused_function():  # noqa: DC002
+                def unused_function():  # noqa: DC02
                     pass
                 """
         }
 
         unused_names = main(["foo.py", "--no-color", "--fix"])
         self.assertEqual(unused_names, None)
 
         self.assertFiles(
             {
                 "foo.py": """
-                def unused_function():  # noqa: DC002
+                def unused_function():  # noqa: DC02
                     pass
                 """
             }
         )
 
     def test_unused_method(self):
         self.files = {
             "foo.py": """
                 class MyTest:
-                    def unused_method(self):  # noqa: DC004
+                    def unused_method(self):  # noqa: DC04
                         pass
 
                 instance = MyTest()
                 print(instance)
                 """
         }
 
         unused_names = main(["foo.py", "--no-color", "--fix"])
 
         self.assertFiles(
             {
                 "foo.py": """
                 class MyTest:
-                    def unused_method(self):  # noqa: DC004
+                    def unused_method(self):  # noqa: DC04
                         pass
 
                 instance = MyTest()
                 print(instance)
                 """
             }
         )
 
         self.assertEqual(unused_names, None)
 
     @skip
     def test_unused_attribute(self):
-        # TODO: DC005 does not work.
+        # TODO: DC05 does not work.
         self.files = {
             "foo.py": """
                 class MyTest:
-                    unused_attribute = 123  # noqa: DC005
+                    unused_attribute = 123  # noqa: DC05
 
                 instance = MyTest()
                 print(instance)
                 """
         }
 
         unused_names = main(["foo.py", "--no-color", "--fix"])
 
         self.assertFiles(
             {
                 "foo.py": """
                 class MyTest:
-                    unused_attribute = 123  # noqa: DC005
+                    unused_attribute = 123  # noqa: DC05
 
                 instance = MyTest()
                 print(instance)
                 """
             }
         )
 
         self.assertEqual(unused_names, None)
 
     @skip
     def test_unused_name(self):
-        # TODO: DC006 does not work.
+        # TODO: DC06 does not work.
         self.files = {
             "foo.py": """
                 class MyTest:
-                    unused_attribute = 123  # noqa: DC006
+                    unused_attribute = 123  # noqa: DC06
 
                 instance = MyTest()
                 print(instance)
                 """
         }
 
         unused_names = main(["foo.py", "--no-color", "--fix"])
 
         self.assertFiles(
             {
                 "foo.py": """
                 class MyTest:
-                    unused_attribute = 123  # noqa: DC006
+                    unused_attribute = 123  # noqa: DC06
 
                 instance = MyTest()
                 print(instance)
                 """
             }
         )
 
         self.assertEqual(unused_names, None)
 
     def test_unused_import(self):
         self.files = {
             "foo.py": """
-                from typing import Optional  # noqa: DC007
+                from typing import Optional  # noqa: DC07
                 """
         }
 
         unused_names = main(["foo.py", "--no-color", "--fix"])
 
         self.assertFiles(
             {
                 "foo.py": """
-                from typing import Optional  # noqa: DC007
+                from typing import Optional  # noqa: DC07
                 """
             }
         )
 
         self.assertEqual(unused_names, None)
 
     @skip
     def test_unused_property(self):
         self.files = {
             "foo.py": """
                 class Foo:
                     @property
-                    def bar(self):  # noqa: DC008
+                    def bar(self):  # noqa: DC08
                         return None
                 """
         }
 
         unused_names = main(["foo.py", "--no-color", "--fix"])
 
         self.assertFiles(
             {
                 "foo.py": """
                 class Foo:
                     @property
-                    def bar(self):  # noqa: DC008
+                    def bar(self):  # noqa: DC08
                         return None
                 """
             }
         )
 
         self.assertEqual(unused_names, None)
 
@@ -236,92 +236,92 @@
     def test_unreachable_code(self):
         # TODO: identify all cases, when unreachable code is detected, and write unit tests
 
         self.files = {
             "foo.py": """
                 if True:
                     pass
-                else:  # noqa: DC009
+                else:  # noqa: DC09
                     print("Hello world")
                 """
         }
 
         unused_names = main(["foo.py", "--no-color", "--fix"])
 
         self.assertFiles(
             {
                 "foo.py": """
                 if True:
                     pass
-                else:  # noqa: DC009
+                else:  # noqa: DC09
                     print("Hello world")
                 """
             }
         )
 
         self.assertEqual(unused_names, None)
 
     def test_empty_file(self):
         # TODO: this test passes only because comment is treated as non empty file content
         self.files = {
             "foo.py": """
-                # noqa: DC011
+                # noqa: DC11
                 """
         }
 
         unused_names = main(["foo.py", "--no-color", "--fix"])
 
         self.assertFiles(
             {
                 "foo.py": """
-                # noqa: DC011
+                # noqa: DC11
                 """
             }
         )
 
         self.assertEqual(unused_names, None)
 
     def test_commented_out_code(self):
         # TODO: this test only passes because commented-out-code check is not yet implemented
         self.files = {
             "foo.py": """
-                # print("Hello world")  # noqa: DC012
+                # print("Hello world")  # noqa: DC12
                 """
         }
 
         unused_names = main(["foo.py", "--no-color", "--fix"])
 
         self.assertFiles(
             {
                 "foo.py": """
-                # print("Hello world")  # noqa: DC012
+                # print("Hello world")  # noqa: DC12
                 """
             }
         )
 
         self.assertEqual(unused_names, None)
 
     @skip
     def test_ignore_expression(self):
         self.files = {
             "foo.py": """
-                class Foo:  # noqa: DC013
+                class Foo:  # noqa: DC13
                     this_attiribute_is_unused = True
 
                     def this_method_is_not_used_as_well(self):
                         pass
                 """
         }
 
         unused_names = main(["foo.py", "--no-color", "--fix"])
 
         self.assertFiles(
             {
                 "foo.py": """
-                class Foo:  # noqa: DC013
+                class Foo:  # noqa: DC13
                     this_attiribute_is_unused = True
 
                     def this_method_is_not_used_as_well(self):
                         pass
                 """
             }
         )
```

### Comparing `deadcode-2.2.2/deadcode/utils/fix_indent.py` & `deadcode-2.3.0/deadcode/utils/fix_indent.py`

 * *Files identical despite different names*

### Comparing `deadcode-2.2.2/deadcode/utils/flatten_lists.py` & `deadcode-2.3.0/deadcode/utils/flatten_lists.py`

 * *Files identical despite different names*

### Comparing `deadcode-2.2.2/deadcode/visitor/code_item.py` & `deadcode-2.3.0/deadcode/visitor/code_item.py`

 * *Files 6% similar despite different names*

```diff
@@ -48,14 +48,15 @@
         "code_parts",
         "scope",
         "inherits_from",
         "name_line",
         "name_column",
         "message",
         "error_code",
+        "number_of_uses",
     )
 
     def __init__(
         self,
         name: str,
         type_: UnusedCodeType,
         filename: Path,
@@ -66,20 +67,22 @@
         # last_column: Optional[int] = None,
         code_parts: Optional[List[Part]] = None,  # TODO: I should use a dataclass instead of a tuple for Part.
         scope: Optional[str] = None,
         inherits_from: Optional[List[str]] = None,
         name_line: Optional[int] = None,
         name_column: Optional[int] = None,
         message: str = "",
+        number_of_uses: int = 0,
     ):
         self.name = name
         self.type_ = type_
         self.filename = filename
         self.scope = scope
         self.inherits_from = inherits_from
+        self.number_of_uses = number_of_uses
 
         if code_parts is None:
             self.code_parts = []
         else:
             self.code_parts = code_parts
 
         # if first_lineno is not None:
```

### Comparing `deadcode-2.2.2/deadcode/visitor/dead_code_visitor.py` & `deadcode-2.3.0/deadcode/visitor/dead_code_visitor.py`

 * *Files 17% similar despite different names*

```diff
@@ -77,91 +77,24 @@
         self.scopes = NestedScope()
 
     @property
     def scope(self) -> str:
         return ".".join(self.scope_parts)
 
     def add_used_name(self, name: str, scope: Optional[str] = None) -> None:
-        self.used_names.add(name)
+        # TODO: Usage should be tracked on CodeItem.
 
-    # def scan(self, code, filename=""):
-    #     filename = Path(filename)
-    #     self.code = code.splitlines()
-    #     self.noqa_lines = noqa.parse_noqa(self.code)
-    #     self.filename = filename
-
-    #     def handle_syntax_error(e):
-    #         text = f' at "{e.text.strip()}"' if e.text else ""
-    #         self._log(
-    #             f"{utils.format_path(filename)}:{e.lineno}: {e.msg}{text}",
-    #             file=sys.stderr,
-    #             force=True,
-    #         )
-    #         self.found_dead_code_or_error = True
-
-    #     try:
-    #         node = ast.parse(code, filename=str(self.filename), type_comments=True)
-    #     except SyntaxError as err:
-    #         handle_syntax_error(err)
-    #     except ValueError as err:
-    #         # ValueError is raised if source contains null bytes.
-    #         self._log(
-    #             f'{utils.format_path(filename)}: invalid source code "{err}"',
-    #             file=sys.stderr,
-    #             force=True,
-    #         )
-    #         self.found_dead_code_or_error = True
-    #     else:
-    #         # When parsing type comments, visiting can throw SyntaxError.
-    #         try:
-    #             self.visit(node)
-    #         except SyntaxError as err:
-    #             handle_syntax_error(err)
-
-    # TODO: do not load the AST of all the files into memory.
-    # Should instead parse the files one by one and discard already parsed files.
-    # The memory might add up for larger projects, especially that AST is whay larger the the code itself.
+        # TODO: Lets first resolve, how to correctly set the type of a function argument.
+        # We should have CodeItem as a type, not only name as string.
+        # TODO: investigate: am I always able to retrieve the type of a variable?
 
-    def visit_abstract_syntax_trees(self) -> None:
-        # NEXTODO:
-        # So whats here? These examples could be moved to exclusion before.
-        # Also AST should not be constructed until the parsing part.
-
-        # def prepare_pattern(pattern):
-        #     if not any(char in pattern for char in "*?["):
-        #         pattern = f"*{pattern}*"
-        #     return pattern
-
-        # exclude = [prepare_pattern(pattern) for pattern in (self.args.exclude or [])]
-
-        # def exclude_path(path):
-        #     return _match(path, exclude, case=False)
-
-        # # paths = [Path(path) for path in paths]
-
-        # for module in utils.get_modules(paths):
-        #     if exclude_path(module):
-        #         self._log("Excluded:", module)
-        #         continue
-
-        # self._log("Scanning:", module)
-        # try:
-        #     module_string = utils.read_file(module)
-        # except utils.VultureInputException as err:  # noqa: F841
-        #     self._log(
-        #         f"Error: Could not read file {module} - {err}\n"
-        #         f"Try to change the encoding to UTF-8.",
-        #         file=sys.stderr,
-        #         force=True,
-        #     )
-        #     self.found_dead_code_or_error = True
-        # else:
-        #     self.scan(module_string, filename=module)
+        self.used_names.add(name)
+        self.scopes.mark_as_used(name, self.scope)
 
-        # TODO: should parse the AST here.
+    def visit_abstract_syntax_trees(self) -> None:
         for file_path in self.filenames:
             with open(file_path) as f:
                 filename = os.path.basename(file_path)
                 module_name = os.path.splitext(filename)[0]
                 self.scope_parts = [module_name]
 
                 file_content = f.read()
@@ -176,32 +109,16 @@
                         CodeItem(
                             name=filename,
                             type_="unused_file",
                             filename=Path(file_path),
                             message="Empty file",
                         )
                     )
-        self.scopes
-
-        # unique_imports = {item.name for item in self.defined_imports}
-        # for import_name in unique_imports:
-        #     path = Path("whitelists") / (import_name + "_whitelist.py")
-        #     if exclude_path(path):
-        #         self._log("Excluded whitelist:", path)
-        #     else:
-        #         try:
-        #             module_data = pkgutil.get_data("vulture", str(path))
-        #             self._log("Included whitelist:", path)
-        #         except OSError:
-        #             # Most imported modules don't have a whitelist.
-        #             continue
-        #         module_string = module_data.decode("utf-8")
-        #         self.scan(module_string, filename=path)
 
-    def get_unused_code_items(self, sort_by_size: bool = False) -> Iterable[CodeItem]:
+    def get_unused_code_items(self) -> Iterable[CodeItem]:
         """
         Return ordered list of unused CodeItem objects.
         """
 
         unused_code = chain(
             self.unused_attrs,
             self.unused_classes,
@@ -212,27 +129,14 @@
             self.unused_vars,
             # self.unreachable_code,  # TODO: removal of unreachable_code has a lot of edge cases
             self.unused_file,
         )
 
         return sorted(unused_code, key=lambda item: (item.filename, item.name_line or 0))
 
-    # TODO: investigate whitelisting options
-    # def report(self, sort_by_size=False, make_whitelist=False):
-    #     """
-    #     Print ordered list of CodeItem objects to stdout.
-    #     """
-    #     for item in self.get_unused_code_items(sort_by_size=sort_by_size):
-    #         self._log(
-    #             item.get_whitelist_string() if make_whitelist else item.get_report(add_size=sort_by_size),
-    #             force=True,
-    #         )
-    #         self.found_dead_code_or_error = True
-    #     return self.found_dead_code_or_error
-
     @property
     def unused_classes(self) -> Iterable[CodeItem]:
         return _get_unused_items(self.defined_classes, self.used_names)
 
     @property
     def unused_funcs(self) -> Iterable[CodeItem]:
         return _get_unused_items(self.defined_funcs, self.used_names)
@@ -268,14 +172,16 @@
                 print(x.encode(), file=file)
 
     def _add_aliases(self, node: Union[ast.Import, ast.ImportFrom]) -> None:
         """
         We delegate to this method instead of using visit_alias() to have
         access to line numbers and to filter imports from __future__.
         """
+        # TODO: store full module path. Consider relative and absolute module import collisions.
+
         assert isinstance(node, (ast.Import, ast.ImportFrom))
         for name_and_alias in node.names:
             # Store only top-level module name ("os.path" -> "os").
             # We can't easily detect when "os.path" is used.
             name = name_and_alias.name.partition(".")[0]
             alias = name_and_alias.asname
             self._define(
@@ -361,15 +267,15 @@
             code_parts=[Part(first_lineno, last_lineno, last_node.col_offset, last_node.end_col_offset or 0)],
             scope=self.scope,
             name_line=last_node.lineno,  # TODO: Maybe this should be a property?
             name_column=last_node.col_offset,  # TODO: Maybe this should be a property?
             message=message,
             inherits_from=inherits_from,
         )
-        self.scopes.add_to_scope(code_item)
+        self.scopes.add(code_item)
 
         if ignored(first_lineno, type_=type_):
             self._log(f'Ignoring {type_} "{name}"')
         else:
             collection.append(code_item)
 
     def _define_variable(self, name: str, node: ast.AST) -> None:
@@ -457,24 +363,18 @@
 
         if not (bases_attr := getattr(node, "bases", None)):
             return None
 
         bases = [base.id for base in bases_attr if getattr(base, "id", None)]
         inherits_from = bases[:]
 
-        current_scope = list((self.scopes.get_scope(self.scope) or {}).keys())
-
         for base in bases:
-            if base in current_scope:
-                try:
-                    base_code_item = current_scope[current_scope.index(base)]
-                    if parent_inherits_from := getattr(base_code_item, "inherits_from", None):
-                        inherits_from.extend(parent_inherits_from)
-                except ValueError:
-                    logger.error("Was not able to resolve base string to code_item in current scope")
+            if base_code_item := self.scopes.get(name=base, scope=self.scope):
+                if base_inherits_from := getattr(base_code_item, "inherits_from", None):
+                    inherits_from.extend(base_inherits_from)
 
         return inherits_from
 
     def visit_ClassDef(self, node: ast.ClassDef) -> None:
         for decorator in node.decorator_list:
             if _match(utils.get_decorator_name(decorator), self.ignore_decorators):  # type: ignore
                 self._log(f'Ignoring class "{node.name}" (decorator whitelisted)')
@@ -535,14 +435,23 @@
     # def visit_MatchClass(self, node: ast.MatchClass) -> None:  # type: ignore
     def visit_MatchClass(self, node) -> None:  # type: ignore
         for kwd_attr in node.kwd_attrs:
             self.add_used_name(kwd_attr)
 
     def visit(self, node: ast.AST) -> None:
         node_name = getattr(node, "name", None)
+
+        # > TODO: Expr scope has to be updated after visiting nested nodes.
+        # Do I have to merge custom visits with visit method in order to achieve this?
+        #
+        # I should write a unit test with only an exrepssion and check which methods are being called.
+        # I should only handled that single expression handling properly.
+
+        # breakpoint()
+
         if inherits_from := self.get_inherits_from(node):
             node.inherits_from = inherits_from  # type: ignore
 
         should_turn_off_ignore_new_definitions = False
         if (
             # Name is in ignore_definitions
             node_name
@@ -554,16 +463,14 @@
         ):
             if not self.should_ignore_new_definitions:
                 self.should_ignore_new_definitions = True
                 should_turn_off_ignore_new_definitions = True
 
         method_name = "visit_" + node.__class__.__name__
         visitor = getattr(self, method_name, None)
-        # if self.verbose:
-        #     lineno = getattr(node, "lineno", 1)
 
         if visitor:
             visitor(node)
 
         # TODO: use decorator for this code chunk
         was_scope_increased = True
         if isinstance(node, ast.ClassDef):
@@ -582,15 +489,27 @@
         # There isn't a clean subset of node types that might have type
         # comments, so just check all of them.
         type_comment = getattr(node, "type_comment", None)
         if type_comment is not None:
             mode = "func_type" if isinstance(node, (ast.FunctionDef, ast.AsyncFunctionDef)) else "eval"
             self.visit(ast.parse(type_comment, filename="<type_comment>", mode=mode))
 
-        self.generic_visit(node)
+        ###########
+        # """Called if no explicit visitor function exists for a node."""
+        # TODO: for assignment statements unused_code unit should be whole assignment statement instead of a name itself
+        # Note: Node is None if file is empty, contains only a docstring, a comment or has a SyntaxError.
+        if node:
+            for _, value in ast.iter_fields(node):
+                if isinstance(value, list):
+                    self._handle_ast_list(value)
+                    for item in value:
+                        if isinstance(item, ast.AST):
+                            self.visit(item)
+                elif isinstance(value, ast.AST):
+                    self.visit(value)
 
         # TODO: use decorator for this code chunk
         if should_turn_off_ignore_new_definitions:
             self.should_ignore_new_definitions = False
 
         # TODO: use decorator for this code chunk
         if was_scope_increased:
@@ -611,24 +530,7 @@
                     self.unreachable_code,
                     class_name,
                     first_unreachable_node,
                     last_node=ast_list[-1],
                     message=f"unreachable code after '{class_name}'",
                 )
                 return None
-
-    def generic_visit(self, node: ast.AST) -> None:
-        """Called if no explicit visitor function exists for a node."""
-        # TODO: for assignment statements unused_code unit should be whole assignment statement instead of a name itself
-
-        # Note: Node is None if file is empty, contains only a docstring, a comment or has a SyntaxError.
-        if not node:
-            return None
-
-        for _, value in ast.iter_fields(node):
-            if isinstance(value, list):
-                self._handle_ast_list(value)
-                for item in value:
-                    if isinstance(item, ast.AST):
-                        self.visit(item)
-            elif isinstance(value, ast.AST):
-                self.visit(value)
```

### Comparing `deadcode-2.2.2/deadcode/visitor/ignore.py` & `deadcode-2.3.0/deadcode/visitor/ignore.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,26 +17,26 @@
     "setup_class",
     "teardown_class",
     "setup_method",
     "teardown_method",
 }
 
 ERROR_CODES = {
-    "variable": "DC001",
-    "function": "DC002",
-    "class": "DC003",
-    "method": "DC004",
-    "attribute": "DC005",
-    "name": "DC006",
-    "import": "DC007",
-    "property": "DC008",
-    "unreachable_code": "DC009",
-    "empty_file": "DC011",
-    "commented_out_code": "DC012",
-    "ignore_expression": "DC013",
+    "variable": "DC01",
+    "function": "DC02",
+    "class": "DC03",
+    "method": "DC04",
+    "attribute": "DC05",
+    "name": "DC06",
+    "import": "DC07",
+    "property": "DC08",
+    "unreachable_code": "DC09",
+    "empty_file": "DC11",
+    "commented_out_code": "DC12",
+    "ignore_expression": "DC13",
 }
 
 
 def _get_unused_items(defined_items: Iterable[CodeItem], used_names: Set[str]) -> Iterable[CodeItem]:
     unused_items = [item for item in defined_items if item.name not in used_names]
     unused_items.sort(key=lambda item: item.name.lower())
     return unused_items
```

### Comparing `deadcode-2.2.2/deadcode/visitor/lines.py` & `deadcode-2.3.0/deadcode/visitor/lines.py`

 * *Files identical despite different names*

### Comparing `deadcode-2.2.2/deadcode/visitor/noqa.py` & `deadcode-2.3.0/deadcode/visitor/noqa.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,29 +12,42 @@
     # `# NoQA: E123,W451,F921`
     r"# noqa(?::[\s]?(?P<codes>([A-Z]+[0-9]+(?:[,\s]+)?)+))?",
     re.IGNORECASE,
 )
 
 NOQA_CODE_MAP = {
     # flake8 F401: module imported but unused.
-    "F401": "DC007",
+    "F401": "DC07",
     # flake8 F841: local variable is assigned to but never used.
-    "F841": "DC001",
-    "DC001": "DC001",
-    "DC002": "DC002",
-    "DC003": "DC003",
-    "DC004": "DC004",
-    "DC005": "DC005",
-    "DC006": "DC006",
-    "DC007": "DC007",
-    "DC008": "DC008",
-    "DC009": "DC009",
-    "DC011": "DC011",
-    "DC012": "DC012",
-    "DC013": "DC013",
+    "F841": "DC01",
+    "DC01": "DC01",
+    "DC02": "DC02",
+    "DC03": "DC03",
+    "DC04": "DC04",
+    "DC05": "DC05",
+    "DC06": "DC06",
+    "DC07": "DC07",
+    "DC08": "DC08",
+    "DC09": "DC09",
+    "DC11": "DC11",
+    "DC12": "DC12",
+    "DC13": "DC13",
+    # For backward compatibility
+    "DC001": "DC01",
+    "DC002": "DC02",
+    "DC003": "DC03",
+    "DC004": "DC04",
+    "DC005": "DC05",
+    "DC006": "DC06",
+    "DC007": "DC07",
+    "DC008": "DC08",
+    "DC009": "DC09",
+    "DC011": "DC11",
+    "DC012": "DC12",
+    "DC013": "DC13",
 }
 
 
 def _parse_error_codes(matches_dict: Dict[str, str]) -> List[str]:
     # If no error code is specified, add the line to the "all" category.
     return [c.strip() for c in (matches_dict["codes"] or "all").split(",")]
```

### Comparing `deadcode-2.2.2/deadcode/visitor/utils.py` & `deadcode-2.3.0/deadcode/visitor/utils.py`

 * *Files identical despite different names*

### Comparing `deadcode-2.2.2/.gitignore` & `deadcode-2.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `deadcode-2.2.2/LICENSE` & `deadcode-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `deadcode-2.2.2/pyproject.toml` & `deadcode-2.3.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "deadcode"
-version = "2.2.2"
+version = "2.3.0"
 authors = [
     {name = "Albertas Gimbutas", email = "albertasgim@gmail.com"},
 ]
 description = "Find and remove dead code."
 readme = "README.md"
 requires-python = ">= 3.8"
 classifiers = [
@@ -69,14 +69,17 @@
     "fix_indent",
     "ignore_definitions_if_decorated_with",
     "ignore_if_decorated_with",
     "ignore_if_inherits_from",
     "ignore_line",
     "ignore_names_if_decorated_with",
     "ignore_names_if_inherits_from",
+    "ignore_bodies_of",
+    "ignore_bodies_if_decorated_with",
+    "ignore_bodies_if_inherits_from",
     "parse_noqa",
     "scoped_name",
     "show",
     "visit_*",
 ]
 
 exclude = ["tests"]
@@ -84,8 +87,8 @@
 [tool.black]
 max_line_length = 120
 line_length = 120
 target_version = ["py38"]
 
 
 [tool.pytest.ini_options]
-addopts = "--cov=. --no-cov-on-fail --cov-fail-under=78.0"
+addopts = "--cov=. --no-cov-on-fail --cov-fail-under=88.0"
```

### Comparing `deadcode-2.2.2/PKG-INFO` & `deadcode-2.3.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,494 +1,618 @@
-00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
-00000010: 3a20 322e 310a 4e61 6d65 3a20 6465 6164  : 2.1.Name: dead
-00000020: 636f 6465 0a56 6572 7369 6f6e 3a20 322e  code.Version: 2.
-00000030: 322e 320a 5375 6d6d 6172 793a 2046 696e  2.2.Summary: Fin
-00000040: 6420 616e 6420 7265 6d6f 7665 2064 6561  d and remove dea
-00000050: 6420 636f 6465 2e0a 5072 6f6a 6563 742d  d code..Project-
-00000060: 5552 4c3a 2048 6f6d 6570 6167 652c 2068  URL: Homepage, h
-00000070: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00000080: 6d2f 616c 6265 7274 6173 2f64 6561 6463  m/albertas/deadc
-00000090: 6f64 650a 5072 6f6a 6563 742d 5552 4c3a  ode.Project-URL:
-000000a0: 2044 6f63 756d 656e 7461 7469 6f6e 2c20   Documentation, 
-000000b0: 6874 7470 733a 2f2f 6465 6164 636f 6465  https://deadcode
-000000c0: 2e72 6561 6474 6865 646f 6373 2e69 6f2f  .readthedocs.io/
-000000d0: 0a41 7574 686f 722d 656d 6169 6c3a 2041  .Author-email: A
-000000e0: 6c62 6572 7461 7320 4769 6d62 7574 6173  lbertas Gimbutas
-000000f0: 203c 616c 6265 7274 6173 6769 6d40 676d   <albertasgim@gm
-00000100: 6169 6c2e 636f 6d3e 0a4c 6963 656e 7365  ail.com>.License
-00000110: 2d46 696c 653a 204c 4943 454e 5345 0a43  -File: LICENSE.C
-00000120: 6c61 7373 6966 6965 723a 2044 6576 656c  lassifier: Devel
-00000130: 6f70 6d65 6e74 2053 7461 7475 7320 3a3a  opment Status ::
-00000140: 2033 202d 2041 6c70 6861 0a43 6c61 7373   3 - Alpha.Class
-00000150: 6966 6965 723a 204c 6963 656e 7365 203a  ifier: License :
-00000160: 3a20 4f53 4920 4170 7072 6f76 6564 203a  : OSI Approved :
-00000170: 3a20 474e 5520 4166 6665 726f 2047 656e  : GNU Affero Gen
-00000180: 6572 616c 2050 7562 6c69 6320 4c69 6365  eral Public Lice
-00000190: 6e73 6520 7633 0a43 6c61 7373 6966 6965  nse v3.Classifie
-000001a0: 723a 204e 6174 7572 616c 204c 616e 6775  r: Natural Langu
-000001b0: 6167 6520 3a3a 2045 6e67 6c69 7368 0a43  age :: English.C
-000001c0: 6c61 7373 6966 6965 723a 204f 7065 7261  lassifier: Opera
-000001d0: 7469 6e67 2053 7973 7465 6d20 3a3a 204f  ting System :: O
-000001e0: 5320 496e 6465 7065 6e64 656e 740a 436c  S Independent.Cl
-000001f0: 6173 7369 6669 6572 3a20 5072 6f67 7261  assifier: Progra
-00000200: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
-00000210: 3a20 5079 7468 6f6e 0a43 6c61 7373 6966  : Python.Classif
-00000220: 6965 723a 2050 726f 6772 616d 6d69 6e67  ier: Programming
-00000230: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
-00000240: 686f 6e20 3a3a 2033 2e38 0a43 6c61 7373  hon :: 3.8.Class
-00000250: 6966 6965 723a 2050 726f 6772 616d 6d69  ifier: Programmi
-00000260: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
-00000270: 7974 686f 6e20 3a3a 2033 2e39 0a43 6c61  ython :: 3.9.Cla
-00000280: 7373 6966 6965 723a 2050 726f 6772 616d  ssifier: Program
-00000290: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
-000002a0: 2050 7974 686f 6e20 3a3a 2033 2e31 300a   Python :: 3.10.
-000002b0: 436c 6173 7369 6669 6572 3a20 5072 6f67  Classifier: Prog
-000002c0: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
-000002d0: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
-000002e0: 3131 0a52 6571 7569 7265 732d 5079 7468  11.Requires-Pyth
-000002f0: 6f6e 3a20 3e3d 332e 380a 5265 7175 6972  on: >=3.8.Requir
-00000300: 6573 2d44 6973 743a 2074 6f6d 6c69 3d3d  es-Dist: tomli==
-00000310: 322e 302e 310a 4465 7363 7269 7074 696f  2.0.1.Descriptio
-00000320: 6e2d 436f 6e74 656e 742d 5479 7065 3a20  n-Content-Type: 
-00000330: 7465 7874 2f6d 6172 6b64 6f77 6e0a 0a23  text/markdown..#
-00000340: 2064 6561 6463 6f64 650a 6064 6561 6463   deadcode.`deadc
-00000350: 6f64 6560 2061 6c6c 6f77 7320 746f 2064  ode` allows to d
-00000360: 6574 6563 7420 616e 6420 6669 7820 756e  etect and fix un
-00000370: 7573 6564 2050 7974 686f 6e20 636f 6465  used Python code
-00000380: 2e20 4974 2069 6d70 6c65 6d65 6e74 7320  . It implements 
-00000390: 6044 4358 5858 600a 7374 6174 6963 2063  `DCXXX`.static c
-000003a0: 6f64 6520 6c69 6e74 696e 6720 7275 6c65  ode linting rule
-000003b0: 7320 666f 7220 6465 7465 6374 696e 6720  s for detecting 
-000003c0: 756e 7573 6564 2063 6f64 6520 7375 6368  unused code such
-000003d0: 2061 730a 7661 7269 6162 6c65 732c 2066   as.variables, f
-000003e0: 756e 6374 696f 6e73 2061 6e64 2063 6c61  unctions and cla
-000003f0: 7373 6573 2e0a 0a23 2320 496e 7374 616c  sses...## Instal
-00000400: 6c61 7469 6f6e 0a60 6060 7368 656c 6c0a  lation.```shell.
-00000410: 7069 7020 696e 7374 616c 6c20 6465 6164  pip install dead
-00000420: 636f 6465 0a60 6060 0a0a 2323 2055 7361  code.```..## Usa
-00000430: 6765 0a60 6060 7368 656c 6c0a 6465 6164  ge.```shell.dead
-00000440: 636f 6465 202e 0a60 6060 0a0a 4f72 2077  code ..```..Or w
-00000450: 6974 6820 636f 6d6d 616e 6420 6c69 6e65  ith command line
-00000460: 206f 7074 696f 6e73 3a0a 6060 600a 6465   options:.```.de
-00000470: 6164 636f 6465 202e 202d 2d65 7863 6c75  adcode . --exclu
-00000480: 6465 3d76 656e 762c 7465 7374 7320 2d2d  de=venv,tests --
-00000490: 6967 6e6f 7265 2d6e 616d 6573 3d42 6173  ignore-names=Bas
-000004a0: 6554 6573 7443 6173 652c 2a4d 6978 696e  eTestCase,*Mixin
-000004b0: 202d 2d69 676e 6f72 652d 6e61 6d65 732d   --ignore-names-
-000004c0: 696e 2d66 696c 6573 3d6d 6967 7261 7469  in-files=migrati
-000004d0: 6f6e 730a 6060 600a 0a54 6865 2073 616d  ons.```..The sam
-000004e0: 6520 6f70 7469 6f6e 7320 6361 6e20 6265  e options can be
-000004f0: 2070 726f 7669 6465 6420 696e 2060 7079   provided in `py
-00000500: 7072 6f6a 6563 742e 746f 6d6c 6020 7365  project.toml` se
-00000510: 7474 696e 6773 2066 696c 653a 0a60 6060  ttings file:.```
-00000520: 0a5b 746f 6f6c 2e64 6561 6463 6f64 655d  .[tool.deadcode]
-00000530: 0a65 7863 6c75 6465 203d 205b 2276 656e  .exclude = ["ven
-00000540: 7622 2c20 2274 6573 7473 225d 0a69 676e  v", "tests"].ign
-00000550: 6f72 652d 6e61 6d65 7320 3d20 5b22 4261  ore-names = ["Ba
-00000560: 7365 5465 7374 4361 7365 222c 2022 2a4d  seTestCase", "*M
-00000570: 6978 696e 225d 0a69 676e 6f72 652d 6e61  ixin"].ignore-na
-00000580: 6d65 732d 696e 2d66 696c 6573 203d 205b  mes-in-files = [
-00000590: 226d 6967 7261 7469 6f6e 7322 5d0a 6060  "migrations"].``
-000005a0: 600a 0a23 2323 2043 6f6d 6d61 6e64 206c  `..### Command l
-000005b0: 696e 6520 6f70 7469 6f6e 730a 0a7c 204f  ine options..| O
-000005c0: 7074 696f 6e26 6e62 7370 3b26 6e62 7370  ption&nbsp;&nbsp
-000005d0: 3b26 6e62 7370 3b26 6e62 7370 3b26 6e62  ;&nbsp;&nbsp;&nb
-000005e0: 7370 3b26 6e62 7370 3b26 6e62 7370 3b26  sp;&nbsp;&nbsp;&
-000005f0: 6e62 7370 3b26 6e62 7370 3b26 6e62 7370  nbsp;&nbsp;&nbsp
-00000600: 3b26 6e62 7370 3b26 6e62 7370 3b26 6e62  ;&nbsp;&nbsp;&nb
-00000610: 7370 3b26 6e62 7370 3b26 6e62 7370 3b26  sp;&nbsp;&nbsp;&
-00000620: 6e62 7370 3b26 6e62 7370 3b26 6e62 7370  nbsp;&nbsp;&nbsp
-00000630: 3b26 6e62 7370 3b26 6e62 7370 3b26 6e62  ;&nbsp;&nbsp;&nb
-00000640: 7370 3b26 6e62 7370 3b26 6e62 7370 3b26  sp;&nbsp;&nbsp;&
-00000650: 6e62 7370 3b26 6e62 7370 3b26 6e62 7370  nbsp;&nbsp;&nbsp
-00000660: 3b26 6e62 7370 3b26 6e62 7370 3b26 6e62  ;&nbsp;&nbsp;&nb
-00000670: 7370 3b26 6e62 7370 3b26 6e62 7370 3b26  sp;&nbsp;&nbsp;&
-00000680: 6e62 7370 3b26 6e62 7370 3b26 6e62 7370  nbsp;&nbsp;&nbsp
-00000690: 3b26 6e62 7370 3b20 7c20 5479 7065 207c  ;&nbsp; | Type |
-000006a0: 204d 6561 6e69 6e67 2020 7c0a 7c2d 2d2d   Meaning  |.|---
-000006b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000006c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000006d0: 2d2d 2d2d 2d2d 2d2d 7c2d 2d2d 2d2d 2d7c  --------|------|
-000006e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000006f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000700: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000710: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000720: 2d2d 2d2d 2d2d 7c0a 7c60 2d2d 6669 7860  ------|.|`--fix`
-00000730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000750: 2020 2020 7c20 2d20 2020 207c 2041 7574      | -    | Aut
-00000760: 6f6d 6174 6963 616c 6c79 2072 656d 6f76  omatically remov
-00000770: 6520 6465 7465 6374 6564 2075 6e75 7365  e detected unuse
-00000780: 6420 636f 6465 2065 7870 7265 7373 696f  d code expressio
-00000790: 6e73 2066 726f 6d20 7468 6520 636f 6465  ns from the code
-000007a0: 2062 6173 652e 207c 0a7c 602d 2d65 7863   base. |.|`--exc
-000007b0: 6c75 6465 6020 2020 2020 2020 2020 2020  lude`           
-000007c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000007d0: 2020 2020 207c 206c 6973 7420 7c20 4669       | list | Fi
-000007e0: 6c65 6e61 6d65 7320 286f 7220 7061 7468  lenames (or path
-000007f0: 2065 7870 7265 7373 696f 6e73 292c 2077   expressions), w
-00000800: 6869 6368 2077 696c 6c20 6265 2063 6f6d  hich will be com
-00000810: 706c 6574 656c 7920 736b 6970 7065 6420  pletely skipped 
-00000820: 7769 7468 6f75 7420 6265 696e 6720 616e  without being an
-00000830: 616c 7973 6564 2e20 7c0a 7c60 2d2d 6967  alysed. |.|`--ig
-00000840: 6e6f 7265 2d6e 616d 6573 6020 2020 2020  nore-names`     
-00000850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000860: 2020 2020 2020 7c20 6c69 7374 207c 2052        | list | R
-00000870: 656d 6f76 6573 2070 726f 7669 6465 6420  emoves provided 
-00000880: 6c69 7374 206f 6620 6e61 6d65 7320 6672  list of names fr
-00000890: 6f6d 2074 6865 206f 7574 7075 742e 2052  om the output. R
-000008a0: 6567 6578 7020 6578 7072 6573 7369 6f6e  egexp expression
-000008b0: 7320 746f 206d 6174 6368 206d 756c 7469  s to match multi
-000008c0: 706c 6520 6e61 6d65 7320 6361 6e20 616c  ple names can al
-000008d0: 736f 2062 6520 7072 6f76 6964 6564 2c20  so be provided, 
-000008e0: 652e 672e 2060 2a4d 6978 696e 6020 7769  e.g. `*Mixin` wi
-000008f0: 6c6c 206d 6174 6368 2061 6c6c 2063 6c61  ll match all cla
-00000900: 7373 6573 2065 6e64 696e 6720 7769 7468  sses ending with
-00000910: 2060 4d69 7869 6e60 2e20 7c0a 7c60 2d2d   `Mixin`. |.|`--
-00000920: 6967 6e6f 7265 2d6e 616d 6573 2d69 6e2d  ignore-names-in-
-00000930: 6669 6c65 7360 2020 2020 2020 2020 2020  files`          
-00000940: 2020 2020 2020 2020 7c20 6c69 7374 207c          | list |
-00000950: 2049 676e 6f72 6573 2075 6e75 7365 6420   Ignores unused 
-00000960: 6e61 6d65 7320 696e 2066 696c 6573 2c20  names in files, 
-00000970: 7768 6963 6820 6669 6c65 6e61 6d65 7320  which filenames 
-00000980: 6d61 7463 6820 7072 6f76 6964 6564 2070  match provided p
-00000990: 6174 6820 6578 7072 6573 7369 6f6e 732e  ath expressions.
-000009a0: 207c 0a7c 602d 2d69 676e 6f72 652d 6e61   |.|`--ignore-na
-000009b0: 6d65 732d 6966 2d69 6e68 6572 6974 732d  mes-if-inherits-
-000009c0: 6672 6f6d 6020 2020 2020 2020 2020 207c  from`          |
-000009d0: 206c 6973 7420 7c20 4967 6e6f 7265 7320   list | Ignores 
-000009e0: 6e61 6d65 7320 6f66 2063 6c61 7373 6573  names of classes
-000009f0: 2c20 7768 6963 6820 696e 6865 7269 7420  , which inherit 
-00000a00: 6672 6f6d 2070 726f 7669 6465 6420 636c  from provided cl
-00000a10: 6173 7320 6e61 6d65 732e 207c 0a7c 602d  ass names. |.|`-
-00000a20: 2d69 676e 6f72 652d 6e61 6d65 732d 6966  -ignore-names-if
-00000a30: 2d64 6563 6f72 6174 6564 2d77 6974 6860  -decorated-with`
-00000a40: 2020 2020 2020 2020 207c 206c 6973 7420           | list 
-00000a50: 7c20 4967 6e6f 7265 7320 6e61 6d65 7320  | Ignores names 
-00000a60: 6f66 2061 6e20 6578 7072 6573 7369 6f6e  of an expression
-00000a70: 2c20 7768 6963 6820 6973 2064 6563 6f72  , which is decor
-00000a80: 6174 6564 2077 6974 6820 6f6e 6520 6f66  ated with one of
-00000a90: 2074 6865 2070 726f 7669 6465 6420 6465   the provided de
-00000aa0: 636f 7261 746f 7220 6e61 6d65 732e 207c  corator names. |
-00000ab0: 0a7c 602d 2d69 676e 6f72 652d 626f 6469  .|`--ignore-bodi
-00000ac0: 6573 2d6f 6660 2020 2020 2020 2020 2020  es-of`          
-00000ad0: 2020 2020 2020 2020 2020 2020 207c 206c               | l
-00000ae0: 6973 7420 7c20 4967 6e6f 7265 7320 626f  ist | Ignores bo
-00000af0: 6479 206f 6620 616e 2065 7870 7265 7373  dy of an express
-00000b00: 696f 6e20 6966 2069 7473 206e 616d 6520  ion if its name 
-00000b10: 6d61 7463 6865 7320 616e 7920 6f66 2074  matches any of t
-00000b20: 6865 2070 726f 7669 6465 6420 6e61 6d65  he provided name
-00000b30: 732e 207c 0a7c 602d 2d69 676e 6f72 652d  s. |.|`--ignore-
-00000b40: 626f 6469 6573 2d69 662d 6465 636f 7261  bodies-if-decora
-00000b50: 7465 642d 7769 7468 6020 2020 2020 2020  ted-with`       
-00000b60: 207c 206c 6973 7420 7c20 4967 6e6f 7265   | list | Ignore
-00000b70: 7320 626f 6479 206f 6620 616e 2065 7870  s body of an exp
-00000b80: 7265 7373 696f 6e20 6966 2069 7473 2064  ression if its d
-00000b90: 6563 6f72 6174 6564 2077 6974 6820 6f6e  ecorated with on
-00000ba0: 6520 6f66 2074 6865 2070 726f 7669 6465  e of the provide
-00000bb0: 6420 6465 636f 7261 746f 7220 6e61 6d65  d decorator name
-00000bc0: 732e 207c 0a7c 602d 2d69 676e 6f72 652d  s. |.|`--ignore-
-00000bd0: 626f 6469 6573 2d69 662d 696e 6865 7269  bodies-if-inheri
-00000be0: 7473 2d66 726f 6d60 2020 2020 2020 2020  ts-from`        
-00000bf0: 207c 206c 6973 7420 7c20 4967 6e6f 7265   | list | Ignore
-00000c00: 7320 626f 6479 206f 6620 6120 636c 6173  s body of a clas
-00000c10: 7320 6966 2069 7420 696e 6865 7269 7473  s if it inherits
-00000c20: 2066 726f 6d20 616e 7920 6f66 2074 6865   from any of the
-00000c30: 2070 726f 7669 6465 6420 636c 6173 7320   provided class 
-00000c40: 6e61 6d65 732e 207c 0a7c 602d 2d69 676e  names. |.|`--ign
-00000c50: 6f72 652d 6465 6669 6e69 7469 6f6e 7360  ore-definitions`
-00000c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000c70: 2020 2020 207c 206c 6973 7420 7c20 4967       | list | Ig
-00000c80: 6e6f 7265 7320 6465 6669 6e69 7469 6f6e  nores definition
-00000c90: 2028 696e 636c 7564 696e 6720 6e61 6d65   (including name
-00000ca0: 2061 6e64 2062 6f64 7929 2069 6620 6120   and body) if a 
-00000cb0: 6e61 6d65 206f 6620 616e 2065 7870 7265  name of an expre
-00000cc0: 7373 696f 6e20 6d61 7463 6865 7320 616e  ssion matches an
-00000cd0: 7920 6f66 2074 6865 2070 726f 7669 6465  y of the provide
-00000ce0: 6420 6f6e 6573 2e20 7c0a 7c60 2d2d 6967  d ones. |.|`--ig
-00000cf0: 6e6f 7265 2d64 6566 696e 6974 696f 6e73  nore-definitions
-00000d00: 2d69 662d 696e 6865 7269 7473 2d66 726f  -if-inherits-fro
-00000d10: 6d60 2020 2020 7c20 6c69 7374 207c 2049  m`    | list | I
-00000d20: 676e 6f72 6573 2064 6566 696e 6974 696f  gnores definitio
-00000d30: 6e20 2869 6e63 6c75 6469 6e67 206e 616d  n (including nam
-00000d40: 6520 616e 6420 626f 6479 2920 6f66 2061  e and body) of a
-00000d50: 2063 6c61 7373 2069 6620 6974 2069 6e68   class if it inh
-00000d60: 6572 6974 7320 6672 6f6d 2061 6e79 206f  erits from any o
-00000d70: 6620 7468 6520 7072 6f76 6964 6564 2063  f the provided c
-00000d80: 6c61 7373 206e 616d 6573 2e20 7c0a 7c60  lass names. |.|`
-00000d90: 2d2d 6967 6e6f 7265 2d64 6566 696e 6974  --ignore-definit
-00000da0: 696f 6e73 2d69 662d 6465 636f 7261 7465  ions-if-decorate
-00000db0: 642d 7769 7468 6020 2020 7c20 6c69 7374  d-with`   | list
-00000dc0: 207c 2049 676e 6f72 6573 2064 6566 696e   | Ignores defin
-00000dd0: 6974 696f 6e20 2869 6e63 6c75 6469 6e67  ition (including
-00000de0: 206e 616d 6520 616e 6420 626f 6479 2920   name and body) 
-00000df0: 6f66 2061 6e20 6578 7072 6573 7369 6f6e  of an expression
-00000e00: 2c20 7768 6963 6820 6973 2064 6563 6f72  , which is decor
-00000e10: 6174 6564 2077 6974 6820 616e 7920 6f66  ated with any of
-00000e20: 2074 6865 2070 726f 7669 6465 6420 6465   the provided de
-00000e30: 636f 7261 746f 7220 6e61 6d65 732e 207c  corator names. |
-00000e40: 0a7c 602d 2d6e 6f2d 636f 6c6f 7260 2020  .|`--no-color`  
-00000e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000e60: 2020 2020 2020 2020 2020 2020 207c 202d               | -
-00000e70: 2020 2020 7c20 5265 6d6f 7665 7320 636f      | Removes co
-00000e80: 6c6f 7273 2066 726f 6d20 7468 6520 6f75  lors from the ou
-00000e90: 7470 7574 2e20 7c0a 7c60 2d2d 636f 756e  tput. |.|`--coun
-00000ea0: 7460 2020 2020 2020 2020 2020 2020 2020  t`              
+00000000: 5b21 5b44 6561 6463 6f64 6520 4c6f 676f  [![Deadcode Logo
+00000010: 5d28 6874 7470 733a 2f2f 7261 772e 6769  ](https://raw.gi
+00000020: 7468 7562 7573 6572 636f 6e74 656e 742e  thubusercontent.
+00000030: 636f 6d2f 616c 6265 7274 6173 2f64 6561  com/albertas/dea
+00000040: 6463 6f64 652f 6d61 696e 2f64 6f63 732f  dcode/main/docs/
+00000050: 5f73 7461 7469 632f 6465 6164 636f 6465  _static/deadcode
+00000060: 2d6c 6f67 6f2d 7265 6164 6d65 2e70 6e67  -logo-readme.png
+00000070: 295d 2868 7474 7073 3a2f 2f64 6561 6463  )](https://deadc
+00000080: 6f64 652e 7265 6164 7468 6564 6f63 732e  ode.readthedocs.
+00000090: 696f 2f65 6e2f 7374 6162 6c65 2f29 0a0a  io/en/stable/)..
+000000a0: 3c68 3220 616c 6967 6e3d 2263 656e 7465  <h2 align="cente
+000000b0: 7222 3e46 696e 6420 616e 6420 4669 7820  r">Find and Fix 
+000000c0: 556e 7573 6564 2050 7974 686f 6e20 436f  Unused Python Co
+000000d0: 6465 3c2f 6832 3e0a 0a3c 7020 616c 6967  de</h2>..<p alig
+000000e0: 6e3d 2263 656e 7465 7222 3e0a 3c61 2068  n="center">.<a h
+000000f0: 7265 663d 2268 7474 7073 3a2f 2f67 6974  ref="https://git
+00000100: 6875 622e 636f 6d2f 616c 6265 7274 6173  hub.com/albertas
+00000110: 2f64 6561 6463 6f64 652f 626c 6f62 2f6d  /deadcode/blob/m
+00000120: 6169 6e2f 4c49 4345 4e53 4522 3e3c 696d  ain/LICENSE"><im
+00000130: 6720 616c 743d 224c 6963 656e 7365 3a20  g alt="License: 
+00000140: 4147 504c 7633 2220 7372 633d 2268 7474  AGPLv3" src="htt
+00000150: 7073 3a2f 2f72 6177 2e67 6974 6875 6275  ps://raw.githubu
+00000160: 7365 7263 6f6e 7465 6e74 2e63 6f6d 2f61  sercontent.com/a
+00000170: 6c62 6572 7461 732f 6465 6164 636f 6465  lbertas/deadcode
+00000180: 2f6d 6169 6e2f 646f 6373 2f5f 7374 6174  /main/docs/_stat
+00000190: 6963 2f41 4750 4c76 332d 6c69 6365 6e73  ic/AGPLv3-licens
+000001a0: 652e 7376 6722 3e3c 2f61 3e0a 3c61 2068  e.svg"></a>.<a h
+000001b0: 7265 663d 2268 7474 7073 3a2f 2f70 7970  ref="https://pyp
+000001c0: 692e 6f72 672f 7072 6f6a 6563 742f 6465  i.org/project/de
+000001d0: 6164 636f 6465 2f22 3e3c 696d 6720 616c  adcode/"><img al
+000001e0: 743d 2250 7950 4922 2073 7263 3d22 6874  t="PyPI" src="ht
+000001f0: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
+00000200: 732e 696f 2f70 7970 692f 762f 6465 6164  s.io/pypi/v/dead
+00000210: 636f 6465 223e 3c2f 613e 0a3c 6120 6872  code"></a>.<a hr
+00000220: 6566 3d22 6874 7470 733a 2f2f 7065 7079  ef="https://pepy
+00000230: 2e74 6563 682f 7072 6f6a 6563 742f 6465  .tech/project/de
+00000240: 6164 636f 6465 223e 3c69 6d67 2061 6c74  adcode"><img alt
+00000250: 3d22 446f 776e 6c6f 6164 7322 2073 7263  ="Downloads" src
+00000260: 3d22 6874 7470 733a 2f2f 7374 6174 6963  ="https://static
+00000270: 2e70 6570 792e 7465 6368 2f62 6164 6765  .pepy.tech/badge
+00000280: 2f64 6561 6463 6f64 6522 3e3c 2f61 3e0a  /deadcode"></a>.
+00000290: 3c2f 703e 0a0a 0a23 2320 496e 7374 616c  </p>...## Instal
+000002a0: 6c61 7469 6f6e 0a60 6060 7368 656c 6c0a  lation.```shell.
+000002b0: 7069 7020 696e 7374 616c 6c20 6465 6164  pip install dead
+000002c0: 636f 6465 0a60 6060 0a0a 2323 2055 7361  code.```..## Usa
+000002d0: 6765 0a54 6f20 7365 6520 756e 7573 6564  ge.To see unused
+000002e0: 2063 6f64 6520 6669 6e64 696e 6773 3a0a   code findings:.
+000002f0: 6060 6073 6865 6c6c 0a64 6561 6463 6f64  ```shell.deadcod
+00000300: 6520 2e0a 6060 600a 0a54 6f20 7365 6520  e ..```..To see 
+00000310: 7375 6767 6573 7465 6420 6669 7865 7320  suggested fixes 
+00000320: 666f 7220 616c 6c20 6669 6c65 733a 0a60  for all files:.`
+00000330: 6060 7368 656c 6c0a 6465 6164 636f 6465  ``shell.deadcode
+00000340: 202e 202d 2d66 6978 202d 2d64 7279 0a60   . --fix --dry.`
+00000350: 6060 0a0a 546f 2073 6565 2073 7567 6765  ``..To see sugge
+00000360: 7374 6564 2066 6978 6573 2066 6f72 206f  sted fixes for o
+00000370: 6e6c 7920 6066 6f6f 2e70 7960 2066 696c  nly `foo.py` fil
+00000380: 653a 0a60 6060 7368 656c 6c0a 6465 6164  e:.```shell.dead
+00000390: 636f 6465 202e 202d 2d66 6978 202d 2d64  code . --fix --d
+000003a0: 7279 2066 6f6f 2e70 790a 6060 600a 0a54  ry foo.py.```..T
+000003b0: 6f20 6669 783a 0a60 6060 7368 656c 6c0a  o fix:.```shell.
+000003c0: 6465 6164 636f 6465 202e 202d 2d66 6978  deadcode . --fix
+000003d0: 0a60 6060 0a0a 5475 6e65 206f 7574 2073  .```..Tune out s
+000003e0: 6f6d 6520 6f66 2074 6865 2066 616c 7365  ome of the false
+000003f0: 2070 6f73 6974 6976 6573 2c20 652e 672e   positives, e.g.
+00000400: 3a0a 6060 600a 6465 6164 636f 6465 202e  :.```.deadcode .
+00000410: 202d 2d65 7863 6c75 6465 3d76 656e 762c   --exclude=venv,
+00000420: 7465 7374 7320 2d2d 6967 6e6f 7265 2d6e  tests --ignore-n
+00000430: 616d 6573 3d42 6173 6554 6573 7443 6173  ames=BaseTestCas
+00000440: 652c 2a4d 6978 696e 202d 2d69 676e 6f72  e,*Mixin --ignor
+00000450: 652d 6e61 6d65 732d 696e 2d66 696c 6573  e-names-in-files
+00000460: 3d6d 6967 7261 7469 6f6e 730a 6060 600a  =migrations.```.
+00000470: 0a54 6865 2073 616d 6520 6f70 7469 6f6e  .The same option
+00000480: 7320 6361 6e20 6265 2070 726f 7669 6465  s can be provide
+00000490: 6420 696e 2060 7079 7072 6f6a 6563 742e  d in `pyproject.
+000004a0: 746f 6d6c 6020 7365 7474 696e 6773 2066  toml` settings f
+000004b0: 696c 653a 0a60 6060 0a5b 746f 6f6c 2e64  ile:.```.[tool.d
+000004c0: 6561 6463 6f64 655d 0a65 7863 6c75 6465  eadcode].exclude
+000004d0: 203d 205b 2276 656e 7622 2c20 2274 6573   = ["venv", "tes
+000004e0: 7473 225d 0a69 676e 6f72 652d 6e61 6d65  ts"].ignore-name
+000004f0: 7320 3d20 5b22 4261 7365 5465 7374 4361  s = ["BaseTestCa
+00000500: 7365 222c 2022 2a4d 6978 696e 225d 0a69  se", "*Mixin"].i
+00000510: 676e 6f72 652d 6e61 6d65 732d 696e 2d66  gnore-names-in-f
+00000520: 696c 6573 203d 205b 226d 6967 7261 7469  iles = ["migrati
+00000530: 6f6e 7322 5d0a 6060 600a 0a23 2323 2043  ons"].```..### C
+00000540: 6f6d 6d61 6e64 206c 696e 6520 6f70 7469  ommand line opti
+00000550: 6f6e 730a 0a7c 204f 7074 696f 6e26 6e62  ons..| Option&nb
+00000560: 7370 3b26 6e62 7370 3b26 6e62 7370 3b26  sp;&nbsp;&nbsp;&
+00000570: 6e62 7370 3b26 6e62 7370 3b26 6e62 7370  nbsp;&nbsp;&nbsp
+00000580: 3b26 6e62 7370 3b26 6e62 7370 3b26 6e62  ;&nbsp;&nbsp;&nb
+00000590: 7370 3b26 6e62 7370 3b26 6e62 7370 3b26  sp;&nbsp;&nbsp;&
+000005a0: 6e62 7370 3b26 6e62 7370 3b26 6e62 7370  nbsp;&nbsp;&nbsp
+000005b0: 3b26 6e62 7370 3b26 6e62 7370 3b26 6e62  ;&nbsp;&nbsp;&nb
+000005c0: 7370 3b26 6e62 7370 3b26 6e62 7370 3b26  sp;&nbsp;&nbsp;&
+000005d0: 6e62 7370 3b26 6e62 7370 3b26 6e62 7370  nbsp;&nbsp;&nbsp
+000005e0: 3b26 6e62 7370 3b26 6e62 7370 3b26 6e62  ;&nbsp;&nbsp;&nb
+000005f0: 7370 3b26 6e62 7370 3b26 6e62 7370 3b26  sp;&nbsp;&nbsp;&
+00000600: 6e62 7370 3b26 6e62 7370 3b26 6e62 7370  nbsp;&nbsp;&nbsp
+00000610: 3b26 6e62 7370 3b26 6e62 7370 3b26 6e62  ;&nbsp;&nbsp;&nb
+00000620: 7370 3b26 6e62 7370 3b26 6e62 7370 3b20  sp;&nbsp;&nbsp; 
+00000630: 7c20 5479 7065 207c 204d 6561 6e69 6e67  | Type | Meaning
+00000640: 2020 7c0a 7c2d 2d2d 2d2d 2d2d 2d2d 2d2d    |.|-----------
+00000650: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000660: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000670: 7c2d 2d2d 2d2d 2d7c 2d2d 2d2d 2d2d 2d2d  |------|--------
+00000680: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000690: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000006a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000006b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 7c0a  --------------|.
+000006c0: 7c60 2d2d 6669 7860 2020 2020 2020 2020  |`--fix`        
+000006d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000006e0: 2020 2020 2020 2020 2020 2020 7c20 2d20              | - 
+000006f0: 2020 207c 2041 7574 6f6d 6174 6963 616c     | Automatical
+00000700: 6c79 2072 656d 6f76 6520 6465 7465 6374  ly remove detect
+00000710: 6564 2075 6e75 7365 6420 636f 6465 2065  ed unused code e
+00000720: 7870 7265 7373 696f 6e73 2066 726f 6d20  xpressions from 
+00000730: 7468 6520 636f 6465 2062 6173 652e 207c  the code base. |
+00000740: 0a7c 602d 2d64 7279 6020 2020 2020 2020  .|`--dry`       
+00000750: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000760: 2020 2020 2020 2020 2020 2020 207c 202d               | -
+00000770: 206f 7220 6c69 7374 207c 2053 686f 7720   or list | Show 
+00000780: 6368 616e 6765 7320 7768 6963 6820 776f  changes which wo
+00000790: 756c 6420 6265 206d 6164 6520 696e 2066  uld be made in f
+000007a0: 696c 6573 2e20 5368 6f77 7320 6368 616e  iles. Shows chan
+000007b0: 6765 7320 666f 7220 7072 6f76 6964 6564  ges for provided
+000007c0: 2066 696c 656e 616d 6573 206f 7220 7368   filenames or sh
+000007d0: 6f77 7320 616c 6c20 6368 616e 6765 7320  ows all changes 
+000007e0: 6966 206e 6f20 6669 6c65 6e61 6d65 2069  if no filename i
+000007f0: 7320 7370 6563 6966 6965 642e 207c 0a7c  s specified. |.|
+00000800: 602d 2d65 7863 6c75 6465 6020 2020 2020  `--exclude`     
+00000810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000820: 2020 2020 2020 2020 2020 207c 206c 6973             | lis
+00000830: 7420 7c20 4669 6c65 6e61 6d65 7320 286f  t | Filenames (o
+00000840: 7220 7061 7468 2065 7870 7265 7373 696f  r path expressio
+00000850: 6e73 292c 2077 6869 6368 2077 696c 6c20  ns), which will 
+00000860: 6265 2063 6f6d 706c 6574 656c 7920 736b  be completely sk
+00000870: 6970 7065 6420 7769 7468 6f75 7420 6265  ipped without be
+00000880: 696e 6720 616e 616c 7973 6564 2e20 7c0a  ing analysed. |.
+00000890: 7c60 2d2d 6967 6e6f 7265 2d6e 616d 6573  |`--ignore-names
+000008a0: 6020 2020 2020 2020 2020 2020 2020 2020  `               
+000008b0: 2020 2020 2020 2020 2020 2020 7c20 6c69              | li
+000008c0: 7374 207c 2052 656d 6f76 6573 2070 726f  st | Removes pro
+000008d0: 7669 6465 6420 6c69 7374 206f 6620 6e61  vided list of na
+000008e0: 6d65 7320 6672 6f6d 2074 6865 206f 7574  mes from the out
+000008f0: 7075 742e 2052 6567 6578 7020 6578 7072  put. Regexp expr
+00000900: 6573 7369 6f6e 7320 746f 206d 6174 6368  essions to match
+00000910: 206d 756c 7469 706c 6520 6e61 6d65 7320   multiple names 
+00000920: 6361 6e20 616c 736f 2062 6520 7072 6f76  can also be prov
+00000930: 6964 6564 2c20 652e 672e 2060 2a4d 6978  ided, e.g. `*Mix
+00000940: 696e 6020 7769 6c6c 206d 6174 6368 2061  in` will match a
+00000950: 6c6c 2063 6c61 7373 6573 2065 6e64 696e  ll classes endin
+00000960: 6720 7769 7468 2060 4d69 7869 6e60 2e20  g with `Mixin`. 
+00000970: 7c0a 7c60 2d2d 6967 6e6f 7265 2d6e 616d  |.|`--ignore-nam
+00000980: 6573 2d69 6e2d 6669 6c65 7360 2020 2020  es-in-files`    
+00000990: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
+000009a0: 6c69 7374 207c 2049 676e 6f72 6573 2075  list | Ignores u
+000009b0: 6e75 7365 6420 6e61 6d65 7320 696e 2066  nused names in f
+000009c0: 696c 6573 2c20 7768 6963 6820 6669 6c65  iles, which file
+000009d0: 6e61 6d65 7320 6d61 7463 6820 7072 6f76  names match prov
+000009e0: 6964 6564 2070 6174 6820 6578 7072 6573  ided path expres
+000009f0: 7369 6f6e 732e 207c 0a7c 602d 2d69 676e  sions. |.|`--ign
+00000a00: 6f72 652d 6e61 6d65 732d 6966 2d69 6e68  ore-names-if-inh
+00000a10: 6572 6974 732d 6672 6f6d 6020 2020 2020  erits-from`     
+00000a20: 2020 2020 207c 206c 6973 7420 7c20 4967       | list | Ig
+00000a30: 6e6f 7265 7320 6e61 6d65 7320 6f66 2063  nores names of c
+00000a40: 6c61 7373 6573 2c20 7768 6963 6820 696e  lasses, which in
+00000a50: 6865 7269 7420 6672 6f6d 2070 726f 7669  herit from provi
+00000a60: 6465 6420 636c 6173 7320 6e61 6d65 732e  ded class names.
+00000a70: 207c 0a7c 602d 2d69 676e 6f72 652d 6e61   |.|`--ignore-na
+00000a80: 6d65 732d 6966 2d64 6563 6f72 6174 6564  mes-if-decorated
+00000a90: 2d77 6974 6860 2020 2020 2020 2020 207c  -with`         |
+00000aa0: 206c 6973 7420 7c20 4967 6e6f 7265 7320   list | Ignores 
+00000ab0: 6e61 6d65 7320 6f66 2061 6e20 6578 7072  names of an expr
+00000ac0: 6573 7369 6f6e 2c20 7768 6963 6820 6973  ession, which is
+00000ad0: 2064 6563 6f72 6174 6564 2077 6974 6820   decorated with 
+00000ae0: 6f6e 6520 6f66 2074 6865 2070 726f 7669  one of the provi
+00000af0: 6465 6420 6465 636f 7261 746f 7220 6e61  ded decorator na
+00000b00: 6d65 732e 207c 0a7c 602d 2d69 676e 6f72  mes. |.|`--ignor
+00000b10: 652d 626f 6469 6573 2d6f 6660 2020 2020  e-bodies-of`    
+00000b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000b30: 2020 207c 206c 6973 7420 7c20 4967 6e6f     | list | Igno
+00000b40: 7265 7320 626f 6479 206f 6620 616e 2065  res body of an e
+00000b50: 7870 7265 7373 696f 6e20 6966 2069 7473  xpression if its
+00000b60: 206e 616d 6520 6d61 7463 6865 7320 616e   name matches an
+00000b70: 7920 6f66 2074 6865 2070 726f 7669 6465  y of the provide
+00000b80: 6420 6e61 6d65 732e 207c 0a7c 602d 2d69  d names. |.|`--i
+00000b90: 676e 6f72 652d 626f 6469 6573 2d69 662d  gnore-bodies-if-
+00000ba0: 6465 636f 7261 7465 642d 7769 7468 6020  decorated-with` 
+00000bb0: 2020 2020 2020 207c 206c 6973 7420 7c20         | list | 
+00000bc0: 4967 6e6f 7265 7320 626f 6479 206f 6620  Ignores body of 
+00000bd0: 616e 2065 7870 7265 7373 696f 6e20 6966  an expression if
+00000be0: 2069 7473 2064 6563 6f72 6174 6564 2077   its decorated w
+00000bf0: 6974 6820 6f6e 6520 6f66 2074 6865 2070  ith one of the p
+00000c00: 726f 7669 6465 6420 6465 636f 7261 746f  rovided decorato
+00000c10: 7220 6e61 6d65 732e 207c 0a7c 602d 2d69  r names. |.|`--i
+00000c20: 676e 6f72 652d 626f 6469 6573 2d69 662d  gnore-bodies-if-
+00000c30: 696e 6865 7269 7473 2d66 726f 6d60 2020  inherits-from`  
+00000c40: 2020 2020 2020 207c 206c 6973 7420 7c20         | list | 
+00000c50: 4967 6e6f 7265 7320 626f 6479 206f 6620  Ignores body of 
+00000c60: 6120 636c 6173 7320 6966 2069 7420 696e  a class if it in
+00000c70: 6865 7269 7473 2066 726f 6d20 616e 7920  herits from any 
+00000c80: 6f66 2074 6865 2070 726f 7669 6465 6420  of the provided 
+00000c90: 636c 6173 7320 6e61 6d65 732e 207c 0a7c  class names. |.|
+00000ca0: 602d 2d69 676e 6f72 652d 6465 6669 6e69  `--ignore-defini
+00000cb0: 7469 6f6e 7360 2020 2020 2020 2020 2020  tions`          
+00000cc0: 2020 2020 2020 2020 2020 207c 206c 6973             | lis
+00000cd0: 7420 7c20 4967 6e6f 7265 7320 6465 6669  t | Ignores defi
+00000ce0: 6e69 7469 6f6e 2028 696e 636c 7564 696e  nition (includin
+00000cf0: 6720 6e61 6d65 2061 6e64 2062 6f64 7929  g name and body)
+00000d00: 2069 6620 6120 6e61 6d65 206f 6620 616e   if a name of an
+00000d10: 2065 7870 7265 7373 696f 6e20 6d61 7463   expression matc
+00000d20: 6865 7320 616e 7920 6f66 2074 6865 2070  hes any of the p
+00000d30: 726f 7669 6465 6420 6f6e 6573 2e20 7c0a  rovided ones. |.
+00000d40: 7c60 2d2d 6967 6e6f 7265 2d64 6566 696e  |`--ignore-defin
+00000d50: 6974 696f 6e73 2d69 662d 696e 6865 7269  itions-if-inheri
+00000d60: 7473 2d66 726f 6d60 2020 2020 7c20 6c69  ts-from`    | li
+00000d70: 7374 207c 2049 676e 6f72 6573 2064 6566  st | Ignores def
+00000d80: 696e 6974 696f 6e20 2869 6e63 6c75 6469  inition (includi
+00000d90: 6e67 206e 616d 6520 616e 6420 626f 6479  ng name and body
+00000da0: 2920 6f66 2061 2063 6c61 7373 2069 6620  ) of a class if 
+00000db0: 6974 2069 6e68 6572 6974 7320 6672 6f6d  it inherits from
+00000dc0: 2061 6e79 206f 6620 7468 6520 7072 6f76   any of the prov
+00000dd0: 6964 6564 2063 6c61 7373 206e 616d 6573  ided class names
+00000de0: 2e20 7c0a 7c60 2d2d 6967 6e6f 7265 2d64  . |.|`--ignore-d
+00000df0: 6566 696e 6974 696f 6e73 2d69 662d 6465  efinitions-if-de
+00000e00: 636f 7261 7465 642d 7769 7468 6020 2020  corated-with`   
+00000e10: 7c20 6c69 7374 207c 2049 676e 6f72 6573  | list | Ignores
+00000e20: 2064 6566 696e 6974 696f 6e20 2869 6e63   definition (inc
+00000e30: 6c75 6469 6e67 206e 616d 6520 616e 6420  luding name and 
+00000e40: 626f 6479 2920 6f66 2061 6e20 6578 7072  body) of an expr
+00000e50: 6573 7369 6f6e 2c20 7768 6963 6820 6973  ession, which is
+00000e60: 2064 6563 6f72 6174 6564 2077 6974 6820   decorated with 
+00000e70: 616e 7920 6f66 2074 6865 2070 726f 7669  any of the provi
+00000e80: 6465 6420 6465 636f 7261 746f 7220 6e61  ded decorator na
+00000e90: 6d65 732e 207c 0a7c 602d 2d6e 6f2d 636f  mes. |.|`--no-co
+00000ea0: 6c6f 7260 2020 2020 2020 2020 2020 2020  lor`            
 00000eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000ec0: 2020 2020 7c20 2d20 2020 207c 2050 726f      | -    | Pro
-00000ed0: 7669 6465 7320 7468 6520 636f 756e 7420  vides the count 
-00000ee0: 6f66 2074 6865 2064 6574 6563 7465 6420  of the detected 
-00000ef0: 756e 7573 6564 206e 616d 6573 2069 6e73  unused names ins
-00000f00: 7465 6164 206f 6620 7072 696e 7469 6e67  tead of printing
-00000f10: 2074 6865 6d20 616c 6c20 6f75 742e 207c   them all out. |
-00000f20: 0a7c 602d 2d71 7569 6574 6020 2020 2020  .|`--quiet`     
-00000f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000f40: 2020 2020 2020 2020 2020 2020 207c 202d               | -
-00000f50: 2020 2020 7c20 446f 6573 206e 6f74 206f      | Does not o
-00000f60: 7574 7075 7420 616e 7974 6869 6e67 2e20  utput anything. 
-00000f70: 4d61 6b65 6669 6c65 2073 7469 6c6c 2066  Makefile still f
-00000f80: 6169 6c73 2077 6974 6820 6578 6974 2063  ails with exit c
-00000f90: 6f64 6520 3120 6966 2075 6e75 7365 6420  ode 1 if unused 
-00000fa0: 6e61 6d65 7320 6172 6520 666f 756e 642e  names are found.
-00000fb0: 207c 0a0a 0a23 2323 2323 2047 6c6f 7373   |...##### Gloss
-00000fc0: 6f72 790a 6e61 6d65 202d 2076 6172 6961  ory.name - varia
-00000fd0: 626c 652c 2066 756e 6374 696f 6e20 6f72  ble, function or
-00000fe0: 2063 6c61 7373 206e 616d 652e 0a62 6f64   class name..bod
-00000ff0: 7920 2d20 636f 6465 2062 6c6f 636b 2077  y - code block w
-00001000: 6869 6368 2066 6f6c 6c6f 7773 2061 6674  hich follows aft
-00001010: 6572 2060 3a60 2069 6e20 6675 6e63 7469  er `:` in functi
-00001020: 6f6e 206f 7220 636c 6173 7320 6465 6669  on or class defi
-00001030: 6e69 7469 6f6e 2e0a 6465 6669 6e69 7469  nition..definiti
-00001040: 6f6e 202d 2077 686f 6c65 2063 6c61 7373  on - whole class
-00001050: 206f 7220 6675 6e63 7469 6f6e 2064 6566   or function def
-00001060: 696e 6974 696f 6e20 6578 7072 6573 7369  inition expressi
-00001070: 6f6e 2069 6e63 6c75 6469 6e67 2069 7473  on including its
-00001080: 206e 616d 6520 616e 6420 626f 6479 2e0a   name and body..
-00001090: 0a0a 2323 2052 756c 6573 0a7c 2043 6f64  ..## Rules.| Cod
-000010a0: 6520 2020 7c20 4e61 6d65 2020 2020 2020  e   | Name      
-000010b0: 2020 2020 2020 2020 207c 204d 6573 7361           | Messa
-000010c0: 6765 2020 2020 2020 2020 7c0a 7c2d 2d2d  ge        |.|---
-000010d0: 2d2d 2d2d 2d7c 2d2d 2d2d 2d2d 2d2d 2d2d  -----|----------
-000010e0: 2d2d 2d2d 2d2d 2d2d 2d2d 7c2d 2d2d 2d2d  ----------|-----
-000010f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d7c 0a7c 2044  -----------|.| D
-00001100: 4330 3031 2020 7c20 756e 7573 6564 2d76  C001  | unused-v
-00001110: 6172 6961 626c 6520 2020 207c 2056 6172  ariable    | Var
-00001120: 6961 626c 6520 607b 6e61 6d65 7d60 2069  iable `{name}` i
-00001130: 7320 6e65 7665 7220 7573 6564 0a7c 2044  s never used.| D
-00001140: 4330 3032 2020 7c20 756e 7573 6564 2d66  C002  | unused-f
-00001150: 756e 6374 696f 6e20 2020 207c 2046 756e  unction    | Fun
-00001160: 6374 696f 6e20 607b 6e61 6d65 7d60 2069  ction `{name}` i
-00001170: 7320 6e65 7665 7220 7573 6564 0a7c 2044  s never used.| D
-00001180: 4330 3033 2020 7c20 756e 7573 6564 2d63  C003  | unused-c
-00001190: 6c61 7373 2020 2020 2020 207c 2043 6c61  lass       | Cla
-000011a0: 7373 2060 7b6e 616d 657d 6020 6973 206e  ss `{name}` is n
-000011b0: 6576 6572 2075 7365 640a 7c20 4443 3030  ever used.| DC00
-000011c0: 3420 207c 2075 6e75 7365 642d 6d65 7468  4  | unused-meth
-000011d0: 6f64 2020 2020 2020 7c20 4d65 7468 6f64  od      | Method
-000011e0: 2060 7b6e 616d 657d 6020 6973 206e 6576   `{name}` is nev
-000011f0: 6572 2075 7365 640a 7c20 4443 3030 3520  er used.| DC005 
-00001200: 207c 2075 6e75 7365 642d 6174 7472 6962   | unused-attrib
-00001210: 7574 6520 2020 7c20 4174 7472 6962 7574  ute   | Attribut
-00001220: 6520 607b 6e61 6d65 7d60 2069 7320 6e65  e `{name}` is ne
-00001230: 7665 7220 7573 6564 0a7c 2044 4330 3036  ver used.| DC006
-00001240: 2020 7c20 756e 7573 6564 2d6e 616d 6520    | unused-name 
-00001250: 2020 2020 2020 207c 204e 616d 6520 607b         | Name `{
-00001260: 6e61 6d65 7d60 2069 7320 6e65 7665 7220  name}` is never 
-00001270: 7573 6564 0a7c 2044 4330 3037 2020 7c20  used.| DC007  | 
-00001280: 756e 7573 6564 2d69 6d70 6f72 7420 2020  unused-import   
-00001290: 2020 207c 2049 6d70 6f72 7420 607b 6e61     | Import `{na
-000012a0: 6d65 7d60 2069 7320 6e65 7665 7220 7573  me}` is never us
-000012b0: 6564 0a7c 2044 4330 3038 2020 7c20 756e  ed.| DC008  | un
-000012c0: 7573 6564 2d70 726f 7065 7274 7920 2020  used-property   
-000012d0: 207c 2050 726f 7065 7274 7920 607b 6e61   | Property `{na
-000012e0: 6d65 7d60 2069 7320 6e65 7665 7220 7573  me}` is never us
-000012f0: 6564 0a7c 2044 4330 3039 2a20 7c20 756e  ed.| DC009* | un
-00001300: 7265 6163 6861 626c 652d 636f 6465 2020  reachable-code  
-00001310: 207c 2055 6e72 6561 6368 6162 6c65 2060   | Unreachable `
-00001320: 656c 7365 6020 626c 6f63 6b0a 7c20 4443  else` block.| DC
-00001330: 3031 3120 207c 2065 6d70 7479 2d66 696c  011  | empty-fil
-00001340: 6520 2020 2020 2020 2020 7c20 456d 7074  e         | Empt
-00001350: 7920 6669 6c65 0a7c 2044 4330 3132 2a20  y file.| DC012* 
-00001360: 7c20 636f 6d6d 656e 7465 642d 6f75 742d  | commented-out-
-00001370: 636f 6465 207c 2043 6f6d 6d65 6e74 6564  code | Commented
-00001380: 206f 7574 2063 6f64 650a 7c20 4443 3031   out code.| DC01
-00001390: 332a 207c 2069 676e 6f72 652d 6578 7072  3* | ignore-expr
-000013a0: 6573 7369 6f6e 2020 7c20 2a54 6869 7320  ession  | *This 
-000013b0: 6572 726f 7220 636f 6465 2063 616e 206f  error code can o
-000013c0: 6e79 2062 6520 7573 6564 2069 6e20 6023  ny be used in `#
-000013d0: 206e 6f71 613a 2044 4330 3133 6020 636f   noqa: DC013` co
-000013e0: 6d6d 656e 7473 2028 6e6f 2065 7272 6f72  mments (no error
-000013f0: 7320 7769 6c6c 2062 6520 7265 706f 7274  s will be report
-00001400: 6564 2066 6f72 2065 7870 7265 7373 696f  ed for expressio
-00001410: 6e20 7768 6963 6820 6265 6769 6e73 2069  n which begins i
-00001420: 6e20 6375 7272 656e 7420 6c69 6e65 292a  n current line)*
-00001430: 0a0a 602a 6020 2d20 6172 6520 6e6f 7420  ..`*` - are not 
-00001440: 7965 7420 696d 706c 656d 656e 7465 6420  yet implemented 
-00001450: 7275 6c65 732e 0a0a 2323 2049 676e 6f72  rules...## Ignor
-00001460: 696e 6720 6368 6563 6b73 2077 6974 6820  ing checks with 
-00001470: 6e6f 7161 2063 6f6d 6d65 6e74 730a 496e  noqa comments.In
-00001480: 6c69 6e65 2060 2320 6e6f 7161 6020 636f  line `# noqa` co
-00001490: 6d6d 656e 7473 2063 616e 2062 6520 7573  mments can be us
-000014a0: 6564 2074 6f20 6967 6e6f 7265 2060 6465  ed to ignore `de
-000014b0: 6164 636f 6465 6020 6368 6563 6b73 2e0a  adcode` checks..
-000014c0: 452e 672e 2075 6e75 7365 6420 6046 6f6f  E.g. unused `Foo
-000014d0: 6020 636c 6173 7320 776f 6e74 2062 6520  ` class wont be 
-000014e0: 6465 7465 6374 6564 2f66 6978 6564 2062  detected/fixed b
-000014f0: 6563 6175 7365 2060 2320 6e6f 7161 3a20  ecause `# noqa: 
-00001500: 4443 3030 3360 2063 6f6d 6d65 6e74 2069  DC003` comment i
-00001510: 7320 7573 6564 3a0a 0a60 6060 7079 7468  s used:..```pyth
-00001520: 6f6e 0a63 6c61 7373 2046 6f6f 3a20 2023  on.class Foo:  #
-00001530: 206e 6f71 613a 2044 4330 3033 0a20 2020   noqa: DC003.   
-00001540: 2070 6173 730a 6060 600a 0a23 2320 436f   pass.```..## Co
-00001550: 6e74 7269 6275 7469 6e67 0a2d 2060 6d61  ntributing.- `ma
-00001560: 6b65 2063 6865 636b 6020 2d20 7275 6e73  ke check` - runs
-00001570: 2075 6e69 7420 7465 7374 7320 616e 6420   unit tests and 
-00001580: 6f74 6865 7220 6368 6563 6b73 2075 7369  other checks usi
-00001590: 6e67 2076 6972 7475 616c 2065 6e76 6972  ng virtual envir
-000015a0: 6f6e 6d65 6e74 2e0a 0a23 2320 5261 7469  onment...## Rati
-000015b0: 6f6e 616c 650a 5b72 7566 665d 2868 7474  onale.[ruff](htt
-000015c0: 7073 3a2f 2f70 7970 692e 6f72 672f 7072  ps://pypi.org/pr
-000015d0: 6f6a 6563 742f 7275 6666 2f29 2061 6e64  oject/ruff/) and
-000015e0: 0a5b 666c 616b 6538 5d28 6874 7470 733a  .[flake8](https:
-000015f0: 2f2f 7079 7069 2e6f 7267 2f70 726f 6a65  //pypi.org/proje
-00001600: 6374 2f66 6c61 6b65 382f 2920 2d20 646f  ct/flake8/) - do
-00001610: 6e27 7420 6861 7665 2072 756c 6573 2066  n't have rules f
-00001620: 6f72 2075 6e75 7365 6420 676c 6f62 616c  or unused global
-00001630: 0a63 6f64 6520 6465 7465 6374 696f 6e2c  .code detection,
-00001640: 206f 6e6c 7920 666f 7220 6c6f 6361 6c20   only for local 
-00001650: 6f6e 6573 2060 4638 3233 602c 2060 4638  ones `F823`, `F8
-00001660: 3431 602c 2060 4638 3432 602e 2060 6465  41`, `F842`. `de
-00001670: 6164 636f 6465 6020 7061 636b 6167 650a  adcode` package.
-00001680: 7472 6965 7320 746f 2061 6464 206e 6577  tries to add new
-00001690: 2060 4443 5858 5860 2063 6865 636b 7320   `DCXXX` checks 
-000016a0: 666f 7220 6465 7465 6374 696e 6720 7661  for detecting va
-000016b0: 7269 6162 6c65 732f 6675 6e63 7469 6f6e  riables/function
-000016c0: 732f 636c 6173 7365 732f 6669 6c65 730a  s/classes/files.
-000016d0: 7768 6963 6820 6172 6520 6e6f 7420 7573  which are not us
-000016e0: 6564 2069 6e20 6120 7768 6f6c 6520 636f  ed in a whole co
-000016f0: 6465 2062 6173 652e 0a0a 6064 6561 6463  de base...`deadc
-00001700: 6f64 6560 202d 2069 7320 7375 7070 6f73  ode` - is suppos
-00001710: 6564 2074 6f20 6265 2075 7365 6420 696e  ed to be used in
-00001720: 6c69 6e65 2077 6974 6820 6f74 6865 7220  line with other 
-00001730: 7374 6174 6963 2063 6f64 6520 6368 6563  static code chec
-00001740: 6b65 7273 206c 696b 6520 6072 7566 6660  kers like `ruff`
-00001750: 2e0a 0a54 6865 7265 2069 7320 616e 2061  ...There is an a
-00001760: 6c74 6572 6e61 7469 7665 205b 7675 6c74  lternative [vult
-00001770: 7572 655d 2868 7474 7073 3a2f 2f70 7970  ure](https://pyp
-00001780: 692e 6f72 672f 7072 6f6a 6563 742f 7675  i.org/project/vu
-00001790: 6c74 7572 652f 2920 7061 636b 6167 652e  lture/) package.
-000017a0: 0a0a 2323 204b 6e6f 776e 206c 696d 6974  ..## Known limit
-000017b0: 6174 696f 6e73 0a49 6e20 6361 7365 2074  ations.In case t
-000017c0: 6865 7265 2061 7265 2073 6576 6572 616c  here are several
-000017d0: 2064 6566 696e 6974 696f 6e73 2075 7369   definitions usi
-000017e0: 6e67 2074 6865 2073 616d 6520 6e61 6d65  ng the same name
-000017f0: 202d 2074 6865 7920 616c 6c20 776f 6e74   - they all wont
-00001800: 2062 650a 7265 706f 7274 6564 2069 6620   be.reported if 
-00001810: 6174 206c 6561 7374 206f 6e65 2075 7361  at least one usa
-00001820: 6765 206f 6620 7468 6174 206e 616d 6520  ge of that name 
-00001830: 6973 2062 6569 6e67 2064 6574 6563 7465  is being detecte
-00001840: 642e 0a0a 4669 6c65 7320 7769 7468 2073  d...Files with s
-00001850: 796e 7461 7820 6572 726f 7273 2077 696c  yntax errors wil
-00001860: 6c20 6265 2069 676e 6f72 6564 2c20 6265  l be ignored, be
-00001870: 6361 7573 6520 6064 6561 6463 6f64 6560  cause `deadcode`
-00001880: 2075 7365 7320 6061 7374 6020 746f 0a62   uses `ast` to.b
-00001890: 7569 6c64 2061 6273 7472 6163 7420 7379  uild abstract sy
-000018a0: 6e74 6178 2074 7265 6520 666f 7220 6e61  ntax tree for na
-000018b0: 6d65 2075 7361 6765 2064 6574 6563 7469  me usage detecti
-000018c0: 6f6e 2e0a 0a49 7420 6973 2061 7373 756d  on...It is assum
-000018d0: 6564 2074 6861 7420 6064 6561 6463 6f64  ed that `deadcod
-000018e0: 6560 2077 696c 6c20 6265 2072 756e 2075  e` will be run u
-000018f0: 7369 6e67 2074 6865 2073 616d 6520 6f72  sing the same or
-00001900: 2068 6967 6865 7220 5079 7468 6f6e 2076   higher Python v
-00001910: 6572 7369 6f6e 2061 7320 7468 650a 636f  ersion as the.co
-00001920: 6465 2062 6173 6520 6973 2069 6d70 6c65  de base is imple
-00001930: 6d65 6e74 6564 2069 6e2e 0a0a 2323 2046  mented in...## F
-00001940: 6561 7475 7265 2072 6571 7565 7374 730a  eature requests.
-00001950: 2d20 5b78 5d20 5265 706c 6163 6520 602e  - [x] Replace `.
-00001960: 2a60 2077 6974 6820 6f6e 6c79 2060 2a60  *` with only `*`
-00001970: 2069 6e20 7265 6765 7870 206d 6174 6368   in regexp match
-00001980: 696e 672e 0a2d 205b 785d 2041 6464 2075  ing..- [x] Add u
-00001990: 6e75 7365 6420 636c 6173 7320 6d65 7468  nused class meth
-000019a0: 6f64 2064 6574 6563 7469 6f6e 2044 4330  od detection DC0
-000019b0: 3034 2063 6865 636b 2e0a 2d20 5b78 5d20  04 check..- [x] 
-000019c0: 4164 6420 602d 2d66 6978 6020 6f70 7469  Add `--fix` opti
-000019d0: 6f6e 2074 6f20 6175 746f 6d61 7469 6361  on to automatica
-000019e0: 6c6c 7920 7265 6d6f 7665 2064 6574 6563  lly remove detec
-000019f0: 7465 6420 6465 6164 2063 6f64 6520 6f63  ted dead code oc
-00001a00: 636f 7572 656e 6369 6573 0a2d 205b 785d  courencies.- [x]
-00001a10: 2041 6464 2061 2063 6865 636b 2066 6f72   Add a check for
-00001a20: 2065 6d70 7479 2070 7974 686f 6e20 6669   empty python fi
-00001a30: 6c65 732e 0a2d 205b 785d 2053 706c 6974  les..- [x] Split
-00001a40: 2065 7272 6f72 2063 6f64 6573 2069 6e74   error codes int
-00001a50: 6f20 4443 3030 312c 2044 4330 3032 2c20  o DC001, DC002, 
-00001a60: 4443 3030 3320 666f 7220 7661 7269 6162  DC003 for variab
-00001a70: 6c65 732c 2066 756e 6374 696f 6e73 2c20  les, functions, 
-00001a80: 636c 6173 732e 0a20 2020 202d 205b 785d  class..    - [x]
-00001a90: 2053 686f 756c 6420 6861 7665 2064 6966   Should have dif
-00001aa0: 6665 7265 6e74 2063 6f64 6573 2066 6f72  ferent codes for
-00001ab0: 2069 676e 6f72 696e 6720 6e61 6d65 2061   ignoring name a
-00001ac0: 6e64 2069 676e 6f72 696e 6720 7768 6f6c  nd ignoring whol
-00001ad0: 6520 6465 6669 6e69 7469 6f6e 2028 7265  e definition (re
-00001ae0: 7365 7276 6564 2044 4378 7830 202d 2069  served DCxx0 - i
-00001af0: 676e 6f72 6520 6e61 6d65 2c20 4443 7878  gnore name, DCxx
-00001b00: 3120 2d20 6967 6e6f 7265 2064 6566 696e  1 - ignore defin
-00001b10: 6974 696f 6e29 2e0a 2020 2020 2d20 5b20  ition)..    - [ 
-00001b20: 5d20 416c 6c6f 7720 746f 2064 6973 6162  ] Allow to disab
-00001b30: 6c65 2065 6163 6820 6368 6563 6b20 7365  le each check se
-00001b40: 7061 7261 7465 6c79 2075 7369 6e67 3a0a  parately using:.
-00001b50: 2020 2020 2020 2020 2d20 5b20 5d20 696e          - [ ] in
-00001b60: 6c69 6e65 2063 6f6d 6d65 6e74 2e0a 2020  line comment..  
-00001b70: 2020 2020 2020 2d20 5b20 5d20 7079 7072        - [ ] pypr
-00001b80: 6f6a 6563 742e 746f 6d6c 2066 696c 650a  oject.toml file.
-00001b90: 2d20 5b20 5d20 4164 6420 6120 6368 6563  - [ ] Add a chec
-00001ba0: 6b20 666f 7220 636f 6465 2069 6e20 636f  k for code in co
-00001bb0: 6d6d 656e 7473 2e0a 2d20 5b20 5d20 4164  mments..- [ ] Ad
-00001bc0: 6420 7461 7267 6574 2070 7974 686f 6e20  d target python 
-00001bd0: 7665 7273 696f 6e20 6f70 7469 6f6e 2c20  version option, 
-00001be0: 6966 2073 7065 6369 6669 6564 2069 7420  if specified it 
-00001bf0: 7769 6c6c 2062 6520 7573 6564 2066 6f72  will be used for
-00001c00: 2063 6f64 6520 6261 7365 2063 6865 636b   code base check
-00001c10: 2e0a 2d20 5b20 5d20 4164 6420 6120 602d  ..- [ ] Add a `-
-00001c20: 2d64 6570 7468 6020 7061 7261 6d65 7465  -depth` paramete
-00001c30: 7220 746f 2069 676e 6f72 6520 6e65 7374  r to ignore nest
-00001c40: 6564 2063 6f64 652e 2e20 2854 6f20 6f6e  ed code.. (To on
-00001c50: 6c79 2063 6865 636b 2067 6c6f 6261 6c20  ly check global 
-00001c60: 7363 6f70 6520 7573 6520 3029 2e0a 2d20  scope use 0)..- 
-00001c70: 5b20 5d20 4164 6420 6f70 7469 6f6e 733a  [ ] Add options:
-00001c80: 0a20 2020 202d 205b 785d 202d 2d69 676e  .    - [x] --ign
-00001c90: 6f72 652d 6465 6669 6e69 7469 6f6e 730a  ore-definitions.
-00001ca0: 2020 2020 2d20 5b78 5d20 2d2d 6967 6e6f      - [x] --igno
-00001cb0: 7265 2d64 6566 696e 6974 696f 6e73 2d69  re-definitions-i
-00001cc0: 662d 696e 6865 7269 7473 2d66 726f 6d0a  f-inherits-from.
-00001cd0: 2020 2020 2d20 5b20 5d20 2d2d 6967 6e6f      - [ ] --igno
-00001ce0: 7265 2d64 6566 696e 6974 696f 6e73 2d69  re-definitions-i
-00001cf0: 662d 6465 636f 7261 7465 642d 7769 7468  f-decorated-with
-00001d00: 0a20 2020 202d 205b 205d 202d 2d69 676e  .    - [ ] --ign
-00001d10: 6f72 652d 6e61 6d65 732d 6966 2d69 6e68  ore-names-if-inh
-00001d20: 6572 6974 732d 6672 6f6d 0a20 2020 202d  erits-from.    -
-00001d30: 205b 205d 202d 2d69 676e 6f72 652d 6e61   [ ] --ignore-na
-00001d40: 6d65 732d 6966 2d64 6563 6f72 6174 6564  mes-if-decorated
-00001d50: 2d77 6974 680a 2d20 5b20 5d20 4469 7374  -with.- [ ] Dist
-00001d60: 696e 6775 6973 6820 6265 7477 6565 6e20  inguish between 
-00001d70: 6465 6669 6e69 7469 6f6e 7320 7769 7468  definitions with
-00001d80: 2073 616d 6520 6e61 6d65 2c20 6275 7420   same name, but 
-00001d90: 6469 6666 6572 656e 7420 6669 6c65 732e  different files.
-00001da0: 0a2d 205b 205d 2052 6570 6561 7465 6420  .- [ ] Repeated 
-00001db0: 6170 706c 6963 6174 696f 6e20 6f66 2060  application of `
-00001dc0: 6465 6164 636f 6465 6020 7469 6c6c 2074  deadcode` till t
-00001dd0: 6865 206f 7574 7075 7420 7374 6f70 7320  he output stops 
-00001de0: 6368 616e 6769 6e67 2e0a 2d20 5b20 5d20  changing..- [ ] 
-00001df0: 556e 7265 6163 6861 626c 6520 636f 6465  Unreachable code
-00001e00: 2064 6574 6563 7469 6f6e 2061 6e64 2066   detection and f
-00001e10: 6978 696e 672e 0a2d 205b 205d 2060 2d2d  ixing..- [ ] `--
-00001e20: 6669 7820 2d2d 6472 7920 5b66 696c 656e  fix --dry [filen
-00001e30: 616d 6573 5d60 202d 206f 6e6c 7920 7368  ames]` - only sh
-00001e40: 6f77 2077 6861 7473 2061 626f 7574 2074  ow whats about t
-00001e50: 6f20 6368 616e 6765 2069 6e20 7468 6520  o change in the 
-00001e60: 6c69 7374 6564 2066 696c 656e 616d 6573  listed filenames
-00001e70: 2e0a 2d20 5b20 5d20 4265 6e63 686d 6172  ..- [ ] Benchmar
-00001e80: 6b69 6e67 2070 6572 666f 726d 616e 6365  king performance
-00001e90: 2077 6974 6820 6c61 7267 6572 2070 726f   with larger pro
-00001ea0: 6a65 6374 7320 2874 696d 652c 2043 5055  jects (time, CPU
-00001eb0: 2061 6e64 206d 656d 6f72 7920 636f 6e73   and memory cons
-00001ec0: 756d 7074 696f 6e29 2069 6e20 6f72 6465  umption) in orde
-00001ed0: 7220 746f 206f 7074 696d 697a 652e 0a    r to optimize..
+00000ec0: 2020 207c 202d 2020 2020 7c20 5265 6d6f     | -    | Remo
+00000ed0: 7665 7320 636f 6c6f 7273 2066 726f 6d20  ves colors from 
+00000ee0: 7468 6520 6f75 7470 7574 2e20 7c0a 7c60  the output. |.|`
+00000ef0: 2d2d 636f 756e 7460 2020 2020 2020 2020  --count`        
+00000f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000f10: 2020 2020 2020 2020 2020 7c20 2d20 2020            | -   
+00000f20: 207c 2050 726f 7669 6465 7320 7468 6520   | Provides the 
+00000f30: 636f 756e 7420 6f66 2074 6865 2064 6574  count of the det
+00000f40: 6563 7465 6420 756e 7573 6564 206e 616d  ected unused nam
+00000f50: 6573 2069 6e73 7465 6164 206f 6620 7072  es instead of pr
+00000f60: 696e 7469 6e67 2074 6865 6d20 616c 6c20  inting them all 
+00000f70: 6f75 742e 207c 0a7c 602d 2d71 7569 6574  out. |.|`--quiet
+00000f80: 6020 2020 2020 2020 2020 2020 2020 2020  `               
+00000f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000fa0: 2020 207c 202d 2020 2020 7c20 446f 6573     | -    | Does
+00000fb0: 206e 6f74 206f 7574 7075 7420 616e 7974   not output anyt
+00000fc0: 6869 6e67 2e20 4d61 6b65 6669 6c65 2073  hing. Makefile s
+00000fd0: 7469 6c6c 2066 6169 6c73 2077 6974 6820  till fails with 
+00000fe0: 6578 6974 2063 6f64 6520 3120 6966 2075  exit code 1 if u
+00000ff0: 6e75 7365 6420 6e61 6d65 7320 6172 6520  nused names are 
+00001000: 666f 756e 642e 207c 0a0a 0a23 2323 2323  found. |...#####
+00001010: 2047 6c6f 7373 6f72 790a 6e61 6d65 202d   Glossory.name -
+00001020: 2076 6172 6961 626c 652c 2066 756e 6374   variable, funct
+00001030: 696f 6e20 6f72 2063 6c61 7373 206e 616d  ion or class nam
+00001040: 652e 0a62 6f64 7920 2d20 636f 6465 2062  e..body - code b
+00001050: 6c6f 636b 2077 6869 6368 2066 6f6c 6c6f  lock which follo
+00001060: 7773 2061 6674 6572 2060 3a60 2069 6e20  ws after `:` in 
+00001070: 6675 6e63 7469 6f6e 206f 7220 636c 6173  function or clas
+00001080: 7320 6465 6669 6e69 7469 6f6e 2e0a 6465  s definition..de
+00001090: 6669 6e69 7469 6f6e 202d 2077 686f 6c65  finition - whole
+000010a0: 2063 6c61 7373 206f 7220 6675 6e63 7469   class or functi
+000010b0: 6f6e 2064 6566 696e 6974 696f 6e20 6578  on definition ex
+000010c0: 7072 6573 7369 6f6e 2069 6e63 6c75 6469  pression includi
+000010d0: 6e67 2069 7473 206e 616d 6520 616e 6420  ng its name and 
+000010e0: 626f 6479 2e0a 0a0a 2323 2052 756c 6573  body....## Rules
+000010f0: 0a7c 2043 6f64 6520 2020 7c20 4e61 6d65  .| Code   | Name
+00001100: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+00001110: 204d 6573 7361 6765 2020 2020 2020 2020   Message        
+00001120: 7c0a 7c2d 2d2d 2d2d 2d2d 2d7c 2d2d 2d2d  |.|--------|----
+00001130: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001140: 7c2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  |---------------
+00001150: 2d7c 0a7c 2044 4330 3120 207c 2075 6e75  -|.| DC01  | unu
+00001160: 7365 642d 7661 7269 6162 6c65 2020 2020  sed-variable    
+00001170: 2020 7c20 5661 7269 6162 6c65 2060 7b6e    | Variable `{n
+00001180: 616d 657d 6020 6973 206e 6576 6572 2075  ame}` is never u
+00001190: 7365 640a 7c20 4443 3032 2020 7c20 756e  sed.| DC02  | un
+000011a0: 7573 6564 2d66 756e 6374 696f 6e20 2020  used-function   
+000011b0: 2020 207c 2046 756e 6374 696f 6e20 607b     | Function `{
+000011c0: 6e61 6d65 7d60 2069 7320 6e65 7665 7220  name}` is never 
+000011d0: 7573 6564 0a7c 2044 4330 3320 207c 2075  used.| DC03  | u
+000011e0: 6e75 7365 642d 636c 6173 7320 2020 2020  nused-class     
+000011f0: 2020 2020 7c20 436c 6173 7320 607b 6e61      | Class `{na
+00001200: 6d65 7d60 2069 7320 6e65 7665 7220 7573  me}` is never us
+00001210: 6564 0a7c 2044 4330 3420 207c 2075 6e75  ed.| DC04  | unu
+00001220: 7365 642d 6d65 7468 6f64 2020 2020 2020  sed-method      
+00001230: 2020 7c20 4d65 7468 6f64 2060 7b6e 616d    | Method `{nam
+00001240: 657d 6020 6973 206e 6576 6572 2075 7365  e}` is never use
+00001250: 640a 7c20 4443 3035 2020 7c20 756e 7573  d.| DC05  | unus
+00001260: 6564 2d61 7474 7269 6275 7465 2020 2020  ed-attribute    
+00001270: 207c 2041 7474 7269 6275 7465 2060 7b6e   | Attribute `{n
+00001280: 616d 657d 6020 6973 206e 6576 6572 2075  ame}` is never u
+00001290: 7365 640a 7c20 4443 3036 2020 7c20 756e  sed.| DC06  | un
+000012a0: 7573 6564 2d6e 616d 6520 2020 2020 2020  used-name       
+000012b0: 2020 207c 204e 616d 6520 607b 6e61 6d65     | Name `{name
+000012c0: 7d60 2069 7320 6e65 7665 7220 7573 6564  }` is never used
+000012d0: 0a7c 2044 4330 3720 207c 2075 6e75 7365  .| DC07  | unuse
+000012e0: 642d 696d 706f 7274 2020 2020 2020 2020  d-import        
+000012f0: 7c20 496d 706f 7274 2060 7b6e 616d 657d  | Import `{name}
+00001300: 6020 6973 206e 6576 6572 2075 7365 640a  ` is never used.
+00001310: 7c20 4443 3038 2020 7c20 756e 7573 6564  | DC08  | unused
+00001320: 2d70 726f 7065 7274 7920 2020 2020 207c  -property      |
+00001330: 2050 726f 7065 7274 7920 607b 6e61 6d65   Property `{name
+00001340: 7d60 2069 7320 6e65 7665 7220 7573 6564  }` is never used
+00001350: 0a7c 2044 4330 3920 207c 2075 6e72 6561  .| DC09  | unrea
+00001360: 6368 6162 6c65 2d69 662d 626c 6f63 6b20  chable-if-block 
+00001370: 7c20 556e 7265 6163 6861 626c 6520 636f  | Unreachable co
+00001380: 6e64 6974 696f 6e61 6c20 7374 6174 656d  nditional statem
+00001390: 656e 7420 626c 6f63 6b0a 7c20 4443 3131  ent block.| DC11
+000013a0: 2020 7c20 656d 7074 792d 6669 6c65 2020    | empty-file  
+000013b0: 2020 2020 2020 2020 207c 2045 6d70 7479           | Empty
+000013c0: 2050 7974 686f 6e20 6669 6c65 0a7c 2044   Python file.| D
+000013d0: 4331 3220 207c 2063 6f6d 6d65 6e74 6564  C12  | commented
+000013e0: 2d6f 7574 2d63 6f64 6520 2020 7c20 436f  -out-code   | Co
+000013f0: 6d6d 656e 7465 6420 6f75 7420 636f 6465  mmented out code
+00001400: 0a7c 2044 4331 3320 207c 2075 6e72 6561  .| DC13  | unrea
+00001410: 6368 6162 6c65 2d63 6f64 6520 2020 2020  chable-code     
+00001420: 7c20 436f 6465 2061 6674 6572 2074 6572  | Code after ter
+00001430: 6d69 6e61 6c20 7374 6174 656d 656e 742c  minal statement,
+00001440: 2065 2e67 2e20 6072 6574 7572 6e60 2c20   e.g. `return`, 
+00001450: 6072 6169 7365 602c 2060 636f 6e74 696e  `raise`, `contin
+00001460: 7565 602c 2060 6272 6561 6b60 0a7c 2044  ue`, `break`.| D
+00001470: 4320 2020 207c 2069 676e 6f72 652d 6578  C    | ignore-ex
+00001480: 7072 6573 7369 6f6e 2020 2020 7c20 446f  pression    | Do
+00001490: 206e 6f74 2073 686f 7720 616e 7920 6669   not show any fi
+000014a0: 6e64 696e 6773 2066 6f72 2061 6e20 6578  ndings for an ex
+000014b0: 7072 6573 7369 6f6e 2c20 7768 6963 6820  pression, which 
+000014c0: 7374 6172 7473 206f 6e20 6375 7272 656e  starts on curren
+000014d0: 7420 6c69 6e65 2028 7468 6973 2063 6f64  t line (this cod
+000014e0: 6520 6361 6e20 6f6e 6c79 2062 6520 7573  e can only be us
+000014f0: 6564 2069 6e20 6023 206e 6f71 613a 2044  ed in `# noqa: D
+00001500: 4360 2063 6f6d 6d65 6e74 7329 0a0a 2323  C` comments)..##
+00001510: 2049 676e 6f72 696e 6720 6368 6563 6b73   Ignoring checks
+00001520: 2077 6974 6820 6e6f 7161 2063 6f6d 6d65   with noqa comme
+00001530: 6e74 730a 496e 6c69 6e65 2060 2320 6e6f  nts.Inline `# no
+00001540: 7161 6020 636f 6d6d 656e 7473 2063 616e  qa` comments can
+00001550: 2062 6520 7573 6564 2074 6f20 6967 6e6f   be used to igno
+00001560: 7265 2060 6465 6164 636f 6465 6020 6368  re `deadcode` ch
+00001570: 6563 6b73 2e0a 452e 672e 2075 6e75 7365  ecks..E.g. unuse
+00001580: 6420 6046 6f6f 6020 636c 6173 7320 776f  d `Foo` class wo
+00001590: 6e74 2062 6520 6465 7465 6374 6564 2f66  nt be detected/f
+000015a0: 6978 6564 2062 6563 6175 7365 2060 2320  ixed because `# 
+000015b0: 6e6f 7161 3a20 4443 3033 6020 636f 6d6d  noqa: DC03` comm
+000015c0: 656e 7420 6973 2075 7365 643a 0a0a 6060  ent is used:..``
+000015d0: 6070 7974 686f 6e0a 636c 6173 7320 466f  `python.class Fo
+000015e0: 6f3a 2020 2320 6e6f 7161 3a20 4443 3033  o:  # noqa: DC03
+000015f0: 0a20 2020 2070 6173 730a 6060 600a 0a23  .    pass.```..#
+00001600: 2320 436f 6e74 7269 6275 7469 6e67 0a2d  # Contributing.-
+00001610: 2060 6d61 6b65 2063 6865 636b 6020 2d20   `make check` - 
+00001620: 7275 6e73 2075 6e69 7420 7465 7374 7320  runs unit tests 
+00001630: 616e 6420 6f74 6865 7220 6368 6563 6b73  and other checks
+00001640: 2075 7369 6e67 2076 6972 7475 616c 2065   using virtual e
+00001650: 6e76 6972 6f6e 6d65 6e74 2e0a 0a23 2320  nvironment...## 
+00001660: 5261 7469 6f6e 616c 650a 5b72 7566 665d  Rationale.[ruff]
+00001670: 2868 7474 7073 3a2f 2f70 7970 692e 6f72  (https://pypi.or
+00001680: 672f 7072 6f6a 6563 742f 7275 6666 2f29  g/project/ruff/)
+00001690: 2061 6e64 0a5b 666c 616b 6538 5d28 6874   and.[flake8](ht
+000016a0: 7470 733a 2f2f 7079 7069 2e6f 7267 2f70  tps://pypi.org/p
+000016b0: 726f 6a65 6374 2f66 6c61 6b65 382f 2920  roject/flake8/) 
+000016c0: 2d20 646f 6e27 7420 6861 7665 2072 756c  - don't have rul
+000016d0: 6573 2066 6f72 2075 6e75 7365 6420 676c  es for unused gl
+000016e0: 6f62 616c 0a63 6f64 6520 6465 7465 6374  obal.code detect
+000016f0: 696f 6e2c 206f 6e6c 7920 666f 7220 6c6f  ion, only for lo
+00001700: 6361 6c20 6f6e 6573 2060 4638 3233 602c  cal ones `F823`,
+00001710: 2060 4638 3431 602c 2060 4638 3432 602e   `F841`, `F842`.
+00001720: 2060 6465 6164 636f 6465 6020 7061 636b   `deadcode` pack
+00001730: 6167 650a 7472 6965 7320 746f 2061 6464  age.tries to add
+00001740: 206e 6577 2060 4443 5858 5860 2063 6865   new `DCXXX` che
+00001750: 636b 7320 666f 7220 6465 7465 6374 696e  cks for detectin
+00001760: 6720 7661 7269 6162 6c65 732f 6675 6e63  g variables/func
+00001770: 7469 6f6e 732f 636c 6173 7365 732f 6669  tions/classes/fi
+00001780: 6c65 730a 7768 6963 6820 6172 6520 6e6f  les.which are no
+00001790: 7420 7573 6564 2069 6e20 6120 7768 6f6c  t used in a whol
+000017a0: 6520 636f 6465 2062 6173 652e 0a0a 6064  e code base...`d
+000017b0: 6561 6463 6f64 6560 202d 2069 7320 7375  eadcode` - is su
+000017c0: 7070 6f73 6564 2074 6f20 6265 2075 7365  pposed to be use
+000017d0: 6420 696e 6c69 6e65 2077 6974 6820 6f74  d inline with ot
+000017e0: 6865 7220 7374 6174 6963 2063 6f64 6520  her static code 
+000017f0: 6368 6563 6b65 7273 206c 696b 6520 6072  checkers like `r
+00001800: 7566 6660 2e0a 0a54 6865 7265 2069 7320  uff`...There is 
+00001810: 616e 2061 6c74 6572 6e61 7469 7665 205b  an alternative [
+00001820: 7675 6c74 7572 655d 2868 7474 7073 3a2f  vulture](https:/
+00001830: 2f70 7970 692e 6f72 672f 7072 6f6a 6563  /pypi.org/projec
+00001840: 742f 7675 6c74 7572 652f 2920 7061 636b  t/vulture/) pack
+00001850: 6167 652e 0a0a 2323 204b 6e6f 776e 206c  age...## Known l
+00001860: 696d 6974 6174 696f 6e73 0a49 6e20 6361  imitations.In ca
+00001870: 7365 2074 6865 7265 2061 7265 2073 6576  se there are sev
+00001880: 6572 616c 2064 6566 696e 6974 696f 6e73  eral definitions
+00001890: 2075 7369 6e67 2074 6865 2073 616d 6520   using the same 
+000018a0: 6e61 6d65 202d 2074 6865 7920 616c 6c20  name - they all 
+000018b0: 776f 6e74 2062 650a 7265 706f 7274 6564  wont be.reported
+000018c0: 2069 6620 6174 206c 6561 7374 206f 6e65   if at least one
+000018d0: 2075 7361 6765 206f 6620 7468 6174 206e   usage of that n
+000018e0: 616d 6520 6973 2062 6569 6e67 2064 6574  ame is being det
+000018f0: 6563 7465 642e 0a0a 4669 6c65 7320 7769  ected...Files wi
+00001900: 7468 2073 796e 7461 7820 6572 726f 7273  th syntax errors
+00001910: 2077 696c 6c20 6265 2069 676e 6f72 6564   will be ignored
+00001920: 2c20 6265 6361 7573 6520 6064 6561 6463  , because `deadc
+00001930: 6f64 6560 2075 7365 7320 6061 7374 6020  ode` uses `ast` 
+00001940: 746f 0a62 7569 6c64 2061 6273 7472 6163  to.build abstrac
+00001950: 7420 7379 6e74 6178 2074 7265 6520 666f  t syntax tree fo
+00001960: 7220 6e61 6d65 2075 7361 6765 2064 6574  r name usage det
+00001970: 6563 7469 6f6e 2e0a 0a49 7420 6973 2061  ection...It is a
+00001980: 7373 756d 6564 2074 6861 7420 6064 6561  ssumed that `dea
+00001990: 6463 6f64 6560 2077 696c 6c20 6265 2072  dcode` will be r
+000019a0: 756e 2075 7369 6e67 2074 6865 2073 616d  un using the sam
+000019b0: 6520 6f72 2068 6967 6865 7220 5079 7468  e or higher Pyth
+000019c0: 6f6e 2076 6572 7369 6f6e 2061 7320 7468  on version as th
+000019d0: 650a 636f 6465 2062 6173 6520 6973 2069  e.code base is i
+000019e0: 6d70 6c65 6d65 6e74 6564 2069 6e2e 0a0a  mplemented in...
+000019f0: 2323 2046 6561 7475 7265 2072 6571 7565  ## Feature reque
+00001a00: 7374 730a 2d20 5b78 5d20 5265 706c 6163  sts.- [x] Replac
+00001a10: 6520 602e 2a60 2077 6974 6820 6f6e 6c79  e `.*` with only
+00001a20: 2060 2a60 2069 6e20 7265 6765 7870 206d   `*` in regexp m
+00001a30: 6174 6368 696e 672e 0a2d 205b 785d 2041  atching..- [x] A
+00001a40: 6464 2075 6e75 7365 6420 636c 6173 7320  dd unused class 
+00001a50: 6d65 7468 6f64 2064 6574 6563 7469 6f6e  method detection
+00001a60: 2044 4330 3420 6368 6563 6b2e 0a2d 205b   DC04 check..- [
+00001a70: 785d 2041 6464 2060 2d2d 6669 7860 206f  x] Add `--fix` o
+00001a80: 7074 696f 6e20 746f 2061 7574 6f6d 6174  ption to automat
+00001a90: 6963 616c 6c79 2072 656d 6f76 6520 6465  ically remove de
+00001aa0: 7465 6374 6564 2064 6561 6420 636f 6465  tected dead code
+00001ab0: 206f 6363 6f75 7265 6e63 6965 730a 2d20   occourencies.- 
+00001ac0: 5b78 5d20 4164 6420 6120 6368 6563 6b20  [x] Add a check 
+00001ad0: 666f 7220 656d 7074 7920 7079 7468 6f6e  for empty python
+00001ae0: 2066 696c 6573 2e0a 2d20 5b78 5d20 5370   files..- [x] Sp
+00001af0: 6c69 7420 6572 726f 7220 636f 6465 7320  lit error codes 
+00001b00: 696e 746f 2044 4330 312c 2044 4330 322c  into DC01, DC02,
+00001b10: 2044 4330 3320 666f 7220 7661 7269 6162   DC03 for variab
+00001b20: 6c65 732c 2066 756e 6374 696f 6e73 2c20  les, functions, 
+00001b30: 636c 6173 732e 0a20 2020 202d 205b 785d  class..    - [x]
+00001b40: 2053 686f 756c 6420 6861 7665 2064 6966   Should have dif
+00001b50: 6665 7265 6e74 2063 6f64 6573 2066 6f72  ferent codes for
+00001b60: 2069 676e 6f72 696e 6720 6e61 6d65 2061   ignoring name a
+00001b70: 6e64 2069 676e 6f72 696e 6720 7768 6f6c  nd ignoring whol
+00001b80: 6520 6465 6669 6e69 7469 6f6e 2028 7265  e definition (re
+00001b90: 7365 7276 6564 2044 4378 7830 202d 2069  served DCxx0 - i
+00001ba0: 676e 6f72 6520 6e61 6d65 2c20 4443 7878  gnore name, DCxx
+00001bb0: 3120 2d20 6967 6e6f 7265 2064 6566 696e  1 - ignore defin
+00001bc0: 6974 696f 6e29 2e0a 2020 2020 2d20 5b20  ition)..    - [ 
+00001bd0: 5d20 416c 6c6f 7720 746f 2064 6973 6162  ] Allow to disab
+00001be0: 6c65 2065 6163 6820 6368 6563 6b20 7365  le each check se
+00001bf0: 7061 7261 7465 6c79 2075 7369 6e67 3a0a  parately using:.
+00001c00: 2020 2020 2020 2020 2d20 5b20 5d20 696e          - [ ] in
+00001c10: 6c69 6e65 2063 6f6d 6d65 6e74 2e0a 2020  line comment..  
+00001c20: 2020 2020 2020 2d20 5b20 5d20 7079 7072        - [ ] pypr
+00001c30: 6f6a 6563 742e 746f 6d6c 2066 696c 650a  oject.toml file.
+00001c40: 2d20 5b20 5d20 4164 6420 6120 6368 6563  - [ ] Add a chec
+00001c50: 6b20 666f 7220 636f 6465 2069 6e20 636f  k for code in co
+00001c60: 6d6d 656e 7473 2e0a 2d20 5b20 5d20 4164  mments..- [ ] Ad
+00001c70: 6420 7461 7267 6574 2070 7974 686f 6e20  d target python 
+00001c80: 7665 7273 696f 6e20 6f70 7469 6f6e 2c20  version option, 
+00001c90: 6966 2073 7065 6369 6669 6564 2069 7420  if specified it 
+00001ca0: 7769 6c6c 2062 6520 7573 6564 2066 6f72  will be used for
+00001cb0: 2063 6f64 6520 6261 7365 2063 6865 636b   code base check
+00001cc0: 2e0a 2d20 5b20 5d20 4164 6420 6120 602d  ..- [ ] Add a `-
+00001cd0: 2d64 6570 7468 6020 7061 7261 6d65 7465  -depth` paramete
+00001ce0: 7220 746f 2069 676e 6f72 6520 6e65 7374  r to ignore nest
+00001cf0: 6564 2063 6f64 652e 2e20 2854 6f20 6f6e  ed code.. (To on
+00001d00: 6c79 2063 6865 636b 2067 6c6f 6261 6c20  ly check global 
+00001d10: 7363 6f70 6520 7573 6520 3029 2e0a 2d20  scope use 0)..- 
+00001d20: 5b20 5d20 4164 6420 6f70 7469 6f6e 733a  [ ] Add options:
+00001d30: 0a20 2020 202d 205b 785d 202d 2d69 676e  .    - [x] --ign
+00001d40: 6f72 652d 6465 6669 6e69 7469 6f6e 730a  ore-definitions.
+00001d50: 2020 2020 2d20 5b78 5d20 2d2d 6967 6e6f      - [x] --igno
+00001d60: 7265 2d64 6566 696e 6974 696f 6e73 2d69  re-definitions-i
+00001d70: 662d 696e 6865 7269 7473 2d66 726f 6d0a  f-inherits-from.
+00001d80: 2020 2020 2d20 5b20 5d20 2d2d 6967 6e6f      - [ ] --igno
+00001d90: 7265 2d64 6566 696e 6974 696f 6e73 2d69  re-definitions-i
+00001da0: 662d 6465 636f 7261 7465 642d 7769 7468  f-decorated-with
+00001db0: 0a20 2020 202d 205b 205d 202d 2d69 676e  .    - [ ] --ign
+00001dc0: 6f72 652d 6e61 6d65 732d 6966 2d69 6e68  ore-names-if-inh
+00001dd0: 6572 6974 732d 6672 6f6d 0a20 2020 202d  erits-from.    -
+00001de0: 205b 205d 202d 2d69 676e 6f72 652d 6e61   [ ] --ignore-na
+00001df0: 6d65 732d 6966 2d64 6563 6f72 6174 6564  mes-if-decorated
+00001e00: 2d77 6974 680a 2020 2020 2d20 5b20 5d20  -with.    - [ ] 
+00001e10: 2d2d 6967 6e6f 7265 2d62 6f64 6965 732d  --ignore-bodies-
+00001e20: 6f66 0a20 2020 202d 205b 205d 202d 2d69  of.    - [ ] --i
+00001e30: 676e 6f72 652d 626f 6469 6573 2d69 662d  gnore-bodies-if-
+00001e40: 6465 636f 7261 7465 642d 7769 7468 0a20  decorated-with. 
+00001e50: 2020 202d 205b 205d 202d 2d69 676e 6f72     - [ ] --ignor
+00001e60: 652d 626f 6469 6573 2d69 662d 696e 6865  e-bodies-if-inhe
+00001e70: 7269 7473 2d66 726f 6d0a 2020 2020 2d20  rits-from.    - 
+00001e80: 5b20 5d20 2d2d 6967 6e6f 7265 2d64 6566  [ ] --ignore-def
+00001e90: 696e 6974 696f 6e73 0a20 2020 202d 205b  initions.    - [
+00001ea0: 205d 202d 2d69 676e 6f72 652d 6465 6669   ] --ignore-defi
+00001eb0: 6e69 7469 6f6e 732d 6966 2d69 6e68 6572  nitions-if-inher
+00001ec0: 6974 732d 6672 6f6d 0a20 2020 202d 205b  its-from.    - [
+00001ed0: 205d 202d 2d69 676e 6f72 652d 6465 6669   ] --ignore-defi
+00001ee0: 6e69 7469 6f6e 732d 6966 2d64 6563 6f72  nitions-if-decor
+00001ef0: 6174 6564 2d77 6974 680a 2020 2020 2020  ated-with.      
+00001f00: 2020 2d20 5175 6573 7469 6f6e 3a20 776f    - Question: wo
+00001f10: 756c 6420 6974 2062 6520 706f 7373 6962  uld it be possib
+00001f20: 6c65 2074 6f20 6967 6e6f 7265 206f 6e6c  le to ignore onl
+00001f30: 7920 6365 7274 6169 6e20 7479 7065 7320  y certain types 
+00001f40: 6f66 2063 6865 636b 7320 666f 7220 6120  of checks for a 
+00001f50: 626f 6479 2c20 652e 672e 206f 6e6c 7920  body, e.g. only 
+00001f60: 7661 7269 6162 6c65 2061 7474 7269 6275  variable attribu
+00001f70: 7465 7320 6f66 2054 7970 6564 4469 6374  tes of TypedDict
+00001f80: 2061 6e64 2073 7469 6c6c 2063 6865 636b   and still check
+00001f90: 2075 7361 6765 206f 6620 6d65 7468 6f64   usage of method
+00001fa0: 7320 616e 6420 7072 6f70 6572 7469 6573  s and properties
+00001fb0: 3f0a 2020 2020 2020 2020 2d20 5768 6174  ?.        - What
+00001fc0: 2065 7870 7265 7373 696f 6e20 776f 756c   expression woul
+00001fd0: 6420 616c 6c6f 7720 7468 6973 2074 7970  d allow this typ
+00001fe0: 6520 6f66 2070 7265 6369 7373 696f 6e3f  e of precission?
+00001ff0: 0a2d 205b 205d 2044 6973 7469 6e67 7569  .- [ ] Distingui
+00002000: 7368 2062 6574 7765 656e 2064 6566 696e  sh between defin
+00002010: 6974 696f 6e73 2077 6974 6820 7361 6d65  itions with same
+00002020: 206e 616d 652c 2062 7574 2064 6966 6665   name, but diffe
+00002030: 7265 6e74 2066 696c 6573 2e0a 2d20 5b20  rent files..- [ 
+00002040: 5d20 5265 7065 6174 6564 2061 7070 6c69  ] Repeated appli
+00002050: 6361 7469 6f6e 206f 6620 6064 6561 6463  cation of `deadc
+00002060: 6f64 6560 2074 696c 6c20 7468 6520 6f75  ode` till the ou
+00002070: 7470 7574 2073 746f 7073 2063 6861 6e67  tput stops chang
+00002080: 696e 672e 0a2d 205b 205d 2055 6e72 6561  ing..- [ ] Unrea
+00002090: 6368 6162 6c65 2063 6f64 6520 6465 7465  chable code dete
+000020a0: 6374 696f 6e20 616e 6420 6669 7869 6e67  ction and fixing
+000020b0: 3a20 7468 6973 2073 686f 756c 6420 6f6e  : this should on
+000020c0: 6c79 2062 6520 7363 6f70 6564 2066 6f72  ly be scoped for
+000020d0: 2069 6620 7374 6174 656d 656e 7473 2061   if statements a
+000020e0: 6e64 206f 6e6c 7920 6c69 6d69 7465 6420  nd only limited 
+000020f0: 746f 2070 7269 6d69 7469 7665 2076 6172  to primitive var
+00002100: 6961 626c 6573 2e0a 2d20 5b20 5d20 602d  iables..- [ ] `-
+00002110: 2d66 6978 202d 2d64 7279 205b 6669 6c65  -fix --dry [file
+00002120: 6e61 6d65 735d 6020 2d20 6f6e 6c79 2073  names]` - only s
+00002130: 686f 7720 7768 6174 7320 6162 6f75 7420  how whats about 
+00002140: 746f 2063 6861 6e67 6520 696e 2074 6865  to change in the
+00002150: 206c 6973 7465 6420 6669 6c65 6e61 6d65   listed filename
+00002160: 732e 0a2d 205b 205d 2042 656e 6368 6d61  s..- [ ] Benchma
+00002170: 726b 696e 6720 7065 7266 6f72 6d61 6e63  rking performanc
+00002180: 6520 7769 7468 206c 6172 6765 7220 7072  e with larger pr
+00002190: 6f6a 6563 7473 2028 7469 6d65 2c20 4350  ojects (time, CP
+000021a0: 5520 616e 6420 6d65 6d6f 7279 2063 6f6e  U and memory con
+000021b0: 7375 6d70 7469 6f6e 2920 696e 206f 7264  sumption) in ord
+000021c0: 6572 2074 6f20 6f70 7469 6d69 7a65 2e0a  er to optimize..
+000021d0: 2d20 5b20 5d20 602d 2d66 6978 6020 636f  - [ ] `--fix` co
+000021e0: 756c 6420 6163 6365 7074 2061 206c 6973  uld accept a lis
+000021f0: 7420 6f66 2066 696c 656e 616d 6573 2061  t of filenames a
+00002200: 7320 7765 6c6c 2028 6f6e 6c79 2074 686f  s well (only tho
+00002210: 7365 2066 696c 6573 2077 6f75 6c64 2062  se files would b
+00002220: 6520 6368 616e 6765 642c 2062 7574 2074  e changed, but t
+00002230: 6865 2073 756d 6d61 7279 2063 6f75 6c64  he summary could
+00002240: 2077 6f75 6c64 2062 6520 6675 6c6c 292e   would be full).
+00002250: 0a20 2020 2028 5468 6973 206d 6967 6874  .    (This might
+00002260: 2062 6520 636f 6e66 7573 696e 672c 2062   be confusing, b
+00002270: 6563 6175 7365 2066 696c 656e 616d 6573  ecause filenames
+00002280: 2c20 7768 6963 6820 6861 7665 2074 6f20  , which have to 
+00002290: 6265 2063 6f6e 7369 6465 7265 6420 6172  be considered ar
+000022a0: 6520 7072 6f76 6964 6564 2077 6974 686f  e provided witho
+000022b0: 7574 2061 6e79 2066 6c61 672c 202d 2d66  ut any flag, --f
+000022c0: 6978 2069 7320 6578 7065 6374 6564 2074  ix is expected t
+000022d0: 6f20 6e6f 7420 6163 6365 7074 2061 7267  o not accept arg
+000022e0: 756d 656e 7473 290a 2d20 5b20 5d20 7072  uments).- [ ] pr
+000022f0: 652d 636f 6d6d 6974 2d68 6f6f 6b2e 0a2d  e-commit-hook..-
+00002300: 205b 205d 206c 616e 6775 6167 6520 7365   [ ] language se
+00002310: 7276 6572 2e0a 2d20 5b20 5d20 5573 6520  rver..- [ ] Use 
+00002320: 6f6e 6c79 2074 776f 2064 6967 6974 7320  only two digits 
+00002330: 666f 7220 6572 726f 7220 636f 6465 7320  for error codes 
+00002340: 696e 7374 6561 6420 6f66 2033 2e20 5477  instead of 3. Tw
+00002350: 6f20 6973 2070 6c65 6e74 7920 616e 6420  o is plenty and 
+00002360: 6974 2073 696d 706c 6966 6965 7320 7573  it simplifies us
+00002370: 6167 6520 6120 6269 740a 2d20 5b20 5d20  age a bit.- [ ] 
+00002380: 4443 3130 3a20 7265 6d6f 7665 2063 6f64  DC10: remove cod
+00002390: 6520 6166 7465 7220 7465 726d 696e 616c  e after terminal
+000023a0: 2073 7461 7465 6d65 6e74 7320 6c69 6b65   statements like
+000023b0: 2060 7261 6973 6560 2c20 6072 6574 7572   `raise`, `retur
+000023c0: 6e60 2c20 6062 7265 616b 602c 2060 636f  n`, `break`, `co
+000023d0: 6e74 696e 7565 6020 616e 6420 636f 6d65  ntinue` and come
+000023e0: 7320 696e 2074 6865 2073 616d 6520 7363  s in the same sc
+000023f0: 6f70 652e 0a2d 205b 205d 2041 6464 2060  ope..- [ ] Add `
+00002400: 6967 6e6f 7265 6020 616e 6420 6070 6572  ignore` and `per
+00002410: 2d66 696c 652d 6967 6e6f 7265 7360 2063  -file-ignores` c
+00002420: 6f6d 6d61 6e64 206c 696e 6520 616e 6420  ommand line and 
+00002430: 7079 7072 6f6a 6563 742e 746f 6d6c 206f  pyproject.toml o
+00002440: 7074 696f 6e73 2c20 7768 6963 6820 616c  ptions, which al
+00002450: 6c6f 7773 2074 6f20 736b 6970 2073 6f6d  lows to skip som
+00002460: 6520 7275 6c65 732e 0a2d 205b 205d 204d  e rules..- [ ] M
+00002470: 616b 6520 7375 7265 2074 6861 7420 616c  ake sure that al
+00002480: 6c20 7275 6c65 7320 6172 6520 6265 696e  l rules are bein
+00002490: 6720 736b 6970 7065 6420 6279 2060 6e6f  g skipped by `no
+000024a0: 7161 6020 636f 6d6d 656e 7420 616e 6420  qa` comment and 
+000024b0: 616c 6c20 7275 6c65 7320 7265 6163 7420  all rules react 
+000024c0: 746f 2060 6e6f 7161 3a20 7275 6c65 5f69  to `noqa: rule_i
+000024d0: 6460 2063 6f6d 6d65 6e74 732e 0a2d 205b  d` comments..- [
+000024e0: 205d 2049 6e63 6c75 6465 2070 6163 6b61   ] Include packa
+000024f0: 6765 206e 616d 6573 2069 6e74 6f20 636f  ge names into co
+00002500: 6465 2069 7465 6d20 7363 6f70 6520 2864  de item scope (d
+00002510: 6f74 2d73 6570 6172 6174 6564 2070 6174  ot-separated pat
+00002520: 6829 2c20 652e 672e 2022 7061 636b 6167  h), e.g. "packag
+00002530: 6531 2e70 6163 6b61 6765 322e 6d6f 6475  e1.package2.modu
+00002540: 6c65 2e63 6c61 7373 2e6d 6574 686f 642e  le.class.method.
+00002550: 7661 7269 6162 6c65 222e 0a2d 205b 205d  variable"..- [ ]
+00002560: 2041 6c6c 206f 7074 696f 6e73 2073 686f   All options sho
+00002570: 756c 6420 6265 2061 626c 6520 746f 2061  uld be able to a
+00002580: 6363 6570 7420 646f 742d 7365 7061 7261  ccept dot-separa
+00002590: 7465 6420 7061 7468 206f 7220 6120 6765  ted path or a ge
+000025a0: 6e65 7269 6320 6e61 6d65 2c20 652e 672e  neric name, e.g.
+000025b0: 2022 6d61 7273 686d 616c 6c6f 772e 5363   "marshmallow.Sc
+000025c0: 6865 6d61 2220 7673 2022 5363 6865 6d61  hema" vs "Schema
+000025d0: 222c 0a20 2064 6f63 756d 656e 7461 7469  ",.  documentati
+000025e0: 6f6e 2073 686f 756c 6420 636c 6561 7279  on should cleary
+000025f0: 2064 656d 6f6e 7374 7261 7465 2074 6865   demonstrate the
+00002600: 2062 6568 6176 696f 7572 2f65 7861 6d70   behaviour/examp
+00002610: 6c65 2074 6861 7420 2253 6368 656d 6122  le that "Schema"
+00002620: 206d 6561 6e73 2022 2a2e 5363 6865 6d61   means "*.Schema
+00002630: 222e 0a2d 205b 205d 2052 6564 6566 696e  "..- [ ] Redefin
+00002640: 6974 696f 6e20 6f66 2061 6e20 6578 6973  ition of an exis
+00002650: 7469 6e67 206e 616d 6520 6d61 6b65 7320  ting name makes 
+00002660: 7072 6576 696f 7573 206e 616d 6520 756e  previous name un
+00002670: 7265 6163 6861 626c 652c 2075 6e6c 6573  reachable, unles
+00002680: 7320 6974 2069 7320 6173 7369 676e 6564  s it is assigned
+00002690: 2073 6f6d 6568 6f77 2e0a                  somehow..
```

