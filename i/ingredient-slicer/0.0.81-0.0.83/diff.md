# Comparing `tmp/ingredient_slicer-0.0.81.tar.gz` & `tmp/ingredient_slicer-0.0.83.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ingredient_slicer-0.0.81.tar", last modified: Fri Mar 29 22:12:19 2024, max compression
+gzip compressed data, was "ingredient_slicer-0.0.83.tar", last modified: Sat Apr  6 15:14:20 2024, max compression
```

## Comparing `ingredient_slicer-0.0.81.tar` & `ingredient_slicer-0.0.83.tar`

### file list

```diff
@@ -1,60 +1,65 @@
-drwxr-xr-x   0 anguswatters   (501) staff       (20)        0 2024-03-29 22:12:19.704382 ingredient_slicer-0.0.81/
-drwxr-xr-x   0 anguswatters   (501) staff       (20)        0 2024-03-29 22:12:19.693407 ingredient_slicer-0.0.81/.github/
-drwxr-xr-x   0 anguswatters   (501) staff       (20)        0 2024-03-29 22:12:19.694542 ingredient_slicer-0.0.81/.github/workflows/
--rw-r--r--   0 anguswatters   (501) staff       (20)     3289 2024-03-23 22:54:52.000000 ingredient_slicer-0.0.81/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 anguswatters   (501) staff       (20)      782 2024-03-23 22:54:24.000000 ingredient_slicer-0.0.81/.github/workflows/run-unit-tests.yml
--rw-r--r--   0 anguswatters   (501) staff       (20)     3118 2024-03-17 16:59:19.000000 ingredient_slicer-0.0.81/.gitignore
--rw-r--r--   0 anguswatters   (501) staff       (20)     1075 2024-03-17 16:52:34.000000 ingredient_slicer-0.0.81/LICENSE
--rw-r--r--   0 anguswatters   (501) staff       (20)     1302 2024-03-29 22:12:19.704101 ingredient_slicer-0.0.81/PKG-INFO
--rw-r--r--   0 anguswatters   (501) staff       (20)      326 2024-03-17 18:11:50.000000 ingredient_slicer-0.0.81/README.md
-drwxr-xr-x   0 anguswatters   (501) staff       (20)        0 2024-03-29 22:12:19.695517 ingredient_slicer-0.0.81/ingredient_slicer/
--rw-r--r--   0 anguswatters   (501) staff       (20)     1891 2024-03-29 22:04:51.000000 ingredient_slicer-0.0.81/ingredient_slicer/__init__.py
--rw-r--r--   0 anguswatters   (501) staff       (20)    83093 2024-03-28 12:57:12.000000 ingredient_slicer-0.0.81/ingredient_slicer/_constants.py
--rw-r--r--   0 anguswatters   (501) staff       (20)   107376 2024-03-29 22:06:49.000000 ingredient_slicer-0.0.81/ingredient_slicer/_ingredient_slicer.py
--rw-r--r--   0 anguswatters   (501) staff       (20)   104238 2024-03-29 20:31:39.000000 ingredient_slicer-0.0.81/ingredient_slicer/_regex_patterns.py
--rw-r--r--   0 anguswatters   (501) staff       (20)    62005 2024-03-29 22:04:55.000000 ingredient_slicer-0.0.81/ingredient_slicer/_utils.py
-drwxr-xr-x   0 anguswatters   (501) staff       (20)        0 2024-03-29 22:12:19.703513 ingredient_slicer-0.0.81/ingredient_slicer.egg-info/
--rw-r--r--   0 anguswatters   (501) staff       (20)     1302 2024-03-29 22:12:19.000000 ingredient_slicer-0.0.81/ingredient_slicer.egg-info/PKG-INFO
--rw-r--r--   0 anguswatters   (501) staff       (20)     1712 2024-03-29 22:12:19.000000 ingredient_slicer-0.0.81/ingredient_slicer.egg-info/SOURCES.txt
--rw-r--r--   0 anguswatters   (501) staff       (20)        1 2024-03-29 22:12:19.000000 ingredient_slicer-0.0.81/ingredient_slicer.egg-info/dependency_links.txt
--rw-r--r--   0 anguswatters   (501) staff       (20)       38 2024-03-29 22:12:19.000000 ingredient_slicer-0.0.81/ingredient_slicer.egg-info/requires.txt
--rw-r--r--   0 anguswatters   (501) staff       (20)       18 2024-03-29 22:12:19.000000 ingredient_slicer-0.0.81/ingredient_slicer.egg-info/top_level.txt
--rw-r--r--   0 anguswatters   (501) staff       (20)     1127 2024-03-29 22:12:11.000000 ingredient_slicer-0.0.81/pyproject.toml
--rw-r--r--   0 anguswatters   (501) staff       (20)       38 2024-03-29 22:12:19.704445 ingredient_slicer-0.0.81/setup.cfg
-drwxr-xr-x   0 anguswatters   (501) staff       (20)        0 2024-03-29 22:12:19.703256 ingredient_slicer-0.0.81/tests/
--rw-r--r--   0 anguswatters   (501) staff       (20)        0 2024-03-18 23:35:35.000000 ingredient_slicer-0.0.81/tests/__init__.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     2402 2024-03-29 21:18:52.000000 ingredient_slicer-0.0.81/tests/test_avg_ranges.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     5832 2024-03-29 21:20:16.000000 ingredient_slicer-0.0.81/tests/test_casual_ingredients.py
--rw-r--r--   0 anguswatters   (501) staff       (20)        0 2024-03-29 21:19:59.000000 ingredient_slicer-0.0.81/tests/test_clean_hyphen_padded_substrings.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     1182 2024-03-29 21:19:57.000000 ingredient_slicer-0.0.81/tests/test_duplicate_unit_ranges.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     8507 2024-03-29 21:18:52.000000 ingredient_slicer-0.0.81/tests/test_extract_dimensions.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     3541 2024-03-29 21:19:50.000000 ingredient_slicer-0.0.81/tests/test_extract_quantities_utils.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     3711 2024-03-29 21:19:48.000000 ingredient_slicer-0.0.81/tests/test_find_and_remove.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     2842 2024-03-29 21:19:52.000000 ingredient_slicer-0.0.81/tests/test_find_and_remove_hyphen_substrings.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     2589 2024-03-29 21:19:47.000000 ingredient_slicer-0.0.81/tests/test_fraction_str_to_decimal.py
--rw-r--r--   0 anguswatters   (501) staff       (20)    20328 2024-03-29 22:11:49.000000 ingredient_slicer-0.0.81/tests/test_ingredient_slicer.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     3364 2024-03-29 21:18:54.000000 ingredient_slicer-0.0.81/tests/test_ingredient_slicer_dimensions.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     7567 2024-03-29 21:18:56.000000 ingredient_slicer-0.0.81/tests/test_ingredient_slicer_x_separators.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     2965 2024-03-29 21:19:46.000000 ingredient_slicer-0.0.81/tests/test_make_int_or_float_str.py
--rw-r--r--   0 anguswatters   (501) staff       (20)    14464 2024-03-29 21:19:43.000000 ingredient_slicer-0.0.81/tests/test_merge_numbers.py
--rw-r--r--   0 anguswatters   (501) staff       (20)    43982 2024-03-29 21:19:18.000000 ingredient_slicer-0.0.81/tests/test_number_ranges.py
--rw-r--r--   0 anguswatters   (501) staff       (20)    56318 2024-03-29 21:19:45.000000 ingredient_slicer-0.0.81/tests/test_number_ranges_separated_by_words.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     5652 2024-03-28 12:32:40.000000 ingredient_slicer-0.0.81/tests/test_numbers_with_inch_symbols.py
--rw-r--r--   0 anguswatters   (501) staff       (20)    15368 2024-03-29 21:19:20.000000 ingredient_slicer-0.0.81/tests/test_parenthesis.py
--rw-r--r--   0 anguswatters   (501) staff       (20)    11034 2024-03-29 21:19:23.000000 ingredient_slicer-0.0.81/tests/test_parenthesis_utils.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     2512 2024-03-29 21:19:22.000000 ingredient_slicer-0.0.81/tests/test_percentages.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     3547 2024-03-29 21:19:26.000000 ingredient_slicer-0.0.81/tests/test_prefixed_number_words_regex.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     5013 2024-03-29 21:19:28.000000 ingredient_slicer-0.0.81/tests/test_prep_words.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     5261 2024-03-29 21:19:25.000000 ingredient_slicer-0.0.81/tests/test_quantity_range_regex.py
--rw-r--r--   0 anguswatters   (501) staff       (20)    27045 2024-03-25 17:18:12.000000 ingredient_slicer-0.0.81/tests/test_quantity_units_regex.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     3571 2024-03-29 21:19:15.000000 ingredient_slicer-0.0.81/tests/test_remove_repeat_units_in_ranges.py
--rw-r--r--   0 anguswatters   (501) staff       (20)      633 2024-03-29 21:19:14.000000 ingredient_slicer-0.0.81/tests/test_remove_x_separators.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     6384 2024-03-29 21:19:12.000000 ingredient_slicer-0.0.81/tests/test_replace_a_or_an_quantities.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     6869 2024-03-29 21:19:08.000000 ingredient_slicer-0.0.81/tests/test_separate_dimensions.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     1808 2024-03-29 21:19:42.000000 ingredient_slicer-0.0.81/tests/test_size_modifiers.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     8974 2024-03-29 21:19:39.000000 ingredient_slicer-0.0.81/tests/test_spaced_numbers.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     5838 2024-03-29 21:19:40.000000 ingredient_slicer-0.0.81/tests/test_unit_regex.py
--rw-r--r--   0 anguswatters   (501) staff       (20)    16942 2024-03-29 21:19:35.000000 ingredient_slicer-0.0.81/tests/test_wild_ingredients.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     8022 2024-03-29 21:19:37.000000 ingredient_slicer-0.0.81/tests/test_word_fractions.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     7167 2024-03-29 21:19:33.000000 ingredient_slicer-0.0.81/tests/test_word_numbers.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     1337 2024-03-29 21:19:32.000000 ingredient_slicer-0.0.81/tests/test_x_after_number_regex.py
+drwxr-xr-x   0 anguswatters   (501) staff       (20)        0 2024-04-06 15:14:20.282654 ingredient_slicer-0.0.83/
+drwxr-xr-x   0 anguswatters   (501) staff       (20)        0 2024-04-06 15:14:20.270927 ingredient_slicer-0.0.83/.github/
+drwxr-xr-x   0 anguswatters   (501) staff       (20)        0 2024-04-06 15:14:20.272086 ingredient_slicer-0.0.83/.github/workflows/
+-rw-r--r--   0 anguswatters   (501) staff       (20)     3289 2024-03-30 17:04:31.000000 ingredient_slicer-0.0.83/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 anguswatters   (501) staff       (20)      782 2024-03-23 22:54:24.000000 ingredient_slicer-0.0.83/.github/workflows/run-unit-tests.yml
+-rw-r--r--   0 anguswatters   (501) staff       (20)     3118 2024-03-17 16:59:19.000000 ingredient_slicer-0.0.83/.gitignore
+-rw-r--r--   0 anguswatters   (501) staff       (20)     1075 2024-03-17 16:52:34.000000 ingredient_slicer-0.0.83/LICENSE
+-rw-r--r--   0 anguswatters   (501) staff       (20)     3408 2024-04-06 15:14:20.282384 ingredient_slicer-0.0.83/PKG-INFO
+-rw-r--r--   0 anguswatters   (501) staff       (20)     2434 2024-04-06 15:12:49.000000 ingredient_slicer-0.0.83/README.md
+drwxr-xr-x   0 anguswatters   (501) staff       (20)        0 2024-04-06 15:14:20.273097 ingredient_slicer-0.0.83/ingredient_slicer/
+-rw-r--r--   0 anguswatters   (501) staff       (20)     1491 2024-04-06 13:29:54.000000 ingredient_slicer-0.0.83/ingredient_slicer/__init__.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)   155365 2024-04-03 20:55:17.000000 ingredient_slicer-0.0.83/ingredient_slicer/_constants.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)   104901 2024-04-06 15:08:23.000000 ingredient_slicer-0.0.83/ingredient_slicer/_ingredient_slicer.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)   108094 2024-04-06 13:59:47.000000 ingredient_slicer-0.0.83/ingredient_slicer/_regex_patterns.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)    92674 2024-04-06 14:42:17.000000 ingredient_slicer-0.0.83/ingredient_slicer/_utils.py
+drwxr-xr-x   0 anguswatters   (501) staff       (20)        0 2024-04-06 15:14:20.281798 ingredient_slicer-0.0.83/ingredient_slicer.egg-info/
+-rw-r--r--   0 anguswatters   (501) staff       (20)     3408 2024-04-06 15:14:20.000000 ingredient_slicer-0.0.83/ingredient_slicer.egg-info/PKG-INFO
+-rw-r--r--   0 anguswatters   (501) staff       (20)     1922 2024-04-06 15:14:20.000000 ingredient_slicer-0.0.83/ingredient_slicer.egg-info/SOURCES.txt
+-rw-r--r--   0 anguswatters   (501) staff       (20)        1 2024-04-06 15:14:20.000000 ingredient_slicer-0.0.83/ingredient_slicer.egg-info/dependency_links.txt
+-rw-r--r--   0 anguswatters   (501) staff       (20)       38 2024-04-06 15:14:20.000000 ingredient_slicer-0.0.83/ingredient_slicer.egg-info/requires.txt
+-rw-r--r--   0 anguswatters   (501) staff       (20)       18 2024-04-06 15:14:20.000000 ingredient_slicer-0.0.83/ingredient_slicer.egg-info/top_level.txt
+-rw-r--r--   0 anguswatters   (501) staff       (20)     1125 2024-04-06 13:47:46.000000 ingredient_slicer-0.0.83/pyproject.toml
+-rw-r--r--   0 anguswatters   (501) staff       (20)       38 2024-04-06 15:14:20.282715 ingredient_slicer-0.0.83/setup.cfg
+drwxr-xr-x   0 anguswatters   (501) staff       (20)        0 2024-04-06 15:14:20.281552 ingredient_slicer-0.0.83/tests/
+-rw-r--r--   0 anguswatters   (501) staff       (20)        0 2024-04-06 13:59:44.000000 ingredient_slicer-0.0.83/tests/__init__.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     2402 2024-03-29 21:18:52.000000 ingredient_slicer-0.0.83/tests/test_avg_ranges.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     5832 2024-03-29 21:20:16.000000 ingredient_slicer-0.0.83/tests/test_casual_ingredients.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)        0 2024-04-06 13:59:43.000000 ingredient_slicer-0.0.83/tests/test_clean_hyphen_padded_substrings.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     5502 2024-03-30 17:00:12.000000 ingredient_slicer-0.0.83/tests/test_convert_fractions_to_decimals.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     1309 2024-04-06 12:45:26.000000 ingredient_slicer-0.0.83/tests/test_convert_volumes_to_milliliters.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     1182 2024-03-29 21:19:57.000000 ingredient_slicer-0.0.83/tests/test_duplicate_unit_ranges.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     8507 2024-03-29 21:18:52.000000 ingredient_slicer-0.0.83/tests/test_extract_dimensions.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     3541 2024-03-29 21:19:50.000000 ingredient_slicer-0.0.83/tests/test_extract_quantities_utils.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     3711 2024-03-29 21:19:48.000000 ingredient_slicer-0.0.83/tests/test_find_and_remove.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     2842 2024-03-29 21:19:52.000000 ingredient_slicer-0.0.83/tests/test_find_and_remove_hyphen_substrings.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     3352 2024-04-06 13:59:33.000000 ingredient_slicer-0.0.83/tests/test_fraction_str_to_decimal.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)    24889 2024-04-06 13:04:35.000000 ingredient_slicer-0.0.83/tests/test_get_gram_weight.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)    20385 2024-04-06 14:42:17.000000 ingredient_slicer-0.0.83/tests/test_ingredient_slicer.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     3374 2024-04-06 15:03:13.000000 ingredient_slicer-0.0.83/tests/test_ingredient_slicer_dimensions.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     4718 2024-04-06 14:44:14.000000 ingredient_slicer-0.0.83/tests/test_ingredient_slicer_fraction_conversions.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     7502 2024-04-06 14:42:17.000000 ingredient_slicer-0.0.83/tests/test_ingredient_slicer_x_separators.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     2965 2024-03-29 21:19:46.000000 ingredient_slicer-0.0.83/tests/test_make_int_or_float_str.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     2167 2024-04-06 12:30:44.000000 ingredient_slicer-0.0.83/tests/test_merge_misleading_ranges.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)    14464 2024-03-29 21:19:43.000000 ingredient_slicer-0.0.83/tests/test_merge_numbers.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)    43982 2024-04-06 14:42:17.000000 ingredient_slicer-0.0.83/tests/test_number_ranges.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)    56318 2024-03-29 21:19:45.000000 ingredient_slicer-0.0.83/tests/test_number_ranges_separated_by_words.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     5652 2024-04-06 13:59:36.000000 ingredient_slicer-0.0.83/tests/test_numbers_with_inch_symbols.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)    15368 2024-03-29 21:19:20.000000 ingredient_slicer-0.0.83/tests/test_parenthesis.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)    11034 2024-03-29 21:19:23.000000 ingredient_slicer-0.0.83/tests/test_parenthesis_utils.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     2512 2024-03-29 21:19:22.000000 ingredient_slicer-0.0.83/tests/test_percentages.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     3547 2024-03-29 21:19:26.000000 ingredient_slicer-0.0.83/tests/test_prefixed_number_words_regex.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     5013 2024-03-29 21:19:28.000000 ingredient_slicer-0.0.83/tests/test_prep_words.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     5261 2024-03-29 21:19:25.000000 ingredient_slicer-0.0.83/tests/test_quantity_range_regex.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)    27045 2024-04-06 13:59:38.000000 ingredient_slicer-0.0.83/tests/test_quantity_units_regex.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     3571 2024-04-06 13:31:28.000000 ingredient_slicer-0.0.83/tests/test_remove_repeat_units_in_ranges.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)      633 2024-03-29 21:19:14.000000 ingredient_slicer-0.0.83/tests/test_remove_x_separators.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     6384 2024-03-29 21:19:12.000000 ingredient_slicer-0.0.83/tests/test_replace_a_or_an_quantities.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     6869 2024-03-29 21:19:08.000000 ingredient_slicer-0.0.83/tests/test_separate_dimensions.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     1808 2024-03-29 21:19:42.000000 ingredient_slicer-0.0.83/tests/test_size_modifiers.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     8974 2024-03-29 21:19:39.000000 ingredient_slicer-0.0.83/tests/test_spaced_numbers.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     5838 2024-03-29 21:19:40.000000 ingredient_slicer-0.0.83/tests/test_unit_regex.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)    16676 2024-04-06 15:13:17.000000 ingredient_slicer-0.0.83/tests/test_wild_ingredients.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     8022 2024-03-29 21:19:37.000000 ingredient_slicer-0.0.83/tests/test_word_fractions.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     7167 2024-03-29 21:19:33.000000 ingredient_slicer-0.0.83/tests/test_word_numbers.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     1337 2024-04-06 14:42:17.000000 ingredient_slicer-0.0.83/tests/test_x_after_number_regex.py
```

### Comparing `ingredient_slicer-0.0.81/.github/workflows/publish-to-pypi.yml` & `ingredient_slicer-0.0.83/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.81/.github/workflows/run-unit-tests.yml` & `ingredient_slicer-0.0.83/.github/workflows/run-unit-tests.yml`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.81/.gitignore` & `ingredient_slicer-0.0.83/.gitignore`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.81/LICENSE` & `ingredient_slicer-0.0.83/LICENSE`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.81/ingredient_slicer/__init__.py` & `ingredient_slicer-0.0.83/ingredient_slicer/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,44 +1,37 @@
 # __init__.py
 
-__version__ = "0.0.81"
+__version__ = "0.0.83"
 
-# from ._constants import NUMBER_WORDS,  NUMBER_PREFIX_WORDS, \
-#     MULTI_FRACTION_WORDS, FRACTION_WORDS, DENOMINATOR_WORDS, UNICODE_FRACTIONS, \
-#     UNITS, BASIC_UNITS, VOLUME_UNITS, WEIGHT_UNITS, DIMENSION_UNITS, \
-#     CASUAL_QUANTITIES, CASUAL_UNITS, UNITS_SET, \
-#     BASIC_UNITS_SET, NON_BASIC_UNITS_SET, SIZE_MODIFIERS_SET, \
-#     VOLUME_UNITS_SET, WEIGHT_UNITS_SET, DIMENSION_UNITS_SET, CASUAL_QUANTITIES_SET, CASUAL_UNITS_SET, \
-#     UNIT_MODIFIERS, PREP_WORDS, APPROXIMATE_STRINGS
-
-from ._constants import UNITS, WEIGHT_UNITS, DIMENSION_UNITS, \
+from ._constants import UNITS, WEIGHT_UNITS, VOLUME_UNITS, DIMENSION_UNITS, \
     CASUAL_UNITS, CASUAL_QUANTITIES, PREP_WORDS, \
-    FOOD_CATALOG, FOOD_CATEGORIES
+    FOOD_CATALOG, FOOD_CATEGORIES, FOOD_DENSITY_BY_GROUP
 
+from ._ingredient_slicer import IngredientSlicer
+# from ._regex_patterns import IngredientTools
 # from ._utils import _make_int_or_float_str, _fraction_str_to_decimal, \
 #     _find_substring_indices, _find_and_remove_hyphens_around_substring
     # _replace_and_with_hyphen, _replace_to_or_with_hyphen, _replace_to_with_hyphen, _replace_or_with_hyphen
 
-from ._regex_patterns import IngredientTools
-from ._ingredient_slicer import IngredientSlicer
 
 __all__ = [
     # Constants
     "UNITS",
     "WEIGHT_UNITS",
+    "VOLUME_UNITS",
     "DIMENSION_UNITS", 
     "CASUAL_UNITS", 
     "CASUAL_QUANTITIES",
     "PREP_WORDS",
     "FOOD_CATALOG",
     "FOOD_CATEGORIES",
-
-    # Recipes regex and parser classes
-    # 'IngredientTools', 
+    "FOOD_DENSITY_BY_GROUP",
+    # Main parser classe
     'IngredientSlicer'
+    # 'IngredientTools',  # Old regex patterns class
     ]
 
 # # ---- OLD Constants ----
 # 'NUMBER_WORDS', 
 # 'NUMBER_PREFIX_WORDS',
 # 'MULTI_FRACTION_WORDS',
 # 'FRACTION_WORDS',
```

### Comparing `ingredient_slicer-0.0.81/ingredient_slicer/_ingredient_slicer.py` & `ingredient_slicer-0.0.83/ingredient_slicer/_ingredient_slicer.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,64 +28,53 @@
         debug (bool): Whether to print debug statements (default is False)
     """
 
     # regex = IngredientTools()
 
     def __init__(self, ingredient: str, debug = False):
         self.ingredient          = ingredient
-        self.standardized_ingredient = ingredient
+        self._standardized_ingredient = ingredient
+        
+        self._food              = None 
+        self._quantity          = None    # the best quantity found in the ingredient string
+        
+        self._unit              = None    # the best unit found in the ingredient string
+        self._standardized_unit = None   # "standard units" are the commonplace names for the found units (i.e. the standard unit of "oz" is "ounce")
         
-        self.food           = None 
-        self.quantity       = None    # the best quantity found in the ingredient string
-        self.unit           = None    # the best unit found in the ingredient string
-
-
         # make member variables for seconday quantities and units
-        self.secondary_quantity = None
-        self.secondary_unit     = None
-
-        # "standard units" are the commonplace names for the found units (i.e. the standard unit of "oz" is "ounce")
-        self.standardized_unit           = None 
-        self.standardized_secondary_unit = None
+        self._secondary_quantity = None
+        self._secondary_unit     = None
+        self._standardized_secondary_unit = None
+
+        self._gram_weight          = None
+        self._min_gram_weight     = None
+        self._max_gram_weight     = None
 
         # "prep" are words that describe the state of the ingredient (i.e. "chopped", "diced", "minced")
-        self.prep                  = []
+        self._prep                  = []
 
         # "size modifiers" are words that describe the size of the ingredient (i.e. "large", "small", "medium")
-        self.size_modifiers        = [] 
+        self._size_modifiers        = [] 
 
         # "dimensions" are numbers and units that describe the dimensions of the ingredient (i.e. "1 inch", "2 ft", "2cm x 3cm")
-        self.dimensions             = []
+        self._dimensions            = []
 
-        self.required            = True    # default sets the ingredient as a required ingredient
+        self._is_required           = True    # default sets the ingredient as a required ingredient
 
-        self.staged_ingredient  = None    # standardized ingredient but keeping the parenthesis content
-        self.reduced_ingredient  = None    # parenthesis removed from the ingredient string
+        self._staged_ingredient      = None    # standardized ingredient but keeping the parenthesis content
 
-        self.parenthesis_content = None  # content of the parenthesis removed from the ingredient string
-        self.parenthesis_notes   = []
+        self._parenthesis_content = None  # content of the parenthesis removed from the ingredient string
+        self._parenthesis_notes   = []
 
         self.debug = debug
         # self.extract_version = extract_version
 
-        self.parse()
-
-        self.parsed_ingredient = self.to_json()
+        self._parse()
 
-        # self.found_units         = None    # where units will get stored after being parsed (temporarily)
-        # self.parenthesis_obj = {
-        #     "raw_ingredient": "",
-        #     "standard_ingredient": "",
-        #     "reduced_ingredient": self.reduced_ingredient,
-        #     "parenthesis_content": ""
-        #     }
-
-    def _standardized_ingredient(self):
-        
-        return self.standardized_ingredient
+        self._parsed_ingredient = self.to_json()
     
     def _find_units(self, ingredient: str) -> List[str]:
         """
         Find units in the ingredient string.
         Args:
             ingredient (str): The ingredient string to parse.
         Returns:
@@ -95,189 +84,157 @@
         # split the input string on whitespaces
         split_ingredient = ingredient.split()
 
         matched_units = [i for i in split_ingredient if i in _constants.UNITS]
 
         return matched_units
     
-    # TODO: move to a utils file for generic functions ---> COMPLETED (Deprecated, this function, use the one in _utils.py)
-    def _make_int_or_float_str(self, number_str: str) -> str:
-        """ Convert a string representation of a number to its integer or float equivalent.
-        If the number is a whole number, return the integer value as a string. If the number is a decimal, return the float value as a string.
-        Args:
-            number_str (str): The string representation of the number.
-        Returns:
-            str: The integer or float value of the number as a string.
-        
-        Examples:
-        >>> make_int_or_float_str("1.0") 
-        "1"
-        >>> make_int_or_float_str("1")
-        "1"
-        >>> make_int_or_float_str("0.25")
-        "0.25"
-        """
-        number = float(number_str.strip())  # Convert string to float
-        if number == int(number):  # Check if float is equal to its integer value
-            return str(int(number))  # Return integer value if it's a whole number
-        else:
-            return str(number)  # Return float if it's a decimal
-
     def _find_and_remove_percentages(self) -> None:
         """
         Find and remove percentages from the ingredient string.
         """
         # ingredient = "1 cup of 2% heavy cream"
         
         for key, pattern in _regex_patterns.PCT_REGEX_MAP.items():
-            pattern_iter = pattern.finditer(self.standardized_ingredient)
+            pattern_iter = pattern.finditer(self._standardized_ingredient)
             offset = 0
             for match in pattern_iter:
                 match_string = match.group()
                 start, end = match.start(), match.end()
                 modified_start = start + offset
                 modified_end = end + offset
 
                 replacement_str = ""
 
                 # Construct the modified string with the replacement applied
-                self.standardized_ingredient = self.standardized_ingredient[:modified_start] + str(replacement_str) + self.standardized_ingredient[modified_end:]
+                self._standardized_ingredient = self._standardized_ingredient[:modified_start] + str(replacement_str) + self._standardized_ingredient[modified_end:]
                 # ingredient = ingredient[:modified_start] + str(replacement_str) + ingredient[modified_end:]
                 offset += len(str(replacement_str)) - (end - start)
-        # pattern_iter = _regex_patterns.NUMBERS_FOLLOWED_BY_PERCENTAGE.finditer(self.standardized_ingredient)
+        # pattern_iter = _regex_patterns.NUMBERS_FOLLOWED_BY_PERCENTAGE.finditer(self._standardized_ingredient)
                 
         return
     
     def _replace_number_followed_by_inch_symbol(self) -> None:
 
-        self.standardized_ingredient = _utils._replace_number_followed_by_inch_symbol(self.standardized_ingredient)
+        self._standardized_ingredient = _utils._replace_number_followed_by_inch_symbol(self._standardized_ingredient)
 
         return 
     
     def _find_and_replace_fraction_words(self) -> None:
         """ Find and replace fraction words with their corresponding numerical values in the parsed ingredient."""
 
         for key, pattern in _regex_patterns.NUMBER_WITH_FRACTION_WORD_MAP.items():
             
-            pattern_iter = pattern.finditer(self.standardized_ingredient)
+            pattern_iter = pattern.finditer(self._standardized_ingredient)
             offset = 0
 
             for match in pattern_iter:
-                print(f"Got a fraction word match with key: {key}") if self.debug else None
+                # print(f"Got a fraction word match with key: {key}") if self.debug else None
                 match_string = match.group(0)
                 start, end = match.start(), match.end()
                 modified_start = start + offset
                 modified_end = end + offset
 
                 match_string = match_string.replace("-", " ")
-                print(f"Match: {match_string}") if self.debug else None
+                # print(f"Match: {match_string}") if self.debug else None
                 # match_string = match_string.replace("-", " ")
                 split_match = match_string.split(" ")
 
                 split_match = [i.strip() for i in split_match]
 
-                print(f"Split Match: {split_match}") if self.debug else None
+                # print(f"Split Match: {split_match}") if self.debug else None
 
                 number_word = split_match[0]
                 fraction_word = split_match[1]
-                
+
                 fraction_value, decimal = _constants.FRACTION_WORDS[fraction_word.lower()]
 
                 updated_value = str(float(number_word) * float(decimal))
-                self.standardized_ingredient = self.standardized_ingredient[:modified_start] + str(updated_value) + self.standardized_ingredient[modified_end:]
-                # self.standardized_ingredient = self.standardized_ingredient[:match.start()] + str(updated_value) + self.standardized_ingredient[match.end():]
+                self._standardized_ingredient = self._standardized_ingredient[:modified_start] + str(updated_value) + self._standardized_ingredient[modified_end:]
+                # self._standardized_ingredient = self._standardized_ingredient[:match.start()] + str(updated_value) + self._standardized_ingredient[match.end():]
                 # ingredient = ingredient[:modified_start] + str(updated_value) + ingredient[modified_end:]
 
                 offset += len(str(updated_value)) - (end - start)
 
-        # pattern_iter = _regex_patterns.NUMBER_WITH_FRACTION_WORD_GROUPS.finditer(self.standardized_ingredient)
+        # pattern_iter = _regex_patterns.NUMBER_WITH_FRACTION_WORD_GROUPS.finditer(self._standardized_ingredient)
         # offset = 0
 
         # for match in pattern_iter:
         #     start, end = match.start(), match.end()
         #     number_word   = match.group(1)
         #     fraction_word = match.group(2)
         #     fraction_value, decimal = _constants.FRACTION_WORDS[fraction_word]
         #     # multiply first number in match by the decimal value of the fraction word (i.e. "2 third" -> 2 * 1/3)
         #     updated_value = str(float(number_word) * float(decimal))
-        #     self.standardized_ingredient = self.standardized_ingredient[:match.start()] + str(updated_value) + self.standardized_ingredient[match.end():]
+        #     self._standardized_ingredient = self._standardized_ingredient[:match.start()] + str(updated_value) + self._standardized_ingredient[match.end():]
         #     offset += len(updated_value) - (end - start)
 
         return 
 
     def _find_and_replace_numbers_separated_by_add_numbers(self) -> None:
         """Find numbers separated by "and", "&", "plus", or "+" and replace the matched strings with their sum of the 2 number values
         Examples:
         "1 and 0.5" -> "1.5"
         "1 & 0.5" -> "1.5"
         "2 plus 0.66" -> "2.66"
         "2 + 0.66" -> "2.66"
         """
-        add_pattern_iter = _regex_patterns.NUMBERS_SEPARATED_BY_ADD_SYMBOLS_GROUPS.finditer(self.standardized_ingredient)
+        add_pattern_iter = _regex_patterns.NUMBERS_SEPARATED_BY_ADD_SYMBOLS_GROUPS.finditer(self._standardized_ingredient)
 
         offset = 0
 
         for match in add_pattern_iter:
             match_string = match.group(0)
             start, end = match.start(), match.end()
             modified_start = start + offset
             modified_end = end + offset
 
             first_number = float(match.group(1).strip())
             second_number = float(match.group(2).strip())
 
