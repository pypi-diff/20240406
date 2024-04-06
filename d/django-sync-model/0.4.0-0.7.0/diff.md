# Comparing `tmp/django_sync_model-0.4.0.tar.gz` & `tmp/django_sync_model-0.7.0.tar.gz`

## Comparing `django_sync_model-0.4.0.tar` & `django_sync_model-0.7.0.tar`

### file list

```diff
@@ -1,25 +1,27 @@
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 django_sync_model-0.4.0/sync_model/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_sync_model-0.4.0/sync_model/__init__.py
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 django_sync_model-0.4.0/sync_model/admin.py
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 django_sync_model-0.4.0/sync_model/apps.py
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 django_sync_model-0.4.0/sync_model/exceptions.py
--rw-r--r--   0        0        0     2218 2020-02-02 00:00:00.000000 django_sync_model-0.4.0/sync_model/models.py
--rw-r--r--   0        0        0     4597 2020-02-02 00:00:00.000000 django_sync_model-0.4.0/sync_model/tests.py
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 django_sync_model-0.4.0/sync_model/types.py
--rw-r--r--   0        0        0     3054 2020-02-02 00:00:00.000000 django_sync_model-0.4.0/sync_model/utils.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 django_sync_model-0.4.0/sync_model/views.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_sync_model-0.4.0/sync_model/management/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_sync_model-0.4.0/sync_model/management/commands/__init__.py
--rw-r--r--   0        0        0     2402 2020-02-02 00:00:00.000000 django_sync_model-0.4.0/sync_model/management/commands/sync_model.py
--rw-r--r--   0        0        0     2170 2020-02-02 00:00:00.000000 django_sync_model-0.4.0/sync_model/migrations/0001_initial.py
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 django_sync_model-0.4.0/sync_model/migrations/0002_synctask_source_db_synctask_target_db.py
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 django_sync_model-0.4.0/sync_model/migrations/0003_synctask_name.py
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 django_sync_model-0.4.0/sync_model/migrations/0004_stockaction_stock_number.py
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 django_sync_model-0.4.0/sync_model/migrations/0005_stockaction_sender.py
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 django_sync_model-0.4.0/sync_model/migrations/0006_stockaction_update_datetime.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_sync_model-0.4.0/sync_model/migrations/__init__.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 django_sync_model-0.4.0/.gitignore
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 django_sync_model-0.4.0/LICENSE
--rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 django_sync_model-0.4.0/README.md
--rw-r--r--   0        0        0     3303 2020-02-02 00:00:00.000000 django_sync_model-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     2059 2020-02-02 00:00:00.000000 django_sync_model-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 django_sync_model-0.7.0/sync_model/__about__.py
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 django_sync_model-0.7.0/sync_model/__init__.py
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 django_sync_model-0.7.0/sync_model/admin.py
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 django_sync_model-0.7.0/sync_model/apps.py
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 django_sync_model-0.7.0/sync_model/exceptions.py
+-rw-r--r--   0        0        0     2364 2020-02-02 00:00:00.000000 django_sync_model-0.7.0/sync_model/models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_sync_model-0.7.0/sync_model/py.typed
+-rw-r--r--   0        0        0     4780 2020-02-02 00:00:00.000000 django_sync_model-0.7.0/sync_model/tests.py
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 django_sync_model-0.7.0/sync_model/types.py
+-rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 django_sync_model-0.7.0/sync_model/utils.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 django_sync_model-0.7.0/sync_model/views.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_sync_model-0.7.0/sync_model/management/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_sync_model-0.7.0/sync_model/management/commands/__init__.py
+-rw-r--r--   0        0        0     3795 2020-02-02 00:00:00.000000 django_sync_model-0.7.0/sync_model/management/commands/sync_model.py
+-rw-r--r--   0        0        0     2170 2020-02-02 00:00:00.000000 django_sync_model-0.7.0/sync_model/migrations/0001_initial.py
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 django_sync_model-0.7.0/sync_model/migrations/0002_synctask_source_db_synctask_target_db.py
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 django_sync_model-0.7.0/sync_model/migrations/0003_synctask_name.py
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 django_sync_model-0.7.0/sync_model/migrations/0004_stockaction_stock_number.py
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 django_sync_model-0.7.0/sync_model/migrations/0005_stockaction_sender.py
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 django_sync_model-0.7.0/sync_model/migrations/0006_stockaction_update_datetime.py
+-rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 django_sync_model-0.7.0/sync_model/migrations/0007_broker_rawstockaction_broker.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_sync_model-0.7.0/sync_model/migrations/__init__.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 django_sync_model-0.7.0/.gitignore
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 django_sync_model-0.7.0/LICENSE
+-rw-r--r--   0        0        0     1343 2020-02-02 00:00:00.000000 django_sync_model-0.7.0/README.md
+-rw-r--r--   0        0        0     3375 2020-02-02 00:00:00.000000 django_sync_model-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     2248 2020-02-02 00:00:00.000000 django_sync_model-0.7.0/PKG-INFO
```

