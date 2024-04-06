# Comparing `tmp/roboquant-0.2.9.tar.gz` & `tmp/roboquant-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roboquant-0.2.9.tar", last modified: Fri Mar 22 14:09:29 2024, max compression
+gzip compressed data, was "roboquant-0.3.0.tar", last modified: Sat Apr  6 18:16:17 2024, max compression
```

## Comparing `roboquant-0.2.9.tar` & `roboquant-0.3.0.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 peter      (501) staff       (20)        0 2024-03-22 14:09:29.545033 roboquant-0.2.9/
--rw-r--r--   0 peter      (501) staff       (20)    11341 2024-02-24 08:38:46.000000 roboquant-0.2.9/LICENSE
--rw-r--r--   0 peter      (501) staff       (20)     5705 2024-03-22 14:09:29.544807 roboquant-0.2.9/PKG-INFO
--rw-r--r--   0 peter      (501) staff       (20)     3969 2024-03-04 21:33:59.000000 roboquant-0.2.9/README.md
--rw-r--r--   0 peter      (501) staff       (20)     2178 2024-03-22 11:34:12.000000 roboquant-0.2.9/pyproject.toml
-drwxr-xr-x   0 peter      (501) staff       (20)        0 2024-03-22 14:09:29.537076 roboquant-0.2.9/roboquant/
--rw-r--r--   0 peter      (501) staff       (20)      510 2024-03-22 13:40:47.000000 roboquant-0.2.9/roboquant/__init__.py
--rw-r--r--   0 peter      (501) staff       (20)     7104 2024-03-15 10:02:45.000000 roboquant-0.2.9/roboquant/account.py
-drwxr-xr-x   0 peter      (501) staff       (20)        0 2024-03-22 14:09:29.538183 roboquant-0.2.9/roboquant/brokers/
--rw-r--r--   0 peter      (501) staff       (20)       60 2024-02-24 08:38:46.000000 roboquant-0.2.9/roboquant/brokers/__init__.py
--rw-r--r--   0 peter      (501) staff       (20)     1630 2024-03-12 18:14:00.000000 roboquant-0.2.9/roboquant/brokers/broker.py
--rw-r--r--   0 peter      (501) staff       (20)     9670 2024-03-20 10:50:54.000000 roboquant-0.2.9/roboquant/brokers/ibkr.py
--rw-r--r--   0 peter      (501) staff       (20)     8130 2024-03-22 13:16:44.000000 roboquant-0.2.9/roboquant/brokers/simbroker.py
--rw-r--r--   0 peter      (501) staff       (20)      656 2024-03-01 08:16:54.000000 roboquant-0.2.9/roboquant/config.py
--rw-r--r--   0 peter      (501) staff       (20)     4997 2024-03-21 19:18:44.000000 roboquant-0.2.9/roboquant/event.py
-drwxr-xr-x   0 peter      (501) staff       (20)        0 2024-03-22 14:09:29.540510 roboquant-0.2.9/roboquant/feeds/
--rw-r--r--   0 peter      (501) staff       (20)      470 2024-03-22 11:40:33.000000 roboquant-0.2.9/roboquant/feeds/__init__.py
--rw-r--r--   0 peter      (501) staff       (20)     3056 2024-03-15 07:59:42.000000 roboquant-0.2.9/roboquant/feeds/aggregate.py
--rw-r--r--   0 peter      (501) staff       (20)     2403 2024-03-21 06:35:23.000000 roboquant-0.2.9/roboquant/feeds/alpacafeed.py
--rw-r--r--   0 peter      (501) staff       (20)     4316 2024-03-22 06:13:57.000000 roboquant-0.2.9/roboquant/feeds/csvfeed.py
--rw-r--r--   0 peter      (501) staff       (20)     2745 2024-03-03 06:53:49.000000 roboquant-0.2.9/roboquant/feeds/eventchannel.py
--rw-r--r--   0 peter      (501) staff       (20)     2977 2024-03-06 10:40:28.000000 roboquant-0.2.9/roboquant/feeds/feed.py
--rw-r--r--   0 peter      (501) staff       (20)     2201 2024-03-22 08:43:24.000000 roboquant-0.2.9/roboquant/feeds/feedutil.py
--rw-r--r--   0 peter      (501) staff       (20)     2161 2024-03-22 06:04:38.000000 roboquant-0.2.9/roboquant/feeds/historic.py
--rw-r--r--   0 peter      (501) staff       (20)     1082 2024-03-22 06:03:18.000000 roboquant-0.2.9/roboquant/feeds/live.py
--rw-r--r--   0 peter      (501) staff       (20)     1920 2024-03-09 08:48:46.000000 roboquant-0.2.9/roboquant/feeds/randomwalk.py
--rw-r--r--   0 peter      (501) staff       (20)    46215 2024-02-29 18:24:43.000000 roboquant-0.2.9/roboquant/feeds/sp500.json
--rw-r--r--   0 peter      (501) staff       (20)     3275 2024-03-15 07:40:52.000000 roboquant-0.2.9/roboquant/feeds/sqllitefeed.py
--rw-r--r--   0 peter      (501) staff       (20)     9382 2024-03-21 19:20:23.000000 roboquant-0.2.9/roboquant/feeds/tiingo.py
--rw-r--r--   0 peter      (501) staff       (20)     1924 2024-03-17 19:26:05.000000 roboquant-0.2.9/roboquant/feeds/yahoo.py
-drwxr-xr-x   0 peter      (501) staff       (20)        0 2024-03-22 14:09:29.541885 roboquant-0.2.9/roboquant/journals/
--rw-r--r--   0 peter      (501) staff       (20)      544 2024-02-27 10:15:50.000000 roboquant-0.2.9/roboquant/journals/__init__.py
--rw-r--r--   0 peter      (501) staff       (20)     2205 2024-03-09 20:55:00.000000 roboquant-0.2.9/roboquant/journals/alphabeta.py
--rw-r--r--   0 peter      (501) staff       (20)     1093 2024-03-22 06:52:35.000000 roboquant-0.2.9/roboquant/journals/basicjournal.py
--rw-r--r--   0 peter      (501) staff       (20)      859 2024-03-15 22:09:02.000000 roboquant-0.2.9/roboquant/journals/feedmetric.py
--rw-r--r--   0 peter      (501) staff       (20)      745 2024-03-08 14:22:23.000000 roboquant-0.2.9/roboquant/journals/journal.py
--rw-r--r--   0 peter      (501) staff       (20)      483 2024-02-27 10:15:50.000000 roboquant-0.2.9/roboquant/journals/metric.py
--rw-r--r--   0 peter      (501) staff       (20)     1973 2024-03-03 14:18:52.000000 roboquant-0.2.9/roboquant/journals/metricsjournal.py
--rw-r--r--   0 peter      (501) staff       (20)     2057 2024-03-09 20:55:19.000000 roboquant-0.2.9/roboquant/journals/pnlmetric.py
--rw-r--r--   0 peter      (501) staff       (20)      768 2024-02-27 12:20:58.000000 roboquant-0.2.9/roboquant/journals/pricemetric.py
--rw-r--r--   0 peter      (501) staff       (20)      709 2024-02-25 19:17:54.000000 roboquant-0.2.9/roboquant/journals/runmetric.py
--rw-r--r--   0 peter      (501) staff       (20)      996 2024-03-08 14:19:09.000000 roboquant-0.2.9/roboquant/journals/tensorboardjournal.py
-drwxr-xr-x   0 peter      (501) staff       (20)        0 2024-03-22 14:09:29.542586 roboquant-0.2.9/roboquant/ml/
--rw-r--r--   0 peter      (501) staff       (20)      263 2024-03-22 12:50:27.000000 roboquant-0.2.9/roboquant/ml/__init__.py
--rw-r--r--   0 peter      (501) staff       (20)     8622 2024-03-20 20:03:10.000000 roboquant-0.2.9/roboquant/ml/envs.py
--rw-r--r--   0 peter      (501) staff       (20)    14489 2024-03-22 13:42:22.000000 roboquant-0.2.9/roboquant/ml/features.py
--rw-r--r--   0 peter      (501) staff       (20)     3542 2024-03-22 13:02:08.000000 roboquant-0.2.9/roboquant/ml/strategies.py
--rw-r--r--   0 peter      (501) staff       (20)     6285 2024-03-22 13:02:36.000000 roboquant-0.2.9/roboquant/ml/torch.py
--rw-r--r--   0 peter      (501) staff       (20)     4477 2024-03-10 08:03:30.000000 roboquant-0.2.9/roboquant/order.py
--rw-r--r--   0 peter      (501) staff       (20)     2152 2024-03-20 10:11:05.000000 roboquant-0.2.9/roboquant/run.py
--rw-r--r--   0 peter      (501) staff       (20)     1480 2024-03-10 18:37:50.000000 roboquant-0.2.9/roboquant/signal.py
-drwxr-xr-x   0 peter      (501) staff       (20)        0 2024-03-22 14:09:29.543486 roboquant-0.2.9/roboquant/strategies/
--rw-r--r--   0 peter      (501) staff       (20)      232 2024-03-18 17:51:57.000000 roboquant-0.2.9/roboquant/strategies/__init__.py
--rw-r--r--   0 peter      (501) staff       (20)     1484 2024-03-22 07:01:54.000000 roboquant-0.2.9/roboquant/strategies/barstrategy.py
--rw-r--r--   0 peter      (501) staff       (20)     2085 2024-03-17 14:29:19.000000 roboquant-0.2.9/roboquant/strategies/buffer.py
--rw-r--r--   0 peter      (501) staff       (20)     1952 2024-03-20 12:16:23.000000 roboquant-0.2.9/roboquant/strategies/emacrossover.py
--rw-r--r--   0 peter      (501) staff       (20)     1248 2024-03-16 07:38:35.000000 roboquant-0.2.9/roboquant/strategies/multistrategy.py
--rw-r--r--   0 peter      (501) staff       (20)     1562 2024-03-16 07:38:35.000000 roboquant-0.2.9/roboquant/strategies/smacrossover.py
--rw-r--r--   0 peter      (501) staff       (20)      657 2024-03-17 10:40:19.000000 roboquant-0.2.9/roboquant/strategies/strategy.py
--rw-r--r--   0 peter      (501) staff       (20)     4692 2024-03-08 07:04:19.000000 roboquant-0.2.9/roboquant/timeframe.py
-drwxr-xr-x   0 peter      (501) staff       (20)        0 2024-03-22 14:09:29.544007 roboquant-0.2.9/roboquant/traders/
--rw-r--r--   0 peter      (501) staff       (20)       62 2024-02-27 10:15:50.000000 roboquant-0.2.9/roboquant/traders/__init__.py
--rw-r--r--   0 peter      (501) staff       (20)     8215 2024-03-21 13:10:58.000000 roboquant-0.2.9/roboquant/traders/flextrader.py
--rw-r--r--   0 peter      (501) staff       (20)     1360 2024-03-21 11:47:01.000000 roboquant-0.2.9/roboquant/traders/sizing.py
--rw-r--r--   0 peter      (501) staff       (20)      972 2024-03-12 18:54:12.000000 roboquant-0.2.9/roboquant/traders/trader.py
-drwxr-xr-x   0 peter      (501) staff       (20)        0 2024-03-22 14:09:29.544169 roboquant-0.2.9/roboquant.egg-info/
--rw-r--r--   0 peter      (501) staff       (20)     5705 2024-03-22 14:09:29.000000 roboquant-0.2.9/roboquant.egg-info/PKG-INFO
--rw-r--r--   0 peter      (501) staff       (20)     1710 2024-03-22 14:09:29.000000 roboquant-0.2.9/roboquant.egg-info/SOURCES.txt
--rw-r--r--   0 peter      (501) staff       (20)        1 2024-03-22 14:09:29.000000 roboquant-0.2.9/roboquant.egg-info/dependency_links.txt
--rw-r--r--   0 peter      (501) staff       (20)      268 2024-03-22 14:09:29.000000 roboquant-0.2.9/roboquant.egg-info/requires.txt
--rw-r--r--   0 peter      (501) staff       (20)       25 2024-03-22 14:09:29.000000 roboquant-0.2.9/roboquant.egg-info/top_level.txt
--rw-r--r--   0 peter      (501) staff       (20)       38 2024-03-22 14:09:29.545077 roboquant-0.2.9/setup.cfg
+drwxr-xr-x   0 peter      (501) staff       (20)        0 2024-04-06 18:16:17.026627 roboquant-0.3.0/
+-rw-r--r--   0 peter      (501) staff       (20)    11341 2024-02-24 08:38:46.000000 roboquant-0.3.0/LICENSE
+-rw-r--r--   0 peter      (501) staff       (20)     5705 2024-04-06 18:16:17.026416 roboquant-0.3.0/PKG-INFO
+-rw-r--r--   0 peter      (501) staff       (20)     3969 2024-03-26 22:23:08.000000 roboquant-0.3.0/README.md
+-rw-r--r--   0 peter      (501) staff       (20)     2207 2024-04-06 09:38:53.000000 roboquant-0.3.0/pyproject.toml
+drwxr-xr-x   0 peter      (501) staff       (20)        0 2024-04-06 18:16:17.014286 roboquant-0.3.0/roboquant/
+-rw-r--r--   0 peter      (501) staff       (20)      499 2024-04-06 07:32:58.000000 roboquant-0.3.0/roboquant/__init__.py
+-rw-r--r--   0 peter      (501) staff       (20)     7367 2024-03-26 09:51:41.000000 roboquant-0.3.0/roboquant/account.py
+drwxr-xr-x   0 peter      (501) staff       (20)        0 2024-04-06 18:16:17.016070 roboquant-0.3.0/roboquant/brokers/
+-rw-r--r--   0 peter      (501) staff       (20)       60 2024-02-24 08:38:46.000000 roboquant-0.3.0/roboquant/brokers/__init__.py
+-rw-r--r--   0 peter      (501) staff       (20)     5021 2024-03-27 14:00:39.000000 roboquant-0.3.0/roboquant/brokers/alpacabroker.py
+-rw-r--r--   0 peter      (501) staff       (20)     2135 2024-03-27 12:19:51.000000 roboquant-0.3.0/roboquant/brokers/broker.py
+-rw-r--r--   0 peter      (501) staff       (20)     9249 2024-03-27 13:52:49.000000 roboquant-0.3.0/roboquant/brokers/ibkr.py
+-rw-r--r--   0 peter      (501) staff       (20)     9090 2024-03-26 07:55:20.000000 roboquant-0.3.0/roboquant/brokers/simbroker.py
+-rw-r--r--   0 peter      (501) staff       (20)      656 2024-03-01 08:16:54.000000 roboquant-0.3.0/roboquant/config.py
+-rw-r--r--   0 peter      (501) staff       (20)     5246 2024-03-25 15:12:17.000000 roboquant-0.3.0/roboquant/event.py
+drwxr-xr-x   0 peter      (501) staff       (20)        0 2024-04-06 18:16:17.019815 roboquant-0.3.0/roboquant/feeds/
+-rw-r--r--   0 peter      (501) staff       (20)      510 2024-04-06 09:06:56.000000 roboquant-0.3.0/roboquant/feeds/__init__.py
+-rw-r--r--   0 peter      (501) staff       (20)     3056 2024-03-15 07:59:42.000000 roboquant-0.3.0/roboquant/feeds/aggregate.py
+-rw-r--r--   0 peter      (501) staff       (20)     2459 2024-03-25 22:24:16.000000 roboquant-0.3.0/roboquant/feeds/alpacafeed.py
+-rw-r--r--   0 peter      (501) staff       (20)     6474 2024-03-27 06:24:15.000000 roboquant-0.3.0/roboquant/feeds/csvfeed.py
+-rw-r--r--   0 peter      (501) staff       (20)     2745 2024-03-03 06:53:49.000000 roboquant-0.3.0/roboquant/feeds/eventchannel.py
+-rw-r--r--   0 peter      (501) staff       (20)     3321 2024-04-05 12:09:17.000000 roboquant-0.3.0/roboquant/feeds/feed.py
+-rw-r--r--   0 peter      (501) staff       (20)     1712 2024-03-25 13:08:16.000000 roboquant-0.3.0/roboquant/feeds/feedutil.py
+-rw-r--r--   0 peter      (501) staff       (20)     2484 2024-03-25 12:56:18.000000 roboquant-0.3.0/roboquant/feeds/historic.py
+-rw-r--r--   0 peter      (501) staff       (20)     1082 2024-03-22 06:03:18.000000 roboquant-0.3.0/roboquant/feeds/live.py
+-rw-r--r--   0 peter      (501) staff       (20)     2528 2024-03-25 09:27:07.000000 roboquant-0.3.0/roboquant/feeds/randomwalk.py
+-rw-r--r--   0 peter      (501) staff       (20)    46215 2024-02-29 18:24:43.000000 roboquant-0.3.0/roboquant/feeds/sp500.json
+-rw-r--r--   0 peter      (501) staff       (20)     3275 2024-03-15 07:40:52.000000 roboquant-0.3.0/roboquant/feeds/sqllitefeed.py
+-rw-r--r--   0 peter      (501) staff       (20)     9394 2024-03-25 12:30:59.000000 roboquant-0.3.0/roboquant/feeds/tiingo.py
+-rw-r--r--   0 peter      (501) staff       (20)     1924 2024-03-17 19:26:05.000000 roboquant-0.3.0/roboquant/feeds/yahoo.py
+drwxr-xr-x   0 peter      (501) staff       (20)        0 2024-04-06 18:16:17.022263 roboquant-0.3.0/roboquant/journals/
+-rw-r--r--   0 peter      (501) staff       (20)      544 2024-02-27 10:15:50.000000 roboquant-0.3.0/roboquant/journals/__init__.py
+-rw-r--r--   0 peter      (501) staff       (20)     2205 2024-03-09 20:55:00.000000 roboquant-0.3.0/roboquant/journals/alphabeta.py
+-rw-r--r--   0 peter      (501) staff       (20)     1082 2024-03-24 15:36:00.000000 roboquant-0.3.0/roboquant/journals/basicjournal.py
+-rw-r--r--   0 peter      (501) staff       (20)      859 2024-03-15 22:09:02.000000 roboquant-0.3.0/roboquant/journals/feedmetric.py
+-rw-r--r--   0 peter      (501) staff       (20)      833 2024-04-04 07:40:36.000000 roboquant-0.3.0/roboquant/journals/journal.py
+-rw-r--r--   0 peter      (501) staff       (20)      478 2024-04-04 07:41:23.000000 roboquant-0.3.0/roboquant/journals/metric.py
+-rw-r--r--   0 peter      (501) staff       (20)     1973 2024-03-03 14:18:52.000000 roboquant-0.3.0/roboquant/journals/metricsjournal.py
+-rw-r--r--   0 peter      (501) staff       (20)     2057 2024-03-09 20:55:19.000000 roboquant-0.3.0/roboquant/journals/pnlmetric.py
+-rw-r--r--   0 peter      (501) staff       (20)      768 2024-02-27 12:20:58.000000 roboquant-0.3.0/roboquant/journals/pricemetric.py
+-rw-r--r--   0 peter      (501) staff       (20)      709 2024-02-25 19:17:54.000000 roboquant-0.3.0/roboquant/journals/runmetric.py
+-rw-r--r--   0 peter      (501) staff       (20)      996 2024-03-08 14:19:09.000000 roboquant-0.3.0/roboquant/journals/tensorboardjournal.py
+drwxr-xr-x   0 peter      (501) staff       (20)        0 2024-04-06 18:16:17.023116 roboquant-0.3.0/roboquant/ml/
+-rw-r--r--   0 peter      (501) staff       (20)        0 2024-04-06 07:33:32.000000 roboquant-0.3.0/roboquant/ml/__init__.py
+-rw-r--r--   0 peter      (501) staff       (20)     9034 2024-04-06 07:32:47.000000 roboquant-0.3.0/roboquant/ml/envs.py
+-rw-r--r--   0 peter      (501) staff       (20)    14583 2024-03-24 21:59:39.000000 roboquant-0.3.0/roboquant/ml/features.py
+-rw-r--r--   0 peter      (501) staff       (20)     9689 2024-04-04 07:32:09.000000 roboquant-0.3.0/roboquant/ml/strategies.py
+-rw-r--r--   0 peter      (501) staff       (20)     4477 2024-03-10 08:03:30.000000 roboquant-0.3.0/roboquant/order.py
+-rw-r--r--   0 peter      (501) staff       (20)     2142 2024-04-06 09:02:56.000000 roboquant-0.3.0/roboquant/run.py
+-rw-r--r--   0 peter      (501) staff       (20)     1500 2024-03-27 16:29:15.000000 roboquant-0.3.0/roboquant/signal.py
+drwxr-xr-x   0 peter      (501) staff       (20)        0 2024-04-06 18:16:17.024703 roboquant-0.3.0/roboquant/strategies/
+-rw-r--r--   0 peter      (501) staff       (20)      232 2024-03-18 17:51:57.000000 roboquant-0.3.0/roboquant/strategies/__init__.py
+-rw-r--r--   0 peter      (501) staff       (20)     1461 2024-03-27 16:30:10.000000 roboquant-0.3.0/roboquant/strategies/barstrategy.py
+-rw-r--r--   0 peter      (501) staff       (20)     2085 2024-03-17 14:29:19.000000 roboquant-0.3.0/roboquant/strategies/buffer.py
+-rw-r--r--   0 peter      (501) staff       (20)     2735 2024-04-05 13:37:28.000000 roboquant-0.3.0/roboquant/strategies/emacrossover.py
+-rw-r--r--   0 peter      (501) staff       (20)     1718 2024-04-05 13:37:34.000000 roboquant-0.3.0/roboquant/strategies/multistrategy.py
+-rw-r--r--   0 peter      (501) staff       (20)     1553 2024-03-27 16:11:34.000000 roboquant-0.3.0/roboquant/strategies/smacrossover.py
+-rw-r--r--   0 peter      (501) staff       (20)      652 2024-03-27 15:27:28.000000 roboquant-0.3.0/roboquant/strategies/strategy.py
+-rw-r--r--   0 peter      (501) staff       (20)     4354 2024-03-29 08:42:07.000000 roboquant-0.3.0/roboquant/timeframe.py
+drwxr-xr-x   0 peter      (501) staff       (20)        0 2024-04-06 18:16:17.025600 roboquant-0.3.0/roboquant/traders/
+-rw-r--r--   0 peter      (501) staff       (20)       62 2024-02-27 10:15:50.000000 roboquant-0.3.0/roboquant/traders/__init__.py
+-rw-r--r--   0 peter      (501) staff       (20)     9641 2024-03-27 16:51:27.000000 roboquant-0.3.0/roboquant/traders/flextrader.py
+-rw-r--r--   0 peter      (501) staff       (20)     1360 2024-03-21 11:47:01.000000 roboquant-0.3.0/roboquant/traders/sizing.py
+-rw-r--r--   0 peter      (501) staff       (20)      967 2024-03-27 16:15:47.000000 roboquant-0.3.0/roboquant/traders/trader.py
+drwxr-xr-x   0 peter      (501) staff       (20)        0 2024-04-06 18:16:17.025844 roboquant-0.3.0/roboquant.egg-info/
+-rw-r--r--   0 peter      (501) staff       (20)     5705 2024-04-06 18:16:17.000000 roboquant-0.3.0/roboquant.egg-info/PKG-INFO
+-rw-r--r--   0 peter      (501) staff       (20)     1722 2024-04-06 18:16:17.000000 roboquant-0.3.0/roboquant.egg-info/SOURCES.txt
+-rw-r--r--   0 peter      (501) staff       (20)        1 2024-04-06 18:16:17.000000 roboquant-0.3.0/roboquant.egg-info/dependency_links.txt
+-rw-r--r--   0 peter      (501) staff       (20)      268 2024-04-06 18:16:17.000000 roboquant-0.3.0/roboquant.egg-info/requires.txt
+-rw-r--r--   0 peter      (501) staff       (20)       25 2024-04-06 18:16:17.000000 roboquant-0.3.0/roboquant.egg-info/top_level.txt
+-rw-r--r--   0 peter      (501) staff       (20)       38 2024-04-06 18:16:17.026666 roboquant-0.3.0/setup.cfg
```

### Comparing `roboquant-0.2.9/LICENSE` & `roboquant-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `roboquant-0.2.9/PKG-INFO` & `roboquant-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roboquant
-Version: 0.2.9
+Version: 0.3.0
 Summary: A fast algo-trading platform
 Author-email: roboquant team <info@roboquant.org>
 Project-URL: Homepage, https://roboquant.org
 Project-URL: Repository, https://github.com/neurallayer/roboquant.py.git
 Project-URL: Issues, https://github.com/neurallayer/roboquant.py/issues
 Keywords: trading,investment,finance,crypto,stocks,exchange,forex
 Classifier: Development Status :: 3 - Alpha
@@ -63,15 +63,15 @@
 strategy = rq.strategies.EMACrossover()
 account = rq.run(feed, strategy)
 print(account)
 ```
 
 ## Install
 Roboquant can be installed like most other Python packages, using pip or conda.
