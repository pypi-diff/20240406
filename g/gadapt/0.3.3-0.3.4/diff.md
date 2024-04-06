# Comparing `tmp/gadapt-0.3.3.tar.gz` & `tmp/gadapt-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gadapt-0.3.3.tar", last modified: Sat Mar 16 18:47:07 2024, max compression
+gzip compressed data, was "gadapt-0.3.4.tar", last modified: Sat Apr  6 20:16:33 2024, max compression
```

## Comparing `gadapt-0.3.3.tar` & `gadapt-0.3.4.tar`

### file list

```diff
@@ -1,115 +1,116 @@
-drwxrwxrwx   0        0        0        0 2024-03-16 18:47:07.258370 gadapt-0.3.3/
--rw-rw-rw-   0        0        0     1522 2023-05-20 09:05:31.000000 gadapt-0.3.3/LICENSE
--rw-rw-rw-   0        0        0    22405 2024-03-16 18:47:07.257867 gadapt-0.3.3/PKG-INFO
--rw-rw-rw-   0        0        0    22080 2024-03-16 18:31:55.000000 gadapt-0.3.3/README.md
-drwxrwxrwx   0        0        0        0 2024-03-16 18:47:06.926356 gadapt-0.3.3/gadapt/
--rw-rw-rw-   0        0        0       36 2023-09-10 20:35:27.000000 gadapt-0.3.3/gadapt/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-16 18:47:06.958857 gadapt-0.3.3/gadapt/adapters/
--rw-rw-rw-   0        0        0       33 2023-09-10 20:35:28.000000 gadapt-0.3.3/gadapt/adapters/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-16 18:47:06.966857 gadapt-0.3.3/gadapt/adapters/ga_logging/
--rw-rw-rw-   0        0        0       28 2023-09-10 20:35:27.000000 gadapt-0.3.3/gadapt/adapters/ga_logging/__init__.py
--rw-rw-rw-   0        0        0     2200 2023-10-06 11:40:57.000000 gadapt-0.3.3/gadapt/adapters/ga_logging/logging_settings.py
-drwxrwxrwx   0        0        0        0 2024-03-16 18:47:06.977358 gadapt-0.3.3/gadapt/adapters/string_operation/
--rw-rw-rw-   0        0        0       92 2023-09-10 20:35:28.000000 gadapt-0.3.3/gadapt/adapters/string_operation/__init__.py
--rw-rw-rw-   0        0        0     4188 2023-09-10 20:35:28.000000 gadapt-0.3.3/gadapt/adapters/string_operation/ga_strings.py
-drwxrwxrwx   0        0        0        0 2024-03-16 18:47:06.984858 gadapt-0.3.3/gadapt/adapters/validation/
--rw-rw-rw-   0        0        0       33 2023-09-10 20:35:28.000000 gadapt-0.3.3/gadapt/adapters/validation/__init__.py
--rw-rw-rw-   0        0        0      939 2023-09-11 06:37:11.000000 gadapt-0.3.3/gadapt/adapters/validation/base_options_validator.py
--rw-rw-rw-   0        0        0    21335 2024-03-05 19:39:48.000000 gadapt-0.3.3/gadapt/adapters/validation/common_options_validator.py
-drwxrwxrwx   0        0        0        0 2024-03-16 18:47:06.992357 gadapt-0.3.3/gadapt/execution/
--rw-rw-rw-   0        0        0       50 2023-09-10 20:35:27.000000 gadapt-0.3.3/gadapt/execution/__init__.py
--rw-rw-rw-   0        0        0     3413 2024-03-16 18:16:05.000000 gadapt-0.3.3/gadapt/execution/ga_executor.py
-drwxrwxrwx   0        0        0        0 2024-03-16 18:47:07.002858 gadapt-0.3.3/gadapt/factory/
--rw-rw-rw-   0        0        0       76 2023-09-10 20:35:27.000000 gadapt-0.3.3/gadapt/factory/__init__.py
--rw-rw-rw-   0        0        0     6349 2024-03-16 18:19:48.000000 gadapt-0.3.3/gadapt/factory/ga_base_factory.py
--rw-rw-rw-   0        0        0    12329 2024-03-16 18:16:05.000000 gadapt-0.3.3/gadapt/factory/ga_factory.py
--rw-rw-rw-   0        0        0    29568 2024-03-16 18:20:17.000000 gadapt-0.3.3/gadapt/ga.py
-drwxrwxrwx   0        0        0        0 2024-03-16 18:47:07.038859 gadapt-0.3.3/gadapt/ga_model/
--rw-rw-rw-   0        0        0       35 2023-09-10 20:35:27.000000 gadapt-0.3.3/gadapt/ga_model/__init__.py
--rw-rw-rw-   0        0        0     9769 2024-03-05 19:39:48.000000 gadapt-0.3.3/gadapt/ga_model/chromosome.py
--rw-rw-rw-   0        0        0      807 2024-03-16 18:16:05.000000 gadapt-0.3.3/gadapt/ga_model/definitions.py
--rw-rw-rw-   0        0        0     6856 2024-03-05 19:39:48.000000 gadapt-0.3.3/gadapt/ga_model/ga_options.py
--rw-rw-rw-   0        0        0     2256 2024-03-05 19:39:48.000000 gadapt-0.3.3/gadapt/ga_model/ga_results.py
--rw-rw-rw-   0        0        0     1995 2024-03-16 18:16:05.000000 gadapt-0.3.3/gadapt/ga_model/gene.py
--rw-rw-rw-   0        0        0     3301 2024-03-16 18:20:24.000000 gadapt-0.3.3/gadapt/ga_model/genetic_variable.py
--rw-rw-rw-   0        0        0       81 2023-09-10 20:35:27.000000 gadapt-0.3.3/gadapt/ga_model/message_levels.py
--rw-rw-rw-   0        0        0    12842 2024-03-05 19:39:48.000000 gadapt-0.3.3/gadapt/ga_model/population.py
--rw-rw-rw-   0        0        0     1269 2024-03-05 19:39:48.000000 gadapt-0.3.3/gadapt/ga_model/ranking_model.py
-drwxrwxrwx   0        0        0        0 2024-03-16 18:47:07.039864 gadapt-0.3.3/gadapt/operations/
--rw-rw-rw-   0        0        0       28 2023-09-10 20:35:27.000000 gadapt-0.3.3/gadapt/operations/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-16 18:47:07.051860 gadapt-0.3.3/gadapt/operations/cost_finding/
--rw-rw-rw-   0        0        0       66 2023-09-10 20:35:27.000000 gadapt-0.3.3/gadapt/operations/cost_finding/__init__.py
--rw-rw-rw-   0        0        0     1239 2023-09-10 20:38:03.000000 gadapt-0.3.3/gadapt/operations/cost_finding/base_cost_finder.py
--rw-rw-rw-   0        0        0     1893 2024-03-05 19:39:48.000000 gadapt-0.3.3/gadapt/operations/cost_finding/elitism_cost_finder.py
-drwxrwxrwx   0        0        0        0 2024-03-16 18:47:07.063360 gadapt-0.3.3/gadapt/operations/crossover/
--rw-rw-rw-   0        0        0       35 2023-09-10 20:35:27.000000 gadapt-0.3.3/gadapt/operations/crossover/__init__.py
--rw-rw-rw-   0        0        0     7663 2024-03-05 19:39:48.000000 gadapt-0.3.3/gadapt/operations/crossover/base_crossover.py
--rw-rw-rw-   0        0        0     1464 2024-03-05 19:39:48.000000 gadapt-0.3.3/gadapt/operations/crossover/uniform_crossover.py
-drwxrwxrwx   0        0        0        0 2024-03-16 18:47:07.075361 gadapt-0.3.3/gadapt/operations/exit_check/
--rw-rw-rw-   0        0        0       58 2023-09-10 20:35:27.000000 gadapt-0.3.3/gadapt/operations/exit_check/__init__.py
--rw-rw-rw-   0        0        0      510 2024-03-05 19:39:48.000000 gadapt-0.3.3/gadapt/operations/exit_check/avg_cost_exit_checker.py
--rw-rw-rw-   0        0        0     1268 2024-03-05 19:39:48.000000 gadapt-0.3.3/gadapt/operations/exit_check/base_exit_checker.py
--rw-rw-rw-   0        0        0      487 2024-03-05 19:39:48.000000 gadapt-0.3.3/gadapt/operations/exit_check/min_cost_exit_checker.py
--rw-rw-rw-   0        0        0      529 2024-03-05 19:39:48.000000 gadapt-0.3.3/gadapt/operations/exit_check/requested_cost_exit_checker.py
-drwxrwxrwx   0        0        0        0 2024-03-16 18:47:07.084361 gadapt-0.3.3/gadapt/operations/gene_combination/
--rw-rw-rw-   0        0        0       93 2023-09-10 20:35:27.000000 gadapt-0.3.3/gadapt/operations/gene_combination/__init__.py
--rw-rw-rw-   0        0        0      608 2024-03-05 19:39:48.000000 gadapt-0.3.3/gadapt/operations/gene_combination/base_gene_combination.py
--rw-rw-rw-   0        0        0     1210 2024-03-05 19:39:48.000000 gadapt-0.3.3/gadapt/operations/gene_combination/blending_gene_combination.py
-drwxrwxrwx   0        0        0        0 2024-03-16 18:47:07.085862 gadapt-0.3.3/gadapt/operations/immigration/
--rw-rw-rw-   0        0        0       56 2023-09-10 20:35:27.000000 gadapt-0.3.3/gadapt/operations/immigration/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-16 18:47:07.096361 gadapt-0.3.3/gadapt/operations/immigration/chromosome_immigration/
--rw-rw-rw-   0        0        0       71 2023-09-10 20:35:27.000000 gadapt-0.3.3/gadapt/operations/immigration/chromosome_immigration/__init__.py
--rw-rw-rw-   0        0        0      787 2024-03-05 19:39:48.000000 gadapt-0.3.3/gadapt/operations/immigration/chromosome_immigration/base_chromosome_immigrator.py
--rw-rw-rw-   0        0        0      422 2024-03-05 19:39:48.000000 gadapt-0.3.3/gadapt/operations/immigration/chromosome_immigration/random_chromosome_immigrator.py
-drwxrwxrwx   0        0        0        0 2024-03-16 18:47:07.108362 gadapt-0.3.3/gadapt/operations/immigration/population_immigration/
--rw-rw-rw-   0        0        0       81 2023-09-10 20:35:27.000000 gadapt-0.3.3/gadapt/operations/immigration/population_immigration/__init__.py
--rw-rw-rw-   0        0        0      473 2024-03-05 19:39:48.000000 gadapt-0.3.3/gadapt/operations/immigration/population_immigration/base_population_immigrator.py
--rw-rw-rw-   0        0        0     1045 2024-03-05 19:39:48.000000 gadapt-0.3.3/gadapt/operations/immigration/population_immigration/common_population_immigrator.py
-drwxrwxrwx   0        0        0        0 2024-03-16 18:47:07.112863 gadapt-0.3.3/gadapt/operations/mutation/
--rw-rw-rw-   0        0        0       40 2023-09-10 20:35:27.000000 gadapt-0.3.3/gadapt/operations/mutation/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-16 18:47:07.129863 gadapt-0.3.3/gadapt/operations/mutation/chromosome_mutation/
--rw-rw-rw-   0        0        0       44 2023-09-10 20:35:27.000000 gadapt-0.3.3/gadapt/operations/mutation/chromosome_mutation/__init__.py
--rw-rw-rw-   0        0        0     1237 2024-03-16 18:16:05.000000 gadapt-0.3.3/gadapt/operations/mutation/chromosome_mutation/base_chromosome_mutator.py
--rw-rw-rw-   0        0        0     1317 2024-03-16 18:15:51.000000 gadapt-0.3.3/gadapt/operations/mutation/chromosome_mutation/cross_diversity_chromosome_mutator.py
--rw-rw-rw-   0        0        0      720 2024-03-16 18:15:51.000000 gadapt-0.3.3/gadapt/operations/mutation/chromosome_mutation/random_chromosome_mutator.py
-drwxrwxrwx   0        0        0        0 2024-03-16 18:47:07.145861 gadapt-0.3.3/gadapt/operations/mutation/gene_mutation/
--rw-rw-rw-   0        0        0       25 2024-03-16 13:31:03.000000 gadapt-0.3.3/gadapt/operations/mutation/gene_mutation/__init__.py
--rw-rw-rw-   0        0        0      328 2024-03-16 18:16:05.000000 gadapt-0.3.3/gadapt/operations/mutation/gene_mutation/base_gene_mutator.py
--rw-rw-rw-   0        0        0     2199 2024-03-16 18:16:05.000000 gadapt-0.3.3/gadapt/operations/mutation/gene_mutation/extreme_pointed_gene_mutator.py
--rw-rw-rw-   0        0        0      901 2024-03-16 18:16:05.000000 gadapt-0.3.3/gadapt/operations/mutation/gene_mutation/normal_distribution_gene_mutator.py
--rw-rw-rw-   0        0        0      342 2024-03-16 18:16:05.000000 gadapt-0.3.3/gadapt/operations/mutation/gene_mutation/random_gene_mutator.py
-drwxrwxrwx   0        0        0        0 2024-03-16 18:47:07.172363 gadapt-0.3.3/gadapt/operations/mutation/population_mutation/
--rw-rw-rw-   0        0        0       53 2023-09-10 20:35:27.000000 gadapt-0.3.3/gadapt/operations/mutation/population_mutation/__init__.py
--rw-rw-rw-   0        0        0     1571 2024-03-05 19:39:48.000000 gadapt-0.3.3/gadapt/operations/mutation/population_mutation/base_population_mutator.py
--rw-rw-rw-   0        0        0     1238 2024-03-16 18:15:51.000000 gadapt-0.3.3/gadapt/operations/mutation/population_mutation/composed_population_mutator.py
--rw-rw-rw-   0        0        0     2205 2024-03-05 19:39:48.000000 gadapt-0.3.3/gadapt/operations/mutation/population_mutation/cost_diversity_population_mutator.py
--rw-rw-rw-   0        0        0     2072 2024-03-05 19:39:48.000000 gadapt-0.3.3/gadapt/operations/mutation/population_mutation/parent_diversity_population_mutator.py
--rw-rw-rw-   0        0        0      925 2024-03-05 19:39:48.000000 gadapt-0.3.3/gadapt/operations/mutation/population_mutation/random_population_mutator.py
-drwxrwxrwx   0        0        0        0 2024-03-16 18:47:07.185865 gadapt-0.3.3/gadapt/operations/parent_selection/
--rw-rw-rw-   0        0        0       39 2023-09-10 20:35:28.000000 gadapt-0.3.3/gadapt/operations/parent_selection/__init__.py
--rw-rw-rw-   0        0        0      737 2023-09-17 10:37:22.000000 gadapt-0.3.3/gadapt/operations/parent_selection/base_parent_selector.py
--rw-rw-rw-   0        0        0     1233 2024-03-05 19:39:48.000000 gadapt-0.3.3/gadapt/operations/parent_selection/sampling_parent_selector.py
-drwxrwxrwx   0        0        0        0 2024-03-16 18:47:07.213365 gadapt-0.3.3/gadapt/operations/sampling/
--rw-rw-rw-   0        0        0      136 2023-09-10 20:52:27.000000 gadapt-0.3.3/gadapt/operations/sampling/__init__.py
--rw-rw-rw-   0        0        0     1102 2024-03-05 19:39:48.000000 gadapt-0.3.3/gadapt/operations/sampling/base_sampling.py
--rw-rw-rw-   0        0        0      509 2024-03-05 19:39:48.000000 gadapt-0.3.3/gadapt/operations/sampling/from_top_to_bottom_sampling.py
--rw-rw-rw-   0        0        0      500 2023-09-17 10:36:51.000000 gadapt-0.3.3/gadapt/operations/sampling/random_sampling.py
--rw-rw-rw-   0        0        0     1917 2024-03-05 19:39:48.000000 gadapt-0.3.3/gadapt/operations/sampling/roulette_wheel_sampling.py
--rw-rw-rw-   0        0        0     2601 2024-03-05 19:39:48.000000 gadapt-0.3.3/gadapt/operations/sampling/tournament_sampling.py
-drwxrwxrwx   0        0        0        0 2024-03-16 18:47:07.225365 gadapt-0.3.3/gadapt/operations/variable_update/
--rw-rw-rw-   0        0        0       55 2023-09-10 20:35:28.000000 gadapt-0.3.3/gadapt/operations/variable_update/__init__.py
--rw-rw-rw-   0        0        0      210 2024-03-05 19:39:48.000000 gadapt-0.3.3/gadapt/operations/variable_update/base_variable_updater.py
--rw-rw-rw-   0        0        0     2037 2024-03-05 19:39:48.000000 gadapt-0.3.3/gadapt/operations/variable_update/common_variable_updater.py
-drwxrwxrwx   0        0        0        0 2024-03-16 18:47:07.244866 gadapt-0.3.3/gadapt/utils/
--rw-rw-rw-   0        0        0      443 2024-03-05 19:39:48.000000 gadapt-0.3.3/gadapt/utils/TimeStampFormatter.py
--rw-rw-rw-   0        0        0       37 2023-09-10 20:35:28.000000 gadapt-0.3.3/gadapt/utils/__init__.py
--rw-rw-rw-   0        0        0     2617 2024-03-16 18:25:48.000000 gadapt-0.3.3/gadapt/utils/ga_utils.py
-drwxrwxrwx   0        0        0        0 2024-03-16 18:47:07.255866 gadapt-0.3.3/gadapt.egg-info/
--rw-rw-rw-   0        0        0    22405 2024-03-16 18:47:06.000000 gadapt-0.3.3/gadapt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4123 2024-03-16 18:47:06.000000 gadapt-0.3.3/gadapt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-16 18:47:06.000000 gadapt-0.3.3/gadapt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-03-16 18:47:06.000000 gadapt-0.3.3/gadapt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-03-16 18:47:06.000000 gadapt-0.3.3/gadapt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      812 2024-03-05 19:18:24.000000 gadapt-0.3.3/pyproject.toml
--rw-rw-rw-   0        0        0      111 2024-03-16 18:47:07.260370 gadapt-0.3.3/setup.cfg
--rw-rw-rw-   0        0        0      512 2024-03-16 18:22:48.000000 gadapt-0.3.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-06 20:16:33.225236 gadapt-0.3.4/
+-rw-rw-rw-   0        0        0     1522 2023-05-20 09:05:31.000000 gadapt-0.3.4/LICENSE
+-rw-rw-rw-   0        0        0    22076 2024-04-06 20:16:33.224734 gadapt-0.3.4/PKG-INFO
+-rw-rw-rw-   0        0        0    21751 2024-03-16 19:55:38.000000 gadapt-0.3.4/README.md
+drwxrwxrwx   0        0        0        0 2024-04-06 20:16:32.984740 gadapt-0.3.4/gadapt/
+-rw-rw-rw-   0        0        0       36 2023-09-10 20:35:27.000000 gadapt-0.3.4/gadapt/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-06 20:16:33.007232 gadapt-0.3.4/gadapt/adapters/
+-rw-rw-rw-   0        0        0       33 2023-09-10 20:35:28.000000 gadapt-0.3.4/gadapt/adapters/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-06 20:16:33.010233 gadapt-0.3.4/gadapt/adapters/ga_logging/
+-rw-rw-rw-   0        0        0       28 2023-09-10 20:35:27.000000 gadapt-0.3.4/gadapt/adapters/ga_logging/__init__.py
+-rw-rw-rw-   0        0        0     2200 2023-10-06 11:40:57.000000 gadapt-0.3.4/gadapt/adapters/ga_logging/logging_settings.py
+drwxrwxrwx   0        0        0        0 2024-04-06 20:16:33.012733 gadapt-0.3.4/gadapt/adapters/string_operation/
+-rw-rw-rw-   0        0        0       92 2023-09-10 20:35:28.000000 gadapt-0.3.4/gadapt/adapters/string_operation/__init__.py
+-rw-rw-rw-   0        0        0     4190 2024-04-06 20:11:32.000000 gadapt-0.3.4/gadapt/adapters/string_operation/ga_strings.py
+drwxrwxrwx   0        0        0        0 2024-04-06 20:16:33.021734 gadapt-0.3.4/gadapt/adapters/validation/
+-rw-rw-rw-   0        0        0       33 2023-09-10 20:35:28.000000 gadapt-0.3.4/gadapt/adapters/validation/__init__.py
+-rw-rw-rw-   0        0        0      939 2023-09-11 06:37:11.000000 gadapt-0.3.4/gadapt/adapters/validation/base_options_validator.py
+-rw-rw-rw-   0        0        0    21348 2024-04-06 20:11:32.000000 gadapt-0.3.4/gadapt/adapters/validation/common_options_validator.py
+drwxrwxrwx   0        0        0        0 2024-04-06 20:16:33.029236 gadapt-0.3.4/gadapt/execution/
+-rw-rw-rw-   0        0        0       50 2023-09-10 20:35:27.000000 gadapt-0.3.4/gadapt/execution/__init__.py
+-rw-rw-rw-   0        0        0     3396 2024-04-06 20:11:32.000000 gadapt-0.3.4/gadapt/execution/ga_executor.py
+drwxrwxrwx   0        0        0        0 2024-04-06 20:16:33.034733 gadapt-0.3.4/gadapt/factory/
+-rw-rw-rw-   0        0        0       76 2023-09-10 20:35:27.000000 gadapt-0.3.4/gadapt/factory/__init__.py
+-rw-rw-rw-   0        0        0     6349 2024-03-16 18:19:48.000000 gadapt-0.3.4/gadapt/factory/ga_base_factory.py
+-rw-rw-rw-   0        0        0    17819 2024-04-06 20:11:32.000000 gadapt-0.3.4/gadapt/factory/ga_factory.py
+-rw-rw-rw-   0        0        0    29258 2024-04-06 20:11:32.000000 gadapt-0.3.4/gadapt/ga.py
+drwxrwxrwx   0        0        0        0 2024-04-06 20:16:33.052234 gadapt-0.3.4/gadapt/ga_model/
+-rw-rw-rw-   0        0        0       35 2023-09-10 20:35:27.000000 gadapt-0.3.4/gadapt/ga_model/__init__.py
+-rw-rw-rw-   0        0        0     9772 2024-04-06 20:11:32.000000 gadapt-0.3.4/gadapt/ga_model/chromosome.py
+-rw-rw-rw-   0        0        0     3739 2024-04-06 20:11:32.000000 gadapt-0.3.4/gadapt/ga_model/decision_variable.py
+-rw-rw-rw-   0        0        0      878 2024-04-06 20:11:32.000000 gadapt-0.3.4/gadapt/ga_model/definitions.py
+-rw-rw-rw-   0        0        0     6865 2024-04-06 20:11:32.000000 gadapt-0.3.4/gadapt/ga_model/ga_options.py
+-rw-rw-rw-   0        0        0     2256 2024-03-05 19:39:48.000000 gadapt-0.3.4/gadapt/ga_model/ga_results.py
+-rw-rw-rw-   0        0        0     2011 2024-04-06 20:11:32.000000 gadapt-0.3.4/gadapt/ga_model/gene.py
+-rw-rw-rw-   0        0        0       81 2023-09-10 20:35:27.000000 gadapt-0.3.4/gadapt/ga_model/message_levels.py
+-rw-rw-rw-   0        0        0    13275 2024-04-06 20:11:32.000000 gadapt-0.3.4/gadapt/ga_model/population.py
+-rw-rw-rw-   0        0        0     1269 2024-03-05 19:39:48.000000 gadapt-0.3.4/gadapt/ga_model/ranking_model.py
+drwxrwxrwx   0        0        0        0 2024-04-06 20:16:33.053232 gadapt-0.3.4/gadapt/operations/
+-rw-rw-rw-   0        0        0       28 2023-09-10 20:35:27.000000 gadapt-0.3.4/gadapt/operations/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-06 20:16:33.056732 gadapt-0.3.4/gadapt/operations/cost_finding/
+-rw-rw-rw-   0        0        0       66 2023-09-10 20:35:27.000000 gadapt-0.3.4/gadapt/operations/cost_finding/__init__.py
+-rw-rw-rw-   0        0        0     1432 2024-04-06 20:11:32.000000 gadapt-0.3.4/gadapt/operations/cost_finding/base_cost_finder.py
+-rw-rw-rw-   0        0        0     1893 2024-03-05 19:39:48.000000 gadapt-0.3.4/gadapt/operations/cost_finding/elitism_cost_finder.py
+drwxrwxrwx   0        0        0        0 2024-04-06 20:16:33.065734 gadapt-0.3.4/gadapt/operations/crossover/
+-rw-rw-rw-   0        0        0       35 2023-09-10 20:35:27.000000 gadapt-0.3.4/gadapt/operations/crossover/__init__.py
+-rw-rw-rw-   0        0        0     7678 2024-04-06 20:11:32.000000 gadapt-0.3.4/gadapt/operations/crossover/base_crossover.py
+-rw-rw-rw-   0        0        0     1464 2024-03-05 19:39:48.000000 gadapt-0.3.4/gadapt/operations/crossover/uniform_crossover.py
+drwxrwxrwx   0        0        0        0 2024-04-06 20:16:33.080735 gadapt-0.3.4/gadapt/operations/exit_check/
+-rw-rw-rw-   0        0        0       58 2023-09-10 20:35:27.000000 gadapt-0.3.4/gadapt/operations/exit_check/__init__.py
+-rw-rw-rw-   0        0        0      510 2024-03-05 19:39:48.000000 gadapt-0.3.4/gadapt/operations/exit_check/avg_cost_exit_checker.py
+-rw-rw-rw-   0        0        0     1268 2024-03-05 19:39:48.000000 gadapt-0.3.4/gadapt/operations/exit_check/base_exit_checker.py
+-rw-rw-rw-   0        0        0      487 2024-03-05 19:39:48.000000 gadapt-0.3.4/gadapt/operations/exit_check/min_cost_exit_checker.py
+-rw-rw-rw-   0        0        0      529 2024-03-05 19:39:48.000000 gadapt-0.3.4/gadapt/operations/exit_check/requested_cost_exit_checker.py
+drwxrwxrwx   0        0        0        0 2024-04-06 20:16:33.089233 gadapt-0.3.4/gadapt/operations/gene_combination/
+-rw-rw-rw-   0        0        0       93 2023-09-10 20:35:27.000000 gadapt-0.3.4/gadapt/operations/gene_combination/__init__.py
+-rw-rw-rw-   0        0        0      608 2024-03-05 19:39:48.000000 gadapt-0.3.4/gadapt/operations/gene_combination/base_gene_combination.py
+-rw-rw-rw-   0        0        0     1217 2024-04-06 20:11:32.000000 gadapt-0.3.4/gadapt/operations/gene_combination/blending_gene_combination.py
+drwxrwxrwx   0        0        0        0 2024-04-06 20:16:33.090734 gadapt-0.3.4/gadapt/operations/immigration/
+-rw-rw-rw-   0        0        0       56 2023-09-10 20:35:27.000000 gadapt-0.3.4/gadapt/operations/immigration/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-06 20:16:33.099232 gadapt-0.3.4/gadapt/operations/immigration/chromosome_immigration/
+-rw-rw-rw-   0        0        0       71 2023-09-10 20:35:27.000000 gadapt-0.3.4/gadapt/operations/immigration/chromosome_immigration/__init__.py
+-rw-rw-rw-   0        0        0      787 2024-03-05 19:39:48.000000 gadapt-0.3.4/gadapt/operations/immigration/chromosome_immigration/base_chromosome_immigrator.py
+-rw-rw-rw-   0        0        0      422 2024-03-05 19:39:48.000000 gadapt-0.3.4/gadapt/operations/immigration/chromosome_immigration/random_chromosome_immigrator.py
+drwxrwxrwx   0        0        0        0 2024-04-06 20:16:33.104732 gadapt-0.3.4/gadapt/operations/immigration/population_immigration/
+-rw-rw-rw-   0        0        0       81 2023-09-10 20:35:27.000000 gadapt-0.3.4/gadapt/operations/immigration/population_immigration/__init__.py
+-rw-rw-rw-   0        0        0      473 2024-03-05 19:39:48.000000 gadapt-0.3.4/gadapt/operations/immigration/population_immigration/base_population_immigrator.py
+-rw-rw-rw-   0        0        0     1045 2024-03-05 19:39:48.000000 gadapt-0.3.4/gadapt/operations/immigration/population_immigration/common_population_immigrator.py
+drwxrwxrwx   0        0        0        0 2024-04-06 20:16:33.107233 gadapt-0.3.4/gadapt/operations/mutation/
+-rw-rw-rw-   0        0        0       40 2023-09-10 20:35:27.000000 gadapt-0.3.4/gadapt/operations/mutation/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-06 20:16:33.120734 gadapt-0.3.4/gadapt/operations/mutation/chromosome_mutation/
+-rw-rw-rw-   0        0        0       44 2023-09-10 20:35:27.000000 gadapt-0.3.4/gadapt/operations/mutation/chromosome_mutation/__init__.py
+-rw-rw-rw-   0        0        0     1240 2024-04-06 20:11:32.000000 gadapt-0.3.4/gadapt/operations/mutation/chromosome_mutation/base_chromosome_mutator.py
+-rw-rw-rw-   0        0        0     1319 2024-04-06 20:11:32.000000 gadapt-0.3.4/gadapt/operations/mutation/chromosome_mutation/cross_diversity_chromosome_mutator.py
+-rw-rw-rw-   0        0        0      720 2024-03-16 18:15:51.000000 gadapt-0.3.4/gadapt/operations/mutation/chromosome_mutation/random_chromosome_mutator.py
+drwxrwxrwx   0        0        0        0 2024-04-06 20:16:33.145733 gadapt-0.3.4/gadapt/operations/mutation/gene_mutation/
+-rw-rw-rw-   0        0        0       25 2024-03-16 13:31:03.000000 gadapt-0.3.4/gadapt/operations/mutation/gene_mutation/__init__.py
+-rw-rw-rw-   0        0        0      328 2024-03-16 18:16:05.000000 gadapt-0.3.4/gadapt/operations/mutation/gene_mutation/base_gene_mutator.py
+-rw-rw-rw-   0        0        0     2232 2024-04-06 20:11:32.000000 gadapt-0.3.4/gadapt/operations/mutation/gene_mutation/extreme_pointed_gene_mutator.py
+-rw-rw-rw-   0        0        0     2287 2024-04-06 20:11:32.000000 gadapt-0.3.4/gadapt/operations/mutation/gene_mutation/normal_distribution_gene_mutator.py
+-rw-rw-rw-   0        0        0      344 2024-04-06 20:11:32.000000 gadapt-0.3.4/gadapt/operations/mutation/gene_mutation/random_gene_mutator.py
+drwxrwxrwx   0        0        0        0 2024-04-06 20:16:33.199733 gadapt-0.3.4/gadapt/operations/mutation/population_mutation/
+-rw-rw-rw-   0        0        0       53 2023-09-10 20:35:27.000000 gadapt-0.3.4/gadapt/operations/mutation/population_mutation/__init__.py
+-rw-rw-rw-   0        0        0     1674 2024-04-06 20:11:32.000000 gadapt-0.3.4/gadapt/operations/mutation/population_mutation/base_population_mutator.py
+-rw-rw-rw-   0        0        0     1728 2024-04-06 20:11:32.000000 gadapt-0.3.4/gadapt/operations/mutation/population_mutation/composed_population_mutator.py
+-rw-rw-rw-   0        0        0     1813 2024-04-06 20:11:32.000000 gadapt-0.3.4/gadapt/operations/mutation/population_mutation/cost_diversity_population_mutator.py
+-rw-rw-rw-   0        0        0     1738 2024-04-06 20:11:32.000000 gadapt-0.3.4/gadapt/operations/mutation/population_mutation/cross_diversity_population_mutator.py
+-rw-rw-rw-   0        0        0     2170 2024-04-06 20:11:32.000000 gadapt-0.3.4/gadapt/operations/mutation/population_mutation/parent_diversity_population_mutator.py
+-rw-rw-rw-   0        0        0     1021 2024-04-06 20:11:32.000000 gadapt-0.3.4/gadapt/operations/mutation/population_mutation/random_population_mutator.py
+drwxrwxrwx   0        0        0        0 2024-04-06 20:16:33.205234 gadapt-0.3.4/gadapt/operations/parent_selection/
+-rw-rw-rw-   0        0        0       39 2023-09-10 20:35:28.000000 gadapt-0.3.4/gadapt/operations/parent_selection/__init__.py
+-rw-rw-rw-   0        0        0      737 2023-09-17 10:37:22.000000 gadapt-0.3.4/gadapt/operations/parent_selection/base_parent_selector.py
+-rw-rw-rw-   0        0        0     1233 2024-03-05 19:39:48.000000 gadapt-0.3.4/gadapt/operations/parent_selection/sampling_parent_selector.py
+drwxrwxrwx   0        0        0        0 2024-04-06 20:16:33.213734 gadapt-0.3.4/gadapt/operations/sampling/
+-rw-rw-rw-   0        0        0      136 2023-09-10 20:52:27.000000 gadapt-0.3.4/gadapt/operations/sampling/__init__.py
+-rw-rw-rw-   0        0        0     1102 2024-03-05 19:39:48.000000 gadapt-0.3.4/gadapt/operations/sampling/base_sampling.py
+-rw-rw-rw-   0        0        0      509 2024-03-05 19:39:48.000000 gadapt-0.3.4/gadapt/operations/sampling/from_top_to_bottom_sampling.py
+-rw-rw-rw-   0        0        0      500 2023-09-17 10:36:51.000000 gadapt-0.3.4/gadapt/operations/sampling/random_sampling.py
+-rw-rw-rw-   0        0        0     1892 2024-04-06 20:11:32.000000 gadapt-0.3.4/gadapt/operations/sampling/roulette_wheel_sampling.py
+-rw-rw-rw-   0        0        0     2601 2024-03-05 19:39:48.000000 gadapt-0.3.4/gadapt/operations/sampling/tournament_sampling.py
+drwxrwxrwx   0        0        0        0 2024-04-06 20:16:33.218733 gadapt-0.3.4/gadapt/operations/variable_update/
+-rw-rw-rw-   0        0        0       56 2024-04-06 20:11:32.000000 gadapt-0.3.4/gadapt/operations/variable_update/__init__.py
+-rw-rw-rw-   0        0        0      210 2024-03-05 19:39:48.000000 gadapt-0.3.4/gadapt/operations/variable_update/base_variable_updater.py
+-rw-rw-rw-   0        0        0     2567 2024-04-06 20:11:32.000000 gadapt-0.3.4/gadapt/operations/variable_update/common_variable_updater.py
+drwxrwxrwx   0        0        0        0 2024-04-06 20:16:33.221734 gadapt-0.3.4/gadapt/utils/
+-rw-rw-rw-   0        0        0      443 2024-03-05 19:39:48.000000 gadapt-0.3.4/gadapt/utils/TimeStampFormatter.py
+-rw-rw-rw-   0        0        0       37 2023-09-10 20:35:28.000000 gadapt-0.3.4/gadapt/utils/__init__.py
+-rw-rw-rw-   0        0        0     2901 2024-04-06 20:11:32.000000 gadapt-0.3.4/gadapt/utils/ga_utils.py
+drwxrwxrwx   0        0        0        0 2024-04-06 20:16:33.223234 gadapt-0.3.4/gadapt.egg-info/
+-rw-rw-rw-   0        0        0    22076 2024-04-06 20:16:32.000000 gadapt-0.3.4/gadapt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4209 2024-04-06 20:16:32.000000 gadapt-0.3.4/gadapt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-06 20:16:32.000000 gadapt-0.3.4/gadapt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-04-06 20:16:32.000000 gadapt-0.3.4/gadapt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-06 20:16:32.000000 gadapt-0.3.4/gadapt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      812 2024-03-05 19:18:24.000000 gadapt-0.3.4/pyproject.toml
+-rw-rw-rw-   0        0        0      111 2024-04-06 20:16:33.227234 gadapt-0.3.4/setup.cfg
+-rw-rw-rw-   0        0        0      512 2024-04-06 20:15:45.000000 gadapt-0.3.4/setup.py
```

### Comparing `gadapt-0.3.3/LICENSE` & `gadapt-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `gadapt-0.3.3/PKG-INFO` & `gadapt-0.3.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gadapt
-Version: 0.3.3
+Version: 0.3.4
 Summary: GAdapt: A Python Library for        Self-Adaptive Genetic Algorithm.
 Home-page: https://github.com/bpzoran/gadapt
 Author: Zoran Jankovic
 Author-email: bpzoran@yahoo.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
@@ -165,17 +165,16 @@
 **must_mutate_for_same_parents**=*True* - Indicates if completely the same parents must influence mutation for their children. In other words, each child will be mutated if it has parents with a diversity value of 0. If *must_mutate_for_same_parents* has the value True, the number of mutated chromosomes can outreach value determined by *number_of_mutation_chromosomes* or *percentage_of_mutation_chromosomes*
 
 **chromosome_mutation**=*"cross_diversity"* - The type of gene selection in chromosomes for mutation  
 Supported values:
 - *"cross_diversity"* - Considers the diversity of genes of the same type in the population. Lower diversity can mean that this genetic variable approaches some local minimums, and therefore such genes increase the chance for mutation. Based on the calculated cross-diversity, chromosomes may be selected by one of the selection methods, which is determined by the value of the *cross_diversity_mutation_gene_selection* parameter.  
 - *"random"* - Genes are randomly selected for the mutation
 
-**gene_mutation**=*"extreme_pointed"* - The type of assigning mutated values to genes
+**gene_mutation**=*"normal_distribution"* - The type of assigning mutated values to genes
 Supported values:
-- *"extreme_pointed"* - Considers the diversity of genes of the same type in the population. Lower diversity can mean that this genetic variable approaches sub-optimal value. In that case, this mutator increases chances to mutate extreme values (minimum or maximum), while keeping the chances to mutate to the other extreme value. 
 - *"normal_distribution"* - assignes normally distributed random number to the variable selected for mutation
 - *"random"* - Random values are assigned to genes
 
 **cross_diversity_mutation_gene_selection**=*"roulette_wheel"* - the selection algorithm for mutating chromosomes when *chromosome_mutation* has value *"cross_diversity"*. It only applies when *chromosome_mutation* has value *"cross_diversity"* . It determines the way how genes are to be selected based on the cross-diversity.  
 Supported values:
 - *"roulette_wheel"* - The Roulette Wheel selection algorithm (also known as "Weighted Random Pairing"). The probabilities assigned to the genes to be mutated are inversely proportional to their cross-diversity. A gene with the lowest cross-diversity has the greatest probability of mutation, while the gene with the highest cross-diversity has the lowest probability of mutation.  
 - *"tournament"* - The Tournament selection algorithm. It randomly picks small subsets (groups) of genes, and genes with the lowest cross-diversity in subsets are chosen to be mutated. *"tournament"* can have an additional parameter separated from the *"tournament"* keyword by the comma. The other value represents a group size. For example, *"tournament,3"* means that the tournament mutation selection algorithm is chosen, and each group contains up to 3 members. The default group size is 4.
```

