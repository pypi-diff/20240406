# Comparing `tmp/langmem-0.0.1rc9.tar.gz` & `tmp/langmem-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langmem-0.0.1rc9.tar", max compression
+gzip compressed data, was "langmem-0.0.2.tar", max compression
```

## Comparing `langmem-0.0.1rc9.tar` & `langmem-0.0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0       44 2024-03-05 21:23:47.510904 langmem-0.0.1rc9/README.md
--rw-r--r--   0        0        0       85 2024-03-05 21:23:47.511099 langmem-0.0.1rc9/langmem/__init__.py
--rw-r--r--   0        0        0        0 2024-03-05 21:23:47.511129 langmem-0.0.1rc9/langmem/_internal/__init__.py
--rw-r--r--   0        0        0      211 2024-03-05 21:23:47.511420 langmem-0.0.1rc9/langmem/_internal/utils.py
--rw-r--r--   0        0        0    61027 2024-03-29 18:45:15.354366 langmem-0.0.1rc9/langmem/client.py
--rw-r--r--   0        0        0        0 2024-03-29 00:44:04.650280 langmem-0.0.1rc9/langmem/integrations/__init__.py
--rw-r--r--   0        0        0     4231 2024-03-29 18:49:53.895861 langmem-0.0.1rc9/langmem/integrations/langchain.py
--rw-r--r--   0        0        0     8284 2024-03-29 20:05:04.806581 langmem-0.0.1rc9/langmem/integrations/langgraph.py
--rw-r--r--   0        0        0      288 2024-03-05 21:23:47.511914 langmem-0.0.1rc9/langmem/schemas.py
--rw-r--r--   0        0        0      632 2024-03-29 20:24:01.784160 langmem-0.0.1rc9/pyproject.toml
--rw-r--r--   0        0        0      731 1970-01-01 00:00:00.000000 langmem-0.0.1rc9/PKG-INFO
+-rw-r--r--   0        0        0     3611 2024-04-06 08:24:46.365379 langmem-0.0.2/README.md
+-rw-r--r--   0        0        0       85 2024-03-05 21:23:47.511099 langmem-0.0.2/langmem/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-05 21:23:47.511129 langmem-0.0.2/langmem/_internal/__init__.py
+-rw-r--r--   0        0        0      211 2024-03-05 21:23:47.511420 langmem-0.0.2/langmem/_internal/utils.py
+-rw-r--r--   0        0        0    63753 2024-04-06 08:14:25.210442 langmem-0.0.2/langmem/client.py
+-rw-r--r--   0        0        0        0 2024-03-29 20:48:10.213763 langmem-0.0.2/langmem/integrations/__init__.py
+-rw-r--r--   0        0        0     4231 2024-04-01 20:43:10.930486 langmem-0.0.2/langmem/integrations/langchain.py
+-rw-r--r--   0        0        0     8311 2024-04-01 20:43:10.930740 langmem-0.0.2/langmem/integrations/langgraph.py
+-rw-r--r--   0        0        0     2413 2024-04-06 08:14:25.210625 langmem-0.0.2/langmem/schemas.py
+-rw-r--r--   0        0        0      629 2024-04-06 08:14:25.210748 langmem-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     4295 1970-01-01 00:00:00.000000 langmem-0.0.2/PKG-INFO
```

### Comparing `langmem-0.0.1rc9/langmem/client.py` & `langmem-0.0.2/langmem/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     Sequence,
     Union,
 )
 
 import httpx
 from langmem._internal.utils import ID_T
 from langmem._internal.utils import as_uuid as _as_uuid
+from langmem import schemas
 from pydantic import BaseModel
 from pydantic.v1 import BaseModel as BaseModelV1
 
 DEFAULT_TIMEOUT = httpx.Timeout(timeout=30.0, connect=10.0)
 
 
 def _ensure_url(url: Optional[str]) -> str:
@@ -363,28 +364,35 @@
         self,
         user_id: ID_T,
         text: str,
         k: int = 200,
         memory_function_ids: Optional[Sequence[ID_T]] = None,
         weights: Optional[dict] = None,
         states_to_return: Optional[Sequence[ID_T]] = None,
