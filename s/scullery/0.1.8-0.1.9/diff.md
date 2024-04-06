# Comparing `tmp/scullery-0.1.8.tar.gz` & `tmp/scullery-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scullery-0.1.8.tar", last modified: Wed Dec 15 18:40:36 2021, max compression
+gzip compressed data, was "scullery-0.1.9.tar", last modified: Wed Nov  8 08:03:49 2023, max compression
```

## Comparing `scullery-0.1.8.tar` & `scullery-0.1.9.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-15 18:40:36.824534 scullery-0.1.8/
--rw-rw-r--   0 root         (0) root         (0)       79 2021-12-15 18:40:34.000000 scullery-0.1.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    12600 2021-12-15 18:40:36.820534 scullery-0.1.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     9855 2021-12-15 15:50:46.000000 scullery-0.1.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-15 18:40:36.820534 scullery-0.1.8/scullery/
--rw-r--r--   0 root         (0) root         (0)       20 2020-01-08 05:53:44.000000 scullery-0.1.8/scullery/__init__.py
--rw-------   0 root         (0) root         (0)     7260 2021-12-15 16:27:28.000000 scullery-0.1.8/scullery/fluidsynth.py
--rw-rw-r--   0 root         (0) root         (0)     3423 2021-12-15 16:06:32.000000 scullery-0.1.8/scullery/iceflow.py
--rw-rw-r--   0 root         (0) root         (0)    37044 2021-12-12 22:26:40.000000 scullery-0.1.8/scullery/iceflow_server.py
--rw-rw-r--   0 root         (0) root         (0)     5999 2021-12-12 22:26:40.000000 scullery-0.1.8/scullery/jack_client_subprocess.py
--rw-rw-r--   0 root         (0) root         (0)    81959 2021-12-15 16:32:44.000000 scullery-0.1.8/scullery/jacktools.py
--rw-rw-r--   0 root         (0) root         (0)    22036 2021-11-28 03:32:40.000000 scullery-0.1.8/scullery/jsonrpyc.py
--rw-rw-r--   0 root         (0) root         (0)    12031 2021-11-22 01:52:00.000000 scullery-0.1.8/scullery/messagebus.py
--rw-r--r--   0 root         (0) root         (0)      899 2020-01-23 21:56:29.000000 scullery-0.1.8/scullery/mnemonics.py
--rw-rw-r--   0 root         (0) root         (0)    21668 2021-12-15 18:20:08.000000 scullery-0.1.8/scullery/mqtt.py
--rw-rw-r--   0 root         (0) root         (0)     8116 2020-06-15 00:57:32.000000 scullery-0.1.8/scullery/persist.py
--rw-r--r--   0 root         (0) root         (0)      309 2020-03-03 22:43:47.000000 scullery-0.1.8/scullery/pulse_jack_rc.txt
--rw-------   0 root         (0) root         (0)     3942 2021-09-14 08:47:57.000000 scullery-0.1.8/scullery/sip.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-15 18:40:36.820534 scullery-0.1.8/scullery/thirdparty/
--rw-r--r--   0 root         (0) root         (0)        0 2020-01-13 13:26:44.000000 scullery-0.1.8/scullery/thirdparty/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-15 18:40:36.820534 scullery-0.1.8/scullery/thirdparty/baresipy/
--rw-rw-r--   0 root         (0) root         (0)    16836 2021-11-06 01:16:29.000000 scullery-0.1.8/scullery/thirdparty/baresipy/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-15 18:40:36.820534 scullery-0.1.8/scullery/thirdparty/baresipy/baresip_template/
--rw-rw-r--   0 root         (0) root         (0)     1084 2020-06-22 18:09:20.000000 scullery-0.1.8/scullery/thirdparty/baresipy/baresip_template/accounts
--rw-rw-r--   0 root         (0) root         (0)     4181 2020-06-22 18:09:20.000000 scullery-0.1.8/scullery/thirdparty/baresipy/baresip_template/config
--rw-rw-r--   0 root         (0) root         (0)      317 2020-06-22 18:09:20.000000 scullery-0.1.8/scullery/thirdparty/baresipy/baresip_template/contacts
--rw-rw-r--   0 root         (0) root         (0)       20 2020-06-22 18:09:20.000000 scullery-0.1.8/scullery/thirdparty/baresipy/baresip_template/current_contact
--rw-rw-r--   0 root         (0) root         (0)       36 2020-06-22 18:09:20.000000 scullery-0.1.8/scullery/thirdparty/baresipy/baresip_template/uuid
--rw-rw-r--   0 root         (0) root         (0)     3383 2020-06-22 18:09:20.000000 scullery-0.1.8/scullery/thirdparty/baresipy/contacts.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-15 18:40:36.820534 scullery-0.1.8/scullery/thirdparty/baresipy/utils/
--rw-rw-r--   0 root         (0) root         (0)      257 2020-06-22 18:09:20.000000 scullery-0.1.8/scullery/thirdparty/baresipy/utils/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     3097 2020-06-22 18:09:20.000000 scullery-0.1.8/scullery/thirdparty/baresipy/utils/log.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-15 18:40:36.820534 scullery-0.1.8/scullery/thirdparty/fluidsynth/
--rw-rw-r--   0 root         (0) root         (0)    51002 2020-05-04 05:42:40.000000 scullery-0.1.8/scullery/thirdparty/fluidsynth/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    10315 2021-11-28 03:32:40.000000 scullery-0.1.8/scullery/units.py
--rw-rw-r--   0 root         (0) root         (0)     1230 2020-06-15 00:57:32.000000 scullery-0.1.8/scullery/util.py
--rw-r--r--   0 root         (0) root         (0)    11018 2020-01-13 13:26:44.000000 scullery-0.1.8/scullery/words_mnemonic.txt
--rw-rw-r--   0 root         (0) root         (0)     9765 2021-12-15 15:56:24.000000 scullery-0.1.8/scullery/workers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-15 18:40:36.820534 scullery-0.1.8/scullery.egg-info/
--rw-r--r--   0 root         (0) root         (0)    12600 2021-12-15 18:40:36.000000 scullery-0.1.8/scullery.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1248 2021-12-15 18:40:36.000000 scullery-0.1.8/scullery.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-12-15 18:40:36.000000 scullery-0.1.8/scullery.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       56 2021-12-15 18:40:36.000000 scullery-0.1.8/scullery.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2021-12-15 18:40:36.000000 scullery-0.1.8/scullery.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2021-12-15 18:40:36.824534 scullery-0.1.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1015 2021-12-15 18:38:43.000000 scullery-0.1.8/setup.py
--rw-r--r--   0 root         (0) root         (0)        9 2020-01-08 06:55:45.000000 scullery-0.1.8/testFile.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-15 18:40:36.820534 scullery-0.1.8/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2020-01-09 03:57:31.000000 scullery-0.1.8/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)      673 2021-12-15 16:35:59.000000 scullery-0.1.8/tests/testFluidSynth.py
--rw-r--r--   0 root         (0) root         (0)     2326 2021-12-15 16:22:20.000000 scullery-0.1.8/tests/testGstStability.py
--rw-r--r--   0 root         (0) root         (0)     1787 2021-12-15 16:04:04.000000 scullery-0.1.8/tests/testJack.py
--rw-rw-r--   0 root         (0) root         (0)     1752 2020-08-09 05:52:10.000000 scullery-0.1.8/tests/testMQTT.py
--rw-r--r--   0 root         (0) root         (0)     2076 2021-12-15 16:14:45.000000 scullery-0.1.8/tests/testMessageBus.py
--rw-r--r--   0 root         (0) root         (0)     1384 2020-01-30 10:47:15.000000 scullery-0.1.8/tests/testMisc.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-11-08 08:03:49.756659 scullery-0.1.9/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)    35149 2023-11-08 06:36:16.000000 scullery-0.1.9/LICENSE
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       79 2023-11-08 06:36:16.000000 scullery-0.1.9/MANIFEST.in
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     6412 2023-11-08 08:03:49.756659 scullery-0.1.9/PKG-INFO
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     5864 2023-11-08 07:34:26.000000 scullery-0.1.9/README.md
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-11-08 08:03:49.752659 scullery-0.1.9/scullery/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       20 2023-11-08 05:34:17.000000 scullery-0.1.9/scullery/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     7290 2023-11-08 05:34:17.000000 scullery-0.1.9/scullery/fluidsynth.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     7451 2023-11-08 05:34:17.000000 scullery-0.1.9/scullery/iceflow.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)    44312 2023-11-08 05:34:17.000000 scullery-0.1.9/scullery/iceflow_server.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     6615 2023-11-08 05:34:17.000000 scullery-0.1.9/scullery/jack_client_subprocess.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)    35952 2023-11-08 05:34:17.000000 scullery-0.1.9/scullery/jacktools.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)    22618 2023-11-08 05:34:17.000000 scullery-0.1.9/scullery/jsonrpyc.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)    12394 2023-11-08 05:34:17.000000 scullery-0.1.9/scullery/messagebus.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      899 2023-11-08 05:34:17.000000 scullery-0.1.9/scullery/mnemonics.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)    16968 2023-11-08 05:34:17.000000 scullery-0.1.9/scullery/mqtt.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     8465 2023-11-08 05:34:17.000000 scullery-0.1.9/scullery/persist.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      309 2023-11-08 05:34:17.000000 scullery-0.1.9/scullery/pulse_jack_rc.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     3942 2023-11-08 05:34:17.000000 scullery-0.1.9/scullery/sip.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-11-08 08:03:49.752659 scullery-0.1.9/scullery/thirdparty/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2023-11-08 05:34:17.000000 scullery-0.1.9/scullery/thirdparty/__init__.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-11-08 08:03:49.752659 scullery-0.1.9/scullery/thirdparty/baresipy/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)    16836 2023-11-08 05:34:17.000000 scullery-0.1.9/scullery/thirdparty/baresipy/__init__.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-11-08 08:03:49.752659 scullery-0.1.9/scullery/thirdparty/baresipy/baresip_template/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1084 2023-11-08 05:34:17.000000 scullery-0.1.9/scullery/thirdparty/baresipy/baresip_template/accounts
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     4181 2023-11-08 05:34:17.000000 scullery-0.1.9/scullery/thirdparty/baresipy/baresip_template/config
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      317 2023-11-08 05:34:17.000000 scullery-0.1.9/scullery/thirdparty/baresipy/baresip_template/contacts
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       20 2023-11-08 05:34:17.000000 scullery-0.1.9/scullery/thirdparty/baresipy/baresip_template/current_contact
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       36 2023-11-08 05:34:17.000000 scullery-0.1.9/scullery/thirdparty/baresipy/baresip_template/uuid
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     3383 2023-11-08 05:34:17.000000 scullery-0.1.9/scullery/thirdparty/baresipy/contacts.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-11-08 08:03:49.756659 scullery-0.1.9/scullery/thirdparty/baresipy/utils/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      257 2023-11-08 05:34:17.000000 scullery-0.1.9/scullery/thirdparty/baresipy/utils/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     3097 2023-11-08 05:34:17.000000 scullery-0.1.9/scullery/thirdparty/baresipy/utils/log.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-11-08 08:03:49.756659 scullery-0.1.9/scullery/thirdparty/fluidsynth/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)    51002 2023-11-08 05:34:17.000000 scullery-0.1.9/scullery/thirdparty/fluidsynth/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)    10611 2023-11-08 05:34:17.000000 scullery-0.1.9/scullery/units.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1230 2023-11-08 05:34:17.000000 scullery-0.1.9/scullery/util.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)    11018 2023-11-08 05:34:17.000000 scullery-0.1.9/scullery/words_mnemonic.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)    11152 2023-11-08 05:34:17.000000 scullery-0.1.9/scullery/workers.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-11-08 08:03:49.752659 scullery-0.1.9/scullery.egg-info/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     6412 2023-11-08 08:03:49.000000 scullery-0.1.9/scullery.egg-info/PKG-INFO
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1242 2023-11-08 08:03:49.000000 scullery-0.1.9/scullery.egg-info/SOURCES.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        1 2023-11-08 08:03:49.000000 scullery-0.1.9/scullery.egg-info/dependency_links.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       49 2023-11-08 08:03:49.000000 scullery-0.1.9/scullery.egg-info/requires.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       15 2023-11-08 08:03:49.000000 scullery-0.1.9/scullery.egg-info/top_level.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       38 2023-11-08 08:03:49.756659 scullery-0.1.9/setup.cfg
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1059 2023-11-08 07:55:54.000000 scullery-0.1.9/setup.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-11-08 08:03:49.756659 scullery-0.1.9/tests/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2023-11-08 06:36:16.000000 scullery-0.1.9/tests/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      673 2023-11-08 06:36:16.000000 scullery-0.1.9/tests/testFluidSynth.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     2326 2023-11-08 06:36:16.000000 scullery-0.1.9/tests/testGstStability.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1787 2023-11-08 06:36:16.000000 scullery-0.1.9/tests/testJack.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1752 2023-11-08 06:36:16.000000 scullery-0.1.9/tests/testMQTT.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     2076 2023-11-08 06:36:16.000000 scullery-0.1.9/tests/testMessageBus.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1384 2023-11-08 06:36:16.000000 scullery-0.1.9/tests/testMisc.py
```

### Comparing `scullery-0.1.8/README.md` & `scullery-0.1.9/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,38 @@
+Metadata-Version: 2.1
+Name: scullery
+Version: 0.1.9
+Summary: A utility library based on KaithemAutomation featuring a GStreamer wrapper
+Home-page: https://github.com/EternityForest/scullery
+Author: Daniel Dunn
+Author-email: dannydunn@eternityforest.com
+License: UNKNOWN
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # scullery
-Python library for things like media playback, thread pools, and a message bus. It is essentially the parts of KaithemAutomation
-that make sense independantly.
 
