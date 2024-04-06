# Comparing `tmp/tracker-exporter-1.0.3.tar.gz` & `tmp/tracker-exporter-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tracker-exporter-1.0.3.tar", last modified: Mon Mar 25 11:38:05 2024, max compression
+gzip compressed data, was "tracker-exporter-2.0.0.tar", last modified: Sat Apr  6 10:41:29 2024, max compression
```

## Comparing `tracker-exporter-1.0.3.tar` & `tracker-exporter-2.0.0.tar`

### file list

```diff
@@ -1,36 +1,41 @@
-drwxr-xr-x   0 akimrx     (503) staff       (20)        0 2024-03-25 11:38:05.621264 tracker-exporter-1.0.3/
--rw-r--r--   0 akimrx     (503) staff       (20)     1074 2023-10-14 19:35:29.000000 tracker-exporter-1.0.3/LICENSE
--rw-r--r--   0 akimrx     (503) staff       (20)    22359 2024-03-25 11:38:05.621366 tracker-exporter-1.0.3/PKG-INFO
--rw-r--r--   0 akimrx     (503) staff       (20)    21822 2024-03-20 10:15:23.000000 tracker-exporter-1.0.3/README.md
--rw-r--r--   0 akimrx     (503) staff       (20)      149 2023-10-19 16:45:27.000000 tracker-exporter-1.0.3/pyproject.toml
--rw-r--r--   0 akimrx     (503) staff       (20)      492 2024-03-25 11:38:05.621708 tracker-exporter-1.0.3/setup.cfg
--rw-r--r--   0 akimrx     (503) staff       (20)     1869 2023-10-17 17:04:12.000000 tracker-exporter-1.0.3/setup.py
-drwxr-xr-x   0 akimrx     (503) staff       (20)        0 2024-03-25 11:38:05.618625 tracker-exporter-1.0.3/tracker_exporter/
--rw-r--r--   0 akimrx     (503) staff       (20)      806 2023-11-08 06:53:26.000000 tracker-exporter-1.0.3/tracker_exporter/__init__.py
--rw-r--r--   0 akimrx     (503) staff       (20)      309 2024-03-25 11:36:19.000000 tracker-exporter-1.0.3/tracker_exporter/_meta.py
--rw-r--r--   0 akimrx     (503) staff       (20)      147 2023-10-17 17:04:12.000000 tracker-exporter-1.0.3/tracker_exporter/_typing.py
--rw-r--r--   0 akimrx     (503) staff       (20)     8931 2023-11-08 07:05:57.000000 tracker-exporter-1.0.3/tracker_exporter/config.py
--rw-r--r--   0 akimrx     (503) staff       (20)    11924 2024-03-25 11:33:31.000000 tracker-exporter-1.0.3/tracker_exporter/etl.py
--rw-r--r--   0 akimrx     (503) staff       (20)      413 2023-10-17 17:04:12.000000 tracker-exporter-1.0.3/tracker_exporter/exceptions.py
--rw-r--r--   0 akimrx     (503) staff       (20)     4591 2023-11-08 08:42:53.000000 tracker-exporter-1.0.3/tracker_exporter/main.py
-drwxr-xr-x   0 akimrx     (503) staff       (20)        0 2024-03-25 11:38:05.620093 tracker-exporter-1.0.3/tracker_exporter/models/
--rw-r--r--   0 akimrx     (503) staff       (20)        0 2023-10-17 16:44:08.000000 tracker-exporter-1.0.3/tracker_exporter/models/__init__.py
--rw-r--r--   0 akimrx     (503) staff       (20)     2962 2023-10-20 07:14:24.000000 tracker-exporter-1.0.3/tracker_exporter/models/base.py
--rw-r--r--   0 akimrx     (503) staff       (20)    11287 2023-10-20 07:14:24.000000 tracker-exporter-1.0.3/tracker_exporter/models/issue.py
-drwxr-xr-x   0 akimrx     (503) staff       (20)        0 2024-03-25 11:38:05.620728 tracker-exporter-1.0.3/tracker_exporter/services/
--rw-r--r--   0 akimrx     (503) staff       (20)      582 2023-10-17 17:04:12.000000 tracker-exporter-1.0.3/tracker_exporter/services/__init__.py
--rw-r--r--   0 akimrx     (503) staff       (20)     4790 2023-10-20 07:14:24.000000 tracker-exporter-1.0.3/tracker_exporter/services/clickhouse.py
--rw-r--r--   0 akimrx     (503) staff       (20)     2695 2023-10-20 07:14:24.000000 tracker-exporter-1.0.3/tracker_exporter/services/monitoring.py
--rw-r--r--   0 akimrx     (503) staff       (20)     4139 2023-10-20 07:14:24.000000 tracker-exporter-1.0.3/tracker_exporter/services/state.py
--rw-r--r--   0 akimrx     (503) staff       (20)     2581 2023-10-20 07:14:24.000000 tracker-exporter-1.0.3/tracker_exporter/services/tracker.py
-drwxr-xr-x   0 akimrx     (503) staff       (20)        0 2024-03-25 11:38:05.621093 tracker-exporter-1.0.3/tracker_exporter/utils/
--rw-r--r--   0 akimrx     (503) staff       (20)        0 2023-10-17 16:44:08.000000 tracker-exporter-1.0.3/tracker_exporter/utils/__init__.py
--rw-r--r--   0 akimrx     (503) staff       (20)    10946 2024-03-20 10:27:16.000000 tracker-exporter-1.0.3/tracker_exporter/utils/helpers.py
-drwxr-xr-x   0 akimrx     (503) staff       (20)        0 2024-03-25 11:38:05.619615 tracker-exporter-1.0.3/tracker_exporter.egg-info/
--rw-r--r--   0 akimrx     (503) staff       (20)    22359 2024-03-25 11:38:05.000000 tracker-exporter-1.0.3/tracker_exporter.egg-info/PKG-INFO
--rw-r--r--   0 akimrx     (503) staff       (20)      882 2024-03-25 11:38:05.000000 tracker-exporter-1.0.3/tracker_exporter.egg-info/SOURCES.txt
--rw-r--r--   0 akimrx     (503) staff       (20)        1 2024-03-25 11:38:05.000000 tracker-exporter-1.0.3/tracker_exporter.egg-info/dependency_links.txt
--rw-r--r--   0 akimrx     (503) staff       (20)       64 2024-03-25 11:38:05.000000 tracker-exporter-1.0.3/tracker_exporter.egg-info/entry_points.txt
--rw-r--r--   0 akimrx     (503) staff       (20)        1 2024-03-25 11:38:05.000000 tracker-exporter-1.0.3/tracker_exporter.egg-info/not-zip-safe
--rw-r--r--   0 akimrx     (503) staff       (20)      236 2024-03-25 11:38:05.000000 tracker-exporter-1.0.3/tracker_exporter.egg-info/requires.txt
--rw-r--r--   0 akimrx     (503) staff       (20)       17 2024-03-25 11:38:05.000000 tracker-exporter-1.0.3/tracker_exporter.egg-info/top_level.txt
+drwxr-xr-x   0 akimrx     (503) staff       (20)        0 2024-04-06 10:41:29.110018 tracker-exporter-2.0.0/
+-rw-r--r--   0 akimrx     (503) staff       (20)     1074 2023-10-14 19:35:29.000000 tracker-exporter-2.0.0/LICENSE
+-rw-r--r--   0 akimrx     (503) staff       (20)    28117 2024-04-06 10:41:29.110105 tracker-exporter-2.0.0/PKG-INFO
+-rw-r--r--   0 akimrx     (503) staff       (20)    27580 2024-04-06 10:37:56.000000 tracker-exporter-2.0.0/README.md
+-rw-r--r--   0 akimrx     (503) staff       (20)      149 2023-10-19 16:45:27.000000 tracker-exporter-2.0.0/pyproject.toml
+-rw-r--r--   0 akimrx     (503) staff       (20)      492 2024-04-06 10:41:29.110411 tracker-exporter-2.0.0/setup.cfg
+-rw-r--r--   0 akimrx     (503) staff       (20)     1869 2023-10-17 17:04:12.000000 tracker-exporter-2.0.0/setup.py
+drwxr-xr-x   0 akimrx     (503) staff       (20)        0 2024-04-06 10:41:29.107545 tracker-exporter-2.0.0/tracker_exporter/
+-rw-r--r--   0 akimrx     (503) staff       (20)      444 2024-04-06 10:37:56.000000 tracker-exporter-2.0.0/tracker_exporter/__init__.py
+-rw-r--r--   0 akimrx     (503) staff       (20)      309 2024-04-06 10:37:56.000000 tracker-exporter-2.0.0/tracker_exporter/_meta.py
+-rw-r--r--   0 akimrx     (503) staff       (20)      147 2023-10-17 17:04:12.000000 tracker-exporter-2.0.0/tracker_exporter/_typing.py
+-rw-r--r--   0 akimrx     (503) staff       (20)     9393 2024-04-06 10:37:56.000000 tracker-exporter-2.0.0/tracker_exporter/config.py
+-rw-r--r--   0 akimrx     (503) staff       (20)    12128 2024-04-06 10:37:56.000000 tracker-exporter-2.0.0/tracker_exporter/etl.py
+-rw-r--r--   0 akimrx     (503) staff       (20)      458 2024-04-06 10:37:56.000000 tracker-exporter-2.0.0/tracker_exporter/exceptions.py
+-rw-r--r--   0 akimrx     (503) staff       (20)     4950 2024-04-06 10:37:56.000000 tracker-exporter-2.0.0/tracker_exporter/main.py
+drwxr-xr-x   0 akimrx     (503) staff       (20)        0 2024-04-06 10:41:29.108771 tracker-exporter-2.0.0/tracker_exporter/models/
+-rw-r--r--   0 akimrx     (503) staff       (20)        0 2023-10-17 16:44:08.000000 tracker-exporter-2.0.0/tracker_exporter/models/__init__.py
+-rw-r--r--   0 akimrx     (503) staff       (20)     1845 2024-04-06 10:37:56.000000 tracker-exporter-2.0.0/tracker_exporter/models/base.py
+-rw-r--r--   0 akimrx     (503) staff       (20)    11287 2023-10-20 07:14:24.000000 tracker-exporter-2.0.0/tracker_exporter/models/issue.py
+drwxr-xr-x   0 akimrx     (503) staff       (20)        0 2024-04-06 10:41:29.109217 tracker-exporter-2.0.0/tracker_exporter/services/
+-rw-r--r--   0 akimrx     (503) staff       (20)      286 2024-04-06 10:37:56.000000 tracker-exporter-2.0.0/tracker_exporter/services/__init__.py
+-rw-r--r--   0 akimrx     (503) staff       (20)     4790 2023-10-20 07:14:24.000000 tracker-exporter-2.0.0/tracker_exporter/services/clickhouse.py
+-rw-r--r--   0 akimrx     (503) staff       (20)     2695 2023-10-20 07:14:24.000000 tracker-exporter-2.0.0/tracker_exporter/services/monitoring.py
+-rw-r--r--   0 akimrx     (503) staff       (20)     2581 2023-10-20 07:14:24.000000 tracker-exporter-2.0.0/tracker_exporter/services/tracker.py
+drwxr-xr-x   0 akimrx     (503) staff       (20)        0 2024-04-06 10:41:29.109718 tracker-exporter-2.0.0/tracker_exporter/state/
+-rw-r--r--   0 akimrx     (503) staff       (20)        0 2024-04-06 10:37:56.000000 tracker-exporter-2.0.0/tracker_exporter/state/__init__.py
+-rw-r--r--   0 akimrx     (503) staff       (20)     9173 2024-04-06 10:37:56.000000 tracker-exporter-2.0.0/tracker_exporter/state/backends.py
+-rw-r--r--   0 akimrx     (503) staff       (20)     1819 2024-04-06 10:37:56.000000 tracker-exporter-2.0.0/tracker_exporter/state/factory.py
+-rw-r--r--   0 akimrx     (503) staff       (20)     7425 2024-04-06 10:37:56.000000 tracker-exporter-2.0.0/tracker_exporter/state/managers.py
+-rw-r--r--   0 akimrx     (503) staff       (20)     2679 2024-04-06 10:37:56.000000 tracker-exporter-2.0.0/tracker_exporter/state/serializers.py
+drwxr-xr-x   0 akimrx     (503) staff       (20)        0 2024-04-06 10:41:29.109912 tracker-exporter-2.0.0/tracker_exporter/utils/
+-rw-r--r--   0 akimrx     (503) staff       (20)        0 2023-10-17 16:44:08.000000 tracker-exporter-2.0.0/tracker_exporter/utils/__init__.py
+-rw-r--r--   0 akimrx     (503) staff       (20)    10946 2024-03-20 10:27:16.000000 tracker-exporter-2.0.0/tracker_exporter/utils/helpers.py
+drwxr-xr-x   0 akimrx     (503) staff       (20)        0 2024-04-06 10:41:29.108435 tracker-exporter-2.0.0/tracker_exporter.egg-info/
+-rw-r--r--   0 akimrx     (503) staff       (20)    28117 2024-04-06 10:41:29.000000 tracker-exporter-2.0.0/tracker_exporter.egg-info/PKG-INFO
+-rw-r--r--   0 akimrx     (503) staff       (20)     1024 2024-04-06 10:41:29.000000 tracker-exporter-2.0.0/tracker_exporter.egg-info/SOURCES.txt
+-rw-r--r--   0 akimrx     (503) staff       (20)        1 2024-04-06 10:41:29.000000 tracker-exporter-2.0.0/tracker_exporter.egg-info/dependency_links.txt
+-rw-r--r--   0 akimrx     (503) staff       (20)       64 2024-04-06 10:41:29.000000 tracker-exporter-2.0.0/tracker_exporter.egg-info/entry_points.txt
+-rw-r--r--   0 akimrx     (503) staff       (20)        1 2024-04-06 10:41:29.000000 tracker-exporter-2.0.0/tracker_exporter.egg-info/not-zip-safe
+-rw-r--r--   0 akimrx     (503) staff       (20)      263 2024-04-06 10:41:29.000000 tracker-exporter-2.0.0/tracker_exporter.egg-info/requires.txt
+-rw-r--r--   0 akimrx     (503) staff       (20)       17 2024-04-06 10:41:29.000000 tracker-exporter-2.0.0/tracker_exporter.egg-info/top_level.txt
```

### Comparing `tracker-exporter-1.0.3/LICENSE` & `tracker-exporter-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tracker-exporter-1.0.3/PKG-INFO` & `tracker-exporter-2.0.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tracker-exporter
-Version: 1.0.3
+Version: 2.0.0
 Summary: Yandex.Tracker issue metrics exporter
 Home-page: https://github.com/akimrx/yandex-tracker-exporter
 Download-URL: https://pypi.org/project/tracker-exporter/
 Author: Akim Faskhutdinov
 Author-email: akimstrong@yandex.ru
 License: MIT
 Keywords: yandex tracker exporter,yandex,tracker,etl,agile,cycle time