### Comparing `django_sync_model-0.4.0/sync_model/models.py` & `django_sync_model-0.7.0/sync_model/models.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,14 +32,18 @@
     )
     filter_by = models.JSONField(default=dict)
 
     def __str__(self):
         return self.name
 
 
+class Broker(models.Model):
+    name = models.TextField(default="")
+
+
 class RawStockAction(models.Model):
     """
     e.g.
         In a stock system, many user will
             1. buy a stock,
             2. sell a stock
             3. cancel some action
@@ -50,14 +54,15 @@
             * order by update_datetime and -sender
     """
     ACTION_TYPE_CHOICES = (
             ("buy", "buy"),
             ("sell", "sell"),
             ("cancel", "cancel"),
     )
+    broker = models.ForeignKey(Broker, null=True, on_delete=models.CASCADE)
     sender = models.CharField(max_length=32)
     action_type = models.CharField(
             choices=ACTION_TYPE_CHOICES,
             max_length=10,
     )
     update_datetime = models.DateTimeField()
     canceled = models.BooleanField()
```

### Comparing `django_sync_model-0.4.0/sync_model/tests.py` & `django_sync_model-0.7.0/sync_model/tests.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,60 +4,65 @@
 from django.core.management import call_command
 from django.test import TestCase
 from django.utils import timezone
 
 from sync_model.exceptions import StepTooSmallException
 from sync_model.models import (
         RawStockAction, StockAction,
-        SyncTask,
+        SyncTask, Broker,
 )
 from sync_model.utils import get_value
 
 
 
 class Test(TestCase):
 
     def test(self):
         now = timezone.make_aware(
                 datetime.datetime(2024, 1, 1, 2, 3, 4)
         )
+        broker = Broker.objects.create()
         second_stock = RawStockAction.objects.create(
                 sender="charlie",
                 action_type="buy",
                 update_datetime=now,
                 canceled=True,
                 stock_number="LUCK",
+                broker=broker,
         )
         fourth_stock = RawStockAction.objects.create(
                 sender="alice",
                 action_type="buy",
                 update_datetime=now,
                 canceled=False,
                 stock_number="LUCK",
+                broker=broker,
         )
         first_stock = RawStockAction.objects.create(
                 sender="bob",
                 action_type="sell",
                 update_datetime=now-datetime.timedelta(days=1),
                 canceled=False,
                 stock_number="LUCK_PRE",
+                broker=broker,
         )
         third_stock = RawStockAction.objects.create(
                 sender="bob",
                 action_type="buy",
                 update_datetime=now,
                 canceled=False,
                 stock_number="LUCK",
+                broker=broker,
         )
         sync_task = SyncTask.objects.create(
                 source=ContentType.objects.get_for_model(RawStockAction),
                 target=ContentType.objects.get_for_model(StockAction),
                 sync_method="sync_model.utils.sync_raw_stock_action",
                 batch_size=1,
-                order_by=["update_datetime", "-sender"],
+                order_by=["update_datetime", "-sender", "broker"],
                 filter_by={
                     "canceled": False,
                 }
         )
         call_command("sync_model")
         sync_task.refresh_from_db()
         first_sync_stock = StockAction.objects.get()
```

### Comparing `django_sync_model-0.4.0/sync_model/utils.py` & `django_sync_model-0.7.0/sync_model/utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,32 +5,39 @@
 
 """
 useful utils to sync model instance
 """
 
 
 import datetime
+import logging
 import warnings
 
-from typing import NewType, List
+from typing import NewType, List, Optional
 
 from django.db.models import Q, Model
+from django.utils import timezone
 
 from .models import (
         SyncTask, StockAction
         )
+from .types import SyncResult
 
 
 OrderBy = NewType("OrderBy", List[str])
+LOGGER = logging.getLogger(__name__)
 
 
 def get_queryset(sync_task: SyncTask):
     """get filtered and ordered queryset from sync_task"""