### Comparing `gadapt-0.3.3/README.md` & `gadapt-0.3.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -154,17 +154,16 @@
 **must_mutate_for_same_parents**=*True* - Indicates if completely the same parents must influence mutation for their children. In other words, each child will be mutated if it has parents with a diversity value of 0. If *must_mutate_for_same_parents* has the value True, the number of mutated chromosomes can outreach value determined by *number_of_mutation_chromosomes* or *percentage_of_mutation_chromosomes*
 
 **chromosome_mutation**=*"cross_diversity"* - The type of gene selection in chromosomes for mutation  
 Supported values:
 - *"cross_diversity"* - Considers the diversity of genes of the same type in the population. Lower diversity can mean that this genetic variable approaches some local minimums, and therefore such genes increase the chance for mutation. Based on the calculated cross-diversity, chromosomes may be selected by one of the selection methods, which is determined by the value of the *cross_diversity_mutation_gene_selection* parameter.  
 - *"random"* - Genes are randomly selected for the mutation
 
-**gene_mutation**=*"extreme_pointed"* - The type of assigning mutated values to genes
+**gene_mutation**=*"normal_distribution"* - The type of assigning mutated values to genes
 Supported values:
-- *"extreme_pointed"* - Considers the diversity of genes of the same type in the population. Lower diversity can mean that this genetic variable approaches sub-optimal value. In that case, this mutator increases chances to mutate extreme values (minimum or maximum), while keeping the chances to mutate to the other extreme value. 
 - *"normal_distribution"* - assignes normally distributed random number to the variable selected for mutation
 - *"random"* - Random values are assigned to genes
 
 **cross_diversity_mutation_gene_selection**=*"roulette_wheel"* - the selection algorithm for mutating chromosomes when *chromosome_mutation* has value *"cross_diversity"*. It only applies when *chromosome_mutation* has value *"cross_diversity"* . It determines the way how genes are to be selected based on the cross-diversity.  
 Supported values:
 - *"roulette_wheel"* - The Roulette Wheel selection algorithm (also known as "Weighted Random Pairing"). The probabilities assigned to the genes to be mutated are inversely proportional to their cross-diversity. A gene with the lowest cross-diversity has the greatest probability of mutation, while the gene with the highest cross-diversity has the lowest probability of mutation.  
 - *"tournament"* - The Tournament selection algorithm. It randomly picks small subsets (groups) of genes, and genes with the lowest cross-diversity in subsets are chosen to be mutated. *"tournament"* can have an additional parameter separated from the *"tournament"* keyword by the comma. The other value represents a group size. For example, *"tournament,3"* means that the tournament mutation selection algorithm is chosen, and each group contains up to 3 members. The default group size is 4.
