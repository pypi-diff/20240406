# Comparing `tmp/morebs2-0.0.6.tar.gz` & `tmp/morebs2-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "morebs2-0.0.6.tar", last modified: Tue Feb  6 01:52:43 2024, max compression
+gzip compressed data, was "morebs2-0.0.7.tar", last modified: Sat Apr  6 15:59:25 2024, max compression
```

## Comparing `morebs2-0.0.6.tar` & `morebs2-0.0.7.tar`

### file list

```diff
@@ -1,81 +1,83 @@
-drwxrwxrwx   0        0        0        0 2024-02-06 01:52:43.235454 morebs2-0.0.6/
--rw-rw-rw-   0        0        0     7169 2023-09-12 01:51:38.000000 morebs2-0.0.6/LICENSE
--rw-rw-rw-   0        0        0      895 2024-02-06 01:52:43.235454 morebs2-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0      308 2023-09-16 02:45:39.000000 morebs2-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2024-02-06 01:52:43.018162 morebs2-0.0.6/morebs2/
--rw-rw-rw-   0        0        0       53 2023-09-12 01:51:38.000000 morebs2-0.0.6/morebs2/__init__.py
--rw-rw-rw-   0        0        0     9609 2023-09-12 01:51:38.000000 morebs2-0.0.6/morebs2/ball_clump_data_generator.py
--rw-rw-rw-   0        0        0     1849 2023-09-12 01:51:38.000000 morebs2-0.0.6/morebs2/ball_clump_data_generator_test.py
--rw-rw-rw-   0        0        0    17948 2024-02-06 01:45:03.000000 morebs2-0.0.6/morebs2/ball_comp.py
--rw-rw-rw-   0        0        0     9508 2023-09-12 01:51:38.000000 morebs2-0.0.6/morebs2/ball_comp_components.py
--rw-rw-rw-   0        0        0     2195 2024-02-06 01:45:05.000000 morebs2-0.0.6/morebs2/ball_comp_test.py
--rw-rw-rw-   0        0        0     3616 2023-09-12 01:51:38.000000 morebs2-0.0.6/morebs2/ball_comp_test_cases.py
--rw-rw-rw-   0        0        0     9384 2023-09-12 01:51:38.000000 morebs2-0.0.6/morebs2/ball_operator.py
--rw-rw-rw-   0        0        0     2172 2023-09-12 01:51:38.000000 morebs2-0.0.6/morebs2/ball_operator_navigation_test.py
--rw-rw-rw-   0        0        0     1346 2023-09-12 01:51:38.000000 morebs2-0.0.6/morebs2/ball_operator_split_test.py
--rw-rw-rw-   0        0        0     1583 2023-09-12 01:51:38.000000 morebs2-0.0.6/morebs2/ball_operator_test_cases.py
--rw-rw-rw-   0        0        0     6030 2023-09-12 01:51:38.000000 morebs2-0.0.6/morebs2/ball_volume_estimators.py
--rw-rw-rw-   0        0        0     3409 2023-09-12 01:51:38.000000 morebs2-0.0.6/morebs2/chained_poly_interpolation.py
--rw-rw-rw-   0        0        0    22003 2023-09-12 01:51:38.000000 morebs2-0.0.6/morebs2/deline.py
--rw-rw-rw-   0        0        0     7064 2023-09-12 01:51:38.000000 morebs2-0.0.6/morebs2/deline_helpers.py
--rw-rw-rw-   0        0        0     4611 2023-09-12 01:51:38.000000 morebs2-0.0.6/morebs2/deline_mc.py
--rw-rw-rw-   0        0        0     4223 2023-09-12 01:51:38.000000 morebs2-0.0.6/morebs2/distributions.py
--rw-rw-rw-   0        0        0     6744 2023-09-12 01:51:38.000000 morebs2-0.0.6/morebs2/fit_2n2.py
--rw-rw-rw-   0        0        0     1211 2023-09-12 01:51:38.000000 morebs2-0.0.6/morebs2/globalls.py
--rw-rw-rw-   0        0        0     6461 2023-09-12 01:51:38.000000 morebs2-0.0.6/morebs2/hop_pattern.py
--rw-rw-rw-   0        0        0    20982 2023-09-12 01:51:38.000000 morebs2-0.0.6/morebs2/line.py
--rw-rw-rw-   0        0        0    30620 2023-09-12 01:51:38.000000 morebs2-0.0.6/morebs2/matrix_methods.py
--rw-rw-rw-   0        0        0     7251 2023-09-12 01:51:38.000000 morebs2-0.0.6/morebs2/measures.py
--rw-rw-rw-   0        0        0     4386 2023-09-12 01:51:38.000000 morebs2-0.0.6/morebs2/message_streamer.py
--rw-rw-rw-   0        0        0     1573 2023-09-12 01:51:38.000000 morebs2-0.0.6/morebs2/modular_labeller.py
--rw-rw-rw-   0        0        0     1991 2023-12-28 08:50:26.000000 morebs2-0.0.6/morebs2/numerical_extras.py
--rw-rw-rw-   0        0        0     9847 2023-09-12 01:51:38.000000 morebs2-0.0.6/morebs2/numerical_generator.py
--rw-rw-rw-   0        0        0     6520 2023-09-12 01:51:38.000000 morebs2-0.0.6/morebs2/numerical_space_data_generator.py
--rw-rw-rw-   0        0        0    13713 2023-09-12 01:51:38.000000 morebs2-0.0.6/morebs2/point_sorter.py
--rw-rw-rw-   0        0        0     4774 2023-09-12 01:51:38.000000 morebs2-0.0.6/morebs2/point_weight_function.py
--rw-rw-rw-   0        0        0    12158 2023-09-12 01:51:38.000000 morebs2-0.0.6/morebs2/poly_factor.py
--rw-rw-rw-   0        0        0    26397 2023-09-12 01:51:38.000000 morebs2-0.0.6/morebs2/poly_interpolation.py
--rw-rw-rw-   0        0        0    12702 2023-09-12 01:51:38.000000 morebs2-0.0.6/morebs2/poly_struct.py
--rw-rw-rw-   0        0        0     4466 2023-09-12 01:51:38.000000 morebs2-0.0.6/morebs2/random_generators.py
--rw-rw-rw-   0        0        0    28986 2023-09-12 01:51:38.000000 morebs2-0.0.6/morebs2/relevance_functions.py
--rw-rw-rw-   0        0        0     1073 2023-09-12 01:51:38.000000 morebs2-0.0.6/morebs2/relevance_functions_extended.py
--rw-rw-rw-   0        0        0    14223 2023-09-12 01:51:38.000000 morebs2-0.0.6/morebs2/rssi.py
--rw-rw-rw-   0        0        0     4015 2023-09-12 01:51:38.000000 morebs2-0.0.6/morebs2/rssi_components.py
--rw-rw-rw-   0        0        0    16342 2023-09-12 01:51:38.000000 morebs2-0.0.6/morebs2/search_space_iterator.py
--rw-rw-rw-   0        0        0     4968 2023-09-12 01:51:38.000000 morebs2-0.0.6/morebs2/set_merger.py
-drwxrwxrwx   0        0        0        0 2024-02-06 01:52:43.217607 morebs2-0.0.6/morebs2/tests/
--rw-rw-rw-   0        0        0        0 2023-09-12 01:51:38.000000 morebs2-0.0.6/morebs2/tests/__init__.py
--rw-rw-rw-   0        0        0     2969 2023-09-12 01:51:38.000000 morebs2-0.0.6/morebs2/tests/ball_comp_components_test.py
--rw-rw-rw-   0        0        0     1117 2023-09-12 01:51:38.000000 morebs2-0.0.6/morebs2/tests/ball_comp_components_test_cases.py
--rw-rw-rw-   0        0        0     2837 2023-09-12 01:51:38.000000 morebs2-0.0.6/morebs2/tests/chained_poly_interpolation_test.py
--rw-rw-rw-   0        0        0     5692 2023-09-12 01:51:38.000000 morebs2-0.0.6/morebs2/tests/deline_test.py
--rw-rw-rw-   0        0        0     1139 2023-09-12 01:51:38.000000 morebs2-0.0.6/morebs2/tests/fit_2n2_test.py
--rw-rw-rw-   0        0        0     6014 2023-09-12 01:51:38.000000 morebs2-0.0.6/morebs2/tests/hop_pattern_test.py
--rw-rw-rw-   0        0        0     4693 2023-09-12 01:51:38.000000 morebs2-0.0.6/morebs2/tests/matrix_methods__bounds__test.py
--rw-rw-rw-   0        0        0     1986 2023-09-12 01:51:38.000000 morebs2-0.0.6/morebs2/tests/message_streamer_test.py
--rw-rw-rw-   0        0        0     2743 2023-09-12 01:51:38.000000 morebs2-0.0.6/morebs2/tests/numerical_generator_test.py
--rw-rw-rw-   0        0        0     5554 2023-09-12 01:51:38.000000 morebs2-0.0.6/morebs2/tests/numerical_space_data_generator_test.py
--rw-rw-rw-   0        0        0     4351 2023-09-12 01:51:38.000000 morebs2-0.0.6/morebs2/tests/point_sorter_test.py
--rw-rw-rw-   0        0        0     8302 2023-09-12 01:51:38.000000 morebs2-0.0.6/morebs2/tests/point_weight_function_test.py
--rw-rw-rw-   0        0        0     2125 2023-09-12 01:51:38.000000 morebs2-0.0.6/morebs2/tests/poly_factor_test.py
--rw-rw-rw-   0        0        0     9908 2023-09-12 01:51:38.000000 morebs2-0.0.6/morebs2/tests/poly_interpolation_test.py
--rw-rw-rw-   0        0        0     1276 2023-09-12 01:51:38.000000 morebs2-0.0.6/morebs2/tests/poly_struct_test.py
--rw-rw-rw-   0        0        0     6627 2023-09-12 01:51:38.000000 morebs2-0.0.6/morebs2/tests/relevance_functions_test.py
--rw-rw-rw-   0        0        0     1590 2023-09-12 01:51:38.000000 morebs2-0.0.6/morebs2/tests/relevance_functions_test2.py
--rw-rw-rw-   0        0        0     2169 2023-09-12 01:51:38.000000 morebs2-0.0.6/morebs2/tests/rssi_test.py
--rw-rw-rw-   0        0        0     1101 2023-09-12 01:51:38.000000 morebs2-0.0.6/morebs2/tests/rssi_test_cases.py
--rw-rw-rw-   0        0        0     9224 2023-09-12 01:51:39.000000 morebs2-0.0.6/morebs2/tests/search_space_iterator_test.py
--rw-rw-rw-   0        0        0     4336 2023-09-12 01:51:39.000000 morebs2-0.0.6/morebs2/tests/search_space_iterator_test_cases.py
--rw-rw-rw-   0        0        0      958 2023-09-12 01:51:39.000000 morebs2-0.0.6/morebs2/tests/set_merger_test_cases.py
--rw-rw-rw-   0        0        0     3246 2023-09-12 01:51:39.000000 morebs2-0.0.6/morebs2/tests/set_merger_tests.py
--rw-rw-rw-   0        0        0     4925 2023-09-12 01:51:39.000000 morebs2-0.0.6/morebs2/travel_data.py
--rw-rw-rw-   0        0        0      665 2023-09-12 01:51:39.000000 morebs2-0.0.6/morebs2/variance_works.py
--rw-rw-rw-   0        0        0     1773 2023-09-16 02:49:08.000000 morebs2-0.0.6/morebs2/violation_handler.py
-drwxrwxrwx   0        0        0        0 2024-02-06 01:52:43.217607 morebs2-0.0.6/morebs2.egg-info/
--rw-rw-rw-   0        0        0      895 2024-02-06 01:52:42.000000 morebs2-0.0.6/morebs2.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2305 2024-02-06 01:52:42.000000 morebs2-0.0.6/morebs2.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-06 01:52:42.000000 morebs2-0.0.6/morebs2.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-02-06 01:52:42.000000 morebs2-0.0.6/morebs2.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      606 2024-02-06 01:51:37.000000 morebs2-0.0.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-02-06 01:52:43.235454 morebs2-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      472 2024-02-06 01:51:43.000000 morebs2-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-06 15:59:25.279532 morebs2-0.0.7/
+-rw-rw-rw-   0        0        0     7169 2023-09-12 01:51:38.000000 morebs2-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0      895 2024-04-06 15:59:25.279532 morebs2-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0      308 2023-09-16 02:45:39.000000 morebs2-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2024-04-06 15:59:24.791031 morebs2-0.0.7/morebs2/
+-rw-rw-rw-   0        0        0       53 2023-09-12 01:51:38.000000 morebs2-0.0.7/morebs2/__init__.py
+-rw-rw-rw-   0        0        0     7468 2024-04-06 15:40:20.000000 morebs2-0.0.7/morebs2/aprng_gauge.py
+-rw-rw-rw-   0        0        0     9609 2023-09-12 01:51:38.000000 morebs2-0.0.7/morebs2/ball_clump_data_generator.py
+-rw-rw-rw-   0        0        0     1849 2023-09-12 01:51:38.000000 morebs2-0.0.7/morebs2/ball_clump_data_generator_test.py
+-rw-rw-rw-   0        0        0    17948 2024-02-06 01:45:03.000000 morebs2-0.0.7/morebs2/ball_comp.py
+-rw-rw-rw-   0        0        0     9508 2024-02-19 04:29:04.000000 morebs2-0.0.7/morebs2/ball_comp_components.py
+-rw-rw-rw-   0        0        0     2195 2024-02-06 01:45:05.000000 morebs2-0.0.7/morebs2/ball_comp_test.py
+-rw-rw-rw-   0        0        0     3616 2023-09-12 01:51:38.000000 morebs2-0.0.7/morebs2/ball_comp_test_cases.py
+-rw-rw-rw-   0        0        0     9384 2023-09-12 01:51:38.000000 morebs2-0.0.7/morebs2/ball_operator.py
+-rw-rw-rw-   0        0        0     2172 2023-09-12 01:51:38.000000 morebs2-0.0.7/morebs2/ball_operator_navigation_test.py
+-rw-rw-rw-   0        0        0     1346 2023-09-12 01:51:38.000000 morebs2-0.0.7/morebs2/ball_operator_split_test.py
+-rw-rw-rw-   0        0        0     1583 2023-09-12 01:51:38.000000 morebs2-0.0.7/morebs2/ball_operator_test_cases.py
+-rw-rw-rw-   0        0        0     6030 2023-09-12 01:51:38.000000 morebs2-0.0.7/morebs2/ball_volume_estimators.py
+-rw-rw-rw-   0        0        0     3409 2023-09-12 01:51:38.000000 morebs2-0.0.7/morebs2/chained_poly_interpolation.py
+-rw-rw-rw-   0        0        0    22003 2023-09-12 01:51:38.000000 morebs2-0.0.7/morebs2/deline.py
+-rw-rw-rw-   0        0        0     7064 2023-09-12 01:51:38.000000 morebs2-0.0.7/morebs2/deline_helpers.py
+-rw-rw-rw-   0        0        0     4611 2023-09-12 01:51:38.000000 morebs2-0.0.7/morebs2/deline_mc.py
+-rw-rw-rw-   0        0        0     4223 2023-09-12 01:51:38.000000 morebs2-0.0.7/morebs2/distributions.py
+-rw-rw-rw-   0        0        0     6744 2023-09-12 01:51:38.000000 morebs2-0.0.7/morebs2/fit_2n2.py
+-rw-rw-rw-   0        0        0     1211 2023-09-12 01:51:38.000000 morebs2-0.0.7/morebs2/globalls.py
+-rw-rw-rw-   0        0        0     6461 2023-09-12 01:51:38.000000 morebs2-0.0.7/morebs2/hop_pattern.py
+-rw-rw-rw-   0        0        0    20982 2023-09-12 01:51:38.000000 morebs2-0.0.7/morebs2/line.py
+-rw-rw-rw-   0        0        0    30620 2023-09-12 01:51:38.000000 morebs2-0.0.7/morebs2/matrix_methods.py
+-rw-rw-rw-   0        0        0     7251 2024-03-08 20:06:07.000000 morebs2-0.0.7/morebs2/measures.py
+-rw-rw-rw-   0        0        0     4386 2023-09-12 01:51:38.000000 morebs2-0.0.7/morebs2/message_streamer.py
+-rw-rw-rw-   0        0        0     1573 2024-03-06 06:26:15.000000 morebs2-0.0.7/morebs2/modular_labeller.py
+-rw-rw-rw-   0        0        0     1991 2023-12-28 08:50:26.000000 morebs2-0.0.7/morebs2/numerical_extras.py
+-rw-rw-rw-   0        0        0     9847 2023-09-12 01:51:38.000000 morebs2-0.0.7/morebs2/numerical_generator.py
+-rw-rw-rw-   0        0        0     6520 2023-09-12 01:51:38.000000 morebs2-0.0.7/morebs2/numerical_space_data_generator.py
+-rw-rw-rw-   0        0        0    13713 2023-09-12 01:51:38.000000 morebs2-0.0.7/morebs2/point_sorter.py
+-rw-rw-rw-   0        0        0     4774 2023-09-12 01:51:38.000000 morebs2-0.0.7/morebs2/point_weight_function.py
+-rw-rw-rw-   0        0        0    12158 2023-09-12 01:51:38.000000 morebs2-0.0.7/morebs2/poly_factor.py
+-rw-rw-rw-   0        0        0    26397 2023-09-12 01:51:38.000000 morebs2-0.0.7/morebs2/poly_interpolation.py
+-rw-rw-rw-   0        0        0    12702 2023-09-12 01:51:38.000000 morebs2-0.0.7/morebs2/poly_struct.py
+-rw-rw-rw-   0        0        0     4466 2023-09-12 01:51:38.000000 morebs2-0.0.7/morebs2/random_generators.py
+-rw-rw-rw-   0        0        0    28986 2024-04-03 21:33:23.000000 morebs2-0.0.7/morebs2/relevance_functions.py
+-rw-rw-rw-   0        0        0     1073 2023-09-12 01:51:38.000000 morebs2-0.0.7/morebs2/relevance_functions_extended.py
+-rw-rw-rw-   0        0        0    14223 2023-09-12 01:51:38.000000 morebs2-0.0.7/morebs2/rssi.py
+-rw-rw-rw-   0        0        0     4015 2023-09-12 01:51:38.000000 morebs2-0.0.7/morebs2/rssi_components.py
+-rw-rw-rw-   0        0        0    16342 2024-04-06 11:44:14.000000 morebs2-0.0.7/morebs2/search_space_iterator.py
+-rw-rw-rw-   0        0        0     4968 2023-09-12 01:51:38.000000 morebs2-0.0.7/morebs2/set_merger.py
+drwxrwxrwx   0        0        0        0 2024-04-06 15:59:25.263911 morebs2-0.0.7/morebs2/tests/
+-rw-rw-rw-   0        0        0        0 2023-09-12 01:51:38.000000 morebs2-0.0.7/morebs2/tests/__init__.py
+-rw-rw-rw-   0        0        0     3332 2024-04-06 15:37:56.000000 morebs2-0.0.7/morebs2/tests/aprng_gauge_test.py
+-rw-rw-rw-   0        0        0     2969 2023-09-12 01:51:38.000000 morebs2-0.0.7/morebs2/tests/ball_comp_components_test.py
+-rw-rw-rw-   0        0        0     1117 2023-09-12 01:51:38.000000 morebs2-0.0.7/morebs2/tests/ball_comp_components_test_cases.py
+-rw-rw-rw-   0        0        0     2837 2023-09-12 01:51:38.000000 morebs2-0.0.7/morebs2/tests/chained_poly_interpolation_test.py
+-rw-rw-rw-   0        0        0     5692 2023-09-12 01:51:38.000000 morebs2-0.0.7/morebs2/tests/deline_test.py
+-rw-rw-rw-   0        0        0     1139 2023-09-12 01:51:38.000000 morebs2-0.0.7/morebs2/tests/fit_2n2_test.py
+-rw-rw-rw-   0        0        0     6014 2023-09-12 01:51:38.000000 morebs2-0.0.7/morebs2/tests/hop_pattern_test.py
+-rw-rw-rw-   0        0        0     4693 2023-09-12 01:51:38.000000 morebs2-0.0.7/morebs2/tests/matrix_methods__bounds__test.py
+-rw-rw-rw-   0        0        0     1986 2023-09-12 01:51:38.000000 morebs2-0.0.7/morebs2/tests/message_streamer_test.py
+-rw-rw-rw-   0        0        0     2743 2023-09-12 01:51:38.000000 morebs2-0.0.7/morebs2/tests/numerical_generator_test.py
+-rw-rw-rw-   0        0        0     5554 2023-09-12 01:51:38.000000 morebs2-0.0.7/morebs2/tests/numerical_space_data_generator_test.py
+-rw-rw-rw-   0        0        0     4351 2023-09-12 01:51:38.000000 morebs2-0.0.7/morebs2/tests/point_sorter_test.py
+-rw-rw-rw-   0        0        0     8302 2023-09-12 01:51:38.000000 morebs2-0.0.7/morebs2/tests/point_weight_function_test.py
+-rw-rw-rw-   0        0        0     2125 2023-09-12 01:51:38.000000 morebs2-0.0.7/morebs2/tests/poly_factor_test.py
+-rw-rw-rw-   0        0        0     9908 2023-09-12 01:51:38.000000 morebs2-0.0.7/morebs2/tests/poly_interpolation_test.py
+-rw-rw-rw-   0        0        0     1276 2023-09-12 01:51:38.000000 morebs2-0.0.7/morebs2/tests/poly_struct_test.py
+-rw-rw-rw-   0        0        0     6627 2023-09-12 01:51:38.000000 morebs2-0.0.7/morebs2/tests/relevance_functions_test.py
+-rw-rw-rw-   0        0        0     1590 2023-09-12 01:51:38.000000 morebs2-0.0.7/morebs2/tests/relevance_functions_test2.py
+-rw-rw-rw-   0        0        0     2169 2023-09-12 01:51:38.000000 morebs2-0.0.7/morebs2/tests/rssi_test.py
+-rw-rw-rw-   0        0        0     1101 2023-09-12 01:51:38.000000 morebs2-0.0.7/morebs2/tests/rssi_test_cases.py
+-rw-rw-rw-   0        0        0     9224 2023-09-12 01:51:39.000000 morebs2-0.0.7/morebs2/tests/search_space_iterator_test.py
+-rw-rw-rw-   0        0        0     4336 2023-09-12 01:51:39.000000 morebs2-0.0.7/morebs2/tests/search_space_iterator_test_cases.py
+-rw-rw-rw-   0        0        0      958 2023-09-12 01:51:39.000000 morebs2-0.0.7/morebs2/tests/set_merger_test_cases.py
+-rw-rw-rw-   0        0        0     3246 2023-09-12 01:51:39.000000 morebs2-0.0.7/morebs2/tests/set_merger_tests.py
+-rw-rw-rw-   0        0        0     4925 2023-09-12 01:51:39.000000 morebs2-0.0.7/morebs2/travel_data.py
+-rw-rw-rw-   0        0        0      665 2023-09-12 01:51:39.000000 morebs2-0.0.7/morebs2/variance_works.py
+-rw-rw-rw-   0        0        0     1773 2023-09-16 02:49:08.000000 morebs2-0.0.7/morebs2/violation_handler.py
+drwxrwxrwx   0        0        0        0 2024-04-06 15:59:25.263911 morebs2-0.0.7/morebs2.egg-info/
+-rw-rw-rw-   0        0        0      895 2024-04-06 15:59:22.000000 morebs2-0.0.7/morebs2.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2362 2024-04-06 15:59:22.000000 morebs2-0.0.7/morebs2.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-06 15:59:22.000000 morebs2-0.0.7/morebs2.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-04-06 15:59:22.000000 morebs2-0.0.7/morebs2.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      606 2024-04-06 15:55:06.000000 morebs2-0.0.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-06 15:59:25.279532 morebs2-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      472 2024-04-06 15:55:16.000000 morebs2-0.0.7/setup.py
```

### Comparing `morebs2-0.0.6/LICENSE` & `morebs2-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `morebs2-0.0.6/PKG-INFO` & `morebs2-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: morebs2
-Version: 0.0.6
+Version: 0.0.7
 Summary: data structures to aid in numerical data generation and clustering
 Home-page: https://github.com/Changissnz/morebs
 Author: Richard Pham
 Author-email: Richard Pham <phamrichard45@gmail.com>
 Project-URL: Homepage, https://www.github.com/changissnz/morebs
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
```

