# Comparing `tmp/tonic_validate-4.0.4.tar.gz` & `tmp/tonic_validate-4.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tonic_validate-4.0.4.tar", max compression
+gzip compressed data, was "tonic_validate-4.0.5.tar", max compression
```

## Comparing `tonic_validate-4.0.4.tar` & `tonic_validate-4.0.5.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0     1063 2024-03-27 18:15:28.298515 tonic_validate-4.0.4/LICENSE
--rw-r--r--   0        0        0    24507 2024-03-27 18:15:28.298515 tonic_validate-4.0.4/README.md
--rw-r--r--   0        0        0      771 2024-03-27 18:15:28.354515 tonic_validate-4.0.4/pyproject.toml
--rw-r--r--   0        0        0      459 2024-03-27 18:15:28.358515 tonic_validate-4.0.4/tonic_validate/__init__.py
--rw-r--r--   0        0        0      387 2024-03-27 18:15:28.358515 tonic_validate-4.0.4/tonic_validate/classes/__init__.py
--rw-r--r--   0        0        0     2106 2024-03-27 18:15:28.358515 tonic_validate-4.0.4/tonic_validate/classes/benchmark.py
--rw-r--r--   0        0        0      247 2024-03-27 18:15:28.358515 tonic_validate-4.0.4/tonic_validate/classes/exceptions.py
--rw-r--r--   0        0        0     1023 2024-03-27 18:15:28.358515 tonic_validate-4.0.4/tonic_validate/classes/llm_response.py
--rw-r--r--   0        0        0     2515 2024-03-27 18:15:28.358515 tonic_validate-4.0.4/tonic_validate/classes/run.py
--rw-r--r--   0        0        0      314 2024-03-27 18:15:28.358515 tonic_validate-4.0.4/tonic_validate/classes/user_info.py
--rw-r--r--   0        0        0      805 2024-03-27 18:15:28.358515 tonic_validate-4.0.4/tonic_validate/config.py
--rw-r--r--   0        0        0     1483 2024-03-27 18:15:28.358515 tonic_validate-4.0.4/tonic_validate/metrics/__init__.py
--rw-r--r--   0        0        0     1509 2024-03-27 18:15:28.358515 tonic_validate-4.0.4/tonic_validate/metrics/answer_consistency_binary_metric.py
--rw-r--r--   0        0        0     1645 2024-03-27 18:15:28.358515 tonic_validate-4.0.4/tonic_validate/metrics/answer_consistency_metric.py
--rw-r--r--   0        0        0     2784 2024-03-27 18:15:28.358515 tonic_validate-4.0.4/tonic_validate/metrics/answer_contains_pii_metric.py
--rw-r--r--   0        0        0     1257 2024-03-27 18:15:28.358515 tonic_validate-4.0.4/tonic_validate/metrics/answer_match_metric.py
--rw-r--r--   0        0        0     1659 2024-03-27 18:15:28.358515 tonic_validate-4.0.4/tonic_validate/metrics/answer_similarity_metric.py
--rw-r--r--   0        0        0     1761 2024-03-27 18:15:28.358515 tonic_validate-4.0.4/tonic_validate/metrics/augmentation_accuracy_metric.py
--rw-r--r--   0        0        0     2354 2024-03-27 18:15:28.358515 tonic_validate-4.0.4/tonic_validate/metrics/augmentation_precision_metric.py
--rw-r--r--   0        0        0     1452 2024-03-27 18:15:28.358515 tonic_validate-4.0.4/tonic_validate/metrics/binary_metric.py
--rw-r--r--   0        0        0     1747 2024-03-27 18:15:28.358515 tonic_validate-4.0.4/tonic_validate/metrics/contains_text_metric.py
--rw-r--r--   0        0        0     2808 2024-03-27 18:15:28.358515 tonic_validate-4.0.4/tonic_validate/metrics/context_contains_pii_metric.py
--rw-r--r--   0        0        0     1786 2024-03-27 18:15:28.358515 tonic_validate-4.0.4/tonic_validate/metrics/context_length_metric.py
--rw-r--r--   0        0        0     1072 2024-03-27 18:15:28.358515 tonic_validate-4.0.4/tonic_validate/metrics/duplication_metric.py
--rw-r--r--   0        0        0      999 2024-03-27 18:15:28.358515 tonic_validate-4.0.4/tonic_validate/metrics/hate_speech_content_metric.py
--rw-r--r--   0        0        0     1173 2024-03-27 18:15:28.358515 tonic_validate-4.0.4/tonic_validate/metrics/latency_metric.py
--rw-r--r--   0        0        0      484 2024-03-27 18:15:28.358515 tonic_validate-4.0.4/tonic_validate/metrics/metric.py
--rw-r--r--   0        0        0     1239 2024-03-27 18:15:28.358515 tonic_validate-4.0.4/tonic_validate/metrics/regex_metric.py
--rw-r--r--   0        0        0     1448 2024-03-27 18:15:28.358515 tonic_validate-4.0.4/tonic_validate/metrics/response_length_metric.py
--rw-r--r--   0        0        0     1724 2024-03-27 18:15:28.362515 tonic_validate-4.0.4/tonic_validate/metrics/retrieval_precision_metric.py
--rw-r--r--   0        0        0     4626 2024-03-27 18:15:28.362515 tonic_validate-4.0.4/tonic_validate/services/openai_service.py
--rw-r--r--   0        0        0    18492 2024-03-27 18:15:28.362515 tonic_validate-4.0.4/tonic_validate/tests/test_scorer.py
--rw-r--r--   0        0        0        0 2024-03-27 18:15:28.362515 tonic_validate-4.0.4/tonic_validate/utils/__init__.py
--rw-r--r--   0        0        0     2880 2024-03-27 18:15:28.362515 tonic_validate-4.0.4/tonic_validate/utils/http_client.py
--rw-r--r--   0        0        0    18924 2024-03-27 18:15:28.362515 tonic_validate-4.0.4/tonic_validate/utils/llm_calls.py
--rw-r--r--   0        0        0     2198 2024-03-27 18:15:28.362515 tonic_validate-4.0.4/tonic_validate/utils/metrics_util.py
--rw-r--r--   0        0        0      530 2024-03-27 18:15:28.362515 tonic_validate-4.0.4/tonic_validate/utils/openai_cache.py
--rw-r--r--   0        0        0     4516 2024-03-27 18:15:28.362515 tonic_validate-4.0.4/tonic_validate/utils/telemetry.py
--rw-r--r--   0        0        0     4271 2024-03-27 18:15:28.362515 tonic_validate-4.0.4/tonic_validate/validate_api.py
--rw-r--r--   0        0        0    12857 2024-03-27 18:15:28.362515 tonic_validate-4.0.4/tonic_validate/validate_scorer.py
--rw-r--r--   0        0        0    25266 1970-01-01 00:00:00.000000 tonic_validate-4.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-04-05 22:11:41.013217 tonic_validate-4.0.5/LICENSE
+-rw-r--r--   0        0        0    24571 2024-04-05 22:11:41.013217 tonic_validate-4.0.5/README.md
+-rw-r--r--   0        0        0      771 2024-04-05 22:11:41.077217 tonic_validate-4.0.5/pyproject.toml
+-rw-r--r--   0        0        0      459 2024-04-05 22:11:41.081217 tonic_validate-4.0.5/tonic_validate/__init__.py
+-rw-r--r--   0        0        0      387 2024-04-05 22:11:41.081217 tonic_validate-4.0.5/tonic_validate/classes/__init__.py
+-rw-r--r--   0        0        0     2106 2024-04-05 22:11:41.081217 tonic_validate-4.0.5/tonic_validate/classes/benchmark.py
+-rw-r--r--   0        0        0      247 2024-04-05 22:11:41.081217 tonic_validate-4.0.5/tonic_validate/classes/exceptions.py
+-rw-r--r--   0        0        0     1023 2024-04-05 22:11:41.081217 tonic_validate-4.0.5/tonic_validate/classes/llm_response.py
+-rw-r--r--   0        0        0     2630 2024-04-05 22:11:41.081217 tonic_validate-4.0.5/tonic_validate/classes/run.py
+-rw-r--r--   0        0        0      314 2024-04-05 22:11:41.081217 tonic_validate-4.0.5/tonic_validate/classes/user_info.py
+-rw-r--r--   0        0        0      805 2024-04-05 22:11:41.081217 tonic_validate-4.0.5/tonic_validate/config.py
+-rw-r--r--   0        0        0     1483 2024-04-05 22:11:41.081217 tonic_validate-4.0.5/tonic_validate/metrics/__init__.py
+-rw-r--r--   0        0        0     1584 2024-04-05 22:11:41.081217 tonic_validate-4.0.5/tonic_validate/metrics/answer_consistency_binary_metric.py
+-rw-r--r--   0        0        0     1971 2024-04-05 22:11:41.081217 tonic_validate-4.0.5/tonic_validate/metrics/answer_consistency_metric.py
+-rw-r--r--   0        0        0     2784 2024-04-05 22:11:41.081217 tonic_validate-4.0.5/tonic_validate/metrics/answer_contains_pii_metric.py
+-rw-r--r--   0        0        0     1257 2024-04-05 22:11:41.081217 tonic_validate-4.0.5/tonic_validate/metrics/answer_match_metric.py
+-rw-r--r--   0        0        0     1728 2024-04-05 22:11:41.081217 tonic_validate-4.0.5/tonic_validate/metrics/answer_similarity_metric.py
+-rw-r--r--   0        0        0     1844 2024-04-05 22:11:41.081217 tonic_validate-4.0.5/tonic_validate/metrics/augmentation_accuracy_metric.py
+-rw-r--r--   0        0        0     2354 2024-04-05 22:11:41.081217 tonic_validate-4.0.5/tonic_validate/metrics/augmentation_precision_metric.py
+-rw-r--r--   0        0        0     1452 2024-04-05 22:11:41.081217 tonic_validate-4.0.5/tonic_validate/metrics/binary_metric.py
+-rw-r--r--   0        0        0     1747 2024-04-05 22:11:41.081217 tonic_validate-4.0.5/tonic_validate/metrics/contains_text_metric.py
+-rw-r--r--   0        0        0     2808 2024-04-05 22:11:41.081217 tonic_validate-4.0.5/tonic_validate/metrics/context_contains_pii_metric.py
+-rw-r--r--   0        0        0     1786 2024-04-05 22:11:41.081217 tonic_validate-4.0.5/tonic_validate/metrics/context_length_metric.py
+-rw-r--r--   0        0        0     1155 2024-04-05 22:11:41.081217 tonic_validate-4.0.5/tonic_validate/metrics/duplication_metric.py
+-rw-r--r--   0        0        0     1076 2024-04-05 22:11:41.081217 tonic_validate-4.0.5/tonic_validate/metrics/hate_speech_content_metric.py
+-rw-r--r--   0        0        0     1173 2024-04-05 22:11:41.081217 tonic_validate-4.0.5/tonic_validate/metrics/latency_metric.py
+-rw-r--r--   0        0        0      725 2024-04-05 22:11:41.081217 tonic_validate-4.0.5/tonic_validate/metrics/metric.py
+-rw-r--r--   0        0        0     1239 2024-04-05 22:11:41.081217 tonic_validate-4.0.5/tonic_validate/metrics/regex_metric.py
+-rw-r--r--   0        0        0     1448 2024-04-05 22:11:41.081217 tonic_validate-4.0.5/tonic_validate/metrics/response_length_metric.py
+-rw-r--r--   0        0        0     1795 2024-04-05 22:11:41.081217 tonic_validate-4.0.5/tonic_validate/metrics/retrieval_precision_metric.py
+-rw-r--r--   0        0        0     4626 2024-04-05 22:11:41.081217 tonic_validate-4.0.5/tonic_validate/services/openai_service.py
+-rw-r--r--   0        0        0    18492 2024-04-05 22:11:41.081217 tonic_validate-4.0.5/tonic_validate/tests/test_scorer.py
+-rw-r--r--   0        0        0        0 2024-04-05 22:11:41.081217 tonic_validate-4.0.5/tonic_validate/utils/__init__.py
+-rw-r--r--   0        0        0     2880 2024-04-05 22:11:41.081217 tonic_validate-4.0.5/tonic_validate/utils/http_client.py
+-rw-r--r--   0        0        0    19067 2024-04-05 22:11:41.081217 tonic_validate-4.0.5/tonic_validate/utils/llm_calls.py
+-rw-r--r--   0        0        0     2198 2024-04-05 22:11:41.081217 tonic_validate-4.0.5/tonic_validate/utils/metrics_util.py
+-rw-r--r--   0        0        0      530 2024-04-05 22:11:41.081217 tonic_validate-4.0.5/tonic_validate/utils/openai_cache.py
+-rw-r--r--   0        0        0     4961 2024-04-05 22:11:41.081217 tonic_validate-4.0.5/tonic_validate/utils/telemetry.py
+-rw-r--r--   0        0        0     4381 2024-04-05 22:11:41.081217 tonic_validate-4.0.5/tonic_validate/validate_api.py
+-rw-r--r--   0        0        0    13171 2024-04-05 22:11:41.081217 tonic_validate-4.0.5/tonic_validate/validate_scorer.py
+-rw-r--r--   0        0        0    25330 1970-01-01 00:00:00.000000 tonic_validate-4.0.5/PKG-INFO
```

### Comparing `tonic_validate-4.0.4/LICENSE` & `tonic_validate-4.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `tonic_validate-4.0.4/README.md` & `tonic_validate-4.0.5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -437,15 +437,17 @@
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 ### Telemetry
 Tonic Validate collects minimal telemetry to help us figure out what users want and how they're using the product. We do not use any existing telemetry framework and instead created our own privacy focused setup. Only the following information is tracked
 
 * What metrics were used for a run
 * Number of questions in a run
+* Time taken for a run to be evaluated
 * Number of questions in a benchmark
+* SDK Version being used
 
 We do **NOT** track things such as the contents of the questions / answers, your scores, or any other sensitive information. For detecting CI/CD, we only check for common environment variables in different CI/CD environments. We do not log the values of these environment variables.
 
 We also generate a random UUID to help us figure out how many users are using the product. This UUID is linked to your Validate account only to help track who is using the SDK and UI at once and to get user counts. If you want to see how we implemented telemetry, you can do so in the `tonic_validate/utils/telemetry.py` file
 
 If you wish to opt out of telemetry, you only need to set the `TONIC_VALIDATE_DO_NOT_TRACK` environment variable to `True`.
```

