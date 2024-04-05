# Comparing `tmp/agentops-0.1.0b7.tar.gz` & `tmp/agentops-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agentops-0.1.0b7.tar", last modified: Tue Apr  2 03:20:06 2024, max compression
+gzip compressed data, was "agentops-0.1.1.tar", last modified: Fri Apr  5 22:40:57 2024, max compression
```

## Comparing `agentops-0.1.0b7.tar` & `agentops-0.1.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 03:20:06.588480 agentops-0.1.0b7/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-02 03:20:02.000000 agentops-0.1.0b7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6219 2024-04-02 03:20:06.588480 agentops-0.1.0b7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5316 2024-04-02 03:20:02.000000 agentops-0.1.0b7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 03:20:06.584480 agentops-0.1.0b7/agentops/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1394 2024-04-02 03:20:02.000000 agentops-0.1.0b7/agentops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-04-02 03:20:02.000000 agentops-0.1.0b7/agentops/agent.py
--rw-r--r--   0 runner    (1001) docker     (127)    12195 2024-04-02 03:20:02.000000 agentops-0.1.0b7/agentops/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     4277 2024-04-02 03:20:02.000000 agentops-0.1.0b7/agentops/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-04-02 03:20:02.000000 agentops-0.1.0b7/agentops/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-02 03:20:02.000000 agentops-0.1.0b7/agentops/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     5782 2024-04-02 03:20:02.000000 agentops-0.1.0b7/agentops/event.py
--rw-r--r--   0 runner    (1001) docker     (127)     4424 2024-04-02 03:20:02.000000 agentops-0.1.0b7/agentops/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-04-02 03:20:02.000000 agentops-0.1.0b7/agentops/host_env.py
--rw-r--r--   0 runner    (1001) docker     (127)     3419 2024-04-02 03:20:02.000000 agentops-0.1.0b7/agentops/http_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    22328 2024-04-02 03:20:02.000000 agentops-0.1.0b7/agentops/langchain_callback_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)    12087 2024-04-02 03:20:02.000000 agentops-0.1.0b7/agentops/llm_tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-04-02 03:20:02.000000 agentops-0.1.0b7/agentops/meta_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-04-02 03:20:02.000000 agentops-0.1.0b7/agentops/session.py
--rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-04-02 03:20:02.000000 agentops-0.1.0b7/agentops/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 03:20:06.584480 agentops-0.1.0b7/agentops.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6219 2024-04-02 03:20:06.000000 agentops-0.1.0b7/agentops.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-02 03:20:06.000000 agentops-0.1.0b7/agentops.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 03:20:06.000000 agentops-0.1.0b7/agentops.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-02 03:20:06.000000 agentops-0.1.0b7/agentops.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-02 03:20:06.000000 agentops-0.1.0b7/agentops.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      979 2024-04-02 03:20:02.000000 agentops-0.1.0b7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 03:20:06.588480 agentops-0.1.0b7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 03:20:06.584480 agentops-0.1.0b7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-04-02 03:20:02.000000 agentops-0.1.0b7/tests/test_canary.py
--rw-r--r--   0 runner    (1001) docker     (127)     2171 2024-04-02 03:20:02.000000 agentops-0.1.0b7/tests/test_patcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     3094 2024-04-02 03:20:02.000000 agentops-0.1.0b7/tests/test_record_function.py
--rw-r--r--   0 runner    (1001) docker     (127)     2762 2024-04-02 03:20:02.000000 agentops-0.1.0b7/tests/test_session.py
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-02 03:20:02.000000 agentops-0.1.0b7/tests/test_teardown.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 22:40:57.348312 agentops-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-05 22:40:52.000000 agentops-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6217 2024-04-05 22:40:57.348312 agentops-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5316 2024-04-05 22:40:52.000000 agentops-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 22:40:57.348312 agentops-0.1.1/agentops/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2866 2024-04-05 22:40:52.000000 agentops-0.1.1/agentops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-04-05 22:40:52.000000 agentops-0.1.1/agentops/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12541 2024-04-05 22:40:52.000000 agentops-0.1.1/agentops/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4277 2024-04-05 22:40:52.000000 agentops-0.1.1/agentops/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-04-05 22:40:52.000000 agentops-0.1.1/agentops/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-05 22:40:52.000000 agentops-0.1.1/agentops/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5607 2024-04-05 22:40:52.000000 agentops-0.1.1/agentops/event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4424 2024-04-05 22:40:52.000000 agentops-0.1.1/agentops/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-04-05 22:40:52.000000 agentops-0.1.1/agentops/host_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3419 2024-04-05 22:40:52.000000 agentops-0.1.1/agentops/http_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22227 2024-04-05 22:40:52.000000 agentops-0.1.1/agentops/langchain_callback_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12087 2024-04-05 22:40:52.000000 agentops-0.1.1/agentops/llm_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-04-05 22:40:52.000000 agentops-0.1.1/agentops/meta_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-04-05 22:40:52.000000 agentops-0.1.1/agentops/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3702 2024-04-05 22:40:52.000000 agentops-0.1.1/agentops/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 22:40:57.348312 agentops-0.1.1/agentops.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6217 2024-04-05 22:40:57.000000 agentops-0.1.1/agentops.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-05 22:40:57.000000 agentops-0.1.1/agentops.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 22:40:57.000000 agentops-0.1.1/agentops.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-05 22:40:57.000000 agentops-0.1.1/agentops.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-05 22:40:57.000000 agentops-0.1.1/agentops.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-04-05 22:40:52.000000 agentops-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 22:40:57.348312 agentops-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 22:40:57.348312 agentops-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-04-05 22:40:52.000000 agentops-0.1.1/tests/test_canary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2171 2024-04-05 22:40:52.000000 agentops-0.1.1/tests/test_patcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3094 2024-04-05 22:40:52.000000 agentops-0.1.1/tests/test_record_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2784 2024-04-05 22:40:52.000000 agentops-0.1.1/tests/test_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-05 22:40:52.000000 agentops-0.1.1/tests/test_teardown.py
```

### Comparing `agentops-0.1.0b7/LICENSE` & `agentops-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `agentops-0.1.0b7/PKG-INFO` & `agentops-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agentops
-Version: 0.1.0b7
+Version: 0.1.1
 Summary: Python SDK for developing AI agent evals and observability
 Author-email: Alex Reibman <areibman@gmail.com>, Shawn Qiu <siyangqiu@gmail.com>, Braelyn Boynton <bboynton97@gmail.com>, Howard Gil <howardbgil@gmail.com>
 Project-URL: Homepage, https://github.com/AgentOps-AI/agentops
 Project-URL: Issues, https://github.com/AgentOps-AI/agentops/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: agentops Version: 0.1.0b7 Summary: Python SDK for
+Metadata-Version: 2.1 Name: agentops Version: 0.1.1 Summary: Python SDK for
 developing AI agent evals and observability Author-email: Alex Reibman
 gmail.com>, Shawn Qiu
 gmail.com>, Braelyn Boynton
 gmail.com>, Howard Gil
 gmail.com> Project-URL: Homepage, https://github.com/AgentOps-AI/agentops
 Project-URL: Issues, https://github.com/AgentOps-AI/agentops/issues Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
```

