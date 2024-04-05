# Comparing `tmp/gen3_tracker-0.0.2rc8.tar.gz` & `tmp/gen3_tracker-0.0.2rc9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gen3_tracker-0.0.2rc8.tar", last modified: Thu Feb 22 21:01:53 2024, max compression
+gzip compressed data, was "gen3_tracker-0.0.2rc9.tar", last modified: Mon Mar  4 21:47:03 2024, max compression
```

## Comparing `gen3_tracker-0.0.2rc8.tar` & `gen3_tracker-0.0.2rc9.tar`

### file list

```diff
@@ -1,118 +1,120 @@
-drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2024-02-22 21:01:53.927065 gen3_tracker-0.0.2rc8/
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     1065 2023-05-04 14:32:05.000000 gen3_tracker-0.0.2rc8/LICENSE
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     2415 2024-02-22 21:01:53.926651 gen3_tracker-0.0.2rc8/PKG-INFO
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     1338 2024-02-22 21:00:10.000000 gen3_tracker-0.0.2rc8/README.md
-drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2024-02-22 21:01:53.925976 gen3_tracker-0.0.2rc8/gen3_tracker.egg-info/
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     2415 2024-02-22 21:01:53.000000 gen3_tracker-0.0.2rc8/gen3_tracker.egg-info/PKG-INFO
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     2827 2024-02-22 21:01:53.000000 gen3_tracker-0.0.2rc8/gen3_tracker.egg-info/SOURCES.txt
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        1 2024-02-22 21:01:53.000000 gen3_tracker-0.0.2rc8/gen3_tracker.egg-info/dependency_links.txt
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)       47 2024-02-22 21:01:53.000000 gen3_tracker-0.0.2rc8/gen3_tracker.egg-info/entry_points.txt
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      186 2024-02-22 21:01:53.000000 gen3_tracker-0.0.2rc8/gen3_tracker.egg-info/requires.txt
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)       16 2024-02-22 21:01:53.000000 gen3_tracker-0.0.2rc8/gen3_tracker.egg-info/top_level.txt
-drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2024-02-22 21:01:53.882720 gen3_tracker-0.0.2rc8/gen3_util/
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     2885 2024-02-22 21:00:10.000000 gen3_tracker-0.0.2rc8/gen3_util/__init__.py
-drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2024-02-22 21:01:53.884830 gen3_tracker-0.0.2rc8/gen3_util/access/
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     3307 2024-02-02 18:31:41.000000 gen3_tracker-0.0.2rc8/gen3_util/access/__init__.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     4512 2024-02-02 18:31:41.000000 gen3_tracker-0.0.2rc8/gen3_util/access/cli.py
-drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2024-02-22 21:01:53.888392 gen3_tracker-0.0.2rc8/gen3_util/access/policies/
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-07-07 00:00:20.000000 gen3_tracker-0.0.2rc8/gen3_util/access/policies/__init__.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      270 2024-02-22 21:00:17.000000 gen3_tracker-0.0.2rc8/gen3_util/access/policies/add-project-default.yaml
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)       77 2024-02-22 21:00:17.000000 gen3_tracker-0.0.2rc8/gen3_util/access/policies/add-user-delete.yaml
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)       76 2023-11-21 01:09:36.000000 gen3_tracker-0.0.2rc8/gen3_util/access/policies/add-user-read.yaml
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      199 2024-02-22 21:00:17.000000 gen3_tracker-0.0.2rc8/gen3_util/access/policies/add-user-write.yaml
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     6744 2024-02-22 21:00:17.000000 gen3_tracker-0.0.2rc8/gen3_util/access/requestor.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     1052 2024-02-02 18:31:41.000000 gen3_tracker-0.0.2rc8/gen3_util/access/submitter.py
-drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2024-02-22 21:01:53.895145 gen3_tracker-0.0.2rc8/gen3_util/buckets/
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     1211 2024-02-02 18:31:41.000000 gen3_tracker-0.0.2rc8/gen3_util/buckets/__init__.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      883 2024-02-02 18:31:41.000000 gen3_tracker-0.0.2rc8/gen3_util/buckets/cli.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      559 2024-02-02 18:31:41.000000 gen3_tracker-0.0.2rc8/gen3_util/buckets/lister.py
-drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2024-02-22 21:01:53.895530 gen3_tracker-0.0.2rc8/gen3_util/common/
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)    12145 2024-02-09 14:41:44.000000 gen3_tracker-0.0.2rc8/gen3_util/common/__init__.py
-drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2024-02-22 21:01:53.896314 gen3_tracker-0.0.2rc8/gen3_util/config/
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     9586 2024-02-02 18:31:41.000000 gen3_tracker-0.0.2rc8/gen3_util/config/__init__.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      876 2024-02-02 18:31:41.000000 gen3_tracker-0.0.2rc8/gen3_util/config/cli.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      137 2024-02-02 18:31:41.000000 gen3_tracker-0.0.2rc8/gen3_util/config.yaml
-drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2024-02-22 21:01:53.905049 gen3_tracker-0.0.2rc8/gen3_util/files/
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     1457 2023-12-27 05:18:50.000000 gen3_tracker-0.0.2rc8/gen3_util/files/__init__.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)    10733 2024-02-02 18:31:41.000000 gen3_tracker-0.0.2rc8/gen3_util/files/cli.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     3751 2024-02-02 18:53:09.000000 gen3_tracker-0.0.2rc8/gen3_util/files/lister.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)    12564 2024-02-02 18:31:41.000000 gen3_tracker-0.0.2rc8/gen3_util/files/manifest.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     1503 2024-02-02 18:31:41.000000 gen3_tracker-0.0.2rc8/gen3_util/files/middleware.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      634 2024-02-02 18:31:41.000000 gen3_tracker-0.0.2rc8/gen3_util/files/remover.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     5194 2023-12-27 05:18:50.000000 gen3_tracker-0.0.2rc8/gen3_util/files/uploader.py
-drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2024-02-22 21:01:53.909989 gen3_tracker-0.0.2rc8/gen3_util/jobs/
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-10-19 18:01:08.000000 gen3_tracker-0.0.2rc8/gen3_util/jobs/__init__.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     2618 2024-02-02 18:31:41.000000 gen3_tracker-0.0.2rc8/gen3_util/jobs/cli.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      559 2024-02-02 18:31:41.000000 gen3_tracker-0.0.2rc8/gen3_util/jobs/lister.py
-drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2024-02-22 21:01:53.913610 gen3_tracker-0.0.2rc8/gen3_util/meta/
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     4438 2024-02-22 21:00:10.000000 gen3_tracker-0.0.2rc8/gen3_util/meta/__init__.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     1415 2024-02-09 14:41:44.000000 gen3_tracker-0.0.2rc8/gen3_util/meta/bundler.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     8981 2024-02-02 18:31:41.000000 gen3_tracker-0.0.2rc8/gen3_util/meta/cli.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      687 2024-02-02 18:31:41.000000 gen3_tracker-0.0.2rc8/gen3_util/meta/delta.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     2894 2024-02-02 18:31:41.000000 gen3_tracker-0.0.2rc8/gen3_util/meta/differ.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      326 2023-10-19 18:01:08.000000 gen3_tracker-0.0.2rc8/gen3_util/meta/downloader.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     2204 2024-02-02 18:31:41.000000 gen3_tracker-0.0.2rc8/gen3_util/meta/importer.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     1655 2024-02-02 18:31:41.000000 gen3_tracker-0.0.2rc8/gen3_util/meta/lister.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     2932 2024-02-09 14:31:03.000000 gen3_tracker-0.0.2rc8/gen3_util/meta/publisher.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)    15494 2024-02-22 21:00:17.000000 gen3_tracker-0.0.2rc8/gen3_util/meta/skeleton.py
-drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2024-02-22 21:01:53.913823 gen3_tracker-0.0.2rc8/gen3_util/meta/tabular/
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)    11706 2024-02-22 21:00:10.000000 gen3_tracker-0.0.2rc8/gen3_util/meta/tabular/__init__.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     4660 2024-02-02 18:31:41.000000 gen3_tracker-0.0.2rc8/gen3_util/meta/uploader.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     4477 2024-02-09 14:41:44.000000 gen3_tracker-0.0.2rc8/gen3_util/meta/validator.py
-drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2024-02-22 21:01:53.914618 gen3_tracker-0.0.2rc8/gen3_util/projects/
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     2778 2024-02-02 18:31:41.000000 gen3_tracker-0.0.2rc8/gen3_util/projects/__init__.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     3696 2024-02-09 14:31:03.000000 gen3_tracker-0.0.2rc8/gen3_util/projects/cli.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     2341 2024-02-02 18:31:41.000000 gen3_tracker-0.0.2rc8/gen3_util/projects/lister.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     1496 2024-02-09 14:31:03.000000 gen3_tracker-0.0.2rc8/gen3_util/projects/remover.py
-drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2024-02-22 21:01:53.916562 gen3_tracker-0.0.2rc8/gen3_util/repo/
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     4557 2024-02-02 18:31:41.000000 gen3_tracker-0.0.2rc8/gen3_util/repo/__init__.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)    17203 2024-02-22 21:00:17.000000 gen3_tracker-0.0.2rc8/gen3_util/repo/cli.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     3726 2024-02-02 18:31:41.000000 gen3_tracker-0.0.2rc8/gen3_util/repo/cloner.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     9643 2024-02-22 21:00:17.000000 gen3_tracker-0.0.2rc8/gen3_util/repo/committer.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2024-02-02 18:31:41.000000 gen3_tracker-0.0.2rc8/gen3_util/repo/history.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     1512 2024-02-02 18:31:41.000000 gen3_tracker-0.0.2rc8/gen3_util/repo/initializer.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     1699 2024-02-02 18:31:41.000000 gen3_tracker-0.0.2rc8/gen3_util/repo/puller.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     4405 2024-02-22 21:00:17.000000 gen3_tracker-0.0.2rc8/gen3_util/repo/pusher.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     2959 2024-02-02 18:31:41.000000 gen3_tracker-0.0.2rc8/gen3_util/repo/status.py
-drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2024-02-22 21:01:53.916910 gen3_tracker-0.0.2rc8/gen3_util/users/
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-10-19 18:09:26.000000 gen3_tracker-0.0.2rc8/gen3_util/users/__init__.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     1694 2024-02-22 21:00:17.000000 gen3_tracker-0.0.2rc8/gen3_util/users/cli.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)       38 2024-02-22 21:01:53.927132 gen3_tracker-0.0.2rc8/setup.cfg
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     5581 2024-02-22 21:01:01.000000 gen3_tracker-0.0.2rc8/setup.py
-drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2024-02-22 21:01:53.858242 gen3_tracker-0.0.2rc8/tests/
-drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2024-02-22 21:01:53.919033 gen3_tracker-0.0.2rc8/tests/integration/
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-05-05 20:31:25.000000 gen3_tracker-0.0.2rc8/tests/integration/__init__.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     1091 2024-02-02 18:31:41.000000 gen3_tracker-0.0.2rc8/tests/integration/conftest.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     1066 2024-02-02 18:31:41.000000 gen3_tracker-0.0.2rc8/tests/integration/test_access.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      454 2024-02-02 18:31:41.000000 gen3_tracker-0.0.2rc8/tests/integration/test_buckets.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     7641 2024-02-22 21:00:17.000000 gen3_tracker-0.0.2rc8/tests/integration/test_commit.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      257 2024-02-02 18:31:41.000000 gen3_tracker-0.0.2rc8/tests/integration/test_config.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     1987 2024-02-02 18:31:41.000000 gen3_tracker-0.0.2rc8/tests/integration/test_init.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     9506 2024-02-02 18:31:41.000000 gen3_tracker-0.0.2rc8/tests/integration/test_meta.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     8848 2024-02-02 18:31:42.000000 gen3_tracker-0.0.2rc8/tests/integration/test_meta_skeleton.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     1321 2024-02-09 14:41:44.000000 gen3_tracker-0.0.2rc8/tests/integration/test_project.py
-drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2024-02-22 21:01:53.922742 gen3_tracker-0.0.2rc8/tests/unit/
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-05-05 20:31:25.000000 gen3_tracker-0.0.2rc8/tests/unit/__init__.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      464 2023-12-27 05:18:50.000000 gen3_tracker-0.0.2rc8/tests/unit/conftest.py
-drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2024-02-22 21:01:53.923054 gen3_tracker-0.0.2rc8/tests/unit/plugins/
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-07-07 00:45:48.000000 gen3_tracker-0.0.2rc8/tests/unit/plugins/__init__.py
-drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2024-02-22 21:01:53.923313 gen3_tracker-0.0.2rc8/tests/unit/plugins/gen3_util_plugin_foo/
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     1450 2023-07-07 00:45:48.000000 gen3_tracker-0.0.2rc8/tests/unit/plugins/gen3_util_plugin_foo/__init__.py
-drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2024-02-22 21:01:53.925588 gen3_tracker-0.0.2rc8/tests/unit/tabular/
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2024-01-05 01:09:09.000000 gen3_tracker-0.0.2rc8/tests/unit/tabular/__init__.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)    16696 2024-02-22 21:00:10.000000 gen3_tracker-0.0.2rc8/tests/unit/tabular/conftest.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     1172 2024-01-05 01:09:09.000000 gen3_tracker-0.0.2rc8/tests/unit/tabular/test_config.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     7826 2024-02-22 21:00:10.000000 gen3_tracker-0.0.2rc8/tests/unit/tabular/test_default_columns.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     1035 2024-02-02 18:31:42.000000 gen3_tracker-0.0.2rc8/tests/unit/tabular/test_dir_to_tabular.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     1888 2024-01-05 01:09:09.000000 gen3_tracker-0.0.2rc8/tests/unit/tabular/test_from_tabular.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     3779 2024-02-22 21:00:10.000000 gen3_tracker-0.0.2rc8/tests/unit/tabular/test_to_tabular.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      737 2024-01-05 01:09:09.000000 gen3_tracker-0.0.2rc8/tests/unit/tabular/test_validate.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     3429 2024-02-02 18:31:42.000000 gen3_tracker-0.0.2rc8/tests/unit/test_cli.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     4881 2024-02-02 18:31:42.000000 gen3_tracker-0.0.2rc8/tests/unit/test_coding.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      565 2023-05-05 20:31:25.000000 gen3_tracker-0.0.2rc8/tests/unit/test_coding_conventions.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      532 2023-12-21 15:16:16.000000 gen3_tracker-0.0.2rc8/tests/unit/test_config.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     1417 2023-12-27 05:18:50.000000 gen3_tracker-0.0.2rc8/tests/unit/test_files.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      445 2024-02-09 14:41:44.000000 gen3_tracker-0.0.2rc8/tests/unit/test_job_dependencies.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      734 2023-12-27 05:18:50.000000 gen3_tracker-0.0.2rc8/tests/unit/test_manifest.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     1546 2024-02-02 18:31:42.000000 gen3_tracker-0.0.2rc8/tests/unit/test_validate_directory.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      625 2024-02-02 18:31:42.000000 gen3_tracker-0.0.2rc8/tests/unit/test_version.py
+drwxr-xr-x   0 peterkor (1520582618) 1971611142        0 2024-03-04 21:47:03.211959 gen3_tracker-0.0.2rc9/
+-rw-r--r--   0 peterkor (1520582618) 1971611142     1065 2024-02-13 19:02:15.000000 gen3_tracker-0.0.2rc9/LICENSE
+-rw-r--r--   0 peterkor (1520582618) 1971611142     2026 2024-03-04 21:47:03.211706 gen3_tracker-0.0.2rc9/PKG-INFO
+-rw-r--r--   0 peterkor (1520582618) 1971611142     1338 2024-02-28 16:48:14.000000 gen3_tracker-0.0.2rc9/README.md
+drwxr-xr-x   0 peterkor (1520582618) 1971611142        0 2024-03-04 21:47:03.038522 gen3_tracker-0.0.2rc9/gen3_tracker.egg-info/
+-rw-r--r--   0 peterkor (1520582618) 1971611142     2026 2024-03-04 21:47:02.000000 gen3_tracker-0.0.2rc9/gen3_tracker.egg-info/PKG-INFO
+-rw-r--r--   0 peterkor (1520582618) 1971611142     2904 2024-03-04 21:47:02.000000 gen3_tracker-0.0.2rc9/gen3_tracker.egg-info/SOURCES.txt
+-rw-r--r--   0 peterkor (1520582618) 1971611142        1 2024-03-04 21:47:02.000000 gen3_tracker-0.0.2rc9/gen3_tracker.egg-info/dependency_links.txt
+-rw-r--r--   0 peterkor (1520582618) 1971611142       48 2024-03-04 21:47:02.000000 gen3_tracker-0.0.2rc9/gen3_tracker.egg-info/entry_points.txt
+-rw-r--r--   0 peterkor (1520582618) 1971611142      186 2024-03-04 21:47:02.000000 gen3_tracker-0.0.2rc9/gen3_tracker.egg-info/requires.txt
+-rw-r--r--   0 peterkor (1520582618) 1971611142       16 2024-03-04 21:47:02.000000 gen3_tracker-0.0.2rc9/gen3_tracker.egg-info/top_level.txt
+drwxr-xr-x   0 peterkor (1520582618) 1971611142        0 2024-03-04 21:47:03.041546 gen3_tracker-0.0.2rc9/gen3_util/
+-rw-r--r--   0 peterkor (1520582618) 1971611142     2885 2024-02-28 16:48:14.000000 gen3_tracker-0.0.2rc9/gen3_util/__init__.py
+drwxr-xr-x   0 peterkor (1520582618) 1971611142        0 2024-03-04 21:47:03.048134 gen3_tracker-0.0.2rc9/gen3_util/access/
+-rw-r--r--   0 peterkor (1520582618) 1971611142     3307 2024-03-04 21:44:58.000000 gen3_tracker-0.0.2rc9/gen3_util/access/__init__.py
+-rw-r--r--   0 peterkor (1520582618) 1971611142     4512 2024-03-04 21:44:58.000000 gen3_tracker-0.0.2rc9/gen3_util/access/cli.py
+drwxr-xr-x   0 peterkor (1520582618) 1971611142        0 2024-03-04 21:47:03.050745 gen3_tracker-0.0.2rc9/gen3_util/access/policies/
+-rw-r--r--   0 peterkor (1520582618) 1971611142        0 2024-02-28 16:48:14.000000 gen3_tracker-0.0.2rc9/gen3_util/access/policies/__init__.py
+-rw-r--r--   0 peterkor (1520582618) 1971611142      189 2024-03-04 21:44:58.000000 gen3_tracker-0.0.2rc9/gen3_util/access/policies/add-project-default.yaml
+-rw-r--r--   0 peterkor (1520582618) 1971611142       77 2024-02-28 16:48:14.000000 gen3_tracker-0.0.2rc9/gen3_util/access/policies/add-user-delete.yaml
+-rw-r--r--   0 peterkor (1520582618) 1971611142       76 2024-02-28 16:48:14.000000 gen3_tracker-0.0.2rc9/gen3_util/access/policies/add-user-read.yaml
+-rw-r--r--   0 peterkor (1520582618) 1971611142      199 2024-02-28 16:48:14.000000 gen3_tracker-0.0.2rc9/gen3_util/access/policies/add-user-write.yaml
+-rw-r--r--   0 peterkor (1520582618) 1971611142     6744 2024-03-04 21:44:58.000000 gen3_tracker-0.0.2rc9/gen3_util/access/requestor.py
+-rw-r--r--   0 peterkor (1520582618) 1971611142     1052 2024-02-28 16:48:14.000000 gen3_tracker-0.0.2rc9/gen3_util/access/submitter.py
+drwxr-xr-x   0 peterkor (1520582618) 1971611142        0 2024-03-04 21:47:03.052103 gen3_tracker-0.0.2rc9/gen3_util/buckets/
+-rw-r--r--   0 peterkor (1520582618) 1971611142     1211 2024-02-28 16:48:14.000000 gen3_tracker-0.0.2rc9/gen3_util/buckets/__init__.py
+-rw-r--r--   0 peterkor (1520582618) 1971611142      883 2024-03-04 21:44:58.000000 gen3_tracker-0.0.2rc9/gen3_util/buckets/cli.py
+-rw-r--r--   0 peterkor (1520582618) 1971611142      559 2024-02-28 16:48:14.000000 gen3_tracker-0.0.2rc9/gen3_util/buckets/lister.py
+drwxr-xr-x   0 peterkor (1520582618) 1971611142        0 2024-03-04 21:47:03.060336 gen3_tracker-0.0.2rc9/gen3_util/common/
+-rw-r--r--   0 peterkor (1520582618) 1971611142    12644 2024-03-04 21:44:58.000000 gen3_tracker-0.0.2rc9/gen3_util/common/__init__.py
+drwxr-xr-x   0 peterkor (1520582618) 1971611142        0 2024-03-04 21:47:03.062342 gen3_tracker-0.0.2rc9/gen3_util/config/
+-rw-r--r--   0 peterkor (1520582618) 1971611142     9586 2024-03-04 21:44:58.000000 gen3_tracker-0.0.2rc9/gen3_util/config/__init__.py
+-rw-r--r--   0 peterkor (1520582618) 1971611142      876 2024-02-28 16:48:14.000000 gen3_tracker-0.0.2rc9/gen3_util/config/cli.py
+-rw-r--r--   0 peterkor (1520582618) 1971611142      137 2024-02-28 16:48:14.000000 gen3_tracker-0.0.2rc9/gen3_util/config.yaml
+drwxr-xr-x   0 peterkor (1520582618) 1971611142        0 2024-03-04 21:47:03.087962 gen3_tracker-0.0.2rc9/gen3_util/files/
+-rw-r--r--   0 peterkor (1520582618) 1971611142     1457 2024-02-28 16:48:14.000000 gen3_tracker-0.0.2rc9/gen3_util/files/__init__.py
+-rw-r--r--   0 peterkor (1520582618) 1971611142    12116 2024-03-04 21:45:26.000000 gen3_tracker-0.0.2rc9/gen3_util/files/cli.py
+-rw-r--r--   0 peterkor (1520582618) 1971611142     3751 2024-02-28 16:48:14.000000 gen3_tracker-0.0.2rc9/gen3_util/files/lister.py
+-rw-r--r--   0 peterkor (1520582618) 1971611142    13433 2024-03-04 21:45:26.000000 gen3_tracker-0.0.2rc9/gen3_util/files/manifest.py
+-rw-r--r--   0 peterkor (1520582618) 1971611142     1503 2024-02-28 16:48:14.000000 gen3_tracker-0.0.2rc9/gen3_util/files/middleware.py
+-rw-r--r--   0 peterkor (1520582618) 1971611142      634 2024-02-28 16:48:14.000000 gen3_tracker-0.0.2rc9/gen3_util/files/remover.py
+-rw-r--r--   0 peterkor (1520582618) 1971611142     5194 2024-02-28 16:48:14.000000 gen3_tracker-0.0.2rc9/gen3_util/files/uploader.py
+drwxr-xr-x   0 peterkor (1520582618) 1971611142        0 2024-03-04 21:47:03.090324 gen3_tracker-0.0.2rc9/gen3_util/jobs/
+-rw-r--r--   0 peterkor (1520582618) 1971611142        0 2024-02-28 16:48:14.000000 gen3_tracker-0.0.2rc9/gen3_util/jobs/__init__.py
+-rw-r--r--   0 peterkor (1520582618) 1971611142     2618 2024-03-04 21:44:58.000000 gen3_tracker-0.0.2rc9/gen3_util/jobs/cli.py
+-rw-r--r--   0 peterkor (1520582618) 1971611142      559 2024-02-28 16:48:14.000000 gen3_tracker-0.0.2rc9/gen3_util/jobs/lister.py
+drwxr-xr-x   0 peterkor (1520582618) 1971611142        0 2024-03-04 21:47:03.095653 gen3_tracker-0.0.2rc9/gen3_util/meta/
+-rw-r--r--   0 peterkor (1520582618) 1971611142     4438 2024-02-28 16:48:14.000000 gen3_tracker-0.0.2rc9/gen3_util/meta/__init__.py
+-rw-r--r--   0 peterkor (1520582618) 1971611142     1415 2024-02-28 16:48:14.000000 gen3_tracker-0.0.2rc9/gen3_util/meta/bundler.py
+-rw-r--r--   0 peterkor (1520582618) 1971611142     8981 2024-03-04 21:44:58.000000 gen3_tracker-0.0.2rc9/gen3_util/meta/cli.py
+-rw-r--r--   0 peterkor (1520582618) 1971611142      687 2024-02-28 16:48:14.000000 gen3_tracker-0.0.2rc9/gen3_util/meta/delta.py
+-rw-r--r--   0 peterkor (1520582618) 1971611142     2894 2024-03-04 21:44:58.000000 gen3_tracker-0.0.2rc9/gen3_util/meta/differ.py
+-rw-r--r--   0 peterkor (1520582618) 1971611142      326 2024-02-28 16:48:14.000000 gen3_tracker-0.0.2rc9/gen3_util/meta/downloader.py
+-rw-r--r--   0 peterkor (1520582618) 1971611142     2204 2024-02-28 16:48:14.000000 gen3_tracker-0.0.2rc9/gen3_util/meta/importer.py
+-rw-r--r--   0 peterkor (1520582618) 1971611142     1655 2024-03-01 18:37:10.000000 gen3_tracker-0.0.2rc9/gen3_util/meta/lister.py
+-rw-r--r--   0 peterkor (1520582618) 1971611142     2932 2024-03-04 21:44:58.000000 gen3_tracker-0.0.2rc9/gen3_util/meta/publisher.py
+-rw-r--r--   0 peterkor (1520582618) 1971611142    15141 2024-03-04 21:44:58.000000 gen3_tracker-0.0.2rc9/gen3_util/meta/skeleton.py
+drwxr-xr-x   0 peterkor (1520582618) 1971611142        0 2024-03-04 21:47:03.125627 gen3_tracker-0.0.2rc9/gen3_util/meta/tabular/
+-rw-r--r--   0 peterkor (1520582618) 1971611142    11706 2024-02-28 16:48:14.000000 gen3_tracker-0.0.2rc9/gen3_util/meta/tabular/__init__.py
+-rw-r--r--   0 peterkor (1520582618) 1971611142     4660 2024-02-28 16:48:14.000000 gen3_tracker-0.0.2rc9/gen3_util/meta/uploader.py
+-rw-r--r--   0 peterkor (1520582618) 1971611142     4477 2024-02-28 16:48:14.000000 gen3_tracker-0.0.2rc9/gen3_util/meta/validator.py
+drwxr-xr-x   0 peterkor (1520582618) 1971611142        0 2024-03-04 21:47:03.135930 gen3_tracker-0.0.2rc9/gen3_util/projects/
+-rw-r--r--   0 peterkor (1520582618) 1971611142     2778 2024-03-04 21:44:58.000000 gen3_tracker-0.0.2rc9/gen3_util/projects/__init__.py
+-rw-r--r--   0 peterkor (1520582618) 1971611142     3696 2024-03-04 21:44:58.000000 gen3_tracker-0.0.2rc9/gen3_util/projects/cli.py
+-rw-r--r--   0 peterkor (1520582618) 1971611142     2341 2024-02-28 16:48:14.000000 gen3_tracker-0.0.2rc9/gen3_util/projects/lister.py
+-rw-r--r--   0 peterkor (1520582618) 1971611142     1496 2024-03-04 21:44:58.000000 gen3_tracker-0.0.2rc9/gen3_util/projects/remover.py
+drwxr-xr-x   0 peterkor (1520582618) 1971611142        0 2024-03-04 21:47:03.151071 gen3_tracker-0.0.2rc9/gen3_util/repo/
+-rw-r--r--   0 peterkor (1520582618) 1971611142     4557 2024-02-28 16:48:14.000000 gen3_tracker-0.0.2rc9/gen3_util/repo/__init__.py
+-rw-r--r--   0 peterkor (1520582618) 1971611142    17705 2024-03-04 21:45:26.000000 gen3_tracker-0.0.2rc9/gen3_util/repo/cli.py
+-rw-r--r--   0 peterkor (1520582618) 1971611142     3726 2024-03-04 21:44:58.000000 gen3_tracker-0.0.2rc9/gen3_util/repo/cloner.py
+-rw-r--r--   0 peterkor (1520582618) 1971611142     9643 2024-02-28 16:48:14.000000 gen3_tracker-0.0.2rc9/gen3_util/repo/committer.py
+-rw-r--r--   0 peterkor (1520582618) 1971611142        0 2024-02-28 16:48:14.000000 gen3_tracker-0.0.2rc9/gen3_util/repo/history.py
+-rw-r--r--   0 peterkor (1520582618) 1971611142     1427 2024-03-04 21:44:58.000000 gen3_tracker-0.0.2rc9/gen3_util/repo/initializer.py
+-rw-r--r--   0 peterkor (1520582618) 1971611142     3629 2024-03-04 21:45:26.000000 gen3_tracker-0.0.2rc9/gen3_util/repo/puller.py
+-rw-r--r--   0 peterkor (1520582618) 1971611142     4405 2024-03-04 21:44:58.000000 gen3_tracker-0.0.2rc9/gen3_util/repo/pusher.py
+-rw-r--r--   0 peterkor (1520582618) 1971611142     2959 2024-03-04 21:44:58.000000 gen3_tracker-0.0.2rc9/gen3_util/repo/status.py
+drwxr-xr-x   0 peterkor (1520582618) 1971611142        0 2024-03-04 21:47:03.151952 gen3_tracker-0.0.2rc9/gen3_util/users/
+-rw-r--r--   0 peterkor (1520582618) 1971611142        0 2024-02-28 16:48:14.000000 gen3_tracker-0.0.2rc9/gen3_util/users/__init__.py
+-rw-r--r--   0 peterkor (1520582618) 1971611142     1694 2024-03-04 21:44:58.000000 gen3_tracker-0.0.2rc9/gen3_util/users/cli.py
+-rw-r--r--   0 peterkor (1520582618) 1971611142       38 2024-03-04 21:47:03.212041 gen3_tracker-0.0.2rc9/setup.cfg
+-rw-r--r--   0 peterkor (1520582618) 1971611142     5581 2024-03-04 21:46:21.000000 gen3_tracker-0.0.2rc9/setup.py
+drwxr-xr-x   0 peterkor (1520582618) 1971611142        0 2024-03-04 21:47:03.028754 gen3_tracker-0.0.2rc9/tests/
+drwxr-xr-x   0 peterkor (1520582618) 1971611142        0 2024-03-04 21:47:03.158045 gen3_tracker-0.0.2rc9/tests/integration/
+-rw-r--r--   0 peterkor (1520582618) 1971611142        0 2024-02-13 19:02:16.000000 gen3_tracker-0.0.2rc9/tests/integration/__init__.py
+-rw-r--r--   0 peterkor (1520582618) 1971611142     1091 2024-02-28 16:48:14.000000 gen3_tracker-0.0.2rc9/tests/integration/conftest.py
+-rw-r--r--   0 peterkor (1520582618) 1971611142     1066 2024-03-04 21:44:58.000000 gen3_tracker-0.0.2rc9/tests/integration/test_access.py
+-rw-r--r--   0 peterkor (1520582618) 1971611142      454 2024-02-28 16:48:14.000000 gen3_tracker-0.0.2rc9/tests/integration/test_buckets.py
+-rw-r--r--   0 peterkor (1520582618) 1971611142    12321 2024-03-04 21:44:58.000000 gen3_tracker-0.0.2rc9/tests/integration/test_commit.py
+-rw-r--r--   0 peterkor (1520582618) 1971611142      257 2024-02-28 16:48:14.000000 gen3_tracker-0.0.2rc9/tests/integration/test_config.py
+-rw-r--r--   0 peterkor (1520582618) 1971611142     4867 2024-03-04 21:45:26.000000 gen3_tracker-0.0.2rc9/tests/integration/test_foreign_bucket.py
+-rw-r--r--   0 peterkor (1520582618) 1971611142     1987 2024-03-04 21:44:58.000000 gen3_tracker-0.0.2rc9/tests/integration/test_init.py
+-rw-r--r--   0 peterkor (1520582618) 1971611142     9506 2024-02-28 16:48:14.000000 gen3_tracker-0.0.2rc9/tests/integration/test_meta.py
+-rw-r--r--   0 peterkor (1520582618) 1971611142     8848 2024-02-28 16:48:14.000000 gen3_tracker-0.0.2rc9/tests/integration/test_meta_skeleton.py
+-rw-r--r--   0 peterkor (1520582618) 1971611142     5763 2024-03-04 21:45:26.000000 gen3_tracker-0.0.2rc9/tests/integration/test_no_bucket.py
+-rw-r--r--   0 peterkor (1520582618) 1971611142     1321 2024-02-28 16:48:14.000000 gen3_tracker-0.0.2rc9/tests/integration/test_project.py
+drwxr-xr-x   0 peterkor (1520582618) 1971611142        0 2024-03-04 21:47:03.170102 gen3_tracker-0.0.2rc9/tests/unit/
+-rw-r--r--   0 peterkor (1520582618) 1971611142        0 2024-02-13 19:02:16.000000 gen3_tracker-0.0.2rc9/tests/unit/__init__.py
+-rw-r--r--   0 peterkor (1520582618) 1971611142      464 2024-02-28 16:48:14.000000 gen3_tracker-0.0.2rc9/tests/unit/conftest.py
+drwxr-xr-x   0 peterkor (1520582618) 1971611142        0 2024-03-04 21:47:03.171085 gen3_tracker-0.0.2rc9/tests/unit/plugins/
+-rw-r--r--   0 peterkor (1520582618) 1971611142        0 2024-02-28 16:48:14.000000 gen3_tracker-0.0.2rc9/tests/unit/plugins/__init__.py
+drwxr-xr-x   0 peterkor (1520582618) 1971611142        0 2024-03-04 21:47:03.171385 gen3_tracker-0.0.2rc9/tests/unit/plugins/gen3_util_plugin_foo/
+-rw-r--r--   0 peterkor (1520582618) 1971611142     1450 2024-02-28 16:48:14.000000 gen3_tracker-0.0.2rc9/tests/unit/plugins/gen3_util_plugin_foo/__init__.py
+drwxr-xr-x   0 peterkor (1520582618) 1971611142        0 2024-03-04 21:47:03.211331 gen3_tracker-0.0.2rc9/tests/unit/tabular/
+-rw-r--r--   0 peterkor (1520582618) 1971611142        0 2024-02-28 16:48:14.000000 gen3_tracker-0.0.2rc9/tests/unit/tabular/__init__.py
+-rw-r--r--   0 peterkor (1520582618) 1971611142    16696 2024-02-28 16:48:14.000000 gen3_tracker-0.0.2rc9/tests/unit/tabular/conftest.py
+-rw-r--r--   0 peterkor (1520582618) 1971611142     1172 2024-02-28 16:48:14.000000 gen3_tracker-0.0.2rc9/tests/unit/tabular/test_config.py
+-rw-r--r--   0 peterkor (1520582618) 1971611142     7826 2024-02-28 16:48:14.000000 gen3_tracker-0.0.2rc9/tests/unit/tabular/test_default_columns.py
+-rw-r--r--   0 peterkor (1520582618) 1971611142     1035 2024-02-28 16:48:14.000000 gen3_tracker-0.0.2rc9/tests/unit/tabular/test_dir_to_tabular.py
+-rw-r--r--   0 peterkor (1520582618) 1971611142     1888 2024-02-28 16:48:14.000000 gen3_tracker-0.0.2rc9/tests/unit/tabular/test_from_tabular.py
+-rw-r--r--   0 peterkor (1520582618) 1971611142     3779 2024-02-28 16:48:14.000000 gen3_tracker-0.0.2rc9/tests/unit/tabular/test_to_tabular.py
+-rw-r--r--   0 peterkor (1520582618) 1971611142      737 2024-02-28 16:48:14.000000 gen3_tracker-0.0.2rc9/tests/unit/tabular/test_validate.py
+-rw-r--r--   0 peterkor (1520582618) 1971611142     3841 2024-03-04 21:44:58.000000 gen3_tracker-0.0.2rc9/tests/unit/test_cli.py
+-rw-r--r--   0 peterkor (1520582618) 1971611142     4881 2024-02-28 16:48:14.000000 gen3_tracker-0.0.2rc9/tests/unit/test_coding.py
+-rw-r--r--   0 peterkor (1520582618) 1971611142      565 2024-02-13 19:02:16.000000 gen3_tracker-0.0.2rc9/tests/unit/test_coding_conventions.py
+-rw-r--r--   0 peterkor (1520582618) 1971611142      532 2024-02-28 16:48:14.000000 gen3_tracker-0.0.2rc9/tests/unit/test_config.py
+-rw-r--r--   0 peterkor (1520582618) 1971611142     1417 2024-02-28 16:48:14.000000 gen3_tracker-0.0.2rc9/tests/unit/test_files.py
+-rw-r--r--   0 peterkor (1520582618) 1971611142      445 2024-02-28 16:48:14.000000 gen3_tracker-0.0.2rc9/tests/unit/test_job_dependencies.py
+-rw-r--r--   0 peterkor (1520582618) 1971611142      734 2024-02-28 16:48:14.000000 gen3_tracker-0.0.2rc9/tests/unit/test_manifest.py
+-rw-r--r--   0 peterkor (1520582618) 1971611142     1546 2024-02-28 16:48:14.000000 gen3_tracker-0.0.2rc9/tests/unit/test_validate_directory.py
+-rw-r--r--   0 peterkor (1520582618) 1971611142      625 2024-02-28 16:48:14.000000 gen3_tracker-0.0.2rc9/tests/unit/test_version.py
```

### Comparing `gen3_tracker-0.0.2rc8/LICENSE` & `gen3_tracker-0.0.2rc9/LICENSE`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.2rc8/README.md` & `gen3_tracker-0.0.2rc9/README.md`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.2rc8/gen3_tracker.egg-info/SOURCES.txt` & `gen3_tracker-0.0.2rc9/gen3_tracker.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -64,17 +64,19 @@
 gen3_util/users/cli.py
 tests/integration/__init__.py
 tests/integration/conftest.py
 tests/integration/test_access.py
 tests/integration/test_buckets.py
 tests/integration/test_commit.py
 tests/integration/test_config.py