### Comparing `tonic_validate-4.0.4/pyproject.toml` & `tonic_validate-4.0.5/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tonic-validate"
-version = "4.0.4"
+version = "4.0.5"
 description = "RAG evaluation metrics."
 authors = ["Joe Ferrara <joeferrara@tonic.ai>", "Ethan Philpott <ephilpott@tonic.ai>", "Adam Kamor <adam@tonic.ai>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0.0"
 openai = ">=1.0.0"
```

### Comparing `tonic_validate-4.0.4/tonic_validate/classes/benchmark.py` & `tonic_validate-4.0.5/tonic_validate/classes/benchmark.py`

 * *Files identical despite different names*

### Comparing `tonic_validate-4.0.4/tonic_validate/classes/llm_response.py` & `tonic_validate-4.0.5/tonic_validate/classes/llm_response.py`

 * *Files identical despite different names*

### Comparing `tonic_validate-4.0.4/tonic_validate/classes/run.py` & `tonic_validate-4.0.5/tonic_validate/classes/run.py`

 * *Files 7% similar despite different names*

```diff
@@ -54,20 +54,23 @@
 
     Parameters:
     -----------
     overall_scores: Dict[str, float]
         The overall scores for the run
     run_data: List[RunData]
         The run data
+    llm_evaluator: Optional[str]
+        The name of the language model evaluator
     id: Optional[UUID]
         The identifier of the run
     """
 
     overall_scores: Dict[str, float]
     run_data: List[RunData]
+    llm_evaluator: Optional[str]
     id: Optional[UUID]
 
     def to_df(self):
         """
         Convert the run data to a pandas DataFrame
 
         Returns:
```

### Comparing `tonic_validate-4.0.4/tonic_validate/config.py` & `tonic_validate-4.0.5/tonic_validate/config.py`

 * *Files identical despite different names*

### Comparing `tonic_validate-4.0.4/tonic_validate/metrics/__init__.py` & `tonic_validate-4.0.5/tonic_validate/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `tonic_validate-4.0.4/tonic_validate/metrics/answer_consistency_binary_metric.py` & `tonic_validate-4.0.5/tonic_validate/metrics/answer_consistency_binary_metric.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import logging
 from tonic_validate.classes.llm_response import LLMResponse
 from tonic_validate.metrics.binary_metric import BinaryMetric
 from tonic_validate.utils.metrics_util import parse_boolean_response
 from tonic_validate.services.openai_service import OpenAIService
-from tonic_validate.utils.llm_calls import answer_consistent_with_context_call
+from tonic_validate.utils.llm_calls import answer_consistent_with_context_call, context_consistency_prompt
 
 logger = logging.getLogger()
 
 
 class AnswerConsistencyBinaryMetric(BinaryMetric):
     name: str = "answer_consistency_binary"
+    prompt: str = context_consistency_prompt()
 
     def __init__(self):
         """
         Binary metric that checks whether there is information in the LLM answer that does not come from the context.
         Returns either 1 (consistent) or 0 (inconsistent).
         """
         super().__init__(self.name, self.metric_callback)
```

### Comparing `tonic_validate-4.0.4/tonic_validate/metrics/answer_consistency_metric.py` & `tonic_validate-4.0.5/tonic_validate/metrics/answer_consistency_metric.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,21 +5,30 @@
     parse_boolean_response,
     parse_bullet_list_response,
 )
 from tonic_validate.services.openai_service import OpenAIService
 from tonic_validate.utils.llm_calls import (
     main_points_call,
     statement_derived_from_context_call,
+    statement_derived_from_context_prompt,
+    main_points_prompt,
 )
 
 logger = logging.getLogger()
 
 
 class AnswerConsistencyMetric(Metric):
     name: str = "answer_consistency"
