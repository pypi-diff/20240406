# Comparing `tmp/aiogram_prometheus-0.2.1.tar.gz` & `tmp/aiogram_prometheus-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiogram_prometheus-0.2.1.tar", max compression
+gzip compressed data, was "aiogram_prometheus-0.2.2.tar", max compression
```

## Comparing `aiogram_prometheus-0.2.1.tar` & `aiogram_prometheus-0.2.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1056 2024-02-13 14:03:21.190198 aiogram_prometheus-0.2.1/LICENSE
--rw-r--r--   0        0        0      432 2024-02-13 14:03:21.190198 aiogram_prometheus-0.2.1/aiogram_prometheus/__init__.py
--rw-r--r--   0        0        0      465 2024-02-13 14:03:21.190198 aiogram_prometheus-0.2.1/aiogram_prometheus/collectors/__init__.py
--rw-r--r--   0        0        0     1194 2024-02-13 14:03:21.190198 aiogram_prometheus-0.2.1/aiogram_prometheus/collectors/asyncio_loop.py
--rw-r--r--   0        0        0      497 2024-02-13 14:03:21.190198 aiogram_prometheus-0.2.1/aiogram_prometheus/collectors/base.py
--rw-r--r--   0        0        0     3214 2024-02-13 14:03:21.190198 aiogram_prometheus-0.2.1/aiogram_prometheus/collectors/bot.py
--rw-r--r--   0        0        0     5144 2024-02-13 14:03:21.190198 aiogram_prometheus-0.2.1/aiogram_prometheus/collectors/dispatcher.py
--rw-r--r--   0        0        0     1149 2024-02-13 14:03:21.190198 aiogram_prometheus-0.2.1/aiogram_prometheus/collectors/push_clients.py
--rw-r--r--   0        0        0     4460 2024-02-13 14:03:21.190198 aiogram_prometheus-0.2.1/aiogram_prometheus/collectors/storages.py
--rw-r--r--   0        0        0     3303 2024-02-13 14:03:21.194198 aiogram_prometheus-0.2.1/aiogram_prometheus/middlewares.py
--rw-r--r--   0        0        0      170 2024-02-13 14:03:21.194198 aiogram_prometheus-0.2.1/aiogram_prometheus/push_clients/__init__.py
--rw-r--r--   0        0        0     2006 2024-02-13 14:03:21.194198 aiogram_prometheus-0.2.1/aiogram_prometheus/push_clients/base.py
--rw-r--r--   0        0        0     2461 2024-02-13 14:03:21.194198 aiogram_prometheus-0.2.1/aiogram_prometheus/push_clients/pushgateway.py
--rw-r--r--   0        0        0      163 2024-02-13 14:03:21.194198 aiogram_prometheus-0.2.1/aiogram_prometheus/push_clients/statsd.py
--rw-r--r--   0        0        0     1442 2024-02-13 14:03:21.194198 aiogram_prometheus-0.2.1/aiogram_prometheus/storages.py
--rw-r--r--   0        0        0     2549 2024-02-13 14:03:21.194198 aiogram_prometheus-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     2815 2024-02-13 14:03:21.198198 aiogram_prometheus-0.2.1/readme.md
--rw-r--r--   0        0        0     4073 1970-01-01 00:00:00.000000 aiogram_prometheus-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1056 2024-04-06 12:49:37.028835 aiogram_prometheus-0.2.2/LICENSE
+-rw-r--r--   0        0        0      432 2024-04-06 12:49:37.028835 aiogram_prometheus-0.2.2/aiogram_prometheus/__init__.py
+-rw-r--r--   0        0        0      465 2024-04-06 12:49:37.028835 aiogram_prometheus-0.2.2/aiogram_prometheus/collectors/__init__.py
+-rw-r--r--   0        0        0     1194 2024-04-06 12:49:37.028835 aiogram_prometheus-0.2.2/aiogram_prometheus/collectors/asyncio_loop.py
+-rw-r--r--   0        0        0      512 2024-04-06 12:49:37.028835 aiogram_prometheus-0.2.2/aiogram_prometheus/collectors/base.py
+-rw-r--r--   0        0        0     3393 2024-04-06 12:49:37.028835 aiogram_prometheus-0.2.2/aiogram_prometheus/collectors/bot.py
+-rw-r--r--   0        0        0     5159 2024-04-06 12:49:37.028835 aiogram_prometheus-0.2.2/aiogram_prometheus/collectors/dispatcher.py
+-rw-r--r--   0        0        0     1149 2024-04-06 12:49:37.032835 aiogram_prometheus-0.2.2/aiogram_prometheus/collectors/push_clients.py
+-rw-r--r--   0        0        0     4475 2024-04-06 12:49:37.032835 aiogram_prometheus-0.2.2/aiogram_prometheus/collectors/storages.py
+-rw-r--r--   0        0        0     3283 2024-04-06 12:49:37.032835 aiogram_prometheus-0.2.2/aiogram_prometheus/middlewares.py
+-rw-r--r--   0        0        0      170 2024-04-06 12:49:37.032835 aiogram_prometheus-0.2.2/aiogram_prometheus/push_clients/__init__.py
+-rw-r--r--   0        0        0     2212 2024-04-06 12:49:37.032835 aiogram_prometheus-0.2.2/aiogram_prometheus/push_clients/base.py
+-rw-r--r--   0        0        0     2461 2024-04-06 12:49:37.032835 aiogram_prometheus-0.2.2/aiogram_prometheus/push_clients/pushgateway.py
+-rw-r--r--   0        0        0      163 2024-04-06 12:49:37.032835 aiogram_prometheus-0.2.2/aiogram_prometheus/push_clients/statsd.py
+-rw-r--r--   0        0        0     1442 2024-04-06 12:49:37.032835 aiogram_prometheus-0.2.2/aiogram_prometheus/storages.py
+-rw-r--r--   0        0        0     2549 2024-04-06 12:49:37.032835 aiogram_prometheus-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     6308 2024-04-06 12:49:37.032835 aiogram_prometheus-0.2.2/readme.md
+-rw-r--r--   0        0        0     7566 1970-01-01 00:00:00.000000 aiogram_prometheus-0.2.2/PKG-INFO
```

### Comparing `aiogram_prometheus-0.2.1/LICENSE` & `aiogram_prometheus-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aiogram_prometheus-0.2.1/aiogram_prometheus/collectors/asyncio_loop.py` & `aiogram_prometheus-0.2.2/aiogram_prometheus/collectors/asyncio_loop.py`

 * *Files identical despite different names*

### Comparing `aiogram_prometheus-0.2.1/aiogram_prometheus/collectors/bot.py` & `aiogram_prometheus-0.2.2/aiogram_prometheus/collectors/bot.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,63 +1,67 @@
 import logging