-There is a lot of functionality planned, but it's not at all neccesary to use or understand all of it to use one piece.
+Python library that provides some core parts of KaithemAutomation, especially things related to media handling.
 
-You will obviously need the Python Gstreamer bindings for those features(but not unrelated features), and several other
-dependancies.
+* Data persistance
+* Message bus
+* Thread pool worker(At one point, Python did not natively have this, may be deprecated now that it does)
+* Media handling library that gives a much nicer interface to gstreamer.
+* JACK connection manager(No longer tested with actual JACK, meant for pipewire)
 
 
 
 ## Intro
 See example.py for more details. Also see the equally simple audio and video player.
 
-## Testing
-Warning, takes over audio, starts JACK, makes noise:python3 -m unittest discover tests
-
-Running just one test suite: python3 -m unittest tests/testFluidSynth.py
 
 ## Examples
 ```python
 import scullery.workers
 "This file demonstrates a lot of scullery's functionality in a small package"
 
 #Most things require this thread pool to be running
@@ -82,122 +95,34 @@
 #### scullery.units.convert(value,fromUnit, toUnit)
 Try to convert the value, falling back to the (very slow) pint library for less common conversions not natively
 supported.
 
 
 ### scullery.mqtt
 
-#### scullery.mqtt.getConnection(server, port=1883, password=None, messageBusName=None)
-
-Creates an MQTT connection. To speify username, use user@server.net syntax.
-
-To use an internal fake server for testing, use the server "__virtual__".
-
-This connection handles automatically reconnecting and resubscribing for you.  If a connection to a user@server already exists,
-it will return that connection.  
-
-All traffic goes through the internal message bus first, on topics that will begin with /mqtt/. Normally, the internal name is server+":"+port
-But you can specify it explicitly.  The topic name also acts as a sort of internal ID, and the system understands new connections with the same ID
-to be replacements for the old one. All subscriptions will carry over.
-
-Resubscriptions are stored in a master list.  If you subscribe, then delete the connection and recreate a new connection with the same message bus
-name, everything will carry on like nothing happened, so long as you kept a reference to the subscribed function.
-
-You can even create one connection, delete it, make a new one with the same internal messageBusName, to a different server, and all the old subscriptions
-will be "remade" at the new server, as the system knows that the new connection is a "replacement" for the old name.
-
-You cannot have two connections to the same user@server combo with different internal names or passwords, however, if you do not supply a password,
-and the existing connection has one, it will still work as it is simply returning the existing one.
-
-This feature is meant to make GUI config easier, so that changing a connection doesn't break all existing users of that connection.
-
-##### Passive connections
-
-If server is '', it will not create any real connections, but will still publish and subscribe to the internal
-bus, meaning that you can use it as a "passive" connection which uses a real connection configured elsewhere.
-
-Note that you will(currently) only recieve through passives if the backend also subscribed to that topic, subscribing through a passive
-connecting is truly passive, but this may change. At the moment, think of them like "spy" connections.
-
-To use a passive connection, you obviously need to specify the same messageBusName on the passive and backend.
-
-##### MQTTConnection.publish(self, topic, message, qos=2, encoding="json"):
-
-Encoding may be: json,msgpack, raw, utf8
-
-##### MQTTConnection.subscribe(self, topic, function, qos=2, encoding="json")
-Function is passed f(topic,message). 
-
-Scullery only weakly references, so if you delete or otherwise let the function be GCed, it is auto unsubscribed.
-
-##### MQTTConnection.unsubscribe(self, topic, function)
-Automatically unsubscribes from the actual MQTT topic when there are no more local subscribers. Note that subscriptions through a "
-
-
-
-
-
-# Everything below this should be moved to a separate library.
-
-It will still be included as a compatibility stub that just calls into the external stuff.
-
-
+Undocumented, deprecated. The functionality is better done by raw Paho.
 
 ### scullery.jack
 
-This submodule requires pyjack, and of course Jack. You should normally import this somewhere if using IceFlow with JACK.
+This submodule requires pyjack, and of course Jack.
 
 #### Message Bus activity
 
 ##### /system/jack/newport
  A PortInfo object with a .name, isInput, and isOutput property gets posted here whenever a new port is added to JACK.
 
 ##### /system/jack/delport
  A PortInfo object gets posted here whenever a port is unregistered.
 
 ##### system/jack/started
 When jack is started or restarted
 
- 
-
-#### Config:
-```python
-
-#Only relevant if manageJackProcess is True
-jackPeriods = 3
-periodSize = 128
-
-#These apply to soundcards other than the main system card
-usbPeriodSize = 384
-usbLatency = 384
-
-realtimePriority = 70
-
-#Do we want to run PulseAudio and the pulse jack backend?
-#Note that we automatically kill any pulseaudio process we find before
-usePulse= True
-
-sharePulse = None
-
-#Should we create alsa_in and alsa_out ports for every soundcard, with persistant names?
-manageSoundcards = True
-
-#Should we start the jack process itself, and auto restart it?
-#If False, we just try to use an existing one.
-#Must set this to True before calling startManaging!
-manageJackProcess = False
-```
-
-
 #### sullery.jack.startManaging()
 Start the worker thread and enable management functions
 
-#### scullery.jack.startJackServer()
-Actually start the jack server. They are separate because you may want to do this yourself.
-
 #### scullery.jack.Airwire(from,to)
 Return an Airwire object. This is a declaration that you want to connect two clients or ports and keep them connected.
 If you try to connect a client to a single port, all outputs get mixed down. Likewise a port to a client duplicates to all inputs.
 
 They start in the disconnected state.
 
 
@@ -270,7 +195,9 @@
 
 #### isActive()
 
 Return True if playing or paused
 
 #### seek(t=None, rate=None)
 Seek to a time, set playback rate, or both.
+
+
```

### Comparing `scullery-0.1.8/scullery/fluidsynth.py` & `scullery-0.1.9/scullery/fluidsynth.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     try:
         for i in players:
             players[i].fs.all_notes_off(-1)
     except:
         pass
 
 
-def stopAll():
+def stop_all():
     try:
         for i in players:
             players[i].close()
     except:
         pass
 
 
@@ -51,15 +51,15 @@
 
 
 def getGMInstruments():
     global gmInstruments
     if gmInstruments:
         return gmInstruments
     with open(os.path.join(os.path.dirname(os.path.abspath(__file__)), 'gm_instruments.yaml')) as f:
-        gmInstruments = yaml.load(f.read())
+        gmInstruments = yaml.load(f.read(), yaml.SafeLoader)
     return gmInstruments
 
 
 def findGMInstrument(name, look_in_soundfont=None, bank=None):
     # Allow manually selected instruments
     try:
         return (bank, int(name))
@@ -109,15 +109,15 @@
                 match = False
         if match:
             return (bank or 0, i)
     raise ValueError("No matching instrument")
 
 
 def waitForJack():
-    from scullery import jacktools
+    from kaithem.src.scullery import jacktools
     for i in range(10):
         if not jacktools.getPorts():
             time.sleep(1)
         else:
             return
 
     raise RuntimeError("It appears that JACK is not running")
```

### Comparing `scullery-0.1.8/scullery/iceflow_server.py` & `scullery-0.1.9/scullery/iceflow_server.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,72 +16,192 @@
 import threading
 import time
 import logging
 import weakref
 import traceback
 import os
 import sys
+import base64
+import math
+
+# import workers  # , ]messagebus
 
-#import workers  # , ]messagebus
 
 def doNow(f):
     f()
 
+
 initialized = False
 initlock = threading.Lock()
 
 lock = threading.RLock()
 Gst = None
 jackChannels = {}
 
+stopflag =[0]
 
 # Overridden later
 print = print
 
 rpc = [None]
 
 
 def tryToAvoidSegfaults(t, v):
     if v.clientName == "system":
-        stopAllJackUsers()
+        stop_allJackUsers()
 
-ppid = os.getppid()
 
 
-#https://stackoverflow.com/questions/568271/how-to-check-if-there-exists-a-process-with-a-given-pid-in-python
-def check_pid(pid):        
+
+# https://stackoverflow.com/questions/568271/how-to-check-if-there-exists-a-process-with-a-given-pid-in-python
+def check_pid(pid):
     """ Check For the existence of a unix pid. """
     try:
         os.kill(pid, 0)
     except OSError:
         return False
     else:
         return True
 
 
-
 #messagebus.subscribe("/system/jack/delport", tryToAvoidSegfaults)
-
 pipes = weakref.WeakValueDictionary()
 
 log = logging.getLogger("IceFlow_gst")
 
 
-import jsonrpyc
+# This is NixOS compatibility stuff, we could be running as an output from setup.py
+# Or we could be running directly with python3 file.py
+try:
+    from . import jsonrpyc
+except ImportError:
+    import jsonrpyc
+
+class PresenceDetectorRegion():
+    def __init__(self):
+        # This is a first order filter(Time domain blur) of the entire image
+
+        self.state = None
+        self.last = None
+
+    def poll(self, val):
+
+        #
+        from PIL import ImageFilter
+        from PIL import ImageChops
+
+        try:
+            import scipy.ndimage
+            ndim = 1
+        except Exception:
+            ndim = 0
+
+        import numpy as np
+        x = val
+
+        self.last = x if x else self.last
+
+        rval = 0
+        if self.state:
+            diff = ImageChops.difference(self.state, self.last)
+            # This is an erosion operation to prioritize multipixel stuff
+            # over single pixel noise
+            d = diff.convert('F')
+
+            if ndim:
+                # This is like 4 times faster.
+                d = scipy.ndimage.grey_erosion(d, (3, 3))
+            else:
+                d = d.filter(ImageFilter.MinFilter(3))
+            d = np.array(d)
+
+            # Ignore everythong below the threshold, that gets rid of a lot of our noise
+            m = np.mean(d) * 1.5 + 4
+            d = np.fmax(d - m, 0)
+
+            x = np.mean(d * d)
+            if x == 0:
+                rval = 0
+
+            rval = math.sqrt(x) / 2.5
+
+        self.state = self.last
+        return rval
+
+
+class PresenceDetector():
+    def __init__(self, capture, regions=None):
+        self.masks = regions
+        self.regions = {}
+        self.entireImage = PresenceDetectorRegion()
+        self.capture = capture
+
+        if regions is not None:
+            for i in regions:
+                self.regions[i] = PresenceDetectorRegion()
+
+    def poll(self):
+        r = {}
+
+        x = self.capture.pull()
+        if x is None:
+            print("Capture returned none")
+            return None
+
+        w = x.width
+        h = x.height
+
+        if self.masks is None:
+            return self.entireImage.poll(x)
+        else:
+            r[''] = self.entireImage.poll(x)
+
+        for i in self.masks:
+            m = self.masks[i]
+            # Crop region is specified as a fraction, convert to pixels and points instead of fraction y,x,w,h
+            i2 = x.crop((int(m[0] * w),
+                         int(m[1] * h),
+                        int(m[0] * w) + int(m[2] * w), 
+                        int(m[1] * h) + int(m[3] * h))
+                        )
+            r[i] = self.regions[i].poll(i2)
+        return r
 
 
 class PILCapture():
     def __init__(self, appsink):
         from PIL import Image
 
         self.img = Image
         self.appsink = appsink
 
-    def pull(self):
-        sample = self.appsink.emit('try-pull-sample', 0.1 * 10**9)
+    def pullToFile(self, f, timeout=0.1):
+        x = self.pull(timeout, True)
+        if not x:
+            return None
+        x.save(f)
+        return 1
+
+    def pull(self, timeout=0.1, forceLatest=False):
+        sample = self.appsink.emit('try-pull-sample', timeout * 10**9)
+
+        if forceLatest:
+            # Try another pull but only wait 1ms.
+            # This is in case there is another queued up frame, such as if we have buffer elements or something
+            # before this
+            sample2 = self.appsink.emit('try-pull-sample', 1000000)
+            c = 10
+            while sample2:
+                if c < 1:
+                    break
+                c -= 1
+                sample2 = self.appsink.emit('try-pull-sample', 1000000)
+
+            sample = sample2 or sample
+
         if not sample:
             return None
 
         buf = sample.get_buffer()
         caps = sample.get_caps()
         h = caps.get_structure(0).get_value('height')
         w = caps.get_structure(0).get_value('width')
@@ -149,22 +269,26 @@
                 unref = True
                 if not b:
                     raise RuntimeError(
                         "B has no pad named sink and A is a pad")
             if not a.link(b) == Gst.PadLinkReturn.OK:
                 raise RuntimeError("Could not link: " + str(a) + str(b))
 
-        elif not a.link(b):
-            raise RuntimeError("Could not link" + str(a) + str(b))
+        else:
+            x = a.link(b)
+
+            if not x:
+                raise RuntimeError("Could not link" + str(a) +
+                                   str(b) + " reason " + str(x))
     finally:
         if unref:
             pass  # b.unref()
 
 
-def stopAllJackUsers():
+def stop_allJackUsers():
     # It seems best to stop everything using jack before stopping and starting the daemon.
     with lock:
         c = list(jackChannels.items())
         for i in c:
             # Sync stop, we gotta wait
             try:
                 i[1]().syncStop = True
@@ -371,14 +495,21 @@
 
     def __init__(self, name=None, realtime=None, systemTime=False):
         init()
         self.lock = threading.RLock()
 
         self.seeklock = self.lock
 
+        self.pilcaptures = []
+
+        # We use this for detecting motion.
+        # We have to use this hack because gstreamer's detection is... not great.
+        self._pilmotiondetectorcapture = None
+        self._pilmotiondetector = None
+
         self.exiting = False
 
         self.uuid = time.time()
         name = name or "Pipeline" + str(time.monotonic())
         self.realtime = realtime
         self._stopped = True
         self.syncStop = False
