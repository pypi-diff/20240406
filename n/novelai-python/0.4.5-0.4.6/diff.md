# Comparing `tmp/novelai_python-0.4.5.tar.gz` & `tmp/novelai_python-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "novelai_python-0.4.5.tar", last modified: Sun Mar 31 10:54:11 2024, max compression
+gzip compressed data, was "novelai_python-0.4.6.tar", last modified: Sat Apr  6 06:10:41 2024, max compression
```

## Comparing `novelai_python-0.4.5.tar` & `novelai_python-0.4.6.tar`

### file list

```diff
@@ -1,62 +1,62 @@
--rwxr-xr-x   0        0        0    11357 2024-03-31 10:53:59.654272 novelai_python-0.4.5/LICENSE
--rwxr-xr-x   0        0        0      522 2024-03-31 10:53:59.654272 novelai_python-0.4.5/NOTICE.MD
--rwxr-xr-x   0        0        0     2852 2024-03-31 10:53:59.654272 novelai_python-0.4.5/README.md
--rw-r--r--   0        0        0     1131 2024-03-31 10:54:11.958332 novelai_python-0.4.5/pyproject.toml
--rwxr-xr-x   0        0        0     1101 2024-03-31 10:53:59.670272 novelai_python-0.4.5/src/novelai_python/__init__.py
--rwxr-xr-x   0        0        0     1761 2024-03-31 10:53:59.670272 novelai_python-0.4.5/src/novelai_python/_exceptions.py
--rwxr-xr-x   0        0        0      410 2024-03-31 10:53:59.670272 novelai_python-0.4.5/src/novelai_python/_response/__init__.py
--rwxr-xr-x   0        0        0      127 2024-03-31 10:53:59.670272 novelai_python-0.4.5/src/novelai_python/_response/ai/__init__.py
--rwxr-xr-x   0        0        0      828 2024-03-31 10:53:59.670272 novelai_python-0.4.5/src/novelai_python/_response/ai/generate_image.py
--rw-r--r--   0        0        0      185 2024-03-31 10:53:59.670272 novelai_python-0.4.5/src/novelai_python/_response/ai/generate_voice.py
--rwxr-xr-x   0        0        0      397 2024-03-31 10:53:59.670272 novelai_python-0.4.5/src/novelai_python/_response/ai/upscale.py
--rwxr-xr-x   0        0        0      195 2024-03-31 10:53:59.670272 novelai_python-0.4.5/src/novelai_python/_response/schema.py
--rwxr-xr-x   0        0        0      128 2024-03-31 10:53:59.670272 novelai_python-0.4.5/src/novelai_python/_response/user/__init__.py
--rwxr-xr-x   0        0        0      721 2024-03-31 10:53:59.670272 novelai_python-0.4.5/src/novelai_python/_response/user/information.py
--rwxr-xr-x   0        0        0      204 2024-03-31 10:53:59.670272 novelai_python-0.4.5/src/novelai_python/_response/user/login.py
--rwxr-xr-x   0        0        0     2359 2024-03-31 10:53:59.670272 novelai_python-0.4.5/src/novelai_python/_response/user/subscription.py
--rwxr-xr-x   0        0        0     1548 2024-03-31 10:53:59.670272 novelai_python-0.4.5/src/novelai_python/credential/ApiToken.py
--rwxr-xr-x   0        0        0     1628 2024-03-31 10:53:59.670272 novelai_python-0.4.5/src/novelai_python/credential/JwtToken.py
--rwxr-xr-x   0        0        0     1701 2024-03-31 10:53:59.670272 novelai_python-0.4.5/src/novelai_python/credential/UserAuth.py
--rwxr-xr-x   0        0        0      424 2024-03-31 10:53:59.670272 novelai_python-0.4.5/src/novelai_python/credential/__init__.py
--rwxr-xr-x   0        0        0      462 2024-03-31 10:53:59.670272 novelai_python-0.4.5/src/novelai_python/credential/_base.py
--rwxr-xr-x   0        0        0      624 2024-03-31 10:53:59.670272 novelai_python-0.4.5/src/novelai_python/sdk/__init__.py
--rwxr-xr-x   0        0        0     1082 2024-03-31 10:53:59.670272 novelai_python-0.4.5/src/novelai_python/sdk/ai/LICENSE
--rwxr-xr-x   0        0        0      130 2024-03-31 10:53:59.670272 novelai_python-0.4.5/src/novelai_python/sdk/ai/__init__.py
--rw-r--r--   0        0        0     2008 2024-03-31 10:53:59.670272 novelai_python-0.4.5/src/novelai_python/sdk/ai/_enum.py
--rwxr-xr-x   0        0        0    31111 2024-03-31 10:53:59.670272 novelai_python-0.4.5/src/novelai_python/sdk/ai/generate_image/__init__.py
--rw-r--r--   0        0        0    52850 2024-03-31 10:53:59.670272 novelai_python-0.4.5/src/novelai_python/sdk/ai/generate_image/_const.py
--rwxr-xr-x   0        0        0     3578 2024-03-31 10:53:59.670272 novelai_python-0.4.5/src/novelai_python/sdk/ai/generate_image/_enum.py
--rwxr-xr-x   0        0        0     5306 2024-03-31 10:53:59.670272 novelai_python-0.4.5/src/novelai_python/sdk/ai/generate_image/suggest_tags.py
--rw-r--r--   0        0        0     7495 2024-03-31 10:53:59.670272 novelai_python-0.4.5/src/novelai_python/sdk/ai/generate_voice.py
--rwxr-xr-x   0        0        0     8223 2024-03-31 10:53:59.670272 novelai_python-0.4.5/src/novelai_python/sdk/ai/upscale.py
--rwxr-xr-x   0        0        0      945 2024-03-31 10:53:59.670272 novelai_python-0.4.5/src/novelai_python/sdk/schema.py
--rwxr-xr-x   0        0        0      130 2024-03-31 10:53:59.670272 novelai_python-0.4.5/src/novelai_python/sdk/user/__init__.py
--rwxr-xr-x   0        0        0     4772 2024-03-31 10:53:59.670272 novelai_python-0.4.5/src/novelai_python/sdk/user/information.py
--rwxr-xr-x   0        0        0     5285 2024-03-31 10:53:59.670272 novelai_python-0.4.5/src/novelai_python/sdk/user/login.py
--rwxr-xr-x   0        0        0     5045 2024-03-31 10:53:59.670272 novelai_python-0.4.5/src/novelai_python/sdk/user/subscription.py
--rwxr-xr-x   0        0        0     5211 2024-03-31 10:53:59.670272 novelai_python-0.4.5/src/novelai_python/server.py
--rw-r--r--   0        0        0     1075 2024-03-31 10:53:59.670272 novelai_python-0.4.5/src/novelai_python/tokenizer/__init__.py
--rw-r--r--   0        0        0  1033724 2024-03-31 10:53:59.674272 novelai_python-0.4.5/src/novelai_python/tokenizer/novelai.model
--rw-r--r--   0        0        0  1033744 2024-03-31 10:53:59.682272 novelai_python-0.4.5/src/novelai_python/tokenizer/novelai_v2.model
--rw-r--r--   0        0        0       24 2024-03-31 10:53:59.682272 novelai_python-0.4.5/src/novelai_python/tool/__init__.py
--rw-r--r--   0        0        0     7948 2024-03-31 10:53:59.682272 novelai_python-0.4.5/src/novelai_python/tool/image_metadata/__init__.py
--rw-r--r--   0        0        0     3316 2024-03-31 10:53:59.682272 novelai_python-0.4.5/src/novelai_python/tool/image_metadata/lsb_extractor.py
--rw-r--r--   0        0        0     2211 2024-03-31 10:53:59.682272 novelai_python-0.4.5/src/novelai_python/tool/image_metadata/lsb_injector.py
--rw-r--r--   0        0        0     3181 2024-03-31 10:53:59.682272 novelai_python-0.4.5/src/novelai_python/tool/paint_mask/__init__.py
--rw-r--r--   0        0        0    17162 2024-03-31 10:53:59.682272 novelai_python-0.4.5/src/novelai_python/tool/random_prompt/__init__.py
--rw-r--r--   0        0        0    84988 2024-03-31 10:53:59.682272 novelai_python-0.4.5/src/novelai_python/tool/random_prompt/tag.py
--rw-r--r--   0        0        0    21015 2024-03-31 10:53:59.682272 novelai_python-0.4.5/src/novelai_python/tool/random_prompt/tag_character.py
--rw-r--r--   0        0        0    15814 2024-03-31 10:53:59.682272 novelai_python-0.4.5/src/novelai_python/tool/random_prompt/tag_nsfw.py
--rwxr-xr-x   0        0        0      533 2024-03-31 10:53:59.682272 novelai_python-0.4.5/src/novelai_python/utils/__init__.py
--rwxr-xr-x   0        0        0     1881 2024-03-31 10:53:59.682272 novelai_python-0.4.5/src/novelai_python/utils/encode.py
--rwxr-xr-x   0        0        0     1243 2024-03-31 10:53:59.682272 novelai_python-0.4.5/src/novelai_python/utils/useful.py
--rwxr-xr-x   0        0        0        0 2024-03-31 10:53:59.682272 novelai_python-0.4.5/tests/__init__.py
--rw-r--r--   0        0        0      870 2024-03-31 10:53:59.682272 novelai_python-0.4.5/tests/test_generate_voice.py
--rwxr-xr-x   0        0        0     2273 2024-03-31 10:53:59.682272 novelai_python-0.4.5/tests/test_random_prompt.py
--rwxr-xr-x   0        0        0      422 2024-03-31 10:53:59.682272 novelai_python-0.4.5/tests/test_server.py
--rwxr-xr-x   0        0        0     1375 2024-03-31 10:53:59.682272 novelai_python-0.4.5/tests/test_server_run.py
--rwxr-xr-x   0        0        0     2772 2024-03-31 10:53:59.682272 novelai_python-0.4.5/tests/test_upscale.py
--rwxr-xr-x   0        0        0     2592 2024-03-31 10:53:59.682272 novelai_python-0.4.5/tests/test_user_information.py
--rwxr-xr-x   0        0        0     3244 2024-03-31 10:53:59.682272 novelai_python-0.4.5/tests/test_user_login.py
--rwxr-xr-x   0        0        0     3270 2024-03-31 10:53:59.682272 novelai_python-0.4.5/tests/test_user_subscription.py
--rw-r--r--   0        0        0     3931 1970-01-01 00:00:00.000000 novelai_python-0.4.5/PKG-INFO
+-rwxr-xr-x   0        0        0    11357 2024-04-06 06:10:20.329774 novelai_python-0.4.6/LICENSE
+-rwxr-xr-x   0        0        0      522 2024-04-06 06:10:20.329774 novelai_python-0.4.6/NOTICE.MD
+-rwxr-xr-x   0        0        0     2854 2024-04-06 06:10:20.329774 novelai_python-0.4.6/README.md
+-rw-r--r--   0        0        0     1131 2024-04-06 06:10:41.165893 novelai_python-0.4.6/pyproject.toml
+-rwxr-xr-x   0        0        0     1101 2024-04-06 06:10:20.345774 novelai_python-0.4.6/src/novelai_python/__init__.py
+-rwxr-xr-x   0        0        0     1761 2024-04-06 06:10:20.345774 novelai_python-0.4.6/src/novelai_python/_exceptions.py
+-rwxr-xr-x   0        0        0      410 2024-04-06 06:10:20.345774 novelai_python-0.4.6/src/novelai_python/_response/__init__.py
+-rwxr-xr-x   0        0        0      127 2024-04-06 06:10:20.345774 novelai_python-0.4.6/src/novelai_python/_response/ai/__init__.py
+-rwxr-xr-x   0        0        0      828 2024-04-06 06:10:20.345774 novelai_python-0.4.6/src/novelai_python/_response/ai/generate_image.py
+-rw-r--r--   0        0        0      185 2024-04-06 06:10:20.345774 novelai_python-0.4.6/src/novelai_python/_response/ai/generate_voice.py
+-rwxr-xr-x   0        0        0      397 2024-04-06 06:10:20.345774 novelai_python-0.4.6/src/novelai_python/_response/ai/upscale.py
+-rwxr-xr-x   0        0        0      195 2024-04-06 06:10:20.345774 novelai_python-0.4.6/src/novelai_python/_response/schema.py
+-rwxr-xr-x   0        0        0      128 2024-04-06 06:10:20.345774 novelai_python-0.4.6/src/novelai_python/_response/user/__init__.py
+-rwxr-xr-x   0        0        0      721 2024-04-06 06:10:20.345774 novelai_python-0.4.6/src/novelai_python/_response/user/information.py
+-rwxr-xr-x   0        0        0      204 2024-04-06 06:10:20.345774 novelai_python-0.4.6/src/novelai_python/_response/user/login.py
+-rwxr-xr-x   0        0        0     2359 2024-04-06 06:10:20.345774 novelai_python-0.4.6/src/novelai_python/_response/user/subscription.py
+-rwxr-xr-x   0        0        0     1548 2024-04-06 06:10:20.345774 novelai_python-0.4.6/src/novelai_python/credential/ApiToken.py
+-rwxr-xr-x   0        0        0     1628 2024-04-06 06:10:20.345774 novelai_python-0.4.6/src/novelai_python/credential/JwtToken.py
+-rwxr-xr-x   0        0        0     1701 2024-04-06 06:10:20.345774 novelai_python-0.4.6/src/novelai_python/credential/UserAuth.py
+-rwxr-xr-x   0        0        0      424 2024-04-06 06:10:20.345774 novelai_python-0.4.6/src/novelai_python/credential/__init__.py
+-rwxr-xr-x   0        0        0      462 2024-04-06 06:10:20.345774 novelai_python-0.4.6/src/novelai_python/credential/_base.py
+-rwxr-xr-x   0        0        0      624 2024-04-06 06:10:20.345774 novelai_python-0.4.6/src/novelai_python/sdk/__init__.py
+-rwxr-xr-x   0        0        0     1082 2024-04-06 06:10:20.345774 novelai_python-0.4.6/src/novelai_python/sdk/ai/LICENSE
+-rwxr-xr-x   0        0        0      130 2024-04-06 06:10:20.345774 novelai_python-0.4.6/src/novelai_python/sdk/ai/__init__.py
+-rwxr-xr-x   0        0        0    34284 2024-04-06 06:10:20.345774 novelai_python-0.4.6/src/novelai_python/sdk/ai/generate_image/__init__.py
+-rw-r--r--   0        0        0    52850 2024-04-06 06:10:20.349774 novelai_python-0.4.6/src/novelai_python/sdk/ai/generate_image/_const.py
+-rwxr-xr-x   0        0        0     3578 2024-04-06 06:10:20.349774 novelai_python-0.4.6/src/novelai_python/sdk/ai/generate_image/_enum.py
+-rwxr-xr-x   0        0        0     5306 2024-04-06 06:10:20.349774 novelai_python-0.4.6/src/novelai_python/sdk/ai/generate_image/suggest_tags.py
+-rw-r--r--   0        0        0     7379 2024-04-06 06:10:20.349774 novelai_python-0.4.6/src/novelai_python/sdk/ai/generate_voice/__init__.py
+-rw-r--r--   0        0        0     2008 2024-04-06 06:10:20.349774 novelai_python-0.4.6/src/novelai_python/sdk/ai/generate_voice/_enum.py
+-rwxr-xr-x   0        0        0     8223 2024-04-06 06:10:20.349774 novelai_python-0.4.6/src/novelai_python/sdk/ai/upscale.py
+-rwxr-xr-x   0        0        0      945 2024-04-06 06:10:20.349774 novelai_python-0.4.6/src/novelai_python/sdk/schema.py
+-rwxr-xr-x   0        0        0      130 2024-04-06 06:10:20.349774 novelai_python-0.4.6/src/novelai_python/sdk/user/__init__.py
+-rwxr-xr-x   0        0        0     4772 2024-04-06 06:10:20.349774 novelai_python-0.4.6/src/novelai_python/sdk/user/information.py
+-rwxr-xr-x   0        0        0     5285 2024-04-06 06:10:20.349774 novelai_python-0.4.6/src/novelai_python/sdk/user/login.py
+-rwxr-xr-x   0        0        0     5045 2024-04-06 06:10:20.349774 novelai_python-0.4.6/src/novelai_python/sdk/user/subscription.py
+-rwxr-xr-x   0        0        0     6287 2024-04-06 06:10:20.349774 novelai_python-0.4.6/src/novelai_python/server.py
+-rw-r--r--   0        0        0     1075 2024-04-06 06:10:20.349774 novelai_python-0.4.6/src/novelai_python/tokenizer/__init__.py
+-rw-r--r--   0        0        0  1033724 2024-04-06 06:10:20.353774 novelai_python-0.4.6/src/novelai_python/tokenizer/novelai.model
+-rw-r--r--   0        0        0  1033744 2024-04-06 06:10:20.357774 novelai_python-0.4.6/src/novelai_python/tokenizer/novelai_v2.model
+-rw-r--r--   0        0        0       24 2024-04-06 06:10:20.357774 novelai_python-0.4.6/src/novelai_python/tool/__init__.py
+-rw-r--r--   0        0        0     7948 2024-04-06 06:10:20.357774 novelai_python-0.4.6/src/novelai_python/tool/image_metadata/__init__.py
+-rw-r--r--   0        0        0     3316 2024-04-06 06:10:20.361774 novelai_python-0.4.6/src/novelai_python/tool/image_metadata/lsb_extractor.py
+-rw-r--r--   0        0        0     2211 2024-04-06 06:10:20.361774 novelai_python-0.4.6/src/novelai_python/tool/image_metadata/lsb_injector.py
+-rw-r--r--   0        0        0     3181 2024-04-06 06:10:20.361774 novelai_python-0.4.6/src/novelai_python/tool/paint_mask/__init__.py
+-rw-r--r--   0        0        0    17162 2024-04-06 06:10:20.361774 novelai_python-0.4.6/src/novelai_python/tool/random_prompt/__init__.py
+-rw-r--r--   0        0        0    84988 2024-04-06 06:10:20.361774 novelai_python-0.4.6/src/novelai_python/tool/random_prompt/tag.py
+-rw-r--r--   0        0        0    21015 2024-04-06 06:10:20.361774 novelai_python-0.4.6/src/novelai_python/tool/random_prompt/tag_character.py
+-rw-r--r--   0        0        0    15814 2024-04-06 06:10:20.361774 novelai_python-0.4.6/src/novelai_python/tool/random_prompt/tag_nsfw.py
+-rwxr-xr-x   0        0        0      533 2024-04-06 06:10:20.361774 novelai_python-0.4.6/src/novelai_python/utils/__init__.py
+-rwxr-xr-x   0        0        0     1881 2024-04-06 06:10:20.361774 novelai_python-0.4.6/src/novelai_python/utils/encode.py
+-rwxr-xr-x   0        0        0     1243 2024-04-06 06:10:20.361774 novelai_python-0.4.6/src/novelai_python/utils/useful.py
+-rwxr-xr-x   0        0        0        0 2024-04-06 06:10:20.361774 novelai_python-0.4.6/tests/__init__.py
+-rw-r--r--   0        0        0      870 2024-04-06 06:10:20.361774 novelai_python-0.4.6/tests/test_generate_voice.py
+-rwxr-xr-x   0        0        0     2273 2024-04-06 06:10:20.361774 novelai_python-0.4.6/tests/test_random_prompt.py
+-rwxr-xr-x   0        0        0      422 2024-04-06 06:10:20.361774 novelai_python-0.4.6/tests/test_server.py
+-rwxr-xr-x   0        0        0     1375 2024-04-06 06:10:20.361774 novelai_python-0.4.6/tests/test_server_run.py
+-rwxr-xr-x   0        0        0     2772 2024-04-06 06:10:20.361774 novelai_python-0.4.6/tests/test_upscale.py
+-rwxr-xr-x   0        0        0     2592 2024-04-06 06:10:20.361774 novelai_python-0.4.6/tests/test_user_information.py
+-rwxr-xr-x   0        0        0     3244 2024-04-06 06:10:20.361774 novelai_python-0.4.6/tests/test_user_login.py
+-rwxr-xr-x   0        0        0     3270 2024-04-06 06:10:20.361774 novelai_python-0.4.6/tests/test_user_subscription.py
+-rw-r--r--   0        0        0     3933 1970-01-01 00:00:00.000000 novelai_python-0.4.6/PKG-INFO
```

### Comparing `novelai_python-0.4.5/LICENSE` & `novelai_python-0.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.5/NOTICE.MD` & `novelai_python-0.4.6/NOTICE.MD`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.5/README.md` & `novelai_python-0.4.6/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -94,15 +94,15 @@
 print(s)
 ```
 
 #### Run A Server
 
 ```shell
 pip install novelai_python
-python3 -m novelai_python.server -h '0.0.0.0' -p 7888
+python3 -m novelai_python.server -h '127.0.0.1' -p 7888
 ```
 
 ## Acknowledgements 🙏
 
 [BackEnd](https://api.novelai.net/docs)
 
 [novelai-api](https://github.com/Aedial/novelai-api)
```

### Comparing `novelai_python-0.4.5/pyproject.toml` & `novelai_python-0.4.6/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "novelai-python"
-version = "0.4.5"
+version = "0.4.6"
 description = "NovelAI Python Binding With Pydantic"
 authors = [
     { name = "sudoskys", email = "coldlando@hotmail.com" },
 ]
 dependencies = [
     "elara>=0.5.5",
     "loguru>=0.7.2",
```

### Comparing `novelai_python-0.4.5/src/novelai_python/__init__.py` & `novelai_python-0.4.6/src/novelai_python/__init__.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.5/src/novelai_python/_exceptions.py` & `novelai_python-0.4.6/src/novelai_python/_exceptions.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.5/src/novelai_python/_response/ai/generate_image.py` & `novelai_python-0.4.6/src/novelai_python/_response/ai/generate_image.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.5/src/novelai_python/_response/user/information.py` & `novelai_python-0.4.6/src/novelai_python/_response/user/information.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.5/src/novelai_python/_response/user/subscription.py` & `novelai_python-0.4.6/src/novelai_python/_response/user/subscription.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.5/src/novelai_python/credential/ApiToken.py` & `novelai_python-0.4.6/src/novelai_python/credential/ApiToken.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.5/src/novelai_python/credential/JwtToken.py` & `novelai_python-0.4.6/src/novelai_python/credential/JwtToken.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.5/src/novelai_python/credential/UserAuth.py` & `novelai_python-0.4.6/src/novelai_python/credential/UserAuth.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.5/src/novelai_python/sdk/__init__.py` & `novelai_python-0.4.6/src/novelai_python/sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.5/src/novelai_python/sdk/ai/LICENSE` & `novelai_python-0.4.6/src/novelai_python/sdk/ai/LICENSE`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.5/src/novelai_python/sdk/ai/_enum.py` & `novelai_python-0.4.6/src/novelai_python/sdk/ai/generate_voice/_enum.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.5/src/novelai_python/sdk/ai/generate_image/__init__.py` & `novelai_python-0.4.6/src/novelai_python/sdk/ai/generate_image/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # @Software: PyCharm
 import base64
 import json
 import math
 import random
 from copy import deepcopy
 from io import BytesIO
-from typing import Optional, Union, Tuple
+from typing import Optional, Union, Tuple, List
 from urllib.parse import urlparse
 from zipfile import ZipFile
 
 import curl_cffi
 import cv2
 import httpx
 import numpy as np
@@ -29,233 +29,284 @@
 from ...schema import ApiBaseModel
 from ...._exceptions import APIError, AuthError, ConcurrentGenerationError, SessionHttpError
 from ...._response.ai.generate_image import ImageGenerateResp
 from ....credential import CredentialBase
 from ....utils import try_jsonfy
 
 
+def is_multiple_of_01(num, precision=1e-10):
+    remainder = num % 0.01
+    return abs(remainder) < precision or abs(0.01 - remainder) < precision
+
+
+class Params(BaseModel):
+    add_original_image: Optional[bool] = Field(True, description="Overlay Original Image")
+    """
+    Overlay Original Image.Prevents the existing image from changing,
+    but can introduce seams along the edge of the mask.
+    叠加原始图像
+    防止现有图像发生更改，但可能会沿蒙版边缘引入接缝。
+    """
+    mask: Optional[Union[str, bytes]] = None
+    """Mask for Inpainting"""
+    cfg_rescale: Optional[float] = Field(0, ge=0, le=1, multiple_of=0.02)
+    """Prompt Guidance Rescale"""
+    controlnet_strength: Optional[float] = Field(1.0, ge=0.1, le=2, multiple_of=0.1)
+    """ControlNet Strength"""
+    dynamic_thresholding: Optional[bool] = False
+    """Reduce artifacts caused by high prompt guidance values"""
+    height: Optional[int] = Field(1216, ge=64, le=49152)
+    """Height For Generate Image"""
+    image: Optional[Union[str, bytes]] = None
+    """Image for img2img"""
+    strength: Optional[float] = Field(default=0.5, ge=0.01, le=0.99, multiple_of=0.01)
+    """Strength for img2img"""
+    noise: Optional[float] = Field(default=0, ge=0, le=0.99, multiple_of=0.01)
+    """Noise for img2img"""
+    controlnet_condition: Optional[str] = None
+    """ControlNet Condition"""
+    controlnet_model: Optional[ControlNetModel] = None
+    """ControlNet Model"""
+    n_samples: Optional[int] = Field(1, ge=1, le=8)
+    """Number of samples"""
+    negative_prompt: Optional[str] = ''
+    """Negative Prompt"""
+    noise_schedule: Optional[NoiseSchedule] = NoiseSchedule.NATIVE
+    """Noise Schedule"""
+    # Misc
+    params_version: Optional[int] = 1
+    """Params Version For Request"""
+    reference_image_multiple: Optional[List[Union[str, bytes]]] = None
+    """Reference Image For Vibe Mode"""
+    reference_information_extracted_multiple: Optional[List[float]] = None
+    """Reference Information Extracted For Vibe Mode"""
+
+    @field_validator('reference_information_extracted_multiple')
+    def reference_information_extracted_multiple_validator(cls, v):
+        # List[Field(..., ge=0, le=1, multiple_of=0.01)]
+        if v is None:
+            return v
+        for i in v:
+            if not 0 <= i <= 1:
+                raise ValueError("Invalid reference_information_extracted_multiple, must be in [0, 1].")
+            if not is_multiple_of_01(i):
+                raise ValueError("Invalid reference_information_extracted_multiple, must be multiple of 0.01.")
+        return v
+
+    reference_strength_multiple: Optional[List[float]] = None
+
+    @field_validator('reference_strength_multiple')
+    def reference_strength_multiple_validator(cls, v):
+        # Field(0.6,ge=0,le=1,multiple_of=0.01,description="the stronger the AI will try to emulate visual cues.")
+        if v is None:
+            return v
+        for i in v:
+            if not 0 <= i <= 1:
+                raise ValueError("Invalid reference_strength_multiple, must be in [0, 1].")
+            if not is_multiple_of_01(i):
+                raise ValueError("Invalid reference_strength_multiple, must be multiple of 0.01.")
+        return v
+
+    """Reference Strength For Vibe Mode"""
+    legacy: Optional[bool] = False
+    # TODO: find out the usage
+    legacy_v3_extend: Optional[bool] = False
+    # TODO: find out the usage
+    qualityToggle: Optional[bool] = True
+    """Whether to add the quality prompt"""
+    sampler: Optional[Sampler] = Sampler.K_EULER
+    """Sampler For Generate Image"""
+    scale: Optional[float] = Field(6.0, ge=0, le=10, multiple_of=0.1)
+    """Prompt Guidance"""
+    # Seed
+    seed: Optional[int] = Field(
+        default_factory=lambda: random.randint(0, 4294967295 - 7),
+        gt=0,
+        le=4294967295 - 7,
+    )
+    """Seed"""
+    extra_noise_seed: Optional[int] = Field(
+        default_factory=lambda: random.randint(0, 4294967295 - 7),
+        gt=0,
+        le=4294967295 - 7,
+    )
+    """Extra Noise Seed"""
+    sm: Optional[bool] = False
+    # TODO: find out the usage
+    sm_dyn: Optional[bool] = False
+    # TODO: find out the usage
+    steps: Optional[int] = Field(28, ge=1, le=50)
+    """Steps"""
+    ucPreset: Optional[UCPreset] = 0
+    """The Negative Prompt Preset"""
+    uncond_scale: Optional[float] = Field(1.0, ge=0, le=1.5, multiple_of=0.05)
+    """Undesired Content Strength"""
+    width: Optional[int] = Field(832, ge=64, le=49152)
+    """Width For Image"""
+
+    @staticmethod
+    def resize_image(image: Union[str, bytes], width: int, height: int):
+        """
+        Resize the image to the specified size.
+        :param image: The image to be resized
+        :param width: The width of the image
+        :param height: The height of the image
+        :return: The resized image
+        """
+        if isinstance(image, str):
+            image = base64.b64decode(image)
+        open_image = Image.open(BytesIO(image)).convert("RGBA")
+        # 如果尺寸相同，直接返回
+        if open_image.width == width and open_image.height == height:
+            logger.debug("Image size is same, return directly.")
+            if isinstance(image, bytes):
+                return base64.b64encode(image).decode("utf-8")
+            return image
+        open_image = open_image.resize((width, height), Image.Resampling.BICUBIC)
+        buffered = BytesIO()
+        open_image.save(buffered, format="PNG")
+        return base64.b64encode(buffered.getvalue()).decode("utf-8")
+
+    @staticmethod
+    def add_image_to_black_background(
+            image: Union[str, bytes],
+            target_size: Tuple[int, int] = (448, 448),
+            transparency: bool = False
+    ):
+
+        """
+        缩放图像到指定的黑色透明背景上，使其尽可能大且保持比例。
+        :param transparency: 是否透明
+        :param image: 图像
+        :param target_size: 目标尺寸
+        :return: 新图像
+        """
+
+        if isinstance(image, str):
+            image = base64.b64decode(image)
+            # Decode the image from the base64 string
+        npimg = np.frombuffer(image, np.uint8)
+        # Load the image with OpenCV
+        img = cv2.imdecode(npimg, cv2.IMREAD_UNCHANGED)
+        # Calculate the aspect ratio (keeping aspect ratio)
+        ratio = min(target_size[0] / img.shape[1], target_size[1] / img.shape[0])
+        new_image_size = (int(img.shape[1] * ratio), int(img.shape[0] * ratio))
+        # Resize the image
+        img = cv2.resize(img, new_image_size, interpolation=cv2.INTER_LINEAR)
+        # Check if the image has alpha channel (transparency)
+        if img.shape[2] == 3:  # no alpha channel, add one
+            img = cv2.cvtColor(img, cv2.COLOR_BGR2BGRA)
+        # Create new image with black background
+        delta_w = target_size[0] - img.shape[1]
+        delta_h = target_size[1] - img.shape[0]
+        top, bottom = delta_h // 2, delta_h - (delta_h // 2)
+        left, right = delta_w // 2, delta_w - (delta_w // 2)
+        # If the transparency flag is set the background is transparent, otherwise it is black
+        color = [0, 0, 0, 0] if transparency else [0, 0, 0, 255]
+        # Add padding to the image
+        new_img = cv2.copyMakeBorder(img, top, bottom, left, right, cv2.BORDER_CONSTANT, value=color)
+        # Convert the image to base64
+        _, buffer = cv2.imencode(".png", new_img)
+        # buffer here is a numpy array, convert it to bytes
+        image_bytes = buffer.tobytes()
+        return base64.b64encode(image_bytes).decode("utf-8")
+
+    # Validators
+    @model_validator(mode="after")
+    def image_validator(self):
+        if self.sampler:
+            if self.sampler in [Sampler.DDIM, Sampler.DDIM_V3]:
+                self.sm = False
+                self.sm_dyn = False
+                if self.sm_dyn or self.sm:
+                    logger.warning("sm and sm_dyn is disabled when using ddim sampler.")
+            if self.sampler in [Sampler.NAI_SMEA_DYN]:
+                self.sm = True
+                self.sm_dyn = True
+                if not self.sm_dyn:
+                    logger.warning("sm and sm_dyn is enabled when using nai_smea_dyn sampler.")
+        if isinstance(self.image, str) and self.image.startswith("data:"):
+            raise ValueError("Invalid `image` format, must be base64 encoded directly.")
+        if isinstance(self.mask, str) and self.mask.startswith("data:"):
+            raise ValueError("Invalid `mask` format, must be base64 encoded directly.")
+        if isinstance(self.image, bytes):
+            self.image = base64.b64encode(self.image).decode("utf-8")
+        # Resize the image to the specified size
+        if self.reference_image_multiple is not None:
+            new_images = []
+            for reference_image in self.reference_image_multiple:
+                if isinstance(reference_image, str):
+                    if reference_image.startswith("data:"):
+                        raise ValueError("Invalid `reference_image` format, must be base64 encoded directly.")
+                    new_images.append(reference_image)
+                elif isinstance(reference_image, bytes):
+                    new_image = self.add_image_to_black_background(reference_image,
+                                                                   target_size=(448, 448),
+                                                                   transparency=True)
+                    if isinstance(new_image, bytes):
+                        new_image = base64.b64encode(new_image).decode("utf-8")
+                    new_images.append(new_image)
+                else:
+                    raise ValueError("Invalid `reference_image` format, must be base64 encoded directly.")
+            self.reference_image_multiple = new_images
+        # 如果都不是 None 时，比较他们的长度
+        if all([self.reference_strength_multiple,
+                self.reference_image_multiple,
+                self.reference_information_extracted_multiple]):
+            if len(self.reference_strength_multiple) != len(self.reference_image_multiple) != len(
+                    self.reference_information_extracted_multiple):
+                raise ValueError("All three reference_* must be of equal length")
+
+        # 如果有一个存在，其他都必须存在
+        ref_items = [self.reference_strength_multiple,
+                     self.reference_image_multiple,
+                     self.reference_information_extracted_multiple]
+        if any(ref_items) and not all(ref_items):
+            raise ValueError("All fields must be present together or none should be present")
+
+        if isinstance(self.mask, bytes):
+            self.mask = base64.b64encode(self.mask).decode("utf-8")
+        if self.image is not None:
+            self.image = self.resize_image(self.image, self.width, self.height)
+        return self
+
+    @field_validator('width')
+    def width_validator(cls, v: int):
+        """
+        Must be multiple of 64
+        :param v:
+        :return: fixed value
+        """
+        if v % 64 != 0:
+            raise ValueError("Invalid width, must be multiple of 64.")
+        return v
+
+    @field_validator('height')
+    def height_validator(cls, v: int):
+        """
+        Must be multiple of 64
+        :param v:
+        :return: fixed value
+        """
+        if v % 64 != 0:
+            raise ValueError("Invalid height, must be multiple of 64.")
+        return v
+
+
 class GenerateImageInfer(ApiBaseModel):
     _endpoint: str = PrivateAttr("https://image.novelai.net")
 
     @property
     def endpoint(self):
         return self._endpoint
 
     @endpoint.setter
     def endpoint(self, value):
         self._endpoint = value
 
-    class Params(BaseModel):
-        add_original_image: Optional[bool] = Field(True, description="Overlay Original Image")
-        """
-        Overlay Original Image.Prevents the existing image from changing,
-        but can introduce seams along the edge of the mask.
-        叠加原始图像
-        防止现有图像发生更改，但可能会沿蒙版边缘引入接缝。
-        """
-        mask: Optional[Union[str, bytes]] = None
-        """Mask for Inpainting"""
-        cfg_rescale: Optional[float] = Field(0, ge=0, le=1, multiple_of=0.02)
-        """Prompt Guidance Rescale"""
-        controlnet_strength: Optional[float] = Field(1.0, ge=0.1, le=2, multiple_of=0.1)
-        """ControlNet Strength"""
-        dynamic_thresholding: Optional[bool] = False
-        """Reduce artifacts caused by high prompt guidance values"""
-        height: Optional[int] = Field(1216, ge=64, le=49152)
-        """Height For Generate Image"""
-        image: Optional[Union[str, bytes]] = None
-        """Image for img2img"""
-        strength: Optional[float] = Field(default=0.5, ge=0.01, le=0.99, multiple_of=0.01)
-        """Strength for img2img"""
-        noise: Optional[float] = Field(default=0, ge=0, le=0.99, multiple_of=0.01)
-        """Noise for img2img"""
-        controlnet_condition: Optional[str] = None
-        """ControlNet Condition"""
-        controlnet_model: Optional[ControlNetModel] = None
-        """ControlNet Model"""
-        n_samples: Optional[int] = Field(1, ge=1, le=8)
-        """Number of samples"""
-        negative_prompt: Optional[str] = ''
-        """Negative Prompt"""
-        noise_schedule: Optional[NoiseSchedule] = NoiseSchedule.NATIVE
-        """Noise Schedule"""
-        # Misc
-        params_version: Optional[int] = 1
-        """Params Version For Request"""
-        reference_image: Optional[Union[str, bytes]] = None
-        """Reference Image For Vibe Mode"""
-        reference_information_extracted: Optional[float] = Field(1,
-                                                                 ge=0,
-                                                                 le=1,
-                                                                 multiple_of=0.01,
-                                                                 description="extracting concepts or features"
-                                                                 )
-        """Reference Information Extracted For Vibe Mode"""
-        reference_strength: Optional[float] = Field(0.6,
-                                                    ge=0,
-                                                    le=1,
-                                                    multiple_of=0.01,
-                                                    description="the stronger the AI will try to emulate visual cues."
-                                                    )
-        """Reference Strength For Vibe Mode"""
-        legacy: Optional[bool] = False
-        # TODO: find out the usage
-        legacy_v3_extend: Optional[bool] = False
-        # TODO: find out the usage
-        qualityToggle: Optional[bool] = True
-        """Whether to add the quality prompt"""
-        sampler: Optional[Sampler] = Sampler.K_EULER
-        """Sampler For Generate Image"""
-        scale: Optional[float] = Field(6.0, ge=0, le=10, multiple_of=0.1)
-        """Prompt Guidance"""
-        # Seed
-        seed: Optional[int] = Field(
-            default_factory=lambda: random.randint(0, 4294967295 - 7),
-            gt=0,
-            le=4294967295 - 7,
-        )
-        """Seed"""
-        extra_noise_seed: Optional[int] = Field(
-            default_factory=lambda: random.randint(0, 4294967295 - 7),
-            gt=0,
-            le=4294967295 - 7,
-        )
-        """Extra Noise Seed"""
-        sm: Optional[bool] = False
-        # TODO: find out the usage
-        sm_dyn: Optional[bool] = False
-        # TODO: find out the usage
-        steps: Optional[int] = Field(28, ge=1, le=50)
-        """Steps"""
-        ucPreset: Optional[UCPreset] = 0
-        """The Negative Prompt Preset"""
-        uncond_scale: Optional[float] = Field(1.0, ge=0, le=1.5, multiple_of=0.05)
-        """Undesired Content Strength"""
-        width: Optional[int] = Field(832, ge=64, le=49152)
-        """Width For Image"""
-
-        @staticmethod
-        def resize_image(image: Union[str, bytes], width: int, height: int):
-            """
-            Resize the image to the specified size.
-            :param image: The image to be resized
-            :param width: The width of the image
-            :param height: The height of the image
-            :return: The resized image
-            """
-            if isinstance(image, str):
-                image = base64.b64decode(image)
-            open_image = Image.open(BytesIO(image)).convert("RGBA")
-            # 如果尺寸相同，直接返回
-            if open_image.width == width and open_image.height == height:
-                logger.debug("Image size is same, return directly.")
-                if isinstance(image, bytes):
-                    return base64.b64encode(image).decode("utf-8")
-                return image
-            open_image = open_image.resize((width, height), Image.Resampling.BICUBIC)
-            buffered = BytesIO()
-            open_image.save(buffered, format="PNG")
-            return base64.b64encode(buffered.getvalue()).decode("utf-8")
-
-        @staticmethod
-        def add_image_to_black_background(
-                image: Union[str, bytes],
-                target_size: Tuple[int, int] = (448, 448),
-                transparency: bool = False
-        ):
-
-            """
-            缩放图像到指定的黑色透明背景上，使其尽可能大且保持比例。
-            :param transparency: 是否透明
-            :param image: 图像
-            :param target_size: 目标尺寸
-            :return: 新图像
-            """
-
-            if isinstance(image, str):
-                image = base64.b64decode(image)
-                # Decode the image from the base64 string
-            npimg = np.frombuffer(image, np.uint8)
-            # Load the image with OpenCV
-            img = cv2.imdecode(npimg, cv2.IMREAD_UNCHANGED)
-            # Calculate the aspect ratio (keeping aspect ratio)
-            ratio = min(target_size[0] / img.shape[1], target_size[1] / img.shape[0])
-            new_image_size = (int(img.shape[1] * ratio), int(img.shape[0] * ratio))
-            # Resize the image
-            img = cv2.resize(img, new_image_size, interpolation=cv2.INTER_LINEAR)
-            # Check if the image has alpha channel (transparency)
-            if img.shape[2] == 3:  # no alpha channel, add one
-                img = cv2.cvtColor(img, cv2.COLOR_BGR2BGRA)
-            # Create new image with black background
-            delta_w = target_size[0] - img.shape[1]
-            delta_h = target_size[1] - img.shape[0]
-            top, bottom = delta_h // 2, delta_h - (delta_h // 2)
-            left, right = delta_w // 2, delta_w - (delta_w // 2)
-            # If the transparency flag is set the background is transparent, otherwise it is black
-            color = [0, 0, 0, 0] if transparency else [0, 0, 0, 255]
-            # Add padding to the image
-            new_img = cv2.copyMakeBorder(img, top, bottom, left, right, cv2.BORDER_CONSTANT, value=color)
-            # Convert the image to base64
-            _, buffer = cv2.imencode(".png", new_img)
-            return base64.b64encode(buffer).decode("utf-8")
-
-        # Validators
-        @model_validator(mode="after")
-        def image_validator(self):
-            if self.sampler:
-                if self.sampler in [Sampler.DDIM, Sampler.DDIM_V3]:
-                    self.sm = False
-                    self.sm_dyn = False
-                    if self.sm_dyn or self.sm:
-                        logger.warning("sm and sm_dyn is disabled when using ddim sampler.")
-                if self.sampler in [Sampler.NAI_SMEA_DYN]:
-                    self.sm = True
-                    self.sm_dyn = True
-                    if not self.sm_dyn:
-                        logger.warning("sm and sm_dyn is enabled when using nai_smea_dyn sampler.")
-            if isinstance(self.image, str) and self.image.startswith("data:"):
-                raise ValueError("Invalid `image` format, must be base64 encoded directly.")
-            if isinstance(self.reference_image, str) and self.reference_image.startswith("data:"):
-                raise ValueError("Invalid `reference_image` format, must be base64 encoded directly.")
-            if isinstance(self.mask, str) and self.mask.startswith("data:"):
-                raise ValueError("Invalid `mask` format, must be base64 encoded directly.")
-            if isinstance(self.image, bytes):
-                self.image = base64.b64encode(self.image).decode("utf-8")
-            if isinstance(self.reference_image, bytes):
-                self.reference_image = base64.b64encode(self.reference_image).decode("utf-8")
-            if isinstance(self.mask, bytes):
-                self.mask = base64.b64encode(self.mask).decode("utf-8")
-            if self.image is not None:
-                self.image = self.resize_image(self.image, self.width, self.height)
-            if self.reference_image is not None:
-                self.reference_image = self.add_image_to_black_background(self.reference_image, width=448, height=448)
-            return self
-
-        @field_validator('width')
-        def width_validator(cls, v: int):
-            """
-            Must be multiple of 64
-            :param v:
-            :return: fixed value
-            """
-            if v % 64 != 0:
-                raise ValueError("Invalid width, must be multiple of 64.")
-            return v
-
-        @field_validator('height')
-        def height_validator(cls, v: int):
-            """
-            Must be multiple of 64
-            :param v:
-            :return: fixed value
-            """
-            if v % 64 != 0:
-                raise ValueError("Invalid height, must be multiple of 64.")
-            return v
-
     action: Union[str, Action] = Field(Action.GENERATE, description="Mode for img generate")
     input: str = "1girl, best quality, amazing quality, very aesthetic, absurdres"
     model: Optional[Model] = "nai-diffusion-3"
     parameters: Params = Params()
     model_config = ConfigDict(extra="ignore")
 
     @override
@@ -415,14 +466,17 @@
               cfg_rescale: float = 0,
               sampler: Union[Sampler, str] = None,
               width: int = 832,
               height: int = 1216,
               qualityToggle: bool = None,
               image: Union[str, bytes] = None,
               noise: float = 0,
+              reference_image_multiple: List[Union[str, bytes]] = None,
+              reference_strength_multiple: List[float] = None,
+              reference_information_extracted_multiple: List[float] = None,
               reference_image: Union[str, bytes] = None,
               reference_strength: float = None,
               reference_information_extracted: float = None,
               add_original_image: bool = True,
               strength: float = None,
               mask: Union[str, bytes] = None,
               controlnet_model: Union[ControlNetModel, str] = None,
@@ -431,14 +485,20 @@
               sm_dyn: bool = False,
               uncond_scale: float = None,
               **kwargs
               ):
         """
         The build function, more convenient to create a GenerateImageInfer instance.
         构建函数，更方便地创建一个GenerateImageInfer实例。
+        :param reference_information_extracted_multiple:  The reference information extracted for Vibe mode.
+                                                            Vibe模式的提取的参考信息。
+        :param reference_image_multiple: The reference image for Vibe mode.
+                                            Vibe模式的参考图像。
+        :param reference_strength_multiple: The strength of the reference image used in Vibe mode.
+                                            在Vibe模式中使用的参考图像的强度。
         :param ucPreset: 0: Heavy, 1: Light, 2: Character
                         0: 重量级, 1: 轻量级, 2: 角色
         :param qualityToggle: add the quality prompt or not.
                               是否添加质量提示。
         :param prompt: input prompt for generation.
                        生成的输入提示。
         :param model: select a model.
@@ -461,20 +521,14 @@
                       图像的宽度。
         :param height: the height of the image.
                        图像的高度。
         :param image: the input image.
                       输入图像。
         :param noise: the noise to be added in the image.
                       要添加到图像中的噪声。
-        :param reference_image: the reference image for Vibe mode.
-                                Vibe模式的参考图像。
-        :param reference_strength: the strength of the reference image used in Vibe mode.
-                                   在Vibe模式中使用的参考图像的强度。
-        :param reference_information_extracted: whether to extract concept or features, for Vibe mode.
-                                                是否提取概念或特征，用于Vibe模式。
         :param add_original_image: Overlay Original Image. Prevents the existing image from changing, only for IMG2IMG mode.
                                    叠加原始图像。防止现有图像发生更改，仅适用于IMG2IMG模式。
         :param strength: the strength of IMG2IMG mode.
                          IMG2IMG模式的强度。
         :param mask: the inpainting mask.
                      纹理绘制掩码。
         :param controlnet_model: the model used for the control network.
@@ -510,19 +564,55 @@
             "mask": mask,
             "controlnet_model": controlnet_model,
             "controlnet_condition": controlnet_condition,
             "sm_dyn": sm_dyn,
             "sm": sm,
             "uncond_scale": uncond_scale,
         })
+
+        def _merge_param(v1, v2):
+            _list = []
+            if isinstance(v1, list):
+                _list.extend(v1)
+            else:
+                if v1 is not None:
+                    _list.append(v1)
+            if isinstance(v2, list):
+                _list.extend(v2)
+            else:
+                if v2 is not None:
+                    _list.append(v2)
+            return _list
+
+        if reference_image:
+            logger.warning(
+                "reference_image is deprecated, use reference_image_multiple instead."
+            )
+            reference_image_multiple = _merge_param(
+                reference_image, reference_image_multiple
+            )
+        if reference_strength:
+            logger.warning(
+                "reference_strength is deprecated, use reference_strength_multiple instead."
+            )
+            reference_strength_multiple = _merge_param(
+                reference_strength, reference_strength_multiple
+            )
+        if reference_information_extracted:
+            logger.warning(
+                "reference_information_extracted is deprecated, use reference_information_extracted_multiple instead."
+            )
+            reference_information_extracted_multiple = _merge_param(
+                reference_information_extracted, reference_information_extracted_multiple
+            )
         kwargs.update(
             {
-                "reference_image": reference_image,
-                "reference_strength": reference_strength,
-                "reference_information_extracted": reference_information_extracted,
+                "reference_image_multiple": reference_image_multiple,
+                "reference_strength_multiple": reference_strength_multiple,
+                "reference_information_extracted_multiple": reference_information_extracted_multiple,
             }
         )
         kwargs.update(
             {
                 "image": image,
                 "strength": strength,
                 "noise": noise,
@@ -530,15 +620,15 @@
         )
         # 清理空值
         param = {k: v for k, v in kwargs.items() if v is not None}
         return cls(
             input=prompt,
             model=model,
             action=action,
-            parameters=cls.Params(**param)
+            parameters=Params(**param)
         )
 
     async def necessary_headers(self, request_data) -> dict:
         """
         :param request_data:
         :return:
         """
@@ -588,15 +678,16 @@
             session.headers.clear()
             session.headers.update(override_headers)
         try:
             _log_data = deepcopy(request_data)
             _log_data.get("parameters", {}).update({
                 "image": "base64 data" if self.parameters.image else None,
                 "mask": "base64 data" if self.parameters.mask else None,
-                "reference_image": "base64 data" if self.parameters.reference_image else None,
+                "reference_image_multiple": ["base64 data"] * len(
+                    self.parameters.reference_image_multiple) if self.parameters.reference_image_multiple else None,
             })
             logger.debug(f"Request Data: {_log_data}")
             del _log_data
         except Exception as e:
             logger.warning(f"Error when print log data: {e}")
         try:
             assert hasattr(session, "post"), "session must have post method."
```

### Comparing `novelai_python-0.4.5/src/novelai_python/sdk/ai/generate_image/_const.py` & `novelai_python-0.4.6/src/novelai_python/sdk/ai/generate_image/_const.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.5/src/novelai_python/sdk/ai/generate_image/_enum.py` & `novelai_python-0.4.6/src/novelai_python/sdk/ai/generate_image/_enum.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.5/src/novelai_python/sdk/ai/generate_image/suggest_tags.py` & `novelai_python-0.4.6/src/novelai_python/sdk/ai/generate_image/suggest_tags.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.5/src/novelai_python/sdk/ai/generate_voice.py` & `novelai_python-0.4.6/src/novelai_python/sdk/ai/generate_voice/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,25 @@
 # -*- coding: utf-8 -*-
 # @Author  : sudoskys
-import base64
-import json
-from io import BytesIO
 from typing import Optional, Union, Literal
 from urllib.parse import urlparse
-from zipfile import ZipFile
 
 import curl_cffi
 import httpx
 import pydantic
 from curl_cffi.requests import AsyncSession
 from loguru import logger
 from pydantic import ConfigDict, PrivateAttr, Field, model_validator
 from tenacity import wait_random, retry, stop_after_attempt, retry_if_exception
 
-from ..schema import ApiBaseModel
-from ..._exceptions import APIError, AuthError, SessionHttpError
-from ..._response.ai.generate_voice import VoiceResponse
-from ...credential import CredentialBase
-from ...utils import try_jsonfy
 from ._enum import VoiceSpeakerV1, VoiceSpeakerV2
+from ...schema import ApiBaseModel
+from ...._exceptions import APIError, SessionHttpError
+from ...._response.ai.generate_voice import VoiceResponse
+from ....credential import CredentialBase
 
 
 class VoiceGenerate(ApiBaseModel):
     """
     Voice Generate for /ai/generate-voice
     """
     _endpoint: str = PrivateAttr("https://api.novelai.net")
```

### Comparing `novelai_python-0.4.5/src/novelai_python/sdk/ai/upscale.py` & `novelai_python-0.4.6/src/novelai_python/sdk/ai/upscale.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.5/src/novelai_python/sdk/schema.py` & `novelai_python-0.4.6/src/novelai_python/sdk/schema.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.5/src/novelai_python/sdk/user/information.py` & `novelai_python-0.4.6/src/novelai_python/sdk/user/information.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.5/src/novelai_python/sdk/user/login.py` & `novelai_python-0.4.6/src/novelai_python/sdk/user/login.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.5/src/novelai_python/sdk/user/subscription.py` & `novelai_python-0.4.6/src/novelai_python/sdk/user/subscription.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.5/src/novelai_python/server.py` & `novelai_python-0.4.6/src/novelai_python/server.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,25 +2,27 @@
 # @Time    : 2024/1/30 下午11:05
 # @Author  : sudoskys
 # @File    : server.py
 
 import io
 import sys
 import zipfile
+from typing import Optional, Literal, Union
 
 import uvicorn
 from fastapi import FastAPI, Depends, Security
 from fastapi.security import APIKeyHeader
 from loguru import logger
 from starlette.responses import JSONResponse, StreamingResponse
 
 from .credential import JwtCredential, SecretStr
-from .sdk.ai.generate_image import GenerateImageInfer
+from .sdk.ai.generate_image import GenerateImageInfer, Model
 from .sdk.ai.generate_image.suggest_tags import SuggestTags
 from .sdk.ai.upscale import Upscale
+from .sdk.ai.generate_voice import VoiceGenerate, VoiceResponse
 from .sdk.user.information import Information
 from .sdk.user.login import Login
 from .sdk.user.subscription import Subscription
 
 app = FastAPI()
 token_key = APIKeyHeader(name="Authorization")
 session = {}
@@ -117,24 +119,27 @@
     except Exception as e:
         logger.exception(e)
         return JSONResponse(status_code=500, content=e.__dict__)
 
 
 @app.get("/ai/generate_image/suggest_tags")
 async def suggest_tags(
-        req: SuggestTags,
+        model: Model,
+        prompt: str,
         current_token: str = Depends(get_current_token)
 ):
     """
     生成建议
     :param current_token: Authorization
-    :param req: SuggestTags
+    :param model: Model
+    :param prompt: str
     :return:
     """
     try:
+        req = SuggestTags(model=model, prompt=prompt)
         _result = await req.request(session=get_session(current_token))
         return _result.model_dump()
     except Exception as e:
         logger.exception(e)
         return JSONResponse(status_code=500, content=e.__dict__)
 
 
@@ -161,14 +166,40 @@
             'Content-Disposition': 'attachment;filename=image.zip'
         })
     except Exception as e:
         logger.exception(e)
         return JSONResponse(status_code=500, content=e.__dict__)
 
 
+@app.get("/ai/generate-voice")
+async def generate_voice(
+        text: str,
+        voice: int = -1,
+        seed: Optional[str] = None,
+        opus: bool = False,
+        version: Union[Literal["v2", "v1"], str] = "v2",
+        current_token: str = Depends(get_current_token)
+):
+    """
+    生成图片
+    :param current_token: Authorization
+    :param req: GenerateImageInfer
+    :return:
+    """
+    try:
+        req = VoiceGenerate(text=text, voice=voice, seed=seed, opus=opus, version=version)
+        _result = await req.request(session=get_session(current_token))
+        return StreamingResponse(io.BytesIO(_result.audio), media_type='audio/mpeg', headers={
+            'Content-Disposition': 'attachment;filename=audio.mp3'
+        })
+    except Exception as e:
+        logger.exception(e)
+        return JSONResponse(status_code=500, content=e.__dict__)
+
+
 # 获取输入参数
 def usage():
     print("Usage: python -m novelai_python.server -h <host> -p <port>")
     sys.exit(0)
 
 
 if __name__ == '__main__':
@@ -176,11 +207,11 @@
 
     opts = {}
     try:
         opts, args = getopt.getopt(sys.argv[1:], "h:p:", ["host=", "port="])
     except getopt.GetoptError:
         usage()
     opts = dict(opts)
-    server_host = opts.get("-h", "0.0.0.0")
+    server_host = opts.get("-h", "127.0.0.1")
     server_port = int(opts.get("-p", 10087))
     print(f"Docs: http://{server_host}:{server_port}/docs")
     uvicorn.run(app, host=server_host, port=server_port)
```

### Comparing `novelai_python-0.4.5/src/novelai_python/tokenizer/__init__.py` & `novelai_python-0.4.6/src/novelai_python/tokenizer/__init__.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.5/src/novelai_python/tokenizer/novelai.model` & `novelai_python-0.4.6/src/novelai_python/tokenizer/novelai.model`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.5/src/novelai_python/tokenizer/novelai_v2.model` & `novelai_python-0.4.6/src/novelai_python/tokenizer/novelai_v2.model`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.5/src/novelai_python/tool/image_metadata/__init__.py` & `novelai_python-0.4.6/src/novelai_python/tool/image_metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.5/src/novelai_python/tool/image_metadata/lsb_extractor.py` & `novelai_python-0.4.6/src/novelai_python/tool/image_metadata/lsb_extractor.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.5/src/novelai_python/tool/image_metadata/lsb_injector.py` & `novelai_python-0.4.6/src/novelai_python/tool/image_metadata/lsb_injector.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.5/src/novelai_python/tool/paint_mask/__init__.py` & `novelai_python-0.4.6/src/novelai_python/tool/paint_mask/__init__.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.5/src/novelai_python/tool/random_prompt/__init__.py` & `novelai_python-0.4.6/src/novelai_python/tool/random_prompt/__init__.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.5/src/novelai_python/tool/random_prompt/tag.py` & `novelai_python-0.4.6/src/novelai_python/tool/random_prompt/tag.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.5/src/novelai_python/tool/random_prompt/tag_character.py` & `novelai_python-0.4.6/src/novelai_python/tool/random_prompt/tag_character.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.5/src/novelai_python/tool/random_prompt/tag_nsfw.py` & `novelai_python-0.4.6/src/novelai_python/tool/random_prompt/tag_nsfw.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.5/src/novelai_python/utils/__init__.py` & `novelai_python-0.4.6/src/novelai_python/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.5/src/novelai_python/utils/encode.py` & `novelai_python-0.4.6/src/novelai_python/utils/encode.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.5/src/novelai_python/utils/useful.py` & `novelai_python-0.4.6/src/novelai_python/utils/useful.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.5/tests/test_generate_voice.py` & `novelai_python-0.4.6/tests/test_generate_voice.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.5/tests/test_random_prompt.py` & `novelai_python-0.4.6/tests/test_random_prompt.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.5/tests/test_server_run.py` & `novelai_python-0.4.6/tests/test_server_run.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.5/tests/test_upscale.py` & `novelai_python-0.4.6/tests/test_upscale.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.5/tests/test_user_information.py` & `novelai_python-0.4.6/tests/test_user_information.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.5/tests/test_user_login.py` & `novelai_python-0.4.6/tests/test_user_login.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.5/tests/test_user_subscription.py` & `novelai_python-0.4.6/tests/test_user_subscription.py`

 * *Files identical despite different names*

### Comparing `novelai_python-0.4.5/PKG-INFO` & `novelai_python-0.4.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: novelai-python
-Version: 0.4.5
+Version: 0.4.6
 Summary: NovelAI Python Binding With Pydantic
 Author-Email: sudoskys <coldlando@hotmail.com>
 License: Apache License 2.0
 Project-URL: Repository, https://github.com/LlmKira/novelai-python/
 Project-URL: Issues, https://github.com/LlmKira/novelai-python/issues
 Requires-Python: >=3.8
 Requires-Dist: elara>=0.5.5
@@ -125,15 +125,15 @@
 print(s)
 ```
 
 #### Run A Server
 
 ```shell
 pip install novelai_python
-python3 -m novelai_python.server -h '0.0.0.0' -p 7888
+python3 -m novelai_python.server -h '127.0.0.1' -p 7888
 ```
 
 ## Acknowledgements 🙏
 
 [BackEnd](https://api.novelai.net/docs)
 
 [novelai-api](https://github.com/Aedial/novelai-api)
```

