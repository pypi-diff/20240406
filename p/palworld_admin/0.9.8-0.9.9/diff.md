# Comparing `tmp/palworld_admin-0.9.8.tar.gz` & `tmp/palworld_admin-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "palworld_admin-0.9.8.tar", max compression
+gzip compressed data, was "palworld_admin-0.9.9.tar", max compression
```

## Comparing `palworld_admin-0.9.8.tar` & `palworld_admin-0.9.9.tar`

### file list

```diff
@@ -1,83 +1,84 @@
--rw-r--r--   0        0        0        0 2024-02-14 05:03:47.786080 palworld_admin-0.9.8/palworld_admin/__init__.py
--rw-r--r--   0        0        0      231 2024-02-15 17:00:06.547705 palworld_admin-0.9.8/palworld_admin/classes/__init__.py
--rw-r--r--   0        0        0     3271 2024-03-14 15:14:56.430666 palworld_admin-0.9.8/palworld_admin/classes/dbmodels.py
--rw-r--r--   0        0        0     2717 2024-03-16 13:01:51.942126 palworld_admin-0.9.8/palworld_admin/classes/localserver.py
--rw-r--r--   0        0        0     3221 2024-02-07 14:55:41.667929 palworld_admin-0.9.8/palworld_admin/classes/memorystorage.py
--rw-r--r--   0        0        0    15613 2024-02-28 12:05:05.450133 palworld_admin-0.9.8/palworld_admin/classes/palworldsettings.py
--rw-r--r--   0        0        0     4026 2024-02-14 14:29:41.390319 palworld_admin-0.9.8/palworld_admin/converter/convert.py
--rw-r--r--   0        0        0        0 2024-01-30 14:26:22.000000 palworld_admin-0.9.8/palworld_admin/converter/lib/__init__.py
--rw-r--r--   0        0        0    28976 2024-02-04 01:47:03.567608 palworld_admin-0.9.8/palworld_admin/converter/lib/archive.py
--rw-r--r--   0        0        0     6000 2024-02-14 14:30:02.314946 palworld_admin-0.9.8/palworld_admin/converter/lib/gvas.py
--rw-r--r--   0        0        0     2379 2024-01-30 14:26:22.000000 palworld_admin-0.9.8/palworld_admin/converter/lib/noindent.py
--rw-r--r--   0        0        0     2188 2024-01-30 14:26:22.000000 palworld_admin-0.9.8/palworld_admin/converter/lib/palsav.py
--rw-r--r--   0        0        0     6050 2024-02-14 14:29:48.858207 palworld_admin-0.9.8/palworld_admin/converter/lib/paltypes.py
--rw-r--r--   0        0        0        0 2024-01-30 14:26:22.000000 palworld_admin-0.9.8/palworld_admin/converter/lib/rawdata/__init__.py
--rw-r--r--   0        0        0     1896 2024-02-14 14:31:00.252519 palworld_admin-0.9.8/palworld_admin/converter/lib/rawdata/base_camp.py
--rw-r--r--   0        0        0     4139 2024-02-14 14:31:13.232419 palworld_admin-0.9.8/palworld_admin/converter/lib/rawdata/base_camp_module.py
--rw-r--r--   0        0        0     1360 2024-02-14 14:30:57.393422 palworld_admin-0.9.8/palworld_admin/converter/lib/rawdata/build_process.py
--rw-r--r--   0        0        0     1519 2024-02-14 14:30:52.965159 palworld_admin-0.9.8/palworld_admin/converter/lib/rawdata/character.py
--rw-r--r--   0        0        0     1565 2024-02-14 14:30:55.145221 palworld_admin-0.9.8/palworld_admin/converter/lib/rawdata/character_container.py
--rw-r--r--   0        0        0     2823 2024-02-14 14:30:50.651103 palworld_admin-0.9.8/palworld_admin/converter/lib/rawdata/connector.py
--rw-r--r--   0        0        0      930 2024-02-14 14:30:47.706295 palworld_admin-0.9.8/palworld_admin/converter/lib/rawdata/debug.py
--rw-r--r--   0        0        0     3723 2024-02-14 14:31:37.121834 palworld_admin-0.9.8/palworld_admin/converter/lib/rawdata/dynamic_item.py
--rw-r--r--   0        0        0     1633 2024-02-14 14:30:39.151955 palworld_admin-0.9.8/palworld_admin/converter/lib/rawdata/foliage_model.py
--rw-r--r--   0        0        0     2179 2024-02-14 14:30:41.927746 palworld_admin-0.9.8/palworld_admin/converter/lib/rawdata/foliage_model_instance.py
--rw-r--r--   0        0        0     4759 2024-02-14 14:30:36.699049 palworld_admin-0.9.8/palworld_admin/converter/lib/rawdata/group.py
--rw-r--r--   0        0        0     1766 2024-02-14 14:30:31.749480 palworld_admin-0.9.8/palworld_admin/converter/lib/rawdata/item_container.py
--rw-r--r--   0        0        0     1870 2024-02-14 14:30:33.911420 palworld_admin-0.9.8/palworld_admin/converter/lib/rawdata/item_container_slots.py
--rw-r--r--   0        0        0     2810 2024-02-14 14:30:29.445165 palworld_admin-0.9.8/palworld_admin/converter/lib/rawdata/map_concrete_model.py
--rw-r--r--   0        0        0     2661 2024-02-14 14:30:26.661016 palworld_admin-0.9.8/palworld_admin/converter/lib/rawdata/map_model.py
--rw-r--r--   0        0        0     1394 2024-02-14 14:30:24.056405 palworld_admin-0.9.8/palworld_admin/converter/lib/rawdata/work_collection.py
--rw-r--r--   0        0        0     1646 2024-02-14 14:30:19.048388 palworld_admin-0.9.8/palworld_admin/converter/lib/rawdata/worker_director.py
--rw-r--r--   0        0        0        0 2024-02-14 03:22:39.448105 palworld_admin-0.9.8/palworld_admin/helper/__init__.py
--rw-r--r--   0        0        0     2525 2024-03-06 15:00:51.835673 palworld_admin-0.9.8/palworld_admin/helper/cli.py
--rw-r--r--   0        0        0      815 2024-03-04 18:44:39.943860 palworld_admin-0.9.8/palworld_admin/helper/consolemanagement.py
--rw-r--r--   0        0        0     7158 2024-03-15 17:43:47.537707 palworld_admin-0.9.8/palworld_admin/helper/dbmanagement.py
--rw-r--r--   0        0        0     2633 2024-03-05 03:45:08.423924 palworld_admin-0.9.8/palworld_admin/helper/dbmigration.py
--rw-r--r--   0        0        0     2855 2024-03-08 17:43:28.960082 palworld_admin-0.9.8/palworld_admin/helper/fileprocessing.py
--rw-r--r--   0        0        0     2277 2024-03-08 17:19:38.174840 palworld_admin-0.9.8/palworld_admin/helper/networking.py
--rw-r--r--   0        0        0     2834 2024-03-10 22:35:49.884735 palworld_admin-0.9.8/palworld_admin/helper/oscommands.py
--rw-r--r--   0        0        0      335 2024-02-07 12:03:32.534896 palworld_admin-0.9.8/palworld_admin/helper/threads.py
--rw-r--r--   0        0        0    96075 2019-10-05 22:44:46.000000 palworld_admin-0.9.8/palworld_admin/icon.png
--rw-r--r--   0        0        0     2655 2024-03-04 18:53:14.275108 palworld_admin-0.9.8/palworld_admin/main.py
--rw-r--r--   0        0        0      857 2024-02-22 07:45:36.451512 palworld_admin-0.9.8/palworld_admin/migrations/alembic.ini
--rw-r--r--   0        0        0     3344 2024-02-22 07:45:36.457512 palworld_admin-0.9.8/palworld_admin/migrations/env.py
--rw-r--r--   0        0        0       41 2024-02-22 07:45:36.462513 palworld_admin-0.9.8/palworld_admin/migrations/README
--rw-r--r--   0        0        0      494 2024-02-22 07:45:36.466513 palworld_admin-0.9.8/palworld_admin/migrations/script.py.mako
--rw-r--r--   0        0        0      964 2024-02-28 11:35:48.293871 palworld_admin-0.9.8/palworld_admin/migrations/versions/170971d44a48_removed_epicapp_palserver_added_query_.py
--rw-r--r--   0        0        0      842 2024-02-27 12:56:10.611969 palworld_admin-0.9.8/palworld_admin/migrations/versions/3103e5ae5314_added_publiclobby_to_launchersettings.py
--rw-r--r--   0        0        0     1072 2024-03-14 15:15:11.034540 palworld_admin-0.9.8/palworld_admin/migrations/versions/59a004fd30a9_added_players_table_added_steamauth_and_.py
--rw-r--r--   0        0        0      579 2024-02-22 07:58:51.155721 palworld_admin-0.9.8/palworld_admin/migrations/versions/ae1eab510d76_added_auto_restart_on_unexpected_.py
--rw-r--r--   0        0        0      857 2024-02-22 07:45:36.451512 palworld_admin-0.9.8/palworld_admin/migrations-backup/version 1 - ae1eab510d76/alembic.ini
--rw-r--r--   0        0        0     3344 2024-02-22 07:45:36.457512 palworld_admin-0.9.8/palworld_admin/migrations-backup/version 1 - ae1eab510d76/env.py
--rw-r--r--   0        0        0       41 2024-02-22 07:45:36.462513 palworld_admin-0.9.8/palworld_admin/migrations-backup/version 1 - ae1eab510d76/README
--rw-r--r--   0        0        0      494 2024-02-22 07:45:36.466513 palworld_admin-0.9.8/palworld_admin/migrations-backup/version 1 - ae1eab510d76/script.py.mako
--rw-r--r--   0        0        0      579 2024-02-22 07:58:51.155721 palworld_admin-0.9.8/palworld_admin/migrations-backup/version 1 - ae1eab510d76/versions/ae1eab510d76_added_auto_restart_on_unexpected_.py
--rw-r--r--   0        0        0      857 2024-02-22 07:45:36.451512 palworld_admin-0.9.8/palworld_admin/migrations-backup/version 2 - 3103e5ae5314/alembic.ini
--rw-r--r--   0        0        0     3344 2024-02-22 07:45:36.457512 palworld_admin-0.9.8/palworld_admin/migrations-backup/version 2 - 3103e5ae5314/env.py
--rw-r--r--   0        0        0       41 2024-02-22 07:45:36.462513 palworld_admin-0.9.8/palworld_admin/migrations-backup/version 2 - 3103e5ae5314/README
--rw-r--r--   0        0        0      494 2024-02-22 07:45:36.466513 palworld_admin-0.9.8/palworld_admin/migrations-backup/version 2 - 3103e5ae5314/script.py.mako
--rw-r--r--   0        0        0      842 2024-02-27 12:56:10.611969 palworld_admin-0.9.8/palworld_admin/migrations-backup/version 2 - 3103e5ae5314/versions/3103e5ae5314_added_publiclobby_to_launchersettings.py
--rw-r--r--   0        0        0      579 2024-02-22 07:58:51.155721 palworld_admin-0.9.8/palworld_admin/migrations-backup/version 2 - 3103e5ae5314/versions/ae1eab510d76_added_auto_restart_on_unexpected_.py
--rw-r--r--   0        0        0    29965 2024-03-17 11:48:47.398140 palworld_admin-0.9.8/palworld_admin/rcon/__init__.py
--rw-r--r--   0        0        0    12633 2024-03-05 20:48:03.656963 palworld_admin-0.9.8/palworld_admin/rcon/rcon.py
--rw-r--r--   0        0        0    66914 2024-03-16 21:51:54.955507 palworld_admin-0.9.8/palworld_admin/servermanager/__init__.py
--rw-r--r--   0        0        0    17074 2024-03-18 01:30:39.238894 palworld_admin-0.9.8/palworld_admin/settings.py
--rw-r--r--   0        0        0    54708 2024-03-17 11:37:27.312183 palworld_admin-0.9.8/palworld_admin/website/__init__.py
--rw-r--r--   0        0        0   232948 2024-02-18 19:53:43.391786 palworld_admin-0.9.8/palworld_admin/website/resources/css/bootstrap.min.css
--rw-r--r--   0        0        0    98255 2024-02-18 19:54:08.576413 palworld_admin-0.9.8/palworld_admin/website/resources/font/bootstrap-icons.css
--rw-r--r--   0        0        0   176032 2024-02-18 20:10:49.750275 palworld_admin-0.9.8/palworld_admin/website/resources/font/fonts/bootstrap-icons.woff
--rw-r--r--   0        0        0   130396 2024-02-18 20:09:57.629334 palworld_admin-0.9.8/palworld_admin/website/resources/font/fonts/bootstrap-icons.woff2
--rw-r--r--   0        0        0    23710 2024-02-16 15:12:21.097164 palworld_admin-0.9.8/palworld_admin/website/resources/images/favicon.ico
--rw-r--r--   0        0        0   256841 2024-02-03 16:58:02.594994 palworld_admin-0.9.8/palworld_admin/website/resources/images/palworld-logo.png
--rw-r--r--   0        0        0    60577 2024-02-18 19:54:16.464908 palworld_admin-0.9.8/palworld_admin/website/resources/js/bootstrap.min.js
--rw-r--r--   0        0        0    87533 2024-02-18 19:54:31.314068 palworld_admin-0.9.8/palworld_admin/website/resources/js/jquery-3.7.1.min.js
--rw-r--r--   0        0        0    49732 2024-02-18 19:54:36.598219 palworld_admin-0.9.8/palworld_admin/website/resources/js/socket.io.min.js
--rw-r--r--   0        0        0    10413 2024-02-21 16:36:00.194740 palworld_admin-0.9.8/palworld_admin/website/views.py
--rw-r--r--   0        0        0      905 2024-03-18 01:27:43.768134 palworld_admin-0.9.8/pyproject.toml
--rw-r--r--   0        0        0    13874 2024-03-18 01:28:24.405092 palworld_admin-0.9.8/README.md
--rw-r--r--   0        0        0   199372 2024-02-17 17:12:58.703357 palworld_admin-0.9.8/ui/assets/icon.ico
--rw-r--r--   0        0        0     5518 2024-03-02 21:11:39.695776 palworld_admin-0.9.8/ui/main.js
--rw-r--r--   0        0        0    86170 2024-02-18 19:43:18.426113 palworld_admin-0.9.8/ui/package-lock.json
--rw-r--r--   0        0        0      359 2024-02-24 13:36:34.429753 palworld_admin-0.9.8/ui/package.json
--rw-r--r--   0        0        0    14546 1970-01-01 00:00:00.000000 palworld_admin-0.9.8/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-02-14 05:03:47.786080 palworld_admin-0.9.9/palworld_admin/__init__.py
+-rw-r--r--   0        0        0      231 2024-02-15 17:00:06.547705 palworld_admin-0.9.9/palworld_admin/classes/__init__.py
+-rw-r--r--   0        0        0     3271 2024-03-14 15:14:56.430666 palworld_admin-0.9.9/palworld_admin/classes/dbmodels.py
+-rw-r--r--   0        0        0     2809 2024-03-18 23:09:34.773080 palworld_admin-0.9.9/palworld_admin/classes/localserver.py
+-rw-r--r--   0        0        0     3221 2024-02-07 14:55:41.667929 palworld_admin-0.9.9/palworld_admin/classes/memorystorage.py
+-rw-r--r--   0        0        0    15613 2024-02-28 12:05:05.450133 palworld_admin-0.9.9/palworld_admin/classes/palworldsettings.py
+-rw-r--r--   0        0        0     4026 2024-02-14 14:29:41.390319 palworld_admin-0.9.9/palworld_admin/converter/convert.py
+-rw-r--r--   0        0        0        0 2024-01-30 14:26:22.000000 palworld_admin-0.9.9/palworld_admin/converter/lib/__init__.py
+-rw-r--r--   0        0        0    28976 2024-02-04 01:47:03.567608 palworld_admin-0.9.9/palworld_admin/converter/lib/archive.py
+-rw-r--r--   0        0        0     6000 2024-02-14 14:30:02.314946 palworld_admin-0.9.9/palworld_admin/converter/lib/gvas.py
+-rw-r--r--   0        0        0     2379 2024-01-30 14:26:22.000000 palworld_admin-0.9.9/palworld_admin/converter/lib/noindent.py
+-rw-r--r--   0        0        0     2188 2024-01-30 14:26:22.000000 palworld_admin-0.9.9/palworld_admin/converter/lib/palsav.py
+-rw-r--r--   0        0        0     6050 2024-02-14 14:29:48.858207 palworld_admin-0.9.9/palworld_admin/converter/lib/paltypes.py
+-rw-r--r--   0        0        0        0 2024-01-30 14:26:22.000000 palworld_admin-0.9.9/palworld_admin/converter/lib/rawdata/__init__.py
+-rw-r--r--   0        0        0     1896 2024-02-14 14:31:00.252519 palworld_admin-0.9.9/palworld_admin/converter/lib/rawdata/base_camp.py
+-rw-r--r--   0        0        0     4139 2024-02-14 14:31:13.232419 palworld_admin-0.9.9/palworld_admin/converter/lib/rawdata/base_camp_module.py
+-rw-r--r--   0        0        0     1360 2024-02-14 14:30:57.393422 palworld_admin-0.9.9/palworld_admin/converter/lib/rawdata/build_process.py
+-rw-r--r--   0        0        0     1519 2024-02-14 14:30:52.965159 palworld_admin-0.9.9/palworld_admin/converter/lib/rawdata/character.py
+-rw-r--r--   0        0        0     1565 2024-02-14 14:30:55.145221 palworld_admin-0.9.9/palworld_admin/converter/lib/rawdata/character_container.py
+-rw-r--r--   0        0        0     2823 2024-02-14 14:30:50.651103 palworld_admin-0.9.9/palworld_admin/converter/lib/rawdata/connector.py
+-rw-r--r--   0        0        0      930 2024-02-14 14:30:47.706295 palworld_admin-0.9.9/palworld_admin/converter/lib/rawdata/debug.py
+-rw-r--r--   0        0        0     3723 2024-02-14 14:31:37.121834 palworld_admin-0.9.9/palworld_admin/converter/lib/rawdata/dynamic_item.py
+-rw-r--r--   0        0        0     1633 2024-02-14 14:30:39.151955 palworld_admin-0.9.9/palworld_admin/converter/lib/rawdata/foliage_model.py
+-rw-r--r--   0        0        0     2179 2024-02-14 14:30:41.927746 palworld_admin-0.9.9/palworld_admin/converter/lib/rawdata/foliage_model_instance.py
+-rw-r--r--   0        0        0     4759 2024-02-14 14:30:36.699049 palworld_admin-0.9.9/palworld_admin/converter/lib/rawdata/group.py
+-rw-r--r--   0        0        0     1766 2024-02-14 14:30:31.749480 palworld_admin-0.9.9/palworld_admin/converter/lib/rawdata/item_container.py
+-rw-r--r--   0        0        0     1870 2024-02-14 14:30:33.911420 palworld_admin-0.9.9/palworld_admin/converter/lib/rawdata/item_container_slots.py
+-rw-r--r--   0        0        0     2810 2024-02-14 14:30:29.445165 palworld_admin-0.9.9/palworld_admin/converter/lib/rawdata/map_concrete_model.py
+-rw-r--r--   0        0        0     2661 2024-02-14 14:30:26.661016 palworld_admin-0.9.9/palworld_admin/converter/lib/rawdata/map_model.py
+-rw-r--r--   0        0        0     1394 2024-02-14 14:30:24.056405 palworld_admin-0.9.9/palworld_admin/converter/lib/rawdata/work_collection.py
+-rw-r--r--   0        0        0     1646 2024-02-14 14:30:19.048388 palworld_admin-0.9.9/palworld_admin/converter/lib/rawdata/worker_director.py
+-rw-r--r--   0        0        0        0 2024-02-14 03:22:39.448105 palworld_admin-0.9.9/palworld_admin/helper/__init__.py
+-rw-r--r--   0        0        0     3075 2024-03-18 22:54:39.031700 palworld_admin-0.9.9/palworld_admin/helper/cli.py
+-rw-r--r--   0        0        0      815 2024-03-04 18:44:39.943860 palworld_admin-0.9.9/palworld_admin/helper/consolemanagement.py
+-rw-r--r--   0        0        0      526 2024-03-18 21:37:23.253142 palworld_admin-0.9.9/palworld_admin/helper/dbcreation.py
+-rw-r--r--   0        0        0     7190 2024-03-18 21:38:19.432666 palworld_admin-0.9.9/palworld_admin/helper/dbmanagement.py
+-rw-r--r--   0        0        0     2089 2024-03-18 21:37:55.407757 palworld_admin-0.9.9/palworld_admin/helper/dbmigration.py
+-rw-r--r--   0        0        0     2855 2024-03-08 17:43:28.960082 palworld_admin-0.9.9/palworld_admin/helper/fileprocessing.py
+-rw-r--r--   0        0        0     2277 2024-03-08 17:19:38.174840 palworld_admin-0.9.9/palworld_admin/helper/networking.py
+-rw-r--r--   0        0        0     2834 2024-03-10 22:35:49.884735 palworld_admin-0.9.9/palworld_admin/helper/oscommands.py
+-rw-r--r--   0        0        0      335 2024-02-07 12:03:32.534896 palworld_admin-0.9.9/palworld_admin/helper/threads.py
+-rw-r--r--   0        0        0    96075 2019-10-05 22:44:46.000000 palworld_admin-0.9.9/palworld_admin/icon.png
+-rw-r--r--   0        0        0      934 2024-03-19 00:26:39.286647 palworld_admin-0.9.9/palworld_admin/main.py
+-rw-r--r--   0        0        0      857 2024-02-22 07:45:36.451512 palworld_admin-0.9.9/palworld_admin/migrations/alembic.ini
+-rw-r--r--   0        0        0     3344 2024-02-22 07:45:36.457512 palworld_admin-0.9.9/palworld_admin/migrations/env.py
+-rw-r--r--   0        0        0       41 2024-02-22 07:45:36.462513 palworld_admin-0.9.9/palworld_admin/migrations/README
+-rw-r--r--   0        0        0      494 2024-02-22 07:45:36.466513 palworld_admin-0.9.9/palworld_admin/migrations/script.py.mako
+-rw-r--r--   0        0        0      964 2024-02-28 11:35:48.293871 palworld_admin-0.9.9/palworld_admin/migrations/versions/170971d44a48_removed_epicapp_palserver_added_query_.py
+-rw-r--r--   0        0        0      842 2024-02-27 12:56:10.611969 palworld_admin-0.9.9/palworld_admin/migrations/versions/3103e5ae5314_added_publiclobby_to_launchersettings.py
+-rw-r--r--   0        0        0     1072 2024-03-14 15:15:11.034540 palworld_admin-0.9.9/palworld_admin/migrations/versions/59a004fd30a9_added_players_table_added_steamauth_and_.py
+-rw-r--r--   0        0        0      579 2024-02-22 07:58:51.155721 palworld_admin-0.9.9/palworld_admin/migrations/versions/ae1eab510d76_added_auto_restart_on_unexpected_.py
+-rw-r--r--   0        0        0      857 2024-02-22 07:45:36.451512 palworld_admin-0.9.9/palworld_admin/migrations-backup/version 1 - ae1eab510d76/alembic.ini
+-rw-r--r--   0        0        0     3344 2024-02-22 07:45:36.457512 palworld_admin-0.9.9/palworld_admin/migrations-backup/version 1 - ae1eab510d76/env.py
+-rw-r--r--   0        0        0       41 2024-02-22 07:45:36.462513 palworld_admin-0.9.9/palworld_admin/migrations-backup/version 1 - ae1eab510d76/README
+-rw-r--r--   0        0        0      494 2024-02-22 07:45:36.466513 palworld_admin-0.9.9/palworld_admin/migrations-backup/version 1 - ae1eab510d76/script.py.mako
+-rw-r--r--   0        0        0      579 2024-02-22 07:58:51.155721 palworld_admin-0.9.9/palworld_admin/migrations-backup/version 1 - ae1eab510d76/versions/ae1eab510d76_added_auto_restart_on_unexpected_.py
+-rw-r--r--   0        0        0      857 2024-02-22 07:45:36.451512 palworld_admin-0.9.9/palworld_admin/migrations-backup/version 2 - 3103e5ae5314/alembic.ini
+-rw-r--r--   0        0        0     3344 2024-02-22 07:45:36.457512 palworld_admin-0.9.9/palworld_admin/migrations-backup/version 2 - 3103e5ae5314/env.py
+-rw-r--r--   0        0        0       41 2024-02-22 07:45:36.462513 palworld_admin-0.9.9/palworld_admin/migrations-backup/version 2 - 3103e5ae5314/README
+-rw-r--r--   0        0        0      494 2024-02-22 07:45:36.466513 palworld_admin-0.9.9/palworld_admin/migrations-backup/version 2 - 3103e5ae5314/script.py.mako
+-rw-r--r--   0        0        0      842 2024-02-27 12:56:10.611969 palworld_admin-0.9.9/palworld_admin/migrations-backup/version 2 - 3103e5ae5314/versions/3103e5ae5314_added_publiclobby_to_launchersettings.py
+-rw-r--r--   0        0        0      579 2024-02-22 07:58:51.155721 palworld_admin-0.9.9/palworld_admin/migrations-backup/version 2 - 3103e5ae5314/versions/ae1eab510d76_added_auto_restart_on_unexpected_.py
+-rw-r--r--   0        0        0    29965 2024-03-17 11:48:47.398140 palworld_admin-0.9.9/palworld_admin/rcon/__init__.py
+-rw-r--r--   0        0        0    12633 2024-03-05 20:48:03.656963 palworld_admin-0.9.9/palworld_admin/rcon/rcon.py
+-rw-r--r--   0        0        0    67100 2024-03-19 01:38:41.317295 palworld_admin-0.9.9/palworld_admin/servermanager/__init__.py
+-rw-r--r--   0        0        0    19403 2024-03-19 02:04:40.979861 palworld_admin-0.9.9/palworld_admin/settings.py
+-rw-r--r--   0        0        0    57284 2024-03-19 02:05:16.921700 palworld_admin-0.9.9/palworld_admin/website/__init__.py
+-rw-r--r--   0        0        0   232948 2024-02-18 19:53:43.391786 palworld_admin-0.9.9/palworld_admin/website/resources/css/bootstrap.min.css
+-rw-r--r--   0        0        0    98255 2024-02-18 19:54:08.576413 palworld_admin-0.9.9/palworld_admin/website/resources/font/bootstrap-icons.css
+-rw-r--r--   0        0        0   176032 2024-02-18 20:10:49.750275 palworld_admin-0.9.9/palworld_admin/website/resources/font/fonts/bootstrap-icons.woff
+-rw-r--r--   0        0        0   130396 2024-02-18 20:09:57.629334 palworld_admin-0.9.9/palworld_admin/website/resources/font/fonts/bootstrap-icons.woff2
+-rw-r--r--   0        0        0    23710 2024-02-16 15:12:21.097164 palworld_admin-0.9.9/palworld_admin/website/resources/images/favicon.ico
+-rw-r--r--   0        0        0   256841 2024-02-03 16:58:02.594994 palworld_admin-0.9.9/palworld_admin/website/resources/images/palworld-logo.png
+-rw-r--r--   0        0        0    60577 2024-02-18 19:54:16.464908 palworld_admin-0.9.9/palworld_admin/website/resources/js/bootstrap.min.js
+-rw-r--r--   0        0        0    87533 2024-02-18 19:54:31.314068 palworld_admin-0.9.9/palworld_admin/website/resources/js/jquery-3.7.1.min.js
+-rw-r--r--   0        0        0    49732 2024-02-18 19:54:36.598219 palworld_admin-0.9.9/palworld_admin/website/resources/js/socket.io.min.js
+-rw-r--r--   0        0        0    10413 2024-02-21 16:36:00.194740 palworld_admin-0.9.9/palworld_admin/website/views.py
+-rw-r--r--   0        0        0      905 2024-03-19 00:34:48.828957 palworld_admin-0.9.9/pyproject.toml
+-rw-r--r--   0        0        0    13874 2024-03-18 01:28:24.405092 palworld_admin-0.9.9/README.md
+-rw-r--r--   0        0        0   199372 2024-02-17 17:12:58.703357 palworld_admin-0.9.9/ui/assets/icon.ico
+-rw-r--r--   0        0        0     5738 2024-03-18 21:02:55.372991 palworld_admin-0.9.9/ui/main.js
+-rw-r--r--   0        0        0    86170 2024-02-18 19:43:18.426113 palworld_admin-0.9.9/ui/package-lock.json
+-rw-r--r--   0        0        0      359 2024-02-24 13:36:34.429753 palworld_admin-0.9.9/ui/package.json
+-rw-r--r--   0        0        0    14546 1970-01-01 00:00:00.000000 palworld_admin-0.9.9/PKG-INFO
```

### Comparing `palworld_admin-0.9.8/palworld_admin/classes/dbmodels.py` & `palworld_admin-0.9.9/palworld_admin/classes/dbmodels.py`

 * *Files identical despite different names*

### Comparing `palworld_admin-0.9.8/palworld_admin/classes/localserver.py` & `palworld_admin-0.9.9/palworld_admin/classes/localserver.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
         self.palguard_installed: bool = False
         self.server_process: subprocess.Popen = None
         self.online_players: list = []
         self.last_online_players: list = []
         self.all_players: list = []
 
         # RCON Variables