### Comparing `agentops-0.1.0b7/README.md` & `agentops-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `agentops-0.1.0b7/agentops/agent.py` & `agentops-0.1.1/agentops/agent.py`

 * *Files identical despite different names*

### Comparing `agentops-0.1.0b7/agentops/client.py` & `agentops-0.1.1/agentops/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -106,17 +106,14 @@
         Record an event with the AgentOps service.
 
         Args:
             event (Event): The event to record.
         """
 
         if self._session is not None and not self._session.has_ended:
-            agent_id = check_call_stack_for_agent_id()
-            if agent_id:
-                event.agent_id = agent_id
             self._worker.add_event(event.__dict__)
         else:
             logging.warning(
                 "AgentOps: Cannot record event - no current session")
 
     def _record_event_sync(self, func, event_name, *args, **kwargs):
         init_time = get_ISO_time()
@@ -211,16 +208,20 @@
             return logging.warning("AgentOps: Cannot start session - session already started")
 
         if not config and not self.config:
             return logging.warning("AgentOps: Cannot start session - missing configuration")
 
         self._session = Session(uuid4(), tags or self._tags, host_env=get_host_env())
         self._worker = Worker(config or self.config)
-        self._worker.start_session(self._session)
-        logging.info('View info on this session at https://app.agentops.ai/dashboard?session_id={}'
+        start_session_result = self._worker.start_session(self._session)
+        if not start_session_result:
+            self._session = None
+            return logging.warning("AgentOps: Cannot start session")
+
+        logging.info('View info on this session at https://app.agentops.ai/drilldown?session_id={}'
                      .format(self._session.session_id))
 
     def end_session(self,
                     end_state: str,
                     end_state_reason: Optional[str] = None,
                     video: Optional[str] = None):
         """
