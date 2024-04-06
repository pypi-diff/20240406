# Comparing `tmp/kevin-toolbox-dev-1.3.3.tar.gz` & `tmp/kevin-toolbox-dev-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/kevin-toolbox-dev-1.3.3.tar", last modified: Mon Apr  1 10:53:27 2024, max compression
+gzip compressed data, was "dist/kevin-toolbox-dev-1.3.4.tar", last modified: Sat Apr  6 13:16:20 2024, max compression
```

## Comparing `kevin-toolbox-dev-1.3.3.tar` & `kevin-toolbox-dev-1.3.4.tar`

### file list

```diff
@@ -1,412 +1,414 @@
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-01 10:53:27.000000 kevin-toolbox-dev-1.3.3/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2008 2024-04-01 10:53:27.000000 kevin-toolbox-dev-1.3.3/PKG-INFO
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1407 2024-04-01 10:50:13.000000 kevin-toolbox-dev-1.3.3/README.md
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-01 10:53:26.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      410 2024-04-01 10:53:25.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/__init__.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-01 10:53:26.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/computer_science/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-12-01 13:56:40.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/computer_science/__init__.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-01 10:53:26.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/computer_science/algorithm/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        1 2023-03-04 15:12:36.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/computer_science/algorithm/__init__.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-01 10:53:26.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/computer_science/algorithm/cache_manager/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       41 2024-03-03 16:14:42.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/computer_science/algorithm/cache_manager/__init__.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-01 10:53:26.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/computer_science/algorithm/cache_manager/cache/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       70 2024-03-03 16:52:11.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/computer_science/algorithm/cache_manager/cache/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2229 2024-03-04 07:36:13.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/computer_science/algorithm/cache_manager/cache/cache_base.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      963 2024-03-04 07:36:45.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/computer_science/algorithm/cache_manager/cache/memo_cache.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     9151 2024-03-04 13:32:58.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/computer_science/algorithm/cache_manager/cache_manager.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-01 10:53:26.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/computer_science/algorithm/cache_manager/strategy/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      199 2024-03-04 13:33:39.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/computer_science/algorithm/cache_manager/strategy/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      770 2024-03-04 12:38:04.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/computer_science/algorithm/cache_manager/strategy/fifo_strategy.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2557 2024-03-04 13:04:24.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/computer_science/algorithm/cache_manager/strategy/lfu_strategy.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1376 2024-03-04 09:11:55.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/computer_science/algorithm/cache_manager/strategy/lru_strategy.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1106 2024-03-04 13:04:24.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/computer_science/algorithm/cache_manager/strategy/lst_strategy.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1457 2024-03-04 08:20:39.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/computer_science/algorithm/cache_manager/strategy/strategy_base.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-01 10:53:26.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/computer_science/algorithm/cache_manager/test/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-03-04 08:47:42.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/computer_science/algorithm/cache_manager/test/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1108 2024-03-03 17:42:33.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/computer_science/algorithm/cache_manager/test/test_cache_builder.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     7944 2024-03-04 13:21:47.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/computer_science/algorithm/cache_manager/test/test_cache_manager.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     5310 2024-03-04 13:07:15.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/computer_science/algorithm/cache_manager/test/test_cache_strategy.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      835 2024-03-03 16:15:58.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/computer_science/algorithm/cache_manager/variable.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-01 10:53:26.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/computer_science/algorithm/combinatorial_optimization/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      142 2023-03-05 16:13:01.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/computer_science/algorithm/combinatorial_optimization/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1832 2023-03-31 07:27:37.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/computer_science/algorithm/combinatorial_optimization/get_subset_with_largest_product.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-01 10:53:26.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/computer_science/algorithm/combinatorial_optimization/test/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-07-30 14:12:33.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/computer_science/algorithm/combinatorial_optimization/test/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1914 2023-06-12 05:50:08.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/computer_science/algorithm/combinatorial_optimization/test/test_get_subset_with_largest_product.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2078 2023-06-12 05:50:08.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/computer_science/algorithm/combinatorial_optimization/test/test_zero_one_knapsack_problem.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2819 2023-03-05 16:40:22.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/computer_science/algorithm/combinatorial_optimization/zero_one_knapsack_problem.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-01 10:53:27.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/computer_science/algorithm/execution_graph/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-08-04 08:58:16.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/computer_science/algorithm/execution_graph/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3297 2023-08-04 11:56:33.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/computer_science/algorithm/execution_graph/jump_node.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3189 2023-08-04 11:50:17.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/computer_science/algorithm/execution_graph/random_node.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3267 2023-08-04 11:50:17.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/computer_science/algorithm/execution_graph/simple_node.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-01 10:53:27.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/computer_science/algorithm/for_dict/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       37 2023-06-12 05:50:08.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/computer_science/algorithm/for_dict/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      666 2023-06-19 08:36:11.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/computer_science/algorithm/for_dict/deep_update.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-01 10:53:27.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/computer_science/algorithm/for_seq/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      121 2023-08-15 11:37:21.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/computer_science/algorithm/for_seq/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2544 2023-08-15 11:44:17.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/computer_science/algorithm/for_seq/chunk_generator.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1046 2023-06-12 05:50:08.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/computer_science/algorithm/for_seq/flatten_list.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      309 2023-06-12 05:50:08.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/computer_science/algorithm/for_seq/get_subsets.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-01 10:53:27.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/computer_science/algorithm/locks/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       35 2023-04-21 13:18:26.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/computer_science/algorithm/locks/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2492 2023-04-24 08:04:07.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/computer_science/algorithm/locks/mutex_lock.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-01 10:53:27.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/computer_science/algorithm/parallel_and_concurrent/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       55 2023-08-15 13:22:31.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/computer_science/algorithm/parallel_and_concurrent/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      896 2023-07-28 14:07:18.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/computer_science/algorithm/parallel_and_concurrent/async_executor.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3126 2023-08-15 13:59:27.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/computer_science/algorithm/parallel_and_concurrent/multi_thread_execute.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-01 10:53:27.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/computer_science/algorithm/pareto_front/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       68 2024-01-05 07:20:07.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/computer_science/algorithm/pareto_front/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3008 2024-01-05 07:20:45.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/computer_science/algorithm/pareto_front/get_pareto_points_idx.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-01 10:53:27.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/computer_science/algorithm/registration/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       49 2023-06-12 14:36:27.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/computer_science/algorithm/registration/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)    17385 2024-03-04 11:52:32.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/computer_science/algorithm/registration/registry.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-01 10:53:27.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/computer_science/algorithm/scheduler/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       76 2023-06-02 12:00:07.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/computer_science/algorithm/scheduler/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)    12194 2023-07-26 06:32:19.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/computer_science/algorithm/scheduler/strategy_manager.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     4470 2023-07-25 12:43:34.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/computer_science/algorithm/scheduler/trigger.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-01 10:53:27.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/computer_science/algorithm/search/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       41 2023-03-20 13:18:25.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/computer_science/algorithm/search/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1013 2023-03-04 15:58:55.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/computer_science/algorithm/search/binary_search.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-01 10:53:27.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/computer_science/algorithm/statistician/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      167 2023-11-13 07:53:49.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/computer_science/algorithm/statistician/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     6098 2023-11-13 07:53:49.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/computer_science/algorithm/statistician/accumulator_base.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2570 2023-11-13 07:54:37.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/computer_science/algorithm/statistician/average_accumulator.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     5363 2023-11-13 07:58:15.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/computer_science/algorithm/statistician/exponential_moving_average.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-01 10:53:27.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/computer_science/algorithm/statistician/init_var/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      121 2023-11-13 07:46:03.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/computer_science/algorithm/statistician/init_var/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      769 2023-11-13 07:46:03.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/computer_science/algorithm/statistician/init_var/init_by_data_format.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      572 2023-11-13 07:46:03.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/computer_science/algorithm/statistician/init_var/init_by_like.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-01 10:53:27.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/computer_science/algorithm/utils/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-08 14:31:25.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/computer_science/algorithm/utils/__init__.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-01 10:53:27.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/computer_science/data_structure/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       31 2023-03-22 06:30:28.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/computer_science/data_structure/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     6206 2023-06-21 01:55:31.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/computer_science/data_structure/executor.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-01 10:53:27.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/dangerous/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       93 2023-03-29 12:29:14.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/dangerous/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2898 2023-03-31 07:27:38.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/dangerous/dump_into_pickle_with_executor_attached.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-01 10:53:27.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/data_flow/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-07-25 12:43:00.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/data_flow/__init__.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-01 10:53:27.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/data_flow/core/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-07-25 09:06:12.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/data_flow/core/__init__.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-01 10:53:27.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/data_flow/core/cache/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       67 2024-03-05 12:26:59.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/data_flow/core/cache/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)    10095 2024-03-05 12:25:44.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/data_flow/core/cache/cache_manager_for_iterator.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-01 10:53:27.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/data_flow/core/cache/test/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-03-04 08:47:42.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/data_flow/core/cache/test/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1147 2024-03-05 12:28:39.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/data_flow/core/cache/test/test_cache_manager_for_iterator.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-01 10:53:27.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/data_flow/core/reader/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      146 2022-02-09 09:12:47.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/data_flow/core/reader/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)    10158 2024-04-01 10:07:02.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/data_flow/core/reader/file_iterative_reader.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2453 2024-04-01 09:44:38.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/data_flow/core/reader/unified_reader.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)    11783 2024-03-05 12:32:31.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/data_flow/core/reader/unified_reader_base.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-01 10:53:27.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/data_flow/file/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        1 2022-07-25 12:56:33.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/data_flow/file/__init__.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-01 10:53:27.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/data_flow/file/json_/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       85 2022-07-25 12:54:00.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/data_flow/file/json_/__init__.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-01 10:53:27.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/data_flow/file/json_/converter/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      401 2024-04-01 10:34:15.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/data_flow/file/json_/converter/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      559 2022-07-25 12:26:23.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/data_flow/file/json_/converter/convert_dict_key_to_number.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      391 2023-05-22 11:15:00.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/data_flow/file/json_/converter/convert_ndarray_to_list.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      809 2023-07-22 15:47:27.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/data_flow/file/json_/converter/escape_non_str_dict_key.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      763 2024-04-01 10:34:15.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/data_flow/file/json_/converter/escape_tuple_and_set.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      377 2023-05-22 11:15:00.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/data_flow/file/json_/converter/integrate.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      808 2023-07-22 16:14:24.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/data_flow/file/json_/converter/unescape_non_str_dict_key.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      814 2024-04-01 10:34:15.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/data_flow/file/json_/converter/unescape_tuple_and_set.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1808 2024-04-01 10:34:15.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/data_flow/file/json_/read_json.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2379 2024-04-01 10:29:58.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/data_flow/file/json_/write_json.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-01 10:53:27.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/data_flow/file/kevin_notation/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      259 2023-02-08 07:16:46.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/data_flow/file/kevin_notation/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3621 2023-08-14 09:11:43.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/data_flow/file/kevin_notation/converter.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     8297 2024-04-01 09:58:49.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/data_flow/file/kevin_notation/kevin_notation_reader.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)    16331 2023-08-23 07:58:51.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/data_flow/file/kevin_notation/kevin_notation_writer.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      544 2024-04-01 10:13:38.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/data_flow/file/kevin_notation/read.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-01 10:53:27.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/data_flow/file/kevin_notation/test/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-07-30 14:12:33.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/data_flow/file/kevin_notation/test/__init__.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-01 10:53:27.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/data_flow/file/kevin_notation/test/test_data/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-08-01 07:19:40.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/data_flow/file/kevin_notation/test/test_data/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      324 2022-08-01 07:19:40.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/data_flow/file/kevin_notation/test/test_data/data_0.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      176 2023-08-23 08:01:05.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/data_flow/file/kevin_notation/test/test_data/data_1.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      438 2023-08-23 08:42:02.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/data_flow/file/kevin_notation/test/test_data/data_all.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     7345 2024-04-01 10:14:44.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/data_flow/file/kevin_notation/test/test_kevin_notation.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      556 2023-06-21 00:11:28.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/data_flow/file/kevin_notation/write.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-01 10:53:27.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/data_flow/file/markdown/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      125 2023-07-26 13:43:05.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/data_flow/file/markdown/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      304 2023-07-26 13:41:36.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/data_flow/file/markdown/generate_link.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1006 2023-07-26 13:41:54.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/data_flow/file/markdown/generate_list.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     7209 2024-03-18 06:57:03.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/data_flow/file/markdown/generate_table.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-01 10:53:27.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/developing/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        1 2022-02-08 10:14:56.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/developing/__init__.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-01 10:53:27.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/developing/decorator/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       66 2022-02-08 10:15:24.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/developing/decorator/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      399 2022-02-08 06:57:21.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/developing/decorator/restore_original_work_path.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-01 10:53:27.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/developing/design_pattern/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       20 2022-04-18 08:15:52.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/developing/design_pattern/__init__.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-01 10:53:27.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/developing/design_pattern/producer_consumer/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       28 2022-04-18 08:15:52.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/developing/design_pattern/producer_consumer/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      892 2022-12-12 08:39:00.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/developing/design_pattern/producer_consumer/consumer.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3164 2022-04-18 08:15:52.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/developing/design_pattern/producer_consumer/for_cvf.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       50 2022-04-18 11:35:30.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/developing/design_pattern/producer_consumer/getter.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      740 2022-04-18 12:49:09.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/developing/design_pattern/producer_consumer/graph.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2299 2022-04-18 12:23:06.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/developing/design_pattern/producer_consumer/node.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-04-18 08:15:52.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/developing/design_pattern/producer_consumer/producer.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       51 2022-04-18 10:40:32.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/developing/design_pattern/producer_consumer/sender.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-01 10:53:27.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/developing/design_pattern/singleton/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       49 2022-04-18 13:24:36.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/developing/design_pattern/singleton/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3803 2023-06-12 12:14:03.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/developing/design_pattern/singleton/singleton_for_uid.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2089 2022-02-28 06:54:56.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/developing/general_matrix_multiplication.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-01 10:53:27.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/developing/numerical_characteristics/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-06-02 05:01:47.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/developing/numerical_characteristics/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2953 2022-06-02 05:03:41.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/developing/numerical_characteristics/iou.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-01 10:53:27.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/developing/temperate/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      630 2022-03-13 18:22:06.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/developing/temperate/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      213 2022-03-10 05:06:13.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/developing/temperate/iterator_base.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1663 2022-03-13 18:22:06.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/developing/temperate/my_iterator.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1214 2022-03-10 05:06:13.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/developing/temperate/my_iterator_base.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      217 2022-03-10 05:06:13.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/developing/temperate/sequence_map_base.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      241 2023-03-31 07:27:37.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/developing/test.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-01 10:53:27.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/env_info/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        1 2023-03-30 13:18:27.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/env_info/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      879 2023-04-10 12:53:17.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/env_info/check_validity_and_uninstall.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1953 2023-06-21 01:55:26.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/env_info/check_version_and_update.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-01 10:53:27.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/env_info/test/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-03-30 12:51:50.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/env_info/test/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1728 2023-04-13 07:53:17.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/env_info/test/test_version.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-01 10:53:27.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/env_info/version/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      187 2023-03-30 13:11:22.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/env_info/version/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2489 2023-04-13 07:51:40.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/env_info/version/compare_version.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      860 2023-04-13 07:46:23.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/env_info/version/parse_version.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2458 2023-03-30 13:11:22.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/env_info/version/sort_version_ls.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-01 10:53:27.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/geometry/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-07-05 07:35:48.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/geometry/__init__.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-01 10:53:27.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/geometry/for_boxes/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      650 2023-03-24 10:03:29.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/geometry/for_boxes/__init__.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-01 10:53:27.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/geometry/for_boxes/__old_version/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-03-24 10:03:09.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/geometry/for_boxes/__old_version/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2564 2023-03-24 09:28:54.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/geometry/for_boxes/__old_version/cal_iou_between_box.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     5701 2023-03-31 07:27:38.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/geometry/for_boxes/boolean_algebra_for_boxes.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      305 2023-03-24 09:34:05.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/geometry/for_boxes/cal_area_of_boxes.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3079 2023-05-16 14:16:04.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/geometry/for_boxes/cal_iou_between_boxes.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     8249 2022-08-01 13:19:11.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/geometry/for_boxes/convert_boxes_from_coord_to_grid_index.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      836 2022-08-01 11:47:43.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/geometry/for_boxes/detect_collision.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2762 2022-07-06 13:18:05.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/geometry/for_boxes/detect_collision_among_boxes_ls.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     8255 2023-05-16 11:51:25.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/geometry/for_boxes/detect_collision_inside_boxes.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     8634 2023-06-21 01:55:28.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/geometry/for_boxes/detect_overlap.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      292 2022-07-05 08:41:47.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/geometry/for_boxes/get_ticks_of_boxes.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-01 10:53:27.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/machine_learning/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-02-28 06:47:25.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/machine_learning/__init__.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-01 10:53:27.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/machine_learning/dataset/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        1 2022-02-10 07:21:33.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/machine_learning/dataset/__init__.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-01 10:53:27.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/machine_learning/dataset/face/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-02-14 08:37:13.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/machine_learning/dataset/face/__init__.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-01 10:53:27.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/machine_learning/dataset/face/analysis/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       69 2022-09-28 09:26:13.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/machine_learning/dataset/face/analysis/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     4714 2023-03-31 07:27:38.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/machine_learning/dataset/face/analysis/get_fail_case_from_iterator.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-01 10:53:27.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/machine_learning/dataset/face/dummy/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       54 2022-02-28 08:44:35.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/machine_learning/dataset/face/dummy/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     7137 2023-03-31 07:27:37.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/machine_learning/dataset/face/dummy/dummy_data.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-01 10:53:27.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/machine_learning/dataset/face/verification/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      259 2022-09-26 09:52:59.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/machine_learning/dataset/face/verification/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      896 2022-03-13 18:22:06.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/machine_learning/dataset/face/verification/build_generator.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1858 2023-03-31 07:27:37.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/machine_learning/dataset/face/verification/build_iterator.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)    17766 2023-03-31 07:27:37.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/machine_learning/dataset/face/verification/factory.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-01 10:53:27.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-01 10:53:27.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/__by_block/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      299 2022-03-13 18:22:06.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/__by_block/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     4480 2023-03-31 07:27:38.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/__by_block/along_axis.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3482 2023-03-31 07:27:37.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/__by_block/along_diagonal.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     4799 2023-03-31 07:27:37.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/__by_block/of_all.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     5480 2023-03-31 07:27:38.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/__by_block/of_triangle.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      224 2022-03-13 18:22:06.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3114 2023-03-31 07:27:38.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/by_block.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3773 2023-03-31 07:27:38.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/by_samples.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      170 2022-03-10 12:36:00.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/machine_learning/dataset/face/verification/merge.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-01 10:53:27.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/machine_learning/statistician/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-02-21 04:21:21.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/machine_learning/statistician/__init__.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-01 10:53:27.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/machine_learning/statistician/binary_classification/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      427 2022-02-22 06:22:25.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/machine_learning/statistician/binary_classification/__init__.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-01 10:53:27.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/machine_learning/statistician/binary_classification/confusion_matrices/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        1 2022-02-21 13:29:08.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/machine_learning/statistician/binary_classification/confusion_matrices/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3247 2022-02-22 06:22:25.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/machine_learning/statistician/binary_classification/confusion_matrices/accumulator_for_cfm.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     5319 2023-03-31 07:27:37.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/machine_learning/statistician/binary_classification/confusion_matrices/cal_cfm.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3355 2023-03-31 07:27:37.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/machine_learning/statistician/binary_classification/confusion_matrices/cal_cfm_iteratively_by_chunk.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      891 2022-04-28 12:02:07.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/machine_learning/statistician/binary_classification/confusion_matrices/cal_tpr_and_fpr.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      442 2022-02-22 05:39:00.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/machine_learning/statistician/binary_classification/confusion_matrices/convert.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3661 2023-03-31 07:27:38.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/machine_learning/statistician/binary_classification/confusion_matrices/merge_cfm_ls.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-01 10:53:27.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/math/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-07-27 07:16:21.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/math/__init__.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-01 10:53:27.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/math/dimension/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-06-03 13:07:44.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/math/dimension/__init__.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-01 10:53:27.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/math/dimension/concat_and_split/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      157 2022-08-08 08:06:40.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/math/dimension/concat_and_split/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)    23861 2023-06-14 03:08:32.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/math/dimension/concat_and_split/computational_tree.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     4997 2022-08-08 08:19:17.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/math/dimension/concat_and_split/concat_crops_into_whole.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3066 2022-08-08 08:19:17.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/math/dimension/concat_and_split/split_whole_into_crops.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-01 10:53:27.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/math/dimension/coordinates/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      232 2023-03-13 06:47:47.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/math/dimension/coordinates/__init__.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-01 10:53:27.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/math/dimension/coordinates/convert/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       43 2023-03-13 06:47:47.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/math/dimension/coordinates/convert/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     4972 2023-03-10 14:11:22.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/math/dimension/coordinates/convert/convert_format.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-01 10:53:27.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/math/dimension/coordinates/generate/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      264 2023-03-13 06:47:47.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/math/dimension/coordinates/generate/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3380 2023-03-13 06:48:36.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/math/dimension/coordinates/generate/generate_integrated_api.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     5738 2023-03-31 07:27:38.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/math/dimension/coordinates/generate/generate_shuffled_index_ls.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     4426 2022-07-29 07:53:01.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/math/dimension/coordinates/generate/generate_z_pattern_indices_ls.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1373 2023-03-10 13:56:45.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/math/dimension/coordinates/generate/normal_indices_generator.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-01 10:53:27.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/math/dimension/reshape/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      220 2022-07-25 13:28:44.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/math/dimension/reshape/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1946 2023-03-31 07:27:38.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/math/dimension/reshape/flatten_along_pattern.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1064 2023-03-31 07:27:37.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/math/dimension/reshape/merge_blocks.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1236 2023-03-31 07:27:37.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/math/dimension/reshape/split_blocks.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1859 2023-03-31 07:27:37.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/math/dimension/reshape/unflatten_along_pattern.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-01 10:53:27.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/math/dimension/transpose/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      177 2022-05-31 10:43:01.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/math/dimension/transpose/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      611 2022-08-09 13:17:49.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/math/dimension/transpose/get_inverse_of_transpose_index_ls.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1472 2023-03-31 07:27:38.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/math/dimension/transpose/transpose_inside_axis.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-01 10:53:27.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/math/number_theory/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      182 2023-03-05 15:57:35.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/math/number_theory/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      244 2023-03-05 15:45:13.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/math/number_theory/cache.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      387 2023-03-05 15:57:35.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/math/number_theory/get_greatest_common_divisor.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      949 2023-03-31 07:27:38.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/math/number_theory/get_primes.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      499 2023-03-31 07:27:37.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/math/number_theory/prime_factorization.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-01 10:53:27.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/math/number_theory/test/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-03-06 07:12:06.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/math/number_theory/test/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      747 2023-03-31 07:27:37.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/math/number_theory/test/test_get_greatest_common_divisor.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      784 2023-03-31 07:27:38.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/math/number_theory/test/test_get_primes.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      551 2023-03-31 07:27:37.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/math/number_theory/test/test_prime_factorization.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-01 10:53:27.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/math/transform/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-06-10 08:52:28.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/math/transform/__init__.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-01 10:53:27.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/math/transform/dct/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      147 2022-07-22 13:25:44.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/math/transform/dct/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     8296 2023-03-31 07:27:37.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/math/transform/dct/dct_calculator.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     4305 2022-07-20 12:21:16.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/math/transform/dct/generate_dct_trans_matrix.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-01 10:53:27.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/math/transform/scaling_and_shift/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       29 2022-07-30 13:19:40.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/math/transform/scaling_and_shift/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1280 2022-07-30 13:48:26.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/math/transform/scaling_and_shift/scaling.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-01 10:53:27.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/math/utils/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      289 2024-03-18 06:58:41.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/math/utils/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1943 2022-08-09 12:09:28.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/math/utils/convert_dtype.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1620 2022-08-08 08:50:02.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/math/utils/get_crop_by_box.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1553 2022-08-02 12:15:03.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/math/utils/get_function_table_for_array_and_tensor.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1775 2022-08-08 08:50:02.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/math/utils/set_crop_by_box.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      345 2024-03-18 06:57:03.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/math/utils/split_integer_most_evenly.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-01 10:53:27.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/nested_dict_list/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      333 2023-12-14 13:19:07.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/nested_dict_list/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     6144 2023-10-16 08:29:56.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/nested_dict_list/copy_.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      614 2023-07-25 12:37:51.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/nested_dict_list/count_leaf_node_nums.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1286 2023-06-21 01:55:54.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/nested_dict_list/get_hash.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3748 2024-01-16 12:22:50.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/nested_dict_list/get_nodes.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2083 2023-07-26 06:32:19.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/nested_dict_list/get_value.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-01 10:53:27.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/nested_dict_list/name_handler/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      107 2023-06-20 10:05:38.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/nested_dict_list/name_handler/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      989 2024-01-16 12:37:35.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/nested_dict_list/name_handler/build_name.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1163 2023-08-14 09:09:48.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/nested_dict_list/name_handler/escape_node.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2280 2024-01-16 12:38:24.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/nested_dict_list/name_handler/parse_name.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-01 10:53:27.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/nested_dict_list/serializer/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       92 2023-11-28 09:25:35.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/nested_dict_list/serializer/__init__.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-01 10:53:27.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/nested_dict_list/serializer/backends/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       39 2023-07-20 06:49:05.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/nested_dict_list/serializer/backends/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2145 2023-08-14 12:43:06.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/nested_dict_list/serializer/backends/_json_.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1652 2023-08-10 04:59:20.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/nested_dict_list/serializer/backends/_ndl.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1470 2023-07-25 12:39:59.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/nested_dict_list/serializer/backends/_numpy_bin.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1384 2023-07-25 12:39:59.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/nested_dict_list/serializer/backends/_numpy_npy.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1282 2023-07-25 12:39:59.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/nested_dict_list/serializer/backends/_pickle_.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      853 2023-07-25 12:39:59.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/nested_dict_list/serializer/backends/_skip_all.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1444 2023-08-14 12:33:39.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/nested_dict_list/serializer/backends/_skip_simple.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1282 2023-07-25 12:39:59.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/nested_dict_list/serializer/backends/_torch_all.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1353 2023-07-25 12:39:59.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/nested_dict_list/serializer/backends/_torch_tensor.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1741 2023-07-20 07:15:24.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/nested_dict_list/serializer/backends/backend_base.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      847 2023-11-28 09:24:46.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/nested_dict_list/serializer/enum_variable.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2577 2023-11-28 09:21:18.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/nested_dict_list/serializer/read.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      392 2023-11-28 09:24:46.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/nested_dict_list/serializer/variable.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)    18145 2023-11-28 09:28:08.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/nested_dict_list/serializer/write.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3460 2024-01-26 09:17:13.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/nested_dict_list/set_default.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3470 2023-12-13 10:59:57.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/nested_dict_list/set_value.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     6846 2023-08-14 09:08:40.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/nested_dict_list/traverse.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-01 10:53:27.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/nested_dict_list/value_parser/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      234 2023-08-23 10:27:58.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/nested_dict_list/value_parser/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3119 2023-07-25 12:39:59.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/nested_dict_list/value_parser/cal_relation_between_references.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2301 2023-07-26 06:32:19.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/nested_dict_list/value_parser/eval_references.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2370 2023-08-23 12:32:31.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/nested_dict_list/value_parser/parse_and_eval_references.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2116 2023-07-26 06:32:19.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/nested_dict_list/value_parser/parse_references.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-01 10:53:27.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/patches/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-03-29 13:28:32.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/patches/__init__.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-01 10:53:27.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/patches/for_logging/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       39 2023-08-17 07:33:01.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/patches/for_logging/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3071 2024-01-05 07:58:55.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/patches/for_logging/build_logger.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-01 10:53:27.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/patches/for_matplotlib/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      180 2024-03-05 12:51:41.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/patches/for_matplotlib/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1837 2023-03-10 10:16:48.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/patches/for_matplotlib/add_trajectory_2d.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1696 2023-03-10 09:17:25.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/patches/for_matplotlib/add_trajectory_3d.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1361 2023-03-10 08:13:57.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/patches/for_matplotlib/arrow3d.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      984 2024-03-05 12:51:00.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/patches/for_matplotlib/generate_color_list.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-01 10:53:27.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/patches/for_numpy/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       21 2023-10-10 13:48:12.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/patches/for_numpy/__init__.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-01 10:53:27.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/patches/for_numpy/linalg/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      128 2024-03-05 12:56:40.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/patches/for_numpy/linalg/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      423 2023-05-17 07:05:16.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/patches/for_numpy/linalg/cos_similar.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1080 2024-03-05 13:02:36.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/patches/for_numpy/linalg/entropy.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      625 2023-04-24 08:52:01.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/patches/for_numpy/linalg/normalize.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2095 2023-12-27 09:20:36.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/patches/for_numpy/linalg/softmax.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-01 10:53:27.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/patches/for_numpy/random/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      149 2024-01-22 07:02:28.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/patches/for_numpy/random/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1999 2024-04-01 10:25:48.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/patches/for_numpy/random/get_rng.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     5859 2024-03-05 13:12:47.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/patches/for_numpy/random/truncated_multivariate_normal.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3726 2024-03-05 13:11:35.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/patches/for_numpy/random/truncated_normal.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      231 2024-01-22 06:17:42.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/patches/for_numpy/random/variable.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-01 10:53:27.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/patches/for_optuna/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      249 2024-01-04 06:48:51.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/patches/for_optuna/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1705 2024-01-04 07:28:28.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/patches/for_optuna/build_sampler.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3327 2024-01-04 07:01:24.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/patches/for_optuna/build_storage.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2253 2024-01-04 07:55:17.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/patches/for_optuna/build_study.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2743 2024-01-04 06:46:32.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/patches/for_optuna/copy_study.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     7071 2023-12-13 09:36:59.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/patches/for_optuna/sample_from_feasible_domain.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-01 10:53:27.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/patches/for_optuna/serialize/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       35 2023-12-18 08:18:28.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/patches/for_optuna/serialize/__init__.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-01 10:53:27.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/patches/for_optuna/serialize/for_study/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       46 2024-01-03 09:50:06.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/patches/for_optuna/serialize/for_study/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2088 2024-01-24 11:00:35.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/patches/for_optuna/serialize/for_study/dump.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1818 2024-01-04 07:10:38.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/patches/for_optuna/serialize/for_study/load.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-01 10:53:27.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/patches/for_optuna/serialize/for_trial/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       46 2023-12-17 15:30:35.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/patches/for_optuna/serialize/for_trial/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      982 2023-12-18 07:02:18.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/patches/for_optuna/serialize/for_trial/dump.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      796 2023-12-17 15:43:49.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/patches/for_optuna/serialize/for_trial/load.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-01 10:53:27.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/patches/for_os/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      128 2023-12-13 07:02:56.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/patches/for_os/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      656 2023-07-21 09:38:57.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/patches/for_os/pack.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      750 2023-12-13 08:34:00.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/patches/for_os/remove.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1047 2023-07-21 09:40:06.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/patches/for_os/unpack.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     8376 2023-12-13 07:22:41.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/patches/for_os/walk.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-01 10:53:27.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/patches/for_test/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       49 2022-07-29 06:55:38.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/patches/for_test/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     5038 2023-08-11 11:15:23.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/patches/for_test/check_consistency.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-01 10:53:27.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/patches/for_torch/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-02-21 06:56:01.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/patches/for_torch/__init__.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-01 10:53:27.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/patches/for_torch/compatible/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       75 2023-03-08 07:01:29.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/patches/for_torch/compatible/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      393 2023-04-12 15:31:18.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/patches/for_torch/compatible/concat.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-01 10:53:27.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/patches/for_torch/compatible/linalg/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       44 2023-03-08 08:04:27.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/patches/for_torch/compatible/linalg/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      770 2023-04-12 15:31:18.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/patches/for_torch/compatible/linalg/norm.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      575 2023-04-12 15:31:18.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/patches/for_torch/compatible/linalg/svd.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-01 10:53:27.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/patches/for_torch/compatible/nn/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       35 2023-05-30 11:36:55.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/patches/for_torch/compatible/nn/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     5357 2023-04-12 15:31:18.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/patches/for_torch/compatible/nn/sequential.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      845 2023-04-12 15:31:18.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/patches/for_torch/compatible/tile.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      733 2023-04-12 15:36:21.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/patches/for_torch/compatible/where.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-01 10:53:27.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/patches/for_torch/math/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       68 2022-02-21 09:51:39.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/patches/for_torch/math/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2047 2022-02-22 06:43:43.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/patches/for_torch/math/get_y_at_x.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1378 2022-02-21 09:44:44.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/patches/for_torch/math/my_around.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-01 10:53:27.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/patches/for_torch/nn/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       39 2023-05-30 11:37:07.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/patches/for_torch/nn/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      223 2023-05-29 08:32:26.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox/patches/for_torch/nn/lambda_layer.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-01 10:53:27.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox_dev.egg-info/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2008 2024-04-01 10:53:26.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox_dev.egg-info/PKG-INFO
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)    19020 2024-04-01 10:53:26.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox_dev.egg-info/SOURCES.txt
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        1 2024-04-01 10:53:26.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox_dev.egg-info/dependency_links.txt
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       92 2024-04-01 10:53:26.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox_dev.egg-info/requires.txt
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       14 2024-04-01 10:53:26.000000 kevin-toolbox-dev-1.3.3/kevin_toolbox_dev.egg-info/top_level.txt
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       59 2023-03-31 06:32:36.000000 kevin-toolbox-dev-1.3.3/pyproject.toml
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      908 2024-04-01 10:53:27.000000 kevin-toolbox-dev-1.3.3/setup.cfg
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      733 2023-03-31 07:25:47.000000 kevin-toolbox-dev-1.3.3/setup.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-06 13:16:20.000000 kevin-toolbox-dev-1.3.4/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2490 2024-04-06 13:16:20.000000 kevin-toolbox-dev-1.3.4/PKG-INFO
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1881 2024-04-06 13:14:40.000000 kevin-toolbox-dev-1.3.4/README.md
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-06 13:16:20.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      410 2024-04-06 13:16:19.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/__init__.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-06 13:16:20.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/computer_science/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-12-01 13:56:40.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/computer_science/__init__.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-06 13:16:20.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/computer_science/algorithm/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        1 2023-03-04 15:12:36.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/computer_science/algorithm/__init__.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-06 13:16:20.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/computer_science/algorithm/cache_manager/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       41 2024-03-03 16:14:42.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/computer_science/algorithm/cache_manager/__init__.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-06 13:16:20.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/computer_science/algorithm/cache_manager/cache/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       70 2024-03-03 16:52:11.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/computer_science/algorithm/cache_manager/cache/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2229 2024-03-04 07:36:13.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/computer_science/algorithm/cache_manager/cache/cache_base.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      963 2024-03-04 07:36:45.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/computer_science/algorithm/cache_manager/cache/memo_cache.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     9151 2024-03-04 13:32:58.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/computer_science/algorithm/cache_manager/cache_manager.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-06 13:16:20.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/computer_science/algorithm/cache_manager/strategy/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      199 2024-03-04 13:33:39.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/computer_science/algorithm/cache_manager/strategy/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      770 2024-03-04 12:38:04.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/computer_science/algorithm/cache_manager/strategy/fifo_strategy.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2557 2024-03-04 13:04:24.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/computer_science/algorithm/cache_manager/strategy/lfu_strategy.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1376 2024-03-04 09:11:55.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/computer_science/algorithm/cache_manager/strategy/lru_strategy.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1106 2024-03-04 13:04:24.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/computer_science/algorithm/cache_manager/strategy/lst_strategy.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1457 2024-03-04 08:20:39.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/computer_science/algorithm/cache_manager/strategy/strategy_base.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-06 13:16:20.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/computer_science/algorithm/cache_manager/test/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-03-04 08:47:42.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/computer_science/algorithm/cache_manager/test/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1108 2024-03-03 17:42:33.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/computer_science/algorithm/cache_manager/test/test_cache_builder.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     7944 2024-03-04 13:21:47.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/computer_science/algorithm/cache_manager/test/test_cache_manager.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     5310 2024-03-04 13:07:15.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/computer_science/algorithm/cache_manager/test/test_cache_strategy.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      835 2024-03-03 16:15:58.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/computer_science/algorithm/cache_manager/variable.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-06 13:16:20.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/computer_science/algorithm/combinatorial_optimization/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      142 2023-03-05 16:13:01.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/computer_science/algorithm/combinatorial_optimization/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1832 2023-03-31 07:27:37.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/computer_science/algorithm/combinatorial_optimization/get_subset_with_largest_product.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-06 13:16:20.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/computer_science/algorithm/combinatorial_optimization/test/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-07-30 14:12:33.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/computer_science/algorithm/combinatorial_optimization/test/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1914 2023-06-12 05:50:08.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/computer_science/algorithm/combinatorial_optimization/test/test_get_subset_with_largest_product.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2078 2023-06-12 05:50:08.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/computer_science/algorithm/combinatorial_optimization/test/test_zero_one_knapsack_problem.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2819 2023-03-05 16:40:22.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/computer_science/algorithm/combinatorial_optimization/zero_one_knapsack_problem.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-06 13:16:20.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/computer_science/algorithm/execution_graph/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-08-04 08:58:16.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/computer_science/algorithm/execution_graph/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3297 2023-08-04 11:56:33.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/computer_science/algorithm/execution_graph/jump_node.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3189 2023-08-04 11:50:17.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/computer_science/algorithm/execution_graph/random_node.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3267 2023-08-04 11:50:17.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/computer_science/algorithm/execution_graph/simple_node.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-06 13:16:20.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/computer_science/algorithm/for_dict/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       37 2023-06-12 05:50:08.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/computer_science/algorithm/for_dict/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      666 2023-06-19 08:36:11.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/computer_science/algorithm/for_dict/deep_update.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-06 13:16:20.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/computer_science/algorithm/for_seq/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      121 2023-08-15 11:37:21.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/computer_science/algorithm/for_seq/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2544 2023-08-15 11:44:17.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/computer_science/algorithm/for_seq/chunk_generator.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1046 2023-06-12 05:50:08.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/computer_science/algorithm/for_seq/flatten_list.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      309 2023-06-12 05:50:08.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/computer_science/algorithm/for_seq/get_subsets.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-06 13:16:20.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/computer_science/algorithm/locks/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       35 2023-04-21 13:18:26.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/computer_science/algorithm/locks/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2492 2023-04-24 08:04:07.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/computer_science/algorithm/locks/mutex_lock.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-06 13:16:20.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/computer_science/algorithm/parallel_and_concurrent/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       55 2023-08-15 13:22:31.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/computer_science/algorithm/parallel_and_concurrent/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      896 2023-07-28 14:07:18.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/computer_science/algorithm/parallel_and_concurrent/async_executor.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3126 2023-08-15 13:59:27.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/computer_science/algorithm/parallel_and_concurrent/multi_thread_execute.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-06 13:16:20.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/computer_science/algorithm/pareto_front/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       68 2024-01-05 07:20:07.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/computer_science/algorithm/pareto_front/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3008 2024-01-05 07:20:45.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/computer_science/algorithm/pareto_front/get_pareto_points_idx.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-06 13:16:20.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/computer_science/algorithm/registration/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       49 2023-06-12 14:36:27.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/computer_science/algorithm/registration/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)    17385 2024-03-04 11:52:32.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/computer_science/algorithm/registration/registry.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-06 13:16:20.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/computer_science/algorithm/scheduler/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       76 2023-06-02 12:00:07.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/computer_science/algorithm/scheduler/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)    12194 2023-07-26 06:32:19.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/computer_science/algorithm/scheduler/strategy_manager.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     4470 2023-07-25 12:43:34.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/computer_science/algorithm/scheduler/trigger.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-06 13:16:20.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/computer_science/algorithm/search/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       41 2023-03-20 13:18:25.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/computer_science/algorithm/search/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1013 2023-03-04 15:58:55.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/computer_science/algorithm/search/binary_search.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-06 13:16:20.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/computer_science/algorithm/statistician/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      167 2023-11-13 07:53:49.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/computer_science/algorithm/statistician/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     6098 2023-11-13 07:53:49.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/computer_science/algorithm/statistician/accumulator_base.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2570 2023-11-13 07:54:37.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/computer_science/algorithm/statistician/average_accumulator.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     5363 2023-11-13 07:58:15.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/computer_science/algorithm/statistician/exponential_moving_average.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-06 13:16:20.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/computer_science/algorithm/statistician/init_var/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      121 2023-11-13 07:46:03.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/computer_science/algorithm/statistician/init_var/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      769 2023-11-13 07:46:03.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/computer_science/algorithm/statistician/init_var/init_by_data_format.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      572 2023-11-13 07:46:03.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/computer_science/algorithm/statistician/init_var/init_by_like.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-06 13:16:20.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/computer_science/algorithm/utils/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-08 14:31:25.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/computer_science/algorithm/utils/__init__.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-06 13:16:20.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/computer_science/data_structure/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       31 2023-03-22 06:30:28.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/computer_science/data_structure/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     6206 2023-06-21 01:55:31.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/computer_science/data_structure/executor.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-06 13:16:20.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/dangerous/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       93 2023-03-29 12:29:14.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/dangerous/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2898 2023-03-31 07:27:38.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/dangerous/dump_into_pickle_with_executor_attached.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-06 13:16:20.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/data_flow/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-07-25 12:43:00.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/data_flow/__init__.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-06 13:16:20.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/data_flow/core/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-07-25 09:06:12.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/data_flow/core/__init__.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-06 13:16:20.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/data_flow/core/cache/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       67 2024-03-05 12:26:59.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/data_flow/core/cache/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)    10095 2024-03-05 12:25:44.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/data_flow/core/cache/cache_manager_for_iterator.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-06 13:16:20.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/data_flow/core/cache/test/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-03-04 08:47:42.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/data_flow/core/cache/test/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1147 2024-03-05 12:28:39.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/data_flow/core/cache/test/test_cache_manager_for_iterator.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-06 13:16:20.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/data_flow/core/reader/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      146 2022-02-09 09:12:47.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/data_flow/core/reader/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)    10158 2024-04-01 10:07:02.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/data_flow/core/reader/file_iterative_reader.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2453 2024-04-01 09:44:38.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/data_flow/core/reader/unified_reader.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)    11783 2024-03-05 12:32:31.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/data_flow/core/reader/unified_reader_base.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-06 13:16:20.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/data_flow/file/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        1 2022-07-25 12:56:33.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/data_flow/file/__init__.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-06 13:16:20.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/data_flow/file/json_/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       85 2022-07-25 12:54:00.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/data_flow/file/json_/__init__.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-06 13:16:20.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/data_flow/file/json_/converter/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      401 2024-04-01 10:34:15.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/data_flow/file/json_/converter/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      559 2022-07-25 12:26:23.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/data_flow/file/json_/converter/convert_dict_key_to_number.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      391 2023-05-22 11:15:00.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/data_flow/file/json_/converter/convert_ndarray_to_list.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      809 2023-07-22 15:47:27.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/data_flow/file/json_/converter/escape_non_str_dict_key.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      763 2024-04-01 10:34:15.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/data_flow/file/json_/converter/escape_tuple_and_set.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      377 2023-05-22 11:15:00.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/data_flow/file/json_/converter/integrate.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      808 2023-07-22 16:14:24.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/data_flow/file/json_/converter/unescape_non_str_dict_key.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      814 2024-04-01 10:34:15.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/data_flow/file/json_/converter/unescape_tuple_and_set.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1808 2024-04-01 10:34:15.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/data_flow/file/json_/read_json.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2379 2024-04-01 10:29:58.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/data_flow/file/json_/write_json.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-06 13:16:20.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/data_flow/file/kevin_notation/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      259 2023-02-08 07:16:46.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/data_flow/file/kevin_notation/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3621 2023-08-14 09:11:43.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/data_flow/file/kevin_notation/converter.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     8297 2024-04-01 09:58:49.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/data_flow/file/kevin_notation/kevin_notation_reader.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)    16331 2023-08-23 07:58:51.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/data_flow/file/kevin_notation/kevin_notation_writer.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      544 2024-04-01 10:13:38.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/data_flow/file/kevin_notation/read.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-06 13:16:20.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/data_flow/file/kevin_notation/test/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-07-30 14:12:33.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/data_flow/file/kevin_notation/test/__init__.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-06 13:16:20.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/data_flow/file/kevin_notation/test/test_data/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-08-01 07:19:40.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/data_flow/file/kevin_notation/test/test_data/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      324 2022-08-01 07:19:40.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/data_flow/file/kevin_notation/test/test_data/data_0.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      176 2023-08-23 08:01:05.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/data_flow/file/kevin_notation/test/test_data/data_1.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      438 2023-08-23 08:42:02.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/data_flow/file/kevin_notation/test/test_data/data_all.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     7345 2024-04-01 10:14:44.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/data_flow/file/kevin_notation/test/test_kevin_notation.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      556 2023-06-21 00:11:28.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/data_flow/file/kevin_notation/write.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-06 13:16:20.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/data_flow/file/markdown/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      125 2023-07-26 13:43:05.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/data_flow/file/markdown/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      304 2023-07-26 13:41:36.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/data_flow/file/markdown/generate_link.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1006 2023-07-26 13:41:54.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/data_flow/file/markdown/generate_list.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     7209 2024-03-18 06:57:03.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/data_flow/file/markdown/generate_table.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-06 13:16:20.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/developing/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        1 2022-02-08 10:14:56.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/developing/__init__.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-06 13:16:20.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/developing/decorator/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       66 2022-02-08 10:15:24.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/developing/decorator/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      399 2022-02-08 06:57:21.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/developing/decorator/restore_original_work_path.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-06 13:16:20.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/developing/design_pattern/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       20 2022-04-18 08:15:52.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/developing/design_pattern/__init__.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-06 13:16:20.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/developing/design_pattern/producer_consumer/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       28 2022-04-18 08:15:52.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/developing/design_pattern/producer_consumer/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      892 2022-12-12 08:39:00.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/developing/design_pattern/producer_consumer/consumer.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3164 2022-04-18 08:15:52.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/developing/design_pattern/producer_consumer/for_cvf.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       50 2022-04-18 11:35:30.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/developing/design_pattern/producer_consumer/getter.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      740 2022-04-18 12:49:09.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/developing/design_pattern/producer_consumer/graph.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2299 2022-04-18 12:23:06.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/developing/design_pattern/producer_consumer/node.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-04-18 08:15:52.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/developing/design_pattern/producer_consumer/producer.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       51 2022-04-18 10:40:32.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/developing/design_pattern/producer_consumer/sender.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-06 13:16:20.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/developing/design_pattern/singleton/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       49 2022-04-18 13:24:36.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/developing/design_pattern/singleton/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3803 2023-06-12 12:14:03.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/developing/design_pattern/singleton/singleton_for_uid.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2089 2022-02-28 06:54:56.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/developing/general_matrix_multiplication.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-06 13:16:20.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/developing/numerical_characteristics/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-06-02 05:01:47.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/developing/numerical_characteristics/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2953 2022-06-02 05:03:41.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/developing/numerical_characteristics/iou.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-06 13:16:20.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/developing/temperate/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      630 2022-03-13 18:22:06.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/developing/temperate/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      213 2022-03-10 05:06:13.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/developing/temperate/iterator_base.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1663 2022-03-13 18:22:06.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/developing/temperate/my_iterator.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1214 2022-03-10 05:06:13.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/developing/temperate/my_iterator_base.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      217 2022-03-10 05:06:13.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/developing/temperate/sequence_map_base.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      241 2023-03-31 07:27:37.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/developing/test.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-06 13:16:20.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/env_info/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        1 2023-03-30 13:18:27.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/env_info/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      879 2023-04-10 12:53:17.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/env_info/check_validity_and_uninstall.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1953 2023-06-21 01:55:26.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/env_info/check_version_and_update.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-06 13:16:20.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/env_info/test/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-03-30 12:51:50.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/env_info/test/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1728 2023-04-13 07:53:17.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/env_info/test/test_version.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-06 13:16:20.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/env_info/version/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      187 2023-03-30 13:11:22.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/env_info/version/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2489 2023-04-13 07:51:40.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/env_info/version/compare_version.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      860 2023-04-13 07:46:23.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/env_info/version/parse_version.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2458 2023-03-30 13:11:22.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/env_info/version/sort_version_ls.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-06 13:16:20.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/geometry/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-07-05 07:35:48.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/geometry/__init__.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-06 13:16:20.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/geometry/for_boxes/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      650 2023-03-24 10:03:29.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/geometry/for_boxes/__init__.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-06 13:16:20.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/geometry/for_boxes/__old_version/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-03-24 10:03:09.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/geometry/for_boxes/__old_version/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2564 2023-03-24 09:28:54.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/geometry/for_boxes/__old_version/cal_iou_between_box.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     5701 2023-03-31 07:27:38.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/geometry/for_boxes/boolean_algebra_for_boxes.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      305 2023-03-24 09:34:05.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/geometry/for_boxes/cal_area_of_boxes.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3079 2023-05-16 14:16:04.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/geometry/for_boxes/cal_iou_between_boxes.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     8249 2022-08-01 13:19:11.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/geometry/for_boxes/convert_boxes_from_coord_to_grid_index.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      836 2022-08-01 11:47:43.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/geometry/for_boxes/detect_collision.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2762 2022-07-06 13:18:05.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/geometry/for_boxes/detect_collision_among_boxes_ls.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     8255 2023-05-16 11:51:25.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/geometry/for_boxes/detect_collision_inside_boxes.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     8634 2023-06-21 01:55:28.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/geometry/for_boxes/detect_overlap.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      292 2022-07-05 08:41:47.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/geometry/for_boxes/get_ticks_of_boxes.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-06 13:16:20.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/machine_learning/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-02-28 06:47:25.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/machine_learning/__init__.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-06 13:16:20.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/machine_learning/dataset/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        1 2022-02-10 07:21:33.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/machine_learning/dataset/__init__.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-06 13:16:20.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/machine_learning/dataset/face/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-02-14 08:37:13.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/machine_learning/dataset/face/__init__.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-06 13:16:20.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/machine_learning/dataset/face/analysis/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       69 2022-09-28 09:26:13.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/machine_learning/dataset/face/analysis/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     4714 2023-03-31 07:27:38.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/machine_learning/dataset/face/analysis/get_fail_case_from_iterator.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-06 13:16:20.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/machine_learning/dataset/face/dummy/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       54 2022-02-28 08:44:35.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/machine_learning/dataset/face/dummy/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     7137 2023-03-31 07:27:37.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/machine_learning/dataset/face/dummy/dummy_data.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-06 13:16:20.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/machine_learning/dataset/face/verification/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      259 2022-09-26 09:52:59.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/machine_learning/dataset/face/verification/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      896 2022-03-13 18:22:06.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/machine_learning/dataset/face/verification/build_generator.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1858 2023-03-31 07:27:37.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/machine_learning/dataset/face/verification/build_iterator.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)    17766 2023-03-31 07:27:37.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/machine_learning/dataset/face/verification/factory.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-06 13:16:20.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-06 13:16:20.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/__by_block/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      299 2022-03-13 18:22:06.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/__by_block/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     4480 2023-03-31 07:27:38.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/__by_block/along_axis.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3482 2023-03-31 07:27:37.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/__by_block/along_diagonal.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     4799 2023-03-31 07:27:37.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/__by_block/of_all.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     5480 2023-03-31 07:27:38.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/__by_block/of_triangle.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      224 2022-03-13 18:22:06.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3114 2023-03-31 07:27:38.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/by_block.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3773 2023-03-31 07:27:38.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/by_samples.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      170 2022-03-10 12:36:00.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/machine_learning/dataset/face/verification/merge.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-06 13:16:20.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/machine_learning/statistician/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-02-21 04:21:21.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/machine_learning/statistician/__init__.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-06 13:16:20.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/machine_learning/statistician/binary_classification/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      427 2022-02-22 06:22:25.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/machine_learning/statistician/binary_classification/__init__.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-06 13:16:20.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/machine_learning/statistician/binary_classification/confusion_matrices/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        1 2022-02-21 13:29:08.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/machine_learning/statistician/binary_classification/confusion_matrices/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3247 2022-02-22 06:22:25.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/machine_learning/statistician/binary_classification/confusion_matrices/accumulator_for_cfm.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     5319 2023-03-31 07:27:37.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/machine_learning/statistician/binary_classification/confusion_matrices/cal_cfm.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3355 2023-03-31 07:27:37.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/machine_learning/statistician/binary_classification/confusion_matrices/cal_cfm_iteratively_by_chunk.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      891 2022-04-28 12:02:07.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/machine_learning/statistician/binary_classification/confusion_matrices/cal_tpr_and_fpr.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      442 2022-02-22 05:39:00.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/machine_learning/statistician/binary_classification/confusion_matrices/convert.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3661 2023-03-31 07:27:38.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/machine_learning/statistician/binary_classification/confusion_matrices/merge_cfm_ls.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-06 13:16:20.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/math/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-07-27 07:16:21.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/math/__init__.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-06 13:16:20.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/math/dimension/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-06-03 13:07:44.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/math/dimension/__init__.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-06 13:16:20.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/math/dimension/concat_and_split/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      157 2022-08-08 08:06:40.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/math/dimension/concat_and_split/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)    23861 2023-06-14 03:08:32.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/math/dimension/concat_and_split/computational_tree.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     4997 2022-08-08 08:19:17.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/math/dimension/concat_and_split/concat_crops_into_whole.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3066 2022-08-08 08:19:17.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/math/dimension/concat_and_split/split_whole_into_crops.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-06 13:16:20.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/math/dimension/coordinates/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      232 2023-03-13 06:47:47.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/math/dimension/coordinates/__init__.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-06 13:16:20.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/math/dimension/coordinates/convert/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       43 2023-03-13 06:47:47.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/math/dimension/coordinates/convert/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     4972 2023-03-10 14:11:22.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/math/dimension/coordinates/convert/convert_format.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-06 13:16:20.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/math/dimension/coordinates/generate/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      264 2023-03-13 06:47:47.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/math/dimension/coordinates/generate/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3380 2023-03-13 06:48:36.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/math/dimension/coordinates/generate/generate_integrated_api.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     5738 2023-03-31 07:27:38.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/math/dimension/coordinates/generate/generate_shuffled_index_ls.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     4426 2022-07-29 07:53:01.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/math/dimension/coordinates/generate/generate_z_pattern_indices_ls.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1373 2023-03-10 13:56:45.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/math/dimension/coordinates/generate/normal_indices_generator.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-06 13:16:20.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/math/dimension/reshape/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      220 2022-07-25 13:28:44.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/math/dimension/reshape/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1946 2023-03-31 07:27:38.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/math/dimension/reshape/flatten_along_pattern.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1064 2023-03-31 07:27:37.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/math/dimension/reshape/merge_blocks.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1236 2023-03-31 07:27:37.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/math/dimension/reshape/split_blocks.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1859 2023-03-31 07:27:37.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/math/dimension/reshape/unflatten_along_pattern.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-06 13:16:20.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/math/dimension/transpose/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      177 2022-05-31 10:43:01.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/math/dimension/transpose/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      611 2022-08-09 13:17:49.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/math/dimension/transpose/get_inverse_of_transpose_index_ls.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1472 2023-03-31 07:27:38.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/math/dimension/transpose/transpose_inside_axis.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-06 13:16:20.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/math/number_theory/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      182 2023-03-05 15:57:35.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/math/number_theory/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      244 2023-03-05 15:45:13.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/math/number_theory/cache.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      387 2023-03-05 15:57:35.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/math/number_theory/get_greatest_common_divisor.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      949 2023-03-31 07:27:38.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/math/number_theory/get_primes.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      499 2023-03-31 07:27:37.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/math/number_theory/prime_factorization.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-06 13:16:20.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/math/number_theory/test/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-03-06 07:12:06.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/math/number_theory/test/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      747 2023-03-31 07:27:37.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/math/number_theory/test/test_get_greatest_common_divisor.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      784 2023-03-31 07:27:38.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/math/number_theory/test/test_get_primes.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      551 2023-03-31 07:27:37.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/math/number_theory/test/test_prime_factorization.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-06 13:16:20.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/math/transform/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-06-10 08:52:28.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/math/transform/__init__.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-06 13:16:20.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/math/transform/dct/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      147 2022-07-22 13:25:44.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/math/transform/dct/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     8296 2023-03-31 07:27:37.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/math/transform/dct/dct_calculator.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     4305 2022-07-20 12:21:16.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/math/transform/dct/generate_dct_trans_matrix.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-06 13:16:20.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/math/transform/scaling_and_shift/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       29 2022-07-30 13:19:40.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/math/transform/scaling_and_shift/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1280 2022-07-30 13:48:26.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/math/transform/scaling_and_shift/scaling.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-06 13:16:20.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/math/utils/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      289 2024-03-18 06:58:41.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/math/utils/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1943 2022-08-09 12:09:28.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/math/utils/convert_dtype.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1620 2022-08-08 08:50:02.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/math/utils/get_crop_by_box.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1553 2022-08-02 12:15:03.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/math/utils/get_function_table_for_array_and_tensor.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1775 2022-08-08 08:50:02.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/math/utils/set_crop_by_box.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      345 2024-03-18 06:57:03.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/math/utils/split_integer_most_evenly.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-06 13:16:20.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/nested_dict_list/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      333 2023-12-14 13:19:07.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/nested_dict_list/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     6144 2023-10-16 08:29:56.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/nested_dict_list/copy_.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      614 2023-07-25 12:37:51.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/nested_dict_list/count_leaf_node_nums.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1286 2023-06-21 01:55:54.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/nested_dict_list/get_hash.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3748 2024-01-16 12:22:50.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/nested_dict_list/get_nodes.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2083 2023-07-26 06:32:19.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/nested_dict_list/get_value.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-06 13:16:20.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/nested_dict_list/name_handler/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      107 2023-06-20 10:05:38.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/nested_dict_list/name_handler/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      989 2024-01-16 12:37:35.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/nested_dict_list/name_handler/build_name.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1163 2023-08-14 09:09:48.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/nested_dict_list/name_handler/escape_node.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2280 2024-01-16 12:38:24.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/nested_dict_list/name_handler/parse_name.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-06 13:16:20.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/nested_dict_list/serializer/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      153 2024-04-05 12:12:56.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/nested_dict_list/serializer/__init__.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-06 13:16:20.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/nested_dict_list/serializer/backends/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       39 2023-07-20 06:49:05.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/nested_dict_list/serializer/backends/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2145 2023-08-14 12:43:06.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/nested_dict_list/serializer/backends/_json_.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1652 2023-08-10 04:59:20.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/nested_dict_list/serializer/backends/_ndl.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1470 2023-07-25 12:39:59.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/nested_dict_list/serializer/backends/_numpy_bin.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1384 2023-07-25 12:39:59.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/nested_dict_list/serializer/backends/_numpy_npy.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1282 2023-07-25 12:39:59.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/nested_dict_list/serializer/backends/_pickle_.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      853 2023-07-25 12:39:59.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/nested_dict_list/serializer/backends/_skip_all.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1444 2023-08-14 12:33:39.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/nested_dict_list/serializer/backends/_skip_simple.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1282 2023-07-25 12:39:59.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/nested_dict_list/serializer/backends/_torch_all.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1353 2023-07-25 12:39:59.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/nested_dict_list/serializer/backends/_torch_tensor.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1741 2023-07-20 07:15:24.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/nested_dict_list/serializer/backends/backend_base.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      847 2023-11-28 09:24:46.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/nested_dict_list/serializer/enum_variable.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2843 2024-04-06 12:37:00.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/nested_dict_list/serializer/read.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1011 2024-04-05 12:12:56.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/nested_dict_list/serializer/saved_node_name_builder.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      392 2023-11-28 09:24:46.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/nested_dict_list/serializer/variable.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)    21024 2024-04-06 12:37:00.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/nested_dict_list/serializer/write.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3460 2024-01-26 09:17:13.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/nested_dict_list/set_default.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3470 2023-12-13 10:59:57.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/nested_dict_list/set_value.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     6846 2023-08-14 09:08:40.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/nested_dict_list/traverse.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-06 13:16:20.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/nested_dict_list/value_parser/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      313 2024-04-06 11:51:04.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/nested_dict_list/value_parser/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3119 2023-07-25 12:39:59.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/nested_dict_list/value_parser/cal_relation_between_references.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2301 2023-07-26 06:32:19.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/nested_dict_list/value_parser/eval_references.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2370 2023-08-23 12:32:31.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/nested_dict_list/value_parser/parse_and_eval_references.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2116 2023-07-26 06:32:19.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/nested_dict_list/value_parser/parse_references.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     5419 2024-04-06 12:03:12.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/nested_dict_list/value_parser/replace_identical_with_reference.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-06 13:16:20.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/patches/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-03-29 13:28:32.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/patches/__init__.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-06 13:16:20.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/patches/for_logging/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       39 2023-08-17 07:33:01.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/patches/for_logging/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3071 2024-01-05 07:58:55.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/patches/for_logging/build_logger.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-06 13:16:20.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/patches/for_matplotlib/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      180 2024-03-05 12:51:41.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/patches/for_matplotlib/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1837 2023-03-10 10:16:48.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/patches/for_matplotlib/add_trajectory_2d.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1696 2023-03-10 09:17:25.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/patches/for_matplotlib/add_trajectory_3d.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1361 2023-03-10 08:13:57.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/patches/for_matplotlib/arrow3d.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      984 2024-03-05 12:51:00.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/patches/for_matplotlib/generate_color_list.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-06 13:16:20.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/patches/for_numpy/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       21 2023-10-10 13:48:12.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/patches/for_numpy/__init__.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-06 13:16:20.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/patches/for_numpy/linalg/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      128 2024-03-05 12:56:40.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/patches/for_numpy/linalg/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      423 2023-05-17 07:05:16.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/patches/for_numpy/linalg/cos_similar.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1080 2024-03-05 13:02:36.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/patches/for_numpy/linalg/entropy.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      625 2023-04-24 08:52:01.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/patches/for_numpy/linalg/normalize.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2095 2023-12-27 09:20:36.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/patches/for_numpy/linalg/softmax.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-06 13:16:20.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/patches/for_numpy/random/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      149 2024-01-22 07:02:28.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/patches/for_numpy/random/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1999 2024-04-01 10:25:48.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/patches/for_numpy/random/get_rng.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     5859 2024-03-05 13:12:47.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/patches/for_numpy/random/truncated_multivariate_normal.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3726 2024-03-05 13:11:35.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/patches/for_numpy/random/truncated_normal.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      231 2024-01-22 06:17:42.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/patches/for_numpy/random/variable.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-06 13:16:20.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/patches/for_optuna/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      249 2024-01-04 06:48:51.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/patches/for_optuna/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1705 2024-01-04 07:28:28.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/patches/for_optuna/build_sampler.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3327 2024-01-04 07:01:24.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/patches/for_optuna/build_storage.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2253 2024-01-04 07:55:17.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/patches/for_optuna/build_study.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2743 2024-01-04 06:46:32.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/patches/for_optuna/copy_study.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     7071 2023-12-13 09:36:59.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/patches/for_optuna/sample_from_feasible_domain.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-06 13:16:20.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/patches/for_optuna/serialize/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       35 2023-12-18 08:18:28.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/patches/for_optuna/serialize/__init__.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-06 13:16:20.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/patches/for_optuna/serialize/for_study/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       46 2024-01-03 09:50:06.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/patches/for_optuna/serialize/for_study/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2088 2024-01-24 11:00:35.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/patches/for_optuna/serialize/for_study/dump.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1818 2024-01-04 07:10:38.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/patches/for_optuna/serialize/for_study/load.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-06 13:16:20.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/patches/for_optuna/serialize/for_trial/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       46 2023-12-17 15:30:35.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/patches/for_optuna/serialize/for_trial/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      982 2023-12-18 07:02:18.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/patches/for_optuna/serialize/for_trial/dump.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      796 2023-12-17 15:43:49.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/patches/for_optuna/serialize/for_trial/load.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-06 13:16:20.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/patches/for_os/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      128 2023-12-13 07:02:56.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/patches/for_os/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      656 2023-07-21 09:38:57.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/patches/for_os/pack.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      750 2023-12-13 08:34:00.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/patches/for_os/remove.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1047 2023-07-21 09:40:06.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/patches/for_os/unpack.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     8376 2023-12-13 07:22:41.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/patches/for_os/walk.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-06 13:16:20.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/patches/for_test/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       49 2022-07-29 06:55:38.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/patches/for_test/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     5038 2023-08-11 11:15:23.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/patches/for_test/check_consistency.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-06 13:16:20.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/patches/for_torch/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-02-21 06:56:01.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/patches/for_torch/__init__.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-06 13:16:20.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/patches/for_torch/compatible/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       75 2023-03-08 07:01:29.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/patches/for_torch/compatible/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      393 2023-04-12 15:31:18.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/patches/for_torch/compatible/concat.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-06 13:16:20.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/patches/for_torch/compatible/linalg/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       44 2023-03-08 08:04:27.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/patches/for_torch/compatible/linalg/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      770 2023-04-12 15:31:18.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/patches/for_torch/compatible/linalg/norm.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      575 2023-04-12 15:31:18.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/patches/for_torch/compatible/linalg/svd.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-06 13:16:20.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/patches/for_torch/compatible/nn/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       35 2023-05-30 11:36:55.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/patches/for_torch/compatible/nn/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     5357 2023-04-12 15:31:18.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/patches/for_torch/compatible/nn/sequential.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      845 2023-04-12 15:31:18.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/patches/for_torch/compatible/tile.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      733 2023-04-12 15:36:21.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/patches/for_torch/compatible/where.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-06 13:16:20.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/patches/for_torch/math/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       68 2022-02-21 09:51:39.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/patches/for_torch/math/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2047 2022-02-22 06:43:43.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/patches/for_torch/math/get_y_at_x.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1378 2022-02-21 09:44:44.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/patches/for_torch/math/my_around.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-06 13:16:20.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/patches/for_torch/nn/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       39 2023-05-30 11:37:07.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/patches/for_torch/nn/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      223 2023-05-29 08:32:26.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox/patches/for_torch/nn/lambda_layer.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2024-04-06 13:16:20.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox_dev.egg-info/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2490 2024-04-06 13:16:20.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox_dev.egg-info/PKG-INFO
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)    19169 2024-04-06 13:16:20.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox_dev.egg-info/SOURCES.txt
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        1 2024-04-06 13:16:20.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox_dev.egg-info/dependency_links.txt
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       92 2024-04-06 13:16:20.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox_dev.egg-info/requires.txt
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       14 2024-04-06 13:16:20.000000 kevin-toolbox-dev-1.3.4/kevin_toolbox_dev.egg-info/top_level.txt
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       59 2023-03-31 06:32:36.000000 kevin-toolbox-dev-1.3.4/pyproject.toml
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      908 2024-04-06 13:16:20.000000 kevin-toolbox-dev-1.3.4/setup.cfg
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      733 2023-03-31 07:25:47.000000 kevin-toolbox-dev-1.3.4/setup.py
```

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/computer_science/algorithm/cache_manager/cache/cache_base.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/computer_science/algorithm/cache_manager/cache/cache_base.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/computer_science/algorithm/cache_manager/cache/memo_cache.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/computer_science/algorithm/cache_manager/cache/memo_cache.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/computer_science/algorithm/cache_manager/cache_manager.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/computer_science/algorithm/cache_manager/cache_manager.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/computer_science/algorithm/cache_manager/strategy/fifo_strategy.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/computer_science/algorithm/cache_manager/strategy/fifo_strategy.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/computer_science/algorithm/cache_manager/strategy/lfu_strategy.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/computer_science/algorithm/cache_manager/strategy/lfu_strategy.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/computer_science/algorithm/cache_manager/strategy/lru_strategy.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/computer_science/algorithm/cache_manager/strategy/lru_strategy.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/computer_science/algorithm/cache_manager/strategy/lst_strategy.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/computer_science/algorithm/cache_manager/strategy/lst_strategy.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/computer_science/algorithm/cache_manager/strategy/strategy_base.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/computer_science/algorithm/cache_manager/strategy/strategy_base.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/computer_science/algorithm/cache_manager/test/test_cache_builder.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/computer_science/algorithm/cache_manager/test/test_cache_builder.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/computer_science/algorithm/cache_manager/test/test_cache_manager.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/computer_science/algorithm/cache_manager/test/test_cache_manager.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/computer_science/algorithm/cache_manager/test/test_cache_strategy.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/computer_science/algorithm/cache_manager/test/test_cache_strategy.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/computer_science/algorithm/cache_manager/variable.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/computer_science/algorithm/cache_manager/variable.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/computer_science/algorithm/combinatorial_optimization/get_subset_with_largest_product.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/computer_science/algorithm/combinatorial_optimization/get_subset_with_largest_product.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/computer_science/algorithm/combinatorial_optimization/test/test_get_subset_with_largest_product.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/computer_science/algorithm/combinatorial_optimization/test/test_get_subset_with_largest_product.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/computer_science/algorithm/combinatorial_optimization/test/test_zero_one_knapsack_problem.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/computer_science/algorithm/combinatorial_optimization/test/test_zero_one_knapsack_problem.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/computer_science/algorithm/combinatorial_optimization/zero_one_knapsack_problem.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/computer_science/algorithm/combinatorial_optimization/zero_one_knapsack_problem.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/computer_science/algorithm/execution_graph/jump_node.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/computer_science/algorithm/execution_graph/jump_node.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/computer_science/algorithm/execution_graph/random_node.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/computer_science/algorithm/execution_graph/random_node.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/computer_science/algorithm/execution_graph/simple_node.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/computer_science/algorithm/execution_graph/simple_node.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/computer_science/algorithm/for_dict/deep_update.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/computer_science/algorithm/for_dict/deep_update.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/computer_science/algorithm/for_seq/chunk_generator.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/computer_science/algorithm/for_seq/chunk_generator.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/computer_science/algorithm/for_seq/flatten_list.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/computer_science/algorithm/for_seq/flatten_list.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/computer_science/algorithm/locks/mutex_lock.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/computer_science/algorithm/locks/mutex_lock.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/computer_science/algorithm/parallel_and_concurrent/async_executor.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/computer_science/algorithm/parallel_and_concurrent/async_executor.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/computer_science/algorithm/parallel_and_concurrent/multi_thread_execute.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/computer_science/algorithm/parallel_and_concurrent/multi_thread_execute.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/computer_science/algorithm/pareto_front/get_pareto_points_idx.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/computer_science/algorithm/pareto_front/get_pareto_points_idx.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/computer_science/algorithm/registration/registry.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/computer_science/algorithm/registration/registry.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/computer_science/algorithm/scheduler/strategy_manager.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/computer_science/algorithm/scheduler/strategy_manager.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/computer_science/algorithm/scheduler/trigger.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/computer_science/algorithm/scheduler/trigger.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/computer_science/algorithm/search/binary_search.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/computer_science/algorithm/search/binary_search.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/computer_science/algorithm/statistician/accumulator_base.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/computer_science/algorithm/statistician/accumulator_base.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/computer_science/algorithm/statistician/average_accumulator.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/computer_science/algorithm/statistician/average_accumulator.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/computer_science/algorithm/statistician/exponential_moving_average.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/computer_science/algorithm/statistician/exponential_moving_average.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/computer_science/algorithm/statistician/init_var/init_by_data_format.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/computer_science/algorithm/statistician/init_var/init_by_data_format.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/computer_science/algorithm/statistician/init_var/init_by_like.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/computer_science/algorithm/statistician/init_var/init_by_like.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/computer_science/data_structure/executor.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/computer_science/data_structure/executor.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/dangerous/dump_into_pickle_with_executor_attached.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/dangerous/dump_into_pickle_with_executor_attached.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/data_flow/core/cache/cache_manager_for_iterator.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/data_flow/core/cache/cache_manager_for_iterator.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/data_flow/core/cache/test/test_cache_manager_for_iterator.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/data_flow/core/cache/test/test_cache_manager_for_iterator.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/data_flow/core/reader/file_iterative_reader.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/data_flow/core/reader/file_iterative_reader.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/data_flow/core/reader/unified_reader.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/data_flow/core/reader/unified_reader.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/data_flow/core/reader/unified_reader_base.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/data_flow/core/reader/unified_reader_base.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/data_flow/file/json_/converter/convert_dict_key_to_number.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/data_flow/file/json_/converter/convert_dict_key_to_number.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/data_flow/file/json_/converter/escape_non_str_dict_key.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/data_flow/file/json_/converter/escape_non_str_dict_key.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/data_flow/file/json_/converter/escape_tuple_and_set.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/data_flow/file/json_/converter/escape_tuple_and_set.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/data_flow/file/json_/converter/unescape_non_str_dict_key.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/data_flow/file/json_/converter/unescape_non_str_dict_key.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/data_flow/file/json_/converter/unescape_tuple_and_set.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/data_flow/file/json_/converter/unescape_tuple_and_set.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/data_flow/file/json_/read_json.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/data_flow/file/json_/read_json.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/data_flow/file/json_/write_json.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/data_flow/file/json_/write_json.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/data_flow/file/kevin_notation/converter.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/data_flow/file/kevin_notation/converter.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/data_flow/file/kevin_notation/kevin_notation_reader.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/data_flow/file/kevin_notation/kevin_notation_reader.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/data_flow/file/kevin_notation/kevin_notation_writer.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/data_flow/file/kevin_notation/kevin_notation_writer.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/data_flow/file/kevin_notation/read.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/data_flow/file/kevin_notation/read.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/data_flow/file/kevin_notation/test/test_kevin_notation.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/data_flow/file/kevin_notation/test/test_kevin_notation.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/data_flow/file/kevin_notation/write.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/data_flow/file/kevin_notation/write.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/data_flow/file/markdown/generate_list.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/data_flow/file/markdown/generate_list.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/data_flow/file/markdown/generate_table.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/data_flow/file/markdown/generate_table.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/developing/design_pattern/producer_consumer/consumer.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/developing/design_pattern/producer_consumer/consumer.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/developing/design_pattern/producer_consumer/for_cvf.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/developing/design_pattern/producer_consumer/for_cvf.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/developing/design_pattern/producer_consumer/graph.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/developing/design_pattern/producer_consumer/graph.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/developing/design_pattern/producer_consumer/node.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/developing/design_pattern/producer_consumer/node.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/developing/design_pattern/singleton/singleton_for_uid.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/developing/design_pattern/singleton/singleton_for_uid.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/developing/general_matrix_multiplication.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/developing/general_matrix_multiplication.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/developing/numerical_characteristics/iou.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/developing/numerical_characteristics/iou.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/developing/temperate/__init__.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/developing/temperate/__init__.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/developing/temperate/my_iterator.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/developing/temperate/my_iterator.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/developing/temperate/my_iterator_base.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/developing/temperate/my_iterator_base.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/env_info/check_validity_and_uninstall.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/env_info/check_validity_and_uninstall.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/env_info/check_version_and_update.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/env_info/check_version_and_update.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/env_info/test/test_version.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/env_info/test/test_version.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/env_info/version/compare_version.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/env_info/version/compare_version.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/env_info/version/parse_version.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/env_info/version/parse_version.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/env_info/version/sort_version_ls.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/env_info/version/sort_version_ls.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/geometry/for_boxes/__init__.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/geometry/for_boxes/__init__.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/geometry/for_boxes/__old_version/cal_iou_between_box.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/geometry/for_boxes/__old_version/cal_iou_between_box.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/geometry/for_boxes/boolean_algebra_for_boxes.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/geometry/for_boxes/boolean_algebra_for_boxes.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/geometry/for_boxes/cal_iou_between_boxes.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/geometry/for_boxes/cal_iou_between_boxes.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/geometry/for_boxes/convert_boxes_from_coord_to_grid_index.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/geometry/for_boxes/convert_boxes_from_coord_to_grid_index.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/geometry/for_boxes/detect_collision.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/geometry/for_boxes/detect_collision.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/geometry/for_boxes/detect_collision_among_boxes_ls.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/geometry/for_boxes/detect_collision_among_boxes_ls.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/geometry/for_boxes/detect_collision_inside_boxes.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/geometry/for_boxes/detect_collision_inside_boxes.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/geometry/for_boxes/detect_overlap.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/geometry/for_boxes/detect_overlap.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/machine_learning/dataset/face/analysis/get_fail_case_from_iterator.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/machine_learning/dataset/face/analysis/get_fail_case_from_iterator.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/machine_learning/dataset/face/dummy/dummy_data.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/machine_learning/dataset/face/dummy/dummy_data.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/machine_learning/dataset/face/verification/build_generator.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/machine_learning/dataset/face/verification/build_generator.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/machine_learning/dataset/face/verification/build_iterator.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/machine_learning/dataset/face/verification/build_iterator.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/machine_learning/dataset/face/verification/factory.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/machine_learning/dataset/face/verification/factory.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/__by_block/along_axis.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/__by_block/along_axis.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/__by_block/along_diagonal.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/__by_block/along_diagonal.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/__by_block/of_all.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/__by_block/of_all.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/__by_block/of_triangle.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/__by_block/of_triangle.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/by_block.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/by_block.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/by_samples.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/by_samples.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/machine_learning/statistician/binary_classification/confusion_matrices/accumulator_for_cfm.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/machine_learning/statistician/binary_classification/confusion_matrices/accumulator_for_cfm.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/machine_learning/statistician/binary_classification/confusion_matrices/cal_cfm.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/machine_learning/statistician/binary_classification/confusion_matrices/cal_cfm.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/machine_learning/statistician/binary_classification/confusion_matrices/cal_cfm_iteratively_by_chunk.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/machine_learning/statistician/binary_classification/confusion_matrices/cal_cfm_iteratively_by_chunk.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/machine_learning/statistician/binary_classification/confusion_matrices/cal_tpr_and_fpr.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/machine_learning/statistician/binary_classification/confusion_matrices/cal_tpr_and_fpr.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/machine_learning/statistician/binary_classification/confusion_matrices/merge_cfm_ls.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/machine_learning/statistician/binary_classification/confusion_matrices/merge_cfm_ls.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/math/dimension/concat_and_split/computational_tree.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/math/dimension/concat_and_split/computational_tree.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/math/dimension/concat_and_split/concat_crops_into_whole.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/math/dimension/concat_and_split/concat_crops_into_whole.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/math/dimension/concat_and_split/split_whole_into_crops.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/math/dimension/concat_and_split/split_whole_into_crops.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/math/dimension/coordinates/convert/convert_format.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/math/dimension/coordinates/convert/convert_format.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/math/dimension/coordinates/generate/generate_integrated_api.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/math/dimension/coordinates/generate/generate_integrated_api.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/math/dimension/coordinates/generate/generate_shuffled_index_ls.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/math/dimension/coordinates/generate/generate_shuffled_index_ls.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/math/dimension/coordinates/generate/generate_z_pattern_indices_ls.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/math/dimension/coordinates/generate/generate_z_pattern_indices_ls.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/math/dimension/coordinates/generate/normal_indices_generator.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/math/dimension/coordinates/generate/normal_indices_generator.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/math/dimension/reshape/flatten_along_pattern.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/math/dimension/reshape/flatten_along_pattern.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/math/dimension/reshape/merge_blocks.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/math/dimension/reshape/merge_blocks.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/math/dimension/reshape/split_blocks.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/math/dimension/reshape/split_blocks.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/math/dimension/reshape/unflatten_along_pattern.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/math/dimension/reshape/unflatten_along_pattern.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/math/dimension/transpose/get_inverse_of_transpose_index_ls.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/math/dimension/transpose/get_inverse_of_transpose_index_ls.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/math/dimension/transpose/transpose_inside_axis.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/math/dimension/transpose/transpose_inside_axis.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/math/number_theory/get_primes.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/math/number_theory/get_primes.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/math/number_theory/test/test_get_greatest_common_divisor.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/math/number_theory/test/test_get_greatest_common_divisor.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/math/number_theory/test/test_get_primes.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/math/number_theory/test/test_get_primes.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/math/number_theory/test/test_prime_factorization.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/math/number_theory/test/test_prime_factorization.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/math/transform/dct/dct_calculator.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/math/transform/dct/dct_calculator.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/math/transform/dct/generate_dct_trans_matrix.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/math/transform/dct/generate_dct_trans_matrix.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/math/transform/scaling_and_shift/scaling.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/math/transform/scaling_and_shift/scaling.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/math/utils/convert_dtype.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/math/utils/convert_dtype.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/math/utils/get_crop_by_box.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/math/utils/get_crop_by_box.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/math/utils/get_function_table_for_array_and_tensor.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/math/utils/get_function_table_for_array_and_tensor.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/math/utils/set_crop_by_box.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/math/utils/set_crop_by_box.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/nested_dict_list/copy_.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/nested_dict_list/copy_.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/nested_dict_list/count_leaf_node_nums.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/nested_dict_list/count_leaf_node_nums.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/nested_dict_list/get_hash.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/nested_dict_list/get_hash.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/nested_dict_list/get_nodes.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/nested_dict_list/get_nodes.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/nested_dict_list/get_value.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/nested_dict_list/get_value.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/nested_dict_list/name_handler/build_name.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/nested_dict_list/name_handler/build_name.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/nested_dict_list/name_handler/escape_node.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/nested_dict_list/name_handler/escape_node.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/nested_dict_list/name_handler/parse_name.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/nested_dict_list/name_handler/parse_name.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/nested_dict_list/serializer/backends/_json_.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/nested_dict_list/serializer/backends/_json_.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/nested_dict_list/serializer/backends/_ndl.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/nested_dict_list/serializer/backends/_ndl.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/nested_dict_list/serializer/backends/_numpy_bin.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/nested_dict_list/serializer/backends/_numpy_bin.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/nested_dict_list/serializer/backends/_numpy_npy.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/nested_dict_list/serializer/backends/_numpy_npy.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/nested_dict_list/serializer/backends/_pickle_.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/nested_dict_list/serializer/backends/_pickle_.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/nested_dict_list/serializer/backends/_skip_all.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/nested_dict_list/serializer/backends/_skip_all.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/nested_dict_list/serializer/backends/_skip_simple.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/nested_dict_list/serializer/backends/_skip_simple.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/nested_dict_list/serializer/backends/_torch_all.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/nested_dict_list/serializer/backends/_torch_all.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/nested_dict_list/serializer/backends/_torch_tensor.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/nested_dict_list/serializer/backends/_torch_tensor.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/nested_dict_list/serializer/backends/backend_base.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/nested_dict_list/serializer/backends/backend_base.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/nested_dict_list/serializer/enum_variable.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/nested_dict_list/serializer/enum_variable.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/nested_dict_list/serializer/read.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/nested_dict_list/serializer/read.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,21 +25,23 @@
                 os.makedirs(temp_dir)
                 break
         for_os.unpack(source=input_path, target=temp_dir)
         input_path = os.path.join(temp_dir, os.listdir(temp_dir)[0])
 
     # 读取 var
     var = json_.read(file_path=os.path.join(input_path, "var.json"), b_use_suggested_converter=True)
+    # 读取 record
+    record_s = dict()
+    if os.path.isfile(os.path.join(input_path, "record.json")):
+        record_s = json_.read(file_path=os.path.join(input_path, "record.json"), b_use_suggested_converter=True)
 
     # 读取被处理的节点
     processed_nodes = []
-    if os.path.isfile(os.path.join(input_path, "record.json")):
-        for name, value in ndl.get_nodes(
-                var=json_.read(file_path=os.path.join(input_path, "record.json"),
-                               b_use_suggested_converter=True)["processed"], level=-1, b_strict=True):
+    if record_s:
+        for name, value in ndl.get_nodes(var=record_s["processed"], level=-1, b_strict=True):
             if value:
                 processed_nodes.append(name)
     else:
         def converter(idx, value):
             processed_nodes.append(idx)
             return value
 
@@ -53,14 +55,19 @@
     for name in processed_nodes:
         value = ndl.get_value(var=var, name=name)
         if isinstance(value, (dict,)) and "backend" in value and "name" in value:
             bk = SERIALIZER_BACKEND.get(name=value.pop("backend"))(folder=os.path.join(input_path, "nodes"))
             ndl.set_value(var=var, name=name, value=bk.read(**value))
 
     #
+    if record_s.get("b_keep_identical_relations", False):
+        from kevin_toolbox.nested_dict_list import value_parser
+        var = value_parser.replace_identical_with_reference(var=var, flag="same", b_reverse=True)
+
+    #
     if temp_dir is not None:
         for_os.remove(path=temp_dir, ignore_errors=True)
 
     return var
 
 
 if __name__ == '__main__':
```

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/nested_dict_list/serializer/write.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/nested_dict_list/serializer/write.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,24 +3,26 @@
 import warnings
 import kevin_toolbox
 from kevin_toolbox.data_flow.file import json_
 from kevin_toolbox.patches import for_os
 import kevin_toolbox.nested_dict_list as ndl
 from kevin_toolbox.nested_dict_list.traverse import Traversal_Mode
 from .enum_variable import Strictness_Level
