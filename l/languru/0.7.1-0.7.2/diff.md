# Comparing `tmp/languru-0.7.1.tar.gz` & `tmp/languru-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "languru-0.7.1.tar", max compression
+gzip compressed data, was "languru-0.7.2.tar", max compression
```

## Comparing `languru-0.7.1.tar` & `languru-0.7.2.tar`

### file list

```diff
@@ -1,59 +1,62 @@
--rw-r--r--   0        0        0    11357 2024-02-01 11:42:52.861485 languru-0.7.1/LICENSE
--rw-r--r--   0        0        0    10182 2024-04-02 11:20:24.107511 languru-0.7.1/README.md
--rw-r--r--   0        0        0        0 2024-02-01 11:42:52.861665 languru-0.7.1/languru/__init__.py
--rw-r--r--   0        0        0        0 2024-02-07 02:51:29.580590 languru-0.7.1/languru/action/__init__.py
--rw-r--r--   0        0        0     4891 2024-03-11 03:18:17.774427 languru-0.7.1/languru/action/base.py
--rw-r--r--   0        0        0     7655 2024-03-19 05:31:55.754602 languru-0.7.1/languru/action/google.py
--rw-r--r--   0        0        0     2816 2024-03-27 09:02:07.247643 languru-0.7.1/languru/action/groq.py
--rw-r--r--   0        0        0    18777 2024-03-19 05:31:55.754961 languru-0.7.1/languru/action/hf.py
--rw-r--r--   0        0        0     7339 2024-03-27 09:02:07.248837 languru-0.7.1/languru/action/openai.py
--rw-r--r--   0        0        0     2999 2024-03-27 09:02:07.249387 languru-0.7.1/languru/action/pplx.py
--rw-r--r--   0        0        0     1105 2024-03-22 10:50:29.684729 languru-0.7.1/languru/action/utils.py
--rw-r--r--   0        0        0        0 2024-02-01 11:42:52.861745 languru-0.7.1/languru/cli/__init__.py
--rw-r--r--   0        0        0     3327 2024-03-22 10:21:59.204779 languru-0.7.1/languru/cli/main.py
--rw-r--r--   0        0        0      221 2024-02-07 08:19:21.426236 languru-0.7.1/languru/config.py
--rw-r--r--   0        0        0        0 2024-03-19 05:31:55.755531 languru-0.7.1/languru/examples/__init__.py
--rw-r--r--   0        0        0        0 2024-03-19 05:31:55.755648 languru-0.7.1/languru/examples/return_values/__init__.py
--rw-r--r--   0        0        0     9704 2024-03-19 05:31:55.755827 languru-0.7.1/languru/examples/return_values/_openai.py
--rw-r--r--   0        0        0       41 2024-02-15 01:55:28.093981 languru-0.7.1/languru/exceptions.py
--rw-r--r--   0        0        0        0 2024-02-07 02:51:29.582508 languru-0.7.1/languru/resources/__init__.py
--rw-r--r--   0        0        0        0 2024-02-07 02:51:29.582657 languru-0.7.1/languru/resources/llm/__init__.py
--rw-r--r--   0        0        0        0 2024-02-07 02:51:29.582788 languru-0.7.1/languru/resources/model/__init__.py
--rw-r--r--   0        0        0     4394 2024-03-09 09:50:32.758650 languru-0.7.1/languru/resources/model/discovery.py
--rw-r--r--   0        0        0        0 2024-02-01 11:42:52.861878 languru-0.7.1/languru/server/__init__.py
--rw-r--r--   0        0        0        0 2024-02-02 02:00:42.777707 languru-0.7.1/languru/server/api/__init__.py
--rw-r--r--   0        0        0      729 2024-02-15 01:55:28.095262 languru-0.7.1/languru/server/api/v1/__init__.py
--rw-r--r--   0        0        0     7533 2024-03-27 09:02:07.250510 languru-0.7.1/languru/server/api/v1/chat.py
--rw-r--r--   0        0        0     5796 2024-03-22 10:07:39.202848 languru-0.7.1/languru/server/api/v1/completions.py
--rw-r--r--   0        0        0     4423 2024-03-22 10:07:39.203160 languru-0.7.1/languru/server/api/v1/embeddings.py
--rw-r--r--   0        0        0     9679 2024-03-19 05:31:55.756461 languru-0.7.1/languru/server/api/v1/model.py
--rw-r--r--   0        0        0     4353 2024-03-22 10:07:39.203389 languru-0.7.1/languru/server/api/v1/moderations.py
--rw-r--r--   0        0        0     5020 2024-03-19 05:31:55.756725 languru-0.7.1/languru/server/api/v1/test_chat.py
--rw-r--r--   0        0        0     4807 2024-03-19 05:31:55.756818 languru-0.7.1/languru/server/api/v1/test_completions.py
--rw-r--r--   0        0        0     2475 2024-03-19 05:31:55.756905 languru-0.7.1/languru/server/api/v1/test_embeddings.py
--rw-r--r--   0        0        0     3501 2024-03-19 05:31:55.757121 languru-0.7.1/languru/server/api/v1/test_model.py
--rw-r--r--   0        0        0     2263 2024-03-19 05:31:55.757219 languru-0.7.1/languru/server/api/v1/test_moderations.py
--rw-r--r--   0        0        0     6958 2024-03-27 09:02:07.250950 languru-0.7.1/languru/server/config.py
--rw-r--r--   0        0        0        0 2024-03-19 05:31:55.757554 languru-0.7.1/languru/server/deps/__init__.py
--rw-r--r--   0        0        0      429 2024-03-19 05:31:55.757647 languru-0.7.1/languru/server/deps/common.py
--rw-r--r--   0        0        0     5166 2024-03-19 05:31:55.757727 languru-0.7.1/languru/server/main.py
--rw-r--r--   0        0        0        0 2024-03-19 05:31:55.757760 languru-0.7.1/languru/server/utils/__init__.py
--rw-r--r--   0        0        0     1270 2024-03-19 05:31:55.758226 languru-0.7.1/languru/server/utils/common.py
--rw-r--r--   0        0        0        0 2024-02-07 02:51:29.585801 languru-0.7.1/languru/types/__init__.py
--rw-r--r--   0        0        0        0 2024-02-07 02:51:29.585941 languru-0.7.1/languru/types/chat/__init__.py
--rw-r--r--   0        0        0     2777 2024-02-07 07:57:15.543854 languru-0.7.1/languru/types/chat/completions.py
--rw-r--r--   0        0        0     2895 2024-03-19 05:31:55.758398 languru-0.7.1/languru/types/completions.py
--rw-r--r--   0        0        0      603 2024-02-15 01:55:28.096416 languru-0.7.1/languru/types/embeddings.py
--rw-r--r--   0        0        0      158 2024-02-07 06:54:11.803747 languru-0.7.1/languru/types/model/__init__.py
--rw-r--r--   0        0        0      454 2024-02-07 07:01:30.525620 languru-0.7.1/languru/types/model/orm.py
--rw-r--r--   0        0        0      403 2024-02-15 01:55:28.096482 languru-0.7.1/languru/types/moderations.py
--rw-r--r--   0        0        0        0 2024-02-15 01:55:28.096547 languru-0.7.1/languru/utils/__init__.py
--rw-r--r--   0        0        0     1622 2024-02-18 04:18:45.843584 languru-0.7.1/languru/utils/calculation.py
--rw-r--r--   0        0        0     2405 2024-03-11 03:18:17.778514 languru-0.7.1/languru/utils/common.py
--rw-r--r--   0        0        0     2328 2024-03-08 08:14:03.711878 languru-0.7.1/languru/utils/device.py
--rw-r--r--   0        0        0     3213 2024-03-11 03:18:17.779132 languru-0.7.1/languru/utils/hf.py
--rw-r--r--   0        0        0     1666 2024-03-19 05:31:55.758527 languru-0.7.1/languru/utils/http.py
--rw-r--r--   0        0        0     1163 2024-02-15 01:55:28.096890 languru-0.7.1/languru/utils/socket.py
--rw-r--r--   0        0        0       63 2024-04-02 11:48:22.742986 languru-0.7.1/languru/version.py
--rw-r--r--   0        0        0     4296 2024-04-02 11:48:13.512193 languru-0.7.1/pyproject.toml
--rw-r--r--   0        0        0    13024 1970-01-01 00:00:00.000000 languru-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-01-29 14:01:08.176794 languru-0.7.2/LICENSE
+-rw-r--r--   0        0        0    10182 2024-04-01 13:52:42.969386 languru-0.7.2/README.md
+-rw-r--r--   0        0        0        0 2024-01-29 14:05:50.312326 languru-0.7.2/languru/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-05 13:57:47.271478 languru-0.7.2/languru/action/__init__.py
+-rw-r--r--   0        0        0     8883 2024-04-06 08:43:25.015213 languru-0.7.2/languru/action/anthropic.py
+-rw-r--r--   0        0        0     4891 2024-03-26 14:02:44.545868 languru-0.7.2/languru/action/base.py
+-rw-r--r--   0        0        0     7655 2024-03-26 14:02:44.546930 languru-0.7.2/languru/action/google.py
+-rw-r--r--   0        0        0     2816 2024-03-26 14:02:44.547223 languru-0.7.2/languru/action/groq.py
+-rw-r--r--   0        0        0    18777 2024-03-26 14:02:44.547591 languru-0.7.2/languru/action/hf.py
+-rw-r--r--   0        0        0     7339 2024-03-26 14:02:44.548675 languru-0.7.2/languru/action/openai.py
+-rw-r--r--   0        0        0     2999 2024-03-26 14:02:44.549070 languru-0.7.2/languru/action/pplx.py
+-rw-r--r--   0        0        0     1105 2024-03-26 14:02:44.549471 languru-0.7.2/languru/action/utils.py
+-rw-r--r--   0        0        0        0 2024-01-30 14:23:22.088837 languru-0.7.2/languru/cli/__init__.py
+-rw-r--r--   0        0        0     3327 2024-03-26 14:02:44.549872 languru-0.7.2/languru/cli/main.py
+-rw-r--r--   0        0        0      221 2024-03-03 04:51:38.853780 languru-0.7.2/languru/config.py
+-rw-r--r--   0        0        0        0 2024-03-26 14:02:44.549916 languru-0.7.2/languru/examples/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-26 14:02:44.550015 languru-0.7.2/languru/examples/return_values/__init__.py
+-rw-r--r--   0        0        0     9704 2024-03-26 14:02:44.550369 languru-0.7.2/languru/examples/return_values/_openai.py
+-rw-r--r--   0        0        0       41 2024-02-10 12:12:53.654103 languru-0.7.2/languru/exceptions.py
+-rw-r--r--   0        0        0        0 2024-02-03 10:10:03.421778 languru-0.7.2/languru/resources/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-03 10:19:09.963208 languru-0.7.2/languru/resources/llm/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-03 10:18:35.609130 languru-0.7.2/languru/resources/model/__init__.py
+-rw-r--r--   0        0        0     4394 2024-03-26 14:02:44.551182 languru-0.7.2/languru/resources/model/discovery.py
+-rw-r--r--   0        0        0        0 2024-01-29 14:28:54.637050 languru-0.7.2/languru/server/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-01 14:35:12.034189 languru-0.7.2/languru/server/api/__init__.py
+-rw-r--r--   0        0        0      729 2024-02-10 12:03:18.878712 languru-0.7.2/languru/server/api/v1/__init__.py
+-rw-r--r--   0        0        0     7533 2024-03-26 14:02:44.552014 languru-0.7.2/languru/server/api/v1/chat.py
+-rw-r--r--   0        0        0     5796 2024-03-26 14:02:44.552963 languru-0.7.2/languru/server/api/v1/completions.py
+-rw-r--r--   0        0        0     4423 2024-03-26 14:02:44.553833 languru-0.7.2/languru/server/api/v1/embeddings.py
+-rw-r--r--   0        0        0     9679 2024-03-26 14:02:44.554362 languru-0.7.2/languru/server/api/v1/model.py
+-rw-r--r--   0        0        0     4353 2024-03-26 14:02:44.555146 languru-0.7.2/languru/server/api/v1/moderations.py
+-rw-r--r--   0        0        0     5020 2024-03-26 14:02:44.555947 languru-0.7.2/languru/server/api/v1/test_chat.py
+-rw-r--r--   0        0        0     4807 2024-03-26 14:02:44.556765 languru-0.7.2/languru/server/api/v1/test_completions.py
+-rw-r--r--   0        0        0     2475 2024-03-26 14:02:44.557059 languru-0.7.2/languru/server/api/v1/test_embeddings.py
+-rw-r--r--   0        0        0     3501 2024-03-26 14:02:44.557249 languru-0.7.2/languru/server/api/v1/test_model.py
+-rw-r--r--   0        0        0     2263 2024-03-26 14:02:44.557524 languru-0.7.2/languru/server/api/v1/test_moderations.py
+-rw-r--r--   0        0        0     6958 2024-03-26 14:02:44.558328 languru-0.7.2/languru/server/config.py
+-rw-r--r--   0        0        0        0 2024-03-26 14:02:44.558372 languru-0.7.2/languru/server/deps/__init__.py
+-rw-r--r--   0        0        0      429 2024-03-26 14:02:44.558691 languru-0.7.2/languru/server/deps/common.py
+-rw-r--r--   0        0        0     5166 2024-03-26 14:02:44.559416 languru-0.7.2/languru/server/main.py
+-rw-r--r--   0        0        0        0 2024-03-26 14:02:44.559457 languru-0.7.2/languru/server/utils/__init__.py
+-rw-r--r--   0        0        0     1270 2024-03-26 14:02:44.559762 languru-0.7.2/languru/server/utils/common.py
+-rw-r--r--   0        0        0        0 2024-02-03 08:58:36.094265 languru-0.7.2/languru/types/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-03 08:59:16.654501 languru-0.7.2/languru/types/chat/__init__.py
+-rw-r--r--   0        0        0     2059 2024-04-06 07:12:32.577046 languru-0.7.2/languru/types/chat/anthropic.py
+-rw-r--r--   0        0        0     3094 2024-04-06 05:54:42.711490 languru-0.7.2/languru/types/chat/completions.py
+-rw-r--r--   0        0        0     2895 2024-03-26 14:02:44.560212 languru-0.7.2/languru/types/completions.py
+-rw-r--r--   0        0        0      603 2024-02-09 09:22:56.989013 languru-0.7.2/languru/types/embeddings.py
+-rw-r--r--   0        0        0      158 2024-02-07 11:22:07.653430 languru-0.7.2/languru/types/model/__init__.py
+-rw-r--r--   0        0        0      454 2024-02-07 11:22:07.653586 languru-0.7.2/languru/types/model/orm.py
+-rw-r--r--   0        0        0      403 2024-02-10 12:09:30.949805 languru-0.7.2/languru/types/moderations.py
+-rw-r--r--   0        0        0        0 2024-02-13 08:54:51.563321 languru-0.7.2/languru/utils/__init__.py
+-rw-r--r--   0        0        0     1622 2024-02-18 07:12:00.382248 languru-0.7.2/languru/utils/calculation.py
+-rw-r--r--   0        0        0     2405 2024-03-26 14:02:44.560637 languru-0.7.2/languru/utils/common.py
+-rw-r--r--   0        0        0     2328 2024-03-06 14:06:53.434085 languru-0.7.2/languru/utils/device.py
+-rw-r--r--   0        0        0     3213 2024-03-26 14:02:44.560917 languru-0.7.2/languru/utils/hf.py
+-rw-r--r--   0        0        0     1666 2024-03-26 14:02:44.561210 languru-0.7.2/languru/utils/http.py
+-rw-r--r--   0        0        0     1163 2024-02-13 12:38:09.199703 languru-0.7.2/languru/utils/socket.py
+-rw-r--r--   0        0        0     2854 2024-04-06 04:19:40.336504 languru-0.7.2/languru/utils/xml.py
+-rw-r--r--   0        0        0       63 2024-04-06 09:02:26.600055 languru-0.7.2/languru/version.py
+-rw-r--r--   0        0        0     4387 2024-04-06 09:02:19.808133 languru-0.7.2/pyproject.toml
+-rw-r--r--   0        0        0    13127 1970-01-01 00:00:00.000000 languru-0.7.2/PKG-INFO
```

### Comparing `languru-0.7.1/LICENSE` & `languru-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `languru-0.7.1/README.md` & `languru-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `languru-0.7.1/languru/action/base.py` & `languru-0.7.2/languru/action/base.py`

 * *Files identical despite different names*

### Comparing `languru-0.7.1/languru/action/google.py` & `languru-0.7.2/languru/action/google.py`

 * *Files identical despite different names*

### Comparing `languru-0.7.1/languru/action/groq.py` & `languru-0.7.2/languru/action/groq.py`

 * *Files identical despite different names*

### Comparing `languru-0.7.1/languru/action/hf.py` & `languru-0.7.2/languru/action/hf.py`

 * *Files identical despite different names*

### Comparing `languru-0.7.1/languru/action/openai.py` & `languru-0.7.2/languru/action/openai.py`

 * *Files identical despite different names*

### Comparing `languru-0.7.1/languru/action/pplx.py` & `languru-0.7.2/languru/action/pplx.py`

 * *Files identical despite different names*

### Comparing `languru-0.7.1/languru/action/utils.py` & `languru-0.7.2/languru/action/utils.py`

 * *Files identical despite different names*

### Comparing `languru-0.7.1/languru/cli/main.py` & `languru-0.7.2/languru/cli/main.py`

 * *Files identical despite different names*

### Comparing `languru-0.7.1/languru/examples/return_values/_openai.py` & `languru-0.7.2/languru/examples/return_values/_openai.py`

 * *Files identical despite different names*

### Comparing `languru-0.7.1/languru/resources/model/discovery.py` & `languru-0.7.2/languru/resources/model/discovery.py`

 * *Files identical despite different names*

### Comparing `languru-0.7.1/languru/server/api/v1/__init__.py` & `languru-0.7.2/languru/server/api/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `languru-0.7.1/languru/server/api/v1/chat.py` & `languru-0.7.2/languru/server/api/v1/chat.py`

 * *Files identical despite different names*