+    prompt: str = (
+        "-------------------\n"
+        f"{main_points_prompt()}\n"
+        "-------------------\n"
+        f"{statement_derived_from_context_prompt(statement='EXAMPLE STATEMENT', context_list=[])}\n"
+        "-------------------\n"
+    )
 
     def __init__(self):
         """
         Metric that checks whether the LLM answer contains information that does not come from the context.
         Returns a float between 0 and 1, where 1 is completely consistent and 0 is completely inconsistent.
         """
         pass
```

### Comparing `tonic_validate-4.0.4/tonic_validate/metrics/answer_contains_pii_metric.py` & `tonic_validate-4.0.5/tonic_validate/metrics/answer_contains_pii_metric.py`

 * *Files identical despite different names*

### Comparing `tonic_validate-4.0.4/tonic_validate/metrics/answer_match_metric.py` & `tonic_validate-4.0.5/tonic_validate/metrics/answer_match_metric.py`

 * *Files identical despite different names*

### Comparing `tonic_validate-4.0.4/tonic_validate/metrics/answer_similarity_metric.py` & `tonic_validate-4.0.5/tonic_validate/metrics/answer_similarity_metric.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import logging
 from tonic_validate.classes.llm_response import LLMResponse
 from tonic_validate.metrics.metric import Metric
 from tonic_validate.services.openai_service import OpenAIService