+from .saved_node_name_builder import Saved_Node_Name_Builder
 
 
 def write(var, output_dir, settings=None, traversal_mode=Traversal_Mode.BFS, b_pack_into_tar=True,
-          strictness_level=Strictness_Level.COMPATIBLE, **kwargs):
+          strictness_level=Strictness_Level.COMPATIBLE, saved_node_name_format='{count}_{hash_name}',
+          b_keep_identical_relations=False, **kwargs):
     """
         将输入的嵌套字典列表 var 的结构和节点值保存到文件中
             遍历 var，匹配并使用 settings 中设置的保存方式来对各部分结构/节点进行序列化
             将会生成一个文件夹或者 .tar 文件，其中包含：
                 - var.json：     用于保存结构、简单节点值、复杂节点值/结构的序列化方式
-                - nodes/目录：    其中包含一系列 <name>.<suffix> 文件或者 <name> 文件夹，其中包含复杂节点值/结构的序列化结果
+                - nodes/：       该目录中包含一系列 <name>.<suffix> 文件或者 <name> 文件夹，其中包含复杂节点值/结构的序列化结果
                 - record.json：   其中记录了：
                                         {
                                             "processed": ... # 对哪些节点/部分进行了处理
                                             "raw_structure": ... # 原始结构
                                             "timestamp": ... # 保存时间
                                             "kt_version": ... # 使用哪个版本下的 kevin_toolbox
                                         }
@@ -78,33 +80,58 @@
                                                                                             且第一个匹配上的 backend 就成功写入。
                                             - "normal" / Strictness_Level.COMPATIBLE    所有节点均有一个或者多个匹配上的 backend，
                                                                                             但是首先匹配到的 backend 写入出错，
                                                                                             使用其后再次匹配到的其他 backend 能够成功写入
                                             - "low" / Strictness_Level.IGNORE_FAILURE   匹配不完整，或者某些节点尝试过所有匹配到
                                                                                             的 backend 之后仍然无法写入
                                         默认是 "normal"
+            saved_node_name_format: <str> nodes/目录下节点文件/文件夹的命名方式。
+                                        基本结构为：  '{<part_0>}...{<part_1>}...'
+                                        其中 {} 内将根据 part 指定的类型进行自动填充。目前支持以下几种选项：
+                                            - "raw_name"        该节点对应位置的 name。
+                                            - "id"              该节点在当前内存中的 id。
+                                            - "hash_name"       该节点位置 name 的 hash 值。
+                                            - "count"           累加计算，表示是保存的第几个节点。
+                                        ！！注意：
+                                            "raw_name" 该选项在 v1.3.3 前被使用，但是由于其可能含有 : 和 / 等特殊符号，当以其作为文件夹名时，
+                                                可能会引发错误。因此对于 windows 用户，禁止使用该选项，对于 mac 和 linux 用户，同样也不建议使用该选项。
+                                            "id" 虽然具有唯一性，但是其值对于每次运行是随机的。
+                                            "hash_name" 有极低的可能会发生 hash 碰撞。
+                                        综合而言：
+                                            建议使用 "hash_name" 和 "count" 的组合。
+                                        默认值为：
+                                            '{count}_{hash_name}'
+            b_keep_identical_relations: <boolean> 是否保留不同节点之间的 id 相等关系。
+                                        具体而言，就是使用 value_parser.replace_identical_with_reference() 函数将具有相同 id 的多个节点，
+                                            替换为单个节点和其多个引用的形式。
+                                        对于 ndl 中存在大量具有相同 id 的重复节点的情况，使用该操作可以额外达到压缩的效果。
+                                        默认为 False
     """
     from kevin_toolbox.nested_dict_list.serializer.variable import SERIALIZER_BACKEND
 
