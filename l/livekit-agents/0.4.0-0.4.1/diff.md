# Comparing `tmp/livekit-agents-0.4.0.tar.gz` & `tmp/livekit-agents-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "livekit-agents-0.4.0.tar", last modified: Tue Feb 20 16:16:10 2024, max compression
+gzip compressed data, was "livekit-agents-0.4.1.tar", last modified: Sat Apr  6 03:24:48 2024, max compression
```

## Comparing `livekit-agents-0.4.0.tar` & `livekit-agents-0.4.1.tar`

### file list

```diff
@@ -1,33 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 16:16:10.515402 livekit-agents-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-02-20 16:16:10.515402 livekit-agents-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-02-20 16:16:02.000000 livekit-agents-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 16:16:10.511402 livekit-agents-0.4.0/livekit/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 16:16:10.511402 livekit-agents-0.4.0/livekit/agents/
--rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-02-20 16:16:02.000000 livekit-agents-0.4.0/livekit/agents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4570 2024-02-20 16:16:02.000000 livekit-agents-0.4.0/livekit/agents/job_context.py
--rw-r--r--   0 runner    (1001) docker     (127)    11178 2024-02-20 16:16:02.000000 livekit-agents-0.4.0/livekit/agents/job_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      712 2024-02-20 16:16:02.000000 livekit-agents-0.4.0/livekit/agents/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 16:16:10.515402 livekit-agents-0.4.0/livekit/agents/stt/
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-02-20 16:16:02.000000 livekit-agents-0.4.0/livekit/agents/stt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2789 2024-02-20 16:16:02.000000 livekit-agents-0.4.0/livekit/agents/stt/stream_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-02-20 16:16:02.000000 livekit-agents-0.4.0/livekit/agents/stt/stt.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 16:16:10.515402 livekit-agents-0.4.0/livekit/agents/tokenize/
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-02-20 16:16:02.000000 livekit-agents-0.4.0/livekit/agents/tokenize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-02-20 16:16:02.000000 livekit-agents-0.4.0/livekit/agents/tokenize/sentence_tokenizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 16:16:10.515402 livekit-agents-0.4.0/livekit/agents/tts/
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-02-20 16:16:02.000000 livekit-agents-0.4.0/livekit/agents/tts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-02-20 16:16:02.000000 livekit-agents-0.4.0/livekit/agents/tts/stream_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-02-20 16:16:02.000000 livekit-agents-0.4.0/livekit/agents/tts/tts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-02-20 16:16:02.000000 livekit-agents-0.4.0/livekit/agents/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-02-20 16:16:02.000000 livekit-agents-0.4.0/livekit/agents/vad.py
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-02-20 16:16:02.000000 livekit-agents-0.4.0/livekit/agents/version.py
--rw-r--r--   0 runner    (1001) docker     (127)    15951 2024-02-20 16:16:02.000000 livekit-agents-0.4.0/livekit/agents/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 16:16:10.515402 livekit-agents-0.4.0/livekit_agents.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-02-20 16:16:10.000000 livekit-agents-0.4.0/livekit_agents.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-02-20 16:16:10.000000 livekit-agents-0.4.0/livekit_agents.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-20 16:16:10.000000 livekit-agents-0.4.0/livekit_agents.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-02-20 16:16:10.000000 livekit-agents-0.4.0/livekit_agents.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-02-20 16:16:10.000000 livekit-agents-0.4.0/livekit_agents.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-02-20 16:16:02.000000 livekit-agents-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-20 16:16:10.515402 livekit-agents-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-02-20 16:16:02.000000 livekit-agents-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 03:24:48.691515 livekit-agents-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-04-06 03:24:48.691515 livekit-agents-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-06 03:24:41.000000 livekit-agents-0.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 03:24:48.687515 livekit-agents-0.4.1/livekit/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 03:24:48.687515 livekit-agents-0.4.1/livekit/agents/
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-04-06 03:24:41.000000 livekit-agents-0.4.1/livekit/agents/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 03:24:48.687515 livekit-agents-0.4.1/livekit/agents/codecs/
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-06 03:24:41.000000 livekit-agents-0.4.1/livekit/agents/codecs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3201 2024-04-06 03:24:41.000000 livekit-agents-0.4.1/livekit/agents/codecs/mp3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4570 2024-04-06 03:24:41.000000 livekit-agents-0.4.1/livekit/agents/job_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11178 2024-04-06 03:24:41.000000 livekit-agents-0.4.1/livekit/agents/job_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-06 03:24:41.000000 livekit-agents-0.4.1/livekit/agents/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 03:24:48.687515 livekit-agents-0.4.1/livekit/agents/stt/
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-06 03:24:41.000000 livekit-agents-0.4.1/livekit/agents/stt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2789 2024-04-06 03:24:41.000000 livekit-agents-0.4.1/livekit/agents/stt/stream_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-04-06 03:24:41.000000 livekit-agents-0.4.1/livekit/agents/stt/stt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 03:24:48.691515 livekit-agents-0.4.1/livekit/agents/tokenize/
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-06 03:24:41.000000 livekit-agents-0.4.1/livekit/agents/tokenize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-06 03:24:41.000000 livekit-agents-0.4.1/livekit/agents/tokenize/sentence_tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 03:24:48.691515 livekit-agents-0.4.1/livekit/agents/tts/
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-06 03:24:41.000000 livekit-agents-0.4.1/livekit/agents/tts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-04-06 03:24:41.000000 livekit-agents-0.4.1/livekit/agents/tts/stream_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-04-06 03:24:41.000000 livekit-agents-0.4.1/livekit/agents/tts/tts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-04-06 03:24:41.000000 livekit-agents-0.4.1/livekit/agents/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-04-06 03:24:41.000000 livekit-agents-0.4.1/livekit/agents/vad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-06 03:24:41.000000 livekit-agents-0.4.1/livekit/agents/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16635 2024-04-06 03:24:41.000000 livekit-agents-0.4.1/livekit/agents/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 03:24:48.691515 livekit-agents-0.4.1/livekit_agents.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-04-06 03:24:48.000000 livekit-agents-0.4.1/livekit_agents.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-06 03:24:48.000000 livekit-agents-0.4.1/livekit_agents.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 03:24:48.000000 livekit-agents-0.4.1/livekit_agents.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-06 03:24:48.000000 livekit-agents-0.4.1/livekit_agents.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-06 03:24:48.000000 livekit-agents-0.4.1/livekit_agents.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-06 03:24:41.000000 livekit-agents-0.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 03:24:48.691515 livekit-agents-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-04-06 03:24:41.000000 livekit-agents-0.4.1/setup.py
```

### Comparing `livekit-agents-0.4.0/PKG-INFO` & `livekit-agents-0.4.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: livekit-agents
-Version: 0.4.0
+Version: 0.4.1
 Summary: LiveKit Python Agents
 Home-page: https://github.com/livekit/agents
 License: Apache-2.0
 Project-URL: Documentation, https://docs.livekit.io
 Project-URL: Website, https://livekit.io/
 Project-URL: Source, https://github.com/livekit/agents
 Keywords: webrtc,realtime,audio,video,livekit,agents,AI
