# Comparing `tmp/message_flow-0.3.6.tar.gz` & `tmp/message_flow-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "message_flow-0.3.6.tar", last modified: Sat Mar 30 11:53:18 2024, max compression
+gzip compressed data, was "message_flow-0.3.7.tar", last modified: Sat Apr  6 20:19:06 2024, max compression
```

## Comparing `message_flow-0.3.6.tar` & `message_flow-0.3.7.tar`

### file list

```diff
@@ -1,101 +1,102 @@
--rw-r--r--   0        0        0    11347 2024-03-30 11:53:15.441301 message_flow-0.3.6/LICENSE
--rw-r--r--   0        0        0     3204 2024-03-30 11:53:15.441301 message_flow-0.3.6/README.md
--rw-r--r--   0        0        0     2547 2024-03-30 11:53:18.417294 message_flow-0.3.6/pyproject.toml
--rw-r--r--   0        0        0      124 2024-03-30 11:53:15.441301 message_flow-0.3.6/src/message_flow/__init__.py
--rw-r--r--   0        0        0       83 2024-03-30 11:53:15.441301 message_flow-0.3.6/src/message_flow/__main__.py
--rw-r--r--   0        0        0       57 2024-03-30 11:53:15.441301 message_flow-0.3.6/src/message_flow/app/__init__.py
--rw-r--r--   0        0        0       53 2024-03-30 11:53:15.445301 message_flow-0.3.6/src/message_flow/app/__init__.pyi
--rw-r--r--   0        0        0      241 2024-03-30 11:53:15.445301 message_flow-0.3.6/src/message_flow/app/_fast_api.py
--rw-r--r--   0        0        0       58 2024-03-30 11:53:15.445301 message_flow-0.3.6/src/message_flow/app/_internal/__init__.py
--rw-r--r--   0        0        0       91 2024-03-30 11:53:15.445301 message_flow-0.3.6/src/message_flow/app/_internal/__init__.pyi
--rw-r--r--   0        0        0       59 2024-03-30 11:53:15.445301 message_flow-0.3.6/src/message_flow/app/_internal/async_api_studio/__init__.py
--rw-r--r--   0        0        0       42 2024-03-30 11:53:15.445301 message_flow-0.3.6/src/message_flow/app/_internal/async_api_studio/__init__.pyi
--rw-r--r--   0        0        0      704 2024-03-30 11:53:15.445301 message_flow-0.3.6/src/message_flow/app/_internal/async_api_studio/config.py
--rw-r--r--   0        0        0     2665 2024-03-30 11:53:15.445301 message_flow-0.3.6/src/message_flow/app/_internal/async_api_studio/page.py
--rw-r--r--   0        0        0     2669 2024-03-30 11:53:15.445301 message_flow-0.3.6/src/message_flow/app/_internal/channels.py
--rw-r--r--   0        0        0      337 2024-03-30 11:53:15.445301 message_flow-0.3.6/src/message_flow/app/_internal/message_flow_schema.py
--rw-r--r--   0        0        0       58 2024-03-30 11:53:15.445301 message_flow-0.3.6/src/message_flow/app/_message_management/__init__.py
--rw-r--r--   0        0        0       81 2024-03-30 11:53:15.445301 message_flow-0.3.6/src/message_flow/app/_message_management/__init__.pyi
--rw-r--r--   0        0        0     1243 2024-03-30 11:53:15.445301 message_flow-0.3.6/src/message_flow/app/_message_management/dispatcher.py
--rw-r--r--   0        0        0      976 2024-03-30 11:53:15.445301 message_flow-0.3.6/src/message_flow/app/_message_management/producer.py
--rw-r--r--   0        0        0      171 2024-03-30 11:53:15.445301 message_flow-0.3.6/src/message_flow/app/_message_management/routing_headers.py
--rw-r--r--   0        0        0       58 2024-03-30 11:53:15.445301 message_flow-0.3.6/src/message_flow/app/_simple_messaging/__init__.py
--rw-r--r--   0        0        0       62 2024-03-30 11:53:15.445301 message_flow-0.3.6/src/message_flow/app/_simple_messaging/__init__.pyi
--rw-r--r--   0        0        0     2755 2024-03-30 11:53:15.445301 message_flow-0.3.6/src/message_flow/app/_simple_messaging/simple_consumer.py
--rw-r--r--   0        0        0      728 2024-03-30 11:53:15.445301 message_flow-0.3.6/src/message_flow/app/_simple_messaging/simple_producer.py
--rw-r--r--   0        0        0    16762 2024-03-30 11:53:15.445301 message_flow-0.3.6/src/message_flow/app/message_flow.py
--rw-r--r--   0        0        0       58 2024-03-30 11:53:15.445301 message_flow-0.3.6/src/message_flow/app/messaging/__init__.py
--rw-r--r--   0        0        0       48 2024-03-30 11:53:15.445301 message_flow-0.3.6/src/message_flow/app/messaging/__init__.pyi
--rw-r--r--   0        0        0     1121 2024-03-30 11:53:15.445301 message_flow-0.3.6/src/message_flow/app/messaging/consumer.py
--rw-r--r--   0        0        0      829 2024-03-30 11:53:15.445301 message_flow-0.3.6/src/message_flow/app/messaging/producer.py
--rw-r--r--   0        0        0       57 2024-03-30 11:53:15.445301 message_flow-0.3.6/src/message_flow/channel/__init__.py
--rw-r--r--   0        0        0       23 2024-03-30 11:53:15.445301 message_flow-0.3.6/src/message_flow/channel/__init__.pyi
--rw-r--r--   0        0        0       58 2024-03-30 11:53:15.445301 message_flow-0.3.6/src/message_flow/channel/_internal/__init__.py
--rw-r--r--   0        0        0       94 2024-03-30 11:53:15.445301 message_flow-0.3.6/src/message_flow/channel/_internal/__init__.pyi
--rw-r--r--   0        0        0     2151 2024-03-30 11:53:15.445301 message_flow-0.3.6/src/message_flow/channel/_internal/channel_construction.py
--rw-r--r--   0        0        0      168 2024-03-30 11:53:15.445301 message_flow-0.3.6/src/message_flow/channel/_internal/channel_info.py
--rw-r--r--   0        0        0      227 2024-03-30 11:53:15.445301 message_flow-0.3.6/src/message_flow/channel/_internal/channel_schema.py
--rw-r--r--   0        0        0    16343 2024-03-30 11:53:15.445301 message_flow-0.3.6/src/message_flow/channel/channel.py
--rw-r--r--   0        0        0       57 2024-03-30 11:53:15.445301 message_flow-0.3.6/src/message_flow/cli/__init__.py
--rw-r--r--   0        0        0       26 2024-03-30 11:53:15.445301 message_flow-0.3.6/src/message_flow/cli/__init__.pyi
--rw-r--r--   0        0        0     3174 2024-03-30 11:53:15.445301 message_flow-0.3.6/src/message_flow/cli/_cli_app.py
--rw-r--r--   0        0        0     1302 2024-03-30 11:53:15.445301 message_flow-0.3.6/src/message_flow/cli/_documentation_server.py
--rw-r--r--   0        0        0      203 2024-03-30 11:53:15.445301 message_flow-0.3.6/src/message_flow/cli/_logging_level.py
--rw-r--r--   0        0        0     1100 2024-03-30 11:53:15.445301 message_flow-0.3.6/src/message_flow/cli/entrypoint.py
--rw-r--r--   0        0        0       57 2024-03-30 11:53:15.445301 message_flow-0.3.6/src/message_flow/message/__init__.py
--rw-r--r--   0        0        0      186 2024-03-30 11:53:15.445301 message_flow-0.3.6/src/message_flow/message/__init__.pyi
--rw-r--r--   0        0        0       58 2024-03-30 11:53:15.445301 message_flow-0.3.6/src/message_flow/message/_internal/__init__.py
--rw-r--r--   0        0        0       66 2024-03-30 11:53:15.445301 message_flow-0.3.6/src/message_flow/message/_internal/__init__.pyi
--rw-r--r--   0        0        0     8360 2024-03-30 11:53:15.445301 message_flow-0.3.6/src/message_flow/message/_internal/message_construction.py
--rw-r--r--   0        0        0      286 2024-03-30 11:53:15.445301 message_flow-0.3.6/src/message_flow/message/_internal/message_schema.py
--rw-r--r--   0        0        0     1631 2024-03-30 11:53:15.445301 message_flow-0.3.6/src/message_flow/message/correlation_id.py
--rw-r--r--   0        0        0     7971 2024-03-30 11:53:15.445301 message_flow-0.3.6/src/message_flow/message/header.py
--rw-r--r--   0        0        0     5762 2024-03-30 11:53:15.445301 message_flow-0.3.6/src/message_flow/message/message.py
--rw-r--r--   0        0        0     1167 2024-03-30 11:53:15.445301 message_flow-0.3.6/src/message_flow/message/message_example.py
--rw-r--r--   0        0        0     3554 2024-03-30 11:53:15.445301 message_flow-0.3.6/src/message_flow/message/message_info.py
--rw-r--r--   0        0        0     4084 2024-03-30 11:53:15.445301 message_flow-0.3.6/src/message_flow/message/message_trait.py
--rw-r--r--   0        0        0     7971 2024-03-30 11:53:15.445301 message_flow-0.3.6/src/message_flow/message/payload.py
--rw-r--r--   0        0        0       57 2024-03-30 11:53:15.445301 message_flow-0.3.6/src/message_flow/operation/__init__.py
--rw-r--r--   0        0        0       83 2024-03-30 11:53:15.445301 message_flow-0.3.6/src/message_flow/operation/__init__.pyi
--rw-r--r--   0        0        0       58 2024-03-30 11:53:15.445301 message_flow-0.3.6/src/message_flow/operation/_internal/__init__.py
--rw-r--r--   0        0        0      100 2024-03-30 11:53:15.445301 message_flow-0.3.6/src/message_flow/operation/_internal/__init__.pyi
--rw-r--r--   0        0        0     2135 2024-03-30 11:53:15.445301 message_flow-0.3.6/src/message_flow/operation/_internal/operation_construction.py
--rw-r--r--   0        0        0      237 2024-03-30 11:53:15.445301 message_flow-0.3.6/src/message_flow/operation/_internal/operation_info.py
--rw-r--r--   0        0        0      410 2024-03-30 11:53:15.445301 message_flow-0.3.6/src/message_flow/operation/_internal/operation_schema.py
--rw-r--r--   0        0        0      101 2024-03-30 11:53:15.445301 message_flow-0.3.6/src/message_flow/operation/action_type.py
--rw-r--r--   0        0        0     4000 2024-03-30 11:53:15.445301 message_flow-0.3.6/src/message_flow/operation/operation.py
--rw-r--r--   0        0        0      555 2024-03-30 11:53:15.445301 message_flow-0.3.6/src/message_flow/operation/operation_reply.py
--rw-r--r--   0        0        0        0 2024-03-30 11:53:15.445301 message_flow-0.3.6/src/message_flow/py.typed
--rw-r--r--   0        0        0       57 2024-03-30 11:53:15.445301 message_flow-0.3.6/src/message_flow/shared/__init__.py
--rw-r--r--   0        0        0       51 2024-03-30 11:53:15.445301 message_flow-0.3.6/src/message_flow/shared/__init__.pyi
--rw-r--r--   0        0        0     1265 2024-03-30 11:53:15.445301 message_flow-0.3.6/src/message_flow/shared/components.py
--rw-r--r--   0        0        0     1189 2024-03-30 11:53:15.445301 message_flow-0.3.6/src/message_flow/shared/reference.py
--rw-r--r--   0        0        0       89 2024-03-30 11:53:15.445301 message_flow-0.3.6/src/message_flow/utils/__init__.py
--rw-r--r--   0        0        0      682 2024-03-30 11:53:15.445301 message_flow-0.3.6/src/message_flow/utils/log.py
--rw-r--r--   0        0        0     2212 2024-03-30 11:53:15.445301 message_flow-0.3.6/src/message_flow/utils/visibility.py
--rw-r--r--   0        0        0        0 2024-03-30 11:53:15.445301 message_flow-0.3.6/tests/__init__.py
--rw-r--r--   0        0        0        0 2024-03-30 11:53:15.445301 message_flow-0.3.6/tests/message/__init__.py
--rw-r--r--   0        0        0     1195 2024-03-30 11:53:15.445301 message_flow-0.3.6/tests/message/test_correlation_id.py
--rw-r--r--   0        0        0     2957 2024-03-30 11:53:15.445301 message_flow-0.3.6/tests/message/test_message.py
--rw-r--r--   0        0        0     1043 2024-03-30 11:53:15.445301 message_flow-0.3.6/tests/message/test_message_example.py
--rw-r--r--   0        0        0     3575 2024-03-30 11:53:15.445301 message_flow-0.3.6/tests/message/test_message_trait.py
--rw-r--r--   0        0        0        0 2024-03-30 11:53:15.445301 message_flow-0.3.6/tests/message_flow/__init__.py
--rw-r--r--   0        0        0      849 2024-03-30 11:53:15.445301 message_flow-0.3.6/tests/message_flow/conftest.py
--rw-r--r--   0        0        0      113 2024-03-30 11:53:15.445301 message_flow-0.3.6/tests/message_flow/message_flow_unit_test_support/__init__.py
--rw-r--r--   0        0        0     1577 2024-03-30 11:53:15.445301 message_flow-0.3.6/tests/message_flow/message_flow_unit_test_support/consumer.py
--rw-r--r--   0        0        0      589 2024-03-30 11:53:15.445301 message_flow-0.3.6/tests/message_flow/message_flow_unit_test_support/fake_message_producer.py
--rw-r--r--   0        0        0     4413 2024-03-30 11:53:15.445301 message_flow-0.3.6/tests/message_flow/message_flow_unit_test_support/message_flow_unit_test_support.py
--rw-r--r--   0        0        0      356 2024-03-30 11:53:15.445301 message_flow-0.3.6/tests/message_flow/message_flow_unit_test_support/message_with_channel.py
--rw-r--r--   0        0        0     2715 2024-03-30 11:53:15.445301 message_flow-0.3.6/tests/message_flow/message_flow_unit_test_support/producer.py
--rw-r--r--   0        0        0     5202 2024-03-30 11:53:15.445301 message_flow-0.3.6/tests/message_flow/test_command_sending.py
--rw-r--r--   0        0        0     1477 2024-03-30 11:53:15.445301 message_flow-0.3.6/tests/message_flow/test_dispatching.py
--rw-r--r--   0        0        0     1646 2024-03-30 11:53:15.445301 message_flow-0.3.6/tests/message_flow/test_event_publishing.py
--rw-r--r--   0        0        0      935 2024-03-30 11:53:15.445301 message_flow-0.3.6/tests/message_flow/test_message_flow.py
--rw-r--r--   0        0        0        0 2024-03-30 11:53:15.445301 message_flow-0.3.6/tests/operation/__init__.py
--rw-r--r--   0        0        0      431 2024-03-30 11:53:15.445301 message_flow-0.3.6/tests/operation/test_operation.py
--rw-r--r--   0        0        0    14330 2024-03-30 11:53:15.445301 message_flow-0.3.6/tests/schema/conftest.py
--rw-r--r--   0        0        0      248 2024-03-30 11:53:15.445301 message_flow-0.3.6/tests/schema/test_channel.py
--rw-r--r--   0        0        0      248 2024-03-30 11:53:15.445301 message_flow-0.3.6/tests/schema/test_message.py
--rw-r--r--   0        0        0      287 2024-03-30 11:53:15.445301 message_flow-0.3.6/tests/schema/test_message_flow.py
--rw-r--r--   0        0        0      272 2024-03-30 11:53:15.445301 message_flow-0.3.6/tests/schema/test_operation.py
--rw-r--r--   0        0        0     3610 1970-01-01 00:00:00.000000 message_flow-0.3.6/PKG-INFO
+-rw-r--r--   0        0        0    11347 2024-04-06 20:19:01.048870 message_flow-0.3.7/LICENSE
+-rw-r--r--   0        0        0     3204 2024-04-06 20:19:01.048870 message_flow-0.3.7/README.md
+-rw-r--r--   0        0        0     2547 2024-04-06 20:19:06.084875 message_flow-0.3.7/pyproject.toml
+-rw-r--r--   0        0        0      124 2024-04-06 20:19:01.052870 message_flow-0.3.7/src/message_flow/__init__.py
+-rw-r--r--   0        0        0       83 2024-04-06 20:19:01.052870 message_flow-0.3.7/src/message_flow/__main__.py
+-rw-r--r--   0        0        0       57 2024-04-06 20:19:01.052870 message_flow-0.3.7/src/message_flow/app/__init__.py
+-rw-r--r--   0        0        0       84 2024-04-06 20:19:01.052870 message_flow-0.3.7/src/message_flow/app/__init__.pyi
+-rw-r--r--   0        0        0      241 2024-04-06 20:19:01.052870 message_flow-0.3.7/src/message_flow/app/_fast_api.py
+-rw-r--r--   0        0        0       58 2024-04-06 20:19:01.052870 message_flow-0.3.7/src/message_flow/app/_internal/__init__.py
+-rw-r--r--   0        0        0       91 2024-04-06 20:19:01.052870 message_flow-0.3.7/src/message_flow/app/_internal/__init__.pyi
+-rw-r--r--   0        0        0       59 2024-04-06 20:19:01.052870 message_flow-0.3.7/src/message_flow/app/_internal/async_api_studio/__init__.py
+-rw-r--r--   0        0        0       42 2024-04-06 20:19:01.052870 message_flow-0.3.7/src/message_flow/app/_internal/async_api_studio/__init__.pyi
+-rw-r--r--   0        0        0      704 2024-04-06 20:19:01.052870 message_flow-0.3.7/src/message_flow/app/_internal/async_api_studio/config.py
+-rw-r--r--   0        0        0     2665 2024-04-06 20:19:01.052870 message_flow-0.3.7/src/message_flow/app/_internal/async_api_studio/page.py
+-rw-r--r--   0        0        0     2669 2024-04-06 20:19:01.052870 message_flow-0.3.7/src/message_flow/app/_internal/channels.py
+-rw-r--r--   0        0        0      337 2024-04-06 20:19:01.052870 message_flow-0.3.7/src/message_flow/app/_internal/message_flow_schema.py
+-rw-r--r--   0        0        0       58 2024-04-06 20:19:01.052870 message_flow-0.3.7/src/message_flow/app/_message_management/__init__.py
+-rw-r--r--   0        0        0       81 2024-04-06 20:19:01.052870 message_flow-0.3.7/src/message_flow/app/_message_management/__init__.pyi
+-rw-r--r--   0        0        0     2229 2024-04-06 20:19:01.052870 message_flow-0.3.7/src/message_flow/app/_message_management/dispatcher.py
+-rw-r--r--   0        0        0      976 2024-04-06 20:19:01.052870 message_flow-0.3.7/src/message_flow/app/_message_management/producer.py
+-rw-r--r--   0        0        0      171 2024-04-06 20:19:01.052870 message_flow-0.3.7/src/message_flow/app/_message_management/routing_headers.py
+-rw-r--r--   0        0        0       58 2024-04-06 20:19:01.052870 message_flow-0.3.7/src/message_flow/app/_simple_messaging/__init__.py
+-rw-r--r--   0        0        0       62 2024-04-06 20:19:01.052870 message_flow-0.3.7/src/message_flow/app/_simple_messaging/__init__.pyi
+-rw-r--r--   0        0        0     2755 2024-04-06 20:19:01.052870 message_flow-0.3.7/src/message_flow/app/_simple_messaging/simple_consumer.py
+-rw-r--r--   0        0        0      728 2024-04-06 20:19:01.052870 message_flow-0.3.7/src/message_flow/app/_simple_messaging/simple_producer.py
+-rw-r--r--   0        0        0     2805 2024-04-06 20:19:01.052870 message_flow-0.3.7/src/message_flow/app/base_middleware.py
+-rw-r--r--   0        0        0    18264 2024-04-06 20:19:01.052870 message_flow-0.3.7/src/message_flow/app/message_flow.py
+-rw-r--r--   0        0        0       58 2024-04-06 20:19:01.052870 message_flow-0.3.7/src/message_flow/app/messaging/__init__.py
+-rw-r--r--   0        0        0       48 2024-04-06 20:19:01.052870 message_flow-0.3.7/src/message_flow/app/messaging/__init__.pyi
+-rw-r--r--   0        0        0     1121 2024-04-06 20:19:01.052870 message_flow-0.3.7/src/message_flow/app/messaging/consumer.py
+-rw-r--r--   0        0        0      829 2024-04-06 20:19:01.052870 message_flow-0.3.7/src/message_flow/app/messaging/producer.py
+-rw-r--r--   0        0        0       57 2024-04-06 20:19:01.052870 message_flow-0.3.7/src/message_flow/channel/__init__.py
+-rw-r--r--   0        0        0       23 2024-04-06 20:19:01.052870 message_flow-0.3.7/src/message_flow/channel/__init__.pyi
+-rw-r--r--   0        0        0       58 2024-04-06 20:19:01.052870 message_flow-0.3.7/src/message_flow/channel/_internal/__init__.py
+-rw-r--r--   0        0        0       94 2024-04-06 20:19:01.052870 message_flow-0.3.7/src/message_flow/channel/_internal/__init__.pyi
+-rw-r--r--   0        0        0     2151 2024-04-06 20:19:01.052870 message_flow-0.3.7/src/message_flow/channel/_internal/channel_construction.py
+-rw-r--r--   0        0        0      168 2024-04-06 20:19:01.052870 message_flow-0.3.7/src/message_flow/channel/_internal/channel_info.py
+-rw-r--r--   0        0        0      227 2024-04-06 20:19:01.052870 message_flow-0.3.7/src/message_flow/channel/_internal/channel_schema.py
+-rw-r--r--   0        0        0    16343 2024-04-06 20:19:01.052870 message_flow-0.3.7/src/message_flow/channel/channel.py
+-rw-r--r--   0        0        0       57 2024-04-06 20:19:01.052870 message_flow-0.3.7/src/message_flow/cli/__init__.py
+-rw-r--r--   0        0        0       26 2024-04-06 20:19:01.052870 message_flow-0.3.7/src/message_flow/cli/__init__.pyi
+-rw-r--r--   0        0        0     3188 2024-04-06 20:19:01.052870 message_flow-0.3.7/src/message_flow/cli/_cli_app.py
+-rw-r--r--   0        0        0     1334 2024-04-06 20:19:01.052870 message_flow-0.3.7/src/message_flow/cli/_documentation_server.py
+-rw-r--r--   0        0        0      235 2024-04-06 20:19:01.052870 message_flow-0.3.7/src/message_flow/cli/_logging_level.py
+-rw-r--r--   0        0        0     1100 2024-04-06 20:19:01.052870 message_flow-0.3.7/src/message_flow/cli/entrypoint.py
+-rw-r--r--   0        0        0       57 2024-04-06 20:19:01.052870 message_flow-0.3.7/src/message_flow/message/__init__.py
+-rw-r--r--   0        0        0      186 2024-04-06 20:19:01.052870 message_flow-0.3.7/src/message_flow/message/__init__.pyi
+-rw-r--r--   0        0        0       58 2024-04-06 20:19:01.052870 message_flow-0.3.7/src/message_flow/message/_internal/__init__.py
+-rw-r--r--   0        0        0       66 2024-04-06 20:19:01.052870 message_flow-0.3.7/src/message_flow/message/_internal/__init__.pyi
+-rw-r--r--   0        0        0     8360 2024-04-06 20:19:01.052870 message_flow-0.3.7/src/message_flow/message/_internal/message_construction.py
+-rw-r--r--   0        0        0      286 2024-04-06 20:19:01.052870 message_flow-0.3.7/src/message_flow/message/_internal/message_schema.py
+-rw-r--r--   0        0        0     1631 2024-04-06 20:19:01.052870 message_flow-0.3.7/src/message_flow/message/correlation_id.py
+-rw-r--r--   0        0        0     7971 2024-04-06 20:19:01.052870 message_flow-0.3.7/src/message_flow/message/header.py
+-rw-r--r--   0        0        0     5762 2024-04-06 20:19:01.052870 message_flow-0.3.7/src/message_flow/message/message.py
+-rw-r--r--   0        0        0     1167 2024-04-06 20:19:01.052870 message_flow-0.3.7/src/message_flow/message/message_example.py
+-rw-r--r--   0        0        0     3554 2024-04-06 20:19:01.052870 message_flow-0.3.7/src/message_flow/message/message_info.py
+-rw-r--r--   0        0        0     4084 2024-04-06 20:19:01.052870 message_flow-0.3.7/src/message_flow/message/message_trait.py
+-rw-r--r--   0        0        0     7971 2024-04-06 20:19:01.052870 message_flow-0.3.7/src/message_flow/message/payload.py
+-rw-r--r--   0        0        0       57 2024-04-06 20:19:01.052870 message_flow-0.3.7/src/message_flow/operation/__init__.py
+-rw-r--r--   0        0        0       83 2024-04-06 20:19:01.052870 message_flow-0.3.7/src/message_flow/operation/__init__.pyi
+-rw-r--r--   0        0        0       58 2024-04-06 20:19:01.052870 message_flow-0.3.7/src/message_flow/operation/_internal/__init__.py
+-rw-r--r--   0        0        0      100 2024-04-06 20:19:01.052870 message_flow-0.3.7/src/message_flow/operation/_internal/__init__.pyi
+-rw-r--r--   0        0        0     2135 2024-04-06 20:19:01.052870 message_flow-0.3.7/src/message_flow/operation/_internal/operation_construction.py
+-rw-r--r--   0        0        0      237 2024-04-06 20:19:01.052870 message_flow-0.3.7/src/message_flow/operation/_internal/operation_info.py
+-rw-r--r--   0        0        0      410 2024-04-06 20:19:01.052870 message_flow-0.3.7/src/message_flow/operation/_internal/operation_schema.py
+-rw-r--r--   0        0        0      101 2024-04-06 20:19:01.052870 message_flow-0.3.7/src/message_flow/operation/action_type.py
+-rw-r--r--   0        0        0     4000 2024-04-06 20:19:01.052870 message_flow-0.3.7/src/message_flow/operation/operation.py
+-rw-r--r--   0        0        0      555 2024-04-06 20:19:01.052870 message_flow-0.3.7/src/message_flow/operation/operation_reply.py
+-rw-r--r--   0        0        0        0 2024-04-06 20:19:01.052870 message_flow-0.3.7/src/message_flow/py.typed
+-rw-r--r--   0        0        0       57 2024-04-06 20:19:01.052870 message_flow-0.3.7/src/message_flow/shared/__init__.py
+-rw-r--r--   0        0        0       51 2024-04-06 20:19:01.052870 message_flow-0.3.7/src/message_flow/shared/__init__.pyi
+-rw-r--r--   0        0        0     1265 2024-04-06 20:19:01.052870 message_flow-0.3.7/src/message_flow/shared/components.py
+-rw-r--r--   0        0        0     1189 2024-04-06 20:19:01.052870 message_flow-0.3.7/src/message_flow/shared/reference.py
+-rw-r--r--   0        0        0       89 2024-04-06 20:19:01.052870 message_flow-0.3.7/src/message_flow/utils/__init__.py
+-rw-r--r--   0        0        0      682 2024-04-06 20:19:01.052870 message_flow-0.3.7/src/message_flow/utils/log.py
+-rw-r--r--   0        0        0     2212 2024-04-06 20:19:01.052870 message_flow-0.3.7/src/message_flow/utils/visibility.py
+-rw-r--r--   0        0        0        0 2024-04-06 20:19:01.052870 message_flow-0.3.7/tests/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-06 20:19:01.052870 message_flow-0.3.7/tests/message/__init__.py
+-rw-r--r--   0        0        0     1195 2024-04-06 20:19:01.052870 message_flow-0.3.7/tests/message/test_correlation_id.py
+-rw-r--r--   0        0        0     2957 2024-04-06 20:19:01.052870 message_flow-0.3.7/tests/message/test_message.py
+-rw-r--r--   0        0        0     1043 2024-04-06 20:19:01.056870 message_flow-0.3.7/tests/message/test_message_example.py
+-rw-r--r--   0        0        0     3575 2024-04-06 20:19:01.056870 message_flow-0.3.7/tests/message/test_message_trait.py
+-rw-r--r--   0        0        0        0 2024-04-06 20:19:01.056870 message_flow-0.3.7/tests/message_flow/__init__.py
+-rw-r--r--   0        0        0      849 2024-04-06 20:19:01.056870 message_flow-0.3.7/tests/message_flow/conftest.py
+-rw-r--r--   0        0        0      113 2024-04-06 20:19:01.056870 message_flow-0.3.7/tests/message_flow/message_flow_unit_test_support/__init__.py
+-rw-r--r--   0        0        0     1577 2024-04-06 20:19:01.056870 message_flow-0.3.7/tests/message_flow/message_flow_unit_test_support/consumer.py
+-rw-r--r--   0        0        0      589 2024-04-06 20:19:01.056870 message_flow-0.3.7/tests/message_flow/message_flow_unit_test_support/fake_message_producer.py
+-rw-r--r--   0        0        0     4413 2024-04-06 20:19:01.056870 message_flow-0.3.7/tests/message_flow/message_flow_unit_test_support/message_flow_unit_test_support.py
+-rw-r--r--   0        0        0      356 2024-04-06 20:19:01.056870 message_flow-0.3.7/tests/message_flow/message_flow_unit_test_support/message_with_channel.py
+-rw-r--r--   0        0        0     2715 2024-04-06 20:19:01.056870 message_flow-0.3.7/tests/message_flow/message_flow_unit_test_support/producer.py
+-rw-r--r--   0        0        0     5202 2024-04-06 20:19:01.056870 message_flow-0.3.7/tests/message_flow/test_command_sending.py
+-rw-r--r--   0        0        0     1477 2024-04-06 20:19:01.056870 message_flow-0.3.7/tests/message_flow/test_dispatching.py
+-rw-r--r--   0        0        0     1646 2024-04-06 20:19:01.056870 message_flow-0.3.7/tests/message_flow/test_event_publishing.py
+-rw-r--r--   0        0        0      935 2024-04-06 20:19:01.056870 message_flow-0.3.7/tests/message_flow/test_message_flow.py
+-rw-r--r--   0        0        0        0 2024-04-06 20:19:01.056870 message_flow-0.3.7/tests/operation/__init__.py
+-rw-r--r--   0        0        0      431 2024-04-06 20:19:01.056870 message_flow-0.3.7/tests/operation/test_operation.py
+-rw-r--r--   0        0        0    14330 2024-04-06 20:19:01.056870 message_flow-0.3.7/tests/schema/conftest.py
+-rw-r--r--   0        0        0      248 2024-04-06 20:19:01.056870 message_flow-0.3.7/tests/schema/test_channel.py
+-rw-r--r--   0        0        0      248 2024-04-06 20:19:01.056870 message_flow-0.3.7/tests/schema/test_message.py
+-rw-r--r--   0        0        0      287 2024-04-06 20:19:01.056870 message_flow-0.3.7/tests/schema/test_message_flow.py
+-rw-r--r--   0        0        0      272 2024-04-06 20:19:01.056870 message_flow-0.3.7/tests/schema/test_operation.py
+-rw-r--r--   0        0        0     3610 1970-01-01 00:00:00.000000 message_flow-0.3.7/PKG-INFO
```

### Comparing `message_flow-0.3.6/LICENSE` & `message_flow-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `message_flow-0.3.6/README.md` & `message_flow-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `message_flow-0.3.6/pyproject.toml` & `message_flow-0.3.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "message-flow"
-version = "0.3.6"
+version = "0.3.7"
 description = "Asynchronous Communication Framework"
 authors = [
     { name = "Valentin Vorobyev", email = "voro6yov.valentin@gmail.com" },
 ]
 dependencies = [
     "pydantic>=2.5.2",
     "typer>=0.9.0",
```

### Comparing `message_flow-0.3.6/src/message_flow/app/_internal/async_api_studio/config.py` & `message_flow-0.3.7/src/message_flow/app/_internal/async_api_studio/config.py`

 * *Files identical despite different names*

### Comparing `message_flow-0.3.6/src/message_flow/app/_internal/async_api_studio/page.py` & `message_flow-0.3.7/src/message_flow/app/_internal/async_api_studio/page.py`

 * *Files identical despite different names*

### Comparing `message_flow-0.3.6/src/message_flow/app/_internal/channels.py` & `message_flow-0.3.7/src/message_flow/app/_internal/channels.py`

 * *Files identical despite different names*

### Comparing `message_flow-0.3.6/src/message_flow/app/_message_management/dispatcher.py` & `message_flow-0.3.7/src/message_flow/app/_message_management/dispatcher.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,38 +1,61 @@
 import logging
+from contextlib import ExitStack
 from typing import final
 
 from ...utils import internal
 from .._internal import Channels
+from ..base_middleware import BaseMiddleware
 from ..messaging import MessageConsumer
 from .producer import Producer
 from .routing_headers import RoutingHeaders
 
 
 @final
 @internal
 class Dispatcher:
     def __init__(
-        self, channels: Channels, message_consumer: MessageConsumer, producer: Producer, logger: logging.Logger
+        self,
+        channels: Channels,
+        message_consumer: MessageConsumer,
+        producer: Producer,
+        logger: logging.Logger,
     ) -> None:
         self._logger = logger
 
         self._channels = channels
         self._message_consumer = message_consumer
         self._producer = producer
+        self._middlewares: list[type[BaseMiddleware]] = []
 
     def initialize(self) -> None:
         self._logger.debug("Initializing dispatcher")
         self._message_consumer.subscribe(
             self._channels.addresses,
             self.message_handler,
         )
         self._logger.debug("Initialized dispatcher")
 
+    def add_middleware(self, middleware: type[BaseMiddleware]) -> None:
+        self._middlewares.append(middleware)
+
     def message_handler(self, payload: bytes, headers: dict[str, str]) -> None:
         if (
             handler := self._channels.operation_of(headers[RoutingHeaders.ADDRESS], headers[RoutingHeaders.TYPE])
         ) is None:
             return
 
-        if (message := handler(handler.message.from_payload_and_headers(payload, headers))) is not None:
-            self._producer.send(headers[RoutingHeaders.REPLY_TO], message)
+        with ExitStack() as dispatcher_stack:
+            self._execute_consume_middlewares(dispatcher_stack, payload, headers)
+
+            if (message := handler(handler.message.from_payload_and_headers(payload, headers))) is not None:
+                self._execute_produce_middlewares(dispatcher_stack, message.payload, message.headers)
+
+                self._producer.send(headers[RoutingHeaders.REPLY_TO], message)
+
+    def _execute_consume_middlewares(self, stack: ExitStack, payload: bytes, headers: dict[str, str]) -> None:
+        for middleware in self._middlewares:
+            stack.enter_context(middleware(payload, headers).consume())
+
+    def _execute_produce_middlewares(self, stack: ExitStack, payload: bytes, headers: dict[str, str]) -> None:
+        for middleware in self._middlewares:
+            stack.enter_context(middleware(payload, headers).produce())
```

### Comparing `message_flow-0.3.6/src/message_flow/app/_message_management/producer.py` & `message_flow-0.3.7/src/message_flow/app/_message_management/producer.py`

 * *Files identical despite different names*

### Comparing `message_flow-0.3.6/src/message_flow/app/_simple_messaging/simple_consumer.py` & `message_flow-0.3.7/src/message_flow/app/_simple_messaging/simple_consumer.py`

 * *Files identical despite different names*

### Comparing `message_flow-0.3.6/src/message_flow/app/_simple_messaging/simple_producer.py` & `message_flow-0.3.7/src/message_flow/app/_simple_messaging/simple_producer.py`

 * *Files identical despite different names*

### Comparing `message_flow-0.3.6/src/message_flow/app/message_flow.py` & `message_flow-0.3.7/src/message_flow/app/message_flow.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from ..channel import Channel
 from ..message import Message
 from ..utils import external, logger
 from ._fast_api import FastAPI
 from ._internal import AsyncAPIStudioPage, Channels, Info, MessageFlowSchema
 from ._message_management import Dispatcher, Producer
 from ._simple_messaging import SimpleMessageConsumer, SimpleMessageProducer
+from .base_middleware import BaseMiddleware
 from .messaging import MessageConsumer, MessageProducer
 
 MessageHandler = Callable[[Message], Message | None]
 
 
 @final
 @external
@@ -552,7 +553,46 @@
 
         documentation_page = self.generate_docs_page()
 
         async def async_api_docs_html(req: Request) -> HTMLResponse:
             return HTMLResponse(documentation_page)
 
         fast_api.add_route(documentation_url, async_api_docs_html, include_in_schema=False)
+
+    def add_middleware(
+        self, middleware: Annotated[type[BaseMiddleware], Doc("Message processing Middleware.")]
+    ) -> None:
+        """
+        Add Middleware.
+
+        **Example**
+
+        ```python title="Adding processing Middleware"
+        import logging
+        from message_flow import MessageFlow, BaseMiddleware
+
+        logger = logging.getLogger(__name__)
+
+
+        class CustomMiddleware(BaseMiddleware):
+            def on_consume(self) -> None:
+                logger.info("Message with %s payload and %s headers received.", self.payload, self.headers)
+                return super().on_consume()
+
+            def after_consume(self, error: Exception | None = None) -> None:
+                logger.info("Message with %s payload and %s headers processed.", self.payload, self.headers)
+                return super().after_consume(error)
+
+            def on_produce(self) -> None:
+                logger.info("Producing message with %s payload and %s headers.", self.payload, self.headers)
+                return super().on_produce()
+
+            def after_produce(self, error: Exception | None = None) -> None:
+                logger.info("Message with %s payload and %s headers produced.", self.payload, self.headers)
+                return super().after_produce(error)
+
+        app = MessageFlow()
+        app.add_middleware(CustomMiddleware)
+
+        ```
+        """
+        self.dispatcher.add_middleware(middleware=middleware)
```

### Comparing `message_flow-0.3.6/src/message_flow/app/messaging/consumer.py` & `message_flow-0.3.7/src/message_flow/app/messaging/consumer.py`

 * *Files identical despite different names*

### Comparing `message_flow-0.3.6/src/message_flow/app/messaging/producer.py` & `message_flow-0.3.7/src/message_flow/app/messaging/producer.py`

 * *Files identical despite different names*

### Comparing `message_flow-0.3.6/src/message_flow/channel/_internal/channel_construction.py` & `message_flow-0.3.7/src/message_flow/channel/_internal/channel_construction.py`

 * *Files identical despite different names*

### Comparing `message_flow-0.3.6/src/message_flow/channel/channel.py` & `message_flow-0.3.7/src/message_flow/channel/channel.py`

 * *Files identical despite different names*

### Comparing `message_flow-0.3.6/src/message_flow/cli/_cli_app.py` & `message_flow-0.3.7/src/message_flow/cli/_cli_app.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import logging
 from collections import defaultdict
 from importlib.util import module_from_spec, spec_from_file_location
 from pathlib import Path
-from typing import DefaultDict
+from typing import DefaultDict, final
 
 import typer
 
 from ..app import MessageFlow
 from ..utils import internal
 from ._documentation_server import DocumentationServer
 from ._logging_level import LoggingLevel
 
 
+@final
 @internal
 class CLIApp:
     LOGGING_LEVELS: DefaultDict[str, int] = defaultdict(
         lambda: logging.INFO,
         **{
             LoggingLevel.CRITICAL: logging.CRITICAL,
             LoggingLevel.ERROR: logging.ERROR,
```

### Comparing `message_flow-0.3.6/src/message_flow/cli/_documentation_server.py` & `message_flow-0.3.7/src/message_flow/cli/_documentation_server.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from http.server import BaseHTTPRequestHandler, HTTPServer
+from typing import final
 
 from ..utils import internal, logger
 
 
+@final
 @internal
 class DocumentationServer:
     def __init__(self, studio_page: str, host: str, port: int) -> None:
         self._host = host
         self._port = port
 
         self.RequestHandler.studio_page = studio_page
```

### Comparing `message_flow-0.3.6/src/message_flow/cli/entrypoint.py` & `message_flow-0.3.7/src/message_flow/cli/entrypoint.py`

 * *Files identical despite different names*

### Comparing `message_flow-0.3.6/src/message_flow/message/_internal/message_construction.py` & `message_flow-0.3.7/src/message_flow/message/_internal/message_construction.py`

 * *Files identical despite different names*

### Comparing `message_flow-0.3.6/src/message_flow/message/correlation_id.py` & `message_flow-0.3.7/src/message_flow/message/correlation_id.py`

 * *Files identical despite different names*

### Comparing `message_flow-0.3.6/src/message_flow/message/header.py` & `message_flow-0.3.7/src/message_flow/message/header.py`

 * *Files identical despite different names*

### Comparing `message_flow-0.3.6/src/message_flow/message/message.py` & `message_flow-0.3.7/src/message_flow/message/message.py`

 * *Files identical despite different names*

### Comparing `message_flow-0.3.6/src/message_flow/message/message_example.py` & `message_flow-0.3.7/src/message_flow/message/message_example.py`

 * *Files identical despite different names*

### Comparing `message_flow-0.3.6/src/message_flow/message/message_info.py` & `message_flow-0.3.7/src/message_flow/message/message_info.py`

 * *Files identical despite different names*

### Comparing `message_flow-0.3.6/src/message_flow/message/message_trait.py` & `message_flow-0.3.7/src/message_flow/message/message_trait.py`

 * *Files identical despite different names*

### Comparing `message_flow-0.3.6/src/message_flow/message/payload.py` & `message_flow-0.3.7/src/message_flow/message/payload.py`

 * *Files identical despite different names*

### Comparing `message_flow-0.3.6/src/message_flow/operation/_internal/operation_construction.py` & `message_flow-0.3.7/src/message_flow/operation/_internal/operation_construction.py`

 * *Files identical despite different names*

### Comparing `message_flow-0.3.6/src/message_flow/operation/operation.py` & `message_flow-0.3.7/src/message_flow/operation/operation.py`

 * *Files identical despite different names*

### Comparing `message_flow-0.3.6/src/message_flow/operation/operation_reply.py` & `message_flow-0.3.7/src/message_flow/operation/operation_reply.py`

 * *Files identical despite different names*

### Comparing `message_flow-0.3.6/src/message_flow/shared/components.py` & `message_flow-0.3.7/src/message_flow/shared/components.py`

 * *Files identical despite different names*

### Comparing `message_flow-0.3.6/src/message_flow/shared/reference.py` & `message_flow-0.3.7/src/message_flow/shared/reference.py`

 * *Files identical despite different names*

### Comparing `message_flow-0.3.6/src/message_flow/utils/log.py` & `message_flow-0.3.7/src/message_flow/utils/log.py`

 * *Files identical despite different names*

### Comparing `message_flow-0.3.6/src/message_flow/utils/visibility.py` & `message_flow-0.3.7/src/message_flow/utils/visibility.py`

 * *Files identical despite different names*

### Comparing `message_flow-0.3.6/tests/message/test_correlation_id.py` & `message_flow-0.3.7/tests/message/test_correlation_id.py`

 * *Files identical despite different names*

### Comparing `message_flow-0.3.6/tests/message/test_message.py` & `message_flow-0.3.7/tests/message/test_message.py`

 * *Files identical despite different names*

### Comparing `message_flow-0.3.6/tests/message/test_message_example.py` & `message_flow-0.3.7/tests/message/test_message_example.py`

 * *Files identical despite different names*

### Comparing `message_flow-0.3.6/tests/message/test_message_trait.py` & `message_flow-0.3.7/tests/message/test_message_trait.py`

 * *Files identical despite different names*

### Comparing `message_flow-0.3.6/tests/message_flow/conftest.py` & `message_flow-0.3.7/tests/message_flow/conftest.py`

 * *Files identical despite different names*

### Comparing `message_flow-0.3.6/tests/message_flow/message_flow_unit_test_support/consumer.py` & `message_flow-0.3.7/tests/message_flow/message_flow_unit_test_support/consumer.py`

 * *Files identical despite different names*

### Comparing `message_flow-0.3.6/tests/message_flow/message_flow_unit_test_support/fake_message_producer.py` & `message_flow-0.3.7/tests/message_flow/message_flow_unit_test_support/fake_message_producer.py`

 * *Files identical despite different names*

### Comparing `message_flow-0.3.6/tests/message_flow/message_flow_unit_test_support/message_flow_unit_test_support.py` & `message_flow-0.3.7/tests/message_flow/message_flow_unit_test_support/message_flow_unit_test_support.py`

 * *Files identical despite different names*

### Comparing `message_flow-0.3.6/tests/message_flow/message_flow_unit_test_support/producer.py` & `message_flow-0.3.7/tests/message_flow/message_flow_unit_test_support/producer.py`

 * *Files identical despite different names*

### Comparing `message_flow-0.3.6/tests/message_flow/test_command_sending.py` & `message_flow-0.3.7/tests/message_flow/test_command_sending.py`

 * *Files identical despite different names*

### Comparing `message_flow-0.3.6/tests/message_flow/test_dispatching.py` & `message_flow-0.3.7/tests/message_flow/test_dispatching.py`

 * *Files identical despite different names*

### Comparing `message_flow-0.3.6/tests/message_flow/test_event_publishing.py` & `message_flow-0.3.7/tests/message_flow/test_event_publishing.py`

 * *Files identical despite different names*

### Comparing `message_flow-0.3.6/tests/message_flow/test_message_flow.py` & `message_flow-0.3.7/tests/message_flow/test_message_flow.py`

 * *Files identical despite different names*

### Comparing `message_flow-0.3.6/tests/schema/conftest.py` & `message_flow-0.3.7/tests/schema/conftest.py`

 * *Files identical despite different names*

### Comparing `message_flow-0.3.6/PKG-INFO` & `message_flow-0.3.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: message-flow
-Version: 0.3.6
+Version: 0.3.7
 Summary: Asynchronous Communication Framework
 Author-Email: Valentin Vorobyev <voro6yov.valentin@gmail.com>
 License: Apache License 2.0
 Requires-Python: >=3.10
 Requires-Dist: pydantic>=2.5.2
 Requires-Dist: typer>=0.9.0
 Requires-Dist: message-flow-rabbitmq>=0.2.2; extra == "rabbitmq"
```