### Comparing `languru-0.7.1/languru/server/api/v1/completions.py` & `languru-0.7.2/languru/server/api/v1/completions.py`

 * *Files identical despite different names*

### Comparing `languru-0.7.1/languru/server/api/v1/embeddings.py` & `languru-0.7.2/languru/server/api/v1/embeddings.py`

 * *Files identical despite different names*

### Comparing `languru-0.7.1/languru/server/api/v1/model.py` & `languru-0.7.2/languru/server/api/v1/model.py`

 * *Files identical despite different names*

### Comparing `languru-0.7.1/languru/server/api/v1/moderations.py` & `languru-0.7.2/languru/server/api/v1/moderations.py`

 * *Files identical despite different names*

### Comparing `languru-0.7.1/languru/server/api/v1/test_chat.py` & `languru-0.7.2/languru/server/api/v1/test_chat.py`

 * *Files identical despite different names*

### Comparing `languru-0.7.1/languru/server/api/v1/test_completions.py` & `languru-0.7.2/languru/server/api/v1/test_completions.py`

 * *Files identical despite different names*

### Comparing `languru-0.7.1/languru/server/api/v1/test_embeddings.py` & `languru-0.7.2/languru/server/api/v1/test_embeddings.py`

 * *Files identical despite different names*

### Comparing `languru-0.7.1/languru/server/api/v1/test_model.py` & `languru-0.7.2/languru/server/api/v1/test_model.py`

 * *Files identical despite different names*