@@ -18,13 +18,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.9.0
 Description-Content-Type: text/markdown
 Requires-Dist: click~=8.1.0
 Requires-Dist: livekit>=0.9.0
 Requires-Dist: livekit-api>=0.4.1
-Requires-Dist: livekit-protocol>=0.3.0
+Requires-Dist: livekit-protocol~=0.3.0
 Requires-Dist: websockets<13,>=12
+Provides-Extra: codecs
+Requires-Dist: pyav>=12.0.2; extra == "codecs"
 
 # LiveKit Agents
 
 The core LiveKit Agents Framework. See top-level README for more information.
```

### Comparing `livekit-agents-0.4.0/livekit/agents/__init__.py` & `livekit-agents-0.4.1/livekit/agents/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     Worker,
     JobCancelledError,
     AssignmentTimeoutError,
     JobType,
     run_app,
 )
 from .plugin import Plugin
-from .utils import AudioBuffer, merge_frames
+from .utils import AudioBuffer, merge_frames, AsyncIterableQueue
 from .job_request import AutoSubscribe, AutoDisconnect, JobRequest
 from .job_context import JobContext
 
 from . import stt
 from . import vad
 from . import tts
 from . import tokenize
@@ -41,12 +41,13 @@
     "JobCancelledError",
     "AssignmentTimeoutError",
     "Plugin",
     "run_app",
     "JobType",
     "AudioBuffer",
     "merge_frames",
+    "AsyncIterableQueue",
     "stt",
     "vad",
     "tts",
     "tokenize",
 ]
```

### Comparing `livekit-agents-0.4.0/livekit/agents/job_context.py` & `livekit-agents-0.4.1/livekit/agents/job_context.py`

 * *Files identical despite different names*

### Comparing `livekit-agents-0.4.0/livekit/agents/job_request.py` & `livekit-agents-0.4.1/livekit/agents/job_request.py`

 * *Files identical despite different names*

### Comparing `livekit-agents-0.4.0/livekit/agents/plugin.py` & `livekit-agents-0.4.1/livekit/agents/plugin.py`

 * *Files identical despite different names*

### Comparing `livekit-agents-0.4.0/livekit/agents/stt/stream_adapter.py` & `livekit-agents-0.4.1/livekit/agents/stt/stream_adapter.py`

 * *Files identical despite different names*

### Comparing `livekit-agents-0.4.0/livekit/agents/stt/stt.py` & `livekit-agents-0.4.1/livekit/agents/stt/stt.py`

 * *Files identical despite different names*

### Comparing `livekit-agents-0.4.0/livekit/agents/tokenize/sentence_tokenizer.py` & `livekit-agents-0.4.1/livekit/agents/tokenize/sentence_tokenizer.py`

 * *Files identical despite different names*

### Comparing `livekit-agents-0.4.0/livekit/agents/tts/stream_adapter.py` & `livekit-agents-0.4.1/livekit/agents/tts/stream_adapter.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,19 @@
-import logging
 import asyncio