+        self.rcon_last_connection_args: dict = {}
         self.base64_encoded: bool = False
         self.connected: bool = False
         self.launch_rcon_on_startup: bool = False
         self.rcon_monitoring_interval = 2
         self.rcon_monitoring_connection_error_count = 0
         self.ip: str = ""
         self.port: int = 0
@@ -44,14 +45,15 @@
         self.first_run: bool = False
         self.shutting_down: bool = False
         self.restarting: bool = False
         self.running_check_count: int = 0
         self.server_monitoring_interval = 5
         self.player_commit_to_db_interval = 60
         self.launcher_args: dict = {}
+        self.server_settings: dict = {}
 
         # Backup Variables
         self.backup_path = ""
         self.data_path = ""
         self.run_auto_backup: bool = False
         self.backup_interval = 0
         self.backup_retain_count = 0
```

### Comparing `palworld_admin-0.9.8/palworld_admin/classes/memorystorage.py` & `palworld_admin-0.9.9/palworld_admin/classes/memorystorage.py`

 * *Files identical despite different names*

### Comparing `palworld_admin-0.9.8/palworld_admin/classes/palworldsettings.py` & `palworld_admin-0.9.9/palworld_admin/classes/palworldsettings.py`

 * *Files identical despite different names*

### Comparing `palworld_admin-0.9.8/palworld_admin/converter/convert.py` & `palworld_admin-0.9.9/palworld_admin/converter/convert.py`

 * *Files identical despite different names*

### Comparing `palworld_admin-0.9.8/palworld_admin/converter/lib/archive.py` & `palworld_admin-0.9.9/palworld_admin/converter/lib/archive.py`

 * *Files identical despite different names*

### Comparing `palworld_admin-0.9.8/palworld_admin/converter/lib/gvas.py` & `palworld_admin-0.9.9/palworld_admin/converter/lib/gvas.py`

 * *Files identical despite different names*

### Comparing `palworld_admin-0.9.8/palworld_admin/converter/lib/noindent.py` & `palworld_admin-0.9.9/palworld_admin/converter/lib/noindent.py`

 * *Files identical despite different names*

### Comparing `palworld_admin-0.9.8/palworld_admin/converter/lib/palsav.py` & `palworld_admin-0.9.9/palworld_admin/converter/lib/palsav.py`

 * *Files identical despite different names*

### Comparing `palworld_admin-0.9.8/palworld_admin/converter/lib/paltypes.py` & `palworld_admin-0.9.9/palworld_admin/converter/lib/paltypes.py`

 * *Files identical despite different names*

### Comparing `palworld_admin-0.9.8/palworld_admin/converter/lib/rawdata/base_camp.py` & `palworld_admin-0.9.9/palworld_admin/converter/lib/rawdata/base_camp.py`

 * *Files identical despite different names*

### Comparing `palworld_admin-0.9.8/palworld_admin/converter/lib/rawdata/base_camp_module.py` & `palworld_admin-0.9.9/palworld_admin/converter/lib/rawdata/base_camp_module.py`

 * *Files identical despite different names*

### Comparing `palworld_admin-0.9.8/palworld_admin/converter/lib/rawdata/build_process.py` & `palworld_admin-0.9.9/palworld_admin/converter/lib/rawdata/build_process.py`

 * *Files identical despite different names*

### Comparing `palworld_admin-0.9.8/palworld_admin/converter/lib/rawdata/character.py` & `palworld_admin-0.9.9/palworld_admin/converter/lib/rawdata/character.py`

 * *Files identical despite different names*

### Comparing `palworld_admin-0.9.8/palworld_admin/converter/lib/rawdata/character_container.py` & `palworld_admin-0.9.9/palworld_admin/converter/lib/rawdata/character_container.py`

 * *Files identical despite different names*

### Comparing `palworld_admin-0.9.8/palworld_admin/converter/lib/rawdata/connector.py` & `palworld_admin-0.9.9/palworld_admin/converter/lib/rawdata/connector.py`

 * *Files identical despite different names*

### Comparing `palworld_admin-0.9.8/palworld_admin/converter/lib/rawdata/debug.py` & `palworld_admin-0.9.9/palworld_admin/converter/lib/rawdata/debug.py`

 * *Files identical despite different names*

### Comparing `palworld_admin-0.9.8/palworld_admin/converter/lib/rawdata/dynamic_item.py` & `palworld_admin-0.9.9/palworld_admin/converter/lib/rawdata/dynamic_item.py`

 * *Files identical despite different names*

### Comparing `palworld_admin-0.9.8/palworld_admin/converter/lib/rawdata/foliage_model.py` & `palworld_admin-0.9.9/palworld_admin/converter/lib/rawdata/foliage_model.py`

 * *Files identical despite different names*

### Comparing `palworld_admin-0.9.8/palworld_admin/converter/lib/rawdata/foliage_model_instance.py` & `palworld_admin-0.9.9/palworld_admin/converter/lib/rawdata/foliage_model_instance.py`

 * *Files identical despite different names*

### Comparing `palworld_admin-0.9.8/palworld_admin/converter/lib/rawdata/group.py` & `palworld_admin-0.9.9/palworld_admin/converter/lib/rawdata/group.py`

 * *Files identical despite different names*

### Comparing `palworld_admin-0.9.8/palworld_admin/converter/lib/rawdata/item_container.py` & `palworld_admin-0.9.9/palworld_admin/converter/lib/rawdata/item_container.py`

 * *Files identical despite different names*

### Comparing `palworld_admin-0.9.8/palworld_admin/converter/lib/rawdata/item_container_slots.py` & `palworld_admin-0.9.9/palworld_admin/converter/lib/rawdata/item_container_slots.py`

 * *Files identical despite different names*

### Comparing `palworld_admin-0.9.8/palworld_admin/converter/lib/rawdata/map_concrete_model.py` & `palworld_admin-0.9.9/palworld_admin/converter/lib/rawdata/map_concrete_model.py`

 * *Files identical despite different names*

### Comparing `palworld_admin-0.9.8/palworld_admin/converter/lib/rawdata/map_model.py` & `palworld_admin-0.9.9/palworld_admin/converter/lib/rawdata/map_model.py`

 * *Files identical despite different names*

### Comparing `palworld_admin-0.9.8/palworld_admin/converter/lib/rawdata/work_collection.py` & `palworld_admin-0.9.9/palworld_admin/converter/lib/rawdata/work_collection.py`

 * *Files identical despite different names*

### Comparing `palworld_admin-0.9.8/palworld_admin/converter/lib/rawdata/worker_director.py` & `palworld_admin-0.9.9/palworld_admin/converter/lib/rawdata/worker_director.py`

 * *Files identical despite different names*

### Comparing `palworld_admin-0.9.8/palworld_admin/helper/cli.py` & `palworld_admin-0.9.9/palworld_admin/helper/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     parser = argparse.ArgumentParser(
         description="Launch the application with optional settings."
     )
     parser.add_argument(
         "-mp",
         "--management-password",
         type=str,
+        default="",
         help="""Set the management password for the Server Manager.
 Must be at least 6 characters long.""",
     )
     parser.add_argument(
         "-r",
         "--remote",
         action="store_true",
@@ -44,14 +45,31 @@
         "-mdb",
         "--migrate-database",
         default=False,
         action="store_true",
         help="Migrate the database to the latest version.",
     )
 