-from typing import Any, Iterable, Optional
+from typing import Any, Iterable, List, Optional
 
 from aiogram import Bot
 from aiogram.methods import Response, TelegramMethod
 from prometheus_client import REGISTRY, CollectorRegistry, Histogram
 from prometheus_client.metrics_core import InfoMetricFamily, Metric
 
 from aiogram_prometheus.collectors.base import BaseAiogramCollector
 
-logger = logging.getLogger('app')
+logger = logging.getLogger('aiogram_prometheus')
 
 
 class BotAiogramCollector(BaseAiogramCollector):
     """Collector for main info about bot
 
     Args:
         bot [aiogram.Bot]: Object of target bot
 
     """
 
-    bot: Bot
+    bots: List[Bot]
 
-    def __init__(self, bot: Bot, prefix: str = 'aiogram', registry: CollectorRegistry = REGISTRY) -> None:
+    def __init__(self, prefix: str = 'aiogram', registry: CollectorRegistry = REGISTRY) -> None:
         super().__init__(prefix, registry)
 
-        self.bot = bot
+        self.bots = []
 
         self.register()
 
+    def add_bot(self, bot: Bot):
+        self.bots.append(bot)
+
     def collect(self) -> Iterable[Metric]:
-        bot_user = self.bot._me
+        for bot in self.bots:
+            bot_user = bot._me
 
-        if bot_user is None:
-            return
+            if bot_user is None:
+                return
 
