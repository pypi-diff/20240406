# Comparing `tmp/deltachat2-0.3.0.tar.gz` & `tmp/deltachat2-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deltachat2-0.3.0.tar", last modified: Wed Apr  3 18:26:08 2024, max compression
+gzip compressed data, was "deltachat2-0.4.0.tar", last modified: Sat Apr  6 20:45:30 2024, max compression
```

## Comparing `deltachat2-0.3.0.tar` & `deltachat2-0.4.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:26:08.728854 deltachat2-0.3.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:26:08.720854 deltachat2-0.3.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:26:08.720854 deltachat2-0.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-04-03 18:25:55.000000 deltachat2-0.3.0/.github/workflows/python-ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-03 18:25:55.000000 deltachat2-0.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    16726 2024-04-03 18:25:55.000000 deltachat2-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2512 2024-04-03 18:26:08.724854 deltachat2-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-04-03 18:25:55.000000 deltachat2-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:26:08.724854 deltachat2-0.3.0/deltachat2/
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-03 18:25:55.000000 deltachat2-0.3.0/deltachat2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-04-03 18:25:55.000000 deltachat2-0.3.0/deltachat2/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4204 2024-04-03 18:25:55.000000 deltachat2-0.3.0/deltachat2/bot.py
--rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-04-03 18:25:55.000000 deltachat2-0.3.0/deltachat2/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     7140 2024-04-03 18:25:55.000000 deltachat2-0.3.0/deltachat2/events.py
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-04-03 18:25:55.000000 deltachat2-0.3.0/deltachat2/rpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     5092 2024-04-03 18:25:55.000000 deltachat2-0.3.0/deltachat2/transport.py
--rw-r--r--   0 runner    (1001) docker     (127)     6018 2024-04-03 18:25:55.000000 deltachat2-0.3.0/deltachat2/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     2394 2024-04-03 18:25:55.000000 deltachat2-0.3.0/deltachat2/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:26:08.724854 deltachat2-0.3.0/deltachat2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2512 2024-04-03 18:26:08.000000 deltachat2-0.3.0/deltachat2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-03 18:26:08.000000 deltachat2-0.3.0/deltachat2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 18:26:08.000000 deltachat2-0.3.0/deltachat2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-03 18:26:08.000000 deltachat2-0.3.0/deltachat2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-03 18:26:08.000000 deltachat2-0.3.0/deltachat2.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:26:08.724854 deltachat2-0.3.0/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-04-03 18:25:55.000000 deltachat2-0.3.0/examples/client.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1256 2024-04-03 18:25:55.000000 deltachat2-0.3.0/examples/echobot.py
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-03 18:25:55.000000 deltachat2-0.3.0/pylama.ini
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-04-03 18:25:55.000000 deltachat2-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 18:26:08.728854 deltachat2-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 20:45:30.865841 deltachat2-0.4.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 20:45:30.861841 deltachat2-0.4.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 20:45:30.861841 deltachat2-0.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-04-06 20:45:19.000000 deltachat2-0.4.0/.github/workflows/python-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-06 20:45:19.000000 deltachat2-0.4.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    16726 2024-04-06 20:45:19.000000 deltachat2-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2512 2024-04-06 20:45:30.865841 deltachat2-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-04-06 20:45:19.000000 deltachat2-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 20:45:30.865841 deltachat2-0.4.0/deltachat2/
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-06 20:45:19.000000 deltachat2-0.4.0/deltachat2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-04-06 20:45:19.000000 deltachat2-0.4.0/deltachat2/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4401 2024-04-06 20:45:19.000000 deltachat2-0.4.0/deltachat2/bot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-04-06 20:45:19.000000 deltachat2-0.4.0/deltachat2/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7140 2024-04-06 20:45:19.000000 deltachat2-0.4.0/deltachat2/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-04-06 20:45:19.000000 deltachat2-0.4.0/deltachat2/rpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5092 2024-04-06 20:45:19.000000 deltachat2-0.4.0/deltachat2/transport.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6018 2024-04-06 20:45:19.000000 deltachat2-0.4.0/deltachat2/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2394 2024-04-06 20:45:19.000000 deltachat2-0.4.0/deltachat2/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 20:45:30.865841 deltachat2-0.4.0/deltachat2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2512 2024-04-06 20:45:30.000000 deltachat2-0.4.0/deltachat2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-06 20:45:30.000000 deltachat2-0.4.0/deltachat2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 20:45:30.000000 deltachat2-0.4.0/deltachat2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-06 20:45:30.000000 deltachat2-0.4.0/deltachat2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-06 20:45:30.000000 deltachat2-0.4.0/deltachat2.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 20:45:30.865841 deltachat2-0.4.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-04-06 20:45:19.000000 deltachat2-0.4.0/examples/client.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1256 2024-04-06 20:45:19.000000 deltachat2-0.4.0/examples/echobot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-06 20:45:19.000000 deltachat2-0.4.0/pylama.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-04-06 20:45:19.000000 deltachat2-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 20:45:30.865841 deltachat2-0.4.0/setup.cfg
```

### Comparing `deltachat2-0.3.0/.github/workflows/python-ci.yml` & `deltachat2-0.4.0/.github/workflows/python-ci.yml`

 * *Files identical despite different names*

### Comparing `deltachat2-0.3.0/LICENSE` & `deltachat2-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `deltachat2-0.3.0/PKG-INFO` & `deltachat2-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deltachat2
-Version: 0.3.0
+Version: 0.4.0
 Summary: Client library for Delta Chat core JSON-RPC interface
 Author-email: adbenitez <adb@merlinux.eu>
 Keywords: deltachat
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
```