### Comparing `languru-0.7.1/languru/server/api/v1/test_moderations.py` & `languru-0.7.2/languru/server/api/v1/test_moderations.py`

 * *Files identical despite different names*

### Comparing `languru-0.7.1/languru/server/config.py` & `languru-0.7.2/languru/server/config.py`

 * *Files identical despite different names*

### Comparing `languru-0.7.1/languru/server/main.py` & `languru-0.7.2/languru/server/main.py`

 * *Files identical despite different names*

### Comparing `languru-0.7.1/languru/server/utils/common.py` & `languru-0.7.2/languru/server/utils/common.py`

 * *Files identical despite different names*

### Comparing `languru-0.7.1/languru/types/chat/completions.py` & `languru-0.7.2/languru/types/chat/completions.py`

 * *Files 11% similar despite different names*

```diff
@@ -71,7 +71,15 @@
     )
     tool_choice: Optional[Union[Text, FunctionChoice]] = Field(
         None, description="Controls which function is called by the model"
     )
     user: Optional[Text] = Field(
         None, description="A unique identifier representing your end-user"
     )
+
+    @classmethod
+    def from_kwargs(cls, **kwargs) -> "ChatCompletionRequest":
+        if "messages" not in kwargs:
+            raise ValueError("Parameter messages is required")
+        if "model" not in kwargs:
+            raise ValueError("Parameter model is required")
+        return cls.model_validate(kwargs)
```

