# Comparing `tmp/pyeventmanager-0.5.1.tar.gz` & `tmp/pyeventmanager-0.5.2.tar.gz`

## Comparing `pyeventmanager-0.5.1.tar` & `pyeventmanager-0.5.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     3998 2020-02-02 00:00:00.000000 pyeventmanager-0.5.1/CHANGELOG.md
--rw-r--r--   0        0        0     2438 2020-02-02 00:00:00.000000 pyeventmanager-0.5.1/.github/workflows/ci.yml
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 pyeventmanager-0.5.1/.github/workflows/docs.yml
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 pyeventmanager-0.5.1/event_manager/__init__.py
--rw-r--r--   0        0        0     5291 2020-02-02 00:00:00.000000 pyeventmanager-0.5.1/event_manager/event_manager.py
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 pyeventmanager-0.5.1/event_manager/fork_types.py
--rw-r--r--   0        0        0     6064 2020-02-02 00:00:00.000000 pyeventmanager-0.5.1/event_manager/tree.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyeventmanager-0.5.1/event_manager/listeners/__init__.py
--rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 pyeventmanager-0.5.1/event_manager/listeners/base.py
--rw-r--r--   0        0        0     6716 2020-02-02 00:00:00.000000 pyeventmanager-0.5.1/event_manager/listeners/batch.py
--rw-r--r--   0        0        0     2643 2020-02-02 00:00:00.000000 pyeventmanager-0.5.1/event_manager/listeners/scheduled.py
--rw-r--r--   0        0        0     2042 2020-02-02 00:00:00.000000 pyeventmanager-0.5.1/event_manager/listeners/simple.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyeventmanager-0.5.1/event_manager/queues/__init__.py
--rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 pyeventmanager-0.5.1/event_manager/queues/base.py
--rw-r--r--   0        0        0     2104 2020-02-02 00:00:00.000000 pyeventmanager-0.5.1/event_manager/queues/memory.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyeventmanager-0.5.1/tests/__init__.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 pyeventmanager-0.5.1/tests/test_dummy.py
--rw-r--r--   0        0        0     3122 2020-02-02 00:00:00.000000 pyeventmanager-0.5.1/.gitignore
--rw-r--r--   0        0        0     6235 2020-02-02 00:00:00.000000 pyeventmanager-0.5.1/README.md
--rw-r--r--   0        0        0     2083 2020-02-02 00:00:00.000000 pyeventmanager-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     6924 2020-02-02 00:00:00.000000 pyeventmanager-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     4313 2020-02-02 00:00:00.000000 pyeventmanager-0.5.2/CHANGELOG.md
+-rw-r--r--   0        0        0     2438 2020-02-02 00:00:00.000000 pyeventmanager-0.5.2/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 pyeventmanager-0.5.2/.github/workflows/docs.yml
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 pyeventmanager-0.5.2/event_manager/__init__.py
+-rw-r--r--   0        0        0     5290 2020-02-02 00:00:00.000000 pyeventmanager-0.5.2/event_manager/event_manager.py
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 pyeventmanager-0.5.2/event_manager/fork_types.py
+-rw-r--r--   0        0        0     6060 2020-02-02 00:00:00.000000 pyeventmanager-0.5.2/event_manager/tree.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyeventmanager-0.5.2/event_manager/listeners/__init__.py
+-rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 pyeventmanager-0.5.2/event_manager/listeners/base.py
+-rw-r--r--   0        0        0     6744 2020-02-02 00:00:00.000000 pyeventmanager-0.5.2/event_manager/listeners/batch.py
+-rw-r--r--   0        0        0     2642 2020-02-02 00:00:00.000000 pyeventmanager-0.5.2/event_manager/listeners/scheduled.py
+-rw-r--r--   0        0        0     2042 2020-02-02 00:00:00.000000 pyeventmanager-0.5.2/event_manager/listeners/simple.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyeventmanager-0.5.2/event_manager/queues/__init__.py
+-rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 pyeventmanager-0.5.2/event_manager/queues/base.py
+-rw-r--r--   0        0        0     2104 2020-02-02 00:00:00.000000 pyeventmanager-0.5.2/event_manager/queues/memory.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyeventmanager-0.5.2/tests/__init__.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 pyeventmanager-0.5.2/tests/test_dummy.py
+-rw-r--r--   0        0        0     3122 2020-02-02 00:00:00.000000 pyeventmanager-0.5.2/.gitignore
+-rw-r--r--   0        0        0     6265 2020-02-02 00:00:00.000000 pyeventmanager-0.5.2/README.md
+-rw-r--r--   0        0        0     2083 2020-02-02 00:00:00.000000 pyeventmanager-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0     6954 2020-02-02 00:00:00.000000 pyeventmanager-0.5.2/PKG-INFO
```

### Comparing `pyeventmanager-0.5.1/CHANGELOG.md` & `pyeventmanager-0.5.2/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,16 @@
 # Changelog
 
