# Comparing `tmp/openpipe-4.4.2.tar.gz` & `tmp/openpipe-4.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openpipe-4.4.2.tar", max compression
+gzip compressed data, was "openpipe-4.6.0.tar", max compression
```

## Comparing `openpipe-4.4.2.tar` & `openpipe-4.6.0.tar`

### file list

```diff
@@ -1,141 +1,173 @@
--rw-r--r--   0        0        0     2552 2024-01-16 03:58:24.400403 openpipe-4.4.2/README.md
--rw-r--r--   0        0        0    11357 2023-08-31 05:50:22.012971 openpipe-4.4.2/openpipe/LICENSE
--rw-r--r--   0        0        0      227 2024-02-01 22:13:10.951151 openpipe-4.4.2/openpipe/__init__.py
--rw-r--r--   0        0        0    16801 2024-02-21 03:18:30.149806 openpipe-4.4.2/openpipe/api_client/__init__.py
--rw-r--r--   0        0        0    33945 2024-02-21 03:18:30.150354 openpipe-4.4.2/openpipe/api_client/client.py
--rw-r--r--   0        0        0      519 2024-01-18 03:37:52.000000 openpipe-4.4.2/openpipe/api_client/core/__init__.py
--rw-r--r--   0        0        0      426 2024-01-18 03:37:52.000000 openpipe-4.4.2/openpipe/api_client/core/api_error.py
--rw-r--r--   0        0        0     1273 2024-01-18 03:37:52.000000 openpipe-4.4.2/openpipe/api_client/core/client_wrapper.py
--rw-r--r--   0        0        0     1047 2024-01-18 03:37:52.000000 openpipe-4.4.2/openpipe/api_client/core/datetime_utils.py
--rw-r--r--   0        0        0     3799 2024-01-18 03:37:52.000000 openpipe-4.4.2/openpipe/api_client/core/jsonable_encoder.py
--rw-r--r--   0        0        0      330 2024-01-18 03:37:52.000000 openpipe-4.4.2/openpipe/api_client/core/remove_none_from_dict.py
--rw-r--r--   0        0        0      167 2024-01-18 03:37:52.000000 openpipe-4.4.2/openpipe/api_client/environment.py
--rw-r--r--   0        0        0    25385 2024-02-21 03:18:30.150862 openpipe-4.4.2/openpipe/api_client/types/__init__.py
--rw-r--r--   0        0        0      991 2024-01-18 03:37:52.000000 openpipe-4.4.2/openpipe/api_client/types/check_cache_response.py
--rw-r--r--   0        0        0      390 2024-01-18 03:37:52.000000 openpipe-4.4.2/openpipe/api_client/types/create_chat_completion_request_function_call.py
--rw-r--r--   0        0        0      900 2024-01-18 03:37:52.000000 openpipe-4.4.2/openpipe/api_client/types/create_chat_completion_request_function_call_name.py
--rw-r--r--   0        0        0      997 2024-01-18 03:37:52.000000 openpipe-4.4.2/openpipe/api_client/types/create_chat_completion_request_functions_item.py
--rw-r--r--   0        0        0     2338 2024-01-18 03:37:52.000000 openpipe-4.4.2/openpipe/api_client/types/create_chat_completion_request_messages_item.py
--rw-r--r--   0        0        0     1630 2024-01-18 03:37:52.000000 openpipe-4.4.2/openpipe/api_client/types/create_chat_completion_request_messages_item_assistant.py
--rw-r--r--   0        0        0      240 2024-01-18 03:37:52.000000 openpipe-4.4.2/openpipe/api_client/types/create_chat_completion_request_messages_item_assistant_content.py
--rw-r--r--   0        0        0      970 2024-01-18 03:37:52.000000 openpipe-4.4.2/openpipe/api_client/types/create_chat_completion_request_messages_item_assistant_function_call.py
--rw-r--r--   0        0        0     1246 2024-01-18 03:37:52.000000 openpipe-4.4.2/openpipe/api_client/types/create_chat_completion_request_messages_item_assistant_tool_calls_item.py
--rw-r--r--   0        0        0      945 2024-01-18 03:37:52.000000 openpipe-4.4.2/openpipe/api_client/types/create_chat_completion_request_messages_item_assistant_tool_calls_item_function.py
--rw-r--r--   0        0        0     1111 2024-01-17 21:12:20.410989 openpipe-4.4.2/openpipe/api_client/types/create_chat_completion_request_messages_item_function.py
--rw-r--r--   0        0        0      239 2024-01-17 21:12:20.411181 openpipe-4.4.2/openpipe/api_client/types/create_chat_completion_request_messages_item_function_content.py
--rw-r--r--   0        0        0      922 2024-01-18 03:37:52.000000 openpipe-4.4.2/openpipe/api_client/types/create_chat_completion_request_messages_item_system.py
--rw-r--r--   0        0        0      942 2024-01-18 03:37:52.000000 openpipe-4.4.2/openpipe/api_client/types/create_chat_completion_request_messages_item_tool.py
--rw-r--r--   0        0        0     1098 2024-01-18 03:37:52.000000 openpipe-4.4.2/openpipe/api_client/types/create_chat_completion_request_messages_item_user.py
--rw-r--r--   0        0        0      367 2024-01-18 03:37:52.000000 openpipe-4.4.2/openpipe/api_client/types/create_chat_completion_request_messages_item_user_content.py
--rw-r--r--   0        0        0     1257 2024-01-18 03:37:52.000000 openpipe-4.4.2/openpipe/api_client/types/create_chat_completion_request_messages_item_user_content_item.py
--rw-r--r--   0        0        0     1167 2024-01-18 03:37:52.000000 openpipe-4.4.2/openpipe/api_client/types/create_chat_completion_request_messages_item_user_content_item_image_url.py
--rw-r--r--   0        0        0     1221 2024-01-18 03:37:52.000000 openpipe-4.4.2/openpipe/api_client/types/create_chat_completion_request_messages_item_user_content_item_image_url_image_url.py
--rw-r--r--   0        0        0      849 2024-01-18 03:37:52.000000 openpipe-4.4.2/openpipe/api_client/types/create_chat_completion_request_messages_item_user_content_item_image_url_image_url_detail.py
--rw-r--r--   0        0        0      915 2024-01-18 03:37:52.000000 openpipe-4.4.2/openpipe/api_client/types/create_chat_completion_request_messages_item_user_content_item_text.py
--rw-r--r--   0        0        0     2357 2024-01-18 03:37:52.000000 openpipe-4.4.2/openpipe/api_client/types/create_chat_completion_request_req_payload.py
--rw-r--r--   0        0        0      450 2024-01-18 03:37:52.000000 openpipe-4.4.2/openpipe/api_client/types/create_chat_completion_request_req_payload_function_call.py
--rw-r--r--   0        0        0      910 2024-01-18 03:37:52.000000 openpipe-4.4.2/openpipe/api_client/types/create_chat_completion_request_req_payload_function_call_name.py
--rw-r--r--   0        0        0     1007 2024-01-18 03:37:52.000000 openpipe-4.4.2/openpipe/api_client/types/create_chat_completion_request_req_payload_functions_item.py
--rw-r--r--   0        0        0     2665 2024-01-18 03:37:52.000000 openpipe-4.4.2/openpipe/api_client/types/create_chat_completion_request_req_payload_messages_item.py
--rw-r--r--   0        0        0     1736 2024-01-18 03:37:52.000000 openpipe-4.4.2/openpipe/api_client/types/create_chat_completion_request_req_payload_messages_item_assistant.py
--rw-r--r--   0        0        0      250 2024-01-18 03:37:52.000000 openpipe-4.4.2/openpipe/api_client/types/create_chat_completion_request_req_payload_messages_item_assistant_content.py
--rw-r--r--   0        0        0      980 2024-01-18 03:37:52.000000 openpipe-4.4.2/openpipe/api_client/types/create_chat_completion_request_req_payload_messages_item_assistant_function_call.py
--rw-r--r--   0        0        0     1288 2024-01-18 03:37:52.000000 openpipe-4.4.2/openpipe/api_client/types/create_chat_completion_request_req_payload_messages_item_assistant_tool_calls_item.py
--rw-r--r--   0        0        0      955 2024-01-18 03:37:52.000000 openpipe-4.4.2/openpipe/api_client/types/create_chat_completion_request_req_payload_messages_item_assistant_tool_calls_item_function.py
--rw-r--r--   0        0        0     1153 2024-01-17 21:12:20.411460 openpipe-4.4.2/openpipe/api_client/types/create_chat_completion_request_req_payload_messages_item_function.py
--rw-r--r--   0        0        0      249 2024-01-17 21:12:20.411643 openpipe-4.4.2/openpipe/api_client/types/create_chat_completion_request_req_payload_messages_item_function_content.py
--rw-r--r--   0        0        0      932 2024-01-18 03:37:52.000000 openpipe-4.4.2/openpipe/api_client/types/create_chat_completion_request_req_payload_messages_item_system.py
--rw-r--r--   0        0        0      952 2024-01-18 03:37:52.000000 openpipe-4.4.2/openpipe/api_client/types/create_chat_completion_request_req_payload_messages_item_tool.py
--rw-r--r--   0        0        0     1140 2024-01-18 03:37:52.000000 openpipe-4.4.2/openpipe/api_client/types/create_chat_completion_request_req_payload_messages_item_user.py
--rw-r--r--   0        0        0      409 2024-01-18 03:37:52.000000 openpipe-4.4.2/openpipe/api_client/types/create_chat_completion_request_req_payload_messages_item_user_content.py
--rw-r--r--   0        0        0     1371 2024-01-18 03:37:52.000000 openpipe-4.4.2/openpipe/api_client/types/create_chat_completion_request_req_payload_messages_item_user_content_item.py
--rw-r--r--   0        0        0     1209 2024-01-18 03:37:52.000000 openpipe-4.4.2/openpipe/api_client/types/create_chat_completion_request_req_payload_messages_item_user_content_item_image_url.py
--rw-r--r--   0        0        0     1263 2024-01-18 03:37:52.000000 openpipe-4.4.2/openpipe/api_client/types/create_chat_completion_request_req_payload_messages_item_user_content_item_image_url_image_url.py
--rw-r--r--   0        0        0      889 2024-01-18 03:37:52.000000 openpipe-4.4.2/openpipe/api_client/types/create_chat_completion_request_req_payload_messages_item_user_content_item_image_url_image_url_detail.py
--rw-r--r--   0        0        0      925 2024-01-18 03:37:52.000000 openpipe-4.4.2/openpipe/api_client/types/create_chat_completion_request_req_payload_messages_item_user_content_item_text.py
--rw-r--r--   0        0        0     1102 2024-01-18 03:37:52.000000 openpipe-4.4.2/openpipe/api_client/types/create_chat_completion_request_req_payload_response_format.py
--rw-r--r--   0        0        0      604 2024-01-18 03:37:52.000000 openpipe-4.4.2/openpipe/api_client/types/create_chat_completion_request_req_payload_response_format_type.py
--rw-r--r--   0        0        0      454 2024-01-18 03:37:52.000000 openpipe-4.4.2/openpipe/api_client/types/create_chat_completion_request_req_payload_tool_choice.py
--rw-r--r--   0        0        0     1243 2024-01-18 03:37:52.000000 openpipe-4.4.2/openpipe/api_client/types/create_chat_completion_request_req_payload_tool_choice_function.py
--rw-r--r--   0        0        0      920 2024-01-18 03:37:52.000000 openpipe-4.4.2/openpipe/api_client/types/create_chat_completion_request_req_payload_tool_choice_function_function.py
--rw-r--r--   0        0        0     1172 2024-01-18 03:37:52.000000 openpipe-4.4.2/openpipe/api_client/types/create_chat_completion_request_req_payload_tools_item.py
--rw-r--r--   0        0        0     1011 2024-01-18 03:37:52.000000 openpipe-4.4.2/openpipe/api_client/types/create_chat_completion_request_req_payload_tools_item_function.py
--rw-r--r--   0        0        0     1068 2024-01-18 03:37:52.000000 openpipe-4.4.2/openpipe/api_client/types/create_chat_completion_request_response_format.py
--rw-r--r--   0        0        0      574 2024-01-18 03:37:52.000000 openpipe-4.4.2/openpipe/api_client/types/create_chat_completion_request_response_format_type.py
--rw-r--r--   0        0        0      394 2024-01-18 03:37:52.000000 openpipe-4.4.2/openpipe/api_client/types/create_chat_completion_request_tool_choice.py
--rw-r--r--   0        0        0     1201 2024-01-18 03:37:52.000000 openpipe-4.4.2/openpipe/api_client/types/create_chat_completion_request_tool_choice_function.py
--rw-r--r--   0        0        0      910 2024-01-18 03:37:52.000000 openpipe-4.4.2/openpipe/api_client/types/create_chat_completion_request_tool_choice_function_function.py
--rw-r--r--   0        0        0     1121 2024-01-18 03:37:52.000000 openpipe-4.4.2/openpipe/api_client/types/create_chat_completion_request_tools_item.py
--rw-r--r--   0        0        0     1001 2024-01-18 03:37:52.000000 openpipe-4.4.2/openpipe/api_client/types/create_chat_completion_request_tools_item_function.py
--rw-r--r--   0        0        0      280 2024-01-18 03:37:52.000000 openpipe-4.4.2/openpipe/api_client/types/create_chat_completion_response.py
--rw-r--r--   0        0        0     1362 2024-01-18 03:37:52.000000 openpipe-4.4.2/openpipe/api_client/types/create_chat_completion_response_choices.py
--rw-r--r--   0        0        0     1561 2024-01-18 03:37:52.000000 openpipe-4.4.2/openpipe/api_client/types/create_chat_completion_response_choices_choices_item.py
--rw-r--r--   0        0        0     1263 2024-01-18 03:37:52.000000 openpipe-4.4.2/openpipe/api_client/types/create_chat_completion_response_choices_choices_item_finish_reason.py
--rw-r--r--   0        0        0     1169 2024-01-18 03:37:52.000000 openpipe-4.4.2/openpipe/api_client/types/create_chat_completion_response_choices_choices_item_logprobs.py
--rw-r--r--   0        0        0     1297 2024-01-18 03:37:52.000000 openpipe-4.4.2/openpipe/api_client/types/create_chat_completion_response_choices_choices_item_logprobs_content_item.py
--rw-r--r--   0        0        0     1004 2024-01-18 03:37:52.000000 openpipe-4.4.2/openpipe/api_client/types/create_chat_completion_response_choices_choices_item_logprobs_content_item_top_logprobs_item.py
--rw-r--r--   0        0        0     1758 2024-01-18 03:37:52.000000 openpipe-4.4.2/openpipe/api_client/types/create_chat_completion_response_choices_choices_item_message.py
--rw-r--r--   0        0        0      245 2024-01-18 03:37:52.000000 openpipe-4.4.2/openpipe/api_client/types/create_chat_completion_response_choices_choices_item_message_content.py
--rw-r--r--   0        0        0      975 2024-01-18 03:37:52.000000 openpipe-4.4.2/openpipe/api_client/types/create_chat_completion_response_choices_choices_item_message_function_call.py
--rw-r--r--   0        0        0     1267 2024-01-18 03:37:52.000000 openpipe-4.4.2/openpipe/api_client/types/create_chat_completion_response_choices_choices_item_message_tool_calls_item.py
--rw-r--r--   0        0        0      950 2024-01-18 03:37:52.000000 openpipe-4.4.2/openpipe/api_client/types/create_chat_completion_response_choices_choices_item_message_tool_calls_item_function.py
--rw-r--r--   0        0        0      961 2024-01-18 03:37:52.000000 openpipe-4.4.2/openpipe/api_client/types/create_chat_completion_response_choices_usage.py
--rw-r--r--   0        0        0     1422 2024-01-18 03:37:52.000000 openpipe-4.4.2/openpipe/api_client/types/local_testing_only_get_latest_logged_call_response.py
--rw-r--r--   0        0        0      214 2024-01-18 03:37:52.000000 openpipe-4.4.2/openpipe/api_client/types/report_request_tags_value.py
--rw-r--r--   0        0        0      947 2024-01-18 03:37:52.000000 openpipe-4.4.2/openpipe/api_client/types/report_response.py
--rw-r--r--   0        0        0      459 2024-01-18 03:37:52.000000 openpipe-4.4.2/openpipe/api_client/types/report_response_status.py
--rw-r--r--   0        0        0      884 2024-02-21 03:18:30.151183 openpipe-4.4.2/openpipe/api_client/types/unstable_dataset_create_response.py
--rw-r--r--   0        0        0     2506 2024-02-21 03:18:30.151420 openpipe-4.4.2/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item.py
--rw-r--r--   0        0        0      479 2024-02-21 03:18:30.151655 openpipe-4.4.2/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_function_call.py
--rw-r--r--   0        0        0      917 2024-02-21 03:18:30.151883 openpipe-4.4.2/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_function_call_name.py
--rw-r--r--   0        0        0     1014 2024-02-21 03:18:30.152094 openpipe-4.4.2/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_functions_item.py
--rw-r--r--   0        0        0     2870 2024-02-21 03:18:30.152326 openpipe-4.4.2/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_messages_item.py
--rw-r--r--   0        0        0     1823 2024-02-21 03:18:30.152494 openpipe-4.4.2/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_messages_item_assistant.py
--rw-r--r--   0        0        0      257 2024-02-21 03:18:30.152634 openpipe-4.4.2/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_messages_item_assistant_content.py
--rw-r--r--   0        0        0      987 2024-02-21 03:18:30.152770 openpipe-4.4.2/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_messages_item_assistant_function_call.py
--rw-r--r--   0        0        0     1317 2024-02-21 03:18:30.152921 openpipe-4.4.2/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_messages_item_assistant_tool_calls_item.py
--rw-r--r--   0        0        0      962 2024-02-21 03:18:30.153103 openpipe-4.4.2/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_messages_item_assistant_tool_calls_item_function.py
--rw-r--r--   0        0        0     1182 2024-02-21 03:18:30.153391 openpipe-4.4.2/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_messages_item_function.py
--rw-r--r--   0        0        0      256 2024-02-21 03:18:30.153658 openpipe-4.4.2/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_messages_item_function_content.py
--rw-r--r--   0        0        0      939 2024-02-21 03:18:30.153887 openpipe-4.4.2/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_messages_item_system.py
--rw-r--r--   0        0        0      959 2024-02-21 03:18:30.154113 openpipe-4.4.2/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_messages_item_tool.py
--rw-r--r--   0        0        0     1169 2024-02-21 03:18:30.154290 openpipe-4.4.2/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_messages_item_user.py
--rw-r--r--   0        0        0      438 2024-02-21 03:18:30.154518 openpipe-4.4.2/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_messages_item_user_content.py
--rw-r--r--   0        0        0     1450 2024-02-21 03:18:30.154719 openpipe-4.4.2/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_messages_item_user_content_item.py
--rw-r--r--   0        0        0     1238 2024-02-21 03:18:30.154998 openpipe-4.4.2/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_messages_item_user_content_item_image_url.py
--rw-r--r--   0        0        0     1306 2024-02-21 03:18:30.155243 openpipe-4.4.2/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_messages_item_user_content_item_image_url_image_url.py
--rw-r--r--   0        0        0      917 2024-02-21 03:18:30.155481 openpipe-4.4.2/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_messages_item_user_content_item_image_url_image_url_detail.py
--rw-r--r--   0        0        0      932 2024-02-21 03:18:30.155674 openpipe-4.4.2/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_messages_item_user_content_item_text.py
--rw-r--r--   0        0        0     1131 2024-02-21 03:18:30.155844 openpipe-4.4.2/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_response_format.py
--rw-r--r--   0        0        0      625 2024-02-21 03:18:30.156026 openpipe-4.4.2/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_response_format_type.py
--rw-r--r--   0        0        0      556 2024-02-21 03:18:30.156224 openpipe-4.4.2/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_split.py
--rw-r--r--   0        0        0      483 2024-02-21 03:18:30.156446 openpipe-4.4.2/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_tool_choice.py
--rw-r--r--   0        0        0     1272 2024-02-21 03:18:30.156695 openpipe-4.4.2/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_tool_choice_function.py
--rw-r--r--   0        0        0      927 2024-02-21 03:18:30.156931 openpipe-4.4.2/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_tool_choice_function_function.py
--rw-r--r--   0        0        0     1201 2024-02-21 03:18:30.157184 openpipe-4.4.2/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_tools_item.py
--rw-r--r--   0        0        0     1018 2024-02-21 03:18:30.157420 openpipe-4.4.2/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_tools_item_function.py
--rw-r--r--   0        0        0     1170 2024-02-21 03:18:30.157657 openpipe-4.4.2/openpipe/api_client/types/unstable_dataset_entry_create_response.py
--rw-r--r--   0        0        0      921 2024-02-21 03:18:30.157876 openpipe-4.4.2/openpipe/api_client/types/unstable_dataset_entry_create_response_errors_item.py
--rw-r--r--   0        0        0     1133 2024-02-21 03:18:30.158103 openpipe-4.4.2/openpipe/api_client/types/unstable_finetune_create_request_base_model.py
--rw-r--r--   0        0        0      885 2024-02-21 03:18:30.158311 openpipe-4.4.2/openpipe/api_client/types/unstable_finetune_create_response.py
--rw-r--r--   0        0        0     1320 2024-02-21 03:18:30.158740 openpipe-4.4.2/openpipe/api_client/types/unstable_finetune_get_response.py
--rw-r--r--   0        0        0     1311 2024-02-21 03:18:30.158989 openpipe-4.4.2/openpipe/api_client/types/unstable_finetune_get_response_status.py
--rw-r--r--   0        0        0     1180 2024-01-18 03:37:52.000000 openpipe-4.4.2/openpipe/api_client/types/update_log_tags_request_filters_item.py
--rw-r--r--   0        0        0      151 2024-01-18 03:37:52.000000 openpipe-4.4.2/openpipe/api_client/types/update_log_tags_request_filters_item_equals.py
--rw-r--r--   0        0        0      221 2024-01-18 03:37:52.000000 openpipe-4.4.2/openpipe/api_client/types/update_log_tags_request_tags_value.py
--rw-r--r--   0        0        0      972 2024-01-18 03:37:52.000000 openpipe-4.4.2/openpipe/api_client/types/update_log_tags_response.py
--rw-r--r--   0        0        0     5963 2024-02-01 22:13:10.951910 openpipe-4.4.2/openpipe/client.py
--rw-r--r--   0        0        0     3074 2024-01-06 18:20:49.920050 openpipe-4.4.2/openpipe/langchain_llm.py
--rw-r--r--   0        0        0     3790 2024-01-16 03:58:24.603704 openpipe-4.4.2/openpipe/merge_openai_chunks.py
--rw-r--r--   0        0        0     7848 2024-02-01 22:13:10.953225 openpipe-4.4.2/openpipe/openai_async_wrapper.py
--rw-r--r--   0        0        0     7018 2024-02-01 22:13:10.954111 openpipe-4.4.2/openpipe/openai_sync_wrapper.py
--rw-r--r--   0        0        0     4629 2024-02-01 22:13:10.954735 openpipe-4.4.2/openpipe/shared.py
--rw-r--r--   0        0        0    15792 2024-02-22 18:51:35.398556 openpipe-4.4.2/openpipe/test_async_client.py
--rw-r--r--   0        0        0     4173 2024-02-01 22:13:10.955933 openpipe-4.4.2/openpipe/test_async_reporting.py
--rw-r--r--   0        0        0    13251 2024-02-01 22:13:10.956349 openpipe-4.4.2/openpipe/test_async_update_logged_call_tags.py
--rw-r--r--   0        0        0     1101 2024-02-01 22:13:10.956680 openpipe-4.4.2/openpipe/test_config.py
--rw-r--r--   0        0        0    13333 2024-02-22 18:51:35.399595 openpipe-4.4.2/openpipe/test_sync_client.py
--rw-r--r--   0        0        0     3765 2024-02-01 22:13:10.957917 openpipe-4.4.2/openpipe/test_sync_reporting.py
--rw-r--r--   0        0        0    12697 2024-02-01 22:13:10.958489 openpipe-4.4.2/openpipe/test_sync_update_logged_call_tags.py
--rw-r--r--   0        0        0      842 2024-02-22 18:54:48.005095 openpipe-4.4.2/pyproject.toml
--rw-r--r--   0        0        0     3440 1970-01-01 00:00:00.000000 openpipe-4.4.2/PKG-INFO
+-rw-r--r--   0        0        0     2552 2024-02-23 22:32:58.732064 openpipe-4.6.0/README.md
+-rw-r--r--   0        0        0    11357 2024-02-23 22:32:58.732154 openpipe-4.6.0/openpipe/LICENSE
+-rw-r--r--   0        0        0      227 2024-02-23 22:32:58.732195 openpipe-4.6.0/openpipe/__init__.py
+-rw-r--r--   0        0        0    20971 2024-04-05 05:12:27.519005 openpipe-4.6.0/openpipe/api_client/__init__.py
+-rw-r--r--   0        0        0    43145 2024-04-05 05:12:27.519383 openpipe-4.6.0/openpipe/api_client/client.py
+-rw-r--r--   0        0        0      519 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/core/__init__.py
+-rw-r--r--   0        0        0      426 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/core/api_error.py
+-rw-r--r--   0        0        0     1273 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/core/client_wrapper.py
+-rw-r--r--   0        0        0     1047 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/core/datetime_utils.py
+-rw-r--r--   0        0        0     3799 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      330 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/core/remove_none_from_dict.py
+-rw-r--r--   0        0        0      167 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/environment.py
+-rw-r--r--   0        0        0    31788 2024-04-05 05:12:27.519869 openpipe-4.6.0/openpipe/api_client/types/__init__.py
+-rw-r--r--   0        0        0      991 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/check_cache_response.py
+-rw-r--r--   0        0        0      390 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_function_call.py
+-rw-r--r--   0        0        0      900 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_function_call_name.py
+-rw-r--r--   0        0        0      997 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_functions_item.py
+-rw-r--r--   0        0        0     2338 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_messages_item.py
+-rw-r--r--   0        0        0     1630 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_messages_item_assistant.py
+-rw-r--r--   0        0        0      240 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_messages_item_assistant_content.py
+-rw-r--r--   0        0        0      970 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_messages_item_assistant_function_call.py
+-rw-r--r--   0        0        0     1246 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_messages_item_assistant_tool_calls_item.py
+-rw-r--r--   0        0        0      945 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_messages_item_assistant_tool_calls_item_function.py
+-rw-r--r--   0        0        0     1111 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_messages_item_function.py
+-rw-r--r--   0        0        0      239 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_messages_item_function_content.py
+-rw-r--r--   0        0        0      922 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_messages_item_system.py
+-rw-r--r--   0        0        0      942 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_messages_item_tool.py
+-rw-r--r--   0        0        0     1098 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_messages_item_user.py
+-rw-r--r--   0        0        0      367 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_messages_item_user_content.py
+-rw-r--r--   0        0        0     1257 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_messages_item_user_content_item.py
+-rw-r--r--   0        0        0     1167 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_messages_item_user_content_item_image_url.py
+-rw-r--r--   0        0        0     1221 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_messages_item_user_content_item_image_url_image_url.py
+-rw-r--r--   0        0        0      849 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_messages_item_user_content_item_image_url_image_url_detail.py
+-rw-r--r--   0        0        0      915 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_messages_item_user_content_item_text.py
+-rw-r--r--   0        0        0     2357 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_req_payload.py
+-rw-r--r--   0        0        0      450 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_req_payload_function_call.py
+-rw-r--r--   0        0        0      910 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_req_payload_function_call_name.py
+-rw-r--r--   0        0        0     1007 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_req_payload_functions_item.py
+-rw-r--r--   0        0        0     2665 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_req_payload_messages_item.py
+-rw-r--r--   0        0        0     1736 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_req_payload_messages_item_assistant.py
+-rw-r--r--   0        0        0      250 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_req_payload_messages_item_assistant_content.py
+-rw-r--r--   0        0        0      980 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_req_payload_messages_item_assistant_function_call.py
+-rw-r--r--   0        0        0     1288 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_req_payload_messages_item_assistant_tool_calls_item.py
+-rw-r--r--   0        0        0      955 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_req_payload_messages_item_assistant_tool_calls_item_function.py
+-rw-r--r--   0        0        0     1153 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_req_payload_messages_item_function.py
+-rw-r--r--   0        0        0      249 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_req_payload_messages_item_function_content.py
+-rw-r--r--   0        0        0      932 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_req_payload_messages_item_system.py
+-rw-r--r--   0        0        0      952 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_req_payload_messages_item_tool.py
+-rw-r--r--   0        0        0     1140 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_req_payload_messages_item_user.py
+-rw-r--r--   0        0        0      409 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_req_payload_messages_item_user_content.py
+-rw-r--r--   0        0        0     1371 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_req_payload_messages_item_user_content_item.py
+-rw-r--r--   0        0        0     1209 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_req_payload_messages_item_user_content_item_image_url.py
+-rw-r--r--   0        0        0     1263 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_req_payload_messages_item_user_content_item_image_url_image_url.py
+-rw-r--r--   0        0        0      889 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_req_payload_messages_item_user_content_item_image_url_image_url_detail.py
+-rw-r--r--   0        0        0      925 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_req_payload_messages_item_user_content_item_text.py
+-rw-r--r--   0        0        0     1102 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_req_payload_response_format.py
+-rw-r--r--   0        0        0      604 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_req_payload_response_format_type.py
+-rw-r--r--   0        0        0      454 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_req_payload_tool_choice.py
+-rw-r--r--   0        0        0     1243 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_req_payload_tool_choice_function.py
+-rw-r--r--   0        0        0      920 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_req_payload_tool_choice_function_function.py
+-rw-r--r--   0        0        0     1172 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_req_payload_tools_item.py
+-rw-r--r--   0        0        0     1011 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_req_payload_tools_item_function.py
+-rw-r--r--   0        0        0     1068 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_response_format.py
+-rw-r--r--   0        0        0      574 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_response_format_type.py
+-rw-r--r--   0        0        0      394 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_tool_choice.py
+-rw-r--r--   0        0        0     1201 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_tool_choice_function.py
+-rw-r--r--   0        0        0      910 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_tool_choice_function_function.py
+-rw-r--r--   0        0        0     1121 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_tools_item.py
+-rw-r--r--   0        0        0     1001 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_tools_item_function.py
+-rw-r--r--   0        0        0      280 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_response.py
+-rw-r--r--   0        0        0     1362 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_response_choices.py
+-rw-r--r--   0        0        0     1561 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_response_choices_choices_item.py
+-rw-r--r--   0        0        0     1263 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_response_choices_choices_item_finish_reason.py
+-rw-r--r--   0        0        0     1169 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_response_choices_choices_item_logprobs.py
+-rw-r--r--   0        0        0     1297 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_response_choices_choices_item_logprobs_content_item.py
+-rw-r--r--   0        0        0     1004 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_response_choices_choices_item_logprobs_content_item_top_logprobs_item.py
+-rw-r--r--   0        0        0     1758 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_response_choices_choices_item_message.py
+-rw-r--r--   0        0        0      245 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_response_choices_choices_item_message_content.py
+-rw-r--r--   0        0        0      975 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_response_choices_choices_item_message_function_call.py
+-rw-r--r--   0        0        0     1267 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_response_choices_choices_item_message_tool_calls_item.py
+-rw-r--r--   0        0        0      950 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_response_choices_choices_item_message_tool_calls_item_function.py
+-rw-r--r--   0        0        0      961 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_response_choices_usage.py
+-rw-r--r--   0        0        0     1422 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/local_testing_only_get_latest_logged_call_response.py
+-rw-r--r--   0        0        0      392 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/report_anthropic_request_req_payload.py
+-rw-r--r--   0        0        0     1516 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/report_anthropic_request_req_payload_one.py
+-rw-r--r--   0        0        0     1294 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/report_anthropic_request_req_payload_one_messages_item.py
+-rw-r--r--   0        0        0      384 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/report_anthropic_request_req_payload_one_messages_item_content.py
+-rw-r--r--   0        0        0     1283 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/report_anthropic_request_req_payload_one_messages_item_content_item.py
+-rw-r--r--   0        0        0     1161 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/report_anthropic_request_req_payload_one_messages_item_content_item_image.py
+-rw-r--r--   0        0        0     1303 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/report_anthropic_request_req_payload_one_messages_item_content_item_image_source.py
+-rw-r--r--   0        0        0     1165 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/report_anthropic_request_req_payload_one_messages_item_content_item_image_source_media_type.py
+-rw-r--r--   0        0        0      919 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/report_anthropic_request_req_payload_one_messages_item_content_item_text.py
+-rw-r--r--   0        0        0      582 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/report_anthropic_request_req_payload_one_messages_item_role.py
+-rw-r--r--   0        0        0     1087 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/report_anthropic_request_req_payload_one_metadata.py
+-rw-r--r--   0        0        0      234 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/report_anthropic_request_req_payload_one_metadata_user_id.py
+-rw-r--r--   0        0        0     1506 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/report_anthropic_request_req_payload_zero.py
+-rw-r--r--   0        0        0     1301 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/report_anthropic_request_req_payload_zero_messages_item.py
+-rw-r--r--   0        0        0      388 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/report_anthropic_request_req_payload_zero_messages_item_content.py
+-rw-r--r--   0        0        0     1294 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/report_anthropic_request_req_payload_zero_messages_item_content_item.py
+-rw-r--r--   0        0        0     1165 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/report_anthropic_request_req_payload_zero_messages_item_content_item_image.py
+-rw-r--r--   0        0        0     1307 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/report_anthropic_request_req_payload_zero_messages_item_content_item_image_source.py
+-rw-r--r--   0        0        0     1170 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/report_anthropic_request_req_payload_zero_messages_item_content_item_image_source_media_type.py
+-rw-r--r--   0        0        0      920 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/report_anthropic_request_req_payload_zero_messages_item_content_item_text.py
+-rw-r--r--   0        0        0      585 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/report_anthropic_request_req_payload_zero_messages_item_role.py
+-rw-r--r--   0        0        0     1100 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/report_anthropic_request_req_payload_zero_metadata.py
+-rw-r--r--   0        0        0      235 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/report_anthropic_request_req_payload_zero_metadata_user_id.py
+-rw-r--r--   0        0        0     1746 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/report_anthropic_request_resp_payload.py
+-rw-r--r--   0        0        0      971 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/report_anthropic_request_resp_payload_content_item.py
+-rw-r--r--   0        0        0      360 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/report_anthropic_request_resp_payload_stop_reason.py
+-rw-r--r--   0        0        0      224 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/report_anthropic_request_resp_payload_stop_sequence.py
+-rw-r--r--   0        0        0      930 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/report_anthropic_request_resp_payload_usage.py
+-rw-r--r--   0        0        0      223 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/report_anthropic_request_tags_value.py
+-rw-r--r--   0        0        0      984 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/report_anthropic_response.py
+-rw-r--r--   0        0        0      486 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/report_anthropic_response_status.py
+-rw-r--r--   0        0        0      214 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/report_request_tags_value.py
+-rw-r--r--   0        0        0      947 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/report_response.py
+-rw-r--r--   0        0        0      459 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/report_response_status.py
+-rw-r--r--   0        0        0      974 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/unstable_dataset_create_response.py
+-rw-r--r--   0        0        0     2506 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item.py
+-rw-r--r--   0        0        0      479 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_function_call.py
+-rw-r--r--   0        0        0      917 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_function_call_name.py
+-rw-r--r--   0        0        0     1014 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_functions_item.py
+-rw-r--r--   0        0        0     2870 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_messages_item.py
+-rw-r--r--   0        0        0     1823 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_messages_item_assistant.py
+-rw-r--r--   0        0        0      257 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_messages_item_assistant_content.py
+-rw-r--r--   0        0        0      987 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_messages_item_assistant_function_call.py
+-rw-r--r--   0        0        0     1317 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_messages_item_assistant_tool_calls_item.py
+-rw-r--r--   0        0        0      962 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_messages_item_assistant_tool_calls_item_function.py
+-rw-r--r--   0        0        0     1182 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_messages_item_function.py
+-rw-r--r--   0        0        0      256 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_messages_item_function_content.py
+-rw-r--r--   0        0        0      939 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_messages_item_system.py
+-rw-r--r--   0        0        0      959 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_messages_item_tool.py
+-rw-r--r--   0        0        0     1169 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_messages_item_user.py
+-rw-r--r--   0        0        0      438 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_messages_item_user_content.py
+-rw-r--r--   0        0        0     1450 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_messages_item_user_content_item.py
+-rw-r--r--   0        0        0     1238 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_messages_item_user_content_item_image_url.py
+-rw-r--r--   0        0        0     1306 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_messages_item_user_content_item_image_url_image_url.py
+-rw-r--r--   0        0        0      917 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_messages_item_user_content_item_image_url_image_url_detail.py
+-rw-r--r--   0        0        0      932 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_messages_item_user_content_item_text.py
+-rw-r--r--   0        0        0     1131 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_response_format.py
+-rw-r--r--   0        0        0      625 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_response_format_type.py
+-rw-r--r--   0        0        0      556 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_split.py
+-rw-r--r--   0        0        0      483 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_tool_choice.py
+-rw-r--r--   0        0        0     1272 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_tool_choice_function.py
+-rw-r--r--   0        0        0      927 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_tool_choice_function_function.py
+-rw-r--r--   0        0        0     1201 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_tools_item.py
+-rw-r--r--   0        0        0     1018 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_tools_item_function.py
+-rw-r--r--   0        0        0     1170 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/unstable_dataset_entry_create_response.py
+-rw-r--r--   0        0        0      921 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/unstable_dataset_entry_create_response_errors_item.py
+-rw-r--r--   0        0        0     1133 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/unstable_finetune_create_request_base_model.py
+-rw-r--r--   0        0        0      885 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/unstable_finetune_create_response.py
+-rw-r--r--   0        0        0      890 2024-04-05 05:12:27.520179 openpipe-4.6.0/openpipe/api_client/types/unstable_finetune_delete_response.py
+-rw-r--r--   0        0        0     1320 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/unstable_finetune_get_response.py
+-rw-r--r--   0        0        0     1311 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/unstable_finetune_get_response_status.py
+-rw-r--r--   0        0        0     1180 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/update_log_tags_request_filters_item.py
+-rw-r--r--   0        0        0      151 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/update_log_tags_request_filters_item_equals.py
+-rw-r--r--   0        0        0      221 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/update_log_tags_request_tags_value.py
+-rw-r--r--   0        0        0      972 2024-04-05 01:17:30.000000 openpipe-4.6.0/openpipe/api_client/types/update_log_tags_response.py
+-rw-r--r--   0        0        0     5963 2024-02-23 22:32:58.739376 openpipe-4.6.0/openpipe/client.py
+-rw-r--r--   0        0        0     3074 2024-02-23 22:32:58.739440 openpipe-4.6.0/openpipe/langchain_llm.py
+-rw-r--r--   0        0        0     3790 2024-02-23 22:32:58.739498 openpipe-4.6.0/openpipe/merge_openai_chunks.py
+-rw-r--r--   0        0        0     7848 2024-04-05 05:24:04.792247 openpipe-4.6.0/openpipe/openai_async_wrapper.py
+-rw-r--r--   0        0        0     7018 2024-02-23 22:32:58.739663 openpipe-4.6.0/openpipe/openai_sync_wrapper.py
+-rw-r--r--   0        0        0     4629 2024-02-23 22:32:58.739734 openpipe-4.6.0/openpipe/shared.py
+-rw-r--r--   0        0        0    15825 2024-04-05 17:59:18.064759 openpipe-4.6.0/openpipe/test_async_client.py
+-rw-r--r--   0        0        0     4173 2024-02-23 22:32:58.740012 openpipe-4.6.0/openpipe/test_async_reporting.py
+-rw-r--r--   0        0        0    13251 2024-02-23 22:32:58.740141 openpipe-4.6.0/openpipe/test_async_update_logged_call_tags.py
+-rw-r--r--   0        0        0     1101 2024-02-23 22:32:58.740196 openpipe-4.6.0/openpipe/test_config.py
+-rw-r--r--   0        0        0    13366 2024-04-05 17:59:18.066602 openpipe-4.6.0/openpipe/test_sync_client.py
+-rw-r--r--   0        0        0     3765 2024-02-23 22:32:58.740380 openpipe-4.6.0/openpipe/test_sync_reporting.py
+-rw-r--r--   0        0        0    12697 2024-02-23 22:32:58.740500 openpipe-4.6.0/openpipe/test_sync_update_logged_call_tags.py
+-rw-r--r--   0        0        0      842 2024-04-05 17:59:18.068750 openpipe-4.6.0/pyproject.toml
+-rw-r--r--   0        0        0     3440 1970-01-01 00:00:00.000000 openpipe-4.6.0/PKG-INFO
```

### Comparing `openpipe-4.4.2/README.md` & `openpipe-4.6.0/README.md`

 * *Files identical despite different names*

### Comparing `openpipe-4.4.2/openpipe/LICENSE` & `openpipe-4.6.0/openpipe/LICENSE`

 * *Files identical despite different names*

### Comparing `openpipe-4.4.2/openpipe/api_client/__init__.py` & `openpipe-4.6.0/openpipe/api_client/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -81,14 +81,49 @@
     CreateChatCompletionResponseChoicesChoicesItemMessage,
     CreateChatCompletionResponseChoicesChoicesItemMessageContent,
     CreateChatCompletionResponseChoicesChoicesItemMessageFunctionCall,
     CreateChatCompletionResponseChoicesChoicesItemMessageToolCallsItem,
     CreateChatCompletionResponseChoicesChoicesItemMessageToolCallsItemFunction,
     CreateChatCompletionResponseChoicesUsage,
     LocalTestingOnlyGetLatestLoggedCallResponse,
