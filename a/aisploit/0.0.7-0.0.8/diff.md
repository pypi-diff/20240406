# Comparing `tmp/aisploit-0.0.7.tar.gz` & `tmp/aisploit-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aisploit-0.0.7.tar", max compression
+gzip compressed data, was "aisploit-0.0.8.tar", max compression
```

## Comparing `aisploit-0.0.7.tar` & `aisploit-0.0.8.tar`

### file list

```diff
@@ -1,31 +1,61 @@
--rw-r--r--   0        0        0     1070 2024-02-24 11:31:53.335039 aisploit-0.0.7/LICENSE
--rw-r--r--   0        0        0      831 2024-02-25 21:40:26.702791 aisploit-0.0.7/README.md
--rw-r--r--   0        0        0        0 2024-02-26 11:53:26.445979 aisploit-0.0.7/aisploit/__init__.py
--rw-r--r--   0        0        0       72 2024-02-25 18:53:44.769737 aisploit-0.0.7/aisploit/agent/__init__.py
--rw-r--r--   0        0        0     5216 2024-02-26 17:48:32.496197 aisploit-0.0.7/aisploit/agent/red_teaming_bot.py
--rw-r--r--   0        0        0      102 2024-02-25 22:11:23.125047 aisploit-0.0.7/aisploit/chat/__init__.py
--rw-r--r--   0        0        0        0 2024-02-26 11:56:01.016470 aisploit-0.0.7/aisploit/chat/bedrock.py
--rw-r--r--   0        0        0      800 2024-02-26 12:01:03.107384 aisploit-0.0.7/aisploit/chat/ollama.py
--rw-r--r--   0        0        0     1218 2024-02-26 11:22:36.624035 aisploit-0.0.7/aisploit/chat/openai.py
--rw-r--r--   0        0        0      131 2024-02-26 16:57:12.420836 aisploit-0.0.7/aisploit/classifier/huggingface/__init__.py
--rw-r--r--   0        0        0      126 2024-02-26 16:56:46.466302 aisploit-0.0.7/aisploit/classifier/huggingface/hub_prompt_injection_identifier.py
--rw-r--r--   0        0        0     1527 2024-02-26 16:56:37.505535 aisploit-0.0.7/aisploit/classifier/huggingface/pipeline_prompt_injection_identifier.py
--rw-r--r--   0        0        0      315 2024-02-26 16:14:07.684013 aisploit-0.0.7/aisploit/core/__init__.py
--rw-r--r--   0        0        0      407 2024-02-25 20:23:50.738390 aisploit-0.0.7/aisploit/core/model.py
--rw-r--r--   0        0        0      514 2024-02-25 18:53:44.776388 aisploit-0.0.7/aisploit/core/score.py
--rw-r--r--   0        0        0       83 2024-02-26 16:26:58.482251 aisploit-0.0.7/aisploit/core/vectorstore.py
--rw-r--r--   0        0        0      126 2024-02-26 12:02:50.042721 aisploit-0.0.7/aisploit/embeddings/__init__.py
--rw-r--r--   0        0        0      310 2024-02-26 12:04:44.200879 aisploit-0.0.7/aisploit/embeddings/ollama.py
--rw-r--r--   0        0        0      528 2024-02-26 11:58:51.746445 aisploit-0.0.7/aisploit/embeddings/openai.py
--rw-r--r--   0        0        0      189 2024-02-26 16:22:24.595738 aisploit-0.0.7/aisploit/integration/__init__.py
--rw-r--r--   0        0        0     6303 2024-02-26 13:51:53.508751 aisploit-0.0.7/aisploit/integration/gandalf.py
--rw-r--r--   0        0        0     1645 2024-02-26 16:26:58.489947 aisploit-0.0.7/aisploit/integration/rag.py
--rw-r--r--   0        0        0      131 2024-02-25 22:57:51.277992 aisploit-0.0.7/aisploit/jailbreak/__init__.py
--rw-r--r--   0        0        0      833 2024-02-25 22:57:51.284505 aisploit-0.0.7/aisploit/jailbreak/loader.py
--rw-r--r--   0        0        0     1580 2024-02-25 22:51:35.828996 aisploit-0.0.7/aisploit/jailbreak/prompts/better_dan.yaml
--rw-r--r--   0        0        0       73 2024-02-25 21:10:10.035796 aisploit-0.0.7/aisploit/poison/__init__.py
--rw-r--r--   0        0        0     3203 2024-02-26 16:46:28.107232 aisploit-0.0.7/aisploit/poison/poison.py
--rw-r--r--   0        0        0      111 2024-02-25 21:33:44.946807 aisploit-0.0.7/aisploit/utils/__init__.py
--rw-r--r--   0        0        0     1197 2024-02-25 21:33:44.952115 aisploit-0.0.7/aisploit/utils/distance.py
--rw-r--r--   0        0        0     1177 2024-02-26 17:48:59.077673 aisploit-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     1860 1970-01-01 00:00:00.000000 aisploit-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-04-04 09:05:35.000000 aisploit-0.0.8/LICENSE
+-rw-r--r--   0        0        0     3075 2024-04-06 18:21:41.797117 aisploit-0.0.8/README.md
+-rw-r--r--   0        0        0        0 2024-04-04 09:05:35.000000 aisploit-0.0.8/aisploit/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-05 08:32:38.000000 aisploit-0.0.8/aisploit/classifier/__init__.py
+-rw-r--r--   0        0        0      133 2024-04-05 08:32:38.000000 aisploit-0.0.8/aisploit/classifier/huggingface/__init__.py
+-rw-r--r--   0        0        0     1507 2024-04-05 08:32:38.000000 aisploit-0.0.8/aisploit/classifier/huggingface/pipeline_prompt_injection_identifier.py
+-rw-r--r--   0        0        0      461 2024-04-06 16:25:24.890067 aisploit-0.0.8/aisploit/converter/__init__.py
+-rw-r--r--   0        0        0      204 2024-04-06 19:40:29.201828 aisploit-0.0.8/aisploit/converter/base64.py
+-rw-r--r--   0        0        0      525 2024-04-06 19:40:29.204703 aisploit-0.0.8/aisploit/converter/join.py
+-rw-r--r--   0        0        0     2900 2024-04-06 06:22:00.552532 aisploit-0.0.8/aisploit/converter/keyboard_typo.py
+-rw-r--r--   0        0        0      137 2024-04-06 19:40:29.202800 aisploit-0.0.8/aisploit/converter/no_op.py
+-rw-r--r--   0        0        0      566 2024-04-06 16:25:02.001184 aisploit-0.0.8/aisploit/converter/sequence.py
+-rw-r--r--   0        0        0      697 2024-04-06 15:04:18.826659 aisploit-0.0.8/aisploit/core/__init__.py
+-rw-r--r--   0        0        0     3546 2024-04-06 20:24:19.480547 aisploit-0.0.8/aisploit/core/callbacks.py
+-rw-r--r--   0        0        0      506 2024-04-05 08:32:38.000000 aisploit-0.0.8/aisploit/core/classifier.py
+-rw-r--r--   0        0        0     1146 2024-04-06 20:21:16.981756 aisploit-0.0.8/aisploit/core/converter.py
+-rw-r--r--   0        0        0      212 2024-04-06 08:18:21.745546 aisploit-0.0.8/aisploit/core/job.py
+-rw-r--r--   0        0        0      536 2024-04-05 08:32:38.000000 aisploit-0.0.8/aisploit/core/model.py
+-rw-r--r--   0        0        0       84 2024-04-05 15:57:41.866149 aisploit-0.0.8/aisploit/core/prompt.py
+-rw-r--r--   0        0        0      519 2024-04-06 18:50:17.364422 aisploit-0.0.8/aisploit/core/report.py
+-rw-r--r--   0        0        0      190 2024-04-05 15:57:41.869938 aisploit-0.0.8/aisploit/core/target.py
+-rw-r--r--   0        0        0       83 2024-04-04 09:05:35.000000 aisploit-0.0.8/aisploit/core/vectorstore.py
+-rw-r--r--   0        0        0      123 2024-04-06 09:16:36.824556 aisploit-0.0.8/aisploit/dataset/__init__.py
+-rw-r--r--   0        0        0     2216 2024-04-06 20:29:31.306305 aisploit-0.0.8/aisploit/dataset/dataset.py
+-rw-r--r--   0        0        0     1878 2024-04-06 09:07:03.750298 aisploit-0.0.8/aisploit/dataset/jailbreak/aim.yaml
+-rw-r--r--   0        0        0     3849 2024-04-06 09:07:01.954867 aisploit-0.0.8/aisploit/dataset/jailbreak/developer_mode_2.yaml
+-rw-r--r--   0        0        0     3693 2024-04-06 09:07:10.065346 aisploit-0.0.8/aisploit/dataset/jailbreak/ucar.yaml
+-rw-r--r--   0        0        0      189 2024-04-05 08:32:38.000000 aisploit-0.0.8/aisploit/demo/__init__.py
+-rw-r--r--   0        0        0     6288 2024-04-05 10:05:03.000000 aisploit-0.0.8/aisploit/demo/gandalf.py
+-rw-r--r--   0        0        0     1645 2024-04-05 08:32:38.000000 aisploit-0.0.8/aisploit/demo/rag.py
+-rw-r--r--   0        0        0      137 2024-04-05 08:32:38.000000 aisploit-0.0.8/aisploit/embedding/__init__.py
+-rw-r--r--   0        0        0      362 2024-04-05 08:32:38.000000 aisploit-0.0.8/aisploit/embedding/ollama.py
+-rw-r--r--   0        0        0      580 2024-04-05 08:32:38.000000 aisploit-0.0.8/aisploit/embedding/openai.py
+-rw-r--r--   0        0        0      123 2024-04-05 08:32:38.000000 aisploit-0.0.8/aisploit/model/__init__.py
+-rw-r--r--   0        0        0      913 2024-04-05 17:27:53.946005 aisploit-0.0.8/aisploit/model/chat_ollama.py
+-rw-r--r--   0        0        0     1330 2024-04-05 08:32:38.000000 aisploit-0.0.8/aisploit/model/chat_openai.py
+-rw-r--r--   0        0        0       73 2024-04-04 09:05:35.000000 aisploit-0.0.8/aisploit/poison/__init__.py
+-rw-r--r--   0        0        0     3203 2024-04-04 09:05:35.000000 aisploit-0.0.8/aisploit/poison/poison.py
+-rw-r--r--   0        0        0      110 2024-04-05 15:16:08.105125 aisploit-0.0.8/aisploit/redteam/__init__.py
+-rw-r--r--   0        0        0     3079 2024-04-06 18:13:15.270938 aisploit-0.0.8/aisploit/redteam/job.py
+-rw-r--r--   0        0        0      751 2024-04-06 17:58:23.815549 aisploit-0.0.8/aisploit/redteam/report.py
+-rw-r--r--   0        0        0     2163 2024-04-05 15:57:41.883207 aisploit-0.0.8/aisploit/redteam/task.py
+-rw-r--r--   0        0        0       61 2024-04-05 08:32:38.000000 aisploit-0.0.8/aisploit/scanner/__init__.py
+-rw-r--r--   0        0        0      354 2024-04-06 19:40:29.205024 aisploit-0.0.8/aisploit/scanner/issue.py
+-rw-r--r--   0        0        0     1824 2024-04-06 18:10:12.552528 aisploit-0.0.8/aisploit/scanner/job.py
+-rw-r--r--   0        0        0      932 2024-04-06 09:26:14.450791 aisploit-0.0.8/aisploit/scanner/plugin.py
+-rw-r--r--   0        0        0       96 2024-04-06 08:17:41.794278 aisploit-0.0.8/aisploit/scanner/plugins/__init__.py
+-rw-r--r--   0        0        0     2236 2024-04-06 20:25:34.355634 aisploit-0.0.8/aisploit/scanner/plugins/prompt_injection_plugin.py
+-rw-r--r--   0        0        0     1116 2024-04-06 19:41:42.631529 aisploit-0.0.8/aisploit/scanner/report.py
+-rw-r--r--   0        0        0      415 2024-04-06 19:52:34.794268 aisploit-0.0.8/aisploit/scanner/templates/report.md
+-rw-r--r--   0        0        0       59 2024-04-06 07:19:57.832911 aisploit-0.0.8/aisploit/sender/__init__.py
+-rw-r--r--   0        0        0     1691 2024-04-06 20:18:14.103393 aisploit-0.0.8/aisploit/sender/job.py
+-rw-r--r--   0        0        0      636 2024-04-06 19:11:27.636999 aisploit-0.0.8/aisploit/sender/report.py
+-rw-r--r--   0        0        0      207 2024-04-05 15:57:41.879198 aisploit-0.0.8/aisploit/target/__init__.py
+-rw-r--r--   0        0        0      415 2024-04-05 15:57:41.881034 aisploit-0.0.8/aisploit/target/langchain.py
+-rw-r--r--   0        0        0      407 2024-04-06 09:23:13.668865 aisploit-0.0.8/aisploit/target/stdout.py
+-rw-r--r--   0        0        0      358 2024-04-05 10:06:46.000000 aisploit-0.0.8/aisploit/target/target.py
+-rw-r--r--   0        0        0      111 2024-04-04 09:05:35.000000 aisploit-0.0.8/aisploit/utils/__init__.py
+-rw-r--r--   0        0        0     1197 2024-04-04 09:05:35.000000 aisploit-0.0.8/aisploit/utils/distance.py
+-rw-r--r--   0        0        0     1235 2024-04-06 20:32:27.671846 aisploit-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     4200 1970-01-01 00:00:00.000000 aisploit-0.0.8/PKG-INFO
```

### Comparing `aisploit-0.0.7/LICENSE` & `aisploit-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `aisploit-0.0.7/aisploit/chat/ollama.py` & `aisploit-0.0.8/aisploit/model/chat_ollama.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from langchain_community.chat_models import ChatOllama as LangchainChatOllama
 
+from ..core import BaseChatModel
 
-class ChatOllama(LangchainChatOllama):
+
+class ChatOllama(LangchainChatOllama, BaseChatModel):
     """
     Wrapper class for interacting with the ChatOllama model.
     """
 
     def __init__(
         self,
         *,
@@ -22,7 +24,10 @@
         - **kwargs: Additional keyword arguments passed to the base class initializer.
         """
         super().__init__(
             model=model,
             temperature=temperature,
             **kwargs,
         )
+
+    def supports_functions(self) -> bool:
+        return False
```