-Make sure you have Python version 3.10 or higher installed.
+Make sure you have Python version 3.11 or higher installed.
 
 ```shell
 python3 -m pip install --upgrade roboquant
 ```
 
 You can also try roboquant in an online Jupyter Notebook [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/neurallayer/roboquant-notebooks/HEAD?labpath=%2Fintro_roboquant.ipynb)
```

### Comparing `roboquant-0.2.9/README.md` & `roboquant-0.3.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 strategy = rq.strategies.EMACrossover()
 account = rq.run(feed, strategy)
 print(account)
 ```
 
 ## Install
 Roboquant can be installed like most other Python packages, using pip or conda.
-Make sure you have Python version 3.10 or higher installed.
+Make sure you have Python version 3.11 or higher installed.
 
 ```shell
 python3 -m pip install --upgrade roboquant
 ```
 
 You can also try roboquant in an online Jupyter Notebook [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/neurallayer/roboquant-notebooks/HEAD?labpath=%2Fintro_roboquant.ipynb)
```

### Comparing `roboquant-0.2.9/pyproject.toml` & `roboquant-0.3.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 addopts = "-ra -q"
 testpaths = [
     "tests/unit"
 ]
 
 [tool.pyright]
 reportOptionalOperand = "none"
-exclude = ["samples/*.py"]
+exclude = ["samples/*.py", "scratch/*.py"]
 
 [tool.pylint.MASTER]
 ignore-paths = 'samples'
 
 [tool.pylint.'MESSAGES CONTROL']
 max-line-length = 127
 disable = "too-few-public-methods,missing-module-docstring,missing-class-docstring,missing-function-docstring,unnecessary-ellipsis"