+import logging
+from typing import AsyncIterable
+
+from ..tokenize import SentenceStream, SentenceTokenizer
 from .tts import (
     TTS,
-    SynthesizeStream,
     SynthesisEvent,
     SynthesisEventType,
     SynthesizedAudio,
+    SynthesizeStream,
 )
-from ..tokenize import SentenceTokenizer, SentenceStream
 
 
 class StreamAdapterWrapper(SynthesizeStream):
     def __init__(self, tts: TTS, sentence_stream: SentenceStream) -> None:
         super().__init__()
         self._closed = False
         self._tts = tts
@@ -19,15 +21,15 @@
         self._queue = asyncio.Queue[str]()
         self._event_queue = asyncio.Queue[SynthesisEvent]()
 
         self._main_task = asyncio.create_task(self._run())
 
         def log_exception(task: asyncio.Task) -> None:
             if not task.cancelled() and task.exception():
-                logging.error(f"google speech task failed: {task.exception()}")
+                logging.error(f"speech task failed: {task.exception()}")
 
         self._main_task.add_done_callback(log_exception)
 
     async def _run(self) -> None:
         while True:
             try:
                 sentence = await self._sentence_stream.__anext__()
@@ -62,12 +64,12 @@
 
 class StreamAdapter(TTS):
     def __init__(self, tts: TTS, tokenizer: SentenceTokenizer) -> None:
         super().__init__(streaming_supported=True)
         self._tts = tts
         self._tokenizer = tokenizer
 
-    async def synthesize(self, *, text: str) -> SynthesizedAudio:
-        return await self._tts.synthesize(text=text)
+    def synthesize(self, *, text: str) -> AsyncIterable[SynthesizedAudio]:
+        return self._tts.synthesize(text=text)
 
     def stream(self) -> SynthesizeStream:
         return StreamAdapterWrapper(self._tts, self._tokenizer.stream())
```

### Comparing `livekit-agents-0.4.0/livekit/agents/tts/tts.py` & `livekit-agents-0.4.1/livekit/agents/tts/tts.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from abc import ABC, abstractmethod
-from typing import Optional
+from dataclasses import dataclass
 from enum import Enum
+from typing import AsyncIterable, Optional
+
 from livekit import rtc
-from dataclasses import dataclass
 
 
 @dataclass
 class SynthesizedAudio:
     text: str
     data: rtc.AudioFrame
 
@@ -50,15 +51,15 @@
 
 
 class TTS(ABC):
     def __init__(self, *, streaming_supported: bool) -> None:
         self._streaming_supported = streaming_supported
 
     @abstractmethod
-    async def synthesize(self, *, text: str) -> SynthesizedAudio:
+    def synthesize(self, *, text: str) -> AsyncIterable[SynthesizedAudio]:
         pass
 
     def stream(self) -> SynthesizeStream:
         raise NotImplementedError(
             "streaming is not supported by this TTS, please use a different TTS or use a StreamAdapter"
         )
```

### Comparing `livekit-agents-0.4.0/livekit/agents/vad.py` & `livekit-agents-0.4.1/livekit/agents/vad.py`

 * *Files identical despite different names*

### Comparing `livekit-agents-0.4.0/livekit/agents/version.py` & `livekit-agents-0.4.1/livekit/agents/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "0.4.0"
+__version__ = "0.4.1"
```

### Comparing `livekit-agents-0.4.0/livekit/agents/worker.py` & `livekit-agents-0.4.1/livekit/agents/worker.py`

 * *Files 2% similar despite different names*

```diff
@@ -385,14 +385,18 @@
         "--log-level",
         default="INFO",
         type=click.Choice(
             ["DEBUG", "INFO", "WARNING", "ERROR", "CRITICAL"], case_sensitive=False
         ),
         help="Set the logging level",
     )
+    def cli(log_level: str) -> None:
+        logging.basicConfig(level=log_level)
+
+    @cli.command(help="Start the worker")
     @click.option(
         "--url",
         required=True,
         envvar="LIVEKIT_URL",
         help="LiveKit server or Cloud project WebSocket URL",
         default="ws://localhost:7880",
     )