@@ -13,30 +13,35 @@
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/tracker-exporter.svg)](https://pypi.org/project/tracker-exporter/)
 [![PyPi Package](https://img.shields.io/pypi/v/tracker-exporter.svg)](https://pypi.org/project/tracker-exporter/)
-[![Codecov](https://codecov.io/gh/akimrx/yandex-tracker-exporter/branch/master/graph/badge.svg)](https://app.codecov.io/gh/akimrx/yandex-tracker-exporter)
 [![Tests](https://github.com/akimrx/yandex-tracker-exporter/workflows/Tests/badge.svg)](https://github.com/akimrx/yandex-tracker-exporter)
 
-
 # Yandex.Tracker ETL
 
-Export issue metadata & agile metrics, transform and load to OLAP data storage. Metrics based on issue changelog.  
+Export issue metadata & agile metrics, transform and load to OLAP data storage. Metrics based on issue changelog.
 
 ⚠️ **Important**  
 **Versions 1.x.x incompatible with 0.1.x. New versions works only on Python >= 3.10**
 
 > You can fork this repository and refine the tool the way you want. Or use it as it is - this will allow you to build basic analytics on the tasks from Yandex.Tracker.
 
-Require:
-* Python `>=3.10.*`
-* Clickhouse + specific [tables](/migrations/clickhouse/) (how to run [migration](#migration))
+**Require:**
+
+- Python `>=3.10.*`
+- Clickhouse + specific [tables](/migrations/clickhouse/) (how to run [migration](#migration))
+
+**Collects:**
+
+- Issue metadata (i.e. title, author, assignee, components, tags, status, etc)
+- Issue changelog (i.e the history of all the events that occurred with the task)
+- Calculated issue metrics by status (i.e. the time spent in a particular status) like Cycle & Lead time
 
 ## Datalens Demo
 
 **[Deploy this demo dashboard to your Datalens instance](https://datalens.yandex.ru/marketplace/f2ejcgrg2h910r7cc93u)**
 
 ## What does this tool do?
 
@@ -47,25 +52,77 @@
 Sometimes he has to go to a lot of endpoints to collect what needs to be taken to the storage (that's the way Yandex.Tracker API).
 
 **Important.**
 
 By default, the exporter processes only those tasks that were changed during the sliding window specified in the `EXPORTER_TRACKER__SEARCH__RANGE` parameter.  
 So, all tasks that have activity (changes) will be uploaded to the storage. Something like eventual consistency.
 
-If you need to upload historical data that will never be updated again, you can flexibly control behavior through the [environment variables described below](#general-settings).  
+If you need to upload historical data that will never be updated again, you can flexibly control behavior through the [environment variables described below](#general-settings).
 
 Here are some recipes for a one-shot export:
+
 1. Launch a exporter with the parameter `EXPORTER_TRACKER__SEARCH__RANGE`, for example, a year ago
 2. More specifically: describe the query in the tracker's QL format using the `EXPORTER_TRACKER__SEARCH__QUERY` environment variable. This way you can export point bundles of tasks and bypass with the [Tracker's strict limit of 10,000 tasks](https://github.com/yandex/yandex_tracker_client/issues/13).
 
+Finally run exporter with `--run-once` flag.
 
-**Collects:**
-- Issue metadata (i.e. title, author, assignee, components, tags, status, etc)
-- Issue changelog (i.e the history of all the events that occurred with the task)
-- Calculated issue metrics by status (i.e. the time spent in a particular status) like Cycle & Lead time
+### Stateful mode
+
+By default, the exporter does not store the state, and as described above, it works within the sliding window. This behavior is not the most optimal, because the exporter performs repeated processing for previous tasks.
+
+The behavior can be changed by enabling stateful mode, which supports 3 backends:
+
+- Local JSON file
+- Remote JSON file (S3 object storage)
+- Redis
+
+#### Local JSON file
+
+```ini
+EXPORTER_STATEFUL=true
+
+# used for the first run to capture historical issues
+# when the previous state is not exists.
+EXPORTER_STATEFUL_INITIAL_RANGE=7d  # this is default value
+
+EXPORTER_STATE__STORAGE=jsonfile  # this is default value
+EXPORTER_STATE__JSONFILE_STRATEGY=local  # this is default value
+
+...
+```
+
+#### Remote JSON file (S3)
+
+```ini
+EXPORTER_STATEFUL=true
+EXPORTER_STATEFUL_INITIAL_RANGE=7d
+
+EXPORTER_STATE__STORAGE=jsonfile
+EXPORTER_STATE__JSONFILE_STRATEGY=s3
+
+EXPORTER_STATE__JSONFILE_S3_BUCKET=tracker-exporter-state
+EXPORTER_STATE__JSONFILE_S3_ACCESS_KEY=YCAxxxxxxxx
+EXPORTER_STATE__JSONFILE_S3_SECRET_KEY=YCxxx-xxxxxxxxxxxxxxx
+EXPORTER_STATE__JSONFILE_S3_ENDPOINT=https://storage.yandexcloud.net
+
+...
+```
+
+#### Redis
+
+```ini
+
+EXPORTER_STATEFUL=true
+EXPORTER_STATEFUL_INITIAL_RANGE=7d
+
+EXPORTER_STATE__STORAGE=redis
+EXPORTER_STATE__REDIS_DSN=redis://localhost:6379
+
+...
+```
 
 ### Cycle time calculation algorithm
 
 Currently, status metrics are calculated based on the transition between statuses (using a issue changelog). The counting algorithm will be improved.
 
 Let's imagine that the task can be, for example, only in 5 statuses:
 
@@ -76,20 +133,21 @@
 - Closed
 
 Employees start working on the task, the history of the task and the actions of employees is described below, with a correlation to the work of the exporter.
 
 1. A new task has created with the initial status `Open`, metrics are not counted.
 2. The developer has taken the task to work, the transition is `Open -> In progress`, the metric for the `Open` status has been calculated, while the current status `In progress` is not yet considered.
 3. The developer has submitted the task to testing, the transition `In progress -> Testing`, the metric for the status `In progress` has been calculated, while the current status is being `Testing` is not yet considered.
-4. QA Engineer returned the task for revision, the transition  `Testing -> In progress`, the time in the status `Testing` has been calculated, the status `In progress` has the previous metric and has not changed yet.
+4. QA Engineer returned the task for revision, the transition `Testing -> In progress`, the time in the status `Testing` has been calculated, the status `In progress` has the previous metric and has not changed yet.
 5. The task has been finalized, re-submitted to testing, the transition `In progress -> Testing`, the delta of this transition is added incrementally to the previous value of the metric `In progress`, but `Testing` has not changed yet.
-6 The task has been tested and submitted for release, the transition  `Testing -> Ready for release`, the delta of this transition is incrementally added to the previous value of the metric `Testing`, the `Ready for Release` status is not considered yet.
-7. The release is completed, the task is closed, the transition `Ready for release -> Closed`, the metric for the `Ready for Release` status is considered. **The metric of the final status of this task (`Closed`) will not be (re)calculated.**
+   6 The task has been tested and submitted for release, the transition `Testing -> Ready for release`, the delta of this transition is incrementally added to the previous value of the metric `Testing`, the `Ready for Release` status is not considered yet.
+6. The release is completed, the task is closed, the transition `Ready for release -> Closed`, the metric for the `Ready for Release` status is considered. **The metric of the final status of this task (`Closed`) will not be (re)calculated.**
 
 #### Planned improvements
+
 Consider the status metric if a transition has been made to it, even if such a status is current and the next transition has not yet been made from it. Exclude the final statuses from the innovation.
 
 ## Tech stats
 
 > Metrics based on 100,000+ constantly changing production issues
 
 - **CPU usage**: from `2%` to `10%`
@@ -103,41 +161,38 @@
 
 This is also the answer to the question why the tool is not asynchronous. Limits in the API would not allow effective use of concurrency.
 
 The processing speed of one issue depends on how many changes there are in the issue in its history. More changes means longer processing.
 
 ## Extend exported issue data by your custom fields
 
-Just declare your `main.py` module in which extended the [TrackerIssue](tracker_exporter/models/issue.py#L65) model using multiple inheritance like
+Just declare your `main.py` module in which extended the [TrackerIssue](tracker_exporter/models/issue.py#L65) model like:
 
 ```python
 
 from tracker_exporter.models.issue import TrackerIssue
 from tracker_exporter.utils.helpers import validate_resource
 from tracker_exporter import run_etl
 
 
-class CustomIssueFields:
+class ExtendedTrackerIssue(TrackerIssue):
     def __init__(self, issue: Issues) -> None:
+        super().__init__(issue)
+
         self.foo_custom_field = validate_resource(issue, "fooCustomField")
         self.bar_custom_field = validate_resource(issue, "barCustomField")
 
 
-class ExtendedTrackerIssue(TrackerIssue, CustomIssueFields):
-    def __init__(self, issue: Issues) -> None:
-        super().__init__(issue)
-        CustomIssueFields.__init__(self, issue)
-
-
 run_etl(issue_model=ExtendedTrackerIssue)
 
 ```
 
-See full example [here](examples/extended_model/main.py)
+**Don't forget about adding fields to the Clickhouse migration.**
 
+See full example with mixin [here](examples/extended_model/main.py)
 
 ## Usage
 
 ### Native
 
 #### Install from source
 
@@ -172,15 +227,14 @@
 
 Read about the settings [here](#environment-variables-settings)
 
 ```bash
 tracker-exporter --env-file /home/akimrx/tracker/.settings
 ```
 
-
 ### Docker
 
 ```bash
 
 cd yandex-tracker-exporter
 docker-compose up -d --build
 
@@ -198,127 +252,126 @@
 So, you can install Clickhouse with Proxy via [Ansible role inside project (previous versions)](https://github.com/akimrx/yandex-tracker-exporter/tree/v0.1.19/ansible).  
 Edit the inventory file `ansible/inventory/hosts.yml` and just run ansible-playbook.
 
 > **Attention:**
 > For the role to work correctly, docker must be installed on the target server.
 
 Example Clickhouse installation:
+
 ```bash
 git clone https://github.com/akimrx/yandex-tracker-exporter.git
 cd yandex-tracker-exporter
 git checkout v0.1.19
 python3 -m venv venv && source venv/bin/activate
 pip3 install -r requirements-dev.txt
 cd ansible
 ansible-playbook -i inventory/hosts.yml playbooks/clickhouse.yml --limit agile
 ```
 
 Also, you can use [this extended Clickhouse role](https://github.com/akimrx/ansible-clickhouse-role)
 
-
 ## Yandex.Cloud – Cloud Functions
 
 ![](/docs/images/agile_metrics_cloud.png)
 
 ### Create a Managed Clickhouse cluster
 
 > How to: https://cloud.yandex.com/en/docs/managed-clickhouse/operations/cluster-create
 
-* Set user for exporter, example: `agile`
-* Set a database name, example: `agile`
-* Enable `Serverless access` flag
-* For testing enable host public access
-* Enable `Access from the management console` flag
-* Run migration or manual create tables (see migration block [here](#migration), see [sql](/migrations/clickhouse/))
+- Set user for exporter, example: `agile`
+- Set a database name, example: `agile`
+- Enable `Serverless access` flag
+- For testing enable host public access
+- Enable `Access from the management console` flag
+- Run migration or manual create tables (see migration block [here](#migration), see [sql](/migrations/clickhouse/))
 
 ### Create Cloud Function
 
 > How to: https://cloud.yandex.com/en/docs/functions/quickstart/create-function/python-function-quickstart
 
-* Use Python >= 3.10
-* Copy/paste example content from `examples/serverless` ([code](/examples/serverless/))
-* Set entrypoint: `main.handler` (for code from examples)
-* Set function timeout to `600`, because the launch can be long if there are a lot of updated issues during the collection period
-* Set memory to `512MB` or more
-* Add environment variables (see variables block [here](#configuration-via-environment-variables))
+- Use Python >= 3.10
+- Copy/paste example content from `examples/serverless` ([code](/examples/serverless/))
+- Set entrypoint: `main.handler` (for code from examples)
+- Set function timeout to `600`, because the launch can be long if there are a lot of updated issues during the collection period
+- Set memory to `512MB` or more
+- Add environment variables (see variables block [here](#configuration-via-environment-variables))
+
 ```ini
 EXPORTER_TRACKER__TOKEN=XXXXXXXXXXXXXXXX
 EXPORTER_TRACKER__CLOUD_ORG_ID=123456
 EXPORTER_TRACKER__SEARCH__RANGE=2h
 EXPORTER_ENABLE__UPLOAD="true"
 EXPORTER_CLICKHOUSE__PROTO=https
 EXPORTER_CLICKHOUSE__CACERT_PATH=/etc/ssl/certs/ca-certificates.crt
 EXPORTER_CLICKHOUSE__PORT=8443
 EXPORTER_CLICKHOUSE__HOST=rc1b-xxxxxx.mdb.yandexcloud.net
 EXPORTER_CLICKHOUSE__USER=agile
 EXPORTER_CLICKHOUSE__PASSWORD=xxxx
 EXPORTER_CHANGELOG_EXPORT_ENABLED="false"
 ```
 
-* Release function
-* Run test
-* See logs
+- Release function
+- Run test
+- See logs
 
 ![](/docs/images/logs.png)
 
-
 ##### Serverless database connection without public access
+
 If you don't want to enable clickhouse public access, use service account with such permissions - `serverless.mdbProxies.user` and set environment variables below:
 
 ```bash
 EXPORTER_CLICKHOUSE__HOST=akfd3bhqk3xxxxxxxxxxx.clickhouse-proxy.serverless.yandexcloud.net
 EXPORTER_CLICKHOUSE__SERVERLESS_PROXY_ID=akfd3bhqk3xxxxxxxxxxxxx
 ```
 
 > How to create database connection: https://cloud.yandex.com/en/docs/functions/operations/database-connection
 
-Also, the `EXPORTER_CLICKHOUSE__PASSWORD` variable with service account must be replaced by IAM-token. Keep this in mind. 
+Also, the `EXPORTER_CLICKHOUSE__PASSWORD` variable with service account must be replaced by IAM-token. Keep this in mind.
 Probably, you should get it in the function code, because the IAM-token works for a limited period of time.
 
 ### Create Trigger
 
 > How to: https://cloud.yandex.com/en/docs/functions/quickstart/create-trigger/timer-quickstart
 
-* Create new trigger
-* Choose type `Timer`
-* Set interval every hour: `0 * ? * * *`
-* Select your function
-* Create serverless service account or use an existing one
-* Save trigger
-
-
-
-
+- Create new trigger
+- Choose type `Timer`
+- Set interval every hour: `0 * ? * * *`
+- Select your function
+- Create serverless service account or use an existing one
+- Save trigger
 
 # Visualization
 
 You can use any BI/observability tool for visualization, for example:
+
 - Yandex DataLens (btw, this is [opensource](https://github.com/datalens-tech/datalens)). Also see [demo set](https://datalens.yandex.ru/marketplace/f2ejcgrg2h910r7cc93u)
 - Apache Superset
 - PowerBI
 - Grafana
 
 ![](/docs/images/datalens_example.png)
 
-
 # Migration
 
 Based on [go-migrate](https://github.com/golang-migrate/migrate) tool.
 
 ## Download and install go-migrate tool
 
 ### macOS
+
 ```shell
 wget https://github.com/golang-migrate/migrate/releases/download/v4.15.2/migrate.darwin-amd64.tar.gz -O migrate.tar.gz
 
 tar xvf migrate.tar.gz
 mv migrate ~/bin
 ```
 
 ### Linux
+
 ```shell
 wget https://github.com/golang-migrate/migrate/releases/download/v4.15.2/migrate.linux-amd64.tar.gz -O migrate.tar.gz
 
 tar -xvf migrate.tar.gz
 mv migrate /usr/local/bin
 ```
 
@@ -364,117 +417,116 @@
 
 # Configuration via environment variables
 
 See config declaration [here](/tracker_exporter/config.py)
 
 ## General settings
 
-| variable | description |
-|----------|-------------|
-| `EXPORTER_STATEFUL` | Enable stateful mode. Required `EXPORTER_STATE__*` params. Default is `False` |
-| `EXPORTER_STATEFUL_INITIAL_RANGE` | Initial search range when unknown last state. Default: `1w` |
-| `EXPORTER_CHANGELOG_EXPORT_ENABLED` | Enable export all issues changelog to Clickhouse. **Can greatly slow down exports** (x5 - x10). Default is `False` |
-| `EXPORTER_LOGLEVEL` | ETL log level. Default: `info` |
-| `EXPORTER_LOG_ETL_STATS` | Enable logging transform stats every N iteration. Default is `True` |
-| `EXPORTER_LOG_ETL_STATS_EACH_N_ITER` | How many iterations must pass to log stats. Default is `100` |
-| `EXPORTER_WORKDAYS` | Workdays for calculate business time. 0 - mon, 6 - sun. Default: `[0,1,2,3,4]` |
-| `EXPORTER_BUSINESS_HOURS_START` | Business hours start for calculate business time. Default: `09:00:00` |
-| `EXPORTER_BUSINESS_HOURS_END` | Business hours end for calculate business time. Default: `22:00:00` |
-| `EXPORTER_DATETIME_RESPONSE_FORMAT` | Yandex.Tracker datetime format in responses. Default: `%Y-%m-%dT%H:%M:%S.%f%z` |
-| `EXPORTER_DATETIME_QUERY_FORMAT` | Datetime format for search queries. Default: `%Y-%m-%d %H:%M:%S` |
-| `EXPORTER_DATETIME_CLICKHOUSE_FORMAT` | Datetime format for Clickhouse. Default: `%Y-%m-%dT%H:%M:%S.%f` |
-| `EXPORTER_ETL_INTERVAL_MINUTES` | Interval between run ETL. Default: `30` (minutes) |
-| `EXPORTER_CLOSED_ISSUE_STATUSES` | Statuses for mark issue as closed. Default: `closed,rejected,resolved,cancelled,released` |
-| `EXPORTER_NOT_NULLABLE_FIELDS` | Fields that should never be null (e.g. dates). Default: all datetime fields |
+| variable                              | description                                                                                                        |
+| ------------------------------------- | ------------------------------------------------------------------------------------------------------------------ |
+| `EXPORTER_STATEFUL`                   | Enable stateful mode. Required `EXPORTER_STATE__*` params. Default is `False`                                      |
+| `EXPORTER_STATEFUL_INITIAL_RANGE`     | Initial search range when unknown last state. Default: `1w`                                                        |
+| `EXPORTER_CHANGELOG_EXPORT_ENABLED`   | Enable export all issues changelog to Clickhouse. **Can greatly slow down exports** (x5 - x10). Default is `False` |
+| `EXPORTER_LOGLEVEL`                   | ETL log level. Default: `info`                                                                                     |
+| `EXPORTER_LOG_ETL_STATS`              | Enable logging transform stats every N iteration. Default is `True`                                                |
+| `EXPORTER_LOG_ETL_STATS_EACH_N_ITER`  | How many iterations must pass to log stats. Default is `100`                                                       |
+| `EXPORTER_WORKDAYS`                   | Workdays for calculate business time. 0 - mon, 6 - sun. Default: `[0,1,2,3,4]`                                     |
+| `EXPORTER_BUSINESS_HOURS_START`       | Business hours start for calculate business time. Default: `09:00:00`                                              |
+| `EXPORTER_BUSINESS_HOURS_END`         | Business hours end for calculate business time. Default: `22:00:00`                                                |
+| `EXPORTER_DATETIME_RESPONSE_FORMAT`   | Yandex.Tracker datetime format in responses. Default: `%Y-%m-%dT%H:%M:%S.%f%z`                                     |
+| `EXPORTER_DATETIME_QUERY_FORMAT`      | Datetime format for search queries. Default: `%Y-%m-%d %H:%M:%S`                                                   |
+| `EXPORTER_DATETIME_CLICKHOUSE_FORMAT` | Datetime format for Clickhouse. Default: `%Y-%m-%dT%H:%M:%S.%f`                                                    |
+| `EXPORTER_ETL_INTERVAL_MINUTES`       | Interval between run ETL. Default: `30` (minutes)                                                                  |
+| `EXPORTER_CLOSED_ISSUE_STATUSES`      | Statuses for mark issue as closed. Default: `closed,rejected,resolved,cancelled,released`                          |
+| `EXPORTER_NOT_NULLABLE_FIELDS`        | Fields that should never be null (e.g. dates). Default: all datetime fields                                        |
 
 ## Tracker settings
 
-| variable | description |
-|----------|-------------|
-| `EXPORTER_TRACKER__LOGLEVEL` | Log level for Yandex.Tracker SDK. Default: `warning` |
-| `EXPORTER_TRACKER__TOKEN` | OAuth2 token. Required if `EXPORTER_TRACKER__IAM_TOKEN` is not passed |
-| `EXPORTER_TRACKER__ORG_ID` | Yandex360 organization ID. Required if `EXPORTER_TRACKER__CLOUD_ORG_ID` is not passed |
-| `EXPORTER_TRACKER__IAM_TOKEN` | Yandex.Cloud IAM token. Required if `EXPORTER_TRACKER__TOKEN` is not passed |
-| `EXPORTER_TRACKER__CLOUD_ORG_ID` | Yandex.Cloud organization ID. Required if `EXPORTER_TRACKER__ORG_ID` is not passed |
-| `EXPORTER_TRACKER__TIMEOUT` | Yandex.Tracker HTTP requests timeout. Default: `10` (sec) |
-| `EXPORTER_TRACKER__MAX_RETRIES` | Yandex.Tracker HTTP requests max retries. Default: `10` |
-| `EXPORTER_TRACKER__LANGUAGE` | Yandex.Tracker language. Default: `en` |
-| `EXPORTER_TRACKER__TIMEZONE` | Yandex.Tracker timezone. Default: `Europe/Moscow` |
-| `EXPORTER_TRACKER__SEARCH__QUERY` | Custom query for search issues. This variable has the highest priority and overrides other search parameters. Default is empty |
-| `EXPORTER_TRACKER__SEARCH__RANGE` | Search issues window. Has no effect in stateful mode. Default: `2h` |
-| `EXPORTER_TRACKER__SEARCH__QUEUES` | Include or exclude queues in search. Example: `DEV,SRE,!TEST,!TRASH` Default is empty (i.e. all queues) |
-| `EXPORTER_TRACKER__SEARCH__PER_PAGE_LIMIT` | Search results per page. Default: `100` |
+| variable                                   | description                                                                                                                    |
+| ------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------ |
+| `EXPORTER_TRACKER__LOGLEVEL`               | Log level for Yandex.Tracker SDK. Default: `warning`                                                                           |
+| `EXPORTER_TRACKER__TOKEN`                  | OAuth2 token. Required if `EXPORTER_TRACKER__IAM_TOKEN` is not passed                                                          |
+| `EXPORTER_TRACKER__ORG_ID`                 | Yandex360 organization ID. Required if `EXPORTER_TRACKER__CLOUD_ORG_ID` is not passed                                          |
+| `EXPORTER_TRACKER__IAM_TOKEN`              | Yandex.Cloud IAM token. Required if `EXPORTER_TRACKER__TOKEN` is not passed                                                    |
+| `EXPORTER_TRACKER__CLOUD_ORG_ID`           | Yandex.Cloud organization ID. Required if `EXPORTER_TRACKER__ORG_ID` is not passed                                             |
+| `EXPORTER_TRACKER__TIMEOUT`                | Yandex.Tracker HTTP requests timeout. Default: `10` (sec)                                                                      |
+| `EXPORTER_TRACKER__MAX_RETRIES`            | Yandex.Tracker HTTP requests max retries. Default: `10`                                                                        |
+| `EXPORTER_TRACKER__LANGUAGE`               | Yandex.Tracker language. Default: `en`                                                                                         |
+| `EXPORTER_TRACKER__TIMEZONE`               | Yandex.Tracker timezone. Default: `Europe/Moscow`                                                                              |
+| `EXPORTER_TRACKER__SEARCH__QUERY`          | Custom query for search issues. This variable has the highest priority and overrides other search parameters. Default is empty |
+| `EXPORTER_TRACKER__SEARCH__RANGE`          | Search issues window. Has no effect in stateful mode. Default: `2h`                                                            |
+| `EXPORTER_TRACKER__SEARCH__QUEUES`         | Include or exclude queues in search. Example: `DEV,SRE,!TEST,!TRASH` Default is empty (i.e. all queues)                        |
+| `EXPORTER_TRACKER__SEARCH__PER_PAGE_LIMIT` | Search results per page. Default: `100`                                                                                        |
 
 ## Clickhouse settings
 
-| variable | description |
-|----------|-------------|
-| `EXPORTER_CLICKHOUSE__ENABLE_UPLOAD` | Enable upload data to Clickhouse. Default is `True` |
-| `EXPORTER_CLICKHOUSE__HOST` | Clickhouse host. Default: `localhost` |
-| `EXPORTER_CLICKHOUSE__PROTO` | Clickhouse protocol: http or https. Default: `http` |
-| `EXPORTER_CLICKHOUSE__PORT` | Clickhouse HTTP(S) port. Default: `8123`
-| `EXPORTER_CLICKHOUSE__CACERT_PATH` | Path to CA cert. Only for HTTPS proto. Default is empty |
-| `EXPORTER_CLICKHOUSE__SERVERLESS_PROXY_ID` | Yandex Cloud Functions proxy ID. Default is empty |
-| `EXPORTER_CLICKHOUSE__USERNAME` | Clickhouse username. Default: `default` |
-| `EXPORTER_CLICKHOUSE__PASSWORD` | Clickhouse password. Can be empty. Default is empty |
-| `EXPORTER_CLICKHOUSE__DATABASE` | Clickhouse database. Default: `agile` |
-| `EXPORTER_CLICKHOUSE__ISSUES_TABLE` | Clickhouse table for issues metadata. Default: `issues` |
-| `EXPORTER_CLICKHOUSE__ISSUE_METRICS_TABLE` | Clickhouse table for issue metrics. Default: `issue_metrics` |
+| variable                                      | description                                                        |
+| --------------------------------------------- | ------------------------------------------------------------------ |
+| `EXPORTER_CLICKHOUSE__ENABLE_UPLOAD`          | Enable upload data to Clickhouse. Default is `True`                |
+| `EXPORTER_CLICKHOUSE__HOST`                   | Clickhouse host. Default: `localhost`                              |
+| `EXPORTER_CLICKHOUSE__PROTO`                  | Clickhouse protocol: http or https. Default: `http`                |
+| `EXPORTER_CLICKHOUSE__PORT`                   | Clickhouse HTTP(S) port. Default: `8123`                           |
+| `EXPORTER_CLICKHOUSE__CACERT_PATH`            | Path to CA cert. Only for HTTPS proto. Default is empty            |
+| `EXPORTER_CLICKHOUSE__SERVERLESS_PROXY_ID`    | Yandex Cloud Functions proxy ID. Default is empty                  |
+| `EXPORTER_CLICKHOUSE__USERNAME`               | Clickhouse username. Default: `default`                            |
+| `EXPORTER_CLICKHOUSE__PASSWORD`               | Clickhouse password. Can be empty. Default is empty                |
+| `EXPORTER_CLICKHOUSE__DATABASE`               | Clickhouse database. Default: `agile`                              |
+| `EXPORTER_CLICKHOUSE__ISSUES_TABLE`           | Clickhouse table for issues metadata. Default: `issues`            |
+| `EXPORTER_CLICKHOUSE__ISSUE_METRICS_TABLE`    | Clickhouse table for issue metrics. Default: `issue_metrics`       |
 | `EXPORTER_CLICKHOUSE__ISSUES_CHANGELOG_TABLE` | Clickhouse table for issues changelog. Default: `issues_changelog` |
-| `EXPORTER_CLICKHOUSE__AUTO_DEDUPLICATE` | Execute `OPTIMIZE` after each `INSERT`. Default is `True` |
-| `EXPORTER_CLICKHOUSE__BACKOFF_BASE_DELAY` | Base delay for backoff strategy. Default: `0.5` (sec) |
-| `EXPORTER_CLICKHOUSE__BACKOFF_EXPO_FACTOR` | Exponential factor for multiply every try. Default: `2.5` (sec) |
-| `EXPORTER_CLICKHOUSE__BACKOFF_MAX_TRIES` | Max tries for backoff strategy. Default: `3` |
-| `EXPORTER_CLICKHOUSE__BACKOFF_JITTER` | Enable jitter (randomize delay) for retries. Default: `True` |
+| `EXPORTER_CLICKHOUSE__AUTO_DEDUPLICATE`       | Execute `OPTIMIZE` after each `INSERT`. Default is `True`          |
+| `EXPORTER_CLICKHOUSE__BACKOFF_BASE_DELAY`     | Base delay for backoff strategy. Default: `0.5` (sec)              |
+| `EXPORTER_CLICKHOUSE__BACKOFF_EXPO_FACTOR`    | Exponential factor for multiply every try. Default: `2.5` (sec)    |
+| `EXPORTER_CLICKHOUSE__BACKOFF_MAX_TRIES`      | Max tries for backoff strategy. Default: `3`                       |
+| `EXPORTER_CLICKHOUSE__BACKOFF_JITTER`         | Enable jitter (randomize delay) for retries. Default: `True`       |
 
 ## State settings
 
-| variable | description |
-|----------|-------------|
-| `EXPORTER_STATE__STORAGE` | Storage type for StateKeeper. Can be: `jsonfile`, `redis`, `custom`. Default: `jsonfile` |
-| `EXPORTER_STATE__REDIS_DSN` | Connection string for Redis state storage when storage type is `redis`. Default is empty. |
-| `EXPORTER_STATE__JSONFILE_STRATEGY` | File store strategy for `jsonfile` storage type. Can be `s3` or `local`. Default: `local` |
-| `EXPORTER_STATE__JSONFILE_PATH` | Path to JSON state file. Default: `./state.json` |
-| `EXPORTER_STATE__JSONFILE_S3_BUCKET` | Bucket for `s3` strategy. Default is empty |
-| `EXPORTER_STATE__JSONFILE_S3_REGION` | Region for `s3` strategy. Default is `eu-east-1` |
-| `EXPORTER_STATE__JSONFILE_S3_ENDPOINT` | Endpoint URL for `s3` strategy. Default is empty |
-| `EXPORTER_STATE__JSONFILE_S3_ACCESS_KEY` | AWS access key id for `s3` strategy. Default is empty |
-| `EXPORTER_STATE__JSONFILE_S3_SECRET_KEY` | AWS secret key for `s3` strategy. Default is empty |
-| `EXPORTER_STATE__CUSTOM_STORAGE_PARAMS` | Settings for custom storage params as `dict`. Default: `{}` |
+| variable                                 | description                                                                               |
+| ---------------------------------------- | ----------------------------------------------------------------------------------------- |
+| `EXPORTER_STATE__STORAGE`                | Storage type for StateKeeper. Can be: `jsonfile`, `redis`, `custom`. Default: `jsonfile`  |
+| `EXPORTER_STATE__REDIS_DSN`              | Connection string for Redis state storage when storage type is `redis`. Default is empty. |
+| `EXPORTER_STATE__JSONFILE_STRATEGY`      | File store strategy for `jsonfile` storage type. Can be `s3` or `local`. Default: `local` |
+| `EXPORTER_STATE__JSONFILE_PATH`          | Path to JSON state file. Default: `./state.json`                                          |
+| `EXPORTER_STATE__JSONFILE_S3_BUCKET`     | Bucket for `s3` strategy. Default is empty                                                |
+| `EXPORTER_STATE__JSONFILE_S3_REGION`     | Region for `s3` strategy. Default is `us-east-1`                                          |
+| `EXPORTER_STATE__JSONFILE_S3_ENDPOINT`   | Endpoint URL for `s3` strategy. Default is empty                                          |
+| `EXPORTER_STATE__JSONFILE_S3_ACCESS_KEY` | AWS access key id for `s3` strategy. Default is empty                                     |
+| `EXPORTER_STATE__JSONFILE_S3_SECRET_KEY` | AWS secret key for `s3` strategy. Default is empty                                        |
+| `EXPORTER_STATE__CUSTOM_STORAGE_PARAMS`  | Settings for custom storage params as `dict`. Default: `{}`                               |
 
 ## Observability settings
 
-| variable | description |
-|----------|-------------|
-| `EXPORTER_MONITORING__METRICS_ENABLED` | Enable send statsd tagged metrics. Default is `False` |
-| `EXPORTER_MONITORING__METRICS_HOST` | DogStatsD / statsd host. Default: `localhost` |
-| `EXPORTER_MONITORING__METRICS_PORT` | DogStatsD / statsd port. Default: `8125` |
-| `EXPORTER_MONITORING__METRICS_BASE_PREFIX` | Prefix for metrics name. Default: `tracker_exporter` |
+| variable                                   | description                                                                  |
+| ------------------------------------------ | ---------------------------------------------------------------------------- |
+| `EXPORTER_MONITORING__METRICS_ENABLED`     | Enable send statsd tagged metrics. Default is `False`                        |
+| `EXPORTER_MONITORING__METRICS_HOST`        | DogStatsD / statsd host. Default: `localhost`                                |
+| `EXPORTER_MONITORING__METRICS_PORT`        | DogStatsD / statsd port. Default: `8125`                                     |
+| `EXPORTER_MONITORING__METRICS_BASE_PREFIX` | Prefix for metrics name. Default: `tracker_exporter`                         |
 | `EXPORTER_MONITORING__METRICS_BASE_LABELS` | List of tags for metrics. Example: `["project:internal",]`. Default is empty |
-| `EXPORTER_MONITORING__SENTRY_ENABLED` | Enable send exception stacktrace to Sentry. Default is `False` |
-| `EXPORTER_MONITORING__SENTRY_DSN` | Sentry DSN. Default is empty |
-
+| `EXPORTER_MONITORING__SENTRY_ENABLED`      | Enable send exception stacktrace to Sentry. Default is `False`               |
+| `EXPORTER_MONITORING__SENTRY_DSN`          | Sentry DSN. Default is empty                                                 |
 
 # Monitoring
 
 Based on DogStatsD tagged format. VictoriaMetrics compatible.
 
-| Metric name | Metric type | Labels | Description |
-|-------------|-------------|--------|-------------|
-| `tracker_exporter_issue_transform_time_seconds` | time | - | Duration of transform per task (data packing to the model) |
-| `tracker_exporter_issues_total_processed_count` | count | - | Total issues processed |
-| `tracker_exporter_issues_search_time_seconds` | time | - | Yandex.Tracker search duration time in seconds |
-| `tracker_exporter_issues_without_metrics` | count | - | Issues with empty metrics (no changelog) |
-| `tracker_exporter_issue_prefetch_seconds` | time | - | Pre-transform data duration in seconds |
-| `tracker_exporter_comments_fetch_seconds` | time | - | Comments fetch duration in seconds |
-| `tracker_exporter_etl_duration_seconds` | time | - | ETL full pipeline duration in seconds |
-| `tracker_exporter_etl_upload_status` | gauge | - | Last upload status, 1 - success, 2 - fail |
-| `tracker_exporter_export_and_transform_time_seconds` | time | - | Overall export and transform duration in seconds |
-| `tracker_exporter_upload_to_storage_time_seconds` | time | - | Overall insert duration time in seconds |
-| `tracker_exporter_last_update_timestamp` | gauge | - | Last data update timestamp |
-| `tracker_exporter_clickhouse_insert_time_seconds` | time | database, table | Insert per table duration time in seconds |
-| `tracker_exporter_clickhouse_inserted_rows` | count | database, table | Inserted rows per table |
-| `tracker_exporter_clickhouse_deduplicate_time_seconds` | time | database, table | Optimize execute time duration in seconds |
-
+| Metric name                                            | Metric type | Labels          | Description                                                |
+| ------------------------------------------------------ | ----------- | --------------- | ---------------------------------------------------------- |
+| `tracker_exporter_issue_transform_time_seconds`        | time        | -               | Duration of transform per task (data packing to the model) |
+| `tracker_exporter_issues_total_processed_count`        | count       | -               | Total issues processed                                     |
+| `tracker_exporter_issues_search_time_seconds`          | time        | -               | Yandex.Tracker search duration time in seconds             |
+| `tracker_exporter_issues_without_metrics`              | count       | -               | Issues with empty metrics (no changelog)                   |
+| `tracker_exporter_issue_prefetch_seconds`              | time        | -               | Pre-transform data duration in seconds                     |
+| `tracker_exporter_comments_fetch_seconds`              | time        | -               | Comments fetch duration in seconds                         |
+| `tracker_exporter_etl_duration_seconds`                | time        | -               | ETL full pipeline duration in seconds                      |
+| `tracker_exporter_etl_upload_status`                   | gauge       | -               | Last upload status, 1 - success, 2 - fail                  |
+| `tracker_exporter_export_and_transform_time_seconds`   | time        | -               | Overall export and transform duration in seconds           |
+| `tracker_exporter_upload_to_storage_time_seconds`      | time        | -               | Overall insert duration time in seconds                    |
+| `tracker_exporter_last_update_timestamp`               | gauge       | -               | Last data update timestamp                                 |
+| `tracker_exporter_clickhouse_insert_time_seconds`      | time        | database, table | Insert per table duration time in seconds                  |
+| `tracker_exporter_clickhouse_inserted_rows`            | count       | database, table | Inserted rows per table                                    |
+| `tracker_exporter_clickhouse_deduplicate_time_seconds` | time        | database, table | Optimize execute time duration in seconds                  |
 
 ### Metrics on dashboard demo
+
 ![](/docs/images/etl_metrics.jpeg)
```

### Comparing `tracker-exporter-1.0.3/README.md` & `tracker-exporter-2.0.0/tracker_exporter.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,25 +1,47 @@
+Metadata-Version: 2.1
+Name: tracker-exporter
+Version: 2.0.0
+Summary: Yandex.Tracker issue metrics exporter
+Home-page: https://github.com/akimrx/yandex-tracker-exporter
+Download-URL: https://pypi.org/project/tracker-exporter/
+Author: Akim Faskhutdinov
+Author-email: akimstrong@yandex.ru
+License: MIT
+Keywords: yandex tracker exporter,yandex,tracker,etl,agile,cycle time
+Platform: osx
+Platform: linux
+Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/tracker-exporter.svg)](https://pypi.org/project/tracker-exporter/)
 [![PyPi Package](https://img.shields.io/pypi/v/tracker-exporter.svg)](https://pypi.org/project/tracker-exporter/)
-[![Codecov](https://codecov.io/gh/akimrx/yandex-tracker-exporter/branch/master/graph/badge.svg)](https://app.codecov.io/gh/akimrx/yandex-tracker-exporter)
 [![Tests](https://github.com/akimrx/yandex-tracker-exporter/workflows/Tests/badge.svg)](https://github.com/akimrx/yandex-tracker-exporter)
 
-
 # Yandex.Tracker ETL
 
-Export issue metadata & agile metrics, transform and load to OLAP data storage. Metrics based on issue changelog.  
+Export issue metadata & agile metrics, transform and load to OLAP data storage. Metrics based on issue changelog.
 
 ⚠️ **Important**  
 **Versions 1.x.x incompatible with 0.1.x. New versions works only on Python >= 3.10**
 
 > You can fork this repository and refine the tool the way you want. Or use it as it is - this will allow you to build basic analytics on the tasks from Yandex.Tracker.
 
-Require:
-* Python `>=3.10.*`
-* Clickhouse + specific [tables](/migrations/clickhouse/) (how to run [migration](#migration))
+**Require:**
+
+- Python `>=3.10.*`
+- Clickhouse + specific [tables](/migrations/clickhouse/) (how to run [migration](#migration))
+
+**Collects:**
+
+- Issue metadata (i.e. title, author, assignee, components, tags, status, etc)
+- Issue changelog (i.e the history of all the events that occurred with the task)
+- Calculated issue metrics by status (i.e. the time spent in a particular status) like Cycle & Lead time
 
 ## Datalens Demo
 
 **[Deploy this demo dashboard to your Datalens instance](https://datalens.yandex.ru/marketplace/f2ejcgrg2h910r7cc93u)**
 
 ## What does this tool do?
 
@@ -30,25 +52,77 @@
 Sometimes he has to go to a lot of endpoints to collect what needs to be taken to the storage (that's the way Yandex.Tracker API).
 
 **Important.**
 
 By default, the exporter processes only those tasks that were changed during the sliding window specified in the `EXPORTER_TRACKER__SEARCH__RANGE` parameter.  
 So, all tasks that have activity (changes) will be uploaded to the storage. Something like eventual consistency.
 
-If you need to upload historical data that will never be updated again, you can flexibly control behavior through the [environment variables described below](#general-settings).  
+If you need to upload historical data that will never be updated again, you can flexibly control behavior through the [environment variables described below](#general-settings).
 
 Here are some recipes for a one-shot export:
+
 1. Launch a exporter with the parameter `EXPORTER_TRACKER__SEARCH__RANGE`, for example, a year ago
 2. More specifically: describe the query in the tracker's QL format using the `EXPORTER_TRACKER__SEARCH__QUERY` environment variable. This way you can export point bundles of tasks and bypass with the [Tracker's strict limit of 10,000 tasks](https://github.com/yandex/yandex_tracker_client/issues/13).
 
+Finally run exporter with `--run-once` flag.
 
-**Collects:**
-- Issue metadata (i.e. title, author, assignee, components, tags, status, etc)
-- Issue changelog (i.e the history of all the events that occurred with the task)
-- Calculated issue metrics by status (i.e. the time spent in a particular status) like Cycle & Lead time
+### Stateful mode
+
+By default, the exporter does not store the state, and as described above, it works within the sliding window. This behavior is not the most optimal, because the exporter performs repeated processing for previous tasks.
+
+The behavior can be changed by enabling stateful mode, which supports 3 backends:
+
+- Local JSON file
+- Remote JSON file (S3 object storage)
+- Redis
+
+#### Local JSON file
+
+```ini
+EXPORTER_STATEFUL=true
+
+# used for the first run to capture historical issues
+# when the previous state is not exists.
+EXPORTER_STATEFUL_INITIAL_RANGE=7d  # this is default value
+
+EXPORTER_STATE__STORAGE=jsonfile  # this is default value
+EXPORTER_STATE__JSONFILE_STRATEGY=local  # this is default value
+
+...
+```
+
+#### Remote JSON file (S3)
+
+```ini
+EXPORTER_STATEFUL=true
+EXPORTER_STATEFUL_INITIAL_RANGE=7d
+
+EXPORTER_STATE__STORAGE=jsonfile
+EXPORTER_STATE__JSONFILE_STRATEGY=s3
+
+EXPORTER_STATE__JSONFILE_S3_BUCKET=tracker-exporter-state
+EXPORTER_STATE__JSONFILE_S3_ACCESS_KEY=YCAxxxxxxxx
+EXPORTER_STATE__JSONFILE_S3_SECRET_KEY=YCxxx-xxxxxxxxxxxxxxx
+EXPORTER_STATE__JSONFILE_S3_ENDPOINT=https://storage.yandexcloud.net
+
+...
+```
+
+#### Redis
+
+```ini
+
+EXPORTER_STATEFUL=true
+EXPORTER_STATEFUL_INITIAL_RANGE=7d
+
+EXPORTER_STATE__STORAGE=redis
+EXPORTER_STATE__REDIS_DSN=redis://localhost:6379
+
+...
+```
 
 ### Cycle time calculation algorithm
 
 Currently, status metrics are calculated based on the transition between statuses (using a issue changelog). The counting algorithm will be improved.
 
 Let's imagine that the task can be, for example, only in 5 statuses:
 
@@ -59,20 +133,21 @@
 - Closed
 
 Employees start working on the task, the history of the task and the actions of employees is described below, with a correlation to the work of the exporter.
 
 1. A new task has created with the initial status `Open`, metrics are not counted.
 2. The developer has taken the task to work, the transition is `Open -> In progress`, the metric for the `Open` status has been calculated, while the current status `In progress` is not yet considered.
 3. The developer has submitted the task to testing, the transition `In progress -> Testing`, the metric for the status `In progress` has been calculated, while the current status is being `Testing` is not yet considered.
-4. QA Engineer returned the task for revision, the transition  `Testing -> In progress`, the time in the status `Testing` has been calculated, the status `In progress` has the previous metric and has not changed yet.
+4. QA Engineer returned the task for revision, the transition `Testing -> In progress`, the time in the status `Testing` has been calculated, the status `In progress` has the previous metric and has not changed yet.
 5. The task has been finalized, re-submitted to testing, the transition `In progress -> Testing`, the delta of this transition is added incrementally to the previous value of the metric `In progress`, but `Testing` has not changed yet.
-6 The task has been tested and submitted for release, the transition  `Testing -> Ready for release`, the delta of this transition is incrementally added to the previous value of the metric `Testing`, the `Ready for Release` status is not considered yet.
-7. The release is completed, the task is closed, the transition `Ready for release -> Closed`, the metric for the `Ready for Release` status is considered. **The metric of the final status of this task (`Closed`) will not be (re)calculated.**
+   6 The task has been tested and submitted for release, the transition `Testing -> Ready for release`, the delta of this transition is incrementally added to the previous value of the metric `Testing`, the `Ready for Release` status is not considered yet.
+6. The release is completed, the task is closed, the transition `Ready for release -> Closed`, the metric for the `Ready for Release` status is considered. **The metric of the final status of this task (`Closed`) will not be (re)calculated.**
 
 #### Planned improvements
+
 Consider the status metric if a transition has been made to it, even if such a status is current and the next transition has not yet been made from it. Exclude the final statuses from the innovation.
 
 ## Tech stats
 
 > Metrics based on 100,000+ constantly changing production issues
 
 - **CPU usage**: from `2%` to `10%`
@@ -86,41 +161,38 @@
 
 This is also the answer to the question why the tool is not asynchronous. Limits in the API would not allow effective use of concurrency.
 
 The processing speed of one issue depends on how many changes there are in the issue in its history. More changes means longer processing.
 
 ## Extend exported issue data by your custom fields
 
-Just declare your `main.py` module in which extended the [TrackerIssue](tracker_exporter/models/issue.py#L65) model using multiple inheritance like
+Just declare your `main.py` module in which extended the [TrackerIssue](tracker_exporter/models/issue.py#L65) model like:
 
 ```python
 
 from tracker_exporter.models.issue import TrackerIssue
 from tracker_exporter.utils.helpers import validate_resource
 from tracker_exporter import run_etl
 
 
-class CustomIssueFields:
+class ExtendedTrackerIssue(TrackerIssue):
     def __init__(self, issue: Issues) -> None:
+        super().__init__(issue)
+
         self.foo_custom_field = validate_resource(issue, "fooCustomField")
         self.bar_custom_field = validate_resource(issue, "barCustomField")
 
 
-class ExtendedTrackerIssue(TrackerIssue, CustomIssueFields):
-    def __init__(self, issue: Issues) -> None:
-        super().__init__(issue)
-        CustomIssueFields.__init__(self, issue)
-
-
 run_etl(issue_model=ExtendedTrackerIssue)
 
 ```
 
-See full example [here](examples/extended_model/main.py)
+**Don't forget about adding fields to the Clickhouse migration.**
 
+See full example with mixin [here](examples/extended_model/main.py)
 
 ## Usage
 
 ### Native
 
 #### Install from source
 
@@ -155,15 +227,14 @@
 
 Read about the settings [here](#environment-variables-settings)
 
 ```bash
 tracker-exporter --env-file /home/akimrx/tracker/.settings
 ```
 
-
 ### Docker
 
 ```bash
 
 cd yandex-tracker-exporter
 docker-compose up -d --build
 
@@ -181,127 +252,126 @@
 So, you can install Clickhouse with Proxy via [Ansible role inside project (previous versions)](https://github.com/akimrx/yandex-tracker-exporter/tree/v0.1.19/ansible).  
 Edit the inventory file `ansible/inventory/hosts.yml` and just run ansible-playbook.
 
 > **Attention:**
 > For the role to work correctly, docker must be installed on the target server.
 
 Example Clickhouse installation:
+
 ```bash
 git clone https://github.com/akimrx/yandex-tracker-exporter.git
 cd yandex-tracker-exporter
 git checkout v0.1.19
 python3 -m venv venv && source venv/bin/activate
 pip3 install -r requirements-dev.txt
 cd ansible
 ansible-playbook -i inventory/hosts.yml playbooks/clickhouse.yml --limit agile
 ```
 
 Also, you can use [this extended Clickhouse role](https://github.com/akimrx/ansible-clickhouse-role)
 
-
 ## Yandex.Cloud – Cloud Functions
 
 ![](/docs/images/agile_metrics_cloud.png)
 
 ### Create a Managed Clickhouse cluster
 
 > How to: https://cloud.yandex.com/en/docs/managed-clickhouse/operations/cluster-create
 
-* Set user for exporter, example: `agile`
-* Set a database name, example: `agile`
-* Enable `Serverless access` flag
-* For testing enable host public access
-* Enable `Access from the management console` flag
-* Run migration or manual create tables (see migration block [here](#migration), see [sql](/migrations/clickhouse/))
+- Set user for exporter, example: `agile`
+- Set a database name, example: `agile`
+- Enable `Serverless access` flag
+- For testing enable host public access
+- Enable `Access from the management console` flag
+- Run migration or manual create tables (see migration block [here](#migration), see [sql](/migrations/clickhouse/))
 
 ### Create Cloud Function
 
 > How to: https://cloud.yandex.com/en/docs/functions/quickstart/create-function/python-function-quickstart
 
-* Use Python >= 3.10
-* Copy/paste example content from `examples/serverless` ([code](/examples/serverless/))
-* Set entrypoint: `main.handler` (for code from examples)
-* Set function timeout to `600`, because the launch can be long if there are a lot of updated issues during the collection period
-* Set memory to `512MB` or more
-* Add environment variables (see variables block [here](#configuration-via-environment-variables))
+- Use Python >= 3.10
+- Copy/paste example content from `examples/serverless` ([code](/examples/serverless/))
+- Set entrypoint: `main.handler` (for code from examples)
+- Set function timeout to `600`, because the launch can be long if there are a lot of updated issues during the collection period
+- Set memory to `512MB` or more
+- Add environment variables (see variables block [here](#configuration-via-environment-variables))
+
 ```ini
 EXPORTER_TRACKER__TOKEN=XXXXXXXXXXXXXXXX
 EXPORTER_TRACKER__CLOUD_ORG_ID=123456
 EXPORTER_TRACKER__SEARCH__RANGE=2h
 EXPORTER_ENABLE__UPLOAD="true"
 EXPORTER_CLICKHOUSE__PROTO=https
 EXPORTER_CLICKHOUSE__CACERT_PATH=/etc/ssl/certs/ca-certificates.crt
 EXPORTER_CLICKHOUSE__PORT=8443
 EXPORTER_CLICKHOUSE__HOST=rc1b-xxxxxx.mdb.yandexcloud.net
 EXPORTER_CLICKHOUSE__USER=agile
 EXPORTER_CLICKHOUSE__PASSWORD=xxxx
 EXPORTER_CHANGELOG_EXPORT_ENABLED="false"
 ```
 
-* Release function
-* Run test
-* See logs
+- Release function
+- Run test
+- See logs
 
 ![](/docs/images/logs.png)
 
-
 ##### Serverless database connection without public access
+
 If you don't want to enable clickhouse public access, use service account with such permissions - `serverless.mdbProxies.user` and set environment variables below:
 
 ```bash
 EXPORTER_CLICKHOUSE__HOST=akfd3bhqk3xxxxxxxxxxx.clickhouse-proxy.serverless.yandexcloud.net
 EXPORTER_CLICKHOUSE__SERVERLESS_PROXY_ID=akfd3bhqk3xxxxxxxxxxxxx
 ```
 
 > How to create database connection: https://cloud.yandex.com/en/docs/functions/operations/database-connection
 
-Also, the `EXPORTER_CLICKHOUSE__PASSWORD` variable with service account must be replaced by IAM-token. Keep this in mind. 
+Also, the `EXPORTER_CLICKHOUSE__PASSWORD` variable with service account must be replaced by IAM-token. Keep this in mind.
 Probably, you should get it in the function code, because the IAM-token works for a limited period of time.
 
 ### Create Trigger
 
 > How to: https://cloud.yandex.com/en/docs/functions/quickstart/create-trigger/timer-quickstart
 
-* Create new trigger
-* Choose type `Timer`
-* Set interval every hour: `0 * ? * * *`
-* Select your function
-* Create serverless service account or use an existing one
-* Save trigger
-
-
-
-
+- Create new trigger
+- Choose type `Timer`
+- Set interval every hour: `0 * ? * * *`
+- Select your function
+- Create serverless service account or use an existing one
+- Save trigger
 
 # Visualization
 
 You can use any BI/observability tool for visualization, for example:
+
 - Yandex DataLens (btw, this is [opensource](https://github.com/datalens-tech/datalens)). Also see [demo set](https://datalens.yandex.ru/marketplace/f2ejcgrg2h910r7cc93u)
 - Apache Superset
 - PowerBI
 - Grafana
 
 ![](/docs/images/datalens_example.png)
 
-
 # Migration
 
 Based on [go-migrate](https://github.com/golang-migrate/migrate) tool.
 
 ## Download and install go-migrate tool
 
 ### macOS
+
 ```shell
 wget https://github.com/golang-migrate/migrate/releases/download/v4.15.2/migrate.darwin-amd64.tar.gz -O migrate.tar.gz
 
 tar xvf migrate.tar.gz
 mv migrate ~/bin
 ```
 
 ### Linux
+
 ```shell
 wget https://github.com/golang-migrate/migrate/releases/download/v4.15.2/migrate.linux-amd64.tar.gz -O migrate.tar.gz
 
 tar -xvf migrate.tar.gz
 mv migrate /usr/local/bin
 ```
 
@@ -347,117 +417,116 @@
 
 # Configuration via environment variables
 
 See config declaration [here](/tracker_exporter/config.py)
 
 ## General settings
 
-| variable | description |
-|----------|-------------|
-| `EXPORTER_STATEFUL` | Enable stateful mode. Required `EXPORTER_STATE__*` params. Default is `False` |
-| `EXPORTER_STATEFUL_INITIAL_RANGE` | Initial search range when unknown last state. Default: `1w` |
-| `EXPORTER_CHANGELOG_EXPORT_ENABLED` | Enable export all issues changelog to Clickhouse. **Can greatly slow down exports** (x5 - x10). Default is `False` |
-| `EXPORTER_LOGLEVEL` | ETL log level. Default: `info` |
-| `EXPORTER_LOG_ETL_STATS` | Enable logging transform stats every N iteration. Default is `True` |
-| `EXPORTER_LOG_ETL_STATS_EACH_N_ITER` | How many iterations must pass to log stats. Default is `100` |
-| `EXPORTER_WORKDAYS` | Workdays for calculate business time. 0 - mon, 6 - sun. Default: `[0,1,2,3,4]` |
-| `EXPORTER_BUSINESS_HOURS_START` | Business hours start for calculate business time. Default: `09:00:00` |
-| `EXPORTER_BUSINESS_HOURS_END` | Business hours end for calculate business time. Default: `22:00:00` |
-| `EXPORTER_DATETIME_RESPONSE_FORMAT` | Yandex.Tracker datetime format in responses. Default: `%Y-%m-%dT%H:%M:%S.%f%z` |
-| `EXPORTER_DATETIME_QUERY_FORMAT` | Datetime format for search queries. Default: `%Y-%m-%d %H:%M:%S` |
-| `EXPORTER_DATETIME_CLICKHOUSE_FORMAT` | Datetime format for Clickhouse. Default: `%Y-%m-%dT%H:%M:%S.%f` |
-| `EXPORTER_ETL_INTERVAL_MINUTES` | Interval between run ETL. Default: `30` (minutes) |
-| `EXPORTER_CLOSED_ISSUE_STATUSES` | Statuses for mark issue as closed. Default: `closed,rejected,resolved,cancelled,released` |
-| `EXPORTER_NOT_NULLABLE_FIELDS` | Fields that should never be null (e.g. dates). Default: all datetime fields |
+| variable                              | description                                                                                                        |
+| ------------------------------------- | ------------------------------------------------------------------------------------------------------------------ |
+| `EXPORTER_STATEFUL`                   | Enable stateful mode. Required `EXPORTER_STATE__*` params. Default is `False`                                      |
+| `EXPORTER_STATEFUL_INITIAL_RANGE`     | Initial search range when unknown last state. Default: `1w`                                                        |
+| `EXPORTER_CHANGELOG_EXPORT_ENABLED`   | Enable export all issues changelog to Clickhouse. **Can greatly slow down exports** (x5 - x10). Default is `False` |
+| `EXPORTER_LOGLEVEL`                   | ETL log level. Default: `info`                                                                                     |
+| `EXPORTER_LOG_ETL_STATS`              | Enable logging transform stats every N iteration. Default is `True`                                                |
+| `EXPORTER_LOG_ETL_STATS_EACH_N_ITER`  | How many iterations must pass to log stats. Default is `100`                                                       |
+| `EXPORTER_WORKDAYS`                   | Workdays for calculate business time. 0 - mon, 6 - sun. Default: `[0,1,2,3,4]`                                     |
+| `EXPORTER_BUSINESS_HOURS_START`       | Business hours start for calculate business time. Default: `09:00:00`                                              |
+| `EXPORTER_BUSINESS_HOURS_END`         | Business hours end for calculate business time. Default: `22:00:00`                                                |
+| `EXPORTER_DATETIME_RESPONSE_FORMAT`   | Yandex.Tracker datetime format in responses. Default: `%Y-%m-%dT%H:%M:%S.%f%z`                                     |
+| `EXPORTER_DATETIME_QUERY_FORMAT`      | Datetime format for search queries. Default: `%Y-%m-%d %H:%M:%S`                                                   |
+| `EXPORTER_DATETIME_CLICKHOUSE_FORMAT` | Datetime format for Clickhouse. Default: `%Y-%m-%dT%H:%M:%S.%f`                                                    |
+| `EXPORTER_ETL_INTERVAL_MINUTES`       | Interval between run ETL. Default: `30` (minutes)                                                                  |
+| `EXPORTER_CLOSED_ISSUE_STATUSES`      | Statuses for mark issue as closed. Default: `closed,rejected,resolved,cancelled,released`                          |
+| `EXPORTER_NOT_NULLABLE_FIELDS`        | Fields that should never be null (e.g. dates). Default: all datetime fields                                        |
 
 ## Tracker settings
 
-| variable | description |
-|----------|-------------|
-| `EXPORTER_TRACKER__LOGLEVEL` | Log level for Yandex.Tracker SDK. Default: `warning` |
-| `EXPORTER_TRACKER__TOKEN` | OAuth2 token. Required if `EXPORTER_TRACKER__IAM_TOKEN` is not passed |
-| `EXPORTER_TRACKER__ORG_ID` | Yandex360 organization ID. Required if `EXPORTER_TRACKER__CLOUD_ORG_ID` is not passed |
-| `EXPORTER_TRACKER__IAM_TOKEN` | Yandex.Cloud IAM token. Required if `EXPORTER_TRACKER__TOKEN` is not passed |
-| `EXPORTER_TRACKER__CLOUD_ORG_ID` | Yandex.Cloud organization ID. Required if `EXPORTER_TRACKER__ORG_ID` is not passed |
-| `EXPORTER_TRACKER__TIMEOUT` | Yandex.Tracker HTTP requests timeout. Default: `10` (sec) |
-| `EXPORTER_TRACKER__MAX_RETRIES` | Yandex.Tracker HTTP requests max retries. Default: `10` |
-| `EXPORTER_TRACKER__LANGUAGE` | Yandex.Tracker language. Default: `en` |
-| `EXPORTER_TRACKER__TIMEZONE` | Yandex.Tracker timezone. Default: `Europe/Moscow` |
-| `EXPORTER_TRACKER__SEARCH__QUERY` | Custom query for search issues. This variable has the highest priority and overrides other search parameters. Default is empty |
-| `EXPORTER_TRACKER__SEARCH__RANGE` | Search issues window. Has no effect in stateful mode. Default: `2h` |
-| `EXPORTER_TRACKER__SEARCH__QUEUES` | Include or exclude queues in search. Example: `DEV,SRE,!TEST,!TRASH` Default is empty (i.e. all queues) |
-| `EXPORTER_TRACKER__SEARCH__PER_PAGE_LIMIT` | Search results per page. Default: `100` |
+| variable                                   | description                                                                                                                    |
+| ------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------ |
+| `EXPORTER_TRACKER__LOGLEVEL`               | Log level for Yandex.Tracker SDK. Default: `warning`                                                                           |
+| `EXPORTER_TRACKER__TOKEN`                  | OAuth2 token. Required if `EXPORTER_TRACKER__IAM_TOKEN` is not passed                                                          |
+| `EXPORTER_TRACKER__ORG_ID`                 | Yandex360 organization ID. Required if `EXPORTER_TRACKER__CLOUD_ORG_ID` is not passed                                          |
+| `EXPORTER_TRACKER__IAM_TOKEN`              | Yandex.Cloud IAM token. Required if `EXPORTER_TRACKER__TOKEN` is not passed                                                    |
+| `EXPORTER_TRACKER__CLOUD_ORG_ID`           | Yandex.Cloud organization ID. Required if `EXPORTER_TRACKER__ORG_ID` is not passed                                             |
+| `EXPORTER_TRACKER__TIMEOUT`                | Yandex.Tracker HTTP requests timeout. Default: `10` (sec)                                                                      |
+| `EXPORTER_TRACKER__MAX_RETRIES`            | Yandex.Tracker HTTP requests max retries. Default: `10`                                                                        |
+| `EXPORTER_TRACKER__LANGUAGE`               | Yandex.Tracker language. Default: `en`                                                                                         |
+| `EXPORTER_TRACKER__TIMEZONE`               | Yandex.Tracker timezone. Default: `Europe/Moscow`                                                                              |
+| `EXPORTER_TRACKER__SEARCH__QUERY`          | Custom query for search issues. This variable has the highest priority and overrides other search parameters. Default is empty |
+| `EXPORTER_TRACKER__SEARCH__RANGE`          | Search issues window. Has no effect in stateful mode. Default: `2h`                                                            |
+| `EXPORTER_TRACKER__SEARCH__QUEUES`         | Include or exclude queues in search. Example: `DEV,SRE,!TEST,!TRASH` Default is empty (i.e. all queues)                        |
+| `EXPORTER_TRACKER__SEARCH__PER_PAGE_LIMIT` | Search results per page. Default: `100`                                                                                        |
 
 ## Clickhouse settings
 
-| variable | description |
-|----------|-------------|
-| `EXPORTER_CLICKHOUSE__ENABLE_UPLOAD` | Enable upload data to Clickhouse. Default is `True` |
-| `EXPORTER_CLICKHOUSE__HOST` | Clickhouse host. Default: `localhost` |
-| `EXPORTER_CLICKHOUSE__PROTO` | Clickhouse protocol: http or https. Default: `http` |
-| `EXPORTER_CLICKHOUSE__PORT` | Clickhouse HTTP(S) port. Default: `8123`
-| `EXPORTER_CLICKHOUSE__CACERT_PATH` | Path to CA cert. Only for HTTPS proto. Default is empty |
-| `EXPORTER_CLICKHOUSE__SERVERLESS_PROXY_ID` | Yandex Cloud Functions proxy ID. Default is empty |
-| `EXPORTER_CLICKHOUSE__USERNAME` | Clickhouse username. Default: `default` |
-| `EXPORTER_CLICKHOUSE__PASSWORD` | Clickhouse password. Can be empty. Default is empty |
-| `EXPORTER_CLICKHOUSE__DATABASE` | Clickhouse database. Default: `agile` |
-| `EXPORTER_CLICKHOUSE__ISSUES_TABLE` | Clickhouse table for issues metadata. Default: `issues` |
-| `EXPORTER_CLICKHOUSE__ISSUE_METRICS_TABLE` | Clickhouse table for issue metrics. Default: `issue_metrics` |
+| variable                                      | description                                                        |
+| --------------------------------------------- | ------------------------------------------------------------------ |
+| `EXPORTER_CLICKHOUSE__ENABLE_UPLOAD`          | Enable upload data to Clickhouse. Default is `True`                |
+| `EXPORTER_CLICKHOUSE__HOST`                   | Clickhouse host. Default: `localhost`                              |
+| `EXPORTER_CLICKHOUSE__PROTO`                  | Clickhouse protocol: http or https. Default: `http`                |
+| `EXPORTER_CLICKHOUSE__PORT`                   | Clickhouse HTTP(S) port. Default: `8123`                           |
+| `EXPORTER_CLICKHOUSE__CACERT_PATH`            | Path to CA cert. Only for HTTPS proto. Default is empty            |
+| `EXPORTER_CLICKHOUSE__SERVERLESS_PROXY_ID`    | Yandex Cloud Functions proxy ID. Default is empty                  |
+| `EXPORTER_CLICKHOUSE__USERNAME`               | Clickhouse username. Default: `default`                            |
+| `EXPORTER_CLICKHOUSE__PASSWORD`               | Clickhouse password. Can be empty. Default is empty                |
+| `EXPORTER_CLICKHOUSE__DATABASE`               | Clickhouse database. Default: `agile`                              |
+| `EXPORTER_CLICKHOUSE__ISSUES_TABLE`           | Clickhouse table for issues metadata. Default: `issues`            |
+| `EXPORTER_CLICKHOUSE__ISSUE_METRICS_TABLE`    | Clickhouse table for issue metrics. Default: `issue_metrics`       |
 | `EXPORTER_CLICKHOUSE__ISSUES_CHANGELOG_TABLE` | Clickhouse table for issues changelog. Default: `issues_changelog` |
-| `EXPORTER_CLICKHOUSE__AUTO_DEDUPLICATE` | Execute `OPTIMIZE` after each `INSERT`. Default is `True` |
-| `EXPORTER_CLICKHOUSE__BACKOFF_BASE_DELAY` | Base delay for backoff strategy. Default: `0.5` (sec) |
-| `EXPORTER_CLICKHOUSE__BACKOFF_EXPO_FACTOR` | Exponential factor for multiply every try. Default: `2.5` (sec) |
-| `EXPORTER_CLICKHOUSE__BACKOFF_MAX_TRIES` | Max tries for backoff strategy. Default: `3` |
-| `EXPORTER_CLICKHOUSE__BACKOFF_JITTER` | Enable jitter (randomize delay) for retries. Default: `True` |
+| `EXPORTER_CLICKHOUSE__AUTO_DEDUPLICATE`       | Execute `OPTIMIZE` after each `INSERT`. Default is `True`          |
+| `EXPORTER_CLICKHOUSE__BACKOFF_BASE_DELAY`     | Base delay for backoff strategy. Default: `0.5` (sec)              |
+| `EXPORTER_CLICKHOUSE__BACKOFF_EXPO_FACTOR`    | Exponential factor for multiply every try. Default: `2.5` (sec)    |
+| `EXPORTER_CLICKHOUSE__BACKOFF_MAX_TRIES`      | Max tries for backoff strategy. Default: `3`                       |
+| `EXPORTER_CLICKHOUSE__BACKOFF_JITTER`         | Enable jitter (randomize delay) for retries. Default: `True`       |
 
 ## State settings
 
-| variable | description |
-|----------|-------------|
-| `EXPORTER_STATE__STORAGE` | Storage type for StateKeeper. Can be: `jsonfile`, `redis`, `custom`. Default: `jsonfile` |
-| `EXPORTER_STATE__REDIS_DSN` | Connection string for Redis state storage when storage type is `redis`. Default is empty. |
-| `EXPORTER_STATE__JSONFILE_STRATEGY` | File store strategy for `jsonfile` storage type. Can be `s3` or `local`. Default: `local` |
-| `EXPORTER_STATE__JSONFILE_PATH` | Path to JSON state file. Default: `./state.json` |
-| `EXPORTER_STATE__JSONFILE_S3_BUCKET` | Bucket for `s3` strategy. Default is empty |
-| `EXPORTER_STATE__JSONFILE_S3_REGION` | Region for `s3` strategy. Default is `eu-east-1` |
-| `EXPORTER_STATE__JSONFILE_S3_ENDPOINT` | Endpoint URL for `s3` strategy. Default is empty |
-| `EXPORTER_STATE__JSONFILE_S3_ACCESS_KEY` | AWS access key id for `s3` strategy. Default is empty |
-| `EXPORTER_STATE__JSONFILE_S3_SECRET_KEY` | AWS secret key for `s3` strategy. Default is empty |
-| `EXPORTER_STATE__CUSTOM_STORAGE_PARAMS` | Settings for custom storage params as `dict`. Default: `{}` |
+| variable                                 | description                                                                               |
+| ---------------------------------------- | ----------------------------------------------------------------------------------------- |
+| `EXPORTER_STATE__STORAGE`                | Storage type for StateKeeper. Can be: `jsonfile`, `redis`, `custom`. Default: `jsonfile`  |
+| `EXPORTER_STATE__REDIS_DSN`              | Connection string for Redis state storage when storage type is `redis`. Default is empty. |
+| `EXPORTER_STATE__JSONFILE_STRATEGY`      | File store strategy for `jsonfile` storage type. Can be `s3` or `local`. Default: `local` |
+| `EXPORTER_STATE__JSONFILE_PATH`          | Path to JSON state file. Default: `./state.json`                                          |
+| `EXPORTER_STATE__JSONFILE_S3_BUCKET`     | Bucket for `s3` strategy. Default is empty                                                |
+| `EXPORTER_STATE__JSONFILE_S3_REGION`     | Region for `s3` strategy. Default is `us-east-1`                                          |
+| `EXPORTER_STATE__JSONFILE_S3_ENDPOINT`   | Endpoint URL for `s3` strategy. Default is empty                                          |
+| `EXPORTER_STATE__JSONFILE_S3_ACCESS_KEY` | AWS access key id for `s3` strategy. Default is empty                                     |
+| `EXPORTER_STATE__JSONFILE_S3_SECRET_KEY` | AWS secret key for `s3` strategy. Default is empty                                        |
+| `EXPORTER_STATE__CUSTOM_STORAGE_PARAMS`  | Settings for custom storage params as `dict`. Default: `{}`                               |
 
 ## Observability settings
 
-| variable | description |
-|----------|-------------|
-| `EXPORTER_MONITORING__METRICS_ENABLED` | Enable send statsd tagged metrics. Default is `False` |
-| `EXPORTER_MONITORING__METRICS_HOST` | DogStatsD / statsd host. Default: `localhost` |
-| `EXPORTER_MONITORING__METRICS_PORT` | DogStatsD / statsd port. Default: `8125` |
-| `EXPORTER_MONITORING__METRICS_BASE_PREFIX` | Prefix for metrics name. Default: `tracker_exporter` |
+| variable                                   | description                                                                  |
+| ------------------------------------------ | ---------------------------------------------------------------------------- |
+| `EXPORTER_MONITORING__METRICS_ENABLED`     | Enable send statsd tagged metrics. Default is `False`                        |
+| `EXPORTER_MONITORING__METRICS_HOST`        | DogStatsD / statsd host. Default: `localhost`                                |
+| `EXPORTER_MONITORING__METRICS_PORT`        | DogStatsD / statsd port. Default: `8125`                                     |
+| `EXPORTER_MONITORING__METRICS_BASE_PREFIX` | Prefix for metrics name. Default: `tracker_exporter`                         |
 | `EXPORTER_MONITORING__METRICS_BASE_LABELS` | List of tags for metrics. Example: `["project:internal",]`. Default is empty |
-| `EXPORTER_MONITORING__SENTRY_ENABLED` | Enable send exception stacktrace to Sentry. Default is `False` |
-| `EXPORTER_MONITORING__SENTRY_DSN` | Sentry DSN. Default is empty |
-
+| `EXPORTER_MONITORING__SENTRY_ENABLED`      | Enable send exception stacktrace to Sentry. Default is `False`               |
+| `EXPORTER_MONITORING__SENTRY_DSN`          | Sentry DSN. Default is empty                                                 |
 
 # Monitoring
 
 Based on DogStatsD tagged format. VictoriaMetrics compatible.
 
-| Metric name | Metric type | Labels | Description |
-|-------------|-------------|--------|-------------|
-| `tracker_exporter_issue_transform_time_seconds` | time | - | Duration of transform per task (data packing to the model) |
-| `tracker_exporter_issues_total_processed_count` | count | - | Total issues processed |
-| `tracker_exporter_issues_search_time_seconds` | time | - | Yandex.Tracker search duration time in seconds |
-| `tracker_exporter_issues_without_metrics` | count | - | Issues with empty metrics (no changelog) |
-| `tracker_exporter_issue_prefetch_seconds` | time | - | Pre-transform data duration in seconds |
-| `tracker_exporter_comments_fetch_seconds` | time | - | Comments fetch duration in seconds |
-| `tracker_exporter_etl_duration_seconds` | time | - | ETL full pipeline duration in seconds |
-| `tracker_exporter_etl_upload_status` | gauge | - | Last upload status, 1 - success, 2 - fail |
-| `tracker_exporter_export_and_transform_time_seconds` | time | - | Overall export and transform duration in seconds |
-| `tracker_exporter_upload_to_storage_time_seconds` | time | - | Overall insert duration time in seconds |
-| `tracker_exporter_last_update_timestamp` | gauge | - | Last data update timestamp |
-| `tracker_exporter_clickhouse_insert_time_seconds` | time | database, table | Insert per table duration time in seconds |
-| `tracker_exporter_clickhouse_inserted_rows` | count | database, table | Inserted rows per table |
-| `tracker_exporter_clickhouse_deduplicate_time_seconds` | time | database, table | Optimize execute time duration in seconds |
-
+| Metric name                                            | Metric type | Labels          | Description                                                |
+| ------------------------------------------------------ | ----------- | --------------- | ---------------------------------------------------------- |
+| `tracker_exporter_issue_transform_time_seconds`        | time        | -               | Duration of transform per task (data packing to the model) |
+| `tracker_exporter_issues_total_processed_count`        | count       | -               | Total issues processed                                     |
+| `tracker_exporter_issues_search_time_seconds`          | time        | -               | Yandex.Tracker search duration time in seconds             |
+| `tracker_exporter_issues_without_metrics`              | count       | -               | Issues with empty metrics (no changelog)                   |
+| `tracker_exporter_issue_prefetch_seconds`              | time        | -               | Pre-transform data duration in seconds                     |
+| `tracker_exporter_comments_fetch_seconds`              | time        | -               | Comments fetch duration in seconds                         |
+| `tracker_exporter_etl_duration_seconds`                | time        | -               | ETL full pipeline duration in seconds                      |
+| `tracker_exporter_etl_upload_status`                   | gauge       | -               | Last upload status, 1 - success, 2 - fail                  |
+| `tracker_exporter_export_and_transform_time_seconds`   | time        | -               | Overall export and transform duration in seconds           |
+| `tracker_exporter_upload_to_storage_time_seconds`      | time        | -               | Overall insert duration time in seconds                    |
+| `tracker_exporter_last_update_timestamp`               | gauge       | -               | Last data update timestamp                                 |
+| `tracker_exporter_clickhouse_insert_time_seconds`      | time        | database, table | Insert per table duration time in seconds                  |
+| `tracker_exporter_clickhouse_inserted_rows`            | count       | database, table | Inserted rows per table                                    |
+| `tracker_exporter_clickhouse_deduplicate_time_seconds` | time        | database, table | Optimize execute time duration in seconds                  |
 
 ### Metrics on dashboard demo
+
 ![](/docs/images/etl_metrics.jpeg)
```

### Comparing `tracker-exporter-1.0.3/setup.py` & `tracker-exporter-2.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `tracker-exporter-1.0.3/tracker_exporter/config.py` & `tracker-exporter-2.0.0/tracker_exporter/config.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,40 +1,35 @@
 import datetime
 import logging
 
 from functools import lru_cache
-from typing import List
+from typing import Literal, Optional, Union
 from pydantic import validator, root_validator
 from pydantic_settings import BaseSettings
 
-from tracker_exporter.models.base import (
-    YandexTrackerLanguages,
-    LogLevels,
-    StateStorageTypes,
-    JsonStorageStrategies,
-)
+from tracker_exporter.models.base import YandexTrackerLanguages, LogLevels
 from tracker_exporter.exceptions import ConfigurationError
 from tracker_exporter.services.monitoring import DogStatsdClient
 
 YANDEX_TRACKER_API_SEARCH_HARD_LIMIT = 10000
 YANDEX_TRACKER_HARD_LIMIT_ISSUE_URL = "https://github.com/yandex/yandex_tracker_client/issues/13"
 
 logger = logging.getLogger(__name__)
 
 
 class MonitoringSettings(BaseSettings):
     """Observability settings."""
 
-    metrics_enabled: bool = False
-    metrics_host: str = "localhost"
-    metrics_port: int = 8125
-    metrics_base_prefix: str = "tracker_exporter"
-    metrics_base_labels: List[str] = []
-    sentry_enabled: bool = False
-    sentry_dsn: str | None = None
+    metrics_enabled: Optional[bool] = False
+    metrics_host: Optional[str] = "localhost"
+    metrics_port: Optional[int] = 8125
+    metrics_base_prefix: Optional[str] = "tracker_exporter"
+    metrics_base_labels: Optional[list[str]] = []
+    sentry_enabled: Optional[bool] = False
+    sentry_dsn: Optional[str] = None
 
     @validator("sentry_dsn", pre=True, always=True)
     def validate_sentry_dsn(cls, value: str | None, values: dict) -> str:
         sentry_enabled = values.get("sentry_enabled")
         if sentry_enabled and not value:
             raise ConfigurationError("Sentry DSN must not be empty when Sentry is enabled")
         return value
@@ -42,31 +37,31 @@
     class Config:
         extra = "ignore"
 
 
 class ClickhouseSettings(BaseSettings):
     """Settings for Clickhouse storage."""
 
-    enable_upload: bool = True
-    host: str = "localhost"
-    proto: str = "http"
-    port: int = 8123
-    cacert_path: str | None = None
+    enable_upload: Optional[bool] = True
+    host: Optional[str] = "localhost"
+    proto: Optional[str] = "http"
+    port: Optional[int] = 8123
+    cacert_path: Optional[str] = None
     serverless_proxy_id: str | None = None
-    username: str = "default"
-    password: str | None = None
-    database: str = "agile"
-    issues_table: str = "issues"
-    issue_metrics_table: str = "issue_metrics"
-    issues_changelog_table: str = "issues_changelog"
-    auto_deduplicate: bool = True
-    backoff_base_delay: int | float = 0.5
-    backoff_expo_factor: int | float = 2.5
-    backoff_max_tries: int = 3
-    backoff_jitter: bool = True
+    username: Optional[str] = "default"
+    password: Optional[str] = None
+    database: Optional[str] = "agile"
+    issues_table: Optional[str] = "issues"
+    issue_metrics_table: Optional[str] = "issue_metrics"
+    issues_changelog_table: Optional[str] = "issues_changelog"
+    auto_deduplicate: Optional[bool] = True
+    backoff_base_delay: Optional[Union[int, float]] = 0.5
+    backoff_expo_factor: Optional[Union[int, float]] = 2.5
+    backoff_max_tries: Optional[int] = 3
+    backoff_jitter: Optional[bool] = True
 
     @validator("serverless_proxy_id", pre=True, always=True)
     def validate_serverless_proxy_id(cls, value: str | None, values: dict) -> str:
         http = values.get("proto") == "http"
         if http and value is not None:
             raise ConfigurationError("Clickhouse proto must be HTTPS when serverless used")
         return value
@@ -81,18 +76,18 @@
     class Config:
         extra = "ignore"
 
 
 class IssuesSearchSettings(BaseSettings):
     """Settings for search & export."""
 
-    query: str | None = None
-    range: str = "2h"
-    queues: str | List[str] | None = None
-    per_page_limit: int = 100
+    query: Optional[str] = None
+    range: Optional[str] = "2h"
+    queues: Optional[Union[str, list[str]]] = None
+    per_page_limit: Optional[int] = 100
 
     @validator("queues", pre=True, always=True)
     def validate_queues(cls, value: str) -> list:
         if value is None:
             return None
 
         if not isinstance(value, (str, list)):
@@ -104,23 +99,23 @@
     class Config:
         extra = "ignore"
 
 
 class TrackerSettings(BaseSettings):
     """Settings for Yandex.Tracker client."""
 
-    loglevel: LogLevels = LogLevels.warning
-    token: str | None = None
-    org_id: str | None = None
-    iam_token: str | None = None
-    cloud_org_id: str | None = None
-    timeout: int = 10
-    max_retries: int = 10
-    language: YandexTrackerLanguages = YandexTrackerLanguages.en
-    timezone: str = "Europe/Moscow"
+    loglevel: Optional[LogLevels] = LogLevels.warning
+    token: Optional[str] = None
+    org_id: Optional[str] = None
+    iam_token: Optional[str] = None
+    cloud_org_id: Optional[str] = None
+    timeout: Optional[int] = 10
+    max_retries: Optional[int] = 10
+    language: Optional[YandexTrackerLanguages] = YandexTrackerLanguages.en
+    timezone: Optional[str] = "Europe/Moscow"
     search: IssuesSearchSettings = IssuesSearchSettings()
 
     @root_validator(pre=True)
     def validate_tokens_and_orgs(cls, values) -> str:
         token = values.get("token")
         iam_token = values.get("iam_token")
         org_id = values.get("org_id")
@@ -141,24 +136,24 @@
     class Config:
         extra = "ignore"
 
 
 class StateSettings(BaseSettings):
     """Settings for stateful mode."""
 
-    storage: StateStorageTypes | None = StateStorageTypes.jsonfile
-    redis_dsn: str = "redis://localhost:6379"
-    jsonfile_strategy: JsonStorageStrategies = JsonStorageStrategies.local
-    jsonfile_path: str = "./state.json"
-    jsonfile_s3_bucket: str | None = None
-    jsonfile_s3_region: str = "eu-east-1"
-    jsonfile_s3_endpoint: str | None = None
-    jsonfile_s3_access_key: str | None = None
-    jsonfile_s3_secret_key: str | None = None
-    custom_storage_params: dict = {}
+    storage: Optional[Literal["redis", "jsonfile", "custom"]] = "jsonfile"
+    redis_dsn: Optional[str] = "redis://localhost:6379"
+    jsonfile_strategy: Optional[Literal["s3", "local"]] = "local"
+    jsonfile_path: Optional[str] = "state.json"
+    jsonfile_s3_bucket: Optional[str] = None
+    jsonfile_s3_region: Optional[str] = "us-east-1"
+    jsonfile_s3_endpoint: Optional[str] = None
+    jsonfile_s3_access_key: Optional[str] = None
+    jsonfile_s3_secret_key: Optional[str] = None
+    custom_storage_params: Optional[dict] = {}
 
     @root_validator(pre=True)
     def validate_state(cls, values) -> str:
         jsonfile_strategy = values.get("jsonfile_strategy")
         jsonfile_s3_bucket = values.get("jsonfile_s3_bucket")
         jsonfile_s3_endpoint = values.get("jsonfile_s3_endpoint")
         jsonfile_s3_access_key = values.get("jsonfile_s3_access_key")
@@ -168,15 +163,15 @@
                 jsonfile_s3_bucket,
                 jsonfile_s3_endpoint,
                 jsonfile_s3_access_key,
                 jsonfile_s3_secret_key,
             )
         )
 
-        if jsonfile_strategy == JsonStorageStrategies.s3 and not s3_is_configured:
+        if jsonfile_strategy == "s3" and not s3_is_configured:
             raise ConfigurationError("S3 must be configured for JSONFileStorage with S3 strategy.")
 
         return values
 
     class Config:
         extra = "ignore"
 
@@ -184,31 +179,31 @@
 class Settings(BaseSettings):
     """Global merged config."""
 
     monitoring: MonitoringSettings = MonitoringSettings()
     clickhouse: ClickhouseSettings = ClickhouseSettings()
     tracker: TrackerSettings = TrackerSettings  # TODO (akimrx): research, called class not see TOKEN's
     state: StateSettings = StateSettings()
-    stateful: bool = False
-    stateful_initial_range: str = "1w"
-    changelog_export_enabled: bool = False
-    log_etl_stats: bool = True
-    log_etl_stats_each_n_iter: int = 100
-
-    loglevel: LogLevels = LogLevels.info
-    workdays: List[int] = [0, 1, 2, 3, 4]
-    business_hours_start: datetime.time = datetime.time(9)
-    business_hours_end: datetime.time = datetime.time(22)
-    datetime_response_format: str = "%Y-%m-%dT%H:%M:%S.%f%z"
-    datetime_query_format: str = "%Y-%m-%d %H:%M:%S"
-    datetime_clickhouse_format: str = "%Y-%m-%dT%H:%M:%S.%f"
-
-    etl_interval_minutes: int = 30
-    closed_issue_statuses: str | list = "closed,rejected,resolved,cancelled,released"
-    not_nullable_fields: tuple | list | str = (
+    stateful: Optional[bool] = False
+    stateful_initial_range: Optional[str] = "1w"
+    changelog_export_enabled: Optional[bool] = False
+    log_etl_stats: Optional[bool] = True
+    log_etl_stats_each_n_iter: Optional[int] = 100
+
+    loglevel: Optional[LogLevels] = LogLevels.info
+    workdays: Optional[list[int]] = [0, 1, 2, 3, 4]
+    business_hours_start: Optional[datetime.time] = datetime.time(9)
+    business_hours_end: Optional[datetime.time] = datetime.time(22)
+    datetime_response_format: Optional[str] = "%Y-%m-%dT%H:%M:%S.%f%z"
+    datetime_query_format: Optional[str] = "%Y-%m-%d %H:%M:%S"
+    datetime_clickhouse_format: Optional[str] = "%Y-%m-%dT%H:%M:%S.%f"
+
+    etl_interval_minutes: Optional[int] = 30
+    closed_issue_statuses: Optional[Union[str, list]] = "closed,rejected,resolved,cancelled,released"
+    not_nullable_fields: Optional[Union[tuple, list, str]] = (
         "created_at",
         "resolved_at",
         "closed_at",
         "updated_at",
         "released_at",
         "deadline",
         "start_date",
```

### Comparing `tracker-exporter-1.0.3/tracker_exporter/etl.py` & `tracker-exporter-2.0.0/tracker_exporter/etl.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import time
 import logging
 from datetime import datetime, timedelta
-from typing import Tuple, List
+from typing import Tuple, List, Optional
 from yandex_tracker_client.collections import Issues
 from yandex_tracker_client.objects import SeekablePaginatedList
 from yandex_tracker_client.exceptions import Forbidden
 
 from tracker_exporter.config import config, monitoring
 from tracker_exporter.models.issue import TrackerIssue
 from tracker_exporter.models.base import ClickhousePayload
-from tracker_exporter.services.state import StateKeeper
+from tracker_exporter.state.managers import AbstractStateManager
 from tracker_exporter.services.tracker import YandexTrackerClient
 from tracker_exporter.services.clickhouse import ClickhouseClient
 from tracker_exporter.exceptions import ConfigurationError, UploadError, ExportOrTransformError
 from tracker_exporter.utils.helpers import (
     fix_null_dates,
     from_human_time,
     convert_datetime,
@@ -27,26 +27,26 @@
     """Export, transform, load facade."""
 
     def __init__(
         self,
         *,
         tracker_client: YandexTrackerClient,
         clickhouse_client: ClickhouseClient,
-        statekeeper: StateKeeper | None = None,
+        state_manager: Optional[AbstractStateManager] = None,
         issue_model: TrackerIssue = TrackerIssue,
         database: str = config.clickhouse.database,
         issues_table: str = config.clickhouse.issues_table,
         metrics_table: str = config.clickhouse.issue_metrics_table,
         changelogs_table: str = config.clickhouse.issues_changelog_table,
         upload_to_storage: bool = config.clickhouse.enable_upload,
         state_key: str = "tracker_etl_default",
     ) -> None:
         self.tracker = tracker_client
         self.clickhouse = clickhouse_client
-        self.state = statekeeper
+        self.state = state_manager
         self.issue_model = issue_model
         self.database = database
         self.issues_table = issues_table
         self.metrics_table = metrics_table
         self.changelogs_table = changelogs_table
         self.upload_to_storage = upload_to_storage
         self.state_key = state_key
@@ -138,15 +138,15 @@
         issues_without_metrics = 0
         possible_new_state = None
         logger.info("Searching, exporting and transform issues...")
 
         found_issues = self.tracker.search_issues(query=query, filter=filter, order=order, limit=limit)
         if len(found_issues) == 0:
             logger.info("Nothing to export. Skipping ETL")
-            return
+            return issues, changelog_events, metrics, possible_new_state
 
         if isinstance(found_issues, SeekablePaginatedList):
             pagination = True
             logger.info("Paginated list received, possible new state will be calculated later")
         else:
             pagination = False
             possible_new_state = self._get_possible_new_state(self.issue_model(found_issues[-1]))
@@ -212,15 +212,15 @@
         auto_deduplicate: bool = True,
     ) -> None:
         """Runs main ETL process."""
         query = self._build_search_query(stateful, queues, search_query, search_range)
         try:
             issues, changelogs, metrics, possible_new_state = self._export_and_transform(**query, limit=limit)
             if stateful and possible_new_state is not None:
-                logger.info(f"Possible new state: {possible_new_state}")
+                logger.info(f"Stateful mode enabled, fetching possible new state: {possible_new_state}")
                 last_saved_state = self.state.get(self.state_key)
                 if last_saved_state == possible_new_state and len(issues) <= 1 and len(metrics) <= 1:
                     logger.info("Data already is up-to-date, skipping upload stage")
                     return
         except Exception as exc:
             logger.error(f"An error occured in ETL while exporting and transform: {exc}")
             if not ignore_exceptions:
@@ -243,14 +243,15 @@
             except Exception as exc:
                 logger.error(f"An exception occured in ETL while uploading: {exc}")
                 success = False
                 if not ignore_exceptions:
                     raise UploadError(str(exc))
             else:
                 if all((stateful, self.state, possible_new_state)):
+                    logger.info(f"Saving last ETL timestamp {possible_new_state}")
                     self.state.set(self.state_key, possible_new_state)
                 else:
                     logger.info(
                         "The state snapshot will not be saved. Not all conditions are met "
                         f"{stateful=} {self.state=} {possible_new_state=}"
                     )
                 monitoring.send_gauge_metric("last_update_timestamp", value=int(time.time()))
```

### Comparing `tracker-exporter-1.0.3/tracker_exporter/main.py` & `tracker-exporter-2.0.0/tracker_exporter/main.py`

 * *Files 17% similar despite different names*

```diff
@@ -19,26 +19,27 @@
     "--env-file",
     metavar="file",
     dest="env_file",
     type=str,
     required=False,
     help="Path to .env file",
 )
+parser.add_argument("--run-once", dest="run_once", action="store_true", help="Run ETL once.")
 args, _ = parser.parse_known_args()
 warnings.filterwarnings("ignore")
 
 if args.env_file:
     load_dotenv(args.env_file)
 else:
     load_dotenv(find_dotenv())
 
 # pylint: disable=C0413
 from tracker_exporter.services.monitoring import sentry_events_filter
-from tracker_exporter.services.state import StateKeeper, LocalFileStorageStrategy, JsonStateStorage
-from tracker_exporter.models.base import StateStorageTypes, JsonStorageStrategies
+from tracker_exporter.state.managers import AbstractStateManager
+from tracker_exporter.state.factory import StateManagerFactory, IObjectStorageProps
 from tracker_exporter.models.issue import TrackerIssue
 from tracker_exporter.etl import YandexTrackerETL
 from tracker_exporter.services.tracker import YandexTrackerClient
 from tracker_exporter.services.clickhouse import ClickhouseClient
 from tracker_exporter._meta import appname, version
 from tracker_exporter.config import config
 
@@ -75,47 +76,45 @@
             traces_sample_rate=1.0,
             release=f"{appname}@{version}",
             before_send=sentry_events_filter,
         )
     logger.info(f"Sentry send traces is {'enabled' if config.monitoring.sentry_enabled else 'disabled'}")
 
 
-def configure_jsonfile_storage() -> JsonStateStorage:
-    """Configure and returns storage for StateKeeper."""
-    match config.state.jsonfile_strategy:
-        case JsonStorageStrategies.local:
-            storage_strategy = LocalFileStorageStrategy(config.state.jsonfile_path)
-        case JsonStorageStrategies.s3:
-            raise NotImplementedError
-        case _:
-            raise ValueError
-    return JsonStateStorage(storage_strategy)
-
-
-def configure_state_service() -> StateKeeper | None:
+def configure_state_manager() -> AbstractStateManager | None:
     """Configure StateKeeper for ETL stateful mode."""
     if not config.stateful:
         return
 
     match config.state.storage:
-        case StateStorageTypes.jsonfile:
-            storage = configure_jsonfile_storage()
-        case StateStorageTypes.redis:
+        case "jsonfile":
+            s3_props: IObjectStorageProps = IObjectStorageProps(
+                bucket_name=config.state.jsonfile_s3_bucket,
+                access_key_id=config.state.jsonfile_s3_access_key,
+                secret_key=config.state.jsonfile_s3_secret_key,
+                endpoint_url=config.state.jsonfile_s3_endpoint,
+                region=config.state.jsonfile_s3_region,
+            )
+            return StateManagerFactory.create_file_state_manager(
+                strategy=config.state.jsonfile_strategy, filename=config.state.jsonfile_path, **s3_props
+            )
+        case "redis":
+            return StateManagerFactory.create_redis_state_manager(config.state.redis_dsn)
+        case "custom":
             raise NotImplementedError
         case _:
             raise ValueError
-    return StateKeeper(storage)
 
 
 def run_etl(ignore_exceptions: bool = False, issue_model: TrackerIssue = TrackerIssue) -> None:
     """Start ETL process."""
     etl = YandexTrackerETL(
         tracker_client=YandexTrackerClient(),
         clickhouse_client=ClickhouseClient(),
-        statekeeper=configure_state_service(),
+        state_manager=configure_state_manager(),
         issue_model=issue_model,
     )
     etl.run(
         stateful=config.stateful,
         queues=config.tracker.search.queues,
         search_query=config.tracker.search.query,
         search_range=config.tracker.search.range,
@@ -124,14 +123,20 @@
         auto_deduplicate=config.clickhouse.auto_deduplicate,
     )
 
 
 def main() -> None:
     """Entry point for CLI command."""
     configure_sentry()
+
+    if args.run_once:
+        logger.info("A one-time launch command is received, the scheduler setting will be skipped")
+        run_etl()
+        sys.exit(0)
+
     signal.signal(signal.SIGINT, signal_handler)
     signal.signal(signal.SIGTERM, signal_handler)
     scheduler.start()
     scheduler.add_job(
         run_etl,
         trigger="interval",
         name="tracker_etl_default",
```

### Comparing `tracker-exporter-1.0.3/tracker_exporter/models/base.py` & `tracker-exporter-2.0.0/tracker_exporter/models/base.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,32 +1,21 @@
 import json
-from abc import ABCMeta, ABC, abstractmethod
+from abc import ABCMeta
 from enum import Enum
 from typing import Any
 
 from pydantic import BaseModel
 
 
 class ClickhousePayload(BaseModel):
     issue: dict
     changelog: list
     metrics: list
 
 
-class StateStorageTypes(str, Enum):
-    redis = "redis"
-    jsonfile = "jsonfile"
-    custom = "custom"
-
-
-class JsonStorageStrategies(str, Enum):
-    local = "local"
-    s3 = "s3"
-
-
 class LogLevels(str, Enum):
     debug = "debug"
     info = "info"
     warning = "warning"
     error = "error"
     critical = "critical"
 
@@ -96,45 +85,7 @@
                 return [parse(it) for it in val]
             if isinstance(val, dict):
                 return {key: null_cleaner(parse(value)) for key, value in val.items() if not key.startswith("_")}
             return val
 
         data = self.__dict__.copy()
         return parse(data)
-
-
-class BaseStateStorage(ABC):
-    """Abstract class for state storage.
-    Allows you to save, receive, delete and flush the state.
-
-    """
-
-    @abstractmethod
-    def set(self, key: str, value: Any) -> None:
-        """Save key:value pair to storage."""
-
-    @abstractmethod
-    def get(self, key: str) -> Any:
-        """Get value by key from storage."""
-
-    @abstractmethod
-    def delete(self, key: str) -> None:
-        """Delete value by key from storage."""
-
-    @abstractmethod
-    def flush(self) -> None:
-        """Flush (drop) state from storage."""
-
-
-class JSONFileStorageStrategy(ABC):
-    """Abstract strategy for store content via file."""
-
-    def __init__(self, file_path: str) -> None:
-        self.file_path = file_path
-
-    @abstractmethod
-    def read(self) -> Any:
-        """Read content from file."""
-
-    @abstractmethod
-    def save(self) -> Any:
-        """Save content to file."""
```

### Comparing `tracker-exporter-1.0.3/tracker_exporter/models/issue.py` & `tracker-exporter-2.0.0/tracker_exporter/models/issue.py`

 * *Files identical despite different names*

### Comparing `tracker-exporter-1.0.3/tracker_exporter/services/clickhouse.py` & `tracker-exporter-2.0.0/tracker_exporter/services/clickhouse.py`

 * *Files identical despite different names*

### Comparing `tracker-exporter-1.0.3/tracker_exporter/services/monitoring.py` & `tracker-exporter-2.0.0/tracker_exporter/services/monitoring.py`

 * *Files identical despite different names*

### Comparing `tracker-exporter-1.0.3/tracker_exporter/services/tracker.py` & `tracker-exporter-2.0.0/tracker_exporter/services/tracker.py`

 * *Files identical despite different names*

### Comparing `tracker-exporter-1.0.3/tracker_exporter/utils/helpers.py` & `tracker-exporter-2.0.0/tracker_exporter/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `tracker-exporter-1.0.3/tracker_exporter.egg-info/SOURCES.txt` & `tracker-exporter-2.0.0/tracker_exporter.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -19,11 +19,15 @@
 tracker_exporter.egg-info/top_level.txt
 tracker_exporter/models/__init__.py
 tracker_exporter/models/base.py
 tracker_exporter/models/issue.py
 tracker_exporter/services/__init__.py
 tracker_exporter/services/clickhouse.py
 tracker_exporter/services/monitoring.py
-tracker_exporter/services/state.py
 tracker_exporter/services/tracker.py
+tracker_exporter/state/__init__.py
+tracker_exporter/state/backends.py
+tracker_exporter/state/factory.py
+tracker_exporter/state/managers.py
+tracker_exporter/state/serializers.py
 tracker_exporter/utils/__init__.py
 tracker_exporter/utils/helpers.py
```