@@ -23,15 +23,15 @@
 max-attributes = 10
 
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.packages.find]
-exclude = ["docs*", "tests*", "samples*"]
+exclude = ["docs*", "tests*", "samples*", "scratch*"]
 
 [tool.setuptools.package-data]
 "*" = ["*.json"]
 
 [project]
 name = "roboquant"
 dynamic = ["version"]
@@ -41,15 +41,15 @@
 requires-python = ">=3.10"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
-    "Programming Language :: Python :: 3.10",
+     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
     "Topic :: Office/Business :: Financial",
     "Topic :: Office/Business :: Financial :: Investment"
 ]
```

### Comparing `roboquant-0.2.9/roboquant/account.py` & `roboquant-0.3.0/roboquant/account.py`

 * *Files 5% similar despite different names*

```diff
@@ -131,14 +131,20 @@
         The returned value is denoted in the base currency of the account.
         """
         return sum(
             [self.contract_value(symbol, pos.size, pos.mkt_price) for symbol, pos in self.positions.items()],
             0.0,
         )
 
+    def position_value(self, symbol) -> float:
+        """Return position value denoted in the base currency of the account.
+        """
+        pos = self.positions.get(symbol)
+        return self.contract_value(symbol, pos.size, pos.mkt_price) if pos else 0.0
+
     def equity(self) -> float:
         """Return the equity of the account. It calcaluates the sum of the mkt value of
         each open position and adds the available cash.
 
         The returned value is denoted in the base currency of the account.
         """
         return self.cash + self.mkt_value()
```

### Comparing `roboquant-0.2.9/roboquant/brokers/broker.py` & `roboquant-0.3.0/roboquant/brokers/broker.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from abc import ABC, abstractmethod
+from datetime import datetime, timedelta, timezone
 
 from roboquant.account import Account
 from roboquant.event import Event
 from roboquant.order import Order
 
 
 class Broker(ABC):
@@ -47,7 +48,26 @@
         return
 
     account.last_update = event.time
 
     for symbol, position in account.positions.items():
         if price := event.get_price(symbol, price_type):
             position.mkt_price = price
+
+
+class LiveBroker(Broker):
+
+    def __init__(self) -> None:
+        super().__init__()
+        self.max_delay = timedelta(minutes=30)
+
+    def guard(self, event: Event | None = None) -> datetime:
+
+        now = datetime.now(timezone.utc)
+
+        if not event:
+            return now
+
+        if now - event.time > self.max_delay:
+            raise ValueError(f"received event too far in the past now={now} event-time={event.time}")
+
+        return now
```

### Comparing `roboquant-0.2.9/roboquant/brokers/ibkr.py` & `roboquant-0.3.0/roboquant/brokers/ibkr.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import logging
 import threading
 import time
-from datetime import datetime, timezone, timedelta
+from datetime import datetime, timedelta
 from decimal import Decimal
 
 from ibapi import VERSION
 from ibapi.account_summary_tags import AccountSummaryTags
 from ibapi.client import EClient
 from ibapi.contract import Contract
 from ibapi.order import Order as IBKROrder
 from ibapi.wrapper import EWrapper
 
 from roboquant.account import Account, Position
 from roboquant.event import Event
 from roboquant.order import Order, OrderStatus
-from roboquant.brokers.broker import Broker, _update_positions
+from roboquant.brokers.broker import LiveBroker, _update_positions
 
 assert VERSION["major"] == 10 and VERSION["minor"] == 19, "Wrong version of the IBAPI found"
 
 logger = logging.getLogger(__name__)
 
 
 # noinspection PyPep8Naming
@@ -112,15 +112,15 @@
                     order.status = OrderStatus.CANCELLED
                 case "Filled":
                     order.status = OrderStatus.FILLED
         else:
             logger.warning("received status for unknown order id=%s status=%s", orderId, status)
 
 
-class IBKRBroker(Broker):
+class IBKRBroker(LiveBroker):
     """
     Attributes
     ==========
     contract_mapping
         Map symbols to IBKR contracts.
         If a symbol is not found, the symbol is assumed to represent a US stock
 