### Comparing `morebs2-0.0.6/morebs2/ball_clump_data_generator.py` & `morebs2-0.0.7/morebs2/ball_clump_data_generator.py`

 * *Files identical despite different names*

### Comparing `morebs2-0.0.6/morebs2/ball_clump_data_generator_test.py` & `morebs2-0.0.7/morebs2/ball_clump_data_generator_test.py`

 * *Files identical despite different names*

### Comparing `morebs2-0.0.6/morebs2/ball_comp.py` & `morebs2-0.0.7/morebs2/ball_comp.py`

 * *Files identical despite different names*

### Comparing `morebs2-0.0.6/morebs2/ball_comp_components.py` & `morebs2-0.0.7/morebs2/ball_comp_components.py`

 * *Files identical despite different names*

### Comparing `morebs2-0.0.6/morebs2/ball_comp_test.py` & `morebs2-0.0.7/morebs2/ball_comp_test.py`

 * *Files identical despite different names*

### Comparing `morebs2-0.0.6/morebs2/ball_comp_test_cases.py` & `morebs2-0.0.7/morebs2/ball_comp_test_cases.py`

 * *Files identical despite different names*

### Comparing `morebs2-0.0.6/morebs2/ball_operator.py` & `morebs2-0.0.7/morebs2/ball_operator.py`

 * *Files identical despite different names*

