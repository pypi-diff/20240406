# Comparing `tmp/nonebot_plugin_bilichat-5.3.1.tar.gz` & `tmp/nonebot_plugin_bilichat-5.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_bilichat-5.3.1.tar", last modified: Fri Apr  5 09:51:38 2024, max compression
+gzip compressed data, was "nonebot_plugin_bilichat-5.3.2.tar", last modified: Sat Apr  6 17:23:17 2024, max compression
```

## Comparing `nonebot_plugin_bilichat-5.3.1.tar` & `nonebot_plugin_bilichat-5.3.2.tar`

### file list

```diff
@@ -1,86 +1,80 @@
--rw-r--r--   0        0        0    34523 2024-04-05 09:51:35.237000 nonebot_plugin_bilichat-5.3.1/LICENSE
--rw-r--r--   0        0        0    17818 2024-04-05 09:51:35.237000 nonebot_plugin_bilichat-5.3.1/README.md
--rw-r--r--   0        0        0     2770 2024-04-05 09:51:35.257000 nonebot_plugin_bilichat-5.3.1/nonebot_plugin_bilichat/__init__.py
--rw-r--r--   0        0        0     1120 2024-04-05 09:51:35.257000 nonebot_plugin_bilichat-5.3.1/nonebot_plugin_bilichat/api/__init__.py
--rw-r--r--   0        0        0      740 2024-04-05 09:51:35.257000 nonebot_plugin_bilichat-5.3.1/nonebot_plugin_bilichat/api/base.py
--rw-r--r--   0        0        0     2232 2024-04-05 09:51:35.257000 nonebot_plugin_bilichat-5.3.1/nonebot_plugin_bilichat/api/bilibili_auth.py
--rw-r--r--   0        0        0     1647 2024-04-05 09:51:35.257000 nonebot_plugin_bilichat-5.3.1/nonebot_plugin_bilichat/api/subs_config.py
--rw-r--r--   0        0        0     2686 2024-04-05 09:51:35.257000 nonebot_plugin_bilichat-5.3.1/nonebot_plugin_bilichat/api/webui.py
--rw-r--r--   0        0        0      575 2024-04-05 09:51:35.257000 nonebot_plugin_bilichat-5.3.1/nonebot_plugin_bilichat/archive/adapters/__init__.py
--rw-r--r--   0        0        0     4461 2024-04-05 09:51:35.257000 nonebot_plugin_bilichat-5.3.1/nonebot_plugin_bilichat/archive/adapters/base_content_parsing.py
--rw-r--r--   0        0        0     5849 2024-04-05 09:51:35.257000 nonebot_plugin_bilichat-5.3.1/nonebot_plugin_bilichat/archive/adapters/mirai2.py
--rw-r--r--   0        0        0     5086 2024-04-05 09:51:35.257000 nonebot_plugin_bilichat-5.3.1/nonebot_plugin_bilichat/archive/adapters/onebot_v11.py
--rw-r--r--   0        0        0     5154 2024-04-05 09:51:35.257000 nonebot_plugin_bilichat-5.3.1/nonebot_plugin_bilichat/archive/adapters/onebot_v12.py
--rw-r--r--   0        0        0     4265 2024-04-05 09:51:35.257000 nonebot_plugin_bilichat-5.3.1/nonebot_plugin_bilichat/archive/adapters/qq.py
--rw-r--r--   0        0        0     8064 2024-04-05 09:51:35.257000 nonebot_plugin_bilichat-5.3.1/nonebot_plugin_bilichat/base_content_parsing.py
--rw-r--r--   0        0        0       60 2024-04-05 09:51:35.257000 nonebot_plugin_bilichat-5.3.1/nonebot_plugin_bilichat/commands/__init__.py
--rw-r--r--   0        0        0     1288 2024-04-05 09:51:35.257000 nonebot_plugin_bilichat-5.3.1/nonebot_plugin_bilichat/commands/auto_delete_subs.py
--rw-r--r--   0        0        0      996 2024-04-05 09:51:35.257000 nonebot_plugin_bilichat-5.3.1/nonebot_plugin_bilichat/commands/base.py
--rw-r--r--   0        0        0      892 2024-04-05 09:51:35.257000 nonebot_plugin_bilichat-5.3.1/nonebot_plugin_bilichat/commands/functions.py
--rw-r--r--   0        0        0     3845 2024-04-05 09:51:35.257000 nonebot_plugin_bilichat-5.3.1/nonebot_plugin_bilichat/commands/login.py
--rw-r--r--   0        0        0     5230 2024-04-05 09:51:35.257000 nonebot_plugin_bilichat-5.3.1/nonebot_plugin_bilichat/commands/subs.py
--rw-r--r--   0        0        0     4996 2024-04-05 09:51:35.257000 nonebot_plugin_bilichat-5.3.1/nonebot_plugin_bilichat/commands/subs_cfg.py
--rw-r--r--   0        0        0     9295 2024-04-05 09:51:35.257000 nonebot_plugin_bilichat-5.3.1/nonebot_plugin_bilichat/config.py
--rw-r--r--   0        0        0       81 2024-04-05 09:51:35.257000 nonebot_plugin_bilichat-5.3.1/nonebot_plugin_bilichat/content/__init__.py
--rw-r--r--   0        0        0     3197 2024-04-05 09:51:35.257000 nonebot_plugin_bilichat-5.3.1/nonebot_plugin_bilichat/content/column.py
--rw-r--r--   0        0        0     4233 2024-04-05 09:51:35.257000 nonebot_plugin_bilichat-5.3.1/nonebot_plugin_bilichat/content/dynamic.py
--rw-r--r--   0        0        0     3975 2024-04-05 09:51:35.257000 nonebot_plugin_bilichat-5.3.1/nonebot_plugin_bilichat/content/video.py
--rw-r--r--   0        0        0      518 2024-04-05 09:51:35.257000 nonebot_plugin_bilichat-5.3.1/nonebot_plugin_bilichat/lib/b23_extract.py
--rw-r--r--   0        0        0     6192 2024-04-05 09:51:35.257000 nonebot_plugin_bilichat-5.3.1/nonebot_plugin_bilichat/lib/bcut_asr.py
--rw-r--r--   0        0        0      506 2024-04-05 09:51:35.257000 nonebot_plugin_bilichat-5.3.1/nonebot_plugin_bilichat/lib/bilibili_request/__init__.py
--rw-r--r--   0        0        0     2406 2024-04-05 09:51:35.257000 nonebot_plugin_bilichat-5.3.1/nonebot_plugin_bilichat/lib/bilibili_request/auth.py
--rw-r--r--   0        0        0      966 2024-04-05 09:51:35.257000 nonebot_plugin_bilichat-5.3.1/nonebot_plugin_bilichat/lib/bilibili_request/gRPC.py
--rw-r--r--   0        0        0     2653 2024-04-05 09:51:35.257000 nonebot_plugin_bilichat-5.3.1/nonebot_plugin_bilichat/lib/bilibili_request/restAPI.py
--rw-r--r--   0        0        0     2653 2024-04-05 09:51:35.257000 nonebot_plugin_bilichat-5.3.1/nonebot_plugin_bilichat/lib/browser.py
--rw-r--r--   0        0        0      444 2024-04-05 09:51:35.257000 nonebot_plugin_bilichat-5.3.1/nonebot_plugin_bilichat/lib/cache/__init__.py
--rw-r--r--   0        0        0      437 2024-04-05 09:51:35.257000 nonebot_plugin_bilichat-5.3.1/nonebot_plugin_bilichat/lib/cache/cache.py
--rw-r--r--   0        0        0      870 2024-04-05 09:51:35.257000 nonebot_plugin_bilichat-5.3.1/nonebot_plugin_bilichat/lib/cache/json_cache.py
--rw-r--r--   0        0        0      531 2024-04-05 09:51:35.257000 nonebot_plugin_bilichat-5.3.1/nonebot_plugin_bilichat/lib/cache/mongo_cache.py
--rw-r--r--   0        0        0      521 2024-04-05 09:51:35.257000 nonebot_plugin_bilichat-5.3.1/nonebot_plugin_bilichat/lib/draw/__init__.py
--rw-r--r--   0        0        0      217 2024-04-05 09:51:35.257000 nonebot_plugin_bilichat-5.3.1/nonebot_plugin_bilichat/lib/draw/column/__init__.py
--rw-r--r--   0        0        0     3189 2024-04-05 09:51:35.257000 nonebot_plugin_bilichat-5.3.1/nonebot_plugin_bilichat/lib/draw/column/browser_shot.py
--rw-r--r--   0        0        0      220 2024-04-05 09:51:35.257000 nonebot_plugin_bilichat-5.3.1/nonebot_plugin_bilichat/lib/draw/dynamic/__init__.py
--rw-r--r--   0        0        0     5103 2024-04-05 09:51:35.257000 nonebot_plugin_bilichat-5.3.1/nonebot_plugin_bilichat/lib/draw/dynamic/browser_shot.py
--rw-r--r--   0        0        0     1160 2024-04-05 09:51:35.257000 nonebot_plugin_bilichat-5.3.1/nonebot_plugin_bilichat/lib/draw/dynamic/dynamicrender.py
--rw-r--r--   0        0        0     7333 2024-04-05 09:51:35.257000 nonebot_plugin_bilichat-5.3.1/nonebot_plugin_bilichat/lib/draw/video/__init__.py
--rw-r--r--   0        0        0     6326 2024-04-05 09:51:35.257000 nonebot_plugin_bilichat-5.3.1/nonebot_plugin_bilichat/lib/draw/video/bbot_default.py
--rw-r--r--   0        0        0     2950 2024-04-05 09:51:35.257000 nonebot_plugin_bilichat-5.3.1/nonebot_plugin_bilichat/lib/draw/video/style_blue.py
--rw-r--r--   0        0        0     3794 2024-04-05 09:51:35.257000 nonebot_plugin_bilichat-5.3.1/nonebot_plugin_bilichat/lib/fetch_dynamic.py
--rw-r--r--   0        0        0     3376 2024-04-05 09:51:35.257000 nonebot_plugin_bilichat-5.3.1/nonebot_plugin_bilichat/lib/fonts_provider.py
--rw-r--r--   0        0        0      546 2024-04-05 09:51:35.257000 nonebot_plugin_bilichat-5.3.1/nonebot_plugin_bilichat/lib/store.py
--rw-r--r--   0        0        0     3115 2024-04-05 09:51:35.257000 nonebot_plugin_bilichat-5.3.1/nonebot_plugin_bilichat/lib/strings.py
--rw-r--r--   0        0        0     3263 2024-04-05 09:51:35.257000 nonebot_plugin_bilichat-5.3.1/nonebot_plugin_bilichat/lib/text_to_image.py
--rw-r--r--   0        0        0     1732 2024-04-05 09:51:35.257000 nonebot_plugin_bilichat-5.3.1/nonebot_plugin_bilichat/lib/tools.py
--rw-r--r--   0        0        0     1788 2024-04-05 09:51:35.257000 nonebot_plugin_bilichat-5.3.1/nonebot_plugin_bilichat/lib/uid_extract.py
--rw-r--r--   0        0        0     4033 2024-04-05 09:51:35.261000 nonebot_plugin_bilichat-5.3.1/nonebot_plugin_bilichat/lib/video_subtitle.py
--rw-r--r--   0        0        0      568 2024-04-05 09:51:35.261000 nonebot_plugin_bilichat-5.3.1/nonebot_plugin_bilichat/model/api/__init__.py
--rw-r--r--   0        0        0      184 2024-04-05 09:51:35.261000 nonebot_plugin_bilichat-5.3.1/nonebot_plugin_bilichat/model/api/bilibili_auth.py
--rw-r--r--   0        0        0      824 2024-04-05 09:51:35.261000 nonebot_plugin_bilichat-5.3.1/nonebot_plugin_bilichat/model/api/subs_config.py
--rw-r--r--   0        0        0      341 2024-04-05 09:51:35.261000 nonebot_plugin_bilichat-5.3.1/nonebot_plugin_bilichat/model/arguments.py
--rw-r--r--   0        0        0     3019 2024-04-05 09:51:35.261000 nonebot_plugin_bilichat-5.3.1/nonebot_plugin_bilichat/model/bcut_asr.py
--rw-r--r--   0        0        0     1326 2024-04-05 09:51:35.261000 nonebot_plugin_bilichat-5.3.1/nonebot_plugin_bilichat/model/bilibili/live.py
--rw-r--r--   0        0        0     1040 2024-04-05 09:51:35.261000 nonebot_plugin_bilichat-5.3.1/nonebot_plugin_bilichat/model/bilibili/summary.py
--rw-r--r--   0        0        0      806 2024-04-05 09:51:35.261000 nonebot_plugin_bilichat-5.3.1/nonebot_plugin_bilichat/model/exception.py
--rw-r--r--   0        0        0      323 2024-04-05 09:51:35.261000 nonebot_plugin_bilichat-5.3.1/nonebot_plugin_bilichat/model/openai.py
--rw-r--r--   0        0        0      277 2024-04-05 09:51:35.261000 nonebot_plugin_bilichat-5.3.1/nonebot_plugin_bilichat/optional.py
--rw-r--r--   0        0        0     9390 2024-04-05 09:51:35.261000 nonebot_plugin_bilichat-5.3.1/nonebot_plugin_bilichat/static/browser/mobile_style.js
--rw-r--r--   0        0        0     1187 2024-04-05 09:51:35.261000 nonebot_plugin_bilichat-5.3.1/nonebot_plugin_bilichat/static/style_blue/assets/business.png
--rw-r--r--   0        0        0     1200 2024-04-05 09:51:35.261000 nonebot_plugin_bilichat-5.3.1/nonebot_plugin_bilichat/static/style_blue/assets/personal.png
--rw-r--r--   0        0        0    93905 2024-04-05 09:51:35.261000 nonebot_plugin_bilichat-5.3.1/nonebot_plugin_bilichat/static/style_blue/assets/video_bottom.png
--rw-r--r--   0        0        0     7545 2024-04-05 09:51:35.261000 nonebot_plugin_bilichat-5.3.1/nonebot_plugin_bilichat/static/style_blue/video-details.html
--rw-r--r--   0        0        0     5777 2024-04-05 09:51:35.261000 nonebot_plugin_bilichat-5.3.1/nonebot_plugin_bilichat/static/summary/bilibili.png
--rw-r--r--   0        0        0     2098 2024-04-05 09:51:35.261000 nonebot_plugin_bilichat-5.3.1/nonebot_plugin_bilichat/static/summary/index.html
--rw-r--r--   0        0        0    47433 2024-04-05 09:51:35.261000 nonebot_plugin_bilichat-5.3.1/nonebot_plugin_bilichat/static/summary/marked.min.js
--rw-r--r--   0        0        0    59199 2024-04-05 09:51:35.261000 nonebot_plugin_bilichat-5.3.1/nonebot_plugin_bilichat/static/summary/openai.png
--rw-r--r--   0        0        0     9556 2024-04-05 09:51:35.261000 nonebot_plugin_bilichat-5.3.1/nonebot_plugin_bilichat/static/upload-webui.html
--rw-r--r--   0        0        0   300664 2024-04-05 09:51:35.261000 nonebot_plugin_bilichat-5.3.1/nonebot_plugin_bilichat/static/webui.tar.gz
--rw-r--r--   0        0        0     2685 2024-04-05 09:51:35.261000 nonebot_plugin_bilichat-5.3.1/nonebot_plugin_bilichat/subscribe/__init__.py
--rw-r--r--   0        0        0     7223 2024-04-05 09:51:35.261000 nonebot_plugin_bilichat-5.3.1/nonebot_plugin_bilichat/subscribe/dynamic.py
--rw-r--r--   0        0        0     4022 2024-04-05 09:51:35.261000 nonebot_plugin_bilichat-5.3.1/nonebot_plugin_bilichat/subscribe/live.py
--rw-r--r--   0        0        0    14446 2024-04-05 09:51:35.261000 nonebot_plugin_bilichat-5.3.1/nonebot_plugin_bilichat/subscribe/manager.py
--rw-r--r--   0        0        0      650 2024-04-05 09:51:35.261000 nonebot_plugin_bilichat-5.3.1/nonebot_plugin_bilichat/summary/__init__.py
--rw-r--r--   0        0        0     4935 2024-04-05 09:51:35.261000 nonebot_plugin_bilichat-5.3.1/nonebot_plugin_bilichat/summary/openai.py
--rw-r--r--   0        0        0     2467 2024-04-05 09:51:35.261000 nonebot_plugin_bilichat-5.3.1/nonebot_plugin_bilichat/summary/openai_summarise.py
--rw-r--r--   0        0        0     1691 2024-04-05 09:51:35.261000 nonebot_plugin_bilichat-5.3.1/nonebot_plugin_bilichat/wordcloud/wordcloud.py
--rw-r--r--   0        0        0     1780 2024-04-05 09:51:38.869015 nonebot_plugin_bilichat-5.3.1/pyproject.toml
--rw-r--r--   0        0        0    19518 1970-01-01 00:00:00.000000 nonebot_plugin_bilichat-5.3.1/PKG-INFO
+-rw-r--r--   0        0        0    34523 2024-04-06 17:23:14.558272 nonebot_plugin_bilichat-5.3.2/LICENSE
+-rw-r--r--   0        0        0    17886 2024-04-06 17:23:14.558272 nonebot_plugin_bilichat-5.3.2/README.md
+-rw-r--r--   0        0        0     2799 2024-04-06 17:23:14.578272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/__init__.py
+-rw-r--r--   0        0        0     1120 2024-04-06 17:23:14.578272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/api/__init__.py
+-rw-r--r--   0        0        0      740 2024-04-06 17:23:14.578272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/api/base.py
+-rw-r--r--   0        0        0     2232 2024-04-06 17:23:14.578272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/api/bilibili_auth.py
+-rw-r--r--   0        0        0     1647 2024-04-06 17:23:14.578272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/api/subs_config.py
+-rw-r--r--   0        0        0     2686 2024-04-06 17:23:14.578272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/api/webui.py
+-rw-r--r--   0        0        0     7742 2024-04-06 17:23:14.578272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/base_content_parsing.py
+-rw-r--r--   0        0        0       60 2024-04-06 17:23:14.578272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/commands/__init__.py
+-rw-r--r--   0        0        0     1300 2024-04-06 17:23:14.578272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/commands/auto_delete_subs.py
+-rw-r--r--   0        0        0      996 2024-04-06 17:23:14.578272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/commands/base.py
+-rw-r--r--   0        0        0      892 2024-04-06 17:23:14.578272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/commands/functions.py
+-rw-r--r--   0        0        0     3845 2024-04-06 17:23:14.578272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/commands/login.py
+-rw-r--r--   0        0        0     5230 2024-04-06 17:23:14.578272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/commands/subs.py
+-rw-r--r--   0        0        0     4996 2024-04-06 17:23:14.578272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/commands/subs_cfg.py
+-rw-r--r--   0        0        0     9273 2024-04-06 17:23:14.578272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/config.py
+-rw-r--r--   0        0        0       81 2024-04-06 17:23:14.578272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/content/__init__.py
+-rw-r--r--   0        0        0     3166 2024-04-06 17:23:14.578272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/content/column.py
+-rw-r--r--   0        0        0     4233 2024-04-06 17:23:14.578272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/content/dynamic.py
+-rw-r--r--   0        0        0     3942 2024-04-06 17:23:14.578272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/content/video.py
+-rw-r--r--   0        0        0      518 2024-04-06 17:23:14.578272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/lib/b23_extract.py
+-rw-r--r--   0        0        0     6192 2024-04-06 17:23:14.578272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/lib/bcut_asr.py
+-rw-r--r--   0        0        0      506 2024-04-06 17:23:14.578272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/lib/bilibili_request/__init__.py
+-rw-r--r--   0        0        0     2406 2024-04-06 17:23:14.578272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/lib/bilibili_request/auth.py
+-rw-r--r--   0        0        0      966 2024-04-06 17:23:14.578272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/lib/bilibili_request/gRPC.py
+-rw-r--r--   0        0        0     2653 2024-04-06 17:23:14.578272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/lib/bilibili_request/restAPI.py
+-rw-r--r--   0        0        0     2657 2024-04-06 17:23:14.578272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/lib/browser.py
+-rw-r--r--   0        0        0      456 2024-04-06 17:23:14.578272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/lib/cache/__init__.py
+-rw-r--r--   0        0        0      437 2024-04-06 17:23:14.578272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/lib/cache/cache.py
+-rw-r--r--   0        0        0      871 2024-04-06 17:23:14.578272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/lib/cache/json_cache.py
+-rw-r--r--   0        0        0      531 2024-04-06 17:23:14.578272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/lib/cache/mongo_cache.py
+-rw-r--r--   0        0        0      521 2024-04-06 17:23:14.578272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/lib/draw/__init__.py
+-rw-r--r--   0        0        0      217 2024-04-06 17:23:14.578272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/lib/draw/column/__init__.py
+-rw-r--r--   0        0        0     3262 2024-04-06 17:23:14.578272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/lib/draw/column/browser_shot.py
+-rw-r--r--   0        0        0      220 2024-04-06 17:23:14.578272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/lib/draw/dynamic/__init__.py
+-rw-r--r--   0        0        0     5145 2024-04-06 17:23:14.578272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/lib/draw/dynamic/browser_shot.py
+-rw-r--r--   0        0        0     1160 2024-04-06 17:23:14.578272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/lib/draw/dynamic/dynamicrender.py
+-rw-r--r--   0        0        0     7333 2024-04-06 17:23:14.578272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/lib/draw/video/__init__.py
+-rw-r--r--   0        0        0     6326 2024-04-06 17:23:14.578272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/lib/draw/video/bbot_default.py
+-rw-r--r--   0        0        0     3040 2024-04-06 17:23:14.578272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/lib/draw/video/style_blue.py
+-rw-r--r--   0        0        0     3796 2024-04-06 17:23:14.578272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/lib/fetch_dynamic.py
+-rw-r--r--   0        0        0     3376 2024-04-06 17:23:14.578272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/lib/fonts_provider.py
+-rw-r--r--   0        0        0      525 2024-04-06 17:23:14.578272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/lib/store.py
+-rw-r--r--   0        0        0     3115 2024-04-06 17:23:14.578272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/lib/strings.py
+-rw-r--r--   0        0        0     3329 2024-04-06 17:23:14.578272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/lib/text_to_image.py
+-rw-r--r--   0        0        0     1732 2024-04-06 17:23:14.578272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/lib/tools.py
+-rw-r--r--   0        0        0     1788 2024-04-06 17:23:14.578272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/lib/uid_extract.py
+-rw-r--r--   0        0        0     4033 2024-04-06 17:23:14.578272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/lib/video_subtitle.py
+-rw-r--r--   0        0        0      568 2024-04-06 17:23:14.578272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/model/api/__init__.py
+-rw-r--r--   0        0        0      184 2024-04-06 17:23:14.578272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/model/api/bilibili_auth.py
+-rw-r--r--   0        0        0      824 2024-04-06 17:23:14.578272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/model/api/subs_config.py
+-rw-r--r--   0        0        0      341 2024-04-06 17:23:14.578272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/model/arguments.py
+-rw-r--r--   0        0        0     3019 2024-04-06 17:23:14.578272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/model/bcut_asr.py
+-rw-r--r--   0        0        0     1326 2024-04-06 17:23:14.578272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/model/bilibili/live.py
+-rw-r--r--   0        0        0     1040 2024-04-06 17:23:14.578272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/model/bilibili/summary.py
+-rw-r--r--   0        0        0     1163 2024-04-06 17:23:14.578272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/model/exception.py
+-rw-r--r--   0        0        0      323 2024-04-06 17:23:14.578272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/model/openai.py
+-rw-r--r--   0        0        0      270 2024-04-06 17:23:14.578272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/optional.py
+-rw-r--r--   0        0        0     9390 2024-04-06 17:23:14.578272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/static/browser/mobile_style.js
+-rw-r--r--   0        0        0     1187 2024-04-06 17:23:14.578272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/static/style_blue/assets/business.png
+-rw-r--r--   0        0        0     1200 2024-04-06 17:23:14.578272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/static/style_blue/assets/personal.png
+-rw-r--r--   0        0        0    93905 2024-04-06 17:23:14.578272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/static/style_blue/assets/video_bottom.png
+-rw-r--r--   0        0        0     7545 2024-04-06 17:23:14.578272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/static/style_blue/video-details.html
+-rw-r--r--   0        0        0     5777 2024-04-06 17:23:14.578272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/static/summary/bilibili.png
+-rw-r--r--   0        0        0     2098 2024-04-06 17:23:14.578272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/static/summary/index.html
+-rw-r--r--   0        0        0    47433 2024-04-06 17:23:14.582272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/static/summary/marked.min.js
+-rw-r--r--   0        0        0    59199 2024-04-06 17:23:14.582272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/static/summary/openai.png
+-rw-r--r--   0        0        0     9556 2024-04-06 17:23:14.582272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/static/upload-webui.html
+-rw-r--r--   0        0        0   300664 2024-04-06 17:23:14.582272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/static/webui.tar.gz
+-rw-r--r--   0        0        0     2623 2024-04-06 17:23:14.582272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/subscribe/__init__.py
+-rw-r--r--   0        0        0     7217 2024-04-06 17:23:14.582272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/subscribe/dynamic.py
+-rw-r--r--   0        0        0     4023 2024-04-06 17:23:14.582272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/subscribe/live.py
+-rw-r--r--   0        0        0    14427 2024-04-06 17:23:14.582272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/subscribe/manager.py
+-rw-r--r--   0        0        0      478 2024-04-06 17:23:14.582272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/summary/__init__.py
+-rw-r--r--   0        0        0     4931 2024-04-06 17:23:14.582272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/summary/openai.py
+-rw-r--r--   0        0        0     2268 2024-04-06 17:23:14.582272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/summary/openai_summarise.py
+-rw-r--r--   0        0        0     1655 2024-04-06 17:23:14.582272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/wordcloud.py
+-rw-r--r--   0        0        0     1780 2024-04-06 17:23:17.694267 nonebot_plugin_bilichat-5.3.2/pyproject.toml
+-rw-r--r--   0        0        0    19586 1970-01-01 00:00:00.000000 nonebot_plugin_bilichat-5.3.2/PKG-INFO
```

### Comparing `nonebot_plugin_bilichat-5.3.1/LICENSE` & `nonebot_plugin_bilichat-5.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.3.1/README.md` & `nonebot_plugin_bilichat-5.3.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -71,24 +71,14 @@
 <details>
 <summary>视频总结</summary>
 
 ![](docs/summary.png)
 
 </details>
 