+    parser.add_argument(
+        "-p",
+        "--port",
+        type=int,
+        default=8210,
+        help="Set the port for the webserver to listen on.",
+        action="store",
+    )
+
+    parser.add_argument(
+        "-ls",
+        "--launch-server",
+        action="store_true",
+        default=False,
+        help="Launch the server immediately.",
+    )
+
     args = parser.parse_args()
     if args.management_password:
         result["ManagementPassword"] = args.management_password
     else:
         result["ManagementPassword"] = ""
     if args.remote:
         result["Remote"] = "remote"
@@ -63,17 +81,22 @@
         if len(args.management_password) < 6:
             raise ValueError(
                 "The management password must be at least 6 characters long."
             )
     else:
         result["Remote"] = "local"
 
+    if args.launch_server:
+        result["LaunchServer"] = True
+    else:
+        result["LaunchServer"] = False
     result["MigrateDatabase"] = args.migrate_database
     result["NoUserInterface"] = args.no_user_interface
     result["NoConsole"] = args.no_console
+    result["Port"] = args.port
     return result
 
 
 def parse_cli():
     """Parse command line arguments."""
     try:
         parsed_args = parse_arguments()
```

### Comparing `palworld_admin-0.9.8/palworld_admin/helper/consolemanagement.py` & `palworld_admin-0.9.9/palworld_admin/helper/consolemanagement.py`

 * *Files identical despite different names*

### Comparing `palworld_admin-0.9.8/palworld_admin/helper/dbmanagement.py` & `palworld_admin-0.9.9/palworld_admin/helper/dbmanagement.py`

 * *Files 2% similar despite different names*

```diff
@@ -186,15 +186,15 @@
                 }
                 new_player = Players(**player_data)
                 db.session.add(new_player)
 
     try:
         db.session.commit()
         logging.info("Committed %s players to the database.", len(players))