@@ -240,15 +241,16 @@
         self._session.video = video
         self._session.end_session(end_state, end_state_reason)
         self._worker.end_session(self._session)
         self._session = None
         self._worker = None
 
     def create_agent(self, agent_id: str, name: str):
-        self._worker.create_agent(agent_id, name)
+        if self._worker:
+            self._worker.create_agent(agent_id, name)
 
     def _handle_unclean_exits(self):
         def cleanup(end_state: Optional[str] = 'Fail', end_state_reason: Optional[str] = None):
             # Only run cleanup function if session is created
             if self._session is not None:
                 self.end_session(end_state=end_state,
                                  end_state_reason=end_state_reason)
@@ -292,7 +294,19 @@
         signal.signal(signal.SIGINT, signal_handler)
         signal.signal(signal.SIGTERM, signal_handler)
         sys.excepthook = handle_exception
 
     @property
     def current_session_id(self):
         return self._session.session_id
+
+    @property
+    def api_key(self):
+        return self.config.api_key
+
+    def set_parent_key(self, parent_key):
+        if self._worker:
+            self._worker.config.parent_key = parent_key
+
+    @property
+    def parent_key(self):
+        return self.config.parent_key
```

### Comparing `agentops-0.1.0b7/agentops/config.py` & `agentops-0.1.1/agentops/config.py`

 * *Files identical despite different names*

### Comparing `agentops-0.1.0b7/agentops/decorators.py` & `agentops-0.1.1/agentops/decorators.py`

 * *Files identical despite different names*

### Comparing `agentops-0.1.0b7/agentops/enums.py` & `agentops-0.1.1/agentops/enums.py`

 * *Files identical despite different names*

### Comparing `agentops-0.1.0b7/agentops/event.py` & `agentops-0.1.1/agentops/event.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 Data Class:
     Event: Represents discrete events to be recorded.
 """
 
 from dataclasses import dataclass, field
 from typing import List, Optional
-from .helpers import get_ISO_time
+from .helpers import get_ISO_time, check_call_stack_for_agent_id
 from .enums import EventType, Models
 from uuid import UUID, uuid4
 
 
 @dataclass
 class Event:
 
@@ -19,14 +19,15 @@
     Abstract base class for events that will be recorded. Should not be instantiated directly.
 
     event_type(str): The type of event. Defined in enums.EventType. Some values are 'llm', 'action', 'api', 'tool', 'error'.
     params(dict, optional): The parameters of the function containing the triggered event, e.g. {'x': 1} in example below
     returns(str, optional): The return value of the function containing the triggered event, e.g. 2 in example below
     init_timestamp(str): A timestamp indicating when the event began. Defaults to the time when this Event was instantiated.
     end_timestamp(str): A timestamp indicating when the event ended. Defaults to the time when this Event was instantiated.
+    agent_id(UUID, optional): The unique identifier of the agent that triggered the event.
     id(UUID): A unique identifier for the event. Defaults to a new UUID.
 
     foo(x=1) {
         ...
         // params equals {'x': 1}
         record(ActionEvent(params=**kwargs, ...))
         ...
@@ -36,32 +37,31 @@
     """
 
     event_type: str  # EventType.ENUM.value
     params: Optional[dict] = None
     returns: Optional[str] = None
     init_timestamp: Optional[str] = field(default_factory=get_ISO_time)
     end_timestamp: str = field(default_factory=get_ISO_time)