+    ReportAnthropicRequestReqPayload,
+    ReportAnthropicRequestReqPayloadOne,
+    ReportAnthropicRequestReqPayloadOneMessagesItem,
+    ReportAnthropicRequestReqPayloadOneMessagesItemContent,
+    ReportAnthropicRequestReqPayloadOneMessagesItemContentItem,
+    ReportAnthropicRequestReqPayloadOneMessagesItemContentItemImage,
+    ReportAnthropicRequestReqPayloadOneMessagesItemContentItemImageSource,
+    ReportAnthropicRequestReqPayloadOneMessagesItemContentItemImageSourceMediaType,
+    ReportAnthropicRequestReqPayloadOneMessagesItemContentItemText,
+    ReportAnthropicRequestReqPayloadOneMessagesItemContentItem_Image,
+    ReportAnthropicRequestReqPayloadOneMessagesItemContentItem_Text,
+    ReportAnthropicRequestReqPayloadOneMessagesItemRole,
+    ReportAnthropicRequestReqPayloadOneMetadata,
+    ReportAnthropicRequestReqPayloadOneMetadataUserId,
+    ReportAnthropicRequestReqPayloadZero,
+    ReportAnthropicRequestReqPayloadZeroMessagesItem,
+    ReportAnthropicRequestReqPayloadZeroMessagesItemContent,
+    ReportAnthropicRequestReqPayloadZeroMessagesItemContentItem,
+    ReportAnthropicRequestReqPayloadZeroMessagesItemContentItemImage,
+    ReportAnthropicRequestReqPayloadZeroMessagesItemContentItemImageSource,
+    ReportAnthropicRequestReqPayloadZeroMessagesItemContentItemImageSourceMediaType,
+    ReportAnthropicRequestReqPayloadZeroMessagesItemContentItemText,
+    ReportAnthropicRequestReqPayloadZeroMessagesItemContentItem_Image,
+    ReportAnthropicRequestReqPayloadZeroMessagesItemContentItem_Text,
+    ReportAnthropicRequestReqPayloadZeroMessagesItemRole,
+    ReportAnthropicRequestReqPayloadZeroMetadata,
+    ReportAnthropicRequestReqPayloadZeroMetadataUserId,
+    ReportAnthropicRequestRespPayload,
+    ReportAnthropicRequestRespPayloadContentItem,
+    ReportAnthropicRequestRespPayloadStopReason,
+    ReportAnthropicRequestRespPayloadStopSequence,
+    ReportAnthropicRequestRespPayloadUsage,
+    ReportAnthropicRequestTagsValue,
+    ReportAnthropicResponse,
+    ReportAnthropicResponseStatus,
     ReportRequestTagsValue,
     ReportResponse,
     ReportResponseStatus,
     UnstableDatasetCreateResponse,
     UnstableDatasetEntryCreateRequestEntriesItem,
     UnstableDatasetEntryCreateRequestEntriesItemFunctionCall,
     UnstableDatasetEntryCreateRequestEntriesItemFunctionCallName,
