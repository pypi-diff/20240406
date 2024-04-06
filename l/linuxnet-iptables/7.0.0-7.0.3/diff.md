# Comparing `tmp/linuxnet-iptables-7.0.0.tar.gz` & `tmp/linuxnet-iptables-7.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linuxnet-iptables-7.0.0.tar", last modified: Thu Mar 21 15:09:12 2024, max compression
+gzip compressed data, was "linuxnet-iptables-7.0.3.tar", last modified: Sat Apr  6 21:45:02 2024, max compression
```

## Comparing `linuxnet-iptables-7.0.0.tar` & `linuxnet-iptables-7.0.3.tar`

### file list

```diff
@@ -1,113 +1,113 @@
-drwxr-sr-x   0 panos     (1001) users      (100)        0 2024-03-21 15:09:12.303460 linuxnet-iptables-7.0.0/
--rw-r--r--   0 panos     (1001) users      (100)    18810 2023-01-01 01:13:07.000000 linuxnet-iptables-7.0.0/.pylintrc
--rw-r--r--   0 panos     (1001) users      (100)     5085 2024-03-21 14:52:18.000000 linuxnet-iptables-7.0.0/CHANGELOG.md
--rw-r--r--   0 panos     (1001) users      (100)    32387 2023-01-01 01:13:10.000000 linuxnet-iptables-7.0.0/LICENSE
--rw-r--r--   0 panos     (1001) users      (100)      284 2023-02-06 17:07:04.000000 linuxnet-iptables-7.0.0/MANIFEST.in
--rw-r--r--   0 panos     (1001) users      (100)     5164 2023-01-01 01:13:07.000000 linuxnet-iptables-7.0.0/Makefile
--rw-r--r--   0 panos     (1001) users      (100)     4108 2024-03-21 15:09:12.302459 linuxnet-iptables-7.0.0/PKG-INFO
--rw-r--r--   0 panos     (1001) users      (100)     3213 2023-07-14 00:05:40.000000 linuxnet-iptables-7.0.0/README.md
-drwxr-sr-x   0 panos     (1001) users      (100)        0 2024-03-21 15:09:12.290459 linuxnet-iptables-7.0.0/docs/
--rw-r--r--   0 panos     (1001) users      (100)      905 2023-01-01 01:13:06.000000 linuxnet-iptables-7.0.0/docs/Makefile
--rw-r--r--   0 panos     (1001) users      (100)     1491 2023-03-01 20:08:53.000000 linuxnet-iptables-7.0.0/docs/chain.rst
--rw-r--r--   0 panos     (1001) users      (100)     2850 2023-01-27 18:52:21.000000 linuxnet-iptables-7.0.0/docs/conf.py
--rw-r--r--   0 panos     (1001) users      (100)     1061 2023-02-06 17:07:04.000000 linuxnet-iptables-7.0.0/docs/exception.rst
--rw-r--r--   0 panos     (1001) users      (100)     8253 2024-03-21 03:17:27.000000 linuxnet-iptables-7.0.0/docs/extensibility.rst
--rw-r--r--   0 panos     (1001) users      (100)     3335 2024-03-21 03:19:46.000000 linuxnet-iptables-7.0.0/docs/index.rst
--rw-r--r--   0 panos     (1001) users      (100)     3543 2024-03-21 03:17:27.000000 linuxnet-iptables-7.0.0/docs/iptables_api.rst
--rw-r--r--   0 panos     (1001) users      (100)     3047 2023-07-09 21:05:25.000000 linuxnet-iptables-7.0.0/docs/match-example.py
--rw-r--r--   0 panos     (1001) users      (100)     2258 2023-02-08 00:19:00.000000 linuxnet-iptables-7.0.0/docs/match.rst
-drwxr-sr-x   0 panos     (1001) users      (100)        0 2024-03-21 15:09:12.293459 linuxnet-iptables-7.0.0/docs/matches/
--rw-r--r--   0 panos     (1001) users      (100)     1335 2023-06-19 04:02:28.000000 linuxnet-iptables-7.0.0/docs/matches/addrtypematch.rst
--rw-r--r--   0 panos     (1001) users      (100)     1431 2023-02-06 17:07:04.000000 linuxnet-iptables-7.0.0/docs/matches/commentmatch.rst
--rw-r--r--   0 panos     (1001) users      (100)     1268 2023-07-14 00:05:40.000000 linuxnet-iptables-7.0.0/docs/matches/connmarkmatch.rst
--rw-r--r--   0 panos     (1001) users      (100)     3253 2023-09-09 02:06:12.000000 linuxnet-iptables-7.0.0/docs/matches/conntrackmatch.rst
--rw-r--r--   0 panos     (1001) users      (100)     1899 2023-02-06 17:07:04.000000 linuxnet-iptables-7.0.0/docs/matches/icmpmatch.rst
--rw-r--r--   0 panos     (1001) users      (100)     1861 2023-02-20 17:08:37.000000 linuxnet-iptables-7.0.0/docs/matches/limitmatch.rst
--rw-r--r--   0 panos     (1001) users      (100)     1430 2023-10-21 19:41:05.000000 linuxnet-iptables-7.0.0/docs/matches/macmatch.rst
--rw-r--r--   0 panos     (1001) users      (100)     1438 2023-07-14 00:05:40.000000 linuxnet-iptables-7.0.0/docs/matches/markmatch.rst
--rw-r--r--   0 panos     (1001) users      (100)     1539 2024-01-19 19:36:42.000000 linuxnet-iptables-7.0.0/docs/matches/multiportmatch.rst
--rw-r--r--   0 panos     (1001) users      (100)     2131 2023-09-09 02:06:12.000000 linuxnet-iptables-7.0.0/docs/matches/ownermatch.rst
--rw-r--r--   0 panos     (1001) users      (100)     2447 2023-02-08 00:19:00.000000 linuxnet-iptables-7.0.0/docs/matches/packetmatch.rst
--rw-r--r--   0 panos     (1001) users      (100)     1511 2023-02-06 17:07:04.000000 linuxnet-iptables-7.0.0/docs/matches/packettypematch.rst
--rw-r--r--   0 panos     (1001) users      (100)     2248 2023-07-14 00:05:40.000000 linuxnet-iptables-7.0.0/docs/matches/recentmatch.rst
--rw-r--r--   0 panos     (1001) users      (100)     1736 2023-09-09 02:06:12.000000 linuxnet-iptables-7.0.0/docs/matches/setmatch.rst
--rw-r--r--   0 panos     (1001) users      (100)     1312 2023-02-06 17:07:04.000000 linuxnet-iptables-7.0.0/docs/matches/statematch.rst
--rw-r--r--   0 panos     (1001) users      (100)     1251 2023-09-09 02:06:12.000000 linuxnet-iptables-7.0.0/docs/matches/statisticmatch.rst
--rw-r--r--   0 panos     (1001) users      (100)     2302 2023-07-14 00:05:40.000000 linuxnet-iptables-7.0.0/docs/matches/tcpmatch.rst
--rw-r--r--   0 panos     (1001) users      (100)     1382 2023-02-06 17:07:04.000000 linuxnet-iptables-7.0.0/docs/matches/tcpmssmatch.rst
--rw-r--r--   0 panos     (1001) users      (100)     1528 2023-09-09 02:06:12.000000 linuxnet-iptables-7.0.0/docs/matches/ttlmatch.rst
--rw-r--r--   0 panos     (1001) users      (100)     1280 2023-02-06 17:07:04.000000 linuxnet-iptables-7.0.0/docs/matches/udpmatch.rst
--rw-r--r--   0 panos     (1001) users      (100)      873 2023-03-01 20:08:53.000000 linuxnet-iptables-7.0.0/docs/rule.rst
--rw-r--r--   0 panos     (1001) users      (100)      903 2023-02-05 23:48:29.000000 linuxnet-iptables-7.0.0/docs/table.rst
--rw-r--r--   0 panos     (1001) users      (100)     1184 2024-03-21 03:17:27.000000 linuxnet-iptables-7.0.0/docs/target-example.py
--rw-r--r--   0 panos     (1001) users      (100)     1201 2023-02-08 00:19:00.000000 linuxnet-iptables-7.0.0/docs/target.rst
-drwxr-sr-x   0 panos     (1001) users      (100)        0 2024-03-21 15:09:12.295459 linuxnet-iptables-7.0.0/docs/targets/
--rw-r--r--   0 panos     (1001) users      (100)      903 2023-02-06 17:07:04.000000 linuxnet-iptables-7.0.0/docs/targets/chaintarget.rst
--rw-r--r--   0 panos     (1001) users      (100)      912 2023-02-06 17:07:04.000000 linuxnet-iptables-7.0.0/docs/targets/connmarktarget.rst
--rw-r--r--   0 panos     (1001) users      (100)      900 2023-02-06 17:07:04.000000 linuxnet-iptables-7.0.0/docs/targets/dnattarget.rst
--rw-r--r--   0 panos     (1001) users      (100)      897 2023-02-06 17:07:04.000000 linuxnet-iptables-7.0.0/docs/targets/logtarget.rst
--rw-r--r--   0 panos     (1001) users      (100)      900 2023-02-06 17:07:04.000000 linuxnet-iptables-7.0.0/docs/targets/marktarget.rst
--rw-r--r--   0 panos     (1001) users      (100)      912 2023-02-06 17:07:04.000000 linuxnet-iptables-7.0.0/docs/targets/masqueradetarget.rst
--rw-r--r--   0 panos     (1001) users      (100)      902 2023-06-04 01:25:41.000000 linuxnet-iptables-7.0.0/docs/targets/notracktarget.rst
--rw-r--r--   0 panos     (1001) users      (100)      906 2023-02-06 17:07:04.000000 linuxnet-iptables-7.0.0/docs/targets/rejecttarget.rst
--rw-r--r--   0 panos     (1001) users      (100)      900 2023-02-06 17:07:04.000000 linuxnet-iptables-7.0.0/docs/targets/snattarget.rst
--rw-r--r--   0 panos     (1001) users      (100)      896 2023-06-04 01:25:41.000000 linuxnet-iptables-7.0.0/docs/targets/tracetarget.rst
--rw-r--r--   0 panos     (1001) users      (100)      897 2023-02-06 17:07:04.000000 linuxnet-iptables-7.0.0/docs/targets/ttltarget.rst
-drwxr-sr-x   0 panos     (1001) users      (100)        0 2024-03-21 15:09:12.295459 linuxnet-iptables-7.0.0/linuxnet/
--rw-r--r--   0 panos     (1001) users      (100)        0 2023-01-01 01:13:07.000000 linuxnet-iptables-7.0.0/linuxnet/__init__.py
-drwxr-sr-x   0 panos     (1001) users      (100)        0 2024-03-21 15:09:12.296459 linuxnet-iptables-7.0.0/linuxnet/iptables/
--rw-r--r--   0 panos     (1001) users      (100)     1170 2023-03-01 20:08:53.000000 linuxnet-iptables-7.0.0/linuxnet/iptables/__init__.py
--rw-r--r--   0 panos     (1001) users      (100)    29055 2023-07-24 18:13:22.000000 linuxnet-iptables-7.0.0/linuxnet/iptables/chain.py
--rw-r--r--   0 panos     (1001) users      (100)      854 2023-02-20 17:08:37.000000 linuxnet-iptables-7.0.0/linuxnet/iptables/deps.py
--rw-r--r--   0 panos     (1001) users      (100)     2564 2024-03-21 03:17:24.000000 linuxnet-iptables-7.0.0/linuxnet/iptables/exceptions.py
--rw-r--r--   0 panos     (1001) users      (100)     1467 2023-07-14 00:05:40.000000 linuxnet-iptables-7.0.0/linuxnet/iptables/extension.py
-drwxr-sr-x   0 panos     (1001) users      (100)        0 2024-03-21 15:09:12.299459 linuxnet-iptables-7.0.0/linuxnet/iptables/matches/
--rw-r--r--   0 panos     (1001) users      (100)     1524 2024-01-19 19:36:42.000000 linuxnet-iptables-7.0.0/linuxnet/iptables/matches/__init__.py
--rw-r--r--   0 panos     (1001) users      (100)     4978 2023-07-09 21:05:25.000000 linuxnet-iptables-7.0.0/linuxnet/iptables/matches/addrtypematch.py
--rw-r--r--   0 panos     (1001) users      (100)     2879 2023-07-09 21:05:25.000000 linuxnet-iptables-7.0.0/linuxnet/iptables/matches/commentmatch.py
--rw-r--r--   0 panos     (1001) users      (100)     2285 2023-07-09 21:05:25.000000 linuxnet-iptables-7.0.0/linuxnet/iptables/matches/connmarkmatch.py
--rw-r--r--   0 panos     (1001) users      (100)    17982 2024-03-21 03:17:25.000000 linuxnet-iptables-7.0.0/linuxnet/iptables/matches/conntrackmatch.py
--rw-r--r--   0 panos     (1001) users      (100)     9761 2023-07-09 21:05:25.000000 linuxnet-iptables-7.0.0/linuxnet/iptables/matches/icmpmatch.py
--rw-r--r--   0 panos     (1001) users      (100)     4559 2023-07-09 21:05:25.000000 linuxnet-iptables-7.0.0/linuxnet/iptables/matches/limitmatch.py
--rw-r--r--   0 panos     (1001) users      (100)     2458 2023-10-21 19:41:05.000000 linuxnet-iptables-7.0.0/linuxnet/iptables/matches/macmatch.py
--rw-r--r--   0 panos     (1001) users      (100)     3872 2023-07-09 21:05:25.000000 linuxnet-iptables-7.0.0/linuxnet/iptables/matches/markmatch.py
--rw-r--r--   0 panos     (1001) users      (100)    16971 2024-03-21 03:17:25.000000 linuxnet-iptables-7.0.0/linuxnet/iptables/matches/match.py
--rw-r--r--   0 panos     (1001) users      (100)     6094 2024-01-19 19:59:34.000000 linuxnet-iptables-7.0.0/linuxnet/iptables/matches/multiportmatch.py
--rw-r--r--   0 panos     (1001) users      (100)     7720 2024-01-19 19:36:42.000000 linuxnet-iptables-7.0.0/linuxnet/iptables/matches/ownermatch.py
--rw-r--r--   0 panos     (1001) users      (100)    13237 2024-03-21 03:17:25.000000 linuxnet-iptables-7.0.0/linuxnet/iptables/matches/packetmatch.py
--rw-r--r--   0 panos     (1001) users      (100)     2827 2023-07-09 21:05:25.000000 linuxnet-iptables-7.0.0/linuxnet/iptables/matches/packettypematch.py
--rw-r--r--   0 panos     (1001) users      (100)    11615 2023-09-09 02:06:12.000000 linuxnet-iptables-7.0.0/linuxnet/iptables/matches/recentmatch.py
--rw-r--r--   0 panos     (1001) users      (100)     9562 2023-09-09 02:06:12.000000 linuxnet-iptables-7.0.0/linuxnet/iptables/matches/setmatch.py
--rw-r--r--   0 panos     (1001) users      (100)     3049 2023-07-14 00:05:40.000000 linuxnet-iptables-7.0.0/linuxnet/iptables/matches/statematch.py
--rw-r--r--   0 panos     (1001) users      (100)     4240 2023-10-21 19:41:05.000000 linuxnet-iptables-7.0.0/linuxnet/iptables/matches/statisticmatch.py
--rw-r--r--   0 panos     (1001) users      (100)    10597 2023-08-20 16:02:58.000000 linuxnet-iptables-7.0.0/linuxnet/iptables/matches/tcpmatch.py
--rw-r--r--   0 panos     (1001) users      (100)     3776 2023-07-09 21:05:25.000000 linuxnet-iptables-7.0.0/linuxnet/iptables/matches/tcpmssmatch.py
--rw-r--r--   0 panos     (1001) users      (100)     4317 2023-07-09 21:05:25.000000 linuxnet-iptables-7.0.0/linuxnet/iptables/matches/ttlmatch.py
--rw-r--r--   0 panos     (1001) users      (100)     2597 2023-07-09 21:05:25.000000 linuxnet-iptables-7.0.0/linuxnet/iptables/matches/udpmatch.py
--rw-r--r--   0 panos     (1001) users      (100)     7827 2023-10-21 19:41:05.000000 linuxnet-iptables-7.0.0/linuxnet/iptables/matches/util.py
--rw-r--r--   0 panos     (1001) users      (100)      924 2024-03-21 03:17:26.000000 linuxnet-iptables-7.0.0/linuxnet/iptables/metadata.py
--rw-r--r--   0 panos     (1001) users      (100)     8386 2023-07-14 00:05:40.000000 linuxnet-iptables-7.0.0/linuxnet/iptables/parsing.py
--rw-r--r--   0 panos     (1001) users      (100)    19537 2024-03-21 03:17:26.000000 linuxnet-iptables-7.0.0/linuxnet/iptables/rule.py
--rw-r--r--   0 panos     (1001) users      (100)    30222 2024-03-21 03:17:26.000000 linuxnet-iptables-7.0.0/linuxnet/iptables/table.py
-drwxr-sr-x   0 panos     (1001) users      (100)        0 2024-03-21 15:09:12.301459 linuxnet-iptables-7.0.0/linuxnet/iptables/targets/
--rw-r--r--   0 panos     (1001) users      (100)     1165 2023-06-04 01:25:41.000000 linuxnet-iptables-7.0.0/linuxnet/iptables/targets/__init__.py
--rw-r--r--   0 panos     (1001) users      (100)     7447 2024-03-21 03:17:26.000000 linuxnet-iptables-7.0.0/linuxnet/iptables/targets/connmarktarget.py
--rw-r--r--   0 panos     (1001) users      (100)     6578 2024-03-21 03:17:26.000000 linuxnet-iptables-7.0.0/linuxnet/iptables/targets/logtarget.py
--rw-r--r--   0 panos     (1001) users      (100)     6613 2024-03-21 03:17:25.000000 linuxnet-iptables-7.0.0/linuxnet/iptables/targets/marktarget.py
--rw-r--r--   0 panos     (1001) users      (100)     4834 2024-03-21 03:17:26.000000 linuxnet-iptables-7.0.0/linuxnet/iptables/targets/masqueradetarget.py
--rw-r--r--   0 panos     (1001) users      (100)    10361 2024-03-21 03:17:25.000000 linuxnet-iptables-7.0.0/linuxnet/iptables/targets/nattarget.py
--rw-r--r--   0 panos     (1001) users      (100)     1405 2023-06-19 04:02:28.000000 linuxnet-iptables-7.0.0/linuxnet/iptables/targets/notracktarget.py
--rw-r--r--   0 panos     (1001) users      (100)     2185 2024-03-21 03:17:25.000000 linuxnet-iptables-7.0.0/linuxnet/iptables/targets/rejecttarget.py
--rw-r--r--   0 panos     (1001) users      (100)    11461 2024-03-21 03:17:25.000000 linuxnet-iptables-7.0.0/linuxnet/iptables/targets/target.py
--rw-r--r--   0 panos     (1001) users      (100)     1387 2023-06-19 04:02:28.000000 linuxnet-iptables-7.0.0/linuxnet/iptables/targets/tracetarget.py
--rw-r--r--   0 panos     (1001) users      (100)     4934 2024-03-21 03:17:25.000000 linuxnet-iptables-7.0.0/linuxnet/iptables/targets/ttltarget.py
-drwxr-sr-x   0 panos     (1001) users      (100)        0 2024-03-21 15:09:12.302459 linuxnet-iptables-7.0.0/linuxnet_iptables.egg-info/
--rw-r--r--   0 panos     (1001) users      (100)     4108 2024-03-21 15:09:12.000000 linuxnet-iptables-7.0.0/linuxnet_iptables.egg-info/PKG-INFO
--rw-r--r--   0 panos     (1001) users      (100)     3049 2024-03-21 15:09:12.000000 linuxnet-iptables-7.0.0/linuxnet_iptables.egg-info/SOURCES.txt
--rw-r--r--   0 panos     (1001) users      (100)        1 2024-03-21 15:09:12.000000 linuxnet-iptables-7.0.0/linuxnet_iptables.egg-info/dependency_links.txt
--rw-r--r--   0 panos     (1001) users      (100)        9 2024-03-21 15:09:12.000000 linuxnet-iptables-7.0.0/linuxnet_iptables.egg-info/top_level.txt
--rw-r--r--   0 panos     (1001) users      (100)       38 2024-03-21 15:09:12.303460 linuxnet-iptables-7.0.0/setup.cfg
--rw-r--r--   0 panos     (1001) users      (100)     6662 2023-06-05 00:27:39.000000 linuxnet-iptables-7.0.0/setup.py
-drwxr-sr-x   0 panos     (1001) users      (100)        0 2024-03-21 15:09:12.302459 linuxnet-iptables-7.0.0/tests/
--rw-r--r--   0 panos     (1001) users      (100)        0 2023-01-01 01:13:07.000000 linuxnet-iptables-7.0.0/tests/__init__.py
--rw-r--r--   0 panos     (1001) users      (100)    93616 2024-03-21 03:17:26.000000 linuxnet-iptables-7.0.0/tests/iptables_test.py
+drwxr-sr-x   0 panos     (1001) users      (100)        0 2024-04-06 21:45:02.170597 linuxnet-iptables-7.0.3/
+-rw-r--r--   0 panos     (1001) users      (100)    18810 2023-01-01 01:13:07.000000 linuxnet-iptables-7.0.3/.pylintrc
+-rw-r--r--   0 panos     (1001) users      (100)     5303 2024-04-06 21:40:18.000000 linuxnet-iptables-7.0.3/CHANGELOG.md
+-rw-r--r--   0 panos     (1001) users      (100)    32387 2023-01-01 01:13:10.000000 linuxnet-iptables-7.0.3/LICENSE
+-rw-r--r--   0 panos     (1001) users      (100)      284 2023-02-06 17:07:04.000000 linuxnet-iptables-7.0.3/MANIFEST.in
+-rw-r--r--   0 panos     (1001) users      (100)     5164 2023-01-01 01:13:07.000000 linuxnet-iptables-7.0.3/Makefile
+-rw-r--r--   0 panos     (1001) users      (100)     4128 2024-04-06 21:45:02.170597 linuxnet-iptables-7.0.3/PKG-INFO
+-rw-r--r--   0 panos     (1001) users      (100)     3233 2024-03-21 15:25:55.000000 linuxnet-iptables-7.0.3/README.md
+drwxr-sr-x   0 panos     (1001) users      (100)        0 2024-04-06 21:45:02.158597 linuxnet-iptables-7.0.3/docs/
+-rw-r--r--   0 panos     (1001) users      (100)      905 2023-01-01 01:13:06.000000 linuxnet-iptables-7.0.3/docs/Makefile
+-rw-r--r--   0 panos     (1001) users      (100)     1491 2023-03-01 20:08:53.000000 linuxnet-iptables-7.0.3/docs/chain.rst
+-rw-r--r--   0 panos     (1001) users      (100)     2850 2023-01-27 18:52:21.000000 linuxnet-iptables-7.0.3/docs/conf.py
+-rw-r--r--   0 panos     (1001) users      (100)     1061 2023-02-06 17:07:04.000000 linuxnet-iptables-7.0.3/docs/exception.rst
+-rw-r--r--   0 panos     (1001) users      (100)     8253 2024-03-21 15:10:01.000000 linuxnet-iptables-7.0.3/docs/extensibility.rst
+-rw-r--r--   0 panos     (1001) users      (100)     3335 2024-03-21 15:10:01.000000 linuxnet-iptables-7.0.3/docs/index.rst
+-rw-r--r--   0 panos     (1001) users      (100)     3543 2024-03-21 15:10:01.000000 linuxnet-iptables-7.0.3/docs/iptables_api.rst
+-rw-r--r--   0 panos     (1001) users      (100)     3047 2023-07-09 21:05:25.000000 linuxnet-iptables-7.0.3/docs/match-example.py
+-rw-r--r--   0 panos     (1001) users      (100)     2258 2023-02-08 00:19:00.000000 linuxnet-iptables-7.0.3/docs/match.rst
+drwxr-sr-x   0 panos     (1001) users      (100)        0 2024-04-06 21:45:02.161597 linuxnet-iptables-7.0.3/docs/matches/
+-rw-r--r--   0 panos     (1001) users      (100)     1335 2023-06-19 04:02:28.000000 linuxnet-iptables-7.0.3/docs/matches/addrtypematch.rst
+-rw-r--r--   0 panos     (1001) users      (100)     1431 2023-02-06 17:07:04.000000 linuxnet-iptables-7.0.3/docs/matches/commentmatch.rst
+-rw-r--r--   0 panos     (1001) users      (100)     1268 2023-07-14 00:05:40.000000 linuxnet-iptables-7.0.3/docs/matches/connmarkmatch.rst
+-rw-r--r--   0 panos     (1001) users      (100)     3253 2023-09-09 02:06:12.000000 linuxnet-iptables-7.0.3/docs/matches/conntrackmatch.rst
+-rw-r--r--   0 panos     (1001) users      (100)     1899 2023-02-06 17:07:04.000000 linuxnet-iptables-7.0.3/docs/matches/icmpmatch.rst
+-rw-r--r--   0 panos     (1001) users      (100)     1861 2023-02-20 17:08:37.000000 linuxnet-iptables-7.0.3/docs/matches/limitmatch.rst
+-rw-r--r--   0 panos     (1001) users      (100)     1430 2023-10-21 19:41:05.000000 linuxnet-iptables-7.0.3/docs/matches/macmatch.rst
+-rw-r--r--   0 panos     (1001) users      (100)     1438 2023-07-14 00:05:40.000000 linuxnet-iptables-7.0.3/docs/matches/markmatch.rst
+-rw-r--r--   0 panos     (1001) users      (100)     1539 2024-01-19 19:36:42.000000 linuxnet-iptables-7.0.3/docs/matches/multiportmatch.rst
+-rw-r--r--   0 panos     (1001) users      (100)     2131 2023-09-09 02:06:12.000000 linuxnet-iptables-7.0.3/docs/matches/ownermatch.rst
+-rw-r--r--   0 panos     (1001) users      (100)     2447 2023-02-08 00:19:00.000000 linuxnet-iptables-7.0.3/docs/matches/packetmatch.rst
+-rw-r--r--   0 panos     (1001) users      (100)     1511 2023-02-06 17:07:04.000000 linuxnet-iptables-7.0.3/docs/matches/packettypematch.rst
+-rw-r--r--   0 panos     (1001) users      (100)     2248 2023-07-14 00:05:40.000000 linuxnet-iptables-7.0.3/docs/matches/recentmatch.rst
+-rw-r--r--   0 panos     (1001) users      (100)     1736 2023-09-09 02:06:12.000000 linuxnet-iptables-7.0.3/docs/matches/setmatch.rst
+-rw-r--r--   0 panos     (1001) users      (100)     1312 2023-02-06 17:07:04.000000 linuxnet-iptables-7.0.3/docs/matches/statematch.rst
+-rw-r--r--   0 panos     (1001) users      (100)     1251 2023-09-09 02:06:12.000000 linuxnet-iptables-7.0.3/docs/matches/statisticmatch.rst
+-rw-r--r--   0 panos     (1001) users      (100)     2302 2023-07-14 00:05:40.000000 linuxnet-iptables-7.0.3/docs/matches/tcpmatch.rst
+-rw-r--r--   0 panos     (1001) users      (100)     1382 2023-02-06 17:07:04.000000 linuxnet-iptables-7.0.3/docs/matches/tcpmssmatch.rst
+-rw-r--r--   0 panos     (1001) users      (100)     1528 2023-09-09 02:06:12.000000 linuxnet-iptables-7.0.3/docs/matches/ttlmatch.rst
+-rw-r--r--   0 panos     (1001) users      (100)     1280 2023-02-06 17:07:04.000000 linuxnet-iptables-7.0.3/docs/matches/udpmatch.rst
+-rw-r--r--   0 panos     (1001) users      (100)      873 2023-03-01 20:08:53.000000 linuxnet-iptables-7.0.3/docs/rule.rst
+-rw-r--r--   0 panos     (1001) users      (100)      903 2023-02-05 23:48:29.000000 linuxnet-iptables-7.0.3/docs/table.rst
+-rw-r--r--   0 panos     (1001) users      (100)     1184 2024-03-21 15:10:01.000000 linuxnet-iptables-7.0.3/docs/target-example.py
+-rw-r--r--   0 panos     (1001) users      (100)     1201 2023-02-08 00:19:00.000000 linuxnet-iptables-7.0.3/docs/target.rst
+drwxr-sr-x   0 panos     (1001) users      (100)        0 2024-04-06 21:45:02.162597 linuxnet-iptables-7.0.3/docs/targets/
+-rw-r--r--   0 panos     (1001) users      (100)      903 2023-02-06 17:07:04.000000 linuxnet-iptables-7.0.3/docs/targets/chaintarget.rst
+-rw-r--r--   0 panos     (1001) users      (100)      912 2023-02-06 17:07:04.000000 linuxnet-iptables-7.0.3/docs/targets/connmarktarget.rst
+-rw-r--r--   0 panos     (1001) users      (100)      900 2023-02-06 17:07:04.000000 linuxnet-iptables-7.0.3/docs/targets/dnattarget.rst
+-rw-r--r--   0 panos     (1001) users      (100)      897 2023-02-06 17:07:04.000000 linuxnet-iptables-7.0.3/docs/targets/logtarget.rst
+-rw-r--r--   0 panos     (1001) users      (100)      900 2023-02-06 17:07:04.000000 linuxnet-iptables-7.0.3/docs/targets/marktarget.rst
+-rw-r--r--   0 panos     (1001) users      (100)      912 2023-02-06 17:07:04.000000 linuxnet-iptables-7.0.3/docs/targets/masqueradetarget.rst
+-rw-r--r--   0 panos     (1001) users      (100)      902 2023-06-04 01:25:41.000000 linuxnet-iptables-7.0.3/docs/targets/notracktarget.rst
+-rw-r--r--   0 panos     (1001) users      (100)      906 2023-02-06 17:07:04.000000 linuxnet-iptables-7.0.3/docs/targets/rejecttarget.rst
+-rw-r--r--   0 panos     (1001) users      (100)      900 2023-02-06 17:07:04.000000 linuxnet-iptables-7.0.3/docs/targets/snattarget.rst
+-rw-r--r--   0 panos     (1001) users      (100)      896 2023-06-04 01:25:41.000000 linuxnet-iptables-7.0.3/docs/targets/tracetarget.rst
+-rw-r--r--   0 panos     (1001) users      (100)      897 2023-02-06 17:07:04.000000 linuxnet-iptables-7.0.3/docs/targets/ttltarget.rst
+drwxr-sr-x   0 panos     (1001) users      (100)        0 2024-04-06 21:45:02.162597 linuxnet-iptables-7.0.3/linuxnet/
+-rw-r--r--   0 panos     (1001) users      (100)        0 2023-01-01 01:13:07.000000 linuxnet-iptables-7.0.3/linuxnet/__init__.py
+drwxr-sr-x   0 panos     (1001) users      (100)        0 2024-04-06 21:45:02.164597 linuxnet-iptables-7.0.3/linuxnet/iptables/
+-rw-r--r--   0 panos     (1001) users      (100)     1170 2023-03-01 20:08:53.000000 linuxnet-iptables-7.0.3/linuxnet/iptables/__init__.py
+-rw-r--r--   0 panos     (1001) users      (100)    29055 2023-07-24 18:13:22.000000 linuxnet-iptables-7.0.3/linuxnet/iptables/chain.py
+-rw-r--r--   0 panos     (1001) users      (100)      854 2023-02-20 17:08:37.000000 linuxnet-iptables-7.0.3/linuxnet/iptables/deps.py
+-rw-r--r--   0 panos     (1001) users      (100)     2564 2024-03-21 15:10:01.000000 linuxnet-iptables-7.0.3/linuxnet/iptables/exceptions.py
+-rw-r--r--   0 panos     (1001) users      (100)     1467 2023-07-14 00:05:40.000000 linuxnet-iptables-7.0.3/linuxnet/iptables/extension.py
+drwxr-sr-x   0 panos     (1001) users      (100)        0 2024-04-06 21:45:02.167597 linuxnet-iptables-7.0.3/linuxnet/iptables/matches/
+-rw-r--r--   0 panos     (1001) users      (100)     1524 2024-01-19 19:36:42.000000 linuxnet-iptables-7.0.3/linuxnet/iptables/matches/__init__.py
+-rw-r--r--   0 panos     (1001) users      (100)     4978 2023-07-09 21:05:25.000000 linuxnet-iptables-7.0.3/linuxnet/iptables/matches/addrtypematch.py
+-rw-r--r--   0 panos     (1001) users      (100)     2879 2023-07-09 21:05:25.000000 linuxnet-iptables-7.0.3/linuxnet/iptables/matches/commentmatch.py
+-rw-r--r--   0 panos     (1001) users      (100)     2285 2023-07-09 21:05:25.000000 linuxnet-iptables-7.0.3/linuxnet/iptables/matches/connmarkmatch.py
+-rw-r--r--   0 panos     (1001) users      (100)    17982 2024-03-21 15:10:01.000000 linuxnet-iptables-7.0.3/linuxnet/iptables/matches/conntrackmatch.py
+-rw-r--r--   0 panos     (1001) users      (100)     9761 2023-07-09 21:05:25.000000 linuxnet-iptables-7.0.3/linuxnet/iptables/matches/icmpmatch.py
+-rw-r--r--   0 panos     (1001) users      (100)     4559 2023-07-09 21:05:25.000000 linuxnet-iptables-7.0.3/linuxnet/iptables/matches/limitmatch.py
+-rw-r--r--   0 panos     (1001) users      (100)     2458 2023-10-21 19:41:05.000000 linuxnet-iptables-7.0.3/linuxnet/iptables/matches/macmatch.py
+-rw-r--r--   0 panos     (1001) users      (100)     3872 2023-07-09 21:05:25.000000 linuxnet-iptables-7.0.3/linuxnet/iptables/matches/markmatch.py
+-rw-r--r--   0 panos     (1001) users      (100)    16971 2024-03-21 15:10:01.000000 linuxnet-iptables-7.0.3/linuxnet/iptables/matches/match.py
+-rw-r--r--   0 panos     (1001) users      (100)     6094 2024-01-19 19:59:34.000000 linuxnet-iptables-7.0.3/linuxnet/iptables/matches/multiportmatch.py
+-rw-r--r--   0 panos     (1001) users      (100)     7720 2024-01-19 19:36:42.000000 linuxnet-iptables-7.0.3/linuxnet/iptables/matches/ownermatch.py
+-rw-r--r--   0 panos     (1001) users      (100)    14131 2024-04-06 20:58:43.000000 linuxnet-iptables-7.0.3/linuxnet/iptables/matches/packetmatch.py
+-rw-r--r--   0 panos     (1001) users      (100)     2827 2023-07-09 21:05:25.000000 linuxnet-iptables-7.0.3/linuxnet/iptables/matches/packettypematch.py
+-rw-r--r--   0 panos     (1001) users      (100)    11615 2023-09-09 02:06:12.000000 linuxnet-iptables-7.0.3/linuxnet/iptables/matches/recentmatch.py
+-rw-r--r--   0 panos     (1001) users      (100)     9562 2023-09-09 02:06:12.000000 linuxnet-iptables-7.0.3/linuxnet/iptables/matches/setmatch.py
+-rw-r--r--   0 panos     (1001) users      (100)     3049 2023-07-14 00:05:40.000000 linuxnet-iptables-7.0.3/linuxnet/iptables/matches/statematch.py
+-rw-r--r--   0 panos     (1001) users      (100)     4240 2023-10-21 19:41:05.000000 linuxnet-iptables-7.0.3/linuxnet/iptables/matches/statisticmatch.py
+-rw-r--r--   0 panos     (1001) users      (100)    10597 2023-08-20 16:02:58.000000 linuxnet-iptables-7.0.3/linuxnet/iptables/matches/tcpmatch.py
+-rw-r--r--   0 panos     (1001) users      (100)     3776 2023-07-09 21:05:25.000000 linuxnet-iptables-7.0.3/linuxnet/iptables/matches/tcpmssmatch.py
+-rw-r--r--   0 panos     (1001) users      (100)     4317 2023-07-09 21:05:25.000000 linuxnet-iptables-7.0.3/linuxnet/iptables/matches/ttlmatch.py
+-rw-r--r--   0 panos     (1001) users      (100)     2597 2023-07-09 21:05:25.000000 linuxnet-iptables-7.0.3/linuxnet/iptables/matches/udpmatch.py
+-rw-r--r--   0 panos     (1001) users      (100)     7827 2023-10-21 19:41:05.000000 linuxnet-iptables-7.0.3/linuxnet/iptables/matches/util.py
+-rw-r--r--   0 panos     (1001) users      (100)      924 2024-04-06 20:58:43.000000 linuxnet-iptables-7.0.3/linuxnet/iptables/metadata.py
+-rw-r--r--   0 panos     (1001) users      (100)     8386 2023-07-14 00:05:40.000000 linuxnet-iptables-7.0.3/linuxnet/iptables/parsing.py
+-rw-r--r--   0 panos     (1001) users      (100)    19537 2024-03-21 15:10:01.000000 linuxnet-iptables-7.0.3/linuxnet/iptables/rule.py
+-rw-r--r--   0 panos     (1001) users      (100)    30222 2024-03-21 15:10:01.000000 linuxnet-iptables-7.0.3/linuxnet/iptables/table.py
+drwxr-sr-x   0 panos     (1001) users      (100)        0 2024-04-06 21:45:02.169597 linuxnet-iptables-7.0.3/linuxnet/iptables/targets/
+-rw-r--r--   0 panos     (1001) users      (100)     1165 2023-06-04 01:25:41.000000 linuxnet-iptables-7.0.3/linuxnet/iptables/targets/__init__.py
+-rw-r--r--   0 panos     (1001) users      (100)     7447 2024-03-21 15:10:01.000000 linuxnet-iptables-7.0.3/linuxnet/iptables/targets/connmarktarget.py
+-rw-r--r--   0 panos     (1001) users      (100)     6578 2024-03-21 15:10:01.000000 linuxnet-iptables-7.0.3/linuxnet/iptables/targets/logtarget.py
+-rw-r--r--   0 panos     (1001) users      (100)     6613 2024-03-21 15:10:01.000000 linuxnet-iptables-7.0.3/linuxnet/iptables/targets/marktarget.py
+-rw-r--r--   0 panos     (1001) users      (100)     4834 2024-03-21 15:10:01.000000 linuxnet-iptables-7.0.3/linuxnet/iptables/targets/masqueradetarget.py
+-rw-r--r--   0 panos     (1001) users      (100)    10361 2024-03-21 15:10:01.000000 linuxnet-iptables-7.0.3/linuxnet/iptables/targets/nattarget.py
+-rw-r--r--   0 panos     (1001) users      (100)     1405 2023-06-19 04:02:28.000000 linuxnet-iptables-7.0.3/linuxnet/iptables/targets/notracktarget.py
+-rw-r--r--   0 panos     (1001) users      (100)     2185 2024-03-21 15:10:01.000000 linuxnet-iptables-7.0.3/linuxnet/iptables/targets/rejecttarget.py
+-rw-r--r--   0 panos     (1001) users      (100)    11461 2024-03-21 15:10:01.000000 linuxnet-iptables-7.0.3/linuxnet/iptables/targets/target.py
+-rw-r--r--   0 panos     (1001) users      (100)     1387 2023-06-19 04:02:28.000000 linuxnet-iptables-7.0.3/linuxnet/iptables/targets/tracetarget.py
+-rw-r--r--   0 panos     (1001) users      (100)     4934 2024-03-21 15:10:01.000000 linuxnet-iptables-7.0.3/linuxnet/iptables/targets/ttltarget.py
+drwxr-sr-x   0 panos     (1001) users      (100)        0 2024-04-06 21:45:02.170597 linuxnet-iptables-7.0.3/linuxnet_iptables.egg-info/
+-rw-r--r--   0 panos     (1001) users      (100)     4128 2024-04-06 21:45:02.000000 linuxnet-iptables-7.0.3/linuxnet_iptables.egg-info/PKG-INFO
+-rw-r--r--   0 panos     (1001) users      (100)     3049 2024-04-06 21:45:02.000000 linuxnet-iptables-7.0.3/linuxnet_iptables.egg-info/SOURCES.txt
+-rw-r--r--   0 panos     (1001) users      (100)        1 2024-04-06 21:45:02.000000 linuxnet-iptables-7.0.3/linuxnet_iptables.egg-info/dependency_links.txt
+-rw-r--r--   0 panos     (1001) users      (100)        9 2024-04-06 21:45:02.000000 linuxnet-iptables-7.0.3/linuxnet_iptables.egg-info/top_level.txt
+-rw-r--r--   0 panos     (1001) users      (100)       38 2024-04-06 21:45:02.170597 linuxnet-iptables-7.0.3/setup.cfg
+-rw-r--r--   0 panos     (1001) users      (100)     6662 2023-06-05 00:27:39.000000 linuxnet-iptables-7.0.3/setup.py
+drwxr-sr-x   0 panos     (1001) users      (100)        0 2024-04-06 21:45:02.170597 linuxnet-iptables-7.0.3/tests/
+-rw-r--r--   0 panos     (1001) users      (100)        0 2023-01-01 01:13:07.000000 linuxnet-iptables-7.0.3/tests/__init__.py
+-rw-r--r--   0 panos     (1001) users      (100)    93616 2024-03-21 15:10:01.000000 linuxnet-iptables-7.0.3/tests/iptables_test.py
```

### Comparing `linuxnet-iptables-7.0.0/.pylintrc` & `linuxnet-iptables-7.0.3/.pylintrc`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-7.0.0/CHANGELOG.md` & `linuxnet-iptables-7.0.3/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,19 @@
 Change Log
 ==========
 
 
+7.0.3 (2024-04-06)
+------------------
+
+- comparison value used in SourceAddressCriterion/DestAddressCriterion
+  may be specified as a IPv4Address/IPv6Address or as a string (in
+  addition to IPv4Network/IPv6Network)
+
+
 7.0.0 (2024-03-21)
 ------------------
 
 - added IPv6 support; the PacketMatch, ConntrackMatch, SnatTarget, DnatTarget
   classes now support both IPv4 and IPv6 addresses
 - SnatTarget now supports the --random-fully option of the SNAT target
 - this version maintains user API backwards-compatibility;
```