-    #
+    # 检查参数
     traversal_mode = Traversal_Mode(traversal_mode)
     strictness_level = Strictness_Level(strictness_level)
     os.makedirs(output_dir, exist_ok=True)
     var = ndl.copy_(var=var, b_deepcopy=False)
+    if b_keep_identical_relations:
+        from kevin_toolbox.nested_dict_list import value_parser
+        var = value_parser.replace_identical_with_reference(var=var, flag="same", b_reverse=False)
     if settings is None:
         settings = [{"match_cond": "<level>-1", "backend": (":skip:simple", ":numpy:npy", ":torch:tensor", ":pickle")}]
+    snn_builder = Saved_Node_Name_Builder(format_=saved_node_name_format)
 
     # 构建 processed_s
     #     为了避免重复处理节点/结构，首先构建与 var 具有相似结构的 processed_s 来记录处理处理进度。
     #     对于 processed_s，其节点值为 True 时表示该节点已经被处理，当节点值为 False 或者 list/dict 类型时表示该节点或者节点下面的结构中仍然
     #       存在未处理的部分。
     #     对于中间节点，只有其下所有叶节点都未处理时才会被匹配。
-    processed_s = dict()
+    processed_s = ndl.copy_(var=var, b_deepcopy=False, b_keep_internal_references=False)
     for n, _ in ndl.get_nodes(var=var, level=-1, b_strict=True):