```

### Comparing `gadapt-0.3.3/gadapt/adapters/ga_logging/logging_settings.py` & `gadapt-0.3.4/gadapt/adapters/ga_logging/logging_settings.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.3.3/gadapt/adapters/string_operation/ga_strings.py` & `gadapt-0.3.4/gadapt/adapters/string_operation/ga_strings.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 def gene_to_string(g):
     """
     Creates string  from the gene
     Args:
         g: Gene for string representation
     """
-    return str(g.genetic_variable.variable_id) + ": " + str(round(g.variable_value, 2))
+    return str(g.decision_variable.variable_id) + ": " + str(round(g.variable_value, 2))
 
 
 def chromosome_to_string(c):
     """
     Creates string  from the chromosome
     Args:
         c: Chromosome for string representation
@@ -23,15 +23,15 @@
     str_res = "Chromosome "
     id_str = str(c.chromosome_id)
     while len(id_str) < 4:
         id_str = " " + id_str
     str_res = str_res + id_str + " - "
     for g in c:
         str_res += (
-            str(g.genetic_variable.variable_id)
+            str(g.decision_variable.variable_id)
             + ": "
             + str(round(g.variable_value, 2))
             + "; "
         )
     str_res += "Cost value: " + str(c.cost_value) + "; "
     str_res += "Chromosome generation: " + str(c.chromosome_generation) + "; "
     if not (
```

### Comparing `gadapt-0.3.3/gadapt/adapters/validation/base_options_validator.py` & `gadapt-0.3.4/gadapt/adapters/validation/base_options_validator.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.3.3/gadapt/adapters/validation/common_options_validator.py` & `gadapt-0.3.4/gadapt/adapters/validation/common_options_validator.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,22 +9,22 @@
 
     def __init__(self, options) -> None:
         super().__init__(options)
         self._validation_messages = []
 
     def _validate_options(self):
         self.success &= self._check_nones_types_and_values()
-        self.success &= self._check_genetic_variables()
+        self.success &= self._check_decision_variables()
         self.success &= self._check_cost_function()
 
-    def _check_genetic_variables(self) -> bool:
-        if self.options._genetic_variables is None:
+    def _check_decision_variables(self) -> bool:
+        if self.options._decision_variables is None:
             return False
         rslt = True
-        for v in self.options._genetic_variables:
+        for v in self.options._decision_variables:
             if v.min_value is None or v.max_value is None or v.step is None:
                 self._add_message(
                     "Min value, max value and step must not be\
                         None! (Variable {var_no})".format(
                         var_no=v.variable_id
                     )
                 )
@@ -77,15 +77,15 @@
             self._add_message("Cost Function must not be None!")
             return False
         elif not callable(self.options.cost_function):
             self._add_message("Cost Function must be callable!")
             return False
         argsmin = {}
         argsmax = {}
-        for v in self.options._genetic_variables:
+        for v in self.options._decision_variables:
             argsmin[v.variable_id] = v.min_value
             argsmax[v.variable_id] = v.max_value
         try:
             func_result_min = self.options.cost_function(argsmin)
             func_result_max = self.options.cost_function(argsmax)
             if not isinstance(func_result_min, float) or not isinstance(
                 func_result_max, float
@@ -190,20 +190,20 @@
                     "Invalid percentage of mutation chromosomes: {0} and number\
                         of mutation chromosomes: {1}".format(
                         str(self.options.percentage_of_mutation_chromosomes),
                         str(self.options.number_of_mutation_chromosomes),
                     )
                 )
                 rslt &= False
-        if self.options._genetic_variables is None:
-            self._add_message("Genetic variables must not be None!")
+        if self.options._decision_variables is None:
+            self._add_message("Decision variables must not be None!")
             rslt &= False
-        num_of_genetic_variables = len(self.options._genetic_variables)  # type: ignore
-        if num_of_genetic_variables < 1:
-            self._add_message("At least one genetic variable must be added!")
+        num_of_decision_variables = len(self.options._decision_variables)  # type: ignore
+        if num_of_decision_variables < 1:
+            self._add_message("At least one decision variable must be added!")
             rslt &= False
         if (
             self.options.number_of_mutation_genes is None
             and self.options.percentage_of_mutation_genes is None
         ):
             self._add_message(
                 "Number Of Mutation Genes or Percentage Of\
@@ -220,16 +220,16 @@
             rslt &= False
         elif (
             (self.options.number_of_mutation_genes is not None)
             and isinstance(self.options.number_of_mutation_genes, int)
             and (self.options.number_of_mutation_genes > 0)
         ):
             if (
-                num_of_genetic_variables > 0
-                and self.options.number_of_mutation_genes > num_of_genetic_variables
+                num_of_decision_variables > 0
+                and self.options.number_of_mutation_genes > num_of_decision_variables
             ):
                 self._add_message(
                     "Invalid number of mutation genes: {0}".format(
                         str(self.options.number_of_mutation_genes)
                     )
                 )
                 rslt &= False
```

### Comparing `gadapt-0.3.3/gadapt/execution/ga_executor.py` & `gadapt-0.3.4/gadapt/execution/ga_executor.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,18 +40,18 @@
             population_mutator = self.factory.get_population_mutator()
             exit_checker = self.factory.get_exit_checker()
             cost_finder = self.factory.get_cost_finder()
             population_immigrator = self.factory.get_population_immigrator()
             chromosome_immigrator = self.factory.get_chromosome_immigrator()
             selector = self.factory.get_parent_selector()
             crossover = self.factory.get_crossover()
-            variable_updater = variable_updater = self.factory.get_variable_updater()
+            variable_updater = self.factory.get_variable_updater()
             gene_mutator = self.factory.get_gene_mutator()
-            for gv in self.ga_options.genetic_variables:
-                gv.gene_mutator = gene_mutator
+            for dv in self.ga_options.decision_variables:
+                dv.gene_mutator = gene_mutator
             population = Population(
                 self.ga_options,
                 chromosome_mutator=chromosome_mutator,
                 population_mutator=population_mutator,
                 exit_checker=exit_checker,
                 cost_finder=cost_finder,
                 population_immigrator=population_immigrator,
@@ -68,12 +68,12 @@
                 population.find_costs()
             if population.timeout_expired:
                 results.messages.append((message_levels.WARNING, "Timeout expired!"))
             best_individual = population.best_individual
             results.min_cost = population.min_cost
             results.number_of_iterations = population.population_generation
             for g in best_individual:
-                results.result_values[g.genetic_variable.variable_id] = g.variable_value
+                results.result_values[g.decision_variable.variable_id] = g.variable_value
         except Exception as ex:
             results.success = False
             results.messages.append((message_levels.ERROR, str(ex)))
         return results
```

### Comparing `gadapt-0.3.3/gadapt/factory/ga_base_factory.py` & `gadapt-0.3.4/gadapt/factory/ga_base_factory.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.3.3/gadapt/ga.py` & `gadapt-0.3.4/gadapt/ga.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 
 import sys
 from typing import List
 from gadapt.execution.ga_executor import GAExecutor
 from gadapt.factory.ga_base_factory import BaseGAFactory
 from gadapt.factory.ga_factory import GAFactory
-from gadapt.ga_model.genetic_variable import GeneticVariable
+from gadapt.ga_model.decision_variable import DecisionVariable
 from gadapt.ga_model.ga_options import GAOptions
 from gadapt.ga_model.ga_results import GAResults
 import gadapt.utils.ga_utils as ga_utils
 import gadapt.ga_model.definitions as definitions
 from gadapt.adapters.validation.common_options_validator import CommonOptionsValidator
 
 
@@ -34,15 +34,15 @@
             definitions.PARENT_DIVERSITY,
         ),
         number_of_mutation_chromosomes=-1,
         percentage_of_mutation_chromosomes=10.0,
         parent_diversity_mutation_chromosome_selection=definitions.ROULETTE_WHEEL,
         must_mutate_for_same_parents=True,
         chromosome_mutation=definitions.CROSS_DIVERSITY,
-        gene_mutation=definitions.EXTREME_POINTED,
+        gene_mutation=definitions.NORMAL_DISTRIBUTION,
         number_of_mutation_genes=-1,
         percentage_of_mutation_genes=10.0,
         cross_diversity_mutation_gene_selection=definitions.ROULETTE_WHEEL,
         immigration_number=0,
         logging=False,
         timeout=120,
         factory: BaseGAFactory = None,
@@ -186,15 +186,15 @@
         self.percentage_of_mutation_chromosomes = percentage_of_mutation_chromosomes
         self.number_of_mutation_genes = number_of_mutation_genes
         self.percentage_of_mutation_genes = percentage_of_mutation_genes
         self.chromosome_mutation = chromosome_mutation
         self.gene_mutation = gene_mutation
         self.immigration_number = immigration_number
         self.logging = logging
-        self._genetic_variables: List[GeneticVariable] = []
+        self._decision_variables: List[DecisionVariable] = []
         self.cross_diversity_mutation_gene_selection = (
             cross_diversity_mutation_gene_selection
         )
         self.parent_diversity_mutation_chromosome_selection = (
             parent_diversity_mutation_chromosome_selection
         )
         self.timeout = timeout
@@ -239,23 +239,25 @@
         Adds variables to be optimized.
         Args:
             min_value (float): lower bound of possible variable values
             max_value (float): upper bound of possible variable values
             step (float): the step that will be used in changing the
             variables values during the optimization
         """