-            print(f"MATCH: {match_string}") if self.debug else None
-            print(f"First Number: {first_number}") if self.debug else None
-            print(f"Second Number: {second_number}") if self.debug else None
+            # print(f"MATCH: {match_string}") if self.debug else None
+            # print(f"First Number: {first_number}") if self.debug else None
+            # print(f"Second Number: {second_number}") if self.debug else None
 
             updated_value = f" {_utils._make_int_or_float_str(str(first_number + second_number))} "
-            print(f"Updated Value: {updated_value}") if self.debug else None
+            # print(f"Updated Value: {updated_value}") if self.debug else None
 
-            self.standardized_ingredient = self.standardized_ingredient[:modified_start] + str(updated_value) + self.standardized_ingredient[modified_end:]
-            # self.standardized_ingredient = self.standardized_ingredient[:match.start()] + updated_value + self.standardized_ingredient[match.end():]
+            self._standardized_ingredient = self._standardized_ingredient[:modified_start] + str(updated_value) + self._standardized_ingredient[modified_end:]
+            # self._standardized_ingredient = self._standardized_ingredient[:match.start()] + updated_value + self._standardized_ingredient[match.end():]
             offset += len(updated_value) - (end - start)
     
         return
-    
-    def _find_and_replace_casual_quantities(self):
-        """
-        Find and replace matches of CASUAL_QUANTITIES_PATTERN with the key from the CASUAL_QUANTITIES dictionary
-        """
-
-        offset = 0
-        pattern_iter = _regex_patterns.CASUAL_QUANTITIES_PATTERN.finditer(self.standardized_ingredient)
 
-        for match in pattern_iter:
-            match_string    = match.group()
-
-            # Get the start and end of the match and the modified start and end positions given the offset
-            start, end = match.start(), match.end()
-            modified_start = start + offset
-            modified_end = end + offset
-
-            replacement_str = _constants.CASUAL_QUANTITIES[match_string] 
+    def _find_and_replace_casual_quantities(self):
 
-            # Construct the modified string with the replacement applied
-            self.standardized_ingredient = self.standardized_ingredient[:modified_start] + str(replacement_str) + self.standardized_ingredient[modified_end:]
-            # input_ingredient = input_ingredient[:modified_start] + str(replacement_str) + input_ingredient[modified_end:]
-            
-            # Update the offset for subsequent removals 
-            offset += len(str(replacement_str)) - (end - start)
+        self._standardized_ingredient = _utils._find_and_replace_casual_quantities(self._standardized_ingredient)
 
+        return 
+    
     def _drop_special_dashes(self) -> None:
         # print("Dropping special dashes")
-        self.standardized_ingredient = self.standardized_ingredient.replace("—", "-").replace("–", "-").replace("~", "-")
+        self._standardized_ingredient = self._standardized_ingredient.replace("—", "-").replace("–", "-").replace("~", "-")
         return
 
     def _find_and_replace_prefixed_number_words(self) -> None:
         """ Replace prefixed number words with their corresponding numerical values in the parsed ingredient 
         Strings like "twenty five" are replaced with "25", or "thirty-two" is replaced with "32"
+        """
+
+        self._standardized_ingredient = _utils._find_and_replace_prefixed_number_words(self._standardized_ingredient)
+        
+        return
+
+    # TODO: DELETE THIS, _utils above has replaced this
+    def _find_and_replace_prefixed_number_words2(self) -> None:
+        """ Replace prefixed number words with their corresponding numerical values in the parsed ingredient 
+        Strings like "twenty five" are replaced with "25", or "thirty-two" is replaced with "32"
 
         """
-        number_words_iter = _regex_patterns.PREFIXED_NUMBER_WORDS_GROUPS.finditer(self.standardized_ingredient)
+        number_words_iter = _regex_patterns.PREFIXED_NUMBER_WORDS_GROUPS.finditer(self._standardized_ingredient)
 
         offset = 0
 
         for match in number_words_iter:
             
             if match:
                 start, end = match.start(), match.end()
@@ -292,216 +249,122 @@
                 combined_value = prefix_value + number_value
 
                 # Calculate the start and end positions in the modified string
                 modified_start = start + offset
                 modified_end = end + offset
 
                 # Construct the modified string with the replacement applied
-                self.standardized_ingredient = self.standardized_ingredient[:modified_start] + str(combined_value) + self.standardized_ingredient[modified_end:]
+                self._standardized_ingredient = self._standardized_ingredient[:modified_start] + str(combined_value) + self._standardized_ingredient[modified_end:]
                 # ingredient = ingredient[:modified_start] + str(combined_value) + ingredient[modified_end:]
 
                 # Update the offset for subsequent replacements
                 offset += len(str(combined_value)) - (end - start)
 
                 # print(f"""
                 # Match string: {match_string}
                 # - Prefix word: {prefix_word}
                 # - Number word: {number_word}
                 # Prefix value ({prefix_value}) + Number value ({number_value}) = Combined value ({combined_value})
                 # > {prefix_value} + {number_value} = {combined_value}
                 # -> Match: {match_string} at positions {start}-{end}
-                # ---> Modified ingredient: {self.standardized_ingredient}""") if self.debug else None
+                # ---> Modified ingredient: {self._standardized_ingredient}""") if self.debug else None
 
     def _find_and_replace_number_words(self) -> None:
         """
         Replace number words with their corresponding numerical values in the parsed ingredient.
         """
-
-        # print("Parsing number words")
-        for word, regex_data in _regex_patterns.NUMBER_WORDS_MAP.items():
-            pattern = regex_data[1]
-            # print statement if word is found in ingredient and replaced
-            if pattern.search(self.standardized_ingredient):
-                # print(f"- Found {word} in ingredient. Replacing with {regex_data[0]}") if self.debug else None
-                self.standardized_ingredient = pattern.sub(regex_data[0], self.standardized_ingredient)
+        self._standardized_ingredient = _utils._find_and_replace_number_words(self._standardized_ingredient)
+        
+        return
 
     def _clean_hyphen_padded_substrings(self) -> None:
         """Find and remove hyphens around "to", "or", and "and" substrings in the parsed ingredient.
         For example, "1-to-3 cups of soup" becomes "1 to 3 cups of soup" and "1-or-2 cups of soup" becomes "1 or 2 cups of soup"
         """
 
         substrings_to_fix = ["to", "or", "and", "&"]
         
         for substring in substrings_to_fix:
-            self.standardized_ingredient = _utils._find_and_remove_hyphens_around_substring(self.standardized_ingredient, substring)
+            self._standardized_ingredient = _utils._find_and_remove_hyphens_around_substring(self._standardized_ingredient, substring)
 
-    
     def _clean_html_and_unicode(self) -> None:
         """Unescape fractions from HTML code coded fractions to unicode fractions."""
+        self._standardized_ingredient = _utils._clean_html_and_unicode(self._standardized_ingredient)
 
-        # Unescape HTML
-        self.standardized_ingredient = unescape(self.standardized_ingredient)
-
-        # Replace unicode fractions with their decimal equivalents
-        for unicode_fraction, decimal_fraction in _constants.UNICODE_FRACTIONS.items():
-            self.standardized_ingredient = self.standardized_ingredient.replace(unicode_fraction, f" {decimal_fraction}")
-            # self.standardized_ingredient = self.standardized_ingredient.replace(unicode_fraction, decimal_fraction)
+        return
+    
+    # # TODO: Delete this, _utils has replaced this
+    # def _clean_html_and_unicode2(self) -> None:
+    #     """Unescape fractions from HTML code coded fractions to unicode fractions."""
+
+    #     # Unescape HTML
+    #     self._standardized_ingredient = unescape(self._standardized_ingredient)
+
+    #     # Replace unicode fractions with their decimal equivalents
+    #     for unicode_fraction, decimal_fraction in _constants.UNICODE_FRACTIONS.items():
+    #         self._standardized_ingredient = self._standardized_ingredient.replace(unicode_fraction, f" {decimal_fraction}")
+    #         # self._standardized_ingredient = self._standardized_ingredient.replace(unicode_fraction, decimal_fraction)
 
     def _replace_unicode_fraction_slashes(self) -> None:
         """Replace unicode fraction slashes with standard slashes in the parsed ingredient."""
 
         # Replace unicode fraction slashes with standard slashes
-        self.standardized_ingredient = self.standardized_ingredient.replace('\u2044', '/') # could use .replace('\u2044', '\u002F'), or just .replace("⁄", "/")
-
+        self._standardized_ingredient = self._standardized_ingredient.replace('\u2044', '/') # could use .replace('\u2044', '\u002F'), or just .replace("⁄", "/")
+        
+        return 
+    
     def _add_whitespace(self):
         # regex pattern to match consecutive sequences of letters or digits
         pattern = _regex_patterns.CONSECUTIVE_LETTERS_DIGITS        
         # pattern = re.compile(r'([a-zA-Z]+)(\d+)|(\d+)([a-zA-Z]+)')
 
         # replace consecutive sequences of letters or digits with whitespace-separated sequences
-        self.standardized_ingredient = re.sub(pattern, r'\1 \2\3 \4', self.standardized_ingredient)
-    
-    # # TODO: Deprecated, DELETE
-    # def _fractions_to_decimals(self) -> None:
-    #     """
-    #     Replace fractions with their decimal equivalents in the parsed ingredient.
-    #     """
-    #     # print("Parsing fractions")
-    #     fractions = re.findall(IngredientSlicer.regex.FRACTION_PATTERN, self.standardized_ingredient)
-
-    #     split_frac = [i.replace(" ", "").split("/") for i in fractions]
-    #     split_frac = [(int(f[0]), int(f[1])) for f in split_frac]
-    #     fraction_decimal = [round(float(Fraction(f[0], f[1])), 3) for f in split_frac]
-
-    #     # replace fractions in original string with decimal equivalents
-    #     for i, f in enumerate(fractions):
-    #         self.standardized_ingredient = self.standardized_ingredient.replace(f, str(fraction_decimal[i]))
+        self._standardized_ingredient = re.sub(pattern, r'\1 \2\3 \4', self._standardized_ingredient)
     
-    # # TODO: Get rid of this (Deprecated, use the one in _utils.py)
-    # def _fraction_str_to_decimal(self, fraction_str: str) -> float:
-    #     """
-    #     Convert a string representation of a fraction to its decimal equivalent.
-    #     """
-    #     # Split the fraction string into its numerator and denominator
-    #     split_fraction = [i.strip() for i in fraction_str.split("/")]
-    #     # print(f"Split Fraction: {split_fraction}") if self.debug else None
-
-    #     # If the fraction is a whole number, return the number
-    #     if len(split_fraction) == 1:
-    #         # print(f"---> Only one part: {split_fraction[0]}")
-
-    #         converted_number = _utils._make_int_or_float_str(split_fraction[0])
-
-    #         # print(f"---> OLD Output: {round(float(split_fraction[0]), 3)}")
-    #         # print(f"---> NEW Output: {converted_number}")
-    #         return converted_number
-
-    #     numerator = int(split_fraction[0])
-    #     denominator = int(split_fraction[1])
-
-    #     # Convert the fraction to a decimal
-    #     # return round(float(Fraction(numerator, denominator)), 3)
-    #     return _utils._make_int_or_float_str(str(round(float(Fraction(numerator, denominator)), 3)))
-
     def _convert_fractions_to_decimals(self) -> None:
         """
         Convert fractions in the parsed ingredient to their decimal equivalents.
         """
-
-        # fraction_str = "1 to 1/2 cups, 2 and 5 animals, 2 2 / 4 cats, 1 and 1/22 cups water melon"
-        matches = _regex_patterns.FRACTION_PATTERN.findall(self.standardized_ingredient)
-        # matches = regex.FRACTION_PATTERN.findall(fraction_str)
-
-        # Replace fractions with their decimal equivalents
-        for match in matches:
-            # print(f"Match: {match}")
-
-            fraction_decimal = _utils._fraction_str_to_decimal(match)
-            # print(f"Fraction Decimal: {fraction_decimal}") if self.debug else None
-            self.standardized_ingredient = self.standardized_ingredient.replace(match, str(fraction_decimal))
-
-    def _force_ws(self):
+        self._standardized_ingredient = _utils._convert_fractions_to_decimals(self._standardized_ingredient)
+        
+        return
+    
+    def _force_ws_between_numbers_and_chars(self):
         
         """Forces spaces between numbers and units and between units and numbers.
         End result is a string with a space between numbers and units and between units and numbers.
         Examples:
         "1cup" becomes "1 cup"
         "cup1" becomes "cup 1" 
         and ultimately "1cup" becomes "1 - cup" and "cup1" becomes "cup - 1"
         """
 
-        NUMBERS_TO_LETTERS = re.compile(r"(\d)\-?([a-zA-Z])")  # 1cup
-        LETTERS_TO_NUMBERS = re.compile(r"([a-zA-Z])(\d)")     # cup1
-        LETTERS_DASH_NUMBERS = re.compile(r"([a-zA-Z])\-(\d)") # cup - 1
-
-        self.standardized_ingredient = NUMBERS_TO_LETTERS.sub(r"\1 \2", self.standardized_ingredient)
-        self.standardized_ingredient = LETTERS_TO_NUMBERS.sub(r"\1 \2", self.standardized_ingredient)
-        self.standardized_ingredient = LETTERS_DASH_NUMBERS.sub(r"\1 - \2", self.standardized_ingredient)
-
-    def _update_ranges(self, ingredient: str, pattern: re.Pattern, replacement_function=None) -> str:
-        """Update the ranges in the ingredient string with the updated ranges
-        Args:
-            ingredient (str): The ingredient string to update
-            pattern (re.Pattern): The pattern to use to find the ranges
-            replacement_function (function, optional): A function to use to replace the matched ranges. Defaults to None.
-        Returns:
-            str: The updated ingredient string
-        """
-        
-        # pattern = _regex_patterns.QUANTITY_DASH_QUANTITY
-        
-        matches = pattern.findall(ingredient)
-        # matched_ranges = [match.split("-") for match in matches]
-
-        if replacement_function:
-            # print(f"Replacement Function given")
-            matched_ranges = [replacement_function(match).split("-") for match in matches]
-        else:
-            # print(f"No Replacement Function given")
-            matched_ranges = [match.split("-") for match in matches]
-
-        # print(f"Matched Ranges: \n > {matched_ranges}") if self.debug else None
-
-        updated_ranges = [" - ".join([str(_utils._fraction_str_to_decimal(i)) for i in match if i]) for match in matched_ranges]
-        # updated_ranges = [" - ".join([str(int(i)) for i in match if i]) for match in matched_ranges]
-        
-        # Create a dictionary to map the matched ranges to the updated ranges
-        ranges_map = dict(zip(matches, updated_ranges))
-
-        # Replace the ranges in the original string with the updated ranges
-        for original_range, updated_range in ranges_map.items():
-            # print(f"Original Range: {original_range}")
-            # print(f"Updated Range: {updated_range}")
-            # if replacement_function:
-            #     print(f"Replacement Function given")
-            #     updated_range = replacement_function(updated_range)
-            ingredient = ingredient.replace(original_range, updated_range)
-            # print("\n") if self.debug else None
+        self._standardized_ingredient = _utils._force_ws_between_numbers_and_chars(self._standardized_ingredient)
 
-        return ingredient
+        return 
     
     def _extract_dimensions(self) -> None:
         """
         Extract dimensions from the parsed ingredient.
         """
 
-        self.standardized_ingredient, self.dimensions = _utils._extract_dimensions(self.standardized_ingredient)
+        self._standardized_ingredient, self._dimensions = _utils._extract_dimensions(self._standardized_ingredient)
         return
 
     def _average_ranges(self) -> None:
         """ Average all hyphen separated ranges of numbers in the parsed ingredient. """
-        self.standardized_ingredient = _utils.avg_ranges(self.standardized_ingredient)
+        self._standardized_ingredient = _utils.avg_ranges(self._standardized_ingredient)
         return
     
-    # TODO: write tests for this
+    # TODO:  DEPRECATED for _utils versions
     def _merge_misleading_ranges(self) -> None:
         """ Merge misleading ranges in the parsed ingredient (i.e. "4-1/2" is not a valid range, it should be "4.5" instead)"""
 
         # Find all the ranges in the ingredient
-        range_iter = _regex_patterns.QUANTITY_DASH_QUANTITY_GROUPS.finditer(self.standardized_ingredient)
+        range_iter = _regex_patterns.QUANTITY_DASH_QUANTITY_GROUPS.finditer(self._standardized_ingredient)
 
         offset = 0
 
         for match in range_iter:
             match_string    = match.group()
             start, end = match.start(), match.end()
             modified_start = start + offset
@@ -516,93 +379,94 @@
             # If the second number is less than the first number, then the range is misleading
             #  and the numbers should be merged (added if second number is a fraction)
             if second_number < first_number:
                 # print(f"Fixing misleading range: {match_string} with ")
                 second_number_is_fraction = second_number < 1
                 multiply_or_add_str = "add" if second_number_is_fraction else "multiply"
 
-                print(f"Second number is a fraction: {second_number_is_fraction}\n > '{multiply_or_add_str}' {first_number} and {second_number}") if self.debug else None
+                # print(f"Second number is a fraction: {second_number_is_fraction}\n > '{multiply_or_add_str}' {first_number} and {second_number}") if self.debug else None
 
                 updated_value = f" {_utils._make_int_or_float_str(str(first_number + second_number))} " if second_number_is_fraction else f" {_utils._make_int_or_float_str(str(first_number * second_number))} "
                 # updated_value = f" {_make_int_or_float_str(str(first_number + second_number))} "
-                print(f"Fixing misleading range: {match_string} with {updated_value}") if self.debug else None
+                # print(f"Fixing misleading range: {match_string} with {updated_value}") if self.debug else None
                 
-                self.standardized_ingredient = self.standardized_ingredient[:modified_start] + updated_value + self.standardized_ingredient[modified_end:]
+                self._standardized_ingredient = self._standardized_ingredient[:modified_start] + updated_value + self._standardized_ingredient[modified_end:]
                 offset += len(updated_value) - (end - start)
 
-                print(f"Ingredient after updating: {self.standardized_ingredient}") if self.debug else None
+                # print(f"Ingredient after updating: {self._standardized_ingredient}") if self.debug else None
 
-        self.standardized_ingredient = self.standardized_ingredient.strip()
+        self._standardized_ingredient = self._standardized_ingredient.strip()
 
         return
 
     def _fix_ranges(self):
         """
         Fix ranges in the parsed ingredient.
         Given a parsed ingredient, this method will fix ranges of numbers that are separated by one or more hyphens, ranges of numbers that are preceded by "between" and followed by "and" or "&", and ranges that are separated by "to" or "or".
         Examples:
         - "1-2 oz" -> "1 - 2 oz"
         - "between 1 and 5" -> "1 - 5"
         - "1 to 5" -> "1 - 5"
 
         """
-        print("Fixing ranges") if self.debug else None
+        # print("Fixing ranges") if self.debug else None
         # Define the regular expression pattern to match ranges
 
-        print(f"Before initial range update:\n {self.standardized_ingredient}") if self.debug else None
+        # print(f"Before initial range update:\n {self._standardized_ingredient}") if self.debug else None
 
         # # NOTE: NEW METHOD (in _utils.py)
         # Update ranges of numbers that are separated by one or more hyphens
-        self.standardized_ingredient = _utils._update_ranges(self.standardized_ingredient, _regex_patterns.QUANTITY_DASH_QUANTITY)
-        # self.standardized_ingredient = self._update_ranges(self.standardized_ingredient, _regex_patterns.QUANTITY_DASH_QUANTITY)
+        self._standardized_ingredient = _utils._update_ranges(self._standardized_ingredient, _regex_patterns.QUANTITY_DASH_QUANTITY)
+        # self._standardized_ingredient = self._update_ranges(self._standardized_ingredient, _regex_patterns.QUANTITY_DASH_QUANTITY)
 
-        print(f"After initial range update:\n {self.standardized_ingredient}") if self.debug else None
+        # print(f"After initial range update:\n {self._standardized_ingredient}") if self.debug else None
 
         # NOTE: NEW METHOD (in _utils.py)
         # # Update ranges of numbers that are preceded by "between" and followed by "and" or "&"
-        self.standardized_ingredient = _utils._update_ranges(self.standardized_ingredient, _regex_patterns.BETWEEN_QUANTITY_AND_QUANTITY)
-        # self.standardized_ingredient = self._update_ranges(self.standardized_ingredient, _regex_patterns.BETWEEN_QUANTITY_AND_QUANTITY, _utils._replace_and_with_hyphen)
+        self._standardized_ingredient = _utils._update_ranges(self._standardized_ingredient, _regex_patterns.BETWEEN_QUANTITY_AND_QUANTITY)
+        # self._standardized_ingredient = self._update_ranges(self._standardized_ingredient, _regex_patterns.BETWEEN_QUANTITY_AND_QUANTITY, _utils._replace_and_with_hyphen)
 
 
         # NOTE: NEW METHOD (in _utils.py)
         # Update ranges that are separated by "to" 
-        self.standardized_ingredient = _utils._update_ranges(self.standardized_ingredient, _regex_patterns.QUANTITY_TO_QUANTITY)
-        # self.standardized_ingredient = self._update_ranges(self.standardized_ingredient, _regex_patterns.QUANTITY_TO_QUANTITY, _utils._replace_to_with_hyphen)
+        self._standardized_ingredient = _utils._update_ranges(self._standardized_ingredient, _regex_patterns.QUANTITY_TO_QUANTITY)
+        # self._standardized_ingredient = self._update_ranges(self._standardized_ingredient, _regex_patterns.QUANTITY_TO_QUANTITY, _utils._replace_to_with_hyphen)
   
-        print(f"After 'TO' update:\n {self.standardized_ingredient}") if self.debug else None
+        # print(f"After 'TO' update:\n {self._standardized_ingredient}") if self.debug else None
 
         # NOTE: NEW METHOD (in _utils.py)
         # Update ranges that are separated by "or"
-        self.standardized_ingredient = _utils._update_ranges(self.standardized_ingredient, _regex_patterns.QUANTITY_OR_QUANTITY)
-        # self.standardized_ingredient = self._update_ranges(self.standardized_ingredient, _regex_patterns.QUANTITY_OR_QUANTITY, _utils._replace_or_with_hyphen)
+        self._standardized_ingredient = _utils._update_ranges(self._standardized_ingredient, _regex_patterns.QUANTITY_OR_QUANTITY)
+        # self._standardized_ingredient = self._update_ranges(self._standardized_ingredient, _regex_patterns.QUANTITY_OR_QUANTITY, _utils._replace_or_with_hyphen)
  
-        print(f"After 'OR' update:\n {self.standardized_ingredient}") if self.debug else None
+        # print(f"After 'OR' update:\n {self._standardized_ingredient}") if self.debug else None
 
         # check and merge any misleading ranges
-        self._merge_misleading_ranges()
+        self._standardized_ingredient = _utils._merge_misleading_ranges(self._standardized_ingredient)
+        # self._merge_misleading_ranges()
 
-        print(f"After misleading range update:\n {self.standardized_ingredient}") if self.debug else None
+        # print(f"After misleading range update:\n {self._standardized_ingredient}") if self.debug else None
 
         return
     
     # TODO: Replace "REPEAT_UNIT_RANGES" pattern with "QUANTITY_UNIT_DASH_QUANTITY_UNIT"
     # TODO: and use _utils version of this function
     def _remove_repeat_units(self) -> None:
         """
         Remove repeat units from the ingredient string.
         Examples:
         "2 oz - 3 oz diced tomatoes" -> "2 - 3 oz diced tomatoes"
         "3cups-4 cups of cats" -> "3 - 4 cups of cats"
         """
 
         # get any strings that match the pattern 1<unitA> - 2<unitA> or 1<unitA> - 2<unitB>
-        repeat_unit_matches = _regex_patterns.REPEAT_UNIT_RANGES.finditer(self.standardized_ingredient)
-        # repeat_unit_matches = _regex_patterns.QUANTITY_UNIT_DASH_QUANTITY_UNIT.finditer(self.standardized_ingredient)
+        repeat_unit_matches = _regex_patterns.REPEAT_UNIT_RANGES.finditer(self._standardized_ingredient)
+        # repeat_unit_matches = _regex_patterns.QUANTITY_UNIT_DASH_QUANTITY_UNIT.finditer(self._standardized_ingredient)
         
-        # matches = pattern.finditer(self.standardized_ingredient)
+        # matches = pattern.finditer(self._standardized_ingredient)
 
         for match in repeat_unit_matches:
 
             # original string matched by the pattern (used for replacement)
             original_string = match.group(0)
 
             # quantities from first quantity/unit pair
@@ -611,19 +475,19 @@
 
             # quantities from second quantity/unit pair
             quantity2 = match.group(3)
             unit2     = match.group(4)
 
             # if the units are the same, replace the original string with the quantities and units
             if unit1 == unit2:
-                self.standardized_ingredient = self.standardized_ingredient.replace(original_string, f"{quantity1} - {quantity2} {unit1}")
+                self._standardized_ingredient = self._standardized_ingredient.replace(original_string, f"{quantity1} - {quantity2} {unit1}")
     
     def _remove_repeat_units_in_ranges(self) -> None:
         
-        self.standardized_ingredient = _utils._remove_repeat_units_in_ranges(self.standardized_ingredient)
+        self._standardized_ingredient = _utils._remove_repeat_units_in_ranges(self._standardized_ingredient)
         
         return
     
     def _remove_x_separators(self):
         """
         Remove "x" separators from the ingredient string and replace with whitespace
         Examples:
@@ -633,15 +497,15 @@
             "5   cartons of eggs"
         """
 
         def replace_x(match):
             return match.group().replace('x', ' ').replace('X', ' ')
 
         # Replace "x"/"X" separators with whitespace
-        self.standardized_ingredient = _regex_patterns.X_AFTER_NUMBER.sub(replace_x, self.standardized_ingredient)
+        self._standardized_ingredient = _regex_patterns.X_AFTER_NUMBER.sub(replace_x, self._standardized_ingredient)
 
     def _merge_spaced_numbers(self, spaced_numbers: str) -> str:
         """ Add or multiply the numbers in a string separated by a space.
         If the second number is less than 1, then add the two numbers together, otherwise multiply them together.
         This was the most generic form of dealing with numbers seperated by spaces that i could come up with
         (i.e. 2 1/2 cups means 2.5 cups but in other contexts a number followed by a non fraction means to multiply the numbers 2 8 oz means 16 oz)
         Args:
@@ -714,15 +578,15 @@
 
         # go the spaced numbers matches and get each spaced seperated numbers match AND 
         # try and get the units that follow them so we can correctly match each spaced number with its corresponding unit
         spaced_nums = []
         units = []
 
         # Create iterable of the matched spaced numbers to insert updated values into the original string
-        spaced_matches = re.finditer(_regex_patterns.SPACE_SEP_NUMBERS, self.standardized_ingredient)
+        spaced_matches = re.finditer(_regex_patterns.SPACE_SEP_NUMBERS, self._standardized_ingredient)
         # spaced_matches = re.finditer(regex_map.SPACE_SEP_NUMBERS, ingredient)
 
         # initialize offset and replacement index values for updating the ingredient string, 
         # these will be used to keep track of the position of the match in the string
         offset = 0
         replacement_index = 0
 
@@ -730,97 +594,87 @@
         for match in spaced_matches:
             # print(f"Ingredient string: {ingredient}")
 
             # Get the start and end positions of the match
             start, end = match.start(), match.end()
 
             # search for the first unit that comes after the spaced numbers
-            unit_after_match = re.search(_regex_patterns.UNITS_PATTERN,  self.standardized_ingredient[end:])
+            unit_after_match = re.search(_regex_patterns.UNITS_PATTERN,  self._standardized_ingredient[end:])
             # unit_after_match = re.search(regex_map.UNITS_PATTERN, ingredient[end:])
             
             if unit_after_match:
-                # print(f"unit after match: > '{unit_after_match.group()}'")
                 units.append(unit_after_match.group())
 
             # add the spaced number to the list
             spaced_nums.append(match.group())
 
-            # print(f"Match: {match.group()} at positions {start}-{end}")
             merged_quantity = self._merge_spaced_numbers(match.group())
             merge_operation = self._which_merge_on_spaced_numbers(match.group())
 
-            # print(f"merged_quantity: {merged_quantity}") if self.debug else None
-            # print(f"merge_operation: {merge_operation}\n") if self.debug else None
-
-            # Calculate the start and end positions in the modified string
             modified_start = start + offset
             modified_end = end + offset
 
-            # print(f" -> Modified match positions: {modified_start}-{modified_end}")
-            # print(f"Replacing {match.group()} with '{merged_quantity}'...") if self.debug else None
-            
-            # Construct the modified string with the replacement applied
-            self.standardized_ingredient = self.standardized_ingredient[:modified_start] + str(merged_quantity) + self.standardized_ingredient[modified_end:]
+            self._standardized_ingredient = self._standardized_ingredient[:modified_start] + str(merged_quantity) + self._standardized_ingredient[modified_end:]
             # ingredient = ingredient[:modified_start] + str(merged_quantity) + ingredient[modified_end:]
 
             # Update the offset for subsequent replacements
             offset += len(merged_quantity) - (end - start)
             replacement_index += 1
 
     def _replace_a_or_an_quantities(self) -> None:
         """
         Replace "a" or "an" with "1" in the parsed ingredient if no number is present in the ingredient string.
         """
-        self.standardized_ingredient = _utils._replace_a_or_an_quantities(self.standardized_ingredient)
+        self._standardized_ingredient = _utils._replace_a_or_an_quantities(self._standardized_ingredient)
         return 
     
     def _drop_special_characters(self):
 
         # Drop unwanted periods and replace them with whitespace
-        self.standardized_ingredient = self.standardized_ingredient.replace(".", " ")
+        self._standardized_ingredient = self._standardized_ingredient.replace(".", " ")
 
     def _separate_dimensions(self) -> None:
         """
         Split the dimensions from the parsed ingredient.
         """
         # Split the dimensions from the ingredient
-        self.standardized_ingredient, self.dimensions = _utils._separate_dimensions(self.standardized_ingredient)
+        self._standardized_ingredient, self._dimensions = _utils._separate_dimensions(self._standardized_ingredient)
         return
 
     def _separate_parenthesis(self):
         
         """Get the content of any parenthesis and store it for analysis later on, also remove those parenthesis from the ingredient.
-        Updates the parenthesis_content and reduced_ingredient variables
+        Updates the parenthesis_content and _reduced_ingredient variables
         """
 
         # # split the ingredient string by the open/close parenthesis sets
-        # no_parenthesis1 = re.split(_regex_patterns.SPLIT_BY_PARENTHESIS, self.standardized_ingredient)
+        # no_parenthesis1 = re.split(_regex_patterns.SPLIT_BY_PARENTHESIS, self._standardized_ingredient)
         # # remove any leading or trailing whitespace from the split strings and join them back together
         # no_parenthesis1 = " ".join([i.strip() for i in no_parenthesis1])
-        # parenthesis1 = re.findall(_regex_patterns.SPLIT_BY_PARENTHESIS, self.standardized_ingredient)
+        # parenthesis1 = re.findall(_regex_patterns.SPLIT_BY_PARENTHESIS, self._standardized_ingredient)
         # # parenthesis = re.findall(_regex_patterns.SPLIT_BY_PARENTHESIS, ingredient)
         
-        ingredient_without_parenthesis, parenthesis = _utils._split_by_parenthesis(self.standardized_ingredient)
+        ingredient_without_parenthesis, parenthesis = _utils._split_by_parenthesis(self._standardized_ingredient)
 
         # # update the paranthensis object with the parsed values
         # self.parenthesis_obj["raw_ingredient"] = self.ingredient
-        # self.parenthesis_obj["standard_ingredient"] = self.standardized_ingredient
-        # self.parenthesis_obj["reduced_ingredient"] = no_parenthesis
+        # self.parenthesis_obj["standard_ingredient"] = self._standardized_ingredient
+        # self.parenthesis_obj["_reduced_ingredient"] = no_parenthesis
         # self.parenthesis_obj["parenthesis_content"] = parenthesis
         
-        self.staged_ingredient = self.standardized_ingredient
+        self._staged_ingredient = self._standardized_ingredient
 
-        # set "reduced_ingredient" to the parsed ingredient with parenthesis removed
-        # self.reduced_ingredient = ingredient_without_parenthesis # TODO: TESTING THIS OUT
-        self.standardized_ingredient = ingredient_without_parenthesis # TODO: TESTING THIS OUT
-        # self.reduced_ingredient = no_parenthesis
+        # set "_reduced_ingredient" to the parsed ingredient with parenthesis removed
+        # self._reduced_ingredient = ingredient_without_parenthesis # TODO: TESTING THIS OUT
+        self._standardized_ingredient = ingredient_without_parenthesis # TODO: TESTING THIS OUT
+        # self._reduced_ingredient = no_parenthesis
 
         # set "parenthesis_content" to the parsed parenthesis strings
-        self.parenthesis_content = parenthesis
-        # self.parenthesis_content = parenthesis1
+        self._parenthesis_content = parenthesis
+        # self._parenthesis_content = parenthesis1
     
     # return parsed_parenthesis
         
     # TODO: delete this 
     # def _pull_units(self):
     #     """
     #     Pull out all of the units in the string
