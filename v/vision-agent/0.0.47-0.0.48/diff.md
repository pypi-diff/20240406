# Comparing `tmp/vision_agent-0.0.47.tar.gz` & `tmp/vision_agent-0.0.48.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vision_agent-0.0.47.tar", max compression
+gzip compressed data, was "vision_agent-0.0.48.tar", max compression
```

## Comparing `vision_agent-0.0.47.tar` & `vision_agent-0.0.48.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0    11357 2024-04-02 23:58:49.103640 vision_agent-0.0.47/LICENSE
--rw-r--r--   0        0        0     4432 2024-04-02 23:58:49.103640 vision_agent-0.0.47/README.md
--rw-r--r--   0        0        0     2166 2024-04-02 23:58:49.643643 vision_agent-0.0.47/pyproject.toml
--rw-r--r--   0        0        0      229 2024-04-02 23:58:49.115640 vision_agent-0.0.47/vision_agent/__init__.py
--rw-r--r--   0        0        0      127 2024-04-02 23:58:49.115640 vision_agent-0.0.47/vision_agent/agent/__init__.py
--rw-r--r--   0        0        0      306 2024-04-02 23:58:49.115640 vision_agent-0.0.47/vision_agent/agent/agent.py
--rw-r--r--   0        0        0    11511 2024-04-02 23:58:49.115640 vision_agent-0.0.47/vision_agent/agent/easytool.py
--rw-r--r--   0        0        0     4493 2024-04-02 23:58:49.115640 vision_agent-0.0.47/vision_agent/agent/easytool_prompts.py
--rw-r--r--   0        0        0    10101 2024-04-02 23:58:49.115640 vision_agent-0.0.47/vision_agent/agent/reflexion.py
--rw-r--r--   0        0        0     9342 2024-04-02 23:58:49.115640 vision_agent-0.0.47/vision_agent/agent/reflexion_prompts.py
--rw-r--r--   0        0        0    17449 2024-04-02 23:58:49.119640 vision_agent-0.0.47/vision_agent/agent/vision_agent.py
--rw-r--r--   0        0        0     6151 2024-04-02 23:58:49.119640 vision_agent-0.0.47/vision_agent/agent/vision_agent_prompts.py
--rw-r--r--   0        0        0       46 2024-04-02 23:58:49.119640 vision_agent-0.0.47/vision_agent/data/__init__.py
--rw-r--r--   0        0        0     5122 2024-04-02 23:58:49.119640 vision_agent-0.0.47/vision_agent/data/data.py
--rw-r--r--   0        0        0       75 2024-04-02 23:58:49.119640 vision_agent-0.0.47/vision_agent/emb/__init__.py
--rw-r--r--   0        0        0     1375 2024-04-02 23:58:49.119640 vision_agent-0.0.47/vision_agent/emb/emb.py
--rw-r--r--   0        0        0     4420 2024-04-02 23:58:49.119640 vision_agent-0.0.47/vision_agent/image_utils.py
--rw-r--r--   0        0        0       32 2024-04-02 23:58:49.119640 vision_agent-0.0.47/vision_agent/llm/__init__.py
--rw-r--r--   0        0        0     3904 2024-04-02 23:58:49.119640 vision_agent-0.0.47/vision_agent/llm/llm.py
--rw-r--r--   0        0        0       51 2024-04-02 23:58:49.119640 vision_agent-0.0.47/vision_agent/lmm/__init__.py
--rw-r--r--   0        0        0     8438 2024-04-02 23:58:49.119640 vision_agent-0.0.47/vision_agent/lmm/lmm.py
--rw-r--r--   0        0        0      235 2024-04-02 23:58:49.119640 vision_agent-0.0.47/vision_agent/tools/__init__.py
--rw-r--r--   0        0        0     1416 2024-04-02 23:58:49.119640 vision_agent-0.0.47/vision_agent/tools/prompts.py
--rw-r--r--   0        0        0    23447 2024-04-02 23:58:49.119640 vision_agent-0.0.47/vision_agent/tools/tools.py
--rw-r--r--   0        0        0     7476 2024-04-02 23:58:49.119640 vision_agent-0.0.47/vision_agent/tools/video.py
--rw-r--r--   0        0        0     5581 1970-01-01 00:00:00.000000 vision_agent-0.0.47/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-05 23:30:06.618450 vision_agent-0.0.48/LICENSE
+-rw-r--r--   0        0        0     4432 2024-04-05 23:30:06.618450 vision_agent-0.0.48/README.md
+-rw-r--r--   0        0        0     2166 2024-04-05 23:30:07.162458 vision_agent-0.0.48/pyproject.toml
+-rw-r--r--   0        0        0      229 2024-04-05 23:30:06.630450 vision_agent-0.0.48/vision_agent/__init__.py
+-rw-r--r--   0        0        0      127 2024-04-05 23:30:06.630450 vision_agent-0.0.48/vision_agent/agent/__init__.py
+-rw-r--r--   0        0        0      306 2024-04-05 23:30:06.630450 vision_agent-0.0.48/vision_agent/agent/agent.py
+-rw-r--r--   0        0        0    11511 2024-04-05 23:30:06.630450 vision_agent-0.0.48/vision_agent/agent/easytool.py
+-rw-r--r--   0        0        0     4493 2024-04-05 23:30:06.630450 vision_agent-0.0.48/vision_agent/agent/easytool_prompts.py
+-rw-r--r--   0        0        0    10101 2024-04-05 23:30:06.630450 vision_agent-0.0.48/vision_agent/agent/reflexion.py
+-rw-r--r--   0        0        0     9342 2024-04-05 23:30:06.630450 vision_agent-0.0.48/vision_agent/agent/reflexion_prompts.py
+-rw-r--r--   0        0        0    17449 2024-04-05 23:30:06.630450 vision_agent-0.0.48/vision_agent/agent/vision_agent.py
+-rw-r--r--   0        0        0     6152 2024-04-05 23:30:06.630450 vision_agent-0.0.48/vision_agent/agent/vision_agent_prompts.py
+-rw-r--r--   0        0        0       46 2024-04-05 23:30:06.630450 vision_agent-0.0.48/vision_agent/data/__init__.py
+-rw-r--r--   0        0        0     5122 2024-04-05 23:30:06.630450 vision_agent-0.0.48/vision_agent/data/data.py
+-rw-r--r--   0        0        0       75 2024-04-05 23:30:06.630450 vision_agent-0.0.48/vision_agent/emb/__init__.py
+-rw-r--r--   0        0        0     1375 2024-04-05 23:30:06.630450 vision_agent-0.0.48/vision_agent/emb/emb.py
+-rw-r--r--   0        0        0     4420 2024-04-05 23:30:06.630450 vision_agent-0.0.48/vision_agent/image_utils.py
+-rw-r--r--   0        0        0       32 2024-04-05 23:30:06.630450 vision_agent-0.0.48/vision_agent/llm/__init__.py
+-rw-r--r--   0        0        0     3904 2024-04-05 23:30:06.630450 vision_agent-0.0.48/vision_agent/llm/llm.py
+-rw-r--r--   0        0        0       51 2024-04-05 23:30:06.630450 vision_agent-0.0.48/vision_agent/lmm/__init__.py
+-rw-r--r--   0        0        0     8438 2024-04-05 23:30:06.630450 vision_agent-0.0.48/vision_agent/lmm/lmm.py
+-rw-r--r--   0        0        0      235 2024-04-05 23:30:06.630450 vision_agent-0.0.48/vision_agent/tools/__init__.py
+-rw-r--r--   0        0        0     1416 2024-04-05 23:30:06.630450 vision_agent-0.0.48/vision_agent/tools/prompts.py
+-rw-r--r--   0        0        0    23884 2024-04-05 23:30:06.630450 vision_agent-0.0.48/vision_agent/tools/tools.py
+-rw-r--r--   0        0        0     7476 2024-04-05 23:30:06.630450 vision_agent-0.0.48/vision_agent/tools/video.py
+-rw-r--r--   0        0        0     5581 1970-01-01 00:00:00.000000 vision_agent-0.0.48/PKG-INFO
```

### Comparing `vision_agent-0.0.47/LICENSE` & `vision_agent-0.0.48/LICENSE`

 * *Files identical despite different names*

### Comparing `vision_agent-0.0.47/README.md` & `vision_agent-0.0.48/README.md`

 * *Files identical despite different names*

### Comparing `vision_agent-0.0.47/pyproject.toml` & `vision_agent-0.0.48/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "vision-agent"
-version = "0.0.47"
+version = "0.0.48"
 description = "Toolset for Vision Agent"
 authors = ["Landing AI <dev@landing.ai>"]
 readme = "README.md"
 packages = [{include = "vision_agent"}]
 
 [tool.poetry.urls]
 "Homepage" = "https://landing.ai"