### Comparing `morebs2-0.0.6/morebs2/ball_operator_navigation_test.py` & `morebs2-0.0.7/morebs2/ball_operator_navigation_test.py`

 * *Files identical despite different names*

### Comparing `morebs2-0.0.6/morebs2/ball_operator_split_test.py` & `morebs2-0.0.7/morebs2/ball_operator_split_test.py`

 * *Files identical despite different names*

### Comparing `morebs2-0.0.6/morebs2/ball_operator_test_cases.py` & `morebs2-0.0.7/morebs2/ball_operator_test_cases.py`

 * *Files identical despite different names*

### Comparing `morebs2-0.0.6/morebs2/ball_volume_estimators.py` & `morebs2-0.0.7/morebs2/ball_volume_estimators.py`

 * *Files identical despite different names*

### Comparing `morebs2-0.0.6/morebs2/chained_poly_interpolation.py` & `morebs2-0.0.7/morebs2/chained_poly_interpolation.py`

 * *Files identical despite different names*

### Comparing `morebs2-0.0.6/morebs2/deline.py` & `morebs2-0.0.7/morebs2/deline.py`

 * *Files identical despite different names*

### Comparing `morebs2-0.0.6/morebs2/deline_helpers.py` & `morebs2-0.0.7/morebs2/deline_helpers.py`

 * *Files identical despite different names*