+tests/integration/test_foreign_bucket.py
 tests/integration/test_init.py
 tests/integration/test_meta.py
 tests/integration/test_meta_skeleton.py
+tests/integration/test_no_bucket.py
 tests/integration/test_project.py
 tests/unit/__init__.py
 tests/unit/conftest.py
 tests/unit/test_cli.py
 tests/unit/test_coding.py
 tests/unit/test_coding_conventions.py
 tests/unit/test_config.py
```

### Comparing `gen3_tracker-0.0.2rc8/gen3_util/__init__.py` & `gen3_tracker-0.0.2rc9/gen3_util/__init__.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.2rc8/gen3_util/access/__init__.py` & `gen3_tracker-0.0.2rc9/gen3_util/access/__init__.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.2rc8/gen3_util/access/cli.py` & `gen3_tracker-0.0.2rc9/gen3_util/access/cli.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.2rc8/gen3_util/access/requestor.py` & `gen3_tracker-0.0.2rc9/gen3_util/access/requestor.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.2rc8/gen3_util/access/submitter.py` & `gen3_tracker-0.0.2rc9/gen3_util/access/submitter.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.2rc8/gen3_util/buckets/__init__.py` & `gen3_tracker-0.0.2rc9/gen3_util/buckets/__init__.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.2rc8/gen3_util/buckets/cli.py` & `gen3_tracker-0.0.2rc9/gen3_util/buckets/cli.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.2rc8/gen3_util/buckets/lister.py` & `gen3_tracker-0.0.2rc9/gen3_util/buckets/lister.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.2rc8/gen3_util/common/__init__.py` & `gen3_tracker-0.0.2rc9/gen3_util/common/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -153,14 +153,22 @@
 
     def emit(self, name: str) -> TextIO:
         """Maintain a hash of open files."""
         if name not in self.emitters:
             self.emitters[name] = open(self.output_path / f"{name}.ndjson", self.file_mode)
             if self.verbose:
                 self.logger.info(f"opened {self.emitters[name].name}")