@@ -133,14 +133,15 @@
        However these are just defaults, and can be modified as desired.
 
     client_id
         The client id to use to connect to TWS or IB Gateway.
     """
 
     def __init__(self, host="127.0.0.1", port=4002, client_id=123) -> None:
+        super().__init__()
         self.__account = Account()
         self.contract_mapping: dict[str, Contract] = {}
         api = _IBApi()
         api.connect(host, port, client_id)
         self.__api = api
         self.__has_new_orders_since_sync = False
         self.price_type = "DEFAULT"
@@ -166,23 +167,15 @@
 
     def _should_sync(self, now: datetime):
         """Avoid too many API calls"""
         return self.__has_new_orders_since_sync or now - self.__account.last_update > timedelta(seconds=1)
 
     def sync(self, event: Event | None = None) -> Account:
         """Sync with the IBKR account"""
-
-        logger.debug("start sync")
-        now = datetime.now(timezone.utc)
-
-        if event:
-            # Let make sure we don't use IBKRBroker by mistake during a back-test.
-            if now - event.time > timedelta(minutes=30):
-                logger.critical("received event from the past, now=%s event-time=%s", now, event.time)
-                raise ValueError(f"received event too far in the past now={now} event-time={event.time}")
+        now = self.guard(event)
 
         api = self.__api
         acc = self.__account
         if self._should_sync(now):
             acc.last_update = now
             self.__has_new_orders_since_sync = False
 
@@ -192,15 +185,14 @@
 
             acc.positions = {k: v for k, v in api.positions.items() if not v.size.is_zero()}
             acc.orders = list(api.orders.values())
             acc.buying_power = api.get_buying_power()
             acc.cash = api.get_cash()
 
         _update_positions(acc, event)
-        logger.debug("end sync")
         return acc
 
     def place_orders(self, orders):
 
         self.__has_new_orders_since_sync = len(orders) > 0
 
         for idx, order in enumerate(orders, start=1):
```

### Comparing `roboquant-0.2.9/roboquant/brokers/simbroker.py` & `roboquant-0.3.0/roboquant/brokers/simbroker.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from dataclasses import dataclass
 from datetime import timedelta
 from decimal import Decimal
 import logging
 
 from roboquant.account import Account, Position
 from roboquant.brokers.broker import Broker, _update_positions
-from roboquant.event import Event
+from roboquant.event import Event, PriceItem
 from roboquant.order import Order, OrderStatus
 
 logger = logging.getLogger(__name__)
 
 
 @dataclass(slots=True, frozen=True)
 class _Trx:
@@ -35,27 +35,29 @@
     ):
         super().__init__()
         self._account = Account()
         self._modify_orders: list[Order] = []
         self._create_orders: dict[str, Order] = {}
         self._account.cash = initial_deposit
         self._account.buying_power = initial_deposit
+        self._last_known_prices: dict[str, PriceItem] = {}
         self._order_id = 0
 
         self.slippage = slippage
         self.price_type = price_type
         self.clean_up_orders = clean_up_orders
         self.initial_deposit = initial_deposit
 
     def reset(self):
         self._account = Account()
         self._modify_orders: list[Order] = []
         self._create_orders: dict[str, Order] = {}
         self._account.cash = self.initial_deposit
         self._account.buying_power = self.initial_deposit
+        self._last_known_prices = {}
         self._order_id = 0
 
     def _update_account(self, trx: _Trx):
         """Update a position and cash based on a new transaction"""
         acc = self._account
         symbol = trx.symbol
         acc.cash -= acc.contract_value(symbol, trx.size, trx.price)
@@ -179,33 +181,51 @@
                     if trx is not None:
                         logger.info("executed order=%s trx=%s", order, trx)
                         self._update_account(trx)
                         order.fill += trx.size
                         if order.fill == order.size:
                             order.status = OrderStatus.FILLED
 
+    def _get_last_known_price(self, symbol):
+        item = self._last_known_prices.get(symbol)
+        return item.price(self.price_type) if item else None
+
+    def calculate_buyingpower(self):
+        """Calculate buying power, based on the available cash minus the open orders"""
+        bp = self._account.cash
+        for order in self._account.open_orders():
+            old_pos = self._account.get_position_size(order.symbol)
+            remaining = order.size - order.fill
+            if abs(old_pos + remaining) > abs(old_pos):
+                price = order.limit or self._get_last_known_price(order.symbol)
+                if price:
+                    reserve = self._account.contract_value(order.symbol, remaining, price)
+                    bp -= abs(reserve)
+        return bp
+
     def sync(self, event: Event | None = None) -> Account:
         """This will perform the order-execution simulation for the open orders and
         return the updated the account as a result."""
 
         acc = self._account
         if event:
             acc.last_update = event.time
 
         prices = event.price_items if event else {}
+        self._last_known_prices.update(prices)
 
         if self.clean_up_orders:
             # only keep the open orders from the previous step
-            # this improces performance a lot for large back tests
+            # this improves performance for large back tests
             self._create_orders = {order_id: order for order_id, order in self._create_orders.items() if order.is_open}
 
         self._process_modify_order()
         self._process_create_orders(prices)
         _update_positions(acc, event, self.price_type)
 
-        acc.buying_power = acc.cash
         acc.orders = list(self._create_orders.values())
+        acc.buying_power = self.calculate_buyingpower()
         return acc
 
     def __str__(self) -> str:
         attrs = " ".join([f"{k}={v}" for k, v in self.__dict__.items() if not k.startswith("_")])
         return f"SimBroker({attrs})"
```

### Comparing `roboquant-0.2.9/roboquant/config.py` & `roboquant-0.3.0/roboquant/config.py`

 * *Files identical despite different names*

### Comparing `roboquant-0.2.9/roboquant/event.py` & `roboquant-0.3.0/roboquant/event.py`

 * *Files 10% similar despite different names*

```diff
@@ -63,33 +63,39 @@
             case _:
                 # Default is the average volume
                 return (self.data[1] + self.data[3]) / 2.0
 
 
 @dataclass(slots=True)
 class Trade(PriceItem):
+    """Holds a single price and optional the volume.
+    Often this reflects an actual trade, but it can also be used in different scenarios.
+    """
     trade_price: float
     trade_volume: float
 
     def price(self, price_type: str = "DEFAULT") -> float:
         return self.trade_price
 
     def volume(self, volume_type: str = "DEFAULT") -> float:
         return self.trade_volume
 
 
 @dataclass(slots=True)
 class Bar(PriceItem):
+    """Represents a bar (a.k.a candlestick) with open, high, low, close and volume data.
+    """
+
     ohlcv: array
     frequency: str = ""  # f.e 1s , 15m, 4h, 1d
 
     @classmethod
     def from_adj_close(cls, symbol, ohlcv: array, adj_close: float, frequency=""):
         adj = adj_close / ohlcv[3]
-        ohlcv = array("f", [ohlcv[0] * adj, ohlcv[1] * adj, ohlcv[2] * adj, ohlcv[5], ohlcv[4] / adj])
+        ohlcv = array("f", [ohlcv[0] * adj, ohlcv[1] * adj, ohlcv[2] * adj, adj_close, ohlcv[4] / adj])
         return cls(symbol, ohlcv, frequency)
 
     def price(self, price_type: str = "DEFAULT") -> float:
         match price_type:
             case "OPEN":
                 return self.ohlcv[0]
             case "HIGH":
```

### Comparing `roboquant-0.2.9/roboquant/feeds/aggregate.py` & `roboquant-0.3.0/roboquant/feeds/aggregate.py`

 * *Files identical despite different names*

### Comparing `roboquant-0.2.9/roboquant/feeds/alpacafeed.py` & `roboquant-0.3.0/roboquant/feeds/alpacafeed.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,19 +13,19 @@
 from roboquant.feeds.live import LiveFeed
 
 
 class AlpacaLiveFeed(LiveFeed):
 
     __one_minute = str(timedelta(minutes=1))
 
-    def __init__(self, market: Literal["iex", "sip", "crypto", "option"] = "iex") -> None:
+    def __init__(self, market: Literal["iex", "sip", "crypto", "option"] = "iex", api_key=None, secret_key=None) -> None:
         super().__init__()
         config = Config()
-        api_key = config.get("alpaca.public.key")
-        secret_key = config.get("alpaca.secret.key")
+        api_key = api_key or config.get("alpaca.public.key")
+        secret_key = secret_key or config.get("alpaca.secret.key")
         match market:
             case "sip":
                 self.stream = StockDataStream(api_key, secret_key, feed=DataFeed.SIP)
             case "iex":
                 self.stream = StockDataStream(api_key, secret_key, feed=DataFeed.IEX)
             case "crypto":
                 self.stream = CryptoDataStream(api_key, secret_key)
```

### Comparing `roboquant-0.2.9/roboquant/feeds/csvfeed.py` & `roboquant-0.3.0/roboquant/feeds/csvfeed.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,40 +1,64 @@
 import csv
+from enum import Enum
 import sys
 import logging
 import os
 import pathlib
 from array import array
 from datetime import datetime, time, timezone
 
 from roboquant.event import Bar
 from roboquant.feeds.historic import HistoricFeed
 
 logger = logging.getLogger(__name__)
 
 
+class CSVColumn(str, Enum):
+
+    DATE = 'Date'
+    OPEN = 'Open'
+    HIGH = 'High'
+    LOW = 'Low'
+    CLOSE = 'Close'
+    VOLUME = "Volume"
+    ADJ_CLOSE = "Adj CLose"
+    TIME = "Time"
+
+    def __str__(self) -> str:
+        return self.value
+
+    @staticmethod
+    def merge(d: dict["CSVColumn", str]) -> list[str]:
+        return [d.get(e, e.value) for e in CSVColumn]
+
+
 class CSVFeed(HistoricFeed):
     """Use CSV files with historic data as a feed."""
 
     def __init__(
         self,
         path: str | pathlib.Path,
         columns=None,
         adj_close=False,
+        has_time_column=False,
         time_offset: str | None = None,
-        datetime_fmt: str | None = None,
+        date_fmt: str | None = None,
+        time_fmt: str | None = None,
         endswith=".csv",
         frequency="",
     ):
         super().__init__()
-        columns = columns or ["Date", "Open", "High", "Low", "Close", "Volume", "AdjClose"]
+        columns = columns or ["Date", "Open", "High", "Low", "Close", "Volume", "Adj Close", "Time"]
         self.ohlcv_columns = columns[1:6]
         self.adj_close_column = columns[6] if adj_close else None
         self.date_column = columns[0]
-        self.datetime_fmt = datetime_fmt
+        self.time_column = columns[7] if has_time_column else None
+        self.date_fmt = date_fmt
+        self.time_fmt = time_fmt
         self.adj_close = adj_close
         self.freq = frequency
         self.endswith = endswith
         self.time_offset = time.fromisoformat(time_offset) if time_offset is not None else None
 
         files = self._get_files(path)
         logger.info("located %s files in path %s", len(files), path)
@@ -51,64 +75,107 @@
         return files
 
     def _get_symbol(self, filename: str):
         """Return the symbol based on the filename"""
         return pathlib.Path(filename).stem.upper()
 
     def _parse_csvfiles(self, filenames: list[str]):
+        # pylint: disable=too-many-locals
         adj_close_column = self.adj_close_column
-        datetime_fmt = self.datetime_fmt
+        date_fmt = self.date_fmt
+        time_fmt = self.time_fmt
         ohlcv_columns = self.ohlcv_columns
         date_column = self.date_column
+        time_column = self.time_column
         freq = self.freq
         time_offset = self.time_offset
 
         for filename in filenames:
             symbol = self._get_symbol(filename)
             with open(filename, encoding="utf8") as csvfile:
                 reader = csv.DictReader(csvfile)
 
                 for row in reader:
                     date_str = row[date_column]
-                    dt = datetime.strptime(date_str, datetime_fmt) if datetime_fmt else datetime.fromisoformat(date_str)
+                    dt = datetime.strptime(date_str, date_fmt) if date_fmt else datetime.fromisoformat(date_str)
+                    if time_column:
+                        time_str = row[time_column]
+                        time_val = datetime.strptime(time_str, time_fmt).time() if time_fmt else time.fromisoformat(time_str)
+                        dt = datetime.combine(dt, time_val, timezone.utc)
+
                     if time_offset:
                         dt = datetime.combine(dt, time_offset)
 
                     ohlcv = array("f", [float(row[column]) for column in ohlcv_columns])
                     if adj_close_column:
                         adj_close = float(row[adj_close_column])
                         pb = Bar.from_adj_close(symbol, ohlcv, adj_close, freq)
                     else:
                         pb = Bar(symbol, ohlcv, freq)
+
                     self._add_item(dt.astimezone(timezone.utc), pb)
 
     @classmethod
     def stooq_us_daily(cls, path):
-        """Parse one or more CSV files that meet the stooq format"""
+        """Parse one or more CSV files that meet the stooq daily file format"""
         columns = ["<DATE>", "<OPEN>", "<HIGH>", "<LOW>", "<CLOSE>", "<VOL>"]
 
-        class StooqCSVFeed(CSVFeed):
+        class StooqDailyFeed(CSVFeed):
             def __init__(self):
                 # from Python 3.11 onwards we can use the fast standard ISO parsing
                 if sys.version_info >= (3, 11):
                     super().__init__(path, columns=columns, time_offset="21:00:00+00:00", endswith=".txt", frequency="1d")
                 else:
                     super().__init__(
                         path,
                         columns=columns,
                         time_offset="21:00:00+00:00",
-                        datetime_fmt="%Y%m%d",
+                        date_fmt="%Y%m%d",
                         endswith=".txt",
                         frequency="1d",
                     )
 
             def _get_symbol(self, filename: str):
-                base = pathlib.Path(filename).stem.upper()
-                return base.split(".")[0]
+                base = pathlib.Path(filename).stem
+                return base.split(".")[0].upper()
 
-        return StooqCSVFeed()
+        return StooqDailyFeed()
+
+    @classmethod
+    def stooq_us_intraday(cls, path):
+        """Parse one or more CSV files that meet the stooq intraday file format"""
+        columns = ["<DATE>", "<OPEN>", "<HIGH>", "<LOW>", "<CLOSE>", "<VOL>", "", "<TIME>"]
+
+        class StooqIntradayFeed(CSVFeed):
+            def __init__(self):
+                # from Python 3.11 onwards we can use the faster standard ISO parsing
+                if sys.version_info >= (3, 11):
+                    super().__init__(path, columns=columns, has_time_column=True, endswith=".txt")
+                else:
+                    super().__init__(
+                        path,
+                        columns=columns,
+                        has_time_column=True,
+                        date_fmt="%Y%m%d",
+                        time_fmt="%H%M%S",
+                        endswith=".txt"
+                    )
+
+            def _get_symbol(self, filename: str):
+                base = pathlib.Path(filename).stem
+                return base.split(".")[0].upper()
+
+        return StooqIntradayFeed()
 
     @classmethod
     def yahoo(cls, path, frequency="1d"):
         """Parse one or more CSV files that meet the Yahoo Finance format"""
         columns = ["Date", "Open", "High", "Low", "Close", "Volume", "Adj Close"]
         return cls(path, columns=columns, adj_close=True, time_offset="21:00:00+00:00", frequency=frequency)
+
+
+if __name__ == "__main__":
+    t = datetime.strptime("210000", "%H%M%S").time()
+    print(t)
+
+    t = time.fromisoformat("210000")
+    print(t)
```

### Comparing `roboquant-0.2.9/roboquant/feeds/eventchannel.py` & `roboquant-0.3.0/roboquant/feeds/eventchannel.py`

 * *Files identical despite different names*

### Comparing `roboquant-0.2.9/roboquant/feeds/feed.py` & `roboquant-0.3.0/roboquant/feeds/feed.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from datetime import datetime
 import threading
 from abc import ABC, abstractmethod
 
 from roboquant.feeds.eventchannel import EventChannel, ChannelClosed
 from roboquant.timeframe import Timeframe
 
 
@@ -19,14 +20,17 @@
         Parameters
         ----------
         channel : EventChannel
             EventChannel where the events will be placed.
         """
         ...
 