### Comparing `morebs2-0.0.6/morebs2/deline_mc.py` & `morebs2-0.0.7/morebs2/deline_mc.py`

 * *Files identical despite different names*

### Comparing `morebs2-0.0.6/morebs2/distributions.py` & `morebs2-0.0.7/morebs2/distributions.py`

 * *Files identical despite different names*

### Comparing `morebs2-0.0.6/morebs2/fit_2n2.py` & `morebs2-0.0.7/morebs2/fit_2n2.py`

 * *Files identical despite different names*

### Comparing `morebs2-0.0.6/morebs2/globalls.py` & `morebs2-0.0.7/morebs2/globalls.py`

 * *Files identical despite different names*

### Comparing `morebs2-0.0.6/morebs2/hop_pattern.py` & `morebs2-0.0.7/morebs2/hop_pattern.py`

 * *Files identical despite different names*

### Comparing `morebs2-0.0.6/morebs2/line.py` & `morebs2-0.0.7/morebs2/line.py`

 * *Files identical despite different names*

### Comparing `morebs2-0.0.6/morebs2/matrix_methods.py` & `morebs2-0.0.7/morebs2/matrix_methods.py`

 * *Files identical despite different names*

### Comparing `morebs2-0.0.6/morebs2/measures.py` & `morebs2-0.0.7/morebs2/measures.py`

 * *Files identical despite different names*