@@ -840,22 +694,22 @@
     #         {'units': ['cups', 'tablespoons', 'stick'],
     #             'basic_units': ['cups', 'tablespoons', 'stick'],
     #             'nonbasic_units': ['stick'],
     #             'volumetric_units': ['cups', 'tablespoons'],
     #             'has_unit': True}
     #     """
 
-    #     if not self.reduced_ingredient:
+    #     if not self._reduced_ingredient:
     #         return None
         
     #     # initliaze the has_unit flag to True, if no units are found, then the flag will be set to False
     #     has_unit = True
 
     #     # get all of the units in the ingredient string
-    #     all_units = _regex_patterns.UNITS_PATTERN.findall(self.reduced_ingredient)
+    #     all_units = _regex_patterns.UNITS_PATTERN.findall(self._reduced_ingredient)
 
     #     # get the basic units in the ingredient string by checking if the units are in the basic units set
     #     basic_units = [unit for unit in all_units if unit in _constants.BASIC_UNITS_SET]
     #     # basic_units = regex.BASIC_UNITS_PATTERN.findall(ingredient) # Does the same thing but uses regex, probably better to NOT regex backtrack if we can avoid it..
 
     #     # get the nonbasic units in the ingredient string by checking if the units are not in the basic units set
     #     nonbasic_units = list(set(all_units) - set(basic_units))
@@ -870,19 +724,19 @@
 
     #     self.found_units = {"units" : all_units,
     #                 "basic_units" : basic_units,
     #                 "nonbasic_units" : nonbasic_units,
     #                 "volumetric_units" : volumetric_units,
     #                 "has_unit" : has_unit}
     
-    def standardize(self):
+    def _standardize(self):
         
-        # TODO: make sure to reset the standardized_ingredient to the original ingredient 
+        # TODO: make sure to reset the _standardized_ingredient to the original ingredient 
         # TODO: string before starting the standardization process
-        # self.standardized_ingredient = self.ingredient
+        # self._standardized_ingredient = self.ingredient
 
         # define a list containing the class methods that should be called in order on the input ingredient string
         methods = [
             self._drop_special_dashes,
             self._find_and_remove_percentages,
             self._replace_number_followed_by_inch_symbol,
             self._find_and_replace_casual_quantities, # NOTE: testing this out
@@ -890,15 +744,16 @@
             self._find_and_replace_number_words,
             self._find_and_replace_fraction_words, # NOTE: testing this out
             self._clean_html_and_unicode,
             self._replace_unicode_fraction_slashes,
             self._convert_fractions_to_decimals,
             # self._fix_ranges, # TODO: ORIGINAL place for fix_ranges() ---> need to decide where this should go
             # self._remove_x_separators,
-            self._force_ws,
+            # self._force_ws,
+            self._force_ws_between_numbers_and_chars,
             # self._extract_dimensions,
             # self._remove_repeat_units,
             self._remove_repeat_units_in_ranges,
             self._separate_dimensions,
             self._remove_x_separators,
             self._clean_hyphen_padded_substrings, # TODO: Still needs tests written for this
             self._merge_multi_nums,
@@ -909,47 +764,47 @@
             self._average_ranges,
             # self._avg_ranges2,
             # self._avg_ranges,
             # self._separate_dimensions,
             self._separate_parenthesis
             # self._pull_units
         ]
-
+        # print(f"Ingredient before standardizing: {self._standardized_ingredient}") if self.debug else None
         # call each method in the list on the input ingredient string
         for method in methods:
-            print(f"Calling method: {method.__name__}") if self.debug else None
-            print(f"> Starting ingredient: '{self.standardized_ingredient}'") if self.debug else None
+            # print(f"Calling method: {method.__name__}") if self.debug else None
+            # print(f"> Starting ingredient: '{self._standardized_ingredient}'") if self.debug else None
 
             method()
 
-            print(f"> Ending ingredient: '{self.standardized_ingredient}'") if self.debug else None
-        
+            # print(f"> Ending ingredient: '{self._standardized_ingredient}'") if self.debug else None
         
-        print(f"Removing extra whitespaces...") if self.debug else None
+        # print(f"Ingredient after standardizing: {self._standardized_ingredient}") if self.debug else None
+        # print(f"Removing extra whitespaces...") if self.debug else None
 
-        self.standardized_ingredient = _utils._remove_extra_whitespaces(self.standardized_ingredient)
-        # self.standardized_ingredient = self._remove_extra_whitespaces(self.standardized_ingredient)
+        self._standardized_ingredient = _utils._remove_extra_whitespaces(self._standardized_ingredient)
+        # self._standardized_ingredient = self._remove_extra_whitespaces(self._standardized_ingredient)
 
-        print(f"Done, returning standardized ingredient: \n > '{self.standardized_ingredient}'") if self.debug else None
+        # print(f"Done, returning standardized ingredient: \n > '{self._standardized_ingredient}'") if self.debug else None
 
         # return the parsed ingredient string
-        # return self.standardized_ingredient
+        # return self._standardized_ingredient
         return
 
     def extract_first_quantity_unit(self) -> None:
 
         """
         Extract the first unit and quantity from an ingredient string.
-        Function will extract the first unit and quantity from the ingredient string and set the self.quantity and self.unit member variables.
+        Function will extract the first unit and quantity from the ingredient string and set the self._quantity and self._unit member variables.
         Quantities and ingredients are extracted in this order and if any of the previous steps are successful, the function will return early.
         1. Check for basic units (e.g. 1 cup, 2 tablespoons)
         2. Check for nonbasic units (e.g. 1 fillet, 2 carrot sticks)
         3. Check for quantity only, no units (e.g. 1, 2)
 
-        If none of the above steps are successful, then the self.quantity and self.unit member variables will be set to None.
+        If none of the above steps are successful, then the self._quantity and self._unit member variables will be set to None.
 
         Args:
             ingredient (str): The ingredient string to parse.
         Returns:
             dict: A dictionary containing the first unit and quantity found in the ingredient string.
         Examples:
             >>> extract_first_unit_quantity('1 1/2 cups diced tomatoes, 2 tablespoons of sugar, 1 stick of butter')
@@ -958,62 +813,62 @@
             {'quantity': '2 1/2', 'unit': 'cups'}
         """
         
         # ---- STEP 1: CHECK FOR QUANTITY - BASIC UNITS (e.g. 1 cup, 2 tablespoons) ----
         # Example: "1.5 cup of sugar" -> quantity: "1.5", unit: "cup"
 
         # get the first number followed by a basic unit in the ingredient string
-        # basic_unit_matches = _regex_patterns.QUANTITY_BASIC_UNIT_GROUPS.findall(self.reduced_ingredient)
-        basic_unit_matches = _regex_patterns.QUANTITY_BASIC_UNIT_GROUPS.findall(self.standardized_ingredient) # TODO: testing
-        # basic_unit_matches = regex.QUANTITY_BASIC_UNIT_GROUPS.findall(reduced_ingredient)
+        basic_unit_matches = _regex_patterns.QUANTITY_BASIC_UNIT_GROUPS.findall(self._standardized_ingredient) # TODO: testing
+        # basic_unit_matches = _regex_patterns.QUANTITY_BASIC_UNIT_GROUPS.findall(self._reduced_ingredient)
+        # basic_unit_matches = regex.QUANTITY_BASIC_UNIT_GROUPS.findall(_reduced_ingredient)
 
         # remove any empty matches
         valid_basic_units = [i for i in basic_unit_matches if len(i) > 0]
 
         # debugging message
         basic_units_message = f"Valid basic units: {valid_basic_units}" if valid_basic_units else f"No valid basic units found..."
         # print(basic_units_message) if self.debug else None
 
-        # if we have valid single number quantities, then set the self.quantity and the self.unit member variables and exit the function
+        # if we have valid single number quantities, then set the self._quantity and the self._unit member variables and exit the function
         if basic_unit_matches and valid_basic_units:
-            self.quantity = valid_basic_units[0][0].strip()
-            self.unit = valid_basic_units[0][1].strip()
-            # return {"quantity": self.quantity, "unit": self.unit}
+            self._quantity = valid_basic_units[0][0].strip()
+            self._unit = valid_basic_units[0][1].strip()
+            # return {"quantity": self._quantity, "unit": self._unit}
             return 
 
         # ---- STEP 2: CHECK FOR QUANTITY - NONBASIC UNITS (e.g. 1 fillet, 2 carrot sticks) ----
         # Example: "1 fillet of salmon" -> quantity: "1", unit: "fillet"
 
         # If no basic units are found, then check for anumber followed by a nonbasic units
-        # nonbasic_unit_matches = _regex_patterns.QUANTITY_NON_BASIC_UNIT_GROUPS.findall(self.reduced_ingredient)
-        nonbasic_unit_matches = _regex_patterns.QUANTITY_NON_BASIC_UNIT_GROUPS.findall(self.standardized_ingredient) # TODO: testing
-        # nonbasic_unit_matches = regex.QUANTITY_NON_BASIC_UNIT_GROUPS.findall(reduced_ingredient)
+        # nonbasic_unit_matches = _regex_patterns.QUANTITY_NON_BASIC_UNIT_GROUPS.findall(self._reduced_ingredient)
+        nonbasic_unit_matches = _regex_patterns.QUANTITY_NON_BASIC_UNIT_GROUPS.findall(self._standardized_ingredient) # TODO: testing
+        # nonbasic_unit_matches = regex.QUANTITY_NON_BASIC_UNIT_GROUPS.findall(_reduced_ingredient)
 
         # remove any empty matches
         valid_nonbasic_units = [i for i in nonbasic_unit_matches if len(i) > 0]
 
         # debugging message
         nonbasic_units_message = f"Valid non basic units: {valid_nonbasic_units}" if valid_nonbasic_units else f"No valid non basic units found..."
-        print(nonbasic_units_message) if self.debug else None
+        # print(nonbasic_units_message) if self.debug else None
 
-        # if we found a number followed by a non basic unit, then set the self.quantity and the self.unit member variables and exit the function
+        # if we found a number followed by a non basic unit, then set the self._quantity and the self._unit member variables and exit the function
         if nonbasic_unit_matches and valid_nonbasic_units:
-            self.quantity = valid_nonbasic_units[0][0].strip()
-            self.unit = valid_nonbasic_units[0][1].strip()
-            # return {"quantity": self.quantity, "unit": self.unit}
+            self._quantity = valid_nonbasic_units[0][0].strip()
+            self._unit = valid_nonbasic_units[0][1].strip()
+            # return {"quantity": self._quantity, "unit": self._unit}
             return
         
         # ---- STEP 3: CHECK FOR ANY QUANTITIES or ANY UNITS in the string, and use the first instances (if they exist) ----
         # Example: "cups, 2 juice of lemon" -> quantity: "2", unit: "juice"
 
         # if neither basic nor nonbasic units are found, then get all of the numbers and all of the units
-        # quantity_matches = _regex_patterns.ALL_NUMBERS.findall(self.reduced_ingredient)
-        # unit_matches     = _regex_patterns.UNITS_PATTERN.findall(self.reduced_ingredient)
-        quantity_matches = _regex_patterns.ALL_NUMBERS.findall(self.standardized_ingredient) # TODO: testing
-        unit_matches     = _regex_patterns.UNITS_PATTERN.findall(self.standardized_ingredient) # TODO: testing
+        quantity_matches = _regex_patterns.ALL_NUMBERS.findall(self._standardized_ingredient) # TODO: testing
+        unit_matches     = _regex_patterns.UNITS_PATTERN.findall(self._standardized_ingredient) # TODO: testing
+        # quantity_matches = _regex_patterns.ALL_NUMBERS.findall(self._reduced_ingredient)
+        # unit_matches     = _regex_patterns.UNITS_PATTERN.findall(self._reduced_ingredient)
 
         # remove any empty matches
         valid_quantities = [i for i in quantity_matches if len(i) > 0]
         valid_units     = [i for i in unit_matches if len(i) > 0]
 
         # debugging messages
         all_quantities_message = f"Valid quantities: {valid_quantities}" if valid_quantities else f"No valid quantities found..."
@@ -1022,39 +877,39 @@
         # print(all_quantities_message) if self.debug else None
         # print(all_units_message) if self.debug else None
 
         # if either have valid quantities then set the best quantity and best unit to 
         # the first valid quantity and units found, otherwise set as None
         # TODO: Drop this "if valid_quantities or valid_units"...?
         if valid_quantities or valid_units:
-            self.quantity = valid_quantities[0].strip() if valid_quantities else None
-            self.unit = valid_units[0].strip() if valid_units else None
-            # return {"quantity": self.quantity, "unit": self.unit}
+            self._quantity = valid_quantities[0].strip() if valid_quantities else None
+            self._unit = valid_units[0].strip() if valid_units else None
+            # return {"quantity": self._quantity, "unit": self._unit}
             return
 
         # # ---- STEP 3: CHECK FOR QUANTITY - NO UNITS (e.g. 1, 2) ----
 
         # # if neither basic nor nonbasic units are found, then get the first number
-        # quantity_matches = _regex_patterns.ALL_NUMBERS.findall(self.reduced_ingredient)
-        # # quantity_matches = regex.ALL_NUMBERS.findall(reduced_ingredient)
+        # quantity_matches = _regex_patterns.ALL_NUMBERS.findall(self._reduced_ingredient)
+        # # quantity_matches = regex.ALL_NUMBERS.findall(_reduced_ingredient)
         # # remove any empty matches
         # valid_quantities = [i for i in quantity_matches if len(i) > 0]
         # # debugging message
         # quantity_only_message = f"Valid quantities: {valid_quantities}" if valid_quantities else f"No valid quantities found..."
         # print(quantity_only_message)
         # # print(quantity_only_message) if self.debug else None
         # # if we have valid single number quantities, then return the first one
         # if quantity_matches and valid_quantities:
-        #     self.quantity = valid_quantities[0].strip()
-        #     # return {"quantity": self.quantity, "unit": self.unit}
+        #     self._quantity = valid_quantities[0].strip()
+        #     # return {"quantity": self._quantity, "unit": self._unit}
         #     return
             
         # # ---- STEP 4: UNITS ONLY ----
-        # regex.print_matches(reduced_ingredient)
-        # unit_matches = regex.UNITS_PATTERN.findall(reduced_ingredient)
+        # regex.print_matches(_reduced_ingredient)
+        # unit_matches = regex.UNITS_PATTERN.findall(_reduced_ingredient)
 
         # ---- STEP 4: NO MATCHES ----
         # just print a message if no valid quantities or units are found and return None
         # best_quantity and best_unit are set to None by default and will remain that way if no units or quantities were found.
         no_matches_message = f"No valid quantities or units found..."
         # print(no_matches_message) if self.debug else None
 
@@ -1106,151 +961,149 @@
         required_str_flag = any([True if word in required_set else False for word in ingredient.replace(",", " ").split()])
 
         # if any "required" strings were matched or found, or if no "optional" strings were matched or found, then the ingredient is required
         is_required = (True if required_match_flag or required_str_flag else False) or (False if optional_match_flag or optional_str_flag else True)
 
         return is_required
     
-    def _is_required(self) -> bool:
+    def _is_ingredient_required(self) -> bool:
         """
         Check if the ingredient is required or optional
         Returns a boolean indicating whether the ingredient is required or optional.
         """
 
         # check if the ingredient string contains the word "optional" or "required"
-        # ingredient_is_required = self._check_if_required_string(self.reduced_ingredient)
-        ingredient_is_required = self._check_if_required_string(self.standardized_ingredient) # TODO: testing this out
+        # ingredient_is_required = self._check_if_required_string(self._reduced_ingredient)
+        ingredient_is_required = self._check_if_required_string(self._standardized_ingredient) # TODO: testing this out
 
         # check the parenthesis content for the word "optional" or "required"
-        parenthesis_is_required = self._check_if_required_parenthesis(self.parenthesis_content)
+        parenthesis_is_required = self._check_if_required_parenthesis(self._parenthesis_content)
 
         # if BOTH of the above conditions are True then return True otherwise return False
         return True if ingredient_is_required and parenthesis_is_required else False
     
     def _address_quantity_only_parenthesis(self, parenthesis: str) -> None:
         """
         Address the case where the parenthesis content only contains a quantity.
-        Attempts to update self.quantity, self.unit, self.secondary_quantity, and self.secondary_unit given 
-        information from the parenthesis string and the current self.quantity and self.unit
+        Attempts to update self._quantity, self._unit, self._secondary_quantity, and self._secondary_unit given 
+        information from the parenthesis string and the current self._quantity and self._unit
         (e.g. "(3)", "(2.5)", "(1/2)")
         Args:
             parenthesis (str): The content of the parenthesis in the ingredient string.
         Returns:
             None
         """
-        
-        # print(f"""Ingredient: '{self.reduced_ingredient}'\nParenthesis: '{parenthesis}'\nQuantity: '{self.quantity}'\nUnit: '{self.unit}'""") if self.debug else None
 
         # Set a None Description
         description = None
 
         # pull out the parenthesis quantity values
         numbers_only = _utils._extract_quantities_only(parenthesis) # NOTE: testing this out
         # numbers_only = _regex_patterns.PARENTHESIS_WITH_NUMBERS_ONLY.findall(parenthesis)
 
         # if no numbers only parenthesis, then just return the original ingredient
         if not numbers_only:
-            print(f"\n > Return early from QUANTITY parenthesis") if self.debug else None
+            # print(f"\n > Return early from QUANTITY parenthesis") if self.debug else None
             description = f"not a quantity only parenthesis"
-            self.parenthesis_notes.append(description)
+            self._parenthesis_notes.append(description)
             return
 
-        # pull out the self.quantity from the parenthesis
+        # pull out the self._quantity from the parenthesis
         parenthesis_quantity = numbers_only[0]
 
         # if there is not a unit or a quantity, then we can use the parenthesis number as the quantity and
         #  return the ingredient with the new quantity
         # TODO: OR the unit MIGHT be the food OR might be a "SOMETIMES_UNIT", maybe do that check here, not sure yet...
-        if not self.quantity and not self.unit:
+        if not self._quantity and not self._unit:
             description = f"maybe unit is: the 'food' or a 'sometimes unit'"
-            self.parenthesis_notes.append(description)
+            self._parenthesis_notes.append(description)
 
-            self.quantity = parenthesis_quantity
+            self._quantity = parenthesis_quantity
             return
         
         # if there is a quantity but no unit, we can try to merge (multiply) the current quantity and the parenthesis quantity 
         # then the unit is also likely the food 
         # TODO: OR the unit MIGHT be the food OR might be a "SOMETIMES_UNIT", maybe do that check here, not sure yet...
-        if self.quantity and not self.unit:
-            updated_quantity = str(float(self.quantity) * float(parenthesis_quantity))
+        if self._quantity and not self._unit:
+            updated_quantity = str(float(self._quantity) * float(parenthesis_quantity))
             
             description = f"maybe unit is: the 'food' or a 'sometimes unit'"
-            self.parenthesis_notes.append(description)
+            self._parenthesis_notes.append(description)
 
             # set the secondary quantity to the ORIGINAL quantity/units
-            self.secondary_quantity = self.quantity 
+            self._secondary_quantity = self._quantity 
 
             # Update the quantity with the updated merged quantity
-            self.quantity = _utils._make_int_or_float_str(updated_quantity)
-            # self.quantity = updated_quantity
+            self._quantity = _utils._make_int_or_float_str(updated_quantity)
+            # self._quantity = updated_quantity
 
-            # return [updated_quantity, self.unit, description]
+            # return [updated_quantity, self._unit, description]
             return
         
         # if there is a unit but no quantity, then we can use the parenthesis number as the quantity and 
         # return the ingredient with the new quantity
-        if not self.quantity and self.unit:
+        if not self._quantity and self._unit:
             # updated_quantity = numbers_only[0]
             description = f"used quantity from parenthesis"
-            self.parenthesis_notes.append(description)
+            self._parenthesis_notes.append(description)
 
             # set the secondary quantity to the ORIGINAL quantity/units
-            self.secondary_quantity = self.quantity 
+            self._secondary_quantity = self._quantity 
 
             # set the quantity to the parenthesis quantity
-            self.quantity = parenthesis_quantity
+            self._quantity = parenthesis_quantity
 
             return
 
         # if there is a quantity and a unit, then we can try
         # to merge (multiply) the current quantity and the parenthesis quantity
         # then return the ingredient with the new quantity
-        if self.quantity and self.unit:
+        if self._quantity and self._unit:
             # if there is a quantity and a unit, then we can try to merge (multiply) the current quantity and the parenthesis quantity
             # then return the ingredient with the new quantity
 
             description = f"multiplied starting quantity with parenthesis quantity"
-            self.parenthesis_notes.append(description)
+            self._parenthesis_notes.append(description)
 
-            updated_quantity = str(float(self.quantity) * float(parenthesis_quantity))
+            updated_quantity = str(float(self._quantity) * float(parenthesis_quantity))
 
             # set the secondary quantity to the ORIGINAL quantity/units
-            self.secondary_quantity = self.quantity 
+            self._secondary_quantity = self._quantity 
 
             # Update the quantity with the updated merged quantity (original quantity * parenthesis quantity)
-            self.quantity = _utils._make_int_or_float_str(updated_quantity)
-            # self.quantity = updated_quantity
+            self._quantity = _utils._make_int_or_float_str(updated_quantity)
+            # self._quantity = updated_quantity
 
             return
 
         description = f"used quantity from parenthesis with quantity only"
-        self.parenthesis_notes.append(description)
+        self._parenthesis_notes.append(description)
         
         # set the secondary quantity to the ORIGINAL quantity/units
-        self.secondary_quantity = self.quantity 
+        self._secondary_quantity = self._quantity 
 
         # update the quantity with the parenthesis quantity value
-        self.quantity = parenthesis_quantity
+        self._quantity = parenthesis_quantity
 
         return
     
     def _address_equivalence_parenthesis(self, parenthesis: str) -> None:
         """
         Address the case where the parenthesis content contains any equivalence strings like "about" or "approximately", followed by a quantity and then a unit later in the sting.
-        Attempts to update self.quantity, self.unit, self.secondary_quantity, and self.secondary_unit given 
-        information from the parenthesis string and the current self.quantity and self.unit
+        Attempts to update self._quantity, self._unit, self._secondary_quantity, and self._secondary_unit given 
+        information from the parenthesis string and the current self._quantity and self._unit
         e.g. "(about 3 ounces)", "(about a 1/3 cup)", "(approximately 1 large tablespoon)"
 
         Args:
             parenthesis (str): A string containing parenthesis from the ingredients string
         Returns:
             None
         """
 
-        # print(f"""Ingredient: '{self.reduced_ingredient}'\nParenthesis: '{parenthesis}'\nQuantity: '{self.quantity}'\nUnit: '{self.unit}'""") if self.debug else None
+        # print(f"""Ingredient: '{self._reduced_ingredient}'\nParenthesis: '{parenthesis}'\nQuantity: '{self._quantity}'\nUnit: '{self._unit}'""") if self.debug else None
 
         
         # Set a None Description
         description = None
 
         # check for the equivelency pattern (e.g. "<equivelent string> <quantity> <unit>" )
         equivalent_quantity_unit = _utils._extract_equivalent_quantity_units(parenthesis)
@@ -1262,389 +1115,389 @@
 
         # Case when: NO equivelence quantity unit matches 
         #           OR parenthesis contains a quantity per unit like string in the parenthesis (i.e. "(about 2 ounces each)" contains "each")
         # Then return early with NO UPDATES and keep the current quantity/unit as is
         if not equivalent_quantity_unit or any([True if i in _constants.QUANTITY_PER_UNIT_STRINGS else False for i in split_parenthesis]):
             # print(f"\n > Return early from EQUIVALENCE parenthesis") if self.debug else None
             description = f"not a equivalence quantity unit parenthesis"
-            self.parenthesis_notes.append(description)
+            self._parenthesis_notes.append(description)
             return
         
         # pull out the suffix word, parenthesis quantity and unit
         parenthesis_suffix, parenthesis_quantity, parenthesis_unit = equivalent_quantity_unit[0]
         
         # Case when: NO quantity, NO unit:
             # if no quantity AND no unit, then we can use the parenthesis quantity-unit as our quantity and unit
-        if not self.quantity and not self.unit:
+        if not self._quantity and not self._unit:
 
             description = f"used equivalence quantity unit as our quantity and unit"
-            self.parenthesis_notes.append(description)
+            self._parenthesis_notes.append(description)
 
             # set quantity/unit to the parenthesis values
-            self.quantity = parenthesis_quantity
-            self.unit = parenthesis_unit
+            self._quantity = parenthesis_quantity
+            self._unit = parenthesis_unit
 
             return
         
         # Case when: YES quantity, NO unit:
             # we can assume the equivelent quantity units 
             # in the parenthesis are actually a better fit for the quantities and units so 
             # we can use those are our quantities/units and then stash the original quantity in the "description" field 
             # with a "maybe quantity is " prefix in front of the original quantity for maybe use later on
-        if self.quantity and not self.unit:
+        if self._quantity and not self._unit:
 
             # stash the old quantity with a trailing string before changing best_quantity
-            description = f"maybe quantity is: {' '.join(self.quantity)}"
-            self.parenthesis_notes.append(description)
+            description = f"maybe quantity is: {' '.join(self._quantity)}"
+            self._parenthesis_notes.append(description)
 
             # make the secondary_quantity the starting quantity before converting the quantity to the value found in the parenthesis
-            self.secondary_quantity = self.quantity
+            self._secondary_quantity = self._quantity
 
             # set the quantity/unit to the parenthesis values
-            self.quantity = parenthesis_quantity
-            self.unit = parenthesis_unit
+            self._quantity = parenthesis_quantity
+            self._unit = parenthesis_unit
 
             return 
 
         # Case when: NO quantity, YES unit:
             # if there is no quantity BUT there IS a unit, then the parenthesis units/quantities are probably "better" so use the
             # parenthesis quantity/units and then stash the old unit in the description
-        if not self.quantity and self.unit:
+        if not self._quantity and self._unit:
 
             # stash the old quantity with a trailing "maybe"
-            description = f"maybe unit is: {self.unit}"
-            self.parenthesis_notes.append(description)
+            description = f"maybe unit is: {self._unit}"
+            self._parenthesis_notes.append(description)
 
             # make the secondary_unit the starting unit before converting the unit to the unit string found in the parenthesis
-            self.secondary_unit = self.unit
+            self._secondary_unit = self._unit
 
-            self.quantity = parenthesis_quantity
-            self.unit = parenthesis_unit
+            self._quantity = parenthesis_quantity
+            self._unit = parenthesis_unit
 
             # return [parenthesis_quantity, parenthesis_unit, description]
             return 
         
         # Case when: YES quantity, YES unit:
             # if we already have a quantity AND a unit, then we likely found an equivalent quantity/unit
             # we will choose to use the quantity/unit pairing that is has a unit in the BASIC_UNITS_SET
-        if self.quantity and self.unit:
+        if self._quantity and self._unit:
             parenthesis_unit_is_basic = parenthesis_unit in _constants.BASIC_UNITS_SET
-            unit_is_basic = self.unit in _constants.BASIC_UNITS_SET
+            unit_is_basic = self._unit in _constants.BASIC_UNITS_SET
 
             # Case when BOTH are basic units:  (# TODO: Maybe we should use parenthesis quantity/unit instead...?)
             #   use the original quantity/unit (stash the parenthesis in the description)
             if parenthesis_unit_is_basic and unit_is_basic:
                 description = f"maybe quantity/unit is: {parenthesis_quantity}/{parenthesis_unit}"
-                self.parenthesis_notes.append(description)
-                # return [self.quantity, self.unit, description]
+                self._parenthesis_notes.append(description)
+                # return [self._quantity, self._unit, description]
 
                 # set the secondary quantity/units to the values in the parenthesis
-                self.secondary_quantity = parenthesis_quantity
-                self.secondary_unit = parenthesis_unit
+                self._secondary_quantity = parenthesis_quantity
+                self._secondary_unit = parenthesis_unit
 
                 return
             
             # Case when NEITHER are basic units:    # TODO: this can be put into the above condition but thought separated was more readible.
             #   use the original quantity/unit (stash the parenthesis in the description)
             if not parenthesis_unit_is_basic and not unit_is_basic:
                 description = f"maybe quantity/unit is: {parenthesis_quantity}/{parenthesis_unit}"
-                self.parenthesis_notes.append(description)
-                # return [self.quantity, self.unit, description]
+                self._parenthesis_notes.append(description)
+                # return [self._quantity, self._unit, description]
                 
                 # set the secondary quantity/units to the values in the parenthesis
-                self.secondary_quantity = parenthesis_quantity
-                self.secondary_unit = parenthesis_unit
+                self._secondary_quantity = parenthesis_quantity
+                self._secondary_unit = parenthesis_unit
 
                 return
 
             # Case when: YES basic parenthesis unit, NO basic original unit: 
             #   then use the parenthesis quantity/unit (stash the original in the description)
             if parenthesis_unit_is_basic:
-                description = f"maybe quantity/unit is: {self.quantity}/{self.unit}"
-                self.parenthesis_notes.append(description)
+                description = f"maybe quantity/unit is: {self._quantity}/{self._unit}"
+                self._parenthesis_notes.append(description)
                 
                 # set the secondary quantity/units to the original quantity/units
-                self.secondary_quantity = self.quantity
-                self.secondary_unit = self.unit
+                self._secondary_quantity = self._quantity
+                self._secondary_unit = self._unit
 
                 # update the primary quantities/units to the parenthesis values
-                self.quantity = parenthesis_quantity
-                self.unit = parenthesis_unit
+                self._quantity = parenthesis_quantity
+                self._unit = parenthesis_unit
                 
                 # return [parenthesis_quantity, parenthesis_unit, description]
                 return
 
             # Case when: NO basic parenthesis unit, YES basic original unit: 
             #   then use the original quantity/unit (stash the parenthesis in the description)
             if unit_is_basic:
                 description = f"maybe quantity/unit is: {parenthesis_quantity}/{parenthesis_unit}"
-                self.parenthesis_notes.append(description)
+                self._parenthesis_notes.append(description)
 
                 # set the secondary quantity/units to the original quantity/units
-                self.secondary_quantity = parenthesis_quantity
-                self.secondary_unit = parenthesis_unit
+                self._secondary_quantity = parenthesis_quantity
+                self._secondary_unit = parenthesis_unit
 
                 return
 
         description = f"used quantity/units from parenthesis with equivalent quantity/units"
-        self.parenthesis_notes.append(description)
+        self._parenthesis_notes.append(description)
 
         # set the secondary quantity/units to the original quantity/units
-        self.secondary_quantity = self.quantity
-        self.secondary_unit = self.unit
+        self._secondary_quantity = self._quantity
+        self._secondary_unit = self._unit
 
-        self.quantity = parenthesis_quantity
-        self.unit = parenthesis_unit
+        self._quantity = parenthesis_quantity
+        self._unit = parenthesis_unit
 
         return
     
     def _address_quantity_unit_only_parenthesis(self, parenthesis: str) -> None:
         """
         Address the case where the parenthesis content contains exactly a quantity and unit (NOT prefixed by any equivalence strings like "about" or "approximately").
-        Attempts to update self.quantity, self.unit, self.secondary_quantity, and self.secondary_unit given 
-        information from the parenthesis string and the current self.quantity and self.unit
+        Attempts to update self._quantity, self._unit, self._secondary_quantity, and self._secondary_unit given 
+        information from the parenthesis string and the current self._quantity and self._unit
         e.g. "(3 ounces)", "(3 ounces each)", "(a 4 cup scoop)"
 
         Args:
             parenthesis (str): A string containing parenthesis from the ingredients string
         Returns:
             None
         """
 
-        # print(f"""Ingredient: '{self.reduced_ingredient}'\nParenthesis: '{parenthesis}'\nQuantity: '{self.quantity}'\nUnit: '{self.unit}'""") if self.debug else None
+        # print(f"""Ingredient: '{self._standardized_ingredient}'\nParenthesis: '{parenthesis}'\nQuantity: '{self._quantity}'\nUnit: '{self._unit}'""") if self.debug else None
 
         # Set a None Description
         description = None
 
         # pull out quantity unit only pattern
         quantity_unit_only = _utils._extract_quantity_unit_pairs(parenthesis)
         # quantity_unit_only = _regex_patterns.QUANTITY_UNIT_GROUPS.findall(parenthesis)
         # quantity_unit_only = [item for i in [_regex_patterns.QUANTITY_UNIT_GROUPS.findall(i) for i in parenthesis] for item in i]
 
         # if no numbers only parenthesis, then just return the original ingredient
         if not quantity_unit_only:
             # print(f"\n > Return early from QUANTITY UNIT parenthesis") if self.debug else None
             description = f"not a quantity unit only parenthesis"