+    def timeframe(self) -> Timeframe | None:
+        return None
+
     def play_background(self, timeframe: Timeframe | None = None, channel_capacity: int = 10) -> EventChannel:
         """
         Plays this feed in the background on its own thread.
 
         Parameters
         ----------
         timeframe : Timeframe or None, optional
@@ -69,22 +73,30 @@
             The type of price to plot, e.g. open, close, high, low. (default is "DEFAULT")
         timeframe : Timeframe or None, optional
             The timeframe over which to plot prices. If None, the entire feed timeframe is used. (default is None)
         **kwargs
             Additional keyword arguments to pass to the plt.plot() function.
         """
 
-        channel = self.play_background(timeframe)
-        times = []
-        prices = []
-        while evt := channel.get():
-            price = evt.get_price(symbol, price_type)
-            if price is not None:
-                times.append(evt.time)
-                prices.append(price)
-
+        times, prices = get_symbol_prices(self, symbol, price_type, timeframe)
         plt.plot(times, prices, **kwargs)
         if hasattr(plt, "set_title"):
             # assume we are in a subplot
             plt.set_title(symbol)
         else:
             plt.title(symbol)
+
+
+def get_symbol_prices(
+        feed: Feed, symbol: str, price_type="DEFAULT", timeframe: Timeframe | None = None
+) -> tuple[list[datetime], list[float]]:
+    """Get prices for a single symbol from a feed"""
+
+    x = []
+    y = []
+    channel = feed.play_background(timeframe)
+    while event := channel.get():
+        price = event.get_price(symbol, price_type)
+        if price:
+            x.append(event.time)
+            y.append(price)
+    return x, y
```

### Comparing `roboquant-0.2.9/roboquant/feeds/feedutil.py` & `roboquant-0.3.0/roboquant/feeds/feedutil.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,32 +1,15 @@
 import json
 import pathlib
-from datetime import datetime
 
 from roboquant.event import Bar
 from roboquant.feeds.feed import Feed
 from roboquant.timeframe import Timeframe
 
 
-def get_symbol_prices(
-        feed: Feed, symbol: str, price_type="DEFAULT", timeframe: Timeframe | None = None
-) -> tuple[list[datetime], list[float]]:
-    """Get prices for a single symbol from a feed"""
-
-    x = []
-    y = []
-    channel = feed.play_background(timeframe)
-    while event := channel.get():
-        price = event.get_price(symbol, price_type)
-        if price:
-            x.append(event.time)
-            y.append(price)
-    return x, y
-
-
 def get_ohlcv(feed: Feed, symbol: str, timeframe: Timeframe | None = None) -> dict[str, list]:
     """Get the OHLCV values for a symbol from a feed.
     The returned value is a dict with the keys being "Date", "Open", "High", "Low", "Close", "Volume"
     and the values a list.
     """
 
     result = {column: [] for column in ["Date", "Open", "High", "Low", "Close", "Volume"]}
```

### Comparing `roboquant-0.2.9/roboquant/feeds/historic.py` & `roboquant-0.3.0/roboquant/feeds/historic.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from itertools import chain
 from typing import List
 
 from roboquant.event import Event, PriceItem
 from roboquant.timeframe import Timeframe
 from .eventchannel import EventChannel
 from .feed import Feed
+from .feedutil import get_ohlcv
 
 
 class HistoricFeed(Feed, ABC):
     """
     Abstract base class for feeds that produce historic price-items.
     """
 
@@ -46,14 +47,20 @@
         """Return the timeframe of this feed"""
         tl = self.timeline()
         if not tl:
             raise ValueError("Feed doesn't contain any events.")
 
         return Timeframe(tl[0], tl[-1], inclusive=True)
 
+    def get_ohlcv(self, symbol: str, timeframe=None) -> dict[str, list]:
+        """Get the OHLCV values for a symbol for the (optional) provided timeframe.
+        This makes it easy to plot prices and use them in a dataframe.
+        """
+        return get_ohlcv(self, symbol, timeframe)
+
     def __update(self):
         if self.__modified:
             self.__data = dict(sorted(self.__data.items()))
             price_items = chain.from_iterable(self.__data.values())
             self.__symbols = list({item.symbol for item in price_items})
             self.__modified = False
```

### Comparing `roboquant-0.2.9/roboquant/feeds/live.py` & `roboquant-0.3.0/roboquant/feeds/live.py`

 * *Files identical despite different names*

### Comparing `roboquant-0.2.9/roboquant/feeds/sp500.json` & `roboquant-0.3.0/roboquant/feeds/sp500.json`

 * *Files identical despite different names*

### Comparing `roboquant-0.2.9/roboquant/feeds/sqllitefeed.py` & `roboquant-0.3.0/roboquant/feeds/sqllitefeed.py`

 * *Files identical despite different names*

### Comparing `roboquant-0.2.9/roboquant/feeds/tiingo.py` & `roboquant-0.3.0/roboquant/feeds/tiingo.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     - Intraday crypto prices
     - Intraday forex prices
     """
 
     def __init__(self, key: str | None = None):
         super().__init__()
         self.key = key or Config().get("tiingo.key")
-        assert self.key, "no Tiingo key found"
+        assert self.key, "no Tiingo key provided or found"
         self.timeout = 10
 
     @staticmethod
     def __get_csv_iter(response: requests.Response):
         lines = response.content.decode("utf-8").splitlines()
         rows = iter(csv.reader(lines))
         next(rows, None)  # skip header line.
```

### Comparing `roboquant-0.2.9/roboquant/feeds/yahoo.py` & `roboquant-0.3.0/roboquant/feeds/yahoo.py`

 * *Files identical despite different names*

### Comparing `roboquant-0.2.9/roboquant/journals/__init__.py` & `roboquant-0.3.0/roboquant/journals/__init__.py`

 * *Files identical despite different names*

### Comparing `roboquant-0.2.9/roboquant/journals/alphabeta.py` & `roboquant-0.3.0/roboquant/journals/alphabeta.py`

 * *Files identical despite different names*

### Comparing `roboquant-0.2.9/roboquant/journals/basicjournal.py` & `roboquant-0.3.0/roboquant/journals/basicjournal.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,26 +5,26 @@
 
 logger = logging.getLogger(__name__)
 
 
 @dataclass
 class BasicJournal(Journal):
     """Tracks a number of basic metrics:
-    - total number of events, items, signalsm, orders and max positions until that time
+    - total number of events, items, signals, orders and max open positions.
 
     It will also log these values at each step in the run at `info` level.
 