### Comparing `languru-0.7.1/languru/types/completions.py` & `languru-0.7.2/languru/types/completions.py`

 * *Files identical despite different names*

### Comparing `languru-0.7.1/languru/types/embeddings.py` & `languru-0.7.2/languru/types/embeddings.py`

 * *Files identical despite different names*

### Comparing `languru-0.7.1/languru/utils/calculation.py` & `languru-0.7.2/languru/utils/calculation.py`

 * *Files identical despite different names*

### Comparing `languru-0.7.1/languru/utils/common.py` & `languru-0.7.2/languru/utils/common.py`

 * *Files identical despite different names*

### Comparing `languru-0.7.1/languru/utils/device.py` & `languru-0.7.2/languru/utils/device.py`

 * *Files identical despite different names*

### Comparing `languru-0.7.1/languru/utils/hf.py` & `languru-0.7.2/languru/utils/hf.py`

 * *Files identical despite different names*

### Comparing `languru-0.7.1/languru/utils/http.py` & `languru-0.7.2/languru/utils/http.py`

 * *Files identical despite different names*

### Comparing `languru-0.7.1/languru/utils/socket.py` & `languru-0.7.2/languru/utils/socket.py`

 * *Files identical despite different names*

### Comparing `languru-0.7.1/pyproject.toml` & `languru-0.7.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -3,19 +3,20 @@
 description = "The general purpose LLM app stacks."
 documentation = "https://dockhardman.github.io/languru/"
 homepage = "https://github.com/dockhardman/languru"
 license = "Apache-2.0 license"
 name = "languru"
 readme = "README.md"
 repository = "https://github.com/dockhardman/languru"