+        if step < 0.000000000000001:
+            step = 0.000000000000001
         if (not isinstance(min_value, float) and not isinstance(min_value, int)) or (
             not isinstance(max_value, float) and not isinstance(max_value, int)
         ):
             raise Exception("min value, max value and step must be numerical values!")
-        genetic_variable = GeneticVariable(self._current_gv_id)
-        genetic_variable.min_value = min_value
-        genetic_variable.max_value = max_value
-        genetic_variable.step = step
-        self._genetic_variables.append(genetic_variable)
+        decision_variable = DecisionVariable(self._current_gv_id)
+        decision_variable.min_value = min_value
+        decision_variable.max_value = max_value
+        decision_variable.step = step
+        self._decision_variables.append(decision_variable)
         self._current_gv_id += 1
 
     @property
     def cost_function(self):
         """
         Custom function for the cost calculation (fitness). The optimisation goal
         is minimising the output of the cost function.
@@ -454,15 +456,15 @@
         """
         The type of mutation of genes in chromosomes.
 
         Supported values:
 
         **"cross_diversity"** - Considers the diversity of genes of the same
         type in the population. Lower diversity can mean
-        that this genetic variable approaches some local
+        that this decision variable approaches some local
         minimums, and therefore such genes increase the
         chance for mutation. Based on the calculated
         cross-diversity, chromosomes may be selected by
         one of the selection methods, which is
         determined by the value of the
         cross_diversity_mutation_gene_selection parameter.
 
