# Comparing `tmp/evennia-4.1.0.tar.gz` & `tmp/evennia-4.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evennia-4.1.0.tar", last modified: Mon Apr  1 18:37:21 2024, max compression
+gzip compressed data, was "evennia-4.1.1.tar", last modified: Sat Apr  6 21:07:27 2024, max compression
```

## Comparing `evennia-4.1.0.tar` & `evennia-4.1.1.tar`

### file list

```diff
@@ -1,988 +1,988 @@
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.223504 evennia-4.1.0/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1531 2024-03-17 13:16:36.000000 evennia-4.1.0/LICENSE.txt
--rw-r--r--   0 griatch   (1000) griatch   (1000)     6510 2024-04-01 18:37:21.223504 evennia-4.1.0/PKG-INFO
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3034 2024-03-17 13:16:36.000000 evennia-4.1.0/README.md
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.175504 evennia-4.1.0/bin/
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.183504 evennia-4.1.0/bin/unix/
--rwxrwxr-x   0 griatch   (1000) griatch   (1000)      210 2024-03-17 13:16:36.000000 evennia-4.1.0/bin/unix/evennia
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.183504 evennia-4.1.0/evennia/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        6 2024-04-01 18:25:42.000000 evennia-4.1.0/evennia/VERSION.txt
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      437 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/VERSION_REQS.txt
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    15076 2024-04-01 15:48:28.000000 evennia-4.1.0/evennia/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1839 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/__main__.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.183504 evennia-4.1.0/evennia/accounts/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      214 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/accounts/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    74120 2024-04-01 15:48:32.000000 evennia-4.1.0/evennia/accounts/accounts.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    26930 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/accounts/bots.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     9574 2024-04-01 15:48:32.000000 evennia-4.1.0/evennia/accounts/manager.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.183504 evennia-4.1.0/evennia/accounts/migrations/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     7211 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/accounts/migrations/0001_initial.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      504 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/accounts/migrations/0002_move_defaults.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      612 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/accounts/migrations/0003_auto_20150209_2234.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2158 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/accounts/migrations/0004_auto_20150403_2339.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1010 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/accounts/migrations/0005_auto_20160905_0902.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1488 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/accounts/migrations/0006_auto_20170606_1731.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1927 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/accounts/migrations/0007_copy_player_to_account.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3944 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/accounts/migrations/0008_auto_20190128_1820.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      867 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/accounts/migrations/0009_auto_20191025_0831.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      467 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/accounts/migrations/0010_auto_20210520_2137.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4017 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/accounts/migrations/0011_convert_contrib_typeclass_paths.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      490 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/accounts/migrations/0012_defaultaccount_alter_accountdb_id_account_bot_and_more.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       24 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/accounts/migrations/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     5741 2024-04-01 15:48:28.000000 evennia-4.1.0/evennia/accounts/models.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    17496 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/accounts/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.183504 evennia-4.1.0/evennia/commands/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      304 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/commands/__init__.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.183504 evennia-4.1.0/evennia/commands/_trial_temp/
--rwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/commands/_trial_temp/_trial_marker
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    31495 2024-04-01 15:48:32.000000 evennia-4.1.0/evennia/commands/cmdhandler.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     8286 2024-04-01 15:48:28.000000 evennia-4.1.0/evennia/commands/cmdparser.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    27313 2024-04-01 15:48:28.000000 evennia-4.1.0/evennia/commands/cmdset.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    26152 2024-04-01 15:48:28.000000 evennia-4.1.0/evennia/commands/cmdsethandler.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    29047 2024-04-01 15:48:32.000000 evennia-4.1.0/evennia/commands/command.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.183504 evennia-4.1.0/evennia/commands/default/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       87 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/commands/default/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    35296 2024-04-01 15:48:28.000000 evennia-4.1.0/evennia/commands/default/account.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    19512 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/commands/default/admin.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    22983 2024-04-01 15:48:28.000000 evennia-4.1.0/evennia/commands/default/batchprocess.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)   172644 2024-04-01 15:48:32.000000 evennia-4.1.0/evennia/commands/default/building.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2358 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/commands/default/cmdset_account.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3033 2024-04-01 15:48:28.000000 evennia-4.1.0/evennia/commands/default/cmdset_character.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      372 2024-04-01 15:48:28.000000 evennia-4.1.0/evennia/commands/default/cmdset_session.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      873 2024-04-01 15:48:28.000000 evennia-4.1.0/evennia/commands/default/cmdset_unloggedin.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    77528 2024-04-01 15:48:32.000000 evennia-4.1.0/evennia/commands/default/comms.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    25743 2024-04-01 18:23:38.000000 evennia-4.1.0/evennia/commands/default/general.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    40503 2024-03-30 15:40:53.000000 evennia-4.1.0/evennia/commands/default/help.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    12774 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/commands/default/muxcommand.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3152 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/commands/default/syscommands.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    42139 2024-04-01 15:48:28.000000 evennia-4.1.0/evennia/commands/default/system.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    84255 2024-04-01 18:13:45.000000 evennia-4.1.0/evennia/commands/default/tests.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    15024 2024-04-01 15:48:28.000000 evennia-4.1.0/evennia/commands/default/unloggedin.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    47839 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/commands/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.183504 evennia-4.1.0/evennia/comms/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      207 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/comms/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    32603 2024-04-01 15:48:28.000000 evennia-4.1.0/evennia/comms/comms.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    16863 2024-04-01 15:48:28.000000 evennia-4.1.0/evennia/comms/managers.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.187504 evennia-4.1.0/evennia/comms/migrations/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3523 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/comms/migrations/0001_initial.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      500 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/comms/migrations/0002_msg_db_hide_from_objects.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3784 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/comms/migrations/0003_auto_20140917_0756.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      504 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/comms/migrations/0004_auto_20150118_1631.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      641 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/comms/migrations/0005_auto_20150223_1517.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      643 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/comms/migrations/0006_channeldb_db_object_subscriptions.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      615 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/comms/migrations/0007_msg_db_tags.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      434 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/comms/migrations/0008_auto_20160905_0902.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3872 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/comms/migrations/0009_auto_20160921_1731.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1079 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/comms/migrations/0010_auto_20161206_1912.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1029 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/comms/migrations/0011_auto_20170217_2039.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4563 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/comms/migrations/0011_auto_20170606_1731.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      267 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/comms/migrations/0012_merge_20170617_2017.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4778 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/comms/migrations/0013_auto_20170705_1726.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1442 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/comms/migrations/0014_auto_20170705_1736.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      943 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/comms/migrations/0015_auto_20170706_2041.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      462 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/comms/migrations/0016_auto_20180925_1735.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     7069 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/comms/migrations/0017_auto_20190128_1820.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      665 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/comms/migrations/0018_auto_20191025_0831.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1713 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/comms/migrations/0019_auto_20210514_2032.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      916 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/comms/migrations/0020_auto_20210514_2210.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3635 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/comms/migrations/0021_auto_20210520_2137.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      711 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/comms/migrations/0022_defaultchannel_alter_channeldb_id_alter_msg_id_and_more.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       24 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/comms/migrations/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    22647 2024-04-01 15:48:28.000000 evennia-4.1.0/evennia/comms/models.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3166 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/comms/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.187504 evennia-4.1.0/evennia/contrib/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1895 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      198 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/__init__.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.187504 evennia-4.1.0/evennia/contrib/base_systems/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       80 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/base_systems/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/base_systems/__init__.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.187504 evennia-4.1.0/evennia/contrib/base_systems/awsstorage/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     7695 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/base_systems/awsstorage/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       48 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/base_systems/awsstorage/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    32479 2024-04-01 15:48:28.000000 evennia-4.1.0/evennia/contrib/base_systems/awsstorage/aws_s3_cdn.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    22503 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/base_systems/awsstorage/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.187504 evennia-4.1.0/evennia/contrib/base_systems/building_menu/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    46012 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/base_systems/building_menu/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      149 2024-04-01 15:48:28.000000 evennia-4.1.0/evennia/contrib/base_systems/building_menu/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    42684 2024-04-01 15:48:28.000000 evennia-4.1.0/evennia/contrib/base_systems/building_menu/building_menu.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     6879 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/base_systems/building_menu/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.187504 evennia-4.1.0/evennia/contrib/base_systems/color_markups/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2641 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/base_systems/color_markups/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       84 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/base_systems/color_markups/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     8605 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/base_systems/color_markups/color_markups.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3356 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/base_systems/color_markups/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.187504 evennia-4.1.0/evennia/contrib/base_systems/components/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     6914 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/base_systems/components/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      514 2024-04-01 15:48:28.000000 evennia-4.1.0/evennia/contrib/base_systems/components/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4638 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/base_systems/components/component.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     5162 2024-04-01 15:48:28.000000 evennia-4.1.0/evennia/contrib/base_systems/components/dbfield.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      157 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/base_systems/components/exceptions.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    10305 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/base_systems/components/holder.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      540 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/base_systems/components/listing.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     7516 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/base_systems/components/signals.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    17207 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/base_systems/components/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.187504 evennia-4.1.0/evennia/contrib/base_systems/custom_gametime/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1549 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/base_systems/custom_gametime/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      439 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/base_systems/custom_gametime/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    10389 2024-04-01 15:48:28.000000 evennia-4.1.0/evennia/contrib/base_systems/custom_gametime/custom_gametime.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2017 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/base_systems/custom_gametime/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.187504 evennia-4.1.0/evennia/contrib/base_systems/email_login/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1022 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/base_systems/email_login/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      136 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/base_systems/email_login/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1445 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/base_systems/email_login/connection_screens.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    10573 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/base_systems/email_login/email_login.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1200 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/base_systems/email_login/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.187504 evennia-4.1.0/evennia/contrib/base_systems/godotwebsocket/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     6041 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/base_systems/godotwebsocket/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      704 2024-04-01 15:48:28.000000 evennia-4.1.0/evennia/contrib/base_systems/godotwebsocket/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3074 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/base_systems/godotwebsocket/test_text2bbcode.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3186 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/base_systems/godotwebsocket/test_webclient.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    27603 2024-04-01 15:48:28.000000 evennia-4.1.0/evennia/contrib/base_systems/godotwebsocket/text2bbcode.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2683 2024-04-01 15:48:28.000000 evennia-4.1.0/evennia/contrib/base_systems/godotwebsocket/webclient.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.187504 evennia-4.1.0/evennia/contrib/base_systems/ingame_python/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    40300 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/base_systems/ingame_python/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      128 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/base_systems/ingame_python/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     6776 2024-04-01 15:48:28.000000 evennia-4.1.0/evennia/contrib/base_systems/ingame_python/callbackhandler.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    21871 2024-04-01 15:48:28.000000 evennia-4.1.0/evennia/contrib/base_systems/ingame_python/commands.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3048 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/base_systems/ingame_python/eventfuncs.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    23988 2024-04-01 15:48:28.000000 evennia-4.1.0/evennia/contrib/base_systems/ingame_python/scripts.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    21615 2024-04-01 15:48:29.000000 evennia-4.1.0/evennia/contrib/base_systems/ingame_python/tests.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    34959 2024-04-01 15:48:28.000000 evennia-4.1.0/evennia/contrib/base_systems/ingame_python/typeclasses.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     8150 2024-04-01 15:48:28.000000 evennia-4.1.0/evennia/contrib/base_systems/ingame_python/utils.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.187504 evennia-4.1.0/evennia/contrib/base_systems/menu_login/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      787 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/base_systems/menu_login/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      143 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/base_systems/menu_login/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1206 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/base_systems/menu_login/connection_screens.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     8937 2024-04-01 15:48:31.000000 evennia-4.1.0/evennia/contrib/base_systems/menu_login/menu_login.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      265 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/base_systems/menu_login/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.187504 evennia-4.1.0/evennia/contrib/base_systems/mux_comms_cmds/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1936 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/base_systems/mux_comms_cmds/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      104 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/base_systems/mux_comms_cmds/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    16013 2024-04-01 15:48:28.000000 evennia-4.1.0/evennia/contrib/base_systems/mux_comms_cmds/mux_comms_cmds.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2298 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/base_systems/mux_comms_cmds/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.187504 evennia-4.1.0/evennia/contrib/base_systems/unixcommand/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2241 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/base_systems/unixcommand/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       94 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/base_systems/unixcommand/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1653 2024-04-01 15:48:28.000000 evennia-4.1.0/evennia/contrib/base_systems/unixcommand/tests.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     9986 2024-04-01 15:48:28.000000 evennia-4.1.0/evennia/contrib/base_systems/unixcommand/unixcommand.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.191504 evennia-4.1.0/evennia/contrib/full_systems/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       75 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/full_systems/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       48 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/full_systems/__init__.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.191504 evennia-4.1.0/evennia/contrib/full_systems/evscaperoom/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     5210 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/full_systems/evscaperoom/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      266 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/full_systems/evscaperoom/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    22694 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/full_systems/evscaperoom/commands.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    10561 2024-04-01 15:48:28.000000 evennia-4.1.0/evennia/contrib/full_systems/evscaperoom/menu.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    34345 2024-04-01 15:48:29.000000 evennia-4.1.0/evennia/contrib/full_systems/evscaperoom/objects.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     7942 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/full_systems/evscaperoom/room.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      751 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/full_systems/evscaperoom/scripts.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     9582 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/full_systems/evscaperoom/state.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.191504 evennia-4.1.0/evennia/contrib/full_systems/evscaperoom/states/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1203 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/full_systems/evscaperoom/states/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4168 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/full_systems/evscaperoom/states/state_001_start.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    10421 2024-04-01 15:48:28.000000 evennia-4.1.0/evennia/contrib/full_systems/evscaperoom/tests.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     6112 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/full_systems/evscaperoom/utils.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.191504 evennia-4.1.0/evennia/contrib/game_systems/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      269 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/game_systems/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/game_systems/__init__.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.191504 evennia-4.1.0/evennia/contrib/game_systems/barter/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4322 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/game_systems/barter/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       80 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/game_systems/barter/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    29726 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/game_systems/barter/barter.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     5976 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/game_systems/barter/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.191504 evennia-4.1.0/evennia/contrib/game_systems/clothing/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4256 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/game_systems/clothing/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      199 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/game_systems/clothing/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    24856 2024-04-01 15:48:31.000000 evennia-4.1.0/evennia/contrib/game_systems/clothing/clothing.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     6344 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/game_systems/clothing/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.191504 evennia-4.1.0/evennia/contrib/game_systems/containers/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2508 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/game_systems/containers/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       66 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/game_systems/containers/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    10016 2024-04-01 15:48:28.000000 evennia-4.1.0/evennia/contrib/game_systems/containers/containers.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2851 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/game_systems/containers/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.191504 evennia-4.1.0/evennia/contrib/game_systems/cooldowns/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2084 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/game_systems/cooldowns/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       88 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/game_systems/cooldowns/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     7580 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/game_systems/cooldowns/cooldowns.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     6135 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/game_systems/cooldowns/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.191504 evennia-4.1.0/evennia/contrib/game_systems/crafting/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    11186 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/game_systems/crafting/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      233 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/game_systems/crafting/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    41698 2024-04-01 15:48:29.000000 evennia-4.1.0/evennia/contrib/game_systems/crafting/crafting.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    17891 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/game_systems/crafting/example_recipes.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    25314 2024-03-30 22:45:30.000000 evennia-4.1.0/evennia/contrib/game_systems/crafting/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.191504 evennia-4.1.0/evennia/contrib/game_systems/gendersub/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1986 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/game_systems/gendersub/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      123 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/game_systems/gendersub/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     5326 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/game_systems/gendersub/gendersub.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2351 2024-04-01 15:48:28.000000 evennia-4.1.0/evennia/contrib/game_systems/gendersub/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.191504 evennia-4.1.0/evennia/contrib/game_systems/mail/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1567 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/game_systems/mail/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      115 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/game_systems/mail/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    14841 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/game_systems/mail/mail.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1852 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/game_systems/mail/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.191504 evennia-4.1.0/evennia/contrib/game_systems/multidescer/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3228 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/game_systems/multidescer/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       83 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/game_systems/multidescer/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     9952 2024-04-01 15:48:29.000000 evennia-4.1.0/evennia/contrib/game_systems/multidescer/multidescer.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1404 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/game_systems/multidescer/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.191504 evennia-4.1.0/evennia/contrib/game_systems/puzzles/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2181 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/game_systems/puzzles/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      124 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/game_systems/puzzles/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    27836 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/game_systems/puzzles/puzzles.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    41327 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/game_systems/puzzles/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.191504 evennia-4.1.0/evennia/contrib/game_systems/turnbattle/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2940 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/game_systems/turnbattle/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      209 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/game_systems/turnbattle/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    28762 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/game_systems/turnbattle/tb_basic.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    23139 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/game_systems/turnbattle/tb_equip.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    37445 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/game_systems/turnbattle/tb_items.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    30705 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/game_systems/turnbattle/tb_magic.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    38339 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/game_systems/turnbattle/tb_range.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    29680 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/game_systems/turnbattle/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.191504 evennia-4.1.0/evennia/contrib/grid/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       84 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/grid/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       81 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/grid/__init__.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.191504 evennia-4.1.0/evennia/contrib/grid/extended_room/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     6358 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/grid/extended_room/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      454 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/grid/extended_room/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    34233 2024-04-01 15:48:31.000000 evennia-4.1.0/evennia/contrib/grid/extended_room/extended_room.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    12949 2024-04-01 15:48:31.000000 evennia-4.1.0/evennia/contrib/grid/extended_room/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.191504 evennia-4.1.0/evennia/contrib/grid/ingame_map_display/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1358 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/grid/ingame_map_display/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       92 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/grid/ingame_map_display/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    10573 2024-04-01 15:48:29.000000 evennia-4.1.0/evennia/contrib/grid/ingame_map_display/ingame_map_display.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1403 2024-04-01 15:48:28.000000 evennia-4.1.0/evennia/contrib/grid/ingame_map_display/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.191504 evennia-4.1.0/evennia/contrib/grid/mapbuilder/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     9672 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/grid/mapbuilder/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       87 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/grid/mapbuilder/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    17398 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/grid/mapbuilder/mapbuilder.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     6435 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/grid/mapbuilder/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.191504 evennia-4.1.0/evennia/contrib/grid/simpledoor/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1356 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/grid/simpledoor/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      129 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/grid/simpledoor/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     5838 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/grid/simpledoor/simpledoor.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1078 2024-04-01 15:48:28.000000 evennia-4.1.0/evennia/contrib/grid/simpledoor/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.191504 evennia-4.1.0/evennia/contrib/grid/slow_exit/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1730 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/grid/slow_exit/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      203 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/grid/slow_exit/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     5046 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/grid/slow_exit/slow_exit.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      824 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/grid/slow_exit/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.191504 evennia-4.1.0/evennia/contrib/grid/wilderness/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4932 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/grid/wilderness/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      394 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/grid/wilderness/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     6226 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/grid/wilderness/tests.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    27385 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/grid/wilderness/wilderness.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.195504 evennia-4.1.0/evennia/contrib/grid/xyzgrid/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    54837 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/grid/xyzgrid/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      244 2024-04-01 15:48:28.000000 evennia-4.1.0/evennia/contrib/grid/xyzgrid/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    20845 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/grid/xyzgrid/commands.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     7823 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/grid/xyzgrid/example.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    13700 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/grid/xyzgrid/launchcmd.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1146 2024-04-01 15:48:28.000000 evennia-4.1.0/evennia/contrib/grid/xyzgrid/prototypes.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    42076 2024-04-01 15:48:31.000000 evennia-4.1.0/evennia/contrib/grid/xyzgrid/tests.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1043 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/grid/xyzgrid/utils.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    40422 2024-04-01 15:48:31.000000 evennia-4.1.0/evennia/contrib/grid/xyzgrid/xymap.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    52059 2024-04-01 15:48:31.000000 evennia-4.1.0/evennia/contrib/grid/xyzgrid/xymap_legend.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    10484 2024-04-01 15:48:29.000000 evennia-4.1.0/evennia/contrib/grid/xyzgrid/xyzgrid.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    24732 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/grid/xyzgrid/xyzroom.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.195504 evennia-4.1.0/evennia/contrib/rpg/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      406 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/rpg/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/rpg/__init__.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.195504 evennia-4.1.0/evennia/contrib/rpg/buffs/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    22364 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/rpg/buffs/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      210 2024-04-01 15:48:31.000000 evennia-4.1.0/evennia/contrib/rpg/buffs/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    45719 2024-04-01 15:48:29.000000 evennia-4.1.0/evennia/contrib/rpg/buffs/buff.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3893 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/rpg/buffs/samplebuffs.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    16471 2024-04-01 15:48:29.000000 evennia-4.1.0/evennia/contrib/rpg/buffs/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.195504 evennia-4.1.0/evennia/contrib/rpg/character_creator/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3922 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/rpg/character_creator/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      176 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/rpg/character_creator/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     7448 2024-04-01 15:48:29.000000 evennia-4.1.0/evennia/contrib/rpg/character_creator/character_creator.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    21006 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/rpg/character_creator/example_menu.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1809 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/rpg/character_creator/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.195504 evennia-4.1.0/evennia/contrib/rpg/dice/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3812 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/rpg/dice/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      177 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/rpg/dice/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    12730 2024-04-01 15:48:29.000000 evennia-4.1.0/evennia/contrib/rpg/dice/dice.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1442 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/rpg/dice/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.195504 evennia-4.1.0/evennia/contrib/rpg/health_bar/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1264 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/rpg/health_bar/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       94 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/rpg/health_bar/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4913 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/rpg/health_bar/health_bar.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1634 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/rpg/health_bar/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.195504 evennia-4.1.0/evennia/contrib/rpg/llm/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    15039 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/rpg/llm/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       90 2024-03-24 16:21:41.000000 evennia-4.1.0/evennia/contrib/rpg/llm/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     5986 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/rpg/llm/llm_client.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     7444 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/rpg/llm/llm_npc.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1185 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/rpg/llm/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.195504 evennia-4.1.0/evennia/contrib/rpg/rpsystem/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    10331 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/rpg/rpsystem/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      793 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/rpg/rpsystem/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    24723 2024-04-01 15:48:29.000000 evennia-4.1.0/evennia/contrib/rpg/rpsystem/rplanguage.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    59481 2024-04-01 15:48:31.000000 evennia-4.1.0/evennia/contrib/rpg/rpsystem/rpsystem.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    17394 2024-04-01 15:48:31.000000 evennia-4.1.0/evennia/contrib/rpg/rpsystem/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.195504 evennia-4.1.0/evennia/contrib/rpg/traits/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    14247 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/rpg/traits/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      294 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/rpg/traits/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    37184 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/rpg/traits/tests.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    54514 2024-04-01 15:48:29.000000 evennia-4.1.0/evennia/contrib/rpg/traits/traits.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.195504 evennia-4.1.0/evennia/contrib/tutorials/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      151 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/tutorials/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       81 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/tutorials/__init__.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.195504 evennia-4.1.0/evennia/contrib/tutorials/batchprocessor/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1623 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/tutorials/batchprocessor/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       50 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/tutorials/batchprocessor/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1567 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/tutorials/batchprocessor/example_batch_cmds.ev
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      942 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/tutorials/batchprocessor/example_batch_cmds_test.ev
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3618 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/tutorials/batchprocessor/example_batch_code.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.195504 evennia-4.1.0/evennia/contrib/tutorials/bodyfunctions/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      471 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/tutorials/bodyfunctions/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      104 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/tutorials/bodyfunctions/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2312 2024-04-01 15:48:29.000000 evennia-4.1.0/evennia/contrib/tutorials/bodyfunctions/bodyfunctions.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3325 2024-04-01 15:48:29.000000 evennia-4.1.0/evennia/contrib/tutorials/bodyfunctions/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.195504 evennia-4.1.0/evennia/contrib/tutorials/evadventure/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1180 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/tutorials/evadventure/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      164 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/tutorials/evadventure/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3758 2024-04-01 15:48:29.000000 evennia-4.1.0/evennia/contrib/tutorials/evadventure/ai.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.195504 evennia-4.1.0/evennia/contrib/tutorials/evadventure/batchscripts/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       73 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/tutorials/evadventure/batchscripts/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1819 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/tutorials/evadventure/batchscripts/turnbased_combat_demo.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1436 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/tutorials/evadventure/batchscripts/twitch_combat_demo.ev
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3996 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/tutorials/evadventure/build_techdemo.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/tutorials/evadventure/build_world.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    12610 2024-03-30 20:22:07.000000 evennia-4.1.0/evennia/contrib/tutorials/evadventure/characters.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    11181 2024-04-01 15:48:29.000000 evennia-4.1.0/evennia/contrib/tutorials/evadventure/chargen.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    16990 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/tutorials/evadventure/combat_base.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    27740 2024-04-01 15:48:29.000000 evennia-4.1.0/evennia/contrib/tutorials/evadventure/combat_turnbased.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    18271 2024-04-01 15:48:31.000000 evennia-4.1.0/evennia/contrib/tutorials/evadventure/combat_twitch.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    12500 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/tutorials/evadventure/commands.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    17570 2024-04-01 15:48:29.000000 evennia-4.1.0/evennia/contrib/tutorials/evadventure/dungeon.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1743 2024-04-01 15:48:29.000000 evennia-4.1.0/evennia/contrib/tutorials/evadventure/enums.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    14537 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/tutorials/evadventure/equipment.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    12402 2024-04-01 15:48:29.000000 evennia-4.1.0/evennia/contrib/tutorials/evadventure/npcs.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    11174 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/tutorials/evadventure/objects.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    11184 2024-04-01 15:48:29.000000 evennia-4.1.0/evennia/contrib/tutorials/evadventure/quests.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    11708 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/tutorials/evadventure/random_tables.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3154 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/tutorials/evadventure/rooms.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    12130 2024-04-01 15:48:29.000000 evennia-4.1.0/evennia/contrib/tutorials/evadventure/rules.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    17153 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/tutorials/evadventure/shops.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.199504 evennia-4.1.0/evennia/contrib/tutorials/evadventure/tests/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       48 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/tutorials/evadventure/tests/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1389 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/tutorials/evadventure/tests/mixins.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1664 2024-04-01 15:48:29.000000 evennia-4.1.0/evennia/contrib/tutorials/evadventure/tests/test_ai.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1266 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/tutorials/evadventure/tests/test_characters.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2150 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/tutorials/evadventure/tests/test_chargen.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    28160 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/tutorials/evadventure/tests/test_combat.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3742 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/tutorials/evadventure/tests/test_commands.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3322 2024-03-24 14:40:20.000000 evennia-4.1.0/evennia/contrib/tutorials/evadventure/tests/test_dungeon.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     7810 2024-04-01 15:48:29.000000 evennia-4.1.0/evennia/contrib/tutorials/evadventure/tests/test_equipment.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      542 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/tutorials/evadventure/tests/test_npcs.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4159 2024-03-30 22:04:09.000000 evennia-4.1.0/evennia/contrib/tutorials/evadventure/tests/test_quests.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2237 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/tutorials/evadventure/tests/test_rooms.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     8083 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/tutorials/evadventure/tests/test_rules.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      711 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/tutorials/evadventure/tests/test_utils.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2237 2024-04-01 15:48:29.000000 evennia-4.1.0/evennia/contrib/tutorials/evadventure/utils.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.199504 evennia-4.1.0/evennia/contrib/tutorials/mirror/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      429 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/tutorials/mirror/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       83 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/tutorials/mirror/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2235 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/tutorials/mirror/mirror.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.199504 evennia-4.1.0/evennia/contrib/tutorials/red_button/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1344 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/tutorials/red_button/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       94 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/tutorials/red_button/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    18610 2024-04-01 15:48:29.000000 evennia-4.1.0/evennia/contrib/tutorials/red_button/red_button.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.199504 evennia-4.1.0/evennia/contrib/tutorials/talking_npc/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      722 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/tutorials/talking_npc/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      124 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/tutorials/talking_npc/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3697 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/tutorials/talking_npc/talking_npc.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      450 2024-04-01 15:48:29.000000 evennia-4.1.0/evennia/contrib/tutorials/talking_npc/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.199504 evennia-4.1.0/evennia/contrib/tutorials/tutorial_world/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4302 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/tutorials/tutorial_world/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      125 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/tutorials/tutorial_world/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    50297 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/tutorials/tutorial_world/build.ev
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    25399 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/tutorials/tutorial_world/intro_menu.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    16130 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/tutorials/tutorial_world/mob.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    42155 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/tutorials/tutorial_world/objects.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    42921 2024-04-01 15:48:29.000000 evennia-4.1.0/evennia/contrib/tutorials/tutorial_world/rooms.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     7522 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/tutorials/tutorial_world/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.199504 evennia-4.1.0/evennia/contrib/utils/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       67 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/utils/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/utils/__init__.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.199504 evennia-4.1.0/evennia/contrib/utils/auditing/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3303 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/utils/auditing/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/utils/auditing/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2066 2024-04-01 15:48:29.000000 evennia-4.1.0/evennia/contrib/utils/auditing/outputs.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     8516 2024-04-01 15:48:29.000000 evennia-4.1.0/evennia/contrib/utils/auditing/server.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     6047 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/utils/auditing/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.199504 evennia-4.1.0/evennia/contrib/utils/fieldfill/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     5816 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/utils/fieldfill/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      288 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/utils/fieldfill/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    26383 2024-04-01 15:48:29.000000 evennia-4.1.0/evennia/contrib/utils/fieldfill/fieldfill.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.199504 evennia-4.1.0/evennia/contrib/utils/git_integration/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3139 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/utils/git_integration/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       86 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/utils/git_integration/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     7737 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/utils/git_integration/git_integration.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2828 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/utils/git_integration/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.199504 evennia-4.1.0/evennia/contrib/utils/name_generator/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     9815 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/utils/name_generator/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/utils/name_generator/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)   232619 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/utils/name_generator/btn_givennames.txt
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    56503 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/utils/name_generator/btn_surnames.txt
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    14447 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/utils/name_generator/namegen.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4914 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/utils/name_generator/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.199504 evennia-4.1.0/evennia/contrib/utils/random_string_generator/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2165 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/utils/random_string_generator/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      268 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/utils/random_string_generator/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    12591 2024-04-01 15:48:29.000000 evennia-4.1.0/evennia/contrib/utils/random_string_generator/random_string_generator.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      737 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/utils/random_string_generator/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.199504 evennia-4.1.0/evennia/contrib/utils/tree_select/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     5935 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/utils/tree_select/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      109 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/utils/tree_select/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2199 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/utils/tree_select/tests.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    20930 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/contrib/utils/tree_select/tree_select.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.199504 evennia-4.1.0/evennia/game_template/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1521 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/game_template/README.md
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.199504 evennia-4.1.0/evennia/game_template/commands/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      676 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/game_template/commands/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/game_template/commands/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     7738 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/game_template/commands/command.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2636 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/game_template/commands/default_cmdsets.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      576 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/game_template/gitignore
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.199504 evennia-4.1.0/evennia/game_template/server/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1718 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/game_template/server/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       24 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/game_template/server/__init__.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.199504 evennia-4.1.0/evennia/game_template/server/conf/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       24 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/game_template/server/conf/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      629 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/game_template/server/conf/at_initial_setup.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2154 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/game_template/server/conf/at_search.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1369 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/game_template/server/conf/at_server_startstop.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2174 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/game_template/server/conf/cmdparser.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1500 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/game_template/server/conf/connection_screens.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1159 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/game_template/server/conf/inlinefuncs.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1419 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/game_template/server/conf/inputfuncs.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1065 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/game_template/server/conf/lockfuncs.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3979 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/game_template/server/conf/mssp.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      709 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/game_template/server/conf/portal_services_plugins.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      714 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/game_template/server/conf/secret_settings.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      705 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/game_template/server/conf/server_services_plugins.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1347 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/game_template/server/conf/serversession.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1545 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/game_template/server/conf/settings.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1185 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/game_template/server/conf/web_plugins.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.199504 evennia-4.1.0/evennia/game_template/server/logs/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      839 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/game_template/server/logs/README.md
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.203504 evennia-4.1.0/evennia/game_template/typeclasses/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      733 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/game_template/typeclasses/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/game_template/typeclasses/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3774 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/game_template/typeclasses/accounts.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2920 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/game_template/typeclasses/channels.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1524 2024-04-01 15:48:29.000000 evennia-4.1.0/evennia/game_template/typeclasses/characters.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2045 2024-04-01 15:48:29.000000 evennia-4.1.0/evennia/game_template/typeclasses/exits.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     8848 2024-04-01 15:48:29.000000 evennia-4.1.0/evennia/game_template/typeclasses/objects.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      562 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/game_template/typeclasses/rooms.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4394 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/game_template/typeclasses/scripts.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.203504 evennia-4.1.0/evennia/game_template/web/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2939 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/game_template/web/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/game_template/web/__init__.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.203504 evennia-4.1.0/evennia/game_template/web/admin/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      296 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/game_template/web/admin/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/game_template/web/admin/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      519 2024-04-01 15:48:29.000000 evennia-4.1.0/evennia/game_template/web/admin/urls.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.203504 evennia-4.1.0/evennia/game_template/web/api/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/game_template/web/api/__init__.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.203504 evennia-4.1.0/evennia/game_template/web/static/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      849 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/game_template/web/static/README.md
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.179504 evennia-4.1.0/evennia/game_template/web/static/rest_framework/
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.203504 evennia-4.1.0/evennia/game_template/web/static/rest_framework/css/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       53 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/game_template/web/static/rest_framework/css/README.md
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.203504 evennia-4.1.0/evennia/game_template/web/static/rest_framework/images/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       47 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/game_template/web/static/rest_framework/images/README.md
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.179504 evennia-4.1.0/evennia/game_template/web/static/webclient/
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.203504 evennia-4.1.0/evennia/game_template/web/static/webclient/css/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      132 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/game_template/web/static/webclient/css/README.md
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.203504 evennia-4.1.0/evennia/game_template/web/static/webclient/js/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      143 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/game_template/web/static/webclient/js/README.md
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.179504 evennia-4.1.0/evennia/game_template/web/static/website/
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.203504 evennia-4.1.0/evennia/game_template/web/static/website/css/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      129 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/game_template/web/static/website/css/README.md
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.203504 evennia-4.1.0/evennia/game_template/web/static/website/images/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      135 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/game_template/web/static/website/images/README.md
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.203504 evennia-4.1.0/evennia/game_template/web/templates/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      760 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/game_template/web/templates/README.md
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.203504 evennia-4.1.0/evennia/game_template/web/templates/rest_framework/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       58 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/game_template/web/templates/rest_framework/README.md
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.203504 evennia-4.1.0/evennia/game_template/web/templates/webclient/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      223 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/game_template/web/templates/webclient/README.md
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.203504 evennia-4.1.0/evennia/game_template/web/templates/website/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      217 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/game_template/web/templates/website/README.md
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.203504 evennia-4.1.0/evennia/game_template/web/templates/website/flatpages/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      185 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/game_template/web/templates/website/flatpages/README.md
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.203504 evennia-4.1.0/evennia/game_template/web/templates/website/registration/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      152 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/game_template/web/templates/website/registration/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1100 2024-04-01 15:48:29.000000 evennia-4.1.0/evennia/game_template/web/urls.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.203504 evennia-4.1.0/evennia/game_template/web/webclient/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1102 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/game_template/web/webclient/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/game_template/web/webclient/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      539 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/game_template/web/webclient/urls.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.203504 evennia-4.1.0/evennia/game_template/web/website/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1262 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/game_template/web/website/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/game_template/web/website/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      509 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/game_template/web/website/urls.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.203504 evennia-4.1.0/evennia/game_template/web/website/views/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/game_template/web/website/views/__init__.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.203504 evennia-4.1.0/evennia/game_template/world/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      467 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/game_template/world/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/game_template/world/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      999 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/game_template/world/batch_cmds.ev
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1936 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/game_template/world/help_entries.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3646 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/game_template/world/prototypes.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.203504 evennia-4.1.0/evennia/help/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      217 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/help/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     8021 2024-03-30 14:56:23.000000 evennia-4.1.0/evennia/help/filehelp.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     6230 2024-04-01 15:48:29.000000 evennia-4.1.0/evennia/help/manager.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.203504 evennia-4.1.0/evennia/help/migrations/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2222 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/help/migrations/0001_initial.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      577 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/help/migrations/0002_auto_20170606_1731.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1688 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/help/migrations/0003_auto_20190128_1820.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      540 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/help/migrations/0004_auto_20210520_2137.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1166 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/help/migrations/0005_auto_20210530_1818.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      473 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/help/migrations/0006_alter_helpentry_id.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       24 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/help/migrations/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     9730 2024-04-01 15:48:29.000000 evennia-4.1.0/evennia/help/models.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3744 2024-03-30 14:56:23.000000 evennia-4.1.0/evennia/help/tests.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     7686 2024-04-01 15:48:29.000000 evennia-4.1.0/evennia/help/utils.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.203504 evennia-4.1.0/evennia/locale/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2686 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/locale/README
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.179504 evennia-4.1.0/evennia/locale/de/
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.203504 evennia-4.1.0/evennia/locale/de/LC_MESSAGES/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    10764 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/locale/de/LC_MESSAGES/django.mo
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    14475 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/locale/de/LC_MESSAGES/django.po
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.179504 evennia-4.1.0/evennia/locale/es/
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.203504 evennia-4.1.0/evennia/locale/es/LC_MESSAGES/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3821 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/locale/es/LC_MESSAGES/django.mo
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    30981 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/locale/es/LC_MESSAGES/django.po
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.179504 evennia-4.1.0/evennia/locale/fr/
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.203504 evennia-4.1.0/evennia/locale/fr/LC_MESSAGES/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    26255 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/locale/fr/LC_MESSAGES/django.mo
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    38581 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/locale/fr/LC_MESSAGES/django.po
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.179504 evennia-4.1.0/evennia/locale/it/
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.203504 evennia-4.1.0/evennia/locale/it/LC_MESSAGES/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     6944 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/locale/it/LC_MESSAGES/django.mo
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    35844 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/locale/it/LC_MESSAGES/django.po
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.179504 evennia-4.1.0/evennia/locale/ko/
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.203504 evennia-4.1.0/evennia/locale/ko/LC_MESSAGES/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3569 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/locale/ko/LC_MESSAGES/django.mo
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    30924 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/locale/ko/LC_MESSAGES/django.po
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.179504 evennia-4.1.0/evennia/locale/la/
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.203504 evennia-4.1.0/evennia/locale/la/LC_MESSAGES/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     6537 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/locale/la/LC_MESSAGES/django.mo
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    32786 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/locale/la/LC_MESSAGES/django.po
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.179504 evennia-4.1.0/evennia/locale/pl/
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.203504 evennia-4.1.0/evennia/locale/pl/LC_MESSAGES/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1631 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/locale/pl/LC_MESSAGES/django.mo
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    28236 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/locale/pl/LC_MESSAGES/django.po
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.179504 evennia-4.1.0/evennia/locale/pt/
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.203504 evennia-4.1.0/evennia/locale/pt/LC_MESSAGES/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    25584 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/locale/pt/LC_MESSAGES/django.mo
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    42122 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/locale/pt/LC_MESSAGES/django.po
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.179504 evennia-4.1.0/evennia/locale/ru/
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.203504 evennia-4.1.0/evennia/locale/ru/LC_MESSAGES/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2281 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/locale/ru/LC_MESSAGES/django.mo
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    29419 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/locale/ru/LC_MESSAGES/django.po
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.179504 evennia-4.1.0/evennia/locale/sv/
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.203504 evennia-4.1.0/evennia/locale/sv/LC_MESSAGES/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    29036 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/locale/sv/LC_MESSAGES/django.mo
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    43353 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/locale/sv/LC_MESSAGES/django.po
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.179504 evennia-4.1.0/evennia/locale/zh/
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.203504 evennia-4.1.0/evennia/locale/zh/LC_MESSAGES/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3300 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/locale/zh/LC_MESSAGES/django.mo
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    30540 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/locale/zh/LC_MESSAGES/django.po
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.203504 evennia-4.1.0/evennia/locks/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      240 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/locks/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    22155 2024-04-01 15:48:29.000000 evennia-4.1.0/evennia/locks/lockfuncs.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    27271 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/locks/lockhandler.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    13732 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/locks/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.203504 evennia-4.1.0/evennia/objects/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      120 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/objects/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    29653 2024-04-01 15:48:32.000000 evennia-4.1.0/evennia/objects/manager.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.207504 evennia-4.1.0/evennia/objects/migrations/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4315 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/objects/migrations/0001_initial.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1193 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/objects/migrations/0002_auto_20140917_0756.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      810 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/objects/migrations/0003_defaultcharacter_defaultexit_defaultobject_defaultroom.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      530 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/objects/migrations/0004_auto_20150118_1622.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      410 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/objects/migrations/0005_auto_20150403_2339.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1599 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/objects/migrations/0006_auto_20170606_1731.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1203 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/objects/migrations/0007_objectdb_db_account.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      757 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/objects/migrations/0008_auto_20170705_1736.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      643 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/objects/migrations/0009_remove_objectdb_db_player.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     5028 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/objects/migrations/0010_auto_20190128_1820.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1351 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/objects/migrations/0011_auto_20191025_0831.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4011 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/objects/migrations/0012_convert_contrib_typeclass_paths.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      488 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/objects/migrations/0013_defaultobject_alter_objectdb_id_defaultcharacter_and_more.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/objects/migrations/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    13400 2024-04-01 15:48:32.000000 evennia-4.1.0/evennia/objects/models.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)   131813 2024-04-01 15:48:32.000000 evennia-4.1.0/evennia/objects/objects.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    21877 2024-04-01 15:48:30.000000 evennia-4.1.0/evennia/objects/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.207504 evennia-4.1.0/evennia/prototypes/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     6567 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/prototypes/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/prototypes/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    92096 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/prototypes/menus.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2912 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/prototypes/protfuncs.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    46538 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/prototypes/prototypes.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    42851 2024-04-01 15:48:30.000000 evennia-4.1.0/evennia/prototypes/spawner.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    39629 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/prototypes/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.207504 evennia-4.1.0/evennia/scripts/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      229 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/scripts/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    11275 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/scripts/manager.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.207504 evennia-4.1.0/evennia/scripts/migrations/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4762 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/scripts/migrations/0001_initial.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      675 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/scripts/migrations/0002_auto_20150118_1625.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1507 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/scripts/migrations/0003_checksessions_defaultscript_donothing_scriptbase_store_validatechannelhandler_validateidmappercache_.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      861 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/scripts/migrations/0004_auto_20150306_1354.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      430 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/scripts/migrations/0005_auto_20150306_1441.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      710 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/scripts/migrations/0006_auto_20150310_2249.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      396 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/scripts/migrations/0007_auto_20150403_2339.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      913 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/scripts/migrations/0008_auto_20170606_1731.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1271 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/scripts/migrations/0009_scriptdb_db_account.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      757 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/scripts/migrations/0010_auto_20170705_1736.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      596 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/scripts/migrations/0011_remove_scriptdb_db_player.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4655 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/scripts/migrations/0012_auto_20190128_1820.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      666 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/scripts/migrations/0013_auto_20191025_0831.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      752 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/scripts/migrations/0014_auto_20210520_2137.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3329 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/scripts/migrations/0015_convert_contrib_paths.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      478 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/scripts/migrations/0016_scriptbase_alter_scriptdb_id_defaultscript_and_more.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       24 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/scripts/migrations/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     6312 2024-04-01 15:48:29.000000 evennia-4.1.0/evennia/scripts/models.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     8762 2024-04-01 15:48:29.000000 evennia-4.1.0/evennia/scripts/monitorhandler.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    27363 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/scripts/ondemandhandler.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     5510 2024-04-01 15:48:29.000000 evennia-4.1.0/evennia/scripts/scripthandler.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    27674 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/scripts/scripts.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    20794 2024-04-01 15:48:29.000000 evennia-4.1.0/evennia/scripts/taskhandler.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    26185 2024-04-01 15:48:32.000000 evennia-4.1.0/evennia/scripts/tests.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    24662 2024-04-01 15:48:30.000000 evennia-4.1.0/evennia/scripts/tickerhandler.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.207504 evennia-4.1.0/evennia/server/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      234 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/server/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     8753 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/server/amp_client.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    16628 2024-04-01 15:48:30.000000 evennia-4.1.0/evennia/server/connection_wizard.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     8129 2024-04-01 15:48:29.000000 evennia-4.1.0/evennia/server/deprecations.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    79791 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/server/evennia_launcher.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.207504 evennia-4.1.0/evennia/server/game_index_client/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4321 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/server/game_index_client/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       45 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/server/game_index_client/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     6182 2024-04-01 15:48:29.000000 evennia-4.1.0/evennia/server/game_index_client/client.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1988 2024-04-01 15:48:29.000000 evennia-4.1.0/evennia/server/game_index_client/service.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     7406 2024-04-01 15:48:29.000000 evennia-4.1.0/evennia/server/initial_setup.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    20403 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/server/inputfuncs.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1846 2024-04-01 15:48:29.000000 evennia-4.1.0/evennia/server/manager.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.207504 evennia-4.1.0/evennia/server/migrations/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      812 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/server/migrations/0001_initial.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1363 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/server/migrations/0002_auto_20190128_2311.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      478 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/server/migrations/0003_alter_serverconfig_id.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       24 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/server/migrations/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3819 2024-04-01 15:48:29.000000 evennia-4.1.0/evennia/server/models.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.211504 evennia-4.1.0/evennia/server/portal/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       24 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/server/portal/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    17922 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/server/portal/amp.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    17650 2024-04-01 15:48:30.000000 evennia-4.1.0/evennia/server/portal/amp_server.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    19120 2024-04-01 15:48:30.000000 evennia-4.1.0/evennia/server/portal/discord.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    11344 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/server/portal/grapevine.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    14242 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/server/portal/irc.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2572 2024-04-01 15:48:29.000000 evennia-4.1.0/evennia/server/portal/mccp.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3883 2024-04-01 15:48:29.000000 evennia-4.1.0/evennia/server/portal/mssp.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2342 2024-04-01 15:48:29.000000 evennia-4.1.0/evennia/server/portal/mxp.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2360 2024-04-01 15:48:29.000000 evennia-4.1.0/evennia/server/portal/naws.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1168 2024-04-01 15:48:29.000000 evennia-4.1.0/evennia/server/portal/portal.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    17379 2024-04-01 15:48:30.000000 evennia-4.1.0/evennia/server/portal/portalsessionhandler.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4451 2024-04-01 15:48:30.000000 evennia-4.1.0/evennia/server/portal/rss.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    14930 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/server/portal/service.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    15898 2024-04-01 15:48:32.000000 evennia-4.1.0/evennia/server/portal/ssh.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3320 2024-04-01 15:48:29.000000 evennia-4.1.0/evennia/server/portal/ssl.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1787 2024-04-01 15:48:29.000000 evennia-4.1.0/evennia/server/portal/suppress_ga.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    17380 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/server/portal/telnet.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    15610 2024-04-01 15:48:30.000000 evennia-4.1.0/evennia/server/portal/telnet_oob.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4751 2024-04-01 15:48:30.000000 evennia-4.1.0/evennia/server/portal/telnet_ssl.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    15494 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/server/portal/tests.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     7073 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/server/portal/ttype.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    11522 2024-04-01 15:48:30.000000 evennia-4.1.0/evennia/server/portal/webclient.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    16166 2024-04-01 15:48:30.000000 evennia-4.1.0/evennia/server/portal/webclient_ajax.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.211504 evennia-4.1.0/evennia/server/profiling/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      212 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/server/profiling/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/server/profiling/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    20879 2024-04-01 15:48:30.000000 evennia-4.1.0/evennia/server/profiling/dummyrunner.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     9428 2024-04-01 15:48:30.000000 evennia-4.1.0/evennia/server/profiling/dummyrunner_settings.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3923 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/server/profiling/memplot.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1375 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/server/profiling/settings_mixin.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1094 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/server/profiling/test_queries.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     5371 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/server/profiling/tests.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1345 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/server/profiling/timetrace.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1167 2024-04-01 15:48:30.000000 evennia-4.1.0/evennia/server/server.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    16593 2024-04-01 15:48:30.000000 evennia-4.1.0/evennia/server/serversession.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    27031 2024-04-01 15:48:30.000000 evennia-4.1.0/evennia/server/service.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     5617 2024-04-01 15:48:30.000000 evennia-4.1.0/evennia/server/session.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    30267 2024-04-01 15:48:30.000000 evennia-4.1.0/evennia/server/sessionhandler.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     5391 2024-04-01 15:48:30.000000 evennia-4.1.0/evennia/server/signals.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.211504 evennia-4.1.0/evennia/server/tests/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/server/tests/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     5193 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/server/tests/test_amp_connection.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      521 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/server/tests/test_initial_setup.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     7305 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/server/tests/test_launcher.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3814 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/server/tests/test_misc.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     8859 2024-04-01 15:48:30.000000 evennia-4.1.0/evennia/server/tests/test_server.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      985 2024-04-01 15:48:30.000000 evennia-4.1.0/evennia/server/tests/testrunner.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     7101 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/server/throttle.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1216 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/server/validators.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     8654 2024-04-01 15:48:30.000000 evennia-4.1.0/evennia/server/webserver.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    62336 2024-04-01 15:48:30.000000 evennia-4.1.0/evennia/settings_default.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.211504 evennia-4.1.0/evennia/typeclasses/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      434 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/typeclasses/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    64400 2024-04-01 15:48:31.000000 evennia-4.1.0/evennia/typeclasses/attributes.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    31305 2024-04-01 15:48:30.000000 evennia-4.1.0/evennia/typeclasses/managers.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.211504 evennia-4.1.0/evennia/typeclasses/migrations/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     6101 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/typeclasses/migrations/0001_initial.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      768 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/typeclasses/migrations/0002_auto_20150109_0913.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2266 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/typeclasses/migrations/0003_defaultcharacter_defaultexit_defaultguest_defaultobject_defaultplayer_defaultroom_defaultscript_dono.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      833 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/typeclasses/migrations/0004_auto_20151101_1759.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      922 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/typeclasses/migrations/0005_auto_20160625_1812.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1444 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/typeclasses/migrations/0006_auto_add_dbmodel_value_for_tags_attributes.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3899 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/typeclasses/migrations/0007_tag_migrations_may_be_slow.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1699 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/typeclasses/migrations/0008_lock_and_perm_rename.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4230 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/typeclasses/migrations/0009_rename_player_cmdsets_typeclasses.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1993 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/typeclasses/migrations/0010_delete_old_player_tables.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     5265 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/typeclasses/migrations/0011_auto_20190128_1820.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      821 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/typeclasses/migrations/0012_attrs_to_picklev4_may_be_slow.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      592 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/typeclasses/migrations/0013_auto_20191015_1922.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      592 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/typeclasses/migrations/0014_alter_tag_db_category.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      362 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/typeclasses/migrations/0015_alter_attribute_options.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      722 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/typeclasses/migrations/0016_alter_attribute_id_alter_tag_id.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       24 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/typeclasses/migrations/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    37171 2024-04-01 15:48:30.000000 evennia-4.1.0/evennia/typeclasses/models.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    30234 2024-04-01 15:48:30.000000 evennia-4.1.0/evennia/typeclasses/tags.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    17814 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/typeclasses/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.211504 evennia-4.1.0/evennia/utils/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      320 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/utils/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    51450 2024-04-01 15:48:31.000000 evennia-4.1.0/evennia/utils/ansi.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    15393 2024-04-01 15:48:30.000000 evennia-4.1.0/evennia/utils/batchprocessors.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     7755 2024-04-01 15:48:30.000000 evennia-4.1.0/evennia/utils/containers.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    10242 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/utils/create.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    32815 2024-04-01 15:48:30.000000 evennia-4.1.0/evennia/utils/dbserialize.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    41555 2024-04-01 15:48:32.000000 evennia-4.1.0/evennia/utils/eveditor.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2734 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/utils/evennia-mode.el
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    21381 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/utils/evform.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    80600 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/utils/evmenu.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    18832 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/utils/evmore.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    65172 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/utils/evtable.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    55430 2024-04-01 15:48:31.000000 evennia-4.1.0/evennia/utils/funcparser.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     8754 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/utils/gametime.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.211504 evennia-4.1.0/evennia/utils/idmapper/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1309 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/utils/idmapper/LICENSE.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1097 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/utils/idmapper/README_evennia.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1992 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/utils/idmapper/README_orig.rst
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       64 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/utils/idmapper/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1182 2024-04-01 15:48:30.000000 evennia-4.1.0/evennia/utils/idmapper/manager.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    24820 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/utils/idmapper/models.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2875 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/utils/idmapper/tests.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    18788 2024-04-01 15:48:30.000000 evennia-4.1.0/evennia/utils/logger.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    10324 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/utils/optionclasses.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     6519 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/utils/optionhandler.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    11093 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/utils/picklefield.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    14179 2024-03-31 10:02:22.000000 evennia-4.1.0/evennia/utils/search.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    25825 2024-04-01 15:48:32.000000 evennia-4.1.0/evennia/utils/test_resources.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.215504 evennia-4.1.0/evennia/utils/tests/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/utils/tests/__init__.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.215504 evennia-4.1.0/evennia/utils/tests/data/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/utils/tests/data/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      274 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/utils/tests/data/broken_script.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1125 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/utils/tests/data/evform_example.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     6245 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/utils/tests/data/evmenu_example.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      382 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/utils/tests/data/prototypes_example.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1608 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/utils/tests/test_ansi.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     7052 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/utils/tests/test_batchprocessors.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3463 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/utils/tests/test_containers.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     7030 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/utils/tests/test_create_functions.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     7888 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/utils/tests/test_dbserialize.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    14444 2024-04-01 15:48:30.000000 evennia-4.1.0/evennia/utils/tests/test_eveditor.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    12171 2024-04-01 15:48:30.000000 evennia-4.1.0/evennia/utils/tests/test_evform.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    11764 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/utils/tests/test_evmenu.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    12705 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/utils/tests/test_evtable.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    31687 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/utils/tests/test_funcparser.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3942 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/utils/tests/test_gametime.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4460 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/utils/tests/test_search.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    13565 2024-04-01 15:48:30.000000 evennia-4.1.0/evennia/utils/tests/test_tagparsing.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     5509 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/utils/tests/test_text2html.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    33293 2024-04-01 15:48:32.000000 evennia-4.1.0/evennia/utils/tests/test_utils.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     6370 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/utils/tests/test_validatorfuncs.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    12235 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/utils/text2html.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)   102284 2024-04-01 15:48:32.000000 evennia-4.1.0/evennia/utils/utils.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     9489 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/utils/validatorfuncs.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.215504 evennia-4.1.0/evennia/utils/verb_conjugation/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    18011 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/utils/verb_conjugation/LICENSE.txt
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/utils/verb_conjugation/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     9944 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/utils/verb_conjugation/conjugate.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    11299 2024-04-01 15:48:30.000000 evennia-4.1.0/evennia/utils/verb_conjugation/pronouns.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    10493 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/utils/verb_conjugation/tests.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)   554408 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/utils/verb_conjugation/verbs.txt
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.215504 evennia-4.1.0/evennia/web/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1150 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      127 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/__init__.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.215504 evennia-4.1.0/evennia/web/admin/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      428 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/admin/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    14125 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/admin/accounts.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     8627 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/admin/attributes.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     8508 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/admin/comms.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      593 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/admin/frontpage.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1890 2024-04-01 15:48:30.000000 evennia-4.1.0/evennia/web/admin/help.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    11705 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/admin/objects.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4498 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/admin/scripts.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      508 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/admin/server.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     8954 2024-04-01 15:48:30.000000 evennia-4.1.0/evennia/web/admin/tags.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      878 2024-04-01 15:48:30.000000 evennia-4.1.0/evennia/web/admin/urls.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2884 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/admin/utils.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.215504 evennia-4.1.0/evennia/web/api/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     7674 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/api/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/api/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4268 2024-04-01 15:48:30.000000 evennia-4.1.0/evennia/web/api/filters.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3948 2024-04-01 15:48:30.000000 evennia-4.1.0/evennia/web/api/permissions.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      277 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/api/root.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     9905 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/api/serializers.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     8147 2024-04-01 15:48:30.000000 evennia-4.1.0/evennia/web/api/tests.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2293 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/api/urls.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     5829 2024-04-01 15:48:30.000000 evennia-4.1.0/evennia/web/api/views.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.179504 evennia-4.1.0/evennia/web/static/
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.179504 evennia-4.1.0/evennia/web/static/rest_framework/
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.215504 evennia-4.1.0/evennia/web/static/rest_framework/css/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      298 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/static/rest_framework/css/api.css
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.215504 evennia-4.1.0/evennia/web/static/rest_framework/images/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1406 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/static/rest_framework/images/favicon.ico
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.179504 evennia-4.1.0/evennia/web/static/webclient/
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.215504 evennia-4.1.0/evennia/web/static/webclient/css/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/static/webclient/css/custom.css
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2104 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/static/webclient/css/goldenlayout.css
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    27268 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/static/webclient/css/webclient.css
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.215504 evennia-4.1.0/evennia/web/static/webclient/fonts/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    22208 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/static/webclient/fonts/DejaVuSansMono-webfont.woff
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      185 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/static/webclient/fonts/DejaVuSansMono.css
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.215504 evennia-4.1.0/evennia/web/static/webclient/js/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    18677 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/static/webclient/js/evennia.js
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.215504 evennia-4.1.0/evennia/web/static/webclient/js/plugins/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      563 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/static/webclient/js/plugins/clienthelp.js
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3914 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/static/webclient/js/plugins/default_in.js
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1967 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/static/webclient/js/plugins/default_out.js
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      345 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/static/webclient/js/plugins/default_unload.js
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3785 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/static/webclient/js/plugins/font.js
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    30344 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/static/webclient/js/plugins/goldenlayout.js
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2114 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/static/webclient/js/plugins/goldenlayout_default_config.js
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2981 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/static/webclient/js/plugins/history.js
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     5031 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/static/webclient/js/plugins/hotbuttons.js
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1969 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/static/webclient/js/plugins/html.js
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1912 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/static/webclient/js/plugins/iframe.js
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4666 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/static/webclient/js/plugins/message_routing.js
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4611 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/static/webclient/js/plugins/multimedia.js
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2842 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/static/webclient/js/plugins/notifications.js
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      909 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/static/webclient/js/plugins/oob.js
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     6262 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/static/webclient/js/plugins/options2.js
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2790 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/static/webclient/js/plugins/popups.js
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    10949 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/static/webclient/js/plugins/text2html.js
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     9615 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/static/webclient/js/webclient_gui.js
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.215504 evennia-4.1.0/evennia/web/static/webclient/media/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3624 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/static/webclient/media/notification.wav
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.179504 evennia-4.1.0/evennia/web/static/website/
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.215504 evennia-4.1.0/evennia/web/static/website/css/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/static/website/css/custom.css
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2013 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/static/website/css/website.css
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.219504 evennia-4.1.0/evennia/web/static/website/images/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      266 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/static/website/images/LICENCE
--rwxrwxr-x   0 griatch   (1000) griatch   (1000)    17938 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/static/website/images/evennia_logo.png
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    21167 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/static/website/images/evennia_logo_festive.png
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1406 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/static/website/images/favicon.ico
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.179504 evennia-4.1.0/evennia/web/templates/
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.219504 evennia-4.1.0/evennia/web/templates/admin/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1621 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/templates/admin/app_list.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     6462 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/templates/admin/frontpage.html
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.219504 evennia-4.1.0/evennia/web/templates/rest_framework/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      903 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/templates/rest_framework/api.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      417 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/templates/rest_framework/redoc.html
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.219504 evennia-4.1.0/evennia/web/templates/webclient/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     8353 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/templates/webclient/base.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1058 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/templates/webclient/webclient.html
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.219504 evennia-4.1.0/evennia/web/templates/website/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      510 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/templates/website/404.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      614 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/templates/website/500.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4059 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/templates/website/_menu.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3132 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/templates/website/base.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2858 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/templates/website/channel_detail.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2667 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/templates/website/channel_list.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1402 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/templates/website/character_form.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      546 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/templates/website/character_list.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1139 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/templates/website/character_manage_list.html
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.219504 evennia-4.1.0/evennia/web/templates/website/flatpages/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      341 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/templates/website/flatpages/default.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1501 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/templates/website/generic_form.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2715 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/templates/website/help_detail.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     5052 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/templates/website/help_list.html
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.219504 evennia-4.1.0/evennia/web/templates/website/homepage/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      593 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/templates/website/homepage/accounts-widget.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      574 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/templates/website/homepage/database-stats-widget.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      542 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/templates/website/homepage/evennia-widget.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1980 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/templates/website/homepage/main-content.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      387 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/templates/website/homepage/recently-connected-widget.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      952 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/templates/website/index.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      180 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/templates/website/messages.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      900 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/templates/website/object_confirm_delete.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1034 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/templates/website/object_detail.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      546 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/templates/website/object_list.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1484 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/templates/website/pagination.html
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.219504 evennia-4.1.0/evennia/web/templates/website/registration/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      942 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/templates/website/registration/logged_out.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1957 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/templates/website/registration/login.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      612 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/templates/website/registration/password_change_done.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1422 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/templates/website/registration/password_change_form.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      813 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/templates/website/registration/password_reset_complete.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1747 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/templates/website/registration/password_reset_confirm.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1185 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/templates/website/registration/password_reset_done.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      566 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/templates/website/registration/password_reset_email.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1577 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/templates/website/registration/password_reset_form.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1895 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/templates/website/registration/register.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      671 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/templates/website/tbi.html
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.219504 evennia-4.1.0/evennia/web/templatetags/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      287 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/templatetags/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/templatetags/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      550 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/templatetags/addclass.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1631 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/urls.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.219504 evennia-4.1.0/evennia/web/utils/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/utils/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1353 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/utils/adminsite.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      596 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/utils/apache_wsgi.conf
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1815 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/utils/backends.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2035 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/utils/evennia_modpy_apache.conf
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1819 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/utils/evennia_wsgi_apache.conf
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4130 2024-04-01 15:48:32.000000 evennia-4.1.0/evennia/web/utils/general_context.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3144 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/utils/middleware.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2444 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/utils/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.219504 evennia-4.1.0/evennia/web/webclient/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/webclient/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      210 2024-04-01 15:48:30.000000 evennia-4.1.0/evennia/web/webclient/urls.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      795 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/webclient/views.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.219504 evennia-4.1.0/evennia/web/website/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       31 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/website/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     5737 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/website/forms.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    12375 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/website/tests.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2576 2024-04-01 15:48:30.000000 evennia-4.1.0/evennia/web/website/urls.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.219504 evennia-4.1.0/evennia/web/website/views/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       24 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/website/views/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2120 2024-04-01 15:48:30.000000 evennia-4.1.0/evennia/web/website/views/accounts.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     5329 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/website/views/channels.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     8802 2024-04-01 15:48:32.000000 evennia-4.1.0/evennia/web/website/views/characters.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      311 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/website/views/errors.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    11790 2024-04-01 15:48:30.000000 evennia-4.1.0/evennia/web/website/views/help.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4611 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/website/views/index.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2354 2024-04-01 15:48:30.000000 evennia-4.1.0/evennia/web/website/views/mixins.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     9037 2024-03-17 13:16:37.000000 evennia-4.1.0/evennia/web/website/views/objects.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-01 18:37:21.219504 evennia-4.1.0/evennia.egg-info/
--rw-r--r--   0 griatch   (1000) griatch   (1000)     6510 2024-04-01 18:37:20.000000 evennia-4.1.0/evennia.egg-info/PKG-INFO
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    35956 2024-04-01 18:37:21.000000 evennia-4.1.0/evennia.egg-info/SOURCES.txt
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        1 2024-04-01 18:37:20.000000 evennia-4.1.0/evennia.egg-info/dependency_links.txt
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      562 2024-04-01 18:37:20.000000 evennia-4.1.0/evennia.egg-info/requires.txt
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        8 2024-04-01 18:37:20.000000 evennia-4.1.0/evennia.egg-info/top_level.txt
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3979 2024-04-01 18:25:49.000000 evennia-4.1.0/pyproject.toml
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       38 2024-04-01 18:37:21.223504 evennia-4.1.0/setup.cfg
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1388 2024-03-17 13:16:37.000000 evennia-4.1.0/setup.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.959616 evennia-4.1.1/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1531 2024-03-17 13:16:36.000000 evennia-4.1.1/LICENSE.txt
+-rw-r--r--   0 griatch   (1000) griatch   (1000)     6510 2024-04-06 21:07:27.959616 evennia-4.1.1/PKG-INFO
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3034 2024-03-17 13:16:36.000000 evennia-4.1.1/README.md
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.911615 evennia-4.1.1/bin/
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.919615 evennia-4.1.1/bin/unix/
+-rwxrwxr-x   0 griatch   (1000) griatch   (1000)      210 2024-03-17 13:16:36.000000 evennia-4.1.1/bin/unix/evennia
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.919615 evennia-4.1.1/evennia/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        6 2024-04-06 21:02:29.000000 evennia-4.1.1/evennia/VERSION.txt
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      437 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/VERSION_REQS.txt
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    15076 2024-04-01 15:48:28.000000 evennia-4.1.1/evennia/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1839 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/__main__.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.919615 evennia-4.1.1/evennia/accounts/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      214 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/accounts/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    74554 2024-04-06 11:55:27.000000 evennia-4.1.1/evennia/accounts/accounts.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    26930 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/accounts/bots.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     9574 2024-04-01 15:48:32.000000 evennia-4.1.1/evennia/accounts/manager.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.919615 evennia-4.1.1/evennia/accounts/migrations/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     7211 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/accounts/migrations/0001_initial.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      504 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/accounts/migrations/0002_move_defaults.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      612 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/accounts/migrations/0003_auto_20150209_2234.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2158 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/accounts/migrations/0004_auto_20150403_2339.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1010 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/accounts/migrations/0005_auto_20160905_0902.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1488 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/accounts/migrations/0006_auto_20170606_1731.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1927 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/accounts/migrations/0007_copy_player_to_account.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3944 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/accounts/migrations/0008_auto_20190128_1820.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      867 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/accounts/migrations/0009_auto_20191025_0831.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      467 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/accounts/migrations/0010_auto_20210520_2137.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4017 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/accounts/migrations/0011_convert_contrib_typeclass_paths.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      490 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/accounts/migrations/0012_defaultaccount_alter_accountdb_id_account_bot_and_more.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       24 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/accounts/migrations/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     5741 2024-04-01 15:48:28.000000 evennia-4.1.1/evennia/accounts/models.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    17496 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/accounts/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.919615 evennia-4.1.1/evennia/commands/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      304 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/commands/__init__.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.919615 evennia-4.1.1/evennia/commands/_trial_temp/
+-rwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/commands/_trial_temp/_trial_marker
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    31495 2024-04-01 15:48:32.000000 evennia-4.1.1/evennia/commands/cmdhandler.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     8286 2024-04-01 15:48:28.000000 evennia-4.1.1/evennia/commands/cmdparser.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    27313 2024-04-01 15:48:28.000000 evennia-4.1.1/evennia/commands/cmdset.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    26152 2024-04-01 15:48:28.000000 evennia-4.1.1/evennia/commands/cmdsethandler.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    29047 2024-04-01 15:48:32.000000 evennia-4.1.1/evennia/commands/command.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.919615 evennia-4.1.1/evennia/commands/default/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       87 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/commands/default/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    35296 2024-04-01 15:48:28.000000 evennia-4.1.1/evennia/commands/default/account.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    19512 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/commands/default/admin.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    22983 2024-04-01 15:48:28.000000 evennia-4.1.1/evennia/commands/default/batchprocess.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)   172881 2024-04-06 11:55:27.000000 evennia-4.1.1/evennia/commands/default/building.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2358 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/commands/default/cmdset_account.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3033 2024-04-01 15:48:28.000000 evennia-4.1.1/evennia/commands/default/cmdset_character.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      372 2024-04-01 15:48:28.000000 evennia-4.1.1/evennia/commands/default/cmdset_session.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      873 2024-04-01 15:48:28.000000 evennia-4.1.1/evennia/commands/default/cmdset_unloggedin.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    77528 2024-04-01 15:48:32.000000 evennia-4.1.1/evennia/commands/default/comms.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    25750 2024-04-06 11:55:27.000000 evennia-4.1.1/evennia/commands/default/general.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    40503 2024-03-30 15:40:53.000000 evennia-4.1.1/evennia/commands/default/help.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    12774 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/commands/default/muxcommand.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3152 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/commands/default/syscommands.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    42139 2024-04-01 15:48:28.000000 evennia-4.1.1/evennia/commands/default/system.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    84651 2024-04-05 20:41:20.000000 evennia-4.1.1/evennia/commands/default/tests.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    15024 2024-04-01 15:48:28.000000 evennia-4.1.1/evennia/commands/default/unloggedin.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    47839 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/commands/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.919615 evennia-4.1.1/evennia/comms/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      207 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/comms/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    32603 2024-04-01 15:48:28.000000 evennia-4.1.1/evennia/comms/comms.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    16863 2024-04-01 15:48:28.000000 evennia-4.1.1/evennia/comms/managers.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.923616 evennia-4.1.1/evennia/comms/migrations/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3523 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/comms/migrations/0001_initial.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      500 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/comms/migrations/0002_msg_db_hide_from_objects.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3784 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/comms/migrations/0003_auto_20140917_0756.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      504 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/comms/migrations/0004_auto_20150118_1631.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      641 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/comms/migrations/0005_auto_20150223_1517.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      643 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/comms/migrations/0006_channeldb_db_object_subscriptions.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      615 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/comms/migrations/0007_msg_db_tags.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      434 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/comms/migrations/0008_auto_20160905_0902.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3872 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/comms/migrations/0009_auto_20160921_1731.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1079 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/comms/migrations/0010_auto_20161206_1912.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1029 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/comms/migrations/0011_auto_20170217_2039.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4563 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/comms/migrations/0011_auto_20170606_1731.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      267 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/comms/migrations/0012_merge_20170617_2017.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4778 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/comms/migrations/0013_auto_20170705_1726.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1442 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/comms/migrations/0014_auto_20170705_1736.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      943 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/comms/migrations/0015_auto_20170706_2041.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      462 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/comms/migrations/0016_auto_20180925_1735.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     7069 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/comms/migrations/0017_auto_20190128_1820.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      665 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/comms/migrations/0018_auto_20191025_0831.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1713 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/comms/migrations/0019_auto_20210514_2032.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      916 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/comms/migrations/0020_auto_20210514_2210.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3635 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/comms/migrations/0021_auto_20210520_2137.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      711 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/comms/migrations/0022_defaultchannel_alter_channeldb_id_alter_msg_id_and_more.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       24 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/comms/migrations/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    22647 2024-04-01 15:48:28.000000 evennia-4.1.1/evennia/comms/models.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3166 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/comms/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.923616 evennia-4.1.1/evennia/contrib/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1895 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      198 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/__init__.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.923616 evennia-4.1.1/evennia/contrib/base_systems/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       80 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/base_systems/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/base_systems/__init__.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.923616 evennia-4.1.1/evennia/contrib/base_systems/awsstorage/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     7695 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/base_systems/awsstorage/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       48 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/base_systems/awsstorage/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    32479 2024-04-01 15:48:28.000000 evennia-4.1.1/evennia/contrib/base_systems/awsstorage/aws_s3_cdn.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    22503 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/base_systems/awsstorage/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.923616 evennia-4.1.1/evennia/contrib/base_systems/building_menu/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    46012 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/base_systems/building_menu/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      149 2024-04-01 15:48:28.000000 evennia-4.1.1/evennia/contrib/base_systems/building_menu/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    42684 2024-04-01 15:48:28.000000 evennia-4.1.1/evennia/contrib/base_systems/building_menu/building_menu.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     6879 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/base_systems/building_menu/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.923616 evennia-4.1.1/evennia/contrib/base_systems/color_markups/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2641 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/base_systems/color_markups/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       84 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/base_systems/color_markups/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     8605 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/base_systems/color_markups/color_markups.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3356 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/base_systems/color_markups/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.923616 evennia-4.1.1/evennia/contrib/base_systems/components/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     6914 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/base_systems/components/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      514 2024-04-01 15:48:28.000000 evennia-4.1.1/evennia/contrib/base_systems/components/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     5129 2024-04-06 20:42:58.000000 evennia-4.1.1/evennia/contrib/base_systems/components/component.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     5208 2024-04-06 20:31:27.000000 evennia-4.1.1/evennia/contrib/base_systems/components/dbfield.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      157 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/base_systems/components/exceptions.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    10305 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/base_systems/components/holder.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      540 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/base_systems/components/listing.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     7516 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/base_systems/components/signals.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    17215 2024-04-06 20:40:48.000000 evennia-4.1.1/evennia/contrib/base_systems/components/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.923616 evennia-4.1.1/evennia/contrib/base_systems/custom_gametime/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1549 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/base_systems/custom_gametime/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      439 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/base_systems/custom_gametime/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    10389 2024-04-01 15:48:28.000000 evennia-4.1.1/evennia/contrib/base_systems/custom_gametime/custom_gametime.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2017 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/base_systems/custom_gametime/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.923616 evennia-4.1.1/evennia/contrib/base_systems/email_login/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1022 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/base_systems/email_login/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      136 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/base_systems/email_login/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1445 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/base_systems/email_login/connection_screens.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    10573 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/base_systems/email_login/email_login.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1200 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/base_systems/email_login/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.923616 evennia-4.1.1/evennia/contrib/base_systems/godotwebsocket/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     6041 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/base_systems/godotwebsocket/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      704 2024-04-01 15:48:28.000000 evennia-4.1.1/evennia/contrib/base_systems/godotwebsocket/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3074 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/base_systems/godotwebsocket/test_text2bbcode.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3186 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/base_systems/godotwebsocket/test_webclient.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    27603 2024-04-01 15:48:28.000000 evennia-4.1.1/evennia/contrib/base_systems/godotwebsocket/text2bbcode.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2683 2024-04-01 15:48:28.000000 evennia-4.1.1/evennia/contrib/base_systems/godotwebsocket/webclient.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.923616 evennia-4.1.1/evennia/contrib/base_systems/ingame_python/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    40300 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/base_systems/ingame_python/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      128 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/base_systems/ingame_python/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     6776 2024-04-01 15:48:28.000000 evennia-4.1.1/evennia/contrib/base_systems/ingame_python/callbackhandler.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    21871 2024-04-01 15:48:28.000000 evennia-4.1.1/evennia/contrib/base_systems/ingame_python/commands.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3048 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/base_systems/ingame_python/eventfuncs.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    23988 2024-04-01 15:48:28.000000 evennia-4.1.1/evennia/contrib/base_systems/ingame_python/scripts.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    21615 2024-04-01 15:48:29.000000 evennia-4.1.1/evennia/contrib/base_systems/ingame_python/tests.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    34959 2024-04-01 15:48:28.000000 evennia-4.1.1/evennia/contrib/base_systems/ingame_python/typeclasses.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     8150 2024-04-01 15:48:28.000000 evennia-4.1.1/evennia/contrib/base_systems/ingame_python/utils.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.923616 evennia-4.1.1/evennia/contrib/base_systems/menu_login/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      787 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/base_systems/menu_login/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      143 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/base_systems/menu_login/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1206 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/base_systems/menu_login/connection_screens.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     8937 2024-04-01 15:48:31.000000 evennia-4.1.1/evennia/contrib/base_systems/menu_login/menu_login.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      265 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/base_systems/menu_login/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.923616 evennia-4.1.1/evennia/contrib/base_systems/mux_comms_cmds/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1936 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/base_systems/mux_comms_cmds/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      104 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/base_systems/mux_comms_cmds/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    16013 2024-04-01 15:48:28.000000 evennia-4.1.1/evennia/contrib/base_systems/mux_comms_cmds/mux_comms_cmds.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2298 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/base_systems/mux_comms_cmds/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.923616 evennia-4.1.1/evennia/contrib/base_systems/unixcommand/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2241 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/base_systems/unixcommand/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       94 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/base_systems/unixcommand/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1653 2024-04-01 15:48:28.000000 evennia-4.1.1/evennia/contrib/base_systems/unixcommand/tests.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     9986 2024-04-01 15:48:28.000000 evennia-4.1.1/evennia/contrib/base_systems/unixcommand/unixcommand.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.923616 evennia-4.1.1/evennia/contrib/full_systems/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       75 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/full_systems/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       48 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/full_systems/__init__.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.923616 evennia-4.1.1/evennia/contrib/full_systems/evscaperoom/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     5210 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/full_systems/evscaperoom/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      266 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/full_systems/evscaperoom/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    22694 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/full_systems/evscaperoom/commands.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    10561 2024-04-01 15:48:28.000000 evennia-4.1.1/evennia/contrib/full_systems/evscaperoom/menu.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    34345 2024-04-01 15:48:29.000000 evennia-4.1.1/evennia/contrib/full_systems/evscaperoom/objects.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     7942 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/full_systems/evscaperoom/room.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      751 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/full_systems/evscaperoom/scripts.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     9582 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/full_systems/evscaperoom/state.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.923616 evennia-4.1.1/evennia/contrib/full_systems/evscaperoom/states/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1203 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/full_systems/evscaperoom/states/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4168 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/full_systems/evscaperoom/states/state_001_start.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    10421 2024-04-01 15:48:28.000000 evennia-4.1.1/evennia/contrib/full_systems/evscaperoom/tests.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     6112 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/full_systems/evscaperoom/utils.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.927616 evennia-4.1.1/evennia/contrib/game_systems/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      269 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/game_systems/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/game_systems/__init__.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.927616 evennia-4.1.1/evennia/contrib/game_systems/barter/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4322 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/game_systems/barter/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       80 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/game_systems/barter/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    29726 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/game_systems/barter/barter.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     5976 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/game_systems/barter/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.927616 evennia-4.1.1/evennia/contrib/game_systems/clothing/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4256 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/game_systems/clothing/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      199 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/game_systems/clothing/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    24856 2024-04-01 15:48:31.000000 evennia-4.1.1/evennia/contrib/game_systems/clothing/clothing.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     6344 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/game_systems/clothing/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.927616 evennia-4.1.1/evennia/contrib/game_systems/containers/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2508 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/game_systems/containers/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       66 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/game_systems/containers/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    10016 2024-04-01 15:48:28.000000 evennia-4.1.1/evennia/contrib/game_systems/containers/containers.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2851 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/game_systems/containers/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.927616 evennia-4.1.1/evennia/contrib/game_systems/cooldowns/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2084 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/game_systems/cooldowns/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       88 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/game_systems/cooldowns/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     7580 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/game_systems/cooldowns/cooldowns.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     6135 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/game_systems/cooldowns/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.927616 evennia-4.1.1/evennia/contrib/game_systems/crafting/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    11186 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/game_systems/crafting/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      233 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/game_systems/crafting/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    41698 2024-04-01 15:48:29.000000 evennia-4.1.1/evennia/contrib/game_systems/crafting/crafting.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    17891 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/game_systems/crafting/example_recipes.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    25314 2024-03-30 22:45:30.000000 evennia-4.1.1/evennia/contrib/game_systems/crafting/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.927616 evennia-4.1.1/evennia/contrib/game_systems/gendersub/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1986 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/game_systems/gendersub/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      123 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/game_systems/gendersub/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     5326 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/game_systems/gendersub/gendersub.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2351 2024-04-01 15:48:28.000000 evennia-4.1.1/evennia/contrib/game_systems/gendersub/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.927616 evennia-4.1.1/evennia/contrib/game_systems/mail/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1567 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/game_systems/mail/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      115 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/game_systems/mail/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    14841 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/game_systems/mail/mail.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1852 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/game_systems/mail/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.927616 evennia-4.1.1/evennia/contrib/game_systems/multidescer/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3228 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/game_systems/multidescer/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       83 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/game_systems/multidescer/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     9952 2024-04-01 15:48:29.000000 evennia-4.1.1/evennia/contrib/game_systems/multidescer/multidescer.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1404 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/game_systems/multidescer/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.927616 evennia-4.1.1/evennia/contrib/game_systems/puzzles/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2181 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/game_systems/puzzles/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      124 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/game_systems/puzzles/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    27836 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/game_systems/puzzles/puzzles.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    41327 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/game_systems/puzzles/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.927616 evennia-4.1.1/evennia/contrib/game_systems/turnbattle/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2940 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/game_systems/turnbattle/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      209 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/game_systems/turnbattle/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    28762 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/game_systems/turnbattle/tb_basic.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    23139 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/game_systems/turnbattle/tb_equip.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    37445 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/game_systems/turnbattle/tb_items.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    30705 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/game_systems/turnbattle/tb_magic.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    38339 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/game_systems/turnbattle/tb_range.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    29680 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/game_systems/turnbattle/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.927616 evennia-4.1.1/evennia/contrib/grid/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       84 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/grid/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       81 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/grid/__init__.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.927616 evennia-4.1.1/evennia/contrib/grid/extended_room/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     6358 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/grid/extended_room/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      454 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/grid/extended_room/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    34233 2024-04-01 15:48:31.000000 evennia-4.1.1/evennia/contrib/grid/extended_room/extended_room.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    12949 2024-04-01 15:48:31.000000 evennia-4.1.1/evennia/contrib/grid/extended_room/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.927616 evennia-4.1.1/evennia/contrib/grid/ingame_map_display/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1358 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/grid/ingame_map_display/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       92 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/grid/ingame_map_display/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    10573 2024-04-01 15:48:29.000000 evennia-4.1.1/evennia/contrib/grid/ingame_map_display/ingame_map_display.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1403 2024-04-01 15:48:28.000000 evennia-4.1.1/evennia/contrib/grid/ingame_map_display/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.927616 evennia-4.1.1/evennia/contrib/grid/mapbuilder/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     9672 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/grid/mapbuilder/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       87 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/grid/mapbuilder/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    17398 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/grid/mapbuilder/mapbuilder.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     6435 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/grid/mapbuilder/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.927616 evennia-4.1.1/evennia/contrib/grid/simpledoor/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1356 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/grid/simpledoor/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      129 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/grid/simpledoor/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     5838 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/grid/simpledoor/simpledoor.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1078 2024-04-01 15:48:28.000000 evennia-4.1.1/evennia/contrib/grid/simpledoor/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.927616 evennia-4.1.1/evennia/contrib/grid/slow_exit/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1730 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/grid/slow_exit/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      203 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/grid/slow_exit/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     5046 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/grid/slow_exit/slow_exit.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      824 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/grid/slow_exit/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.927616 evennia-4.1.1/evennia/contrib/grid/wilderness/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4932 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/grid/wilderness/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      394 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/grid/wilderness/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     6226 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/grid/wilderness/tests.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    27385 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/grid/wilderness/wilderness.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.931615 evennia-4.1.1/evennia/contrib/grid/xyzgrid/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    54837 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/grid/xyzgrid/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      244 2024-04-01 15:48:28.000000 evennia-4.1.1/evennia/contrib/grid/xyzgrid/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    20845 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/grid/xyzgrid/commands.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     7823 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/grid/xyzgrid/example.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    13700 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/grid/xyzgrid/launchcmd.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1146 2024-04-01 15:48:28.000000 evennia-4.1.1/evennia/contrib/grid/xyzgrid/prototypes.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    42076 2024-04-01 15:48:31.000000 evennia-4.1.1/evennia/contrib/grid/xyzgrid/tests.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1043 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/grid/xyzgrid/utils.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    40422 2024-04-01 15:48:31.000000 evennia-4.1.1/evennia/contrib/grid/xyzgrid/xymap.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    52392 2024-04-06 11:55:26.000000 evennia-4.1.1/evennia/contrib/grid/xyzgrid/xymap_legend.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    10484 2024-04-01 15:48:29.000000 evennia-4.1.1/evennia/contrib/grid/xyzgrid/xyzgrid.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    24750 2024-04-06 11:55:26.000000 evennia-4.1.1/evennia/contrib/grid/xyzgrid/xyzroom.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.931615 evennia-4.1.1/evennia/contrib/rpg/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      406 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/rpg/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/rpg/__init__.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.931615 evennia-4.1.1/evennia/contrib/rpg/buffs/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    22364 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/rpg/buffs/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      210 2024-04-01 15:48:31.000000 evennia-4.1.1/evennia/contrib/rpg/buffs/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    45719 2024-04-01 15:48:29.000000 evennia-4.1.1/evennia/contrib/rpg/buffs/buff.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3893 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/rpg/buffs/samplebuffs.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    16471 2024-04-01 15:48:29.000000 evennia-4.1.1/evennia/contrib/rpg/buffs/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.931615 evennia-4.1.1/evennia/contrib/rpg/character_creator/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3922 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/rpg/character_creator/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      176 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/rpg/character_creator/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     7448 2024-04-01 15:48:29.000000 evennia-4.1.1/evennia/contrib/rpg/character_creator/character_creator.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    21006 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/rpg/character_creator/example_menu.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1809 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/rpg/character_creator/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.931615 evennia-4.1.1/evennia/contrib/rpg/dice/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3812 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/rpg/dice/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      177 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/rpg/dice/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    12730 2024-04-01 15:48:29.000000 evennia-4.1.1/evennia/contrib/rpg/dice/dice.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1442 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/rpg/dice/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.931615 evennia-4.1.1/evennia/contrib/rpg/health_bar/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1264 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/rpg/health_bar/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       94 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/rpg/health_bar/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4913 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/rpg/health_bar/health_bar.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1634 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/rpg/health_bar/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.931615 evennia-4.1.1/evennia/contrib/rpg/llm/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    15039 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/rpg/llm/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       90 2024-03-24 16:21:41.000000 evennia-4.1.1/evennia/contrib/rpg/llm/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     5986 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/rpg/llm/llm_client.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     7444 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/rpg/llm/llm_npc.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1185 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/rpg/llm/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.931615 evennia-4.1.1/evennia/contrib/rpg/rpsystem/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    10331 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/rpg/rpsystem/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      793 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/rpg/rpsystem/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    24723 2024-04-01 15:48:29.000000 evennia-4.1.1/evennia/contrib/rpg/rpsystem/rplanguage.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    59481 2024-04-01 15:48:31.000000 evennia-4.1.1/evennia/contrib/rpg/rpsystem/rpsystem.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    17394 2024-04-01 15:48:31.000000 evennia-4.1.1/evennia/contrib/rpg/rpsystem/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.931615 evennia-4.1.1/evennia/contrib/rpg/traits/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    14247 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/rpg/traits/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      294 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/rpg/traits/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    37184 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/rpg/traits/tests.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    54514 2024-04-01 15:48:29.000000 evennia-4.1.1/evennia/contrib/rpg/traits/traits.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.931615 evennia-4.1.1/evennia/contrib/tutorials/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      151 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/tutorials/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       81 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/tutorials/__init__.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.931615 evennia-4.1.1/evennia/contrib/tutorials/batchprocessor/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1623 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/tutorials/batchprocessor/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       50 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/tutorials/batchprocessor/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1567 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/tutorials/batchprocessor/example_batch_cmds.ev
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      942 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/tutorials/batchprocessor/example_batch_cmds_test.ev
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3618 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/tutorials/batchprocessor/example_batch_code.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.931615 evennia-4.1.1/evennia/contrib/tutorials/bodyfunctions/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      471 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/tutorials/bodyfunctions/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      104 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/tutorials/bodyfunctions/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2312 2024-04-01 15:48:29.000000 evennia-4.1.1/evennia/contrib/tutorials/bodyfunctions/bodyfunctions.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3325 2024-04-01 15:48:29.000000 evennia-4.1.1/evennia/contrib/tutorials/bodyfunctions/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.931615 evennia-4.1.1/evennia/contrib/tutorials/evadventure/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1180 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/tutorials/evadventure/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      164 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/tutorials/evadventure/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3758 2024-04-01 15:48:29.000000 evennia-4.1.1/evennia/contrib/tutorials/evadventure/ai.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.931615 evennia-4.1.1/evennia/contrib/tutorials/evadventure/batchscripts/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       73 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/tutorials/evadventure/batchscripts/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1819 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/tutorials/evadventure/batchscripts/turnbased_combat_demo.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1436 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/tutorials/evadventure/batchscripts/twitch_combat_demo.ev
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3996 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/tutorials/evadventure/build_techdemo.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/tutorials/evadventure/build_world.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    12610 2024-03-30 20:22:07.000000 evennia-4.1.1/evennia/contrib/tutorials/evadventure/characters.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    11181 2024-04-06 11:55:27.000000 evennia-4.1.1/evennia/contrib/tutorials/evadventure/chargen.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    16990 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/tutorials/evadventure/combat_base.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    27740 2024-04-01 15:48:29.000000 evennia-4.1.1/evennia/contrib/tutorials/evadventure/combat_turnbased.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    18271 2024-04-01 15:48:31.000000 evennia-4.1.1/evennia/contrib/tutorials/evadventure/combat_twitch.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    12500 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/tutorials/evadventure/commands.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    17570 2024-04-01 15:48:29.000000 evennia-4.1.1/evennia/contrib/tutorials/evadventure/dungeon.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1743 2024-04-01 15:48:29.000000 evennia-4.1.1/evennia/contrib/tutorials/evadventure/enums.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    14537 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/tutorials/evadventure/equipment.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    12402 2024-04-01 15:48:29.000000 evennia-4.1.1/evennia/contrib/tutorials/evadventure/npcs.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    11174 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/tutorials/evadventure/objects.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    11184 2024-04-01 15:48:29.000000 evennia-4.1.1/evennia/contrib/tutorials/evadventure/quests.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    11708 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/tutorials/evadventure/random_tables.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3154 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/tutorials/evadventure/rooms.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    12130 2024-04-01 15:48:29.000000 evennia-4.1.1/evennia/contrib/tutorials/evadventure/rules.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    17153 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/tutorials/evadventure/shops.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.935615 evennia-4.1.1/evennia/contrib/tutorials/evadventure/tests/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       48 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/tutorials/evadventure/tests/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1389 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/tutorials/evadventure/tests/mixins.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1664 2024-04-01 15:48:29.000000 evennia-4.1.1/evennia/contrib/tutorials/evadventure/tests/test_ai.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1266 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/tutorials/evadventure/tests/test_characters.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2150 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/tutorials/evadventure/tests/test_chargen.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    28160 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/tutorials/evadventure/tests/test_combat.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3742 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/tutorials/evadventure/tests/test_commands.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3322 2024-03-24 14:40:20.000000 evennia-4.1.1/evennia/contrib/tutorials/evadventure/tests/test_dungeon.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     7810 2024-04-01 15:48:29.000000 evennia-4.1.1/evennia/contrib/tutorials/evadventure/tests/test_equipment.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      542 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/tutorials/evadventure/tests/test_npcs.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4159 2024-03-30 22:04:09.000000 evennia-4.1.1/evennia/contrib/tutorials/evadventure/tests/test_quests.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2237 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/tutorials/evadventure/tests/test_rooms.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     8083 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/tutorials/evadventure/tests/test_rules.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      711 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/tutorials/evadventure/tests/test_utils.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2237 2024-04-01 15:48:29.000000 evennia-4.1.1/evennia/contrib/tutorials/evadventure/utils.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.935615 evennia-4.1.1/evennia/contrib/tutorials/mirror/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      429 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/tutorials/mirror/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       83 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/tutorials/mirror/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2235 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/tutorials/mirror/mirror.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.935615 evennia-4.1.1/evennia/contrib/tutorials/red_button/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1344 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/tutorials/red_button/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       94 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/tutorials/red_button/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    18610 2024-04-01 15:48:29.000000 evennia-4.1.1/evennia/contrib/tutorials/red_button/red_button.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.935615 evennia-4.1.1/evennia/contrib/tutorials/talking_npc/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      722 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/tutorials/talking_npc/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      124 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/tutorials/talking_npc/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3697 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/tutorials/talking_npc/talking_npc.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      450 2024-04-01 15:48:29.000000 evennia-4.1.1/evennia/contrib/tutorials/talking_npc/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.935615 evennia-4.1.1/evennia/contrib/tutorials/tutorial_world/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4302 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/tutorials/tutorial_world/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      125 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/tutorials/tutorial_world/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    50297 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/tutorials/tutorial_world/build.ev
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    25399 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/tutorials/tutorial_world/intro_menu.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    16130 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/tutorials/tutorial_world/mob.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    42155 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/tutorials/tutorial_world/objects.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    42921 2024-04-01 15:48:29.000000 evennia-4.1.1/evennia/contrib/tutorials/tutorial_world/rooms.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     7522 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/tutorials/tutorial_world/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.935615 evennia-4.1.1/evennia/contrib/utils/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       67 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/utils/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/utils/__init__.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.935615 evennia-4.1.1/evennia/contrib/utils/auditing/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3303 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/utils/auditing/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/utils/auditing/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2066 2024-04-01 15:48:29.000000 evennia-4.1.1/evennia/contrib/utils/auditing/outputs.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     8516 2024-04-01 15:48:29.000000 evennia-4.1.1/evennia/contrib/utils/auditing/server.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     6047 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/utils/auditing/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.935615 evennia-4.1.1/evennia/contrib/utils/fieldfill/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     5816 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/utils/fieldfill/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      288 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/utils/fieldfill/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    26383 2024-04-01 15:48:29.000000 evennia-4.1.1/evennia/contrib/utils/fieldfill/fieldfill.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.935615 evennia-4.1.1/evennia/contrib/utils/git_integration/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3139 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/utils/git_integration/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       86 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/utils/git_integration/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     7737 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/utils/git_integration/git_integration.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2828 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/utils/git_integration/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.935615 evennia-4.1.1/evennia/contrib/utils/name_generator/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     9815 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/utils/name_generator/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/utils/name_generator/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)   232619 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/utils/name_generator/btn_givennames.txt
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    56503 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/utils/name_generator/btn_surnames.txt
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    14447 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/utils/name_generator/namegen.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4914 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/utils/name_generator/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.935615 evennia-4.1.1/evennia/contrib/utils/random_string_generator/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2165 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/utils/random_string_generator/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      268 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/utils/random_string_generator/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    12591 2024-04-01 15:48:29.000000 evennia-4.1.1/evennia/contrib/utils/random_string_generator/random_string_generator.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      737 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/utils/random_string_generator/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.935615 evennia-4.1.1/evennia/contrib/utils/tree_select/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     5935 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/utils/tree_select/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      109 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/utils/tree_select/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2199 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/utils/tree_select/tests.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    20930 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/contrib/utils/tree_select/tree_select.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.935615 evennia-4.1.1/evennia/game_template/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1521 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/game_template/README.md
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.935615 evennia-4.1.1/evennia/game_template/commands/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      676 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/game_template/commands/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/game_template/commands/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     7738 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/game_template/commands/command.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2636 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/game_template/commands/default_cmdsets.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      576 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/game_template/gitignore
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.935615 evennia-4.1.1/evennia/game_template/server/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1718 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/game_template/server/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       24 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/game_template/server/__init__.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.935615 evennia-4.1.1/evennia/game_template/server/conf/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       24 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/game_template/server/conf/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      629 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/game_template/server/conf/at_initial_setup.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2154 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/game_template/server/conf/at_search.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1369 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/game_template/server/conf/at_server_startstop.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2174 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/game_template/server/conf/cmdparser.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1500 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/game_template/server/conf/connection_screens.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1159 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/game_template/server/conf/inlinefuncs.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1419 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/game_template/server/conf/inputfuncs.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1065 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/game_template/server/conf/lockfuncs.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3979 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/game_template/server/conf/mssp.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      709 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/game_template/server/conf/portal_services_plugins.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      714 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/game_template/server/conf/secret_settings.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      705 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/game_template/server/conf/server_services_plugins.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1347 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/game_template/server/conf/serversession.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1545 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/game_template/server/conf/settings.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1185 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/game_template/server/conf/web_plugins.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.935615 evennia-4.1.1/evennia/game_template/server/logs/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      839 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/game_template/server/logs/README.md
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.935615 evennia-4.1.1/evennia/game_template/typeclasses/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      733 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/game_template/typeclasses/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/game_template/typeclasses/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3774 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/game_template/typeclasses/accounts.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2920 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/game_template/typeclasses/channels.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1524 2024-04-01 15:48:29.000000 evennia-4.1.1/evennia/game_template/typeclasses/characters.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2045 2024-04-01 15:48:29.000000 evennia-4.1.1/evennia/game_template/typeclasses/exits.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     8848 2024-04-01 15:48:29.000000 evennia-4.1.1/evennia/game_template/typeclasses/objects.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      562 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/game_template/typeclasses/rooms.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4394 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/game_template/typeclasses/scripts.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.935615 evennia-4.1.1/evennia/game_template/web/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2939 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/game_template/web/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/game_template/web/__init__.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.939615 evennia-4.1.1/evennia/game_template/web/admin/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      296 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/game_template/web/admin/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/game_template/web/admin/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      519 2024-04-01 15:48:29.000000 evennia-4.1.1/evennia/game_template/web/admin/urls.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.939615 evennia-4.1.1/evennia/game_template/web/api/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/game_template/web/api/__init__.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.939615 evennia-4.1.1/evennia/game_template/web/static/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      849 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/game_template/web/static/README.md
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.915615 evennia-4.1.1/evennia/game_template/web/static/rest_framework/
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.939615 evennia-4.1.1/evennia/game_template/web/static/rest_framework/css/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       53 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/game_template/web/static/rest_framework/css/README.md
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.939615 evennia-4.1.1/evennia/game_template/web/static/rest_framework/images/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       47 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/game_template/web/static/rest_framework/images/README.md
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.915615 evennia-4.1.1/evennia/game_template/web/static/webclient/
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.939615 evennia-4.1.1/evennia/game_template/web/static/webclient/css/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      132 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/game_template/web/static/webclient/css/README.md
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.939615 evennia-4.1.1/evennia/game_template/web/static/webclient/js/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      143 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/game_template/web/static/webclient/js/README.md
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.915615 evennia-4.1.1/evennia/game_template/web/static/website/
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.939615 evennia-4.1.1/evennia/game_template/web/static/website/css/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      129 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/game_template/web/static/website/css/README.md
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.939615 evennia-4.1.1/evennia/game_template/web/static/website/images/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      135 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/game_template/web/static/website/images/README.md
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.939615 evennia-4.1.1/evennia/game_template/web/templates/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      760 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/game_template/web/templates/README.md
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.939615 evennia-4.1.1/evennia/game_template/web/templates/rest_framework/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       58 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/game_template/web/templates/rest_framework/README.md
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.939615 evennia-4.1.1/evennia/game_template/web/templates/webclient/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      223 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/game_template/web/templates/webclient/README.md
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.939615 evennia-4.1.1/evennia/game_template/web/templates/website/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      217 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/game_template/web/templates/website/README.md
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.939615 evennia-4.1.1/evennia/game_template/web/templates/website/flatpages/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      185 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/game_template/web/templates/website/flatpages/README.md
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.939615 evennia-4.1.1/evennia/game_template/web/templates/website/registration/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      152 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/game_template/web/templates/website/registration/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1100 2024-04-01 15:48:29.000000 evennia-4.1.1/evennia/game_template/web/urls.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.939615 evennia-4.1.1/evennia/game_template/web/webclient/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1102 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/game_template/web/webclient/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/game_template/web/webclient/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      539 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/game_template/web/webclient/urls.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.939615 evennia-4.1.1/evennia/game_template/web/website/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1262 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/game_template/web/website/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/game_template/web/website/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      509 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/game_template/web/website/urls.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.939615 evennia-4.1.1/evennia/game_template/web/website/views/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/game_template/web/website/views/__init__.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.939615 evennia-4.1.1/evennia/game_template/world/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      467 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/game_template/world/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/game_template/world/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      999 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/game_template/world/batch_cmds.ev
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1936 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/game_template/world/help_entries.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3646 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/game_template/world/prototypes.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.939615 evennia-4.1.1/evennia/help/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      217 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/help/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     8021 2024-03-30 14:56:23.000000 evennia-4.1.1/evennia/help/filehelp.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     6230 2024-04-01 15:48:29.000000 evennia-4.1.1/evennia/help/manager.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.939615 evennia-4.1.1/evennia/help/migrations/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2222 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/help/migrations/0001_initial.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      577 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/help/migrations/0002_auto_20170606_1731.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1688 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/help/migrations/0003_auto_20190128_1820.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      540 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/help/migrations/0004_auto_20210520_2137.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1166 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/help/migrations/0005_auto_20210530_1818.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      473 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/help/migrations/0006_alter_helpentry_id.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       24 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/help/migrations/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     9730 2024-04-01 15:48:29.000000 evennia-4.1.1/evennia/help/models.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3744 2024-03-30 14:56:23.000000 evennia-4.1.1/evennia/help/tests.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     7686 2024-04-01 15:48:29.000000 evennia-4.1.1/evennia/help/utils.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.939615 evennia-4.1.1/evennia/locale/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2686 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/locale/README
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.915615 evennia-4.1.1/evennia/locale/de/
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.939615 evennia-4.1.1/evennia/locale/de/LC_MESSAGES/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    10764 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/locale/de/LC_MESSAGES/django.mo
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    14475 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/locale/de/LC_MESSAGES/django.po
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.915615 evennia-4.1.1/evennia/locale/es/
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.939615 evennia-4.1.1/evennia/locale/es/LC_MESSAGES/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3821 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/locale/es/LC_MESSAGES/django.mo
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    30981 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/locale/es/LC_MESSAGES/django.po
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.915615 evennia-4.1.1/evennia/locale/fr/
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.939615 evennia-4.1.1/evennia/locale/fr/LC_MESSAGES/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    26255 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/locale/fr/LC_MESSAGES/django.mo
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    38581 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/locale/fr/LC_MESSAGES/django.po
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.915615 evennia-4.1.1/evennia/locale/it/
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.939615 evennia-4.1.1/evennia/locale/it/LC_MESSAGES/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     6944 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/locale/it/LC_MESSAGES/django.mo
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    35844 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/locale/it/LC_MESSAGES/django.po
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.915615 evennia-4.1.1/evennia/locale/ko/
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.939615 evennia-4.1.1/evennia/locale/ko/LC_MESSAGES/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3569 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/locale/ko/LC_MESSAGES/django.mo
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    30924 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/locale/ko/LC_MESSAGES/django.po
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.915615 evennia-4.1.1/evennia/locale/la/
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.939615 evennia-4.1.1/evennia/locale/la/LC_MESSAGES/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     6537 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/locale/la/LC_MESSAGES/django.mo
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    32786 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/locale/la/LC_MESSAGES/django.po
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.915615 evennia-4.1.1/evennia/locale/pl/
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.939615 evennia-4.1.1/evennia/locale/pl/LC_MESSAGES/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1631 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/locale/pl/LC_MESSAGES/django.mo
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    28236 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/locale/pl/LC_MESSAGES/django.po
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.915615 evennia-4.1.1/evennia/locale/pt/
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.939615 evennia-4.1.1/evennia/locale/pt/LC_MESSAGES/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    25584 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/locale/pt/LC_MESSAGES/django.mo
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    42122 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/locale/pt/LC_MESSAGES/django.po
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.915615 evennia-4.1.1/evennia/locale/ru/
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.939615 evennia-4.1.1/evennia/locale/ru/LC_MESSAGES/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2281 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/locale/ru/LC_MESSAGES/django.mo
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    29419 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/locale/ru/LC_MESSAGES/django.po
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.915615 evennia-4.1.1/evennia/locale/sv/
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.939615 evennia-4.1.1/evennia/locale/sv/LC_MESSAGES/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    29036 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/locale/sv/LC_MESSAGES/django.mo
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    43353 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/locale/sv/LC_MESSAGES/django.po
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.915615 evennia-4.1.1/evennia/locale/zh/
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.939615 evennia-4.1.1/evennia/locale/zh/LC_MESSAGES/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3300 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/locale/zh/LC_MESSAGES/django.mo
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    30540 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/locale/zh/LC_MESSAGES/django.po
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.939615 evennia-4.1.1/evennia/locks/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      240 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/locks/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    22155 2024-04-01 15:48:29.000000 evennia-4.1.1/evennia/locks/lockfuncs.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    27271 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/locks/lockhandler.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    13732 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/locks/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.939615 evennia-4.1.1/evennia/objects/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      120 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/objects/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    29653 2024-04-01 15:48:32.000000 evennia-4.1.1/evennia/objects/manager.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.943616 evennia-4.1.1/evennia/objects/migrations/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4315 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/objects/migrations/0001_initial.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1193 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/objects/migrations/0002_auto_20140917_0756.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      810 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/objects/migrations/0003_defaultcharacter_defaultexit_defaultobject_defaultroom.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      530 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/objects/migrations/0004_auto_20150118_1622.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      410 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/objects/migrations/0005_auto_20150403_2339.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1599 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/objects/migrations/0006_auto_20170606_1731.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1203 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/objects/migrations/0007_objectdb_db_account.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      757 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/objects/migrations/0008_auto_20170705_1736.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      643 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/objects/migrations/0009_remove_objectdb_db_player.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     5028 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/objects/migrations/0010_auto_20190128_1820.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1351 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/objects/migrations/0011_auto_20191025_0831.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4011 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/objects/migrations/0012_convert_contrib_typeclass_paths.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      488 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/objects/migrations/0013_defaultobject_alter_objectdb_id_defaultcharacter_and_more.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/objects/migrations/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    13400 2024-04-01 15:48:32.000000 evennia-4.1.1/evennia/objects/models.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)   131845 2024-04-06 11:55:27.000000 evennia-4.1.1/evennia/objects/objects.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    25362 2024-04-06 20:15:54.000000 evennia-4.1.1/evennia/objects/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.943616 evennia-4.1.1/evennia/prototypes/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     6567 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/prototypes/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/prototypes/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    92096 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/prototypes/menus.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2912 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/prototypes/protfuncs.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    46538 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/prototypes/prototypes.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    42851 2024-04-01 15:48:30.000000 evennia-4.1.1/evennia/prototypes/spawner.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    39629 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/prototypes/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.943616 evennia-4.1.1/evennia/scripts/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      229 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/scripts/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    11275 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/scripts/manager.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.943616 evennia-4.1.1/evennia/scripts/migrations/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4762 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/scripts/migrations/0001_initial.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      675 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/scripts/migrations/0002_auto_20150118_1625.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1507 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/scripts/migrations/0003_checksessions_defaultscript_donothing_scriptbase_store_validatechannelhandler_validateidmappercache_.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      861 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/scripts/migrations/0004_auto_20150306_1354.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      430 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/scripts/migrations/0005_auto_20150306_1441.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      710 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/scripts/migrations/0006_auto_20150310_2249.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      396 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/scripts/migrations/0007_auto_20150403_2339.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      913 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/scripts/migrations/0008_auto_20170606_1731.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1271 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/scripts/migrations/0009_scriptdb_db_account.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      757 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/scripts/migrations/0010_auto_20170705_1736.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      596 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/scripts/migrations/0011_remove_scriptdb_db_player.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4655 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/scripts/migrations/0012_auto_20190128_1820.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      666 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/scripts/migrations/0013_auto_20191025_0831.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      752 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/scripts/migrations/0014_auto_20210520_2137.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3329 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/scripts/migrations/0015_convert_contrib_paths.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      478 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/scripts/migrations/0016_scriptbase_alter_scriptdb_id_defaultscript_and_more.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       24 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/scripts/migrations/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     6312 2024-04-01 15:48:29.000000 evennia-4.1.1/evennia/scripts/models.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     8762 2024-04-01 15:48:29.000000 evennia-4.1.1/evennia/scripts/monitorhandler.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    27363 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/scripts/ondemandhandler.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     5510 2024-04-01 15:48:29.000000 evennia-4.1.1/evennia/scripts/scripthandler.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    27674 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/scripts/scripts.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    20794 2024-04-01 15:48:29.000000 evennia-4.1.1/evennia/scripts/taskhandler.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    26185 2024-04-01 15:48:32.000000 evennia-4.1.1/evennia/scripts/tests.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    24662 2024-04-01 15:48:30.000000 evennia-4.1.1/evennia/scripts/tickerhandler.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.943616 evennia-4.1.1/evennia/server/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      234 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/server/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     8753 2024-04-05 22:13:15.000000 evennia-4.1.1/evennia/server/amp_client.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    16628 2024-04-01 15:48:30.000000 evennia-4.1.1/evennia/server/connection_wizard.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     8129 2024-04-01 15:48:29.000000 evennia-4.1.1/evennia/server/deprecations.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    79878 2024-04-06 11:54:05.000000 evennia-4.1.1/evennia/server/evennia_launcher.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.943616 evennia-4.1.1/evennia/server/game_index_client/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4321 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/server/game_index_client/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       45 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/server/game_index_client/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     6182 2024-04-01 15:48:29.000000 evennia-4.1.1/evennia/server/game_index_client/client.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1988 2024-04-01 15:48:29.000000 evennia-4.1.1/evennia/server/game_index_client/service.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     7406 2024-04-01 15:48:29.000000 evennia-4.1.1/evennia/server/initial_setup.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    20403 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/server/inputfuncs.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1846 2024-04-01 15:48:29.000000 evennia-4.1.1/evennia/server/manager.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.943616 evennia-4.1.1/evennia/server/migrations/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      812 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/server/migrations/0001_initial.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1363 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/server/migrations/0002_auto_20190128_2311.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      478 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/server/migrations/0003_alter_serverconfig_id.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       24 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/server/migrations/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3819 2024-04-01 15:48:29.000000 evennia-4.1.1/evennia/server/models.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.947615 evennia-4.1.1/evennia/server/portal/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       24 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/server/portal/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    17922 2024-04-05 22:13:15.000000 evennia-4.1.1/evennia/server/portal/amp.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    18288 2024-04-06 11:55:27.000000 evennia-4.1.1/evennia/server/portal/amp_server.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    19120 2024-04-01 15:48:30.000000 evennia-4.1.1/evennia/server/portal/discord.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    11344 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/server/portal/grapevine.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    14242 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/server/portal/irc.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2572 2024-04-01 15:48:29.000000 evennia-4.1.1/evennia/server/portal/mccp.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3883 2024-04-01 15:48:29.000000 evennia-4.1.1/evennia/server/portal/mssp.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2342 2024-04-01 15:48:29.000000 evennia-4.1.1/evennia/server/portal/mxp.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2360 2024-04-01 15:48:29.000000 evennia-4.1.1/evennia/server/portal/naws.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1168 2024-04-01 15:48:29.000000 evennia-4.1.1/evennia/server/portal/portal.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    17379 2024-04-01 15:48:30.000000 evennia-4.1.1/evennia/server/portal/portalsessionhandler.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4451 2024-04-01 15:48:30.000000 evennia-4.1.1/evennia/server/portal/rss.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    14930 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/server/portal/service.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    15898 2024-04-01 15:48:32.000000 evennia-4.1.1/evennia/server/portal/ssh.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3320 2024-04-01 15:48:29.000000 evennia-4.1.1/evennia/server/portal/ssl.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1787 2024-04-01 15:48:29.000000 evennia-4.1.1/evennia/server/portal/suppress_ga.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    17380 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/server/portal/telnet.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    15610 2024-04-01 15:48:30.000000 evennia-4.1.1/evennia/server/portal/telnet_oob.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4751 2024-04-01 15:48:30.000000 evennia-4.1.1/evennia/server/portal/telnet_ssl.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    15494 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/server/portal/tests.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     7073 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/server/portal/ttype.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    11522 2024-04-01 15:48:30.000000 evennia-4.1.1/evennia/server/portal/webclient.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    16166 2024-04-01 15:48:30.000000 evennia-4.1.1/evennia/server/portal/webclient_ajax.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.947615 evennia-4.1.1/evennia/server/profiling/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      212 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/server/profiling/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/server/profiling/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    20879 2024-04-01 15:48:30.000000 evennia-4.1.1/evennia/server/profiling/dummyrunner.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     9428 2024-04-01 15:48:30.000000 evennia-4.1.1/evennia/server/profiling/dummyrunner_settings.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3923 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/server/profiling/memplot.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1375 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/server/profiling/settings_mixin.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1094 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/server/profiling/test_queries.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     5371 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/server/profiling/tests.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1345 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/server/profiling/timetrace.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1167 2024-04-01 15:48:30.000000 evennia-4.1.1/evennia/server/server.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    16593 2024-04-01 15:48:30.000000 evennia-4.1.1/evennia/server/serversession.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    27031 2024-04-06 11:55:27.000000 evennia-4.1.1/evennia/server/service.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     5617 2024-04-01 15:48:30.000000 evennia-4.1.1/evennia/server/session.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    30267 2024-04-01 15:48:30.000000 evennia-4.1.1/evennia/server/sessionhandler.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     5391 2024-04-01 15:48:30.000000 evennia-4.1.1/evennia/server/signals.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.947615 evennia-4.1.1/evennia/server/tests/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/server/tests/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     5193 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/server/tests/test_amp_connection.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      521 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/server/tests/test_initial_setup.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     7305 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/server/tests/test_launcher.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3814 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/server/tests/test_misc.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     8859 2024-04-01 15:48:30.000000 evennia-4.1.1/evennia/server/tests/test_server.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      985 2024-04-01 15:48:30.000000 evennia-4.1.1/evennia/server/tests/testrunner.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     7101 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/server/throttle.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1216 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/server/validators.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     8654 2024-04-01 15:48:30.000000 evennia-4.1.1/evennia/server/webserver.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    62336 2024-04-01 15:48:30.000000 evennia-4.1.1/evennia/settings_default.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.947615 evennia-4.1.1/evennia/typeclasses/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      434 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/typeclasses/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    64960 2024-04-06 20:24:30.000000 evennia-4.1.1/evennia/typeclasses/attributes.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    31305 2024-04-01 15:48:30.000000 evennia-4.1.1/evennia/typeclasses/managers.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.947615 evennia-4.1.1/evennia/typeclasses/migrations/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     6101 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/typeclasses/migrations/0001_initial.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      768 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/typeclasses/migrations/0002_auto_20150109_0913.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2266 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/typeclasses/migrations/0003_defaultcharacter_defaultexit_defaultguest_defaultobject_defaultplayer_defaultroom_defaultscript_dono.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      833 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/typeclasses/migrations/0004_auto_20151101_1759.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      922 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/typeclasses/migrations/0005_auto_20160625_1812.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1444 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/typeclasses/migrations/0006_auto_add_dbmodel_value_for_tags_attributes.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3899 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/typeclasses/migrations/0007_tag_migrations_may_be_slow.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1699 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/typeclasses/migrations/0008_lock_and_perm_rename.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4230 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/typeclasses/migrations/0009_rename_player_cmdsets_typeclasses.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1993 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/typeclasses/migrations/0010_delete_old_player_tables.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     5265 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/typeclasses/migrations/0011_auto_20190128_1820.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      821 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/typeclasses/migrations/0012_attrs_to_picklev4_may_be_slow.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      592 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/typeclasses/migrations/0013_auto_20191015_1922.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      592 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/typeclasses/migrations/0014_alter_tag_db_category.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      362 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/typeclasses/migrations/0015_alter_attribute_options.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      722 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/typeclasses/migrations/0016_alter_attribute_id_alter_tag_id.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       24 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/typeclasses/migrations/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    37171 2024-04-01 15:48:30.000000 evennia-4.1.1/evennia/typeclasses/models.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    30234 2024-04-01 15:48:30.000000 evennia-4.1.1/evennia/typeclasses/tags.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    17814 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/typeclasses/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.947615 evennia-4.1.1/evennia/utils/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      320 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/utils/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    51450 2024-04-01 15:48:31.000000 evennia-4.1.1/evennia/utils/ansi.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    15393 2024-04-01 15:48:30.000000 evennia-4.1.1/evennia/utils/batchprocessors.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     7755 2024-04-01 15:48:30.000000 evennia-4.1.1/evennia/utils/containers.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    10242 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/utils/create.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    32815 2024-04-01 15:48:30.000000 evennia-4.1.1/evennia/utils/dbserialize.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    41870 2024-04-06 11:55:27.000000 evennia-4.1.1/evennia/utils/eveditor.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2734 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/utils/evennia-mode.el
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    21381 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/utils/evform.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    80600 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/utils/evmenu.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    18832 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/utils/evmore.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    65172 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/utils/evtable.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    55430 2024-04-01 15:48:31.000000 evennia-4.1.1/evennia/utils/funcparser.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     8754 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/utils/gametime.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.947615 evennia-4.1.1/evennia/utils/idmapper/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1309 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/utils/idmapper/LICENSE.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1097 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/utils/idmapper/README_evennia.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1992 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/utils/idmapper/README_orig.rst
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       64 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/utils/idmapper/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1182 2024-04-01 15:48:30.000000 evennia-4.1.1/evennia/utils/idmapper/manager.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    24820 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/utils/idmapper/models.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2875 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/utils/idmapper/tests.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    18788 2024-04-01 15:48:30.000000 evennia-4.1.1/evennia/utils/logger.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    10324 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/utils/optionclasses.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     6519 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/utils/optionhandler.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    11093 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/utils/picklefield.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    14179 2024-03-31 10:02:22.000000 evennia-4.1.1/evennia/utils/search.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    25825 2024-04-01 15:48:32.000000 evennia-4.1.1/evennia/utils/test_resources.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.951615 evennia-4.1.1/evennia/utils/tests/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/utils/tests/__init__.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.951615 evennia-4.1.1/evennia/utils/tests/data/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/utils/tests/data/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      274 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/utils/tests/data/broken_script.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1125 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/utils/tests/data/evform_example.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     6245 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/utils/tests/data/evmenu_example.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      382 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/utils/tests/data/prototypes_example.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1608 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/utils/tests/test_ansi.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     7052 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/utils/tests/test_batchprocessors.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3463 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/utils/tests/test_containers.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     7030 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/utils/tests/test_create_functions.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     7888 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/utils/tests/test_dbserialize.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    14444 2024-04-01 15:48:30.000000 evennia-4.1.1/evennia/utils/tests/test_eveditor.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    12171 2024-04-01 15:48:30.000000 evennia-4.1.1/evennia/utils/tests/test_evform.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    11764 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/utils/tests/test_evmenu.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    12705 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/utils/tests/test_evtable.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    31687 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/utils/tests/test_funcparser.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3942 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/utils/tests/test_gametime.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4460 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/utils/tests/test_search.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    13565 2024-04-01 15:48:30.000000 evennia-4.1.1/evennia/utils/tests/test_tagparsing.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     5509 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/utils/tests/test_text2html.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    33293 2024-04-01 15:48:32.000000 evennia-4.1.1/evennia/utils/tests/test_utils.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     6370 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/utils/tests/test_validatorfuncs.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    12235 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/utils/text2html.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)   102284 2024-04-01 15:48:32.000000 evennia-4.1.1/evennia/utils/utils.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     9489 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/utils/validatorfuncs.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.951615 evennia-4.1.1/evennia/utils/verb_conjugation/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    18011 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/utils/verb_conjugation/LICENSE.txt
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/utils/verb_conjugation/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     9944 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/utils/verb_conjugation/conjugate.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    11299 2024-04-01 15:48:30.000000 evennia-4.1.1/evennia/utils/verb_conjugation/pronouns.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    10493 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/utils/verb_conjugation/tests.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)   554408 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/utils/verb_conjugation/verbs.txt
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.951615 evennia-4.1.1/evennia/web/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1150 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/web/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      127 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/web/__init__.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.951615 evennia-4.1.1/evennia/web/admin/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      428 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/web/admin/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    14125 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/web/admin/accounts.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     8627 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/web/admin/attributes.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     8508 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/web/admin/comms.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      593 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/web/admin/frontpage.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1890 2024-04-01 15:48:30.000000 evennia-4.1.1/evennia/web/admin/help.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    11705 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/web/admin/objects.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4498 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/web/admin/scripts.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      508 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/web/admin/server.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     8954 2024-04-01 15:48:30.000000 evennia-4.1.1/evennia/web/admin/tags.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      878 2024-04-01 15:48:30.000000 evennia-4.1.1/evennia/web/admin/urls.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2884 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/web/admin/utils.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.951615 evennia-4.1.1/evennia/web/api/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     7674 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/web/api/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/web/api/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4268 2024-04-01 15:48:30.000000 evennia-4.1.1/evennia/web/api/filters.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3948 2024-04-01 15:48:30.000000 evennia-4.1.1/evennia/web/api/permissions.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      277 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/web/api/root.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     9905 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/web/api/serializers.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     8147 2024-04-01 15:48:30.000000 evennia-4.1.1/evennia/web/api/tests.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2293 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/web/api/urls.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     5829 2024-04-01 15:48:30.000000 evennia-4.1.1/evennia/web/api/views.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.915615 evennia-4.1.1/evennia/web/static/
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.915615 evennia-4.1.1/evennia/web/static/rest_framework/
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.951615 evennia-4.1.1/evennia/web/static/rest_framework/css/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      298 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/web/static/rest_framework/css/api.css
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.951615 evennia-4.1.1/evennia/web/static/rest_framework/images/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1406 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/web/static/rest_framework/images/favicon.ico
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.915615 evennia-4.1.1/evennia/web/static/webclient/
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.951615 evennia-4.1.1/evennia/web/static/webclient/css/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/web/static/webclient/css/custom.css
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2104 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/web/static/webclient/css/goldenlayout.css
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    27268 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/web/static/webclient/css/webclient.css
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.951615 evennia-4.1.1/evennia/web/static/webclient/fonts/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    22208 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/web/static/webclient/fonts/DejaVuSansMono-webfont.woff
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      185 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/web/static/webclient/fonts/DejaVuSansMono.css
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.951615 evennia-4.1.1/evennia/web/static/webclient/js/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    18677 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/web/static/webclient/js/evennia.js
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.951615 evennia-4.1.1/evennia/web/static/webclient/js/plugins/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      563 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/web/static/webclient/js/plugins/clienthelp.js
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3914 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/web/static/webclient/js/plugins/default_in.js
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1967 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/web/static/webclient/js/plugins/default_out.js
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      345 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/web/static/webclient/js/plugins/default_unload.js
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3785 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/web/static/webclient/js/plugins/font.js
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    30344 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/web/static/webclient/js/plugins/goldenlayout.js
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2114 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/web/static/webclient/js/plugins/goldenlayout_default_config.js
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2981 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/web/static/webclient/js/plugins/history.js
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     5031 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/web/static/webclient/js/plugins/hotbuttons.js
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1969 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/web/static/webclient/js/plugins/html.js
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1912 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/web/static/webclient/js/plugins/iframe.js
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4666 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/web/static/webclient/js/plugins/message_routing.js
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4611 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/web/static/webclient/js/plugins/multimedia.js
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2842 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/web/static/webclient/js/plugins/notifications.js
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      909 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/web/static/webclient/js/plugins/oob.js
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     6262 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/web/static/webclient/js/plugins/options2.js
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2790 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/web/static/webclient/js/plugins/popups.js
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    10949 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/web/static/webclient/js/plugins/text2html.js
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     9615 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/web/static/webclient/js/webclient_gui.js
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.951615 evennia-4.1.1/evennia/web/static/webclient/media/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3624 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/web/static/webclient/media/notification.wav
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.915615 evennia-4.1.1/evennia/web/static/website/
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.951615 evennia-4.1.1/evennia/web/static/website/css/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/web/static/website/css/custom.css
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2013 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/web/static/website/css/website.css
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.951615 evennia-4.1.1/evennia/web/static/website/images/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      266 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/web/static/website/images/LICENCE
+-rwxrwxr-x   0 griatch   (1000) griatch   (1000)    17938 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/web/static/website/images/evennia_logo.png
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    21167 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/web/static/website/images/evennia_logo_festive.png
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1406 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/web/static/website/images/favicon.ico
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.915615 evennia-4.1.1/evennia/web/templates/
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.951615 evennia-4.1.1/evennia/web/templates/admin/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1621 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/web/templates/admin/app_list.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     6462 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/web/templates/admin/frontpage.html
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.955615 evennia-4.1.1/evennia/web/templates/rest_framework/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      903 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/web/templates/rest_framework/api.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      417 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/web/templates/rest_framework/redoc.html
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.955615 evennia-4.1.1/evennia/web/templates/webclient/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     8353 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/web/templates/webclient/base.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1058 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/web/templates/webclient/webclient.html
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.955615 evennia-4.1.1/evennia/web/templates/website/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      510 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/web/templates/website/404.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      614 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/web/templates/website/500.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4059 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/web/templates/website/_menu.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3132 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/web/templates/website/base.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2858 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/web/templates/website/channel_detail.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2667 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/web/templates/website/channel_list.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1402 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/web/templates/website/character_form.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      546 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/web/templates/website/character_list.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1139 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/web/templates/website/character_manage_list.html
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.955615 evennia-4.1.1/evennia/web/templates/website/flatpages/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      341 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/web/templates/website/flatpages/default.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1501 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/web/templates/website/generic_form.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2715 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/web/templates/website/help_detail.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     5052 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/web/templates/website/help_list.html
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.955615 evennia-4.1.1/evennia/web/templates/website/homepage/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      593 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/web/templates/website/homepage/accounts-widget.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      574 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/web/templates/website/homepage/database-stats-widget.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      542 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/web/templates/website/homepage/evennia-widget.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1980 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/web/templates/website/homepage/main-content.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      387 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/web/templates/website/homepage/recently-connected-widget.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      952 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/web/templates/website/index.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      180 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/web/templates/website/messages.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      900 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/web/templates/website/object_confirm_delete.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1034 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/web/templates/website/object_detail.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      546 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/web/templates/website/object_list.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1484 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/web/templates/website/pagination.html
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.955615 evennia-4.1.1/evennia/web/templates/website/registration/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      942 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/web/templates/website/registration/logged_out.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1957 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/web/templates/website/registration/login.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      612 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/web/templates/website/registration/password_change_done.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1422 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/web/templates/website/registration/password_change_form.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      813 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/web/templates/website/registration/password_reset_complete.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1747 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/web/templates/website/registration/password_reset_confirm.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1185 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/web/templates/website/registration/password_reset_done.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      566 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/web/templates/website/registration/password_reset_email.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1577 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/web/templates/website/registration/password_reset_form.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1895 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/web/templates/website/registration/register.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      671 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/web/templates/website/tbi.html
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.955615 evennia-4.1.1/evennia/web/templatetags/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      287 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/web/templatetags/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/web/templatetags/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      550 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/web/templatetags/addclass.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1631 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/web/urls.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.955615 evennia-4.1.1/evennia/web/utils/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/web/utils/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1353 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/web/utils/adminsite.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      596 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/web/utils/apache_wsgi.conf
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1815 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/web/utils/backends.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2035 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/web/utils/evennia_modpy_apache.conf
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1819 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/web/utils/evennia_wsgi_apache.conf
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4130 2024-04-01 15:48:32.000000 evennia-4.1.1/evennia/web/utils/general_context.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3144 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/web/utils/middleware.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2444 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/web/utils/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.955615 evennia-4.1.1/evennia/web/webclient/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/web/webclient/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      210 2024-04-01 15:48:30.000000 evennia-4.1.1/evennia/web/webclient/urls.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      795 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/web/webclient/views.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.955615 evennia-4.1.1/evennia/web/website/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       31 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/web/website/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     5737 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/web/website/forms.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    12375 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/web/website/tests.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2576 2024-04-01 15:48:30.000000 evennia-4.1.1/evennia/web/website/urls.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.955615 evennia-4.1.1/evennia/web/website/views/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       24 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/web/website/views/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2120 2024-04-01 15:48:30.000000 evennia-4.1.1/evennia/web/website/views/accounts.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     5329 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/web/website/views/channels.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     8802 2024-04-01 15:48:32.000000 evennia-4.1.1/evennia/web/website/views/characters.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      311 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/web/website/views/errors.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    11790 2024-04-01 15:48:30.000000 evennia-4.1.1/evennia/web/website/views/help.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4611 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/web/website/views/index.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2354 2024-04-01 15:48:30.000000 evennia-4.1.1/evennia/web/website/views/mixins.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     9037 2024-03-17 13:16:37.000000 evennia-4.1.1/evennia/web/website/views/objects.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2024-04-06 21:07:27.955615 evennia-4.1.1/evennia.egg-info/
+-rw-r--r--   0 griatch   (1000) griatch   (1000)     6510 2024-04-06 21:07:27.000000 evennia-4.1.1/evennia.egg-info/PKG-INFO
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    35956 2024-04-06 21:07:27.000000 evennia-4.1.1/evennia.egg-info/SOURCES.txt
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        1 2024-04-06 21:07:27.000000 evennia-4.1.1/evennia.egg-info/dependency_links.txt
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      562 2024-04-06 21:07:27.000000 evennia-4.1.1/evennia.egg-info/requires.txt
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        8 2024-04-06 21:07:27.000000 evennia-4.1.1/evennia.egg-info/top_level.txt
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3979 2024-04-06 21:02:36.000000 evennia-4.1.1/pyproject.toml
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       38 2024-04-06 21:07:27.959616 evennia-4.1.1/setup.cfg
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1388 2024-03-17 13:16:37.000000 evennia-4.1.1/setup.py
```

### Comparing `evennia-4.1.0/LICENSE.txt` & `evennia-4.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/PKG-INFO` & `evennia-4.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evennia
-Version: 4.1.0
+Version: 4.1.1
 Summary: A full-featured toolkit and server for text-based multiplayer games (MUDs, MU*, etc).
 Maintainer-email: Griatch <griatch@gmail.com>
 License: BSD
 Project-URL: Homepage, https://www.evennia.com
 Project-URL: Github, https://github.com/evennia/evennia
 Project-URL: Documentation, https://www.evennia.com/docs/latest/index.html
 Project-URL: Live Demo, https://demo.evennia.com/