-## 🔌 适配器
-
-| 项目       | 视频解析 | 关注订阅 |
-| ---------- | -------- | -------- |
-| Onebot V11 | ✅       | ✅(SAA)  |
-| Onebot V12 | ✅       | ✅(SAA)  |
-| mirai2     | ✅       | ✅(SAA)  |
-| qq (频道)  | ✅       | ⏳(SAA)  |
-| qq (群)    | ⏳       | ❌       |
-
 ## 💿 安装
 
 > Linux 用户在安装时如果出现 `libGL.so.1: cannot open shared object file: No such file or directory` 错误，说明缺少 OpenGL 的运行环境，可以参考 [dynamicrender](https://pypi.org/project/dynrender-skia/) 中的 README 安装对应的依赖后重试
 
 <details>
 <summary>使用 nb-cli 安装</summary>
 在 nonebot2 项目的根目录下打开命令行, 输入以下指令即可安装
@@ -162,32 +152,33 @@
 bilichat_openai_token = sk-xxxxxxx
 # 网络代理
 bilichat_openai_proxy = "http://127.0.0.1:7890/"
 ```
 
 ### 通用配置项
 
-|         配置项          |   类型    |  默认值  |                               说明                               |
-| :---------------------: | :-------: | :------: | :--------------------------------------------------------------: |
-|     bilichat_block      |   bool    |  False   |                是否拦截事件(防止其他插件二次解析)                |
-|  bilichat_enable_self   |   bool    |  False   |                      是否允许响应自身的消息                      |
-|   bilichat_only_self    |   bool    |  False   | 是否仅响应自身的消息，开启后会**覆盖全部其他规则**(人机合一特供) |
-|   bilichat_only_to_me   |   bool    |  False   |      非自身消息是否需要 `@机器人` 或使用机器人的昵称才响应       |
-|   bilichat_whitelist    | list[str] |    []    |                 **响应**的会话名单, 会覆盖黑名单                 |
-|   bilichat_blacklist    | list[str] |    []    |                       **不响应**的会话名单                       |
-|  bilichat_dynamic_font  |    str    |   None   |                   视频信息及词云图片使用的字体                   |
-|    bilichat_cd_time     |    int    |   120    |                对同一视频的响应冷却时间(防止刷屏)                |
-| bilichat_neterror_retry |    int    |    3     |                   对部分网络请求错误的尝试次数                   |
-|  bilichat_use_bcut_asr  |   bool    |   True   |             是否在**没有字幕时**调用必剪接口生成字幕             |
-| bilichat_show_error_msg |   bool    |   True   |                   是否在解析失败时发送错误信息                   |
-|  bilichat_use_browser   |   bool    |   Auto   |     是否使用浏览器，`Auto` 会根据是否含有相应的依赖进行选择      |
-|  bilichat_cache_serive  |    str    |   Auto   |         使用的缓存类型，可用类型包含 `json` 和 `mongodb`         |
-|   bilichat_text_fonts   |    str    | default  |          可供自定义的字体，仅作用于 dynamicrender 绘图           |
-|  bilichat_emoji_fonts   |    str    | default  |          可供自定义的字体，仅作用于 dynamicrender 绘图           |
-|   bilichat_webui_path   |    str    | bilichat |               WebUI 的路径，设置为空则不开启 WebUI               |
+|            配置项             |   类型    |  默认值  |                               说明                               |
+| :---------------------------: | :-------: | :------: | :--------------------------------------------------------------: |
+|        bilichat_block         |   bool    |  False   |                是否拦截事件(防止其他插件二次解析)                |
+|     bilichat_enable_self      |   bool    |  False   |                      是否允许响应自身的消息                      |
+|      bilichat_only_self       |   bool    |  False   | 是否仅响应自身的消息，开启后会**覆盖全部其他规则**(人机合一特供) |
+|      bilichat_only_to_me      |   bool    |  False   |      非自身消息是否需要 `@机器人` 或使用机器人的昵称才响应       |
+|      bilichat_whitelist       | list[str] |    []    |                 **响应**的会话名单, 会覆盖黑名单                 |
+|      bilichat_blacklist       | list[str] |    []    |                       **不响应**的会话名单                       |
+|     bilichat_dynamic_font     |    str    |   None   |                   视频信息及词云图片使用的字体                   |
+|       bilichat_cd_time        |    int    |   120    |                对同一视频的响应冷却时间(防止刷屏)                |
+|    bilichat_neterror_retry    |    int    |    3     |                   对部分网络请求错误的尝试次数                   |
+|     bilichat_use_bcut_asr     |   bool    |   True   |             是否在**没有字幕时**调用必剪接口生成字幕             |
+|    bilichat_show_error_msg    |   bool    |   True   |                   是否在解析失败时发送错误信息                   |
+|     bilichat_use_browser      |   bool    |   Auto   |     是否使用浏览器，`Auto` 会根据是否含有相应的依赖进行选择      |
+| bilichat_browser_shot_quality |    int    |    75    |      浏览器截图质量，取值范围 10-100，越高则截图的体积越大       |
+|     bilichat_cache_serive     |    str    |   Auto   |         使用的缓存类型，可用类型包含 `json` 和 `mongodb`         |
+|      bilichat_text_fonts      |    str    | default  |          可供自定义的字体，仅作用于 dynamicrender 绘图           |
+|     bilichat_emoji_fonts      |    str    | default  |          可供自定义的字体，仅作用于 dynamicrender 绘图           |
+|      bilichat_webui_path      |    str    | bilichat |               WebUI 的路径，设置为空则不开启 WebUI               |
 
 注:
 
 1. 由于 OneBot 协议未规定是否应上报自身事件，因此在不同的场景下能否获取自身事件并不一定，`bilichat_enable_self` 实际能否生效也与之相关
 2. 当 `bilichat_whitelist` 存在时，`bilichat_blacklist` 将会被禁用
 3. `bilichat_dynamic_font` 可填写自定义的字体 url，但并不推荐修改
 4. 当使用 `bcut_asr` 接口来生成 AI 字幕时，根据视频时长和网络情况有可能会识别失败，Bot 会提示 `BCut-ASR conversion failed due to network error`。可以通过调高 `bilichat_neterror_retry` 次数或几分钟后重试来尝试重新生成字幕
@@ -262,19 +253,18 @@
 
 </details>
 
 ### 词云配置项
 
 开启此功能需要安装对应的依赖 `nonebot-plugin-bilichat[wordcloud]`
 
-|       配置项        | 类型 | 默认值 |       说明       |
-| :-----------------: | :--: | :----: | :--------------: |
-| bilichat_word_cloud | bool | False  | 是否开启词云功能 |
-
-注：词云功能在 python3.11 中由于 `wordcloud` 包安装失败暂时无法启用，请不要在 3.11 中开启此功能
+|          配置项          |   类型    |   默认值    |       说明       |
+| :----------------------: | :-------: | :---------: | :--------------: |
+|   bilichat_word_cloud    |   bool    |    False    | 是否开启词云功能 |
+| bilichat_word_cloud_size | List[int] | [1000, 800] |   词云图片尺寸   |
 
 ### AI 视频总结配置项
 
 开启此功能需要安装对应的依赖 `nonebot-plugin-bilichat[summary]`
 
 |            配置项            | 类型 |       默认值       |                                      说明                                      |
 | :--------------------------: | :--: | :----------------: | :----------------------------------------------------------------------------: |
@@ -310,16 +300,14 @@
 |    指令    | 简写 |                        说明                        |
 | :--------: | :--: | :------------------------------------------------: |
 | --no-cache |  -n  |     本次总结禁用缓存(不会影响已存在的缓存文件)     |
 | --refresh  |  -r  | 刷新此视频的词云和总结缓存(会覆盖已存在的缓存文件) |
 
 ### 指令表
 
-> 此部分当前仅适配了 OneBot 11 ，如果有其他适配器的需求可以新建 issue 来提出
-
 指令部分由 `指令前缀` 和 `指令名` 组成，其中 `指令前缀` 包含 `COMMAND_START` `bilichat_cmd_start` `COMMAND_SEP` 三部分，默认的 `指令前缀` 为 `/bilichat.` ，即完整的指令为 `/bilichat.xxx`
 
 `指令前缀` 部分也是可以修改的，例如 .env 中填入如下设置即可实现无 `指令前缀`
 
 ```dotenv
 COMMAND_SEP=[""]
 COMMAND_START=[""]
@@ -344,18 +332,21 @@
 
 ## 🙏 感谢
 
 在此感谢以下开发者(项目)对本项目做出的贡献：
 
 -   [BibiGPT](https://github.com/JimmyLv/BibiGPT) 项目灵感来源
 -   [bilibili-API-collect](https://github.com/SocialSisterYi/bilibili-API-collect) 易姐收集的各种 BiliBili Api 及其提供的 gRPC Api 调用方案
+-   [HarukaBot](https://github.com/SK-415/HarukaBot) 功能来源
 -   [BBot-Graia](https://github.com/djkcyl/BBot-Graia) 功能来源 ~~(我 牛 我 自 己)~~
 -   [ABot-Graia](https://github.com/djkcyl/ABot-Graia) 永远怀念最好的 ABot 🙏
+-   [bilireq](https://github.com/SK-415/bilireq) 项目使用的 bilibili 请求库
 -   [nonebot-plugin-template](https://github.com/A-kirami/nonebot-plugin-template): 项目的 README 模板
 -   [Misaka-Mikoto-Tech](https://github.com/Misaka-Mikoto-Tech) 为本项目提交了多项 BUG 修复和代码参考
 -   [hamo-reid](https://github.com/hamo-reid) 为 style_blue 绘制了界面
 -   [dynamicrender](https://pypi.org/project/dynrender-skia/) 提供 t2i 和动态渲染
 -   [SAA](https://github.com/MountainDash/nonebot-plugin-send-anything-anywhere) 提供指令及订阅部分的跨平台支持
+-   [ALC](https://github.com/nonebot/plugin-alconna) 提供跨平台支持
 
 ## ⏳ Star 趋势
 
 [![Stargazers over time](https://starchart.cc/djkcyl/nonebot-plugin-bilichat.svg)](https://starchart.cc/djkcyl/nonebot-plugin-bilichat)
```

#### html2text {}

```diff
@@ -3,20 +3,17 @@
    # nonebot-plugin-bilichat _â¨ å¤åè½ç B ç«è§é¢è§£æå·¥å· â¨_
  _[_l_i_c_e_n_s_e_]_[_P_y_P_I_ _-_ _D_o_w_n_l_o_a_d_s_]_[_p_y_p_i_][python]_[_p_d_m_-_m_a_n_a_g_e_d_]_[_C_o_d_e_ _s_t_y_l_e_:_ _b_l_a_c_k_]_[_Q_Q
                           _C_h_a_t_ _G_r_o_u_p_]_[_Q_Q_ _C_h_a_t_ _G_r_o_u_p_]
 ## ð ä»ç»
 è§é¢é¾æ¥è§£æï¼å¹¶æ ¹æ®å¶åå®¹çæ**åºæ¬ä¿¡æ¯**ã**è¯äº**å**åå®¹æ»ç»**
 ææºç«¯è§å¾ ![](docs/mobile.png) åºæ¬ä¿¡æ¯ ![bbot_default](docs/
 bbot_default.png) ![style_blue](docs/style_blue.png) è¯äº ![](docs/
-wordcloud.png) è§é¢æ»ç» ![](docs/summary.png) ## ð ééå¨ | é¡¹ç® |
-è§é¢è§£æ | å³æ³¨è®¢é | | ---------- | -------- | -------- | | Onebot V11
-| â | â(SAA) | | Onebot V12 | â | â(SAA) | | mirai2 | â | â(SAA) |
-| qq (é¢é) | â | â³(SAA) | | qq (ç¾¤) | â³ | â | ## ð¿ å®è£ >
-Linux ç¨æ·å¨å®è£æ¶å¦æåºç° `libGL.so.1: cannot open shared object
-file: No such file or directory` éè¯¯ï¼è¯´æç¼ºå° OpenGL
+wordcloud.png) è§é¢æ»ç» ![](docs/summary.png) ## ð¿ å®è£ > Linux
+ç¨æ·å¨å®è£æ¶å¦æåºç° `libGL.so.1: cannot open shared object file: No
+such file or directory` éè¯¯ï¼è¯´æç¼ºå° OpenGL
 çè¿è¡ç¯å¢ï¼å¯ä»¥åè [dynamicrender](https://pypi.org/project/
 dynrender-skia/) ä¸­ç README å®è£å¯¹åºçä¾èµåéè¯ ä½¿ç¨ nb-cli
 å®è£ å¨ nonebot2 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡,
 è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ nb plugin install nonebot-plugin-bilichat æ³¨:
 ç±äº nb-cli ä¸æ¯æä¾èµç»ï¼å æ­¤éè¦å¯ç¨è¯äºå AI
 æ»ç»çç¨æ·è¦éè¿å¶ä»çåç®¡çå¨å®è£é¢å¤çä¾èµ pip install
 nonebot-plugin-bilichat[all] ä½¿ç¨åç®¡çå¨å®è£ å¨ nonebot2
@@ -32,17 +29,17 @@
 å¯¹åä¸è§é¢çååºå·å´æ¶é´(é²æ­¢å·å±) bilichat_cd_time = 120 #
 ç½ç»è¯·æ±éè¯æ¬¡æ° bilichat_neterror_retry = 3 #
 æ¯å¦ä½¿ç¨æµè§å¨æªå¾(éè¦é¢å¤ä¾èµ) bilichat_use_browser = True #
 æ¯å¦å¼å¯è¯äº(éè¦é¢å¤ä¾èµ) bilichat_word_cloud = True # === AI
 æ»ç»ç¸å³ === # å®æ¹æ»ç»æ¥å£ bilichat_official_summary = True # openai
 æ¥å£(éè¦é¢å¤ä¾èµ) bilichat_openai_token = sk-xxxxxxx # ç½ç»ä»£ç
 bilichat_openai_proxy = "http://127.0.0.1:7890/" ``` ### éç¨éç½®é¡¹ |
-éç½®é¡¹ | ç±»å | é»è®¤å¼ | è¯´æ | | :---------------------: | :-------:
-| :------: | :--------------------------------------------------------------: |
-| bilichat_block | bool | False | æ¯å¦æ¦æªäºä»¶
+éç½®é¡¹ | ç±»å | é»è®¤å¼ | è¯´æ | | :---------------------------: | :--
+-----: | :------: | :----------------------------------------------------------
+----: | | bilichat_block | bool | False | æ¯å¦æ¦æªäºä»¶
 (é²æ­¢å¶ä»æä»¶äºæ¬¡è§£æ) | | bilichat_enable_self | bool | False |
 æ¯å¦åè®¸ååºèªèº«çæ¶æ¯ | | bilichat_only_self | bool | False |
 æ¯å¦ä»ååºèªèº«çæ¶æ¯ï¼å¼å¯åä¼**è¦çå¨é¨å¶ä»è§å**
 (äººæºåä¸ç¹ä¾) | | bilichat_only_to_me | bool | False |
 éèªèº«æ¶æ¯æ¯å¦éè¦ `@æºå¨äºº` æä½¿ç¨æºå¨äººçæµç§°æååº |
 | bilichat_whitelist | list[str] | [] | **ååº**çä¼è¯åå,
 ä¼è¦çé»åå | | bilichat_blacklist | list[str] | [] |
@@ -51,17 +48,19 @@
 å¯¹åä¸è§é¢çååºå·å´æ¶é´(é²æ­¢å·å±) | | bilichat_neterror_retry
 | int | 3 | å¯¹é¨åç½ç»è¯·æ±éè¯¯çå°è¯æ¬¡æ° | |
 bilichat_use_bcut_asr | bool | True |
 æ¯å¦å¨**æ²¡æå­å¹æ¶**è°ç¨å¿åªæ¥å£çæå­å¹ | |
 bilichat_show_error_msg | bool | True |
 æ¯å¦å¨è§£æå¤±è´¥æ¶åééè¯¯ä¿¡æ¯ | | bilichat_use_browser | bool |
 Auto | æ¯å¦ä½¿ç¨æµè§å¨ï¼`Auto`
-ä¼æ ¹æ®æ¯å¦å«æç¸åºçä¾èµè¿è¡éæ© | | bilichat_cache_serive |
-str | Auto | ä½¿ç¨çç¼å­ç±»åï¼å¯ç¨ç±»ååå« `json` å `mongodb` |
-| bilichat_text_fonts | str | default | å¯ä¾èªå®ä¹çå­ä½ï¼ä»ä½ç¨äº
+ä¼æ ¹æ®æ¯å¦å«æç¸åºçä¾èµè¿è¡éæ© | |
+bilichat_browser_shot_quality | int | 75 | æµè§å¨æªå¾è´¨éï¼åå¼èå´
+10-100ï¼è¶é«åæªå¾çä½ç§¯è¶å¤§ | | bilichat_cache_serive | str | Auto
+| ä½¿ç¨çç¼å­ç±»åï¼å¯ç¨ç±»ååå« `json` å `mongodb` | |
+bilichat_text_fonts | str | default | å¯ä¾èªå®ä¹çå­ä½ï¼ä»ä½ç¨äº
 dynamicrender ç»å¾ | | bilichat_emoji_fonts | str | default |
 å¯ä¾èªå®ä¹çå­ä½ï¼ä»ä½ç¨äº dynamicrender ç»å¾ | |
 bilichat_webui_path | str | bilichat | WebUI
 çè·¯å¾ï¼è®¾ç½®ä¸ºç©ºåä¸å¼å¯ WebUI | æ³¨: 1. ç±äº OneBot
 åè®®æªè§å®æ¯å¦åºä¸æ¥èªèº«äºä»¶ï¼å æ­¤å¨ä¸åçåºæ¯ä¸è½å¦è·åèªèº«äºä»¶å¹¶ä¸ä¸å®ï¼`bilichat_enable_self`
 å®éè½å¦çæä¹ä¸ä¹ç¸å³ 2. å½ `bilichat_whitelist`
 å­å¨æ¶ï¼`bilichat_blacklist` å°ä¼è¢«ç¦ç¨ 3. `bilichat_dynamic_font`
@@ -113,19 +112,18 @@
 é¤é»è®¤ç dynamicrender ä½¿ç¨ Skia
 ç»å¾ï¼æªå¼å¯æµè§å¨æ¶é»è®¤éæ©ï¼ï¼å¶ä»åä¾èµäºæµè§å¨è¿è¡æ¸²æï¼éè¦è®¾ç½®
 bilichat_use_browser ä¸º True æ Autoï¼ï¼å¶å¯ç¨çæ ·å¼å¦ä¸æç¤º
 dynamicrender ï¼æ æµè§å¨æ¶é»è®¤ï¼ ![](docs/dynamicrender.jpg)
 browser_mobile ï¼ææµè§å¨æ¶é»è®¤ï¼ ![](docs/dynamic_mobile.jpg)
 browser_pc ![](docs/dynamic_pc.jpg) ### è¯äºéç½®é¡¹
 å¼å¯æ­¤åè½éè¦å®è£å¯¹åºçä¾èµ `nonebot-plugin-bilichat[wordcloud]`
-| éç½®é¡¹ | ç±»å | é»è®¤å¼ | è¯´æ | | :-----------------: | :--: | :---
--: | :--------------: | | bilichat_word_cloud | bool | False |
-æ¯å¦å¼å¯è¯äºåè½ | æ³¨ï¼è¯äºåè½å¨ python3.11 ä¸­ç±äº
-`wordcloud` åå®è£å¤±è´¥ææ¶æ æ³å¯ç¨ï¼è¯·ä¸è¦å¨ 3.11
-ä¸­å¼å¯æ­¤åè½ ### AI è§é¢æ»ç»éç½®é¡¹
+| éç½®é¡¹ | ç±»å | é»è®¤å¼ | è¯´æ | | :----------------------: | :-----
+--: | :---------: | :--------------: | | bilichat_word_cloud | bool | False |
+æ¯å¦å¼å¯è¯äºåè½ | | bilichat_word_cloud_size | List[int] | [1000, 800]
+| è¯äºå¾çå°ºå¯¸ | ### AI è§é¢æ»ç»éç½®é¡¹
 å¼å¯æ­¤åè½éè¦å®è£å¯¹åºçä¾èµ `nonebot-plugin-bilichat[summary]` |
 éç½®é¡¹ | ç±»å | é»è®¤å¼ | è¯´æ | | :--------------------------: | :--:
 | :----------------: | :-------------------------------------------------------
 ---------------------: | | bilichat_summary_ignore_null | bool | True |
 æ¯å¦å¿½ç¥æ æä¹çæ»ç»åå®¹ | | bilichat_official_summary | bool |
 False | æ¯å¦å¼å¯å®æ¹æ»ç»ï¼æ­¤æ»ç»ç¬ç«äºä¸æ¹ AI
 æ»ç»ï¼å¯ä¸ä¸æ¹ AI æ»ç»åæ¶çæ | | bilichat_openai_token | str |
@@ -146,20 +144,18 @@
 BV12v4y1E7NT --refresh BV12v4y1E7NT -r # å¯ä»¥ä½¿ç¨ç®å BV12v4y1E7NT -r --
 no-cache # å¯ä»¥å¤ä¸ªåæ°æ··ç¨ -r BV12v4y1E7NT -n #
 è½ç¶ä¸å»ºè®®ï¼ä½ç¡®å®å¯ä»¥æåæ°æ¾åé¢ ``` | æä»¤ | ç®å |
 è¯´æ | | :--------: | :--: | :-----------------------------------------------
 -: | | --no-cache | -n | æ¬æ¬¡æ»ç»ç¦ç¨ç¼å­
 (ä¸ä¼å½±åå·²å­å¨çç¼å­æä»¶) | | --refresh | -r |
 å·æ°æ­¤è§é¢çè¯äºåæ»ç»ç¼å­(ä¼è¦çå·²å­å¨çç¼å­æä»¶) |
-### æä»¤è¡¨ > æ­¤é¨åå½åä»ééäº OneBot 11
-ï¼å¦ææå¶ä»ééå¨çéæ±å¯ä»¥æ°å»º issue æ¥æåº
-æä»¤é¨åç± `æä»¤åç¼` å `æä»¤å` ç»æï¼å¶ä¸­ `æä»¤åç¼`
-åå« `COMMAND_START` `bilichat_cmd_start` `COMMAND_SEP` ä¸é¨åï¼é»è®¤ç
-`æä»¤åç¼` ä¸º `/bilichat.` ï¼å³å®æ´çæä»¤ä¸º `/bilichat.xxx`
-`æä»¤åç¼` é¨åä¹æ¯å¯ä»¥ä¿®æ¹çï¼ä¾å¦ .env
+### æä»¤è¡¨ æä»¤é¨åç± `æä»¤åç¼` å `æä»¤å` ç»æï¼å¶ä¸­
+`æä»¤åç¼` åå« `COMMAND_START` `bilichat_cmd_start` `COMMAND_SEP`
+ä¸é¨åï¼é»è®¤ç `æä»¤åç¼` ä¸º `/bilichat.` ï¼å³å®æ´çæä»¤ä¸º
+`/bilichat.xxx` `æä»¤åç¼` é¨åä¹æ¯å¯ä»¥ä¿®æ¹çï¼ä¾å¦ .env
 ä¸­å¡«å¥å¦ä¸è®¾ç½®å³å¯å®ç°æ  `æä»¤åç¼` ```dotenv COMMAND_SEP=[""]
 COMMAND_START=[""] bilichat_cmd_start="" ``` `æä»¤å`
 å¦ä¸è¡¨æç¤ºï¼å¶ä¸­é¤ç»å½ç¸å³çæä»¤åå¯èªå®ä¹ï¼å¯åèä¸æç
 [æä»¤åè®¢ééç½®é¡¹](#æä»¤åè®¢ééç½®é¡¹) | æä»¤ | æé |
 èå´ | åæ° | è¯´æ | | :----------: | :----: | :----: | :----------------
 --------------------: | :--------------------------------------: | | sub |
 ä¸»äºº | ç¾¤è | UP ä¸»çæµç§°æ UID | æ·»å è®¢é | | unsub | ä¸»äºº |
@@ -176,19 +172,22 @@
 checklogin | ä¸»äºº | æ éå¶ | æ  | æ¥çå½åå·²ç»å½çå¨é¨è´¦å· |
 | qrlogin | ä¸»äºº | æ éå¶ | æ  | ä½¿ç¨äºç»´ç ç»å½ B
 ç«ï¼é²æ­¢é£æ§ | | logout | ä¸»äºº | æ éå¶ | è´¦å·ç UID |
 ç»åºæå®çè´¦å· | ## ð æè°¢ å¨æ­¤æè°¢ä»¥ä¸å¼åè
 (é¡¹ç®)å¯¹æ¬é¡¹ç®ååºçè´¡ç®ï¼ - [BibiGPT](https://github.com/JimmyLv/
 BibiGPT) é¡¹ç®çµææ¥æº - [bilibili-API-collect](https://github.com/
 SocialSisterYi/bilibili-API-collect) æå§æ¶éçåç§ BiliBili Api
-åå¶æä¾ç gRPC Api è°ç¨æ¹æ¡ - [BBot-Graia](https://github.com/djkcyl/
-BBot-Graia) åè½æ¥æº ~~(æ ç æ èª å·±)~~ - [ABot-Graia](https://
-github.com/djkcyl/ABot-Graia) æ°¸è¿æå¿µæå¥½ç ABot ð - [nonebot-
+åå¶æä¾ç gRPC Api è°ç¨æ¹æ¡ - [HarukaBot](https://github.com/SK-415/
+HarukaBot) åè½æ¥æº - [BBot-Graia](https://github.com/djkcyl/BBot-Graia)
+åè½æ¥æº ~~(æ ç æ èª å·±)~~ - [ABot-Graia](https://github.com/
+djkcyl/ABot-Graia) æ°¸è¿æå¿µæå¥½ç ABot ð - [bilireq](https://
+github.com/SK-415/bilireq) é¡¹ç®ä½¿ç¨ç bilibili è¯·æ±åº - [nonebot-
 plugin-template](https://github.com/A-kirami/nonebot-plugin-template):
 é¡¹ç®ç README æ¨¡æ¿ - [Misaka-Mikoto-Tech](https://github.com/Misaka-
 Mikoto-Tech) ä¸ºæ¬é¡¹ç®æäº¤äºå¤é¡¹ BUG ä¿®å¤åä»£ç åè - [hamo-
 reid](https://github.com/hamo-reid) ä¸º style_blue ç»å¶äºçé¢ -
 [dynamicrender](https://pypi.org/project/dynrender-skia/) æä¾ t2i
 åå¨ææ¸²æ - [SAA](https://github.com/MountainDash/nonebot-plugin-send-
-anything-anywhere) æä¾æä»¤åè®¢éé¨åçè·¨å¹³å°æ¯æ ## â³ Star
-è¶å¿ [![Stargazers over time](https://starchart.cc/djkcyl/nonebot-plugin-
+anything-anywhere) æä¾æä»¤åè®¢éé¨åçè·¨å¹³å°æ¯æ - [ALC](https:
+//github.com/nonebot/plugin-alconna) æä¾è·¨å¹³å°æ¯æ ## â³ Star è¶å¿
+[![Stargazers over time](https://starchart.cc/djkcyl/nonebot-plugin-
 bilichat.svg)](https://starchart.cc/djkcyl/nonebot-plugin-bilichat)
```

### Comparing `nonebot_plugin_bilichat-5.3.1/nonebot_plugin_bilichat/__init__.py` & `nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 from nonebot import require
 from nonebot.plugin import PluginMetadata
 
 from .config import __version__, plugin_config, raw_config
 
 require("nonebot_plugin_apscheduler")
+require("nonebot_plugin_alconna")
 require("nonebot_plugin_saa")
 
 from nonebot_plugin_saa import enable_auto_select_bot  # noqa: E402
 
 enable_auto_select_bot()
 
 cmd_perfix = f"{raw_config.command_start}{plugin_config.bilichat_cmd_start}{raw_config.command_sep}"
 
 __plugin_meta__ = PluginMetadata(
     name="nonebot-plugin-bilichat",
     description="多种B站链接解析，视频词云，AI总结，你想要的都在 bilichat",
     usage="视频、专栏、动态解析直接发送链接、小程序、xml卡片即可，指令请参考 https://github.com/Well2333/nonebot-plugin-bilichat",
     homepage="https://github.com/Well2333/nonebot-plugin-bilichat",
     type="application",
-    supported_adapters={"~onebot.v11", "~onebot.v12", "~qqguild", "~mirai2"},
+    supported_adapters={"~onebot.v11", "~onebot.v12", "~qq", "~mirai2"},
     extra={
         "author": "djkcyl & Well404",
         "version": __version__,
         "priority": 1,
         "menu_data": [
             {
                 "func": "添加订阅",
```

### Comparing `nonebot_plugin_bilichat-5.3.1/nonebot_plugin_bilichat/api/__init__.py` & `nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/api/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.3.1/nonebot_plugin_bilichat/api/base.py` & `nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/api/base.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.3.1/nonebot_plugin_bilichat/api/bilibili_auth.py` & `nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/api/bilibili_auth.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.3.1/nonebot_plugin_bilichat/api/subs_config.py` & `nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/api/subs_config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.3.1/nonebot_plugin_bilichat/api/webui.py` & `nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/api/webui.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.3.1/nonebot_plugin_bilichat/base_content_parsing.py` & `nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/base_content_parsing.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,25 +12,22 @@
 from nonebot_plugin_alconna.uniseg import Hyper, Image, MsgTarget, Reply, Text, UniMessage, UniMsg
 
 from .config import plugin_config
 from .content import Column, Dynamic, Video
 from .lib.b23_extract import b23_extract
 from .lib.text_to_image import t2i
 from .model.arguments import Options
-from .model.exception import AbortError
+from .model.exception import AbortError, ProssesError
 from .optional import capture_exception
 
 if plugin_config.bilichat_openai_token:
-    ENABLE_SUMMARY = True
     from .summary import summarization
-else:
-    ENABLE_SUMMARY = False
 
 if plugin_config.bilichat_word_cloud:
-    from .wordcloud.wordcloud import wordcloud
+    from .wordcloud import wordcloud
 
 cd: Dict[str, int] = {}
 cd_size_limit = plugin_config.bilichat_cd_time // 2
 
 # 临时解决方案
 try:
     lock = asyncio.Lock()
@@ -50,18 +47,18 @@
     # not check cd
     if not check:
         cd[uid] = now + plugin_config.bilichat_cd_time
         return
     # check cd
     session, id_ = uid.split("_-_")
     if cd.get(uid, 0) > now:
-        logger.warning(f"Duplicate content {id_} from session {session}. Skip the video parsing process")
+        logger.warning(f"会话 [{session}] 的重复内容 [{id_}]. 跳过解析")
         raise FinishedException
     elif cd.get(id_, 0) > now:
-        logger.warning(f"Duplicate content {id_} from global. Skip the video parsing process")
+        logger.warning(f"会话 [全局] 的重复内容 [{id_}]. 跳过解析")
         raise FinishedException
     else:
         cd[uid] = now + plugin_config.bilichat_cd_time
 
 
 async def _permission_check(bot: Bot, event: Event, target: MsgTarget, state: T_State):
     # 自身消息
@@ -177,49 +174,46 @@
     future_msg = UniMessage()
     future_msg.append(reply)
 
     if isinstance(content, Video) and plugin_config.bilichat_official_summary:
         # 获取官方总结内容
         try:
             official_summary_response = await content.get_offical_summary()
-            official_summary = await t2i(data=official_summary_response.result.markdown(), src="bilibili")
-            if isinstance(official_summary, str):
+            official_summary = official_summary_response.result.markdown()
+            try:
+                future_msg.append(Image(raw=await t2i(data=official_summary, src="bilibili")))
+            except ProssesError:
                 future_msg.append(Text(official_summary))
-            elif isinstance(official_summary, bytes):
-                future_msg.append(Image(raw=official_summary))
-            else:
-                raise TypeError(f"未知的 official_summary 类型: {type(official_summary)}")
         except Exception as e:
             if not plugin_config.bilichat_summary_ignore_null:
                 future_msg.append(Text(f"当前视频不支持AI视频总结: {e}"))
     try:
         async with lock:
-            if ENABLE_SUMMARY or plugin_config.bilichat_word_cloud:
+            if plugin_config.bilichat_openai_token or plugin_config.bilichat_word_cloud:
                 subtitle = await content.get_subtitle()
                 if not subtitle:
                     raise AbortError("视频无有效字幕")
 
                 # wordcloud
                 if plugin_config.bilichat_word_cloud:
                     if wc_image := await wordcloud(cache=content.cache):
                         future_msg.append(Image(raw=wc_image))
 
                 # summary
-                if ENABLE_SUMMARY:
+                if plugin_config.bilichat_openai_token:
                     if summary := await summarization(cache=content.cache):
-                        if isinstance(summary, str):
-                            future_msg.append(Text(summary))
-                        elif isinstance(summary, bytes):
-                            future_msg.append(Image(raw=summary))
+                        future_msg.append(Image(raw=summary))
 
     except FinishedException:
         raise
     except AbortError as e:
         if plugin_config.bilichat_show_error_msg:
             future_msg.append(Text(str(e)))
+    except ProssesError as e:
+        future_msg.append(Text(str(e)))
     except Exception as e:
         capture_exception()
         logger.exception(e)
         if plugin_config.bilichat_show_error_msg:
             future_msg.append(Text(str(e)))
 
     if len(future_msg) > 1:
```

### Comparing `nonebot_plugin_bilichat-5.3.1/nonebot_plugin_bilichat/commands/auto_delete_subs.py` & `nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/commands/auto_delete_subs.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from ..subscribe.manager import CONFIG_LOCK, SubscriptionSystem, User
 
 auto_delete_subs = on_notice(block=False)
 
 
 async def remove_sub(target: SaaTarget):
     platform, user_id = User.extract_saa_target(target)
-    logger.info(f"remove subs from {user_id}")
+    logger.info(f"移除用户 {user_id} 的全部订阅")
     async with CONFIG_LOCK:
         if user := SubscriptionSystem.users.get(f"{platform}-_-{user_id}"):
             for up in user.subscribe_ups:
                 await user.remove_subscription(up)
         SubscriptionSystem.save_to_file()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `nonebot_plugin_bilichat-5.3.1/nonebot_plugin_bilichat/commands/base.py` & `nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/commands/base.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.3.1/nonebot_plugin_bilichat/commands/functions.py` & `nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/commands/functions.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.3.1/nonebot_plugin_bilichat/commands/login.py` & `nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/commands/login.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.3.1/nonebot_plugin_bilichat/commands/subs.py` & `nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/commands/subs.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.3.1/nonebot_plugin_bilichat/commands/subs_cfg.py` & `nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/commands/subs_cfg.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.3.1/nonebot_plugin_bilichat/config.py` & `nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/config.py`

 * *Files 10% similar despite different names*

```diff
@@ -30,14 +30,15 @@
     bilichat_only_to_me: bool = False
     bilichat_whitelist: List[str] = []
     bilichat_blacklist: List[str] = []
     bilichat_cd_time: int = 120
     bilichat_neterror_retry: int = 3
     bilichat_show_error_msg: bool = True
     bilichat_use_browser: bool = Field(default="Auto")
+    bilichat_browser_shot_quality: int = Field(default=75, ge=10, le=100)
     bilichat_cache_serive: Literal["json", "mongodb"] = Field(default="Auto")
     bilichat_text_fonts: str = "default"
     bilichat_emoji_fonts: str = "default"
     bilichat_webui_path: Optional[str] = "bilichat"
 
     # command and subscribe
     bilichat_command_to_me: bool = True
@@ -66,14 +67,15 @@
     bilichat_bilibili_cookie: Optional[str] = None
 
     # both WC and AI
     bilichat_use_bcut_asr: bool = True
 
     # Word Cloud
     bilichat_word_cloud: bool = False
+    bilichat_word_cloud_size: List[int] = [1000, 800]
 
     # AI Summary
     bilichat_summary_ignore_null: bool = True
     bilichat_official_summary: bool = False
     bilichat_openai_token: Optional[str] = None
     bilichat_openai_proxy: Optional[str] = None
     bilichat_openai_model: Literal[
@@ -93,104 +95,100 @@
     @validator("bilichat_cache_serive", always=True, pre=True)
     def check_cache_serive(cls, v):
         if v == "json":
             return v
         try:
             require("nonebot_plugin_mongodb")
             if v == "Auto":
-                logger.info("bilichat_cache_serive can use MongoDB as cache serive")
+                logger.info("bilichat_cache_serive 可以使用 MongoDB 作为缓存服务")
             return "mongodb"
         except Exception as e:
             if v == "Auto":
-                logger.info("bilichat_cache_serive can't use MongoDB as cache serive, using JsonFile")
+                logger.info("bilichat_cache_serive 无法使用 MongoDB 作为缓存服务, 使用 JSON 文件作为缓存服务")
                 return "json"
             raise RuntimeError(
-                "Package(s) of MongoDB not installed, "
-                "use **pip install nonebot-plugin-bilichat[all]** to install required dependencies"
+                "未安装 MongoDB 所需依赖, 使用 **pip install nonebot-plugin-bilichat[all]** 来安装所需依赖"
             ) from e
 
     @validator("bilichat_use_browser", always=True, pre=True)
     def check_htmlrender(cls, v):
         if not v:
             return v
         try:
             require("nonebot_plugin_htmlrender")
             if v == "Auto":
-                logger.info("bilichat_use_browser dependencies have been satisfied, enable bilichat_use_browser")
+                logger.info("bilichat_use_browser 所需依赖已安装，采用浏览器渲染模式")
             return True
         except Exception as e:
             if v == "Auto":
-                logger.info("bilichat_use_browser's dependency is not satisfied, disable bilichat_use_browser")
+                logger.info("bilichat_use_browser 所需依赖未安装，采用绘图渲染模式")
                 return False
             raise RuntimeError(
-                "Package(s) of fuction styles not installed, "
-                "use **pip install nonebot-plugin-bilichat[all]** to install required dependencies"
+                "浏览器渲染依赖未安装, 请选择其他渲染模式或使用 **pip install nonebot-plugin-bilichat[all]** 来安装所需依赖"
             ) from e
 
     @validator("bilichat_basic_info_style", always=True, pre=True)
     def check_use_browser_basic(cls, v, values):
         if v == "bbot_default":
             return v
         # 不包含浏览器
         if values["bilichat_use_browser"] is not True:
             if v == "Auto":
                 return "bbot_default"
             raise RuntimeError(
-                f"style {v} require browser to work, please enable **bilichat_use_browser** or set style to Auto"
+                f"样式 {v} 需要浏览器渲染, 请开启 **bilichat_use_browser** 或设置 bilichat_basic_info_style 为 Auto"
             )
         # 包含浏览器
         return "style_blue" if v == "Auto" else v
 
     @validator("bilichat_dynamic_style", always=True, pre=True)
     def check_use_browser_dynamic(cls, v, values):
         if v == "dynamicrender":
             return v
         # 不包含浏览器
         if values["bilichat_use_browser"] is not True:
             if v == "Auto":
                 return "dynamicrender"
             raise RuntimeError(
-                f"style {v} require browser to work, please enable **bilichat_use_browser** or set style to Auto"
+                f"样式 {v} 需要浏览器渲染, 请开启 **bilichat_use_browser** 或设置 bilichat_dynamic_style 为 Auto"
             )
         # 包含浏览器
         return "browser_mobile" if v == "Auto" else v
 
     @validator("bilichat_bilibili_cookie", always=True)
     def check_bilibili_cookie(cls, v):
         if not v:
             return v
         # verify cookie file
         if Path(v).is_file():
             try:
                 json.loads(Path(v).read_text("utf-8"))
             except Exception as e:
-                raise ValueError("Config bilichat_browser_cookie got a problem occurred") from e
+                raise ValueError(f"无法读取 bilichat_bilibili_cookie: {v}") from e
 
         elif Path(v).is_dir():
-            raise ValueError(f"Config bilichat_browser_cookie requires a file, but {v} is a folder")
+            raise ValueError(f"bilichat_browser_cookie 需要一个文件, 而 {v} 是一个文件夹")
 
         elif v == "api":
             cookie_file = cache_dir.joinpath("bilibili_browser_cookies.json").absolute()
             cookie_file.touch(0o755)
-            logger.info(f"create bilibili cookies file at {cookie_file.as_posix()}")
+            logger.info(f"在 {cookie_file.as_posix()} 创建 bilichat_bilibili_cookie 文件")
             return cookie_file.as_posix()
 
         else:
-            raise ValueError(f"Path {v} is not recognized")
+            raise ValueError(f"路径 {v} 无法识别")
 
         return v
 
     @validator("bilichat_openai_proxy", always=True, pre=True)
     def check_openai_proxy(cls, v, values):
         if not values["bilichat_openai_token"]:
             return v
         if v is None:
-            logger.warning(
-                "you have enabled openai or newbing summary without a proxy, this may cause request failure."
-            )
+            logger.warning("你设置了 bilichat_openai_token 但未设置 bilichat_openai_proxy ，这可能会导致请求失败.")
         return v
 
     @validator("bilichat_openai_token_limit")
     def check_token_limit(cls, v, values):
         if values["bilichat_openai_token"] is None:
             return v
         if not isinstance(v, int):
@@ -199,47 +197,43 @@
         if model.startswith("gpt-3.5"):
             max_limit = 15000 if "16k" in model else 3500
         elif model.startswith("gpt-4"):
             max_limit = 32200 if "32k" in model else 7600
         else:
             max_limit = 3500
         if v > max_limit:
-            logger.error(
-                f"Model {model} has a token cap of {max_limit} instead of {v}, token will be replaced with {max_limit}"
-            )
+            logger.error(f"模型 {model} 的 token 上限为 {max_limit} 而不是 {v}, token 将被重置为 {max_limit}")
             v = max_limit
         return v
 
     @validator("bilichat_openai_token", always=True)
     def check_pypackage_openai(cls, v):
         if importlib.util.find_spec("tiktoken") or not v:
             return v
         else:
             raise RuntimeError(
-                "Package(s) of fuction openai summary not installed, "
-                "use **pip install nonebot-plugin-bilichat[summary]** to install required dependencies"
+                "openai 依赖未安装, 使用 **pip install nonebot-plugin-bilichat[summary]** 来安装所需依赖"
             )
 
     @validator("bilichat_word_cloud", always=True)
     def check_pypackage_wordcloud(cls, v):
         if (importlib.util.find_spec("wordcloud") and importlib.util.find_spec("jieba")) or not v:
             return v
         else:
             raise RuntimeError(
-                "Package(s) of fuction wordcloud not installed, "
-                "use **pip install nonebot-plugin-bilichat[wordcloud]** to install required dependencies"
+                "wordcloud 依赖未安装, 使用 **pip install nonebot-plugin-bilichat[wordcloud]** 来安装所需依赖"
             )
 
     @validator("bilichat_webui_path", always=True)
     def check_api(cls, v: str):
         if not v:
             return v
         v = v.strip("/")
         if "/" in v:
-            raise ValueError("bilichat_webui_path should not contain '/'")
+            raise ValueError("bilichat_webui_path 不应包含 '/'")
         return v
 
     def verify_permission(self, uid: Union[str, int]):
         if self.bilichat_whitelist:
             return str(uid) in self.bilichat_whitelist
         elif self.bilichat_blacklist:
             return str(uid) not in self.bilichat_blacklist
```

### Comparing `nonebot_plugin_bilichat-5.3.1/nonebot_plugin_bilichat/content/column.py` & `nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/content/column.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,26 +44,26 @@
             main_article: _Element = http_parser.xpath('//div[@id="read-article-holder"]')[0]
             plist: _ElementUnicodeResult = main_article.xpath(XPATH)
             cv_text = [text.strip() for text in plist if text.strip()]
             b23_url = await get_b23_url(f"https://www.bilibili.com/read/cv{cvid}")
         except AbortError:
             raise
         except TimeoutException:
-            logger.warning("Column parsing API call timeout")
+            logger.warning("专栏解析超时")
             raise AbortError(f"{bili_number} 专栏信息生成超时，请稍后再试。")
         except Exception as e:  # noqa
             logger.exception(f"Column parsing API call error: {e}")
             raise AbortError(f"专栏解析 API 调用出错：{e}") from e
 
         if options:
             if options.no_cache:
-                logger.debug(f"parameter --no-cache of cv{cvid} detected, using temporary cache")
+                logger.debug(f"cv{cvid} 包含参数 --no-cache, 使用一次性缓存")
                 cache = BaseCache(id=f"cv{cvid}", title=cv_title, content=cv_text)
             elif options.refresh:
-                logger.debug(f"parameter --refresh of cv{cvid} detected, remove cache")
+                logger.debug(f"cv{cvid} 包含参数 --refresh, 刷新缓存")
                 cache = Cache(id=f"cv{cvid}", title=cv_title, content=cv_text)
                 await cache.save()
             else:
                 cache = await Cache.load(f"cv{cvid}", title=cv_title, content=cv_text)
         else:
             cache = await Cache.load(f"cv{cvid}", title=cv_title, content=cv_text)
```

### Comparing `nonebot_plugin_bilichat-5.3.1/nonebot_plugin_bilichat/content/dynamic.py` & `nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/content/dynamic.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.3.1/nonebot_plugin_bilichat/content/video.py` & `nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/content/video.py`

 * *Files 5% similar despite different names*

```diff
@@ -50,18 +50,18 @@
 
         aid = video_info.activity_season.arc.aid or video_info.arc.aid
         title = video_info.activity_season.arc.title or video_info.arc.title
         b23_url = await get_b23_url(f"https://www.bilibili.com/video/av{aid}")
 
         if options:
             if options.no_cache:
-                logger.debug(f"parameter --no-cache of av{aid} detected, using temporary cache")
+                logger.debug(f"av{aid} 包含参数 --no-cache, 使用一次性缓存")
                 cache = BaseCache(id=f"av{aid}", title=title)
             elif options.refresh:
-                logger.debug(f"parameter --refresh of av{aid} detected, remove cache")
+                logger.debug(f"av{aid} 包含参数 --refresh, 刷新缓存")
                 cache = Cache(id=f"av{aid}", title=title)
                 await cache.save()
             else:
                 cache = await Cache.load(f"av{aid}", title=title)
         else:
             cache = await Cache.load(f"av{aid}", title=title)
 
@@ -69,17 +69,17 @@
         return content
 
     async def get_subtitle(self):
         cid = (
             self.raw.activity_season.pages[0].page.cid if self.raw.activity_season.pages else self.raw.pages[0].page.cid
         )
         if self.cache.content:
-            logger.debug(f"subtitle cache of av{self.id} exists, use cache")
+            logger.debug(f"av{self.id} 已有字幕缓存")
         else:
-            logger.debug(f"subtitle cache of av{self.id} not exists")
+            logger.debug(f"av{self.id} 无字幕缓存，获取字幕")
             subtitle = await get_subtitle(aid=self.id, cid=cid)
             self.cache.content = subtitle
             await self.cache.save()
         return self.cache.content
 
     async def get_image(self, style: str):
         return await (await VideoImage.from_view_rely(self.raw, self.url)).render(style)
```

### Comparing `nonebot_plugin_bilichat-5.3.1/nonebot_plugin_bilichat/lib/b23_extract.py` & `nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/lib/b23_extract.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.3.1/nonebot_plugin_bilichat/lib/bcut_asr.py` & `nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/lib/bcut_asr.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.3.1/nonebot_plugin_bilichat/lib/bilibili_request/auth.py` & `nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/lib/bilibili_request/auth.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.3.1/nonebot_plugin_bilichat/lib/bilibili_request/gRPC.py` & `nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/lib/bilibili_request/gRPC.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.3.1/nonebot_plugin_bilichat/lib/bilibili_request/restAPI.py` & `nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/lib/bilibili_request/restAPI.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.3.1/nonebot_plugin_bilichat/lib/browser.py` & `nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/lib/browser.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 
 async def pw_font_injecter(route: Route, request: Request):
     url = URL(request.url)
     if not url.is_absolute():
         raise ValueError("字体地址不合法")
     try:
-        logger.debug(f"Font {url.query['name']} requested")
+        logger.debug(f"请求字体文件 {url.query['name']}")
         await route.fulfill(
             path=await get_font_async(url.query["name"]),
             content_type=font_mime_map.get(url.suffix),
         )
         return
     except Exception:
         logger.error(f"找不到字体 {url.query['name']}")
```

### Comparing `nonebot_plugin_bilichat-5.3.1/nonebot_plugin_bilichat/lib/cache/json_cache.py` & `nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/lib/cache/json_cache.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from ..store import cache_dir
 from .cache import BaseCache
 
 
 class JSONFileCache(BaseCache):
     async def save(self) -> None:
         file_path = cache_dir.joinpath(f"{self.id}.json")
-        logger.debug(f"saving cache of {self.id} to {file_path.absolute().as_posix()}")
+        logger.debug(f"保存 {self.id} 的缓存到 {file_path.absolute().as_posix()}")
         if PYDANTIC_V2:
             await Path(file_path).write_text(self.model_dump_json(), encoding="utf-8")  # type: ignore
         else:
             await Path(file_path).write_text(self.json(ensure_ascii=False), encoding="utf-8")  # type: ignore
 
     @classmethod
     async def load(cls, id: str, **kwargs) -> "JSONFileCache":
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `nonebot_plugin_bilichat-5.3.1/nonebot_plugin_bilichat/lib/cache/mongo_cache.py` & `nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/lib/cache/mongo_cache.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.3.1/nonebot_plugin_bilichat/lib/draw/__init__.py` & `nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/lib/draw/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.3.1/nonebot_plugin_bilichat/lib/draw/column/browser_shot.py` & `nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/lib/draw/column/browser_shot.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import asyncio
 import re
 
 from nonebot.log import logger
 
+from ....config import plugin_config
+
 try:
     from playwright._impl._errors import TimeoutError  # type: ignore
 except ImportError:
     from playwright._impl._api_types import TimeoutError  # type: ignore
 
 from ....model.exception import AbortError, CaptchaAbortError, NotFindAbortError
 from ....optional import capture_exception
@@ -32,35 +34,37 @@
             clip["y"] = clip["y"] - 30  # 增加顶部白边
             clip["height"] = min(clip["height"] + 30, 32766)  # 增加顶部白边，限制高度
             clip["x"] = clip["x"] + 40  # 移除左右一半的白边
             clip["width"] = clip["width"] - 80  # 移除左右一半的白边
             await page.set_viewport_size({"width": 1080, "height": int(clip["height"] + 720)})
             await asyncio.sleep(1)
             await page.wait_for_load_state(state="networkidle")
-            if picture := await page.screenshot(clip=clip, full_page=True, type="jpeg", quality=98):
+            if picture := await page.screenshot(
+                clip=clip, full_page=True, type="jpeg", quality=plugin_config.bilichat_browser_shot_quality
+            ):
                 return picture
         except CaptchaAbortError:
             raise
         except TimeoutError:
             if retry:
-                logger.error(f"Column cv{cvid} screenshot timed out, retrying...")
+                logger.error(f"专栏 cv{cvid} 截图超时, 重试...")
                 return await screenshot(cvid, retry=False)
             raise AbortError(f"cv{cvid} 专栏截图超时")
         except NotFindAbortError:
             if retry:
-                logger.error(f"Column cv{cvid} screenshot not found, retry in 3 secs...")
+                logger.error(f"专栏 cv{cvid} 不存在, 3秒后重试...")
                 await asyncio.sleep(3)
                 return await screenshot(cvid, retry=False)
             raise
         except Exception as e:  # noqa
             if "waiting until" in str(e):
                 if retry:
-                    logger.error(f"Column cv{cvid} screenshot timed out, retrying...")
+                    logger.error(f"专栏 cv{cvid} 截图超时, 3秒后重试...")
                     await asyncio.sleep(3)
                     return await screenshot(cvid, retry=False)
                 raise AbortError(f"cv{cvid} 专栏截图超时")
             else:
                 capture_exception()
                 if retry:
-                    logger.exception(f"Column cv{cvid} screenshot not found, retrying...")
+                    logger.exception(f"专栏 cv{cvid} 截图失败, 重试...")
                     return await screenshot(cvid, retry=False)
                 raise AbortError(f"cv{cvid} 专栏截图失败")
```

### Comparing `nonebot_plugin_bilichat-5.3.1/nonebot_plugin_bilichat/lib/draw/dynamic/browser_shot.py` & `nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/lib/draw/dynamic/browser_shot.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,17 +22,17 @@
         nonlocal captcha
         logger.debug(f"[Captcha] Get captcha image url: {response.url}")
         if await response.body():
             captcha = True
 
     page.on(
         "response",
-        lambda response: detect_captcha(response)
-        if response.url.startswith("https://static.geetest.com/captcha_v3/")
-        else None,
+        lambda response: (
+            detect_captcha(response) if response.url.startswith("https://static.geetest.com/captcha_v3/") else None
+        ),
     )
 
     url = f"https://m.bilibili.com/dynamic/{dynid}"
     await page.set_viewport_size({"width": 460, "height": 780})
     await page.route(re.compile("^https://static.graiax/fonts/(.+)$"), pw_font_injecter)
     await page.goto(url, wait_until="networkidle")
 
@@ -93,35 +93,37 @@
             # page.on("requestfinished", network_request)
             page.on("requestfailed", network_requestfailed)
             if plugin_config.bilichat_dynamic_style == "browser_mobile":
                 page, clip = await get_mobile_screenshot(page, dynid)
             else:
                 page, clip = await get_pc_screenshot(page, dynid)
             clip["height"] = min(clip["height"], 32766)  # 限制高度
-            if picture := await page.screenshot(clip=clip, full_page=True, type="jpeg", quality=98):
+            if picture := await page.screenshot(
+                clip=clip, full_page=True, type="jpeg", quality=plugin_config.bilichat_browser_shot_quality
+            ):
                 return picture
         except CaptchaAbortError:
             raise
         except TimeoutError:
             if retry:
-                logger.error(f"Dynamic {dynid} screenshot timed out, retrying...")
+                logger.error(f"动态 {dynid} 截图超时, 重试...")
                 return await screenshot(dynid, retry=False)
             raise AbortError(f"{dynid} 动态截图超时")
         except NotFindAbortError:
             if retry:
-                logger.error(f"Dynamic {dynid} screenshot not found, retry in 3 secs...")
+                logger.error(f"动态 {dynid} 截图超时, 3秒后重试...")
                 await asyncio.sleep(3)
                 return await screenshot(dynid, retry=False)
             raise
         except Exception as e:  # noqa
             if "waiting until" in str(e):
                 if retry:
-                    logger.error(f"Dynamic {dynid} screenshot timed out, retrying...")
+                    logger.error(f"动态 {dynid} 截图超时, 3秒后重试...")
                     await asyncio.sleep(3)
                     return await screenshot(dynid, retry=False)
                 raise AbortError(f"{dynid} 动态截图超时")
             else:
                 capture_exception()
                 if retry:
-                    logger.exception(f"Dynamic {dynid} screenshot not found, retrying...")
+                    logger.exception(f"动态 {dynid} 截图超时, 重试...")
                     return await screenshot(dynid, retry=False)
                 raise AbortError(f"{dynid} 动态截图失败")
```

### Comparing `nonebot_plugin_bilichat-5.3.1/nonebot_plugin_bilichat/lib/draw/dynamic/dynamicrender.py` & `nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/lib/draw/dynamic/dynamicrender.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.3.1/nonebot_plugin_bilichat/lib/draw/video/__init__.py` & `nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/lib/draw/video/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.3.1/nonebot_plugin_bilichat/lib/draw/video/bbot_default.py` & `nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/lib/draw/video/bbot_default.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.3.1/nonebot_plugin_bilichat/lib/draw/video/style_blue.py` & `nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/lib/draw/video/style_blue.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from io import BytesIO
 
 import jinja2
 from nonebot_plugin_htmlrender.browser import get_new_page
 from qrcode.image.pil import PilImage
 from qrcode.main import QRCode
 
+from ....config import plugin_config
 from ...browser import pw_font_injecter
 from ...store import static_dir
 from . import VideoImage
 
 style_bule = static_dir.joinpath("style_blue")
 
 
@@ -71,10 +72,10 @@
 
     async with get_new_page() as page:
         await page.route(re.compile("^https://fonts.bbot/(.+)$"), pw_font_injecter)
         await page.goto(template_path)
         await page.set_content(html, wait_until="networkidle")
         await page.wait_for_timeout(5)
         img_raw = await page.locator(".video").screenshot(
-            type="png",
+            type="jpeg", quality=plugin_config.bilichat_browser_shot_quality
         )
     return img_raw
```

### Comparing `nonebot_plugin_bilichat-5.3.1/nonebot_plugin_bilichat/lib/fetch_dynamic.py` & `nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/lib/fetch_dynamic.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,19 +51,19 @@
         return await _fetch_rest(up.mid, up.nickname)
 
 
 async def _fetch_rest(up_mid: int, up_name: str) -> Union[Dynamic, None]:
     try:
         resp: List = (await get_user_dynamics(up_mid))["items"]
     except TimeoutException:
-        logger.error(f"[Dynamic] fetch {up_name}({up_mid}) timeout")
+        logger.error(f"[Dynamic] 获取 {up_name}({up_mid}) 超时")
         raise AbortError("Dynamic Abort")
     except ResponseCodeError as e:
         logger.error(
-            f"[Dynamic] fetch {up_name}({up_mid}) failed: "
+            f"[Dynamic] 获取 {up_name}({up_mid}) 失败: "
             f"[{e.code}] {e.details() if isinstance(e, AioRpcError) else e.msg}"
         )
         raise AbortError("Dynamic Abort")
     # 如果动态为空
     if not resp:
         logger.debug("未获取到任何动态")
         return
@@ -78,19 +78,19 @@
     return dynamic
 
 
 async def _fetch_grpc(up_mid: int, up_name: str) -> Union[Dynamic, None]:
     try:
         resp = await asyncio.wait_for(grpc_get_user_dynamics(up_mid, auth=AuthManager.get_auth()), timeout=10)
     except asyncio.TimeoutError:
-        logger.error(f"[Dynamic] fetch {up_name}({up_mid}) timeout")
+        logger.error(f"[Dynamic] 获取 {up_name}({up_mid}) 超时")
         raise AbortError("Dynamic Abort")
     except (GrpcError, AioRpcError) as e:
         logger.error(
-            f"[Dynamic] fetch {up_name}({up_mid}) failed: "
+            f"[Dynamic] 获取 {up_name}({up_mid}) 失败: "
             f"[{e.code}] {e.details() if isinstance(e, AioRpcError) else e.msg}"
         )
         raise AbortError("Dynamic Abort")
     except Exception as e:
         capture_exception(e)
         raise e
     # 如果动态为空
```

### Comparing `nonebot_plugin_bilichat-5.3.1/nonebot_plugin_bilichat/lib/fonts_provider.py` & `nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/lib/fonts_provider.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.3.1/nonebot_plugin_bilichat/lib/strings.py` & `nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/lib/strings.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.3.1/nonebot_plugin_bilichat/lib/text_to_image.py` & `nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/lib/text_to_image.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import skia
 from dynamicadaptor.Content import RichTextDetail, Text
 from dynrender_skia.DynConfig import SetDynStyle
 from dynrender_skia.DynText import BiliText
 from nonebot.log import logger
 
 from ..config import plugin_config
+from ..model.exception import ProssesError
 from .fonts_provider import get_font_sync
 from .store import cache_dir
 
 data_path = cache_dir.joinpath("render")
 data_path.mkdir(parents=True, exist_ok=True)
 
 
@@ -83,22 +84,20 @@
     async with get_new_page() as page:
         await page.route(re.compile("^https://fonts.bbot/(.+)$"), pw_font_injecter)
         await page.set_viewport_size({"width": 800, "height": 2000})
         await page.goto(template_path)
         await page.set_content(html, wait_until="networkidle")
         await page.wait_for_timeout(5)
         img_raw = await page.get_by_alt_text("main").screenshot(
-            type="png",
+            type="jpeg", quality=plugin_config.bilichat_browser_shot_quality
         )
     return img_raw
 
 
-async def t2i(data: str, src: str):
+async def t2i(data: str, src: str) -> bytes:
     try:
-        if len(data.strip()) < 30:
-            return data
         if plugin_config.bilichat_use_browser:
             return await pw_text2image(data, src)
         return await rich_text2image(data, src)
     except Exception as e:
         logger.exception(e)
-        return f"总结图片生成失败 {e}\n {data}"
+        raise ProssesError(f"总结图片生成失败 {e}\n {data}") from e
```

### Comparing `nonebot_plugin_bilichat-5.3.1/nonebot_plugin_bilichat/lib/tools.py` & `nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/lib/tools.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.3.1/nonebot_plugin_bilichat/lib/uid_extract.py` & `nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/lib/uid_extract.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.3.1/nonebot_plugin_bilichat/lib/video_subtitle.py` & `nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/lib/video_subtitle.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.3.1/nonebot_plugin_bilichat/model/api/__init__.py` & `nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/model/api/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.3.1/nonebot_plugin_bilichat/model/api/subs_config.py` & `nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/model/api/subs_config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.3.1/nonebot_plugin_bilichat/model/bcut_asr.py` & `nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/model/bcut_asr.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.3.1/nonebot_plugin_bilichat/model/bilibili/live.py` & `nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/model/bilibili/live.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.3.1/nonebot_plugin_bilichat/model/bilibili/summary.py` & `nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/model/bilibili/summary.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.3.1/nonebot_plugin_bilichat/static/browser/mobile_style.js` & `nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/static/browser/mobile_style.js`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.3.1/nonebot_plugin_bilichat/static/style_blue/assets/business.png` & `nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/static/style_blue/assets/business.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.3.1/nonebot_plugin_bilichat/static/style_blue/assets/personal.png` & `nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/static/style_blue/assets/personal.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.3.1/nonebot_plugin_bilichat/static/style_blue/assets/video_bottom.png` & `nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/static/style_blue/assets/video_bottom.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.3.1/nonebot_plugin_bilichat/static/style_blue/video-details.html` & `nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/static/style_blue/video-details.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.3.1/nonebot_plugin_bilichat/static/summary/bilibili.png` & `nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/static/summary/bilibili.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.3.1/nonebot_plugin_bilichat/static/summary/index.html` & `nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/static/summary/index.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.3.1/nonebot_plugin_bilichat/static/summary/marked.min.js` & `nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/static/summary/marked.min.js`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.3.1/nonebot_plugin_bilichat/static/summary/openai.png` & `nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/static/summary/openai.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.3.1/nonebot_plugin_bilichat/static/upload-webui.html` & `nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/static/upload-webui.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.3.1/nonebot_plugin_bilichat/static/webui.tar.gz` & `nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/static/webui.tar.gz`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.3.1/nonebot_plugin_bilichat/subscribe/__init__.py` & `nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/subscribe/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -15,63 +15,63 @@
     seconds=90,
     id="dynamic_update",
     jitter=5,
     max_instances=1,
 )
 async def run_dynamic_update():
     if not SubscriptionSystem.activate_uploaders:
-        logger.debug("no activate uploaders to check, skip...")
+        logger.trace("[Dynamic] 无活跃的UP, 跳过...")
         return
     # 动态
-    logger.debug("[Dynamic] Updating start")
+    logger.debug("[Dynamic] 开始获取动态...")
     up_groups = list(SubscriptionSystem.activate_uploaders.keys()).copy()
     for up_id in up_groups:
         await asyncio.sleep(0)
         up = SubscriptionSystem.activate_uploaders.get(up_id)
         if not up:
             continue
         while CONFIG_LOCK.locked():
             await asyncio.sleep(0)
         async with CONFIG_LOCK:
             if SubscriptionSystem.config.dynamic_grpc:
                 try:
-                    logger.debug(f"[Dynamic] fetch {up.nickname}({up.uid}) by gRPC | offset={up.dyn_offset}")
+                    logger.debug(f"[Dynamic] 使用gRPC获取 {up.nickname}({up.uid}) | offset={up.dyn_offset}")
                     await fetch_dynamics_grpc(up)
                     continue
                 except AbortError:
-                    logger.error(f"[Dynamic] fetch dynamic for {up} failed.")
+                    logger.error(f"[Dynamic] 获取 {up} 失败.")
                 except Exception:
                     capture_exception()
-                    logger.exception(f"[Dynamic] fetch dynamic for {up} failed.")
+                    logger.exception(f"[Dynamic] 获取 {up} 失败.")
 
             try:
-                logger.debug(f"[Dynamic] fetch {up.nickname}({up.uid}) by RestAPI | offset={up.dyn_offset}")
+                logger.debug(f"[Dynamic] 使用 RestAPI 获取 {up.nickname}({up.uid}) | offset={up.dyn_offset}")
                 await fetch_dynamics_rest(up)
                 continue
             except AbortError:
-                logger.error(f"[Dynamic] fetch dynamic for {up} failed, skip...")
+                logger.error(f"[Dynamic] 获取 {up} 失败, skip...")
             except Exception:
                 capture_exception()
-                logger.exception(f"[Dynamic] fetch dynamic for {up} failed, skip...")
-    logger.debug("[Dynamic] Updating finished")
+                logger.exception(f"[Dynamic] 获取 {up} 失败, skip...")
+    logger.debug("[Dynamic] 获取完成")
 
 
 @scheduler.scheduled_job(
     "interval",
     seconds=60,
     id="live_update",
     jitter=5,
     max_instances=1,
 )
 async def run_live_update():
     if not SubscriptionSystem.activate_uploaders:
-        logger.debug("no activate uploaders to check, skip...")
+        logger.trace("[Live] 无活跃的UP, 跳过...")
         return
     try:
-        logger.debug("[Live] Updating start")
+        logger.debug("[Live] 获取开始")
         await fetch_live(list(SubscriptionSystem.activate_uploaders.keys()).copy())
     except AbortError:
-        logger.error("[Live] fetch live failed.")
+        logger.error("[Live] 获取中断.")
     except Exception:
         capture_exception()
-        logger.exception("[Live] fetch live failed.")
-    logger.debug("[Live] Updating finished")
+        logger.exception("[Live] 获取失败.")
+    logger.debug("[Live] 获取完成")
```

### Comparing `nonebot_plugin_bilichat-5.3.1/nonebot_plugin_bilichat/subscribe/dynamic.py` & `nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/subscribe/dynamic.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,19 +23,19 @@
 from .manager import Uploader
 
 
 async def fetch_dynamics_rest(up: Uploader):
     try:
         resp: List = (await get_user_dynamics(up.uid))["items"]
     except TimeoutException:
-        logger.error(f"[Dynamic] fetch {up.nickname}({up.uid}) timeout")
+        logger.error(f"[Dynamic] 获取 {up.nickname}({up.uid}) 超时")
         raise AbortError("Dynamic Abort")
     except ResponseCodeError as e:
         logger.error(
-            f"[Dynamic] fetch {up.nickname}({up.uid}) failed: "
+            f"[Dynamic] 获取 {up.nickname}({up.uid}) 失败: "
             f"[{e.code}] {e.details() if isinstance(e, AioRpcError) else e.msg}"
         )
         raise AbortError("Dynamic Abort")
     # 如果动态为空
     if not resp:
         logger.debug("未获取到任何动态")
         return
@@ -46,15 +46,15 @@
     dyns = [x for x in resp if int(x["id_str"]) > up.dyn_offset and x["type"] not in DYNAMIC_TYPE_IGNORE]
     dyns.reverse()
     for dyn in dyns:
         check_cd(dyn["id_str"], check=False)
         up.dyn_offset = max(up.dyn_offset, int(dyn["id_str"]))
         up_name = dyn["modules"]["module_author"]["name"]
         if up.nickname != up_name:
-            logger.info(f"[Dynamic] Up {up.nickname}({up.uid}) nickname changed to {up_name}")
+            logger.info(f"[Dynamic] Up {up.nickname}({up.uid}) 更改昵称为 {up_name}")
             up.nickname = up_name
 
         url = ""
         type_text = f"{up.nickname} "
         dyn_type = DYNAMIC_TYPE_MAP.get(dyn["type"], DynamicType.dyn_none)
         if dyn_type == DynamicType.av:
             type_text += "投稿了视频"
@@ -93,19 +93,19 @@
                 )
 
 
 async def fetch_dynamics_grpc(up: Uploader):
     try:
         resp = await asyncio.wait_for(grpc_get_user_dynamics(up.uid, auth=AuthManager.get_auth()), timeout=10)
     except asyncio.TimeoutError:
-        logger.error(f"[Dynamic] fetch {up.nickname}({up.uid}) timeout")
+        logger.error(f"[Dynamic] 获取 {up.nickname}({up.uid}) 超时")
         raise AbortError("Dynamic Abort")
     except (GrpcError, AioRpcError) as e:
         logger.error(
-            f"[Dynamic] fetch {up.nickname}({up.uid}) failed: "
+            f"[Dynamic] 获取 {up.nickname}({up.uid}) 失败: "
             f"[{e.code}] {e.details() if isinstance(e, AioRpcError) else e.msg}"
         )
         raise AbortError("Dynamic Abort")
     except Exception as e:
         capture_exception(e)
         raise e
     # 如果动态为空
@@ -118,15 +118,15 @@
     dyns = [x for x in resp.list if int(x.extend.dyn_id_str) > up.dyn_offset and x.card_type not in DYNAMIC_TYPE_IGNORE]
     dyns.reverse()
     for dyn in dyns:
         check_cd(dyn.extend.dyn_id_str, check=False)
         up.dyn_offset = max(up.dyn_offset, int(dyn.extend.dyn_id_str))
         up_name = dyn.modules[0].module_author.author.name
         if up.nickname != up_name:
-            logger.info(f"[Dynamic] Up {up.nickname}({up.uid}) nickname changed to {up_name}")
+            logger.info(f"[Dynamic] Up {up.nickname}({up.uid}) 更改昵称为 {up_name}")
             up.nickname = up_name
 
         url = ""
         type_text = f"{up.nickname} "
         if dyn.card_type == DynamicType.av:
             type_text += "投稿了视频"
             for module in dyn.modules:
```

### Comparing `nonebot_plugin_bilichat-5.3.1/nonebot_plugin_bilichat/subscribe/live.py` & `nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/subscribe/live.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 from .manager import CONFIG_LOCK, SubscriptionSystem
 
 
 async def fetch_live(ups: Sequence[int]):
     try:
         status_infos = await get_rooms_info_by_uids(list(ups))
     except (TransportError, ConnectError, JSONDecodeError, ResponseCodeError) as e:
-        logger.error(f"[Live] fetch live status failed: {type(e)} {e}")
+        logger.error(f"[Live] 获取直播状态失败: {type(e)} {e}")
         raise AbortError("Live Abort")
     except RuntimeError as e:
-        logger.error(f"[Live] fetch live status failed: {type(e)} {e}")
+        logger.error(f"[Live] 获取直播状态失败: {type(e)} {e}")
         if "The connection pool was closed while" not in str(e):
             capture_exception(e)
         raise AbortError("Live Abort")
     except Exception as e:  # noqa
         capture_exception(e)
         raise e
 
@@ -40,15 +40,15 @@
         if not up:
             # 如果没找到该UP，则跳过
             continue
         while CONFIG_LOCK.locked():
             await asyncio.sleep(0)
         async with CONFIG_LOCK:
             try:
-                logger.debug(f"[Live] {up.nickname}({up.uid}) live_status: {room.live_status}")
+                logger.debug(f"[Live] {up.nickname}({up.uid}) 直播状态: {room.live_status}")
                 # 已开播
                 if room.live_status == 1:
                     # 如果是 -1 则为第一次刷取，跳过后续推送部分
                     if up.living == -1:
                         up.living = room.live_time
                     # 如果记录值为 0 则是刚开播，开始开播推送
                     elif up.living == 0:
```

### Comparing `nonebot_plugin_bilichat-5.3.1/nonebot_plugin_bilichat/subscribe/manager.py` & `nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/subscribe/manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -210,15 +210,15 @@
         msg = MessageFactory(at)
         msg.extend([Image(x) if isinstance(x, bytes) else x for x in content])  # type: ignore
         try:
             await msg.send_to(target)
         except NoBotFound:
             pass
         except Exception as e:
-            logger.exception("Failed to push message to user")
+            logger.exception(f"无法为用户 {self.user_id} 推送消息")
             capture_exception(e)
 
         await asyncio.sleep(SubscriptionSystem.config.push_delay)
 
     def add_subscription(self, uploader: Uploader) -> Union[None, str]:
         """Add a subscription for a user to an uploader."""
 
@@ -341,15 +341,15 @@
 
     @classmethod
     async def load_from_file(cls):
         """Load data from the JSON file."""
         try:
             text = subscribe_file.read_text(encoding="utf-8")
         except UnicodeDecodeError:
-            logger.warning("subscribe.json is not UTF-8 encoded, trying to decode with system default encoding")
+            logger.warning("subscribe.json 非 UTF-8 编码, 尝试使用系统默认编码")
             text = subscribe_file.read_text()
         await cls.load(json.loads(text or "{}"))
 
     @classmethod
     def save_to_file(cls):
         """Save data to the JSON file."""
         subscribe_file.write_text(
@@ -361,29 +361,29 @@
             ),
             encoding="utf-8",
         )
 
     @classmethod
     def get_activate_uploaders(cls):
         at_ups = "\n".join([str(up) for up in cls.activate_uploaders.values()])
-        logger.debug("activate uploaders:\n" + (at_ups or "None activate uploaders"))
+        logger.debug("已激活的UP:\n" + (at_ups or "无已激活的UP"))
         return at_ups
 
     @classmethod
     def refresh_activate_uploaders(cls):
         """通过当前 Bot 覆盖的平台，激活需要推送的UP"""
-        logger.debug("refreshing activate uploaders")
+        logger.debug("刷新已激活的UP")
         cls.activate_uploaders = {}
         for user in cls.users.values():
             target = user.create_saa_target()
             try:
                 get_bot(target)
                 cls.activate_uploaders.update({int(up): cls.uploaders[int(up)] for up in user.subscriptions.keys()})
             except NoBotFound:
-                logger.debug(f"no bot found for user {user._id}")
+                logger.debug(f"用户 {user._id} 无可用推送 Bot")
                 continue
         cls.get_activate_uploaders()
 
 
 driver.on_startup(SubscriptionSystem.load_from_file)
```

### Comparing `nonebot_plugin_bilichat-5.3.1/nonebot_plugin_bilichat/summary/openai.py` & `nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/summary/openai.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 import httpx
 import tiktoken
 from nonebot.log import logger
 
 from ..config import plugin_config
 from ..model.openai import OpenAI, TokenUsage
 
-logger.info("Loading OpenAI Token enc model, this may take a few minutes to download")
+logger.info("加载 OpenAI Token enc 模型, 这可能需要一段时间进行下载")
 tiktoken_enc = tiktoken.encoding_for_model(plugin_config.bilichat_openai_model)
-logger.success(f"Enc model {tiktoken_enc.name} load successfully")
+logger.success(f"Enc 模型 {tiktoken_enc.name} 加载成功")
 
 
 def get_summarise_prompt(title: str, transcript: str, type_: Literal["视频字幕", "专栏文章"] = "视频字幕"):
     title = title.replace("\n", " ").strip() if title else ""
     transcript = transcript.replace("\n", " ").strip() if transcript else ""
     return get_full_prompt(
         prompt=(
```

### Comparing `nonebot_plugin_bilichat-5.3.1/nonebot_plugin_bilichat/summary/openai_summarise.py` & `nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/summary/openai_summarise.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import List
 
 from nonebot.log import logger
 
 from ..config import plugin_config
 from ..lib.cache import BaseCache
 from ..lib.text_to_image import t2i
-from ..model.exception import AbortError
+from ..model.exception import ProssesError
 from ..optional import capture_exception  # type: ignore
 from .openai import get_small_size_transcripts, get_summarise_prompt, openai_req
 
 
 async def subtitle_summarise(title: str, sub: List[str]):
     small_size_transcripts = get_small_size_transcripts(title, sub)
     prompt = get_summarise_prompt(title, small_size_transcripts)
@@ -28,32 +28,27 @@
     try:
         if not cache.openai:
             if cache.id[:2].lower() in ["bv", "av"]:
                 ai_summary = await subtitle_summarise(cache.title, cache.content)  # type: ignore
             elif cache.id[:2].lower() == "cv":
                 ai_summary = await column_summarise(cache.title, cache.content)  # type: ignore
             else:
-                raise ValueError(f"Illegal Video(Column) types {cache.id}")
+                raise ValueError(f"未知内容类型 {cache.id}")
 
             if ai_summary.response:
                 cache.openai = ai_summary.response
+                summary = ai_summary.response
                 await cache.save()
             else:
-                logger.warning(f"Video(Column) {cache.id} summary failure: {ai_summary.raw}")
+                logger.warning(f"视频(专栏) {cache.id} 总结失败: {ai_summary.raw}")
                 if plugin_config.bilichat_summary_ignore_null:
-                    return ""
+                    return
                 else:
-                    return f"视频(专栏) {cache.id} 总结失败: 响应内容异常\n{ai_summary.raw}"
-        return await t2i(cache.openai or "视频无法总结", plugin_config.bilichat_openai_model)
-    except AbortError as e:
-        logger.exception(f"Video(Column) {cache.id} summary aborted: {e}")
-        if plugin_config.bilichat_summary_ignore_null:
-            return ""
+                    summary = f"视频(专栏) {cache.id} 总结失败: 响应内容异常\n{ai_summary.raw}"
         else:
-            return f"视频(专栏) {cache.id} 总结中止: {e}"
+            summary = cache.openai
+        return await t2i(summary or "视频无法总结", plugin_config.bilichat_openai_model)
     except Exception as e:
         capture_exception()
-        logger.exception(f"Video(Column) {cache.id} summary failed: {e}")
-        if plugin_config.bilichat_summary_ignore_null:
-            return ""
-        else:
-            return f"视频(专栏) {cache.id} 总结失败: {e}"
+        logger.exception(f"视频(专栏) {cache.id} 总结失败: {e}")
+        if not plugin_config.bilichat_summary_ignore_null:
+            raise ProssesError(f"视频(专栏) {cache.id} 总结失败: {e}")
```

### Comparing `nonebot_plugin_bilichat-5.3.1/pyproject.toml` & `nonebot_plugin_bilichat-5.3.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-bilichat"
-version = "5.3.1"
+version = "5.3.2"
 description = "多种B站链接解析，视频词云，AI总结，你想要的都在 bilichat"
 authors = [
     { name = "djkcyl", email = "cyl@cyllive.cn" },
     { name = "Well404", email = "well_404@outlook.com" },
 ]
 dependencies = [
     "bilireq>=0.2.8",
@@ -15,15 +15,15 @@
     "nonebot2[fastapi,websockets]>=2.0.0",
     "httpx>=0.24.1",
     "dynrender-skia-opt>=0.3.8",
     "nonebot-plugin-apscheduler>=0.3.0",
     "nonebot-plugin-send-anything-anywhere>=0.4.0",
     "packaging>=23.2",
     "python-multipart>=0.0.6",
-    "nonebot-plugin-alconna>=0.41.1",
+    "nonebot-plugin-alconna>=0.42.0",
 ]
 requires-python = ">=3.8,<4.0"
 readme = "README.md"
 
 [project.license]
 text = "AGPL3.0"
```

### Comparing `nonebot_plugin_bilichat-5.3.1/PKG-INFO` & `nonebot_plugin_bilichat-5.3.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-bilichat
-Version: 5.3.1
+Version: 5.3.2
 Summary: 多种B站链接解析，视频词云，AI总结，你想要的都在 bilichat
 Author-Email: djkcyl <cyl@cyllive.cn>, Well404 <well_404@outlook.com>
 License: AGPL3.0
 Requires-Python: <4.0,>=3.8
 Requires-Dist: bilireq>=0.2.8
 Requires-Dist: qrcode>=7.4.2
 Requires-Dist: pillow>=9.5.0
@@ -13,15 +13,15 @@
 Requires-Dist: nonebot2[fastapi,websockets]>=2.0.0
 Requires-Dist: httpx>=0.24.1
 Requires-Dist: dynrender-skia-opt>=0.3.8
 Requires-Dist: nonebot-plugin-apscheduler>=0.3.0
 Requires-Dist: nonebot-plugin-send-anything-anywhere>=0.4.0
 Requires-Dist: packaging>=23.2
 Requires-Dist: python-multipart>=0.0.6
-Requires-Dist: nonebot-plugin-alconna>=0.41.1
+Requires-Dist: nonebot-plugin-alconna>=0.42.0
 Requires-Dist: numpy<1.25.0,>=1.20.1; extra == "extra"
 Requires-Dist: nonebot-plugin-sentry>=0.2.2; extra == "extra"
 Requires-Dist: nonebot-plugin-htmlrender>=0.2.0.3; extra == "extra"
 Requires-Dist: nonebot-plugin-mongodb>=0.1.0; extra == "extra"
 Requires-Dist: jieba>=0.42.1; extra == "wordcloud"
 Requires-Dist: wordcloud>=1.8.2.2; extra == "wordcloud"
 Requires-Dist: tiktoken>=0.6.0; extra == "summary"
@@ -111,24 +111,14 @@
 <details>
 <summary>视频总结</summary>
 
 ![](docs/summary.png)
 
 </details>
 
-## 🔌 适配器
-
-| 项目       | 视频解析 | 关注订阅 |
-| ---------- | -------- | -------- |
-| Onebot V11 | ✅       | ✅(SAA)  |
-| Onebot V12 | ✅       | ✅(SAA)  |
-| mirai2     | ✅       | ✅(SAA)  |
-| qq (频道)  | ✅       | ⏳(SAA)  |
-| qq (群)    | ⏳       | ❌       |
-
 ## 💿 安装
 
 > Linux 用户在安装时如果出现 `libGL.so.1: cannot open shared object file: No such file or directory` 错误，说明缺少 OpenGL 的运行环境，可以参考 [dynamicrender](https://pypi.org/project/dynrender-skia/) 中的 README 安装对应的依赖后重试
 
 <details>
 <summary>使用 nb-cli 安装</summary>
 在 nonebot2 项目的根目录下打开命令行, 输入以下指令即可安装
@@ -202,32 +192,33 @@
 bilichat_openai_token = sk-xxxxxxx
 # 网络代理
 bilichat_openai_proxy = "http://127.0.0.1:7890/"
 ```
 
 ### 通用配置项
 
-|         配置项          |   类型    |  默认值  |                               说明                               |
-| :---------------------: | :-------: | :------: | :--------------------------------------------------------------: |
-|     bilichat_block      |   bool    |  False   |                是否拦截事件(防止其他插件二次解析)                |
-|  bilichat_enable_self   |   bool    |  False   |                      是否允许响应自身的消息                      |
-|   bilichat_only_self    |   bool    |  False   | 是否仅响应自身的消息，开启后会**覆盖全部其他规则**(人机合一特供) |
-|   bilichat_only_to_me   |   bool    |  False   |      非自身消息是否需要 `@机器人` 或使用机器人的昵称才响应       |
-|   bilichat_whitelist    | list[str] |    []    |                 **响应**的会话名单, 会覆盖黑名单                 |
-|   bilichat_blacklist    | list[str] |    []    |                       **不响应**的会话名单                       |
-|  bilichat_dynamic_font  |    str    |   None   |                   视频信息及词云图片使用的字体                   |
-|    bilichat_cd_time     |    int    |   120    |                对同一视频的响应冷却时间(防止刷屏)                |
-| bilichat_neterror_retry |    int    |    3     |                   对部分网络请求错误的尝试次数                   |
-|  bilichat_use_bcut_asr  |   bool    |   True   |             是否在**没有字幕时**调用必剪接口生成字幕             |
-| bilichat_show_error_msg |   bool    |   True   |                   是否在解析失败时发送错误信息                   |
-|  bilichat_use_browser   |   bool    |   Auto   |     是否使用浏览器，`Auto` 会根据是否含有相应的依赖进行选择      |
-|  bilichat_cache_serive  |    str    |   Auto   |         使用的缓存类型，可用类型包含 `json` 和 `mongodb`         |
-|   bilichat_text_fonts   |    str    | default  |          可供自定义的字体，仅作用于 dynamicrender 绘图           |
-|  bilichat_emoji_fonts   |    str    | default  |          可供自定义的字体，仅作用于 dynamicrender 绘图           |
-|   bilichat_webui_path   |    str    | bilichat |               WebUI 的路径，设置为空则不开启 WebUI               |
+|            配置项             |   类型    |  默认值  |                               说明                               |
+| :---------------------------: | :-------: | :------: | :--------------------------------------------------------------: |
+|        bilichat_block         |   bool    |  False   |                是否拦截事件(防止其他插件二次解析)                |
+|     bilichat_enable_self      |   bool    |  False   |                      是否允许响应自身的消息                      |
+|      bilichat_only_self       |   bool    |  False   | 是否仅响应自身的消息，开启后会**覆盖全部其他规则**(人机合一特供) |
+|      bilichat_only_to_me      |   bool    |  False   |      非自身消息是否需要 `@机器人` 或使用机器人的昵称才响应       |
+|      bilichat_whitelist       | list[str] |    []    |                 **响应**的会话名单, 会覆盖黑名单                 |
+|      bilichat_blacklist       | list[str] |    []    |                       **不响应**的会话名单                       |
+|     bilichat_dynamic_font     |    str    |   None   |                   视频信息及词云图片使用的字体                   |
+|       bilichat_cd_time        |    int    |   120    |                对同一视频的响应冷却时间(防止刷屏)                |
+|    bilichat_neterror_retry    |    int    |    3     |                   对部分网络请求错误的尝试次数                   |
+|     bilichat_use_bcut_asr     |   bool    |   True   |             是否在**没有字幕时**调用必剪接口生成字幕             |
+|    bilichat_show_error_msg    |   bool    |   True   |                   是否在解析失败时发送错误信息                   |
+|     bilichat_use_browser      |   bool    |   Auto   |     是否使用浏览器，`Auto` 会根据是否含有相应的依赖进行选择      |
+| bilichat_browser_shot_quality |    int    |    75    |      浏览器截图质量，取值范围 10-100，越高则截图的体积越大       |
+|     bilichat_cache_serive     |    str    |   Auto   |         使用的缓存类型，可用类型包含 `json` 和 `mongodb`         |
+|      bilichat_text_fonts      |    str    | default  |          可供自定义的字体，仅作用于 dynamicrender 绘图           |
+|     bilichat_emoji_fonts      |    str    | default  |          可供自定义的字体，仅作用于 dynamicrender 绘图           |
+|      bilichat_webui_path      |    str    | bilichat |               WebUI 的路径，设置为空则不开启 WebUI               |
 
 注:
 
 1. 由于 OneBot 协议未规定是否应上报自身事件，因此在不同的场景下能否获取自身事件并不一定，`bilichat_enable_self` 实际能否生效也与之相关
 2. 当 `bilichat_whitelist` 存在时，`bilichat_blacklist` 将会被禁用
 3. `bilichat_dynamic_font` 可填写自定义的字体 url，但并不推荐修改
 4. 当使用 `bcut_asr` 接口来生成 AI 字幕时，根据视频时长和网络情况有可能会识别失败，Bot 会提示 `BCut-ASR conversion failed due to network error`。可以通过调高 `bilichat_neterror_retry` 次数或几分钟后重试来尝试重新生成字幕
@@ -302,19 +293,18 @@
 
 </details>
 
 ### 词云配置项
 
 开启此功能需要安装对应的依赖 `nonebot-plugin-bilichat[wordcloud]`
 
-|       配置项        | 类型 | 默认值 |       说明       |
-| :-----------------: | :--: | :----: | :--------------: |
-| bilichat_word_cloud | bool | False  | 是否开启词云功能 |
-
-注：词云功能在 python3.11 中由于 `wordcloud` 包安装失败暂时无法启用，请不要在 3.11 中开启此功能
+|          配置项          |   类型    |   默认值    |       说明       |
+| :----------------------: | :-------: | :---------: | :--------------: |
+|   bilichat_word_cloud    |   bool    |    False    | 是否开启词云功能 |
+| bilichat_word_cloud_size | List[int] | [1000, 800] |   词云图片尺寸   |
 
 ### AI 视频总结配置项
 
 开启此功能需要安装对应的依赖 `nonebot-plugin-bilichat[summary]`
 
 |            配置项            | 类型 |       默认值       |                                      说明                                      |
 | :--------------------------: | :--: | :----------------: | :----------------------------------------------------------------------------: |
@@ -350,16 +340,14 @@
 |    指令    | 简写 |                        说明                        |
 | :--------: | :--: | :------------------------------------------------: |
 | --no-cache |  -n  |     本次总结禁用缓存(不会影响已存在的缓存文件)     |
 | --refresh  |  -r  | 刷新此视频的词云和总结缓存(会覆盖已存在的缓存文件) |
 
 ### 指令表
 
-> 此部分当前仅适配了 OneBot 11 ，如果有其他适配器的需求可以新建 issue 来提出
-
 指令部分由 `指令前缀` 和 `指令名` 组成，其中 `指令前缀` 包含 `COMMAND_START` `bilichat_cmd_start` `COMMAND_SEP` 三部分，默认的 `指令前缀` 为 `/bilichat.` ，即完整的指令为 `/bilichat.xxx`
 
 `指令前缀` 部分也是可以修改的，例如 .env 中填入如下设置即可实现无 `指令前缀`
 
 ```dotenv
 COMMAND_SEP=[""]
 COMMAND_START=[""]
@@ -384,18 +372,21 @@
 
 ## 🙏 感谢
 
 在此感谢以下开发者(项目)对本项目做出的贡献：
 
 -   [BibiGPT](https://github.com/JimmyLv/BibiGPT) 项目灵感来源
 -   [bilibili-API-collect](https://github.com/SocialSisterYi/bilibili-API-collect) 易姐收集的各种 BiliBili Api 及其提供的 gRPC Api 调用方案
+-   [HarukaBot](https://github.com/SK-415/HarukaBot) 功能来源
 -   [BBot-Graia](https://github.com/djkcyl/BBot-Graia) 功能来源 ~~(我 牛 我 自 己)~~
 -   [ABot-Graia](https://github.com/djkcyl/ABot-Graia) 永远怀念最好的 ABot 🙏
+-   [bilireq](https://github.com/SK-415/bilireq) 项目使用的 bilibili 请求库
 -   [nonebot-plugin-template](https://github.com/A-kirami/nonebot-plugin-template): 项目的 README 模板
 -   [Misaka-Mikoto-Tech](https://github.com/Misaka-Mikoto-Tech) 为本项目提交了多项 BUG 修复和代码参考
 -   [hamo-reid](https://github.com/hamo-reid) 为 style_blue 绘制了界面
 -   [dynamicrender](https://pypi.org/project/dynrender-skia/) 提供 t2i 和动态渲染
 -   [SAA](https://github.com/MountainDash/nonebot-plugin-send-anything-anywhere) 提供指令及订阅部分的跨平台支持
+-   [ALC](https://github.com/nonebot/plugin-alconna) 提供跨平台支持
 
 ## ⏳ Star 趋势
 
 [![Stargazers over time](https://starchart.cc/djkcyl/nonebot-plugin-bilichat.svg)](https://starchart.cc/djkcyl/nonebot-plugin-bilichat)
```

#### html2text {}

```diff
@@ -1,19 +1,19 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-bilichat Version: 5.3.1 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-bilichat Version: 5.3.2 Summary:
 å¤ç§Bç«é¾æ¥è§£æï¼è§é¢è¯äºï¼AIæ»ç»ï¼ä½ æ³è¦çé½å¨ bilichat
 Author-Email: djkcyl
 cyllive.cn>, Well404
 outlook.com> License: AGPL3.0 Requires-Python: <4.0,>=3.8 Requires-Dist:
 bilireq>=0.2.8 Requires-Dist: qrcode>=7.4.2 Requires-Dist: pillow>=9.5.0
 Requires-Dist: lxml>=4.9.2 Requires-Dist: nonebot-plugin-localstore>=0.4.1
 Requires-Dist: nonebot2[fastapi,websockets]>=2.0.0 Requires-Dist: httpx>=0.24.1
 Requires-Dist: dynrender-skia-opt>=0.3.8 Requires-Dist: nonebot-plugin-
 apscheduler>=0.3.0 Requires-Dist: nonebot-plugin-send-anything-anywhere>=0.4.0
 Requires-Dist: packaging>=23.2 Requires-Dist: python-multipart>=0.0.6 Requires-
-Dist: nonebot-plugin-alconna>=0.41.1 Requires-Dist: numpy<1.25.0,>=1.20.1;
+Dist: nonebot-plugin-alconna>=0.42.0 Requires-Dist: numpy<1.25.0,>=1.20.1;
 extra == "extra" Requires-Dist: nonebot-plugin-sentry>=0.2.2; extra == "extra"
 Requires-Dist: nonebot-plugin-htmlrender>=0.2.0.3; extra == "extra" Requires-
 Dist: nonebot-plugin-mongodb>=0.1.0; extra == "extra" Requires-Dist:
 jieba>=0.42.1; extra == "wordcloud" Requires-Dist: wordcloud>=1.8.2.2; extra ==
 "wordcloud" Requires-Dist: tiktoken>=0.6.0; extra == "summary" Requires-Dist:
 numpy<1.25.0,>=1.20.1; extra == "all" Requires-Dist: jieba>=0.42.1; extra ==
 "all" Requires-Dist: wordcloud>=1.8.2.2; extra == "all" Requires-Dist: nonebot-
@@ -27,20 +27,17 @@
    # nonebot-plugin-bilichat _â¨ å¤åè½ç B ç«è§é¢è§£æå·¥å· â¨_
  _[_l_i_c_e_n_s_e_]_[_P_y_P_I_ _-_ _D_o_w_n_l_o_a_d_s_]_[_p_y_p_i_][python]_[_p_d_m_-_m_a_n_a_g_e_d_]_[_C_o_d_e_ _s_t_y_l_e_:_ _b_l_a_c_k_]_[_Q_Q
                           _C_h_a_t_ _G_r_o_u_p_]_[_Q_Q_ _C_h_a_t_ _G_r_o_u_p_]
 ## ð ä»ç»
 è§é¢é¾æ¥è§£æï¼å¹¶æ ¹æ®å¶åå®¹çæ**åºæ¬ä¿¡æ¯**ã**è¯äº**å**åå®¹æ»ç»**
 ææºç«¯è§å¾ ![](docs/mobile.png) åºæ¬ä¿¡æ¯ ![bbot_default](docs/
 bbot_default.png) ![style_blue](docs/style_blue.png) è¯äº ![](docs/
-wordcloud.png) è§é¢æ»ç» ![](docs/summary.png) ## ð ééå¨ | é¡¹ç® |
-è§é¢è§£æ | å³æ³¨è®¢é | | ---------- | -------- | -------- | | Onebot V11
-| â | â(SAA) | | Onebot V12 | â | â(SAA) | | mirai2 | â | â(SAA) |
-| qq (é¢é) | â | â³(SAA) | | qq (ç¾¤) | â³ | â | ## ð¿ å®è£ >
-Linux ç¨æ·å¨å®è£æ¶å¦æåºç° `libGL.so.1: cannot open shared object
-file: No such file or directory` éè¯¯ï¼è¯´æç¼ºå° OpenGL
+wordcloud.png) è§é¢æ»ç» ![](docs/summary.png) ## ð¿ å®è£ > Linux
+ç¨æ·å¨å®è£æ¶å¦æåºç° `libGL.so.1: cannot open shared object file: No
+such file or directory` éè¯¯ï¼è¯´æç¼ºå° OpenGL
 çè¿è¡ç¯å¢ï¼å¯ä»¥åè [dynamicrender](https://pypi.org/project/
 dynrender-skia/) ä¸­ç README å®è£å¯¹åºçä¾èµåéè¯ ä½¿ç¨ nb-cli
 å®è£ å¨ nonebot2 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡,
 è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ nb plugin install nonebot-plugin-bilichat æ³¨:
 ç±äº nb-cli ä¸æ¯æä¾èµç»ï¼å æ­¤éè¦å¯ç¨è¯äºå AI
 æ»ç»çç¨æ·è¦éè¿å¶ä»çåç®¡çå¨å®è£é¢å¤çä¾èµ pip install
 nonebot-plugin-bilichat[all] ä½¿ç¨åç®¡çå¨å®è£ å¨ nonebot2
@@ -56,17 +53,17 @@
 å¯¹åä¸è§é¢çååºå·å´æ¶é´(é²æ­¢å·å±) bilichat_cd_time = 120 #
 ç½ç»è¯·æ±éè¯æ¬¡æ° bilichat_neterror_retry = 3 #
 æ¯å¦ä½¿ç¨æµè§å¨æªå¾(éè¦é¢å¤ä¾èµ) bilichat_use_browser = True #
 æ¯å¦å¼å¯è¯äº(éè¦é¢å¤ä¾èµ) bilichat_word_cloud = True # === AI
 æ»ç»ç¸å³ === # å®æ¹æ»ç»æ¥å£ bilichat_official_summary = True # openai
 æ¥å£(éè¦é¢å¤ä¾èµ) bilichat_openai_token = sk-xxxxxxx # ç½ç»ä»£ç
 bilichat_openai_proxy = "http://127.0.0.1:7890/" ``` ### éç¨éç½®é¡¹ |
-éç½®é¡¹ | ç±»å | é»è®¤å¼ | è¯´æ | | :---------------------: | :-------:
-| :------: | :--------------------------------------------------------------: |
-| bilichat_block | bool | False | æ¯å¦æ¦æªäºä»¶
+éç½®é¡¹ | ç±»å | é»è®¤å¼ | è¯´æ | | :---------------------------: | :--
+-----: | :------: | :----------------------------------------------------------
+----: | | bilichat_block | bool | False | æ¯å¦æ¦æªäºä»¶
 (é²æ­¢å¶ä»æä»¶äºæ¬¡è§£æ) | | bilichat_enable_self | bool | False |
 æ¯å¦åè®¸ååºèªèº«çæ¶æ¯ | | bilichat_only_self | bool | False |
 æ¯å¦ä»ååºèªèº«çæ¶æ¯ï¼å¼å¯åä¼**è¦çå¨é¨å¶ä»è§å**
 (äººæºåä¸ç¹ä¾) | | bilichat_only_to_me | bool | False |
 éèªèº«æ¶æ¯æ¯å¦éè¦ `@æºå¨äºº` æä½¿ç¨æºå¨äººçæµç§°æååº |
 | bilichat_whitelist | list[str] | [] | **ååº**çä¼è¯åå,
 ä¼è¦çé»åå | | bilichat_blacklist | list[str] | [] |
@@ -75,17 +72,19 @@
 å¯¹åä¸è§é¢çååºå·å´æ¶é´(é²æ­¢å·å±) | | bilichat_neterror_retry
 | int | 3 | å¯¹é¨åç½ç»è¯·æ±éè¯¯çå°è¯æ¬¡æ° | |
 bilichat_use_bcut_asr | bool | True |
 æ¯å¦å¨**æ²¡æå­å¹æ¶**è°ç¨å¿åªæ¥å£çæå­å¹ | |
 bilichat_show_error_msg | bool | True |
 æ¯å¦å¨è§£æå¤±è´¥æ¶åééè¯¯ä¿¡æ¯ | | bilichat_use_browser | bool |
 Auto | æ¯å¦ä½¿ç¨æµè§å¨ï¼`Auto`
-ä¼æ ¹æ®æ¯å¦å«æç¸åºçä¾èµè¿è¡éæ© | | bilichat_cache_serive |
-str | Auto | ä½¿ç¨çç¼å­ç±»åï¼å¯ç¨ç±»ååå« `json` å `mongodb` |
-| bilichat_text_fonts | str | default | å¯ä¾èªå®ä¹çå­ä½ï¼ä»ä½ç¨äº
+ä¼æ ¹æ®æ¯å¦å«æç¸åºçä¾èµè¿è¡éæ© | |
+bilichat_browser_shot_quality | int | 75 | æµè§å¨æªå¾è´¨éï¼åå¼èå´
+10-100ï¼è¶é«åæªå¾çä½ç§¯è¶å¤§ | | bilichat_cache_serive | str | Auto
+| ä½¿ç¨çç¼å­ç±»åï¼å¯ç¨ç±»ååå« `json` å `mongodb` | |
+bilichat_text_fonts | str | default | å¯ä¾èªå®ä¹çå­ä½ï¼ä»ä½ç¨äº
 dynamicrender ç»å¾ | | bilichat_emoji_fonts | str | default |
 å¯ä¾èªå®ä¹çå­ä½ï¼ä»ä½ç¨äº dynamicrender ç»å¾ | |
 bilichat_webui_path | str | bilichat | WebUI
 çè·¯å¾ï¼è®¾ç½®ä¸ºç©ºåä¸å¼å¯ WebUI | æ³¨: 1. ç±äº OneBot
 åè®®æªè§å®æ¯å¦åºä¸æ¥èªèº«äºä»¶ï¼å æ­¤å¨ä¸åçåºæ¯ä¸è½å¦è·åèªèº«äºä»¶å¹¶ä¸ä¸å®ï¼`bilichat_enable_self`
 å®éè½å¦çæä¹ä¸ä¹ç¸å³ 2. å½ `bilichat_whitelist`
 å­å¨æ¶ï¼`bilichat_blacklist` å°ä¼è¢«ç¦ç¨ 3. `bilichat_dynamic_font`
@@ -137,19 +136,18 @@
 é¤é»è®¤ç dynamicrender ä½¿ç¨ Skia
 ç»å¾ï¼æªå¼å¯æµè§å¨æ¶é»è®¤éæ©ï¼ï¼å¶ä»åä¾èµäºæµè§å¨è¿è¡æ¸²æï¼éè¦è®¾ç½®
 bilichat_use_browser ä¸º True æ Autoï¼ï¼å¶å¯ç¨çæ ·å¼å¦ä¸æç¤º
 dynamicrender ï¼æ æµè§å¨æ¶é»è®¤ï¼ ![](docs/dynamicrender.jpg)
 browser_mobile ï¼ææµè§å¨æ¶é»è®¤ï¼ ![](docs/dynamic_mobile.jpg)
 browser_pc ![](docs/dynamic_pc.jpg) ### è¯äºéç½®é¡¹
 å¼å¯æ­¤åè½éè¦å®è£å¯¹åºçä¾èµ `nonebot-plugin-bilichat[wordcloud]`
-| éç½®é¡¹ | ç±»å | é»è®¤å¼ | è¯´æ | | :-----------------: | :--: | :---
--: | :--------------: | | bilichat_word_cloud | bool | False |
-æ¯å¦å¼å¯è¯äºåè½ | æ³¨ï¼è¯äºåè½å¨ python3.11 ä¸­ç±äº
-`wordcloud` åå®è£å¤±è´¥ææ¶æ æ³å¯ç¨ï¼è¯·ä¸è¦å¨ 3.11
-ä¸­å¼å¯æ­¤åè½ ### AI è§é¢æ»ç»éç½®é¡¹
+| éç½®é¡¹ | ç±»å | é»è®¤å¼ | è¯´æ | | :----------------------: | :-----
+--: | :---------: | :--------------: | | bilichat_word_cloud | bool | False |
+æ¯å¦å¼å¯è¯äºåè½ | | bilichat_word_cloud_size | List[int] | [1000, 800]
+| è¯äºå¾çå°ºå¯¸ | ### AI è§é¢æ»ç»éç½®é¡¹
 å¼å¯æ­¤åè½éè¦å®è£å¯¹åºçä¾èµ `nonebot-plugin-bilichat[summary]` |
 éç½®é¡¹ | ç±»å | é»è®¤å¼ | è¯´æ | | :--------------------------: | :--:
 | :----------------: | :-------------------------------------------------------
 ---------------------: | | bilichat_summary_ignore_null | bool | True |
 æ¯å¦å¿½ç¥æ æä¹çæ»ç»åå®¹ | | bilichat_official_summary | bool |
 False | æ¯å¦å¼å¯å®æ¹æ»ç»ï¼æ­¤æ»ç»ç¬ç«äºä¸æ¹ AI
 æ»ç»ï¼å¯ä¸ä¸æ¹ AI æ»ç»åæ¶çæ | | bilichat_openai_token | str |
@@ -170,20 +168,18 @@
 BV12v4y1E7NT --refresh BV12v4y1E7NT -r # å¯ä»¥ä½¿ç¨ç®å BV12v4y1E7NT -r --
 no-cache # å¯ä»¥å¤ä¸ªåæ°æ··ç¨ -r BV12v4y1E7NT -n #
 è½ç¶ä¸å»ºè®®ï¼ä½ç¡®å®å¯ä»¥æåæ°æ¾åé¢ ``` | æä»¤ | ç®å |
 è¯´æ | | :--------: | :--: | :-----------------------------------------------
 -: | | --no-cache | -n | æ¬æ¬¡æ»ç»ç¦ç¨ç¼å­
 (ä¸ä¼å½±åå·²å­å¨çç¼å­æä»¶) | | --refresh | -r |
 å·æ°æ­¤è§é¢çè¯äºåæ»ç»ç¼å­(ä¼è¦çå·²å­å¨çç¼å­æä»¶) |
-### æä»¤è¡¨ > æ­¤é¨åå½åä»ééäº OneBot 11
-ï¼å¦ææå¶ä»ééå¨çéæ±å¯ä»¥æ°å»º issue æ¥æåº
-æä»¤é¨åç± `æä»¤åç¼` å `æä»¤å` ç»æï¼å¶ä¸­ `æä»¤åç¼`
-åå« `COMMAND_START` `bilichat_cmd_start` `COMMAND_SEP` ä¸é¨åï¼é»è®¤ç
-`æä»¤åç¼` ä¸º `/bilichat.` ï¼å³å®æ´çæä»¤ä¸º `/bilichat.xxx`
-`æä»¤åç¼` é¨åä¹æ¯å¯ä»¥ä¿®æ¹çï¼ä¾å¦ .env
+### æä»¤è¡¨ æä»¤é¨åç± `æä»¤åç¼` å `æä»¤å` ç»æï¼å¶ä¸­
+`æä»¤åç¼` åå« `COMMAND_START` `bilichat_cmd_start` `COMMAND_SEP`
+ä¸é¨åï¼é»è®¤ç `æä»¤åç¼` ä¸º `/bilichat.` ï¼å³å®æ´çæä»¤ä¸º
+`/bilichat.xxx` `æä»¤åç¼` é¨åä¹æ¯å¯ä»¥ä¿®æ¹çï¼ä¾å¦ .env
 ä¸­å¡«å¥å¦ä¸è®¾ç½®å³å¯å®ç°æ  `æä»¤åç¼` ```dotenv COMMAND_SEP=[""]
 COMMAND_START=[""] bilichat_cmd_start="" ``` `æä»¤å`
 å¦ä¸è¡¨æç¤ºï¼å¶ä¸­é¤ç»å½ç¸å³çæä»¤åå¯èªå®ä¹ï¼å¯åèä¸æç
 [æä»¤åè®¢ééç½®é¡¹](#æä»¤åè®¢ééç½®é¡¹) | æä»¤ | æé |
 èå´ | åæ° | è¯´æ | | :----------: | :----: | :----: | :----------------
 --------------------: | :--------------------------------------: | | sub |
 ä¸»äºº | ç¾¤è | UP ä¸»çæµç§°æ UID | æ·»å è®¢é | | unsub | ä¸»äºº |
@@ -200,19 +196,22 @@
 checklogin | ä¸»äºº | æ éå¶ | æ  | æ¥çå½åå·²ç»å½çå¨é¨è´¦å· |
 | qrlogin | ä¸»äºº | æ éå¶ | æ  | ä½¿ç¨äºç»´ç ç»å½ B
 ç«ï¼é²æ­¢é£æ§ | | logout | ä¸»äºº | æ éå¶ | è´¦å·ç UID |
 ç»åºæå®çè´¦å· | ## ð æè°¢ å¨æ­¤æè°¢ä»¥ä¸å¼åè
 (é¡¹ç®)å¯¹æ¬é¡¹ç®ååºçè´¡ç®ï¼ - [BibiGPT](https://github.com/JimmyLv/
 BibiGPT) é¡¹ç®çµææ¥æº - [bilibili-API-collect](https://github.com/
 SocialSisterYi/bilibili-API-collect) æå§æ¶éçåç§ BiliBili Api
-åå¶æä¾ç gRPC Api è°ç¨æ¹æ¡ - [BBot-Graia](https://github.com/djkcyl/
-BBot-Graia) åè½æ¥æº ~~(æ ç æ èª å·±)~~ - [ABot-Graia](https://
-github.com/djkcyl/ABot-Graia) æ°¸è¿æå¿µæå¥½ç ABot ð - [nonebot-
+åå¶æä¾ç gRPC Api è°ç¨æ¹æ¡ - [HarukaBot](https://github.com/SK-415/
+HarukaBot) åè½æ¥æº - [BBot-Graia](https://github.com/djkcyl/BBot-Graia)
+åè½æ¥æº ~~(æ ç æ èª å·±)~~ - [ABot-Graia](https://github.com/
+djkcyl/ABot-Graia) æ°¸è¿æå¿µæå¥½ç ABot ð - [bilireq](https://
+github.com/SK-415/bilireq) é¡¹ç®ä½¿ç¨ç bilibili è¯·æ±åº - [nonebot-
 plugin-template](https://github.com/A-kirami/nonebot-plugin-template):
 é¡¹ç®ç README æ¨¡æ¿ - [Misaka-Mikoto-Tech](https://github.com/Misaka-
 Mikoto-Tech) ä¸ºæ¬é¡¹ç®æäº¤äºå¤é¡¹ BUG ä¿®å¤åä»£ç åè - [hamo-
 reid](https://github.com/hamo-reid) ä¸º style_blue ç»å¶äºçé¢ -
 [dynamicrender](https://pypi.org/project/dynrender-skia/) æä¾ t2i
 åå¨ææ¸²æ - [SAA](https://github.com/MountainDash/nonebot-plugin-send-
-anything-anywhere) æä¾æä»¤åè®¢éé¨åçè·¨å¹³å°æ¯æ ## â³ Star
-è¶å¿ [![Stargazers over time](https://starchart.cc/djkcyl/nonebot-plugin-
+anything-anywhere) æä¾æä»¤åè®¢éé¨åçè·¨å¹³å°æ¯æ - [ALC](https:
+//github.com/nonebot/plugin-alconna) æä¾è·¨å¹³å°æ¯æ ## â³ Star è¶å¿
+[![Stargazers over time](https://starchart.cc/djkcyl/nonebot-plugin-
 bilichat.svg)](https://starchart.cc/djkcyl/nonebot-plugin-bilichat)
```