-    except Exception as e:
+    except Exception as e:  # pylint: disable=broad-except
         db.session.rollback()
         logging.error("Error committing players to the database: %s", str(e))
     finally:
         db.session.close()
 
 
 def get_players_from_db() -> list:
```

### Comparing `palworld_admin-0.9.8/palworld_admin/helper/dbmigration.py` & `palworld_admin-0.9.9/palworld_admin/helper/dbmigration.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,15 +10,16 @@
 
 import pkg_resources
 
 from flask import Flask
 from flask_migrate import Migrate, upgrade
 
 from palworld_admin.classes.dbmodels import db
-from palworld_admin.settings import app_settings
+
+# from palworld_admin.settings import app_settings
 
 
 def get_long_path_name(short_path):
     """
     Resolves a short path to its long form.
     """
     buffer_size = 256
@@ -34,51 +35,32 @@
     result_size = long_path_name(short_path, buffer, buffer_size)
     if result_size == 0:
         raise ctypes.WinError()
 
     return buffer[:result_size]
 
 
-def create_app():
-    """Create a Flask app with the database URI set."""
-    app = Flask(__name__)
-    # Example configuration, adjust as necessary
-    app.config["SQLALCHEMY_DATABASE_URI"] = (
-        f'sqlite:///{os.path.join(app_settings.exe_path,"palworld-admin.db")}'
-    )
-    db.init_app(app)
-    Migrate(app, db)
-    return app
-
-
-def apply_migrations():
+def apply_migrations(exe_path: str = None):
     """Apply any outstanding Alembic migrations."""
     app = Flask(__name__)
     app.secret_key = uuid.uuid4().hex
     app.config["SQLALCHEMY_DATABASE_URI"] = (
-        f'sqlite:///{os.path.join(app_settings.exe_path,"palworld-admin.db")}'
+        f'sqlite:///{os.path.join(exe_path,"palworld-admin.db")}'
     )
 