-        ndl.set_value(var=processed_s, name=n, value=False, b_force=True)
+        ndl.set_value(var=processed_s, name=n, value=False, b_force=False)
     # processed_s_bak 用于记录 var 的原始结构
     processed_s_bak = ndl.copy_(var=processed_s, b_deepcopy=True)
     if "_hook_for_debug" in kwargs:
         kwargs["_hook_for_debug"]["processed"] = [["raw", ndl.copy_(var=processed_s, b_deepcopy=True)], ]
 
     # 处理 var
     backend_s = dict()
@@ -122,35 +149,29 @@
         t_mode = Traversal_Mode(setting.get("traversal_mode", traversal_mode))
         # _process and  paras
         if callable(setting["match_cond"]):
             if t_mode in (Traversal_Mode.DFS_PRE_ORDER, Traversal_Mode.BFS):
                 _process = _process_from_top_to_down
             else:
                 _process = _process_from_down_to_top
-            paras = dict(
-                var=var, processed_s=processed_s, match_cond=setting["match_cond"],
-                traversal_mode=t_mode, strictness_level=strictness_level
-            )
+            paras = dict(var=var, match_cond=setting["match_cond"], traversal_mode=t_mode)
         elif setting["match_cond"].startswith("<level>"):
             _process = _process_for_level