@@ -125,14 +160,15 @@
     UnstableDatasetEntryCreateRequestEntriesItemToolChoiceFunctionFunction,
     UnstableDatasetEntryCreateRequestEntriesItemToolsItem,
     UnstableDatasetEntryCreateRequestEntriesItemToolsItemFunction,
     UnstableDatasetEntryCreateResponse,
     UnstableDatasetEntryCreateResponseErrorsItem,
     UnstableFinetuneCreateRequestBaseModel,
     UnstableFinetuneCreateResponse,
+    UnstableFinetuneDeleteResponse,
     UnstableFinetuneGetResponse,
     UnstableFinetuneGetResponseStatus,
     UpdateLogTagsRequestFiltersItem,
     UpdateLogTagsRequestFiltersItemEquals,
     UpdateLogTagsRequestTagsValue,
     UpdateLogTagsResponse,
 )
@@ -220,14 +256,49 @@
     "CreateChatCompletionResponseChoicesChoicesItemMessageContent",
     "CreateChatCompletionResponseChoicesChoicesItemMessageFunctionCall",
     "CreateChatCompletionResponseChoicesChoicesItemMessageToolCallsItem",
     "CreateChatCompletionResponseChoicesChoicesItemMessageToolCallsItemFunction",
     "CreateChatCompletionResponseChoicesUsage",
     "LocalTestingOnlyGetLatestLoggedCallResponse",
     "OpenPipeApiEnvironment",