@@ -404,28 +408,49 @@
     )
     @click.option(
         "--api-secret",
         envvar="LIVEKIT_API_SECRET",
         help="LiveKit server or Cloud project's API secret",
         required=True,
     )
-    def cli(log_level: str, url: str, api_key: str, api_secret: str) -> None:
-        logging.basicConfig(level=log_level)
+    def start(url: str, api_key: str, api_secret: str) -> None:
         worker._set_url(url)
         worker._api_key = api_key
         worker._api_secret = api_secret
-
-    @cli.command(help="Start the worker")
-    def start() -> None:
         _run_worker(worker)
 
     @cli.command(help="Start a worker and simulate a job, useful for testing")
     @click.option("--room-name", help="The room name", required=True)
     @click.option("--identity", help="The participant identity")
-    def simulate_job(room_name: str, identity: str) -> None:
+    @click.option(
+        "--url",
+        required=True,
+        envvar="LIVEKIT_URL",
+        help="LiveKit server or Cloud project WebSocket URL",
+        default="ws://localhost:7880",
+    )
+    @click.option(
+        "--api-key",
+        envvar="LIVEKIT_API_KEY",
+        help="LiveKit server or Cloud project's API key",
+        required=True,
+    )
+    @click.option(
+        "--api-secret",
+        envvar="LIVEKIT_API_SECRET",
+        help="LiveKit server or Cloud project's API secret",
+        required=True,
+    )
+    def simulate_job(
+        room_name: str, identity: str, url: str, api_key: str, api_secret: str
+    ) -> None:
+        worker._set_url(url)
+        worker._api_key = api_key
+        worker._api_secret = api_secret
+
         async def _pre_run() -> (
             Tuple[proto_models.Room, Optional[proto_models.ParticipantInfo]]
         ):
             lkapi = api.LiveKitAPI(worker._rtc_url, worker._api_key, worker._api_secret)
 
             try:
                 room = await lkapi.room.create_room(
```

### Comparing `livekit-agents-0.4.0/livekit_agents.egg-info/PKG-INFO` & `livekit-agents-0.4.1/livekit_agents.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: livekit-agents
-Version: 0.4.0
+Version: 0.4.1
 Summary: LiveKit Python Agents
 Home-page: https://github.com/livekit/agents
 License: Apache-2.0
 Project-URL: Documentation, https://docs.livekit.io
 Project-URL: Website, https://livekit.io/
 Project-URL: Source, https://github.com/livekit/agents
 Keywords: webrtc,realtime,audio,video,livekit,agents,AI
@@ -18,13 +18,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.9.0
 Description-Content-Type: text/markdown
 Requires-Dist: click~=8.1.0
 Requires-Dist: livekit>=0.9.0
 Requires-Dist: livekit-api>=0.4.1
-Requires-Dist: livekit-protocol>=0.3.0
+Requires-Dist: livekit-protocol~=0.3.0
 Requires-Dist: websockets<13,>=12
+Provides-Extra: codecs
+Requires-Dist: pyav>=12.0.2; extra == "codecs"
 
 # LiveKit Agents
 
 The core LiveKit Agents Framework. See top-level README for more information.
```

### Comparing `livekit-agents-0.4.0/livekit_agents.egg-info/SOURCES.txt` & `livekit-agents-0.4.1/livekit_agents.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 livekit/agents/job_context.py
 livekit/agents/job_request.py
 livekit/agents/plugin.py
 livekit/agents/utils.py
 livekit/agents/vad.py
 livekit/agents/version.py
 livekit/agents/worker.py
+livekit/agents/codecs/__init__.py
+livekit/agents/codecs/mp3.py
 livekit/agents/stt/__init__.py
 livekit/agents/stt/stream_adapter.py
 livekit/agents/stt/stt.py
 livekit/agents/tokenize/__init__.py
 livekit/agents/tokenize/sentence_tokenizer.py
 livekit/agents/tts/__init__.py
 livekit/agents/tts/stream_adapter.py
```

### Comparing `livekit-agents-0.4.0/setup.py` & `livekit-agents-0.4.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -48,17 +48,20 @@
     license="Apache-2.0",
     packages=setuptools.find_namespace_packages(include=["livekit.*"]),
     python_requires=">=3.9.0",
     install_requires=[
         "click~=8.1.0",
         "livekit>=0.9.0",
         "livekit-api>=0.4.1",
-        "livekit-protocol>=0.3.0",
+        "livekit-protocol~=0.3.0",
         "websockets>=12,<13",
     ],
+    extras_require={
+        "codecs": ["pyav>=12.0.2"],
+    },
     package_data={},
     project_urls={
         "Documentation": "https://docs.livekit.io",
         "Website": "https://livekit.io/",
         "Source": "https://github.com/livekit/agents",
     },
 )
```