-from tonic_validate.utils.llm_calls import similarity_score_call
+from tonic_validate.utils.llm_calls import similarity_score_call, similarity_score_prompt
 
 logger = logging.getLogger()
 
 
 class AnswerSimilarityMetric(Metric):
     name: str = "answer_similarity"
+    prompt: str = similarity_score_prompt()
 
     def __init__(self) -> None:
         """
         Metric that checks how well the reference answer matches the LLM answer.
         Returns a float between 0 and 5, where 5 is the most similar and 0 is the least similar.
         """
         pass
```

### Comparing `tonic_validate-4.0.4/tonic_validate/metrics/augmentation_accuracy_metric.py` & `tonic_validate-4.0.5/tonic_validate/metrics/augmentation_accuracy_metric.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import logging
 from typing import List, Tuple
 from tonic_validate.classes.llm_response import LLMResponse
 from tonic_validate.metrics.metric import Metric
 from tonic_validate.utils.metrics_util import parse_boolean_response
 from tonic_validate.services.openai_service import OpenAIService
-from tonic_validate.utils.llm_calls import answer_contains_context_call
+from tonic_validate.utils.llm_calls import answer_contains_context_call, answer_contains_context_prompt
 
 logger = logging.getLogger()
 
 
 class AugmentationAccuracyMetric(Metric):
     name: str = "augmentation_accuracy"