+        thread_summaries: Optional[Sequence[ID_T]] = None,
+        thread_summaries_k: Optional[int] = None,
     ) -> List:
         """Query a user's memory.
 
         Args:
             user_id (ID_T): The user's ID.
             text (str): The query text.
             k (int, optional): The number of results to return. Defaults to 200.
             memory_function_ids (Optional[Sequence[ID_T]], optional): Semantic memory outputs
-                to include. Defaults to None, meaning just the unstructured memories.
+                    to include. Defaults to None, meaning just the unstructured memories.
             weights (Optional[dict], optional): Weights for the different memory types.
-                Backend default equally weights relevance, recency, and importance.
-                Defaults to None.
+                    Backend default equally weights relevance, recency, and importance.
+                    Defaults to None.
             states_to_return (Optional[Sequence[ID_T]], optional): The user state
-                memory function IDs to include in the response.
+                    memory function IDs to include in the response.
+            thread_summaries (Optional[Sequence[ID_T]], optional): The thread
+                    summary memory function IDs to include in the response, if any.
+            thread_summaries_k (Optional[int], optional): If you include thread summaries,
+                this controls the number of threads whose summaries you wish to return per
+                thread summary memory function. Defaults to None.
 
         Returns:
             List: The query results.
 
 
         Examples:
 
@@ -400,37 +408,61 @@
                 ...     user_id,
                 ...     text="pikas",
                 ...     k=10,
                 ...     weights={"relevance": 1.0, "recency": 0.0, "importance": 0.0},
                 ... )
 
             Include user state memories in the response (to save the number of API calls):
-                >>> mem_functions_ = client.list_memory_functions(target_type="user_state")
+                >>> mem_functions_ = client.list_memory_functions(target_type="user")
                 >>> mem_functions = []
                 >>> async for mem_function in mem_functions_:
-                ...     mem_functions.append(mem_function)
+                ...     if mem_function["type"] == "user_state":
+                ...         mem_functions.append(mem_function["id"])
                 >>> await client.query_user_memory(
                 ...     user_id,
                 ...     text="pikas",
                 ...     k=10,
                 ...     states_to_return=mem_functions,
                 ... )
 
             Query over user_append_state memories:
-                >>> mem_functions_ = client.list_memory_functions(target_type="user_append_state")
+                >>> mem_functions_ = client.list_memory_functions(target_type="user")
                 >>> mem_functions = []
                 >>> async for mem_function in mem_functions_:
-                ...     mem_functions.append(mem_function)
+                ...     if mem_function["type"] == "user_append_state":
+                ...         mem_functions.append(mem_function["id"])
                 >>> await client.query_user_memory(
                 ...     user_id,
                 ...     text="pikas",
                 ...     k=10,
                 ...     memory_function_ids=mem_functions,
                 ... )
+
+            Include thread summaries for the most recent threads:
+                >>> mem_functions_ = client.list_memory_functions(target_type="thread")
+                >>> mem_functions = []
+                >>> async for mem_function in mem_functions_:
+                ...     mem_functions.append(mem_function["id"])
+                >>> await client.query_user_memory(
+                ...     user_id,
+                ...     text="pikas",
+                ...     k=10,
+                ...     thread_summaries=mem_functions,
+                ...     thread_summaries_k=5,
+                ... )
+
         """