+    "ReportAnthropicRequestReqPayload",
+    "ReportAnthropicRequestReqPayloadOne",
+    "ReportAnthropicRequestReqPayloadOneMessagesItem",
+    "ReportAnthropicRequestReqPayloadOneMessagesItemContent",
+    "ReportAnthropicRequestReqPayloadOneMessagesItemContentItem",
+    "ReportAnthropicRequestReqPayloadOneMessagesItemContentItemImage",
+    "ReportAnthropicRequestReqPayloadOneMessagesItemContentItemImageSource",
+    "ReportAnthropicRequestReqPayloadOneMessagesItemContentItemImageSourceMediaType",
+    "ReportAnthropicRequestReqPayloadOneMessagesItemContentItemText",
+    "ReportAnthropicRequestReqPayloadOneMessagesItemContentItem_Image",
+    "ReportAnthropicRequestReqPayloadOneMessagesItemContentItem_Text",
+    "ReportAnthropicRequestReqPayloadOneMessagesItemRole",
+    "ReportAnthropicRequestReqPayloadOneMetadata",
+    "ReportAnthropicRequestReqPayloadOneMetadataUserId",
+    "ReportAnthropicRequestReqPayloadZero",
+    "ReportAnthropicRequestReqPayloadZeroMessagesItem",
+    "ReportAnthropicRequestReqPayloadZeroMessagesItemContent",
+    "ReportAnthropicRequestReqPayloadZeroMessagesItemContentItem",
+    "ReportAnthropicRequestReqPayloadZeroMessagesItemContentItemImage",
+    "ReportAnthropicRequestReqPayloadZeroMessagesItemContentItemImageSource",
+    "ReportAnthropicRequestReqPayloadZeroMessagesItemContentItemImageSourceMediaType",
+    "ReportAnthropicRequestReqPayloadZeroMessagesItemContentItemText",
+    "ReportAnthropicRequestReqPayloadZeroMessagesItemContentItem_Image",
+    "ReportAnthropicRequestReqPayloadZeroMessagesItemContentItem_Text",
+    "ReportAnthropicRequestReqPayloadZeroMessagesItemRole",
+    "ReportAnthropicRequestReqPayloadZeroMetadata",
+    "ReportAnthropicRequestReqPayloadZeroMetadataUserId",
+    "ReportAnthropicRequestRespPayload",
+    "ReportAnthropicRequestRespPayloadContentItem",
+    "ReportAnthropicRequestRespPayloadStopReason",
+    "ReportAnthropicRequestRespPayloadStopSequence",
+    "ReportAnthropicRequestRespPayloadUsage",
+    "ReportAnthropicRequestTagsValue",
+    "ReportAnthropicResponse",
+    "ReportAnthropicResponseStatus",
     "ReportRequestTagsValue",
     "ReportResponse",
     "ReportResponseStatus",
     "UnstableDatasetCreateResponse",
     "UnstableDatasetEntryCreateRequestEntriesItem",
     "UnstableDatasetEntryCreateRequestEntriesItemFunctionCall",
     "UnstableDatasetEntryCreateRequestEntriesItemFunctionCallName",