### Comparing `morebs2-0.0.6/morebs2/message_streamer.py` & `morebs2-0.0.7/morebs2/message_streamer.py`

 * *Files identical despite different names*

### Comparing `morebs2-0.0.6/morebs2/modular_labeller.py` & `morebs2-0.0.7/morebs2/modular_labeller.py`

 * *Files identical despite different names*

### Comparing `morebs2-0.0.6/morebs2/numerical_extras.py` & `morebs2-0.0.7/morebs2/numerical_extras.py`

 * *Files identical despite different names*

### Comparing `morebs2-0.0.6/morebs2/numerical_generator.py` & `morebs2-0.0.7/morebs2/numerical_generator.py`

 * *Files identical despite different names*

### Comparing `morebs2-0.0.6/morebs2/numerical_space_data_generator.py` & `morebs2-0.0.7/morebs2/numerical_space_data_generator.py`

 * *Files identical despite different names*

### Comparing `morebs2-0.0.6/morebs2/point_sorter.py` & `morebs2-0.0.7/morebs2/point_sorter.py`

 * *Files identical despite different names*

### Comparing `morebs2-0.0.6/morebs2/point_weight_function.py` & `morebs2-0.0.7/morebs2/point_weight_function.py`

 * *Files identical despite different names*

### Comparing `morebs2-0.0.6/morebs2/poly_factor.py` & `morebs2-0.0.7/morebs2/poly_factor.py`

 * *Files identical despite different names*