-    if not os.path.exists(
-        os.path.join(app_settings.exe_path, "palworld-admin.db")
-    ):
+    if not os.path.exists(os.path.join(exe_path, "palworld-admin.db")):
         logging.error("Database file not found.")
         sys.exit(1)
 
     db.init_app(app)
 
     migrations_directory = "migrations"  # Default migrations directory path
-    if app_settings.pyinstaller_mode:
-        migrations_directory = os.path.join(
-            app_settings.meipass, migrations_directory
-        )
-    else:
-        migrations_directory = pkg_resources.resource_filename(
-            "palworld_admin", migrations_directory
-        )
+    migrations_directory = pkg_resources.resource_filename(
+        "palworld_admin", migrations_directory
+    )
 
     # Check if any shortening of the path took place
     if "~" in migrations_directory:
         migrations_directory = get_long_path_name(migrations_directory)
 
     try:
         logging.info("Applying Database Migrations if any...")
```

### Comparing `palworld_admin-0.9.8/palworld_admin/helper/fileprocessing.py` & `palworld_admin-0.9.9/palworld_admin/helper/fileprocessing.py`

 * *Files identical despite different names*

### Comparing `palworld_admin-0.9.8/palworld_admin/helper/networking.py` & `palworld_admin-0.9.9/palworld_admin/helper/networking.py`

 * *Files identical despite different names*

### Comparing `palworld_admin-0.9.8/palworld_admin/helper/oscommands.py` & `palworld_admin-0.9.9/palworld_admin/helper/oscommands.py`

 * *Files identical despite different names*

### Comparing `palworld_admin-0.9.8/palworld_admin/icon.png` & `palworld_admin-0.9.9/palworld_admin/icon.png`

 * *Files identical despite different names*

### Comparing `palworld_admin-0.9.8/palworld_admin/migrations/alembic.ini` & `palworld_admin-0.9.9/palworld_admin/migrations/alembic.ini`

 * *Files identical despite different names*

### Comparing `palworld_admin-0.9.8/palworld_admin/migrations/env.py` & `palworld_admin-0.9.9/palworld_admin/migrations/env.py`

 * *Files identical despite different names*

### Comparing `palworld_admin-0.9.8/palworld_admin/migrations/versions/170971d44a48_removed_epicapp_palserver_added_query_.py` & `palworld_admin-0.9.9/palworld_admin/migrations/versions/170971d44a48_removed_epicapp_palserver_added_query_.py`

 * *Files identical despite different names*

### Comparing `palworld_admin-0.9.8/palworld_admin/migrations/versions/3103e5ae5314_added_publiclobby_to_launchersettings.py` & `palworld_admin-0.9.9/palworld_admin/migrations/versions/3103e5ae5314_added_publiclobby_to_launchersettings.py`

 * *Files identical despite different names*

### Comparing `palworld_admin-0.9.8/palworld_admin/migrations/versions/59a004fd30a9_added_players_table_added_steamauth_and_.py` & `palworld_admin-0.9.9/palworld_admin/migrations/versions/59a004fd30a9_added_players_table_added_steamauth_and_.py`

 * *Files identical despite different names*

### Comparing `palworld_admin-0.9.8/palworld_admin/migrations/versions/ae1eab510d76_added_auto_restart_on_unexpected_.py` & `palworld_admin-0.9.9/palworld_admin/migrations/versions/ae1eab510d76_added_auto_restart_on_unexpected_.py`

 * *Files identical despite different names*

### Comparing `palworld_admin-0.9.8/palworld_admin/migrations-backup/version 1 - ae1eab510d76/alembic.ini` & `palworld_admin-0.9.9/palworld_admin/migrations-backup/version 1 - ae1eab510d76/alembic.ini`

 * *Files identical despite different names*

### Comparing `palworld_admin-0.9.8/palworld_admin/migrations-backup/version 1 - ae1eab510d76/env.py` & `palworld_admin-0.9.9/palworld_admin/migrations-backup/version 1 - ae1eab510d76/env.py`

 * *Files identical despite different names*

### Comparing `palworld_admin-0.9.8/palworld_admin/migrations-backup/version 1 - ae1eab510d76/versions/ae1eab510d76_added_auto_restart_on_unexpected_.py` & `palworld_admin-0.9.9/palworld_admin/migrations-backup/version 1 - ae1eab510d76/versions/ae1eab510d76_added_auto_restart_on_unexpected_.py`

 * *Files identical despite different names*

### Comparing `palworld_admin-0.9.8/palworld_admin/migrations-backup/version 2 - 3103e5ae5314/alembic.ini` & `palworld_admin-0.9.9/palworld_admin/migrations-backup/version 2 - 3103e5ae5314/alembic.ini`

 * *Files identical despite different names*

### Comparing `palworld_admin-0.9.8/palworld_admin/migrations-backup/version 2 - 3103e5ae5314/env.py` & `palworld_admin-0.9.9/palworld_admin/migrations-backup/version 2 - 3103e5ae5314/env.py`

 * *Files identical despite different names*

### Comparing `palworld_admin-0.9.8/palworld_admin/migrations-backup/version 2 - 3103e5ae5314/versions/3103e5ae5314_added_publiclobby_to_launchersettings.py` & `palworld_admin-0.9.9/palworld_admin/migrations-backup/version 2 - 3103e5ae5314/versions/3103e5ae5314_added_publiclobby_to_launchersettings.py`

 * *Files identical despite different names*

### Comparing `palworld_admin-0.9.8/palworld_admin/migrations-backup/version 2 - 3103e5ae5314/versions/ae1eab510d76_added_auto_restart_on_unexpected_.py` & `palworld_admin-0.9.9/palworld_admin/migrations-backup/version 2 - 3103e5ae5314/versions/ae1eab510d76_added_auto_restart_on_unexpected_.py`

 * *Files identical despite different names*

### Comparing `palworld_admin-0.9.8/palworld_admin/rcon/__init__.py` & `palworld_admin-0.9.9/palworld_admin/rcon/__init__.py`

 * *Files identical despite different names*

### Comparing `palworld_admin-0.9.8/palworld_admin/rcon/rcon.py` & `palworld_admin-0.9.9/palworld_admin/rcon/rcon.py`

 * *Files identical despite different names*

### Comparing `palworld_admin-0.9.8/palworld_admin/servermanager/__init__.py` & `palworld_admin-0.9.9/palworld_admin/servermanager/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,14 +65,15 @@
             ) as file:
                 file_content = file.read()
             # Remove leading and trailing whitespace
             file_content = file_content.strip()
             if len(file_content) > 0:
                 result["status"] = "success"
                 result["value"] = True