-        yield InfoMetricFamily(
-            f'{self.prefix}_bot',
-            'Info about bot',
-            {
-                'id': str(self.bot.id),
-                'username': str(bot_user.username),
-                'is_bot': str(bot_user.is_bot),
-                'first_name': str(bot_user.first_name),
-                'last_name': str(bot_user.last_name),
-                'language_code': str(bot_user.language_code),
-                'is_premium': str(bot_user.is_premium),
-                'added_to_attachment_menu': str(bot_user.added_to_attachment_menu),
-                'can_join_groups': str(bot_user.can_join_groups),
-                'can_read_all_group_messages': str(bot_user.can_read_all_group_messages),
-                'supports_inline_queries': str(bot_user.supports_inline_queries),
-                'parse_mode': str(self.bot.parse_mode),
-                'disable_web_page_preview': str(self.bot.disable_web_page_preview),
-                'protect_content': str(self.bot.protect_content),
-            },
-        )
+            yield InfoMetricFamily(
+                f'{self.prefix}_bot',
+                'Info about bot',
+                {
+                    'id': str(bot.id),
+                    'username': str(bot_user.username),
+                    'is_bot': str(bot_user.is_bot),
+                    'first_name': str(bot_user.first_name),
+                    'last_name': str(bot_user.last_name),
+                    'language_code': str(bot_user.language_code),
+                    'is_premium': str(bot_user.is_premium),
+                    'added_to_attachment_menu': str(bot_user.added_to_attachment_menu),
+                    'can_join_groups': str(bot_user.can_join_groups),
+                    'can_read_all_group_messages': str(bot_user.can_read_all_group_messages),
+                    'supports_inline_queries': str(bot_user.supports_inline_queries),
+                    'parse_mode': str(bot.parse_mode),
+                    'disable_web_page_preview': str(bot.disable_web_page_preview),
+                    'protect_content': str(bot.protect_content),
+                },
+            )
 
 
 class RequestsBotAiogramCollector(BaseAiogramCollector):
     """Collector for requests from bot to server
 
     Used inside aiogram_prometheus.middlewares.PrometheusMetricRequestMiddleware
```

### Comparing `aiogram_prometheus-0.2.1/aiogram_prometheus/collectors/dispatcher.py` & `aiogram_prometheus-0.2.2/aiogram_prometheus/collectors/dispatcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from aiogram import Bot, Dispatcher
 from aiogram.types import Message, TelegramObject
 from prometheus_client import REGISTRY, CollectorRegistry, Counter, Histogram
 from prometheus_client.metrics_core import GaugeMetricFamily, InfoMetricFamily, Metric
 
 from aiogram_prometheus.collectors.base import BaseAiogramCollector
 
-logger = logging.getLogger('app')
+logger = logging.getLogger('aiogram_prometheus')
 
 
 class DispatcherAiogramCollector(BaseAiogramCollector):
     dp: Dispatcher
 
     def __init__(self, dp: Dispatcher, prefix: str = 'aiogram', registry: CollectorRegistry = REGISTRY) -> None:
         super().__init__(prefix, registry)
```

### Comparing `aiogram_prometheus-0.2.1/aiogram_prometheus/collectors/push_clients.py` & `aiogram_prometheus-0.2.2/aiogram_prometheus/collectors/push_clients.py`

 * *Files identical despite different names*

### Comparing `aiogram_prometheus-0.2.1/aiogram_prometheus/collectors/storages.py` & `aiogram_prometheus-0.2.2/aiogram_prometheus/collectors/storages.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 from aiogram.fsm.storage.base import BaseStorage, StorageKey
 from prometheus_client import REGISTRY, CollectorRegistry, Counter, Histogram
 from prometheus_client.metrics_core import GaugeMetricFamily, InfoMetricFamily, Metric
 
 from aiogram_prometheus.collectors.base import BaseAiogramCollector
 
-logger = logging.getLogger('app')
+logger = logging.getLogger('aiogram_prometheus')
 
 
 class StorageAiogramCollector(BaseAiogramCollector):
     """Storage for metric Storages action
 
     Need use with PrometheusMetricStorageMixin
```

### Comparing `aiogram_prometheus-0.2.1/aiogram_prometheus/middlewares.py` & `aiogram_prometheus-0.2.2/aiogram_prometheus/middlewares.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from aiogram.methods.base import TelegramType
 from aiogram.types import Message, TelegramObject
 
 from aiogram_prometheus.collectors import MessageMiddlewareAiogramCollector, RequestsBotAiogramCollector
 
 logger = logging.getLogger('aiogram_prometheus')
 
-__all__ = ('PrometheusMetricMessageMiddleware', 'PrometheusPrometheusMetricRequestMiddleware')
+__all__ = ('PrometheusMetricMessageMiddleware', 'PrometheusMetricRequestMiddleware')
 
 
 class PrometheusMetricMessageMiddleware(BaseMiddleware):
     """Middleware for metrics messages in Dispatcher
 
     ### Args
 
@@ -61,15 +61,15 @@
             raise ex
 
         delta_time = time.time() - start_time
         self.collector.add_event(event, delta_time)
         return res
 
 
-class PrometheusPrometheusMetricRequestMiddleware(BaseRequestMiddleware):
+class PrometheusMetricRequestMiddleware(BaseRequestMiddleware):
     """Middleware for metric requests from Bot
 
     ### Args
 
     - collector [RequestsBotAiogramCollector] optional
 
     ### Usage
```

### Comparing `aiogram_prometheus-0.2.1/aiogram_prometheus/push_clients/pushgateway.py` & `aiogram_prometheus-0.2.2/aiogram_prometheus/push_clients/pushgateway.py`

 * *Files identical despite different names*

### Comparing `aiogram_prometheus-0.2.1/aiogram_prometheus/storages.py` & `aiogram_prometheus-0.2.2/aiogram_prometheus/storages.py`

 * *Files identical despite different names*

### Comparing `aiogram_prometheus-0.2.1/pyproject.toml` & `aiogram_prometheus-0.2.2/pyproject.toml`

 * *Files identical despite different names*