@@ -479,20 +481,14 @@
         """
         Way of assigning the value to the gene
 
         Supported values:
 
         **"normal_distribution"** - assignes normally distributed random number to the variable selected for mutation
 
-                **"extreme_pointed"** - Considers the diversity of genes of the same
-        type in the population. Lower diversity can mean
-        that this genetic variable approaches sub-optimal value.
-                In that case, this mutator increases chances to mutate extreme values (minimum or maximum),
-                while keeping the chances to mutate to the other extreme value.
-
         **"random"** - Random values are assigned to genes
         """
         return self._gene_mutation
 
     @gene_mutation.setter
     def gene_mutation(self, value: str):
         self._gene_mutation = ga_utils.prepare_string(value)
```

### Comparing `gadapt-0.3.3/gadapt/ga_model/chromosome.py` & `gadapt-0.3.4/gadapt/ga_model/chromosome.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Chromosome
 """
 
 from typing import List
 from gadapt.ga_model.gene import Gene
-from gadapt.ga_model.genetic_variable import GeneticVariable
+from gadapt.ga_model.decision_variable import DecisionVariable
 from gadapt.ga_model.ranking_model import RankingModel
 from gadapt.operations.immigration.chromosome_immigration.base_chromosome_immigrator import (
     BaseChromosomeImmigrator,
 )
 from gadapt.operations.mutation.chromosome_mutation.base_chromosome_mutator import (
     BaseChromosomeMutator,
 )
@@ -193,15 +193,15 @@
         return self._father_id
 
     @father_id.setter
     def father_id(self, value: int):
         self._father_id = value
 
     def add_gene(
-        self, gen_var: GeneticVariable, gen_var_value: float = definitions.FLOAT_NAN
+        self, gen_var: DecisionVariable, gen_var_value: float = definitions.FLOAT_NAN
     ):
         """
         Adds a gene to the chromosome
         """
         g = Gene(gen_var, gen_var_value)
         self.append(g)
```

### Comparing `gadapt-0.3.3/gadapt/ga_model/definitions.py` & `gadapt-0.3.4/gadapt/ga_model/definitions.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,11 +15,12 @@
 AVG = "avg"
 MIN = "min"
 PARAM_SEPARATOR = ","
 FLOAT_NAN = float("NaN")
 NOT_IMPLEMENTED = "not implemented"
 EXTREME_POINTED = "extreme_pointed"
 NORMAL_DISTRIBUTION = "normal_distribution"
-POPULATION_MUTATOR_STRINGS = [COST_DIVERSITY, PARENT_DIVERSITY, RANDOM]
+POPULATION_MUTATOR_STRINGS = [COST_DIVERSITY, PARENT_DIVERSITY, RANDOM, CROSS_DIVERSITY]
 CHROMOSOME_MUTATOR_STRINGS = [RANDOM, CROSS_DIVERSITY]
+GENE_MUTATOR_STRINGS = [RANDOM, NORMAL_DISTRIBUTION]
 SELECTION_STRINGS = [RANDOM, FROM_TOP_TO_BOTTOM, ROULETTE_WHEEL, TOURNAMENT]
 EXIT_CRITERIA_STRINGS = [AVG_COST, MIN_COST, REQUESTED]
```

### Comparing `gadapt-0.3.3/gadapt/ga_model/ga_options.py` & `gadapt-0.3.4/gadapt/ga_model/ga_options.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 Genetic algorithm options
 """
 
 from typing import List
-from gadapt.ga_model.genetic_variable import GeneticVariable
+from gadapt.ga_model.decision_variable import DecisionVariable
 
 
 class GAOptions:
     def __init__(self, ga) -> None:
         """
         Genetic algorithm options class
         Args:
@@ -17,15 +17,15 @@
         self._population_size = ga.population_size
         self._cost_function = ga.cost_function
         self._immigration_number = ga.immigration_number
         self._set_number_of_mutation_chromosomes(ga)
         self._max_attempt_no = ga.max_attempt_no
         self._requested_cost = ga.requested_cost
         self._logging = ga.logging
-        self._genetic_variables = ga._genetic_variables
+        self._decision_variables = ga._decision_variables
         self._set_number_of_mutation_genes(ga)
         self._must_mutate_for_same_parents = ga.must_mutate_for_same_parents
         self._timeout = ga.timeout
 
     def _set_number_of_mutation_chromosomes(self, ga):
         if (
             (ga.number_of_mutation_chromosomes is not None)
@@ -62,15 +62,15 @@
         elif (
             (ga.percentage_of_mutation_genes is not None)
             and isinstance(ga.percentage_of_mutation_genes, float)
             and ga.percentage_of_mutation_genes >= 0.0
             and ga.percentage_of_mutation_genes <= 100
         ):
             self._number_of_mutation_genes = round(
-                float(len(self._genetic_variables))
+                float(len(self._decision_variables))
                 * (ga.percentage_of_mutation_genes / 100)
             )
         else:
             self._number_of_mutation_genes = ga.number_of_mutation_genes
 
     @property
     def requested_cost(self) -> float:
@@ -147,19 +147,19 @@
         return self._population_size
 
     @population_size.setter
     def population_size(self, value: int):
         self._population_size = value
 
     @property
-    def genetic_variables(self) -> List[GeneticVariable]:
+    def decision_variables(self) -> List[DecisionVariable]:
         """
-        Collection of genetic variables
+        Collection of decision variables
         """
-        return self._genetic_variables
+        return self._decision_variables
 
     @property
     def _abandon_number(self) -> int:
         return self._get_abandon_number()
 
     def _get_abandon_number(self) -> int:
         if self.population_size % 2 == 0:
```

### Comparing `gadapt-0.3.3/gadapt/ga_model/ga_results.py` & `gadapt-0.3.4/gadapt/ga_model/ga_results.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.3.3/gadapt/ga_model/gene.py` & `gadapt-0.3.4/gadapt/ga_model/gene.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,67 +1,67 @@
 """
 Gene
 """
 
 import math
-from gadapt.ga_model.genetic_variable import GeneticVariable
+from gadapt.ga_model.decision_variable import DecisionVariable
 from gadapt.ga_model.ranking_model import RankingModel
 import gadapt.adapters.string_operation.ga_strings as ga_strings
 import gadapt.ga_model.definitions as definitions
 
 
 class Gene(RankingModel):
     def __init__(self, gen_variable, var_value=None):
         """
         Gene class. Gene is a part of chromosome.
-        It contains concrete values for genetic variables.
+        It contains concrete values for decision variables.
         Args:
-            gen_variable: Genetic variable which defines the gene
+            gen_variable: Decision variable which defines the gene
             var_value: Value of the gene
         """
         super().__init__()
-        self.genetic_variable = gen_variable
+        self.decision_variable = gen_variable
         self.variable_value = var_value
         self._rank = -1
         self._cummulative_probability = definitions.FLOAT_NAN
         if self.variable_value is None or math.isnan(self.variable_value):
             self.set_random_value()
 
     def __str__(self) -> str:
         return self._to_string()
 
     def _to_string(self):
         return ga_strings.gene_to_string(self)
 
     @property
-    def genetic_variable(self) -> GeneticVariable:
+    def decision_variable(self) -> DecisionVariable:
         """
-        Genetic variable which defines the gene
+        Decision variable which defines the gene
         """
-        return self._genetic_variable
+        return self._decision_variable
 
-    @genetic_variable.setter
-    def genetic_variable(self, value: GeneticVariable):
-        if not isinstance(value, GeneticVariable):
+    @decision_variable.setter
+    def decision_variable(self, value: DecisionVariable):
+        if not isinstance(value, DecisionVariable):
             pass
             raise
-        self._genetic_variable = value
+        self._decision_variable = value
 
     @property
     def variable_value(self):
         """
         Value of the gene
         """
         return self._variable_value
 
     @variable_value.setter
     def variable_value(self, value):
         self._variable_value = value
 
     def mutate(self):
-        self.genetic_variable.gene_mutator.mutate(self)
+        self.decision_variable.gene_mutator.mutate(self)
 
     def set_random_value(self):
         """
         Sets a random value for the variable_value property
         """
-        self.variable_value = self.genetic_variable.make_random_value()
+        self.variable_value = self.decision_variable.make_random_value()
```

### Comparing `gadapt-0.3.3/gadapt/ga_model/genetic_variable.py` & `gadapt-0.3.4/gadapt/ga_model/decision_variable.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,41 +1,42 @@
 """
-Genetic variable
+Decision variable
 """
 
 import random
 import gadapt.ga_model.definitions as definitions
 
 
-class GeneticVariable:
+class DecisionVariable:
     def __init__(self, id: int) -> None:
         """
-        Genetic variable class defines genes.
-        Each gene has a reference to one genetic variable.
-        Genetic variable contains common values for genes: variable id, maximal\
+        Decision variable class defines genes.
+        Each gene has a reference to one decision variable.
+        Decision variable contains common values for genes: variable id, maximal\
             value, minimal value, step.
         Args:
-            id (int): identifier of the genetic variable
+            id (int): identifier of the decision variable
         """
         self.variable_id = id
         self._standard_deviation = definitions.FLOAT_NAN
         self._gene_mutator = None
+        self._initial_st_dev = -1.0
 
     def __eq__(self, other):
-        if not isinstance(other, GeneticVariable):
+        if not isinstance(other, DecisionVariable):
             return False
         return self.variable_id == other.variable_id
 
     def __hash__(self) -> int:
         return self.variable_id
 
     @property
     def variable_id(self) -> int:
         """
-        Unique ID for genetic variable
+        Unique ID for decision variable
         """
         return self._variable_id
 
     @variable_id.setter
     def variable_id(self, value: int):
         self._variable_id = value
 
@@ -69,47 +70,52 @@
         return self._step
 
     @step.setter
     def step(self, value: float):
         self._decimal_places = self._get_decimal_places(value)
         self._step = value
 
-    def _get_decimal_places(self, f: float) -> int:
-        dp = str(f)[::-1].find(".")
-        if dp == -1:
+    def _get_decimal_places(self, num):
+        num_str = str(num)
+        if 'e-' in num_str:
+            num_str = num_str.split('e-')[-1]
+            return int(num_str)
+        if '.' in num_str:
+            _, fractional_part = num_str.split('.')
+            return len(fractional_part)
+        else:
             return 0
-        return dp
 
     @property
     def decimal_places(self) -> int:
         """
         Number of decimal places of the gene value
         """
         return self._decimal_places
 
     @property
     def stacked(self) -> bool:
         """
-        Indicates if all genes have the same value for the same genetic variable
+        Indicates if all genes have the same value for the same decision variable
         """
         return self._stacked
 
     @stacked.setter
     def stacked(self, value: bool):
         self._stacked = value
 
     @property
-    def relative_standard_deviation(self) -> float:
+    def cross_diversity_coefficient(self) -> float:
         """
-        Relative standard deviation of all genes for the same genetic variable
+        Relative standard deviation of all genes for the same decision variable
         """
         return self._standard_deviation
 
-    @relative_standard_deviation.setter
-    def relative_standard_deviation(self, value: float):
+    @cross_diversity_coefficient.setter
+    def cross_diversity_coefficient(self, value: float):
         self._standard_deviation = value
 
     @property
     def gene_mutator(self):
         return self._gene_mutator
 
     @gene_mutator.setter
@@ -120,7 +126,15 @@
         """
         Makes random value, based on min value, max value, and step
         """
         number_of_steps = random.randint(
             0, round((self.max_value - self.min_value) / self.step)
         )
         return self.min_value + number_of_steps * self.step
+
+    @property
+    def initial_st_dev(self) -> float:
+        return self._initial_st_dev
+
+    @initial_st_dev.setter
+    def initial_st_dev(self, value: float):
+        self._initial_st_dev = value
```

### Comparing `gadapt-0.3.3/gadapt/ga_model/population.py` & `gadapt-0.3.4/gadapt/ga_model/population.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 Population
 """
 
+import math
 from typing import List, Tuple
 from gadapt.operations.exit_check.base_exit_checker import BaseExitChecker
 from gadapt.operations.cost_finding.base_cost_finder import BaseCostFinder
 from gadapt.operations.crossover.base_crossover import BaseCrossover
 from gadapt.ga_model.chromosome import Chromosome
 from gadapt.ga_model.ga_options import GAOptions
 from gadapt.ga_model.gene import Gene
@@ -22,14 +23,15 @@
     BasePopulationMutator,
 )
 from gadapt.operations.parent_selection.base_parent_selector import BaseParentSelector
 from gadapt.operations.variable_update.base_variable_updater import BaseVariableUpdater
 import gadapt.adapters.string_operation.ga_strings as ga_strings
 from datetime import datetime
 import gadapt.ga_model.definitions as definitions