+                app_settings.localserver.palserver_installed = True
             else:
                 result["status"] = "success"
                 result["value"] = False
         else:
             result["status"] = "success"
             result["value"] = False
     except Exception as e:  # pylint: disable=broad-except
@@ -161,14 +162,16 @@
         local_ip = get_local_ip()
         if not local_ip:
             result["status"] = "error"
             result["message"] = "Error getting local IP address"
         else:
             result["settings"]["LocalIP"] = local_ip
 
+        app_settings.localserver.server_settings = settings_dict
+
     except Exception as e:  # pylint: disable=broad-except
         result["status"] = "error"
         result["value"] = "Error processing settings file"
         logging.error("Error processing settings file: %s", e)
 
     return result
 
@@ -672,14 +675,15 @@
         else:
             result["status"] = "error"
             result["message"] = "Error starting server"
         logging.info(
             "Palguard installed: %s",
             app_settings.localserver.palguard_installed,
         )
+        app_settings.localserver.running = True
     except Exception as e:  # pylint: disable=broad-except
         if log:
             logging.error("Error starting server: %s", e)
         result["status"] = "error"
         result["message"] = "Error starting server"
     return result
```

### Comparing `palworld_admin-0.9.8/palworld_admin/settings.py` & `palworld_admin-0.9.9/palworld_admin/settings.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,15 +8,20 @@
 import sys
 import time
 
 from threading import Thread
 
 # from palworld_admin.helper.cli import parse_cli
 from palworld_admin.classes import PalWorldSettings, LocalServer, MemoryStorage
+from palworld_admin.helper.cli import parse_cli
+from palworld_admin.helper.consolemanagement import (
+    hide_console,
+)  # pylint: disable=wrong-import-position
 from palworld_admin.helper.oscommands import detect_virtual_machine
+from palworld_admin.helper.dbmigration import apply_migrations
 
 # from palworld_admin.ui import BrowserManager
 
 # Get the waitress logger
 logger = logging.getLogger("waitress")
 logger.setLevel(logging.ERROR)  # Only show errors and above
 
@@ -62,86 +67,98 @@
 class Settings:
     """Class to manage the settings for the server.
     This class is used to store and manage the server settings."""
 
     def __init__(self):
         self.dev: bool = False
         self.dev_ui: bool = False
-        self.no_ui: bool = False
-        self.version: str = "0.9.8"
+        self.no_ui: bool = True
+        self.version: str = "0.9.9"
         self.supporter_build: bool = False
-        self.supporter_version: str = "0.9.8"
+        self.supporter_version: str = "0.9.9"
+        self.migration_mode: bool = False
         self.alembic_version: str = "59a004fd30a9"
         self.exe_path: str = ""
         self.app_os = ""
+        self.app_port: int = 8210
         self.main_ui = None
         self.ready = False
         self.force_error = False
         self.meipass = None
         self.steam_openid_url = "https://steamcommunity.com/openid"
 
+        self.cli_launch_server: bool = False
+        self.cli_management_password: str = ""
+        self.cli_migrate_database: bool = False
+        self.cli_no_console: bool = False
+        self.cli_no_ui: bool = False
+        self.cli_port: int = 8210
+        self.cli_remote: bool = False
+
         self.palworldsettings_defaults = PalWorldSettings()
         self.localserver = LocalServer()
         self.memorystorage = MemoryStorage(
             BASE_URL,
             (
                 DEV_TEMPLATES
                 if self.dev_ui
                 else SUPPORTER_TEMPLATES if self.supporter_build else TEMPLATES
             ),
             STATIC_FILES,
         )
 
         self.pyinstaller_mode: bool = False
 
-        self.shutdown_requested = False
+        # self.shutdown_requested = False
 
-        self.current_client: str = ""
+        self.current_client: str = None
 
         self.set_logging()
-        self.set_pyinstaller_mode()
+        # self.set_pyinstaller_mode()
         self.set_app_os()
         self.detect_virtual_machine()
         self.detect_cpu_cores()
         self.set_local_server_paths()
+        self._parse_cli()
         self.check_for_palguard()
         self.download_ui()
         self.launch_ui()
         self.monitor_shutdown()
-        self.ready = True
+        self.settings_ready = True
+        self.app_ready = False
 
     def set_logging(self):
         """Set the logging configuration."""
         if self.dev:
             logging.basicConfig(
                 level=logging.DEBUG,
                 format="%(asctime)s - %(levelname)s - %(message)s",
             )
         else:
             logging.basicConfig(
                 level=logging.INFO,
                 format="%(asctime)s - %(levelname)s - %(message)s",
             )
 
-    def set_pyinstaller_mode(self):
-        """Set the pyinstaller mode based on the current environment."""
-        if getattr(sys, "frozen", False) and hasattr(sys, "_MEIPASS"):
-            self.pyinstaller_mode = True
-            self.meipass = sys._MEIPASS  # pylint: disable=protected-access
-            logging.info("MEIPASS: %s", self.meipass)
-        else:
-            self.pyinstaller_mode = False
-        logging.info("Pyinstaller mode: %s", self.pyinstaller_mode)
+    # def set_pyinstaller_mode(self):
+    #     """Set the pyinstaller mode based on the current environment."""
+    #     if getattr(sys, "frozen", False) and hasattr(sys, "_MEIPASS"):
+    #         self.pyinstaller_mode = True
+    #         self.meipass = sys._MEIPASS  # pylint: disable=protected-access
+    #         logging.info("MEIPASS: %s", self.meipass)
+    #     else:
+    #         self.pyinstaller_mode = False
+    #     logging.info("Pyinstaller mode: %s", self.pyinstaller_mode)
 
     def set_local_server_paths(self):
         """Set the paths for the local server based on the current environment."""