@@ -264,14 +335,15 @@
     "UnstableDatasetEntryCreateRequestEntriesItemToolChoiceFunctionFunction",
     "UnstableDatasetEntryCreateRequestEntriesItemToolsItem",
     "UnstableDatasetEntryCreateRequestEntriesItemToolsItemFunction",
     "UnstableDatasetEntryCreateResponse",
     "UnstableDatasetEntryCreateResponseErrorsItem",
     "UnstableFinetuneCreateRequestBaseModel",
     "UnstableFinetuneCreateResponse",
+    "UnstableFinetuneDeleteResponse",
     "UnstableFinetuneGetResponse",
     "UnstableFinetuneGetResponseStatus",
     "UpdateLogTagsRequestFiltersItem",
     "UpdateLogTagsRequestFiltersItemEquals",
     "UpdateLogTagsRequestTagsValue",
     "UpdateLogTagsResponse",
 ]
```

### Comparing `openpipe-4.4.2/openpipe/api_client/client.py` & `openpipe-4.6.0/openpipe/api_client/client.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,21 +17,26 @@
 from .types.create_chat_completion_request_messages_item import CreateChatCompletionRequestMessagesItem
 from .types.create_chat_completion_request_req_payload import CreateChatCompletionRequestReqPayload
 from .types.create_chat_completion_request_response_format import CreateChatCompletionRequestResponseFormat
 from .types.create_chat_completion_request_tool_choice import CreateChatCompletionRequestToolChoice
 from .types.create_chat_completion_request_tools_item import CreateChatCompletionRequestToolsItem
 from .types.create_chat_completion_response import CreateChatCompletionResponse
 from .types.local_testing_only_get_latest_logged_call_response import LocalTestingOnlyGetLatestLoggedCallResponse
+from .types.report_anthropic_request_req_payload import ReportAnthropicRequestReqPayload
+from .types.report_anthropic_request_resp_payload import ReportAnthropicRequestRespPayload
+from .types.report_anthropic_request_tags_value import ReportAnthropicRequestTagsValue
+from .types.report_anthropic_response import ReportAnthropicResponse
 from .types.report_request_tags_value import ReportRequestTagsValue
 from .types.report_response import ReportResponse
 from .types.unstable_dataset_create_response import UnstableDatasetCreateResponse
 from .types.unstable_dataset_entry_create_request_entries_item import UnstableDatasetEntryCreateRequestEntriesItem
 from .types.unstable_dataset_entry_create_response import UnstableDatasetEntryCreateResponse
 from .types.unstable_finetune_create_request_base_model import UnstableFinetuneCreateRequestBaseModel
 from .types.unstable_finetune_create_response import UnstableFinetuneCreateResponse