-            paras = dict(
-                var=var, processed_s=processed_s, processed_s_bak=processed_s_bak,
-                level=int(setting["match_cond"][7:]), strictness_level=strictness_level
-            )
+            paras = dict(var=var, processed_s_bak=processed_s_bak, level=int(setting["match_cond"][7:]))
         elif setting["match_cond"].startswith("<node>"):
             _process = _process_for_name
-            paras = dict(var=var, processed_s=processed_s, name=setting["match_cond"][6:],
-                         strictness_level=strictness_level)
+            paras = dict(var=var, name=setting["match_cond"][6:])
         else:
             raise ValueError(f'invalid match_cond: {setting["match_cond"]}')
         # 执行
         for i in backend_name_ls:
             # print(processed_s)
             # print(f'backend: {i}')
-            _process(backend=backend_s[i], **paras)
+            _process(backend=backend_s[i], strictness_level=strictness_level, processed_s=processed_s,
+                     snn_builder=snn_builder, **paras)
             if "_hook_for_debug" in kwargs:
                 kwargs["_hook_for_debug"]["processed"].append([i, ndl.copy_(var=processed_s, b_deepcopy=True)])
 
     # print(processed_s)
     # print(var)
 
     # 完整性检查
@@ -167,15 +188,16 @@
         assert len(failed_nodes) == 0, \
             f'please check settings to make sure all nodes have been covered and can be deal with backend'
 
     # 保存 var 的结构
     json_.write(content=var, file_path=os.path.join(output_dir, "var.json"), b_use_suggested_converter=True)
     # 保存处理结果（非必要）
     json_.write(content=dict(processed=processed_s, raw_structure=processed_s_bak, timestamp=time.time(),
-                             kt_version=kevin_toolbox.__version__),
+                             kt_version=kevin_toolbox.__version__,
+                             b_keep_identical_relations=b_keep_identical_relations),
                 file_path=os.path.join(output_dir, "record.json"), b_use_suggested_converter=True)
 
     # 打包成 .tar 文件
     if b_pack_into_tar:
         for_os.pack(source=output_dir)
         for_os.remove(path=output_dir, ignore_errors=True)
 