```

### Comparing `evennia-4.1.0/README.md` & `evennia-4.1.1/README.md`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/__init__.py` & `evennia-4.1.1/evennia/__init__.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/__main__.py` & `evennia-4.1.1/evennia/__main__.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/accounts/accounts.py` & `evennia-4.1.1/evennia/accounts/accounts.py`

 * *Files 1% similar despite different names*

```diff
@@ -369,14 +369,26 @@
         if session:
             return bool(session.protocol_flags.get("SCREENREADER", False))
         else:
             return any(
                 session.protocol_flags.get("SCREENREADER") for session in self.sessions.all()
             )
 
+    def get_extra_display_name_info(self, looker, **kwargs):
+        """
+        Used in .get_display_name() to provide extra information to the looker. We split this
+        to be consistent with the Object version of this method.
+
+        This is used e.g. by the `find` command by default.
+
+        """
+        if looker and self.locks.check_lockstring(looker, "perm(Admin)"):
+            return f"(#{self.id})"
+        return ""
+
     def get_display_name(self, looker, **kwargs):
         """
         This is used by channels and other OOC communications methods to give a
         custom display of this account's input.
 
         Args:
             looker (Account): The one that will see this name.
```

### Comparing `evennia-4.1.0/evennia/accounts/bots.py` & `evennia-4.1.1/evennia/accounts/bots.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/accounts/manager.py` & `evennia-4.1.1/evennia/accounts/manager.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/accounts/migrations/0001_initial.py` & `evennia-4.1.1/evennia/accounts/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/accounts/migrations/0003_auto_20150209_2234.py` & `evennia-4.1.1/evennia/accounts/migrations/0003_auto_20150209_2234.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/accounts/migrations/0004_auto_20150403_2339.py` & `evennia-4.1.1/evennia/accounts/migrations/0004_auto_20150403_2339.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/accounts/migrations/0005_auto_20160905_0902.py` & `evennia-4.1.1/evennia/accounts/migrations/0005_auto_20160905_0902.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/accounts/migrations/0006_auto_20170606_1731.py` & `evennia-4.1.1/evennia/accounts/migrations/0006_auto_20170606_1731.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/accounts/migrations/0007_copy_player_to_account.py` & `evennia-4.1.1/evennia/accounts/migrations/0007_copy_player_to_account.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/accounts/migrations/0008_auto_20190128_1820.py` & `evennia-4.1.1/evennia/accounts/migrations/0008_auto_20190128_1820.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/accounts/migrations/0009_auto_20191025_0831.py` & `evennia-4.1.1/evennia/accounts/migrations/0009_auto_20191025_0831.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/accounts/migrations/0011_convert_contrib_typeclass_paths.py` & `evennia-4.1.1/evennia/accounts/migrations/0011_convert_contrib_typeclass_paths.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/accounts/models.py` & `evennia-4.1.1/evennia/accounts/models.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/accounts/tests.py` & `evennia-4.1.1/evennia/accounts/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/commands/cmdhandler.py` & `evennia-4.1.1/evennia/commands/cmdhandler.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/commands/cmdparser.py` & `evennia-4.1.1/evennia/commands/cmdparser.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/commands/cmdset.py` & `evennia-4.1.1/evennia/commands/cmdset.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/commands/cmdsethandler.py` & `evennia-4.1.1/evennia/commands/cmdsethandler.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/commands/command.py` & `evennia-4.1.1/evennia/commands/command.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/commands/default/account.py` & `evennia-4.1.1/evennia/commands/default/account.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/commands/default/admin.py` & `evennia-4.1.1/evennia/commands/default/admin.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/commands/default/batchprocess.py` & `evennia-4.1.1/evennia/commands/default/batchprocess.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/commands/default/building.py` & `evennia-4.1.1/evennia/commands/default/building.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,15 @@
     "CmdScripts",
     "CmdObjects",
     "CmdTag",
     "CmdSpawn",
 )
 
 # used by set