-    source_model = sync_task.source.model_class()
-    queryset = source_model.objects.using(sync_task.source_db).filter(
+    source_model: Optional[type[Model]] = sync_task.source.model_class()
+    if source_model is None:
+        raise ValueError(f"A sync task {sync_task} use an deleted model")
+    all_queryset = source_model.objects.using(sync_task.source_db)  # type: ignore[attr-defined]
+    queryset = all_queryset.filter(
             **sync_task.filter_by
     ).order_by(*sync_task.order_by)
     filter_q = get_Q(sync_task.order_by, sync_task.last_sync)
     return queryset.filter(filter_q)
 
 
 def get_value(instance: Model, order_by: OrderBy, datetime2str: bool) -> dict:
@@ -38,20 +45,19 @@
     get last sync value from instance according order_by
     e.g.
         >>> get_value(User, order_by: ["id", "-username"])
         {"id": 888, "-username": "alice"}
     """
     result = {}
     for key in order_by:
-        if key.startswith("-"):
-            result[key] = getattr(instance, key[1:])
-        else:
-            result[key] = getattr(instance, key)
+        result[key] = getattr(instance, key.lstrip("-"))
         if datetime2str and isinstance(result[key], datetime.datetime):
             result[key] = result[key].isoformat()
+        elif isinstance(result[key], Model):
+            result[key] = result[key].pk
     return result
 
 
 def get_Q(order_by: OrderBy, last_sync: dict) -> Q:  # pylint: disable=invalid-name
     """
     get django Q filter from order_by and last_sync data
     """
@@ -83,25 +89,41 @@
         }
         result |= Q(
             **same_dict,
             **greater_dict,
         )
         same_dict[greater_key.strip("-")] = last_sync[greater_key]
     result |= Q(**same_dict)
+    LOGGER.debug("query: %s", result)
     return result
 
 
-def sync_raw_stock_action(queryset,
-                          target_model: StockAction,
-                          sync_task: SyncTask):  # pylint: disable=unused-argument
+def sync_raw_stock_action(
+        queryset,
+        target_model: StockAction,
+        sync_task: SyncTask) -> SyncResult:
+    # pylint: disable=unused-argument
     """
     only sync the id field
     """
+    sync_result: SyncResult = {
+            "finished": False,
+            "count": 0,
+            "start": timezone.now(),
+            "last_sync_model": None,
+            "end": timezone.now(),
+    }
     for raw_stockaction in queryset:
         target_model.objects.get_or_create(
                 id=raw_stockaction.id,
                 defaults={
                     "update_datetime": raw_stockaction.update_datetime,
                     "stock_number": raw_stockaction.stock_number,
                     "sender": raw_stockaction.sender,
                 }
         )
+        sync_result["last_sync_model"] = raw_stockaction
+        sync_result["count"] += 1
+    if sync_result["count"] < sync_task.batch_size:
+        sync_result["finished"] = True
+    sync_result["end"] = timezone.now()
+    return sync_result
```

### Comparing `django_sync_model-0.4.0/sync_model/management/commands/sync_model.py` & `django_sync_model-0.7.0/sync_model/management/commands/sync_model.py`

 * *Files 25% similar despite different names*

```diff
@@ -23,16 +23,23 @@
 
 LOGGER = logging.getLogger(__name__)
 
 
 class Command(BaseCommand):
     """run sync model task"""
 
+    def add_arguments(self, parser):
+        parser.add_argument("--name", type=str)
+
     def handle(self, *args, **kwargs):  # pylint: disable=unused-argument
-        LOGGER.info("start run sync model")
+        if kwargs.get("name"):
+            self.run_sync_task(
+                    SyncTask.objects.get(name=kwargs["name"])
+            )
+            return
         synced_tasks = set()
         finished_tasks = set()
         next_tasks = set(SyncTask.objects.filter(dependencies=None))
         while next_tasks:
             sync_task = next_tasks.pop()
             result = self.run_sync_task(sync_task)
             synced_tasks.add(sync_task)
@@ -47,28 +54,52 @@
                         continue
                     next_tasks.add(nomination_task)
 
     @staticmethod
     def run_sync_task(sync_task: SyncTask) -> SyncResult:
         """
         sync a single SyncTask
-        """
-        result = {}
-        queryset = get_queryset(sync_task)
-        module, function = sync_task.sync_method.rsplit(".", 1)
-        sync_function = getattr(
-            importlib.import_module(module),
-            function
-        )
+
+        previous version: the queryset.count() will be very slow, so I require the sync_method to return a syncresult
+
+        ```python
         if queryset.count() > sync_task.batch_size:
             last_sync_model = queryset[sync_task.batch_size - 1]
             result["finished"] = False
         else:
             last_sync_model = queryset.last()
             result["finished"] = True
         sync_function(queryset[0:sync_task.batch_size], sync_task.target.model_class(), sync_task)
         last_value = get_value(last_sync_model, sync_task.order_by, datetime2str=True)
         if result["finished"] is False and sync_task.last_sync == last_value:
+        ```
+
+        """
+        LOGGER.info("start sync: %s", sync_task)
+        queryset = get_queryset(sync_task)
+        module, function = sync_task.sync_method.rsplit(".", 1)
+        sync_function = getattr(
+            importlib.import_module(module),
+            function
+        )
+        LOGGER.debug("sync_function realized")
+        sync_result: SyncResult = sync_function(
+                queryset[0:sync_task.batch_size],
+                sync_task.target.model_class(),
+                sync_task)
+        if sync_result["last_sync_model"] is None:
+            if sync_result["count"] == 0:
+                LOGGER.info("Origin model has deleted the last model")
+                LOGGER.info("%s finished %s, last_sync: %s",
+                            sync_task, sync_result, sync_task.last_sync)
+                return sync_result
+            raise ValueError("sync count is not None, but the last_sync_model is empty")
+        last_value = get_value(sync_result["last_sync_model"],
+                               sync_task.order_by,
+                               datetime2str=True)
+        if sync_result["finished"] is False and sync_task.last_sync == last_value:
             raise StepTooSmallException
         sync_task.last_sync = last_value
         sync_task.save()
-        return result
+        LOGGER.info("%s finished %s, last_sync: %s",
+                    sync_task, sync_result, sync_task.last_sync)
+        return sync_result
```

### Comparing `django_sync_model-0.4.0/sync_model/migrations/0001_initial.py` & `django_sync_model-0.7.0/sync_model/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_sync_model-0.4.0/sync_model/migrations/0002_synctask_source_db_synctask_target_db.py` & `django_sync_model-0.7.0/sync_model/migrations/0002_synctask_source_db_synctask_target_db.py`

 * *Files identical despite different names*

### Comparing `django_sync_model-0.4.0/.gitignore` & `django_sync_model-0.7.0/.gitignore`

 * *Files identical despite different names*

### Comparing `django_sync_model-0.4.0/LICENSE` & `django_sync_model-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_sync_model-0.4.0/README.md` & `django_sync_model-0.7.0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -26,22 +26,30 @@
         sync_method="sync_model.utils.sync_raw_stock_action",
         batch_size=2,
         order_by=["update_datetime", "-sender"],
         filter_by={
             "canceled": False,
         }
 )