-            self.parenthesis_notes.append(description)
-            # return [self.quantity, unit, description]
+            self._parenthesis_notes.append(description)
+            # return [self._quantity, unit, description]
             return
         
         # pull out the parenthesis quantity and unit
         parenthesis_quantity, parenthesis_unit = quantity_unit_only[0]
 
         # Case when: NO quantity, NO unit:
-            # if no quantity AND no unit, then we can use the parenthesis self.quantity-unit as our self.quantity and unit
-        if not self.quantity and not self.unit:
+            # if no quantity AND no unit, then we can use the parenthesis self._quantity-unit as our self._quantity and unit
+        if not self._quantity and not self._unit:
             # updated_quantity, updated_unit = quantity_unit_only[0]
             # print(f"\n > Case when: NO quantity, NO unit") if self.debug else None
 
             description = f"used quantity/unit from parenthesis with no quantity/unit"
-            self.parenthesis_notes.append(description)
+            self._parenthesis_notes.append(description)
 
             # set the secondary quantity/units to the original quantity/units
-            self.secondary_quantity = self.quantity
-            self.secondary_unit = self.unit
+            self._secondary_quantity = self._quantity
+            self._secondary_unit = self._unit
 
-            self.quantity = parenthesis_quantity
-            self.unit = parenthesis_unit
+            self._quantity = parenthesis_quantity
+            self._unit = parenthesis_unit
 
             # return [parenthesis_quantity, parenthesis_unit, description]
             return
 
         # Case when: YES quantity, NO unit:
             # if there is a quantity but no unit, we can try to merge (multiply) the current quantity and the parenthesis quantity 
             # then use the unit in the parenthesis
-        if self.quantity and not self.unit:
+        if self._quantity and not self._unit:
             # print(f"\n > Case when: YES quantity, NO unit") if self.debug else None
 
             # quantity_unit_only[0][0]
-            updated_quantity = str(float(self.quantity) * float(parenthesis_quantity))
+            updated_quantity = str(float(self._quantity) * float(parenthesis_quantity))
 
             description = f"multiplied starting quantity with parenthesis quantity"
-            self.parenthesis_notes.append(description)
+            self._parenthesis_notes.append(description)
 
             # set the secondary quantity/units to the original quantity/units
-            self.secondary_quantity = self.quantity
-            self.secondary_unit = self.unit
+            self._secondary_quantity = self._quantity
+            self._secondary_unit = self._unit
 
-            # self.quantity = updated_quantity
-            self.quantity = _utils._make_int_or_float_str(updated_quantity)
-            self.unit = parenthesis_unit
+            # self._quantity = updated_quantity
+            self._quantity = _utils._make_int_or_float_str(updated_quantity)
+            self._unit = parenthesis_unit
 
             # return [updated_quantity, parenthesis_unit, description]
             return
 
         # Case when: NO quantity, YES unit:
             # if there is no quantity BUT there IS a unit, then the parenthesis units/quantities are either:
             # 1. A description/note (i.e. cut 0.5 inch slices)
             # 2. A quantity and unit (i.e. 2 ounces)
             # either case, just return the parenthesis units to use those
-        if not self.quantity and self.unit:
+        if not self._quantity and self._unit:
             # print(f"\n > Case when: NO quantity, YES unit") if self.debug else None
 
-            description = f"No quantity but has units, used parenthesis. maybe quantity/unit is: {self.quantity}/{self.unit}"
-            self.parenthesis_notes.append(description)
+            description = f"No quantity but has units, used parenthesis. maybe quantity/unit is: {self._quantity}/{self._unit}"
+            self._parenthesis_notes.append(description)
 
             # set the secondary quantity/units to the original quantity/units
-            self.secondary_quantity = self.quantity
-            self.secondary_unit = self.unit
+            self._secondary_quantity = self._quantity
+            self._secondary_unit = self._unit
 
-            self.quantity = parenthesis_quantity
-            self.unit = parenthesis_unit
+            self._quantity = parenthesis_quantity
+            self._unit = parenthesis_unit
 
             # return [parenthesis_quantity, parenthesis_unit, description]
             return
 
         # Case when: YES quantity, YES unit:
             # if we already have a quantity AND a unit, then we likely just found a description 
             # OR we may have found an equivalence quantity unit.
             # we will choose to use the quantity/unit pairing that is has a unit in the BASIC_UNITS_SET
-        if self.quantity and self.unit:
+        if self._quantity and self._unit:
             # print(f"\n > Case when: YES quantity, YES unit") if self.debug else None
 
             # flags for if original unit/parenthesis unit are in the set of basic units (BASIC_UNITS_SET) or not
             parenthesis_unit_is_basic = parenthesis_unit in _constants.BASIC_UNITS_SET
-            unit_is_basic = self.unit in _constants.BASIC_UNITS_SET
+            unit_is_basic = self._unit in _constants.BASIC_UNITS_SET
 
             # Case when BOTH are basic units: 
             #   use the original quantity/unit (stash the parenthesis in the description)
             if parenthesis_unit_is_basic and unit_is_basic:
                 # print(f"\n >>> Case when: BASIC parenthesis unit, BASIC unit") if self.debug else None
 
                 description = f"maybe quantity/unit is: {parenthesis_quantity}/{parenthesis_unit}"
-                self.parenthesis_notes.append(description)
+                self._parenthesis_notes.append(description)
 
                 # set the secondary quantity/units to the parenthesis quantity/units
-                self.secondary_quantity = parenthesis_quantity
-                self.secondary_unit = parenthesis_unit
+                self._secondary_quantity = parenthesis_quantity
+                self._secondary_unit = parenthesis_unit
                 return
             
             # Case when NEITHER are basic units:    # TODO: this can be put into the above condition but thought separated was more readible.
             #   use the original quantity/unit AND set the secondary quantity/units to the PARENTHESIS values 
             #   (stash the parenthesis in the description)
             if not parenthesis_unit_is_basic and not unit_is_basic:
                 # print(f"\n >>> Case when: NOT BASIC parenthesis unit, NOT BASIC unit") if self.debug else None
                 description = f"maybe quantity/unit is: {parenthesis_quantity}/{parenthesis_unit}"
-                self.parenthesis_notes.append(description)
+                self._parenthesis_notes.append(description)
 
                 # set the secondary quantity/units to the parenthesis quantity/units
-                self.secondary_quantity = parenthesis_quantity
-                self.secondary_unit = parenthesis_unit
+                self._secondary_quantity = parenthesis_quantity
+                self._secondary_unit = parenthesis_unit
                 return
 
             # Case when: YES basic parenthesis unit, NO basic original unit (EXPLICIT):
             #  Try to merge (multiply) the current quantity and the parenthesis quantity
             #  AND set the secondary quantity/units to the ORIGINAL values
             if parenthesis_unit_is_basic and not unit_is_basic:
                 # print(f"\n >>> Case when: BASIC parenthesis unit, NOT BASIC unit (EXPLICIT)") if self.debug else None
-                updated_quantity = str(float(self.quantity) * float(parenthesis_quantity))
+                updated_quantity = str(float(self._quantity) * float(parenthesis_quantity))
 
                 description = f"multiplied starting quantity with parenthesis quantity"
-                self.parenthesis_notes.append(description)
+                self._parenthesis_notes.append(description)
 
                 # set the secondary quantity/units to the original quantity/units
-                self.secondary_quantity = self.quantity
-                self.secondary_unit = self.unit
+                self._secondary_quantity = self._quantity
+                self._secondary_unit = self._unit
 
-                # self.quantity = updated_quantity
-                self.quantity = _utils._make_int_or_float_str(updated_quantity)
-                self.unit = parenthesis_unit
+                # self._quantity = updated_quantity
+                self._quantity = _utils._make_int_or_float_str(updated_quantity)
+                self._unit = parenthesis_unit
 
                 return
 
             # TODO: I think this condition can be dropped, gets covered by previous condition...
             # Case when: YES basic parenthesis unit, NO basic original unit (IMPLICITLY): 
             #   then use the parenthesis quantity/unit AND set the secondary quantity/units to the ORIGINAL values
             #   (stash the original in the description)
             if parenthesis_unit_is_basic:
                 # print(f"\n >>> Case when: BASIC parenthesis unit, NOT BASIC unit (IMPLICIT)") if self.debug else None
-                description = f"maybe quantity/unit is: {self.quantity}/{self.unit}"
-                self.parenthesis_notes.append(description)
+                description = f"maybe quantity/unit is: {self._quantity}/{self._unit}"
+                self._parenthesis_notes.append(description)
 
                 # set the secondary quantity/units to the original quantity/units
-                self.secondary_quantity = self.quantity
-                self.secondary_unit = self.unit
+                self._secondary_quantity = self._quantity
+                self._secondary_unit = self._unit
 
-                self.quantity = parenthesis_quantity
-                self.unit = parenthesis_unit
+                self._quantity = parenthesis_quantity
+                self._unit = parenthesis_unit
 
                 return
 
             # Case when: NO basic parenthesis unit, YES basic original unit: 
             #   then just keep the original quantity/unit AND set the secondary quantity/units to the PARENTHESIS values
             #   (stash the original in the description)
             if unit_is_basic:
                 # print(f"\n >>> Case when: NOT BASIC parenthesis unit, BASIC unit (IMPLICIT)") if self.debug else None
-                description = f"maybe quantity/unit is: {self.quantity}/{self.unit}"
-                self.parenthesis_notes.append(description)
+                description = f"maybe quantity/unit is: {self._quantity}/{self._unit}"
+                self._parenthesis_notes.append(description)
 
                 # set the secondary quantity/units to the parenthesis quantity/units
-                self.secondary_quantity = parenthesis_quantity
-                self.secondary_unit = parenthesis_unit
+                self._secondary_quantity = parenthesis_quantity
+                self._secondary_unit = parenthesis_unit
 
                 return
         
-        print(f"\n ----> Case when: ALL OTHER CASES FAILED") if self.debug else None
+        # print(f"\n ----> Case when: ALL OTHER CASES FAILED") if self.debug else None
 
         # TODO: Don't think this should ever happen, need to rethink this part
         # Case when: All other conditions were NOT met:
             # just set the quantity/unit to the parenthesis values 
             # and then put the original quantity/units in the secondary quantity/units
         description = f"used quantity/units from parenthesis with quantity/units only"
-        self.parenthesis_notes.append(description)
+        self._parenthesis_notes.append(description)
 
         # set the secondary quantity/units to the ORIGINAL quantity/units
-        self.secondary_quantity = self.quantity 
-        self.secondary_unit = self.unit
+        self._secondary_quantity = self._quantity 
+        self._secondary_unit = self._unit
 
         # set the primary quantity/units to the parenthesis quantity/units
-        self.quantity = parenthesis_quantity
-        self.unit = parenthesis_unit
+        self._quantity = parenthesis_quantity
+        self._unit = parenthesis_unit
 
         return
     
     def _add_standard_units(self) -> None:
         """
         Add standard units to the parsed ingredient if they are present in the
         constants units to standard units map.
         If the "unit"/"secondary_unit" exists and it is present in the unit to standard unit map, 
         then get the standard unit name for the unit and set the "standardized_unit" and "standardized_secondary_unit" member variables.
         """
 
-        if self.unit and self.unit in _constants.UNIT_TO_STANDARD_UNIT:
-            self.standardized_unit = _constants.UNIT_TO_STANDARD_UNIT[self.unit]
+        if self._unit and self._unit in _constants.UNIT_TO_STANDARD_UNIT:
+            self._standardized_unit = _constants.UNIT_TO_STANDARD_UNIT[self._unit]
         
-        if self.secondary_unit and self.secondary_unit in _constants.UNIT_TO_STANDARD_UNIT:
-            self.standardized_secondary_unit = _constants.UNIT_TO_STANDARD_UNIT[self.secondary_unit]
+        if self._secondary_unit and self._secondary_unit in _constants.UNIT_TO_STANDARD_UNIT:
+            self._standardized_secondary_unit = _constants.UNIT_TO_STANDARD_UNIT[self._secondary_unit]
 
         return 
 
     def _prioritize_weight_units(self) -> None:
         """
         Prioritize weight units over volume units if both are present in the parsed ingredient.
         If the first unit is not a weight unit but the secondary_unit is a weight unit, then swap them so 
         the weight unit is always given as the primary unit.
         (i.e. unit = "cups", secondary_unit = "ounces" --> Swap them so that unit = "ounces" and secondary_unit = "cups")
         """
 
         # # if the first unit is already a weight, just return early
-        if self.unit in _constants.WEIGHT_UNITS_SET:
+        if self._unit in _constants.WEIGHT_UNITS_SET:
             return 
         
         # TODO: first part of this if statement is probably redundent...
         # if the first unit is NOT a weight and the second unit IS a weight, then swap them
-        if self.unit not in _constants.WEIGHT_UNITS_SET and self.secondary_unit in _constants.WEIGHT_UNITS_SET:
+        if self._unit not in _constants.WEIGHT_UNITS_SET and self._secondary_unit in _constants.WEIGHT_UNITS_SET:
 
-            print(f"Swapping first quantity/units with second quantity/units") if self.debug else None
+            # print(f"Swapping first quantity/units with second quantity/units") if self.debug else None
             # print(f"Swapping first quantity/units with second quantity/units") if self.debug else None
 
             # switch the units and quantities with the secondary units and quantities
-            self.quantity, self.secondary_quantity = self.secondary_quantity, self.quantity
-            self.unit, self.secondary_unit = self.secondary_unit,  self.unit
-            self.standardized_unit, self.standardized_secondary_unit = self.standardized_secondary_unit, self.standardized_unit
+            self._quantity, self._secondary_quantity = self._secondary_quantity, self._quantity
+            self._unit, self._secondary_unit = self._secondary_unit,  self._unit
+            self._standardized_unit, self._standardized_secondary_unit = self._standardized_secondary_unit, self._standardized_unit
 
         return 
     
     def _find_and_remove(self, string: str, pattern: re.Pattern) -> str:
         """Find and remove all matches of a pattern from a string.
         Args:
             string (str): The string to search for matches in
@@ -1664,15 +1517,15 @@
             # Get the start and end of the match and the modified start and end positions given the offset
             start, end = match.start(), match.end()
             modified_start = start + offset
             modified_end = end + offset
 
             # Construct the modified string with the replacement applied
             string = string[:modified_start] + str(replacement_str) + string[modified_end:]
-            # self.standardized_ingredient = self.standardized_ingredient[:modified_start] + str(replacement_str) + self.standardized_ingredient[modified_end:]
+            # self._standardized_ingredient = self._standardized_ingredient[:modified_start] + str(replacement_str) + self._standardized_ingredient[modified_end:]
 
             # Update the offset for subsequent removals # TODO: this is always 0 because we're removing the match, probably just remove...
             offset += len(str(replacement_str)) - (end - start)
             # print(f"""
             # Match string: {match_string}
             # -> Match: {match_string} at positions {start}-{end}
             # --> Modified start/end match positions: {modified_start}-{modified_end}
@@ -1681,15 +1534,15 @@
         return string
     
     def _extract_foods(self, ingredient: str) -> str:
         """Does a best effort attempt to extract foods from the ingredient by 
         removing all extraneous details, words, characters and hope we get left with the food.
         """
 
-        print(f"Best effort extraction of food words from: {ingredient}") if self.debug else None
+        # print(f"Best effort extraction of food words from: {ingredient}") if self.debug else None
 
         # Apply _utils._remove_parenthesis_from_str() to remove parenthesis content
         ingredient = _utils._remove_parenthesis_from_str(ingredient)
 
         # regular expressions to find and remove from the ingredient
         # NOTE: important to remove "parenthesis" first and "stop words" last to.
         # Parenthesis can contain other patterns and they need to be dealt with first (i.e. "(about 8 oz)" contains a number and a unit)
@@ -1704,26 +1557,24 @@
             "approximate strings" : _regex_patterns.APPROXIMATE_STRINGS_PATTERN,
             "size modifiers" : _regex_patterns.SIZE_MODIFIERS_PATTERN,
             "casual quantities" : _regex_patterns.CASUAL_QUANTITIES_PATTERN,
             "stop words" : _regex_patterns.STOP_WORDS_PATTERN
         }
 
         for key, pattern in patterns_map.items():
-            print(f" > Removing '{key}' from the ingredient\n") if self.debug else None
-
-            print(f"Starting ingredient:\n > '{ingredient}'") if self.debug else None
+            # print(f" > Removing '{key}' from the ingredient\n") if self.debug else None
+            # print(f"Starting ingredient:\n > '{ingredient}'") if self.debug else None
             # ingredient = self._find_and_remove(ingredient, pattern)
             ingredient = _utils._find_and_remove(ingredient, pattern)
-            print(f"Ending ingredient:\n > '{ingredient}'") if self.debug else None
-
-        print(f" > Removing any remaining special characters") if self.debug else None
+            # print(f"Ending ingredient:\n > '{ingredient}'") if self.debug else None
+        # print(f" > Removing any remaining special characters") if self.debug else None
         
         ingredient = re.sub(r'[^\w\s]', '', ingredient) # remove any special characters
 
-        print(f" > Removing any extra whitespaces") if self.debug else None
+        # print(f" > Removing any extra whitespaces") if self.debug else None
 
         ingredient = re.sub(r'\s+', ' ', ingredient).strip() # remove any extra whitespace
 
         return ingredient
     
     def _extract_prep_words(self, ingredient: str) -> str:
         """Get prep words from the ingredient (including words ending in 'ly')"""
@@ -1745,107 +1596,100 @@
         size_modifiers.sort()
 
         return size_modifiers
 
     # def _extract_dimension_units(self, ingredient: str) -> str:
     #     """Add sometimes units to the units variables if they are the only possible units after the ingredient has been parsed."""
     #     # ingredient = "2 1/2 cups of sugar (about 1/2 inch squares of sugar)"
-
     #     dimension_units = _regex_patterns.QUANTITY_DIMENSION_UNIT_GROUPS.findall(ingredient)
-    #     dimension_units.sort()
-
     #     return dimension_units
+    
+    def _add_gram_weights(self):
+        """Add gram weights to the units variables if they are the only possible units after the ingredient has been parsed."""
+        # ingredient = "2 1/2 cups of sugar (about 1/2 inch squares of sugar)"
+        grams_map = _utils._get_gram_weight(self._food, self._quantity, self._unit, "levenshtein")
+
+        if grams_map:
+            self._gram_weight      = grams_map.get("gram_weight", None)
+            self._min_gram_weight = grams_map.get("min_gram_weight", None)
+            self._max_gram_weight = grams_map.get("max_gram_weight", None)
+
+        return
 
     def _address_parenthesis(self) -> None:
         """
         Address any parenthesis that were in the ingredient.
         """
-
-        # print(f"Addressing parenthesis: '{self.parenthesis_content}'") if self.debug else None
+        # print(f"Addressing parenthesis: '{self._parenthesis_content}'") if self.debug else None
 
         # loop through each of the parenthesis in the parenthesis content and apply address_parenthesis functions 
-        for parenthesis in self.parenthesis_content:
-            print(f"Addressing parenthesis: '{parenthesis}'") if self.debug else None
+        for parenthesis in self._parenthesis_content:
+            # print(f"Addressing parenthesis: '{parenthesis}'") if self.debug else None
 
             # address the case where the parenthesis content only contains a quantity
-            print(f"> Apply QUANTITY Parenthesis to: '{self.quantity} {self.unit}'") if self.debug else None
+            # print(f"> Apply QUANTITY Parenthesis to: '{self._quantity} {self._unit}'") if self.debug else None
             self._address_quantity_only_parenthesis(parenthesis)
             
-            print(f"> Apply EQUIVALENCE Parenthesis to: '{self.quantity} {self.unit}'") if self.debug else None
+            # print(f"> Apply EQUIVALENCE Parenthesis to: '{self._quantity} {self._unit}'") if self.debug else None
             self._address_equivalence_parenthesis(parenthesis)
 
-            print(f"> Apply QUANTITY UNIT Parenthesis to: '{self.quantity} {self.unit}'") if self.debug else None
+            # print(f"> Apply QUANTITY UNIT Parenthesis to: '{self._quantity} {self._unit}'") if self.debug else None
             self._address_quantity_unit_only_parenthesis(parenthesis)
 
         return
 
-    def parse(self):
+    def _parse(self):
         # TODO: process parenthesis content
 
         print(f"Standardizing ingredient: \n > '{self.ingredient}'") if self.debug else None
         # print(f"Standardizing ingredient: \n > '{self.ingredient}'")
 
         # ----------------------------------- STEP 1 ------------------------------------------
         # ---- Get the input ingredient string into a standardized form ----
         # -------------------------------------------------------------------------------------
 
-        # run the standardization method to cleanup raw ingredient and create the "standard_ingredient" and "reduced_ingredient" member variables 
-        self.standardize()
+        # run the standardization method to cleanup raw ingredient and create the "standard_ingredient" and "_reduced_ingredient" member variables 
+        self._standardize()
 
-        print(f"Standardized ingredient: \n > '{self.standardized_ingredient}'") if self.debug else None
-        print(f"Reduced ingredient: \n > '{self.reduced_ingredient}'") if self.debug else None
-        print(f"Extracting first quantity and unit from reduced ingredient: \n > '{self.reduced_ingredient}'") if self.debug else None
+        print(f"Standardized ingredient: \n > '{self._standardized_ingredient}'") if self.debug else None
+        # print(f"Reduced ingredient: \n > '{self._reduced_ingredient}'") if self.debug else None
+        # print(f"Extracting first quantity and unit from reduced ingredient: \n > '{self._reduced_ingredient}'") if self.debug else None
         # ----------------------------------- STEP 2 ------------------------------------------
         # ---- Check if there is any indication of the ingredient being required/optional ----
         # -------------------------------------------------------------------------------------
 
         # run the is_required method to check if the ingredient is required or optional and set the "is_required" member variable to the result
-        self.is_required = self._is_required()
+        self._is_required = self._is_ingredient_required()
 
-        print(f"Is the ingredient required? {self.is_required}") if self.debug else None
+        print(f"Is the ingredient required? {self._is_required}") if self.debug else None
 
         # ----------------------------------- STEP 3 ------------------------------------------
-        # ---- Extract first options of quantities and units from the "reduced_ingredient" ----
+        # ---- Extract first options of quantities and units from the "_reduced_ingredient" ----
         # -------------------------------------------------------------------------------------
-
-        #  reduced_ingredient ---> (i.e. standardized ingredient with parenthesis content removed)
+        print(f"Attempting to extract quantity and unit") if self.debug else None
+        #  _reduced_ingredient ---> (i.e. standardized ingredient with parenthesis content removed)
         # run the extract_first_quantity_unit method to extract the first unit and quantity from the ingredient string
         self.extract_first_quantity_unit()
 
         # ----------------------------------- STEP 4 ------------------------------------------
         # ---- Address any parenthesis that were in the ingredient  ----
         # -------------------------------------------------------------------------------------
         # NOTE: Stash the best_quantity and best_units before preceeding (for debugging)
 