-        if self.pyinstaller_mode:
-            exe_path = os.path.dirname(sys.executable)
-        else:
-            exe_path = os.getcwd()
+        # if self.pyinstaller_mode:
+        #     exe_path = os.path.dirname(sys.executable)
+        # else:
+        exe_path = os.getcwd()
         self.exe_path = exe_path
         windows_or_linux = (
             "Windows"
             if self.app_os == "Windows" or self.app_os == "Wine"
             else "Linux"
         )
         # Set the launcher path and steamcmd path based on the operating system
@@ -368,14 +385,16 @@
         self.localserver.management_password = password
         logging.info(
             "Management password: %s", self.localserver.management_password
         )
 
     def download_ui(self):
         """Download the UI files if necessary."""
+        if self.migration_mode:
+            return
         if not self.dev:
             self.memorystorage.download_static_files()
             self.memorystorage.download_templates()
 
     def detect_virtual_machine(self):
         """Detect if the server is running in a virtual machine."""
         detection = detect_virtual_machine(self.app_os)
@@ -404,52 +423,95 @@
                 )
 
     def detect_cpu_cores(self):
         """Detect the number of CPU cores."""
         self.localserver.cpu_cores = multiprocessing.cpu_count()
         logging.info("CPU cores: %s", self.localserver.cpu_cores)
 
+    def _parse_cli(self):
+        """Parse CLI arguments."""
+        args = parse_cli()
+
+        self.cli_launch_server = args["LaunchServer"]
+        self.cli_port = args["Port"]
+        self.cli_no_ui = args["NoUserInterface"]
+        self.cli_no_console = args["NoConsole"]
+        self.cli_migrate_database = args["MigrateDatabase"]
+        self.cli_remote = args["Remote"]
+        self.cli_management_password = args["ManagementPassword"]
+
+        self.app_port = args["Port"]
+        self.set_management_mode(self.cli_remote)
+        self.set_management_password(self.cli_management_password)
+
+        try:
+            if self.app_os != "Windows" and self.cli_remote != "remote":
+                raise ValueError(
+                    "\nNon-Windows operating system requires -r and -mp flags. See -h\n"
+                )
+        except ValueError as e:
+            print(f"Error: {e}")
+            sys.exit(1)
+
+        if self.cli_migrate_database:
+            self.migration_mode = True
+            apply_migrations(self.exe_path)
+            sys.exit(0)
+
+        if self.cli_no_console:
+            hide_console()
+
     def launch_ui(self):
         """Launch the main UI."""
         # If the app is being built for pip, then don't launch the UI
-        if self.no_ui:
+        if self.migration_mode or self.cli_no_ui or self.no_ui:
             return
         if self.app_os == "Windows":
             try:
-                if self.pyinstaller_mode:
-                    ui_path = os.path.join(
-                        self.meipass,
-                        "ui",
-                        "palworld-admin-ui.exe",
-                    )
-                else:
-                    ui_path = os.path.join(
-                        self.exe_path,
-                        "ui",
-                        "palworld-admin-ui-win32-x64",
-                        "palworld-admin-ui.exe",
-                    )
+                # if self.pyinstaller_mode:
+                #     ui_path = os.path.join(
+                #         self.meipass,
+                #         "ui",
+                #         "palworld-admin-ui.exe",
+                #     )
+                # else:
+                ui_path = os.path.join(
+                    self.exe_path,
+                    "ui",
+                    "palworld-admin-ui-win32-x64",
+                    "palworld-admin-ui.exe",
+                )
 
                 if not os.path.exists(ui_path):
                     logging.info("UI not found, skipping launch.")
                 else:
                     logging.info("Launching UI: %s", ui_path)
-                    self.main_ui = subprocess.Popen(ui_path)
+                    self.main_ui = subprocess.Popen(
+                        [ui_path, f"--port={str(self.app_port)}"]
+                    )
                     logging.info("Launched UI.")
             except Exception as e:  # pylint: disable=broad-except
                 logging.error("Failed to launch UI: %s", e)
                 sys.exit(1)
         else:  # Linux
             pass  # No UI for Linux
 
     def monitor_shutdown(self):
         """Monitor the shutdown status of the UI."""
+        if self.main_ui is None:
+            return
 
         def monitor():
-            while not self.shutdown_requested:
+            # while not self.shutdown_requested:
+            #     time.sleep(1)
+            # Check if the UI is still running using poll
+            while True:
+                if self.main_ui.poll() is not None:
+                    logging.info("UI has closed.")
+                    break
                 time.sleep(1)
             logging.info("Shutdown requested, waiting 1 second.")
             time.sleep(1)  # Wait for the UI to close
             # Get PID of own process
             pid = os.getpid()
             logging.info("Terminating own Process with Pid: %s", pid)
             if app_settings.app_os == "Windows":
```

### Comparing `palworld_admin-0.9.8/palworld_admin/website/__init__.py` & `palworld_admin-0.9.9/palworld_admin/website/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 import logging
 from mimetypes import guess_type
 import os
 import uuid
 import shutil
 
 # Must be included for pyinstaller to work
-from engineio.async_drivers import eventlet  # pylint: disable=unused-import
-import eventlet  # pylint: disable=unused-import disable=reimported
+# from engineio.async_drivers import eventlet  # pylint: disable=unused-import
+# import eventlet  # pylint: disable=unused-import disable=reimported
 
 from flask_socketio import SocketIO
 
 from flask import (
     Flask,
     Response,
     abort,
@@ -220,14 +220,21 @@
     with app.app_context():
         db.create_all()
         initialize_database_defaults()
         app_settings.localserver.all_players = get_players_from_db()
         app_settings.localserver.launcher_args = get_stored_default_settings(
             "LauncherSettings"
         )
+        app_settings.localserver.rcon_last_connection_args = (
+            get_stored_default_settings("Connection")
+        )
+        logging.info(
+            "Last RCON Connection: %s",
+            app_settings.localserver.rcon_last_connection_args,
+        )
         alembic_version = get_alembic_version()
 
     if alembic_version:
         logging.info("Alembic DB Version: %s", alembic_version)
 
     @app.route("/restore-server-data", methods=["POST"])
     @maybe_requires_auth
@@ -366,20 +373,20 @@
             logging.info("Querying the database. Data: %s", request.json)
         data = request.json
         if data["function"] == "get_default_settings":
             result = get_stored_default_settings(data["data"]["model"])
         return jsonify(result)
 
     # Route for shutting down the server
-    @app.route("/shutdown", methods=["POST"])
-    def shutdown():
-        logging.info("Shutting down the server...")
-        app_settings.shutdown_requested = True
+    # @app.route("/shutdown", methods=["POST"])
+    # def shutdown():
+    #     logging.info("Shutting down the server...")
+    #     app_settings.shutdown_requested = True
 
-        return "Server shutting down..."
+    #     return "Server shutting down..."
 
     if app_settings.localserver.management_mode == "remote":
 
         @app.route("/login", methods=["GET", "POST"])
         def login():
             """Render the login page."""
             management_mode = session.get("management_mode", None)
@@ -414,17 +421,17 @@
         return redirect(
             url_for("custom_static", filename="images/favicon.ico")
         )
 
     # Route for serving the resources directory
     @app.route("/resources/<path:filename>")
     def custom_static(filename):
-        if app_settings.pyinstaller_mode:
-            directory = os.path.join(app_settings.meipass, "resources")
-            return send_from_directory(directory, filename)
+        # if app_settings.pyinstaller_mode:
+        #     directory = os.path.join(app_settings.meipass, "resources")
+        #     return send_from_directory(directory, filename)
         return send_from_directory("resources", filename)
 
     @app.route("/generate_sav", methods=["POST"])
     def generate_sav():
         """Generate WorldOption.sav and return it as a file download."""
         # Generate WorldOption.sav.json and convert it to WorldOption.sav
         properties_data = {
@@ -737,15 +744,15 @@
             }
 
             if "palguard_commands" in message:
                 reply["vars"]["palguardCommands"] = message[
                     "palguard_commands"
                 ]
 
-            logging.info("Reply: %s", reply)
+            # logging.info("Reply: %s", reply)
             return reply
 
         return process_frontend_command(func, data)
 
     @socketio.on("disconnect_rcon", namespace="/socket")
     def disconnect_rcon():
         def func():
@@ -944,15 +951,15 @@
             func, frontend_event="install_server", indicator="IO"
         )
 
     @socketio.on("launch_server", namespace="/socket")
     def start_server_socket(data):
         def func(data):
             result = run_server(launcher_args=data)