-from ast import literal_eval as _LITERAL_EVAL
+from ast import literal_eval as _LITERAL_EVAL  # noqa
 
 LIST_APPEND_CHAR = "+"
 
 # used by find
 CHAR_TYPECLASS = settings.BASE_CHARACTER_TYPECLASS
 ROOM_TYPECLASS = settings.BASE_ROOM_TYPECLASS
 EXIT_TYPECLASS = settings.BASE_EXIT_TYPECLASS
@@ -1401,15 +1401,15 @@
             new_home = self.caller.search(self.rhs, global_search=True)
             if not new_home:
                 return
             old_home = obj.home
             obj.home = new_home
             if old_home:
                 string = (
-                    f"Home location of {obj} was changed from {old_home}({old_home.dbref} to"
+                    f"Home location of {obj} was changed from {old_home}({old_home.dbref}) to"
                     f" {new_home}({new_home.dbref})."
                 )
             else:
                 string = f"Home location of {obj} was set to {new_home}({new_home.dbref})."
         self.msg(string)
 
 
@@ -3278,17 +3278,23 @@
 
             if not result:
                 string += "\n   |RNo match found.|n"
             elif not low <= int(result[0].id) <= high:
                 string += f"\n   |RNo match found for '{searchstring}' in #dbref interval.|n"
             else:
                 result = result[0]