-        print(f"""Status of ingredients before parenthesis handling: {self.ingredient}
-            Ingredient: > '{self.ingredient}'
-                > Standard ingredient: '{self.standardized_ingredient}'
-                > Parenthesis content: '{self.parenthesis_content}'
+        print(f"""Addressing parenthesis: 
+                > Standard ingredient: '{self._standardized_ingredient}'
+                > Parenthesis content: '{self._parenthesis_content}'
             """) if self.debug else None
-        
-        # # loop through each of the parenthesis in the parenthesis content and apply address_parenthesis functions 
-        # for parenthesis in self.parenthesis_content:
-        #     print(f"Addressing parenthesis: '{parenthesis}'") if self.debug else None
-
-        #     # address the case where the parenthesis content only contains a quantity
-        #     print(f"> Apply QUANTITY Parenthesis to: '{self.quantity} {self.unit}'") if self.debug else None
-        #     self._address_quantity_only_parenthesis(parenthesis)
-            
-        #     print(f"> Apply EQUIVALENCE Parenthesis to: '{self.quantity} {self.unit}'") if self.debug else None
-        #     self._address_equivalence_parenthesis(parenthesis)
-
-        #     print(f"> Apply QUANTITY UNIT Parenthesis to: '{self.quantity} {self.unit}'") if self.debug else None
-        #     self._address_quantity_unit_only_parenthesis(parenthesis)
 
         self._address_parenthesis()
 
         # ----------------------------------- STEP 5 ------------------------------------------
         # ---- Get the standard names of the units and secondary units ----
         # -------------------------------------------------------------------------------------
-        print(f"Adding standard unit names for {self.unit} and {self.secondary_unit}") if self.debug else None
+        print(f"Adding standard unit names for {self._unit} and {self._secondary_unit}") if self.debug else None
 
         self._add_standard_units()
 
         # ----------------------------------- STEP 6 ------------------------------------------
         # ---- Prioritize weight units and always place the weight unit as the primary ingredient if it exists ----
         # -------------------------------------------------------------------------------------
         print(f"Prioritizing weight units") if self.debug else None
@@ -1860,59 +1704,216 @@
         # > quantities
         # > prep words
         # > "ly"-words
         # -------------------------------------------------------------------------------------
         print(f"Extracting food words") if self.debug else None
         # print(f"Extracting food words (version {self.extract_version})") if self.debug else None
         
-        self.food = self._extract_foods(self.standardized_ingredient)
+        self._food = self._extract_foods(self._standardized_ingredient)
 
         # ----------------------------------- STEP 8 ------------------------------------------
         # ---- Extract extra, descriptors (prep words, size modifiers, dimension units) ----
         # -------------------------------------------------------------------------------------
         print(f"Extracting prep words, size modifiers") if self.debug else None
         # print(f"Extracting food words (version {self.extract_version})") if self.debug else None
-        self.prep = self._extract_prep_words(self.staged_ingredient) # TODO: testing using staged_ingredient
-        self.size_modifiers = self._extract_size_modifiers(self.staged_ingredient) # TODO: testing using staged_ingredient
+        self._prep = self._extract_prep_words(self._staged_ingredient) # TODO: testing using staged_ingredient
+        self._size_modifiers = self._extract_size_modifiers(self._staged_ingredient) # TODO: testing using staged_ingredient
+        # self._prep = self._extract_prep_words(self._standardized_ingredient) 
+        # self._size_modifiers = self._extract_size_modifiers(self._standardized_ingredient)
+
+        # ----------------------------------- STEP 9 ------------------------------------------
+        # ---- Calculate gram weights if possible ----
+        # -------------------------------------------------------------------------------------
+        print(f"Calculating gram weights") if self.debug else None
+        self._add_gram_weights() # TODO: testing using staged_ingredient
+
 
-        # self.prep = self._extract_prep_words(self.standardized_ingredient) 
-        # self.size_modifiers = self._extract_size_modifiers(self.standardized_ingredient)
+    def standardized_ingredient(self) -> str:
+        """
+        Return the standardized ingredient string.
+        Returns:
+            str: The standardized ingredient string.
+        """
+        return self._standardized_ingredient
 
+    def food(self) -> str:
+        """
+        Return the food string.
+        Returns:
+            str: The food string.
+        """
+        return self._food
+    
+    def quantity(self) -> str:
+        """
+        Return the quantity string.
+        Returns:
+            str: The quantity string.
+        """
+        return self._quantity
+    
+    def unit(self) -> str:
+        """
+        Return the unit string.
+        Returns:
+            str: The unit string.
+        """
+        return self._unit
+    
+    def standardized_unit(self) -> str:
+        """
+        Return the standardized unit string.
+        Returns:
+            str: The standardized unit string.
+        """
+        return self._standardized_unit
+    
+    def secondary_quantity(self) -> str:
+        """
+        Return the secondary quantity string.
+        Returns:
+            str: The secondary quantity string.
+        """
+        return self._secondary_quantity
+    
+    def secondary_unit(self) -> str:
+        """
+        Return the secondary unit string.
+        Returns:
+            str: The secondary unit string.
+        """
+        return self._secondary_unit
+    
+    def standardized_secondary_unit(self) -> str:
+        """
+        Return the standardized secondary unit string.
+        Returns:
+            str: The standardized secondary unit string.
+        """
+        return self._standardized_secondary_unit
+    
+    def gram_weight(self) -> str:
+        """
+        Return the estimated gram weight of the given ingredient.
+        Returns:
+            str: The estimated gram weight of the given ingredient.
+        """
+        return self._gram_weight
+    
+    def min_gram_weight(self) -> str:
+        """
+        Return the estimated minimum gram weight of the given ingredient.
+        Returns:
+            str: The estimated minimum gram weight of the given ingredient.
+        """
+        return self._min_gram_weight
+    
+    def max_gram_weight(self) -> str:
+        """
+        Return the estimated maximum gram weight of the given ingredient.
+        Returns:
+            str: The estimated maximum gram weight of the given ingredient.
+        """
+        return self._max_gram_weight
+    
+    def prep(self) -> list:
+        """
+        Return the prep list.
+        Returns:
+            list: The prep list.
+        """
+        return self._prep
+    
+    def size_modifiers(self) -> list:
+        """
+        Return the size modifiers list.
+        Returns:
+            list: The size modifiers list.
+        """
+        return self._size_modifiers
+    
+    def dimensions(self) -> list:
+        """
+        Return the dimensions list.
+        Returns:
+            list: The dimensions list.
+        """
+        return self._dimensions
+    
+    def is_required(self) -> bool:
+        """
+        Check if the ingredient is required or optional.
+        Returns:
+            bool: True if the ingredient is required, False if the ingredient is optional.
+        """
 
+        return self._is_required
+    
+    def parsed_ingredient(self) -> dict:
+        """
+        Return the parsed ingredient dictionary.
+        Returns:
+            dict: The parsed ingredient dictionary (duplicate to to_json()) method
+        """
 
+        return self._parsed_ingredient
+    
     def to_json(self) -> dict:
         """
         Convert the IngredientSlicer object to a dictionary.
         Returns:
             dict: A dictionary containing the IngredientSlicer object's member variables.
         """
         return {
-            "ingredient": self.ingredient,                                # "2 1/2 large cups of sugar lightly packed (about 40 tbsp of sugar)"
-            "standardized_ingredient": self.standardized_ingredient,          # "2.5 cups of sugar"
+            # "ingredient": self.ingredient,                                # "2 1/2 large cups of sugar lightly packed (about 40 tbsp of sugar)"
+            "standardized_ingredient": self._standardized_ingredient,          # "2.5 cups of sugar"
         
-            "food" : self.food,                                           # "sugar"
+            "food" : self._food,                                           # "sugar"
+
+            "quantity": self._quantity,                                    # "2.5"
+            "unit": self._unit,                                            # "cups"
+            "standardized_unit": self._standardized_unit,                      # "cup"
+
+            "secondary_quantity": self._secondary_quantity,                # "40"
+            "secondary_unit": self._secondary_unit,                        # "tbsp"
+            "standardized_secondary_unit": self._standardized_secondary_unit,  # "tablespoon"
 
-            "quantity": self.quantity,                                    # "2.5"
-            "unit": self.unit,                                            # "cups"
-            "standardized_unit": self.standardized_unit,                      # "cup"
-
-            "secondary_quantity": self.secondary_quantity,                # "40"
-            "secondary_unit": self.secondary_unit,                        # "tbsp"
-            "standardized_secondary_unit": self.standardized_secondary_unit,  # "tablespoon"
-
-            "prep": self.prep,                                            # ["lightly", "packed"]
-            "size_modifiers": self.size_modifiers,                        # ["large"]
-            "dimensions": self.dimensions,                                # ["2 inches"]
-            "is_required": self.is_required,                              # True
+            "gram_weight": self._gram_weight,                              # "113.4 grams
+
+            "prep": self._prep,                                            # ["lightly", "packed"]
+            "size_modifiers": self._size_modifiers,                        # ["large"]
+            "dimensions": self._dimensions,                                # ["2 inches"]
+            "is_required": self._is_required,                              # True
 
             # NOTE: drop these at some point
-            "parenthesis_content": self.parenthesis_content               # ["(about 40 tbsp of sugar)"]
-            # "parenthesis_notes": self.parenthesis_notes,
-            # "reduced_ingredient": self.reduced_ingredient, 
+            "parenthesis_content": self._parenthesis_content               # ["(about 40 tbsp of sugar)"]
+            # "parenthesis_notes": self._parenthesis_notes,
         }
+    
+    def __str__(self) -> str:
+        """
+        Return a string representation of the IngredientSlicer object.
+        Returns:
+            str: A string representation of the IngredientSlicer object.
+        """
+        return f"""IngredientSlicer Object:
+    \tStandardized Ingredient: '{self._standardized_ingredient}'
+    \tFood: '{self._food}'
+    \tQuantity: '{self._quantity}'
+    \tUnit: '{self._unit}'
+    \tStandardized Unit: '{self._standardized_unit}'
+    \tSecondary Quantity: '{self._secondary_quantity}'
+    \tSecondary Unit: '{self._secondary_unit}'
+    \tStandardized Secondary Unit: '{self._standardized_secondary_unit}'
+    \tGram Weight: '{self._gram_weight}'
+    \tPrep: '{self._prep}'
+    \tSize Modifiers: '{self._size_modifiers}'
+    \tDimensions: '{self._dimensions}'
+    \tIs Required: '{self._is_required}'
+    \tParenthesis Content: '{self._parenthesis_content}'"""
 
 
 # # ####### Deprecated ####### 
 # def _merge_multi_nums2(self) -> None:
 #     """
 #     Replace unicode and standard fractions with their decimal equivalents in the parsed ingredient.
 #     Assumes that numeric values in string have been padded with a space between numbers and non numeric characters and
@@ -1926,18 +1927,18 @@
 #     '2.5 cups of sugar'
 #     >>> _merge_multi_nums('1 0.5 pounds skinless, boneless chicken breasts, cut into 0.5 inch pieces')
 #     '1.5 pounds skinless, boneless chicken breasts, cut into 0.5 inch pieces'
 #     """
     
 #     # get the units from the ingredient string
 #     # units = re.findall(regex_map.UNITS_PATTERN, ingredient)
-#     units = re.findall(_regex_patterns.UNITS_PATTERN, self.standardized_ingredient)
+#     units = re.findall(_regex_patterns.UNITS_PATTERN, self._standardized_ingredient)
 
 #     # spaced_nums = re.findall(regex.SPACE_SEP_NUMBERS, '2 0.5 cups of sugar 3 0.5 lbs of carrots')
-#     spaced_nums = re.findall(_regex_patterns.SPACE_SEP_NUMBERS, self.standardized_ingredient)
+#     spaced_nums = re.findall(_regex_patterns.SPACE_SEP_NUMBERS, self._standardized_ingredient)
 
 #     # Merge the numbers from the space seperated string of numbers
 #     merged_values = [self._merge_spaced_numbers(num_pair) for num_pair in spaced_nums]
 
 #     # Was the operation to merge the numbers an addition or a multiplication?
 #     merge_type = [self._which_merge_on_spaced_numbers(num_pair) for num_pair in spaced_nums]
 
@@ -1957,24 +1958,24 @@
 #     if len(spaced_nums) != len(conversions_map):
 #         warnings.warn(f"Number of spaced numbers and number of converted matches (MAP) are not equal...")
 
 #     if len(spaced_nums) != len(conversions_list):    
 #         warnings.warn(f"Number of spaced numbers and number of converted matches (LIST) are not equal...")
     
 #     # Create iterable of the matched spaced numbers to insert updated values into the original string
-#     spaced_matches = re.finditer(_regex_patterns.SPACE_SEP_NUMBERS, self.standardized_ingredient)
+#     spaced_matches = re.finditer(_regex_patterns.SPACE_SEP_NUMBERS, self._standardized_ingredient)
 
 #     # initialize offset and replacement index values for updating the ingredient string, 
 #     # these will be used to keep track of the position of the match in the string
 #     offset = 0
 #     replacement_index = 0
 
 #     # Update the ingredient string with the merged values
 #     for match in spaced_matches:
-#         # print(f"Ingredient string: {self.standardized_ingredient}")
+#         # print(f"Ingredient string: {self._standardized_ingredient}")
 
 #         # Get the start and end positions of the match
 #         start, end = match.start(), match.end()
 
 #         # print(f"Match: {match.group()} at positions {start}-{end}")
 
 #         # Get key value pair in the conversions_map that corresponds to the current match and the new quantity values to sub in
@@ -1994,38 +1995,38 @@
 #         modified_start = start + offset
 #         modified_end = end + offset
 
 #         # print(f" -> Modified match positions: {modified_start}-{modified_end}")
 #         # print(f"Replacing {match.group()} with '{merged_quantity}'...")
         
 #         # Construct the modified string with the replacement applied
-#         self.standardized_ingredient = self.standardized_ingredient[:modified_start] + str(merged_quantity) + self.standardized_ingredient[modified_end:]
+#         self._standardized_ingredient = self._standardized_ingredient[:modified_start] + str(merged_quantity) + self._standardized_ingredient[modified_end:]
 #         # ingredient = ingredient[:modified_start] + str(merged_quantity) + ingredient[modified_end:]
 
 #         # Update the offset for subsequent replacements
 #         offset += len(merged_quantity) - (end - start)
 #         replacement_index += 1
-#         # print(f" --> Output ingredient: \n > '{self.standardized_ingredient}'")
+#         # print(f" --> Output ingredient: \n > '{self._standardized_ingredient}'")
 
 # ####### Deprecated ####### 
 # def _parse_fractions(self):
 #     """
 #     Replace unicode and standard fractions with their decimal equivalents in the parsed ingredient.
 #     """
 #     # print("Parsing fractions")
 #     # regex.MULTI_PART_FRACTIONS_PATTERN
-#     # fractions = re.findall(regex.MULTI_PART_FRACTIONS_PATTERN, self.standardized_ingredient)
-#     # fractions = re.findall(regex.MULTI_PART_FRACTIONS_PATTERN_AND, self.standardized_ingredient)
+#     # fractions = re.findall(regex.MULTI_PART_FRACTIONS_PATTERN, self._standardized_ingredient)
+#     # fractions = re.findall(regex.MULTI_PART_FRACTIONS_PATTERN_AND, self._standardized_ingredient)
 
 #     # finditer() method
-#     fractions = re.finditer(_regex_patterns.MULTI_PART_FRACTIONS_PATTERN, self.standardized_ingredient)
-#     # fractions = re.finditer(regex.MULTI_PART_FRACTIONS_PATTERN_AND, self.standardized_ingredient)
+#     fractions = re.finditer(_regex_patterns.MULTI_PART_FRACTIONS_PATTERN, self._standardized_ingredient)
+#     # fractions = re.finditer(regex.MULTI_PART_FRACTIONS_PATTERN_AND, self._standardized_ingredient)
 
 #     # Replace fractions in the original string with their sum based on match indices
-#     # updated_ingredient = self.standardized_ingredient
+#     # updated_ingredient = self._standardized_ingredient
 #     offset = 0
 
 #     for match in fractions:
 
 #         # keep track of the offset to adjust the index of the match
 #         start_index = match.start() + offset
 #         end_index = match.end() + offset
@@ -2044,15 +2045,15 @@
 
 #         # Replace the matched fraction with the sum of the parse    d fraction
 #         sum_fraction = self._sum_parsed_fractions(parsed_fraction)
 
 #         print(f"Sum Fraction: {sum_fraction}")
 #         # Insert the sum of the fraction into the updated ingredient string
 #         # updated_ingredient = updated_ingredient[:start_index] + str(sum_fraction) + updated_ingredient[end_index:]
-#         self.standardized_ingredient = self.standardized_ingredient[:start_index] + " " + str(sum_fraction) + self.standardized_ingredient[end_index:]
+#         self._standardized_ingredient = self._standardized_ingredient[:start_index] + " " + str(sum_fraction) + self._standardized_ingredient[end_index:]
 
 #         # Update the offset to account for the difference in length between the matched fraction and the sum of the fraction
 #         offset += len(str(sum_fraction)) - len(matched_fraction)
 
 # ####### Deprecated ####### 
 # def _parse_mixed_fraction(self, fraction_str: str) -> list:
 #     # Remove whitespace to the left and right of a slash
```

### Comparing `ingredient_slicer-0.0.81/ingredient_slicer/_regex_patterns.py` & `ingredient_slicer-0.0.83/ingredient_slicer/_regex_patterns.py`

 * *Files 6% similar despite different names*

```diff
@@ -305,21 +305,80 @@
 # - match whole numbers and fractions
 # - match a number followed by a space and then a word and then a number or a fraction
 # -----------------------------------------------------------------------------
 
 # Regex pattern for fraction parts, finds all the fraction parts in a string (e.g. 1/2, 1/4, 3/4). 
 # A number followed by 0+ white space characters followed by a number then a forward slash then another number.
 # FRACTION_PATTERN = re.compile(r'\d*\s*/\s*\d+')
-FRACTION_PATTERN = re.compile(r'\d+\s*/\s*\d+') # TODO: Testing new fraction pattern, old pattern would match even if there was NOT a number in front of the forward slash...
+
+# NOTE: THIS is the working one
+FRACTION_PATTERN = re.compile(r'\d+\s*/\s*\d+') # TODO: Current good to go basic fraction matter, below are some alternatives, not sure how safe they are though....
+# FRACTION_PATTERN = re.compile(r'(?:\d*\.\d+|\d+\s*/\s*\d+|\d+)?\s*/\s*(?:\d*\.\d+|\d+\s*/\s*\d+|\d+)?', re.IGNORECASE) # TODO: runner up, not sure if its completly safe though....
+# FRACTION_PATTERN = re.compile(r'\b(?:\d*\.\d+|\d+\s*/\s*\d+|\d+)\s*/\s*(?:\d*\.\d+|\d+\s*/\s*\d+|\d+)\b', re.IGNORECASE) # TODO: Version 3 test
 
 # Regex for capturing and splitting whitespace seperated numbers/decimals/fractions 
 # (e.g. 1 1/2 -> ["1", "1/2"], "2 2.3 -> ["2", "2.3"])
 SPLIT_SPACED_NUMS   = re.compile(r'^(\d+(?:/\d+|\.\d+)?)\s+(\d+(?:/\d+|\.\d+)?)$')
 # NUMS_SPLIT_BY_SPACES = re.compile(r'^(\d+(?:/\d+|\.\d+)?)\s+(\d+(?:/\d+|\.\d+)?)$')
 
+
+# the 9 types of fractions are:
+# - Whole number / Whole number
+# - Whole number / Decimal
+# - Whole number / Fraction
+# - Decimal / Decimal
+# - Decimal / Whole number
+# - Decimal / Fraction
+# - Fraction / Fraction
+# - Fraction / Decimal
+# - Fraction / Whole number
+FRACTION_TYPE_MAP = {
+    # Put the decimal based patterns first (order matters)
+    "DECIMAL_SLASH_DECIMAL": re.compile(r"\d+\.\d+\s*/\s*\d+\.\d+"),
+    "DECIMAL_SLASH_NUMBER": re.compile(r"\d+\.\d+\s*/\s*\d+"),
+    "DECIMAL_SLASH_FRACTION": re.compile(r"\d+\.\d+\s*/\s*\d+/\d+"),
+    "FRACTION_SLASH_DECIMAL": re.compile(r"\d+/\d+\s*/\s*\d+\.\d+"),
+    "NUMBER_SLASH_DECIMAL": re.compile(r"\d+\s*/\s*\d+\.\d+"),
+
+    # the rest of the patterns without decimals
+    "NUMBER_SLASH_NUMBER": re.compile(r"\d+\s*/\s*\d+"),
+    "NUMBER_SLASH_FRACTION": re.compile(r"\d+\s*/\s*\d+/\d+"),
+    "FRACTION_SLASH_FRACTION": re.compile(r"\d+/\d+\s*/\s*\d+/\d+"),
+    "FRACTION_SLASH_NUMBER": re.compile(r"\d+/\d+\s*/\s*\d+")
+}
+
+# Any fractions with decimals, need to be handled first, hence the order definition here, if you want to find and 
+# convert the fraction patterns in the FRACTION_TYPE_MAP, this is the recommended order to do so
+FRACTION_TYPE_ORDER = ("DECIMAL_SLASH_DECIMAL", "DECIMAL_SLASH_NUMBER", "DECIMAL_SLASH_FRACTION", 
+                           "FRACTION_SLASH_DECIMAL", "NUMBER_SLASH_DECIMAL", 
+                           "NUMBER_SLASH_NUMBER", "NUMBER_SLASH_FRACTION", "FRACTION_SLASH_FRACTION", 
+                           "FRACTION_SLASH_NUMBER")
+# FRACTION_TYPE_MAP = {
+#     # Starts with a decimal:
+#     "DECIMAL_SLASH_DECIMAL": re.compile(r"\d+\.\d+\s*/\s*\d+\.\d+"),
+#     "DECIMAL_SLASH_NUMBER": re.compile(r"\d+\.\d+\s*/\s*\d+"),
+#     "DECIMAL_SLASH_FRACTION": re.compile(r"\d+\.\d+\s*/\s*\d+/\d+"),
+
+#     # Starts with a whole number:
+#     "NUMBER_SLASH_DECIMAL": re.compile(r"\d+\s*/\s*\d+\.\d+"),
+#     "NUMBER_SLASH_NUMBER": re.compile(r"\d+\s*/\s*\d+"),
+#     "NUMBER_SLASH_FRACTION": re.compile(r"\d+\s*/\s*\d+/\d+"),
+
+#     # Starts with a fraction:
+#     "FRACTION_SLASH_FRACTION": re.compile(r"\d+/\d+\s*/\s*\d+/\d+"),
+#     "FRACTION_SLASH_DECIMAL": re.compile(r"\d+/\d+\s*/\s*\d+\.\d+"),
+#     "FRACTION_SLASH_NUMBER": re.compile(r"\d+/\d+\s*/\s*\d+")
+# }
+
+# FRACTION_PATTERN = re.compile(r'\d+\s*/\s*\d+') # TODO: Testing new fraction pattern, old pattern would match even if there was NOT a number in front of the forward slash...
+# FRACTION_PATTERN2 = re.compile(r'\b(\d*\.\d+|\d+)\s*/\s*(\d*\.\d+|\d+)\b')
+# NUMBER_SLASH_NUMBER = re.compile(r'(?:\d*\.\d+|\d+\s*/\s*\d+|\d+)?\s*/\s*(?:\d*\.\d+|\d+\s*/\s*\d+|\d+)?', re.IGNORECASE)
+# NUMBER_SLASH_NUMBER = re.compile(r"\d+(?:/\d+|\.\d+)?\s*/\s*\d+(?:/\d+|\.\d+)?", re.IGNORECASE) # NOTE: NEW version (SAFE)
+
+
 # -----------------------------------------------------------------------------
 # --------------------------- Repeated strings PATTERNS -----------------------
 # Patterns to match specific cases when a known unit string is repeated in a string
 # This is typically seen in ranges where the unit appears after both quantities (e.g. 100 g - 200 g)
 # These regular expressions are used for removing the unit from the string if its repeated
 # -----------------------------------------------------------------------------
 
@@ -414,298 +473,301 @@
 # NUMBER_WITH_INCH_SYMBOL = re.compile(r'(?:\d*\.\d+|\d+\s*/\s*\d+|\d+)\s*\”')
 # NUMBER_WITH_INCH_SYMBOL = re.compile(r'(?:\d*\.\d+|\d+\s*/\s*\d+|\d+)\s*\"')
 
 NUMBER_WITH_INCH_SYMBOL_MAP = {}
 for inch_symbol in ["\"", "”"]:
     NUMBER_WITH_INCH_SYMBOL_MAP[inch_symbol] = re.compile(r'(?:\d*\.\d+|\d+\s*/\s*\d+|\d+)\s*' + inch_symbol + r'')
 
-
-# -----------------------------------------------------------------------------
-# --------------------------- Class to store all regex patterns -----------------------
-# A class to hold all regex patterns used in the recipe parser (version 2)
-# - Each pattern is stored as a class attribute and the class 
-# - IngredientTools class has a single method that applies ALL of the 
-#     regex patterns to a given string and return a dictionary of matches (for testing mainly)
-# -----------------------------------------------------------------------------
-# regex variables and maps to put in the class:
-class IngredientTools:
-    """
-    A class to hold all regex patterns used in recipe parsing.
-    """
-
-    def __init__(self) -> None:
-        # Constant data values and lookup tables
-        self.constants = {
-
-            # regex hashmaps
-            "NUMBER_WORDS": _constants.NUMBER_WORDS,
-            "NUMBER_PREFIX_WORDS": _constants.NUMBER_PREFIX_WORDS,
-            "MULTI_FRACTION_WORDS": _constants.MULTI_FRACTION_WORDS,
-            "FRACTION_WORDS": _constants.FRACTION_WORDS,
-            # "DENOMINATOR_WORDS": _constants.DENOMINATOR_WORDS,
-            "UNICODE_FRACTIONS": _constants.UNICODE_FRACTIONS,
+# # -----------------------------------------------------------------------------
+# # ---------------------------- OLD IngredientTools class... ---------------------------------
+# # -----------------------------------------------------------------------------
+    
+# # -----------------------------------------------------------------------------
+# # --------------------------- Class to store all regex patterns -----------------------
+# # A class to hold all regex patterns used in the recipe parser (version 2)
+# # - Each pattern is stored as a class attribute and the class 
+# # - IngredientTools class has a single method that applies ALL of the 
+# #     regex patterns to a given string and return a dictionary of matches (for testing mainly)
+# # -----------------------------------------------------------------------------
+# # regex variables and maps to put in the class:
+# class IngredientTools:
+#     """
+#     A class to hold all regex patterns used in recipe parsing.
+#     """
+
+#     def __init__(self) -> None:
+#         # Constant data values and lookup tables
+#         self.constants = {
+
+#             # regex hashmaps
+#             "NUMBER_WORDS": _constants.NUMBER_WORDS,
+#             "NUMBER_PREFIX_WORDS": _constants.NUMBER_PREFIX_WORDS,
+#             "MULTI_FRACTION_WORDS": _constants.MULTI_FRACTION_WORDS,
+#             "FRACTION_WORDS": _constants.FRACTION_WORDS,
+#             # "DENOMINATOR_WORDS": _constants.DENOMINATOR_WORDS,
+#             "UNICODE_FRACTIONS": _constants.UNICODE_FRACTIONS,
             
-            # unit hashmaps
-            "UNITS": _constants.UNITS,
-            "BASIC_UNITS": _constants.BASIC_UNITS,
-            "VOLUME_UNITS": _constants.VOLUME_UNITS,
-            "WEIGHT_UNITS": _constants.WEIGHT_UNITS,
-            "DIMENSION_UNITS": _constants.DIMENSION_UNITS,
-            "CASUAL_UNITS": _constants.CASUAL_UNITS,
-
-            # unit hashsets
-            "UNITS_SET": _constants.UNITS_SET,
-            "BASIC_UNITS_SET": _constants.BASIC_UNITS_SET,
-            "NON_BASIC_UNITS_SET": _constants.NON_BASIC_UNITS_SET, 
-            "VOLUME_UNITS_SET": _constants.VOLUME_UNITS_SET,
-            "WEIGHT_UNITS_SET": _constants.WEIGHT_UNITS_SET,
-            "DIMENSION_UNITS_SET": _constants.DIMENSION_UNITS_SET,
-            "SIZE_MODIFIERS_SET": _constants.SIZE_MODIFIERS_SET,
-            "CASUAL_UNITS_SET": _constants.CASUAL_UNITS_SET,
-            "CASUAL_QUANTITIES_SET": _constants.CASUAL_QUANTITIES_SET,
-
-            "CASUAL_QUANTITIES": _constants.CASUAL_QUANTITIES,
-            "UNIT_MODIFIERS": _constants.UNIT_MODIFIERS,
-            "PREP_WORDS": _constants.PREP_WORDS,
-            "APPROXIMATE_STRINGS": _constants.APPROXIMATE_STRINGS,
-            "QUANTITY_PER_UNIT_STRINGS": _constants.QUANTITY_PER_UNIT_STRINGS,
-            "UNIT_TO_STANDARD_UNIT": _constants.UNIT_TO_STANDARD_UNIT,
-            "STOP_WORDS": _constants.STOP_WORDS,
-            "DASH_SYMBOLS": _constants.DASH_SYMBOLS,
-            'REMOVABLE_DASH_SYMBOLS': _constants.REMOVABLE_DASH_SYMBOLS
-        }
-
-        # Define regex patterns
-        # string numbers to number map
-        self.NUMBER_WORDS_MAP = NUMBER_WORDS_MAP
-        self.PREFIXED_NUMBER_WORDS = PREFIXED_NUMBER_WORDS
-        self.PREFIXED_NUMBER_WORDS_GROUPS = PREFIXED_NUMBER_WORDS_GROUPS
+#             # unit hashmaps
+#             "UNITS": _constants.UNITS,
+#             "BASIC_UNITS": _constants.BASIC_UNITS,
+#             "VOLUME_UNITS": _constants.VOLUME_UNITS,
+#             "WEIGHT_UNITS": _constants.WEIGHT_UNITS,
+#             "DIMENSION_UNITS": _constants.DIMENSION_UNITS,
+#             "CASUAL_UNITS": _constants.CASUAL_UNITS,
+
+#             # unit hashsets
+#             "UNITS_SET": _constants.UNITS_SET,
+#             "BASIC_UNITS_SET": _constants.BASIC_UNITS_SET,
+#             "NON_BASIC_UNITS_SET": _constants.NON_BASIC_UNITS_SET, 
+#             "VOLUME_UNITS_SET": _constants.VOLUME_UNITS_SET,
+#             "WEIGHT_UNITS_SET": _constants.WEIGHT_UNITS_SET,
+#             "DIMENSION_UNITS_SET": _constants.DIMENSION_UNITS_SET,
+#             "SIZE_MODIFIERS_SET": _constants.SIZE_MODIFIERS_SET,
+#             "CASUAL_UNITS_SET": _constants.CASUAL_UNITS_SET,
+#             "CASUAL_QUANTITIES_SET": _constants.CASUAL_QUANTITIES_SET,
+
+#             "CASUAL_QUANTITIES": _constants.CASUAL_QUANTITIES,
+#             "UNIT_MODIFIERS": _constants.UNIT_MODIFIERS,
+#             "PREP_WORDS": _constants.PREP_WORDS,
+#             "APPROXIMATE_STRINGS": _constants.APPROXIMATE_STRINGS,
+#             "QUANTITY_PER_UNIT_STRINGS": _constants.QUANTITY_PER_UNIT_STRINGS,
+#             "UNIT_TO_STANDARD_UNIT": _constants.UNIT_TO_STANDARD_UNIT,
+#             "STOP_WORDS": _constants.STOP_WORDS,
+#             "DASH_SYMBOLS": _constants.DASH_SYMBOLS,
+#             'REMOVABLE_DASH_SYMBOLS': _constants.REMOVABLE_DASH_SYMBOLS
+#         }
+
+#         # Define regex patterns
+#         # string numbers to number map
+#         self.NUMBER_WORDS_MAP = NUMBER_WORDS_MAP
+#         self.PREFIXED_NUMBER_WORDS = PREFIXED_NUMBER_WORDS
+#         self.PREFIXED_NUMBER_WORDS_GROUPS = PREFIXED_NUMBER_WORDS_GROUPS
 
-        # unicode fractions
-        self.UNICODE_FRACTIONS_PATTERN = UNICODE_FRACTIONS_PATTERN
+#         # unicode fractions
+#         self.UNICODE_FRACTIONS_PATTERN = UNICODE_FRACTIONS_PATTERN
         
-        # unit matching patterns
-        self.UNITS_PATTERN = UNITS_PATTERN
-        self.BASIC_UNITS_PATTERN = BASIC_UNITS_PATTERN
-        self.NON_BASIC_UNITS_PATTERN = NON_BASIC_UNITS_PATTERN
-        self.VOLUME_UNITS_PATTERN = VOLUME_UNITS_PATTERN
-        self.SIZE_MODIFIERS_PATTERN = SIZE_MODIFIERS_PATTERN
-        self.PREP_WORDS_PATTERN = PREP_WORDS_PATTERN
-        self.STOP_WORDS_PATTERN = STOP_WORDS_PATTERN
-        self.CASUAL_QUANTITIES_PATTERN = CASUAL_QUANTITIES_PATTERN
-        self.CASUAL_UNITS_PATTERN = CASUAL_UNITS_PATTERN
-        self.DIMENSION_UNITS_PATTERN = DIMENSION_UNITS_PATTERN
-        self.UNIT_MODIFIERS_PATTERN = UNIT_MODIFIERS_PATTERN
-        self.APPROXIMATE_STRINGS_PATTERN = APPROXIMATE_STRINGS_PATTERN
-
-        # capture groups for getting anumber followed by the next closest units/basics units/non-basic units
-        self.QUANTITY_UNIT_GROUPS = QUANTITY_UNIT_GROUPS
-        self.QUANTITY_BASIC_UNIT_GROUPS = QUANTITY_BASIC_UNIT_GROUPS
-        self.QUANTITY_NON_BASIC_UNIT_GROUPS = QUANTITY_NON_BASIC_UNIT_GROUPS
-        self.QUANTITY_SOMETIMES_UNIT_GROUPS = QUANTITY_SOMETIMES_UNIT_GROUPS
-        self.QUANTITY_DIMENSION_UNIT_GROUPS = QUANTITY_DIMENSION_UNIT_GROUPS
-        self.QUANTITY_ANYTHING_UNIT_GROUPS = QUANTITY_ANYTHING_UNIT_GROUPS
-        self.QUANTITY_UNIT_ONLY_GROUPS = QUANTITY_UNIT_ONLY_GROUPS
-        self.EQUIV_QUANTITY_UNIT_GROUPS = EQUIV_QUANTITY_UNIT_GROUPS
+#         # unit matching patterns
+#         self.UNITS_PATTERN = UNITS_PATTERN
+#         self.BASIC_UNITS_PATTERN = BASIC_UNITS_PATTERN
+#         self.NON_BASIC_UNITS_PATTERN = NON_BASIC_UNITS_PATTERN
+#         self.VOLUME_UNITS_PATTERN = VOLUME_UNITS_PATTERN
+#         self.SIZE_MODIFIERS_PATTERN = SIZE_MODIFIERS_PATTERN
+#         self.PREP_WORDS_PATTERN = PREP_WORDS_PATTERN
+#         self.STOP_WORDS_PATTERN = STOP_WORDS_PATTERN
+#         self.CASUAL_QUANTITIES_PATTERN = CASUAL_QUANTITIES_PATTERN
+#         self.CASUAL_UNITS_PATTERN = CASUAL_UNITS_PATTERN
+#         self.DIMENSION_UNITS_PATTERN = DIMENSION_UNITS_PATTERN
+#         self.UNIT_MODIFIERS_PATTERN = UNIT_MODIFIERS_PATTERN
+#         self.APPROXIMATE_STRINGS_PATTERN = APPROXIMATE_STRINGS_PATTERN
+
+#         # capture groups for getting anumber followed by the next closest units/basics units/non-basic units
+#         self.QUANTITY_UNIT_GROUPS = QUANTITY_UNIT_GROUPS
+#         self.QUANTITY_BASIC_UNIT_GROUPS = QUANTITY_BASIC_UNIT_GROUPS
+#         self.QUANTITY_NON_BASIC_UNIT_GROUPS = QUANTITY_NON_BASIC_UNIT_GROUPS
+#         self.QUANTITY_SOMETIMES_UNIT_GROUPS = QUANTITY_SOMETIMES_UNIT_GROUPS
+#         self.QUANTITY_DIMENSION_UNIT_GROUPS = QUANTITY_DIMENSION_UNIT_GROUPS
+#         self.QUANTITY_ANYTHING_UNIT_GROUPS = QUANTITY_ANYTHING_UNIT_GROUPS
+#         self.QUANTITY_UNIT_ONLY_GROUPS = QUANTITY_UNIT_ONLY_GROUPS
+#         self.EQUIV_QUANTITY_UNIT_GROUPS = EQUIV_QUANTITY_UNIT_GROUPS
         
-        # word fraction patterns
-        self.NUMBER_WITH_FRACTION_WORD = NUMBER_WITH_FRACTION_WORD
-        self.NUMBER_WITH_FRACTION_WORD_GROUPS = NUMBER_WITH_FRACTION_WORD_GROUPS
-        self.NUMBER_WITH_FRACTION_WORD_MAP = NUMBER_WITH_FRACTION_WORD_MAP
-
-        # generic number matchings and/or numbers with specific separators
-        self.ALL_NUMBERS = ALL_NUMBERS
-        self.SPACE_SEP_NUMBERS = SPACE_SEP_NUMBERS
-        self.NUMBERS_SEPARATED_BY_ADD_SYMBOLS = NUMBERS_SEPARATED_BY_ADD_SYMBOLS
-        self.NUMBERS_SEPARATED_BY_ADD_SYMBOLS_GROUPS = NUMBERS_SEPARATED_BY_ADD_SYMBOLS_GROUPS
-
-        # range patterns
-        self.QUANTITY_DASH_QUANTITY = QUANTITY_DASH_QUANTITY
-        self.QUANTITY_DASH_QUANTITY_GROUPS = QUANTITY_DASH_QUANTITY_GROUPS
-        self.QUANTITY_DASH_QUANTITY_UNIT = QUANTITY_DASH_QUANTITY_UNIT
-        self.QUANTITY_OR_QUANTITY = QUANTITY_OR_QUANTITY
-        self.QUANTITY_TO_QUANTITY = QUANTITY_TO_QUANTITY
-        self.BETWEEN_QUANTITY_AND_QUANTITY = BETWEEN_QUANTITY_AND_QUANTITY
-
-        # fraction specific patterns
-        self.FRACTION_PATTERN = FRACTION_PATTERN
-        self.SPLIT_SPACED_NUMS = SPLIT_SPACED_NUMS
+#         # word fraction patterns
+#         self.NUMBER_WITH_FRACTION_WORD = NUMBER_WITH_FRACTION_WORD
+#         self.NUMBER_WITH_FRACTION_WORD_GROUPS = NUMBER_WITH_FRACTION_WORD_GROUPS
+#         self.NUMBER_WITH_FRACTION_WORD_MAP = NUMBER_WITH_FRACTION_WORD_MAP
+
+#         # generic number matchings and/or numbers with specific separators
+#         self.ALL_NUMBERS = ALL_NUMBERS
+#         self.SPACE_SEP_NUMBERS = SPACE_SEP_NUMBERS
+#         self.NUMBERS_SEPARATED_BY_ADD_SYMBOLS = NUMBERS_SEPARATED_BY_ADD_SYMBOLS
+#         self.NUMBERS_SEPARATED_BY_ADD_SYMBOLS_GROUPS = NUMBERS_SEPARATED_BY_ADD_SYMBOLS_GROUPS
+
+#         # range patterns
+#         self.QUANTITY_DASH_QUANTITY = QUANTITY_DASH_QUANTITY
+#         self.QUANTITY_DASH_QUANTITY_GROUPS = QUANTITY_DASH_QUANTITY_GROUPS
+#         self.QUANTITY_DASH_QUANTITY_UNIT = QUANTITY_DASH_QUANTITY_UNIT
+#         self.QUANTITY_OR_QUANTITY = QUANTITY_OR_QUANTITY
+#         self.QUANTITY_TO_QUANTITY = QUANTITY_TO_QUANTITY
+#         self.BETWEEN_QUANTITY_AND_QUANTITY = BETWEEN_QUANTITY_AND_QUANTITY
+
+#         # fraction specific patterns
+#         self.FRACTION_PATTERN = FRACTION_PATTERN
+#         self.SPLIT_SPACED_NUMS = SPLIT_SPACED_NUMS
         
-        # repeated unit string patterns
-        self.REPEAT_UNIT_RANGES = REPEAT_UNIT_RANGES
+#         # repeated unit string patterns
+#         self.REPEAT_UNIT_RANGES = REPEAT_UNIT_RANGES
 
-        # miscellaneous patterns
-        self.CONSECUTIVE_LETTERS_DIGITS = CONSECUTIVE_LETTERS_DIGITS
+#         # miscellaneous patterns
+#         self.CONSECUTIVE_LETTERS_DIGITS = CONSECUTIVE_LETTERS_DIGITS
 
-        self.SPLIT_BY_PARENTHESIS = SPLIT_BY_PARENTHESIS
+#         self.SPLIT_BY_PARENTHESIS = SPLIT_BY_PARENTHESIS
 
-        # "x" and "X" separators
-        self.X_AFTER_NUMBER = X_AFTER_NUMBER
-
-        # match specific strings 
-        self.OPTIONAL_STRING = OPTIONAL_STRING
-        self.REQUIRED_STRING = REQUIRED_STRING
-        self.WORDS_ENDING_IN_LY = WORDS_ENDING_IN_LY
-        self.PCT_REGEX_MAP = PCT_REGEX_MAP
-        self.NUMBER_WITH_INCH_SYMBOL_MAP = NUMBER_WITH_INCH_SYMBOL_MAP
-
-        # get a list of all the attributes of the class in sorted order by name
-        self.sorted_keys = sorted(self.__dict__.keys(), key=lambda x: x[0])
-
-        # # Sort attributes by name
-        # self.sorted_attrs = sorted(self.__dict__.items(), key=lambda x: x[0])
-
-    def find_matches(self, input_string: str) -> Dict[str, List[Union[str, Tuple[str]]]]:
-        """
-        Find all matches in the input string for each regex pattern.
-        Returns a dictionary with pattern names as keys and corresponding matches as values.
-        """
-
-        matches = {}
-        for name, pattern in self.__dict__.items():
-            if isinstance(pattern, re.Pattern):
-                matches[name] = pattern.findall(input_string)
-        return matches
+#         # "x" and "X" separators
+#         self.X_AFTER_NUMBER = X_AFTER_NUMBER
+
+#         # match specific strings 
+#         self.OPTIONAL_STRING = OPTIONAL_STRING
+#         self.REQUIRED_STRING = REQUIRED_STRING
+#         self.WORDS_ENDING_IN_LY = WORDS_ENDING_IN_LY
+#         self.PCT_REGEX_MAP = PCT_REGEX_MAP
+#         self.NUMBER_WITH_INCH_SYMBOL_MAP = NUMBER_WITH_INCH_SYMBOL_MAP
+
+#         # get a list of all the attributes of the class in sorted order by name
+#         self.sorted_keys = sorted(self.__dict__.keys(), key=lambda x: x[0])
+
+#         # # Sort attributes by name
+#         # self.sorted_attrs = sorted(self.__dict__.items(), key=lambda x: x[0])
+
+#     def find_matches(self, input_string: str) -> Dict[str, List[Union[str, Tuple[str]]]]:
+#         """
+#         Find all matches in the input string for each regex pattern.
+#         Returns a dictionary with pattern names as keys and corresponding matches as values.
+#         """
+
+#         matches = {}
+#         for name, pattern in self.__dict__.items():
+#             if isinstance(pattern, re.Pattern):
+#                 matches[name] = pattern.findall(input_string)
+#         return matches
     
-    def print_matches(self, input_string: str) -> None:
-        """
-        Print out all matches in the input string for each regex pattern.
-        Returns None
-        """
-        matches = {}
+#     def print_matches(self, input_string: str) -> None:
+#         """
+#         Print out all matches in the input string for each regex pattern.
+#         Returns None
+#         """
+#         matches = {}
         
-        for key in self.sorted_keys:
-            attribute = self.__dict__[key]
-            if isinstance(attribute, re.Pattern):
-                matches[key] = attribute.findall(input_string)
-                print(f"{key}: {matches[key]}")
-
-        # matches = {}
-        # for name, pattern in self.__dict__.items():
-        #     if isinstance(pattern, re.Pattern):
-        #         matches[name] = pattern.findall(input_string)
-        #         print(f"{name}: {matches[name]}")
+#         for key in self.sorted_keys:
+#             attribute = self.__dict__[key]
+#             if isinstance(attribute, re.Pattern):
+#                 matches[key] = attribute.findall(input_string)
+#                 print(f"{key}: {matches[key]}")
+
+#         # matches = {}
+#         # for name, pattern in self.__dict__.items():
+#         #     if isinstance(pattern, re.Pattern):
+#         #         matches[name] = pattern.findall(input_string)
+#         #         print(f"{name}: {matches[name]}")
 
         
-    def list_constants(self) -> None:
-        """
-        List all the attributes of the class.
-        """ 
-
-        # attrs = [name for name in self.__dict__]
-
-        for name, pattern in self.__dict__.items():
-            print(f"- {name} ({type(self.__dict__[name]).__name__})")
-            if isinstance(self.__dict__[name], dict):
-                print(f"  > {len(self.__dict__[name])} items")
-                # for key, value in self.__dict__[name].items():
-                #     print(f"   - {key}")
-        # return [name for name in self.__dict__ if isinstance(self.__dict__[name], re.Pattern)]
+#     def list_constants(self) -> None:
+#         """
+#         List all the attributes of the class.
+#         """ 
+
+#         # attrs = [name for name in self.__dict__]
+
+#         for name, pattern in self.__dict__.items():
+#             print(f"- {name} ({type(self.__dict__[name]).__name__})")
+#             if isinstance(self.__dict__[name], dict):
+#                 print(f"  > {len(self.__dict__[name])} items")
+#                 # for key, value in self.__dict__[name].items():
+#                 #     print(f"   - {key}")
+#         # return [name for name in self.__dict__ if isinstance(self.__dict__[name], re.Pattern)]
     
-    def get_desc(self, pattern_name: str) -> str:
-        """
-        Get the description of a specific regex pattern.
-        Returns the description of the pattern if found, otherwise returns an empty string.
-        """
+#     def get_desc(self, pattern_name: str) -> str:
+#         """
+#         Get the description of a specific regex pattern.
+#         Returns the description of the pattern if found, otherwise returns an empty string.
+#         """
         
-        # Define descriptions for each pattern
-        descriptions = {
-            ### Constants and lookup tables
-            "NUMBER_WORDS": "Dictionary of number words to numerical values.",
-            "MULTI_FRACTION_WORDS": "Dictionary of fraction phrases (i.e. 'two thirds' or '1 half') to their fractional string value",
-            "FRACTION_WORDS": "Dictionary of single fraction words that represent a singular fraction (i.e. a quarter is equal to 1/4).",
-            "UNICODE_FRACTIONS": "Dictionary of unicode fractions to numerical values.",
-
-            # dictionaries of units
-            "UNITS": "Dictionary of units used in the recipe parser (All units, including basic, volume, and specific units).",
-            "BASIC_UNITS": "Dictionary of basic units used in the recipe parser (The most common units).",
-            "VOLUME_UNITS": "Dictionary of volume units used in the recipe parser (Units used for measuring volume).",
-            "WEIGHT_UNITS": "Dictionary of weight units used in the recipe parser (Units used for measuring weight).",
-            "DIMENSION_UNITS": "Dictionary of dimension units used in the recipe parser (Units used for measuring dimensions).",
-            "CASUAL_UNITS": "Dictionary of casual units used in the recipe parser (Units that are not standard units).",
-
-            # sets of all unit words
-            "UNITS_SET": "Set of units used in the recipe parser (All units, including basic, volume, and specific units).",
-            "BASIC_UNITS_SET": "Set of basic units used in the recipe parser (The most common units).",
-            "NON_BASIC_UNITS_SET": "Set of non-basic units used in the recipe parser (Units that are not in the BASIC_UNITS dictionary).",
-            "SIZE_MODIFIERS_SET": "Set of units that are sometimes used in the recipe parser (Set of words that MIGHT be units if no other units are around).",
-            "VOLUME_UNITS_SET": "Set of volume units used in the recipe parser (Units used for measuring volume).",
-            "WEIGHT_UNITS_SET": "Set of weight units used in the recipe parser (Units used for measuring weight).",
-            "DIMENSION_UNITS_SET": "Set of dimension units used in the recipe parser (Units used for measuring dimensions).",
-            "CASUAL_UNITS_SET": "Set of casual units used in the recipe parser (Units that are not standard units).",
-            "CASUAL_QUANTITIES_SET": "Set of casual quantities used in the recipe parser (Quantities that are not standard quantities).",
-
-            "CASUAL_QUANTITIES": "Dictionary of casual quantities used in the recipe parser.",
-            "UNIT_MODIFIERS": "Set of unit modifier words for lookups in recipe parser.",
-            "PREP_WORDS": "Set of preparation words for lookups in recipe parser.",
-            "APPROXIMATE_STRINGS": "Set of strings that indicate an approximate quantity in the recipe parser.",
-            "QUANTITY_PER_UNIT_STRINGS": "Set of strings that indicate a quantity per unit in the recipe parser.",
-            "NUMBER_WORDS_MAP": "Dictionary of regex patterns to match number words in a string (i.e. 'one' : '1', 'two' : '2').",
+#         # Define descriptions for each pattern
+#         descriptions = {
+#             ### Constants and lookup tables
+#             "NUMBER_WORDS": "Dictionary of number words to numerical values.",
+#             "MULTI_FRACTION_WORDS": "Dictionary of fraction phrases (i.e. 'two thirds' or '1 half') to their fractional string value",
+#             "FRACTION_WORDS": "Dictionary of single fraction words that represent a singular fraction (i.e. a quarter is equal to 1/4).",
+#             "UNICODE_FRACTIONS": "Dictionary of unicode fractions to numerical values.",
+
+#             # dictionaries of units
+#             "UNITS": "Dictionary of units used in the recipe parser (All units, including basic, volume, and specific units).",
+#             "BASIC_UNITS": "Dictionary of basic units used in the recipe parser (The most common units).",
+#             "VOLUME_UNITS": "Dictionary of volume units used in the recipe parser (Units used for measuring volume).",
+#             "WEIGHT_UNITS": "Dictionary of weight units used in the recipe parser (Units used for measuring weight).",
+#             "DIMENSION_UNITS": "Dictionary of dimension units used in the recipe parser (Units used for measuring dimensions).",
+#             "CASUAL_UNITS": "Dictionary of casual units used in the recipe parser (Units that are not standard units).",
+
+#             # sets of all unit words
+#             "UNITS_SET": "Set of units used in the recipe parser (All units, including basic, volume, and specific units).",
+#             "BASIC_UNITS_SET": "Set of basic units used in the recipe parser (The most common units).",
+#             "NON_BASIC_UNITS_SET": "Set of non-basic units used in the recipe parser (Units that are not in the BASIC_UNITS dictionary).",
+#             "SIZE_MODIFIERS_SET": "Set of units that are sometimes used in the recipe parser (Set of words that MIGHT be units if no other units are around).",
+#             "VOLUME_UNITS_SET": "Set of volume units used in the recipe parser (Units used for measuring volume).",
+#             "WEIGHT_UNITS_SET": "Set of weight units used in the recipe parser (Units used for measuring weight).",
+#             "DIMENSION_UNITS_SET": "Set of dimension units used in the recipe parser (Units used for measuring dimensions).",
+#             "CASUAL_UNITS_SET": "Set of casual units used in the recipe parser (Units that are not standard units).",
+#             "CASUAL_QUANTITIES_SET": "Set of casual quantities used in the recipe parser (Quantities that are not standard quantities).",
+
+#             "CASUAL_QUANTITIES": "Dictionary of casual quantities used in the recipe parser.",
+#             "UNIT_MODIFIERS": "Set of unit modifier words for lookups in recipe parser.",
+#             "PREP_WORDS": "Set of preparation words for lookups in recipe parser.",
+#             "APPROXIMATE_STRINGS": "Set of strings that indicate an approximate quantity in the recipe parser.",
+#             "QUANTITY_PER_UNIT_STRINGS": "Set of strings that indicate a quantity per unit in the recipe parser.",
+#             "NUMBER_WORDS_MAP": "Dictionary of regex patterns to match number words in a string (i.e. 'one' : '1', 'two' : '2').",
             
-            ### Regex patterns
+#             ### Regex patterns
 
-            # simple unit matching patterns
-            "UNITS_PATTERN": "Matches units in a string.",
-            "BASIC_UNITS_PATTERN": "Matches just the basic units from the BASIC_UNITS dictionary.",
-            "NON_BASIC_UNITS_PATTERN": "Matches non-basic units in a string.",
-            "VOLUME_UNITS_PATTERN": "Matches specifically volume units in a string.",
-            "SIZE_MODIFIERS_PATTERN": "Matches sometimes units in a string.",
-            "PREP_WORDS_PATTERN": "Matches preparation words in a string.",
-            "STOP_WORDS_PATTERN": "Matches stop words in a string.",
-            "CASUAL_QUANTITIES_PATTERN": "Matches casual quantities in a string (i.e. 'couple' = 2).",
-            "CASUAL_UNITS_PATTERN": "Matches casual units in a string (i.e. 'dash', 'pinch').",
-            "DIMENSION_UNITS_PATTERN": "Matches dimension units in a string (i.e. 'inches', 'cm').",
-            "UNIT_MODIFIERS_PATTERN": "Matches unit modifiers in a string (i.e. 'large', 'small').",
-            "APPROXIMATE_STRINGS_PATTERN": "Matches approximate strings in a string (i.e. 'about', 'approximately').",
-
-            "QUANTITY_UNIT_GROUPS": "Matches a number followed by a unit with capture groups.", 
-            "QUANTITY_BASIC_UNIT_GROUPS": "Matches a number followed by a basic unit with capture groups.",
-            "QUANTITY_NON_BASIC_UNIT_GROUPS": "Matches a number followed by a non-basic unit with capture groups.",
-            "QUANTITY_SOMETIMES_UNIT_GROUPS": "Matches a number followed by a 'sometimes unit' with capture groups (i.e. 'large' is sometimes a unit if no other units are around).",
-            "QUANTITY_ANYTHING_UNIT_GROUPS": "Matches a number followed by any text and then a unit with capture groups.",
-            "QUANTITY_DIMENSION_UNIT_GROUPS": "Matches a number followed by a dimension unit with capture groups.",
-            "QUANTITY_UNIT_ONLY_GROUPS": "Matches a quantity followed by  0+whitespaces/hypens and then a unit with capture groups.",
-            "EQUIV_QUANTITY_UNIT_GROUPS": "Matches an 'approximate/equivalent' string followed by a number followed by a unit with capture groups (helpful for finding equivalent quantity-unit patterns i.e. 'about 1/2 cup').",
-
-            # general umber matching patterns and number with specific separators
-            "ALL_NUMBERS": "Matches ALL number/decimal/fraction in a string regardless of padding.",
-            "SPACE_SEP_NUMBERS": "Matches any number/decimal/fraction followed by a space and then another number/decimal/fraction.",
-            "NUMBERS_SEPARATED_BY_ADD_SYMBOLS_GROUPS": "Matches numbers/decimals/fractions separated by 'and', '&', 'plus', or '+' symbols with capture groups.",
-
-            "QUANTITY_DASH_QUANTITY": "Matches numbers/decimals/fractions followed by a hyphen to numbers/decimals/fractions.",
-            "QUANTITY_DASH_QUANTITY_GROUPS": "Matches numbers/decimals/fractions followed by a hyphen to numbers/decimals/fractions with capture groups.",
-            "QUANTITY_DASH_QUANTITY_UNIT": "Matches numbers/decimals/fractions followed by a hyphen to numbers/decimals/fractions followed by a unit (0+ whitespace between last number and the unit).",
-            "QUANTITY_OR_QUANTITY": "Matches numbers/decimals/fractions separated by 'or'.",
-            "QUANTITY_TO_QUANTITY": "Matches numbers/decimals/fractions separated by 'to'.",
-            "BETWEEN_QUANTITY_AND_QUANTITY": "Matches numbers/decimals/fractions separated by 'between' and 'and'.",
+#             # simple unit matching patterns
+#             "UNITS_PATTERN": "Matches units in a string.",
+#             "BASIC_UNITS_PATTERN": "Matches just the basic units from the BASIC_UNITS dictionary.",
+#             "NON_BASIC_UNITS_PATTERN": "Matches non-basic units in a string.",
+#             "VOLUME_UNITS_PATTERN": "Matches specifically volume units in a string.",
+#             "SIZE_MODIFIERS_PATTERN": "Matches sometimes units in a string.",
+#             "PREP_WORDS_PATTERN": "Matches preparation words in a string.",
+#             "STOP_WORDS_PATTERN": "Matches stop words in a string.",
+#             "CASUAL_QUANTITIES_PATTERN": "Matches casual quantities in a string (i.e. 'couple' = 2).",
+#             "CASUAL_UNITS_PATTERN": "Matches casual units in a string (i.e. 'dash', 'pinch').",
+#             "DIMENSION_UNITS_PATTERN": "Matches dimension units in a string (i.e. 'inches', 'cm').",
+#             "UNIT_MODIFIERS_PATTERN": "Matches unit modifiers in a string (i.e. 'large', 'small').",
+#             "APPROXIMATE_STRINGS_PATTERN": "Matches approximate strings in a string (i.e. 'about', 'approximately').",
+
+#             "QUANTITY_UNIT_GROUPS": "Matches a number followed by a unit with capture groups.", 
+#             "QUANTITY_BASIC_UNIT_GROUPS": "Matches a number followed by a basic unit with capture groups.",
+#             "QUANTITY_NON_BASIC_UNIT_GROUPS": "Matches a number followed by a non-basic unit with capture groups.",
+#             "QUANTITY_SOMETIMES_UNIT_GROUPS": "Matches a number followed by a 'sometimes unit' with capture groups (i.e. 'large' is sometimes a unit if no other units are around).",
+#             "QUANTITY_ANYTHING_UNIT_GROUPS": "Matches a number followed by any text and then a unit with capture groups.",
+#             "QUANTITY_DIMENSION_UNIT_GROUPS": "Matches a number followed by a dimension unit with capture groups.",
+#             "QUANTITY_UNIT_ONLY_GROUPS": "Matches a quantity followed by  0+whitespaces/hypens and then a unit with capture groups.",
+#             "EQUIV_QUANTITY_UNIT_GROUPS": "Matches an 'approximate/equivalent' string followed by a number followed by a unit with capture groups (helpful for finding equivalent quantity-unit patterns i.e. 'about 1/2 cup').",
+
+#             # general umber matching patterns and number with specific separators
+#             "ALL_NUMBERS": "Matches ALL number/decimal/fraction in a string regardless of padding.",
+#             "SPACE_SEP_NUMBERS": "Matches any number/decimal/fraction followed by a space and then another number/decimal/fraction.",
+#             "NUMBERS_SEPARATED_BY_ADD_SYMBOLS_GROUPS": "Matches numbers/decimals/fractions separated by 'and', '&', 'plus', or '+' symbols with capture groups.",
+
+#             "QUANTITY_DASH_QUANTITY": "Matches numbers/decimals/fractions followed by a hyphen to numbers/decimals/fractions.",
+#             "QUANTITY_DASH_QUANTITY_GROUPS": "Matches numbers/decimals/fractions followed by a hyphen to numbers/decimals/fractions with capture groups.",
+#             "QUANTITY_DASH_QUANTITY_UNIT": "Matches numbers/decimals/fractions followed by a hyphen to numbers/decimals/fractions followed by a unit (0+ whitespace between last number and the unit).",
+#             "QUANTITY_OR_QUANTITY": "Matches numbers/decimals/fractions separated by 'or'.",
+#             "QUANTITY_TO_QUANTITY": "Matches numbers/decimals/fractions separated by 'to'.",
+#             "BETWEEN_QUANTITY_AND_QUANTITY": "Matches numbers/decimals/fractions separated by 'between' and 'and'.",
             
-            # Unicode fractions
-            "UNICODE_FRACTIONS_PATTERN": "Matches unicode fractions in the string.",
+#             # Unicode fractions
+#             "UNICODE_FRACTIONS_PATTERN": "Matches unicode fractions in the string.",
             
-            # fraction word patterns
-            "NUMBER_WITH_FRACTION_WORD_GROUPS": "Matches a number followed by a fraction word with capture groups.",
-            "NUMBER_WITH_FRACTION_WORD_MAP": "Dictionary of regex patterns to match number followed by a fraction word in a string (i.e. '1 half' : '1 1/2').",
-
-            # fraction specific patterns
-            "FRACTION_PATTERN": "Matches fraction parts in a string.",
-            "SPLIT_SPACED_NUMS": "Splits numbers/decimals/fractions separated by 1+ whitespaces into a capture group (i.e '1.5 1/2' -> ['1.5', '1/2']).",
-            "REPEAT_UNIT_RANGES": "Matches repeated unit strings in a string.",
-
-            "SPLIT_BY_PARENTHESIS": "Matches parentheses in a string and splits the string by them if used with re.split().",
-
-            "CONSECUTIVE_LETTERS_DIGITS": "Matches consecutive letters and digits in a string.",
-            "X_AFTER_NUMBER": "Matches a number followed by an 'x'/'X' (can't be the start of a word starting with xX).",
-            "OPTIONAL_STRING": "Matches the word 'optional', 'option', 'opt', etc. in a string.",
-            "REQUIRED_STRING": "Matches the word 'required', 'requirement', 'req', etc. in a string.",
-            "WORDS_ENDING_IN_LY": "Matches any word ending in 'ly' (i.e. 'firmly', 'lightly', 'rapidly').",
-            "PCT_REGEX_MAP" : "Dictionary of regex patterns to match numbers followed by a percentage character '%', 'percentage', 'percent', or 'pct'."
-        }
+#             # fraction word patterns
+#             "NUMBER_WITH_FRACTION_WORD_GROUPS": "Matches a number followed by a fraction word with capture groups.",
+#             "NUMBER_WITH_FRACTION_WORD_MAP": "Dictionary of regex patterns to match number followed by a fraction word in a string (i.e. '1 half' : '1 1/2').",
+
+#             # fraction specific patterns
+#             "FRACTION_PATTERN": "Matches fraction parts in a string.",
+#             "SPLIT_SPACED_NUMS": "Splits numbers/decimals/fractions separated by 1+ whitespaces into a capture group (i.e '1.5 1/2' -> ['1.5', '1/2']).",
+#             "REPEAT_UNIT_RANGES": "Matches repeated unit strings in a string.",
+
+#             "SPLIT_BY_PARENTHESIS": "Matches parentheses in a string and splits the string by them if used with re.split().",
+
+#             "CONSECUTIVE_LETTERS_DIGITS": "Matches consecutive letters and digits in a string.",
+#             "X_AFTER_NUMBER": "Matches a number followed by an 'x'/'X' (can't be the start of a word starting with xX).",
+#             "OPTIONAL_STRING": "Matches the word 'optional', 'option', 'opt', etc. in a string.",
+#             "REQUIRED_STRING": "Matches the word 'required', 'requirement', 'req', etc. in a string.",
+#             "WORDS_ENDING_IN_LY": "Matches any word ending in 'ly' (i.e. 'firmly', 'lightly', 'rapidly').",
+#             "PCT_REGEX_MAP" : "Dictionary of regex patterns to match numbers followed by a percentage character '%', 'percentage', 'percent', or 'pct'."
+#         }
 
-        # Retrieve description based on pattern name
-        return descriptions.get(pattern_name, "")
+#         # Retrieve description based on pattern name
+#         return descriptions.get(pattern_name, "")
     
 # ##################################################################################################################
 # ##################################################################################################################
 # ########################################## OLD SETUP CODE BELOW ##################################################
 # ##################################################################################################################
 
 # # Description: This module contains all the regex patterns used in the recipe parser.
```

### Comparing `ingredient_slicer-0.0.81/ingredient_slicer/_utils.py` & `ingredient_slicer-0.0.83/ingredient_slicer/_utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 
+
 from fractions import Fraction
+from html import unescape
 import re
+import warnings
+from typing import List, Dict, Any, Union, Tuple, Callable
 
 from ingredient_slicer import _constants, _regex_patterns
 
 # -----------------------------------------------------------------------------------------------
 # ---- Utility functions for handling numbers, decimals, and fractions in strings ----
 # -----------------------------------------------------------------------------------------------
 
@@ -21,44 +25,70 @@
         "1"
         >>> make_int_or_float_str("1")
         "1"
         >>> make_int_or_float_str("0.25")
         "0.25"
         """
 
+        # convert integer/float to string if it's not already a string
+        if isinstance(number_str, (int, float)):
+            number_str = str(number_str)
+
         number_str = number_str.replace(" ", "")
 
+        # # NOTE: remove negative sign if it exists and replace whitespace
+        # is_negative = False
+        # if number_str[0] == "-":
+        #     is_negative = True
+        #     number_str = number_str[1:]
+        #     number_str = number_str.replace(" ", "")
+
         period_count = 0
 
         for i in number_str:
             if i == ".":
                 period_count += 1
             if not i.isdigit() and i != ".":
                 raise ValueError("Invalid character in number. Only digits and periods are allowed.")
             
         if period_count > 1:
             raise ValueError("Invalid number format. Only one period is allowed in a number.")
-
+        
         number = float(number_str.strip())  # Convert string to float
 
         if number == int(number):  # Check if float is equal to its integer value
+
+            # f"-{str(int(number))}" if is_negative else str(int(number))
+
             return str(int(number))  # Return integer value if it's a whole number
         else:
+            # f"-{str(number)}" if is_negative else str(number)
+
             return str(number)  # Return float if it's a decimal
 
+# -----------------------------------------------------------------------------------------------
+# ---- Convert a string fraction to a decimal (i.e. "1/2" -> "0.5") ----
+# -----------------------------------------------------------------------------------------------
+
 def _fraction_str_to_decimal(fraction_str: str) -> str:
         """
         Convert a string representation of a fraction to its decimal equivalent.
         Args:
             fraction_str (str): The string representation of the fraction. Must only contain digits, a forward slash, and possible whitespace. 
                                     Numbers must be separated by a forward slash. If a whole number string or a decimal string is passed, it will be returned as a string, 
                                     and converted to a whole number if values after the decimal point are only zeros (i.e. 1.0 -> 1, 2.0 -> 2, 3.00 -> 3).
         Returns:
             str: The decimal value of the fraction as a string. 
         """
+        # FRACTION_PATTERN2 = re.compile(r'\d+(?:\.\d+|/\d+)')
+
+        # fraction_str = "4/0.48"
+        # fraction_str = "4/0.48"
+        # FRACTION_PATTERN2.findall(fraction_str)
+        # 4/0.48
 
         if not isinstance(fraction_str, str):
             raise ValueError("Invalid input. Fraction string must be a string.")
 
         # Split the fraction string into its numerator and denominator
         split_fraction = [i.strip() for i in fraction_str.split("/")]
         # print(f"Split Fraction: {split_fraction}") if self.debug else None
@@ -71,21 +101,111 @@
 
             # print(f"---> OLD Output: {round(float(split_fraction[0]), 3)}")
             # print(f"---> NEW Output: {converted_number}")
             return converted_number
         
         # after returning cases of just a whole number or decimal number and returning that, 
         # we make sure all of our characters are valid 
-        has_only_valid_chars = all([i.isdigit() or i in {"-", "/", " "} for i in fraction_str])
+        has_only_valid_chars = all([i.isdigit() or i in {"-", "/", " ", "."} for i in fraction_str])
+        # has_only_valid_chars = all([i.isdigit() or i in {"-", "/", " "} for i in fraction_str])
+
+        if not has_only_valid_chars:
+            raise ValueError("Invalid input. Fraction string must contain only digits, hyphens, and a forward slash (possible invalid characters and/or periods?)")
+
+        # # numerator = int(split_fraction[0])
+        # # denominator = int(split_fraction[1])
+        # numerator = int(float(split_fraction[0])) # TODO: This is being tested out
+        # denominator = int(float(split_fraction[1]))
+        # is_negative = True if (numerator < 0 and denominator >= 0) or (numerator >= 0 and denominator < 0) else False
+
+        # Convert the fraction to a decimal
+        # return round(float(Fraction(numerator, denominator)), 3)
+
+        # decimal_value = round(float(Fraction(numerator, denominator)), 3)
+        
+        # converts the split up fraction list to a float
+        decimal_value = round(_split_fraction_to_float(split_fraction), 3)
+
+        is_negative   = True if decimal_value < 0 else False
+
+        if is_negative:
+            decimal_value = decimal_value * -1
+            # decimal_value = decimal_value.replace("-", "")
+        
+        decimal_str = f"-{_make_int_or_float_str(str(decimal_value))}" if is_negative else _make_int_or_float_str(str(decimal_value))
+
+        # return _make_int_or_float_str(str(round(float(Fraction(numerator, denominator)), 3)))
+        return decimal_str
+
+def _split_fraction_to_float(split_fraction: list) -> float:
+    """
+    Convert a split fraction to a float.
+    Args:
+        split_fraction (list): A list containing the numerator and denominator of a fraction.
+    Returns:
+        float: The float value of the fraction.
+    """
+
+    numerator_fraction =  Fraction(split_fraction[0])
+    denominator_fraction = Fraction(split_fraction[1])
+
+    return float(Fraction(numerator_fraction, denominator_fraction))
+
+# TODO: Delete/Deprecated, this is the old version of the _fraction_str_to_decimal function above
+def _fraction_str_to_decimal2(fraction_str: str) -> str:
+        """
+        Convert a string representation of a fraction to its decimal equivalent.
+        Args:
+            fraction_str (str): The string representation of the fraction. Must only contain digits, a forward slash, and possible whitespace. 
+                                    Numbers must be separated by a forward slash. If a whole number string or a decimal string is passed, it will be returned as a string, 
+                                    and converted to a whole number if values after the decimal point are only zeros (i.e. 1.0 -> 1, 2.0 -> 2, 3.00 -> 3).
+        Returns:
+            str: The decimal value of the fraction as a string. 
+        """
+        # FRACTION_PATTERN2 = re.compile(r'\d+(?:\.\d+|/\d+)')
+
+        # fraction_str = "4/0.48"
+        # fraction_str = "4/0.48."
+        # fraction_str = ".3/4"
+        # FRACTION_PATTERN2.findall(fraction_str)
+        # 4/0.48
+        
+        if not isinstance(fraction_str, str):
+            raise ValueError("Invalid input. Fraction string must be a string.")
+
+        # Split the fraction string into its numerator and denominator
+        split_fraction = [i.strip() for i in fraction_str.split("/")]
+        # print(f"Split Fraction: {split_fraction}") if self.debug else None
+
+        # If the fraction is a whole number, return the number
+        if len(split_fraction) == 1:
+            # print(f"---> Only one part: {split_fraction[0]}")
+
+            converted_number = _make_int_or_float_str(split_fraction[0])
+
+            # print(f"---> OLD Output: {round(float(split_fraction[0]), 3)}")
+            # print(f"---> NEW Output: {converted_number}")
+            return converted_number
+        
+        # remove trailing period if it exists
+        if split_fraction[1][-1] == ".":
+            split_fraction[1] = split_fraction[1][:-1]
+
+        # after returning cases of just a whole number or decimal number and returning that, 
+        # we make sure all of our characters are valid 
+        has_only_valid_chars = all([i.isdigit() or i in {"-", "/", " ", "."} for i in fraction_str])
+        # has_only_valid_chars = all([i.isdigit() or i in {"-", "/", " "} for i in fraction_str])
 
         if not has_only_valid_chars:
             raise ValueError("Invalid input. Fraction string must contain only digits, hyphens, and a forward slash (possible invalid characters and/or periods?)")
 
         numerator = int(split_fraction[0])
         denominator = int(split_fraction[1])
+        # numerator = int(float(split_fraction[0])) # TODO: This is being tested out
+        # denominator = int(float(split_fraction[1]))
 
         is_negative = True if (numerator < 0 and denominator >= 0) or (numerator >= 0 and denominator < 0) else False
 
         # Convert the fraction to a decimal
         # return round(float(Fraction(numerator, denominator)), 3)
         decimal_value = round(float(Fraction(numerator, denominator)), 3)
 
@@ -94,90 +214,122 @@
             # decimal_value = decimal_value.replace("-", "")
         
         decimal_str = f"-{_make_int_or_float_str(str(decimal_value))}" if is_negative else _make_int_or_float_str(str(decimal_value))
 
         # return _make_int_or_float_str(str(round(float(Fraction(numerator, denominator)), 3)))
         return decimal_str
 
+# -----------------------------------------------------------------------------------------------
+# -----------------------------------------------------------------------------------------------
+
+# -----------------------------------------------------------------------------------------------
+# ---- Convert ALL fractions in a string to their decimal equivalent ----
+# -----------------------------------------------------------------------------------------------
+
+# TODO: Replace the _convert_fractions_to_decimals function defined in the IngredientSlicer class with this version
+# NOTE: This is the NEW implementation of _convert_fractions_to_decimals and specifically deals with each fraction type
+# NOTE: in a specific order and with a specific regex pattern to ensure the most accurate conversion
+def _convert_fractions_to_decimals(ingredient: str) -> list:
+        """
+        Find all fractions in the parsed ingredient string.
+        Args:
+            ingredient (str): The ingredient string to parse.
+        Returns:
+            list: A list of all fractions found in the ingredient string.
+        """
+
+        if not isinstance(ingredient, str):
+            raise ValueError("Invalid input. Ingredient must be a string.")
+
+        # use the predefined order of FRACTION_TYPE_ORDER to iterate through the patterns in 
+        # an order that will allow for the most accurate conversion (deals with decimal fractions first if they exist)
+        for pattern_key in _regex_patterns.FRACTION_TYPE_ORDER:
+        # for key, pattern in _regex_patterns.FRACTION_TYPE_MAP.items():
+        # # for key, pattern in list(_regex_patterns.FRACTION_TYPE_MAP.items())[::-1]:
+            pattern = _regex_patterns.FRACTION_TYPE_MAP[pattern_key]
+
+            # match_fraction = pattern.findall(ingredient)
+            match_fraction_iter = pattern.finditer(ingredient)
+
+            offset = 0
+
+            for match in match_fraction_iter:
+                match_string    = match.group()
+                start, end = match.start(), match.end()
+                modified_start = start + offset
+                modified_end = end + offset
+
+                fraction_decimal = _fraction_str_to_decimal(match_string)
+
+                ingredient = ingredient[:modified_start] + str(fraction_decimal) + ingredient[modified_end:]
+                offset += len(str(fraction_decimal)) - (end - start)
+
+        # # NOTE: trying the second loop implementation below will show why the order matters 
+        # for key, pattern in _regex_patterns.FRACTION_TYPE_MAP.items():
+        # # for key, pattern in list(_regex_patterns.FRACTION_TYPE_MAP.items())[::-1]: # NOTE: SHOWS WHY ORDER MATTERS
 
-# ingredient = "2 oz (56g / 1/8 package) dry"
+        return ingredient
 
-# def _convert_fractions_to_decimals(ingredient) -> None:
+# # NOTE: Old implementation of _convert_fractions_to_decimals 
+# # NOTE: (this is roughly what was used in the IngredientSlicer class, relies mainly on correct matching from the FRACTION_PATTERN)
+# def _convert_fractions_to_decimals2(ingredient: str) -> str:
 #     """
 #     Convert fractions in the parsed ingredient to their decimal equivalents.
 #     """
-#     ingredient = "large (7-1/4inch to 8-/1/2inch long)"
-#     FRACTION_PATTERN = re.compile(r'\d+\s*/\s*\d+')
-#     FRAC_PAT.findall(ingredient)
+
 #     # fraction_str = "1 to 1/2 cups, 2 and 5 animals, 2 2 / 4 cats, 1 and 1/22 cups water melon"
 #     matches = _regex_patterns.FRACTION_PATTERN.findall(ingredient)
-#     matches = FRAC_PAT.findall(ingredient)
 #     # matches = regex.FRACTION_PATTERN.findall(fraction_str)
 
 #     # Replace fractions with their decimal equivalents
 #     for match in matches:
 #         # print(f"Match: {match}")
 
 #         fraction_decimal = _fraction_str_to_decimal(match)
 #         # print(f"Fraction Decimal: {fraction_decimal}") if self.debug else None
 #         ingredient = ingredient.replace(match, str(fraction_decimal))
 
-# ingredient = "large (7-1/4inch to 8-/1/2inch long)"
-
-# regex_patterns = _regex_patterns.IngredientTools()
-
-# ingredient = "1-2 apples and 1- 45 orange slices (2)"
-# pattern = regex_patterns.QUANTITY_DASH_QUANTITY
-# replacement_function=None
-
-
-# BETWEEN_QUANTITY_AND_QUANTITY 
-# # _replace_and_with_hyphen
-# def _update_ranges(ingredient: str, pattern: re.Pattern, replacement_function=None) -> str:
-#         """Update the ranges in the ingredient string with the updated ranges
-#         Args:
-#             ingredient (str): The ingredient string to update
-#             pattern (re.Pattern): The pattern to use to find the ranges
-#             replacement_function (function, optional): A function to use to replace the matched ranges. Defaults to None.
-#         Returns:
-#             str: The updated ingredient string
-#         """
-        
-#         # pattern = IngredientSlicer.regex.QUANTITY_DASH_QUANTITY
-        
-#         matches = pattern.findall(ingredient)
-
-#         # matched_ranges = [match.split("-") for match in matches]
+#     return ingredient
 
-#         if replacement_function:
-#             # print(f"Replacement Function given")
-#             matched_ranges = [replacement_function(match).split("-") for match in matches]
-#         else:
-#             # print(f"No Replacement Function given")
-#             matched_ranges = [match.split("-") for match in matches]
+# TODO: USE these as a basis for tests
+# ingredient = "1 to 1/2 cups, 2 and 5 animals, 2 2 / 4 cats, 1 and 1/22 cups water melon"
+# _convert_fractions_to_decimals(ingredient)
+# _convert_fractions_to_decimals2(ingredient)
+
+# ingredient = "1 to 1/2 cups, 2 and 5 animals, 2 2 / 4 cats, 1 and 1/22 cups water melon, 2.0/4"
+# _convert_fractions_to_decimals(ingredient)
+# _convert_fractions_to_decimals2(ingredient)
+
+# -----------------------------------------------------------------------------------------------------------------------
+# ---- Force whitespaces between an number followed by a character or vice versa (i.e. "1cup" -> "1 cup") ----
+# -----------------------------------------------------------------------------------------------------------------------
 
-#         # print(f"Matched Ranges: \n > {matched_ranges}") if self.debug else None
+def _force_ws_between_numbers_and_chars(ingredient: str) -> str:
+    
+    """Forces spaces between numbers and units and between units and numbers.
+    End result is a string with a space between numbers and units and between units and numbers.
+    Examples:
+    "1cup" becomes "1 cup"
+    "cup1" becomes "cup 1" 
+    and ultimately "1cup" becomes "1 - cup" and "cup1" becomes "cup - 1"
+    """
 
-#         updated_ranges = [" - ".join([str(_fraction_str_to_decimal(i)) for i in match if i]) for match in matched_ranges]
-#         # updated_ranges = [" - ".join([str(int(i)) for i in match if i]) for match in matched_ranges]
-        
-#         # Create a dictionary to map the matched ranges to the updated ranges
-#         ranges_map = dict(zip(matches, updated_ranges))
+    NUMBERS_TO_LETTERS = re.compile(r"(\d)\-?([a-zA-Z])")  # 1cup
+    LETTERS_TO_NUMBERS = re.compile(r"([a-zA-Z])(\d)")     # cup1
+    LETTERS_DASH_NUMBERS = re.compile(r"([a-zA-Z])\-(\d)") # cup - 1
+
+    ingredient = NUMBERS_TO_LETTERS.sub(r"\1 \2", ingredient)
+    ingredient = LETTERS_TO_NUMBERS.sub(r"\1 \2", ingredient)
+    ingredient = LETTERS_DASH_NUMBERS.sub(r"\1 - \2", ingredient)
 
-#         # Replace the ranges in the original string with the updated ranges
-#         for original_range, updated_range in ranges_map.items():
-#             # print(f"Original Range: {original_range}")
-#             # print(f"Updated Range: {updated_range}")
-#             # if replacement_function:
-#             #     print(f"Replacement Function given")
-#             #     updated_range = replacement_function(updated_range)
-#             ingredient = ingredient.replace(original_range, updated_range)
-#             # print("\n") if self.debug else None
+    return ingredient
 
-#         return ingredient
+# -----------------------------------------------------------------------------------------------
+# ---- Standardize ranges (numbers separated by "-") so they all are the same form ----
+# -----------------------------------------------------------------------------------------------
 
 def _update_ranges(ingredient: str, pattern: re.Pattern) -> str:
         """Update the number ranges in the ingredient string to always have two numbers separated by a whitespace, then a hyphen, then another whitespace.
         Notes: Currently supports the following patterns in the IngredientTools class:
             - QUANTITY_DASH_QUANTITY
             - BETWEEN_QUANTITY_AND_QUANTITY
             - QUANTITY_TO_QUANTITY
@@ -185,60 +337,94 @@
         Args:
             ingredient (str): The ingredient string to update
             pattern (re.Pattern): The pattern to use to find the ranges
         Returns:
             str: The updated ingredient string with all possible ranges updated to always 
                 have 2 numbers separated by a whitespace, then a hyphen, then another whitespace.
         """
-        
+
         # # pattern = IngredientSlicer.regex.QUANTITY_DASH_QUANTITY
         # ingredient = "1-2 apples and 1- 45 orange slices between 4 and 5 lemons or 1 or 2 oranges and use 1 to 2 lemons"
         # pattern = _regex_patterns.QUANTITY_DASH_QUANTITY
         
-        # ingredient = '1 - 2 apples and 1 - 45 orange slices between 4 and 5 lemons or 1 or 2 oranges and use 1 to 2 lemons'
-        # pattern = _regex_patterns.BETWEEN_QUANTITY_AND_QUANTITY
-
-        # ingredient = '1 - 2 apples and 1 - 45 orange slices 4 - 5 lemons or 1 or 2 oranges and use 1 to 2 lemons'
-        # pattern = _regex_patterns.QUANTITY_TO_QUANTITY
-
-        # ingredient = '1 - 2 apples and 1 - 45 orange slices 4 - 5 lemons or 1 or 2 oranges and use 1 - 2 lemons'
-        # pattern = _regex_patterns.QUANTITY_OR_QUANTITY
-        
         matched_ranges_iter = pattern.finditer(ingredient)
         offset = 0
 
         for match in matched_ranges_iter:
             start, end = match.start(), match.end()
             modified_start = start + offset  # new start position
             modified_end = end + offset      # new end position
             match_string = match.group()
 
-            # print(f"Match String: '{match_string}'")
-            # print(f"Start: {start} | End: {end}")
-            # print(f"Modified Start: {modified_start} | Modified End: {modified_end}")
-            # print(f"Offset: {offset}")
-
             # In the match string, replace all instances of "and", "&", "to", and "or" with hyphens
             match_string = match_string.replace("and", "-") \
                 .replace("&", "-") \
                 .replace("to", "-") \
                 .replace("or", "-") \
                 .replace("between", "").strip()
-                
-            # print(f"Match AFTER replacement: '{match_string}'\n")
-            # print()
+            
             updated_range = " - ".join([str(_fraction_str_to_decimal(i)) for i in match_string.split("-")])
 
             ingredient = ingredient[:modified_start] + updated_range + ingredient[modified_end:]
 
             # # Update the offset for subsequent replacements
             offset += len(str(updated_range)) - (end - start)
             
         return ingredient
 
+# -----------------------------------------------------------------------------------------------
+# ---- Merge/Fix any ranges that are not really ranges (i.e. "4-1/2" -> "4.5")
+# -----------------------------------------------------------------------------------------------
+
+def _merge_misleading_ranges(ingredient:str) -> str:
+    """ Merge misleading ranges in the parsed ingredient (i.e. "4-1/2" is not a valid range, it should be "4.5" instead)"""
+
+    # Find all the ranges in the ingredient
+    range_iter = _regex_patterns.QUANTITY_DASH_QUANTITY_GROUPS.finditer(ingredient)
+
+    offset = 0
+
+    for match in range_iter:
+        match_string    = match.group()
+        start, end = match.start(), match.end()
+        modified_start = start + offset
+        modified_end = end + offset
+
+        left_range = match.group(1).strip()
+        right_range = match.group(2).strip()
+
+        first_number  = float(_fraction_str_to_decimal(left_range).strip())
+        second_number = float(_fraction_str_to_decimal(right_range).strip())
+
+        # If the second number is less than the first number, then the range is misleading
+        #  and the numbers should be merged (added if second number is a fraction)
+        if second_number < first_number:
+            # print(f"Fixing misleading range: {match_string} with ")
+            second_number_is_fraction = second_number < 1
+            multiply_or_add_str = "add" if second_number_is_fraction else "multiply"
+
+            # print(f"Second number is a fraction: {second_number_is_fraction}\n > '{multiply_or_add_str}' {first_number} and {second_number}") if self.debug else None
+
+            updated_value = f" {_make_int_or_float_str(str(first_number + second_number))} " if second_number_is_fraction else f" {_make_int_or_float_str(str(first_number * second_number))} "
+            # updated_value = f" {_make_int_or_float_str(str(first_number + second_number))} "
+            # print(f"Fixing misleading range: {match_string} with {updated_value}") if self.debug else None
+            
+            ingredient = ingredient[:modified_start] + updated_value + ingredient[modified_end:]
+            offset += len(updated_value) - (end - start)
+
+            # print(f"Ingredient after updating: {ingredient}") if self.debug else None
+
+    ingredient = ingredient.strip()
+
+    return ingredient
+
+# -----------------------------------------------------------------------------------------------
+# ---- Collapse ranges of numbers by averaging the values in the range ----
+# -----------------------------------------------------------------------------------------------
+
 def avg_ranges(ingredient: str) -> str:
     """
     Replace ranges of numbers with their average in the parsed ingredient.
     Examples:
     "1-2 oz" -> "1.5 oz"
     "1 - 2 ft" -> "1.5 ft"
     """
@@ -357,108 +543,76 @@
     Returns:
         str: The updated text with the hyphens removed from around the substring
     """
 
     # substrings_to_fix = ["to", "or", "and"]
     # substring = "to"
     # text = '1 to- 4.5 cups of sugar'
-    # text = '1 -to 4.5 cups of sugar'
-    # text = "1-to-three cups of tomato-juice"
-    # debug = True
 
     text = text.lower()
     substring = substring.lower().replace("-", "")
 
     substring_length = len(substring)
 
     L = 0
     substring_indices = []
     hypen_substrings = []
 
     for R in range(0, len(text)):
 
-        # print(f"L: {L}") if debug else None
-        # print(f"R: {R}") if debug else None
-        # print(f"text[L:R]: {text[L:R]}") if debug else None
         if R - L == substring_length:
             # print(f"Found window the size of substring!") if debug else None
             if text[L:R] == substring:
                 substring_indices.append([L, R])
                 
                 has_left_hyphen = False
                 has_right_hyphen = False
 
                 char_to_left = text[L - 1] if L - 1 >= 0 else None
                 char_to_right = text[R] if R < len(text) else None
                 
-
                 # character to the left or right of the substring is 
                 # a digit, hyphen, or whitespace or is at the beginning/end of the string
                 valid_left_char  = char_to_left is None or char_to_left.isdigit() or char_to_left == "-" or char_to_left == " "
                 valid_right_char = char_to_right is None or char_to_right.isdigit() or char_to_right == "-" or char_to_right == " "
 
                 # character to the left or right of the substring is NOT a digit, hyphen, or whitespace 
                 # (i.e. the matched substring is part of a larger word)
                 if not valid_left_char or not valid_right_char:
-                    # print(f"Substring is part of a larger word") if debug else None
-                    # print(f" - char_to_left: '{char_to_left}'") if debug else None
-                    # print(f" - char_to_right: '{char_to_right}'") if debug else None
-                    # print(f"Still increment L from {L} to {L + 1}") if debug else None
-                    # print() if debug else None
                     L += 1
                     continue
 
                 # look LEFT of the matched substring
                 GO_LEFT_INDEX = L - 1
 
                 # print(f"Try to go LEFT of '{substring}' substring") if debug else None
                 while GO_LEFT_INDEX >= 0 and (text[GO_LEFT_INDEX] == " " or text[GO_LEFT_INDEX] == "-"):
-                    # print(f"GO_LEFT_INDEX: '{GO_LEFT_INDEX}'") if debug else None
-                    # print(f" - text[GO_LEFT_INDEX]: '{text[GO_LEFT_INDEX]}'") if debug else None
                     if text[GO_LEFT_INDEX] == "-":
                         has_left_hyphen = True
                     GO_LEFT_INDEX -= 1
-                    # print(f" --> Ending text[GO_LEFT_INDEX]: '{text[GO_LEFT_INDEX]}'") if debug else None
                 
-                # print() if debug else None
-
                 # look RIGHT of the matched substring
-                # print(f"Try to go RIGHT of '{substring}' substring") if debug else None
 
                 GO_RIGHT_INDEX = R
-                # GO_RIGHT_INDEX = R + 1 # NOTE: Bug fix, Setting the GO_RIGHT_INDEX to R + 1 will skip the first character after the substring
 
                 while GO_RIGHT_INDEX < len(text) and (text[GO_RIGHT_INDEX] == " " or text[GO_RIGHT_INDEX] == "-"):
-                    # print(f"GO_RIGHT_INDEX: '{GO_RIGHT_INDEX}'") if debug else None
-                    # print(f" - text[GO_RIGHT_INDEX]: '{text[GO_RIGHT_INDEX]}'") if debug else None
+
                     if text[GO_RIGHT_INDEX] == "-":
                         has_right_hyphen = True
                     GO_RIGHT_INDEX += 1
-                    # print(f" --> Ending text[GO_RIGHT_INDEX]: '{text[GO_RIGHT_INDEX]}'") if debug else None
 
                 look_around_string = text[GO_LEFT_INDEX+1:GO_RIGHT_INDEX]
 
                 if has_left_hyphen or has_right_hyphen:
                     hypen_substrings.append(look_around_string)
-                    # print(f"Added '{look_around_string}' to hypen_substrings:\n > '{hypen_substrings}'") if debug else None
-                # print(f"FINAL --> GO_LEFT_INDEX: {GO_LEFT_INDEX} --> has LEFT hypen: {has_left_hyphen}") if debug else None
-                # print(f"FINAL --> GO_RIGHT_INDEX: {GO_RIGHT_INDEX} --> has RIGHT hypen: {has_right_hyphen}") if debug else None
-                # print(f"Final substring: '{look_around_string}'") if debug else None
-
-            # print(f"Incrementing L from {L} to {L + 1}") if debug else None
             L += 1
-        # print(f"----" * 5) if debug else None
-        # print() if debug else None
-    
-    # print(f"hypen_substrings: {hypen_substrings}") if debug else None
-    
+
     for hyphen_substring in hypen_substrings:
         replacement_string = f" {hyphen_substring.replace('-', '').replace(' ', '')} " 
         text = text.replace(hyphen_substring, replacement_string) 
-        # print(f"Replacing '{hyphen_substring}' in 'text' with '{replacement_string}'\n") if debug else None
 
     text = text.strip()
 
     return text
 
 # -----------------------------------------------------------------------------------------------
 # ---- Set of simple replacement functions for replacing words in strings ----
@@ -657,38 +811,35 @@
         str_after_approx_match = input_string[end:] # string after the approximate match
 
         # _regex_patterns.ALL_NUMBERS.findall(after_approx_match)
         nearest_number_search = _regex_patterns.ALL_NUMBERS.search(str_after_approx_match) # search for the nearest number after the approximate string
 
         if not nearest_number_search:
             # print(f"No number found after approximate match")
-            # print()
             continue
 
         closest_number = nearest_number_search.group() # the actual matching number string
         # print(f"Closest Number: '{closest_number}'")
         current_result.append(closest_number) # add the number to the result
         
         # string after the number 
         str_after_number_match = str_after_approx_match[nearest_number_search.end():] # string after the number match
 
         nearest_unit_search = _regex_patterns.UNITS_PATTERN.search(str_after_number_match) # search for the nearest unit after the number
 
         if not nearest_unit_search: # if we don't find a unit after the number, we skip this triplet
             # print(f"No unit found after approximate match")
-            # print()
             continue
 
         closest_unit = nearest_unit_search.group() # the actual matching unit string
         # print(f"Closest Unit: '{closest_unit}'")
 
         current_result.append(closest_unit) # add the unit to the result
         # approximate_triplets.append(current_result) # add the triplet to the list of approximate triplets
         approximate_triplets.append(tuple(current_result)) # add the triplet to the list of approximate triplets
-        # print()
     
 
     # look for trailing approximate strings
     trailing_approx_strings = _regex_patterns.APPROXIMATE_STRINGS_PATTERN.findall(input_string)
 
     # if we didn't get any [approximate, quantity, unit] triplets, but we did get a trailing approximate strings
     # check the string again for quantity unit pairs and 
@@ -899,14 +1050,110 @@
             # --> Modified start/end match positions: {modified_start}-{modified_end}
             # ---> Modified string: {string}""")
         
         string = string.strip()
 
         return string
 