@@ -192,69 +214,71 @@
                 b_processed = True
                 break
         else:
             b_processed = False
     return b_processed
 
 
-def _process_for_level(var, processed_s, processed_s_bak, level, backend, strictness_level):
+def _process_for_level(var, processed_s, processed_s_bak, level, backend, strictness_level, snn_builder):
     for name, _ in ndl.get_nodes(var=processed_s_bak, level=level, b_strict=True):
         _process_for_name(var=var, processed_s=processed_s, name=name, backend=backend,
-                          strictness_level=strictness_level)
+                          strictness_level=strictness_level, snn_builder=snn_builder)
 
 
-def _process_for_name(var, processed_s, name, backend, strictness_level):
+def _process_for_name(var, processed_s, name, backend, strictness_level, snn_builder):
     if _judge_processed_or_not(processed_s=processed_s, name=name) is True:
         # has been processed
         return
     value = ndl.get_value(var=var, name=name, b_pop=False)
     if not backend.writable(var=value):
         # cannot be written by backend
         return
 
     # write by backend
+    snn_name = snn_builder(name=name, value=value)
     try:
-        res = backend.write(name=name, var=value)
+        res = backend.write(name=snn_name, var=value)
     except:
         assert strictness_level in (Strictness_Level.IGNORE_FAILURE, Strictness_Level.COMPATIBLE), \
             f'An error occurred when node {name} was saved using the first matched backend {backend}'
         return
     ndl.set_value(var=processed_s, name=name, value=True, b_force=False)
     ndl.set_value(var=var, name=name, value=res, b_force=False)
 
 