+    prompt: str = answer_contains_context_prompt()
 
     def __init__(self):
         """
         Metric that checks whether the LLM answer includes all of the context.
         Returns a float between 0 and 1. 1 indicates that the answer contains all of the context. 0 indicates that it contains none of the context.
         """
         pass
```

### Comparing `tonic_validate-4.0.4/tonic_validate/metrics/augmentation_precision_metric.py` & `tonic_validate-4.0.5/tonic_validate/metrics/augmentation_precision_metric.py`

 * *Files identical despite different names*

### Comparing `tonic_validate-4.0.4/tonic_validate/metrics/binary_metric.py` & `tonic_validate-4.0.5/tonic_validate/metrics/binary_metric.py`

 * *Files identical despite different names*

### Comparing `tonic_validate-4.0.4/tonic_validate/metrics/contains_text_metric.py` & `tonic_validate-4.0.5/tonic_validate/metrics/contains_text_metric.py`

 * *Files identical despite different names*

### Comparing `tonic_validate-4.0.4/tonic_validate/metrics/context_contains_pii_metric.py` & `tonic_validate-4.0.5/tonic_validate/metrics/context_contains_pii_metric.py`

 * *Files identical despite different names*

### Comparing `tonic_validate-4.0.4/tonic_validate/metrics/context_length_metric.py` & `tonic_validate-4.0.5/tonic_validate/metrics/context_length_metric.py`

 * *Files identical despite different names*

### Comparing `tonic_validate-4.0.4/tonic_validate/metrics/duplication_metric.py` & `tonic_validate-4.0.5/tonic_validate/metrics/duplication_metric.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import logging
 
 from tonic_validate.classes.llm_response import LLMResponse
 from tonic_validate.metrics.binary_metric import BinaryMetric
 from tonic_validate.services.openai_service import OpenAIService