+
+            # If the user already has metadata in the resource file but wants to add
+            # another file the the first line will create a 2nd record on the same line causing the commit step to error
+            if os.path.getsize(self.emitters[name].name) > 0:
+                self.emitters[name].seek(self.emitters[name].tell() - 1, os.SEEK_SET)
+                last_char = self.emitters[name].read()
+                if last_char == "}":
+                    self.emitters[name].write("\n")
         return self.emitters[name]
 
 
 def validate_project_id(project_id) -> list[str]:
     """Ensure that the project_id is valid"""
     msgs = []
     if not project_id:
```

### Comparing `gen3_tracker-0.0.2rc8/gen3_util/config/__init__.py` & `gen3_tracker-0.0.2rc9/gen3_util/config/__init__.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.2rc8/gen3_util/config/cli.py` & `gen3_tracker-0.0.2rc9/gen3_util/config/cli.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.2rc8/gen3_util/files/__init__.py` & `gen3_tracker-0.0.2rc9/gen3_util/files/__init__.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.2rc8/gen3_util/files/cli.py` & `gen3_tracker-0.0.2rc9/gen3_util/files/cli.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import json
 import os
 import sys
+from datetime import datetime
 from json import JSONDecodeError
 from pathlib import Path
 
 import click
 from requests import HTTPError
 
 from gen3_util.repo import CLIOutput, ENV_VARIABLE_PREFIX