-                string += f"\n|g   {result.get_display_name(caller)} - {result.path}|n"
+                string += (
+                    f"\n|g   {result.get_display_name(caller)}"
+                    f"{result.get_extra_display_name_info(caller)} - {result.path}|n"
+                )
                 if "loc" in self.switches and not is_account and result.location:
-                    string += f" (|wlocation|n: |g{result.location.get_display_name(caller)}|n)"
+                    string += (
+                        f" (|wlocation|n: |g{result.location.get_display_name(caller)}"
+                        f"{result.get_extra_display_name_info(caller)}|n)"
+                    )
         else:
             # Not an account/dbref search but a wider search; build a queryset.
             # Searches for key and aliases
             if "exact" in switches:
                 keyquery = Q(db_key__iexact=searchstring, id__gte=low, id__lte=high)
                 aliasquery = Q(
                     db_tags__db_key__iexact=searchstring,
```

### Comparing `evennia-4.1.0/evennia/commands/default/cmdset_account.py` & `evennia-4.1.1/evennia/commands/default/cmdset_account.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/commands/default/cmdset_character.py` & `evennia-4.1.1/evennia/commands/default/cmdset_character.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/commands/default/cmdset_unloggedin.py` & `evennia-4.1.1/evennia/commands/default/cmdset_unloggedin.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/commands/default/comms.py` & `evennia-4.1.1/evennia/commands/default/comms.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/commands/default/general.py` & `evennia-4.1.1/evennia/commands/default/general.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """
 General Character commands usually available to all characters
 """
 
 import re
 
-import evennia
 from django.conf import settings
+
+import evennia
 from evennia.typeclasses.attributes import NickTemplateInvalid
 from evennia.utils import utils
 
 COMMAND_DEFAULT_CLASS = utils.class_from_module(settings.COMMAND_DEFAULT_CLASS)
 
 # limit symbol import for API
 __all__ = (
@@ -393,15 +394,15 @@
         For example, if the input string is "3 apples", this parser will set `self.number = 3` and
         `self.args = "apples"`. If the input string is "apples", this parser will set
         `self.number = 0` and `self.args = "apples"`.
 
         """
         super().parse()
         self.number = 0
-        if hasattr(self, "lhs"):
+        if getattr(self, "lhs", None):
             # handle self.lhs but don't require it
             count, *args = self.lhs.split(maxsplit=1)
             # we only use the first word as a count if it's a number and
             # there is more text afterwards
             if args and count.isdecimal():
                 self.number = int(count)
                 self.lhs = args[0]
```

### Comparing `evennia-4.1.0/evennia/commands/default/help.py` & `evennia-4.1.1/evennia/commands/default/help.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/commands/default/muxcommand.py` & `evennia-4.1.1/evennia/commands/default/muxcommand.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/commands/default/syscommands.py` & `evennia-4.1.1/evennia/commands/default/syscommands.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/commands/default/system.py` & `evennia-4.1.1/evennia/commands/default/system.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/commands/default/tests.py` & `evennia-4.1.1/evennia/commands/default/tests.py`

 * *Files 1% similar despite different names*

```diff
@@ -130,14 +130,25 @@
         self.call(general.CmdGive(), "Obj to Char2", "You give")
         self.call(general.CmdGive(), "Obj = Char", "You give", caller=self.char2)
         # test stacking
         self.obj2.key = "Obj"
         self.obj2.location = self.char1
         self.call(general.CmdGive(), "2 Obj = Char2", "You give two Objs")
 
+    def test_numbered_target_command(self):
+        class CmdTest(general.NumberedTargetCommand):
+            key = "test"
+
+            def func(self):
+                self.msg(f"Number: {self.number} Args: {self.args}")
+
+        self.call(CmdTest(), "", "Number: 0 Args: ")
+        self.call(CmdTest(), "obj", "Number: 0 Args: obj")
+        self.call(CmdTest(), "1 obj", "Number: 1 Args: obj")
+
     def test_mux_command(self):
         class CmdTest(MuxCommand):
             key = "test"
             switch_options = ("test", "testswitch", "testswitch2")
 
             def func(self):
                 self.msg("Switches matched: {}".format(self.switches))
```

### Comparing `evennia-4.1.0/evennia/commands/default/unloggedin.py` & `evennia-4.1.1/evennia/commands/default/unloggedin.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/commands/tests.py` & `evennia-4.1.1/evennia/commands/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/comms/comms.py` & `evennia-4.1.1/evennia/comms/comms.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/comms/managers.py` & `evennia-4.1.1/evennia/comms/managers.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/comms/migrations/0001_initial.py` & `evennia-4.1.1/evennia/comms/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/comms/migrations/0003_auto_20140917_0756.py` & `evennia-4.1.1/evennia/comms/migrations/0003_auto_20140917_0756.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/comms/migrations/0005_auto_20150223_1517.py` & `evennia-4.1.1/evennia/comms/migrations/0005_auto_20150223_1517.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/comms/migrations/0006_channeldb_db_object_subscriptions.py` & `evennia-4.1.1/evennia/comms/migrations/0006_channeldb_db_object_subscriptions.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/comms/migrations/0007_msg_db_tags.py` & `evennia-4.1.1/evennia/comms/migrations/0007_msg_db_tags.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/comms/migrations/0009_auto_20160921_1731.py` & `evennia-4.1.1/evennia/comms/migrations/0009_auto_20160921_1731.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/comms/migrations/0010_auto_20161206_1912.py` & `evennia-4.1.1/evennia/comms/migrations/0010_auto_20161206_1912.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/comms/migrations/0011_auto_20170217_2039.py` & `evennia-4.1.1/evennia/comms/migrations/0011_auto_20170217_2039.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/comms/migrations/0011_auto_20170606_1731.py` & `evennia-4.1.1/evennia/comms/migrations/0011_auto_20170606_1731.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/comms/migrations/0013_auto_20170705_1726.py` & `evennia-4.1.1/evennia/comms/migrations/0013_auto_20170705_1726.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/comms/migrations/0014_auto_20170705_1736.py` & `evennia-4.1.1/evennia/comms/migrations/0014_auto_20170705_1736.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/comms/migrations/0015_auto_20170706_2041.py` & `evennia-4.1.1/evennia/comms/migrations/0015_auto_20170706_2041.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/comms/migrations/0017_auto_20190128_1820.py` & `evennia-4.1.1/evennia/comms/migrations/0017_auto_20190128_1820.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/comms/migrations/0018_auto_20191025_0831.py` & `evennia-4.1.1/evennia/comms/migrations/0018_auto_20191025_0831.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/comms/migrations/0019_auto_20210514_2032.py` & `evennia-4.1.1/evennia/comms/migrations/0019_auto_20210514_2032.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/comms/migrations/0020_auto_20210514_2210.py` & `evennia-4.1.1/evennia/comms/migrations/0020_auto_20210514_2210.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/comms/migrations/0021_auto_20210520_2137.py` & `evennia-4.1.1/evennia/comms/migrations/0021_auto_20210520_2137.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/comms/migrations/0022_defaultchannel_alter_channeldb_id_alter_msg_id_and_more.py` & `evennia-4.1.1/evennia/comms/migrations/0022_defaultchannel_alter_channeldb_id_alter_msg_id_and_more.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/comms/models.py` & `evennia-4.1.1/evennia/comms/models.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/comms/tests.py` & `evennia-4.1.1/evennia/comms/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/README.md` & `evennia-4.1.1/evennia/contrib/README.md`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/base_systems/awsstorage/README.md` & `evennia-4.1.1/evennia/contrib/base_systems/awsstorage/README.md`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/base_systems/awsstorage/aws_s3_cdn.py` & `evennia-4.1.1/evennia/contrib/base_systems/awsstorage/aws_s3_cdn.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/base_systems/awsstorage/tests.py` & `evennia-4.1.1/evennia/contrib/base_systems/awsstorage/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/base_systems/building_menu/README.md` & `evennia-4.1.1/evennia/contrib/base_systems/building_menu/README.md`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/base_systems/building_menu/building_menu.py` & `evennia-4.1.1/evennia/contrib/base_systems/building_menu/building_menu.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/base_systems/building_menu/tests.py` & `evennia-4.1.1/evennia/contrib/base_systems/building_menu/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/base_systems/color_markups/README.md` & `evennia-4.1.1/evennia/contrib/base_systems/color_markups/README.md`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/base_systems/color_markups/color_markups.py` & `evennia-4.1.1/evennia/contrib/base_systems/color_markups/color_markups.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/base_systems/color_markups/tests.py` & `evennia-4.1.1/evennia/contrib/base_systems/color_markups/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/base_systems/components/README.md` & `evennia-4.1.1/evennia/contrib/base_systems/components/README.md`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/base_systems/components/__init__.py` & `evennia-4.1.1/evennia/contrib/base_systems/components/__init__.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/base_systems/components/component.py` & `evennia-4.1.1/evennia/contrib/base_systems/components/component.py`

 * *Files 3% similar despite different names*

```diff
@@ -152,14 +152,30 @@
         Returns:
             AttributeHandler: The Host's AttributeHandler
 
         """
         return self.host.attributes
 
     @property
+    def pk(self):
+        """
+        Shortcut property returning the host's primary key.
+
+        Returns:
+            int: The Host's primary key.
+
+        Notes:
+            This is requried to allow AttributeProperties to correctly update `_SaverMutable` data
+            (like lists) in-place (since the DBField sits on the Component which doesn't itself
+            have a primary key, this save operation would otherwise fail).
+
+        """
+        return self.host.pk
+
+    @property
     def nattributes(self):
         """
         Shortcut property returning the host's In-Memory AttributeHandler (Non Persisted).
 
         Returns:
             AttributeHandler: The Host's In-Memory AttributeHandler
```

### Comparing `evennia-4.1.0/evennia/contrib/base_systems/components/dbfield.py` & `evennia-4.1.1/evennia/contrib/base_systems/components/dbfield.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 Components - ChrisLR 2022
 
 This file contains the Descriptors used to set Fields in Components
 """
 
 import typing
 
-from evennia.typeclasses.attributes import AttributeProperty, NAttributeProperty
+from evennia.typeclasses.attributes import (AttributeProperty,
+                                            NAttributeProperty)
 
 if typing.TYPE_CHECKING:
     from .components import Component
 
 
 class DBField(AttributeProperty):
     """
```

### Comparing `evennia-4.1.0/evennia/contrib/base_systems/components/holder.py` & `evennia-4.1.1/evennia/contrib/base_systems/components/holder.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/base_systems/components/listing.py` & `evennia-4.1.1/evennia/contrib/base_systems/components/listing.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/base_systems/components/signals.py` & `evennia-4.1.1/evennia/contrib/base_systems/components/signals.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/base_systems/components/tests.py` & `evennia-4.1.1/evennia/contrib/base_systems/components/tests.py`

 * *Files 1% similar despite different names*

```diff
@@ -264,15 +264,15 @@
         )
         self.assertTrue(self.char1.tags.has(key="first value", category="test_b::multiple_tags"))
         self.assertTrue(self.char1.tags.has(key="second value", category="test_b::multiple_tags"))
         self.assertTrue(self.char1.tags.has(key="third value", category="test_b::multiple_tags"))
 
     def test_mutables_are_not_shared_when_autocreate(self):
         self.char1.test_a.my_list.append(1)
-        self.assertNotEqual(self.char1.test_a.my_list, self.char2.test_a.my_list)
+        self.assertNotEqual(id(self.char1.test_a.my_list), id(self.char2.test_a.my_list))
 
     def test_replacing_class_component_slot_with_runtime_component(self):
         self.char1.components.add_default("replacement_inherited_test_a")
         self.assertEqual(self.char1.ic_a.replacement_field, 6)
 
 
 class CharWithSignal(ComponentHolderMixin, DefaultCharacter):
```

### Comparing `evennia-4.1.0/evennia/contrib/base_systems/custom_gametime/README.md` & `evennia-4.1.1/evennia/contrib/base_systems/custom_gametime/README.md`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/base_systems/custom_gametime/custom_gametime.py` & `evennia-4.1.1/evennia/contrib/base_systems/custom_gametime/custom_gametime.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/base_systems/custom_gametime/tests.py` & `evennia-4.1.1/evennia/contrib/base_systems/custom_gametime/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/base_systems/email_login/README.md` & `evennia-4.1.1/evennia/contrib/base_systems/email_login/README.md`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/base_systems/email_login/connection_screens.py` & `evennia-4.1.1/evennia/contrib/base_systems/email_login/connection_screens.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/base_systems/email_login/email_login.py` & `evennia-4.1.1/evennia/contrib/base_systems/email_login/email_login.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/base_systems/email_login/tests.py` & `evennia-4.1.1/evennia/contrib/base_systems/email_login/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/base_systems/godotwebsocket/README.md` & `evennia-4.1.1/evennia/contrib/base_systems/godotwebsocket/README.md`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/base_systems/godotwebsocket/__init__.py` & `evennia-4.1.1/evennia/contrib/base_systems/godotwebsocket/__init__.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/base_systems/godotwebsocket/test_text2bbcode.py` & `evennia-4.1.1/evennia/contrib/base_systems/godotwebsocket/test_text2bbcode.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/base_systems/godotwebsocket/test_webclient.py` & `evennia-4.1.1/evennia/contrib/base_systems/godotwebsocket/test_webclient.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/base_systems/godotwebsocket/text2bbcode.py` & `evennia-4.1.1/evennia/contrib/base_systems/godotwebsocket/text2bbcode.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/base_systems/godotwebsocket/webclient.py` & `evennia-4.1.1/evennia/contrib/base_systems/godotwebsocket/webclient.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/base_systems/ingame_python/README.md` & `evennia-4.1.1/evennia/contrib/base_systems/ingame_python/README.md`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/base_systems/ingame_python/callbackhandler.py` & `evennia-4.1.1/evennia/contrib/base_systems/ingame_python/callbackhandler.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/base_systems/ingame_python/commands.py` & `evennia-4.1.1/evennia/contrib/base_systems/ingame_python/commands.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/base_systems/ingame_python/eventfuncs.py` & `evennia-4.1.1/evennia/contrib/base_systems/ingame_python/eventfuncs.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/base_systems/ingame_python/scripts.py` & `evennia-4.1.1/evennia/contrib/base_systems/ingame_python/scripts.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/base_systems/ingame_python/tests.py` & `evennia-4.1.1/evennia/contrib/base_systems/ingame_python/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/base_systems/ingame_python/typeclasses.py` & `evennia-4.1.1/evennia/contrib/base_systems/ingame_python/typeclasses.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/base_systems/ingame_python/utils.py` & `evennia-4.1.1/evennia/contrib/base_systems/ingame_python/utils.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/base_systems/menu_login/README.md` & `evennia-4.1.1/evennia/contrib/base_systems/menu_login/README.md`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/base_systems/menu_login/connection_screens.py` & `evennia-4.1.1/evennia/contrib/base_systems/menu_login/connection_screens.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/base_systems/menu_login/menu_login.py` & `evennia-4.1.1/evennia/contrib/base_systems/menu_login/menu_login.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/base_systems/mux_comms_cmds/README.md` & `evennia-4.1.1/evennia/contrib/base_systems/mux_comms_cmds/README.md`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/base_systems/mux_comms_cmds/mux_comms_cmds.py` & `evennia-4.1.1/evennia/contrib/base_systems/mux_comms_cmds/mux_comms_cmds.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/base_systems/mux_comms_cmds/tests.py` & `evennia-4.1.1/evennia/contrib/base_systems/mux_comms_cmds/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/base_systems/unixcommand/README.md` & `evennia-4.1.1/evennia/contrib/base_systems/unixcommand/README.md`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/base_systems/unixcommand/tests.py` & `evennia-4.1.1/evennia/contrib/base_systems/unixcommand/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/base_systems/unixcommand/unixcommand.py` & `evennia-4.1.1/evennia/contrib/base_systems/unixcommand/unixcommand.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/full_systems/evscaperoom/README.md` & `evennia-4.1.1/evennia/contrib/full_systems/evscaperoom/README.md`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/full_systems/evscaperoom/commands.py` & `evennia-4.1.1/evennia/contrib/full_systems/evscaperoom/commands.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/full_systems/evscaperoom/menu.py` & `evennia-4.1.1/evennia/contrib/full_systems/evscaperoom/menu.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/full_systems/evscaperoom/objects.py` & `evennia-4.1.1/evennia/contrib/full_systems/evscaperoom/objects.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/full_systems/evscaperoom/room.py` & `evennia-4.1.1/evennia/contrib/full_systems/evscaperoom/room.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/full_systems/evscaperoom/scripts.py` & `evennia-4.1.1/evennia/contrib/full_systems/evscaperoom/scripts.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/full_systems/evscaperoom/state.py` & `evennia-4.1.1/evennia/contrib/full_systems/evscaperoom/state.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/full_systems/evscaperoom/states/README.md` & `evennia-4.1.1/evennia/contrib/full_systems/evscaperoom/states/README.md`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/full_systems/evscaperoom/states/state_001_start.py` & `evennia-4.1.1/evennia/contrib/full_systems/evscaperoom/states/state_001_start.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/full_systems/evscaperoom/tests.py` & `evennia-4.1.1/evennia/contrib/full_systems/evscaperoom/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/full_systems/evscaperoom/utils.py` & `evennia-4.1.1/evennia/contrib/full_systems/evscaperoom/utils.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/game_systems/barter/README.md` & `evennia-4.1.1/evennia/contrib/game_systems/barter/README.md`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/game_systems/barter/barter.py` & `evennia-4.1.1/evennia/contrib/game_systems/barter/barter.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/game_systems/barter/tests.py` & `evennia-4.1.1/evennia/contrib/game_systems/barter/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/game_systems/clothing/README.md` & `evennia-4.1.1/evennia/contrib/game_systems/clothing/README.md`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/game_systems/clothing/clothing.py` & `evennia-4.1.1/evennia/contrib/game_systems/clothing/clothing.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/game_systems/clothing/tests.py` & `evennia-4.1.1/evennia/contrib/game_systems/clothing/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/game_systems/containers/README.md` & `evennia-4.1.1/evennia/contrib/game_systems/containers/README.md`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/game_systems/containers/containers.py` & `evennia-4.1.1/evennia/contrib/game_systems/containers/containers.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/game_systems/containers/tests.py` & `evennia-4.1.1/evennia/contrib/game_systems/containers/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/game_systems/cooldowns/README.md` & `evennia-4.1.1/evennia/contrib/game_systems/cooldowns/README.md`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/game_systems/cooldowns/cooldowns.py` & `evennia-4.1.1/evennia/contrib/game_systems/cooldowns/cooldowns.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/game_systems/cooldowns/tests.py` & `evennia-4.1.1/evennia/contrib/game_systems/cooldowns/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/game_systems/crafting/README.md` & `evennia-4.1.1/evennia/contrib/game_systems/crafting/README.md`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/game_systems/crafting/crafting.py` & `evennia-4.1.1/evennia/contrib/game_systems/crafting/crafting.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/game_systems/crafting/example_recipes.py` & `evennia-4.1.1/evennia/contrib/game_systems/crafting/example_recipes.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/game_systems/crafting/tests.py` & `evennia-4.1.1/evennia/contrib/game_systems/crafting/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/game_systems/gendersub/README.md` & `evennia-4.1.1/evennia/contrib/game_systems/gendersub/README.md`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/game_systems/gendersub/gendersub.py` & `evennia-4.1.1/evennia/contrib/game_systems/gendersub/gendersub.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/game_systems/gendersub/tests.py` & `evennia-4.1.1/evennia/contrib/game_systems/gendersub/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/game_systems/mail/README.md` & `evennia-4.1.1/evennia/contrib/game_systems/mail/README.md`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/game_systems/mail/mail.py` & `evennia-4.1.1/evennia/contrib/game_systems/mail/mail.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/game_systems/mail/tests.py` & `evennia-4.1.1/evennia/contrib/game_systems/mail/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/game_systems/multidescer/README.md` & `evennia-4.1.1/evennia/contrib/game_systems/multidescer/README.md`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/game_systems/multidescer/multidescer.py` & `evennia-4.1.1/evennia/contrib/game_systems/multidescer/multidescer.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/game_systems/multidescer/tests.py` & `evennia-4.1.1/evennia/contrib/game_systems/multidescer/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/game_systems/puzzles/README.md` & `evennia-4.1.1/evennia/contrib/game_systems/puzzles/README.md`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/game_systems/puzzles/puzzles.py` & `evennia-4.1.1/evennia/contrib/game_systems/puzzles/puzzles.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/game_systems/puzzles/tests.py` & `evennia-4.1.1/evennia/contrib/game_systems/puzzles/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/game_systems/turnbattle/README.md` & `evennia-4.1.1/evennia/contrib/game_systems/turnbattle/README.md`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/game_systems/turnbattle/tb_basic.py` & `evennia-4.1.1/evennia/contrib/game_systems/turnbattle/tb_basic.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/game_systems/turnbattle/tb_equip.py` & `evennia-4.1.1/evennia/contrib/game_systems/turnbattle/tb_equip.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/game_systems/turnbattle/tb_items.py` & `evennia-4.1.1/evennia/contrib/game_systems/turnbattle/tb_items.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/game_systems/turnbattle/tb_magic.py` & `evennia-4.1.1/evennia/contrib/game_systems/turnbattle/tb_magic.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/game_systems/turnbattle/tb_range.py` & `evennia-4.1.1/evennia/contrib/game_systems/turnbattle/tb_range.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/game_systems/turnbattle/tests.py` & `evennia-4.1.1/evennia/contrib/game_systems/turnbattle/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/grid/extended_room/README.md` & `evennia-4.1.1/evennia/contrib/grid/extended_room/README.md`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/grid/extended_room/extended_room.py` & `evennia-4.1.1/evennia/contrib/grid/extended_room/extended_room.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/grid/extended_room/tests.py` & `evennia-4.1.1/evennia/contrib/grid/extended_room/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/grid/ingame_map_display/README.md` & `evennia-4.1.1/evennia/contrib/grid/ingame_map_display/README.md`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/grid/ingame_map_display/ingame_map_display.py` & `evennia-4.1.1/evennia/contrib/grid/ingame_map_display/ingame_map_display.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/grid/ingame_map_display/tests.py` & `evennia-4.1.1/evennia/contrib/grid/ingame_map_display/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/grid/mapbuilder/README.md` & `evennia-4.1.1/evennia/contrib/grid/mapbuilder/README.md`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/grid/mapbuilder/mapbuilder.py` & `evennia-4.1.1/evennia/contrib/grid/mapbuilder/mapbuilder.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/grid/mapbuilder/tests.py` & `evennia-4.1.1/evennia/contrib/grid/mapbuilder/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/grid/simpledoor/README.md` & `evennia-4.1.1/evennia/contrib/grid/simpledoor/README.md`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/grid/simpledoor/simpledoor.py` & `evennia-4.1.1/evennia/contrib/grid/simpledoor/simpledoor.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/grid/simpledoor/tests.py` & `evennia-4.1.1/evennia/contrib/grid/simpledoor/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/grid/slow_exit/README.md` & `evennia-4.1.1/evennia/contrib/grid/slow_exit/README.md`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/grid/slow_exit/slow_exit.py` & `evennia-4.1.1/evennia/contrib/grid/slow_exit/slow_exit.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/grid/slow_exit/tests.py` & `evennia-4.1.1/evennia/contrib/grid/slow_exit/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/grid/wilderness/README.md` & `evennia-4.1.1/evennia/contrib/grid/wilderness/README.md`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/grid/wilderness/tests.py` & `evennia-4.1.1/evennia/contrib/grid/wilderness/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/grid/wilderness/wilderness.py` & `evennia-4.1.1/evennia/contrib/grid/wilderness/wilderness.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/grid/xyzgrid/README.md` & `evennia-4.1.1/evennia/contrib/grid/xyzgrid/README.md`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/grid/xyzgrid/commands.py` & `evennia-4.1.1/evennia/contrib/grid/xyzgrid/commands.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/grid/xyzgrid/example.py` & `evennia-4.1.1/evennia/contrib/grid/xyzgrid/example.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/grid/xyzgrid/launchcmd.py` & `evennia-4.1.1/evennia/contrib/grid/xyzgrid/launchcmd.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/grid/xyzgrid/prototypes.py` & `evennia-4.1.1/evennia/contrib/grid/xyzgrid/prototypes.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/grid/xyzgrid/tests.py` & `evennia-4.1.1/evennia/contrib/grid/xyzgrid/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/grid/xyzgrid/utils.py` & `evennia-4.1.1/evennia/contrib/grid/xyzgrid/utils.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/grid/xyzgrid/xymap.py` & `evennia-4.1.1/evennia/contrib/grid/xyzgrid/xymap.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/grid/xyzgrid/xymap_legend.py` & `evennia-4.1.1/evennia/contrib/grid/xyzgrid/xymap_legend.py`

 * *Files 0% similar despite different names*

```diff
@@ -323,14 +323,21 @@
                     f"The prototype {self.prototype} for this node has no 'typeclass' key.", self
                 )
             self.log(f"  spawning room at xyz={xyz} ({typeclass})")
             Typeclass = class_from_module(typeclass)
             nodeobj, err = Typeclass.create(self.prototype.get("key", "An empty room"), xyz=xyz)
             if err:
                 raise RuntimeError(err)
+        except django_exceptions.MultipleObjectsReturned:
+            raise MapError(
+                f"Multiple objects found: {NodeTypeclass.objects.filter_xyz(xyz=xyz)}. "
+                "This may be due to manual creation of XYZRooms at this position. "
+                "Delete duplicates.",
+                self,
+            )
         else:
             self.log(f"  updating existing room (if changed) at xyz={xyz}")
 
         if not self.prototype.get("prototype_key"):
             # make sure there is a prototype_key in prototype
             self.prototype["prototype_key"] = self.generate_prototype_key()
```

### Comparing `evennia-4.1.0/evennia/contrib/grid/xyzgrid/xyzgrid.py` & `evennia-4.1.1/evennia/contrib/grid/xyzgrid/xyzgrid.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/grid/xyzgrid/xyzroom.py` & `evennia-4.1.1/evennia/contrib/grid/xyzgrid/xyzroom.py`

 * *Files 0% similar despite different names*

```diff
@@ -279,15 +279,15 @@
     map_separator_char = "|x~|n"
 
     def __str__(self):
         return repr(self)
 
     def __repr__(self):
         x, y, z = self.xyz
-        return f"<XYZRoom '{self.db_key}', XYZ=({x},{y},{z})>"
+        return f"<{self.__class__.__name__} '{self.db_key}', XYZ=({x},{y},{z})>"
 
     @property
     def xyz(self):
         if not hasattr(self, "_xyz"):
             x = self.tags.get(category=MAP_X_TAG_CATEGORY, return_list=False)
             y = self.tags.get(category=MAP_Y_TAG_CATEGORY, return_list=False)
             z = self.tags.get(category=MAP_Z_TAG_CATEGORY, return_list=False)
```

### Comparing `evennia-4.1.0/evennia/contrib/rpg/buffs/README.md` & `evennia-4.1.1/evennia/contrib/rpg/buffs/README.md`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/rpg/buffs/buff.py` & `evennia-4.1.1/evennia/contrib/rpg/buffs/buff.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/rpg/buffs/samplebuffs.py` & `evennia-4.1.1/evennia/contrib/rpg/buffs/samplebuffs.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/rpg/buffs/tests.py` & `evennia-4.1.1/evennia/contrib/rpg/buffs/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/rpg/character_creator/README.md` & `evennia-4.1.1/evennia/contrib/rpg/character_creator/README.md`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/rpg/character_creator/character_creator.py` & `evennia-4.1.1/evennia/contrib/rpg/character_creator/character_creator.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/rpg/character_creator/example_menu.py` & `evennia-4.1.1/evennia/contrib/rpg/character_creator/example_menu.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/rpg/character_creator/tests.py` & `evennia-4.1.1/evennia/contrib/rpg/character_creator/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/rpg/dice/README.md` & `evennia-4.1.1/evennia/contrib/rpg/dice/README.md`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/rpg/dice/dice.py` & `evennia-4.1.1/evennia/contrib/rpg/dice/dice.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/rpg/dice/tests.py` & `evennia-4.1.1/evennia/contrib/rpg/dice/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/rpg/health_bar/README.md` & `evennia-4.1.1/evennia/contrib/rpg/health_bar/README.md`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/rpg/health_bar/health_bar.py` & `evennia-4.1.1/evennia/contrib/rpg/health_bar/health_bar.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/rpg/health_bar/tests.py` & `evennia-4.1.1/evennia/contrib/rpg/health_bar/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/rpg/llm/README.md` & `evennia-4.1.1/evennia/contrib/rpg/llm/README.md`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/rpg/llm/llm_client.py` & `evennia-4.1.1/evennia/contrib/rpg/llm/llm_client.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/rpg/llm/llm_npc.py` & `evennia-4.1.1/evennia/contrib/rpg/llm/llm_npc.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/rpg/llm/tests.py` & `evennia-4.1.1/evennia/contrib/rpg/llm/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/rpg/rpsystem/README.md` & `evennia-4.1.1/evennia/contrib/rpg/rpsystem/README.md`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/rpg/rpsystem/__init__.py` & `evennia-4.1.1/evennia/contrib/rpg/rpsystem/__init__.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/rpg/rpsystem/rplanguage.py` & `evennia-4.1.1/evennia/contrib/rpg/rpsystem/rplanguage.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/rpg/rpsystem/rpsystem.py` & `evennia-4.1.1/evennia/contrib/rpg/rpsystem/rpsystem.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/rpg/rpsystem/tests.py` & `evennia-4.1.1/evennia/contrib/rpg/rpsystem/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/rpg/traits/README.md` & `evennia-4.1.1/evennia/contrib/rpg/traits/README.md`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/rpg/traits/tests.py` & `evennia-4.1.1/evennia/contrib/rpg/traits/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/rpg/traits/traits.py` & `evennia-4.1.1/evennia/contrib/rpg/traits/traits.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/tutorials/batchprocessor/README.md` & `evennia-4.1.1/evennia/contrib/tutorials/batchprocessor/README.md`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/tutorials/batchprocessor/example_batch_cmds.ev` & `evennia-4.1.1/evennia/contrib/tutorials/batchprocessor/example_batch_cmds.ev`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/tutorials/batchprocessor/example_batch_cmds_test.ev` & `evennia-4.1.1/evennia/contrib/tutorials/batchprocessor/example_batch_cmds_test.ev`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/tutorials/batchprocessor/example_batch_code.py` & `evennia-4.1.1/evennia/contrib/tutorials/batchprocessor/example_batch_code.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/tutorials/bodyfunctions/bodyfunctions.py` & `evennia-4.1.1/evennia/contrib/tutorials/bodyfunctions/bodyfunctions.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/tutorials/bodyfunctions/tests.py` & `evennia-4.1.1/evennia/contrib/tutorials/bodyfunctions/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/tutorials/evadventure/README.md` & `evennia-4.1.1/evennia/contrib/tutorials/evadventure/README.md`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/tutorials/evadventure/ai.py` & `evennia-4.1.1/evennia/contrib/tutorials/evadventure/ai.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/tutorials/evadventure/batchscripts/turnbased_combat_demo.py` & `evennia-4.1.1/evennia/contrib/tutorials/evadventure/batchscripts/turnbased_combat_demo.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/tutorials/evadventure/batchscripts/twitch_combat_demo.ev` & `evennia-4.1.1/evennia/contrib/tutorials/evadventure/batchscripts/twitch_combat_demo.ev`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/tutorials/evadventure/build_techdemo.py` & `evennia-4.1.1/evennia/contrib/tutorials/evadventure/build_techdemo.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/tutorials/evadventure/characters.py` & `evennia-4.1.1/evennia/contrib/tutorials/evadventure/characters.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/tutorials/evadventure/chargen.py` & `evennia-4.1.1/evennia/contrib/tutorials/evadventure/chargen.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/tutorials/evadventure/combat_base.py` & `evennia-4.1.1/evennia/contrib/tutorials/evadventure/combat_base.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/tutorials/evadventure/combat_turnbased.py` & `evennia-4.1.1/evennia/contrib/tutorials/evadventure/combat_turnbased.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/tutorials/evadventure/combat_twitch.py` & `evennia-4.1.1/evennia/contrib/tutorials/evadventure/combat_twitch.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/tutorials/evadventure/commands.py` & `evennia-4.1.1/evennia/contrib/tutorials/evadventure/commands.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/tutorials/evadventure/dungeon.py` & `evennia-4.1.1/evennia/contrib/tutorials/evadventure/dungeon.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/tutorials/evadventure/enums.py` & `evennia-4.1.1/evennia/contrib/tutorials/evadventure/enums.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/tutorials/evadventure/equipment.py` & `evennia-4.1.1/evennia/contrib/tutorials/evadventure/equipment.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/tutorials/evadventure/npcs.py` & `evennia-4.1.1/evennia/contrib/tutorials/evadventure/npcs.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/tutorials/evadventure/objects.py` & `evennia-4.1.1/evennia/contrib/tutorials/evadventure/objects.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/tutorials/evadventure/quests.py` & `evennia-4.1.1/evennia/contrib/tutorials/evadventure/quests.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/tutorials/evadventure/random_tables.py` & `evennia-4.1.1/evennia/contrib/tutorials/evadventure/random_tables.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/tutorials/evadventure/rooms.py` & `evennia-4.1.1/evennia/contrib/tutorials/evadventure/rooms.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/tutorials/evadventure/rules.py` & `evennia-4.1.1/evennia/contrib/tutorials/evadventure/rules.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/tutorials/evadventure/shops.py` & `evennia-4.1.1/evennia/contrib/tutorials/evadventure/shops.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/tutorials/evadventure/tests/mixins.py` & `evennia-4.1.1/evennia/contrib/tutorials/evadventure/tests/mixins.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/tutorials/evadventure/tests/test_ai.py` & `evennia-4.1.1/evennia/contrib/tutorials/evadventure/tests/test_ai.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/tutorials/evadventure/tests/test_characters.py` & `evennia-4.1.1/evennia/contrib/tutorials/evadventure/tests/test_characters.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/tutorials/evadventure/tests/test_chargen.py` & `evennia-4.1.1/evennia/contrib/tutorials/evadventure/tests/test_chargen.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/tutorials/evadventure/tests/test_combat.py` & `evennia-4.1.1/evennia/contrib/tutorials/evadventure/tests/test_combat.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/tutorials/evadventure/tests/test_commands.py` & `evennia-4.1.1/evennia/contrib/tutorials/evadventure/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/tutorials/evadventure/tests/test_dungeon.py` & `evennia-4.1.1/evennia/contrib/tutorials/evadventure/tests/test_dungeon.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/tutorials/evadventure/tests/test_equipment.py` & `evennia-4.1.1/evennia/contrib/tutorials/evadventure/tests/test_equipment.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/tutorials/evadventure/tests/test_npcs.py` & `evennia-4.1.1/evennia/contrib/tutorials/evadventure/tests/test_npcs.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/tutorials/evadventure/tests/test_quests.py` & `evennia-4.1.1/evennia/contrib/tutorials/evadventure/tests/test_quests.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/tutorials/evadventure/tests/test_rooms.py` & `evennia-4.1.1/evennia/contrib/tutorials/evadventure/tests/test_rooms.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/tutorials/evadventure/tests/test_rules.py` & `evennia-4.1.1/evennia/contrib/tutorials/evadventure/tests/test_rules.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/tutorials/evadventure/tests/test_utils.py` & `evennia-4.1.1/evennia/contrib/tutorials/evadventure/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/tutorials/evadventure/utils.py` & `evennia-4.1.1/evennia/contrib/tutorials/evadventure/utils.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/tutorials/mirror/mirror.py` & `evennia-4.1.1/evennia/contrib/tutorials/mirror/mirror.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/tutorials/red_button/README.md` & `evennia-4.1.1/evennia/contrib/tutorials/red_button/README.md`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/tutorials/red_button/red_button.py` & `evennia-4.1.1/evennia/contrib/tutorials/red_button/red_button.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/tutorials/talking_npc/README.md` & `evennia-4.1.1/evennia/contrib/tutorials/talking_npc/README.md`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/tutorials/talking_npc/talking_npc.py` & `evennia-4.1.1/evennia/contrib/tutorials/talking_npc/talking_npc.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/tutorials/tutorial_world/README.md` & `evennia-4.1.1/evennia/contrib/tutorials/tutorial_world/README.md`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/tutorials/tutorial_world/build.ev` & `evennia-4.1.1/evennia/contrib/tutorials/tutorial_world/build.ev`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/tutorials/tutorial_world/intro_menu.py` & `evennia-4.1.1/evennia/contrib/tutorials/tutorial_world/intro_menu.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/tutorials/tutorial_world/mob.py` & `evennia-4.1.1/evennia/contrib/tutorials/tutorial_world/mob.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/tutorials/tutorial_world/objects.py` & `evennia-4.1.1/evennia/contrib/tutorials/tutorial_world/objects.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/tutorials/tutorial_world/rooms.py` & `evennia-4.1.1/evennia/contrib/tutorials/tutorial_world/rooms.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/tutorials/tutorial_world/tests.py` & `evennia-4.1.1/evennia/contrib/tutorials/tutorial_world/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/utils/auditing/README.md` & `evennia-4.1.1/evennia/contrib/utils/auditing/README.md`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/utils/auditing/outputs.py` & `evennia-4.1.1/evennia/contrib/utils/auditing/outputs.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/utils/auditing/server.py` & `evennia-4.1.1/evennia/contrib/utils/auditing/server.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/utils/auditing/tests.py` & `evennia-4.1.1/evennia/contrib/utils/auditing/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/utils/fieldfill/README.md` & `evennia-4.1.1/evennia/contrib/utils/fieldfill/README.md`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/utils/fieldfill/fieldfill.py` & `evennia-4.1.1/evennia/contrib/utils/fieldfill/fieldfill.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/utils/git_integration/README.md` & `evennia-4.1.1/evennia/contrib/utils/git_integration/README.md`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/utils/git_integration/git_integration.py` & `evennia-4.1.1/evennia/contrib/utils/git_integration/git_integration.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/utils/git_integration/tests.py` & `evennia-4.1.1/evennia/contrib/utils/git_integration/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/utils/name_generator/README.md` & `evennia-4.1.1/evennia/contrib/utils/name_generator/README.md`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/utils/name_generator/btn_givennames.txt` & `evennia-4.1.1/evennia/contrib/utils/name_generator/btn_givennames.txt`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/utils/name_generator/btn_surnames.txt` & `evennia-4.1.1/evennia/contrib/utils/name_generator/btn_surnames.txt`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/utils/name_generator/namegen.py` & `evennia-4.1.1/evennia/contrib/utils/name_generator/namegen.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/utils/name_generator/tests.py` & `evennia-4.1.1/evennia/contrib/utils/name_generator/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/utils/random_string_generator/README.md` & `evennia-4.1.1/evennia/contrib/utils/random_string_generator/README.md`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/utils/random_string_generator/random_string_generator.py` & `evennia-4.1.1/evennia/contrib/utils/random_string_generator/random_string_generator.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/utils/random_string_generator/tests.py` & `evennia-4.1.1/evennia/contrib/utils/random_string_generator/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/utils/tree_select/README.md` & `evennia-4.1.1/evennia/contrib/utils/tree_select/README.md`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/utils/tree_select/tests.py` & `evennia-4.1.1/evennia/contrib/utils/tree_select/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/contrib/utils/tree_select/tree_select.py` & `evennia-4.1.1/evennia/contrib/utils/tree_select/tree_select.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/game_template/README.md` & `evennia-4.1.1/evennia/game_template/README.md`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/game_template/commands/README.md` & `evennia-4.1.1/evennia/game_template/commands/README.md`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/game_template/commands/command.py` & `evennia-4.1.1/evennia/game_template/commands/command.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/game_template/commands/default_cmdsets.py` & `evennia-4.1.1/evennia/game_template/commands/default_cmdsets.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/game_template/gitignore` & `evennia-4.1.1/evennia/game_template/gitignore`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/game_template/server/README.md` & `evennia-4.1.1/evennia/game_template/server/README.md`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/game_template/server/conf/at_initial_setup.py` & `evennia-4.1.1/evennia/game_template/server/conf/at_initial_setup.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/game_template/server/conf/at_search.py` & `evennia-4.1.1/evennia/game_template/server/conf/at_search.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/game_template/server/conf/at_server_startstop.py` & `evennia-4.1.1/evennia/game_template/server/conf/at_server_startstop.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/game_template/server/conf/cmdparser.py` & `evennia-4.1.1/evennia/game_template/server/conf/cmdparser.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/game_template/server/conf/connection_screens.py` & `evennia-4.1.1/evennia/game_template/server/conf/connection_screens.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/game_template/server/conf/inlinefuncs.py` & `evennia-4.1.1/evennia/game_template/server/conf/inlinefuncs.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/game_template/server/conf/inputfuncs.py` & `evennia-4.1.1/evennia/game_template/server/conf/inputfuncs.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/game_template/server/conf/lockfuncs.py` & `evennia-4.1.1/evennia/game_template/server/conf/lockfuncs.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/game_template/server/conf/mssp.py` & `evennia-4.1.1/evennia/game_template/server/conf/mssp.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/game_template/server/conf/portal_services_plugins.py` & `evennia-4.1.1/evennia/game_template/server/conf/portal_services_plugins.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/game_template/server/conf/secret_settings.py` & `evennia-4.1.1/evennia/game_template/server/conf/secret_settings.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/game_template/server/conf/server_services_plugins.py` & `evennia-4.1.1/evennia/game_template/server/conf/server_services_plugins.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/game_template/server/conf/serversession.py` & `evennia-4.1.1/evennia/game_template/server/conf/serversession.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/game_template/server/conf/settings.py` & `evennia-4.1.1/evennia/game_template/server/conf/settings.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/game_template/server/conf/web_plugins.py` & `evennia-4.1.1/evennia/game_template/server/conf/web_plugins.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/game_template/server/logs/README.md` & `evennia-4.1.1/evennia/game_template/server/logs/README.md`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/game_template/typeclasses/README.md` & `evennia-4.1.1/evennia/game_template/typeclasses/README.md`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/game_template/typeclasses/accounts.py` & `evennia-4.1.1/evennia/game_template/typeclasses/accounts.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/game_template/typeclasses/channels.py` & `evennia-4.1.1/evennia/game_template/typeclasses/channels.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/game_template/typeclasses/characters.py` & `evennia-4.1.1/evennia/game_template/typeclasses/characters.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/game_template/typeclasses/exits.py` & `evennia-4.1.1/evennia/game_template/typeclasses/exits.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/game_template/typeclasses/objects.py` & `evennia-4.1.1/evennia/game_template/typeclasses/objects.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/game_template/typeclasses/rooms.py` & `evennia-4.1.1/evennia/game_template/typeclasses/rooms.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/game_template/typeclasses/scripts.py` & `evennia-4.1.1/evennia/game_template/typeclasses/scripts.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/game_template/web/README.md` & `evennia-4.1.1/evennia/game_template/web/README.md`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/game_template/web/admin/urls.py` & `evennia-4.1.1/evennia/game_template/web/admin/urls.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/game_template/web/static/README.md` & `evennia-4.1.1/evennia/game_template/web/static/README.md`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/game_template/web/templates/README.md` & `evennia-4.1.1/evennia/game_template/web/templates/README.md`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/game_template/web/urls.py` & `evennia-4.1.1/evennia/game_template/web/urls.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/game_template/web/webclient/README.md` & `evennia-4.1.1/evennia/game_template/web/webclient/README.md`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/game_template/web/webclient/urls.py` & `evennia-4.1.1/evennia/game_template/web/webclient/urls.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/game_template/web/website/README.md` & `evennia-4.1.1/evennia/game_template/web/website/README.md`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/game_template/world/batch_cmds.ev` & `evennia-4.1.1/evennia/game_template/world/batch_cmds.ev`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/game_template/world/help_entries.py` & `evennia-4.1.1/evennia/game_template/world/help_entries.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/game_template/world/prototypes.py` & `evennia-4.1.1/evennia/game_template/world/prototypes.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/help/filehelp.py` & `evennia-4.1.1/evennia/help/filehelp.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/help/manager.py` & `evennia-4.1.1/evennia/help/manager.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/help/migrations/0001_initial.py` & `evennia-4.1.1/evennia/help/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/help/migrations/0002_auto_20170606_1731.py` & `evennia-4.1.1/evennia/help/migrations/0002_auto_20170606_1731.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/help/migrations/0003_auto_20190128_1820.py` & `evennia-4.1.1/evennia/help/migrations/0003_auto_20190128_1820.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/help/migrations/0004_auto_20210520_2137.py` & `evennia-4.1.1/evennia/help/migrations/0004_auto_20210520_2137.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/help/migrations/0005_auto_20210530_1818.py` & `evennia-4.1.1/evennia/help/migrations/0005_auto_20210530_1818.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/help/models.py` & `evennia-4.1.1/evennia/help/models.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/help/tests.py` & `evennia-4.1.1/evennia/help/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/help/utils.py` & `evennia-4.1.1/evennia/help/utils.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/locale/README` & `evennia-4.1.1/evennia/locale/README`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/locale/de/LC_MESSAGES/django.mo` & `evennia-4.1.1/evennia/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/locale/de/LC_MESSAGES/django.po` & `evennia-4.1.1/evennia/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/locale/es/LC_MESSAGES/django.mo` & `evennia-4.1.1/evennia/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/locale/es/LC_MESSAGES/django.po` & `evennia-4.1.1/evennia/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/locale/fr/LC_MESSAGES/django.mo` & `evennia-4.1.1/evennia/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/locale/fr/LC_MESSAGES/django.po` & `evennia-4.1.1/evennia/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/locale/it/LC_MESSAGES/django.mo` & `evennia-4.1.1/evennia/locale/it/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/locale/it/LC_MESSAGES/django.po` & `evennia-4.1.1/evennia/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/locale/ko/LC_MESSAGES/django.mo` & `evennia-4.1.1/evennia/locale/ko/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/locale/ko/LC_MESSAGES/django.po` & `evennia-4.1.1/evennia/locale/ko/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/locale/la/LC_MESSAGES/django.mo` & `evennia-4.1.1/evennia/locale/la/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/locale/la/LC_MESSAGES/django.po` & `evennia-4.1.1/evennia/locale/la/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/locale/pl/LC_MESSAGES/django.mo` & `evennia-4.1.1/evennia/locale/pl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/locale/pl/LC_MESSAGES/django.po` & `evennia-4.1.1/evennia/locale/pl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/locale/pt/LC_MESSAGES/django.mo` & `evennia-4.1.1/evennia/locale/pt/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/locale/pt/LC_MESSAGES/django.po` & `evennia-4.1.1/evennia/locale/pt/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/locale/ru/LC_MESSAGES/django.mo` & `evennia-4.1.1/evennia/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/locale/ru/LC_MESSAGES/django.po` & `evennia-4.1.1/evennia/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/locale/sv/LC_MESSAGES/django.mo` & `evennia-4.1.1/evennia/locale/sv/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/locale/sv/LC_MESSAGES/django.po` & `evennia-4.1.1/evennia/locale/sv/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/locale/zh/LC_MESSAGES/django.mo` & `evennia-4.1.1/evennia/locale/zh/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/locale/zh/LC_MESSAGES/django.po` & `evennia-4.1.1/evennia/locale/zh/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/locks/lockfuncs.py` & `evennia-4.1.1/evennia/locks/lockfuncs.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/locks/lockhandler.py` & `evennia-4.1.1/evennia/locks/lockhandler.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/locks/tests.py` & `evennia-4.1.1/evennia/locks/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/objects/manager.py` & `evennia-4.1.1/evennia/objects/manager.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/objects/migrations/0001_initial.py` & `evennia-4.1.1/evennia/objects/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/objects/migrations/0002_auto_20140917_0756.py` & `evennia-4.1.1/evennia/objects/migrations/0002_auto_20140917_0756.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/objects/migrations/0003_defaultcharacter_defaultexit_defaultobject_defaultroom.py` & `evennia-4.1.1/evennia/objects/migrations/0003_defaultcharacter_defaultexit_defaultobject_defaultroom.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/objects/migrations/0004_auto_20150118_1622.py` & `evennia-4.1.1/evennia/objects/migrations/0004_auto_20150118_1622.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/objects/migrations/0006_auto_20170606_1731.py` & `evennia-4.1.1/evennia/objects/migrations/0006_auto_20170606_1731.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/objects/migrations/0007_objectdb_db_account.py` & `evennia-4.1.1/evennia/objects/migrations/0007_objectdb_db_account.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/objects/migrations/0008_auto_20170705_1736.py` & `evennia-4.1.1/evennia/objects/migrations/0008_auto_20170705_1736.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/objects/migrations/0009_remove_objectdb_db_player.py` & `evennia-4.1.1/evennia/objects/migrations/0009_remove_objectdb_db_player.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/objects/migrations/0010_auto_20190128_1820.py` & `evennia-4.1.1/evennia/objects/migrations/0010_auto_20190128_1820.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/objects/migrations/0011_auto_20191025_0831.py` & `evennia-4.1.1/evennia/objects/migrations/0011_auto_20191025_0831.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/objects/migrations/0012_convert_contrib_typeclass_paths.py` & `evennia-4.1.1/evennia/objects/migrations/0012_convert_contrib_typeclass_paths.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/objects/models.py` & `evennia-4.1.1/evennia/objects/models.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/objects/objects.py` & `evennia-4.1.1/evennia/objects/objects.py`

 * *Files 0% similar despite different names*

```diff
@@ -940,15 +940,15 @@
         is_outcmd = text and is_iter(text)
         inmessage = text[0] if is_outcmd else text
         outkwargs = text[1] if is_outcmd and len(text) > 1 else {}
         mapping = mapping or {}
         you = from_obj or self
 
         if "you" not in mapping:
-            mapping[you] = you
+            mapping["you"] = you
 
         contents = self.contents
         if exclude:
             exclude = make_iter(exclude)
             contents = [obj for obj in contents if obj not in exclude]
 
         for receiver in contents:
@@ -1430,15 +1430,16 @@
             Override this
             method to implement custom visibility mechanics.
 
         """
         return [
             obj
             for obj in obj_list
-            if (obj.access(looker, "view") and obj.access(looker, "search", default=True))
+            if obj != looker
+            and (obj.access(looker, "view") and obj.access(looker, "search", default=True))
         ]
 
     # name and return_appearance hooks
 
     def get_display_name(self, looker=None, **kwargs):
         """
         Displays the name of the object in a viewer-aware manner.
```

### Comparing `evennia-4.1.0/evennia/objects/tests.py` & `evennia-4.1.1/evennia/objects/tests.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,14 @@
 from unittest import skip
 
 from evennia import DefaultCharacter, DefaultExit, DefaultObject, DefaultRoom
 from evennia.objects.models import ObjectDB
 from evennia.typeclasses.attributes import AttributeProperty
-from evennia.typeclasses.tags import (
-    AliasProperty,
-    PermissionProperty,
-    TagCategoryProperty,
-    TagProperty,
-)
+from evennia.typeclasses.tags import (AliasProperty, PermissionProperty,
+                                      TagCategoryProperty, TagProperty)
 from evennia.utils import create, search
 from evennia.utils.test_resources import BaseEvenniaTest, EvenniaTestCase
 
 
 class DefaultObjectTest(BaseEvenniaTest):
     ip = "212.216.139.14"
 
@@ -352,14 +348,18 @@
 
 
 class TestObjectPropertiesClass(DefaultObject):
     attr1 = AttributeProperty(default="attr1")
     attr2 = AttributeProperty(default="attr2", category="attrcategory")
     attr3 = AttributeProperty(default="attr3", autocreate=False)
     attr4 = SubAttributeProperty(default="attr4")
+    attr5 = AttributeProperty(default=list, autocreate=False)
+    attr6 = AttributeProperty(default=[None], autocreate=False)
+    attr7 = AttributeProperty(default=list)
+    attr8 = AttributeProperty(default=[None])
     cusattr = CustomizedProperty(default=5)
     tag1 = TagProperty()
     tag2 = TagProperty(category="tagcategory")
     tag3 = SubTagProperty()
     testalias = AliasProperty()
     testperm = PermissionProperty()
     awaretest = 5
@@ -537,7 +537,103 @@
             db_attributes__db_key="attr1", db_attributes__db_value=obj2
         )
 
         self.assertEqual(list(query), [obj1])
 
         obj1.delete()
         obj2.delete()
+
+    def test_not_create_attribute_with_autocreate_false(self):
+        """
+        Test that AttributeProperty with autocreate=False does not create an attribute in the database.
+
+        """
+        obj = create.create_object(TestObjectPropertiesClass, key="obj1")
+
+        self.assertEqual(obj.attr3, "attr3")
+        self.assertEqual(obj.attributes.get("attr3"), None)
+
+        self.assertEqual(obj.attr5, [])
+        self.assertEqual(obj.attributes.get("attr5"), None)
+
+        obj.delete()
+
+    def test_callable_defaults__autocreate_false(self):
+        """
+        Test https://github.com/evennia/evennia/issues/3488, where a callable default value like `list`
+        would produce an infinitely empty result even when appended to.
+
+        """
+        obj1 = create.create_object(TestObjectPropertiesClass, key="obj1")
+        obj2 = create.create_object(TestObjectPropertiesClass, key="obj2")
+
+        self.assertEqual(obj1.attr5, [])
+        obj1.attr5.append(1)
+        self.assertEqual(obj1.attr5, [1])
+
+        # check cross-instance sharing
+        self.assertEqual(obj2.attr5, [], "cross-instance sharing detected")
+
+
+    def test_mutable_defaults__autocreate_false(self):
+        """
+        Test https://github.com/evennia/evennia/issues/3488, where a mutable default value (like a
+        list `[]` or `[None]`) would not be updated in the database when appended to.
+
+        Note that using a mutable default value is not recommended, as the mutable will share the
+        same memory space across all instances of the class. This means that if one instance modifiesA
+        the mutable, all instances will be affected.
+
+        """
+        obj1 = create.create_object(TestObjectPropertiesClass, key="obj1")
+        obj2 = create.create_object(TestObjectPropertiesClass, key="obj2")
+
+        self.assertEqual(obj1.attr6, [None])
+        obj1.attr6.append(1)
+        self.assertEqual(obj1.attr6, [None, 1])
+
+        obj1.attr6[1] = 2
+        self.assertEqual(obj1.attr6, [None, 2])
+
+        # check cross-instance sharing
+        self.assertEqual(obj2.attr6, [None], "cross-instance sharing detected")
+
+        obj1.delete()
+        obj2.delete()
+
+    def test_callable_defaults__autocreate_true(self):
+        """
+        Test callables with autocreate=True.
+
+        """
+        obj1 = create.create_object(TestObjectPropertiesClass, key="obj1")
+        obj2 = create.create_object(TestObjectPropertiesClass, key="obj1")
+
+        self.assertEqual(obj1.attr7, [])
+        obj1.attr7.append(1)
+        self.assertEqual(obj1.attr7, [1])
+
+        # check cross-instance sharing
+        self.assertEqual(obj2.attr7, [])
+
+
+    def test_mutable_defaults__autocreate_true(self):
+        """
+        Test mutable defaults with autocreate=True.
+
+        """
+        obj1 = create.create_object(TestObjectPropertiesClass, key="obj1")
+        obj2 = create.create_object(TestObjectPropertiesClass, key="obj2")
+
+        self.assertEqual(obj1.attr8, [None])
+        obj1.attr8.append(1)
+        self.assertEqual(obj1.attr8, [None, 1])
+
+        obj1.attr8[1] = 2
+        self.assertEqual(obj1.attr8, [None, 2])
+
+        # check cross-instance sharing
+        self.assertEqual(obj2.attr8, [None])
+
+        obj1.delete()
+        obj2.delete()
+
```

### Comparing `evennia-4.1.0/evennia/prototypes/README.md` & `evennia-4.1.1/evennia/prototypes/README.md`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/prototypes/menus.py` & `evennia-4.1.1/evennia/prototypes/menus.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/prototypes/protfuncs.py` & `evennia-4.1.1/evennia/prototypes/protfuncs.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/prototypes/prototypes.py` & `evennia-4.1.1/evennia/prototypes/prototypes.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/prototypes/spawner.py` & `evennia-4.1.1/evennia/prototypes/spawner.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/prototypes/tests.py` & `evennia-4.1.1/evennia/prototypes/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/scripts/manager.py` & `evennia-4.1.1/evennia/scripts/manager.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/scripts/migrations/0001_initial.py` & `evennia-4.1.1/evennia/scripts/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/scripts/migrations/0002_auto_20150118_1625.py` & `evennia-4.1.1/evennia/scripts/migrations/0002_auto_20150118_1625.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/scripts/migrations/0003_checksessions_defaultscript_donothing_scriptbase_store_validatechannelhandler_validateidmappercache_.py` & `evennia-4.1.1/evennia/scripts/migrations/0003_checksessions_defaultscript_donothing_scriptbase_store_validatechannelhandler_validateidmappercache_.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/scripts/migrations/0004_auto_20150306_1354.py` & `evennia-4.1.1/evennia/scripts/migrations/0004_auto_20150306_1354.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/scripts/migrations/0006_auto_20150310_2249.py` & `evennia-4.1.1/evennia/scripts/migrations/0006_auto_20150310_2249.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/scripts/migrations/0008_auto_20170606_1731.py` & `evennia-4.1.1/evennia/scripts/migrations/0008_auto_20170606_1731.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/scripts/migrations/0009_scriptdb_db_account.py` & `evennia-4.1.1/evennia/scripts/migrations/0009_scriptdb_db_account.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/scripts/migrations/0010_auto_20170705_1736.py` & `evennia-4.1.1/evennia/scripts/migrations/0010_auto_20170705_1736.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/scripts/migrations/0011_remove_scriptdb_db_player.py` & `evennia-4.1.1/evennia/scripts/migrations/0011_remove_scriptdb_db_player.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/scripts/migrations/0012_auto_20190128_1820.py` & `evennia-4.1.1/evennia/scripts/migrations/0012_auto_20190128_1820.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/scripts/migrations/0013_auto_20191025_0831.py` & `evennia-4.1.1/evennia/scripts/migrations/0013_auto_20191025_0831.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/scripts/migrations/0014_auto_20210520_2137.py` & `evennia-4.1.1/evennia/scripts/migrations/0014_auto_20210520_2137.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/scripts/migrations/0015_convert_contrib_paths.py` & `evennia-4.1.1/evennia/scripts/migrations/0015_convert_contrib_paths.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/scripts/models.py` & `evennia-4.1.1/evennia/scripts/models.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/scripts/monitorhandler.py` & `evennia-4.1.1/evennia/scripts/monitorhandler.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/scripts/ondemandhandler.py` & `evennia-4.1.1/evennia/scripts/ondemandhandler.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/scripts/scripthandler.py` & `evennia-4.1.1/evennia/scripts/scripthandler.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/scripts/scripts.py` & `evennia-4.1.1/evennia/scripts/scripts.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/scripts/taskhandler.py` & `evennia-4.1.1/evennia/scripts/taskhandler.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/scripts/tests.py` & `evennia-4.1.1/evennia/scripts/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/scripts/tickerhandler.py` & `evennia-4.1.1/evennia/scripts/tickerhandler.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/server/amp_client.py` & `evennia-4.1.1/evennia/server/amp_client.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/server/connection_wizard.py` & `evennia-4.1.1/evennia/server/connection_wizard.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/server/deprecations.py` & `evennia-4.1.1/evennia/server/deprecations.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/server/evennia_launcher.py` & `evennia-4.1.1/evennia/server/evennia_launcher.py`

 * *Files 0% similar despite different names*

```diff
@@ -638,14 +638,16 @@
 def send_instruction(operation, arguments, callback=None, errback=None):
     """
     Send instruction and handle the response.
 
     """
     global AMP_CONNECTION, REACTOR_RUN
 
+    # print("launcher: Sending to portal: {} + {}".format(ord(operation), arguments))
+
     if None in (AMP_HOST, AMP_PORT, AMP_INTERFACE):
         print(ERROR_AMP_UNCONFIGURED)
         sys.exit()
 
     def _callback(result):
         if callback:
             callback(result)
```

### Comparing `evennia-4.1.0/evennia/server/game_index_client/README.md` & `evennia-4.1.1/evennia/server/game_index_client/README.md`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/server/game_index_client/client.py` & `evennia-4.1.1/evennia/server/game_index_client/client.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/server/game_index_client/service.py` & `evennia-4.1.1/evennia/server/game_index_client/service.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/server/initial_setup.py` & `evennia-4.1.1/evennia/server/initial_setup.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/server/inputfuncs.py` & `evennia-4.1.1/evennia/server/inputfuncs.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/server/manager.py` & `evennia-4.1.1/evennia/server/manager.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/server/migrations/0001_initial.py` & `evennia-4.1.1/evennia/server/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/server/migrations/0002_auto_20190128_2311.py` & `evennia-4.1.1/evennia/server/migrations/0002_auto_20190128_2311.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/server/models.py` & `evennia-4.1.1/evennia/server/models.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/server/portal/amp.py` & `evennia-4.1.1/evennia/server/portal/amp.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/server/portal/amp_server.py` & `evennia-4.1.1/evennia/server/portal/amp_server.py`

 * *Files 2% similar despite different names*

```diff
@@ -193,16 +193,14 @@
                 logger.log_trace()
 
             self.factory.portal.server_twistd_cmd = server_twistd_cmd
             logfile.flush()
         if process and not _is_windows():
             # avoid zombie-process on Unix/BSD
             process.wait()
-        # unset the reset-mode flag on the portal
-        self.factory.portal.server_restart_mode = None
         return
 
     def wait_for_disconnect(self, callback, *args, **kwargs):
         """
         Add a callback for when this connection is lost.
 
         Args:
@@ -228,19 +226,26 @@
         Shut down server in one or more modes.
 
         Args:
             mode (str): One of 'shutdown', 'reload' or 'reset'.
 
         """
         if mode == "reload":
-            self.send_AdminPortal2Server(amp.DUMMYSESSION, operation=amp.SRELOAD)
+            self.send_AdminPortal2Server(
+                amp.DUMMYSESSION, operation=amp.SRELOAD, server_restart_mode=mode
+            )
         elif mode == "reset":
-            self.send_AdminPortal2Server(amp.DUMMYSESSION, operation=amp.SRESET)
+            self.send_AdminPortal2Server(
+                amp.DUMMYSESSION, operation=amp.SRESET, server_restart_mode=mode
+            )
         elif mode == "shutdown":
-            self.send_AdminPortal2Server(amp.DUMMYSESSION, operation=amp.SSHUTD)
+            self.send_AdminPortal2Server(
+                amp.DUMMYSESSION, operation=amp.SSHUTD, server_restart_mode=mode
+            )
+        # store the mode for use once server comes back up again
         self.factory.portal.server_restart_mode = mode
 
     # sending amp data
 
     def send_Status2Launcher(self):
         """
         Send a status stanza to the launcher.
@@ -322,15 +327,14 @@
         """
         # Since the launcher command uses amp.String() we need to convert from byte here.
         operation = str(operation, "utf-8")
         self.factory.launcher_connection = self
         _, server_connected, _, _, _, _ = self.get_status()
 
         # logger.log_msg("Evennia Launcher->Portal operation %s:%s received" % (ord(operation), arguments))
-
         # logger.log_msg("operation == amp.SSTART: {}: {}".format(operation == amp.SSTART, amp.loads(arguments)))
 
         if operation == amp.SSTART:  # portal start  #15
             # first, check if server is already running
             if not server_connected:
                 self.wait_for_server_connect(self.send_Status2Launcher)
                 self.start_server(amp.loads(arguments))
@@ -401,19 +405,19 @@
             packed_data (str): Data received, a pickled tuple (sessid, kwargs).
 
         """
         self.factory.server_connection = self
 
         sessid, kwargs = self.data_in(packed_data)
 
-        # logger.log_msg("Evennia Server->Portal admin data %s:%s received" % (sessid, kwargs))
-
         operation = kwargs.pop("operation")
         portal_sessionhandler = evennia.PORTAL_SESSION_HANDLER
 
+        # logger.log_msg(f"Evennia Server->Portal admin data operation {ord(operation)}")
+
         if operation == amp.SLOGIN:  # server_session_login
             # a session has authenticated; sync it.
             session = portal_sessionhandler.get(sessid)
             if session:
                 portal_sessionhandler.server_logged_in(session, kwargs.get("sessiondata"))
 
         elif operation == amp.SDISCONN:  # server_session_disconnect
@@ -423,48 +427,56 @@
                 portal_sessionhandler.server_disconnect(session, reason=kwargs.get("reason"))
 
         elif operation == amp.SDISCONNALL:  # server_session_disconnect_all
             # server orders all sessions to disconnect
             portal_sessionhandler.server_disconnect_all(reason=kwargs.get("reason"))
 
         elif operation == amp.SRELOAD:  # server reload
+            # set up callback to restart server once it has disconnected
             self.factory.server_connection.wait_for_disconnect(
                 self.start_server, self.factory.portal.server_twistd_cmd
             )
+            # tell server to reload
             self.stop_server(mode="reload")
 
         elif operation == amp.SRESET:  # server reset
+            # set up callback to restart server once it has disconnected
             self.factory.server_connection.wait_for_disconnect(
                 self.start_server, self.factory.portal.server_twistd_cmd
             )
+            # tell server to reset
             self.stop_server(mode="reset")
 
         elif operation == amp.SSHUTD:  # server-only shutdown
             self.stop_server(mode="shutdown")
 
         elif operation == amp.PSHUTD:  # full server+server shutdown
+            # set up callback to shut down portal once server has disconnected
             self.factory.server_connection.wait_for_disconnect(self.factory.portal.shutdown)
+            # tell server to shut down
             self.stop_server(mode="shutdown")
 
         elif operation == amp.PSYNC:  # portal sync
             # Server has (re-)connected and wants the session data from portal
             self.factory.portal.server_info_dict = kwargs.get("info_dict", {})
             self.factory.portal.server_process_id = kwargs.get("spid", None)
             # this defaults to 'shutdown' or whatever value set in server_stop
             server_restart_mode = self.factory.portal.server_restart_mode
+            # print("Server has connected. Sending session data to Server ... mode: {}".format(server_restart_mode))
 
             sessdata = evennia.PORTAL_SESSION_HANDLER.get_all_sync_data()
             self.send_AdminPortal2Server(
                 amp.DUMMYSESSION,
                 amp.PSYNC,
                 server_restart_mode=server_restart_mode,
                 sessiondata=sessdata,
                 portal_start_time=self.factory.portal.start_time,
             )
             evennia.PORTAL_SESSION_HANDLER.at_server_connection()
+            self.factory.portal.server_restart_mode = None
 
             if self.factory.server_connection:
                 # this is an indication the server has successfully connected, so
                 # we trigger any callbacks (usually to tell the launcher server is up)
                 for callback, args, kwargs in self.factory.server_connect_callbacks:
                     try:
                         callback(*args, **kwargs)
@@ -476,15 +488,15 @@
             # server wants to save session data to the portal,
             # maybe because it's about to shut down.
             portal_sessionhandler.server_session_sync(
                 kwargs.get("sessiondata"), kwargs.get("clean", True)
             )
 
             # set a flag in case we are about to shut down soon
-            self.factory.server_restart_mode = True
+            self.factory.server_restart_mode = "shutdown"
 
         elif operation == amp.SCONN:  # server_force_connection (for irc/etc)
             portal_sessionhandler.server_connect(**kwargs)
 
         else:
             raise Exception("operation %(op)s not recognized." % {"op": operation})
         return {}
```

### Comparing `evennia-4.1.0/evennia/server/portal/discord.py` & `evennia-4.1.1/evennia/server/portal/discord.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/server/portal/grapevine.py` & `evennia-4.1.1/evennia/server/portal/grapevine.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/server/portal/irc.py` & `evennia-4.1.1/evennia/server/portal/irc.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/server/portal/mccp.py` & `evennia-4.1.1/evennia/server/portal/mccp.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/server/portal/mssp.py` & `evennia-4.1.1/evennia/server/portal/mssp.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/server/portal/mxp.py` & `evennia-4.1.1/evennia/server/portal/mxp.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/server/portal/naws.py` & `evennia-4.1.1/evennia/server/portal/naws.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/server/portal/portal.py` & `evennia-4.1.1/evennia/server/portal/portal.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/server/portal/portalsessionhandler.py` & `evennia-4.1.1/evennia/server/portal/portalsessionhandler.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/server/portal/rss.py` & `evennia-4.1.1/evennia/server/portal/rss.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/server/portal/service.py` & `evennia-4.1.1/evennia/server/portal/service.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/server/portal/ssh.py` & `evennia-4.1.1/evennia/server/portal/ssh.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/server/portal/ssl.py` & `evennia-4.1.1/evennia/server/portal/ssl.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/server/portal/suppress_ga.py` & `evennia-4.1.1/evennia/server/portal/suppress_ga.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/server/portal/telnet.py` & `evennia-4.1.1/evennia/server/portal/telnet.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/server/portal/telnet_oob.py` & `evennia-4.1.1/evennia/server/portal/telnet_oob.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/server/portal/telnet_ssl.py` & `evennia-4.1.1/evennia/server/portal/telnet_ssl.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/server/portal/tests.py` & `evennia-4.1.1/evennia/server/portal/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/server/portal/ttype.py` & `evennia-4.1.1/evennia/server/portal/ttype.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/server/portal/webclient.py` & `evennia-4.1.1/evennia/server/portal/webclient.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/server/portal/webclient_ajax.py` & `evennia-4.1.1/evennia/server/portal/webclient_ajax.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/server/profiling/dummyrunner.py` & `evennia-4.1.1/evennia/server/profiling/dummyrunner.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/server/profiling/dummyrunner_settings.py` & `evennia-4.1.1/evennia/server/profiling/dummyrunner_settings.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/server/profiling/memplot.py` & `evennia-4.1.1/evennia/server/profiling/memplot.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/server/profiling/settings_mixin.py` & `evennia-4.1.1/evennia/server/profiling/settings_mixin.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/server/profiling/test_queries.py` & `evennia-4.1.1/evennia/server/profiling/test_queries.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/server/profiling/tests.py` & `evennia-4.1.1/evennia/server/profiling/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/server/profiling/timetrace.py` & `evennia-4.1.1/evennia/server/profiling/timetrace.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/server/server.py` & `evennia-4.1.1/evennia/server/server.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/server/serversession.py` & `evennia-4.1.1/evennia/server/serversession.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/server/service.py` & `evennia-4.1.1/evennia/server/service.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/server/session.py` & `evennia-4.1.1/evennia/server/session.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/server/sessionhandler.py` & `evennia-4.1.1/evennia/server/sessionhandler.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/server/signals.py` & `evennia-4.1.1/evennia/server/signals.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/server/tests/test_amp_connection.py` & `evennia-4.1.1/evennia/server/tests/test_amp_connection.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/server/tests/test_initial_setup.py` & `evennia-4.1.1/evennia/server/tests/test_initial_setup.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/server/tests/test_launcher.py` & `evennia-4.1.1/evennia/server/tests/test_launcher.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/server/tests/test_misc.py` & `evennia-4.1.1/evennia/server/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/server/tests/test_server.py` & `evennia-4.1.1/evennia/server/tests/test_server.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/server/tests/testrunner.py` & `evennia-4.1.1/evennia/server/tests/testrunner.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/server/throttle.py` & `evennia-4.1.1/evennia/server/throttle.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/server/validators.py` & `evennia-4.1.1/evennia/server/validators.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/server/webserver.py` & `evennia-4.1.1/evennia/server/webserver.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/settings_default.py` & `evennia-4.1.1/evennia/settings_default.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/typeclasses/attributes.py` & `evennia-4.1.1/evennia/typeclasses/attributes.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,19 +8,19 @@
 
 
 """
 
 import fnmatch
 import re
 from collections import defaultdict
+from copy import copy
 
 from django.conf import settings
 from django.db import models
 from django.utils.encoding import smart_str
-
 from evennia.locks.lockhandler import LockHandler
 from evennia.utils.dbserialize import from_pickle, to_pickle
 from evennia.utils.idmapper.models import SharedMemoryModel
 from evennia.utils.picklefield import PickledObjectField
 from evennia.utils.utils import is_iter, lazy_property, make_iter, to_str
 
 _TYPECLASS_AGGRESSIVE_CACHE = settings.TYPECLASS_AGGRESSIVE_CACHE
@@ -162,14 +162,15 @@
 class AttributeProperty:
     """
     AttributeProperty.
 
     """
 
     attrhandler_name = "attributes"
+    cached_default_name_template = "_property_attribute_default_{key}"
 
     def __init__(self, default=None, category=None, strattr=False, lockstring="", autocreate=True):
         """
         Allows for specifying Attributes as Django-like 'fields' on the class level. Note that while
         one can set a lock on the Attribute, there is no way to *check* said lock when accessing via
         the property - use the full `AttributeHandler` if you need to do access checks. Note however
         that if you use the full `AttributeHandler` to access this Attribute, the `at_get/at_set`
@@ -203,58 +204,61 @@
         self._default = default
         self._category = category
         self._strattr = strattr
         self._lockstring = lockstring
         self._autocreate = autocreate
         self._key = ""
 
-    @property
-    def _default(self):
-        """
-        Tries returning a new instance of default if callable.
-
-        """
-        if callable(self.__default):
-            return self.__default()
-
-        return self.__default
-
-    @_default.setter
-    def _default(self, value):
-        self.__default = value
-
     def __set_name__(self, cls, name):
         """
         Called when descriptor is first assigned to the class. It is called with
         the name of the field.
 
         """
         self._key = name
 
+    def _get_and_cache_default(self, instance):
+        """
+        Get and cache the default value for this attribute. We make sure to convert any mutables
+        into _Saver* equivalent classes here and cache the result on the instance's AttributeHandler.
+
+        """
+        attrhandler = getattr(instance, self.attrhandler_name)
+        value = getattr(attrhandler, self.cached_default_name_template.format(key=self._key), None)
+        if not value:
+            if callable(self._default):
+                value = self._default()
+            else:
+                value = copy(self._default)
+            value = from_pickle(value, db_obj=instance)
+            setattr(attrhandler, self.cached_default_name_template.format(key=self._key), value)
+        return value
+
     def __get__(self, instance, owner):
         """
         Called when the attrkey is retrieved from the instance.
 
         """
-        value = self._default
+        value = self._get_and_cache_default(instance)
+
         try:
             value = self.at_get(
                 getattr(instance, self.attrhandler_name).get(
                     key=self._key,
-                    default=self._default,
+                    default=value,
                     category=self._category,
                     strattr=self._strattr,
                     raise_exception=self._autocreate,
                 ),
                 instance,
             )
         except AttributeError:
             if self._autocreate:
                 # attribute didn't exist and autocreate is set
-                self.__set__(instance, self._default)
+                self.__set__(instance, value)
             else:
                 raise
         return value
 
     def __set__(self, instance, value):
         """
         Called when assigning to the property (and when auto-creating an Attribute).
```

### Comparing `evennia-4.1.0/evennia/typeclasses/managers.py` & `evennia-4.1.1/evennia/typeclasses/managers.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/typeclasses/migrations/0001_initial.py` & `evennia-4.1.1/evennia/typeclasses/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/typeclasses/migrations/0002_auto_20150109_0913.py` & `evennia-4.1.1/evennia/typeclasses/migrations/0002_auto_20150109_0913.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/typeclasses/migrations/0003_defaultcharacter_defaultexit_defaultguest_defaultobject_defaultplayer_defaultroom_defaultscript_dono.py` & `evennia-4.1.1/evennia/typeclasses/migrations/0003_defaultcharacter_defaultexit_defaultguest_defaultobject_defaultplayer_defaultroom_defaultscript_dono.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/typeclasses/migrations/0004_auto_20151101_1759.py` & `evennia-4.1.1/evennia/typeclasses/migrations/0004_auto_20151101_1759.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/typeclasses/migrations/0005_auto_20160625_1812.py` & `evennia-4.1.1/evennia/typeclasses/migrations/0005_auto_20160625_1812.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/typeclasses/migrations/0006_auto_add_dbmodel_value_for_tags_attributes.py` & `evennia-4.1.1/evennia/typeclasses/migrations/0006_auto_add_dbmodel_value_for_tags_attributes.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/typeclasses/migrations/0007_tag_migrations_may_be_slow.py` & `evennia-4.1.1/evennia/typeclasses/migrations/0007_tag_migrations_may_be_slow.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/typeclasses/migrations/0008_lock_and_perm_rename.py` & `evennia-4.1.1/evennia/typeclasses/migrations/0008_lock_and_perm_rename.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/typeclasses/migrations/0009_rename_player_cmdsets_typeclasses.py` & `evennia-4.1.1/evennia/typeclasses/migrations/0009_rename_player_cmdsets_typeclasses.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/typeclasses/migrations/0010_delete_old_player_tables.py` & `evennia-4.1.1/evennia/typeclasses/migrations/0010_delete_old_player_tables.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/typeclasses/migrations/0011_auto_20190128_1820.py` & `evennia-4.1.1/evennia/typeclasses/migrations/0011_auto_20190128_1820.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/typeclasses/migrations/0012_attrs_to_picklev4_may_be_slow.py` & `evennia-4.1.1/evennia/typeclasses/migrations/0012_attrs_to_picklev4_may_be_slow.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/typeclasses/migrations/0013_auto_20191015_1922.py` & `evennia-4.1.1/evennia/typeclasses/migrations/0013_auto_20191015_1922.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/typeclasses/migrations/0014_alter_tag_db_category.py` & `evennia-4.1.1/evennia/typeclasses/migrations/0014_alter_tag_db_category.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/typeclasses/migrations/0016_alter_attribute_id_alter_tag_id.py` & `evennia-4.1.1/evennia/typeclasses/migrations/0016_alter_attribute_id_alter_tag_id.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/typeclasses/models.py` & `evennia-4.1.1/evennia/typeclasses/models.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/typeclasses/tags.py` & `evennia-4.1.1/evennia/typeclasses/tags.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/typeclasses/tests.py` & `evennia-4.1.1/evennia/typeclasses/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/utils/ansi.py` & `evennia-4.1.1/evennia/utils/ansi.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/utils/batchprocessors.py` & `evennia-4.1.1/evennia/utils/batchprocessors.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/utils/containers.py` & `evennia-4.1.1/evennia/utils/containers.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/utils/create.py` & `evennia-4.1.1/evennia/utils/create.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/utils/dbserialize.py` & `evennia-4.1.1/evennia/utils/dbserialize.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/utils/eveditor.py` & `evennia-4.1.1/evennia/utils/eveditor.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,15 +94,15 @@
  :r  <l> <txt>  - replace line <l> with text <txt>
  :I  <l> <txt>  - insert text at the beginning of line <l>
  :A  <l> <txt>  - append text after the end of line <l>
 
  :s <l> <w> <txt> - search/replace word or regex <w> in buffer or on line <l>
 
  :j <l> <w> - justify buffer or line <l>. <w> is f, c, l or r. Default f (full)
- :f <l>     - flood-fill entire buffer or line <l>: Equivalent to :j left
+ :f <l>     - flood-fill entire buffer or line <l>. Equivalent to :j <l> l
  :fi <l>    - indent entire buffer or line <l>
  :fd <l>    - de-indent entire buffer or line <l>
 
  :echo - turn echoing of the input on/off (helpful for some clients)
 """
 )
 