-    This journal adds little overhead to a run, both CPU and memory wise and is helfull in
+    This journal adds little overhead to a run, both CPU and memory wise and is helpful in
     determning if the setup works correctly.
     """
 
+    events: int
     items: int
-    orders: int
     signals: int
-    events: int
+    orders: int
     max_positions: int
 
     def __init__(self):
         self.events = 0
         self.signals = 0
         self.items = 0
         self.orders = 0
```

### Comparing `roboquant-0.2.9/roboquant/journals/feedmetric.py` & `roboquant-0.3.0/roboquant/journals/feedmetric.py`

 * *Files identical despite different names*

### Comparing `roboquant-0.2.9/roboquant/journals/journal.py` & `roboquant-0.3.0/roboquant/journals/journal.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,11 +10,14 @@
     """
     A journal enables the tracking and/or logging of one or more metrics during a run.
 
     A journal can hold detailed records of all your trading activities in the financial markets.
     It serves as a tool to track and analyze their performance, decisions, and outcomes over time
     """
 
-    def track(self, event: Event, account: Account, signals: dict[str, Signal], orders: list[Order]):
+    def track(self, event: Event, account: Account, signals: list[Signal], orders: list[Order]):
         """invoked at each step of a run that provides the journal with the opportunity to
         track and log various metrics."""
         ...
+
+    def reset(self):
+        """reset the state of the journal, default is to do nothing"""
```

### Comparing `roboquant-0.2.9/roboquant/journals/metricsjournal.py` & `roboquant-0.3.0/roboquant/journals/metricsjournal.py`

 * *Files identical despite different names*

### Comparing `roboquant-0.2.9/roboquant/journals/pnlmetric.py` & `roboquant-0.3.0/roboquant/journals/pnlmetric.py`

 * *Files identical despite different names*

### Comparing `roboquant-0.2.9/roboquant/journals/pricemetric.py` & `roboquant-0.3.0/roboquant/journals/pricemetric.py`

 * *Files identical despite different names*

### Comparing `roboquant-0.2.9/roboquant/journals/runmetric.py` & `roboquant-0.3.0/roboquant/journals/runmetric.py`

 * *Files identical despite different names*

### Comparing `roboquant-0.2.9/roboquant/journals/tensorboardjournal.py` & `roboquant-0.3.0/roboquant/journals/tensorboardjournal.py`

 * *Files identical despite different names*

### Comparing `roboquant-0.2.9/roboquant/ml/envs.py` & `roboquant-0.3.0/roboquant/ml/envs.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from decimal import Decimal
 import logging
 import gymnasium as gym
 from gymnasium import spaces
+from gymnasium.envs.registration import register
 import numpy as np
 from numpy.typing import NDArray
 from roboquant.account import Account
 
 from roboquant.brokers.broker import Broker
 from roboquant.brokers.simbroker import SimBroker
 from roboquant.event import Event
@@ -15,30 +16,38 @@
 from roboquant.signal import Signal
 from roboquant.ml.features import Feature
 from roboquant.timeframe import Timeframe
 from roboquant.traders.flextrader import FlexTrader
 from roboquant.traders.trader import Trader
 
 
+register(id="roboquant/StrategyEnv-v0", entry_point="roboquant.ml.envs:StrategyEnv")
+register(id="roboquant/TraderEnv-v0", entry_point="roboquant.ml.envs:TraderEnv")
 logger = logging.getLogger(__name__)
 
 
 class Action2Signals:
+    """Transforms an action into signals"""
 
     def __init__(self, symbols: list[str]):
         self.symbols = symbols
 
+    @staticmethod
+    def __limit(rating):
+        return max(-1.0, min(1.0, float(rating)))
+
     def get_signals(self, action, _):
-        return {symbol: Signal(rating) for symbol, rating in zip(self.symbols, action)}
+        return [Signal(symbol, self.__limit(rating)) for symbol, rating in zip(self.symbols, action)]
 
     def get_action_space(self):
         return spaces.Box(-1.0, 1.0, shape=(len(self.symbols),), dtype=np.float32)
 
 
 class Action2Orders:
+    """Transforms an action into orders"""
 
     def __init__(self, symbols: list[str]):
         self.symbols = symbols
 
     def _account_rebalance(self, account: Account, new_sizes: dict[str, Decimal]) -> list[Order]:
         orders = []
         for symbol, new_size in new_sizes.items():
@@ -46,18 +55,18 @@
             order_size = new_size - old_size
             if order_size != Decimal(0):
                 order = Order(symbol, order_size)
                 orders.append(order)
 
         return orders
 
-    def get_orders(self, action, event: Event, account: Account) -> list[Order]:
+    def get_orders(self, actions, event: Event, account: Account) -> list[Order]:
         new_positions = {}
         equity = account.equity()
-        for symbol, fraction in zip(self.symbols, action):
+        for symbol, fraction in zip(self.symbols, actions):
             price = event.get_price(symbol)
             if price:
                 rel_fraction = fraction / len(self.symbols)
                 contract_value = account.contract_value(symbol, Decimal(1), price)
                 size = equity * rel_fraction / contract_value
                 new_positions[symbol] = Decimal(size).quantize(Decimal(1))
             else:
@@ -133,15 +142,15 @@
 
         self.channel = self.feed.play_background(self.timeframe)
 
         while True:
             self.event = self.channel.get()
             assert self.event is not None, "feed empty during warmup"
             self.account = self.broker.sync(self.event)
-            self.trader.create_orders({}, self.event, self.account)
+            self.trader.create_orders([], self.event, self.account)
             observation = self.get_observation(self.event)
             self.get_reward(self.event, self.account)
             if not np.any(np.isnan(observation)):
                 return observation, {}
 
     def render(self):
         pass
```

### Comparing `roboquant-0.2.9/roboquant/ml/features.py` & `roboquant-0.3.0/roboquant/ml/features.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,16 +6,17 @@
 from numpy.typing import NDArray
 
 from roboquant.account import Account
 from roboquant.event import Event, Bar
 
 
 class Feature(ABC):
-    """Features allows to create features from an event or account object.
-    Many features also allow post transformation after that, like normalization.
+    """Features allows to:
+    - extract features from an event and/or account.
+    - transform other features.
     """
 
     @abstractmethod
     def calc(self, evt: Event, account: Account | None) -> NDArray:
         """
         Return the result as a 1-dimensional NDArray.
         The result should always be the same size.
@@ -90,15 +91,15 @@
         close = ohlcv[3]
 
         prev_close = self.prev_close if self.prev_close is not None else low
         self.prev_close = close
 
         result = max(high - low, abs(high - prev_close), abs(low - prev_close))
 
-        return np.array([result])
+        return np.array([result], dtype=np.float32)
 
     def size(self) -> int:
         return 1
 
     def reset(self):
         self.prev_close = None
 
@@ -206,57 +207,29 @@
         return result
 
     def size(self) -> int:
         return 5 * len(self.symbols)
 
 
 class CombinedFeature(Feature):
-    """Combine multiple features into one single feature"""
+    """Combine multiple features into one single feature by stacking them."""
 
     def __init__(self, *features: Feature) -> None:
         super().__init__()
         self.features = features
         self._size = sum(feature.size() for feature in self.features)
 
     def calc(self, evt, account):
         data = [feature.calc(evt, account) for feature in self.features]
         return np.hstack(data, dtype=np.float32)
 
     def size(self) -> int:
         return self._size
 
 
-class RunningStats:
-
-    def __init__(self, size) -> None:
-        self.existing_aggregate = (0, self._zeros(size), self._zeros(size))
-
-    @staticmethod
-    def _zeros(size):
-        return np.zeros((size,), dtype=np.float32)
-
-    def push(self, new_value):
-        (count, mean, m2) = self.existing_aggregate
-        count += 1
-        delta = new_value - mean
-        mean += delta / count
-        delta2 = new_value - mean
-        m2 += delta * delta2
-        self.existing_aggregate = (count, mean, m2)
-
-    # Retrieve the mean, variance and sample variance from an aggregate
-    def get_normalize_values(self):
-        (count, mean, m2) = self.existing_aggregate
-        if count < 1:
-            raise ValueError("not enough data")
-
-        variance = m2 / count
-        return mean, np.sqrt(variance)
-
-
 class NormalizeFeature(Feature):
     """online normalization calculator"""
 
     def __init__(self, feature: Feature, min_count: int = 3) -> None:
         super().__init__()
         self.feature = feature
         self.min_count = min_count
@@ -295,15 +268,15 @@
         return self.feature.size()
 
     def reset(self):
         self.existing_aggregate = (self._zero_int(), self._zeros(), self._zeros())
 
 
 class FillFeature(Feature):
-    """If a feature returns a nan value, use the last known value instead"""
+    """If a feature contains a nan value, use the last known value instead"""
 
     def __init__(self, feature: Feature) -> None:
         super().__init__()
         self.feature: Feature = feature
         self.fill = self._full_nan()
 
     def calc(self, evt, account):
@@ -444,14 +417,47 @@
         return self.feature.size()
 
     def reset(self):
         self.history.clear()
         self.feature.reset()
 
 
+class MaxReturnFeature2(Feature):
+    """Calculate the maximum return over a certain period.
+    """
+
+    def __init__(self, feature: Feature, period: int) -> None:
+        super().__init__()
+        self.feature: Feature = feature
+        self.history = np.full((period, self.size()), float("nan"), dtype=np.float32)
+        self.idx = -1
+
+    def calc(self, evt, account):
+        self.idx += 1
+        values = self.feature.calc(evt, account)
+        h = self.history
+        h[self.idx] = values
+
+        hist_len = len(h)
+        if self.idx < hist_len:
+            return self._full_nan()
+
+        root_idx = self.idx % hist_len + 1
+        root_idx = root_idx if root_idx < hist_len else 0
+        r = np.max(h) / h[root_idx] - 1.0
+        return r
+
+    def size(self) -> int:
+        return self.feature.size()
+
+    def reset(self):
+        self.idx = -1
+        self.feature.reset()
+
+
 class MinReturnFeature(Feature):
     """Calculate the minimum return over a certain period.
     This will only work on features that return a single value.
     """
 
     def __init__(self, feature: Feature, period: int) -> None:
         super().__init__()
@@ -514,13 +520,13 @@
 
     def __init__(self, tz=timezone.utc) -> None:
         self.tz = tz
 
     def calc(self, evt, account):
         dt = datetime.astimezone(evt.time, self.tz)
         weekday = dt.weekday()
-        result = np.zeros(7)
+        result = np.zeros(7, dtype=np.float32)
         result[weekday] = 1.0
         return result
 
     def size(self) -> int:
         return 7
```

### Comparing `roboquant-0.2.9/roboquant/order.py` & `roboquant-0.3.0/roboquant/order.py`

 * *Files identical despite different names*

### Comparing `roboquant-0.2.9/roboquant/run.py` & `roboquant-0.3.0/roboquant/run.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,46 +6,46 @@
 from roboquant.strategies.strategy import Strategy
 from roboquant.traders.flextrader import FlexTrader
 from roboquant.traders.trader import Trader
 from roboquant.timeframe import Timeframe
 
 
 def run(
-        feed: Feed,
-        strategy: Strategy | None = None,
-        trader: Trader | None = None,
-        broker: Broker | None = None,
-        journal: Journal | None = None,
-        timeframe: Timeframe | None = None,
-        capacity: int = 10,
-        heartbeat_timeout: float | None = None
+    feed: Feed,
+    strategy: Strategy | None = None,
+    trader: Trader | None = None,
+    broker: Broker | None = None,
+    journal: Journal | None = None,
+    timeframe: Timeframe | None = None,
+    capacity: int = 10,
+    heartbeat_timeout: float | None = None,
 ) -> Account:
     """Start a new run.
 
     Args:
         feed: The feed to use for this run
         strategy: Your strategy that you want to use. Default is None, meaning no signals will be created.
         trader: The trader you want to use. If None is specified, the `FlexTrader` will be used with its default settings
         broker: The broker you want to use. If None is specified, the `SimBroker` will be used with its default settings
         journal: Journal to use to log and/or store progress and metrics, default is None.
         timeframe: Optionally limit the run to events within this timeframe. The default is None
-        capacity: The max capacity of the event channel. Default is 10 events.
-        heartbeat_timeout: Optionally, a heartbeat will be generated if no other events are received within the specified
-            timeout in seconds. The default is None.
+        capacity: The max capacity of the used event channel. Default is 10 events.
+        heartbeat_timeout: Optionally, a heartbeat (is an empty event) will be generated if no other events are received
+        within the specified timeout in seconds. The default is None.
 
     Returns:
         The latest version of the account
     """
 
     trader = trader or FlexTrader()
     broker = broker or SimBroker()
     channel = feed.play_background(timeframe, capacity)
 
     while event := channel.get(heartbeat_timeout):
         account = broker.sync(event)
-        signals = strategy.create_signals(event) if strategy else {}
+        signals = strategy.create_signals(event) if strategy else []
         orders = trader.create_orders(signals, event, account)
         broker.place_orders(orders)
         if journal:
             journal.track(event, account, signals, orders)
 
     return broker.sync()
```

### Comparing `roboquant-0.2.9/roboquant/signal.py` & `roboquant-0.3.0/roboquant/signal.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,47 +1,49 @@
 from dataclasses import dataclass
 from enum import Flag, auto
 
 
 class SignalType(Flag):
-    """Type of signal, either ENTRY, EXIT or BOTH"""
+    """Type of signal, either ENTRY, EXIT or ENTRY_EXIT"""
 
     ENTRY = auto()
     EXIT = auto()
-    BOTH = ENTRY | EXIT
+    ENTRY_EXIT = ENTRY | EXIT
 
-    def __repr__(self):
+    def __str__(self):
         return self.name
 
 
 @dataclass(slots=True, frozen=True)
 class Signal:
-    """Signal that a strategy can create.
-    It contains both a rating between -1.0 and 1.0 and the type of signal.
+    """Signal that a strategy can create.It contains both a rating and the type of signal.
+
+    A rating is a float normally between -1.0 and 1.0, where -1.0 is a strong sell and 1.0 is a strong buy.
+    But in cases it can exceed these values. It is up to the used trader to handle these values
 
     Examples:
     ```
     Signal.buy("XYZ")
     Signal.sell("XYZ", SignalType.EXIT)
     Signal("XYZ", 0.5, SignalType.ENTRY)
     ```
     """