@@ -13,14 +14,15 @@
 from gen3_util.config import Config
 from gen3_util.files.middleware import files_ls_driver
 from gen3_util.files.manifest import put as manifest_put, save as manifest_save, ls as manifest_ls, upload_indexd, \
     upload_files, rm as manifest_rm
 from gen3_util.files.remover import rm
 from gen3_util.meta.publisher import publish_meta_data
 from gen3_util.meta.skeleton import study_metadata
+from urllib.parse import urlparse
 
 
 @click.group(name='files', cls=NaturalOrderGroup)
 @click.pass_obj
 def file_group(config):
     """Manage file transfers."""
     pass
@@ -50,53 +52,75 @@
               help="long format")
 def files_ls(config: Config, object_id: str, project_id: str, specimen: str, patient: str, observation: str, task: str, md5: str, is_metadata: bool, is_snapshot: bool, long: bool):
     """List uploaded files in a project bucket."""
     files_ls_driver(config, object_id, project_id, specimen, patient, observation, task, md5, is_metadata, is_snapshot, long)
 
 
 @file_group.command(name="add")
-@click.argument('local_path', type=click.Path(exists=True, dir_okay=False))
+@click.argument('path')
 # @click.argument('remote_path', required=False, default=None)
 @click.option('--project_id', default=None, required=False, show_default=True,
               help="Gen3 program-project", envvar=f"{ENV_VARIABLE_PREFIX}PROJECT_ID", hidden=True)
 # @click.option('--source_path', required=False, default=None, show_default=True,
 #               help='Path on local file system')
 @click.option('--specimen', default=None, required=False, show_default=True,
               help="fhir specimen identifier", envvar=f'{ENV_VARIABLE_PREFIX}SPECIMEN')
 @click.option('--patient', default=None, required=False, show_default=True,
               help="fhir patient identifier", envvar=f'{ENV_VARIABLE_PREFIX}PATIENT')
 @click.option('--task', default=None, required=False, show_default=True,
               help="fhir task identifier", envvar=f'{ENV_VARIABLE_PREFIX}TASK')
 @click.option('--observation', default=None, required=False, show_default=True,
               help="fhir observation identifier", envvar=f'{ENV_VARIABLE_PREFIX}OBSERVATION')
 @click.option('--md5', default=None, required=False, show_default=True,
-              help="MD5 sum, if not provided, will be calculated before upload")
+              help="MD5 sum, if not provided, will be calculated before upload, required for non-local files")
+@click.option('--size', default=None, required=False, show_default=True, type=int,
+              help="file size in bytes, required for non-local files")
+@click.option('--no-bucket', 'no_bucket', default=False, required=False, show_default=True, is_flag=True,
+              envvar=f'{ENV_VARIABLE_PREFIX}NO_BUCKET',
+              help="Do not upload to bucket, only add to index. (Uses symlink or scp to download).")
+@click.option('--modified', default=None, required=False, show_default=True, type=click.DateTime(),
+              help="Modified datetime of the file, required for non-local files")
 @click.pass_obj