+def _find_and_replace_casual_quantities(ingredient: str) -> str:
+    """
+    Find and replace matches of CASUAL_QUANTITIES_PATTERN with the key from the CASUAL_QUANTITIES dictionary
+    """
+
+    offset = 0
+    pattern_iter = _regex_patterns.CASUAL_QUANTITIES_PATTERN.finditer(ingredient)
+
+    for match in pattern_iter:
+        match_string    = match.group()
+
+        # Get the start and end of the match and the modified start and end positions given the offset
+        start, end = match.start(), match.end()
+        modified_start = start + offset
+        modified_end = end + offset
+
+        replacement_str = _constants.CASUAL_QUANTITIES[match_string] 
+
+        # Construct the modified string with the replacement applied
+        ingredient = ingredient[:modified_start] + str(replacement_str) + ingredient[modified_end:]
+
+        # Update the offset for subsequent removals 
+        offset += len(str(replacement_str)) - (end - start)
+
+    return ingredient
+
+def _find_and_replace_prefixed_number_words(ingredient: str) -> str:
+    """ Replace prefixed number words with their corresponding numerical values in the parsed ingredient 
+    Strings like "twenty five" are replaced with "25", or "thirty-two" is replaced with "32"
+
+    """
+    number_words_iter = _regex_patterns.PREFIXED_NUMBER_WORDS_GROUPS.finditer(ingredient)
+
+    offset = 0
+
+    for match in number_words_iter:
+        
+        if match:
+            start, end = match.start(), match.end()
+
+            match_string = match.group()
+            prefix_word = match.group(1)
+            number_word = match.group(2)
+            
+            prefix_value = _constants.NUMBER_PREFIX_WORDS.get(prefix_word, 0)
+            number_value = _constants.NUMBER_WORDS.get(number_word, 0)
+
+            combined_value = prefix_value + number_value
+
+            # Calculate the start and end positions in the modified string
+            modified_start = start + offset
+            modified_end = end + offset
+
+            # Construct the modified string with the replacement applied
+            ingredient = ingredient[:modified_start] + str(combined_value) + ingredient[modified_end:]
+            # ingredient = ingredient[:modified_start] + str(combined_value) + ingredient[modified_end:]
+
+            # Update the offset for subsequent replacements
+            offset += len(str(combined_value)) - (end - start)
+
+            # print(f"""
+            # Match string: {match_string}
+            # - Prefix word: {prefix_word}
+            # - Number word: {number_word}
+            # Prefix value ({prefix_value}) + Number value ({number_value}) = Combined value ({combined_value})
+            # > {prefix_value} + {number_value} = {combined_value}
+            # -> Match: {match_string} at positions {start}-{end}
+            # ---> Modified ingredient: {self.standardized_ingredient}""") if self.debug else None
+
+    return ingredient
+
+def _find_and_replace_number_words(ingredient:str) -> str:
+    """
+    Replace number words with their corresponding numerical values in the parsed ingredient.
+    """
+
+    # print("Parsing number words")
+    for word, regex_data in _regex_patterns.NUMBER_WORDS_MAP.items():
+        pattern = regex_data[1]
+        # print statement if word is found in ingredient and replaced
+        if pattern.search(ingredient):
+            ingredient = pattern.sub(regex_data[0], ingredient)
+    
+    return ingredient
+
+def _clean_html_and_unicode(ingredient: str) -> str:
+    """Unescape fractions from HTML code coded fractions to unicode fractions."""
+
+    # Unescape HTML
+    ingredient = unescape(ingredient)
+
+    # Replace unicode fractions with their decimal equivalents
+    for unicode_fraction, decimal_fraction in _constants.UNICODE_FRACTIONS.items():
+        ingredient = ingredient.replace(unicode_fraction, f" {decimal_fraction}")
+
+    return ingredient
 
 # def replace_number_followed_by_inch_symbol(ingredient: str) -> str:
 #     """Replace numbers followed by the inch symbol with the word 'inch' in the ingredient string.
 #     Args:
 #         ingredient (str): The ingredient string to parse.
 #     Returns:
 #         str: The updated ingredient string with numbers followed by the inch symbol replaced with the word 'inch'.