-from tonic_validate.utils.llm_calls import contains_duplicate_information
+from tonic_validate.utils.llm_calls import contains_duplicate_information, contains_duplicate_info_prompt
 from tonic_validate.utils.metrics_util import parse_boolean_response
 
 logger = logging.getLogger()
 
 
 class DuplicationMetric(BinaryMetric):
     name: str = "duplication_metric"
+    prompt: str = contains_duplicate_info_prompt()
 
     def __init__(self):
         """
         Binary metric that checks whether the response contains duplicate information.
         Returns 1 (True) if the response contains duplicate information. Returns 0 (False) if it does not contain duplicate information.
         """
         super().__init__(self.name, self.metric_callback)
```

### Comparing `tonic_validate-4.0.4/tonic_validate/metrics/hate_speech_content_metric.py` & `tonic_validate-4.0.5/tonic_validate/metrics/hate_speech_content_metric.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import logging
 
 from tonic_validate.classes.llm_response import LLMResponse
 from tonic_validate.metrics.binary_metric import BinaryMetric
 from tonic_validate.services.openai_service import OpenAIService
-from tonic_validate.utils.llm_calls import contains_hate_speech
+from tonic_validate.utils.llm_calls import contains_hate_speech, contains_hate_speech_prompt
 from tonic_validate.utils.metrics_util import parse_boolean_response
 
 logger = logging.getLogger()
 
 
 class HateSpeechContentMetric(BinaryMetric):
     name: str = "hate_speech_content"
+    prompt: str = contains_hate_speech_prompt()
 
     def __init__(self):
         """
         Binary metric that checks whether the response contains hate speech.
         Returns 1 (True) if the response contains hate speech. Returns 0 (False) if it does not contain hate speech.
         """
         super().__init__(self.name, self.metric_callback)
```

### Comparing `tonic_validate-4.0.4/tonic_validate/metrics/latency_metric.py` & `tonic_validate-4.0.5/tonic_validate/metrics/latency_metric.py`

 * *Files identical despite different names*

### Comparing `tonic_validate-4.0.4/tonic_validate/metrics/regex_metric.py` & `tonic_validate-4.0.5/tonic_validate/metrics/regex_metric.py`

 * *Files identical despite different names*

### Comparing `tonic_validate-4.0.4/tonic_validate/metrics/response_length_metric.py` & `tonic_validate-4.0.5/tonic_validate/metrics/response_length_metric.py`

 * *Files identical despite different names*

### Comparing `tonic_validate-4.0.4/tonic_validate/metrics/retrieval_precision_metric.py` & `tonic_validate-4.0.5/tonic_validate/metrics/retrieval_precision_metric.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import logging
 from typing import List, Tuple
 from tonic_validate.classes.llm_response import LLMResponse
 from tonic_validate.metrics.metric import Metric
 from tonic_validate.utils.metrics_util import parse_boolean_response
 from tonic_validate.services.openai_service import OpenAIService
-from tonic_validate.utils.llm_calls import context_relevancy_call
+from tonic_validate.utils.llm_calls import context_relevancy_call, context_relevancy_prompt
 
 logger = logging.getLogger()
 
 
 class RetrievalPrecisionMetric(Metric):
     name: str = "retrieval_precision"
+    prompt: str = context_relevancy_prompt()
 
     def __init__(self):
         """
         Metric that checks whether the retrieved context is relevant to answer the given question.
         Returns a float between 0 and 1. 1 indicates that all of the context is relevant. 0 indicates that none of the context is relevant.
         """
         pass