-def _process_from_top_to_down(var, processed_s, match_cond, backend, traversal_mode, strictness_level):
+def _process_from_top_to_down(var, processed_s, match_cond, backend, traversal_mode, strictness_level, snn_builder):
     def match_cond_(parent_type, idx, value):
         nonlocal match_cond, processed_s
 
         b_processed = _judge_processed_or_not(processed_s=processed_s, name=idx)
         if b_processed is True or not backend.writable(var=value):
             # has been processed or cannot be written by backend
             return False
 
         return match_cond(parent_type, idx, value)
 
     def converter(idx, value):
         nonlocal processed_s, backend, strictness_level
 
         # write by backend
+        snn_name = snn_builder(name=idx, value=value)
         try:
-            res = backend.write(name=idx, var=value)
+            res = backend.write(name=snn_name, var=value)
         except:
             assert strictness_level in (Strictness_Level.IGNORE_FAILURE, Strictness_Level.COMPATIBLE), \
                 f'An error occurred when node {name} was saved using the first matched backend {backend}'
             return value
         ndl.set_value(var=processed_s, name=idx, value=True, b_force=True)
         return res
 
     ndl.traverse(var=var, match_cond=match_cond_, action_mode="replace", converter=converter,
                  b_use_name_as_idx=True, traversal_mode=traversal_mode, b_traverse_matched_element=False)
 
 