+## [0.5.2](https://github.com/JeordyR/PyEventManager/compare/v0.5.1...v0.5.2) (2024-04-06)
+
+
+### Bug Fixes
+
+* fix batch to handle 0 batch_count, EventManager methods to classmethods, schedule listener to daemon ([c503205](https://github.com/JeordyR/PyEventManager/commit/c5032051d44e561734a4797d43cde1f3a07be3eb))
+
 ## [0.5.1](https://github.com/JeordyR/PyEventManager/compare/v0.5.0...v0.5.1) (2024-04-02)
 
 
 ### Bug Fixes
 
 * update interfaces to use Protocol instead of abc ([d028702](https://github.com/JeordyR/PyEventManager/commit/d0287024b52ef6f13ebb2a7b560b4e23496316a3))
```

### Comparing `pyeventmanager-0.5.1/.github/workflows/ci.yml` & `pyeventmanager-0.5.2/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `pyeventmanager-0.5.1/.github/workflows/docs.yml` & `pyeventmanager-0.5.2/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `pyeventmanager-0.5.1/event_manager/event_manager.py` & `pyeventmanager-0.5.2/event_manager/event_manager.py`

 * *Files 11% similar despite different names*

```diff
@@ -20,49 +20,51 @@
 logger = logging.getLogger("event_manager")
 
 
 class EventManager:
     _event_tree = Tree()
     _scheduled_listeners: list[ScheduledListener] = []
 
-    @staticmethod
+    @classmethod
     def on(
+        cls,
         event: list[str] | str,
         func: Callable | None = None,
         fork_type: ForkType = ForkType.PROCESS,
     ):
         if isinstance(event, str):
             event = [event]
 
         def _on(func: Callable) -> Callable:
             for e in event:
                 logger.info(f"Registered function {func.__name__} to run on {e} event.")
-                EventManager._event_tree.add_data(name=e, data=Listener(func=func, event=e, fork_type=fork_type))
+                cls._event_tree.add_data(name=e, data=Listener(func=func, event=e, fork_type=fork_type))
 
             return func
 
         return _on(func) if func else _on
 
-    @staticmethod
+    @classmethod
     def on_batch(
+        cls,
         event: list[str] | str,
         func: Callable | None = None,
         fork_type: ForkType = ForkType.PROCESS,
         batch_count: int = 0,
         batch_idle_window: int = 0,
         batch_window: int = 30,
         queue_type: type[QueueInterface] = ProcessQueue,
     ):
         if isinstance(event, str):
             event = [event]
 
         def _on_batch(func: Callable) -> Callable:
             for e in event:
                 logger.info(f"Registered function {func.__name__} to run on {e} event.")
-                EventManager._event_tree.add_data(
+                cls._event_tree.add_data(
                     name=e,
                     data=BatchListener(
                         event=e,
                         func=func,
                         fork_type=fork_type,
                         batch_count=batch_count,
                         batch_idle_window=batch_idle_window,
@@ -71,16 +73,17 @@
                     ),
                 )
 
             return func
 
         return _on_batch(func) if func else _on_batch
 
-    @staticmethod
+    @classmethod
     def schedule(
+        cls,
         interval: timedelta,
         func: Callable[[None], None] | None = None,
         fork_type: ForkType = ForkType.PROCESS,
     ) -> Callable:
         """
         Registers a scheduled function that will be executed on the specified interval.
 
@@ -93,44 +96,44 @@
             Callable: Returns the registered function, for use in decorators.
         """
 
         def schedule(func: Callable) -> Callable:
             logger.info(f"Scheduling {func.__name__} to run every {interval.total_seconds()} seconds.")
             listener = ScheduledListener(interval=interval, func=func, fork_type=fork_type)
             listener()
-            EventManager._scheduled_listeners.append(listener)
+            cls._scheduled_listeners.append(listener)
             return func
 
         return schedule(func) if func else schedule
 
-    @staticmethod
-    def listeners(event: str) -> list[Callable]:
+    @classmethod
+    def listeners(cls, event: str) -> list[Callable]:
         """
         Returns all functions that are registered to an event.
 
         Args:
             event (str): Event to get listeners for.
 
         Returns:
             list[Callable]: List of functions registered to the provided event.
         """
-        return [listener.func for listener in EventManager._event_tree.find_data(event)]
+        return [listener.func for listener in cls._event_tree.find_data(event)]
 
-    @staticmethod
-    def emit(event: str, *args, **kwargs) -> list[Future]:
+    @classmethod
+    def emit(cls, event: str, *args, **kwargs) -> list[Future]:
         """
         Emit an event into the system, calling all functions listening for the provided event.
 
         Args:
             event (str): Event to emit into the system.
 
         Returns:
             list[Future]: List of futures from the executed listeners.
         """
-        listeners = EventManager._event_tree.find_data(name=event)
+        listeners = cls._event_tree.find_data(name=event)
 
         logger.debug(f"{event} event emitted, executing on {len(listeners)} listener functions")
 
         futures = []
 
         # call listeners
         for listener in listeners:
```

### Comparing `pyeventmanager-0.5.1/event_manager/tree.py` & `pyeventmanager-0.5.2/event_manager/tree.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import collections
 import fnmatch
 from typing import Any
 
 
 class Node:
-    @classmethod
-    def str_is_pattern(cls, s: str) -> bool:
+    @staticmethod
+    def str_is_pattern(s: str) -> bool:
         """
         Check if the provided string is a pattern or not.
 
         Args:
             s (str): String to check for pattern contents.
 
         Returns:
```

### Comparing `pyeventmanager-0.5.1/event_manager/listeners/base.py` & `pyeventmanager-0.5.2/event_manager/listeners/base.py`

 * *Files identical despite different names*

### Comparing `pyeventmanager-0.5.1/event_manager/listeners/batch.py` & `pyeventmanager-0.5.2/event_manager/listeners/batch.py`

 * *Files 7% similar despite different names*

```diff
@@ -33,31 +33,31 @@
     while True:
         print("looping...")
         time.sleep(sleep_time)
         elapsed += 1
 
         logger.debug(f"{callback.__name__}: {queue.last_updated=}")
 
-        if len(queue) >= batch_count:
+        if batch_count > 0 and len(queue) >= batch_count:
             print("breaking for batch count...")
             break
-        elif batch_idle_window and queue.last_updated:
+        elif batch_idle_window > 0 and queue.last_updated:
             since_last = datetime.now() - queue.last_updated
             since_last = since_last.seconds
             logger.debug(f"{callback.__name__}: {since_last=}")
 
             if since_last > batch_idle_window:
                 print("breaking for idle window...")
                 break
             else:
                 print("waiting for idle window...")
                 logger.info(
                     f"Batch data updated too recently for func {callback.__name__}, waiting {batch_window} seconds."
                 )
-        elif batch_window and batch_window <= elapsed:
+        elif batch_window > 0 and batch_window <= elapsed:
             print("breaking for batch window...")
             break
 
     logger.debug(f"Batching complete for {callback.__name__}, executing...")
 
     if batch_count > 0:
         return callback(queue.get_all())
```

### Comparing `pyeventmanager-0.5.1/event_manager/listeners/scheduled.py` & `pyeventmanager-0.5.2/event_manager/listeners/scheduled.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,15 +62,15 @@
         kwargs = {
             "_interval": self.interval,
             "_func": self.func,
             "_event": self.sync_event,
             **kwargs,
         }
 
-        self.fork_type.value(target=run, daemon=False, args=args, kwargs=kwargs).start()
+        self.fork_type.value(target=run, daemon=True, args=args, kwargs=kwargs).start()
 
     def stop(self):
         """
         Stop the scheduled listener.
         """
         logger.debug(f"Stopping {self.func.__name__} from running on schedule.")
         self.sync_event.set()
```

### Comparing `pyeventmanager-0.5.1/event_manager/listeners/simple.py` & `pyeventmanager-0.5.2/event_manager/listeners/simple.py`

 * *Files identical despite different names*

### Comparing `pyeventmanager-0.5.1/event_manager/queues/base.py` & `pyeventmanager-0.5.2/event_manager/queues/base.py`

 * *Files identical despite different names*

### Comparing `pyeventmanager-0.5.1/event_manager/queues/memory.py` & `pyeventmanager-0.5.2/event_manager/queues/memory.py`

 * *Files identical despite different names*

### Comparing `pyeventmanager-0.5.1/.gitignore` & `pyeventmanager-0.5.2/.gitignore`

 * *Files identical despite different names*

### Comparing `pyeventmanager-0.5.1/README.md` & `pyeventmanager-0.5.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 * **Process(Default)**: The listener is run in a new Process
 * **Thread**: The listener is run in a new Thread
 
 ---
 
 ## Todo
 
+* Clean up/improve docstrings
 * Add tests
 * Add support for async execution within an existing event loop
 * Add support for external data stores (redis, rabbitmq?, etc.) for persistence of event data / batching
 
 
 ---
```

### Comparing `pyeventmanager-0.5.1/pyproject.toml` & `pyeventmanager-0.5.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pyeventmanager"
-version = "0.5.1"
+version = "0.5.2"
 authors = [{ name = "Jeordy", email = "JeordyR@users.noreply.github.com" }]
 description = "Event management system for Python with support for Threading and Multiprocessing for task running."
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
```

### Comparing `pyeventmanager-0.5.1/PKG-INFO` & `pyeventmanager-0.5.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pyeventmanager
-Version: 0.5.1
+Version: 0.5.2
 Summary: Event management system for Python with support for Threading and Multiprocessing for task running.
 Project-URL: Documentation, https://event-manager.jeofi.com
 Project-URL: Homepage, https://event-manager.jeofi.com
 Project-URL: Repository, https://github.com/JeordyR/PyEventManager
 Project-URL: Issues, https://github.com/JeordyR/PyEventManager/issues
 Author-email: Jeordy <JeordyR@users.noreply.github.com>
 Classifier: Operating System :: OS Independent
@@ -34,14 +34,15 @@
 * **Process(Default)**: The listener is run in a new Process
 * **Thread**: The listener is run in a new Thread
 
 ---
 
 ## Todo
 
+* Clean up/improve docstrings
 * Add tests
 * Add support for async execution within an existing event loop
 * Add support for external data stores (redis, rabbitmq?, etc.) for persistence of event data / batching
 
 
 ---
```