-def manifest_put_cli(config: Config, local_path: str, project_id: str, md5: str,
-                     specimen: str, patient: str, observation: str, task: str):
+def manifest_put_cli(config: Config, path: str, project_id: str, md5: str,
+                     specimen: str, patient: str, observation: str, task: str, no_bucket: bool, size: int, modified: datetime):
     """Add file to the index.
 
     \b
     local_path: relative path to file or symbolic link on the local file system
     """
     # TODO deprecate `remote_path` insist on relative paths
     with CLIOutput(config=config) as output:
         try:
-            assert Path(PROJECT_DIR).exists(), "Please add files from the project root directory."
-            assert Path(local_path).absolute().is_relative_to(Path.cwd().absolute()), \
-                f"{local_path} must be relative to the project root, please move the file or create a symbolic link"
+            _parsed = urlparse(path, allow_fragments=False)
+            if _parsed.scheme != '' and _parsed.scheme in ['s3', 'gs', 'abfs']:
+                local_path = _parsed.path.lstrip('/')
+                url = path
+            elif _parsed.scheme != '':
+                raise ValueError(f"Unsupported url scheme {_parsed.scheme}")
+            elif _parsed.scheme == '' and Path(path).exists():
+                local_path = path
+                url = None
+                assert Path(PROJECT_DIR).exists(), "Please add files from the project root directory."
+                assert Path(local_path).absolute().is_relative_to(Path.cwd().absolute()), \
+                    f"{local_path} must be relative to the project root, please move the file or create a symbolic link"
+            if url:
+                assert all([size, md5, modified]), "size, md5, and modified are required for bucket objects"
 
             if not project_id:
                 project_id = config.gen3.project_id