@@ -460,16 +591,28 @@
         self.targetRate = 1.0
         self.pipelineRate = 1.0
 
     def sendEOS(self):
         self.pipeline.send_event(Gst.Event.new_eos())
 
     def loopCallback(self):
-        # Meant to subclass. Gets called under the lock
-        pass
+        if self._pilmotiondetector:
+            x = self._pilmotiondetector.poll()
+            if x is None:
+                return
+            rpc[0]("onPresenceValue", [x])
+
+    def addPresenceDetector(self, resolution, connectToOutput=None, regions=None):
+        if self._pilmotiondetector:
+            raise RuntimeError("Already have one of these")
+
+        self._pilmotiondetectorcapture = self.addPILCapture(
+            resolution, connectToOutput, method=0)
+        self._pilmotiondetector = PresenceDetector(
+            self._pilmotiondetectorcapture, regions)
 
     def seek(self, t=None, rate=None, _raw=False, _offset=0.008, flush=True, segment=False, sync=False, skip=False):
         "Seek the pipeline to a position in seconds, set the playback rate, or both"
         with self.lock:
             if self.exiting:
                 return
             if not self.running:
@@ -508,15 +651,15 @@
             e = threading.Event()
 
             def f():
                 # Seek is especiallly problematic, we must isolate it from state changes
                 with self.seeklock:
                     if (not flush) and self.pipeline.get_state(1000_000_000)[1] == Gst.State.PAUSED:
                         raise RuntimeError(
-                            "Cannot do non-flushing seek in paused state as this may deadlock.  State has changed while request inflight, request cancelled.")
+                            "Cannot do non-flushing seek in paused as this may deadlock.  State has changed while request inflight, request cancelled.")
 
                     self.pipeline.seek(rate, Gst.Format.TIME,
                                        flags, Gst.SeekType.NONE if t is None else Gst.SeekType.SET, max(
                                            ((t or 0) + _offset) * 10**9, 0),
                                        Gst.SeekType.NONE, 0)
                     e.set()
             if sync:
@@ -611,20 +754,44 @@
     def on_message(self, bus, message, userdata):
         s = message.get_structure()
         if s:
             self.onMessage(message.src, s.get_name(), s)
 
         return True
 
+    # def appsinkhandler(self,appsink, user_data):
+    #     sample = appsink.emit("pull-sample")
+    #     gst_buffer = sample.get_buffer()
+    #     (ret, buffer_map) = gst_buffer.map(Gst.MapFlags.READ)
+    #     rpc[0]("_onAppsinkData", [str(user_data), base64.b64encode(buffer_map.data).decode()])
+    #     return Gst.FlowReturn.OK
+
     def onMessage(self, src, name, s):
         if s.get_name() == 'level':
             rms = sum([i for i in s['rms']]) / len(s['rms'])
             decay = sum([i for i in s['decay']]) / len(s['decay'])
             rpc[0]("onLevelMessage", [str(src), rms, decay])
 
+        elif s.get_name() == 'motion':
+            if s.has_field("motion_begin"):
+                rpc[0]("onMotionBegin", [])
+            if s.has_field("motion_finished"):
+                rpc[0]("onMotionEnd", [])
+
+        elif s.get_name() == 'GstVideoAnalyse':
+            rpc[0]("onVideoAnalyze", [{'luma-average': s.get_double('luma-average')[
+                   1], 'luma-variance':s.get_double('luma-variance')[1]}])
+
+        elif s.get_name() == 'barcode':
+            rpc[0]("onBarcode", [s.get_string("type"),
+                   s.get_string("symbol"), s.get_int("quality")[1]])
+
+        elif s.get_name() == 'GstMultiFileSink':
+            rpc[0]("onMultiFileSink", [''])
+
         elif s.get_name() == 'pocketsphynx':
             if s.get_value('hypothesis'):
                 rpc[0]("onSTTMessage", [str(src), s.get_value('hypothesis')])
             if s.get_value('final'):
                 rpc[0]("onSTTMessageFinal", [str(src), s.get_value('final')])
 
     def on_error(self, bus, msg, userdata):
@@ -641,15 +808,15 @@
         # Called when a segment finishes playback, but NOT whem a segment ends because you did a seek to a new segment,
         # As that is usually not what you want when doing seamless loops.
         rpc[0]("onSegmentDone", [])
         pass
 
     def _waitForState(self, s, timeout=10):
         t = time.monotonic()
-        i = 0.001
+        i = 0.01
         while not self.pipeline.get_state(1000_000_000)[1] == s:
             if time.monotonic() - t > timeout:
                 raise RuntimeError("Timeout, pipeline still in: ",
                                    self.pipeline.get_state(1000_000_000)[1])
             time.sleep(min(i, 0.1))
             i *= 2
 
@@ -676,33 +843,36 @@
                 return
 
             x = effectiveStartTime or time.time()
             timeAgo = time.time() - x
             # Convert to monotonic time that the nternal APIs use
             self.startTime = time.monotonic() - timeAgo
 
-            if not self.pipeline.get_state(1000_000_000)[1] == (Gst.State.PAUSED, Gst.State.PLAYING):
-                with self.seeklock:
-                    self.pipeline.set_state(Gst.State.PAUSED)
-                self._waitForState(Gst.State.PAUSED)
+            # Go straight to playing, no need to locally do paused if we aren't using that feature
+            if self.systemTime or effectiveStartTime or segment:
+                if not self.pipeline.get_state(1000_000_000)[1] == (Gst.State.PAUSED, Gst.State.PLAYING):
+                    with self.seeklock:
+                        self.pipeline.set_state(Gst.State.PAUSED)
+                    self._waitForState(Gst.State.PAUSED)
 
             # Seek to where we should be, if we had actually
             # Started when we should have. We want to get everything set up in the pause state
             # First so we have the right "effective" start time.
 
             # We accept cutting off a few 100 milliseconds if it means
             # staying synced.
             if self.systemTime:
                 self.seek(time.monotonic() - self.startTime)
 
-            if segment:
+            elif segment:
                 self.seek(0, segment=True, flush=True)
 
             with self.seeklock:
                 self.pipeline.set_state(Gst.State.PLAYING)
+
             self._waitForState(Gst.State.PLAYING, timeout)
 
             self.running = True
 
             for i in range(0, 500):
                 try:
                     # Test that we can actually read the clock
@@ -807,15 +977,16 @@
                     time.sleep(0.01)
                     time.sleep(0.01)
                     time.sleep(0.01)
 
                 # On account of the race condition, it is possible that the thread actually never did start yet
                 # So we have to ignore the exit flag stuff.
 
-                # It shouldn't really be critical, most likely the thread can stop on it's own time anyway, because it doesn't do anything without getting the lock.
+                # It shouldn't really be critical, most likely the thread can stop on it's own time anyway,
+                # because it doesn't do anything without getting the lock.
                 if self.threadStarted:
                     while not self.exitSignal:
                         time.sleep(0.1)
                         if time.monotonic() - t > 10:
                             break
 
                 with self.lock:
@@ -847,40 +1018,46 @@
                             except KeyError:
                                 pass
 
                     doNow(f)
 
                     self._stopped = True
         finally:
-            import sys
-            sys.exit()
+           stopflag[0]=1
 
-
-
-    def addPILCapture(self, resolution, connectToOutput=None, buffer=1):
-        "Return a video capture object"
+    def addPILCapture(self, resolution=None, connectToOutput=None, buffer=1, method=1):
+        "Return a video capture object.  Now that we use BG threads this is just used to save snapshots to file"
+        if resolution:
+            scale = self.addElement("videoscale", method=method)
+            caps = self.addElement("capsfilter", caps="video/x-raw,width=" +
+                                   str(resolution[0]) + ",height=" + str(resolution[0]))
         conv = self.addElement("videoconvert", connectToOutput=connectToOutput)
-        scale = self.addElement("videoscale")
-        caps = self.addElement("capsfilter", caps="video/x-raw,width=" +
-                               str(resolution[0]) + ",height=" + str(resolution[0]) + ", format=RGB")
+        caps = self.addElement("capsfilter", caps="video/x-raw,format=RGB")
+
         appsink = self.addElement(
             "appsink", drop=True, sync=False, max_buffers=buffer)
 
-        return PILCapture(appsink)
+        p = PILCapture(appsink)
+        elementsByShortId[id(p)] = p
+        self.pilcaptures.append(p)
+        return p
+
+    def addRemotePILCapture(self, *a, **k):
+        return id(self.addPILCapture(*a, **k))
 
     def addPILSource(self, resolution, buffer=1, greyscale=False):
         "Return a video source object that we can use to put PIL buffers into the stream"
 
         appsrc = self.addElement("appsrc", caps="video/x-raw,width=" + str(resolution[0]) + ",height=" + str(
             resolution[0]) + ", format=" + "GREy8" if greyscale else "RGB", connectToOutput=False)
         conv = self.addElement("videoconvert")
         scale = self.addElement("videoscale")
 
         # Start with a blck image to make things prerooll
-        if(greyscale):
+        if (greyscale):
             appsrc.emit(
                 "push-buffer", Gst.Buffer.new_wrapped(bytes(resolution[0] * resolution[1])))
         else:
             appsrc.emit(
                 "push-buffer", Gst.Buffer.new_wrapped(bytes(resolution[0] * resolution[1] * 3)))
 
         return PILSource(appsrc, greyscale)
@@ -895,67 +1072,103 @@
 
     def addAppSrc(self, connectToOutput=None, buffer=1, caps=''):
         "Return a video capture object"
 
         appsrc = self.addElement("appsrc", caps=caps, connectToOutput=False)
         return AppSource(appsrc)
 
+    def pullBuffer(self, element, timeout=0.1):
+        if isinstance(element, int):
+            element = elementsByShortId[element]
+
+        sample = self.appsink.emit('try-pull-sample', timeout * 10**9)
+        if not sample:
+            return None
+
+        buf = sample.get_buffer()
+        caps = sample.get_caps()
+
+        return base64.b64encode(buf.extract_dup(0, buf.get_size()))
+
+    def pullToFile(self, element, fn):
+        if isinstance(element, int):
+            element = elementsByShortId[element]
+
+        return element.pullToFile(fn)
+
     def addElement(self, t, name=None, connectWhenAvailable=False, connectToOutput=None, sidechain=False, **kwargs):
 
         with self.lock:
             if not isinstance(t, str):
                 raise ValueError("Element type must be string")
 
             e = Gst.ElementFactory.make(t, name)
 
+            # if t=='appsink':
+            #     e.connect("new-sample", self.appsinkhandler, name)
+
             if e == None:
                 raise ValueError("Nonexistant element type: " + t)
             self.weakrefs[str(e)] = e
             self.elementTypesById[id(e)] = t
             elementsByShortId[id(e)] = e
 
             for i in kwargs:
                 v = kwargs[i]
                 self.setProperty(e, i, v)
 
             self.pipeline.add(e)
-
+            op = []
             # May need to use an ID if its a remore command
             if connectToOutput:
-                if isinstance(connectToOutput, int):
-                    connectToOutput = elementsByShortId[connectToOutput]
+                if not isinstance(connectToOutput, (list, tuple)):
+                    cto = [connectToOutput]
+                else:
+                    cto = connectToOutput
 
-                if not id(connectToOutput) in self.elementTypesById:
-                    raise ValueError("Cannot connect to the output of: " +
-                                     str(connectToOutput) + ", no such element in pipeline.")
-
-            # Element doesn't have an input pad, we want this to be usable as a fake source to go after a real source if someone
-            # wants to use it as a effect
-            if t == "audiotestsrc":
-                connectToOutput = False
-
-            # This could be the first element
-            if self.elements and (not (connectToOutput is False)):
-                connectToOutput = connectToOutput or self.elements[-1]
+                for connectToOutput in cto:
 
-                # Fakesinks have no output, we automatically don't connect those
-                if self.elementTypesById[id(connectToOutput)] == 'fakesink':
+                    if not connectToOutput is False:
+                        if isinstance(connectToOutput, int):
+                            connectToOutput = elementsByShortId[connectToOutput]
+
+                        if not id(connectToOutput) in self.elementTypesById:
+                            raise ValueError("Cannot connect to the output of: " +
+                                             str(connectToOutput) + ", no such element in pipeline.")
+                        op.append(connectToOutput)
+            else:
+                # One auto connect
+                if connectToOutput is None:
+                    op = [None]
+
+            for connectToOutput in op:
+                # Element doesn't have an input pad, we want this to be usable as a fake source to go after a real source if someone
+                # wants to use it as a effect
+                if t == "audiotestsrc":
                     connectToOutput = False
 
-                # Decodebin doesn't have a pad yet for some awful reason
-                elif (self.elementTypesById[id(connectToOutput)] == 'decodebin') or connectWhenAvailable:
-                    eid = time.time()
-                    f = linkClosureMaker(weakref.ref(
-                        self), connectToOutput, e, connectWhenAvailable, eid)
-
-                    self.waitingCallbacks[eid] = f
-                    # Dummy 1 param because some have claimed to get segfaults without
-                    connectToOutput.connect("pad-added", f, 1)
-                else:
-                    link(connectToOutput, e)
+                # This could be the first element
+                if self.elements and (not (connectToOutput is False)):
+                    connectToOutput = connectToOutput or self.elements[-1]
+
+                    # Fakesinks have no output, we automatically don't connect those
+                    if self.elementTypesById[id(connectToOutput)] == 'fakesink':
+                        connectToOutput = False
+
+                    # Decodebin doesn't have a pad yet for some awful reason
+                    elif (self.elementTypesById[id(connectToOutput)] == 'decodebin') or connectWhenAvailable:
+                        eid = time.time()
+                        f = linkClosureMaker(weakref.ref(
+                            self), connectToOutput, e, connectWhenAvailable, eid)
+
+                        self.waitingCallbacks[eid] = f
+                        # Dummy 1 param because some have claimed to get segfaults without
+                        connectToOutput.connect("pad-added", f, 1)
+                    else:
+                        link(connectToOutput, e)
 
             # Sidechain means don't set this element as the
             # automatic thing that the next entry links to
             if not sidechain:
                 self.elements.append(e)
             else:
                 self.sidechainElements.append(e)