```

### Comparing `tonic_validate-4.0.4/tonic_validate/services/openai_service.py` & `tonic_validate-4.0.5/tonic_validate/services/openai_service.py`

 * *Files identical despite different names*

### Comparing `tonic_validate-4.0.4/tonic_validate/tests/test_scorer.py` & `tonic_validate-4.0.5/tonic_validate/tests/test_scorer.py`

 * *Files identical despite different names*

### Comparing `tonic_validate-4.0.4/tonic_validate/utils/http_client.py` & `tonic_validate-4.0.5/tonic_validate/utils/http_client.py`

 * *Files identical despite different names*

### Comparing `tonic_validate-4.0.4/tonic_validate/utils/llm_calls.py` & `tonic_validate-4.0.5/tonic_validate/utils/llm_calls.py`

 * *Files 2% similar despite different names*

```diff
@@ -356,20 +356,17 @@
     -------
     str
         Response from OpenAI API.
     """
     logger.debug(
         f"Asking {openai_service.model} whether statement is derived from context"
     )
-    main_message = "Considering the following statement and list of context(s)"
-    main_message += f"\n\nSTATEMENT:\n{statement}\nEND OF STATEMENT"
-    for i, context in enumerate(context_list):
-        main_message += f"\n\nCONTEXT {i}:\n{context}\nEND OF CONTEXT {i}"
 
-    main_message = statement_derived_from_context_prompt(main_message)
+    main_message = statement_derived_from_context_prompt(statement, context_list)
+
     try:
         response_message = await openai_service.get_response(main_message)
     except ContextLengthException as e:
         statement_tokens = openai_service.get_token_count(statement)
         context_tokens = 0
         for context in context_list:
             context_tokens += openai_service.get_token_count(context)
@@ -387,26 +384,36 @@
             f"\nBase prompt tokens: {base_prompt_tokens}"
             f"\nTotal tokens: {total_tokens}"
         ) from e
 
     return response_message
 
 
-def statement_derived_from_context_prompt(main_message):
+def statement_derived_from_context_prompt(statement: str, context_list: List[str]):
     """
 
     Parameters
     ----------
-    main_message : The main message to which additional instructions will be added.
+    statement: str
+        The statement to be checked.
+    context_list: List[str]
+        List of retrieved context.
 
     Returns
     -------
     prompt message for determining if a statement can be derived from context.
 
     """
+    if not context_list:
+        context_list = ["EXAMPLE CONTEXT"]
+
+    main_message = "Considering the following statement and list of context(s)"
+    main_message += f"\n\nSTATEMENT:\n{statement}\nEND OF STATEMENT"
+    for i, context in enumerate(context_list):
+        main_message += f"\n\nCONTEXT {i}:\n{context}\nEND OF CONTEXT {i}"
     main_message += (
         "\n\nDetermine whether the listed statement above can be derived from the "
         "context listed above. If the statement can "
         "be derived from the context then you should respond with 'true'. Otherwise "
         "respond with 'false'. Your response must be either 'true' or 'false' with no "
         "additional text."
     )
```

### Comparing `tonic_validate-4.0.4/tonic_validate/utils/metrics_util.py` & `tonic_validate-4.0.5/tonic_validate/utils/metrics_util.py`

 * *Files identical despite different names*

### Comparing `tonic_validate-4.0.4/tonic_validate/utils/openai_cache.py` & `tonic_validate-4.0.5/tonic_validate/utils/openai_cache.py`

 * *Files identical despite different names*

### Comparing `tonic_validate-4.0.4/tonic_validate/utils/telemetry.py` & `tonic_validate-4.0.5/tonic_validate/utils/telemetry.py`

 * *Files 9% similar despite different names*

```diff
@@ -62,36 +62,47 @@
         Checks whether the current environment is a CI/CD environment
         """
         for var in env_vars:
             if os.environ.get(var):
                 return True
         return False
 
-    def log_run(self, num_of_questions: int, metrics: List[str]):
+    def log_run(self, num_of_questions: int, metrics: List[str], run_time: float):
         """
         Logs a run to the Tonic Validate server
 
         Parameters
         ----------
         num_of_questions: int
             The number of questions asked
         metrics: List[str]
             The metrics that were used to evaluate the run
+        run_time: float
+            The time taken to evaluate the run            
         """
         if self.config.TONIC_VALIDATE_DO_NOT_TRACK:
             return
+        try:
+            from importlib.metadata import version
+            sdk_version = version('tonic-validate')
+        except Exception:
+            sdk_version = "unknown"
+        
         user_id = self.get_user()["user_id"]
         self.http_client.http_post(
             "/runs",
             data={
                 "user_id": user_id,
                 "num_of_questions": num_of_questions,
                 "metrics": metrics,
+                "run_time": run_time,
+                "sdk_version": sdk_version,
                 "is_ci": self.__is_ci(),
                 "validate_gh_action": self.config.TONIC_VALIDATE_GITHUB_ACTION,
+                "backend": "validate"
             },
             timeout=5,
         )
 
     def log_benchmark(self, num_of_questions: int):
         """
         Logs a benchmark to the Tonic Validate server
@@ -107,14 +118,15 @@
         self.http_client.http_post(
             "/benchmarks",
             data={
                 "user_id": user_id,
                 "num_of_questions": num_of_questions,
                 "is_ci": self.__is_ci(),
                 "validate_gh_action": self.config.TONIC_VALIDATE_GITHUB_ACTION,
+                "backend": "validate"
             },
             timeout=5,
         )
 
     def link_user(self):
         """
         In the telemetry, links an API user to an SDK user. Used to filter out users that do not use the web application