### Comparing `deltachat2-0.3.0/README.md` & `deltachat2-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `deltachat2-0.3.0/deltachat2/_utils.py` & `deltachat2-0.4.0/deltachat2/_utils.py`

 * *Files identical despite different names*

### Comparing `deltachat2-0.3.0/deltachat2/bot.py` & `deltachat2-0.4.0/deltachat2/bot.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,18 +6,19 @@
 from .client import Client
 from .events import EventFilter, HookCallback, NewMessage
 from .rpc import Rpc
 from .types import Event, EventType, Message, NewMsgEvent, SpecialContactId
 
 
 class Bot(Client):
-    """A Delta Chat client with the bot flag set.
+    """A Delta Chat client with the bot setting set to 1.
 
     This bot client triggers "NewMessage" highlevel events
-    in addition to raw core events.
+    in addition to raw core events. The account will have the settings bcc_self set to 0,
+    and delete_server_after set to 1.
     """
 
     def __init__(
         self,
         rpc: Rpc,
         hooks: Optional[Iterable[Tuple[HookCallback, Union[type, EventFilter]]]] = None,
         logger: Optional[logging.Logger] = None,
@@ -27,14 +28,16 @@
         self.command_prefix = command_prefix
         logger = logger or logging.getLogger("deltachat2.Bot")
         super().__init__(rpc, hooks, logger)
 
     def configure(self, account_id: int, email: str, password: str, **kwargs) -> None:
         """Configure the account with the given account ID."""
         kwargs.setdefault("bot", "1")
+        kwargs.setdefault("delete_server_after", "1")
+        kwargs.setdefault("bcc_self", "0")
         super().configure(account_id, email, password, **kwargs)
 
     def has_command(self, command: str) -> bool:
         """Return True if the bot has a hook/callback registered for the given command,
         False otherwise."""
         if not command or not command.startswith(self.command_prefix):
             return False
```

### Comparing `deltachat2-0.3.0/deltachat2/client.py` & `deltachat2-0.4.0/deltachat2/client.py`

 * *Files identical despite different names*

### Comparing `deltachat2-0.3.0/deltachat2/events.py` & `deltachat2-0.4.0/deltachat2/events.py`

 * *Files identical despite different names*

### Comparing `deltachat2-0.3.0/deltachat2/rpc.py` & `deltachat2-0.4.0/deltachat2/rpc.py`

 * *Files identical despite different names*

### Comparing `deltachat2-0.3.0/deltachat2/transport.py` & `deltachat2-0.4.0/deltachat2/transport.py`

 * *Files identical despite different names*

### Comparing `deltachat2-0.3.0/deltachat2/types.py` & `deltachat2-0.4.0/deltachat2/types.py`

 * *Files identical despite different names*

### Comparing `deltachat2-0.3.0/deltachat2/util.py` & `deltachat2-0.4.0/deltachat2/util.py`

 * *Files identical despite different names*

### Comparing `deltachat2-0.3.0/deltachat2.egg-info/PKG-INFO` & `deltachat2-0.4.0/deltachat2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deltachat2
-Version: 0.3.0
+Version: 0.4.0
 Summary: Client library for Delta Chat core JSON-RPC interface
 Author-email: adbenitez <adb@merlinux.eu>
 Keywords: deltachat
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
```

### Comparing `deltachat2-0.3.0/examples/client.py` & `deltachat2-0.4.0/examples/client.py`

 * *Files identical despite different names*

### Comparing `deltachat2-0.3.0/examples/echobot.py` & `deltachat2-0.4.0/examples/echobot.py`

 * *Files identical despite different names*

### Comparing `deltachat2-0.3.0/pyproject.toml` & `deltachat2-0.4.0/pyproject.toml`

 * *Files identical despite different names*