@@ -347,14 +347,43 @@
         self.linerange = linerange
         self.lstr = lstr
         self.words = words
         self.args = args
         self.arg1 = arg1
         self.arg2 = arg2
 
+    def insert_raw_string_into_buffer(self):
+        """
+        Insert a line into the buffer. Used by both CmdLineInput and CmdEditorGroup.
+
+        """
+        caller = self.caller
+        editor = caller.ndb._eveditor
+        buf = editor.get_buffer()
+
+        # add a line of text to buffer
+        line = self.raw_string.strip("\r\n")
+        if editor._codefunc and editor._indent >= 0:
+            # if automatic indentation is active, add spaces
+            line = editor.deduce_indent(line, buf)
+        buf = line if not buf else buf + "\n%s" % line
+        self.editor.update_buffer(buf)
+        if self.editor._echo_mode:
+            # need to do it here or we will be off one line
+            cline = len(self.editor.get_buffer().split("\n"))
+            if editor._codefunc:
+                # display the current level of identation
+                indent = editor._indent
+                if indent < 0:
+                    indent = "off"
+
+                self.caller.msg("|b%02i|||n (|g%s|n) %s" % (cline, indent, raw(line)))
+            else:
+                self.caller.msg("|b%02i|||n %s" % (cline, raw(line)))
+
 
 def _load_editor(caller):
     """
     Load persistent editor from storage.
 
     """
     saved_options = caller.attributes.get("_eveditor_saved")