```

### Comparing `vision_agent-0.0.47/vision_agent/agent/easytool.py` & `vision_agent-0.0.48/vision_agent/agent/easytool.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.0.47/vision_agent/agent/easytool_prompts.py` & `vision_agent-0.0.48/vision_agent/agent/easytool_prompts.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.0.47/vision_agent/agent/reflexion.py` & `vision_agent-0.0.48/vision_agent/agent/reflexion.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.0.47/vision_agent/agent/reflexion_prompts.py` & `vision_agent-0.0.48/vision_agent/agent/reflexion_prompts.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.0.47/vision_agent/agent/vision_agent.py` & `vision_agent-0.0.48/vision_agent/agent/vision_agent.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.0.47/vision_agent/agent/vision_agent_prompts.py` & `vision_agent-0.0.48/vision_agent/agent/vision_agent_prompts.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-VISION_AGENT_REFLECTION = """You are an advanced reasoning agent that can improve based on self refection. You will be given a previous reasoning trial in which you were given the user's question, the available tools that the agent has, the decomposed tasks and tools that the agent used to answer the question and the final answer the agent provided. You must determine if the agent's answer was correct or incorrect. If the agent's answer was correct, respond with Finish. If the agent's answer was incorrect, you must diagnose a possible reason for failure or phrasing discrepancy and devise a new, concise, high level plan that aims to mitigate the same failure with the tools avilable. Use complete sentences.
+VISION_AGENT_REFLECTION = """You are an advanced reasoning agent that can improve based on self refection. You will be given a previous reasoning trial in which you were given the user's question, the available tools that the agent has, the decomposed tasks and tools that the agent used to answer the question and the final answer the agent provided. You must determine if the agent's answer was correct or incorrect. If the agent's answer was correct, respond with Finish. If the agent's answer was incorrect, you must diagnose a possible reason for failure or phrasing discrepancy and devise a new, concise, high level plan that aims to mitigate the same failure with the tools available. Use complete sentences.
 
 User's question: {question}
 
 Tools available:
 {tools}
 
 Tasks and tools used:
```

### Comparing `vision_agent-0.0.47/vision_agent/data/data.py` & `vision_agent-0.0.48/vision_agent/data/data.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.0.47/vision_agent/emb/emb.py` & `vision_agent-0.0.48/vision_agent/emb/emb.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.0.47/vision_agent/image_utils.py` & `vision_agent-0.0.48/vision_agent/image_utils.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.0.47/vision_agent/llm/llm.py` & `vision_agent-0.0.48/vision_agent/llm/llm.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.0.47/vision_agent/lmm/lmm.py` & `vision_agent-0.0.48/vision_agent/lmm/lmm.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.0.47/vision_agent/tools/prompts.py` & `vision_agent-0.0.48/vision_agent/tools/prompts.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.0.47/vision_agent/tools/tools.py` & `vision_agent-0.0.48/vision_agent/tools/tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,14 +47,33 @@
 
 class Tool(ABC):
     name: str
     description: str
     usage: Dict
 
 
+class NoOp(Tool):
+    name = "noop_"
+    description = (
+        "'noop_' is a no-op tool that does nothing if you do not need to use a tool."
+    )
+    usage = {
+        "required_parameters": [],
+        "examples": [
+            {
+                "scenario": "If you do not want to use a tool.",
+                "parameters": {},
+            }
+        ],
+    }
+
+    def __call__(self) -> None:
+        return None
+
+
 class CLIP(Tool):
     r"""CLIP is a tool that can classify or tag any image given a set if input classes
     or tags.
 
     Example
     -------
         >>> import vision_agent as va
@@ -608,14 +627,15 @@
         return round(input[0] / input[1], 2)
 
 
 TOOLS = {
     i: {"name": c.name, "description": c.description, "usage": c.usage, "class": c}
     for i, c in enumerate(
         [
+            NoOp,
             CLIP,
             GroundingDINO,
             AgentGroundingSAM,
             ExtractFrames,
             Counter,
             Crop,
             BboxArea,
```

### Comparing `vision_agent-0.0.47/vision_agent/tools/video.py` & `vision_agent-0.0.48/vision_agent/tools/video.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.0.47/PKG-INFO` & `vision_agent-0.0.48/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vision-agent
-Version: 0.0.47
+Version: 0.0.48
 Summary: Toolset for Vision Agent
 Author: Landing AI
 Author-email: dev@landing.ai
 Requires-Python: >=3.9,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