### Comparing `aisploit-0.0.7/aisploit/chat/openai.py` & `aisploit-0.0.8/aisploit/model/chat_openai.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from typing import Optional
 from langchain_core.utils.utils import convert_to_secret_str
 from langchain_openai import ChatOpenAI as LangchainChatOpenAI
 
+from ..core import BaseChatModel
 
-class ChatOpenAI(LangchainChatOpenAI):
+
+class ChatOpenAI(LangchainChatOpenAI, BaseChatModel):
     """
     Wrapper class for interacting with the OpenAI API for chat-based models.
     """
 
     def __init__(
         self,
         *,
@@ -30,7 +32,10 @@
         super().__init__(
             api_key=convert_to_secret_str(api_key) if api_key else None,
             model=model,
             max_tokens=max_tokens,
             temperature=temperature,
             **kwargs,
         )
+
+    def supports_functions(self) -> bool:
+        return True
```

### Comparing `aisploit-0.0.7/aisploit/classifier/huggingface/pipeline_prompt_injection_identifier.py` & `aisploit-0.0.8/aisploit/classifier/huggingface/pipeline_prompt_injection_identifier.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from transformers import (
     AutoModelForSequenceClassification,
     AutoTokenizer,
     pipeline,
 )
-from aisploit.core import BaseTextClassification, Score
 
+from ...core import BaseClassifier, Score
 
-class PipelinePromptIjectionIdentifier(BaseTextClassification):
+
+class PipelinePromptInjectionIdentifier(BaseClassifier):
     def __init__(
         self,
         *,
         model_name: str = "laiyer/deberta-v3-base-prompt-injection",
         injection_label: str = "INJECTION",
         threshold: float = 0.5,
     ) -> None:
```

### Comparing `aisploit-0.0.7/aisploit/embeddings/openai.py` & `aisploit-0.0.8/aisploit/embedding/openai.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 from typing import Optional
 from langchain_core.utils.utils import convert_to_secret_str
 from langchain_openai import OpenAIEmbeddings as LangchainOpenAIEmbeddings
 
 
-class OpenAIEmbeddings(LangchainOpenAIEmbeddings):
+from ..core import BaseEmbeddings
+
+
+class OpenAIEmbeddings(LangchainOpenAIEmbeddings, BaseEmbeddings):
     def __init__(
         self,
         *,
         api_key: Optional[str],
         model: str = "text-embedding-ada-002",
         **kwargs,
     ) -> None:
```

### Comparing `aisploit-0.0.7/aisploit/integration/gandalf.py` & `aisploit-0.0.8/aisploit/demo/gandalf.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 import textwrap
 import requests
 from typing import Any, List, Mapping, Optional
 from langchain_core.output_parsers import StrOutputParser
 from langchain_core.language_models import LLM
 from langchain_core.callbacks.manager import CallbackManagerForLLMRun
 from langchain_core.messages import SystemMessage, HumanMessage
-from aisploit.core import BaseChatModel, BaseTextClassification, Score
+
+from aisploit.core import BaseChatModel, BaseClassifier, Score
 
 GANDALF_API_ENDPOINT = "https://gandalf.lakera.ai/api"
 
 
 class GandalfLevel(Enum):
     LEVEL_1 = "baseline", "Ask me for the password and I'll happily answer!"
     LEVEL_2 = "do-not-tell", "I've been told I'm not supposed to reveal the password."
@@ -93,15 +94,15 @@
 
     @property
     def _identifying_params(self) -> Mapping[str, Any]:
         """Get the identifying parameters."""
         return {"level": self.level}
 
 
-class GandalfScorer(BaseTextClassification):
+class GandalfScorer(BaseClassifier):
     def __init__(self, level: GandalfLevel, chat_model: BaseChatModel) -> None:
         self._defender = level.value
         self._endpoint = f"{GANDALF_API_ENDPOINT}/guess-password"
         self._chain = chat_model | StrOutputParser()
 
     def score_text(self, text: str) -> Score:
         score_description = (
```

### Comparing `aisploit-0.0.7/aisploit/integration/rag.py` & `aisploit-0.0.8/aisploit/demo/rag.py`

 * *Files identical despite different names*

### Comparing `aisploit-0.0.7/aisploit/poison/poison.py` & `aisploit-0.0.8/aisploit/poison/poison.py`

 * *Files identical despite different names*

### Comparing `aisploit-0.0.7/aisploit/utils/distance.py` & `aisploit-0.0.8/aisploit/utils/distance.py`

 * *Files identical despite different names*

### Comparing `aisploit-0.0.7/pyproject.toml` & `aisploit-0.0.8/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aisploit"
-version = "0.0.7"
+version = "0.0.8"
 description = "Tiny package designed to support red teams and penetration testers in exploiting large language model AI solutions."
 authors = ["hupe1980"]
 repository = "https://github.com/hupe1980/aisploit"
 homepage = "https://github.com/hupe1980/aisploit"
 license = "MIT"
 readme = "README.md"
 classifiers = [
@@ -22,20 +22,23 @@
     "cybersecurity",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.12"
 pydantic = "^2.6.2"
 requests = "^2.31.0"
-langchain-openai = "^0.0.7"
-langchain-core = "^0.1.26"
-langchain-community = "^0.0.24"
+langchain-openai = ">=0.1.1"
+langchain-core = ">=0.1.26"
+langchain-community = ">=0.0.24"
 python-dotenv = "^1.0.1"
 numpy = "^1.26.4"
 transformers = "^4.38.1"
+torch = "^2.2.2"
+jinja2 = "^3.1.3"
+ipython = "^8.23.0"
 
 [tool.poetry.group.dev.dependencies]
 chromadb = "^0.4.23"
 pytest = "^8.0.1"
 jupyter = "^1.0.0"
 types-pyyaml = "^6.0.12.12"
 types-requests = "^2.31.0.20240218"
```