+    agent_id: Optional[UUID] = field(default_factory=check_call_stack_for_agent_id)
     id: UUID = field(default_factory=uuid4)
     # TODO: has_been_recorded: bool = False
 
 
 @dataclass
 class ActionEvent(Event):
     """
     For generic events
 
-    agent_id(UUID, optional): The unique identifier of the agent that triggered the event.
     action_type(str, optional): High level name describing the action
     logs(str, optional): For detailed information/logging related to the action
     screenshot(str, optional): url to snapshot if agent interacts with UI
     """
 
     event_type: str = EventType.ACTION.value
     # TODO: Should not be optional, but non-default argument 'agent_id' follows default argument error
-    agent_id: Optional[UUID] = None
     action_type: Optional[str] = None
     logs: Optional[str] = None
     screenshot: Optional[str] = None
 
     # May be needed if we keep Optional for agent_id
     # def __post_init__(self):
     #     if self.agent_id is None:
@@ -70,46 +70,42 @@
 
 @dataclass
 class LLMEvent(Event):
 
     """
     For recording calls to LLMs. AgentOps auto-instruments calls to the most popular LLMs e.g. GPT, Claude, Gemini, etc.
 
-    agent_id(UUID, optional): The unique identifier of the agent that triggered the event.
     thread_id(UUID, optional): The unique identifier of the contextual thread that a message pertains to.
     prompt(str, list, optional): The message or messages that were used to prompt the LLM. Preferably in ChatML format which is more fully supported by AgentOps.
     prompt_tokens(int, optional): The number of tokens in the prompt message.
     completion(str, object, optional): The message or returned by the LLM. Preferably in ChatML format which is more fully supported by AgentOps.
     completion_tokens(int, optional): The number of tokens in the completion message.
     model(Models, str, optional): LLM model e.g. "gpt-4". Models defined in enums.Models are more fully supported by AgentOps e.g. extra features in dashboard.
 
     """
 
     event_type: str = EventType.LLM.value
-    agent_id: Optional[UUID] = None
     thread_id: Optional[UUID] = None
     prompt: str | List = None
     prompt_tokens: Optional[int] = None
     completion: str | object = None
     completion_tokens: Optional[int] = None
     model: Optional[Models | str] = None
 
 
 @dataclass
 class ToolEvent(Event):
     """
     For recording calls to tools e.g. searchWeb, fetchFromDB
 
-    agent_id(UUID, optional): The unique identifier of the agent that triggered the event.
     name(str, optional): A name describing the tool or the actual function name if applicable e.g. searchWeb, fetchFromDB.
     logs(str, dict, optional): For detailed information/logging related to the tool.
 
     """
     event_type: str = EventType.TOOL.value
-    agent_id: Optional[UUID] = None
     name: Optional[str] = None
     logs: Optional[str | dict] = None
 
 # Does not inherit from Event because error will (optionally) be linked to an ActionEvent, LLMEvent, etc that will have the details
 
 
 @dataclass
