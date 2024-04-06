# Comparing `tmp/invertedai-0.0.8.post1.tar.gz` & `tmp/invertedai-0.0.9rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "invertedai-0.0.8.post1.tar", max compression
+gzip compressed data, was "invertedai-0.0.9rc0.tar", max compression
```

## Comparing `invertedai-0.0.8.post1.tar` & `invertedai-0.0.9rc0.tar`

### file list

```diff
@@ -1,17 +1,18 @@
--rw-r--r--   0        0        0     1068 2023-03-10 01:37:12.874715 invertedai-0.0.8.post1/LICENSE
--rw-r--r--   0        0        0     7549 2023-03-10 01:37:12.874715 invertedai-0.0.8.post1/README.md
--rw-r--r--   0        0        0     1437 2023-03-10 01:37:13.398720 invertedai-0.0.8.post1/invertedai/__init__.py
--rw-r--r--   0        0        0      276 2023-03-10 01:37:13.398720 invertedai-0.0.8.post1/invertedai/api/__init__.py
--rw-r--r--   0        0        0       78 2023-03-10 01:37:13.398720 invertedai-0.0.8.post1/invertedai/api/config.py
--rw-r--r--   0        0        0     8275 2023-03-10 01:37:13.398720 invertedai-0.0.8.post1/invertedai/api/drive.py
--rw-r--r--   0        0        0    10364 2023-03-10 01:37:13.398720 invertedai-0.0.8.post1/invertedai/api/initialize.py
--rw-r--r--   0        0        0     2759 2023-03-10 01:37:13.398720 invertedai-0.0.8.post1/invertedai/api/light.py
--rw-r--r--   0        0        0     3880 2023-03-10 01:37:13.398720 invertedai-0.0.8.post1/invertedai/api/location.py
--rw-r--r--   0        0        0    39828 2023-03-10 01:37:13.398720 invertedai-0.0.8.post1/invertedai/api/mock.py
--rw-r--r--   0        0        0     7361 2023-03-10 01:37:13.398720 invertedai-0.0.8.post1/invertedai/common.py
--rw-r--r--   0        0        0     9030 2023-03-10 01:37:13.398720 invertedai-0.0.8.post1/invertedai/cosimulation.py
--rw-r--r--   0        0        0     4154 2023-03-10 01:37:13.398720 invertedai-0.0.8.post1/invertedai/error.py
--rw-r--r--   0        0        0      959 2023-03-10 01:37:13.398720 invertedai-0.0.8.post1/invertedai/future.py
--rw-r--r--   0        0        0    39446 2023-03-10 01:37:13.398720 invertedai-0.0.8.post1/invertedai/utils.py
--rw-r--r--   0        0        0     1152 2023-03-10 01:37:13.406720 invertedai-0.0.8.post1/pyproject.toml
--rw-r--r--   0        0        0     8194 1970-01-01 00:00:00.000000 invertedai-0.0.8.post1/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-08-04 00:38:13.841995 invertedai-0.0.9rc0/LICENSE
+-rw-r--r--   0        0        0     7551 2023-08-04 00:38:13.841995 invertedai-0.0.9rc0/README.md
+-rw-r--r--   0        0        0     1637 2023-08-04 00:38:14.421999 invertedai-0.0.9rc0/invertedai/__init__.py
+-rw-r--r--   0        0        0      276 2023-08-04 00:38:14.421999 invertedai-0.0.9rc0/invertedai/api/__init__.py
+-rw-r--r--   0        0        0     6835 2023-08-04 00:38:14.421999 invertedai-0.0.9rc0/invertedai/api/blame.py
+-rw-r--r--   0        0        0       78 2023-08-04 00:38:14.421999 invertedai-0.0.9rc0/invertedai/api/config.py
+-rw-r--r--   0        0        0     8293 2023-08-04 00:38:14.421999 invertedai-0.0.9rc0/invertedai/api/drive.py
+-rw-r--r--   0        0        0    10382 2023-08-04 00:38:14.421999 invertedai-0.0.9rc0/invertedai/api/initialize.py
+-rw-r--r--   0        0        0     2777 2023-08-04 00:38:14.421999 invertedai-0.0.9rc0/invertedai/api/light.py
+-rw-r--r--   0        0        0     3898 2023-08-04 00:38:14.421999 invertedai-0.0.9rc0/invertedai/api/location.py
+-rw-r--r--   0        0        0    40028 2023-08-04 00:38:14.421999 invertedai-0.0.9rc0/invertedai/api/mock.py
+-rw-r--r--   0        0        0     7361 2023-08-04 00:38:14.421999 invertedai-0.0.9rc0/invertedai/common.py
+-rw-r--r--   0        0        0     9505 2023-08-04 00:38:14.425999 invertedai-0.0.9rc0/invertedai/cosimulation.py
+-rw-r--r--   0        0        0     4207 2023-08-04 00:38:14.425999 invertedai-0.0.9rc0/invertedai/error.py
+-rw-r--r--   0        0        0      959 2023-08-04 00:38:14.425999 invertedai-0.0.9rc0/invertedai/future.py
+-rw-r--r--   0        0        0    39667 2023-08-04 00:38:14.425999 invertedai-0.0.9rc0/invertedai/utils.py
+-rw-r--r--   0        0        0     1149 2023-08-04 00:38:14.429999 invertedai-0.0.9rc0/pyproject.toml
+-rw-r--r--   0        0        0     8193 1970-01-01 00:00:00.000000 invertedai-0.0.9rc0/PKG-INFO
```

### Comparing `invertedai-0.0.8.post1/LICENSE` & `invertedai-0.0.9rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `invertedai-0.0.8.post1/README.md` & `invertedai-0.0.9rc0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [pypi-badge]: https://badge.fury.io/py/invertedai.svg
 [pypi-link]: https://pypi.org/project/invertedai/
 [colab-badge]: https://colab.research.google.com/assets/colab-badge.svg
 [colab-link]: https://colab.research.google.com/github/inverted-ai/invertedai/blob/develop/examples/IAI_demo.ipynb
-[rest-link]: https://app.swaggerhub.com/apis/swaggerhub59/Inverted-AI
+[rest-link]: https://app.swaggerhub.com/apis-docs/InvertedAI/InvertedAI
 [examples-link]: https://github.com/inverted-ai/invertedai/tree/master/examples
 
 [![Documentation Status](https://readthedocs.org/projects/inverted-ai/badge/?version=latest)](https://inverted-ai.readthedocs.io/en/latest/?badge=latest)
 [![PyPI][pypi-badge]][pypi-link]
 [![Open In Colab][colab-badge]][colab-link]
 
 # InvertedAI
```