@@ -964,30 +1177,26 @@
 
             self.lastElementType = t
             p = weakref.proxy(e)
 
             self.proxyToElement[id(p)] = e
             # List it under the proxy as well
             self.elementTypesById[id(p)] = t
-            elementsByShortId[id(p)]=e
+            elementsByShortId[id(p)] = e
 
         # Mark as a JACK user so we can stop if needed for JACK
         # Stuff
         if t.startswith("jackaudio"):
             with lock:
                 jackChannels[self.uuid] = weakref.ref(self)
         return p
 
     def addElementRemote(self, *a, **k):
         return id(self.addElement(*a, **k))
 
-    def addElementRemote(self, *a, **k):
-        return id(self.addElement(*a, **k))
-
-
     def addJackMixerSendElements(self, target, idee, volume=-60):
         with self.lock:
             if not isinstance(target, str):
                 raise ValueError("Target must be string")
 
             e = self.makeElement("tee")
             q = self.makeElement("queue")
@@ -1005,32 +1214,29 @@
             e2.set_property("port-pattern", "fdgjkndgmkndfmfgkjkf")
             e2.set_property("sync", False)
             e2.set_property("slave-method", 0)
             e2.set_property('provide-clock', False)
             e2.set_property('connect', False)
 
             e2.latency_time = 10
-           
 
             tee_src_pad_template = e.get_pad_template("src_%u")
             tee_audio_pad = e.request_pad(tee_src_pad_template, None, None)
             tee_audio_pad2 = e.request_pad(tee_src_pad_template, None, None)
 
             if self.elements:
-               link(self.elements[-1], e)
+                link(self.elements[-1], e)
             link(tee_audio_pad, q)
             link(tee_audio_pad2, q2)
             self.elements.append(q2)
 
             link(q, l)
             link(l, e2)
 
-            return id(l),id(e2)
-
-
+            return id(l), id(e2)
 
     def setProperty(self, element, prop, value):
         with self.lock:
 
             if isinstance(element, int):
                 element = elementsByShortId[element]
 
@@ -1038,14 +1244,17 @@
                 if not os.path.isfile(value):
                     raise ValueError("No such file: " + value)
 
             if prop == 'caps':
                 value = Gst.Caps(value)
                 self.weakrefs[str(value)] = value
 
+            if prop.startswith("_"):
+                prop = prop[1:]
+                
             prop = prop.replace("_", "-")
 
             prop = prop.split(":")
             if len(prop) > 1:
                 childIndex = int(prop[0])
                 target = element.get_child_by_index(childIndex)
                 target.set_property(prop[1], value)
@@ -1055,19 +1264,35 @@
 
     def isActive(self):
         with self.lock:
             if self.pipeline.get_state(1000_000_000)[1] == Gst.State.PAUSED:
                 return True
             if self.pipeline.get_state(1000_000_000)[1] == Gst.State.PLAYING:
                 return True
+            
+
+gstp = None
+
+ppid = os.getppid()
+
 
-gstp=GStreamerPipeline()
-rpc[0] = jsonrpyc.RPC(target=gstp)
+def main():
+    global gstp
 
+    gstp = GStreamerPipeline()
+    rpc[0] = jsonrpyc.RPC(target=gstp)
+
+
+    # def print(*a):
+    #     rpc[0]("print", [str(a)])
+
+    while not rpc[0].threadStopped:
+        time.sleep(1)
+
+        if (not check_pid(ppid)) or stopflag[0]:
+            sys.exit()
 
-def print(*a):
-    rpc[0]("print", str(a))
+        if not os.getppid() == ppid:
+            return
 
-while not rpc[0].threadStopped:
-    time.sleep(10)
-    if not check_pid(ppid):
-        sys.exit()
+if __name__ == '__main__':
+    main()
```

### Comparing `scullery-0.1.8/scullery/jsonrpyc.py` & `scullery-0.1.9/scullery/jsonrpyc.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,17 +22,20 @@
 import sys
 import json
 import io
 import time
 import threading
 import weakref
 import traceback
+import os
+
+
+server_only = False
 
 
-server_only=False
 class Spec(object):
     """
     This class wraps methods that create JSON-RPC 2.0 compatible string representations of
     request, response and error objects. All methods are class members, so you might never want to
     create an instance of this class, but rather use the methods directly:
 
     .. code-block:: python
@@ -50,35 +53,39 @@
     @classmethod
     def check_id(cls, id, allow_empty=False):
         """
         Value check for *id* entries. When *allow_empty* is *True*, *id* is allowed to be *None*.
         Raises a *TypeError* when *id* is neither an integer nor a string.
         """
         if (id is not None or not allow_empty) and not isinstance(id, (int, str)):
-            raise TypeError("id must be an integer or string, got {} ({})".format(id, type(id)))
+            raise TypeError(
+                "id must be an integer or string, got {} ({})".format(id, type(id)))
 
     @classmethod
     def check_method(cls, method):
         """
         Value check for *method* entries. Raises a *TypeError* when *method* is not a string.
         """
         if not isinstance(method, str):
-            raise TypeError("method must be a string, got {} ({})".format(method, type(method)))
+            raise TypeError(
+                "method must be a string, got {} ({})".format(method, type(method)))
 
     @classmethod
     def check_code(cls, code):
         """
         Value check for *code* entries. Raises a *TypeError* when *code* is not an integer, or a
         *KeyError* when there is no :py:class:`RPCError` subclass registered for that *code*.
         """
         if not isinstance(code, int):
-            raise TypeError("code must be an integer, got {} ({})".format(id, type(id)))
+            raise TypeError(
+                "code must be an integer, got {} ({})".format(id, type(id)))
 
         if not get_error(code):
-            raise ValueError("unknown code, got {} ({})".format(code, type(code)))
+            raise ValueError(
+                "unknown code, got {} ({})".format(code, type(code)))
 
     @classmethod
     def request(cls, method, id=None, params=None):
         """
         Creates the string representation of a request that calls *method* with optional *params*
         which are encoded by ``json.dumps``. When *id* is *None*, the request is considered a
         notification.
@@ -124,15 +131,16 @@
 
         # encode string ids
         if isinstance(id, str):
             id = json.dumps(id)
 
         # build the response string
         try:
-            res = "{{\"jsonrpc\":\"2.0\",\"id\":{},\"result\":{}}}".format(id, json.dumps(result))
+            res = "{{\"jsonrpc\":\"2.0\",\"id\":{},\"result\":{}}}".format(
+                id, json.dumps(result))
         except Exception as e:
             raise RPCParseError(str(e))
 
         return res
 
     @classmethod
     def error(cls, id, code, data=None):
@@ -145,15 +153,16 @@
             cls.check_id(id)
             cls.check_code(code)
         except Exception as e:
             raise RPCInvalidRequest(str(e))
 
         # build the inner error data
         message = get_error(code).title
-        err_data = "{{\"code\":{},\"message\":\"{}\"".format(code, message).replace("\n",'').replace("\r",'')
+        err_data = "{{\"code\":{},\"message\":\"{}\"".format(
+            code, message).replace("\n", '').replace("\r", '')
 
         # insert data when given
         if data is not None:
             try:
                 err_data += ",\"data\":{}}}".format(json.dumps(data))
             except Exception as e:
                 raise RPCParseError(str(e))
@@ -161,20 +170,23 @@
             err_data += "}"
 
         # encode string ids
         if isinstance(id, str):
             id = json.dumps(id)
 
         # start building the error string
-        err = "{{\"jsonrpc\":\"2.0\",\"id\":{},\"error\":{}}}".format(id, err_data)
+        err = "{{\"jsonrpc\":\"2.0\",\"id\":{},\"error\":{}}}".format(
+            id, err_data)
 
         return err
 
+
 leakDebug = weakref.WeakValueDictionary()
 
+
 class RPC(object):
     """
     The main class of *jsonrpyc*. Instances of this class wrap an input stream *stdin* and an output
     stream *stdout* in order to communicate with other services. A service is not even forced to be
     written in Python as long as it strictly implements the JSON-RPC 2.0 specification. RPC
     instances may wrap a *target* object. By means of a :py:class:`Watchdog` instance, incoming
     requests are routed to methods of this object whose result might be sent back as a response.
@@ -248,59 +260,57 @@
 
     def __init__(self, target=None, stdin=None, stdout=None, watch=True, **kwargs):
         super(RPC, self).__init__()
         self.fastResponseFlag = threading.Event()
 
         # the wrapped target object
         self.target = weakref.ref(target)
-        leakDebug[id(self)]=self
+        leakDebug[id(self)] = self
 
         # open streams
         stdin = sys.stdin if stdin is None else stdin
         stdout = sys.stdout if stdout is None else stdout
         self.stdin = io.open(stdin.fileno(), "rb")
         self.stdout = io.open(stdout.fileno(), "wb")
 
         # other attributes
         self._i = -1
         self._callbacks = {}
         self._results = {}
-        self.stopFlag=False
+        self.stopFlag = False
 
         # create and optionall start the watchdog
         kwargs["start"] = watch
         kwargs.setdefault("daemon", target is None)
         self.watchdog = Watchdog(self, **kwargs)
 
         self.threadStopped = False
 
-
-
     def __del__(self):
-       if server_only:
-        try:
-            self.stdin.close()
-        except:
-            pass
-        try:
-            self.stdout.close()
-        except:
-            pass
-            
-        watchdog = getattr(self, "watchdog", None)
-        if watchdog:
-            watchdog.stop()
+        if server_only:
+            try:
+                self.stdin.close()
+            except Exception:
+                pass
+            try:
+                self.stdout.close()
+            except Exception:
+                pass
+
+            watchdog = getattr(self, "watchdog", None)
+            if watchdog:
+                watchdog.stop()
 
     def __call__(self, *args, **kwargs):
         """
         Shorthand for :py:meth:`call`.
         """
         return self.call(*args, **kwargs)
 
-    def call(self, method, args=(), kwargs=None, callback=None, block=0,timeout=60):
+    def call(self, method, args=(), kwargs=None, callback=None, block=0, timeout=60):
         """
         Performs an actual remote procedure call by writing a request representation (a string) to
         the output stream. The remote RPC instance uses *method* to route to the actual method to
         call with *args* and *kwargs*. When *callback* is set, it will be called with the result of
         the remote call. When *block* is larger than *0*, the calling thread is blocked until the
         result is received. In this case, *block* will be the poll interval, emulating synchronuous
         return value behavior. When both *callback* is *None* and *block* is *0* or smaller, the
@@ -329,46 +339,45 @@
 
         # create the request
         params = {"args": args, "kwargs": kwargs}
         req = Spec.request(method, id=id, params=params)
         self.fastResponseFlag.clear()
 
         self._write(req)
-        
+
         st = time.time()
 
         # blocking return value behavior
         if block > 0:
 
             while True:
                 if self._results[id] != self.EMPTY_RESULT:
                     result = self._results[id]
                     del self._results[id]
                     if isinstance(result, Exception):
                         raise result
                     else:
                         return result
-                #Block for up to the specified time, but also, whenever any new data comes in we immediately check.
+                # Block for up to the specified time, but also, whenever any new data comes in we immediately check.
 
                 if self.fastResponseFlag.wait(block):
                     self.fastResponseFlag.clear()
-                if timeout and (time.time()-st)> timeout:
+                if timeout and (time.time() - st) > timeout:
                     raise TimeoutError("Request Timed Out")
 
     def _handle(self, line):
         """
         Handles an incoming *line* and dispatches the parsed object to the request, response, or
         error handlers.
         """
         try:
             obj = json.loads(line)
-        except:
-
-            print("Bad JSON",line)
-            #What if we just didn't?
+        except Exception:
+            print("Bad JSON", line)
+            # What if we just didn't?
             return
 
         # dispatch to the correct handler
         if "method" in obj:
             # request
             self._handle_request(obj)
         elif "error" not in obj:
@@ -391,18 +400,18 @@
                 self._write(res)
         except Exception as e:
             sys.stderr.write(traceback.format_exc())
             if "id" in req:
                 if isinstance(e, RPCError):
                     err = Spec.error(req["id"], e.code, e.data)
                 else:
-                    err = Spec.error(req["id"], -32603, str(traceback.format_exc()))
+                    err = Spec.error(req["id"], -32603,
+                                     str(traceback.format_exc()))
 
                 self._write(err)
-        
 
     def _handle_response(self, res):
         """
         Handles an incoming successful response *res*. Blocking calls are resolved and registered
         callbacks are invoked with the first error argument being set to *None*.
         """
         # set the result
@@ -477,15 +486,16 @@
         """
         Writes a string *s* to the output stream.
         """
         self.stdout.write(bytearray(s + "\n", "utf-8"))
         self.stdout.flush()
 
 
-wdl=weakref.WeakValueDictionary()
+wdl = weakref.WeakValueDictionary()
+
 
 class Watchdog(threading.Thread):
     """
     This class represents a thread that watches the input stream of an :py:class:`RPC` instance for
     incoming content and dispatches requests to it.
 
     .. py:attribute:: rpc
@@ -503,15 +513,15 @@
     .. py:attribute:: daemon
 
        The thread's daemon flag.
     """
 
     def __init__(self, rpc, name="nostartstoplog.rpcwatchdog", interval=0.02, daemon=False, start=True):
         super(Watchdog, self).__init__()