```

### Comparing `tonic_validate-4.0.4/tonic_validate/validate_api.py` & `tonic_validate-4.0.5/tonic_validate/validate_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -52,14 +52,16 @@
             The run to upload.
         run_metadata : Optional[Dict[str, Any]]
             Metadata to attach to the run. If the values are not strings, then they are
             converted to strings before making the request.
         tags : Optional[List[str]]
             A list of tags which can be used to identify this run.  Tags will be rendered in the UI and can also make run searchable.
         """
+        if "llm_evaluator" not in run_metadata:
+            run_metadata["llm_evaluator"] = run.llm_evaluator
         run_response = self.client.http_post(
             f"/projects/{project_id}/runs/with_data",
             data={
                 "run_metadata": run_metadata,
                 "tags": tags,
                 "data": [run_data.to_dict() for run_data in run.run_data],
             },
```

### Comparing `tonic_validate-4.0.4/tonic_validate/validate_scorer.py` & `tonic_validate-4.0.5/tonic_validate/validate_scorer.py`

 * *Files 3% similar despite different names*

```diff
@@ -161,20 +161,18 @@
 
         Returns
         -------
         Run
             The Run object containing the scores and other data.
         """
         try:
-            self.telemetry.log_run(
-                len(responses), [metric.name for metric in self.metrics]
-            )
+            start_time = time.time()
         except Exception as _:
-            pass
-
+            start_time = -1
+        
         semaphore = Semaphore(parallelism)
         tasks = [
             self._score_item_rundata(response, semaphore) for response in responses
         ]
 
         run_data: List[RunData] = await async_tqdm.gather(
             *tasks,
@@ -192,16 +190,28 @@
                 if score is not None:
                     total_scores[metric_name] += score
                     num_scores[metric_name] += 1
 
         overall_scores: Dict[str, float] = {
             metric: total / num_scores[metric] for metric, total in total_scores.items()
         }
+        try:
+            end_time = time.time()
+            run_time = end_time - start_time
+        except Exception as _:
+            run_time = -1
+
+        try:
+            self.telemetry.log_run(
+                len(responses), [metric.name for metric in self.metrics], run_time
+            )
+        except Exception as _:
+            pass
 
-        return Run(overall_scores=overall_scores, run_data=run_data, id=None)
+        return Run(overall_scores=overall_scores, run_data=run_data, llm_evaluator=self.model_evaluator, id=None)
 
     @validate_call(config=ConfigDict(arbitrary_types_allowed=True))
     def score_responses(
         self,
         responses: List[LLMResponse],
         parallelism: int = DEFAULT_PARALLELISM_SCORING,
     ) -> Run:
```

### Comparing `tonic_validate-4.0.4/PKG-INFO` & `tonic_validate-4.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tonic-validate
-Version: 4.0.4
+Version: 4.0.5
 Summary: RAG evaluation metrics.
 Author: Joe Ferrara
 Author-email: joeferrara@tonic.ai
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -458,15 +458,17 @@
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 ### Telemetry
 Tonic Validate collects minimal telemetry to help us figure out what users want and how they're using the product. We do not use any existing telemetry framework and instead created our own privacy focused setup. Only the following information is tracked
 
 * What metrics were used for a run
 * Number of questions in a run
+* Time taken for a run to be evaluated
 * Number of questions in a benchmark
+* SDK Version being used
 
 We do **NOT** track things such as the contents of the questions / answers, your scores, or any other sensitive information. For detecting CI/CD, we only check for common environment variables in different CI/CD environments. We do not log the values of these environment variables.
 
 We also generate a random UUID to help us figure out how many users are using the product. This UUID is linked to your Validate account only to help track who is using the SDK and UI at once and to get user counts. If you want to see how we implemented telemetry, you can do so in the `tonic_validate/utils/telemetry.py` file
 
 If you wish to opt out of telemetry, you only need to set the `TONIC_VALIDATE_DO_NOT_TRACK` environment variable to `True`.
```