+import gadapt.utils.ga_utils as ga_utils
 
 
 class Population:
     def __init__(
         self,
         options: GAOptions,
         chromosome_mutator: BaseChromosomeMutator,
@@ -76,14 +78,15 @@
         self.last_chromosome_id = 1
         self._population_generation = 0
         self.options = options
         self.chromosomes: List[Chromosome] = []
         self.generate_initial_population()
         self.start_time = datetime.now()
         self.timeout_expired = False
+        self.average_cost_step_in_first_population = float("NaN")
 
     def __iter__(self):
         return PopulationIterator(self)
 
     def __getitem__(self, index):
         return self.chromosomes[index]
 
@@ -385,25 +388,31 @@
         """
         if len(self) >= self.options.population_size:
             return
         if chromosome.chromosome_id is None or chromosome.chromosome_id == -1:
             chromosome.chromosome_id = self.last_chromosome_id
             self.last_chromosome_id += 1
         if len(chromosome) == 0:
-            for gv in self.options.genetic_variables:
-                g = Gene(gv)
+            for dv in self.options.decision_variables:
+                g = Gene(dv)
                 chromosome.append(g)
         self.append(chromosome)
 
     def update_variables(self):
         """
-        Updates genetic variables
+        Updates decision variables
         """
         self.variable_updater.update_variables(self)
 
+    def calculate_average_cost_step(self):
+        allocated_values = [c.cost_value for c in self.chromosomes if c.cost_value is not None and not math.isnan(c.cost_value)]        
+        if allocated_values:
+            return ga_utils.average_difference(allocated_values)
+        return float("NaN")
+
 
 class PopulationIterator:
     def __init__(self, population):
         self.population = population
         self.index = 0
 
     def __iter__(self):
```

### Comparing `gadapt-0.3.3/gadapt/ga_model/ranking_model.py` & `gadapt-0.3.4/gadapt/ga_model/ranking_model.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.3.3/gadapt/operations/cost_finding/base_cost_finder.py` & `gadapt-0.3.4/gadapt/operations/cost_finding/base_cost_finder.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from abc import ABC, abstractmethod
+import math
 import sys
 import traceback
 from gadapt.ga_model.chromosome import Chromosome
 
 
 class BaseCostFinder(ABC):
     """
@@ -16,15 +17,15 @@
         Args:
             cost_function: Function to execute
             c (Chromosome): The chromosome with
             genes containing values for the function execution.
         """
         dict = {}
         for g in c:
-            dict[g.genetic_variable.variable_id] = g.variable_value
+            dict[g.decision_variable.variable_id] = g.variable_value
         try:
             cost_value = cost_function(dict)
             c.cost_value = cost_value
         except Exception:
             print(Exception)
             traceback.print_exc()
             c.succ = False
@@ -38,7 +39,9 @@
         """
         Finds costs for the population
 
         Args:
             population (Population): The population to find costs for each chromosome
         """
         self._find_costs_for_population(population)
+        if math.isnan(population.average_cost_step_in_first_population):
+            population.average_cost_step_in_first_population = population.calculate_average_cost_step()
```

### Comparing `gadapt-0.3.3/gadapt/operations/cost_finding/elitism_cost_finder.py` & `gadapt-0.3.4/gadapt/operations/cost_finding/elitism_cost_finder.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.3.3/gadapt/operations/crossover/base_crossover.py` & `gadapt-0.3.4/gadapt/operations/crossover/base_crossover.py`

 * *Files 3% similar despite different names*

```diff
@@ -49,44 +49,44 @@
         Returns:
             Chromosome: the first offspring chromosome
             Chromosome: the second offspring chromosome
         """
 
         def get_genetic_diversity(g_m: Gene, g_f: Gene) -> float:
             return abs(g_m.variable_value - g_f.variable_value) / (
-                g_f.genetic_variable.max_value - g_f.genetic_variable.min_value
+                g_f.decision_variable.max_value - g_f.decision_variable.min_value
             )
 
         if len(mother) != len(father):
             raise Exception("Mother and father must have the same number of genes!")
         offspring1 = Chromosome(self._mutator, self._immigrator, population_generation)
         offspring2 = Chromosome(self._mutator, self._immigrator, population_generation)
         self.number_of_genes = len(father)
         genetic_diversity = []
         for self._current_gene_number in range(self.number_of_genes):
             mother_gene, father_gene = self._get_mother_father_genes(mother, father)
-            genetic_variable_father = father_gene.genetic_variable
-            genetic_variable_mother = mother_gene.genetic_variable
-            if genetic_variable_father != genetic_variable_mother:
-                genetic_variable_mother = next(
+            decision_variable_father = father_gene.decision_variable
+            decision_variable_mother = mother_gene.decision_variable
+            if decision_variable_father != decision_variable_mother:
+                decision_variable_mother = next(
                     (
-                        item.genetic_variable
+                        item.decision_variable
                         for item in mother
-                        if item.genetic_variable == genetic_variable_father
+                        if item.decision_variable == decision_variable_father
                     ),
                     None,
                 )
-            if genetic_variable_mother is None:
+            if decision_variable_mother is None:
                 raise Exception(
                     "chromosomes in crossover do not have the same structure!"
                 )
             genetic_diversity.append(get_genetic_diversity(mother_gene, father_gene))
             var1, var2 = self._combine(mother_gene, father_gene)
-            offspring1.add_gene(genetic_variable_father, var1)
-            offspring2.add_gene(genetic_variable_father, var2)
+            offspring1.add_gene(decision_variable_father, var1)
+            offspring2.add_gene(decision_variable_father, var2)
         parrents_diversity = round(ga_utils.average(genetic_diversity), 2)
         offspring1.parent_diversity = parrents_diversity
         offspring2.parent_diversity = parrents_diversity
         offspring1.mutation_on_both_sides = self._mutation_on_both_sides
         offspring2.mutation_on_both_sides = self._mutation_on_both_sides
         offspring1.mother_id = mother.chromosome_id
         offspring2.mother_id = mother.chromosome_id
```

### Comparing `gadapt-0.3.3/gadapt/operations/crossover/uniform_crossover.py` & `gadapt-0.3.4/gadapt/operations/crossover/uniform_crossover.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.3.3/gadapt/operations/exit_check/base_exit_checker.py` & `gadapt-0.3.4/gadapt/operations/exit_check/base_exit_checker.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.3.3/gadapt/operations/exit_check/requested_cost_exit_checker.py` & `gadapt-0.3.4/gadapt/operations/exit_check/requested_cost_exit_checker.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.3.3/gadapt/operations/gene_combination/base_gene_combination.py` & `gadapt-0.3.4/gadapt/operations/gene_combination/base_gene_combination.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.3.3/gadapt/operations/gene_combination/blending_gene_combination.py` & `gadapt-0.3.4/gadapt/operations/gene_combination/blending_gene_combination.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,25 +8,25 @@
     Blending gene combination combines
     gene values from the two parents into new variable values in offsprings.
     One value of the offspring variable comes from a combination of the two
     corresponding values of the parental genes
     """
 
     def _combine_genes(self, mother_gene: Gene, father_gene: Gene):
-        genetic_variable = father_gene.genetic_variable
+        decision_variable = father_gene.decision_variable
         val_father = father_gene.variable_value
         val_mother = mother_gene.variable_value
         x = 1
         if val_mother > val_father:
             x = -1
         beta_steps = random.randint(
-            0, round(abs((val_father - val_mother) / genetic_variable.step))
+            0, round(abs((val_father - val_mother) / decision_variable.step))
         )
         val1 = round(
-            val_father - (beta_steps * x) * genetic_variable.step,
-            genetic_variable.decimal_places,
+            val_father - (beta_steps * x) * decision_variable.step,
+            decision_variable.decimal_places,
         )
         val2 = round(
-            val_mother + (beta_steps * x) * genetic_variable.step,
-            genetic_variable.decimal_places,
+            val_mother + (beta_steps * x) * decision_variable.step,
+            decision_variable.decimal_places,
         )
         return val1, val2
```

### Comparing `gadapt-0.3.3/gadapt/operations/immigration/chromosome_immigration/base_chromosome_immigrator.py` & `gadapt-0.3.4/gadapt/operations/immigration/chromosome_immigration/base_chromosome_immigrator.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.3.3/gadapt/operations/immigration/population_immigration/common_population_immigrator.py` & `gadapt-0.3.4/gadapt/operations/immigration/population_immigration/common_population_immigrator.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.3.3/gadapt/operations/mutation/chromosome_mutation/base_chromosome_mutator.py` & `gadapt-0.3.4/gadapt/operations/mutation/chromosome_mutation/base_chromosome_mutator.py`

 * *Files 11% similar despite different names*

```diff
@@ -19,20 +19,20 @@
 
     @abstractmethod
     def _mutate_chromosome(self, c, number_of_mutation_genes: int):
         pass
 
     def _set_gene_value(self, g, c):
         g.variable_value = round(
-            g.genetic_variable.make_random_value(), g.genetic_variable.decimal_places
+            g.decision_variable.make_random_value(), g.decision_variable.decimal_places
         )
         self._gene_mutated(g, c)
 
     def _gene_mutated(self, g, c):
-        c.mutated_variables_id_list.append(g.genetic_variable.variable_id)
+        c.mutated_variables_id_list.append(g.decision_variable.variable_id)
 
     def _chromosome_mutated(self, c):
         c.is_mutated = True
         if c.first_mutant_generation == 0:
             c.first_mutant_generation += 1
         c.last_mutant_generation = 1
```

### Comparing `gadapt-0.3.3/gadapt/operations/mutation/chromosome_mutation/random_chromosome_mutator.py` & `gadapt-0.3.4/gadapt/operations/mutation/chromosome_mutation/random_chromosome_mutator.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.3.3/gadapt/operations/mutation/gene_mutation/extreme_pointed_gene_mutator.py` & `gadapt-0.3.4/gadapt/operations/mutation/gene_mutation/extreme_pointed_gene_mutator.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,55 +2,56 @@
 from gadapt.ga_model.gene import Gene
 from gadapt.operations.mutation.gene_mutation.random_gene_mutator import (
     RandomGeneMutator,
 )
 from gadapt.utils.ga_utils import get_rand_bool, get_rand_bool_with_probability
 
 
+# *** Obsolete ***
 class ExtremePointedGeneMutator(RandomGeneMutator):
 
     def _make_mutated_value(self, g: Gene):
         return self._make_mutation(g)
 
     def _make_rounded_random_value_below_or_above(self, g: Gene):
         return round(
-            self._make_random_value_below_or_above(g), g.genetic_variable.decimal_places
+            self._make_random_value_below_or_above(g), g.decision_variable.decimal_places
         )
 
     def _make_random_value_below_or_above(self, g: Gene):
         if get_rand_bool():
             return self._make_random_value_above(g)
         return self._make_random_value_below(g)
 
     def _make_random_value_below(self, g: Gene):
-        if g.variable_value == g.genetic_variable.min_value:
-            return g.genetic_variable.make_random_value()
+        if g.variable_value == g.decision_variable.min_value:
+            return g.decision_variable.make_random_value()
         number_of_steps = random.randint(
             0,
             round(
-                (g.variable_value - g.genetic_variable.min_value)
-                / g.genetic_variable.step
+                (g.variable_value - g.decision_variable.min_value)
+                / g.decision_variable.step
             ),
         )
-        return g.genetic_variable.min_value + number_of_steps * g.genetic_variable.step
+        return g.decision_variable.min_value + number_of_steps * g.decision_variable.step
 
     def _make_random_value_above(self, g: Gene):
-        if g.variable_value == g.genetic_variable.max_value:
-            return g.genetic_variable.make_random_value()
+        if g.variable_value == g.decision_variable.max_value:
+            return g.decision_variable.make_random_value()
         number_of_steps = random.randint(
             0,
             round(
-                (g.genetic_variable.max_value - g.variable_value)
-                / g.genetic_variable.step
+                (g.decision_variable.max_value - g.variable_value)
+                / g.decision_variable.step
             ),
         )
-        return g.variable_value + number_of_steps * g.genetic_variable.step
+        return g.variable_value + number_of_steps * g.decision_variable.step
 
     def _get_mutate_func(self, g: Gene):
-        prob = g.genetic_variable.relative_standard_deviation
+        prob = g.decision_variable.cross_diversity_coefficient
         if prob > 1.0:
             prob = 1.0
         should_mutate_random = get_rand_bool_with_probability(prob)
         if should_mutate_random:
             return super()._make_mutated_value
         else:
             return self._make_rounded_random_value_below_or_above
```

### Comparing `gadapt-0.3.3/gadapt/operations/mutation/population_mutation/base_population_mutator.py` & `gadapt-0.3.4/gadapt/operations/mutation/population_mutation/base_population_mutator.py`

 * *Files 7% similar despite different names*

```diff
@@ -43,7 +43,10 @@
         lst = [c for c in population if (unallocated_chromosomes_condition(c))]
         if sort_key_function is not None:
             lst.sort(key=sort_key_function)
         return lst
 
     def _sort_key_random(self, c: Chromosome):
         return random.random()
+    
+    def requires_continuous_execution_in_composed_mutation(self) -> bool:
+        return False
```

### Comparing `gadapt-0.3.3/gadapt/operations/mutation/population_mutation/composed_population_mutator.py` & `gadapt-0.3.4/gadapt/operations/mutation/population_mutation/composed_population_mutator.py`

 * *Files 26% similar despite different names*

```diff
@@ -24,12 +24,22 @@
     def _mutate_population(self, population, number_of_mutation_chromosomes):
         if population is None:
             raise Exception("Population must not be null")
         if len(self.mutators) == 0:
             raise Exception("at least one mutator must be added")
         random.shuffle(self.mutators)
         nmc = 0
-        for m in self.mutators:
-            if nmc < number_of_mutation_chromosomes:
-                nmc += m._mutate_population(
+        if not self.requires_continuous_execution_in_composed_mutation():
+            nmc = self.mutators[0]._mutate_population(
                     population, number_of_mutation_chromosomes - nmc
                 )
+        else:
+            for m in self.mutators:            
+                if nmc < number_of_mutation_chromosomes:
+                    mc = m._mutate_population(
+                        population, number_of_mutation_chromosomes - nmc
+                    )
+                    nmc += mc
+        return nmc
+    
+    def requires_continuous_execution_in_composed_mutation(self):
+        return all([m.requires_continuous_execution_in_composed_mutation() for m in self.mutators])
```

### Comparing `gadapt-0.3.3/gadapt/operations/mutation/population_mutation/cost_diversity_population_mutator.py` & `gadapt-0.3.4/gadapt/operations/mutation/population_mutation/parent_diversity_population_mutator.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,56 +1,50 @@
-import math
+from ast import List
+import random
+from gadapt.ga_model.chromosome import Chromosome
 from gadapt.operations.mutation.population_mutation.base_population_mutator import (
     BasePopulationMutator,
 )
-import gadapt.utils.ga_utils as ga_utils
-import statistics as stat
+from gadapt.operations.sampling.base_sampling import BaseSampling
 
 
-class CostDiversityPopulationMutator(BasePopulationMutator):
+class ParentDiversityPopulationMutator(BasePopulationMutator):
     """
-    Population mutator based on cost diversity
+    Population mutator based on parent diversity
     """
 
-    def __init__(
-        self,
-        population_mutator_for_execution: BasePopulationMutator,
-    ) -> None:
+    def __init__(self, sampling: BaseSampling) -> None:
         super().__init__()
-        self._population_mutator_for_execution = population_mutator_for_execution
+        self._sampling = sampling
 
-    def _get_number_of_mutation_cromosomes(
-        self, allocated_chromosomes, number_of_mutation_chromosomes
-    ) -> int:
-        def get_mutation_rate() -> float:
-            current_costs = []
-            current_min_value = min(allocated_chromosomes, key=lambda x: x.cost_value)
-            for c in allocated_chromosomes:
-                # current_costs.append(c.cost_value - self.first_cost)
-                # current_costs.append(c.cost_value)
-                current_costs.append(c.cost_value - current_min_value.cost_value)
-            stddev = stat.stdev(current_costs)
-            avg = abs(ga_utils.average(current_costs))
-            if avg == 0:
-                rel_stddev = 0
-            else:
-                rel_stddev = stddev / avg
-            if rel_stddev > 1:
-                return 0
-            return 1 - rel_stddev
-
-        mutation_rate = get_mutation_rate()
-        f_return_value = mutation_rate * float(number_of_mutation_chromosomes)
-        return round(f_return_value)
+    def _sort_key_parent_diversity_random(self, c: Chromosome):
+        return (c.parent_diversity, random.random())
 
     def _mutate_population(self, population, number_of_mutation_chromosomes):
         if population is None:
             raise Exception("Population must not be null")
-        allocated_chromosomes = [c for c in population if not math.isnan(c.cost_value)]
-        current_number_of_mutation_chromosomes = (
-            self._get_number_of_mutation_cromosomes(
-                allocated_chromosomes, number_of_mutation_chromosomes
-            )
-        )
-        return self._population_mutator_for_execution._mutate_population(
-            population, current_number_of_mutation_chromosomes
+        unallocated_chromosomes: List[Chromosome] = self._get_unallocated_chromosomes(
+            population, self._sort_key_parent_diversity_random
         )
+        chromosomes_for_mutation: List[Chromosome] = []
+        if population.options.must_mutate_for_same_parents:
+            chromosomes_for_mutation = [
+                c for c in unallocated_chromosomes if c.parent_diversity == 0
+            ]
+        chromosomes_for_mutation_count = len(chromosomes_for_mutation)
+        rest_number = number_of_mutation_chromosomes - chromosomes_for_mutation_count
+        if rest_number > 0:
+            if population.options.must_mutate_for_same_parents:
+                chromosomes_for_mutation = [
+                    c for c in unallocated_chromosomes if (not c.parent_diversity == 0)
+                ]
+            else:
+                chromosomes_for_mutation = [c for c in unallocated_chromosomes]
+            chromosomes_for_mutation = self._sampling.get_sample(
+                chromosomes_for_mutation, rest_number, lambda c: c.parent_diversity
+            )
+        for c in chromosomes_for_mutation:
+            c.mutate(population.options.number_of_mutation_genes)
+        return len(chromosomes_for_mutation)
+
+    def requires_continuous_execution_in_composed_mutation(self) -> bool:
+        return True
```

### Comparing `gadapt-0.3.3/gadapt/operations/mutation/population_mutation/random_population_mutator.py` & `gadapt-0.3.4/gadapt/operations/mutation/population_mutation/random_population_mutator.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,7 +20,10 @@
         )
         chromosomes_for_mutation = unallocated_chromosomes[
             :number_of_mutation_chromosomes
         ]
         for c in chromosomes_for_mutation:
             c.mutate(number_of_mutation_genes)
         return number_of_mutation_chromosomes
+
+    def requires_continuous_execution_in_composed_mutation(self) -> bool:
+        return True
```

### Comparing `gadapt-0.3.3/gadapt/operations/parent_selection/base_parent_selector.py` & `gadapt-0.3.4/gadapt/operations/parent_selection/base_parent_selector.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.3.3/gadapt/operations/parent_selection/sampling_parent_selector.py` & `gadapt-0.3.4/gadapt/operations/parent_selection/sampling_parent_selector.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.3.3/gadapt/operations/sampling/base_sampling.py` & `gadapt-0.3.4/gadapt/operations/sampling/base_sampling.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.3.3/gadapt/operations/sampling/roulette_wheel_sampling.py` & `gadapt-0.3.4/gadapt/operations/sampling/roulette_wheel_sampling.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,14 @@
         rank = 0
         unallocated_members = [rm for rm in lst]
         unallocated_members.sort(key=self._sort_key, reverse=True)
         members_for_action = []
         for j in range(self.max_num):
             if len(unallocated_members) == 0:
                 continue
-            i_c_p_l = 0
             for i_c_p_l, m in enumerate(unallocated_members):
                 m.action_probability = cummultative_probability_list[i_c_p_l]
             rnd_value = random.random()
             max_prob = (
                 max(unallocated_members, key=lambda m: m.action_probability)
             ).action_probability
             rnd_value = rnd_value * max_prob
```

### Comparing `gadapt-0.3.3/gadapt/operations/sampling/tournament_sampling.py` & `gadapt-0.3.4/gadapt/operations/sampling/tournament_sampling.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.3.3/gadapt/operations/variable_update/common_variable_updater.py` & `gadapt-0.3.4/gadapt/operations/variable_update/common_variable_updater.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,49 +1,63 @@
 import statistics as stat
-from gadapt.ga_model.genetic_variable import GeneticVariable
+from gadapt.ga_model.decision_variable import DecisionVariable
 import gadapt.utils.ga_utils as ga_utils
 
 
 class CommonVariableUpdater:
     """
     Common variable updater
     """
 
     def update_variables(self, population):
-        def scale_values(gv: GeneticVariable, values):
-            min_val = min(values)
-            return [(v - min_val) / (gv.max_value - gv.min_value) for v in values]
+
+        def scale_values(dv: DecisionVariable, values):
+            scaled_values = []
+            if dv.min_value == dv.max_value:
+                return [0.5] * len(values)  # If min_val and max_val are the same, return a list of 0.5s
+
+            for value in values:
+                scaled_value = (value - dv.min_value) / (dv.max_value - dv.min_value)
+                scaled_values.append(scaled_value)
+            return scaled_values
+
+        # def scale_values(data):
+        #     min_val = min(data)
+        #     max_val = max(data)
+        #     scaled_data = [(x - min_val) / (max_val - min_val) for x in data]
+        #     return scaled_data
 
         unique_values_per_variables = {}
         values_per_variables = {}
         for c in population:
             if c.is_immigrant:
                 continue
             for g in c:
                 unique_var_values = unique_values_per_variables.get(
-                    g.genetic_variable, None
+                    g.decision_variable, None
                 )
-                var_values = values_per_variables.get(g.genetic_variable, None)
+                var_values = values_per_variables.get(g.decision_variable, None)
                 if unique_var_values is None:
                     unique_var_values = set()
-                    unique_values_per_variables[g.genetic_variable] = unique_var_values
+                    unique_values_per_variables[g.decision_variable] = unique_var_values
                 if var_values is None:
                     var_values = []
-                    values_per_variables[g.genetic_variable] = var_values
+                    values_per_variables[g.decision_variable] = var_values
                 unique_var_values.add(g.variable_value)
                 var_values.append(g.variable_value)
         for key in unique_values_per_variables:
             if len(unique_values_per_variables[key]) == 1:
                 key.stacked = True
             else:
                 key.stacked = False
         for key in values_per_variables:
             if key.stacked:
-                key.relative_standard_deviation = 0.0
+                key.cross_diversity_coefficient = 0.0
                 continue
-            scaled_values = scale_values(key, values_per_variables[key])
-            range = max(scaled_values) - min(scaled_values)
-            if range == 0:
-                key.relative_standard_deviation = 0.0
+            values_scaled = scale_values(key, values_per_variables[key])
+            st_dev = stat.stdev(values_scaled)
+            if key.initial_st_dev < 0:
+                key.initial_st_dev = st_dev
+            if max(values_scaled) - min(values_scaled) == 0:
+                key.cross_diversity_coefficient = 0.0
             else:
-                rel_st_dev = stat.stdev(scaled_values) / ga_utils.average(scaled_values)
-                key.relative_standard_deviation = range / rel_st_dev
+                key.cross_diversity_coefficient = st_dev / key.initial_st_dev
```

### Comparing `gadapt-0.3.3/gadapt/utils/ga_utils.py` & `gadapt-0.3.4/gadapt/utils/ga_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -106,7 +106,15 @@
     return str_return
 
 
 def normally_distributed_random(mean, std_dev, lower_bound, upper_bound):
     num = np.random.normal(mean, std_dev)
     num = np.clip(num, lower_bound, upper_bound)
     return num
+
+def average_difference(diff_list):
+    if len(diff_list) < 2:
+        return float("NaN")
+    diff_list.sort()
+    differences = [diff_list[i+1] - diff_list[i] for i in range(len(diff_list)-1)]
+    avg_difference = sum(differences) / len(differences)
+    return avg_difference
```

### Comparing `gadapt-0.3.3/gadapt.egg-info/PKG-INFO` & `gadapt-0.3.4/gadapt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gadapt
-Version: 0.3.3
+Version: 0.3.4
 Summary: GAdapt: A Python Library for        Self-Adaptive Genetic Algorithm.
 Home-page: https://github.com/bpzoran/gadapt
 Author: Zoran Jankovic
 Author-email: bpzoran@yahoo.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
@@ -165,17 +165,16 @@
 **must_mutate_for_same_parents**=*True* - Indicates if completely the same parents must influence mutation for their children. In other words, each child will be mutated if it has parents with a diversity value of 0. If *must_mutate_for_same_parents* has the value True, the number of mutated chromosomes can outreach value determined by *number_of_mutation_chromosomes* or *percentage_of_mutation_chromosomes*
 
 **chromosome_mutation**=*"cross_diversity"* - The type of gene selection in chromosomes for mutation  
 Supported values:
 - *"cross_diversity"* - Considers the diversity of genes of the same type in the population. Lower diversity can mean that this genetic variable approaches some local minimums, and therefore such genes increase the chance for mutation. Based on the calculated cross-diversity, chromosomes may be selected by one of the selection methods, which is determined by the value of the *cross_diversity_mutation_gene_selection* parameter.  
 - *"random"* - Genes are randomly selected for the mutation
 
-**gene_mutation**=*"extreme_pointed"* - The type of assigning mutated values to genes
+**gene_mutation**=*"normal_distribution"* - The type of assigning mutated values to genes
 Supported values:
-- *"extreme_pointed"* - Considers the diversity of genes of the same type in the population. Lower diversity can mean that this genetic variable approaches sub-optimal value. In that case, this mutator increases chances to mutate extreme values (minimum or maximum), while keeping the chances to mutate to the other extreme value. 
 - *"normal_distribution"* - assignes normally distributed random number to the variable selected for mutation
 - *"random"* - Random values are assigned to genes
 
 **cross_diversity_mutation_gene_selection**=*"roulette_wheel"* - the selection algorithm for mutating chromosomes when *chromosome_mutation* has value *"cross_diversity"*. It only applies when *chromosome_mutation* has value *"cross_diversity"* . It determines the way how genes are to be selected based on the cross-diversity.  
 Supported values:
 - *"roulette_wheel"* - The Roulette Wheel selection algorithm (also known as "Weighted Random Pairing"). The probabilities assigned to the genes to be mutated are inversely proportional to their cross-diversity. A gene with the lowest cross-diversity has the greatest probability of mutation, while the gene with the highest cross-diversity has the lowest probability of mutation.  
 - *"tournament"* - The Tournament selection algorithm. It randomly picks small subsets (groups) of genes, and genes with the lowest cross-diversity in subsets are chosen to be mutated. *"tournament"* can have an additional parameter separated from the *"tournament"* keyword by the comma. The other value represents a group size. For example, *"tournament,3"* means that the tournament mutation selection algorithm is chosen, and each group contains up to 3 members. The default group size is 4.
```

### Comparing `gadapt-0.3.3/gadapt.egg-info/SOURCES.txt` & `gadapt-0.3.4/gadapt.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -21,19 +21,19 @@
 gadapt/execution/__init__.py
 gadapt/execution/ga_executor.py
 gadapt/factory/__init__.py
 gadapt/factory/ga_base_factory.py
 gadapt/factory/ga_factory.py
 gadapt/ga_model/__init__.py
 gadapt/ga_model/chromosome.py
+gadapt/ga_model/decision_variable.py
 gadapt/ga_model/definitions.py
 gadapt/ga_model/ga_options.py
 gadapt/ga_model/ga_results.py
 gadapt/ga_model/gene.py
-gadapt/ga_model/genetic_variable.py
 gadapt/ga_model/message_levels.py
 gadapt/ga_model/population.py
 gadapt/ga_model/ranking_model.py
 gadapt/operations/__init__.py
 gadapt/operations/cost_finding/__init__.py
 gadapt/operations/cost_finding/base_cost_finder.py
 gadapt/operations/cost_finding/elitism_cost_finder.py
@@ -65,14 +65,15 @@
 gadapt/operations/mutation/gene_mutation/extreme_pointed_gene_mutator.py
 gadapt/operations/mutation/gene_mutation/normal_distribution_gene_mutator.py
 gadapt/operations/mutation/gene_mutation/random_gene_mutator.py
 gadapt/operations/mutation/population_mutation/__init__.py
 gadapt/operations/mutation/population_mutation/base_population_mutator.py
 gadapt/operations/mutation/population_mutation/composed_population_mutator.py
 gadapt/operations/mutation/population_mutation/cost_diversity_population_mutator.py
+gadapt/operations/mutation/population_mutation/cross_diversity_population_mutator.py
 gadapt/operations/mutation/population_mutation/parent_diversity_population_mutator.py
 gadapt/operations/mutation/population_mutation/random_population_mutator.py
 gadapt/operations/parent_selection/__init__.py
 gadapt/operations/parent_selection/base_parent_selector.py
 gadapt/operations/parent_selection/sampling_parent_selector.py
 gadapt/operations/sampling/__init__.py
 gadapt/operations/sampling/base_sampling.py
```

### Comparing `gadapt-0.3.3/pyproject.toml` & `gadapt-0.3.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gadapt-0.3.3/setup.py` & `gadapt-0.3.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="gadapt",
-    version="0.3.3",
+    version="0.3.4",
     author="Zoran Jankovic",
     author_email="bpzoran@yahoo.com",
     url="https://github.com/bpzoran/gadapt",
     packages=find_packages(),
     long_description=open("README.md").read(),
     # Specify the content type explicitly
     long_description_content_type="text/markdown",
```