### Comparing `morebs2-0.0.6/morebs2/poly_interpolation.py` & `morebs2-0.0.7/morebs2/poly_interpolation.py`

 * *Files identical despite different names*

### Comparing `morebs2-0.0.6/morebs2/poly_struct.py` & `morebs2-0.0.7/morebs2/poly_struct.py`

 * *Files identical despite different names*

### Comparing `morebs2-0.0.6/morebs2/random_generators.py` & `morebs2-0.0.7/morebs2/random_generators.py`

 * *Files identical despite different names*

### Comparing `morebs2-0.0.6/morebs2/relevance_functions.py` & `morebs2-0.0.7/morebs2/relevance_functions.py`

 * *Files identical despite different names*

### Comparing `morebs2-0.0.6/morebs2/relevance_functions_extended.py` & `morebs2-0.0.7/morebs2/relevance_functions_extended.py`

 * *Files identical despite different names*

### Comparing `morebs2-0.0.6/morebs2/rssi.py` & `morebs2-0.0.7/morebs2/rssi.py`

 * *Files identical despite different names*

### Comparing `morebs2-0.0.6/morebs2/rssi_components.py` & `morebs2-0.0.7/morebs2/rssi_components.py`

 * *Files identical despite different names*

### Comparing `morebs2-0.0.6/morebs2/search_space_iterator.py` & `morebs2-0.0.7/morebs2/search_space_iterator.py`

 * *Files identical despite different names*

