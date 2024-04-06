# Comparing `tmp/deltabot-cli-6.0.0.tar.gz` & `tmp/deltabot-cli-6.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deltabot-cli-6.0.0.tar", last modified: Fri Mar 29 19:20:18 2024, max compression
+gzip compressed data, was "deltabot-cli-6.0.1.tar", last modified: Sat Apr  6 20:47:00 2024, max compression
```

## Comparing `deltabot-cli-6.0.0.tar` & `deltabot-cli-6.0.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 19:20:18.676833 deltabot-cli-6.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 19:20:18.672832 deltabot-cli-6.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 19:20:18.672832 deltabot-cli-6.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-03-29 19:20:05.000000 deltabot-cli-6.0.0/.github/workflows/python-ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-03-29 19:20:05.000000 deltabot-cli-6.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    16726 2024-03-29 19:20:05.000000 deltabot-cli-6.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-03-29 19:20:18.676833 deltabot-cli-6.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-03-29 19:20:05.000000 deltabot-cli-6.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 19:20:18.672832 deltabot-cli-6.0.0/deltabot_cli/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-29 19:20:05.000000 deltabot-cli-6.0.0/deltabot_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-03-29 19:20:05.000000 deltabot-cli-6.0.0/deltabot_cli/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    13259 2024-03-29 19:20:05.000000 deltabot-cli-6.0.0/deltabot_cli/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 19:20:18.676833 deltabot-cli-6.0.0/deltabot_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-03-29 19:20:18.000000 deltabot-cli-6.0.0/deltabot_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-03-29 19:20:18.000000 deltabot-cli-6.0.0/deltabot_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 19:20:18.000000 deltabot-cli-6.0.0/deltabot_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-03-29 19:20:18.000000 deltabot-cli-6.0.0/deltabot_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-03-29 19:20:18.000000 deltabot-cli-6.0.0/deltabot_cli.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 19:20:18.676833 deltabot-cli-6.0.0/examples/
--rwxr-xr-x   0 runner    (1001) docker     (127)      504 2024-03-29 19:20:05.000000 deltabot-cli-6.0.0/examples/echobot.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2370 2024-03-29 19:20:05.000000 deltabot-cli-6.0.0/examples/echobot_advanced.py
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-03-29 19:20:05.000000 deltabot-cli-6.0.0/pylama.ini
--rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-03-29 19:20:05.000000 deltabot-cli-6.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-29 19:20:18.676833 deltabot-cli-6.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 20:47:00.137868 deltabot-cli-6.0.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 20:47:00.129868 deltabot-cli-6.0.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 20:47:00.133868 deltabot-cli-6.0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-04-06 20:46:43.000000 deltabot-cli-6.0.1/.github/workflows/python-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-06 20:46:43.000000 deltabot-cli-6.0.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    16726 2024-04-06 20:46:43.000000 deltabot-cli-6.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-04-06 20:47:00.133868 deltabot-cli-6.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-04-06 20:46:43.000000 deltabot-cli-6.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 20:47:00.133868 deltabot-cli-6.0.1/deltabot_cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-06 20:46:43.000000 deltabot-cli-6.0.1/deltabot_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-04-06 20:46:43.000000 deltabot-cli-6.0.1/deltabot_cli/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13272 2024-04-06 20:46:43.000000 deltabot-cli-6.0.1/deltabot_cli/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 20:47:00.133868 deltabot-cli-6.0.1/deltabot_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-04-06 20:47:00.000000 deltabot-cli-6.0.1/deltabot_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-06 20:47:00.000000 deltabot-cli-6.0.1/deltabot_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 20:47:00.000000 deltabot-cli-6.0.1/deltabot_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-06 20:47:00.000000 deltabot-cli-6.0.1/deltabot_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-06 20:47:00.000000 deltabot-cli-6.0.1/deltabot_cli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 20:47:00.133868 deltabot-cli-6.0.1/examples/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      504 2024-04-06 20:46:43.000000 deltabot-cli-6.0.1/examples/echobot.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2270 2024-04-06 20:46:43.000000 deltabot-cli-6.0.1/examples/echobot_advanced.py
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-06 20:46:43.000000 deltabot-cli-6.0.1/pylama.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-04-06 20:46:43.000000 deltabot-cli-6.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 20:47:00.137868 deltabot-cli-6.0.1/setup.cfg
```

### Comparing `deltabot-cli-6.0.0/.github/workflows/python-ci.yml` & `deltabot-cli-6.0.1/.github/workflows/python-ci.yml`

 * *Files identical despite different names*

### Comparing `deltabot-cli-6.0.0/LICENSE` & `deltabot-cli-6.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `deltabot-cli-6.0.0/PKG-INFO` & `deltabot-cli-6.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deltabot-cli
-Version: 6.0.0
+Version: 6.0.1
 Summary: Library to speedup Delta Chat bot development
 Author-email: adbenitez <adb@merlinux.eu>
 Keywords: deltachat,bot,deltabot-cli
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
```

### Comparing `deltabot-cli-6.0.0/README.md` & `deltabot-cli-6.0.1/README.md`

 * *Files identical despite different names*

### Comparing `deltabot-cli-6.0.0/deltabot_cli/_utils.py` & `deltabot-cli-6.0.1/deltabot_cli/_utils.py`

 * *Files identical despite different names*

### Comparing `deltabot-cli-6.0.0/deltabot_cli/cli.py` & `deltabot-cli-6.0.1/deltabot_cli/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -201,15 +201,15 @@
         if not accid:
             bot.logger.error(f"unknown account: {args.account!r}")
             sys.exit(1)
     else:
         accid = cli.get_or_create_account(bot.rpc, args.addr)
 
     bot.logger.info("Starting configuration process...")
-    task = Thread(target=configure)
+    task = Thread(target=configure, daemon=True)
     task.start()
     pbar = ConfigProgressBar()
     while True:
         raw_event = bot.rpc.get_next_event()
         accid = raw_event.context_id
         event = raw_event.event
         if event.kind == EventType.CONFIGURE_PROGRESS:
```

### Comparing `deltabot-cli-6.0.0/deltabot_cli.egg-info/PKG-INFO` & `deltabot-cli-6.0.1/deltabot_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deltabot-cli
-Version: 6.0.0
+Version: 6.0.1
 Summary: Library to speedup Delta Chat bot development
 Author-email: adbenitez <adb@merlinux.eu>
 Keywords: deltachat,bot,deltabot-cli
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
```

### Comparing `deltabot-cli-6.0.0/examples/echobot_advanced.py` & `deltabot-cli-6.0.1/examples/echobot_advanced.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 def on_init(bot, args):
     bot.logger.info("Initializing CLI with args: %s", args)
     for accid in bot.rpc.get_all_account_ids():
         if not bot.rpc.get_config(accid, "displayname"):
             bot.rpc.set_config(accid, "displayname", "EchoBot")
             status = "I am a Delta Chat bot, I will repeat anything you say to me"
             bot.rpc.set_config(accid, "selfstatus", status)
-            bot.rpc.set_config(accid, "delete_server_after", "1")  # delete immediately from server
             # bot.rpc.set_config(accid, "delete_device_after", "3600")
 
 
 @cli.on_start
 def on_start(bot, _args):
     bot.logger.info(
         "Bot is listening to requests... here connect to databases, start worker threads, etc"
```

### Comparing `deltabot-cli-6.0.0/pyproject.toml` & `deltabot-cli-6.0.1/pyproject.toml`

 * *Files identical despite different names*