+        thread_query = None
+        if thread_summaries is not None:
+            thread_query: dict = {
+                "memory_function_ids": thread_summaries,
+            }
+            if thread_summaries_k is not None:
+                thread_query["k"] = thread_summaries_k
+
         response = await self.client.post(
             f"/users/{_as_uuid(user_id)}/memory/query",
             data=json.dumps(  # type: ignore[arg-type]
                 {
                     "text": text,
                     "k": k,
                     "memory_function_ids": memory_function_ids,
@@ -636,15 +668,15 @@
             "metadata": metadata,
         }
         response = await self.client.post("/threads", json=data)
         raise_for_status_with_text(response)
         return response.json()
 
     async def add_messages(
-        self, thread_id: ID_T, *, messages: Sequence[Dict[str, Any]]
+        self, thread_id: ID_T, *, messages: Sequence[schemas.MESSAGE_LIKE]
     ) -> None:
         """Add messages to a thread.
 
         This method allows you to add messages to a specific thread identified by its ID.
 
         Args:
             thread_id (ID_T): The ID of the thread to which the messages will be added.
@@ -1171,14 +1203,16 @@
         self,
         user_id: ID_T,
         text: str,
         k: int = 200,
         memory_function_ids: Optional[Sequence[ID_T]] = None,
         weights: Optional[dict] = None,
         states_to_return: Optional[Sequence[ID_T]] = None,
+        thread_summaries: Optional[Sequence[ID_T]] = None,
+        thread_summaries_k: Optional[int] = None,
     ) -> List:
         """Query a user's memory.
 
         Args:
             user_id (ID_T): The user's ID.
             text (str): The query text.
             k (int, optional): The number of results to return. Defaults to 200.
@@ -1208,42 +1242,69 @@
                 ...     user_id,
                 ...     text="pikas",
                 ...     k=10,
                 ...     weights={"relevance": 1.0, "recency": 0.0, "importance": 0.0},
                 ... )
 
             Include user state memories in the response (to save the number of API calls):
-                >>> mem_functions = list(client.list_memory_functions(target_type="user_state"))
+                >>> mem_functions = [
+                ...     f["id"]
+                ...     for f in client.list_memory_functions(target_type="user")
+                ...     if f["type"] == "user_state"
+                ... ]
                 >>> client.query_user_memory(
                 ...     user_id,
                 ...     text="pikas",
                 ...     k=10,
                 ...     states_to_return=mem_functions,
                 ... )
 
             Query over user_append_state memories:
-                >>> mem_functions = list(
-                ...     client.list_memory_functions(target_type="user_append_state")
+                >>> mem_functions = [
+                ...    f["id"]
+                ...    for f in client.list_memory_functions(target_type="user")
+                ...    if f["type"] == "user_append_state"
                 ... )
                 >>> client.query_user_memory(
                 ...     user_id,
                 ...     text="pikas",
                 ...     k=10,
                 ...     memory_function_ids=mem_functions,
                 ... )
+
+            Include thread summaries for the most recent threads:
+
+                >>> mem_functions = [
+                ...     f["id"] for f in client.list_memory_functions(target_type="thread")
+                ... ]
+                >>> client.query_user_memory(
+                ...     user_id,
+                ...     text="pikas",
+                ...     k=10,
+                ...     thread_summaries=mem_functions,
+                ...     thread_summaries_k=5,
+                ... )
         """
+        thread_query = None
+        if thread_summaries is not None:
+            thread_query = {
+                "memory_function_ids": thread_summaries,
+            }
+            if thread_summaries_k is not None:
+                thread_query["k"] = thread_summaries
         response = self.client.post(
             f"/users/{_as_uuid(user_id)}/memory/query",
             data=json.dumps(  # type: ignore[arg-type]
                 {
                     "text": text,
                     "k": k,
                     "memory_function_ids": memory_function_ids,
                     "weights": weights,
                     "state": states_to_return,
+                    "thread_query": thread_query,
                 },
                 default=_default_serializer,
             ),
         )
         raise_for_status_with_text(response)
         return response.json()
 
@@ -1390,15 +1451,15 @@
 
 
         Examples:
 
             Update a memory function's name:
                 >>> from langmem import Client
                 >>> client = Client()
-                >>> memory_function_id = client.list_memory_functions()[0]["id"]
+                >>> memory_function_id = list(client.list_memory_functions())[0]["id"]
                 >>> client.update_memory_function(memory_function_id, name="New Name")
 
             Disable a memory function:
                 >>> client.update_memory_function(memory_function_id, status="disabled")
 
             Update a memory function's schema:
                 >>> from pydantic import BaseModel, Field
@@ -1454,15 +1515,15 @@
         raise_for_status_with_text(response)
         return response.json()
 
     def create_thread(
         self,
         *,
         thread_id: Optional[ID_T] = None,
-        messages: Optional[Sequence[Dict[str, Any]]] = None,
+        messages: Optional[Sequence[schemas.MESSAGE_LIKE]] = None,
         metadata: Optional[Dict[str, str]] = None,
     ) -> Dict[str, Any]:
         """Create a thread.
 
         Args:
             thread_id (ID_T): The thread's ID.
             messages (Sequence[Dict[str, Any]]): The messages to add.
```

### Comparing `langmem-0.0.1rc9/langmem/integrations/langchain.py` & `langmem-0.0.2/langmem/integrations/langchain.py`

 * *Files identical despite different names*

### Comparing `langmem-0.0.1rc9/langmem/integrations/langgraph.py` & `langmem-0.0.2/langmem/integrations/langgraph.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 from collections import defaultdict
 from typing import TYPE_CHECKING, Any, Callable, Dict, List, Optional, TypedDict
 
 from langmem.client import AsyncClient as AsyncLangMemClient
 from langmem.client import Client as LangMemClient
 
 if TYPE_CHECKING:
-
     from langgraph.checkpoint.base import (  # type: ignore[import]
         BaseCheckpointSaver,
         Checkpoint,
     )
 try:
     from langchain_core.messages import BaseMessage  # type: ignore[import]
     from langchain_core.pydantic_v1 import Field  # type: ignore[import]
@@ -24,15 +23,15 @@
         RunnableConfig,
     )
     from langgraph.checkpoint.base import (  # type: ignore[import]
         BaseCheckpointSaver,
         Checkpoint,
     )
 except Exception:
-    from pydantic import BaseModel, Field
+    from pydantic import BaseModel, Field  # type: ignore[assignment]
 
     BaseCheckpointSaver = BaseModel  # type: ignore[misc, assignment]
 
 
 logger = logging.getLogger(__name__)
```

### Comparing `langmem-0.0.1rc9/pyproject.toml` & `langmem-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "langmem"
-version = "0.0.1rc9"
+version = "0.0.2"
 description = "The langmem alpha SDK"
 authors = ["William Fu-Hinthorn <13333726+hinthornw@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