-            _ = manifest_put(config, local_path, project_id=project_id, md5=md5)
+
+            _ = manifest_put(config, local_path, project_id=project_id, md5=md5, size=size, modified=modified)
+
             _['observation_id'] = observation
             _['patient_id'] = patient
             _['specimen_id'] = specimen
             _['task_id'] = task
             _['remote_path'] = None
+            _['no_bucket'] = no_bucket
+            _['url'] = url
             output.update(_)
             manifest_save(config, project_id, [_])
         except Exception as e:
             output.exit_code = 1
             output.update({'msg': str(e)})
```

### Comparing `gen3_tracker-0.0.2rc8/gen3_util/files/lister.py` & `gen3_tracker-0.0.2rc9/gen3_util/files/lister.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.2rc8/gen3_util/files/manifest.py` & `gen3_tracker-0.0.2rc9/gen3_util/files/manifest.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import json
 import logging
 import pathlib
+import socket
 import sqlite3
 import subprocess
 import sys
 import uuid
 from datetime import datetime, time
 import multiprocessing
 # from multiprocessing.pool import Pool
@@ -35,39 +36,52 @@
         sqllite_path = config.state_dir / config.gen3.project_id / 'commits' / commit_id / 'manifest.sqlite'
     _connection = sqlite3.connect(sqllite_path)
     with _connection:
         _connection.execute('CREATE TABLE if not exists manifest (object_id PRIMARY KEY, project_id Text, entity Text)')
     return _connection
 
 
-def put(config: Config, file_name: str, project_id: str, md5: str):
+def put(config: Config, file_name: str, project_id: str, md5: str, size: int = None, modified: str = None):
     """Create manifest entry for a file."""
     object_name = _normalize_file_url(file_name)
+
     file = pathlib.Path(object_name)
-    assert file.is_file(), f"{file} is not a file"
 
     assert project_id, "project_id is missing"
     assert project_id.count('-') == 1, f"{project_id} should have a single '-' delimiter."
 
-    stat = file.stat()
+    is_symlink = False
+    realpath = None
+    if file.is_file():  # could be a url
+        if not md5:
+            md5 = md5sum(file)
+        if not size:
+            size = file.stat().st_size
+        if not modified:
+            modified = datetime.fromtimestamp(file.stat().st_mtime)
+        is_symlink = file.is_symlink()
+        realpath = str(file.resolve())
+
     mime = get_mime_type(file)
 
     object_id = str(uuid.uuid5(ACED_NAMESPACE, project_id + f"::{file}"))
 
-    if not md5:
-        md5 = md5sum(file)
-
-    return {
+    _ = {
         "object_id": object_id,
         "file_name": object_name,
-        "size": stat.st_size,
-        "modified": datetime.fromtimestamp(stat.st_mtime),
+        "size": size,
+        "modified": modified,
         "md5": md5,
         "mime_type": mime,
+        "is_symlink": is_symlink,
     }
+    if realpath:
+        _['realpath'] = realpath
+
+    return _
 
 
 def save(config: Config, project_id: str, generator, max_retries: int = 3, base_delay=2):
     """Write to local sqlite."""
     for retry_count in range(max_retries):
         try:
             connection = _get_connection(config)
@@ -137,25 +151,36 @@
     if restricted_project_id:
         _ = restricted_project_id.split('-')
         authz.append(f'/programs/{_[0]}/projects/{_[1]}')
 
     # strip any file:/// prefix
     manifest_item['file_name'] = urlparse(manifest_item['file_name']).path
 
+    if 'realpath' in manifest_item:
+        metadata['realpath'] = urlparse(manifest_item['realpath']).path
+
     if not existing_record:
         try:
             file_name = manifest_item['remote_path'] or manifest_item['file_name']
+            urls = [f"s3://{bucket_name}/{manifest_item['object_id']}/{file_name}"]
+            if manifest_item.get('no_bucket', False):
+                hostname = socket.gethostname()
+                _ = f"{hostname}/{metadata['realpath']}".replace('//', '/')
+                urls = [f"scp://{_}"]
+            if manifest_item.get('url', None):
+                urls = [manifest_item['url']]
+
             response = index_client.create_record(
                 did=manifest_item["object_id"],
                 hashes=hashes,
                 size=manifest_item["size"],
                 authz=authz,
                 file_name=file_name,
                 metadata=metadata,
-                urls=[f"s3://{bucket_name}/{manifest_item['object_id']}/{file_name}"]
+                urls=urls
             )
             assert response, "Expected response from indexd create_record"
         except (requests.exceptions.HTTPError, AssertionError) as e:
             if 'already exists' in str(e):
                 logger.error(f"indexd record already exists, consider using --overwrite. {manifest_item['object_id']} {str(e)}")
             raise e
     return True
@@ -167,14 +192,15 @@
         **{
             'document_reference_id': manifest_item['object_id'],
             'specimen_identifier': manifest_item.get('specimen_id', None),
             'patient_identifier': manifest_item.get('patient_id', None),
             'task_identifier': manifest_item.get('task_id', None),
             'observation_identifier': manifest_item.get('observation_id', None),
             'project_id': f'{program}-{project}',
+            'no_bucket': manifest_item.get('no_bucket', False),
         },
         **hashes}
     return hashes, metadata
 
 
 def worker_count():
     """Return number of workers for multiprocessing."""