### Comparing `invertedai-0.0.8.post1/invertedai/__init__.py` & `invertedai-0.0.9rc0/invertedai/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 import os
+import importlib.metadata
 from distutils.util import strtobool
 
 from invertedai.api.light import light
 from invertedai.api.location import location_info
 from invertedai.api.initialize import initialize, async_initialize
 from invertedai.api.drive import drive, async_drive
+from invertedai.api.blame import blame, async_blame
 from invertedai.cosimulation import BasicCosimulation
 from invertedai.utils import Jupyter_Render, IAILogger, Session
 
 dev = strtobool(os.environ.get("IAI_DEV", "false"))
 if dev:
     dev_url = os.environ.get("IAI_DEV_URL", "http://localhost:8000")
+
 log_level = os.environ.get("IAI_LOG_LEVEL", "WARNING")
 log_console = strtobool(os.environ.get("IAI_LOG_CONSOLE", "true"))
 log_file = strtobool(os.environ.get("IAI_LOG_FILE", "false"))
 api_key = os.environ.get("IAI_API_KEY", "")
 
 logger = IAILogger(level=log_level, consoel=bool(log_console), log_file=bool(log_file))
 
@@ -23,26 +26,31 @@
 use_mock_api = session.use_mock_api
 
 if strtobool(os.environ.get("IAI_MOCK_API", "false")):
     use_mock_api()
 
 model_resources = {
     "initialize": ("post", "/initialize"),
+    "blame": ("post", "/blame"),
     "drive": ("post", "/drive"),
     "location_info": ("get", "/location_info"),
     "light": ("get", "/light"),
     "test": ("get", "/test"),
 }
 __all__ = [
     "BasicCosimulation",
     "Jupyter_Render",
     "logger",
     "session",
     "add_apikey",
     "use_mock_api",
+    "blame",
     "drive",
     "initialize",
     "location_info",
     "light",
     "async_initialize",
     "async_drive",
+    "async_blame",
 ]
+
+__version__ = importlib.metadata.version("invertedai")
```

### Comparing `invertedai-0.0.8.post1/invertedai/api/drive.py` & `invertedai-0.0.9rc0/invertedai/api/drive.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,14 +100,15 @@
         Controls the stochastic aspects of agent behavior for reproducibility.
 
     See Also
     --------
     :func:`initialize`
     :func:`location_info`
     :func:`light`