@@ -390,37 +419,15 @@
     def func(self):
         """
         Adds the line without any formatting changes.
 
         If the editor handles code, it might add automatic
         indentation.
         """
-        caller = self.caller
-        editor = caller.ndb._eveditor
-        buf = editor.get_buffer()
-
-        # add a line of text to buffer
-        line = self.raw_string.strip("\r\n")
-        if editor._codefunc and editor._indent >= 0:
-            # if automatic indentation is active, add spaces
-            line = editor.deduce_indent(line, buf)
-        buf = line if not buf else buf + "\n%s" % line
-        self.editor.update_buffer(buf)
-        if self.editor._echo_mode:
-            # need to do it here or we will be off one line
-            cline = len(self.editor.get_buffer().split("\n"))
-            if editor._codefunc:
-                # display the current level of identation
-                indent = editor._indent
-                if indent < 0:
-                    indent = "off"
-
-                self.caller.msg("|b%02i|||n (|g%s|n) %s" % (cline, indent, raw(line)))
-            else:
-                self.caller.msg("|b%02i|||n %s" % (cline, raw(line)))
+        self.insert_raw_string_into_buffer()
 
 
 class CmdEditorGroup(CmdEditorBase):
     """
     Commands for the editor
     """
 
@@ -797,14 +804,17 @@
                 indent = editor._indent
                 if indent >= 0:
                     caller.msg(_("Auto-indentation turned on."))
                 else:
                     caller.msg(_("Auto-indentation turned off."))
             else:
                 caller.msg(_("This command is only available in code editor mode."))