```

### Comparing `gen3_tracker-0.0.2rc8/gen3_util/files/middleware.py` & `gen3_tracker-0.0.2rc9/gen3_util/files/middleware.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.2rc8/gen3_util/files/remover.py` & `gen3_tracker-0.0.2rc9/gen3_util/files/remover.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.2rc8/gen3_util/files/uploader.py` & `gen3_tracker-0.0.2rc9/gen3_util/files/uploader.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.2rc8/gen3_util/jobs/cli.py` & `gen3_tracker-0.0.2rc9/gen3_util/jobs/cli.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.2rc8/gen3_util/jobs/lister.py` & `gen3_tracker-0.0.2rc9/gen3_util/jobs/lister.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.2rc8/gen3_util/meta/__init__.py` & `gen3_tracker-0.0.2rc9/gen3_util/meta/__init__.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.2rc8/gen3_util/meta/bundler.py` & `gen3_tracker-0.0.2rc9/gen3_util/meta/bundler.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.2rc8/gen3_util/meta/cli.py` & `gen3_tracker-0.0.2rc9/gen3_util/meta/cli.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.2rc8/gen3_util/meta/delta.py` & `gen3_tracker-0.0.2rc9/gen3_util/meta/delta.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.2rc8/gen3_util/meta/differ.py` & `gen3_tracker-0.0.2rc9/gen3_util/meta/differ.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.2rc8/gen3_util/meta/importer.py` & `gen3_tracker-0.0.2rc9/gen3_util/meta/importer.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.2rc8/gen3_util/meta/lister.py` & `gen3_tracker-0.0.2rc9/gen3_util/meta/lister.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.2rc8/gen3_util/meta/publisher.py` & `gen3_tracker-0.0.2rc9/gen3_util/meta/publisher.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.2rc8/gen3_util/meta/skeleton.py` & `gen3_tracker-0.0.2rc9/gen3_util/meta/skeleton.py`

 * *Files 3% similar despite different names*

```diff
@@ -99,26 +99,21 @@
         # get all records already uploaded from current manifest
         # object_id = ','.join([_['object_id'] for _ in manifest_ls(config, project_id=project_id)])
         # records = ls(config, object_id=object_id)['records']
         records = manifest_to_indexd(config, project_id)
     else:
         raise ValueError(f"source must be 'indexd' or 'manifest' not {source}")
 
-    with EmitterContextManager(output_path, file_mode="a") as emitter:
+    with EmitterContextManager(output_path, file_mode="a+") as emitter:
         if len(records) == 0:
             print(f"No records found for project_id:{project_id}", file=sys.stderr)
-
         new_record_count = 0
         existing_record_count = 0
-
-        existing_research_study_ids = [_['id'] for _ in read_meta_index(config.state_dir) if _['resourceType'] == 'ResearchStudy']
-        existing_research_study_ids.extend([_['id'] for _ in Push(config=config).pending_meta_index() if _['resourceType'] == 'ResearchStudy'])
-
         for _ in records:
-            resources = create_skeleton(config=config, metadata=_['metadata'], indexd_record=_, existing_research_study_ids=existing_research_study_ids)
+            resources = create_skeleton(config=config, metadata=_['metadata'], indexd_record=_)
             for resource in resources:
 
                 # check document references
                 if resource.id in existing_resource_ids:
                     existing_record_count += 1
                     continue
 
@@ -195,15 +190,15 @@
         return identifier.split('#')[0]
     if '|' in identifier:
         return identifier.split('|')[0]
     # default
     return f"https://aced-idp.org/{project_id}"
 
 
-def create_skeleton(metadata: dict, indexd_record: dict, config: Config = None, existing_research_study_ids: list[str] = []) -> list[Resource]:  # TODO fix caller auth
+def create_skeleton(metadata: dict, indexd_record: dict, config: Config = None) -> list[Resource]:  # TODO fix caller auth
     """
     Create a skeleton graph for document and ancestors from a set of identifiers.
     """
 
     document_reference_id = metadata.get('document_reference_id', None)
     specimen_identifier = metadata.get('specimen_identifier', None)
     patient_identifier = metadata.get('patient_identifier', None)
@@ -216,37 +211,39 @@
 
     if not document_reference_id:
         return []
         # metadata can include submission files, etc. that are not attached to a document reference ie is_metadata = True
 
     assert project_id, "project_id required"
     assert project_id.count('-') == 1, "project_id must be of the form program-project"
-    # program, project = project_id.split('-')
+    program, project = project_id.split('-')
 
     already_created = set()
     if config:
         existing_meta_index = {_['id']: _['md5'] for _ in read_meta_index(config.state_dir)}
         pending_meta_index = {_['id']: _['md5'] for _ in Push(config=config).pending_meta_index()}
         already_created = set(existing_meta_index.keys())
         already_created.update(pending_meta_index.keys())
 
     # create entities
     research_study = research_subject = observation = specimen = patient = task = None
 
     # _existing_research_study = meta_resource(submission_client=submission_client, identifier=None, project_id=project_id, gen3_type='research_study')
-    if len(existing_research_study_ids) == 0:
+    _existing_research_study = None
+    if not _existing_research_study:
         research_study = ResearchStudy(status='active')
         research_study.description = f"Skeleton ResearchStudy for {project_id}"
         research_study.identifier = [
             Identifier(value=project_id, system=_get_system(project_id, project_id=project_id),
                        use='official')]
         research_study.id = create_id(research_study, project_id)
         research_study_id = research_study.id
+
     else:
-        research_study_id = existing_research_study_ids[0]
+        research_study_id = _existing_research_study['id']
 
     document_reference = DocumentReference(status='current', content=[{'attachment': {'url': "file://"}}])
     document_reference.id = document_reference_id
     document_reference.identifier = [
         Identifier(value=document_reference_id, system=_get_system(document_reference_id, project_id=project_id),
                    use='official')]
     update_document_reference(document_reference, indexd_record)
@@ -334,12 +331,12 @@
     if observation:
         document_reference.subject = {'reference': f"Observation/{observation.id}"}
     if specimen and not document_reference.subject:
         document_reference.subject = {'reference': f"Specimen/{specimen.id}"}
     if patient and not document_reference.subject:
         document_reference.subject = {'reference': f"Patient/{patient.id}"}
     if not document_reference.subject:
-        document_reference.subject = {'reference': f"ResearchStudy/{research_study_id}"}
+        document_reference.subject = {'reference': f"ResearchStudy/{research_study.id}"}
 
     if discard_specimen:
         specimen = None
     return [_ for _ in [research_study, research_subject, patient, observation, specimen, task, document_reference] if _]