-def _process_from_down_to_top(var, processed_s, match_cond, backend, traversal_mode, strictness_level):
+def _process_from_down_to_top(var, processed_s, match_cond, backend, traversal_mode, strictness_level, snn_builder):
     processed_s_raw, processed_s = processed_s, ndl.copy_(var=processed_s, b_deepcopy=True)
 
     def match_cond_(parent_type, idx, value):
         nonlocal match_cond, processed_s
 
         b_processed = _judge_processed_or_not(processed_s=processed_s, name=idx)
         ndl.set_value(var=processed_s, name=idx, value=b_processed, b_force=False)
@@ -264,16 +288,17 @@
 
         return match_cond(parent_type, idx, value)
 
     def converter(idx, value):
         nonlocal processed_s, backend, processed_s_raw, strictness_level
 
         # write by backend
+        snn_name = snn_builder(name=idx, value=value)
         try:
-            res = backend.write(name=idx, var=value)
+            res = backend.write(name=snn_name, var=value)
         except:
             assert strictness_level in (Strictness_Level.IGNORE_FAILURE, Strictness_Level.COMPATIBLE), \
                 f'An error occurred when node {name} was saved using the first matched backend {backend}'
             return value
         ndl.set_value(var=processed_s, name=idx, value=True, b_force=True)
         ndl.set_value(var=processed_s_raw, name=idx, value=True, b_force=True)
         return res
@@ -301,13 +326,13 @@
          "backend": (":pickle",),
          "traversal_mode": "dfs_post_order"},
         {"match_cond": "<level>-1",
          "backend": (":numpy:bin", ":torch:tensor")},
         {"match_cond": lambda _, __, value: not isinstance(value, (list, dict)),
          "backend": (":skip:simple",)},
     ]
-    write(var=var_, output_dir=os.path.join(os.path.dirname(__file__), "temp3"), traversal_mode="bfs",
+    write(var=var_, output_dir=os.path.join(os.path.dirname(__file__), "temp"), traversal_mode="bfs",
           b_pack_into_tar=True, settings=settings_, _hook_for_debug=_hook_for_debug)
 
     for bk_name, p in _hook_for_debug["processed"]:
         print(f'backend: {bk_name}')
         print(p)
```

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/nested_dict_list/set_default.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/nested_dict_list/set_default.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/nested_dict_list/set_value.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/nested_dict_list/set_value.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/nested_dict_list/traverse.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/nested_dict_list/traverse.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/nested_dict_list/value_parser/cal_relation_between_references.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/nested_dict_list/value_parser/cal_relation_between_references.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/nested_dict_list/value_parser/eval_references.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/nested_dict_list/value_parser/eval_references.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/nested_dict_list/value_parser/parse_and_eval_references.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/nested_dict_list/value_parser/parse_and_eval_references.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/nested_dict_list/value_parser/parse_references.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/nested_dict_list/value_parser/parse_references.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/patches/for_logging/build_logger.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/patches/for_logging/build_logger.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/patches/for_matplotlib/add_trajectory_2d.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/patches/for_matplotlib/add_trajectory_2d.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/patches/for_matplotlib/add_trajectory_3d.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/patches/for_matplotlib/add_trajectory_3d.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/patches/for_matplotlib/arrow3d.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/patches/for_matplotlib/arrow3d.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/patches/for_matplotlib/generate_color_list.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/patches/for_matplotlib/generate_color_list.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/patches/for_numpy/linalg/entropy.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/patches/for_numpy/linalg/entropy.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/patches/for_numpy/linalg/normalize.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/patches/for_numpy/linalg/normalize.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/patches/for_numpy/linalg/softmax.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/patches/for_numpy/linalg/softmax.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/patches/for_numpy/random/get_rng.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/patches/for_numpy/random/get_rng.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/patches/for_numpy/random/truncated_multivariate_normal.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/patches/for_numpy/random/truncated_multivariate_normal.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/patches/for_numpy/random/truncated_normal.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/patches/for_numpy/random/truncated_normal.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/patches/for_optuna/build_sampler.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/patches/for_optuna/build_sampler.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/patches/for_optuna/build_storage.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/patches/for_optuna/build_storage.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/patches/for_optuna/build_study.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/patches/for_optuna/build_study.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/patches/for_optuna/copy_study.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/patches/for_optuna/copy_study.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/patches/for_optuna/sample_from_feasible_domain.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/patches/for_optuna/sample_from_feasible_domain.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/patches/for_optuna/serialize/for_study/dump.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/patches/for_optuna/serialize/for_study/dump.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/patches/for_optuna/serialize/for_study/load.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/patches/for_optuna/serialize/for_study/load.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/patches/for_optuna/serialize/for_trial/dump.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/patches/for_optuna/serialize/for_trial/dump.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/patches/for_optuna/serialize/for_trial/load.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/patches/for_optuna/serialize/for_trial/load.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/patches/for_os/pack.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/patches/for_os/pack.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/patches/for_os/remove.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/patches/for_os/remove.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/patches/for_os/unpack.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/patches/for_os/unpack.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/patches/for_os/walk.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/patches/for_os/walk.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/patches/for_test/check_consistency.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/patches/for_test/check_consistency.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/patches/for_torch/compatible/linalg/norm.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/patches/for_torch/compatible/linalg/norm.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/patches/for_torch/compatible/linalg/svd.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/patches/for_torch/compatible/linalg/svd.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/patches/for_torch/compatible/nn/sequential.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/patches/for_torch/compatible/nn/sequential.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/patches/for_torch/compatible/tile.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/patches/for_torch/compatible/tile.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/patches/for_torch/compatible/where.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/patches/for_torch/compatible/where.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/patches/for_torch/math/get_y_at_x.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/patches/for_torch/math/get_y_at_x.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox/patches/for_torch/math/my_around.py` & `kevin-toolbox-dev-1.3.4/kevin_toolbox/patches/for_torch/math/my_around.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/kevin_toolbox_dev.egg-info/SOURCES.txt` & `kevin-toolbox-dev-1.3.4/kevin_toolbox_dev.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -230,14 +230,15 @@
 kevin_toolbox/nested_dict_list/name_handler/__init__.py
 kevin_toolbox/nested_dict_list/name_handler/build_name.py
 kevin_toolbox/nested_dict_list/name_handler/escape_node.py
 kevin_toolbox/nested_dict_list/name_handler/parse_name.py
 kevin_toolbox/nested_dict_list/serializer/__init__.py
 kevin_toolbox/nested_dict_list/serializer/enum_variable.py
 kevin_toolbox/nested_dict_list/serializer/read.py
+kevin_toolbox/nested_dict_list/serializer/saved_node_name_builder.py
 kevin_toolbox/nested_dict_list/serializer/variable.py
 kevin_toolbox/nested_dict_list/serializer/write.py
 kevin_toolbox/nested_dict_list/serializer/backends/__init__.py
 kevin_toolbox/nested_dict_list/serializer/backends/_json_.py
 kevin_toolbox/nested_dict_list/serializer/backends/_ndl.py
 kevin_toolbox/nested_dict_list/serializer/backends/_numpy_bin.py
 kevin_toolbox/nested_dict_list/serializer/backends/_numpy_npy.py
@@ -248,14 +249,15 @@
 kevin_toolbox/nested_dict_list/serializer/backends/_torch_tensor.py
 kevin_toolbox/nested_dict_list/serializer/backends/backend_base.py
 kevin_toolbox/nested_dict_list/value_parser/__init__.py
 kevin_toolbox/nested_dict_list/value_parser/cal_relation_between_references.py
 kevin_toolbox/nested_dict_list/value_parser/eval_references.py
 kevin_toolbox/nested_dict_list/value_parser/parse_and_eval_references.py
 kevin_toolbox/nested_dict_list/value_parser/parse_references.py
+kevin_toolbox/nested_dict_list/value_parser/replace_identical_with_reference.py
 kevin_toolbox/patches/__init__.py
 kevin_toolbox/patches/for_logging/__init__.py
 kevin_toolbox/patches/for_logging/build_logger.py
 kevin_toolbox/patches/for_matplotlib/__init__.py
 kevin_toolbox/patches/for_matplotlib/add_trajectory_2d.py
 kevin_toolbox/patches/for_matplotlib/add_trajectory_3d.py
 kevin_toolbox/patches/for_matplotlib/arrow3d.py
```

### Comparing `kevin-toolbox-dev-1.3.3/setup.cfg` & `kevin-toolbox-dev-1.3.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-dev-1.3.3/setup.py` & `kevin-toolbox-dev-1.3.4/setup.py`

 * *Files identical despite different names*