-        wdl[id(self)]=self
+        wdl[id(self)] = self
 
         # store attributes
         self.rpc = weakref.ref(rpc)
         self.name = name
         self.interval = interval
         self.daemon = daemon
 
@@ -555,58 +565,66 @@
                     break
 
                 if rpc.stopFlag:
                     break
 
                 # read from stdin depending on whether it is a tty or not
                 if rpc.stdin.isatty():
-                    cur_pos =rpc.stdin.tell()
+                    cur_pos = rpc.stdin.tell()
                     if cur_pos != last_pos:
                         rpc.stdin.seek(last_pos)
-                        lines =rpc.stdin.readlines()
-                        last_pos =rpc.stdin.tell()
+                        lines = rpc.stdin.readlines()
+                        last_pos = rpc.stdin.tell()
                         rpc.stdin.seek(cur_pos)
                 else:
                     try:
-                        rfds, wfds, efds = select.select( [ sys.stdin.fileno()], [], [], self.interval)
-                        #On some systems it seems we never got the select return,
-                        #So we had to resort to polling way too much.
-                        #It seems that might be fixed, so if possible we go back to slower
-                        #polling and select() based response.
+                        rfds, wfds, efds = select.select(
+                            [rpc.stdin.fileno()], [], [], self.interval)
+                        # On some systems it seems we never got the select return,
+                        # So we had to resort to polling way too much.
+                        # It seems that might be fixed, so if possible we go back to slower
+                        # polling and select() based response.
                         if rfds:
-                            self.interval=0.1
+                            self.interval = 0.1
+                        # We should exit if we detect we have been adopted by pid1
+                        if os.getppid() < 2:
+                            exit(1)
+
                         lines = [rpc.stdin.readline()]
                     except IOError:
                         # prevent residual race conditions occurring when stdin is closed externally
                         pass
 
                 # handle new lines if any
-                if lines:
+                if lines and lines[0]:
                     rpc.fastResponseFlag.set()
                     for line in lines:
-                        line = line.decode("utf-8").strip()
+                        try:
+                            line = line.decode("utf-8").strip()
+                        except Exception:
+                            print("Bad line", line)
                         if line:
                             rpc._handle(line)
                 else:
                     self._stop.wait(self.interval)
                 del rpc
-        except:
-            print(traceback.format_exc())      
+        except Exception:
+            print(traceback.format_exc())
 
         finally:
             if server_only:
                 try:
                     self.rpc().stdin.close()
                     self.rpc().stdout.close()
-                except:
+                except Exception:
                     pass
 
             x = self.rpc()
             if x:
-                x.threadStopped=True
+                x.threadStopped = True
 
 
 class RPCError(Exception):
 
     """
     Base class for RPC errors.
```

### Comparing `scullery-0.1.8/scullery/messagebus.py` & `scullery-0.1.9/scullery/messagebus.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,320 +1,333 @@
-#Copyright Daniel Dunn 2013
-#This file is part of Kaithem Automation.
 
-#Kaithem Automation is free software: you can redistribute it and/or modify
-#it under the terms of the GNU General Public License as published by
-#the Free Software Foundation, version 3.
-
-#Kaithem Automation is distributed in the hope that it will be useful,
-#but WITHOUT ANY WARRANTY; without even the implied warranty of
-#MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#GNU General Public License for more details.
+# Copyright Daniel Dunn 2013
+# This file is part of Kaithem Automation.
 
-#You should have received a copy of the GNU General Public License
-#along with Kaithem Automation.  If not, see <http://www.gnu.org/licenses/>.
+# Kaithem Automation is free software: you can redistribute it and/or modify
+# it under the terms of the GNU General Public License as published by
+# the Free Software Foundation, version 3.
+
+# Kaithem Automation is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU General Public License for more details.
+
+# You should have received a copy of the GNU General Public License
+# along with Kaithem Automation.  If not, see <http://www.gnu.org/licenses/>.
 
 "This file manages the kaithem global message bus that is used mostly for logging but also for many other tasks."
 
-import weakref,threading,time,os,random,traceback,logging,inspect,types,copy
-from typing import Callable,Optional
+import weakref
+import threading
+import time
+import traceback
+import logging
+import inspect
+import types
+import copy
+from typing import Callable, Optional, Any, Set
 
 from typeguard import typechecked
 
 from . import workers
 from collections import defaultdict, OrderedDict
 
 _subscribers_list_modify_lock = threading.RLock()
 cachelock = threading.RLock()
-#OrderedDict doesn't seem as fast as dict. So I have a cache of the cache
+# OrderedDict doesn't seem as fast as dict. So I have a cache of the cache
 parsecache = OrderedDict()
 parsecachecache = {}
 
-log =logging.getLogger("system.messagebus")
-def normalize_topic(topic):
+log = logging.getLogger("system.messagebus")
+
+
+def normalize_topic(topic: str) -> str:
     """"Because some topics are equivalent("/foo" and "foo"), this lets us convert them to the canonical "/foo" representation.
     Note that "/foo/" is not the same as "/foo", because a trailing slash indicates a "directory"."""
     topic = topic.strip()
     if not topic.startswith('/'):
-        return '/'+topic
+        return '/' + topic
     else:
         return topic
 
+
 def _shouldReRaiseAttrErr():
     return True
 
+
 def defaultErrorHandler(*a):
     print(traceback.format_exc())
-    
+
+
 subscriberErrorHandlers = []
 
-def handleError(f,topic,value):
+
+def handleError(f: Callable[..., Any], topic: str, value: Any):
     log.exception("Message bus subscriber error")
-    if hasattr(f,"messagebusWrapperFor"):
-        f= f.messagebusWrapperFor
+    if hasattr(f, "messagebusWrapperFor"):
+        f = f.messagebusWrapperFor
     for i in subscriberErrorHandlers:
         try:
-            i(f,topic,value)
-        except:
+            i(f, topic, value)
+        except Exception:
             print(traceback.format_exc())
 
-def runFunction(f,a):
+
+def runFunction(f, a):
     return f(*a)
 
+
 class MessageBus(object):
-    def __init__(self,executor:Optional[Callable] = None):
+    def __init__(self, executor: Optional[Callable[..., Any]] = None):
         """You pass this a function of one argument that just calls its argument. Defaults to calling in
         same thread and ignoring errors.
         """
-        if executor==None:
-            def do(self, f):
+        if executor == None:
+            def do(self, f: Callable[[], Any]):
                 try:
                     f()
-                except:
+                except Exception:
                     pass
             self.executor = do
         else:
             self.executor = executor
 
         self.subscribers = defaultdict(list)
         self.subscribers_immutable = {}
 
     @typechecked
-    def subscribe(self,topic:str,callback:Callable):
-        topic=normalize_topic(topic)
-       
+    def subscribe(self, topic: str, callback: Callable[..., Any]):
+        topic = normalize_topic(topic)
+
         with _subscribers_list_modify_lock:
-            wrappedCallback = self.wrap_callback(callback,topic)
+            wrappedCallback = self.wrap_callback(callback, topic)
 
-           
             self.subscribers[topic].append(wrappedCallback)
             self.subscribers_immutable = copy.deepcopy(self.subscribers)
 
-    def unsubscribe(self,topic, function):
-            "Unsubscribe topic from function"
-            try:
-                with _subscribers_list_modify_lock:
-                    target = None
-                    for j in self.subscribers[topic]:
-                        if j.originalFunction()==function:
-                            target = j
-                    if target:
-                        self.subscribers[topic].remove(target)
-                    else:
-                        pass
-            except:
-                print(traceback.format_exception())
-                pass
-            #There is a very slight chance someone will
-            #Add something to topic before we delete it but after the test.
-            #That would result in a canceled subscription
-            #So we use this lock.
-            try:
-                with _subscribers_list_modify_lock:
-                    if not self.subscribers[topic]:
-                        self.subscribers.pop(topic)
-            except AttributeError as e:
-                #This try and if statement are supposed to catch nuisiance errors when shutting down.
-                if _shouldReRaiseAttrErr():
-                    raise e
- 
-            finally:
-                with _subscribers_list_modify_lock:
-                    self.subscribers_immutable = copy.deepcopy(self.subscribers)
+    def unsubscribe(self, topic: str, function: Callable[..., Any]):
+        "Unsubscribe topic from function"
+        try:
+            with _subscribers_list_modify_lock:
+                target = None
+                for j in self.subscribers[topic]:
+                    if j.originalFunction() == function:
+                        target = j
+                if target:
+                    self.subscribers[topic].remove(target)
+                else:
+                    pass
+        except Exception:
+            print(traceback.format_exception())
+            pass
+        # There is a very slight chance someone will
+        # Add something to topic before we delete it but after the test.
+        # That would result in a canceled subscription
+        # So we use this lock.
+        try:
+            with _subscribers_list_modify_lock:
+                if not self.subscribers[topic]:
+                    self.subscribers.pop(topic)
+        except AttributeError as e:
+            # This try and if statement are supposed to catch nuisiance errors when shutting down.
+            if _shouldReRaiseAttrErr():
+                raise e
+
+        finally:
+            with _subscribers_list_modify_lock:
+                self.subscribers_immutable = copy.deepcopy(self.subscribers)
 
     @staticmethod
-    def parseTopic(topic):
+    def parseTopic(topic: str) -> Set[str]:
         "Parse the topic string into a list of all subscriptions that could possibly match."
         global parsecache
-        #Since this is a pure function(except the caching itself) we can cache it
+        # Since this is a pure function(except the caching itself) we can cache it
         if topic in parsecache:
             return parsecache[topic]
-        
-        #Let's cache by the original version of the topic, so we don't have to convert it to the canonical
+
+        # Let's cache by the original version of the topic, so we don't have to convert it to the canonical
         oldtopic = topic
-        topic=normalize_topic(topic)
+        topic = normalize_topic(topic)
 
-        #A topic foo/bar/baz would go to
-        #foo, foo/bar, and /foo/bar/baz
-        #So we need to make a list like that
+        # A topic foo/bar/baz would go to
+        # foo, foo/bar, and /foo/bar/baz
+        # So we need to make a list like that
         matchingtopics = set(['/#'])
         parts = topic.split("/")
         last = ""
 
-        #Add the exact one
+        # Add the exact one
         matchingtopics.add(topic)
-        
-        
+
         for i in parts:
-            last += (i+'/')
-            matchingtopics.add(last+"#")
+            last += (i + '/')
+            matchingtopics.add(last + "#")
         parsecache[oldtopic] = matchingtopics
-        #Don't let the cache get too big.
-        #Getting rid of the oldest should hopefully converge to the most used topics being cached
+        # Don't let the cache get too big.
+        # Getting rid of the oldest should hopefully converge to the most used topics being cached
         if len(parsecache) > 600:
             parsecache.popitem(last=False)
         return matchingtopics
 
     @typechecked
-    def wrap_callback(self,f:Callable,topic:str):
+    def wrap_callback(self, f: Callable[..., Any], topic: str):
         """return function g that calls f with (topic,message) or just f(topic), depending
         on how many args there are.
          and if errors is true logs the error"""
 
         args = len(inspect.signature(f).parameters)
 
-
         timestamp = time.monotonic()
 
         try:
-            desc=str(f.__name__+' of '+f.__module__)
-        except:
+            desc = str(f.__name__ + ' of ' + f.__module__)
+        except Exception:
             desc = str(f)
 
+        # Allright, here is how this works.
+        # We have to deal with the possibility that, at any time,
+        # The callback will cease to exist. That, in fact, is how one unsubscribes.
+        # So, we make this here closure that knows the topic, and
+        # When the GC goes Om Nom Nom on the function, we get passed the weakref to it.
+        # Then we get rid of the empty weakref and if that causes the entire topic
+        # To have no subscribers, delete that too in case of memory leak.
 
-        #Allright, here is how this works.
-        #We have to deal with the possibility that, at any time,
-        #The callback will cease to exist. That, in fact, is how one unsubscribes.
-        #So, we make this here closure that knows the topic, and
-        #When the GC goes Om Nom Nom on the function, we get passed the weakref to it.
-        #Then we get rid of the empty weakref and if that causes the entire topic
-        #To have no subscribers, delete that too in case of memory leak.
         def delsubscription(weakrefobject):
-            if time.monotonic()<timestamp-0.5:
-                logging.warning("Function: " +desc+" was deleted 0.5s after being subscribed.  This is probably not what you wanted.")
-                
+            if time.monotonic() < timestamp - 0.5:
+                logging.warning(
+                    "Function: " + desc + " was deleted 0.5s after being subscribed.  This is probably not what you wanted.")
+
             try:
                 with _subscribers_list_modify_lock:
                     self.subscribers[topic].remove(weakrefobject)
-            except:
+            except Exception:
                 pass
-            #There is a very slight chance someone will
-            #Add something to topic before we delete it but after the test.
-            #That would result in a canceled subscription
-            #So we use this lock.
+            # There is a very slight chance someone will
+            # Add something to topic before we delete it but after the test.
+            # That would result in a canceled subscription
+            # So we use this lock.
             try:
                 with _subscribers_list_modify_lock:
                     if not self.subscribers[topic]:
                         self.subscribers.pop(topic)
             except AttributeError as e:
-                #This try and if statement are supposed to catch nuisiance errors when shutting down.
+                # This try and if statement are supposed to catch nuisiance errors when shutting down.
                 if _shouldReRaiseAttrErr():
                     raise e
-               
+
             finally:
                 with _subscribers_list_modify_lock:
-                    self.subscribers_immutable = copy.deepcopy(self.subscribers)
+                    self.subscribers_immutable = copy.deepcopy(
+                        self.subscribers)
 
-
-
-        if isinstance(f,types.MethodType):
-            f=weakref.WeakMethod(f,delsubscription)
+        if isinstance(f, types.MethodType):
+            f = weakref.WeakMethod(f, delsubscription)
         else:
-            f = weakref.ref(f,delsubscription)
+            f = weakref.ref(f, delsubscription)
 
-        #Mutable object that gets saved to the closure for keeping track of if we already loggged this
-        alreadyLogged=[False]
-        if args==0:
-            def g(topic, message,errors,timestamp,annotation):
+        # Mutable object that gets saved to the closure for keeping track of if we already loggged this
+        alreadyLogged = [False]
+        if args == 0:
+            def g(topic, message, errors, timestamp, annotation):
                 try:
                     f2 = f()
                     if f2:
                         f2()
-                except:
+                except Exception:
                     try:
                         if errors:
                             if not alreadyLogged[0]:
-                                handleError(f2, topic,message)
-                            alreadyLogged[0]=True
+                                handleError(f2, topic, message)
+                            alreadyLogged[0] = True
                     except Exception as e:
-                            print("err",e)
-        elif args==2:
-            def g(topic, message,errors,timestamp,annotation):
+                        print("err", e)
+        elif args == 2:
+            def g(topic, message, errors, timestamp, annotation):
                 try:
                     f2 = f()
                     if f2:
-                        f2(topic,message)
-                except:
+                        f2(topic, message)
+                except Exception:
                     try:
                         if errors:
                             if not alreadyLogged[0]:
-                                handleError(f2,topic,message)
-                            alreadyLogged[0]=True
+                                handleError(f2, topic, message)
+                            alreadyLogged[0] = True
 
                     except Exception as e:
-                            print("err",e)
-        elif args==4:
-            def g(topic, message,errors,timestamp,annotation):
+                        print("err", e)
+        elif args == 4:
+            def g(topic, message, errors, timestamp, annotation):
                 try:
                     f2 = f()
                     if f2:
-                        f2(topic,message,timestamp,annotation)
-                except:
+                        f2(topic, message, timestamp, annotation)
+                except Exception:
                     try:
                         if errors:
                             if not alreadyLogged[0]:
-                                handleError(f2,topic,message)
-                            alreadyLogged[0]=True
+                                handleError(f2, topic, message)
+                            alreadyLogged[0] = True
 
                     except Exception as e:
-                            print("err",e)
-        elif args==1:
-            def g(topic, message,errors,timestamp,annotation):
+                        print("err", e)
+        elif args == 1:
+            def g(topic, message, errors, timestamp, annotation):
                 try:
                     f2 = f()
                     if f2:
                         f2(message)
-                except:
+                except Exception:
                     try:
                         if errors:
                             if not alreadyLogged[0]:
-                                handleError(f2,topic,message)
-                            alreadyLogged[0]=True
+                                handleError(f2, topic, message)
+                            alreadyLogged[0] = True
                     except Exception as e:
-                            print("err",e)
+                        print("err", e)
         else:
-            raise ValueError("Invalid function signature(0,1,2, or 4 args supported, not "+str(args)+")")
+            raise ValueError(
+                "Invalid function signature(0,1,2, or 4 args supported, not " + str(args) + ")")
 
-        #Ref to the weakref so it's easy to check if the function we are wrapping
-        #Still exists.
-        g.originalFunction = f    
+        # Ref to the weakref so it's easy to check if the function we are wrapping
+        # Still exists.
+        g.originalFunction = f
         return g
 
-
-
-    def _post(self, topic,message,errors,timestamp,annotation,executor=None):
+    def _post(self, topic, message, errors, timestamp, annotation, executor=None):
 
         executor = executor or self.executor
 
         matchingtopics = self.parseTopic(topic)
-        #We can't iterate on anything that could possibly change so we make copies
+        # We can't iterate on anything that could possibly change so we make copies
         d = self.subscribers_immutable
         for i in matchingtopics:
             if i in d:
-                #When we find a match, we make a copy of that subscriber list
+                # When we find a match, we make a copy of that subscriber list
                 x = d[i][:]
-                #And iterate the copy
+                # And iterate the copy
                 for f in x:
-                    #we call the ref to get its refferent
-                    #An error could happen in the subscriber
-                    #Or a typeerror could because the weakref has been collected
-                    #We ignore both of these errors and move on
-                    executor(f,(topic,message,errors,timestamp,annotation))
-
-    def postMessage(self, topic, message,errors=True, timestamp=None,annotation=None, synchronous=False):
-        #Use the executor to run the post message job
-        #To allow for the possibility of it running in the background as a thread
-        topic=normalize_topic(topic)
+                    # we call the ref to get its refferent
+                    # An error could happen in the subscriber
+                    # Or a typeerror could because the weakref has been collected
+                    # We ignore both of these errors and move on
+                    executor(f, (topic, message, errors, timestamp, annotation))
+
+    def postMessage(self, topic: str, message: Any, errors: bool = True, timestamp: Optional[float] = None, annotation: Any = None, synchronous: bool = False):
+        # Use the executor to run the post message job
+        # To allow for the possibility of it running in the background as a thread
+        topic = normalize_topic(topic)
         try:
             topic = str(topic)
         except Exception:
             raise TypeError("Topic must be a string or castable to a string.")
 
         timestamp = timestamp or time.monotonic()
-        self._post(topic,message,errors,timestamp, annotation, runFunction if synchronous else None)
+        self._post(topic, message, errors, timestamp, annotation,
+                   runFunction if synchronous else None)
 
 
-#Setup the default system messagebus
+# Setup the default system messagebus
 _bus = MessageBus(workers.do)
 subscribe = _bus.subscribe
 unsubscribe = _bus.unsubscribe
 postMessage = _bus.postMessage
```

### Comparing `scullery-0.1.8/scullery/mnemonics.py` & `scullery-0.1.9/scullery/mnemonics.py`

 * *Files identical despite different names*

### Comparing `scullery-0.1.8/scullery/mqtt.py` & `scullery-0.1.9/scullery/mqtt.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,19 +19,19 @@
 import logging
 import time
 import uuid
 import traceback
 import json
 import asyncio
 
-from scullery import messagebus, workers, util
+from kaithem.src.scullery import messagebus, workers, util
 
 try:
     import msgpack
-except:
+except Exception:
     pass
 
 logger = logging.getLogger("system.mqtt")
 
 
 connections = {}
 
@@ -43,177 +43,94 @@
 
 
 # list them by local name.  But only real, phsyical MQTT connections.
 # This is how passive connections find their real one
 connectionsByBusName = weakref.WeakValueDictionary()
 
 
-def checkIfConnected(c, delay):
-    time.sleep(delay)
-    if not c.isConnected:
-        logging.warning("An MQTT connection to : " + str(c.server) + " was not connected after "+str(delay) + " seconds of waiting")
 
 
 def getWeakrefHandlers(self):
     self = weakref.ref(self)
 
     def on_connect(client, userdata=None, flags=None, rc=0, *a):
         if not rc == 0:
             self().onDisconnected()
             return
 
-        logger.info("Connected to MQTT server: " +
-                    self().server + "result code " + str(rc))
+        logger.info(
+            "Connected to MQTT server: " + self().server + "result code " + str(rc)
+        )
         self().onStillConnected()
         # Don't block the network thread too long
 
         def subscriptionRefresh():
             try:
                 with self().lock:
                     for i in allSubscriptions:
                         # Here the bus prefix is our connection ID
                         if i[0] == self().busPrefix:
                             if allSubscriptions[i]():
                                 # Refresh all subscriptions
                                 self().connection.subscribe(i[1], i[2])
-            except:
+            except Exception:
                 logger.exception("Error subscription refresh")
+
         workers.do(subscriptionRefresh)
 
     def on_disconnect(client, *a):
         if not self():
             return
         logger.info("Disconnected from MQTT server: " + self().server)
         self().onDisconnected()
         logger.info("Disconnected from MQTT server: " + self().server)
 
     def on_message(client, userdata, msg):
         try:
             s = self()
             # Everything must be fine, because we are getting messages
-            messagebus.postMessage(s.busPrefix + "/in/" + msg.topic,
-                                   msg.payload,
-                                   )
+            messagebus.postMessage(
+                s.busPrefix + "/in/" + msg.topic,
+                msg.payload,
+            )
             s.onStillConnected()
         except Exception:
             print(traceback.format_exc())
 
     return on_connect, on_disconnect, on_message
 
 
 # Used to fake a crash fro unit testing purposes
-testCrashOnce = False
 
 
-def makeThread(c, ref):
-    def f2():
-        global testCrashOnce
-        try:
-            if testCrashOnce:
-                testCrashOnce = False
-                raise RuntimeError("Test crash once")
-            c.loop_forever(retry_first_connection=True)
-        except:
-            if ref():
-                ref().onConnectionCrash(traceback.format_exc())
-                logger.exception("MQTT Crash")
-
-    return f2
-
-
-class HBMQTTMessage():
-    pass
 
 
-class HBMQTTWrapper():
-    def __init__(self, manager_ref, client) -> None:
-        self.client = client
-        self.ref = manager_ref()
-        from hbmqtt.mqtt.constants import QOS_0, QOS_1, QOS_2
-        self.qosmap = {0: QOS_0, 1: QOS_1, 2: QOS_2}
-        # For connect_async
-        self.connectFunction = None
-
-    def subscribe(self, topic, qos=0):
-        @asyncio.coroutine
-        def f():
-            yield from self.client.subscribe([(topic, self.qosmap[qos])])
-
-        asyncio.get_event_loop().run_until_complete(f())
-
-    def unsubscribe(self, topic):
-        @asyncio.coroutine
-        def f():
-            yield from self.client.unsubscribe([topic])
-
-        asyncio.get_event_loop().run_until_complete(f())
-
-    def publish(self, topic, payload, qos=0, retain=False):
-        @asyncio.coroutine
-        def f():
-            yield from self.client.publish(topic, payload, self.qosmap[qos], retain)
-
-        asyncio.get_event_loop().run_until_complete(f())
-
-    def connect_async(self, host, port=1883, keepalive=60, bind_address=""):
-        def connectFunction():
-
-            @asyncio.coroutine
-            def f():
-                yield from self.client.connect(host + ":" + port)
-
-            asyncio.get_event_loop().run_until_complete(f())
-        self.connectFunction = connectFunction
-
-    def connect(self, host, port=1883, keepalive=60, bind_address=""):
-        self.connect_async(host, port, keepalive, bind_address)
-        self.connectFunction()
-
-    def loop_forever(timeout=1.0, max_packets=1, retry_first_connection=False):
-        if self.connectFunction:
-            self.connectFunction()
-
-    @asyncio.coroutine
-    def run(self):
-        r = self.ref
-        from hbmqtt.client import MQTTClient, ClientException
-
-        C = MQTTClient()
-        yield from C.connect(r().server + ':' + str(r().port))
-        self.connected = True
-        # Subscribe to '$SYS/broker/uptime' with QOS=1
-        # Subscribe to '$SYS/broker/load/#' with QOS=2
-        self.on_connect(self, None, None, None)
-
-        while r():
-
-            message = yield from C.deliver_message(timeout=3)
-            packet = message.publish_packet
-            msg = HBMQTTMessage
-            msg.payload = packet.payload.data
-            msg.packet.variable_header.topic_name
-            self.on_message(None, None, msg)
-
-        yield from C.disconnect()
-
-
-class Connection():
-    def __init__(self, server, port=1883, password=None, messageBusName=None, *, alertPriority="info", alertAck=True, connectionID=''):
-
+class Connection:
+    def __init__(
+        self,
+        server,
+        port=1883,
+        password=None,
+        messageBusName=None,
+        *,
+        alertPriority="info",
+        alertAck=True,
+        connectionID=""
+    ):
         # ConnectionID is used to ensure separate *physical* connections and prevent reuse
         self.server = server
         self.port = port
         self.lock = threading.Lock()
         self.password = password
 
         self.messageBusName = messageBusName
         self.connection = None
 
-        #Defensive against None
-        connectionID = connectionID or ''
+        # Defensive against None
+        connectionID = connectionID or ""
 
         self.isConnected = False
 
         if not server:
             passive = True
         else:
             passive = False
@@ -221,40 +138,43 @@
         self.passive = passive
 
         server = server or str(uuid.uuid4())
         virtual = server.startswith("__virtual__")
 
         if passive and (not messageBusName):
             raise ValueError(
-                "No server specified. To create a passive connection you must specify an internal messageBusName")
-        self.busPrefix = "/mqtt/" + server + ":" + str(port) + (connectionID or '')
+                "No server specified. To create a passive connection you must specify an internal messageBusName"
+            )
+        self.busPrefix = "/mqtt/" + server + ":" + str(port) + (connectionID or "")
 
         self.subscriptions = {}
         logger.info("Creating connection object to: " + self.server)
 
         self.localStatusTopic = self.busPrefix + "/connectionStatus"
 
         # paho requires non-python stuff.
         try:
             import paho.mqtt.client as mqtt
+
             paho = True
 
         except ImportError:
             logging.exception(
-                "PahoMQTT not installed. No MQTT connection possible here. continuing with dummy.")
+                "PahoMQTT not installed. No MQTT connection possible here. continuing with dummy."
+            )
             paho = False
 
         # When we wrap a function store a weakref to the original here,
         # Pplus the wrapper, so the wrapper doesn't get GCed till
         # The wearkref callback deletes it.
         self.subscribeWrappers = {}
 
         with lock:
             if connectionID:
-                connectionID = '?' + connectionID
+                connectionID = "?" + connectionID
             self.connectionID = connectionID
 
             n = server + ":" + str(port) + connectionID
             if n in connections and connections[n]():
                 raise RuntimeError("There is already a connection")
             torm = []
             for i in connections:
@@ -264,93 +184,53 @@
                 del connections[i]
             connections[n] = weakref.ref(self)
 
             if messageBusName:
                 self.busPrefix = "/mqtt/" + messageBusName
 
             try:
-
                 if not virtual and not passive:
+
                     def out_handler(topic, message, timestamp, annotation):
-                        self.connection.publish(topic[len(
-                            self.busPrefix + "/out/"):], payload=message, qos=annotation[0], retain=annotation[1])
+                        self.connection.publish(
+                            topic[len(self.busPrefix + "/out/") :],
+                            payload=message,
+                            qos=annotation[0],
+                            retain=annotation[1],
+                        )
+
                 else:
                     if not passive:
                         # Virtual loopback server doesn't actually use a real server
                         def out_handler(topic, message, timestamp, annotation):
-                            t = topic[len(self.busPrefix + "/out/"):]
-                            messagebus.postMessage(
-                                self.busPrefix + "/in/" + t, message)
+                            t = topic[len(self.busPrefix + "/out/") :]
+                            messagebus.postMessage(self.busPrefix + "/in/" + t, message)
 
                 if not passive:
-                    messagebus.subscribe(
-                        self.busPrefix + "/out/#", out_handler)
+                    messagebus.subscribe(self.busPrefix + "/out/#", out_handler)
                     self.out_handler = out_handler
 
                 if not virtual and not passive:
                     x = server.split("@")
 
                     if len(x) == 2:
                         host = x[1]
                         user = x[0]
                     elif len(x) == 1:
                         host = x[0]
                         user = None
                     else:
-                        raise ValueError(
-                            "More than one @ symbol in server name??")
+                        raise ValueError("More than one @ symbol in server name??")
 
                     self.username = user
                     self.password = password
 
                     self.configureAlert(alertPriority, alertAck)
 
-                    if paho:
-                        # Ok so the connection is supposed to do this by itself. Some condition can
-                        # Cause the loop to crash and I do not know what!
-                        def reconnect():
-                            try:
-                                if self.connection:
-                                    self.connection.disconnect()
-                            except:
-                                pass
-
-                            self.connection = mqtt.Client()
-                            # We don't want the connection to stringly reference us, that would interfere with GC
-                            on_connect, on_disconnect, on_message = getWeakrefHandlers(
-                                self)
-
-                            if self.username:
-                                self.username_pw_set(
-                                    self.username, self.password)
-
-                            self.connection.connect_async(
-                                host, port=port, keepalive=60, bind_address="")
-
-                            self.connection.on_connect = on_connect
-                            self.connection.on_disconnect = on_disconnect
-                            self.connection.on_message = on_message
-
-                            self._thread = threading.Thread(target=makeThread(
-                                self.connection, weakref.ref(self)), name=server + ":" + str(port), daemon=True)
-                            self._thread.start()
-
-                    # Independant hbmqtt implementation
-                    else:
-                        raise RuntimeError(
-                            "Only Paho is supported at the moment")
 
-                    self.reconnect = reconnect
-
-                    # Actually do the connection.
-                    self.reconnect()
-                    # Give it 5 mins before we print a warning.
-                    def f():
-                        checkIfConnected(self,5)
-                    workers.do(f)
                 else:
                     self.connection = None
                     self.configureAlert(alertPriority, alertAck)
                     self.onStillConnected()
 
                 if not passive:
                     connectionsByBusName[self.busPrefix] = self
@@ -375,49 +255,51 @@
     def onStillConnected(self):
         if not self.isConnected:
             messagebus.postMessage(self.localStatusTopic, "connected")
         self.isConnected = True
         pass
 
     def onDisconnected(self):
-        logging.warning("A connection has disconnected from MQTT server: " + self.server)
+        logging.warning(
+            "A connection has disconnected from MQTT server: " + self.server
+        )
         if self.isConnected:
             messagebus.postMessage(self.localStatusTopic, "disconnected")
         self.isConnected = False
-        
 
     def subscribeToStatus(self, f):
         messagebus.subscribe(self.localStatusTopic, f)
 
     def close(self):
         # Attempt cleanup
         try:
             self.connection.disconnect()
         except Exception:
             pass
         try:
-            del connections[self.server + ":" +
-                            str(self.port) + self.connectionID]
+            del connections[self.server + ":" + str(self.port) + self.connectionID]
         except Exception:
             pass
 
     def __del__(self):
         if self.connection:
             self.connection.disconnect()
 
     def unsubscribe(self, topic, function):
-
         with self.lock:
-
             # Very expensive to search this dict like this, but unsub shouldn't happen much.
             try:
                 torm = []
                 # Find any subscriptions to the topic for this particular bus prefix and delete them
                 for i in allSubscriptions:
-                    if i[0] == self.busPrefix and i[1] == topic and allSubscriptions[i]() == function:
+                    if (
+                        i[0] == self.busPrefix
+                        and i[1] == topic
+                        and allSubscriptions[i]() == function
+                    ):
                         torm.append(i)
                 for i in torm:
                     allSubscriptions.pop(i)
             except KeyError:
                 print(traceback.format_exc())
                 pass
 
@@ -436,16 +318,15 @@
             for i in self.subscribeWrappers:
                 x = self.subscribeWrappers[i]
                 if x[2] == topic:
                     return
 
             # We could not find even a single subscriber function
             # So we unsubscribe at the MQTT level
-            logging.debug("MQTT Unsubscribe from " +
-                          topic + " at " + self.server)
+            logging.debug("MQTT Unsubscribe from " + topic + " at " + self.server)
             if self.connection:
                 self.connection.unsubscribe(topic)
 
     def configureAlert(self, *a):
         pass
 
     def _mqttSubscribe(topic, qos):
@@ -495,108 +376,134 @@
         # Connection.subscribe was blocking forever.
         # Use a different thread, to hopefully avoid deadlocks
 
         def backgroundSubscribeTask():
             with self.lock:
                 self.connection.subscribe(topic, qos)
 
-        if encoding == 'json':
+        if encoding == "json":
+
             def wrapper(t, m):
                 # Get rid of the extra kaithem framing part of the topic
-                t = t[len(self.busPrefix + "/in/"):]
+                t = t[len(self.busPrefix + "/in/") :]
                 if not isinstance(m, str):
-                    m = m.decode('utf-8')
+                    m = m.decode("utf-8")
                 try:
                     m = json.loads(m)
-                except:
+                except Exception:
                     logging.debug("Bad JSON:" + m[:64])
                 function()(t, m)
 
-        elif encoding == 'msgpack':
+        elif encoding == "msgpack":
+
             def wrapper(t, m):
                 # Get rid of the extra kaithem framing part of the topic
-                t = t[len(self.busPrefix + "/in/"):]
+                t = t[len(self.busPrefix + "/in/") :]
                 function()(t, msgpack.unpackb(m, raw=False))
 
-        elif encoding == 'utf8':
+        elif encoding == "utf8":
+
             def wrapper(t, m):
                 # Get rid of the extra kaithem framing part of the topic
-                t = t[len(self.busPrefix + "/in/"):]
+                t = t[len(self.busPrefix + "/in/") :]
                 if not isinstance(m, str):
-                    m = m.decode('utf-8')
+                    m = m.decode("utf-8")
                 function()(t, m)
 
-        elif encoding == 'raw':
+        elif encoding == "raw":
+
             def wrapper(t, m):
                 # Get rid of the extra kaithem framing part of the topic
-                t = t[len(self.busPrefix + "/in/"):]
+                t = t[len(self.busPrefix + "/in/") :]
                 function()(t, m)
+
         else:
             raise ValueError("Invalid encoding: " + encoding)
 
         # Correctly call message bus error handlers
         wrapper.messagebusWrapperFor = function
 
         internalTopic = self.busPrefix + "/in/" + topic
 
         # Extra data is mostly used for unsubscription
         self.subscribeWrappers[x] = (function, wrapper, topic, internalTopic)
 
-        logging.debug("MQTT subscribe to " + topic + " at " + self.server)
+        # logging.debug("MQTT subscribe to " + topic + " at " + self.server)
         # Ref to f exists as long as the original does because it's kept in subscribeWrappers
         messagebus.subscribe(internalTopic, wrapper)
 
         # Important we do this *after*, because the server might auto-send us something that could be important for.
         # Only the first function will get it, but whatever, at least we can see certain things when manually subscribing, for test purposes.
         # Or should we do it before, to resolve that bit of ambiguity and never get the message???
         if self.connection:
             workers.do(backgroundSubscribeTask)
 
     def publish(self, topic, message, qos=2, encoding="json", retain=False):
-        if encoding == 'json':
+        if encoding == "json":
             message = json.dumps(message)
-        elif encoding == 'msgpack':
+        elif encoding == "msgpack":
             message = msgpack.packb(message, use_bin_type=True)
-        elif encoding == 'utf8':
+        elif encoding == "utf8":
             message = message.encode("utf8")
-        elif encoding == 'raw':
+        elif encoding == "raw":
             pass
         else:
             raise ValueError("Invalid encoding!")
-        messagebus.postMessage(self.busPrefix + "/out/" +
-                               topic, message, annotation=(qos, retain))
+        messagebus.postMessage(
+            self.busPrefix + "/out/" + topic, message, annotation=(qos, retain)
+        )
 
 
-def getConnection(server, port=1883, password=None, messageBusName=None, *, alertPriority="info", alertAck=True, connectionID=''):
+def getConnection(
+    server,
+    port=1883,
+    password=None,
+    messageBusName=None,
+    *,
+    alertPriority="info",
+    alertAck=True,
+    connectionID=""
+):
     # Kaithem is gonna monkeypatch kaithem with one that has better
     # logging
     global Connection
 
     # Blank password means no password
     password = password or None
     with lock:
         x = None
 
-        connectionIDSuffix = ''
+        connectionIDSuffix = ""
         if connectionID:
-            connectionIDSuffix = '?' + connectionID
+            connectionIDSuffix = "?" + connectionID
 
         if server + ":" + str(port) + connectionIDSuffix in connections:
             x = connections[server + ":" + str(port) + connectionIDSuffix]()
 
         if x:
             if not messageBusName == x.messageBusName:
-               # We can safely use the existing one.   If t
+                # We can safely use the existing one.   If t
                 logging.warning(
-                    "Using connection that already exists, but with a different message bus name:  " + x.messageBusName)
+                    "Using connection that already exists, but with a different message bus name:  "
+                    + x.messageBusName
+                )
 
                 messageBusName = x.messageBusName
 
             if x.password or password:
                 if not x.password == password:
                     raise ValueError(
-                        "There is already a connection to the same host and user, but with a different password.")
+                        "There is already a connection to the same host and user, but with a different password."
+                    )
 
             x.configureAlert(alertPriority, alertAck)
             return x
 
-        return Connection(server, port, password=password, alertAck=True, alertPriority="info", messageBusName=messageBusName, connectionID=connectionID)
+        return Connection(
+            server,
+            port,
+            password=password,
+            alertAck=True,
+            alertPriority="info",
+            messageBusName=messageBusName,
+            connectionID=connectionID,
+        )
```

### Comparing `scullery-0.1.8/scullery/persist.py` & `scullery-0.1.9/scullery/persist.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,30 +16,28 @@
 
 posix_rename = False
 if sys.platform.startswith('linux'):
     posix_rename =True
 if sys.platform.startswith('darwin'):
     posix_rename =True
 
+# Purely just a dict for the rest of the application to keep track of what files are changed and not saved.
+unsavedFiles = {}
 
 def resolvePath(fn,expand=True):
     if not expand:
         return fn
     return (os.path.expandvars(os.path.expanduser(fn)))
 
 
 
 #TODO: Ensure only one thread can save a file at a time
 
-if sys.version_info <(3,0):
-    import StringIO
-    strio = StringIO.StringIO
-else:
-    import io
-    strio = io.BytesIO
+import io
+strio = io.BytesIO
 
 persisters = []
 
 #must be Rlock because load is recursive
 lock = threading.RLock()
 
 def saveExecutor(f):
@@ -47,17 +45,17 @@
     f()
 
 def saveAllAtExit():
     while persisters:
         i = persisters.pop()()
         try:
             i.save()
-        except:
-            logging.exception()
-
+        except Exception:
+            logging.exception("err")
+import stat
 def chmod_private_try(p, execute=True):
     try:
         if execute:
             os.chmod(p,stat.S_IRUSR|stat.S_IWUSR|stat.S_IXUSR|stat.S_IRGRP|stat.S_IWGRP|stat.S_IXGRP)
         else:
             os.chmod(p,stat.S_IRUSR|stat.S_IWUSR|stat.S_IRGRP|stat.S_IWGRP)
     except Exception as e:
@@ -68,15 +66,15 @@
         os.makedirs(d)
 
 class Persister():
     def __init__(self,fn,default=None):
         self.fn= fn
         try:
             self.reload()
-        except:
+        except Exception:
             self.value = default
         torm = []
         #Before we add ourselves, clear out any old persisters that are no longer needed.
         for i in persisters:
             if not i():
                 torm.append(i)
         for i in torm:
@@ -138,14 +136,19 @@
             x=fn
         #Encode the data into our chosen format
         if x.endswith(".json"):
             data = json.dumps(data).encode('utf8')
         elif x.endswith(".yaml"):
             import yaml
             data = yaml.dump(data).encode('utf8')
+
+        elif x.endswith(".toml"):
+            import toml
+            data = toml.dumps(data).encode("utf8")
+
         elif x.endswith(".txt") or x.endswith(".md") or x.endswith(".rst"):
             data = (str(data).encode('utf8'))
         elif x.endswith(".bin"):
             data = (data)
         else:
             raise ValueError('Unsupported or missing File Extension')
 
@@ -228,26 +231,31 @@
                 f = open(filename,'rb')
                 x = filename
 
             if x.endswith(".json"):
                 r=json.loads(f.read().decode('utf8'))
             elif x.endswith(".yaml"):
                 import yaml
-                r=yaml.load(f.read().decode('utf8'))
+                r=yaml.load(f.read().decode('utf8'), Loader=yaml.SafeLoader)
+
+            elif x.endswith(".toml"):
+                import toml
+                r = toml.loads(f.read().decode('utf8'))
+
             elif x.endswith(".txt") or x.endswith(".md") or x.endswith(".rst"):
                 r=f.read().decode('utf8')
             elif x.endswith(".bin"):
                 r=f.read()
             else:
                 raise ValueError('Unsupported File Extension')
         except Exception as e:
             try:
                 f.close()
-            except:
+            except Exception:
                 pass
             raise
         try:
             f.close()
-        except:
+        except Exception:
             pass
 
         return r
```

### Comparing `scullery-0.1.8/scullery/sip.py` & `scullery-0.1.9/scullery/sip.py`

 * *Files identical despite different names*

### Comparing `scullery-0.1.8/scullery/thirdparty/baresipy/__init__.py` & `scullery-0.1.9/scullery/thirdparty/baresipy/__init__.py`

 * *Files identical despite different names*

### Comparing `scullery-0.1.8/scullery/thirdparty/baresipy/baresip_template/accounts` & `scullery-0.1.9/scullery/thirdparty/baresipy/baresip_template/accounts`

 * *Files identical despite different names*

### Comparing `scullery-0.1.8/scullery/thirdparty/baresipy/baresip_template/config` & `scullery-0.1.9/scullery/thirdparty/baresipy/baresip_template/config`

 * *Files identical despite different names*

### Comparing `scullery-0.1.8/scullery/thirdparty/baresipy/contacts.py` & `scullery-0.1.9/scullery/thirdparty/baresipy/contacts.py`

 * *Files identical despite different names*

### Comparing `scullery-0.1.8/scullery/thirdparty/baresipy/utils/log.py` & `scullery-0.1.9/scullery/thirdparty/baresipy/utils/log.py`

 * *Files identical despite different names*

### Comparing `scullery-0.1.8/scullery/thirdparty/fluidsynth/__init__.py` & `scullery-0.1.9/scullery/thirdparty/fluidsynth/__init__.py`

 * *Files identical despite different names*

### Comparing `scullery-0.1.8/scullery/units.py` & `scullery-0.1.9/scullery/units.py`

 * *Files 6% similar despite different names*

```diff
@@ -48,22 +48,39 @@
     "%": 0.01,
     "ppm": 100/10**6,
     "ppb": 100/10**9,
     "dB":  (lambda x: 10**(x*10), lambda x: 10*math.log10(x)),
     
     'Pa': 1,
     'psi': 6894.76,
-    'PSI': 6894.76
+    'PSI': 6894.76,
+    'bar': 100000,
+    'millibar': 100,
+
+    'boolean': 1,
+    'bool': 1,
+
+
+    "KPH": 1,
+    "MPH": 1.60934,
+    "km/h": 1
 }
 
-unitTypes={
+unitTypes = {
      #Base unit of mass is grams
     "g":  "mass",
     "lb": "mass",
     "oz": "mass",
+    
+    "boolean": "boolean",
+    "boolean": "boolean",
+
+    "MPH": "speed",
+    "KPH": "speed",
+    "km/h": "speed",
 
     #Base unit of distance is meters
     "m":  "length",
     "in": "length",
 
     #Base unit of temperature is Kelvin
     "K":    "temperature",
@@ -80,15 +97,17 @@
     "ppb":"ratio",
     "U": "ratio",
     "uno": "ratio",
     'dB': "ratio",
 
     'psi': 'pressure',
     'Pa': 'pressure',
-    "PSI": 'pressure'
+    "PSI": 'pressure',
+    'bar':'pressure',
+    'millibar': 'pressure'
 }
 
 _prefixes = {"n":10**-9,"u":10**-6, "m":0.001, "k":1000,"M":1000000,"G":1000000000,"T":1000000000000}
 def getUnitType(u):
     return unitTypes(u)
 
 def parsePrefix(u):
```

### Comparing `scullery-0.1.8/scullery/util.py` & `scullery-0.1.9/scullery/util.py`

 * *Files identical despite different names*

### Comparing `scullery-0.1.8/scullery/words_mnemonic.txt` & `scullery-0.1.9/scullery/words_mnemonic.txt`

 * *Files identical despite different names*

### Comparing `scullery-0.1.8/scullery/workers.py` & `scullery-0.1.9/scullery/workers.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+
 #Copyright Daniel Dunn 2013
 #This file is part of Kaithem Automation.
 
 #Kaithem Automation is free software: you can redistribute it and/or modify
 #it under the terms of the GNU General Public License as published by
 #the Free Software Foundation, version 3.
 
@@ -123,22 +124,23 @@
 
         runningState = [True]
         handle = (e, runningState)
         with spawnLock:
             wakeupHandlesMutable.append(handle)
             wakeupHandles = wakeupHandlesMutable[:]
 
+
         while (run):
             try:
                 runningState[0] = True
                 #While either our direct  queue or the overflow queue has things in it we do them.
                 while (len(taskQueue)):
                     try:
                         f = pop()
-                    except:
+                    except Exception:
                         f = None
 
                     if f:
                         try:
                             f[0](*f[1])
                             lastActivity = monotonic()
                         except Exception:
@@ -151,22 +153,22 @@
                                         f[0].__module__ + "\r\n")
                                     lastWorkersError = monotonic()
 
                                 logger.exception(
                                     "Error in function running in thread pool "
                                     + f[0].__name__ + " from " +
                                     f[0].__module__)
-                            except:
+                            except Exception:
                                 print("Failed to handle error: " +
                                       traceback.format_exc(6))
 
                             for i in backgroundFunctionErrorHandlers:
                                 try:
                                     i(f)
-                                except:
+                                except Exception:
                                     print("Failed to handle error: " +
                                           traceback.format_exc(6))
                         finally:
                             #We do not want f staying around, if might hold references that should be GCed away immediatly
                             f = None
                 #Ensure the lock is acqured so we can sto the next time
                 #We try in blocking mode
@@ -189,89 +191,123 @@
 
                     #Fast prelim check.
                     if len(workers) > minWorkers:
                         #The elements of handle are never copied anywhere,
                         #Once the list is clear, we can be sure there is no further inserts, and the next round will catch almost
                         #all race conditions. Any remaining one in a million ones will be caught in 1 second
                         if lastActivity < (monotonic() - 10):
-                            with spawnLock:
-                                if len(workers) > minWorkers:
-                                    #Only stop one thread per 5 seconds to prevent
-                                    #chattering
-
-                                    #Also don't stop a thread when there aren't at least
-                                    #2 threads that aren't busy.
-                                    unbusyCount = 0
-                                    for i in wakeupHandles:
-                                        if not i[1][0]:
-                                            unbusyCount += 1
-
-                                    if unbusyCount > 2 and lastStoppedThread < (
-                                            monotonic() - 5):
-                                        lastStoppedThread = monotonic()
-                                        shouldRun = None
-                                        del workersMutable[id]
-                                        workers = workersMutable.copy()
-                                        wakeupHandlesMutable.remove(handle)
-                                        wakeupHandles = wakeupHandlesMutable[:]
-            except:
+                            # This should not block.
+                            if spawnLock.acquire(timeout=2):
+                                try:
+                                    if len(workers) > minWorkers:
+                                        #Only stop one thread per 5 seconds to prevent
+                                        #chattering
+
+                                        #Also don't stop a thread when there aren't at least
+                                        #2 threads that aren't busy.
+                                        unbusyCount = 0
+                                        for i in wakeupHandles:
+                                            if not i[1][0]:
+                                                unbusyCount += 1
+
+                                        if unbusyCount > 2 and lastStoppedThread < (
+                                                monotonic() - 5):
+                                            lastStoppedThread = monotonic()
+                                            shouldRun = None
+                                            del workersMutable[id]
+                                            workers = workersMutable.copy()
+                                            wakeupHandlesMutable.remove(handle)
+                                            wakeupHandles = wakeupHandlesMutable[:]
+                                finally:
+                                    spawnLock.release()
+            except Exception:
                 print("Exception in worker loop: " + traceback.format_exc(6))
 
     return workerloop
 
 
 def addWorker():
     global workers
-    with spawnLock:
-        q = []
-        e = threading.Lock()
-        e.acquire()
-
-        id = time.time()
-        #First worker always polls at 100hz
-        t = threading.Thread(target=makeWorker(e, q, id),
-                             name="nostartstoplog.ThreadPoolWorker-" + str(id))
-        workersMutable[id] = t
-        t.start()
-        workers = workersMutable.copy()
+    if spawnLock.acquire(timeout=60):
+        try:
+            q = []
+            e = threading.Lock()
+            e.acquire()
+
+            id = time.time()
+            #First worker always polls at 100hz
+            t = threading.Thread(target=makeWorker(e, q, id),
+                                name="nostartstoplog.ThreadPoolWorker-" + str(id))
+            workersMutable[id] = t
+            t.start()
+            workers = workersMutable.copy()
+        finally:
+            spawnLock.release()
+    else:
+        raise RuntimeError("Could not get the lock!")
 
 
 _append = taskQueue.append
 
 
 def do(func, args=[]):
     """Run a function in the background
 
     funct(function):
         A function of 0 arguments to be ran in the background in another thread immediatly,
     """
 
+    if not callable(func):
+        raise ValueError("Non callable value")
+        
     _append((func, args))
 
     for i in wakeupHandles:
         try:
             if i[0].locked():
                 i[0].release()
                 return
         except RuntimeError:
             pass
 
+    if len(workers)> 4:
+        # Wait and retry before attempting to spawn a new thread, if there is probable already enough.
+        # that is a slow problematic thing
+        time.sleep(0.001)
+        time.sleep(0.0001)
+
+        for i in wakeupHandles:
+            try:
+                if i[0].locked():
+                    i[0].release()
+                    return
+            except RuntimeError:
+                pass
+
     #Sleep 1/25000th of a second for every item in the queue past the max number of threads
     #In an attempt to rate limit
     if len(taskQueue) > maxWorkers:
         time.sleep(max(0, (len(taskQueue) - maxWorkers) / 25000))
 
     #No unbusy threads? It must go in the overflow queue.
     #Soft rate limit here should work a bit better than the old hard limit at keeping away
     #the deadlocks.
     #Under lock
-    with spawnLock:
-        if len(workers) < maxWorkers:
-            addWorker()
-            return
+    
+    #We also need this fast preliminary check to use that lock as rarely as possible.
+    if len(workers) < maxWorkers:
+        if spawnLock.acquire(timeout=15):
+            try:
+                if len(workers) < maxWorkers:
+                    addWorker()
+                    return
+            finally:
+                spawnLock.release()
+        else:
+            print("COULD NOT GET SPAWN LOCK TO CREATE ADDITIONAL THREAD. CONTINUING WITH FEWER THREADS. RESTART SUGGESTED")
 
     #If we can't spawn a new thread
     #Wait a maximum of 15ms before
     #just giving up and leaving
     #it for when somethin
     #wakes up
     for n in range(0, 25):
```

### Comparing `scullery-0.1.8/scullery.egg-info/SOURCES.txt` & `scullery-0.1.9/scullery.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
+LICENSE
 MANIFEST.in
 README.md
 setup.py
-testFile.json
 scullery/__init__.py
 scullery/fluidsynth.py
 scullery/iceflow.py
 scullery/iceflow_server.py
 scullery/jack_client_subprocess.py
 scullery/jacktools.py
 scullery/jsonrpyc.py
```

### Comparing `scullery-0.1.8/setup.py` & `scullery-0.1.9/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="scullery",
-    version="0.1.8",
+    version="0.1.9",
     author="Daniel Dunn",
     author_email="dannydunn@eternityforest.com",
     description="A utility library based on KaithemAutomation featuring a GStreamer wrapper",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/EternityForest/scullery",
     packages=setuptools.find_packages(),
+    package_data={'':["**/scullery/thirdparty/baresip/**"]},
+
+
     include_package_data=True,
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Operating System :: OS Independent"
     ],
     python_requires='>=3.6',
     install_requires=[
           'pyyaml',
           'typeguard',
           "sf2utils",
           "pyFluidSynth",
           "paho-mqtt",
-          "pyreap"
       ],
 )
 
 
 #To push to pypi
 #sudo python3 setup.py sdist bdist_wheel
 #python3 -m twine upload dist/*
```

### Comparing `scullery-0.1.8/tests/testFluidSynth.py` & `scullery-0.1.9/tests/testFluidSynth.py`

 * *Files identical despite different names*

### Comparing `scullery-0.1.8/tests/testGstStability.py` & `scullery-0.1.9/tests/testGstStability.py`

 * *Files identical despite different names*

### Comparing `scullery-0.1.8/tests/testJack.py` & `scullery-0.1.9/tests/testJack.py`

 * *Files identical despite different names*

### Comparing `scullery-0.1.8/tests/testMQTT.py` & `scullery-0.1.9/tests/testMQTT.py`

 * *Files identical despite different names*

### Comparing `scullery-0.1.8/tests/testMessageBus.py` & `scullery-0.1.9/tests/testMessageBus.py`

 * *Files identical despite different names*

### Comparing `scullery-0.1.8/tests/testMisc.py` & `scullery-0.1.9/tests/testMisc.py`

 * *Files identical despite different names*