### Comparing `morebs2-0.0.6/morebs2/set_merger.py` & `morebs2-0.0.7/morebs2/set_merger.py`

 * *Files identical despite different names*

### Comparing `morebs2-0.0.6/morebs2/tests/ball_comp_components_test.py` & `morebs2-0.0.7/morebs2/tests/ball_comp_components_test.py`

 * *Files identical despite different names*

### Comparing `morebs2-0.0.6/morebs2/tests/ball_comp_components_test_cases.py` & `morebs2-0.0.7/morebs2/tests/ball_comp_components_test_cases.py`

 * *Files identical despite different names*

### Comparing `morebs2-0.0.6/morebs2/tests/chained_poly_interpolation_test.py` & `morebs2-0.0.7/morebs2/tests/chained_poly_interpolation_test.py`

 * *Files identical despite different names*

### Comparing `morebs2-0.0.6/morebs2/tests/deline_test.py` & `morebs2-0.0.7/morebs2/tests/deline_test.py`

 * *Files identical despite different names*

### Comparing `morebs2-0.0.6/morebs2/tests/fit_2n2_test.py` & `morebs2-0.0.7/morebs2/tests/fit_2n2_test.py`

 * *Files identical despite different names*

### Comparing `morebs2-0.0.6/morebs2/tests/hop_pattern_test.py` & `morebs2-0.0.7/morebs2/tests/hop_pattern_test.py`

 * *Files identical despite different names*

### Comparing `morebs2-0.0.6/morebs2/tests/matrix_methods__bounds__test.py` & `morebs2-0.0.7/morebs2/tests/matrix_methods__bounds__test.py`

 * *Files identical despite different names*

### Comparing `morebs2-0.0.6/morebs2/tests/message_streamer_test.py` & `morebs2-0.0.7/morebs2/tests/message_streamer_test.py`

 * *Files identical despite different names*

### Comparing `morebs2-0.0.6/morebs2/tests/numerical_generator_test.py` & `morebs2-0.0.7/morebs2/tests/numerical_generator_test.py`

 * *Files identical despite different names*

### Comparing `morebs2-0.0.6/morebs2/tests/numerical_space_data_generator_test.py` & `morebs2-0.0.7/morebs2/tests/numerical_space_data_generator_test.py`

 * *Files identical despite different names*

### Comparing `morebs2-0.0.6/morebs2/tests/point_sorter_test.py` & `morebs2-0.0.7/morebs2/tests/point_sorter_test.py`

 * *Files identical despite different names*

### Comparing `morebs2-0.0.6/morebs2/tests/point_weight_function_test.py` & `morebs2-0.0.7/morebs2/tests/point_weight_function_test.py`

 * *Files identical despite different names*