@@ -1029,30 +1276,19 @@
         # quantities from second quantity/unit pair
         quantity2 = match.group(3)
         unit2     = match.group(4)
 
         unit1_is_dimension = unit1 in _constants.DIMENSION_UNITS_SET
         unit2_is_dimension = unit2 in _constants.DIMENSION_UNITS_SET
 
-        # print(f"Original String: {original_string}")
-        # print("First Quantity/Unit Pair")
-        # print(f"- Quantity 1: {quantity1}")
-        # print(f"- Unit 1: {unit1}")
-        # print(f" >> '{unit1}' is dimension? {unit1_is_dimension}")
-        # print("Second Quantity/Unit Pair")
-        # print(f"- Quantity 2: {quantity2}")
-        # print(f"- Unit 2: {unit2}")
-        # print(f" >> '{unit2}' is dimension? {unit2_is_dimension}")
-
         if unit1_is_dimension and unit2_is_dimension:
             # print(f"Both units are dimensions")
             # ingredient = _find_and_remove(ingredient, pattern)
             dimension_units.append(original_string)
             ingredient = ingredient.replace(original_string, "")
-        # print()
 
     return [ingredient, dimension_units]
 
 def _split_single_unit_dimension_ranges(ingredient: str) -> list[str]:
     """Split an ingredient string by any quantity dimension unit separated by an 'by' character.
     (i.e. "2 steaks, 3 inches by 4 inches thick" -> ("2 steaks, thick", "3 inches by 4 inches")
     
@@ -1078,22 +1314,14 @@
         # quantities from second quantity/unit pair
         quantity2 = match.group(2)
         unit2     = match.group(3)
 
         # unit1_is_dimension = unit1 in _constants.DIMENSION_UNITS_SET
         unit2_is_dimension = unit2 in _constants.DIMENSION_UNITS_SET
 
-        # print(f"Original String: {original_string}")
-        # print("First Quantity Pair")
-        # print(f"- Quantity 1: {quantity1}")
-        # print("Second Quantity/Unit Pair")
-        # print(f"- Quantity 2: {quantity2}")
-        # print(f"- Unit 2: {unit2}")
-        # print(f" >> '{unit2}' is dimension? {unit2_is_dimension}")
-
         if unit2_is_dimension:
             # print(f"---> Second unit is dimension!!!")
             # ingredient = _find_and_remove(ingredient, pattern)
             dimension_units.append(original_string)
             ingredient = ingredient.replace(original_string, "")
 
         # print()
@@ -1113,22 +1341,14 @@
 
     dimensions = dimension_ranges1 + dimension_ranges2 + dimensions_with_number
 
     ingredient = _remove_extra_whitespaces(ingredient)
 
     return [ingredient, dimensions]
 
-# ingredient = "2 steaks, 3 inches x 4 inches thick"
-# ingredient = "2 steaks, 3 inches x 4 inches thick"
-# ingredient = "2 steaks, 3 cm x 4 inches thick"
-# ingredient = "2 steaks, 3 cm x 4 inches thick"
-# ingredient = "2 steaks, (3 cm x 4 inches) thick"
-# ingredient = "2 steaks, (3 cm by 4 inches) thick"
-# ingredient = "2 steaks, (4 oz, but 3 cm x 4 inches thick), or cut 1 inch slices, (1 x 2 inch)"
-
 def _remove_x_separators(ingredient: str) -> str:
     """
     Remove "x" separators from the ingredient string and replace with whitespace
     Examples:
         >>> _removed_x_separators("1x2 cups")
         '1 2 cups'
         >>> _remove_x_separators("5 x cartons of eggs")
@@ -1180,19 +1400,451 @@
 
         # if the units are the same, replace the original string with the quantities and units
         if unit1 == unit2:
             ingredient = ingredient.replace(original_string, f"{quantity1} - {quantity2} {unit1}")
 
     return ingredient 
 
-# QUANTITY_UNIT_X_QUANTITY_UNIT
-# QUANTITY_UNIT_BY_QUANTITY_UNIT
 