```

### Comparing `agentops-0.1.0b7/agentops/helpers.py` & `agentops-0.1.1/agentops/helpers.py`

 * *Files identical despite different names*

### Comparing `agentops-0.1.0b7/agentops/host_env.py` & `agentops-0.1.1/agentops/host_env.py`

 * *Files identical despite different names*

### Comparing `agentops-0.1.0b7/agentops/http_client.py` & `agentops-0.1.1/agentops/http_client.py`

 * *Files identical despite different names*

### Comparing `agentops-0.1.0b7/agentops/langchain_callback_handler.py` & `agentops-0.1.1/agentops/langchain_callback_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -429,15 +429,14 @@
             llm_event.completion_tokens = response.llm_output['token_usage']['completion_tokens']
         self.ao_client.record(llm_event)
 
         if len(response.generations) == 0:
             # TODO: more descriptive error
             error_event = ErrorEvent(trigger_event=self.events.llm[str(run_id)],
                                      details="on_llm_end: No generations", timestamp=get_ISO_time())
-                                     details="on_llm_end: No generations", timestamp=get_ISO_time())
             self.ao_client.record(error_event)
 
     @debug_print_function_params
     async def on_chain_start(
         self,
         serialized: Dict[str, Any],
         inputs: Dict[str, Any],
```

### Comparing `agentops-0.1.0b7/agentops/llm_tracker.py` & `agentops-0.1.1/agentops/llm_tracker.py`

 * *Files identical despite different names*

### Comparing `agentops-0.1.0b7/agentops/meta_client.py` & `agentops-0.1.1/agentops/meta_client.py`

 * *Files identical despite different names*

### Comparing `agentops-0.1.0b7/agentops/session.py` & `agentops-0.1.1/agentops/session.py`

 * *Files identical despite different names*

### Comparing `agentops-0.1.0b7/agentops/worker.py` & `agentops-0.1.1/agentops/worker.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,18 +45,23 @@
     def start_session(self, session: Session) -> None:
         self._session = session
         with self.lock:
             payload = {
                 "session": session.__dict__
             }
             serialized_payload = json.dumps(filter_unjsonable(payload)).encode("utf-8")
-            HttpClient.post(f'{self.config.endpoint}/sessions',
-                            serialized_payload,
-                            self.config.api_key,
-                            self.config.parent_key)
+            res = HttpClient.post(f'{self.config.endpoint}/sessions',
+                                  serialized_payload,
+                                  self.config.api_key,
+                                  self.config.parent_key)
+
+            if res.code != 200:
+                return False
+
+            return True
 
     def end_session(self, session: Session) -> None:
         self.stop_flag.set()
         self.thread.join(timeout=1)
         self.flush_queue()
         self._session = None
```

### Comparing `agentops-0.1.0b7/agentops.egg-info/PKG-INFO` & `agentops-0.1.1/agentops.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agentops
-Version: 0.1.0b7
+Version: 0.1.1
 Summary: Python SDK for developing AI agent evals and observability
 Author-email: Alex Reibman <areibman@gmail.com>, Shawn Qiu <siyangqiu@gmail.com>, Braelyn Boynton <bboynton97@gmail.com>, Howard Gil <howardbgil@gmail.com>
 Project-URL: Homepage, https://github.com/AgentOps-AI/agentops
 Project-URL: Issues, https://github.com/AgentOps-AI/agentops/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: agentops Version: 0.1.0b7 Summary: Python SDK for
+Metadata-Version: 2.1 Name: agentops Version: 0.1.1 Summary: Python SDK for
 developing AI agent evals and observability Author-email: Alex Reibman
 gmail.com>, Shawn Qiu
 gmail.com>, Braelyn Boynton
 gmail.com>, Howard Gil
 gmail.com> Project-URL: Homepage, https://github.com/AgentOps-AI/agentops
 Project-URL: Issues, https://github.com/AgentOps-AI/agentops/issues Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
```

### Comparing `agentops-0.1.0b7/agentops.egg-info/SOURCES.txt` & `agentops-0.1.1/agentops.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `agentops-0.1.0b7/pyproject.toml` & `agentops-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "agentops"
-version = "0.1.0-beta.7"
+version = "0.1.1"
 authors = [
   { name="Alex Reibman", email="areibman@gmail.com" },
   { name="Shawn Qiu", email="siyangqiu@gmail.com" },
   { name="Braelyn Boynton", email="bboynton97@gmail.com" },
   { name="Howard Gil", email="howardbgil@gmail.com" }
 ]
 description = "Python SDK for developing AI agent evals and observability"
```

### Comparing `agentops-0.1.0b7/tests/test_canary.py` & `agentops-0.1.1/tests/test_canary.py`

 * *Files identical despite different names*

### Comparing `agentops-0.1.0b7/tests/test_patcher.py` & `agentops-0.1.1/tests/test_patcher.py`

 * *Files identical despite different names*

### Comparing `agentops-0.1.0b7/tests/test_record_function.py` & `agentops-0.1.1/tests/test_record_function.py`

 * *Files identical despite different names*

### Comparing `agentops-0.1.0b7/tests/test_session.py` & `agentops-0.1.1/tests/test_session.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,67 +14,64 @@
         yield m
 
 
 class TestSessions:
     def setup_method(self):
         self.api_key = "random_api_key"
         self.event_type = 'test_event_type'
-        agentops.init(api_key=self.api_key, max_wait_time=5, auto_start_session=False)
+        self.config = agentops.Configuration(api_key=self.api_key, max_wait_time=50)
 
     def test_session(self, mock_req):
-        # Arrange
-        agentops.start_session()
+        agentops.start_session(config=self.config)
 
-        # Act
+        agentops.record(ActionEvent(self.event_type))
         agentops.record(ActionEvent(self.event_type))
 
-        # Assert the session has been initiated and the id has been created on backend.
+        # We should have 1 requests (session start).
         assert len(mock_req.request_history) == 1
+        time.sleep(0.15)
 
-        # Act
-        agentops.record(ActionEvent(self.event_type))
-        time.sleep(0.1)
-
-        # Assert an event has been added
+        # We should have 2 requests (session and 2 events combined into 1)
+        print(mock_req.last_request.json())
         assert len(mock_req.request_history) == 2
         assert mock_req.last_request.headers['X-Agentops-Auth'] == self.api_key
         request_json = mock_req.last_request.json()
         assert request_json['events'][0]['event_type'] == self.event_type
 
-        # Act
         end_state = 'Success'
         agentops.end_session(end_state)
-        time.sleep(0.1)
+        time.sleep(0.15)
 
-        # Since a session has ended, no more events should be recorded, but end_session should be called
+        # We should have 3 requests (additional end session)
         assert len(mock_req.request_history) == 3
         assert mock_req.last_request.headers['X-Agentops-Auth'] == self.api_key
         request_json = mock_req.last_request.json()
         assert request_json['session']['end_state'] == end_state
         assert request_json['session']['tags'] == None
 
     def test_tags(self, mock_req):
         # Arrange
         tags = ['GPT-4']
-        agentops.start_session(tags=tags)
+        agentops.start_session(tags=tags, config=self.config)
 
         # Act
         agentops.record(ActionEvent(self.event_type))
-        time.sleep(0.1)
+        time.sleep(0.15)
 
         # Assert 2 requests - 1 for session init, 1 for event
+        print(mock_req.last_request.json())
         assert len(mock_req.request_history) == 2
         assert mock_req.last_request.headers['X-Agentops-Auth'] == self.api_key
         request_json = mock_req.last_request.json()
         assert request_json['events'][0]['event_type'] == self.event_type
 
         # Act
         end_state = 'Success'
         agentops.end_session(end_state)
-        time.sleep(0.1)
+        time.sleep(0.15)
 
         # Assert 3 requets, 1 for session init, 1 for event, 1 for end session
         assert len(mock_req.request_history) == 3
         assert mock_req.last_request.headers['X-Agentops-Auth'] == self.api_key
         request_json = mock_req.last_request.json()
         assert request_json['session']['end_state'] == end_state
         assert request_json['session']['tags'] == tags
```

### Comparing `agentops-0.1.0b7/tests/test_teardown.py` & `agentops-0.1.1/tests/test_teardown.py`

 * *Files identical despite different names*