### Comparing `morebs2-0.0.6/morebs2/tests/poly_factor_test.py` & `morebs2-0.0.7/morebs2/tests/poly_factor_test.py`

 * *Files identical despite different names*

### Comparing `morebs2-0.0.6/morebs2/tests/poly_interpolation_test.py` & `morebs2-0.0.7/morebs2/tests/poly_interpolation_test.py`

 * *Files identical despite different names*

### Comparing `morebs2-0.0.6/morebs2/tests/poly_struct_test.py` & `morebs2-0.0.7/morebs2/tests/poly_struct_test.py`

 * *Files identical despite different names*

### Comparing `morebs2-0.0.6/morebs2/tests/relevance_functions_test.py` & `morebs2-0.0.7/morebs2/tests/relevance_functions_test.py`

 * *Files identical despite different names*

### Comparing `morebs2-0.0.6/morebs2/tests/relevance_functions_test2.py` & `morebs2-0.0.7/morebs2/tests/relevance_functions_test2.py`

 * *Files identical despite different names*

### Comparing `morebs2-0.0.6/morebs2/tests/rssi_test.py` & `morebs2-0.0.7/morebs2/tests/rssi_test.py`

 * *Files identical despite different names*

### Comparing `morebs2-0.0.6/morebs2/tests/rssi_test_cases.py` & `morebs2-0.0.7/morebs2/tests/rssi_test_cases.py`

 * *Files identical despite different names*

### Comparing `morebs2-0.0.6/morebs2/tests/search_space_iterator_test.py` & `morebs2-0.0.7/morebs2/tests/search_space_iterator_test.py`

 * *Files identical despite different names*

### Comparing `morebs2-0.0.6/morebs2/tests/search_space_iterator_test_cases.py` & `morebs2-0.0.7/morebs2/tests/search_space_iterator_test_cases.py`

 * *Files identical despite different names*

### Comparing `morebs2-0.0.6/morebs2/tests/set_merger_test_cases.py` & `morebs2-0.0.7/morebs2/tests/set_merger_test_cases.py`

 * *Files identical despite different names*

### Comparing `morebs2-0.0.6/morebs2/tests/set_merger_tests.py` & `morebs2-0.0.7/morebs2/tests/set_merger_tests.py`

 * *Files identical despite different names*

### Comparing `morebs2-0.0.6/morebs2/travel_data.py` & `morebs2-0.0.7/morebs2/travel_data.py`

 * *Files identical despite different names*

### Comparing `morebs2-0.0.6/morebs2/variance_works.py` & `morebs2-0.0.7/morebs2/variance_works.py`

 * *Files identical despite different names*

### Comparing `morebs2-0.0.6/morebs2/violation_handler.py` & `morebs2-0.0.7/morebs2/violation_handler.py`

 * *Files identical despite different names*

### Comparing `morebs2-0.0.6/morebs2.egg-info/PKG-INFO` & `morebs2-0.0.7/morebs2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: morebs2
-Version: 0.0.6
+Version: 0.0.7
 Summary: data structures to aid in numerical data generation and clustering
 Home-page: https://github.com/Changissnz/morebs
 Author: Richard Pham
 Author-email: Richard Pham <phamrichard45@gmail.com>
 Project-URL: Homepage, https://www.github.com/changissnz/morebs
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
```

### Comparing `morebs2-0.0.6/morebs2.egg-info/SOURCES.txt` & `morebs2-0.0.7/morebs2.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 LICENSE
 README.md
 pyproject.toml
 setup.py
 morebs2/__init__.py
+morebs2/aprng_gauge.py
 morebs2/ball_clump_data_generator.py
 morebs2/ball_clump_data_generator_test.py
 morebs2/ball_comp.py
 morebs2/ball_comp_components.py
 morebs2/ball_comp_test.py
 morebs2/ball_comp_test_cases.py
 morebs2/ball_operator.py
@@ -46,14 +47,15 @@
 morebs2/variance_works.py
 morebs2/violation_handler.py
 morebs2.egg-info/PKG-INFO
 morebs2.egg-info/SOURCES.txt
 morebs2.egg-info/dependency_links.txt
 morebs2.egg-info/top_level.txt
 morebs2/tests/__init__.py
+morebs2/tests/aprng_gauge_test.py
 morebs2/tests/ball_comp_components_test.py
 morebs2/tests/ball_comp_components_test_cases.py
 morebs2/tests/chained_poly_interpolation_test.py
 morebs2/tests/deline_test.py
 morebs2/tests/fit_2n2_test.py
 morebs2/tests/hop_pattern_test.py
 morebs2/tests/matrix_methods__bounds__test.py
```

### Comparing `morebs2-0.0.6/pyproject.toml` & `morebs2-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=40.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "morebs2"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="Richard Pham", email="phamrichard45@gmail.com" },
 ]
 description = "data structures to aid in numerical data generation and clustering"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