+def _get_gram_weight(food:str, quantity:str, unit:str, method:str = "levenshtein") -> dict:
+
+    """ Get the gram weight of a given quantity of food item.
+    Args:
+        food (str): The food item to convert.
+        quantity (Union[str, int, float]): The quantity of the food item.
+        unit (str): The unit of measurement for the quantity.
+    Returns:
+        dict: A dictionary containing the gram weight, maximum gram weight, and minimum gram weight.
+    """
+    # food = "olive oil"
+    # quantity = "1"
+    # unit = "teaspoon"
+
+    if not unit:
+        return {
+            "gram_weight" : None,
+            "min_gram_weight" : None,
+            "max_gram_weight" : None
+        }
+
+    if quantity is None:
+        quantity = "1"
+
+    # ValueError checks
+    if not isinstance(food, str):
+        raise ValueError("'food' must be a string")
+
+    if not isinstance(method, str):
+        raise ValueError("'method' must be a string")
+
+    method = method.lower()
+
+    if method not in ["levenshtein", "jaccard", "dice"]:
+        raise ValueError("Invalid 'method'. Options are 'levenshtein', 'jaccard', or 'dice'.")
+    
+    if not isinstance(quantity, (str, int, float)):
+        raise ValueError("'quantity' must be a string, integer, or float")
+    
+    if not isinstance(unit, str):
+        raise ValueError("'unit' must be a string")
+
+    quantity = float(quantity)
+    
+    gram_weight     = None
+    min_gram_weight = None
+    max_gram_weight = None
+    
+    unit = unit.lower()
+
+    # weight check
+    if unit in _constants.WEIGHT_UNIT_TO_STANDARD_WEIGHT_UNIT:
+        gram_weight = _convert_weights_to_grams(quantity, unit)
+
+        return {
+            "gram_weight" : str(round(gram_weight, 2)) if gram_weight else None,
+            "min_gram_weight" : str(round(min_gram_weight, 2)) if min_gram_weight else None,
+            "max_gram_weight" : str(round(max_gram_weight, 2)) if max_gram_weight else None
+            }
+    
+    # volume check
+    if unit in _constants.VOLUME_UNIT_TO_STANDARD_VOLUME_UNIT:
+        gram_values_map = _convert_volume_to_grams(food, quantity, unit, method)  
+
+        return {
+            "gram_weight" : str(round(gram_values_map["gram_weight"], 2)) if gram_values_map["gram_weight"] else None,
+            "min_gram_weight" : str(round(gram_values_map["min_gram_weight"], 2)) if gram_values_map["min_gram_weight"] else None,
+            "max_gram_weight" : str(round(gram_values_map["max_gram_weight"], 2)) if gram_values_map["max_gram_weight"] else None
+            }
+
+    # if the given unit was not a weight or volume unit, return None for all of the gram weights
+    return {
+        "gram_weight" : str(round(gram_weight, 2)) if gram_weight else None,
+        "min_gram_weight" : str(round(min_gram_weight, 2)) if min_gram_weight else None,
+        "max_gram_weight" : str(round(max_gram_weight, 2)) if max_gram_weight else None
+        }
+    
+
+def _convert_weights_to_grams(quantity: Union[str, int, float], unit:str) -> str:
+    """
+    Get the weight of a given quantity of units in grams
+    If the given unit is not in the set of standard weight units (e.g. "pounds", "ounces", "grams", "kilograms", "milligrams", "micrograms") or an abbreviated form,
+    the function returns None.
+    Args:
+        quantity (Union[str, int, float]): The quantity of the food item.
+        unit (str): The unit of measurement for the quantity.
+    Returns:
+        str: The weight of the quantity in grams.
+    """
+
+    if not isinstance(quantity, (str, int, float)):
+        raise ValueError("'quantity' must be a string, integer, or float")
+    
+    if not isinstance(unit, str):
+        raise ValueError("'unit' must be a string")
+    
+    if isinstance(quantity, str):
+        quantity = float(quantity)
+
+    if unit in _constants.WEIGHT_UNIT_TO_STANDARD_WEIGHT_UNIT:
+        
+        standard_unit     = _constants.WEIGHT_UNIT_TO_STANDARD_WEIGHT_UNIT[unit]
+        conversion_factor = _constants.GRAM_CONVERSION_FACTORS[standard_unit]
+
+        gram_weight = quantity * conversion_factor
+
+        return gram_weight
+    
+    return None
+
+
+def _convert_volumes_to_milliliters(quantity: Union[str, int, float], unit:str) -> str:
+    """
+    Get the volume of a given quantity of units in milliliters
+    If the given unit is not in the set of standard volume units (e.g. "teaspoons", "tablespoons", 
+    "fluid ounces", "cups", "pints", "quarts", "gallons", "milliliters", "liters") or an abbreviated form, 
+    then the function returns None.
+    Args:
+        quantity (Union[str, int, float]): The quantity of the food item. Can be a string, float, or integer (e.g. "1.0", 1, 1.0)
+        unit (str): The unit of measurement for the quantity. (e.g. "cups", "teaspoons", "tablespoons", "fluid ounces", "milliliters", "liters")
+    Returns:
+        str: The volume of the quantity in milliliters.
+
+    """
+
+    if not isinstance(quantity, (str, int, float)):
+        raise ValueError("'quantity' must be a string, integer, or float")
+    
+    if not isinstance(unit, str):
+        raise ValueError("'unit' must be a string")
+    
+    if isinstance(quantity, str):
+        quantity = float(quantity)
+
+    if unit in _constants.VOLUME_UNIT_TO_STANDARD_VOLUME_UNIT:
+        
+        standard_unit     = _constants.VOLUME_UNIT_TO_STANDARD_VOLUME_UNIT[unit]
+        conversion_factor = _constants.MILLILITER_CONVERSION_FACTORS[standard_unit]
+
+        milliliter_volume = quantity * conversion_factor
+
+        return milliliter_volume
+    
+    return None
+
+def _convert_volume_to_grams(food: str, quantity: Union[str, int, float], unit: str, method:str = "levenshtein") -> dict:
+
+    """
+    Convert a volume measurement to a weight measurement in grams.
+    Args:
+        food (str): The food item to convert.
+        quantity (Union[str, int, float]): The quantity of the food item.
+        unit (str): The unit of measurement for the quantity.
+        method (str): The method to use for fuzzy string matching. Options are "levenshtein", "jaccard", or "dice". Defaults to "levenshtein".
+    Returns:
+        dict: A dictionary containing the gram weight, maximum gram weight, and minimum gram weight.
+    """
+
+    # ############################################################
+    # ingredient = "1 1/2 cups of all purpose almond flour, grounded"
+    # method = "jaccard"
+    # method = "levenshtein"
+    # ############################################################
+
+    if not isinstance(method, str):
+        raise ValueError("'method' must be a string")
+    
+    method = method.lower()
+
+    if method not in ["levenshtein", "jaccard", "dice"]:
+        raise ValueError("Invalid 'method'. Options are 'levenshtein', 'jaccard', or 'dice'.")
+
+    fuzzy_matcher =  _get_fuzzy_matcher(method)
+
+    milliliter_quantity = _convert_volumes_to_milliliters(quantity, unit)
+
+    # print(f"Looking for categories and densities for:\n > '{food}'")
+    # no_match_string = "no match found in FOOD_CATALOG"
+    
+    # try to get the food groups for the given food...
+    food_groups = _constants.FOOD_CATALOG.get(food, None)
+    # food_groups = _constants.FOOD_CATALOG.get(food, no_match_string)
+
+    # print(f"Categories for '{food}':\n--> '{food_groups}'")
+
+    if not food_groups:
+        # print(f"Going for the layup classification for '{food}'...")
+        food_group = _check_food_for_easy_categorization(food)
+        # print(f"Easily classified as '{food_group}'")
+        if food_group:
+            # print(f"Setting previously None 'food_groups' to '{[food_group, food_group]}'")
+            food_groups = [food_group, food_group]
+
+    # print(f"Categories for '{food}':\n--> '{food_groups}'")
+            
+    # Case when we get a real match in the FOOD_CATALOG, 
+    # then we can just use the corresponding densities for the matched food
+    if food_groups:
+    # if food_groups != no_match_string:
+        # print(f"Found exact category match:\n '{food}' >>> '{food_groups}'")
+        primary_category, secondary_category = food_groups
+
+        # try to get the density values for the given primary category food group, 
+        # if that fails try to get the density values for the secondary category food group
+        # and all else fails, use the default density map
+        if primary_category in _constants.FOOD_DENSITY_BY_GROUP:
+            density_map = _constants.FOOD_DENSITY_BY_GROUP.get(primary_category, _constants.DEFAULT_DENSITY_MAP)
+        elif secondary_category in _constants.FOOD_DENSITY_BY_GROUP:
+            density_map = _constants.FOOD_DENSITY_BY_GROUP.get(secondary_category, _constants.DEFAULT_DENSITY_MAP)
+        else:
+            density_map = _constants.DEFAULT_DENSITY_MAP
+            
+        # try to get the density values for the given primary category food group, 
+
+        # print(f"Using density values for category:\n > '{density_map['category']}'")
+
+        density     = density_map.get("density_g_per_ml", 1)
+        min_density = density_map.get("min_density_g_per_ml", 0.9)
+        max_density = density_map.get("max_density_g_per_ml", 1.1)
+
+        # if primary_density and secondary_density:
+            # print(" > Both densities are available")
+        # print(f"Primary density: {primary_density}\nSecondary density: {secondary_density}")
+
+        gram_weight     = milliliter_quantity * density
+        min_gram_weight = milliliter_quantity * min_density
+        max_gram_weight = milliliter_quantity * max_density
+        
+        return {
+            "gram_weight" : gram_weight, 
+            "min_gram_weight" : min_gram_weight,
+            "max_gram_weight" : max_gram_weight
+            }
+
+    # However, if we do NOT get a match in the FOOD_CATALOG, we will have to do a fuzzy match between our given food
+    # and all of the foods and determine the closet match and use the density of that food group (FOOD_DENSITY_BY_GROUP)
+
+    similarity_scores = {}
+    top_scoring_foods = {}
+
+    for category in _constants.FOOD_DENSITY_BY_GROUP:
+        food_set = _constants.FOODS_BY_CATEGORY[category]
+        # print(f"Category: {category}\nFood set: {food_set}")
+
+        # find the closeness from the given food to each food in the current category
+        # and extract that food and its value, to stash the top matched food and its score for each category
+        scores =  {i: round(fuzzy_matcher(food, i), 2) for i in food_set}
+        top_score_key = max(scores, key=scores.get) 
+        top_score_value = scores[top_score_key] if top_score_key else 0
+        
+        # NOTE: keep track of the food with the highest similarity score for each category
+        top_scoring_foods[category] = [top_score_key, top_score_value]
+        # print(f" - Top score key/value:\n ----> '{top_score_key} ({scores[top_score_key]})'\n")
+
+        max_similarity = max([round(fuzzy_matcher(food, i), 2) for i in food_set])
+        # max_similarity = max([round(_utils.score_sentence_similarity(food, i), 2) for i in food_set])
+
+        similarity_scores[category] = max_similarity
+        
+    # get the key that has the highest similarity score in the dictionary of similarity scores
+    best_category_match = max(similarity_scores, key=similarity_scores.get)
+
+    # print(f"Key with max similarity score:\n > '{best_category_match}'")
+    # print(f"Top score: {similarity_scores[best_category_match]}")
+    # print(f"Top scoring food:\n > {top_scoring_foods[best_category_match]}")
+
+    density = 1
+    min_density = 0.9
+    max_density = 1.1
+
+    try: 
+        # print(f"Successful best effort category match: \n '{food}' >>> '{best_category_match}'")
+        gram_map    = _constants.FOOD_DENSITY_BY_GROUP[best_category_match]
+        density     = gram_map["density_g_per_ml"]
+        max_density = gram_map["max_density_g_per_ml"]
+        min_density = gram_map["min_density_g_per_ml"]
+        # print(f"Using density value of:\n > '{density} g/ml'")
+    except:
+        warnings.warn(f"No good food denstity match was found, defaulting to the density of water (1 g/ml)")
+
+    # # NOTE: old way of catching if no good match was made or the matched category does not exist / density is <= 0
+    # if ((best_category_match not in _constants.FOOD_DENSITY_BY_GROUP) or \
+    #     (best_category_match in _constants.FOOD_DENSITY_BY_GROUP and _constants.FOOD_DENSITY_BY_GROUP[best_category_match]['density_g_per_ml'] <= 0)
+    #     ):
+    #     density = 1
+    # else:
+    #     density = _constants.FOOD_DENSITY_BY_GROUP[best_category_match]["density_g_per_ml"]
+        
+    gram_weight     = density * milliliter_quantity
+    max_gram_weight = max_density * milliliter_quantity
+    min_gram_weight = min_density * milliliter_quantity
+
+    return {
+        "gram_weight" : gram_weight, 
+        "min_gram_weight" : min_gram_weight,
+        "max_gram_weight" : max_gram_weight, 
+        }
+
+# # ingredient = "1 1/2 cups of all purpose almond flour, grounded"
+# ingredient = "1 1/2 cups of chick nuggets, grounded"
+
+# # ingredient = "1 1/2 cups of chicken nuggets, grounded"
+# # ingredient = "1 1/2 cups of White whole wheat flour, grounded"
+
+# slicer = IngredientSlicer(ingredient)
+# food = slicer.food
+# # food = "112"
+# unit = slicer.standardized_unit if slicer.standardized_unit else slicer.unit
+# quantity = slicer.quantity
+
+def _check_food_for_easy_categorization(food:str) -> str:
+
+    """Check if the food can be easily categorized based on the food name.
+    If it can, return the category. Otherwise, return just return None.
+    Args:
+        food: str: The name of the food to categorize.
+    Returns:
+        str: The category of the food if it can be easily categorized. Otherwise, None.
+    """
+
+    # food = "whole  wheat  oaty flour  oil"
+    # food = "toats vdf asvfgf df"
+
+    # clean up tasks
+    food = food.lower().strip()
+    food = _remove_extra_whitespaces(food)
+    food = food.split()
 
+    matched_categories = []
+    for word in food:
+        match = _constants.INDICATOR_STRINGS_MAP.get(word, None)
+        if match:
+            matched_categories.append(match)
 
+    # if we have multiple matches, return the last one because I think its more likely that the last match indicates the category
+    # TODO: this might be stupid but made sense to me ("olive oil", "brown sugar", "white sugar", the indicator word seems to come last-ish)
+    # TODO: Regardless, its pretty unlikely youll get multiple matches anyway
+    category = matched_categories[-1] if matched_categories else None
+
+    return category
+
+def _get_fuzzy_matcher(method: str) -> Callable:
+    """
+    Get the fuzzy string matching function based on the given method.
+    Internal conveniance function
+    Args:
+        method (str): The method to use for fuzzy string matching. Options are "levenshtein", "jaccard", or "dice".
+    Returns:
+        Callable: The fuzzy string matching function.
+    """
+
+    method = method.lower()
+
+    if method not in ["levenshtein", "jaccard", "dice"]:
+        raise ValueError("Invalid 'method'. Options are 'levenshtein', 'jaccard', or 'dice'.")
+
+    fuzzy_matchers = {
+        "levenshtein" : _levenshtein_similarity,
+        "jaccard" : _jaccard_similarity,
+        "dice" : _dice_coeff_similarity
+        }
+
+    return fuzzy_matchers[method]
+
+# _convert_volume_to_grams(food, quantity, unit)
+def _levenshtein_dist(str1, str2):
+    # set up a matrix with the dimensions of the two strings
+    matrix = [[0] * (len(str2) + 1) for _ in range(len(str1) + 1)]
+    
+    # initialize the matrix with the values of the first row and column
+    for i in range(len(str1) + 1):
+        matrix[i][0] = i
+    for j in range(len(str2) + 1):
+        matrix[0][j] = j
+
+    for i in range(1, len(str1) + 1):
+        for j in range(1, len(str2) + 1):
+            substitute = 0 if str1[i - 1] == str2[j - 1] else 1
+            matrix[i][j] = min(
+                matrix[i - 1][j] + 1,              # delete
+                matrix[i][j - 1] + 1,               # isert 
+                matrix[i - 1][j - 1] + substitute  # substitute
+            )
+
+    # levenstein distance == bottom right corner of matrix
+    return matrix[len(str1)][len(str2)]
+
+def _levenshtein_similarity(str1, str2):
+    distance = _levenshtein_dist(str1, str2)
+    max_len = max(len(str1), len(str2))
+    return 1 - (distance / max_len)
+
+def _jaccard_similarity(str1, str2):
+    set1 = set(str1)
+    set2 = set(str2)
+    intersection = len(set1.intersection(set2))
+    union = len(set1.union(set2))
+    return intersection / union
+
+# Credit: to recipe_scrapers (hhruvs) GitHub repository for the following code
+def _dice_coeff_similarity(first: str, second: str) -> float:
+    """Calculate Dice coefficient for two strings.
+
+    The dice coefficient is a measure of similarity determined by calculating
+    the proportion of shared bigrams.
+
+    Parameters
+    ----------
+    first : str
+        First string
+    second : str
+        Second string
+
+    Returns
+    -------
+    float
+        Similarity score between 0 and 1.
+        0 means the two strings do not share any bigrams.
+        1 means the two strings are identical.
+    """
+
+    if first == second:
+        # Indentical sentences have maximum score of 1
+        return 1
+
+    if len(first) < 2 or len(second) < 2:
+        # If either sentence has 0 or 1 character we can't generate bigrams,
+        # so the score is 0
+        return 0
+
+    first_bigrams = {first[i : i + 2] for i in range(len(first) - 1)}
+    second_bigrams = {second[i : i + 2] for i in range(len(second) - 1)}
+
+    intersection = first_bigrams & second_bigrams
+
+    return 2.0 * len(intersection) / (len(first_bigrams) + len(second_bigrams))
 
 # def _split_dimension_unit_x_ranges(ingredient: str) -> tuple[str]:
 #     """Split an ingredient string by any quantity dimension unit separated by an 'x' character.
 #     (i.e. "2 steaks, 3 inches x 4 inches thick" -> ("2 steaks, thick", "3 inches x 4 inches")
 
 #     Args:
 #         ingredient (str): The ingredient string to parse.
@@ -1459,7 +2111,80 @@
 #             replacement_str = match_string.replace(key, "inch")
 
 #             # Construct the modified string with the replacement applied
 #             ingredient = ingredient[:modified_start] + str(replacement_str) + ingredient[modified_end:]
 
 #             offset += len(str(replacement_str)) - (end - start)
 #     return
+
+
+# def _update_ranges(ingredient: str, pattern: re.Pattern, replacement_function=None) -> str:
+#         """Update the ranges in the ingredient string with the updated ranges
+#         Args:
+#             ingredient (str): The ingredient string to update
+#             pattern (re.Pattern): The pattern to use to find the ranges
+#             replacement_function (function, optional): A function to use to replace the matched ranges. Defaults to None.
+#         Returns:
+#             str: The updated ingredient string
+#         """
+        
+#         # pattern = IngredientSlicer.regex.QUANTITY_DASH_QUANTITY
+        
+#         matches = pattern.findall(ingredient)
+
+#         # matched_ranges = [match.split("-") for match in matches]
+
+#         if replacement_function:
+#             # print(f"Replacement Function given")
+#             matched_ranges = [replacement_function(match).split("-") for match in matches]
+#         else:
+#             # print(f"No Replacement Function given")
+#             matched_ranges = [match.split("-") for match in matches]
+
+#         # print(f"Matched Ranges: \n > {matched_ranges}") if self.debug else None
+
+#         updated_ranges = [" - ".join([str(_fraction_str_to_decimal(i)) for i in match if i]) for match in matched_ranges]
+#         # updated_ranges = [" - ".join([str(int(i)) for i in match if i]) for match in matched_ranges]
+        
+#         # Create a dictionary to map the matched ranges to the updated ranges
+#         ranges_map = dict(zip(matches, updated_ranges))
+
+#         # Replace the ranges in the original string with the updated ranges
+#         for original_range, updated_range in ranges_map.items():
+#             # print(f"Original Range: {original_range}")
+#             # print(f"Updated Range: {updated_range}")
+#             # if replacement_function:
+#             #     print(f"Replacement Function given")
+#             #     updated_range = replacement_function(updated_range)
+#             ingredient = ingredient.replace(original_range, updated_range)
+#             # print("\n") if self.debug else None
+
+#         return ingredient
+# def _update_ranges(self, ingredient: str, pattern: re.Pattern, replacement_function=None) -> str:
+#     """Update the ranges in the ingredient string with the updated ranges
+#     Args:
+#         ingredient (str): The ingredient string to update
+#         pattern (re.Pattern): The pattern to use to find the ranges
+#         replacement_function (function, optional): A function to use to replace the matched ranges. Defaults to None.
+#     Returns:
+#         str: The updated ingredient string
+#     """
+    
+#     matches = pattern.findall(ingredient)
+#     # matched_ranges = [match.split("-") for match in matches]
+
+#     if replacement_function:
+#         matched_ranges = [replacement_function(match).split("-") for match in matches]
+#     else:
+#         matched_ranges = [match.split("-") for match in matches]
+
+#     updated_ranges = [" - ".join([str(_utils._fraction_str_to_decimal(i)) for i in match if i]) for match in matched_ranges]
+#     # updated_ranges = [" - ".join([str(int(i)) for i in match if i]) for match in matched_ranges]
+    
+#     # Create a dictionary to map the matched ranges to the updated ranges
+#     ranges_map = dict(zip(matches, updated_ranges))
+
+#     # Replace the ranges in the original string with the updated ranges
+#     for original_range, updated_range in ranges_map.items():
+#         ingredient = ingredient.replace(original_range, updated_range)
+
+#     return ingredient
```

### Comparing `ingredient_slicer-0.0.81/ingredient_slicer.egg-info/SOURCES.txt` & `ingredient_slicer-0.0.83/ingredient_slicer.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -14,24 +14,29 @@
 ingredient_slicer.egg-info/dependency_links.txt
 ingredient_slicer.egg-info/requires.txt
 ingredient_slicer.egg-info/top_level.txt
 tests/__init__.py
 tests/test_avg_ranges.py
 tests/test_casual_ingredients.py
 tests/test_clean_hyphen_padded_substrings.py
+tests/test_convert_fractions_to_decimals.py
+tests/test_convert_volumes_to_milliliters.py
 tests/test_duplicate_unit_ranges.py
 tests/test_extract_dimensions.py
 tests/test_extract_quantities_utils.py
 tests/test_find_and_remove.py
 tests/test_find_and_remove_hyphen_substrings.py
 tests/test_fraction_str_to_decimal.py
+tests/test_get_gram_weight.py
 tests/test_ingredient_slicer.py
 tests/test_ingredient_slicer_dimensions.py
+tests/test_ingredient_slicer_fraction_conversions.py
 tests/test_ingredient_slicer_x_separators.py
 tests/test_make_int_or_float_str.py
+tests/test_merge_misleading_ranges.py
 tests/test_merge_numbers.py
 tests/test_number_ranges.py
 tests/test_number_ranges_separated_by_words.py
 tests/test_numbers_with_inch_symbols.py
 tests/test_parenthesis.py
 tests/test_parenthesis_utils.py
 tests/test_percentages.py
```

### Comparing `ingredient_slicer-0.0.81/pyproject.toml` & `ingredient_slicer-0.0.83/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 requires = ["setuptools", "setuptools-scm"]
 
 [project]
 name = "ingredient_slicer"
 authors = [
   {name = "Angus Watters", email = "anguswatters@gmail.com"},
 ]
-version = "0.0.81"
-description = "Parse quantities, units, and (sometimes) foods from recipe ingredients into structured data"
+version = "0.0.83"
+description = "Parses unstructured recipe ingredient text into standardized quantities, units, and foods"
 classifiers = [
   "Development Status :: 3 - Alpha",
   "Intended Audience :: Developers",
   "License :: OSI Approved :: MIT License",
   "Operating System :: Microsoft :: Windows",
   "Operating System :: Unix",
   "Programming Language :: Python :: 3.9",
```

### Comparing `ingredient_slicer-0.0.81/tests/test_avg_ranges.py` & `ingredient_slicer-0.0.83/tests/test_avg_ranges.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.81/tests/test_casual_ingredients.py` & `ingredient_slicer-0.0.83/tests/test_casual_ingredients.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.81/tests/test_duplicate_unit_ranges.py` & `ingredient_slicer-0.0.83/tests/test_duplicate_unit_ranges.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.81/tests/test_extract_dimensions.py` & `ingredient_slicer-0.0.83/tests/test_extract_dimensions.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.81/tests/test_extract_quantities_utils.py` & `ingredient_slicer-0.0.83/tests/test_extract_quantities_utils.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.81/tests/test_find_and_remove.py` & `ingredient_slicer-0.0.83/tests/test_find_and_remove.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.81/tests/test_find_and_remove_hyphen_substrings.py` & `ingredient_slicer-0.0.83/tests/test_find_and_remove_hyphen_substrings.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.81/tests/test_fraction_str_to_decimal.py` & `ingredient_slicer-0.0.83/tests/test_fraction_str_to_decimal.py`

 * *Files 20% similar despite different names*

```diff
@@ -36,35 +36,51 @@
 
 def test_whitespace_padded_fraction_2():
     assert _utils._fraction_str_to_decimal("  3 /4  ") == '0.75'
 
 def test_whitespace_padded_fraction_3():
     assert _utils._fraction_str_to_decimal("  3 / 4  ") == '0.75'
 
+def test_decimals_in_fraction():
+    assert  _utils._fraction_str_to_decimal("2.0/4.0") == '0.5'
+
+def test_fraction_in_numerator_only():
+    assert _utils._fraction_str_to_decimal("3.0/4") == '0.75'
+
+def test_fraction_in_denominator_only():
+    assert _utils._fraction_str_to_decimal("3/4.0") == '0.75'
+
+def test_fraction_with_trailing_period():
+    assert _utils._fraction_str_to_decimal("3/4.") == '0.75'
+
+def test_fraction_with_leading_period():
+    # assert _utils._fraction_str_to_decimal(".3/4") == '0' # NOTE: this should be 0.075 not 0
+    assert _utils._fraction_str_to_decimal(".3/4") == '0.075' # NOTE: this should be 0.075 not 0
+
+def test_fraction_with_leading_and_trailing_periods():
+    # assert _utils._fraction_str_to_decimal(".3/4.") == '0' # NOTE: this should be 0.075 not 0
+    assert _utils._fraction_str_to_decimal(".3/4.") == '0.075' # NOTE: this should be 0.075 not 0
+
 # Error cases
 def test_number_input_error():
     with pytest.raises(ValueError):
         _utils._fraction_str_to_decimal(3)
 
 def test_float_input_error():
     with pytest.raises(ValueError):
         _utils._fraction_str_to_decimal(3.0)
 
 def test_boolean_input_error():
     with pytest.raises(ValueError):
         _utils._fraction_str_to_decimal(True)
 
-def test_invalid_characters_in_fraction():
+def test_invalid_characters_in_fraction_1():
     with pytest.raises(ValueError):
         _utils._fraction_str_to_decimal("43/aaaaa4")
 
-def test_invalid_characters_in_fraction():
-    with pytest.raises(ValueError):
-        _utils._fraction_str_to_decimal("2.0/4.0")
-
 def test_fraction_str_to_decimal_zero_denominator():
     with pytest.raises(ZeroDivisionError):
         _utils._fraction_str_to_decimal("3/0")
 
 def test_fraction_str_to_decimal_mixed_number_1():
     with pytest.raises(ValueError):
         _utils._fraction_str_to_decimal("1 1/2")
```

### Comparing `ingredient_slicer-0.0.81/tests/test_ingredient_slicer.py` & `ingredient_slicer-0.0.83/tests/test_ingredient_slicer.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,22 +17,22 @@
     # slicer.parse()
     parsed = slicer.to_json()
     assert parsed['quantity'] == "2"
     assert parsed['unit'] == 'tablespoons'
     assert parsed['is_required'] == True
 
     parse2 = IngredientSlicer("1/2 cup of sugar")
-    parse2.parse()
+    # parse2.parse()
     parsed = parse2.to_json()
     assert parsed['quantity'] == "0.5"
     assert parsed['unit'] == 'cup'
     assert parsed['is_required'] == True
 
     parse3 = IngredientSlicer("1 1/2 cups of sugar")
-    parse3.parse()
+    # parse3.parse()
     parsed = parse3.to_json()
     assert parsed['quantity'] == "1.5"
     assert parsed['unit'] == 'cups'
     assert parsed['is_required'] == True
 
 def test_quantity_and_unit_1():
     parse = IngredientSlicer("3 pounds of beef")
@@ -195,14 +195,15 @@
     assert parsed['is_required'] == True
 
 # -------------------------------------------------------------------------------
 # ---- Unicode fraction tests ----
 # -------------------------------------------------------------------------------
 def test_single_unicode_fractions_1():
     parse = IngredientSlicer("½cup of sugar")
+    # IngredientSlicer("½cup of sugar", debug=True)
     # parse.parse()
     parsed = parse.to_json()
 
     assert parsed["standardized_ingredient"] == '0.5 cup of sugar' # TODO: add a strip() to the end of the standardized_ingredient
     assert parsed['quantity'] == "0.5"
     assert parsed['unit'] == 'cup'
     assert parsed['standardized_unit'] == 'cup'
```

### Comparing `ingredient_slicer-0.0.81/tests/test_ingredient_slicer_dimensions.py` & `ingredient_slicer-0.0.83/tests/test_ingredient_slicer_dimensions.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,91 +9,92 @@
 # -------------------------------------------------------------------------------
 # ---- Test the dimensions attribute of the IngredientSlicer ----
 # -------------------------------------------------------------------------------
 
 def test_single_inch_ingredient_no_real_quantity_units():
     ing = IngredientSlicer("flour (4 inch)")
 
-    assert ing.dimensions == ["4 inch"]
+    assert ing.dimensions() == ["4 inch"]
 
 def test_single_inch_ingredient_with_real_quantity_units():
     ing = IngredientSlicer("1 cup of flour (4 inch)")
 
-    assert ing.dimensions == ["4 inch"]
+    assert ing.dimensions() == ["4 inch"]
 
 def test_single_inch_ingredient_with_real_quantity_units_and_no_space():
     ing = IngredientSlicer("1 cup of flour (4inch)")
 
-    assert ing.dimensions == ["4 inch"]
+    assert ing.dimensions() == ["4 inch"]
 
 def test_multiple_inch_units():
     ing = IngredientSlicer("1 cup of flour (4 x 3 inch)")
 
 
-    assert ing.dimensions == ["4 x 3 inch"]
+    assert ing.dimensions() == ["4 x 3 inch"]
 
 def test_multiple_inch_units_no_space():
     ing = IngredientSlicer("1 cup of flour (4x3 inch)")
 
-    assert ing.dimensions == ["4 x 3 inch"]
+    assert ing.dimensions() == ["4 x 3 inch"]
 
 def test_multiple_inch_units_no_space_between_numbers():
     ing = IngredientSlicer("1 cup of flour (4x3inch)")
 
-    assert ing.dimensions == ["4 x 3 inch"]
+    assert ing.dimensions() == ["4 x 3 inch"]
 
 def test_multiple_inch_units_no_space_between_numbers_and_no_space():
     ing = IngredientSlicer("1 cup of flour 12.5inch)")
 
-    assert ing.dimensions == ["12.5 inch"]
+    assert ing.dimensions() == ["12.5 inch"]
 
 def test_multiple_inch_units_no_space_between_numbers_and_no_space_no_decimal():
     ing = IngredientSlicer("1 cup of flour 12inch)")
 
-    assert ing.dimensions == ["12 inch"]
+    assert ing.dimensions() == ["12 inch"]
 
 def test_multiple_inch_units_no_space_between_numbers_and_no_space_no_decimal_no_number():
     ing = IngredientSlicer("1 cup of flour 12inch)")
 
-    assert ing.dimensions == ["12 inch"]
+    assert ing.dimensions() == ["12 inch"]
 
 def test_two_sets_of_dimension_unit_ranges_separator_x():
     ing = IngredientSlicer("1 cup of flour (4 x 3 inch) (2 x 2 inch)")
 
-    assert ing.dimensions == ["4 x 3 inch", "2 x 2 inch"]
+    assert ing.dimensions() == ["4 x 3 inch", "2 x 2 inch"]
 
 def test_two_sets_of_dimension_unit_ranges_separator_x_no_space():
     ing = IngredientSlicer("1 cup of flour (4x3 inch) (2x2 inch)")
 
-    assert ing.dimensions == ["4 x 3 inch", "2 x 2 inch"]
+    assert ing.dimensions() == ["4 x 3 inch", "2 x 2 inch"]
 
 def test_two_sets_of_dimension_unit_ranges_separator_by():
     ing = IngredientSlicer("1 cup of flour (4 by 3 inch) (2 by 2 inch)")
 
-    assert ing.dimensions == ["4 by 3 inch", "2 by 2 inch"]
+    assert ing.dimensions() == ["4 by 3 inch", "2 by 2 inch"]
 
 def test_two_sets_of_dimension_unit_ranges_separator_by_no_space():
     ing = IngredientSlicer("1 cup of flour (4by3 inch) (2by2 inch)")
 
-    assert ing.dimensions == ["4 by 3 inch", "2 by 2 inch"]
+    assert ing.dimensions() == ["4 by 3 inch", "2 by 2 inch"]
 
 # TODO: this test is a bug and it needs to be fixed, i.e. the quantity/unit should be 1 cup and thats it. 
 def test_three_consequetive_x_separated_dimension_units():
     ing = IngredientSlicer("1 cup of flour (4 x 3 x 2 inch)")
 
-    expected_output = {'ingredient': '1 cup of flour (4 x 3 x 2 inch)',
+    expected_output = {
     'standardized_ingredient': '1 cup of flour', 
     'food': 'flour',
     'quantity': '12', 
     'unit': 'cup', 
     'standardized_unit': 'cup', 
     'secondary_quantity': '1', 
     'secondary_unit': None, 
     'standardized_secondary_unit': None, 
+    'gram_weight': "1641.26",
     'prep': [], 
     'size_modifiers': [], 
     'dimensions': ['2 inch'],
     'is_required': True, 
     'parenthesis_content': ['12']
     }
 
-    assert ing.parsed_ingredient == expected_output
+    assert ing.parsed_ingredient() == expected_output
```

### Comparing `ingredient_slicer-0.0.81/tests/test_ingredient_slicer_x_separators.py` & `ingredient_slicer-0.0.83/tests/test_ingredient_slicer_x_separators.py`

 * *Files 1% similar despite different names*

```diff
@@ -182,16 +182,14 @@
     assert parsed["dimensions"] == ['2 inch']
 
     assert parsed["parenthesis_content"] == ['thick']
 
 def test_ingredient_slicer_x_separators_quantity_multiplier_with_number_quantity_to_multiply_and_multiple_dimension_units_separated_by_x():
                                             
     slicer = IngredientSlicer("3 x 4oz salmon fillets (2 inch x 3 inch)")
-    slicer.reduced_ingredient
-    slicer.standardized_ingredient
     parsed = slicer.to_json()
 
     assert parsed["standardized_ingredient"] == '12 oz salmon fillets'
 
     assert parsed['quantity'] == "12"
     assert parsed['unit'] == 'oz'
     assert parsed['standardized_unit'] == 'ounce'
```

### Comparing `ingredient_slicer-0.0.81/tests/test_make_int_or_float_str.py` & `ingredient_slicer-0.0.83/tests/test_make_int_or_float_str.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.81/tests/test_merge_numbers.py` & `ingredient_slicer-0.0.83/tests/test_merge_numbers.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.81/tests/test_number_ranges.py` & `ingredient_slicer-0.0.83/tests/test_number_ranges.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.81/tests/test_number_ranges_separated_by_words.py` & `ingredient_slicer-0.0.83/tests/test_number_ranges_separated_by_words.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.81/tests/test_numbers_with_inch_symbols.py` & `ingredient_slicer-0.0.83/tests/test_numbers_with_inch_symbols.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.81/tests/test_parenthesis.py` & `ingredient_slicer-0.0.83/tests/test_parenthesis.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.81/tests/test_parenthesis_utils.py` & `ingredient_slicer-0.0.83/tests/test_parenthesis_utils.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.81/tests/test_percentages.py` & `ingredient_slicer-0.0.83/tests/test_percentages.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.81/tests/test_prefixed_number_words_regex.py` & `ingredient_slicer-0.0.83/tests/test_prefixed_number_words_regex.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.81/tests/test_prep_words.py` & `ingredient_slicer-0.0.83/tests/test_prep_words.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.81/tests/test_quantity_range_regex.py` & `ingredient_slicer-0.0.83/tests/test_quantity_range_regex.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.81/tests/test_quantity_units_regex.py` & `ingredient_slicer-0.0.83/tests/test_quantity_units_regex.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.81/tests/test_remove_repeat_units_in_ranges.py` & `ingredient_slicer-0.0.83/tests/test_remove_repeat_units_in_ranges.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.81/tests/test_remove_x_separators.py` & `ingredient_slicer-0.0.83/tests/test_remove_x_separators.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.81/tests/test_replace_a_or_an_quantities.py` & `ingredient_slicer-0.0.83/tests/test_replace_a_or_an_quantities.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.81/tests/test_separate_dimensions.py` & `ingredient_slicer-0.0.83/tests/test_separate_dimensions.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.81/tests/test_size_modifiers.py` & `ingredient_slicer-0.0.83/tests/test_size_modifiers.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.81/tests/test_spaced_numbers.py` & `ingredient_slicer-0.0.83/tests/test_spaced_numbers.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.81/tests/test_unit_regex.py` & `ingredient_slicer-0.0.83/tests/test_unit_regex.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.81/tests/test_wild_ingredients.py` & `ingredient_slicer-0.0.83/tests/test_wild_ingredients.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 # pytest library
 import pytest
 
 import re
 
 from ingredient_slicer import IngredientSlicer
 
-# IngredientSlicer.regex.PREP_WORDS_PATTERN.findall("3 tablespoons unsalted butter, softened at room temperature")
-# IngredientSlicer.regex.print_matches("3 tablespoons unsalted butter, softened at room temperature")
-# IngredientSlicer.regex.constants["PREP_WORDS"]
-
 # -------------------------------------------------------------------------------
 # ---- Assortment of different ingredients seen in the "wild" tests ----
 # -------------------------------------------------------------------------------
+
 def test_wild_ingredients_1():
 
     parse = IngredientSlicer("1 (10 ounce) package frozen chopped spinach, thawed, drained and squeezed dry")
     # parse.parse()
     parsed = parse.to_json()
 
     assert parsed['quantity'] == "10"
```

### Comparing `ingredient_slicer-0.0.81/tests/test_word_fractions.py` & `ingredient_slicer-0.0.83/tests/test_word_fractions.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.81/tests/test_word_numbers.py` & `ingredient_slicer-0.0.83/tests/test_word_numbers.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.81/tests/test_x_after_number_regex.py` & `ingredient_slicer-0.0.83/tests/test_x_after_number_regex.py`

 * *Files identical despite different names*