+    :func:`blame`
     """
     if len(agent_states) != len(agent_attributes):
         raise InvalidInput("Incompatible Number of Agents in either 'agent_states' or 'agent_attributes'.")
     if len(agent_states) != len(recurrent_states):
         raise InvalidInput("Incompatible Number of Agents in either 'agent_states' or 'recurrent_states'.")
 
     if should_use_mock_api():
```

### Comparing `invertedai-0.0.8.post1/invertedai/api/initialize.py` & `invertedai-0.0.9rc0/invertedai/api/initialize.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,14 +105,15 @@
         Controls the stochastic aspects of initialization for reproducibility.
 
     See Also
     --------
     :func:`drive`
     :func:`location_info`
     :func:`light`
+    :func:`blame`
     """
 
     if (states_history is not None) or (agent_attributes is not None):
         if (agent_attributes is None) or (states_history is None):
             raise InvalidInput("'agent_attributes' or 'states_history' are not provided.")
         for agent_states in states_history:
             if len(agent_states) != len(agent_attributes):
```

### Comparing `invertedai-0.0.8.post1/invertedai/api/light.py` & `invertedai-0.0.9rc0/invertedai/api/light.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,14 +45,15 @@
         Controls the stochastic aspects of agent behavior for reproducibility.
 
     See Also
     --------
     :func:`initialize`
     :func:`location_info`
     :func:`drive`