+from .types.unstable_finetune_delete_response import UnstableFinetuneDeleteResponse
 from .types.unstable_finetune_get_response import UnstableFinetuneGetResponse
 from .types.update_log_tags_request_filters_item import UpdateLogTagsRequestFiltersItem
 from .types.update_log_tags_request_tags_value import UpdateLogTagsRequestTagsValue
 from .types.update_log_tags_response import UpdateLogTagsResponse
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
@@ -187,15 +192,15 @@
         req_payload: typing.Optional[typing.Any] = OMIT,
         resp_payload: typing.Optional[typing.Any] = OMIT,
         status_code: typing.Optional[float] = OMIT,
         error_message: typing.Optional[str] = OMIT,
         tags: typing.Optional[typing.Dict[str, ReportRequestTagsValue]] = OMIT,
     ) -> ReportResponse:
         """
-        Report an API call
+        Record request logs from OpenAI models
 
         Parameters:
             - requested_at: typing.Optional[float]. Unix timestamp in milliseconds
 
             - received_at: typing.Optional[float]. Unix timestamp in milliseconds
 
             - req_payload: typing.Optional[typing.Any].
@@ -241,14 +246,80 @@
             return pydantic.parse_obj_as(ReportResponse, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
+    def report_anthropic(
+        self,
+        *,
+        requested_at: typing.Optional[float] = OMIT,
+        received_at: typing.Optional[float] = OMIT,
+        req_payload: typing.Optional[ReportAnthropicRequestReqPayload] = OMIT,
+        resp_payload: typing.Optional[ReportAnthropicRequestRespPayload] = OMIT,
+        status_code: typing.Optional[float] = OMIT,
+        error_message: typing.Optional[str] = OMIT,
+        tags: typing.Optional[typing.Dict[str, ReportAnthropicRequestTagsValue]] = OMIT,
+    ) -> ReportAnthropicResponse:
+        """
+        Record request logs from Anthropic models
+
+        Parameters:
+            - requested_at: typing.Optional[float]. Unix timestamp in milliseconds
+
+            - received_at: typing.Optional[float]. Unix timestamp in milliseconds
+
+            - req_payload: typing.Optional[ReportAnthropicRequestReqPayload]. JSON-encoded request payload
+
+            - resp_payload: typing.Optional[ReportAnthropicRequestRespPayload]. JSON-encoded response payload
+
+            - status_code: typing.Optional[float]. HTTP status code of response
+
+            - error_message: typing.Optional[str]. User-friendly error message
+
+            - tags: typing.Optional[typing.Dict[str, ReportAnthropicRequestTagsValue]]. Extra tags to attach to the call for filtering. Eg { "userId": "123", "promptId": "populate-title" }
+        ---
+        from OpenPipe.client import OpenPipeApi
+
+        client = OpenPipeApi(
+            token="YOUR_TOKEN",
+        )
+        client.report_anthropic()
+        """
+        _request: typing.Dict[str, typing.Any] = {}
+        if requested_at is not OMIT:
+            _request["requestedAt"] = requested_at
+        if received_at is not OMIT:
+            _request["receivedAt"] = received_at
+        if req_payload is not OMIT:
+            _request["reqPayload"] = req_payload
+        if resp_payload is not OMIT:
+            _request["respPayload"] = resp_payload
+        if status_code is not OMIT:
+            _request["statusCode"] = status_code
+        if error_message is not OMIT:
+            _request["errorMessage"] = error_message
+        if tags is not OMIT:
+            _request["tags"] = tags
+        _response = self._client_wrapper.httpx_client.request(
+            "POST",
+            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "report-anthropic"),
+            json=jsonable_encoder(_request),
+            headers=self._client_wrapper.get_headers(),
+            timeout=240,
+        )
+        if 200 <= _response.status_code < 300:
+            return pydantic.parse_obj_as(ReportAnthropicResponse, _response.json())  # type: ignore
+        try:
+            _response_json = _response.json()
+        except JSONDecodeError:
+            raise ApiError(status_code=_response.status_code, body=_response.text)
+        raise ApiError(status_code=_response.status_code, body=_response_json)
+
     def update_log_tags(
         self,
         *,
         filters: typing.List[UpdateLogTagsRequestFiltersItem],
         tags: typing.Dict[str, UpdateLogTagsRequestTagsValue],
     ) -> UpdateLogTagsResponse:
         """
@@ -366,36 +437,71 @@
             return pydantic.parse_obj_as(UnstableFinetuneCreateResponse, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def unstable_finetune_get(self, *, fine_tune_id: str) -> UnstableFinetuneGetResponse:
+    def unstable_finetune_get(
+        self, *, id: typing.Optional[str] = None, slug: typing.Optional[str] = None
+    ) -> UnstableFinetuneGetResponse:
         """
         Get a finetune by ID. Note, this endpoint is unstable and may change without notice. Do not use without consulting the OpenPipe team.
 
         Parameters:
-            - fine_tune_id: str.
+            - id: typing.Optional[str].
+
+            - slug: typing.Optional[str].
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "unstable/finetune/get"),
-            params=remove_none_from_dict({"fineTuneId": fine_tune_id}),
+            params=remove_none_from_dict({"id": id, "slug": slug}),
             headers=self._client_wrapper.get_headers(),
             timeout=240,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(UnstableFinetuneGetResponse, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
+    def unstable_finetune_delete(
+        self, *, id: typing.Optional[str] = OMIT, slug: typing.Optional[str] = OMIT
+    ) -> UnstableFinetuneDeleteResponse:
+        """
+        Delete an existing finetune. Note, this endpoint is unstable and may change without notice. Do not use without consulting the OpenPipe team.
+
+        Parameters:
+            - id: typing.Optional[str].
+
+            - slug: typing.Optional[str].
+        """
+        _request: typing.Dict[str, typing.Any] = {}
+        if id is not OMIT:
+            _request["id"] = id
+        if slug is not OMIT:
+            _request["slug"] = slug
+        _response = self._client_wrapper.httpx_client.request(
+            "POST",
+            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "unstable/finetune/delete"),
+            json=jsonable_encoder(_request),
+            headers=self._client_wrapper.get_headers(),
+            timeout=240,
+        )
+        if 200 <= _response.status_code < 300:
+            return pydantic.parse_obj_as(UnstableFinetuneDeleteResponse, _response.json())  # type: ignore
+        try:
+            _response_json = _response.json()
+        except JSONDecodeError:
+            raise ApiError(status_code=_response.status_code, body=_response.text)
+        raise ApiError(status_code=_response.status_code, body=_response_json)
+
 
 class AsyncOpenPipeApi:
     def __init__(
         self,
         *,
         base_url: typing.Optional[str] = None,
         environment: OpenPipeApiEnvironment = OpenPipeApiEnvironment.DEFAULT,
@@ -538,15 +644,15 @@
         req_payload: typing.Optional[typing.Any] = OMIT,
         resp_payload: typing.Optional[typing.Any] = OMIT,
         status_code: typing.Optional[float] = OMIT,
         error_message: typing.Optional[str] = OMIT,
         tags: typing.Optional[typing.Dict[str, ReportRequestTagsValue]] = OMIT,
     ) -> ReportResponse:
         """
-        Report an API call
+        Record request logs from OpenAI models
 
         Parameters:
             - requested_at: typing.Optional[float]. Unix timestamp in milliseconds
 
             - received_at: typing.Optional[float]. Unix timestamp in milliseconds
 
             - req_payload: typing.Optional[typing.Any].
@@ -592,14 +698,80 @@
             return pydantic.parse_obj_as(ReportResponse, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
+    async def report_anthropic(
+        self,
+        *,
+        requested_at: typing.Optional[float] = OMIT,
+        received_at: typing.Optional[float] = OMIT,
+        req_payload: typing.Optional[ReportAnthropicRequestReqPayload] = OMIT,
+        resp_payload: typing.Optional[ReportAnthropicRequestRespPayload] = OMIT,
+        status_code: typing.Optional[float] = OMIT,
+        error_message: typing.Optional[str] = OMIT,
+        tags: typing.Optional[typing.Dict[str, ReportAnthropicRequestTagsValue]] = OMIT,
+    ) -> ReportAnthropicResponse:
+        """
+        Record request logs from Anthropic models
+
+        Parameters:
+            - requested_at: typing.Optional[float]. Unix timestamp in milliseconds
+
+            - received_at: typing.Optional[float]. Unix timestamp in milliseconds
+
+            - req_payload: typing.Optional[ReportAnthropicRequestReqPayload]. JSON-encoded request payload
+
+            - resp_payload: typing.Optional[ReportAnthropicRequestRespPayload]. JSON-encoded response payload
+
+            - status_code: typing.Optional[float]. HTTP status code of response
+
+            - error_message: typing.Optional[str]. User-friendly error message
+
+            - tags: typing.Optional[typing.Dict[str, ReportAnthropicRequestTagsValue]]. Extra tags to attach to the call for filtering. Eg { "userId": "123", "promptId": "populate-title" }
+        ---
+        from OpenPipe.client import AsyncOpenPipeApi
+
+        client = AsyncOpenPipeApi(
+            token="YOUR_TOKEN",
+        )
+        await client.report_anthropic()
+        """
+        _request: typing.Dict[str, typing.Any] = {}
+        if requested_at is not OMIT:
+            _request["requestedAt"] = requested_at
+        if received_at is not OMIT:
+            _request["receivedAt"] = received_at
+        if req_payload is not OMIT:
+            _request["reqPayload"] = req_payload
+        if resp_payload is not OMIT:
+            _request["respPayload"] = resp_payload
+        if status_code is not OMIT:
+            _request["statusCode"] = status_code
+        if error_message is not OMIT:
+            _request["errorMessage"] = error_message
+        if tags is not OMIT:
+            _request["tags"] = tags
+        _response = await self._client_wrapper.httpx_client.request(
+            "POST",
+            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "report-anthropic"),
+            json=jsonable_encoder(_request),
+            headers=self._client_wrapper.get_headers(),
+            timeout=240,
+        )
+        if 200 <= _response.status_code < 300:
+            return pydantic.parse_obj_as(ReportAnthropicResponse, _response.json())  # type: ignore
+        try:
+            _response_json = _response.json()
+        except JSONDecodeError:
+            raise ApiError(status_code=_response.status_code, body=_response.text)
+        raise ApiError(status_code=_response.status_code, body=_response_json)
+
     async def update_log_tags(
         self,
         *,
         filters: typing.List[UpdateLogTagsRequestFiltersItem],
         tags: typing.Dict[str, UpdateLogTagsRequestTagsValue],
     ) -> UpdateLogTagsResponse:
         """
@@ -719,36 +891,71 @@
             return pydantic.parse_obj_as(UnstableFinetuneCreateResponse, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def unstable_finetune_get(self, *, fine_tune_id: str) -> UnstableFinetuneGetResponse:
+    async def unstable_finetune_get(
+        self, *, id: typing.Optional[str] = None, slug: typing.Optional[str] = None
+    ) -> UnstableFinetuneGetResponse:
         """
         Get a finetune by ID. Note, this endpoint is unstable and may change without notice. Do not use without consulting the OpenPipe team.
 
         Parameters:
-            - fine_tune_id: str.
+            - id: typing.Optional[str].
+
+            - slug: typing.Optional[str].
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "unstable/finetune/get"),
-            params=remove_none_from_dict({"fineTuneId": fine_tune_id}),
+            params=remove_none_from_dict({"id": id, "slug": slug}),
             headers=self._client_wrapper.get_headers(),
             timeout=240,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(UnstableFinetuneGetResponse, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
+    async def unstable_finetune_delete(
+        self, *, id: typing.Optional[str] = OMIT, slug: typing.Optional[str] = OMIT
+    ) -> UnstableFinetuneDeleteResponse:
+        """
+        Delete an existing finetune. Note, this endpoint is unstable and may change without notice. Do not use without consulting the OpenPipe team.
+
+        Parameters:
+            - id: typing.Optional[str].
+
+            - slug: typing.Optional[str].
+        """
+        _request: typing.Dict[str, typing.Any] = {}
+        if id is not OMIT:
+            _request["id"] = id
+        if slug is not OMIT:
+            _request["slug"] = slug
+        _response = await self._client_wrapper.httpx_client.request(
+            "POST",
+            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "unstable/finetune/delete"),
+            json=jsonable_encoder(_request),
+            headers=self._client_wrapper.get_headers(),
+            timeout=240,
+        )
+        if 200 <= _response.status_code < 300:
+            return pydantic.parse_obj_as(UnstableFinetuneDeleteResponse, _response.json())  # type: ignore
+        try:
+            _response_json = _response.json()
+        except JSONDecodeError:
+            raise ApiError(status_code=_response.status_code, body=_response.text)
+        raise ApiError(status_code=_response.status_code, body=_response_json)
+
 
 def _get_base_url(*, base_url: typing.Optional[str] = None, environment: OpenPipeApiEnvironment) -> str:
     if base_url is not None:
         return base_url
     elif environment is not None:
         return environment.value
     else:
```

### Comparing `openpipe-4.4.2/openpipe/api_client/core/__init__.py` & `openpipe-4.6.0/openpipe/api_client/core/__init__.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.4.2/openpipe/api_client/core/client_wrapper.py` & `openpipe-4.6.0/openpipe/api_client/core/client_wrapper.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.4.2/openpipe/api_client/core/datetime_utils.py` & `openpipe-4.6.0/openpipe/api_client/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.4.2/openpipe/api_client/core/jsonable_encoder.py` & `openpipe-4.6.0/openpipe/api_client/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.4.2/openpipe/api_client/types/check_cache_response.py` & `openpipe-4.6.0/openpipe/api_client/types/check_cache_response.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.4.2/openpipe/api_client/types/create_chat_completion_request_function_call_name.py` & `openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_function_call_name.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.4.2/openpipe/api_client/types/create_chat_completion_request_functions_item.py` & `openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_functions_item.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.4.2/openpipe/api_client/types/create_chat_completion_request_messages_item.py` & `openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_messages_item.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.4.2/openpipe/api_client/types/create_chat_completion_request_messages_item_assistant.py` & `openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_messages_item_assistant.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.4.2/openpipe/api_client/types/create_chat_completion_request_messages_item_assistant_function_call.py` & `openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_messages_item_assistant_function_call.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.4.2/openpipe/api_client/types/create_chat_completion_request_messages_item_assistant_tool_calls_item.py` & `openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_messages_item_assistant_tool_calls_item.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.4.2/openpipe/api_client/types/create_chat_completion_request_messages_item_assistant_tool_calls_item_function.py` & `openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_messages_item_assistant_tool_calls_item_function.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.4.2/openpipe/api_client/types/create_chat_completion_request_messages_item_function.py` & `openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_messages_item_function.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.4.2/openpipe/api_client/types/create_chat_completion_request_messages_item_system.py` & `openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_messages_item_system.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.4.2/openpipe/api_client/types/create_chat_completion_request_messages_item_tool.py` & `openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_messages_item_tool.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.4.2/openpipe/api_client/types/create_chat_completion_request_messages_item_user.py` & `openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_messages_item_user.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.4.2/openpipe/api_client/types/create_chat_completion_request_messages_item_user_content_item.py` & `openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_messages_item_user_content_item.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.4.2/openpipe/api_client/types/create_chat_completion_request_messages_item_user_content_item_image_url.py` & `openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_messages_item_user_content_item_image_url.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.4.2/openpipe/api_client/types/create_chat_completion_request_messages_item_user_content_item_image_url_image_url.py` & `openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_messages_item_user_content_item_image_url_image_url.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.4.2/openpipe/api_client/types/create_chat_completion_request_messages_item_user_content_item_image_url_image_url_detail.py` & `openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_messages_item_user_content_item_image_url_image_url_detail.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.4.2/openpipe/api_client/types/create_chat_completion_request_messages_item_user_content_item_text.py` & `openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_messages_item_user_content_item_text.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.4.2/openpipe/api_client/types/create_chat_completion_request_req_payload.py` & `openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_req_payload.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.4.2/openpipe/api_client/types/create_chat_completion_request_req_payload_function_call_name.py` & `openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_req_payload_function_call_name.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.4.2/openpipe/api_client/types/create_chat_completion_request_req_payload_functions_item.py` & `openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_req_payload_functions_item.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.4.2/openpipe/api_client/types/create_chat_completion_request_req_payload_messages_item.py` & `openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_req_payload_messages_item.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.4.2/openpipe/api_client/types/create_chat_completion_request_req_payload_messages_item_assistant.py` & `openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_req_payload_messages_item_assistant.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.4.2/openpipe/api_client/types/create_chat_completion_request_req_payload_messages_item_assistant_function_call.py` & `openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_req_payload_messages_item_assistant_function_call.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.4.2/openpipe/api_client/types/create_chat_completion_request_req_payload_messages_item_assistant_tool_calls_item.py` & `openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_req_payload_messages_item_assistant_tool_calls_item.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.4.2/openpipe/api_client/types/create_chat_completion_request_req_payload_messages_item_assistant_tool_calls_item_function.py` & `openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_req_payload_messages_item_assistant_tool_calls_item_function.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.4.2/openpipe/api_client/types/create_chat_completion_request_req_payload_messages_item_function.py` & `openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_req_payload_messages_item_function.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.4.2/openpipe/api_client/types/create_chat_completion_request_req_payload_messages_item_system.py` & `openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_req_payload_messages_item_system.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.4.2/openpipe/api_client/types/create_chat_completion_request_req_payload_messages_item_tool.py` & `openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_req_payload_messages_item_tool.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.4.2/openpipe/api_client/types/create_chat_completion_request_req_payload_messages_item_user.py` & `openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_req_payload_messages_item_user.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.4.2/openpipe/api_client/types/create_chat_completion_request_req_payload_messages_item_user_content_item.py` & `openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_req_payload_messages_item_user_content_item.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.4.2/openpipe/api_client/types/create_chat_completion_request_req_payload_messages_item_user_content_item_image_url.py` & `openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_req_payload_messages_item_user_content_item_image_url.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.4.2/openpipe/api_client/types/create_chat_completion_request_req_payload_messages_item_user_content_item_image_url_image_url.py` & `openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_req_payload_messages_item_user_content_item_image_url_image_url.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.4.2/openpipe/api_client/types/create_chat_completion_request_req_payload_messages_item_user_content_item_image_url_image_url_detail.py` & `openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_req_payload_messages_item_user_content_item_image_url_image_url_detail.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.4.2/openpipe/api_client/types/create_chat_completion_request_req_payload_messages_item_user_content_item_text.py` & `openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_req_payload_messages_item_user_content_item_text.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.4.2/openpipe/api_client/types/create_chat_completion_request_req_payload_response_format.py` & `openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_req_payload_response_format.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.4.2/openpipe/api_client/types/create_chat_completion_request_req_payload_response_format_type.py` & `openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_req_payload_response_format_type.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.4.2/openpipe/api_client/types/create_chat_completion_request_req_payload_tool_choice_function.py` & `openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_req_payload_tool_choice_function.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.4.2/openpipe/api_client/types/create_chat_completion_request_req_payload_tool_choice_function_function.py` & `openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_req_payload_tool_choice_function_function.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.4.2/openpipe/api_client/types/create_chat_completion_request_req_payload_tools_item.py` & `openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_req_payload_tools_item.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.4.2/openpipe/api_client/types/create_chat_completion_request_req_payload_tools_item_function.py` & `openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_req_payload_tools_item_function.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.4.2/openpipe/api_client/types/create_chat_completion_request_response_format.py` & `openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_response_format.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.4.2/openpipe/api_client/types/create_chat_completion_request_response_format_type.py` & `openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_response_format_type.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.4.2/openpipe/api_client/types/create_chat_completion_request_tool_choice_function.py` & `openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_tool_choice_function.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.4.2/openpipe/api_client/types/create_chat_completion_request_tool_choice_function_function.py` & `openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_tool_choice_function_function.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.4.2/openpipe/api_client/types/create_chat_completion_request_tools_item.py` & `openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_tools_item.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.4.2/openpipe/api_client/types/create_chat_completion_request_tools_item_function.py` & `openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_request_tools_item_function.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.4.2/openpipe/api_client/types/create_chat_completion_response_choices.py` & `openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_response_choices.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.4.2/openpipe/api_client/types/create_chat_completion_response_choices_choices_item.py` & `openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_response_choices_choices_item.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.4.2/openpipe/api_client/types/create_chat_completion_response_choices_choices_item_finish_reason.py` & `openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_response_choices_choices_item_finish_reason.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.4.2/openpipe/api_client/types/create_chat_completion_response_choices_choices_item_logprobs.py` & `openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_response_choices_choices_item_logprobs.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.4.2/openpipe/api_client/types/create_chat_completion_response_choices_choices_item_logprobs_content_item.py` & `openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_response_choices_choices_item_logprobs_content_item.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.4.2/openpipe/api_client/types/create_chat_completion_response_choices_choices_item_logprobs_content_item_top_logprobs_item.py` & `openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_response_choices_choices_item_logprobs_content_item_top_logprobs_item.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.4.2/openpipe/api_client/types/create_chat_completion_response_choices_choices_item_message.py` & `openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_response_choices_choices_item_message.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.4.2/openpipe/api_client/types/create_chat_completion_response_choices_choices_item_message_function_call.py` & `openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_response_choices_choices_item_message_function_call.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.4.2/openpipe/api_client/types/create_chat_completion_response_choices_choices_item_message_tool_calls_item.py` & `openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_response_choices_choices_item_message_tool_calls_item.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.4.2/openpipe/api_client/types/create_chat_completion_response_choices_choices_item_message_tool_calls_item_function.py` & `openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_response_choices_choices_item_message_tool_calls_item_function.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.4.2/openpipe/api_client/types/create_chat_completion_response_choices_usage.py` & `openpipe-4.6.0/openpipe/api_client/types/create_chat_completion_response_choices_usage.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.4.2/openpipe/api_client/types/local_testing_only_get_latest_logged_call_response.py` & `openpipe-4.6.0/openpipe/api_client/types/local_testing_only_get_latest_logged_call_response.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.4.2/openpipe/api_client/types/report_response.py` & `openpipe-4.6.0/openpipe/api_client/types/report_response.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.4.2/openpipe/api_client/types/unstable_dataset_create_response.py` & `openpipe-4.6.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_function_call_name.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class UnstableDatasetCreateResponse(pydantic.BaseModel):
-    id: str
+class UnstableDatasetEntryCreateRequestEntriesItemFunctionCallName(pydantic.BaseModel):
+    name: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `openpipe-4.4.2/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item.py` & `openpipe-4.6.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.4.2/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_function_call_name.py` & `openpipe-4.6.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_messages_item_user_content_item_text.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class UnstableDatasetEntryCreateRequestEntriesItemFunctionCallName(pydantic.BaseModel):
-    name: str
+class UnstableDatasetEntryCreateRequestEntriesItemMessagesItemUserContentItemText(pydantic.BaseModel):
+    text: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `openpipe-4.4.2/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_functions_item.py` & `openpipe-4.6.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_functions_item.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.4.2/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_messages_item.py` & `openpipe-4.6.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_messages_item.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.4.2/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_messages_item_assistant.py` & `openpipe-4.6.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_messages_item_assistant.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.4.2/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_messages_item_assistant_function_call.py` & `openpipe-4.6.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_messages_item_assistant_function_call.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.4.2/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_messages_item_assistant_tool_calls_item.py` & `openpipe-4.6.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_messages_item_assistant_tool_calls_item.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.4.2/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_messages_item_assistant_tool_calls_item_function.py` & `openpipe-4.6.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_messages_item_assistant_tool_calls_item_function.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.4.2/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_messages_item_function.py` & `openpipe-4.6.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_messages_item_function.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.4.2/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_messages_item_system.py` & `openpipe-4.6.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_messages_item_system.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.4.2/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_messages_item_tool.py` & `openpipe-4.6.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_messages_item_tool.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.4.2/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_messages_item_user.py` & `openpipe-4.6.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_messages_item_user.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.4.2/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_messages_item_user_content_item.py` & `openpipe-4.6.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_messages_item_user_content_item.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.4.2/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_messages_item_user_content_item_image_url.py` & `openpipe-4.6.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_messages_item_user_content_item_image_url.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.4.2/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_messages_item_user_content_item_image_url_image_url.py` & `openpipe-4.6.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_messages_item_user_content_item_image_url_image_url.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.4.2/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_messages_item_user_content_item_image_url_image_url_detail.py` & `openpipe-4.6.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_messages_item_user_content_item_image_url_image_url_detail.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.4.2/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_messages_item_user_content_item_text.py` & `openpipe-4.6.0/openpipe/api_client/types/update_log_tags_response.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,22 +7,23 @@
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class UnstableDatasetEntryCreateRequestEntriesItemMessagesItemUserContentItemText(pydantic.BaseModel):
-    text: str
+class UpdateLogTagsResponse(pydantic.BaseModel):
+    matched_logs: float = pydantic.Field(alias="matchedLogs")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        allow_population_by_field_name = True
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `openpipe-4.4.2/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_response_format.py` & `openpipe-4.6.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_response_format.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.4.2/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_response_format_type.py` & `openpipe-4.6.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_response_format_type.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.4.2/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_split.py` & `openpipe-4.6.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_split.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.4.2/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_tool_choice_function.py` & `openpipe-4.6.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_tool_choice_function.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.4.2/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_tool_choice_function_function.py` & `openpipe-4.6.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_tool_choice_function_function.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.4.2/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_tools_item.py` & `openpipe-4.6.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_tools_item.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.4.2/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_tools_item_function.py` & `openpipe-4.6.0/openpipe/api_client/types/unstable_dataset_entry_create_request_entries_item_tools_item_function.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.4.2/openpipe/api_client/types/unstable_dataset_entry_create_response.py` & `openpipe-4.6.0/openpipe/api_client/types/unstable_dataset_entry_create_response.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.4.2/openpipe/api_client/types/unstable_dataset_entry_create_response_errors_item.py` & `openpipe-4.6.0/openpipe/api_client/types/unstable_dataset_entry_create_response_errors_item.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.4.2/openpipe/api_client/types/unstable_finetune_create_request_base_model.py` & `openpipe-4.6.0/openpipe/api_client/types/unstable_finetune_create_request_base_model.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.4.2/openpipe/api_client/types/unstable_finetune_create_response.py` & `openpipe-4.6.0/openpipe/api_client/types/unstable_finetune_create_response.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.4.2/openpipe/api_client/types/unstable_finetune_get_response.py` & `openpipe-4.6.0/openpipe/api_client/types/unstable_finetune_get_response.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.4.2/openpipe/api_client/types/unstable_finetune_get_response_status.py` & `openpipe-4.6.0/openpipe/api_client/types/unstable_finetune_get_response_status.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.4.2/openpipe/api_client/types/update_log_tags_request_filters_item.py` & `openpipe-4.6.0/openpipe/api_client/types/update_log_tags_request_filters_item.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.4.2/openpipe/api_client/types/update_log_tags_response.py` & `openpipe-4.6.0/openpipe/api_client/types/unstable_dataset_create_response.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class UpdateLogTagsResponse(pydantic.BaseModel):
-    matched_logs: float = pydantic.Field(alias="matchedLogs")
+class UnstableDatasetCreateResponse(pydantic.BaseModel):
+    dataset_id: str = pydantic.Field(alias="datasetId")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `openpipe-4.4.2/openpipe/client.py` & `openpipe-4.6.0/openpipe/client.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.4.2/openpipe/langchain_llm.py` & `openpipe-4.6.0/openpipe/langchain_llm.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.4.2/openpipe/merge_openai_chunks.py` & `openpipe-4.6.0/openpipe/merge_openai_chunks.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.4.2/openpipe/openai_async_wrapper.py` & `openpipe-4.6.0/openpipe/openai_async_wrapper.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.4.2/openpipe/openai_sync_wrapper.py` & `openpipe-4.6.0/openpipe/openai_sync_wrapper.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.4.2/openpipe/shared.py` & `openpipe-4.6.0/openpipe/shared.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.4.2/openpipe/test_async_client.py` & `openpipe-4.6.0/openpipe/test_async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -452,15 +452,15 @@
         return
 
     await asyncio.sleep(0.1)
     last_logged = (
         await client.openpipe_reporting_client.base_client.local_testing_only_get_latest_logged_call()
     )
     assert (
-        last_logged.error_message == "The model `gpt-3.5-turbo-blaster` does not exist"
+        last_logged.error_message == "The model `gpt-3.5-turbo-blaster` does not exist or you do not have access to it."
     )
     assert last_logged.status_code == 404
 
 
 async def test_async_bad_openpipe_call():
     try:
         await client.chat.completions.create(
```

### Comparing `openpipe-4.4.2/openpipe/test_async_reporting.py` & `openpipe-4.6.0/openpipe/test_async_reporting.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.4.2/openpipe/test_async_update_logged_call_tags.py` & `openpipe-4.6.0/openpipe/test_async_update_logged_call_tags.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.4.2/openpipe/test_config.py` & `openpipe-4.6.0/openpipe/test_config.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.4.2/openpipe/test_sync_client.py` & `openpipe-4.6.0/openpipe/test_sync_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -393,15 +393,15 @@
     if not TEST_LAST_LOGGED:
         return
 
     last_logged = (
         client.openpipe_reporting_client.base_client.local_testing_only_get_latest_logged_call()
     )
     assert (
-        last_logged.error_message == "The model `gpt-3.5-turbo-blaster` does not exist"
+        last_logged.error_message == "The model `gpt-3.5-turbo-blaster` does not exist or you do not have access to it."
     )
     assert last_logged.status_code == 404
 
 
 def test_bad_openpipe_call():
     try:
         client.chat.completions.create(
```

### Comparing `openpipe-4.4.2/openpipe/test_sync_reporting.py` & `openpipe-4.6.0/openpipe/test_sync_reporting.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.4.2/openpipe/test_sync_update_logged_call_tags.py` & `openpipe-4.6.0/openpipe/test_sync_update_logged_call_tags.py`

 * *Files identical despite different names*

### Comparing `openpipe-4.4.2/pyproject.toml` & `openpipe-4.6.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "openpipe"
-version = "4.4.2"
+version = "4.6.0"
 description = "Python client library for the OpenPipe service"
 authors = ["Kyle Corbitt <kyle@openpipe.ai>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/OpenPipe/OpenPipe"
 repository = "https://github.com/OpenPipe/OpenPipe"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 httpx = "^0.24.1"
 attrs = "^23.1.0"
 python-dateutil = "^2.8.2"
-openai = ">=1.7,<1.13"
+openai = ">=1.7,<1.16"
 
 [tool.poetry.dev-dependencies]
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.7.0"
 isort = "^5.12.0"
 autoflake = "^2.2.0"
```

### Comparing `openpipe-4.4.2/PKG-INFO` & `openpipe-4.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openpipe
-Version: 4.4.2
+Version: 4.6.0
 Summary: Python client library for the OpenPipe service
 Home-page: https://github.com/OpenPipe/OpenPipe
 License: Apache-2.0
 Author: Kyle Corbitt
 Author-email: kyle@openpipe.ai
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: attrs (>=23.1.0,<24.0.0)
 Requires-Dist: httpx (>=0.24.1,<0.25.0)
-Requires-Dist: openai (>=1.7,<1.13)
+Requires-Dist: openai (>=1.7,<1.16)
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
 Project-URL: Repository, https://github.com/OpenPipe/OpenPipe
 Description-Content-Type: text/markdown
 
 # OpenPipe Python Client
 
 This client allows you automatically report your OpenAI calls to [OpenPipe](https://openpipe.ai/).
```