+        else:
+            # no match - insert as line in buffer
+            self.insert_raw_string_into_buffer()
 
 
 class EvEditorCmdSet(CmdSet):
     """CmdSet for the editor commands"""
 
     key = "editorcmdset"
     mergetype = "Replace"
```

### Comparing `evennia-4.1.0/evennia/utils/evennia-mode.el` & `evennia-4.1.1/evennia/utils/evennia-mode.el`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/utils/evform.py` & `evennia-4.1.1/evennia/utils/evform.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/utils/evmenu.py` & `evennia-4.1.1/evennia/utils/evmenu.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/utils/evmore.py` & `evennia-4.1.1/evennia/utils/evmore.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/utils/evtable.py` & `evennia-4.1.1/evennia/utils/evtable.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/utils/funcparser.py` & `evennia-4.1.1/evennia/utils/funcparser.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/utils/gametime.py` & `evennia-4.1.1/evennia/utils/gametime.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/utils/idmapper/LICENSE.md` & `evennia-4.1.1/evennia/utils/idmapper/LICENSE.md`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/utils/idmapper/README_evennia.md` & `evennia-4.1.1/evennia/utils/idmapper/README_evennia.md`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/utils/idmapper/README_orig.rst` & `evennia-4.1.1/evennia/utils/idmapper/README_orig.rst`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/utils/idmapper/manager.py` & `evennia-4.1.1/evennia/utils/idmapper/manager.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/utils/idmapper/models.py` & `evennia-4.1.1/evennia/utils/idmapper/models.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/utils/idmapper/tests.py` & `evennia-4.1.1/evennia/utils/idmapper/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/utils/logger.py` & `evennia-4.1.1/evennia/utils/logger.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/utils/optionclasses.py` & `evennia-4.1.1/evennia/utils/optionclasses.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/utils/optionhandler.py` & `evennia-4.1.1/evennia/utils/optionhandler.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/utils/picklefield.py` & `evennia-4.1.1/evennia/utils/picklefield.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/utils/search.py` & `evennia-4.1.1/evennia/utils/search.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/utils/test_resources.py` & `evennia-4.1.1/evennia/utils/test_resources.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/utils/tests/data/evform_example.py` & `evennia-4.1.1/evennia/utils/tests/data/evform_example.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/utils/tests/data/evmenu_example.py` & `evennia-4.1.1/evennia/utils/tests/data/evmenu_example.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/utils/tests/test_ansi.py` & `evennia-4.1.1/evennia/utils/tests/test_ansi.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/utils/tests/test_batchprocessors.py` & `evennia-4.1.1/evennia/utils/tests/test_batchprocessors.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/utils/tests/test_containers.py` & `evennia-4.1.1/evennia/utils/tests/test_containers.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/utils/tests/test_create_functions.py` & `evennia-4.1.1/evennia/utils/tests/test_create_functions.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/utils/tests/test_dbserialize.py` & `evennia-4.1.1/evennia/utils/tests/test_dbserialize.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/utils/tests/test_eveditor.py` & `evennia-4.1.1/evennia/utils/tests/test_eveditor.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/utils/tests/test_evform.py` & `evennia-4.1.1/evennia/utils/tests/test_evform.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/utils/tests/test_evmenu.py` & `evennia-4.1.1/evennia/utils/tests/test_evmenu.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/utils/tests/test_evtable.py` & `evennia-4.1.1/evennia/utils/tests/test_evtable.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/utils/tests/test_funcparser.py` & `evennia-4.1.1/evennia/utils/tests/test_funcparser.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/utils/tests/test_gametime.py` & `evennia-4.1.1/evennia/utils/tests/test_gametime.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/utils/tests/test_search.py` & `evennia-4.1.1/evennia/utils/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/utils/tests/test_tagparsing.py` & `evennia-4.1.1/evennia/utils/tests/test_tagparsing.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/utils/tests/test_text2html.py` & `evennia-4.1.1/evennia/utils/tests/test_text2html.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/utils/tests/test_utils.py` & `evennia-4.1.1/evennia/utils/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/utils/tests/test_validatorfuncs.py` & `evennia-4.1.1/evennia/utils/tests/test_validatorfuncs.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/utils/text2html.py` & `evennia-4.1.1/evennia/utils/text2html.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/utils/utils.py` & `evennia-4.1.1/evennia/utils/utils.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/utils/validatorfuncs.py` & `evennia-4.1.1/evennia/utils/validatorfuncs.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/utils/verb_conjugation/LICENSE.txt` & `evennia-4.1.1/evennia/utils/verb_conjugation/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/utils/verb_conjugation/conjugate.py` & `evennia-4.1.1/evennia/utils/verb_conjugation/conjugate.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/utils/verb_conjugation/pronouns.py` & `evennia-4.1.1/evennia/utils/verb_conjugation/pronouns.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/utils/verb_conjugation/tests.py` & `evennia-4.1.1/evennia/utils/verb_conjugation/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/utils/verb_conjugation/verbs.txt` & `evennia-4.1.1/evennia/utils/verb_conjugation/verbs.txt`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/web/README.md` & `evennia-4.1.1/evennia/web/README.md`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/web/admin/accounts.py` & `evennia-4.1.1/evennia/web/admin/accounts.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/web/admin/attributes.py` & `evennia-4.1.1/evennia/web/admin/attributes.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/web/admin/comms.py` & `evennia-4.1.1/evennia/web/admin/comms.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/web/admin/frontpage.py` & `evennia-4.1.1/evennia/web/admin/frontpage.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/web/admin/help.py` & `evennia-4.1.1/evennia/web/admin/help.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/web/admin/objects.py` & `evennia-4.1.1/evennia/web/admin/objects.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/web/admin/scripts.py` & `evennia-4.1.1/evennia/web/admin/scripts.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/web/admin/tags.py` & `evennia-4.1.1/evennia/web/admin/tags.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/web/admin/urls.py` & `evennia-4.1.1/evennia/web/admin/urls.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/web/admin/utils.py` & `evennia-4.1.1/evennia/web/admin/utils.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/web/api/README.md` & `evennia-4.1.1/evennia/web/api/README.md`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/web/api/filters.py` & `evennia-4.1.1/evennia/web/api/filters.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/web/api/permissions.py` & `evennia-4.1.1/evennia/web/api/permissions.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/web/api/serializers.py` & `evennia-4.1.1/evennia/web/api/serializers.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/web/api/tests.py` & `evennia-4.1.1/evennia/web/api/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/web/api/urls.py` & `evennia-4.1.1/evennia/web/api/urls.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/web/api/views.py` & `evennia-4.1.1/evennia/web/api/views.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/web/static/rest_framework/images/favicon.ico` & `evennia-4.1.1/evennia/web/static/rest_framework/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/web/static/webclient/css/goldenlayout.css` & `evennia-4.1.1/evennia/web/static/webclient/css/goldenlayout.css`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/web/static/webclient/css/webclient.css` & `evennia-4.1.1/evennia/web/static/webclient/css/webclient.css`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/web/static/webclient/fonts/DejaVuSansMono-webfont.woff` & `evennia-4.1.1/evennia/web/static/webclient/fonts/DejaVuSansMono-webfont.woff`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/web/static/webclient/js/evennia.js` & `evennia-4.1.1/evennia/web/static/webclient/js/evennia.js`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/web/static/webclient/js/plugins/clienthelp.js` & `evennia-4.1.1/evennia/web/static/webclient/js/plugins/clienthelp.js`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/web/static/webclient/js/plugins/default_in.js` & `evennia-4.1.1/evennia/web/static/webclient/js/plugins/default_in.js`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/web/static/webclient/js/plugins/default_out.js` & `evennia-4.1.1/evennia/web/static/webclient/js/plugins/default_out.js`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/web/static/webclient/js/plugins/font.js` & `evennia-4.1.1/evennia/web/static/webclient/js/plugins/font.js`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/web/static/webclient/js/plugins/goldenlayout.js` & `evennia-4.1.1/evennia/web/static/webclient/js/plugins/goldenlayout.js`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/web/static/webclient/js/plugins/goldenlayout_default_config.js` & `evennia-4.1.1/evennia/web/static/webclient/js/plugins/goldenlayout_default_config.js`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/web/static/webclient/js/plugins/history.js` & `evennia-4.1.1/evennia/web/static/webclient/js/plugins/history.js`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/web/static/webclient/js/plugins/hotbuttons.js` & `evennia-4.1.1/evennia/web/static/webclient/js/plugins/hotbuttons.js`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/web/static/webclient/js/plugins/html.js` & `evennia-4.1.1/evennia/web/static/webclient/js/plugins/html.js`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/web/static/webclient/js/plugins/iframe.js` & `evennia-4.1.1/evennia/web/static/webclient/js/plugins/iframe.js`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/web/static/webclient/js/plugins/message_routing.js` & `evennia-4.1.1/evennia/web/static/webclient/js/plugins/message_routing.js`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/web/static/webclient/js/plugins/multimedia.js` & `evennia-4.1.1/evennia/web/static/webclient/js/plugins/multimedia.js`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/web/static/webclient/js/plugins/notifications.js` & `evennia-4.1.1/evennia/web/static/webclient/js/plugins/notifications.js`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/web/static/webclient/js/plugins/oob.js` & `evennia-4.1.1/evennia/web/static/webclient/js/plugins/oob.js`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/web/static/webclient/js/plugins/options2.js` & `evennia-4.1.1/evennia/web/static/webclient/js/plugins/options2.js`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/web/static/webclient/js/plugins/popups.js` & `evennia-4.1.1/evennia/web/static/webclient/js/plugins/popups.js`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/web/static/webclient/js/plugins/text2html.js` & `evennia-4.1.1/evennia/web/static/webclient/js/plugins/text2html.js`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/web/static/webclient/js/webclient_gui.js` & `evennia-4.1.1/evennia/web/static/webclient/js/webclient_gui.js`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/web/static/webclient/media/notification.wav` & `evennia-4.1.1/evennia/web/static/webclient/media/notification.wav`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/web/static/website/css/website.css` & `evennia-4.1.1/evennia/web/static/website/css/website.css`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/web/static/website/images/evennia_logo.png` & `evennia-4.1.1/evennia/web/static/website/images/evennia_logo.png`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/web/static/website/images/evennia_logo_festive.png` & `evennia-4.1.1/evennia/web/static/website/images/evennia_logo_festive.png`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/web/static/website/images/favicon.ico` & `evennia-4.1.1/evennia/web/static/website/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/web/templates/admin/app_list.html` & `evennia-4.1.1/evennia/web/templates/admin/app_list.html`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/web/templates/admin/frontpage.html` & `evennia-4.1.1/evennia/web/templates/admin/frontpage.html`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/web/templates/rest_framework/api.html` & `evennia-4.1.1/evennia/web/templates/rest_framework/api.html`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/web/templates/webclient/base.html` & `evennia-4.1.1/evennia/web/templates/webclient/base.html`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/web/templates/webclient/webclient.html` & `evennia-4.1.1/evennia/web/templates/webclient/webclient.html`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/web/templates/website/500.html` & `evennia-4.1.1/evennia/web/templates/website/500.html`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/web/templates/website/_menu.html` & `evennia-4.1.1/evennia/web/templates/website/_menu.html`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/web/templates/website/base.html` & `evennia-4.1.1/evennia/web/templates/website/base.html`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/web/templates/website/channel_detail.html` & `evennia-4.1.1/evennia/web/templates/website/channel_detail.html`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/web/templates/website/channel_list.html` & `evennia-4.1.1/evennia/web/templates/website/channel_list.html`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/web/templates/website/character_form.html` & `evennia-4.1.1/evennia/web/templates/website/character_form.html`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/web/templates/website/character_list.html` & `evennia-4.1.1/evennia/web/templates/website/character_list.html`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/web/templates/website/character_manage_list.html` & `evennia-4.1.1/evennia/web/templates/website/character_manage_list.html`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/web/templates/website/generic_form.html` & `evennia-4.1.1/evennia/web/templates/website/generic_form.html`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/web/templates/website/help_detail.html` & `evennia-4.1.1/evennia/web/templates/website/help_detail.html`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/web/templates/website/help_list.html` & `evennia-4.1.1/evennia/web/templates/website/help_list.html`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/web/templates/website/homepage/accounts-widget.html` & `evennia-4.1.1/evennia/web/templates/website/homepage/accounts-widget.html`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/web/templates/website/homepage/database-stats-widget.html` & `evennia-4.1.1/evennia/web/templates/website/homepage/database-stats-widget.html`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/web/templates/website/homepage/evennia-widget.html` & `evennia-4.1.1/evennia/web/templates/website/homepage/evennia-widget.html`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/web/templates/website/homepage/main-content.html` & `evennia-4.1.1/evennia/web/templates/website/homepage/main-content.html`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/web/templates/website/index.html` & `evennia-4.1.1/evennia/web/templates/website/index.html`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/web/templates/website/object_confirm_delete.html` & `evennia-4.1.1/evennia/web/templates/website/object_confirm_delete.html`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/web/templates/website/object_detail.html` & `evennia-4.1.1/evennia/web/templates/website/object_detail.html`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/web/templates/website/object_list.html` & `evennia-4.1.1/evennia/web/templates/website/object_list.html`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/web/templates/website/pagination.html` & `evennia-4.1.1/evennia/web/templates/website/pagination.html`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/web/templates/website/registration/logged_out.html` & `evennia-4.1.1/evennia/web/templates/website/registration/logged_out.html`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/web/templates/website/registration/login.html` & `evennia-4.1.1/evennia/web/templates/website/registration/login.html`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/web/templates/website/registration/password_change_done.html` & `evennia-4.1.1/evennia/web/templates/website/registration/password_change_done.html`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/web/templates/website/registration/password_change_form.html` & `evennia-4.1.1/evennia/web/templates/website/registration/password_change_form.html`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/web/templates/website/registration/password_reset_complete.html` & `evennia-4.1.1/evennia/web/templates/website/registration/password_reset_complete.html`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/web/templates/website/registration/password_reset_confirm.html` & `evennia-4.1.1/evennia/web/templates/website/registration/password_reset_confirm.html`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/web/templates/website/registration/password_reset_done.html` & `evennia-4.1.1/evennia/web/templates/website/registration/password_reset_done.html`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/web/templates/website/registration/password_reset_email.html` & `evennia-4.1.1/evennia/web/templates/website/registration/password_reset_email.html`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/web/templates/website/registration/password_reset_form.html` & `evennia-4.1.1/evennia/web/templates/website/registration/password_reset_form.html`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/web/templates/website/registration/register.html` & `evennia-4.1.1/evennia/web/templates/website/registration/register.html`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/web/templates/website/tbi.html` & `evennia-4.1.1/evennia/web/templates/website/tbi.html`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/web/templatetags/addclass.py` & `evennia-4.1.1/evennia/web/templatetags/addclass.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/web/urls.py` & `evennia-4.1.1/evennia/web/urls.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/web/utils/adminsite.py` & `evennia-4.1.1/evennia/web/utils/adminsite.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/web/utils/apache_wsgi.conf` & `evennia-4.1.1/evennia/web/utils/apache_wsgi.conf`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/web/utils/backends.py` & `evennia-4.1.1/evennia/web/utils/backends.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/web/utils/evennia_modpy_apache.conf` & `evennia-4.1.1/evennia/web/utils/evennia_modpy_apache.conf`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/web/utils/evennia_wsgi_apache.conf` & `evennia-4.1.1/evennia/web/utils/evennia_wsgi_apache.conf`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/web/utils/general_context.py` & `evennia-4.1.1/evennia/web/utils/general_context.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/web/utils/middleware.py` & `evennia-4.1.1/evennia/web/utils/middleware.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/web/utils/tests.py` & `evennia-4.1.1/evennia/web/utils/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/web/webclient/views.py` & `evennia-4.1.1/evennia/web/webclient/views.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/web/website/forms.py` & `evennia-4.1.1/evennia/web/website/forms.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/web/website/tests.py` & `evennia-4.1.1/evennia/web/website/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/web/website/urls.py` & `evennia-4.1.1/evennia/web/website/urls.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/web/website/views/accounts.py` & `evennia-4.1.1/evennia/web/website/views/accounts.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/web/website/views/channels.py` & `evennia-4.1.1/evennia/web/website/views/channels.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/web/website/views/characters.py` & `evennia-4.1.1/evennia/web/website/views/characters.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/web/website/views/help.py` & `evennia-4.1.1/evennia/web/website/views/help.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/web/website/views/index.py` & `evennia-4.1.1/evennia/web/website/views/index.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/web/website/views/mixins.py` & `evennia-4.1.1/evennia/web/website/views/mixins.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia/web/website/views/objects.py` & `evennia-4.1.1/evennia/web/website/views/objects.py`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia.egg-info/PKG-INFO` & `evennia-4.1.1/evennia.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evennia
-Version: 4.1.0
+Version: 4.1.1
 Summary: A full-featured toolkit and server for text-based multiplayer games (MUDs, MU*, etc).
 Maintainer-email: Griatch <griatch@gmail.com>
 License: BSD
 Project-URL: Homepage, https://www.evennia.com
 Project-URL: Github, https://github.com/evennia/evennia
 Project-URL: Documentation, https://www.evennia.com/docs/latest/index.html
 Project-URL: Live Demo, https://demo.evennia.com/
```

### Comparing `evennia-4.1.0/evennia.egg-info/SOURCES.txt` & `evennia-4.1.1/evennia.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/evennia.egg-info/requires.txt` & `evennia-4.1.1/evennia.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `evennia-4.1.0/pyproject.toml` & `evennia-4.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "evennia"
-version = "4.1.0"
+version = "4.1.1"
 maintainers = [{ name = "Griatch", email = "griatch@gmail.com" }]
 description = "A full-featured toolkit and server for text-based multiplayer games (MUDs, MU*, etc)."
 requires-python = ">=3.10"
 readme = { file = "README.md", content-type = "text/markdown" }
 license = { text = "BSD" }
 keywords = [
   "MUD",
```

### Comparing `evennia-4.1.0/setup.py` & `evennia-4.1.1/setup.py`

 * *Files identical despite different names*