-version = "0.7.1"
+version = "0.7.2"
 
 [tool.poetry.dependencies]
 accelerate = { version = "^0.27.2", optional = true, markers = "sys_platform == 'linux'" }
 aiohttp = "^3.9.3"
+anthropic = {version = "<1,>0.21", optional = true}
 bitsandbytes = { version = "^0.42", optional = true, markers = "sys_platform == 'linux'" }
 click = "^8.1.7"
 colorama = "^0.4.6"
 einops = { version = "^0.7.0", optional = true }
 fastapi = { extras = ["all"], version = "^0.109.0", optional = true }
 flash-attn = { version = "^2", optional = true, markers = "sys_platform == 'linux'" }
 google-cloud-aiplatform = { version = "^1.38", optional = true }
@@ -40,15 +41,16 @@
 transformers = { extras = ["torch"], version = "^4.37.2", optional = true }
 typing-extensions = "^4.9.0"
 
 [tool.poetry.scripts]
 languru = "languru.cli.main:app"
 
 [tool.poetry.extras]
-all = ["einops", "fastapi", "google-cloud-aiplatform", "google-generativeai", "groq", "huggingface", "ninja", "nvgpu", "sentencepiece", "torch", "torchaudio", "torchvision", "transformers"]
+all = ["anthropic", "einops", "fastapi", "google-cloud-aiplatform", "google-generativeai", "groq", "huggingface", "ninja", "nvgpu", "sentencepiece", "torch", "torchaudio", "torchvision", "transformers"]
+anthropic = ["anthropic"]
 cuda = ["accelerate", "bitsandbytes", "flash-attn", "nvgpu"]
 google = ["google-cloud-aiplatform", "google-generativeai"]
 groq = ["groq"]
 huggingface = ["einops", "ninja", "nvgpu", "sentencepiece", "torch", "torchaudio", "torchvision", "transformers"]
 huggingface_cpu = ["transformers"]
 server = ["fastapi"]
 torch = ["torch", "torchaudio", "torchvision"]