```

### Comparing `gen3_tracker-0.0.2rc8/gen3_util/meta/tabular/__init__.py` & `gen3_tracker-0.0.2rc9/gen3_util/meta/tabular/__init__.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.2rc8/gen3_util/meta/uploader.py` & `gen3_tracker-0.0.2rc9/gen3_util/meta/uploader.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.2rc8/gen3_util/meta/validator.py` & `gen3_tracker-0.0.2rc9/gen3_util/meta/validator.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.2rc8/gen3_util/projects/__init__.py` & `gen3_tracker-0.0.2rc9/gen3_util/projects/__init__.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.2rc8/gen3_util/projects/cli.py` & `gen3_tracker-0.0.2rc9/gen3_util/projects/cli.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.2rc8/gen3_util/projects/lister.py` & `gen3_tracker-0.0.2rc9/gen3_util/projects/lister.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.2rc8/gen3_util/projects/remover.py` & `gen3_tracker-0.0.2rc9/gen3_util/projects/remover.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.2rc8/gen3_util/repo/__init__.py` & `gen3_tracker-0.0.2rc9/gen3_util/repo/__init__.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.2rc8/gen3_util/repo/cli.py` & `gen3_tracker-0.0.2rc9/gen3_util/repo/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -204,18 +204,15 @@
     \b
     METADATA_PATH: directory containing metadata files to be compared. [default: ./META]
     """
     with CLIOutput(config=config) as output:
         try:
             assert config.gen3.project_id, "Not in an initialed project directory."
             metadata_path = pathlib.Path(metadata_path)
-            _ = {'diff': [_ for _ in diff(config, metadata_path)]}
-            if len(_['diff']) == 0:
-                _['msg'] = "Everything up-to-date"
-            output.update(_)
+            output.update({'diff': [_ for _ in diff(config, metadata_path)]})
 
         except AssertionError as e:
             output.update({'msg': str(e)})
             output.exit_code = 1
 
 
 @cli.command(name='push')
@@ -351,15 +348,16 @@
                     config=config,
                     auth=auth,
                     snapshot_manifest=snapshot_manifest,
                     logs=logs,
                     original_path=original_path,
                     extract_to=path
                 )
-                output.update(logs)
+
+            output.update({'logs': logs})
 
         except AssertionError as e:
             output.update({'msg': str(e)})
             output.exit_code = 1
 
 
 @cli.command(name="update-index")
@@ -387,43 +385,53 @@
     """Remove project.
     """
     with CLIOutput(config=config) as output:
         output.update(rm(config, project_id))
 
 
 @cli.command(name="reset")
+@click.argument('project_id', default=None, required=False, envvar=f"{ENV_VARIABLE_PREFIX}PROJECT_ID")
 @click.pass_obj
-def project_empty(config: Config):
+def project_empty(config: Config, project_id: str):
     """Empty all metadata (graph, flat) for a project."""
     with CLIOutput(config=config) as output:
         try:
-            assert config.gen3.project_id, "Not in an initialized project directory."
-            project_id = config.gen3.project_id
+            in_project = False
+            if not project_id:
+                assert config.gen3.project_id, "Not in an initialized project directory."
+                project_id = config.gen3.project_id
+                in_project = True
+
             _check_parameters(config, project_id)
             _ = empty(config, project_id)
             _['msg'] = f"Emptied {project_id}"
             output.update(_)
 
-            delete_all_commits(config.commit_dir())
-            for file in [".g3t/state/manifest.sqlite", ".g3t/state/meta-index.ndjson"]:
-                if os.path.isfile(file):
-                    os.unlink(file)
-
-            push_ = Push(config=config)
-            push_.published_job = _
-            completed_path = push_.config.commit_dir() / "emptied.ndjson"
-            push_.published_timestamp = datetime.now()
-
-            with open(completed_path, "w") as fp:
-                fp.write(push_.model_dump_json())
-                fp.write("\n")
-            print(
-                f"Updated {completed_path}",
-                file=sys.stderr
-            )
+            if in_project:
+                """Delete all previous commits and manifests, but keep the project config file."""
+                delete_all_commits(config.commit_dir())
+                for file in [".g3t/state/manifest.sqlite", ".g3t/state/meta-index.ndjson"]:
+                    if os.path.isfile(file):
+                        os.unlink(file)
+
+                """
+                Create a new push file titled 'emptied.ndjson' that contains
+                the job metadata from the empty function called above.
+                """
+                push_ = Push(config=config)
+                push_.published_job = _
+                completed_path = push_.config.commit_dir() / "emptied.ndjson"
+                push_.published_timestamp = datetime.now()
+
+                with open(completed_path, "w") as fp:
+                    fp.write(push_.model_dump_json())
+                    fp.write("\n")
+                click.secho(
+                    f"Updated {completed_path}",
+                    file=sys.stderr, fg='green')
 
         except Exception as e:
             output.update({'msg': str(e)})
             output.exit_code = 1
 
 
 @cli.group(name='utilities', cls=NaturalOrderGroup)
```

### Comparing `gen3_tracker-0.0.2rc8/gen3_util/repo/cloner.py` & `gen3_tracker-0.0.2rc9/gen3_util/repo/cloner.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.2rc8/gen3_util/repo/committer.py` & `gen3_tracker-0.0.2rc9/gen3_util/repo/committer.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.2rc8/gen3_util/repo/initializer.py` & `gen3_tracker-0.0.2rc9/gen3_util/repo/initializer.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,15 +16,14 @@
             return ["Disconnected mode, skipping server side initialization"]
         auth = ensure_auth(config=config)
 
     logs = []
     program, project = project_id.split('-')
     projects = project_ls(config, auth=auth)
     existing_project = [_ for _ in projects.complete if _.endswith(project)]
-    existing_project.extend([_ for _ in projects.incomplete if _.endswith(project)])
     policy_msgs = []
     if len(existing_project) > 0:
         submission_client = Gen3Submission(auth)
         links = submission_client.get_projects(program)['links']
         sheepdog = [_ for _ in links if _ == f"/v0/submission/{program}/{project}"]
         if len(sheepdog) > 0:
             logs.append(f"Project already exists on server: {program}-{project}")
```

### Comparing `gen3_tracker-0.0.2rc8/gen3_util/repo/pusher.py` & `gen3_tracker-0.0.2rc9/gen3_util/repo/pusher.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.2rc8/gen3_util/repo/status.py` & `gen3_tracker-0.0.2rc9/gen3_util/repo/status.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.2rc8/gen3_util/users/cli.py` & `gen3_tracker-0.0.2rc9/gen3_util/users/cli.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.2rc8/setup.py` & `gen3_tracker-0.0.2rc9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     # There are some restrictions on what makes a valid project name
     # specification here:
     # https://packaging.python.org/specifications/core-metadata/#name
     name='gen3_tracker',  # Required
 
     # Versions should comply with PEP 440:
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='0.0.2rc8',  # Required
+    version='0.0.2rc9',  # Required
 
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description='Commons utilities',
     # Optional
```

### Comparing `gen3_tracker-0.0.2rc8/tests/integration/conftest.py` & `gen3_tracker-0.0.2rc9/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.2rc8/tests/integration/test_access.py` & `gen3_tracker-0.0.2rc9/tests/integration/test_access.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.2rc8/tests/integration/test_init.py` & `gen3_tracker-0.0.2rc9/tests/integration/test_init.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.2rc8/tests/integration/test_meta.py` & `gen3_tracker-0.0.2rc9/tests/integration/test_meta.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.2rc8/tests/integration/test_meta_skeleton.py` & `gen3_tracker-0.0.2rc9/tests/integration/test_meta_skeleton.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.2rc8/tests/integration/test_project.py` & `gen3_tracker-0.0.2rc9/tests/integration/test_project.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.2rc8/tests/unit/plugins/gen3_util_plugin_foo/__init__.py` & `gen3_tracker-0.0.2rc9/tests/unit/plugins/gen3_util_plugin_foo/__init__.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.2rc8/tests/unit/tabular/conftest.py` & `gen3_tracker-0.0.2rc9/tests/unit/tabular/conftest.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.2rc8/tests/unit/tabular/test_config.py` & `gen3_tracker-0.0.2rc9/tests/unit/tabular/test_config.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.2rc8/tests/unit/tabular/test_default_columns.py` & `gen3_tracker-0.0.2rc9/tests/unit/tabular/test_default_columns.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.2rc8/tests/unit/tabular/test_dir_to_tabular.py` & `gen3_tracker-0.0.2rc9/tests/unit/tabular/test_dir_to_tabular.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.2rc8/tests/unit/tabular/test_from_tabular.py` & `gen3_tracker-0.0.2rc9/tests/unit/tabular/test_from_tabular.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.2rc8/tests/unit/tabular/test_to_tabular.py` & `gen3_tracker-0.0.2rc9/tests/unit/tabular/test_to_tabular.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.2rc8/tests/unit/tabular/test_validate.py` & `gen3_tracker-0.0.2rc9/tests/unit/tabular/test_validate.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.2rc8/tests/unit/test_cli.py` & `gen3_tracker-0.0.2rc9/tests/unit/test_cli.py`

 * *Files 9% similar despite different names*

```diff
@@ -89,7 +89,18 @@
     assert result.exit_code == 0, result.output
     print(result.output)
     expected_strings = """
       ls  Show defaults.
     """.split()
     for expected_string in expected_strings:
         assert expected_string in result.output, f"Should have printed {expected_string}"
+
+
+def test_add():
+    """Ensure no-bucket flag is present"""
+    runner = CliRunner()
+    result = runner.invoke(cli, 'add --help'.split())
+    assert result.exit_code == 0, result.output
+    print(result.output)
+    expected_strings = ["no-bucket", "Do not upload to bucket"]
+    for expected_string in expected_strings:
+        assert expected_string in result.output, f"Should have printed {expected_string}"
```

### Comparing `gen3_tracker-0.0.2rc8/tests/unit/test_coding.py` & `gen3_tracker-0.0.2rc9/tests/unit/test_coding.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.2rc8/tests/unit/test_coding_conventions.py` & `gen3_tracker-0.0.2rc9/tests/unit/test_coding_conventions.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.2rc8/tests/unit/test_config.py` & `gen3_tracker-0.0.2rc9/tests/unit/test_config.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.2rc8/tests/unit/test_files.py` & `gen3_tracker-0.0.2rc9/tests/unit/test_files.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.2rc8/tests/unit/test_manifest.py` & `gen3_tracker-0.0.2rc9/tests/unit/test_manifest.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.2rc8/tests/unit/test_validate_directory.py` & `gen3_tracker-0.0.2rc9/tests/unit/test_validate_directory.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.2rc8/tests/unit/test_version.py` & `gen3_tracker-0.0.2rc9/tests/unit/test_version.py`

 * *Files identical despite different names*