### Comparing `linuxnet-iptables-7.0.0/LICENSE` & `linuxnet-iptables-7.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-7.0.0/Makefile` & `linuxnet-iptables-7.0.3/Makefile`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-7.0.0/PKG-INFO` & `linuxnet-iptables-7.0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linuxnet-iptables
-Version: 7.0.0
+Version: 7.0.3
 Summary: programmatic access to Linux iptables
 Home-page: https://gitlab.com/panos-tools/linuxnet-iptables
 Author: Panagiotis (Panos) Tsirigotis
 Author-email: ptsirigotis01@gmail.com
 License: AGPLv3
 Project-URL: Source, https://gitlab.com/panos-tools/linuxnet-iptables
 Project-URL: Documentation, https://linuxnet-iptables.readthedocs.io/en/latest/index.html
@@ -18,15 +18,15 @@
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # linuxnet-iptables
 
 **linuxnet-iptables** provides programmatic access to the
-Linux `iptables(8)` command.
+Linux `iptables(8)` (or `ip6tables(8)`) command.
 Using **linuxnet-iptables** one can view existing chains/rules,
 create new ones, or delete existing ones.
 The package documentation is available
 [here](https://linuxnet-iptables.readthedocs.io/en/latest/index.html).
 
 For the following examples, Python3 (3.6 or later) is required.
```

### Comparing `linuxnet-iptables-7.0.0/README.md` & `linuxnet-iptables-7.0.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # linuxnet-iptables
 
 **linuxnet-iptables** provides programmatic access to the
-Linux `iptables(8)` command.
+Linux `iptables(8)` (or `ip6tables(8)`) command.
 Using **linuxnet-iptables** one can view existing chains/rules,
 create new ones, or delete existing ones.
 The package documentation is available
 [here](https://linuxnet-iptables.readthedocs.io/en/latest/index.html).
 
 For the following examples, Python3 (3.6 or later) is required.
```

### Comparing `linuxnet-iptables-7.0.0/docs/Makefile` & `linuxnet-iptables-7.0.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-7.0.0/docs/chain.rst` & `linuxnet-iptables-7.0.3/docs/chain.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-7.0.0/docs/conf.py` & `linuxnet-iptables-7.0.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-7.0.0/docs/exception.rst` & `linuxnet-iptables-7.0.3/docs/exception.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-7.0.0/docs/extensibility.rst` & `linuxnet-iptables-7.0.3/docs/extensibility.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-7.0.0/docs/index.rst` & `linuxnet-iptables-7.0.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-7.0.0/docs/iptables_api.rst` & `linuxnet-iptables-7.0.3/docs/iptables_api.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-7.0.0/docs/match-example.py` & `linuxnet-iptables-7.0.3/docs/match-example.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-7.0.0/docs/match.rst` & `linuxnet-iptables-7.0.3/docs/match.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-7.0.0/docs/matches/addrtypematch.rst` & `linuxnet-iptables-7.0.3/docs/matches/addrtypematch.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-7.0.0/docs/matches/commentmatch.rst` & `linuxnet-iptables-7.0.3/docs/matches/commentmatch.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-7.0.0/docs/matches/connmarkmatch.rst` & `linuxnet-iptables-7.0.3/docs/matches/connmarkmatch.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-7.0.0/docs/matches/conntrackmatch.rst` & `linuxnet-iptables-7.0.3/docs/matches/conntrackmatch.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-7.0.0/docs/matches/icmpmatch.rst` & `linuxnet-iptables-7.0.3/docs/matches/icmpmatch.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-7.0.0/docs/matches/limitmatch.rst` & `linuxnet-iptables-7.0.3/docs/matches/limitmatch.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-7.0.0/docs/matches/macmatch.rst` & `linuxnet-iptables-7.0.3/docs/matches/macmatch.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-7.0.0/docs/matches/markmatch.rst` & `linuxnet-iptables-7.0.3/docs/matches/markmatch.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-7.0.0/docs/matches/multiportmatch.rst` & `linuxnet-iptables-7.0.3/docs/matches/multiportmatch.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-7.0.0/docs/matches/ownermatch.rst` & `linuxnet-iptables-7.0.3/docs/matches/ownermatch.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-7.0.0/docs/matches/packetmatch.rst` & `linuxnet-iptables-7.0.3/docs/matches/packetmatch.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-7.0.0/docs/matches/packettypematch.rst` & `linuxnet-iptables-7.0.3/docs/matches/packettypematch.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-7.0.0/docs/matches/recentmatch.rst` & `linuxnet-iptables-7.0.3/docs/matches/recentmatch.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-7.0.0/docs/matches/setmatch.rst` & `linuxnet-iptables-7.0.3/docs/matches/setmatch.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-7.0.0/docs/matches/statematch.rst` & `linuxnet-iptables-7.0.3/docs/matches/statematch.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-7.0.0/docs/matches/statisticmatch.rst` & `linuxnet-iptables-7.0.3/docs/matches/statisticmatch.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-7.0.0/docs/matches/tcpmatch.rst` & `linuxnet-iptables-7.0.3/docs/matches/tcpmatch.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-7.0.0/docs/matches/tcpmssmatch.rst` & `linuxnet-iptables-7.0.3/docs/matches/tcpmssmatch.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-7.0.0/docs/matches/ttlmatch.rst` & `linuxnet-iptables-7.0.3/docs/matches/ttlmatch.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-7.0.0/docs/matches/udpmatch.rst` & `linuxnet-iptables-7.0.3/docs/matches/udpmatch.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-7.0.0/docs/rule.rst` & `linuxnet-iptables-7.0.3/docs/rule.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-7.0.0/docs/table.rst` & `linuxnet-iptables-7.0.3/docs/table.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-7.0.0/docs/target-example.py` & `linuxnet-iptables-7.0.3/docs/target-example.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-7.0.0/docs/target.rst` & `linuxnet-iptables-7.0.3/docs/target.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-7.0.0/docs/targets/chaintarget.rst` & `linuxnet-iptables-7.0.3/docs/targets/chaintarget.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-7.0.0/docs/targets/connmarktarget.rst` & `linuxnet-iptables-7.0.3/docs/targets/connmarktarget.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-7.0.0/docs/targets/dnattarget.rst` & `linuxnet-iptables-7.0.3/docs/targets/dnattarget.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-7.0.0/docs/targets/logtarget.rst` & `linuxnet-iptables-7.0.3/docs/targets/logtarget.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-7.0.0/docs/targets/marktarget.rst` & `linuxnet-iptables-7.0.3/docs/targets/marktarget.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-7.0.0/docs/targets/masqueradetarget.rst` & `linuxnet-iptables-7.0.3/docs/targets/masqueradetarget.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-7.0.0/docs/targets/notracktarget.rst` & `linuxnet-iptables-7.0.3/docs/targets/notracktarget.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-7.0.0/docs/targets/rejecttarget.rst` & `linuxnet-iptables-7.0.3/docs/targets/rejecttarget.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-7.0.0/docs/targets/snattarget.rst` & `linuxnet-iptables-7.0.3/docs/targets/snattarget.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-7.0.0/docs/targets/tracetarget.rst` & `linuxnet-iptables-7.0.3/docs/targets/tracetarget.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-7.0.0/docs/targets/ttltarget.rst` & `linuxnet-iptables-7.0.3/docs/targets/ttltarget.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-7.0.0/linuxnet/iptables/__init__.py` & `linuxnet-iptables-7.0.3/linuxnet/iptables/__init__.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-7.0.0/linuxnet/iptables/chain.py` & `linuxnet-iptables-7.0.3/linuxnet/iptables/chain.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-7.0.0/linuxnet/iptables/deps.py` & `linuxnet-iptables-7.0.3/linuxnet/iptables/deps.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-7.0.0/linuxnet/iptables/exceptions.py` & `linuxnet-iptables-7.0.3/linuxnet/iptables/exceptions.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-7.0.0/linuxnet/iptables/extension.py` & `linuxnet-iptables-7.0.3/linuxnet/iptables/extension.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-7.0.0/linuxnet/iptables/matches/__init__.py` & `linuxnet-iptables-7.0.3/linuxnet/iptables/matches/__init__.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-7.0.0/linuxnet/iptables/matches/addrtypematch.py` & `linuxnet-iptables-7.0.3/linuxnet/iptables/matches/addrtypematch.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-7.0.0/linuxnet/iptables/matches/commentmatch.py` & `linuxnet-iptables-7.0.3/linuxnet/iptables/matches/commentmatch.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-7.0.0/linuxnet/iptables/matches/connmarkmatch.py` & `linuxnet-iptables-7.0.3/linuxnet/iptables/matches/connmarkmatch.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-7.0.0/linuxnet/iptables/matches/conntrackmatch.py` & `linuxnet-iptables-7.0.3/linuxnet/iptables/matches/conntrackmatch.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-7.0.0/linuxnet/iptables/matches/icmpmatch.py` & `linuxnet-iptables-7.0.3/linuxnet/iptables/matches/icmpmatch.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-7.0.0/linuxnet/iptables/matches/limitmatch.py` & `linuxnet-iptables-7.0.3/linuxnet/iptables/matches/limitmatch.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-7.0.0/linuxnet/iptables/matches/macmatch.py` & `linuxnet-iptables-7.0.3/linuxnet/iptables/matches/macmatch.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-7.0.0/linuxnet/iptables/matches/markmatch.py` & `linuxnet-iptables-7.0.3/linuxnet/iptables/matches/markmatch.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-7.0.0/linuxnet/iptables/matches/match.py` & `linuxnet-iptables-7.0.3/linuxnet/iptables/matches/match.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-7.0.0/linuxnet/iptables/matches/multiportmatch.py` & `linuxnet-iptables-7.0.3/linuxnet/iptables/matches/multiportmatch.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-7.0.0/linuxnet/iptables/matches/ownermatch.py` & `linuxnet-iptables-7.0.3/linuxnet/iptables/matches/ownermatch.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-7.0.0/linuxnet/iptables/matches/packetmatch.py` & `linuxnet-iptables-7.0.3/linuxnet/iptables/matches/packetmatch.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 # <https://www.gnu.org/licenses/>.
 
 """
 This module provides the PacketMatch class which supports
 matching against standard packet attributes
 """
 
-from ipaddress import IPv4Network, IPv6Network
+from ipaddress import IPv4Network, IPv6Network, IPv4Address, IPv6Address
 from typing import Iterable, List, Optional, Union
 
 from ..exceptions import IptablesError, IptablesParsingError
 from ..deps import get_logger
 
 from .match import Criterion, Match, MatchParser
 from .util import BooleanCriterion, GenericCriterion
@@ -75,17 +75,36 @@
         return self.__option
 
     def get_value(self) -> Union[IPv4Network, IPv6Network, None]:
         """Returns the criterion value
         """
         return self.__value
 
-    def equals(self, value: Union[IPv4Network, IPv6Network]) -> Match:    # pylint: disable=arguments-differ
-        """Compare with the specified value
+    def equals(self,                    # pylint: disable=arguments-differ
+        value: Union[IPv4Network, IPv6Network,
+                        IPv4Address, IPv6Address, str]) -> Match:
+        """Compare with the specified value, which can be specified as
+        an :class:`IPv4Network`, an :class:`IPv6Network`,
+        an :class:`IPv4Address`, an :class:`IPv6Address`, or as
+        a string. Internally the value is always stored as
+        an :class:`IPv4Network`, or an :class:`IPv6Network`.
         """
+        if isinstance(value, str):
+            try:
+                if ':' in value:
+                    value = IPv6Network(value)
+                else:
+                    value = IPv4Network(value)
+            except Exception as ex:
+                raise IptablesError(
+                    f"{value} cannot be parsed as IPv4/IPv6 address") from ex
+        elif isinstance(value, IPv4Address):
+            value = IPv4Network(value)
+        elif isinstance(value, IPv6Address):
+            value = IPv6Network(value)
         if isinstance(value, IPv4Network):
             if self.__ipv6 is not None:
                 if self.__ipv6:
                     raise IptablesError(
                         f"criterion expects IPv6 address (got {value}")
             else:
                 self.__ipv6 = False
```

### Comparing `linuxnet-iptables-7.0.0/linuxnet/iptables/matches/packettypematch.py` & `linuxnet-iptables-7.0.3/linuxnet/iptables/matches/packettypematch.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-7.0.0/linuxnet/iptables/matches/recentmatch.py` & `linuxnet-iptables-7.0.3/linuxnet/iptables/matches/recentmatch.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-7.0.0/linuxnet/iptables/matches/setmatch.py` & `linuxnet-iptables-7.0.3/linuxnet/iptables/matches/setmatch.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-7.0.0/linuxnet/iptables/matches/statematch.py` & `linuxnet-iptables-7.0.3/linuxnet/iptables/matches/statematch.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-7.0.0/linuxnet/iptables/matches/statisticmatch.py` & `linuxnet-iptables-7.0.3/linuxnet/iptables/matches/statisticmatch.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-7.0.0/linuxnet/iptables/matches/tcpmatch.py` & `linuxnet-iptables-7.0.3/linuxnet/iptables/matches/tcpmatch.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-7.0.0/linuxnet/iptables/matches/tcpmssmatch.py` & `linuxnet-iptables-7.0.3/linuxnet/iptables/matches/tcpmssmatch.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-7.0.0/linuxnet/iptables/matches/ttlmatch.py` & `linuxnet-iptables-7.0.3/linuxnet/iptables/matches/ttlmatch.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-7.0.0/linuxnet/iptables/matches/udpmatch.py` & `linuxnet-iptables-7.0.3/linuxnet/iptables/matches/udpmatch.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-7.0.0/linuxnet/iptables/matches/util.py` & `linuxnet-iptables-7.0.3/linuxnet/iptables/matches/util.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-7.0.0/linuxnet/iptables/metadata.py` & `linuxnet-iptables-7.0.3/linuxnet/iptables/metadata.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,10 +18,10 @@
 """
 Metadata information intended to be used by setup.py and the
 Sphinx conf.py
 """
 
 # pylint: disable=invalid-name
 
-_version_ = "7.0.0"
+_version_ = "7.0.3"
 _author_ = "Panagiotis (Panos) Tsirigotis"
 _package_ = "linuxnet.iptables"
```

### Comparing `linuxnet-iptables-7.0.0/linuxnet/iptables/parsing.py` & `linuxnet-iptables-7.0.3/linuxnet/iptables/parsing.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-7.0.0/linuxnet/iptables/rule.py` & `linuxnet-iptables-7.0.3/linuxnet/iptables/rule.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-7.0.0/linuxnet/iptables/table.py` & `linuxnet-iptables-7.0.3/linuxnet/iptables/table.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-7.0.0/linuxnet/iptables/targets/__init__.py` & `linuxnet-iptables-7.0.3/linuxnet/iptables/targets/__init__.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-7.0.0/linuxnet/iptables/targets/connmarktarget.py` & `linuxnet-iptables-7.0.3/linuxnet/iptables/targets/connmarktarget.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-7.0.0/linuxnet/iptables/targets/logtarget.py` & `linuxnet-iptables-7.0.3/linuxnet/iptables/targets/logtarget.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-7.0.0/linuxnet/iptables/targets/marktarget.py` & `linuxnet-iptables-7.0.3/linuxnet/iptables/targets/marktarget.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-7.0.0/linuxnet/iptables/targets/masqueradetarget.py` & `linuxnet-iptables-7.0.3/linuxnet/iptables/targets/masqueradetarget.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-7.0.0/linuxnet/iptables/targets/nattarget.py` & `linuxnet-iptables-7.0.3/linuxnet/iptables/targets/nattarget.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-7.0.0/linuxnet/iptables/targets/notracktarget.py` & `linuxnet-iptables-7.0.3/linuxnet/iptables/targets/notracktarget.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-7.0.0/linuxnet/iptables/targets/rejecttarget.py` & `linuxnet-iptables-7.0.3/linuxnet/iptables/targets/rejecttarget.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-7.0.0/linuxnet/iptables/targets/target.py` & `linuxnet-iptables-7.0.3/linuxnet/iptables/targets/target.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-7.0.0/linuxnet/iptables/targets/tracetarget.py` & `linuxnet-iptables-7.0.3/linuxnet/iptables/targets/tracetarget.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-7.0.0/linuxnet/iptables/targets/ttltarget.py` & `linuxnet-iptables-7.0.3/linuxnet/iptables/targets/ttltarget.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-7.0.0/linuxnet_iptables.egg-info/PKG-INFO` & `linuxnet-iptables-7.0.3/linuxnet_iptables.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linuxnet-iptables
-Version: 7.0.0
+Version: 7.0.3
 Summary: programmatic access to Linux iptables
 Home-page: https://gitlab.com/panos-tools/linuxnet-iptables
 Author: Panagiotis (Panos) Tsirigotis
 Author-email: ptsirigotis01@gmail.com
 License: AGPLv3
 Project-URL: Source, https://gitlab.com/panos-tools/linuxnet-iptables
 Project-URL: Documentation, https://linuxnet-iptables.readthedocs.io/en/latest/index.html
@@ -18,15 +18,15 @@
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # linuxnet-iptables
 
 **linuxnet-iptables** provides programmatic access to the
-Linux `iptables(8)` command.
+Linux `iptables(8)` (or `ip6tables(8)`) command.
 Using **linuxnet-iptables** one can view existing chains/rules,
 create new ones, or delete existing ones.
 The package documentation is available
 [here](https://linuxnet-iptables.readthedocs.io/en/latest/index.html).
 
 For the following examples, Python3 (3.6 or later) is required.
```

### Comparing `linuxnet-iptables-7.0.0/linuxnet_iptables.egg-info/SOURCES.txt` & `linuxnet-iptables-7.0.3/linuxnet_iptables.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-7.0.0/setup.py` & `linuxnet-iptables-7.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-7.0.0/tests/iptables_test.py` & `linuxnet-iptables-7.0.3/tests/iptables_test.py`

 * *Files identical despite different names*