-
+    symbol: str
     rating: float
-    type: SignalType = SignalType.BOTH
+    type: SignalType = SignalType.ENTRY_EXIT
 
     @staticmethod
-    def buy(signal_type=SignalType.BOTH):
+    def buy(symbol, signal_type=SignalType.ENTRY_EXIT):
         """Create a BUY signal with a rating of 1.0"""
-        return Signal(1.0, signal_type)
+        return Signal(symbol, 1.0, signal_type)
 
     @staticmethod
-    def sell(signal_type=SignalType.BOTH):
+    def sell(symbol, signal_type=SignalType.ENTRY_EXIT):
         """Create a SELL signal with a rating of -1.0"""
-        return Signal(-1.0, signal_type)
+        return Signal(symbol, -1.0, signal_type)
 
     @property
     def is_buy(self):
         return self.rating > 0.0
 
     @property
     def is_sell(self):
@@ -50,14 +52,7 @@
     @property
     def is_entry(self):
         return SignalType.ENTRY in self.type
 
     @property
     def is_exit(self):
         return SignalType.EXIT in self.type
-
-
-BUY = Signal.buy(SignalType.BOTH)
-"""BUY signal with a rating of 1.0 and valid for both entry and exit signals"""
-
-SELL = Signal.sell(SignalType.BOTH)
-"""SELL signal with a rating of -1.0 and valid for both entry and exit signals"""
```

### Comparing `roboquant-0.2.9/roboquant/strategies/barstrategy.py` & `roboquant-0.3.0/roboquant/strategies/barstrategy.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,27 +15,27 @@
     """
 
     def __init__(self, size: int) -> None:
         super().__init__()
         self._data: dict[str, OHLCVBuffer] = {}
         self.size = size
 
-    def create_signals(self, event) -> dict[str, Signal]:
-        signals = {}
+    def create_signals(self, event):
+        signals = []
         for item in event.items:
             if isinstance(item, Bar):
                 symbol = item.symbol
                 if symbol not in self._data:
                     self._data[symbol] = OHLCVBuffer(self.size)
                 ohlcv = self._data[symbol]
                 ohlcv.append(item.ohlcv)
                 if ohlcv.is_full():
                     signal = self._create_signal(symbol, ohlcv)
                     if signal is not None:
-                        signals[symbol] = signal
+                        signals.append(signal)
         return signals
 
     @abstractmethod
     def _create_signal(self, symbol: str, ohlcv: OHLCVBuffer) -> Signal | None:
         """
         Return a signal or None for the provided symbol and ohlcv data.
         """
```

### Comparing `roboquant-0.2.9/roboquant/strategies/buffer.py` & `roboquant-0.3.0/roboquant/strategies/buffer.py`

 * *Files identical despite different names*

### Comparing `roboquant-0.2.9/roboquant/strategies/smacrossover.py` & `roboquant-0.3.0/roboquant/strategies/smacrossover.py`

 * *Files 20% similar despite different names*

```diff
@@ -21,28 +21,28 @@
 
         # SMA(MIN) > SMA(MAX)
         new_rating: bool = prices[-self.min_period:].mean() > prices[-self.max_period:].mean()
         result = None
         if symbol in self._prev_ratings:
             prev_rating = self._prev_ratings[symbol]
             if prev_rating != new_rating:
-                result = Signal.buy() if new_rating else Signal.sell()
+                result = Signal.buy(symbol) if new_rating else Signal.sell(symbol)
 
         self._prev_ratings[symbol] = new_rating
         return result
 
     def create_signals(self, event):
-        signals: dict[str, Signal] = {}
+        signals = []
         for (symbol, item) in event.price_items.items():
             h = self._history.get(symbol)
 
             if h is None:
                 maxlen = max(self.max_period, self.min_period)
                 h = collections.deque(maxlen=maxlen)
                 self._history[symbol] = h
 
             h.append(item.price())
             if len(h) == h.maxlen:
                 if signal := self.__get_signal(symbol):
-                    signals[symbol] = signal
+                    signals.append(signal)
 
         return signals
```

### Comparing `roboquant-0.2.9/roboquant/strategies/strategy.py` & `roboquant-0.3.0/roboquant/strategies/strategy.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 class Strategy(ABC):
     """A strategy creates signals based on incoming events and the items these events contain.
 
     Often these items represent market data, but other types of items are also possible.
     """
 
     @abstractmethod
-    def create_signals(self, event: Event) -> dict[str, Signal]:
+    def create_signals(self, event: Event) -> list[Signal]:
         """Create a signal for zero or more symbols. Signals are returned as a dictionary with key being the symbol and
         the value being the Signal.
         """
         ...
 
     def reset(self):
         """Reset the state of the strategy"""
```

### Comparing `roboquant-0.2.9/roboquant/timeframe.py` & `roboquant-0.3.0/roboquant/timeframe.py`

 * *Files 24% similar despite different names*

```diff
@@ -33,43 +33,33 @@
         return cls(s, e, inclusive)
 
     @staticmethod
     def empty():
         return Timeframe.fromisoformat("1900-01-01T00:00:00+00:00", "1900-01-01T00:00:00+00:00", False)
 
     @staticmethod
-    def previous(days=0, seconds=0, microseconds=0, milliseconds=0, minutes=0, hours=0, weeks=0, inclusive=False):
-        """Convenient method to create a historic timeframe"""
+    def previous(inclusive=False, **kwargs):
+        """Convenient method to create a historic timeframe, the kwargs arguments will be passed to the timedelta
 
-        td = timedelta(
-            days=days,
-            seconds=seconds,
-            microseconds=microseconds,
-            milliseconds=milliseconds,
-            minutes=minutes,
-            hours=hours,
-            weeks=weeks,
-        )
+        timeframe = Timeframe.previous(days=365)
+        """
+
+        td = timedelta(**kwargs)
         end = datetime.now(timezone.utc)
         start = end - td
         return Timeframe(start, end, inclusive)
 
     @staticmethod
-    def next(days=0, seconds=0, microseconds=0, milliseconds=0, minutes=0, hours=0, weeks=0, inclusive=False):
-        """Convenient method to create a future timeframe"""
+    def next(inclusive=False, **kwargs):
+        """Convenient method to create a future timeframe, the kwargs arguments will be passed to the timedelta
+
+        timeframe = Timeframe.next(minutes=30)
+        """
 
-        td = timedelta(
-            days=days,
-            seconds=seconds,
-            microseconds=microseconds,
-            milliseconds=milliseconds,
-            minutes=minutes,
-            hours=hours,
-            weeks=weeks,
-        )
+        td = timedelta(**kwargs)
         start = datetime.now(timezone.utc)
         end = start + td
         return Timeframe(start, end, inclusive)
 
     def __contains__(self, time):
         if self.inclusive:
             return self.start <= time <= self.end
@@ -93,15 +83,15 @@
             return float("NaN")
 
         years = timedelta(days=365) / self.duration
         return (1.0 + rate) ** years - 1.0
 
     def split(self, n: int | timedelta | Any) -> list["Timeframe"]:
         """Split the timeframe in sequential parts and return the resulting list of timeframes.
-        The parameter `n` can be a number or a timedelta instance or other types like relativedelta that support
+        The parameter `n` can be a number, a timedelta instance or other types like relativedelta that support
         datetime calculations.
         """
 
         period = self.duration / n if isinstance(n, int) else n
         end = self.start
         result = []
         while end < self.end:
```

### Comparing `roboquant-0.2.9/roboquant/traders/flextrader.py` & `roboquant-0.3.0/roboquant/traders/flextrader.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,138 +1,178 @@
 from datetime import datetime, timedelta
 import logging
 from decimal import Decimal
-from enum import Enum
+from enum import Flag, auto
+import random
 
 from roboquant.event import Event
 from roboquant.order import Order
 from roboquant.signal import Signal
 from .trader import Trader
 from ..account import Account
 from ..event import PriceItem
 
 logger = logging.getLogger(__name__)
 
 
-class _PositionChange(Enum):
-    OPEN_LONG = 1
-    OPEN_SHORT = 2
-    CLOSE = 3
-    INCREASE = 4
+class _PositionChange(Flag):
+    ENTRY_LONG = auto()
+    ENTRY_SHORT = auto()
+    EXIT_LONG = auto()
+    EXIT_SHORT = auto()
+
+    _ENTRY = ENTRY_LONG | ENTRY_SHORT
+    _EXIT = EXIT_LONG | EXIT_SHORT
+
+    @property
+    def is_entry(self):
+        """Return True is the status is open, False otherwise"""
+        return self in _PositionChange._ENTRY
+
+    @property
+    def is_exit(self):
+        """Return True is the status is closed, False otherwise"""
+        return self in _PositionChange._EXIT
 
     @staticmethod
-    def get_change(rating: float, pos_size: Decimal) -> "_PositionChange":
-        """Determine the kind of change a certain rating has on the position"""
+    def get_change(is_buy: bool, pos_size: Decimal) -> "_PositionChange":
+        """Determine the kind of change a certain action would have on the position"""
         if pos_size.is_zero():
-            return _PositionChange.OPEN_LONG if rating > 0.0 else _PositionChange.OPEN_SHORT
-        return _PositionChange.CLOSE if float(pos_size) * rating < 0.0 else _PositionChange.INCREASE
+            return _PositionChange.ENTRY_LONG if is_buy else _PositionChange.ENTRY_SHORT
+        if pos_size > 0:
+            return _PositionChange.ENTRY_LONG if is_buy else _PositionChange.EXIT_LONG
+
+        return _PositionChange.EXIT_SHORT if is_buy else _PositionChange.ENTRY_SHORT
 
 
 def _log_rule(rule: str, signal: Signal, symbol: str, position: Decimal):
     if logger.isEnabledFor(logging.INFO):
-        logger.info("signal=%s symbol=%s position=%s discarded because of %s", signal, symbol, position, rule)
+        logger.info(
+            "rating=%s type=%s symbol=%s position=%s discarded because of %s",
+            signal.rating,
+            signal.type,
+            symbol,
+            position,
+            rule,
+        )
 
 
 class FlexTrader(Trader):
     """Implementation of a Trader that has configurable rules to modify which signals are converted into orders.
     This implementation will not generate orders if there is not a price in the event for the underlying symbol.
 
     The configurable parameters include:
 
     - one_order_only: don't create new orders for a symbol if there is already an open orders for that same symbol
     - size_fractions: enable fractional order sizes (if size_fractions is larger than 0), default is 0