```

### Comparing `languru-0.7.1/PKG-INFO` & `languru-0.7.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 Metadata-Version: 2.1
 Name: languru
-Version: 0.7.1
+Version: 0.7.2
 Summary: The general purpose LLM app stacks.
 Home-page: https://github.com/dockhardman/languru
 License: Apache-2.0 license
 Author: Allen Chou
 Author-email: f1470891079@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: all
+Provides-Extra: anthropic
 Provides-Extra: cuda
 Provides-Extra: google
 Provides-Extra: groq
 Provides-Extra: huggingface
 Provides-Extra: huggingface-cpu
 Provides-Extra: server
 Provides-Extra: torch
 Requires-Dist: accelerate (>=0.27.2,<0.28.0) ; (sys_platform == "linux") and (extra == "cuda")
 Requires-Dist: aiohttp (>=3.9.3,<4.0.0)
+Requires-Dist: anthropic (>0.21,<1) ; extra == "all" or extra == "anthropic"
 Requires-Dist: bitsandbytes (>=0.42,<0.43) ; (sys_platform == "linux") and (extra == "cuda")
 Requires-Dist: click (>=8.1.7,<9.0.0)
 Requires-Dist: colorama (>=0.4.6,<0.5.0)
 Requires-Dist: einops (>=0.7.0,<0.8.0) ; extra == "all" or extra == "huggingface"
 Requires-Dist: fastapi[all] (>=0.109.0,<0.110.0) ; extra == "all" or extra == "server"
 Requires-Dist: flash-attn (>=2,<3) ; (sys_platform == "linux") and (extra == "cuda")
 Requires-Dist: google-cloud-aiplatform (>=1.38,<2.0) ; extra == "all" or extra == "google"
```