+
+here your sync_method should return a sync result
 ```
 
 2. run sync task
 ```
 python3 manage.py sync_model
 ```
 
 # Features
 * [x] support sync data from one database to another
 * [x] incremental update
 * [x] support non-cycle dependency
 * [x] support filter
 * [x] support custom sync size of each table
+* [ ] support foreign key sort
 * [ ] support exclude filters
 * [ ] support timeout parameter
+* [ ] support None value
+
+# Release Notes
+* 0.5.0
+break change: `sync_function` should return `SyncResult`
```

### Comparing `django_sync_model-0.4.0/pyproject.toml` & `django_sync_model-0.7.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -164,7 +164,10 @@
 packages = ["src/sync_model"]
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/sync_model"]
 exclude = [
     "/example",
 ]
+
+[tool.setuptools.package-data]
+duration2 = ["src/sync_model/py.typed"]
```

### Comparing `django_sync_model-0.4.0/PKG-INFO` & `django_sync_model-0.7.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.3
+Metadata-Version: 2.1
 Name: django-sync-model
-Version: 0.4.0
+Version: 0.7.0
 Project-URL: Documentation, https://github.com/ramwin/django-sync-model#readme
 Project-URL: Issues, https://github.com/ramwin/django-sync-model/issues
 Project-URL: Source, https://github.com/ramwin/django-sync-model
 Author-email: Xiang Wang <ramwin@qq.com>
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
@@ -47,22 +47,30 @@
         sync_method="sync_model.utils.sync_raw_stock_action",
         batch_size=2,
         order_by=["update_datetime", "-sender"],
         filter_by={
             "canceled": False,
         }
 )
+
+here your sync_method should return a sync result
 ```
 
 2. run sync task
 ```
 python3 manage.py sync_model
 ```
 
 # Features
 * [x] support sync data from one database to another
 * [x] incremental update
 * [x] support non-cycle dependency
 * [x] support filter
 * [x] support custom sync size of each table
+* [ ] support foreign key sort
 * [ ] support exclude filters
 * [ ] support timeout parameter
+* [ ] support None value
+
+# Release Notes
+* 0.5.0
+break change: `sync_function` should return `SyncResult`
```