-    - min_buying_power: the minimal buying power that should remain available (to avoid margin calls), default is 0.0
-    - increase_position: allow an order to potentially increase an open position size, default is False
+    - safety_margin_perc: the safety margin as percentage of equity that should remain available (to avoid margin calls),
+    default is 0.05 (5%)
+    - max_position_perc: the max percentage of the equity to allocate to a single position, default is 0.1 (10%)
     - max_order_perc: the max percentage of the equity to allocate to a new order, default is 0.05 (5%)
     - min_order_perc: the min percentage of the equity to allocate to a new order, default is 0.02 (2%)
     - shorting: allow orders that could result in a short position, default is false
-    - price_type: the price type to use when determining order value
+    - price_type: the price type to use when determining order value, for example "CLOSE". Default is "DEFAULT"
 
     It might be sometimes challenging to understand wby a signal isn't converted into an order. The flex-trader logs
     at INFO level when certain rules have been fired.
 
+    import logging
+    logging.basicConfig(level=logging.WARNING)
+    logging.getLogger("roboquant.traders.flextrader").setLevel(logging.INFO)
     """
 
     def __init__(
         self,
         one_order_only=True,
         size_fractions=0,
-        min_buying_power_perc=0.05,
-        increase_position=False,
+        safety_margin_perc=0.05,
         shorting=False,
         max_order_perc=0.05,
         min_order_perc=0.02,
+        max_position_perc=0.1,
         price_type="DEFAULT",
+        shuffle_signals=False,
     ) -> None:
         super().__init__()
         self.one_order_only = one_order_only
         self.size_digits: int = size_fractions
-        self.min_buying_power_perc: float = min_buying_power_perc
-        self.increase_position = increase_position
+        self.safety_margin_perc: float = safety_margin_perc
         self.shorting = shorting
         self.max_order_perc = max_order_perc
         self.min_order_perc = min_order_perc
+        self.max_position_perc = max_position_perc
         self.price_type = price_type
+        self.shuffle_signals = shuffle_signals
 
     def _get_order_size(self, rating: float, contract_price: float, max_order_value: float) -> Decimal:
         """Return the order size"""
         size = Decimal(rating * max_order_value / contract_price)
         rounded_size = round(size, self.size_digits)
         return rounded_size
 
-    def create_orders(self, signals: dict[str, Signal], event: Event, account: Account) -> list[Order]:
-        # pylint: disable=too-many-branches,too-many-statements
+    def create_orders(self, signals: list[Signal], event: Event, account: Account) -> list[Order]:
+        # pylint: disable=too-many-branches,too-many-statements,too-many-locals
         if not signals:
             return []
 
+        if self.shuffle_signals:
+            random.shuffle(signals)
+
         orders: list[Order] = []
         equity = account.equity()
         max_order_value = equity * self.max_order_perc
         min_order_value = equity * self.min_order_perc
-        available = account.buying_power - self.min_buying_power_perc * equity
+        max_pos_value = equity * self.max_position_perc
+        available = account.buying_power - self.safety_margin_perc * equity
 
-        for symbol, signal in signals.items():
+        for signal in signals:
+            symbol = signal.symbol
             pos_size = account.get_position_size(symbol)
 
             if self.one_order_only and account.has_open_order(symbol):
                 _log_rule("one order only", signal, symbol, pos_size)
                 continue
 
             item = event.price_items.get(symbol)
             if item is None:
                 _log_rule("no price is available", signal, symbol, pos_size)
                 continue
 
             price = item.price(self.price_type)
-            change = _PositionChange.get_change(signal.rating, pos_size)
+            change = _PositionChange.get_change(signal.is_buy, pos_size)
 
-            if not self.shorting and change == _PositionChange.OPEN_SHORT:
+            if not self.shorting and change == _PositionChange.ENTRY_SHORT:
                 _log_rule("no shorting", signal, symbol, pos_size)
                 continue
-            if not self.increase_position and change == _PositionChange.INCREASE:
-                _log_rule("no increase position sizing", signal, symbol, pos_size)
-                continue
 
-            if change == _PositionChange.CLOSE:
+            if change.is_exit:
                 # Closing orders don't require or use buying power
                 if not signal.is_exit:
                     _log_rule("no exit signal", signal, symbol, pos_size)
                     continue
-                new_orders = self._get_orders(symbol, pos_size * -1, item, signal.rating, event.time)
+                rounded_size = round(pos_size * Decimal(signal.rating), self.size_digits)
+                if rounded_size.is_zero():
+                    _log_rule("cannot exit with order size zero", signal, symbol, pos_size)
+                    continue
+                new_orders = self._get_orders(symbol, rounded_size, item, signal, event.time)
                 orders += new_orders
             else:
                 if not signal.is_entry:
                     _log_rule("no entry signal", signal, symbol, pos_size)
                     continue
 
                 if available < min_order_value:
                     _log_rule("available buying power below minimum order value", signal, symbol, pos_size)
                     continue
 
-                available_order_value = min(available, max_order_value)
+                available_order_value = min(available, max_order_value, max_pos_value - abs(account.position_value(symbol)))
+                if available_order_value < min_order_value:
+                    _log_rule("calculated available order value below minimum order value", signal, symbol, pos_size)
+                    continue
+
                 contract_price = account.contract_value(symbol, Decimal(1), price)
                 order_size = self._get_order_size(signal.rating, contract_price, available_order_value)
 
                 if order_size.is_zero():
                     _log_rule("calculated order size is zero", signal, symbol, pos_size)
                     continue
 
@@ -140,22 +180,22 @@
                 if order_value > available:
                     _log_rule("order value above available buying power", signal, symbol, pos_size)
                     continue
                 if order_value < min_order_value:
                     _log_rule("order value below minimum order value", signal, symbol, pos_size)
                     continue
 
-                new_orders = self._get_orders(symbol, order_size, item, signal.rating, event.time)
+                new_orders = self._get_orders(symbol, order_size, item, signal, event.time)
                 if new_orders:
                     orders += new_orders
                     available -= order_value
 
         return orders
 
-    def _get_orders(self, symbol: str, size: Decimal, item: PriceItem, rating: float, time: datetime) -> list[Order]:
+    def _get_orders(self, symbol: str, size: Decimal, item: PriceItem, signal: Signal, time: datetime) -> list[Order]:
         # pylint: disable=unused-argument
         """Return zero or more orders for the provided symbol and size.
 
         Default is a MarketOrder. Overwrite this method to create different order types.
         """
 
         return [Order(symbol, size)]
@@ -168,33 +208,35 @@
 class FlexLimitOrderTrader(FlexTrader):
     """A FlexTrader version that returns a limit order"""
 
     def __init__(
         self,
         one_order_only=True,
         size_fractions=0,
-        min_buying_power_perc=0.05,
-        increase_position=False,
+        safety_margin_perc=0.05,
         shorting=False,
         max_order_perc=0.05,
         min_order_perc=0.02,
+        max_position_perc=0.05,
         price_type="DEFAULT",
-        gtd=timedelta(days=3)
+        shuffle_signals=False,
+        gtd=timedelta(days=3),
     ) -> None:
         super().__init__(
             one_order_only,
             size_fractions,
-            min_buying_power_perc,
-            increase_position,
+            safety_margin_perc,
             shorting,
             max_order_perc,
             min_order_perc,
+            max_position_perc,
             price_type,
+            shuffle_signals,
         )
         self.gtd_timedelta = gtd
 
-    def _get_orders(self, symbol: str, size: Decimal, item: PriceItem, rating: float, time: datetime) -> list[Order]:
+    def _get_orders(self, symbol: str, size: Decimal, item: PriceItem, signal: Signal, time: datetime) -> list[Order]:
         # pylint: disable=unused-argument
         """Return a single limit-order with the limit the current price a GTD with a configurable 3 days from now."""
         gtd = time + self.gtd_timedelta
         limit = item.price(self.price_type)
         return [Order(symbol, size, limit, gtd)]
```

### Comparing `roboquant-0.2.9/roboquant/traders/sizing.py` & `roboquant-0.3.0/roboquant/traders/sizing.py`

 * *Files identical despite different names*

### Comparing `roboquant-0.2.9/roboquant/traders/trader.py` & `roboquant-0.3.0/roboquant/traders/trader.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     """A trader creates the orders, typically based on the signals it receives from a strategy.
 
     But it is also possible to implement all logic in a Trader and don't rely on signals at all.
     In contrast to a `Strategy`, a `Trader` can also access the `Account` object.
     """
 
     @abstractmethod
-    def create_orders(self, signals: dict[str, Signal], event: Event, account: Account) -> list[Order]:
+    def create_orders(self, signals: list[Signal], event: Event, account: Account) -> list[Order]:
         """Create zero or more orders.
 
         Arguments
             signals: Zero or more signals created by the strategy.
             event: The event with its items.
             account: The latest account object.
```

### Comparing `roboquant-0.2.9/roboquant.egg-info/PKG-INFO` & `roboquant-0.3.0/roboquant.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roboquant
-Version: 0.2.9
+Version: 0.3.0
 Summary: A fast algo-trading platform
 Author-email: roboquant team <info@roboquant.org>
 Project-URL: Homepage, https://roboquant.org
 Project-URL: Repository, https://github.com/neurallayer/roboquant.py.git
 Project-URL: Issues, https://github.com/neurallayer/roboquant.py/issues
 Keywords: trading,investment,finance,crypto,stocks,exchange,forex
 Classifier: Development Status :: 3 - Alpha
@@ -63,15 +63,15 @@
 strategy = rq.strategies.EMACrossover()
 account = rq.run(feed, strategy)
 print(account)
 ```
 
 ## Install
 Roboquant can be installed like most other Python packages, using pip or conda.
-Make sure you have Python version 3.10 or higher installed.
+Make sure you have Python version 3.11 or higher installed.
 
 ```shell
 python3 -m pip install --upgrade roboquant
 ```
 
 You can also try roboquant in an online Jupyter Notebook [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/neurallayer/roboquant-notebooks/HEAD?labpath=%2Fintro_roboquant.ipynb)
```

### Comparing `roboquant-0.2.9/roboquant.egg-info/SOURCES.txt` & `roboquant-0.3.0/roboquant.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 roboquant/timeframe.py
 roboquant.egg-info/PKG-INFO
 roboquant.egg-info/SOURCES.txt
 roboquant.egg-info/dependency_links.txt
 roboquant.egg-info/requires.txt
 roboquant.egg-info/top_level.txt
 roboquant/brokers/__init__.py
+roboquant/brokers/alpacabroker.py
 roboquant/brokers/broker.py
 roboquant/brokers/ibkr.py
 roboquant/brokers/simbroker.py
 roboquant/feeds/__init__.py
 roboquant/feeds/aggregate.py
 roboquant/feeds/alpacafeed.py
 roboquant/feeds/csvfeed.py
@@ -43,15 +44,14 @@
 roboquant/journals/pricemetric.py
 roboquant/journals/runmetric.py
 roboquant/journals/tensorboardjournal.py
 roboquant/ml/__init__.py
 roboquant/ml/envs.py
 roboquant/ml/features.py
 roboquant/ml/strategies.py
-roboquant/ml/torch.py
 roboquant/strategies/__init__.py
 roboquant/strategies/barstrategy.py
 roboquant/strategies/buffer.py
 roboquant/strategies/emacrossover.py
 roboquant/strategies/multistrategy.py
 roboquant/strategies/smacrossover.py
 roboquant/strategies/strategy.py
```