-            # logging.info("Launch Server Result: %s", result)
+            logging.info("Launch Server Result: %s", result)
 
             message = result["message"]
             reply = {
                 "command": "launch server",
                 "success": result["status"] == "success",
                 "outputMessage": message,
                 "toastMessage": message,
@@ -996,17 +1003,39 @@
     @socketio.on("check_server_running", namespace="/socket")
     def check_server_running_socket():
         def func():
             reply = {}
             result = check_server_running()
             # logging.info("Result: %s", result)
 
+            launcher_args = app_settings.localserver.launcher_args
+
             if result["value"] is False:
                 app_settings.localserver.running = False
 
+            # If the server is not running and it's expected to be running,
+            # And no client is connected to backend, restart the server
+            if (
+                not app_settings.localserver.running
+                and app_settings.localserver.expected_to_be_running
+                and app_settings.localserver.launcher_args[
+                    "auto_restart_on_unexpected_shutdown"
+                ]
+                and app_settings.localserver.launcher_args[
+                    "auto_restart_triggers"
+                ]
+                and app_settings.current_client is None
+            ):
+                logging.info(
+                    "Server stopped, and there's no client to restart it. Restarting Server..."
+                )
+                with app.app_context():
+                    run_server(launcher_args=launcher_args)
+                return
+
             # If this is the first check, set the expected_to_be_running variable
             if (
                 app_settings.localserver.running_check_count == 0
                 and result["status"] == "success"
                 and result["value"] is True
             ):
                 logging.info(
@@ -1026,14 +1055,16 @@
                 reply["outputMessage"] = (
                     "Server Running on Startup, Starting Monitoring..."
                 )
 
             reply["command"] = "check server running"
             reply["success"] = result["status"] == "success"
             reply["vars"] = {
+                "launcherArgs": app_settings.localserver.launcher_args,
+                "expectedToBeRunning": app_settings.localserver.expected_to_be_running,
                 "serverRunning": result["value"],
                 "runningCheckCount": app_settings.localserver.running_check_count,
                 "cpuUsage": result["cpu_usage"],
                 "ramUsage": result["ram_usage"],
             }
 
             app_settings.localserver.last_cpu_usage = result["cpu_usage"]
@@ -1429,18 +1460,43 @@
                         )
 
             timer += 0.5
             # logging.info("Server Monitor Timer: %s", timer)
             # Use socketio.sleep for proper thread management
             socketio.sleep(0.5)
 
+    check_install()
+    # Start the server from the CLI if the settings are set
+    if (
+        app_settings.cli_launch_server
+        and app_settings.localserver.palserver_installed
+        and app_settings.localserver.launcher_args is not {}
+        and app_settings.localserver.rcon_last_connection_args is not {}
+    ):
+
+        def task__launch_server_from_cli():
+            """Launch the server from the CLI."""
+            socketio.sleep(5)
+            with app.app_context():
+                launcher_args = app_settings.localserver.launcher_args
+                launcher_args["rcon_port"] = (
+                    app_settings.localserver.rcon_last_connection_args["port"]
+                )
+                launcher_args["public_port"] = (
+                    app_settings.localserver.server_settings["PublicPort"]
+                )
+
+                run_server(launcher_args=launcher_args)
+                app_settings.localserver.running = True
+                app_settings.localserver.expected_to_be_running = True
+
+        # Start the server from the CLI
+        socketio.start_background_task(task__launch_server_from_cli)
+
     # Start the server monitor in the background
     socketio.start_background_task(server_minitor_task)
 
     # Set socketIO to use the Flask app
-
-    if app_settings.dev:
-        socketio.run(app, host="0.0.0.0", port=8210, debug=False)
-    else:
-        socketio.run(app, host="0.0.0.0", port=8210, debug=False)
+    logging.info("Launching application on port %s", app_settings.app_port)
+    socketio.run(app, host="0.0.0.0", port=app_settings.app_port, debug=False)
 
     return app
```

### Comparing `palworld_admin-0.9.8/palworld_admin/website/resources/css/bootstrap.min.css` & `palworld_admin-0.9.9/palworld_admin/website/resources/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `palworld_admin-0.9.8/palworld_admin/website/resources/font/bootstrap-icons.css` & `palworld_admin-0.9.9/palworld_admin/website/resources/font/bootstrap-icons.css`

 * *Files identical despite different names*

### Comparing `palworld_admin-0.9.8/palworld_admin/website/resources/font/fonts/bootstrap-icons.woff` & `palworld_admin-0.9.9/palworld_admin/website/resources/font/fonts/bootstrap-icons.woff`

 * *Files identical despite different names*

### Comparing `palworld_admin-0.9.8/palworld_admin/website/resources/font/fonts/bootstrap-icons.woff2` & `palworld_admin-0.9.9/palworld_admin/website/resources/font/fonts/bootstrap-icons.woff2`

 * *Files identical despite different names*

### Comparing `palworld_admin-0.9.8/palworld_admin/website/resources/images/favicon.ico` & `palworld_admin-0.9.9/palworld_admin/website/resources/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `palworld_admin-0.9.8/palworld_admin/website/resources/images/palworld-logo.png` & `palworld_admin-0.9.9/palworld_admin/website/resources/images/palworld-logo.png`

 * *Files identical despite different names*

### Comparing `palworld_admin-0.9.8/palworld_admin/website/resources/js/bootstrap.min.js` & `palworld_admin-0.9.9/palworld_admin/website/resources/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `palworld_admin-0.9.8/palworld_admin/website/resources/js/jquery-3.7.1.min.js` & `palworld_admin-0.9.9/palworld_admin/website/resources/js/jquery-3.7.1.min.js`

 * *Files identical despite different names*

### Comparing `palworld_admin-0.9.8/palworld_admin/website/resources/js/socket.io.min.js` & `palworld_admin-0.9.9/palworld_admin/website/resources/js/socket.io.min.js`

 * *Files identical despite different names*

### Comparing `palworld_admin-0.9.8/palworld_admin/website/views.py` & `palworld_admin-0.9.9/palworld_admin/website/views.py`

 * *Files identical despite different names*

### Comparing `palworld_admin-0.9.8/README.md` & `palworld_admin-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `palworld_admin-0.9.8/ui/assets/icon.ico` & `palworld_admin-0.9.9/ui/assets/icon.ico`

 * *Files identical despite different names*

### Comparing `palworld_admin-0.9.8/ui/main.js` & `palworld_admin-0.9.9/ui/main.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -80,15 +80,18 @@
         title: 'Palworld ADMIN',
         backgroundColor: "#212529",
         show: false,
     });
 
     mainWindow.setMenu(null);
 
-    mainWindow.loadURL('http://localhost:8210');
+    const portArgIndex = process.argv.findIndex(arg => arg.startsWith('--port='));
+    const port = portArgIndex !== -1 ? process.argv[portArgIndex].split('=')[1] : 8210;
+
+    mainWindow.loadURL(`http://localhost:${port}`);
 
     mainWindow.once('ready-to-show', () => {
         mainWindow.show();
     });
 
     mainWindow.webContents.on('did-finish-load', () => {
         checkZoom();
@@ -173,23 +176,23 @@
     if (process.platform !== 'darwin') {
         app.quit();
     }
 });
 
 app.on('before-quit', () => {
     // Post to /shutdown to shutdown the server
-    const http = require('http');
-    const options = {
-        hostname: '127.0.0.1',
-        port: 8210,
-        path: '/shutdown',
-        method: 'POST',
-    };
-    const req = http.request(options, (res) => {
-        console.log(`statusCode: ${res.statusCode}`);
-    });
-    req.on('error', (error) => {
-        console.error(error);
-    });
-    req.end();
+    // const http = require('http');
+    // const options = {
+    //     hostname: '127.0.0.1',
+    //     port: 8210,
+    //     path: '/shutdown',
+    //     method: 'POST',
+    // };
+    // const req = http.request(options, (res) => {
+    //     console.log(`statusCode: ${res.statusCode}`);
+    // });
+    // req.on('error', (error) => {
+    //     console.error(error);
+    // });
+    // req.end();    
     app.isQuitting = true;
 });
```

### Comparing `palworld_admin-0.9.8/ui/package-lock.json` & `palworld_admin-0.9.9/ui/package-lock.json`

 * *Files identical despite different names*

### Comparing `palworld_admin-0.9.8/PKG-INFO` & `palworld_admin-0.9.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: palworld_admin
-Version: 0.9.8
+Version: 0.9.9
 Summary: Palworld Admin is a GUI to manage your Palworld Dedicated Server, including deployment, configuration, monitoring and backups.
 License: Expressed Permission Only
 Author: Lukium
 Author-email: mrlukium@outlook.com
 Requires-Python: >=3.11,<3.13
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