+    :func:`blame`
     """
     if should_use_mock_api():
         response = LightResponse(traffic_lights_states={123: TrafficLightState("green"),
                                                         124: TrafficLightState("red"),
                                                         126: TrafficLightState("yellow")},
                                  recurrent_states="ABC-DEF-GHI@12"
                                  )
```

### Comparing `invertedai-0.0.8.post1/invertedai/api/location.py` & `invertedai-0.0.9rc0/invertedai/api/location.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,14 +51,15 @@
     rendering_center:
         Optional center x,y coordinates for the rendered birdview.
     See Also
     --------
     :func:`drive`
     :func:`initialize`
     :func:`light`
+    :func:`blame`
     """
 
     if should_use_mock_api():
         response = LocationResponse(
             version="v0.0.0",
             birdview_image=get_mock_birdview(),
             osm_map=None,
```

### Comparing `invertedai-0.0.8.post1/invertedai/api/mock.py` & `invertedai-0.0.9rc0/invertedai/api/mock.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List
+from typing import List, Tuple
 
 from invertedai.common import (
     AgentAttributes,
     AgentState,
     RecurrentState,
     InfractionIndicators,
     Point,
@@ -24,14 +24,26 @@
     return state
 
 
 def get_mock_recurrent_state() -> RecurrentState:
     return RecurrentState()  # TODO
 
 
+def get_mock_agents_at_fault() -> Tuple[int, ...]:
+    return 0, 1
+
+
+def get_mock_blamed_reasons() -> str:
+    return {0: ["mock"]}
+
+
+def get_mock_confidence_score() -> float:
+    return 0.8
+
+
 def mock_update_agent_state(state: AgentState) -> AgentState:
     return state
 
 
 def get_mock_infractions(agent_count: int) -> List[InfractionIndicators]:
     infractions = [
         InfractionIndicators(collisions=False, offroad=False, wrong_way=False)
```

### Comparing `invertedai-0.0.8.post1/invertedai/common.py` & `invertedai-0.0.9rc0/invertedai/common.py`

 * *Files identical despite different names*

### Comparing `invertedai-0.0.8.post1/invertedai/cosimulation.py` & `invertedai-0.0.9rc0/invertedai/cosimulation.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,14 +113,21 @@
     def agent_states(self) -> List[AgentState]:
         """
         The predicted states for all agents, including ego.
         """
         return self._agent_states
 
     @property
+    def agent_attributes(self) -> List[AgentAttributes]:
+        """
+        The attributes (length, width, rear_axis_offset) for all agents, including ego.
+        """
+        return self._agent_attributes
+
+    @property
     def ego_agent_mask(self) -> List[bool]:
         """
         Lists which agents are ego, which means that you control them externally.
         It can be updated during the simulation, but see caveats in user guide
         regarding the quality of resulting predictions.
         """
         return self._ego_agent_mask
@@ -134,14 +141,22 @@
         """
         Returns the predicted states of ego agents in order.
         The NPC agents are excluded.
         """
         return [d for d, s in zip(self._agent_states, self._ego_agent_mask) if s]
 
     @property
+    def ego_attributes(self):
+        """
+        Returns the attributes of ego agents in order.
+        The NPC agents are excluded.
+        """
+        return [attr for attr, s in zip(self._agent_attributes, self._ego_agent_mask) if s]
+
+    @property
     def infractions(self) -> Optional[List[InfractionIndicators]]:
         """
         If `monitor_infractions` was set in the constructor,
         lists infractions currently committed by each agent, including ego agents.
         """
         return self._infractions
```

### Comparing `invertedai-0.0.8.post1/invertedai/error.py` & `invertedai-0.0.9rc0/invertedai/error.py`

 * *Files 2% similar despite different names*

```diff
@@ -158,14 +158,16 @@
 class ServiceUnavailableError(InvertedAIError):
     pass
 
 
 class InvalidAPIType(InvertedAIError):
     pass
 
+class LargeRequestTimeout(InvertedAIError):
+    pass
 
 class SignatureVerificationError(InvertedAIError):
     def __init__(self, message, sig_header, http_body=None):
         super(SignatureVerificationError, self).__init__(message, http_body)
         self.sig_header = sig_header
 
     def __reduce__(self):
```

### Comparing `invertedai-0.0.8.post1/invertedai/future.py` & `invertedai-0.0.9rc0/invertedai/future.py`

 * *Files identical despite different names*

### Comparing `invertedai-0.0.8.post1/invertedai/utils.py` & `invertedai-0.0.9rc0/invertedai/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -128,14 +128,16 @@
                 raise error.AuthenticationError(
                     "Access denied. Please check the provided API key."
                 )
             elif e.response.status_code in [400, 422]:
                 raise error.InvalidRequestError(e.response.text, param="")
             elif e.response.status_code == 404:
                 raise error.ResourceNotFoundError(e.response.text)
+            elif e.response.status_code == 413:
+                raise error.LargeRequestTimeout(e.response.text)
             elif e.response.status_code == 429:
                 raise error.RateLimitError("Throttled")
             elif e.response.status_code == 503:
                 raise error.ServiceUnavailableError("Service Unavailable")
             elif 400 <= e.response.status_code < 500:
                 raise error.APIError("Invalid request. Please check the sent data again.")
             else:
@@ -796,15 +798,16 @@
         if self.velocity_vec:
             if agent_idx not in self.v_lines:
                 self.v_lines[agent_idx] = self.current_ax.plot(
                     box[2:4, 0], box[2:4, 1], lw=1.5, c=self.v_c)[0]  # plot the speed
             else:
                 self.v_lines[agent_idx].set_xdata(box[2:4, 0])
                 self.v_lines[agent_idx].set_ydata(box[2:4, 1])
-        if self.numbers:
+        if (type(self.numbers) == bool and self.numbers) or \
+           (type(self.numbers) == list and agent_idx in self.numbers):
             if agent_idx not in self.box_labels:
                 self.box_labels[agent_idx] = self.current_ax.text(
                     x, y, str(agent_idx), c='r', fontsize=18)
                 self.box_labels[agent_idx].set_clip_on(True)
             else:
                 self.box_labels[agent_idx].set_x(x)
                 self.box_labels[agent_idx].set_y(y)
```

### Comparing `invertedai-0.0.8.post1/pyproject.toml` & `invertedai-0.0.9rc0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "invertedai"
-version = "0.0.8.post1"
+version = "0.0.9rc0"
 description = "Client SDK for InvertedAI"
 authors = ["Inverted AI <info@inverted.ai>"]
 readme = "README.md"
 license = "MIT"
 packages = [
     { include = "invertedai" },
 ]
```

### Comparing `invertedai-0.0.8.post1/PKG-INFO` & `invertedai-0.0.9rc0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invertedai
-Version: 0.0.8.post1
+Version: 0.0.9rc0
 Summary: Client SDK for InvertedAI
 License: MIT
 Author: Inverted AI
 Author-email: info@inverted.ai
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -17,15 +17,15 @@
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Description-Content-Type: text/markdown
 
 [pypi-badge]: https://badge.fury.io/py/invertedai.svg
 [pypi-link]: https://pypi.org/project/invertedai/
 [colab-badge]: https://colab.research.google.com/assets/colab-badge.svg
 [colab-link]: https://colab.research.google.com/github/inverted-ai/invertedai/blob/develop/examples/IAI_demo.ipynb
-[rest-link]: https://app.swaggerhub.com/apis/swaggerhub59/Inverted-AI
+[rest-link]: https://app.swaggerhub.com/apis-docs/InvertedAI/InvertedAI
 [examples-link]: https://github.com/inverted-ai/invertedai/tree/master/examples
 
 [![Documentation Status](https://readthedocs.org/projects/inverted-ai/badge/?version=latest)](https://inverted-ai.readthedocs.io/en/latest/?badge=latest)
 [![PyPI][pypi-badge]][pypi-link]
 [![Open In Colab][colab-badge]][colab-link]
 
 # InvertedAI
```

