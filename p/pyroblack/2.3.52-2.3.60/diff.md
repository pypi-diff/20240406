# Comparing `tmp/pyroblack-2.3.52.tar.gz` & `tmp/pyroblack-2.3.60.tar.gz`

## Comparing `pyroblack-2.3.52.tar` & `pyroblack-2.3.60.tar`

### file list

```diff
@@ -1,553 +1,559 @@
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 pyroblack-2.3.52/MANIFEST.in
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 pyroblack-2.3.52/Makefile
--rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 pyroblack-2.3.52/build-docs.sh
--rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 pyroblack-2.3.52/compiler/__init__.py
--rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 pyroblack-2.3.52/compiler/api/__init__.py
--rw-r--r--   0        0        0    23145 2020-02-02 00:00:00.000000 pyroblack-2.3.52/compiler/api/compiler.py
--rw-r--r--   0        0        0     2233 2020-02-02 00:00:00.000000 pyroblack-2.3.52/compiler/api/source/auth_key.tl
--rw-r--r--   0        0        0   198353 2020-02-02 00:00:00.000000 pyroblack-2.3.52/compiler/api/source/main_api.tl
--rw-r--r--   0        0        0     3425 2020-02-02 00:00:00.000000 pyroblack-2.3.52/compiler/api/source/sys_msgs.tl
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 pyroblack-2.3.52/compiler/api/template/combinator.txt
--rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 pyroblack-2.3.52/compiler/api/template/type.txt
--rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 pyroblack-2.3.52/compiler/errors/__init__.py
--rw-r--r--   0        0        0     5446 2020-02-02 00:00:00.000000 pyroblack-2.3.52/compiler/errors/compiler.py
--rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 pyroblack-2.3.52/compiler/errors/sort.py
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 pyroblack-2.3.52/compiler/errors/source/303_SEE_OTHER.tsv
--rw-r--r--   0        0        0    23909 2020-02-02 00:00:00.000000 pyroblack-2.3.52/compiler/errors/source/400_BAD_REQUEST.tsv
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 pyroblack-2.3.52/compiler/errors/source/401_UNAUTHORIZED.tsv
--rw-r--r--   0        0        0     2807 2020-02-02 00:00:00.000000 pyroblack-2.3.52/compiler/errors/source/403_FORBIDDEN.tsv
--rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 pyroblack-2.3.52/compiler/errors/source/406_NOT_ACCEPTABLE.tsv
--rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 pyroblack-2.3.52/compiler/errors/source/420_FLOOD.tsv
--rw-r--r--   0        0        0     4323 2020-02-02 00:00:00.000000 pyroblack-2.3.52/compiler/errors/source/500_INTERNAL_SERVER_ERROR.tsv
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 pyroblack-2.3.52/compiler/errors/source/503_SERVICE_UNAVAILABLE.tsv
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 pyroblack-2.3.52/compiler/errors/template/class.txt
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 pyroblack-2.3.52/compiler/errors/template/sub_class.txt
--rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/__init__.py
--rw-r--r--   0        0        0    48369 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/client.py
--rw-r--r--   0        0        0    12082 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/dispatcher.py
--rw-r--r--   0        0        0   209155 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/emoji.py
--rw-r--r--   0        0        0    15602 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/file_id.py
--rw-r--r--   0        0        0    27713 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/filters.py
--rw-r--r--   0        0        0    61915 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/mime_types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/py.typed
--rw-r--r--   0        0        0     3944 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/sync.py
--rw-r--r--   0        0        0    16394 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/utils.py
--rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/connection/__init__.py
--rw-r--r--   0        0        0     2828 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/connection/connection.py
--rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/connection/transport/__init__.py
--rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/connection/transport/tcp/__init__.py
--rw-r--r--   0        0        0     4115 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/connection/transport/tcp/tcp.py
--rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/connection/transport/tcp/tcp_abridged.py
--rw-r--r--   0        0        0     2960 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/connection/transport/tcp/tcp_abridged_o.py
--rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/connection/transport/tcp/tcp_full.py
--rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/connection/transport/tcp/tcp_intermediate.py
--rw-r--r--   0        0        0     2471 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/connection/transport/tcp/tcp_intermediate_o.py
--rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/crypto/__init__.py
--rw-r--r--   0        0        0     4073 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/crypto/aes.py
--rw-r--r--   0        0        0     4118 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/crypto/mtproto.py
--rw-r--r--   0        0        0     2448 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/crypto/prime.py
--rw-r--r--   0        0        0    13485 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/crypto/rsa.py
--rw-r--r--   0        0        0     2176 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/enums/__init__.py
--rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/enums/auto_name.py
--rw-r--r--   0        0        0     1261 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/enums/business_schedule.py
--rw-r--r--   0        0        0     2307 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/enums/chat_action.py
--rw-r--r--   0        0        0     4665 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/enums/chat_event_action.py
--rw-r--r--   0        0        0     1265 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/enums/chat_member_status.py
--rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/enums/chat_members_filter.py
--rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/enums/chat_type.py
--rw-r--r--   0        0        0     1211 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/enums/listerner_types.py
--rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/enums/message_entity_type.py
--rw-r--r--   0        0        0     1765 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/enums/message_media_type.py
--rw-r--r--   0        0        0     3008 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/enums/message_service_type.py
--rw-r--r--   0        0        0     2406 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/enums/messages_filter.py
--rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/enums/next_code_type.py
--rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/enums/parse_mode.py
--rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/enums/poll_type.py
--rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/enums/profile_color.py
--rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/enums/reaction_type.py
--rw-r--r--   0        0        0     2541 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/enums/reply_color.py
--rw-r--r--   0        0        0     2000 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/enums/sent_code_type.py
--rw-r--r--   0        0        0     1378 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/enums/stories_privacy_rules.py
--rw-r--r--   0        0        0     1316 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/enums/story_privacy.py
--rw-r--r--   0        0        0     1299 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/enums/user_status.py
--rw-r--r--   0        0        0     2669 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/errors/__init__.py
--rw-r--r--   0        0        0     3539 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/errors/rpc_error.py
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/errors/pyromod/__init__.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/errors/pyromod/listener_stopped.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/errors/pyromod/listener_timeout.py
--rw-r--r--   0        0        0     1877 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/handlers/__init__.py
--rw-r--r--   0        0        0     7884 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/handlers/callback_query_handler.py
--rw-r--r--   0        0        0     2011 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/handlers/chat_join_request_handler.py
--rw-r--r--   0        0        0     2046 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/handlers/chat_member_updated_handler.py
--rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/handlers/chosen_inline_result_handler.py
--rw-r--r--   0        0        0     2527 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/handlers/conversation_handler.py
--rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/handlers/deleted_messages_handler.py
--rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/handlers/disconnect_handler.py
--rw-r--r--   0        0        0     1979 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/handlers/edited_message_handler.py
--rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/handlers/handler.py
--rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/handlers/inline_query_handler.py
--rw-r--r--   0        0        0     6078 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/handlers/message_handler.py
--rw-r--r--   0        0        0     2143 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/handlers/message_reaction_count_updated_handler.py
--rw-r--r--   0        0        0     2089 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/handlers/message_reaction_updated_handler.py
--rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/handlers/poll_handler.py
--rw-r--r--   0        0        0     2942 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/handlers/raw_update_handler.py
--rw-r--r--   0        0        0     1996 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/handlers/story_handler.py
--rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/handlers/user_status_handler.py
--rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/helpers/__init__.py
--rw-r--r--   0        0        0     3480 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/helpers/helpers.py
--rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/__init__.py
--rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/advanced/__init__.py
--rw-r--r--   0        0        0     3163 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/advanced/invoke.py
--rw-r--r--   0        0        0     4304 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/advanced/resolve_peer.py
--rw-r--r--   0        0        0     8592 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/advanced/save_file.py
--rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/auth/__init__.py
--rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/auth/accept_terms_of_service.py
--rw-r--r--   0        0        0     1900 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/auth/check_password.py
--rw-r--r--   0        0        0     1774 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/auth/connect.py
--rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/auth/disconnect.py
--rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/auth/get_password_hint.py
--rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/auth/initialize.py
--rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/auth/log_out.py
--rw-r--r--   0        0        0     1771 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/auth/recover_password.py
--rw-r--r--   0        0        0     2118 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/auth/resend_code.py
--rw-r--r--   0        0        0     5099 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/auth/send_code.py
--rw-r--r--   0        0        0     1473 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/auth/send_recovery_code.py
--rw-r--r--   0        0        0     3087 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/auth/sign_in.py
--rw-r--r--   0        0        0     2719 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/auth/sign_in_bot.py
--rw-r--r--   0        0        0     2357 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/auth/sign_up.py
--rw-r--r--   0        0        0     2042 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/auth/terminate.py
--rw-r--r--   0        0        0     2148 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/bots/__init__.py
--rw-r--r--   0        0        0     3313 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/bots/answer_callback_query.py
--rw-r--r--   0        0        0     5060 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/bots/answer_inline_query.py
--rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/bots/answer_web_app_query.py
--rw-r--r--   0        0        0     2360 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/bots/delete_bot_commands.py
--rw-r--r--   0        0        0     2573 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/bots/get_bot_commands.py
--rw-r--r--   0        0        0     2037 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/bots/get_bot_default_privileges.py
--rw-r--r--   0        0        0     1887 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/bots/get_bot_info.py
--rw-r--r--   0        0        0     2364 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/bots/get_chat_menu_button.py
--rw-r--r--   0        0        0     2909 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/bots/get_game_high_scores.py
--rw-r--r--   0        0        0     3479 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/bots/get_inline_bot_results.py
--rw-r--r--   0        0        0     2964 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/bots/request_callback_answer.py
--rw-r--r--   0        0        0     4645 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/bots/send_game.py
--rw-r--r--   0        0        0     4394 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/bots/send_inline_bot_result.py
--rw-r--r--   0        0        0     2710 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/bots/set_bot_commands.py
--rw-r--r--   0        0        0     3284 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/bots/set_bot_default_privileges.py
--rw-r--r--   0        0        0     2325 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/bots/set_bot_info.py
--rw-r--r--   0        0        0     2070 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/bots/set_chat_menu_button.py
--rw-r--r--   0        0        0     4056 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/bots/set_game_score.py
--rw-r--r--   0        0        0     4717 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/chats/__init__.py
--rw-r--r--   0        0        0     3412 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/chats/add_chat_members.py
--rw-r--r--   0        0        0     2252 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/chats/archive_chats.py
--rw-r--r--   0        0        0     4871 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/chats/ban_chat_member.py
--rw-r--r--   0        0        0     1939 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/chats/close_forum_topic.py
--rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/chats/close_general_topic.py
--rw-r--r--   0        0        0     1769 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/chats/create_channel.py
--rw-r--r--   0        0        0     2494 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/chats/create_forum_topic.py
--rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/chats/create_group.py
--rw-r--r--   0        0        0     1907 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/chats/create_supergroup.py
--rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/chats/delete_channel.py
--rw-r--r--   0        0        0     2345 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/chats/delete_chat_photo.py
--rw-r--r--   0        0        0     2046 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/chats/delete_forum_topic.py
--rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/chats/delete_supergroup.py
--rw-r--r--   0        0        0     2143 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/chats/delete_user_history.py
--rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/chats/edit_forum_topic.py
--rw-r--r--   0        0        0     1921 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/chats/edit_general_topic.py
--rw-r--r--   0        0        0     3378 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/chats/get_chat.py
--rw-r--r--   0        0        0     4120 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/chats/get_chat_event_log.py
--rw-r--r--   0        0        0     3399 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/chats/get_chat_member.py
--rw-r--r--   0        0        0     5305 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/chats/get_chat_members.py
--rw-r--r--   0        0        0     2206 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/chats/get_chat_members_count.py
--rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/chats/get_chat_online_count.py
--rw-r--r--   0        0        0     3574 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/chats/get_dialogs.py
--rw-r--r--   0        0        0     2203 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/chats/get_dialogs_count.py
--rw-r--r--   0        0        0     2495 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/chats/get_forum_topics.py
--rw-r--r--   0        0        0     3314 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/chats/get_forum_topics_by_id.py
--rw-r--r--   0        0        0     2327 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/chats/get_nearby_chats.py
--rw-r--r--   0        0        0     2275 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/chats/get_send_as_chats.py
--rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/chats/hide_general_topic.py
--rw-r--r--   0        0        0     2669 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/chats/join_chat.py
--rw-r--r--   0        0        0     2585 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/chats/leave_chat.py
--rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/chats/mark_chat_unread.py
--rw-r--r--   0        0        0     3244 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/chats/pin_chat_message.py
--rw-r--r--   0        0        0     4461 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/chats/promote_chat_member.py
--rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/chats/reopen_forum_topic.py
--rw-r--r--   0        0        0     1859 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/chats/reopen_general_topic.py
--rw-r--r--   0        0        0    10996 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/chats/restrict_chat_member.py
--rw-r--r--   0        0        0     3313 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/chats/set_administrator_title.py
--rw-r--r--   0        0        0     2259 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/chats/set_chat_description.py
--rw-r--r--   0        0        0    10011 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/chats/set_chat_permissions.py
--rw-r--r--   0        0        0     4629 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/chats/set_chat_photo.py
--rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/chats/set_chat_protected_content.py
--rw-r--r--   0        0        0     2526 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/chats/set_chat_title.py
--rw-r--r--   0        0        0     2342 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/chats/set_chat_username.py
--rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/chats/set_send_as_chat.py
--rw-r--r--   0        0        0     2132 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/chats/set_slow_mode.py
--rw-r--r--   0        0        0     1491 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/chats/toggle_folder_tags.py
--rw-r--r--   0        0        0     2069 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/chats/toggle_forum_topics.py
--rw-r--r--   0        0        0     2152 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/chats/toggle_join_to_send.py
--rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/chats/unarchive_chats.py
--rw-r--r--   0        0        0     2338 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/chats/unban_chat_member.py
--rw-r--r--   0        0        0     1849 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/chats/unhide_general_topic.py
--rw-r--r--   0        0        0     2026 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/chats/unpin_all_chat_messages.py
--rw-r--r--   0        0        0     2177 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/chats/unpin_chat_message.py
--rw-r--r--   0        0        0     2758 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/chats/update_color.py
--rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/contacts/__init__.py
--rw-r--r--   0        0        0     2655 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/contacts/add_contact.py
--rw-r--r--   0        0        0     2527 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/contacts/delete_contacts.py
--rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/contacts/get_contacts.py
--rw-r--r--   0        0        0     1430 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/contacts/get_contacts_count.py
--rw-r--r--   0        0        0     1896 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/contacts/import_contacts.py
--rw-r--r--   0        0        0     2021 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/decorators/__init__.py
--rw-r--r--   0        0        0     2352 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/decorators/on_callback_query.py
--rw-r--r--   0        0        0     2342 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/decorators/on_chat_join_request.py
--rw-r--r--   0        0        0     2365 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/decorators/on_chat_member_updated.py
--rw-r--r--   0        0        0     2393 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/decorators/on_chosen_inline_result.py
--rw-r--r--   0        0        0     2357 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/decorators/on_deleted_messages.py
--rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/decorators/on_disconnect.py
--rw-r--r--   0        0        0     2349 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/decorators/on_edited_message.py
--rw-r--r--   0        0        0     2336 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/decorators/on_inline_query.py
--rw-r--r--   0        0        0     2271 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/decorators/on_message.py
--rw-r--r--   0        0        0     2400 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/decorators/on_message_reaction_count_updated.py
--rw-r--r--   0        0        0     2310 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/decorators/on_message_reaction_updated.py
--rw-r--r--   0        0        0     2250 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/decorators/on_poll.py
--rw-r--r--   0        0        0     1806 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/decorators/on_raw_update.py
--rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/decorators/on_story.py
--rw-r--r--   0        0        0     2324 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/decorators/on_user_status.py
--rw-r--r--   0        0        0     2436 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/invite_links/__init__.py
--rw-r--r--   0        0        0     1932 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/invite_links/approve_all_chat_join_requests.py
--rw-r--r--   0        0        0     2098 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/invite_links/approve_chat_join_request.py
--rw-r--r--   0        0        0     3457 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/invite_links/create_chat_invite_link.py
--rw-r--r--   0        0        0     1933 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/invite_links/decline_all_chat_join_requests.py
--rw-r--r--   0        0        0     2099 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/invite_links/decline_chat_join_request.py
--rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/invite_links/delete_chat_admin_invite_links.py
--rw-r--r--   0        0        0     1837 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/invite_links/delete_chat_invite_link.py
--rw-r--r--   0        0        0     3621 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/invite_links/edit_chat_invite_link.py
--rw-r--r--   0        0        0     2652 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/invite_links/export_chat_invite_link.py
--rw-r--r--   0        0        0     3740 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/invite_links/get_chat_admin_invite_links.py
--rw-r--r--   0        0        0     2509 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/invite_links/get_chat_admin_invite_links_count.py
--rw-r--r--   0        0        0     2083 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/invite_links/get_chat_admins_with_invite_links.py
--rw-r--r--   0        0        0     1995 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/invite_links/get_chat_invite_link.py
--rw-r--r--   0        0        0     3016 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/invite_links/get_chat_invite_link_joiners.py
--rw-r--r--   0        0        0     2000 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/invite_links/get_chat_invite_link_joiners_count.py
--rw-r--r--   0        0        0     3035 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/invite_links/get_chat_join_requests.py
--rw-r--r--   0        0        0     2383 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/invite_links/revoke_chat_invite_link.py
--rw-r--r--   0        0        0     4116 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/messages/__init__.py
--rw-r--r--   0        0        0     7610 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/messages/copy_media_group.py
--rw-r--r--   0        0        0     6018 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/messages/copy_message.py
--rw-r--r--   0        0        0     3143 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/messages/delete_messages.py
--rw-r--r--   0        0        0     7839 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/messages/download_media.py
--rw-r--r--   0        0        0     2273 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/messages/edit_inline_caption.py
--rw-r--r--   0        0        0    10655 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/messages/edit_inline_media.py
--rw-r--r--   0        0        0     2466 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/messages/edit_inline_reply_markup.py
--rw-r--r--   0        0        0     3118 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/messages/edit_inline_text.py
--rw-r--r--   0        0        0     3066 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/messages/edit_message_caption.py
--rw-r--r--   0        0        0    13153 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/messages/edit_message_media.py
--rw-r--r--   0        0        0     3113 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/messages/edit_message_reply_markup.py
--rw-r--r--   0        0        0     4045 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/messages/edit_message_text.py
--rw-r--r--   0        0        0     5568 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/messages/forward_messages.py
--rw-r--r--   0        0        0     4737 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/messages/get_chat_history.py
--rw-r--r--   0        0        0     2468 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/messages/get_chat_history_count.py
--rw-r--r--   0        0        0     2058 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/messages/get_custom_emoji_stickers.py
--rw-r--r--   0        0        0     2299 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/messages/get_discussion_message.py
--rw-r--r--   0        0        0     2895 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/messages/get_discussion_replies.py
--rw-r--r--   0        0        0     2037 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/messages/get_discussion_replies_count.py
--rw-r--r--   0        0        0     3057 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/messages/get_media_group.py
--rw-r--r--   0        0        0     6735 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/messages/get_messages.py
--rw-r--r--   0        0        0     2177 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/messages/get_scheduled_messages.py
--rw-r--r--   0        0        0     2079 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/messages/get_stickers.py
--rw-r--r--   0        0        0     2138 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/messages/inline_session.py
--rw-r--r--   0        0        0     2505 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/messages/read_chat_history.py
--rw-r--r--   0        0        0     2162 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/messages/retract_vote.py
--rw-r--r--   0        0        0     4151 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/messages/search_global.py
--rw-r--r--   0        0        0     2157 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/messages/search_global_count.py
--rw-r--r--   0        0        0     5378 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/messages/search_messages.py
--rw-r--r--   0        0        0     3213 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/messages/search_messages_count.py
--rw-r--r--   0        0        0    14974 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/messages/send_animation.py
--rw-r--r--   0        0        0    13598 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/messages/send_audio.py
--rw-r--r--   0        0        0     7695 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/messages/send_cached_media.py
--rw-r--r--   0        0        0     3309 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/messages/send_chat_action.py
--rw-r--r--   0        0        0     6863 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/messages/send_contact.py
--rw-r--r--   0        0        0     7023 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/messages/send_dice.py
--rw-r--r--   0        0        0    12824 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/messages/send_document.py
--rw-r--r--   0        0        0     6501 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/messages/send_location.py
--rw-r--r--   0        0        0    24429 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/messages/send_media_group.py
--rw-r--r--   0        0        0     9372 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/messages/send_message.py
--rw-r--r--   0        0        0    11662 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/messages/send_photo.py
--rw-r--r--   0        0        0    10180 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/messages/send_poll.py
--rw-r--r--   0        0        0     5258 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/messages/send_reaction.py
--rw-r--r--   0        0        0    10894 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/messages/send_sticker.py
--rw-r--r--   0        0        0     7323 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/messages/send_venue.py
--rw-r--r--   0        0        0    14360 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/messages/send_video.py
--rw-r--r--   0        0        0    12209 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/messages/send_video_note.py
--rw-r--r--   0        0        0    11864 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/messages/send_voice.py
--rw-r--r--   0        0        0     8273 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/messages/send_web_page.py
--rw-r--r--   0        0        0     2855 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/messages/stop_poll.py
--rw-r--r--   0        0        0     4068 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/messages/stream_media.py
--rw-r--r--   0        0        0     2612 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/messages/vote_poll.py
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/password/__init__.py
--rw-r--r--   0        0        0     2759 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/password/change_cloud_password.py
--rw-r--r--   0        0        0     2984 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/password/enable_cloud_password.py
--rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/password/remove_cloud_password.py
--rw-r--r--   0        0        0     1976 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/pyromod/__init__.py
--rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/pyromod/ask.py
--rw-r--r--   0        0        0     2193 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/pyromod/get_listener_matching_with_data.py
--rw-r--r--   0        0        0     2576 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/pyromod/get_listener_matching_with_identifier_pattern.py
--rw-r--r--   0        0        0     1955 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/pyromod/get_many_listeners_matching_with_data.py
--rw-r--r--   0        0        0     2337 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/pyromod/get_many_listeners_matching_with_identifier_pattern.py
--rw-r--r--   0        0        0     4617 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/pyromod/listen.py
--rw-r--r--   0        0        0     3405 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/pyromod/register_next_step_handler.py
--rw-r--r--   0        0        0     1503 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/pyromod/remove_listerner.py
--rw-r--r--   0        0        0     2155 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/pyromod/stop_listener.py
--rw-r--r--   0        0        0     2844 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/pyromod/stop_listening.py
--rw-r--r--   0        0        0     2999 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/pyromod/wait_for_callback_query.py
--rw-r--r--   0        0        0     2926 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/pyromod/wait_for_message.py
--rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/stickers/__init__.py
--rw-r--r--   0        0        0     2842 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/stickers/add_sticker_to_set.py
--rw-r--r--   0        0        0     4266 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/stickers/create_sticker_set.py
--rw-r--r--   0        0        0     1836 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/stickers/get_sticker_set.py
--rw-r--r--   0        0        0     2267 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/users/__init__.py
--rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/users/block_user.py
--rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/users/check_username.py
--rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/users/delete_profile_photos.py
--rw-r--r--   0        0        0     2558 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/users/delete_stories.py
--rw-r--r--   0        0        0    10449 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/users/edit_story.py
--rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/users/export_story_link.py
--rw-r--r--   0        0        0     4853 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/users/forward_story.py
--rw-r--r--   0        0        0     1961 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/users/get_all_stories.py
--rw-r--r--   0        0        0     4508 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/users/get_chat_photos.py
--rw-r--r--   0        0        0     2540 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/users/get_chat_photos_count.py
--rw-r--r--   0        0        0     2438 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/users/get_common_chats.py
--rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/users/get_default_emoji_statuses.py
--rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/users/get_me.py
--rw-r--r--   0        0        0     2507 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/users/get_peer_stories.py
--rw-r--r--   0        0        0     3123 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/users/get_stories.py
--rw-r--r--   0        0        0     2681 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/users/get_stories_history.py
--rw-r--r--   0        0        0     2589 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/users/get_users.py
--rw-r--r--   0        0        0    11088 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/users/send_story.py
--rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/users/set_emoji_status.py
--rw-r--r--   0        0        0     2699 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/users/set_profile_photo.py
--rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/users/set_username.py
--rw-r--r--   0        0        0     1808 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/users/unblock_user.py
--rw-r--r--   0        0        0     2347 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/users/update_profile.py
--rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/utilities/__init__.py
--rw-r--r--   0        0        0     2316 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/utilities/add_handler.py
--rw-r--r--   0        0        0     2222 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/utilities/compose.py
--rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/utilities/export_session_string.py
--rw-r--r--   0        0        0     2754 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/utilities/idle.py
--rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/utilities/remove_handler.py
--rw-r--r--   0        0        0     2272 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/utilities/restart.py
--rw-r--r--   0        0        0     2835 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/utilities/run.py
--rwxr-xr-x   0        0        0     1592 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/utilities/run_sync.py
--rw-r--r--   0        0        0     2388 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/utilities/start.py
--rw-r--r--   0        0        0     2095 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/utilities/stop.py
--rw-r--r--   0        0        0     1869 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/methods/utilities/stop_transmission.py
--rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/nav/__init__.py
--rw-r--r--   0        0        0     3663 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/nav/pagination.py
--rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/parser/__init__.py
--rw-r--r--   0        0        0     8840 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/parser/html.py
--rw-r--r--   0        0        0     8216 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/parser/markdown.py
--rw-r--r--   0        0        0     2082 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/parser/parser.py
--rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/parser/utils.py
--rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/raw/__init__.py
--rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/raw/core/__init__.py
--rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/raw/core/future_salt.py
--rw-r--r--   0        0        0     1891 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/raw/core/future_salts.py
--rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/raw/core/gzip_packed.py
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/raw/core/list.py
--rw-r--r--   0        0        0     1851 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/raw/core/message.py
--rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/raw/core/msg_container.py
--rw-r--r--   0        0        0     2519 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/raw/core/tl_object.py
--rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/raw/core/primitives/__init__.py
--rw-r--r--   0        0        0     1497 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/raw/core/primitives/bool.py
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/raw/core/primitives/bytes.py
--rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/raw/core/primitives/double.py
--rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/raw/core/primitives/int.py
--rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/raw/core/primitives/string.py
--rw-r--r--   0        0        0     2207 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/raw/core/primitives/vector.py
--rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/session/__init__.py
--rw-r--r--   0        0        0    12124 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/session/auth.py
--rw-r--r--   0        0        0    15248 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/session/session.py
--rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/session/internals/__init__.py
--rw-r--r--   0        0        0     2629 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/session/internals/data_center.py
--rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/session/internals/msg_factory.py
--rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/session/internals/msg_id.py
--rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/session/internals/seq_no.py
--rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/storage/__init__.py
--rw-r--r--   0        0        0     1340 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/storage/dummy_client.py
--rw-r--r--   0        0        0     2062 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/storage/file_storage.py
--rw-r--r--   0        0        0     2965 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/storage/memory_storage.py
--rw-r--r--   0        0        0     7282 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/storage/mongo_storage.py
--rw-r--r--   0        0        0     7958 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/storage/sqlite_storage.py
--rw-r--r--   0        0        0     5888 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/storage/storage.py
--rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/__init__.py
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/list.py
--rw-r--r--   0        0        0     3923 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/object.py
--rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/update.py
--rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/authorization/__init__.py
--rw-r--r--   0        0        0     2362 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/authorization/sent_code.py
--rw-r--r--   0        0        0     2007 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/authorization/terms_of_service.py
--rw-r--r--   0        0        0     3209 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/bots_and_keyboards/__init__.py
--rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/bots_and_keyboards/bot_command.py
--rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/bots_and_keyboards/bot_command_scope.py
--rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/bots_and_keyboards/bot_command_scope_all_chat_administrators.py
--rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/bots_and_keyboards/bot_command_scope_all_group_chats.py
--rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/bots_and_keyboards/bot_command_scope_all_private_chats.py
--rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/bots_and_keyboards/bot_command_scope_chat.py
--rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_administrators.py
--rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_member.py
--rw-r--r--   0        0        0     1308 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/bots_and_keyboards/bot_command_scope_default.py
--rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/bots_and_keyboards/bot_info.py
--rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/bots_and_keyboards/callback_game.py
--rw-r--r--   0        0        0    12925 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/bots_and_keyboards/callback_query.py
--rw-r--r--   0        0        0     2320 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/bots_and_keyboards/force_reply.py
--rw-r--r--   0        0        0     2263 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/bots_and_keyboards/game_high_score.py
--rw-r--r--   0        0        0     7625 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/bots_and_keyboards/inline_keyboard_button.py
--rw-r--r--   0        0        0     2438 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/bots_and_keyboards/inline_keyboard_markup.py
--rw-r--r--   0        0        0     7088 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/bots_and_keyboards/keyboard_button.py
--rw-r--r--   0        0        0     3676 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/bots_and_keyboards/login_url.py
--rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/bots_and_keyboards/menu_button.py
--rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/bots_and_keyboards/menu_button_commands.py
--rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/bots_and_keyboards/menu_button_default.py
--rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/bots_and_keyboards/menu_button_web_app.py
--rw-r--r--   0        0        0     4736 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/bots_and_keyboards/reply_keyboard_markup.py
--rw-r--r--   0        0        0     2273 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/bots_and_keyboards/reply_keyboard_remove.py
--rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/bots_and_keyboards/request_peer_type_channel.py
--rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/bots_and_keyboards/request_peer_type_chat.py
--rw-r--r--   0        0        0     1421 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/bots_and_keyboards/request_peer_type_user.py
--rw-r--r--   0        0        0     2297 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/bots_and_keyboards/requested_chats.py
--rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/bots_and_keyboards/sent_web_app_message.py
--rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/bots_and_keyboards/web_app_info.py
--rw-r--r--   0        0        0     2812 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/inline_mode/__init__.py
--rw-r--r--   0        0        0     3859 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/inline_mode/chosen_inline_result.py
--rw-r--r--   0        0        0     7397 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/inline_mode/inline_query.py
--rw-r--r--   0        0        0     2412 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/inline_mode/inline_query_result.py
--rw-r--r--   0        0        0     6059 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/inline_mode/inline_query_result_animation.py
--rw-r--r--   0        0        0     3413 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/inline_mode/inline_query_result_article.py
--rw-r--r--   0        0        0     5193 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/inline_mode/inline_query_result_audio.py
--rw-r--r--   0        0        0     4374 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/inline_mode/inline_query_result_cached_animation.py
--rw-r--r--   0        0        0     4158 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/inline_mode/inline_query_result_cached_audio.py
--rw-r--r--   0        0        0     4517 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/inline_mode/inline_query_result_cached_document.py
--rw-r--r--   0        0        0     4441 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/inline_mode/inline_query_result_cached_photo.py
--rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/inline_mode/inline_query_result_cached_sticker.py
--rw-r--r--   0        0        0     4523 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/inline_mode/inline_query_result_cached_video.py
--rw-r--r--   0        0        0     4331 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/inline_mode/inline_query_result_cached_voice.py
--rw-r--r--   0        0        0     4287 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/inline_mode/inline_query_result_contact.py
--rw-r--r--   0        0        0     5398 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/inline_mode/inline_query_result_document.py
--rw-r--r--   0        0        0     4694 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/inline_mode/inline_query_result_location.py
--rw-r--r--   0        0        0     5323 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/inline_mode/inline_query_result_photo.py
--rw-r--r--   0        0        0     4941 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/inline_mode/inline_query_result_venue.py
--rw-r--r--   0        0        0     5615 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/inline_mode/inline_query_result_video.py
--rw-r--r--   0        0        0     4452 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/inline_mode/inline_query_result_voice.py
--rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/input_media/__init__.py
--rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/input_media/input_media.py
--rw-r--r--   0        0        0     3429 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/input_media/input_media_animation.py
--rw-r--r--   0        0        0     1329 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/input_media/input_media_area.py
--rw-r--r--   0        0        0     1973 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/input_media/input_media_area_channel_post.py
--rw-r--r--   0        0        0     3283 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/input_media/input_media_audio.py
--rw-r--r--   0        0        0     2772 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/input_media/input_media_document.py
--rw-r--r--   0        0        0     2686 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/input_media/input_media_photo.py
--rw-r--r--   0        0        0     3652 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/input_media/input_media_video.py
--rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/input_media/input_phone_contact.py
--rw-r--r--   0        0        0     1316 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/input_message_content/__init__.py
--rw-r--r--   0        0        0     1413 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/input_message_content/input_message_content.py
--rw-r--r--   0        0        0     3248 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/input_message_content/input_reply_to_message.py
--rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/input_message_content/input_reply_to_story.py
--rw-r--r--   0        0        0     2670 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/input_message_content/input_text_message_content.py
--rw-r--r--   0        0        0     3528 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/messages_and_media/__init__.py
--rw-r--r--   0        0        0     4032 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/messages_and_media/animation.py
--rw-r--r--   0        0        0     4057 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/messages_and_media/audio.py
--rw-r--r--   0        0        0     2223 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/messages_and_media/contact.py
--rw-r--r--   0        0        0     1541 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/messages_and_media/dice.py
--rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/messages_and_media/document.py
--rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/messages_and_media/exported_story_link.py
--rw-r--r--   0        0        0     3042 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/messages_and_media/game.py
--rw-r--r--   0        0        0     2319 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/messages_and_media/gift_code.py
--rw-r--r--   0        0        0     3842 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/messages_and_media/giveaway.py
--rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/messages_and_media/giveaway_launched.py
--rw-r--r--   0        0        0     4895 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/messages_and_media/giveaway_result.py
--rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/messages_and_media/location.py
--rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/messages_and_media/media_area.py
--rw-r--r--   0        0        0     2354 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/messages_and_media/media_area_channel_post.py
--rw-r--r--   0        0        0     2614 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/messages_and_media/media_area_coordinates.py
--rw-r--r--   0        0        0   202766 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/messages_and_media/message.py
--rw-r--r--   0        0        0     4364 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/messages_and_media/message_entity.py
--rw-r--r--   0        0        0     2928 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/messages_and_media/message_reaction_count_updated.py
--rw-r--r--   0        0        0     4255 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/messages_and_media/message_reaction_updated.py
--rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/messages_and_media/message_reactions.py
--rw-r--r--   0        0        0     2889 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/messages_and_media/message_story.py
--rw-r--r--   0        0        0     4233 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/messages_and_media/photo.py
--rw-r--r--   0        0        0     8233 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/messages_and_media/poll.py
--rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/messages_and_media/poll_option.py
--rw-r--r--   0        0        0     2641 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/messages_and_media/reaction.py
--rw-r--r--   0        0        0     1937 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/messages_and_media/reaction_count.py
--rw-r--r--   0        0        0     2400 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/messages_and_media/reaction_type.py
--rw-r--r--   0        0        0     7010 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/messages_and_media/sticker.py
--rw-r--r--   0        0        0     2879 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/messages_and_media/stickerset.py
--rw-r--r--   0        0        0     1927 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/messages_and_media/stories_privacy_rules.py
--rw-r--r--   0        0        0    76095 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/messages_and_media/story.py
--rw-r--r--   0        0        0     2520 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/messages_and_media/story_deleted.py
--rw-r--r--   0        0        0     3044 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/messages_and_media/story_forward_header.py
--rw-r--r--   0        0        0     3291 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/messages_and_media/story_skipped.py
--rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/messages_and_media/story_views.py
--rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/messages_and_media/stripped_thumbnail.py
--rw-r--r--   0        0        0     3773 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/messages_and_media/thumbnail.py
--rw-r--r--   0        0        0     2293 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/messages_and_media/venue.py
--rw-r--r--   0        0        0     4377 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/messages_and_media/video.py
--rw-r--r--   0        0        0     3829 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/messages_and_media/video_note.py
--rw-r--r--   0        0        0     3462 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/messages_and_media/voice.py
--rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/messages_and_media/web_app_data.py
--rw-r--r--   0        0        0     6424 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/messages_and_media/web_page.py
--rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/messages_and_media/web_page_empty.py
--rw-r--r--   0        0        0     2665 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/messages_and_media/web_page_preview.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/pyromod/__init__.py
--rw-r--r--   0        0        0     3385 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/pyromod/identifier.py
--rw-r--r--   0        0        0     2911 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/pyromod/listener.py
--rw-r--r--   0        0        0     3631 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/user_and_chats/__init__.py
--rw-r--r--   0        0        0     3066 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/user_and_chats/business_info.py
--rw-r--r--   0        0        0     4565 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/user_and_chats/business_message.py
--rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/user_and_chats/business_recipients.py
--rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/user_and_chats/business_weekly_open.py
--rw-r--r--   0        0        0     2044 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/user_and_chats/business_working_hours.py
--rw-r--r--   0        0        0    42910 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/user_and_chats/chat.py
--rw-r--r--   0        0        0     2247 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/user_and_chats/chat_admin_with_invite_links.py
--rw-r--r--   0        0        0     2402 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/user_and_chats/chat_color.py
--rw-r--r--   0        0        0    22799 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/user_and_chats/chat_event.py
--rw-r--r--   0        0        0     5524 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/user_and_chats/chat_event_filter.py
--rw-r--r--   0        0        0     4590 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/user_and_chats/chat_invite_link.py
--rw-r--r--   0        0        0     4120 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/user_and_chats/chat_join_request.py
--rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/user_and_chats/chat_joined_by_request.py
--rw-r--r--   0        0        0     2565 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/user_and_chats/chat_joiner.py
--rw-r--r--   0        0        0     9490 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/user_and_chats/chat_member.py
--rw-r--r--   0        0        0     3758 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/user_and_chats/chat_member_updated.py
--rw-r--r--   0        0        0    10248 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/user_and_chats/chat_permissions.py
--rw-r--r--   0        0        0     3986 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/user_and_chats/chat_photo.py
--rw-r--r--   0        0        0     2662 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/user_and_chats/chat_preview.py
--rw-r--r--   0        0        0     6413 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/user_and_chats/chat_privileges.py
--rw-r--r--   0        0        0     2491 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/user_and_chats/chat_reactions.py
--rw-r--r--   0        0        0     2684 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/user_and_chats/dialog.py
--rw-r--r--   0        0        0     2357 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/user_and_chats/emoji_status.py
--rw-r--r--   0        0        0     5071 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/user_and_chats/forum_topic.py
--rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/user_and_chats/forum_topic_closed.py
--rw-r--r--   0        0        0     2045 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/user_and_chats/forum_topic_created.py
--rw-r--r--   0        0        0     1919 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/user_and_chats/forum_topic_edited.py
--rw-r--r--   0        0        0     1126 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/user_and_chats/forum_topic_reopened.py
--rw-r--r--   0        0        0     1126 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/user_and_chats/general_forum_topic_hidden.py
--rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/user_and_chats/general_forum_topic_unhidden.py
--rw-r--r--   0        0        0     1922 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/user_and_chats/invite_link_importer.py
--rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/user_and_chats/peer_channel.py
--rw-r--r--   0        0        0     1328 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/user_and_chats/peer_user.py
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/user_and_chats/restriction.py
--rw-r--r--   0        0        0    17664 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/user_and_chats/user.py
--rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/user_and_chats/username.py
--rw-r--r--   0        0        0     1324 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/user_and_chats/video_chat_ended.py
--rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/user_and_chats/video_chat_members_invited.py
--rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/user_and_chats/video_chat_scheduled.py
--rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyrogram/types/user_and_chats/video_chat_started.py
--rw-r--r--   0        0        0     1580 2020-02-02 00:00:00.000000 pyroblack-2.3.52/.gitignore
--rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 pyroblack-2.3.52/COPYING
--rw-r--r--   0        0        0     7651 2020-02-02 00:00:00.000000 pyroblack-2.3.52/COPYING.lesser
--rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 pyroblack-2.3.52/NOTICE
--rw-r--r--   0        0        0     2206 2020-02-02 00:00:00.000000 pyroblack-2.3.52/README.md
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 pyroblack-2.3.52/hatch_build.py
--rw-r--r--   0        0        0     2709 2020-02-02 00:00:00.000000 pyroblack-2.3.52/pyproject.toml
--rw-r--r--   0        0        0     4839 2020-02-02 00:00:00.000000 pyroblack-2.3.52/PKG-INFO
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 pyroblack-2.3.60/MANIFEST.in
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 pyroblack-2.3.60/Makefile
+-rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 pyroblack-2.3.60/build-docs.sh
+-rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 pyroblack-2.3.60/compiler/__init__.py
+-rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 pyroblack-2.3.60/compiler/api/__init__.py
+-rw-r--r--   0        0        0    23145 2020-02-02 00:00:00.000000 pyroblack-2.3.60/compiler/api/compiler.py
+-rw-r--r--   0        0        0     2233 2020-02-02 00:00:00.000000 pyroblack-2.3.60/compiler/api/source/auth_key.tl
+-rw-r--r--   0        0        0   198353 2020-02-02 00:00:00.000000 pyroblack-2.3.60/compiler/api/source/main_api.tl
+-rw-r--r--   0        0        0     3425 2020-02-02 00:00:00.000000 pyroblack-2.3.60/compiler/api/source/sys_msgs.tl
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 pyroblack-2.3.60/compiler/api/template/combinator.txt
+-rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 pyroblack-2.3.60/compiler/api/template/type.txt
+-rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 pyroblack-2.3.60/compiler/errors/__init__.py
+-rw-r--r--   0        0        0     5446 2020-02-02 00:00:00.000000 pyroblack-2.3.60/compiler/errors/compiler.py
+-rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 pyroblack-2.3.60/compiler/errors/sort.py
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 pyroblack-2.3.60/compiler/errors/source/303_SEE_OTHER.tsv
+-rw-r--r--   0        0        0    23909 2020-02-02 00:00:00.000000 pyroblack-2.3.60/compiler/errors/source/400_BAD_REQUEST.tsv
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 pyroblack-2.3.60/compiler/errors/source/401_UNAUTHORIZED.tsv
+-rw-r--r--   0        0        0     2807 2020-02-02 00:00:00.000000 pyroblack-2.3.60/compiler/errors/source/403_FORBIDDEN.tsv
+-rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 pyroblack-2.3.60/compiler/errors/source/406_NOT_ACCEPTABLE.tsv
+-rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 pyroblack-2.3.60/compiler/errors/source/420_FLOOD.tsv
+-rw-r--r--   0        0        0     4323 2020-02-02 00:00:00.000000 pyroblack-2.3.60/compiler/errors/source/500_INTERNAL_SERVER_ERROR.tsv
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 pyroblack-2.3.60/compiler/errors/source/503_SERVICE_UNAVAILABLE.tsv
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 pyroblack-2.3.60/compiler/errors/template/class.txt
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 pyroblack-2.3.60/compiler/errors/template/sub_class.txt
+-rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/__init__.py
+-rw-r--r--   0        0        0    48369 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/client.py
+-rw-r--r--   0        0        0    12082 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/dispatcher.py
+-rw-r--r--   0        0        0   209155 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/emoji.py
+-rw-r--r--   0        0        0    15602 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/file_id.py
+-rw-r--r--   0        0        0    27713 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/filters.py
+-rw-r--r--   0        0        0    61915 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/mime_types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/py.typed
+-rw-r--r--   0        0        0     3944 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/sync.py
+-rw-r--r--   0        0        0    16394 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/utils.py
+-rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/connection/__init__.py
+-rw-r--r--   0        0        0     2828 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/connection/connection.py
+-rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/connection/transport/__init__.py
+-rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/connection/transport/tcp/__init__.py
+-rw-r--r--   0        0        0     4115 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/connection/transport/tcp/tcp.py
+-rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/connection/transport/tcp/tcp_abridged.py
+-rw-r--r--   0        0        0     2960 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/connection/transport/tcp/tcp_abridged_o.py
+-rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/connection/transport/tcp/tcp_full.py
+-rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/connection/transport/tcp/tcp_intermediate.py
+-rw-r--r--   0        0        0     2471 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/connection/transport/tcp/tcp_intermediate_o.py
+-rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/crypto/__init__.py
+-rw-r--r--   0        0        0     4073 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/crypto/aes.py
+-rw-r--r--   0        0        0     4118 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/crypto/mtproto.py
+-rw-r--r--   0        0        0     2448 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/crypto/prime.py
+-rw-r--r--   0        0        0    13485 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/crypto/rsa.py
+-rw-r--r--   0        0        0     2176 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/enums/__init__.py
+-rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/enums/auto_name.py
+-rw-r--r--   0        0        0     1261 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/enums/business_schedule.py
+-rw-r--r--   0        0        0     2307 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/enums/chat_action.py
+-rw-r--r--   0        0        0     4665 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/enums/chat_event_action.py
+-rw-r--r--   0        0        0     1265 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/enums/chat_member_status.py
+-rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/enums/chat_members_filter.py
+-rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/enums/chat_type.py
+-rw-r--r--   0        0        0     1211 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/enums/listerner_types.py
+-rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/enums/message_entity_type.py
+-rw-r--r--   0        0        0     1765 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/enums/message_media_type.py
+-rw-r--r--   0        0        0     3008 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/enums/message_service_type.py
+-rw-r--r--   0        0        0     2406 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/enums/messages_filter.py
+-rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/enums/next_code_type.py
+-rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/enums/parse_mode.py
+-rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/enums/poll_type.py
+-rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/enums/profile_color.py
+-rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/enums/reaction_type.py
+-rw-r--r--   0        0        0     2541 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/enums/reply_color.py
+-rw-r--r--   0        0        0     2000 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/enums/sent_code_type.py
+-rw-r--r--   0        0        0     1378 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/enums/stories_privacy_rules.py
+-rw-r--r--   0        0        0     1316 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/enums/story_privacy.py
+-rw-r--r--   0        0        0     1299 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/enums/user_status.py
+-rw-r--r--   0        0        0     2669 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/errors/__init__.py
+-rw-r--r--   0        0        0     3539 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/errors/rpc_error.py
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/errors/pyromod/__init__.py
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/errors/pyromod/listener_stopped.py
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/errors/pyromod/listener_timeout.py
+-rw-r--r--   0        0        0     1877 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/handlers/__init__.py
+-rw-r--r--   0        0        0     7884 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/handlers/callback_query_handler.py
+-rw-r--r--   0        0        0     2011 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/handlers/chat_join_request_handler.py
+-rw-r--r--   0        0        0     2046 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/handlers/chat_member_updated_handler.py
+-rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/handlers/chosen_inline_result_handler.py
+-rw-r--r--   0        0        0     2527 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/handlers/conversation_handler.py
+-rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/handlers/deleted_messages_handler.py
+-rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/handlers/disconnect_handler.py
+-rw-r--r--   0        0        0     1979 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/handlers/edited_message_handler.py
+-rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/handlers/handler.py
+-rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/handlers/inline_query_handler.py
+-rw-r--r--   0        0        0     6078 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/handlers/message_handler.py
+-rw-r--r--   0        0        0     2143 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/handlers/message_reaction_count_updated_handler.py
+-rw-r--r--   0        0        0     2089 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/handlers/message_reaction_updated_handler.py
+-rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/handlers/poll_handler.py
+-rw-r--r--   0        0        0     2942 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/handlers/raw_update_handler.py
+-rw-r--r--   0        0        0     1996 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/handlers/story_handler.py
+-rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/handlers/user_status_handler.py
+-rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/helpers/__init__.py
+-rw-r--r--   0        0        0     3480 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/helpers/helpers.py
+-rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/__init__.py
+-rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/advanced/__init__.py
+-rw-r--r--   0        0        0     3163 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/advanced/invoke.py
+-rw-r--r--   0        0        0     4304 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/advanced/resolve_peer.py
+-rw-r--r--   0        0        0     8592 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/advanced/save_file.py
+-rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/auth/__init__.py
+-rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/auth/accept_terms_of_service.py
+-rw-r--r--   0        0        0     1900 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/auth/check_password.py
+-rw-r--r--   0        0        0     1774 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/auth/connect.py
+-rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/auth/disconnect.py
+-rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/auth/get_password_hint.py
+-rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/auth/initialize.py
+-rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/auth/log_out.py
+-rw-r--r--   0        0        0     1771 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/auth/recover_password.py
+-rw-r--r--   0        0        0     2118 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/auth/resend_code.py
+-rw-r--r--   0        0        0     5099 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/auth/send_code.py
+-rw-r--r--   0        0        0     1473 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/auth/send_recovery_code.py
+-rw-r--r--   0        0        0     3087 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/auth/sign_in.py
+-rw-r--r--   0        0        0     2719 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/auth/sign_in_bot.py
+-rw-r--r--   0        0        0     2357 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/auth/sign_up.py
+-rw-r--r--   0        0        0     2042 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/auth/terminate.py
+-rw-r--r--   0        0        0     2148 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/bots/__init__.py
+-rw-r--r--   0        0        0     3313 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/bots/answer_callback_query.py
+-rw-r--r--   0        0        0     5060 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/bots/answer_inline_query.py
+-rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/bots/answer_web_app_query.py
+-rw-r--r--   0        0        0     2360 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/bots/delete_bot_commands.py
+-rw-r--r--   0        0        0     2573 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/bots/get_bot_commands.py
+-rw-r--r--   0        0        0     2037 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/bots/get_bot_default_privileges.py
+-rw-r--r--   0        0        0     1887 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/bots/get_bot_info.py
+-rw-r--r--   0        0        0     2364 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/bots/get_chat_menu_button.py
+-rw-r--r--   0        0        0     2909 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/bots/get_game_high_scores.py
+-rw-r--r--   0        0        0     3479 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/bots/get_inline_bot_results.py
+-rw-r--r--   0        0        0     2964 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/bots/request_callback_answer.py
+-rw-r--r--   0        0        0     4645 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/bots/send_game.py
+-rw-r--r--   0        0        0     4394 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/bots/send_inline_bot_result.py
+-rw-r--r--   0        0        0     2710 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/bots/set_bot_commands.py
+-rw-r--r--   0        0        0     3284 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/bots/set_bot_default_privileges.py
+-rw-r--r--   0        0        0     2325 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/bots/set_bot_info.py
+-rw-r--r--   0        0        0     2070 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/bots/set_chat_menu_button.py
+-rw-r--r--   0        0        0     4056 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/bots/set_game_score.py
+-rw-r--r--   0        0        0     4824 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/chats/__init__.py
+-rw-r--r--   0        0        0     3412 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/chats/add_chat_members.py
+-rw-r--r--   0        0        0     2252 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/chats/archive_chats.py
+-rw-r--r--   0        0        0     4871 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/chats/ban_chat_member.py
+-rw-r--r--   0        0        0     1939 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/chats/close_forum_topic.py
+-rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/chats/close_general_topic.py
+-rw-r--r--   0        0        0     1769 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/chats/create_channel.py
+-rw-r--r--   0        0        0     2494 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/chats/create_forum_topic.py
+-rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/chats/create_group.py
+-rw-r--r--   0        0        0     1907 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/chats/create_supergroup.py
+-rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/chats/delete_channel.py
+-rw-r--r--   0        0        0     2345 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/chats/delete_chat_photo.py
+-rw-r--r--   0        0        0     2046 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/chats/delete_forum_topic.py
+-rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/chats/delete_supergroup.py
+-rw-r--r--   0        0        0     2143 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/chats/delete_user_history.py
+-rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/chats/edit_forum_topic.py
+-rw-r--r--   0        0        0     1921 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/chats/edit_general_topic.py
+-rw-r--r--   0        0        0     3378 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/chats/get_chat.py
+-rw-r--r--   0        0        0     4120 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/chats/get_chat_event_log.py
+-rw-r--r--   0        0        0     3399 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/chats/get_chat_member.py
+-rw-r--r--   0        0        0     5305 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/chats/get_chat_members.py
+-rw-r--r--   0        0        0     2206 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/chats/get_chat_members_count.py
+-rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/chats/get_chat_online_count.py
+-rw-r--r--   0        0        0     3574 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/chats/get_dialogs.py
+-rw-r--r--   0        0        0     2203 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/chats/get_dialogs_count.py
+-rw-r--r--   0        0        0     2495 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/chats/get_forum_topics.py
+-rw-r--r--   0        0        0     3314 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/chats/get_forum_topics_by_id.py
+-rw-r--r--   0        0        0     2327 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/chats/get_nearby_chats.py
+-rw-r--r--   0        0        0     2275 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/chats/get_send_as_chats.py
+-rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/chats/hide_general_topic.py
+-rw-r--r--   0        0        0     2669 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/chats/join_chat.py
+-rw-r--r--   0        0        0     2440 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/chats/join_folder.py
+-rw-r--r--   0        0        0     2585 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/chats/leave_chat.py
+-rw-r--r--   0        0        0     2724 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/chats/leave_folder.py
+-rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/chats/mark_chat_unread.py
+-rw-r--r--   0        0        0     3244 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/chats/pin_chat_message.py
+-rw-r--r--   0        0        0     4461 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/chats/promote_chat_member.py
+-rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/chats/reopen_forum_topic.py
+-rw-r--r--   0        0        0     1859 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/chats/reopen_general_topic.py
+-rw-r--r--   0        0        0    10996 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/chats/restrict_chat_member.py
+-rw-r--r--   0        0        0     3313 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/chats/set_administrator_title.py
+-rw-r--r--   0        0        0     2259 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/chats/set_chat_description.py
+-rw-r--r--   0        0        0    10011 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/chats/set_chat_permissions.py
+-rw-r--r--   0        0        0     4629 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/chats/set_chat_photo.py
+-rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/chats/set_chat_protected_content.py
+-rw-r--r--   0        0        0     2526 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/chats/set_chat_title.py
+-rw-r--r--   0        0        0     2342 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/chats/set_chat_username.py
+-rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/chats/set_send_as_chat.py
+-rw-r--r--   0        0        0     2132 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/chats/set_slow_mode.py
+-rw-r--r--   0        0        0     1491 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/chats/toggle_folder_tags.py
+-rw-r--r--   0        0        0     2069 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/chats/toggle_forum_topics.py
+-rw-r--r--   0        0        0     2152 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/chats/toggle_join_to_send.py
+-rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/chats/unarchive_chats.py
+-rw-r--r--   0        0        0     2338 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/chats/unban_chat_member.py
+-rw-r--r--   0        0        0     1849 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/chats/unhide_general_topic.py
+-rw-r--r--   0        0        0     2026 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/chats/unpin_all_chat_messages.py
+-rw-r--r--   0        0        0     2177 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/chats/unpin_chat_message.py
+-rw-r--r--   0        0        0     2758 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/chats/update_color.py
+-rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/contacts/__init__.py
+-rw-r--r--   0        0        0     2655 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/contacts/add_contact.py
+-rw-r--r--   0        0        0     2527 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/contacts/delete_contacts.py
+-rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/contacts/get_contacts.py
+-rw-r--r--   0        0        0     1430 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/contacts/get_contacts_count.py
+-rw-r--r--   0        0        0     1896 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/contacts/import_contacts.py
+-rw-r--r--   0        0        0     2021 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/decorators/__init__.py
+-rw-r--r--   0        0        0     2352 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/decorators/on_callback_query.py
+-rw-r--r--   0        0        0     2342 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/decorators/on_chat_join_request.py
+-rw-r--r--   0        0        0     2365 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/decorators/on_chat_member_updated.py
+-rw-r--r--   0        0        0     2393 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/decorators/on_chosen_inline_result.py
+-rw-r--r--   0        0        0     2357 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/decorators/on_deleted_messages.py
+-rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/decorators/on_disconnect.py
+-rw-r--r--   0        0        0     2349 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/decorators/on_edited_message.py
+-rw-r--r--   0        0        0     2336 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/decorators/on_inline_query.py
+-rw-r--r--   0        0        0     2271 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/decorators/on_message.py
+-rw-r--r--   0        0        0     2400 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/decorators/on_message_reaction_count_updated.py
+-rw-r--r--   0        0        0     2310 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/decorators/on_message_reaction_updated.py
+-rw-r--r--   0        0        0     2250 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/decorators/on_poll.py
+-rw-r--r--   0        0        0     1806 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/decorators/on_raw_update.py
+-rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/decorators/on_story.py
+-rw-r--r--   0        0        0     2324 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/decorators/on_user_status.py
+-rw-r--r--   0        0        0     2436 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/invite_links/__init__.py
+-rw-r--r--   0        0        0     1932 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/invite_links/approve_all_chat_join_requests.py
+-rw-r--r--   0        0        0     2098 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/invite_links/approve_chat_join_request.py
+-rw-r--r--   0        0        0     3457 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/invite_links/create_chat_invite_link.py
+-rw-r--r--   0        0        0     1933 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/invite_links/decline_all_chat_join_requests.py
+-rw-r--r--   0        0        0     2099 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/invite_links/decline_chat_join_request.py
+-rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/invite_links/delete_chat_admin_invite_links.py
+-rw-r--r--   0        0        0     1837 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/invite_links/delete_chat_invite_link.py
+-rw-r--r--   0        0        0     3621 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/invite_links/edit_chat_invite_link.py
+-rw-r--r--   0        0        0     2652 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/invite_links/export_chat_invite_link.py
+-rw-r--r--   0        0        0     3740 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/invite_links/get_chat_admin_invite_links.py
+-rw-r--r--   0        0        0     2509 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/invite_links/get_chat_admin_invite_links_count.py
+-rw-r--r--   0        0        0     2083 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/invite_links/get_chat_admins_with_invite_links.py
+-rw-r--r--   0        0        0     1995 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/invite_links/get_chat_invite_link.py
+-rw-r--r--   0        0        0     3016 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/invite_links/get_chat_invite_link_joiners.py
+-rw-r--r--   0        0        0     2000 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/invite_links/get_chat_invite_link_joiners_count.py
+-rw-r--r--   0        0        0     3035 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/invite_links/get_chat_join_requests.py
+-rw-r--r--   0        0        0     2383 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/invite_links/revoke_chat_invite_link.py
+-rw-r--r--   0        0        0     4116 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/messages/__init__.py
+-rw-r--r--   0        0        0     7610 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/messages/copy_media_group.py
+-rw-r--r--   0        0        0     6018 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/messages/copy_message.py
+-rw-r--r--   0        0        0     3143 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/messages/delete_messages.py
+-rw-r--r--   0        0        0     8038 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/messages/download_media.py
+-rw-r--r--   0        0        0     2273 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/messages/edit_inline_caption.py
+-rw-r--r--   0        0        0    10655 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/messages/edit_inline_media.py
+-rw-r--r--   0        0        0     2466 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/messages/edit_inline_reply_markup.py
+-rw-r--r--   0        0        0     3118 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/messages/edit_inline_text.py
+-rw-r--r--   0        0        0     3066 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/messages/edit_message_caption.py
+-rw-r--r--   0        0        0    13153 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/messages/edit_message_media.py
+-rw-r--r--   0        0        0     3113 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/messages/edit_message_reply_markup.py
+-rw-r--r--   0        0        0     4045 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/messages/edit_message_text.py
+-rw-r--r--   0        0        0     5568 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/messages/forward_messages.py
+-rw-r--r--   0        0        0     4737 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/messages/get_chat_history.py
+-rw-r--r--   0        0        0     2468 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/messages/get_chat_history_count.py
+-rw-r--r--   0        0        0     2058 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/messages/get_custom_emoji_stickers.py
+-rw-r--r--   0        0        0     2299 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/messages/get_discussion_message.py
+-rw-r--r--   0        0        0     2895 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/messages/get_discussion_replies.py
+-rw-r--r--   0        0        0     2037 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/messages/get_discussion_replies_count.py
+-rw-r--r--   0        0        0     3057 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/messages/get_media_group.py
+-rw-r--r--   0        0        0     6735 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/messages/get_messages.py
+-rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/messages/get_scheduled_messages.py
+-rw-r--r--   0        0        0     2079 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/messages/get_stickers.py
+-rw-r--r--   0        0        0     2138 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/messages/inline_session.py
+-rw-r--r--   0        0        0     2505 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/messages/read_chat_history.py
+-rw-r--r--   0        0        0     2162 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/messages/retract_vote.py
+-rw-r--r--   0        0        0     4151 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/messages/search_global.py
+-rw-r--r--   0        0        0     2157 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/messages/search_global_count.py
+-rw-r--r--   0        0        0     5378 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/messages/search_messages.py
+-rw-r--r--   0        0        0     3213 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/messages/search_messages_count.py
+-rw-r--r--   0        0        0    14974 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/messages/send_animation.py
+-rw-r--r--   0        0        0    13598 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/messages/send_audio.py
+-rw-r--r--   0        0        0     7695 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/messages/send_cached_media.py
+-rw-r--r--   0        0        0     3309 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/messages/send_chat_action.py
+-rw-r--r--   0        0        0     6863 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/messages/send_contact.py
+-rw-r--r--   0        0        0     7023 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/messages/send_dice.py
+-rw-r--r--   0        0        0    12824 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/messages/send_document.py
+-rw-r--r--   0        0        0     6501 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/messages/send_location.py
+-rw-r--r--   0        0        0    24429 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/messages/send_media_group.py
+-rw-r--r--   0        0        0     9372 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/messages/send_message.py
+-rw-r--r--   0        0        0    11662 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/messages/send_photo.py
+-rw-r--r--   0        0        0    10180 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/messages/send_poll.py
+-rw-r--r--   0        0        0     5258 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/messages/send_reaction.py
+-rw-r--r--   0        0        0    10894 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/messages/send_sticker.py
+-rw-r--r--   0        0        0     7323 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/messages/send_venue.py
+-rw-r--r--   0        0        0    14360 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/messages/send_video.py
+-rw-r--r--   0        0        0    12209 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/messages/send_video_note.py
+-rw-r--r--   0        0        0    11864 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/messages/send_voice.py
+-rw-r--r--   0        0        0     8273 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/messages/send_web_page.py
+-rw-r--r--   0        0        0     2855 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/messages/stop_poll.py
+-rw-r--r--   0        0        0     4068 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/messages/stream_media.py
+-rw-r--r--   0        0        0     2612 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/messages/vote_poll.py
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/password/__init__.py
+-rw-r--r--   0        0        0     2759 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/password/change_cloud_password.py
+-rw-r--r--   0        0        0     2984 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/password/enable_cloud_password.py
+-rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/password/remove_cloud_password.py
+-rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/payments/__init__.py
+-rw-r--r--   0        0        0     2174 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/payments/check_giftcode.py
+-rw-r--r--   0        0        0     1976 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/pyromod/__init__.py
+-rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/pyromod/ask.py
+-rw-r--r--   0        0        0     2193 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/pyromod/get_listener_matching_with_data.py
+-rw-r--r--   0        0        0     2576 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/pyromod/get_listener_matching_with_identifier_pattern.py
+-rw-r--r--   0        0        0     1955 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/pyromod/get_many_listeners_matching_with_data.py
+-rw-r--r--   0        0        0     2337 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/pyromod/get_many_listeners_matching_with_identifier_pattern.py
+-rw-r--r--   0        0        0     4617 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/pyromod/listen.py
+-rw-r--r--   0        0        0     3405 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/pyromod/register_next_step_handler.py
+-rw-r--r--   0        0        0     1503 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/pyromod/remove_listerner.py
+-rw-r--r--   0        0        0     2155 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/pyromod/stop_listener.py
+-rw-r--r--   0        0        0     2844 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/pyromod/stop_listening.py
+-rw-r--r--   0        0        0     2999 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/pyromod/wait_for_callback_query.py
+-rw-r--r--   0        0        0     2926 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/pyromod/wait_for_message.py
+-rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/stickers/__init__.py
+-rw-r--r--   0        0        0     2842 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/stickers/add_sticker_to_set.py
+-rw-r--r--   0        0        0     4266 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/stickers/create_sticker_set.py
+-rw-r--r--   0        0        0     1836 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/stickers/get_sticker_set.py
+-rw-r--r--   0        0        0     2267 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/users/__init__.py
+-rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/users/block_user.py
+-rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/users/check_username.py
+-rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/users/delete_profile_photos.py
+-rw-r--r--   0        0        0     2558 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/users/delete_stories.py
+-rw-r--r--   0        0        0    10449 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/users/edit_story.py
+-rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/users/export_story_link.py
+-rw-r--r--   0        0        0     4853 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/users/forward_story.py
+-rw-r--r--   0        0        0     1961 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/users/get_all_stories.py
+-rw-r--r--   0        0        0     4508 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/users/get_chat_photos.py
+-rw-r--r--   0        0        0     2540 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/users/get_chat_photos_count.py
+-rw-r--r--   0        0        0     2438 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/users/get_common_chats.py
+-rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/users/get_default_emoji_statuses.py
+-rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/users/get_me.py
+-rw-r--r--   0        0        0     2507 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/users/get_peer_stories.py
+-rw-r--r--   0        0        0     3123 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/users/get_stories.py
+-rw-r--r--   0        0        0     2681 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/users/get_stories_history.py
+-rw-r--r--   0        0        0     2589 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/users/get_users.py
+-rw-r--r--   0        0        0    11088 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/users/send_story.py
+-rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/users/set_emoji_status.py
+-rw-r--r--   0        0        0     3229 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/users/set_profile_photo.py
+-rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/users/set_username.py
+-rw-r--r--   0        0        0     1808 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/users/unblock_user.py
+-rw-r--r--   0        0        0     2347 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/users/update_profile.py
+-rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/utilities/__init__.py
+-rw-r--r--   0        0        0     2316 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/utilities/add_handler.py
+-rw-r--r--   0        0        0     2222 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/utilities/compose.py
+-rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/utilities/export_session_string.py
+-rw-r--r--   0        0        0     2754 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/utilities/idle.py
+-rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/utilities/remove_handler.py
+-rw-r--r--   0        0        0     2272 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/utilities/restart.py
+-rw-r--r--   0        0        0     2835 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/utilities/run.py
+-rwxr-xr-x   0        0        0     1592 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/utilities/run_sync.py
+-rw-r--r--   0        0        0     2388 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/utilities/start.py
+-rw-r--r--   0        0        0     2095 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/utilities/stop.py
+-rw-r--r--   0        0        0     1869 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/methods/utilities/stop_transmission.py
+-rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/nav/__init__.py
+-rw-r--r--   0        0        0     3663 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/nav/pagination.py
+-rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/parser/__init__.py
+-rw-r--r--   0        0        0     8840 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/parser/html.py
+-rw-r--r--   0        0        0     8216 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/parser/markdown.py
+-rw-r--r--   0        0        0     2082 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/parser/parser.py
+-rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/parser/utils.py
+-rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/raw/__init__.py
+-rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/raw/core/__init__.py
+-rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/raw/core/future_salt.py
+-rw-r--r--   0        0        0     1891 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/raw/core/future_salts.py
+-rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/raw/core/gzip_packed.py
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/raw/core/list.py
+-rw-r--r--   0        0        0     1851 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/raw/core/message.py
+-rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/raw/core/msg_container.py
+-rw-r--r--   0        0        0     2519 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/raw/core/tl_object.py
+-rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/raw/core/primitives/__init__.py
+-rw-r--r--   0        0        0     1497 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/raw/core/primitives/bool.py
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/raw/core/primitives/bytes.py
+-rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/raw/core/primitives/double.py
+-rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/raw/core/primitives/int.py
+-rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/raw/core/primitives/string.py
+-rw-r--r--   0        0        0     2207 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/raw/core/primitives/vector.py
+-rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/session/__init__.py
+-rw-r--r--   0        0        0    12124 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/session/auth.py
+-rw-r--r--   0        0        0    15248 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/session/session.py
+-rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/session/internals/__init__.py
+-rw-r--r--   0        0        0     2629 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/session/internals/data_center.py
+-rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/session/internals/msg_factory.py
+-rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/session/internals/msg_id.py
+-rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/session/internals/seq_no.py
+-rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/storage/__init__.py
+-rw-r--r--   0        0        0     1340 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/storage/dummy_client.py
+-rw-r--r--   0        0        0     2062 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/storage/file_storage.py
+-rw-r--r--   0        0        0     2965 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/storage/memory_storage.py
+-rw-r--r--   0        0        0     7282 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/storage/mongo_storage.py
+-rw-r--r--   0        0        0     7958 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/storage/sqlite_storage.py
+-rw-r--r--   0        0        0     5888 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/storage/storage.py
+-rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/__init__.py
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/list.py
+-rw-r--r--   0        0        0     3923 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/object.py
+-rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/update.py
+-rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/authorization/__init__.py
+-rw-r--r--   0        0        0     2362 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/authorization/sent_code.py
+-rw-r--r--   0        0        0     2007 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/authorization/terms_of_service.py
+-rw-r--r--   0        0        0     3209 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/bots_and_keyboards/__init__.py
+-rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/bots_and_keyboards/bot_command.py
+-rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/bots_and_keyboards/bot_command_scope.py
+-rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/bots_and_keyboards/bot_command_scope_all_chat_administrators.py
+-rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/bots_and_keyboards/bot_command_scope_all_group_chats.py
+-rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/bots_and_keyboards/bot_command_scope_all_private_chats.py
+-rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/bots_and_keyboards/bot_command_scope_chat.py
+-rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_administrators.py
+-rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_member.py
+-rw-r--r--   0        0        0     1308 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/bots_and_keyboards/bot_command_scope_default.py
+-rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/bots_and_keyboards/bot_info.py
+-rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/bots_and_keyboards/callback_game.py
+-rw-r--r--   0        0        0    12925 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/bots_and_keyboards/callback_query.py
+-rw-r--r--   0        0        0     2320 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/bots_and_keyboards/force_reply.py
+-rw-r--r--   0        0        0     2263 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/bots_and_keyboards/game_high_score.py
+-rw-r--r--   0        0        0     7625 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/bots_and_keyboards/inline_keyboard_button.py
+-rw-r--r--   0        0        0     2438 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/bots_and_keyboards/inline_keyboard_markup.py
+-rw-r--r--   0        0        0     7088 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/bots_and_keyboards/keyboard_button.py
+-rw-r--r--   0        0        0     3676 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/bots_and_keyboards/login_url.py
+-rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/bots_and_keyboards/menu_button.py
+-rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/bots_and_keyboards/menu_button_commands.py
+-rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/bots_and_keyboards/menu_button_default.py
+-rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/bots_and_keyboards/menu_button_web_app.py
+-rw-r--r--   0        0        0     4736 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/bots_and_keyboards/reply_keyboard_markup.py
+-rw-r--r--   0        0        0     2273 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/bots_and_keyboards/reply_keyboard_remove.py
+-rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/bots_and_keyboards/request_peer_type_channel.py
+-rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/bots_and_keyboards/request_peer_type_chat.py
+-rw-r--r--   0        0        0     1421 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/bots_and_keyboards/request_peer_type_user.py
+-rw-r--r--   0        0        0     2297 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/bots_and_keyboards/requested_chats.py
+-rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/bots_and_keyboards/sent_web_app_message.py
+-rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/bots_and_keyboards/web_app_info.py
+-rw-r--r--   0        0        0     2812 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/inline_mode/__init__.py
+-rw-r--r--   0        0        0     3859 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/inline_mode/chosen_inline_result.py
+-rw-r--r--   0        0        0     7397 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/inline_mode/inline_query.py
+-rw-r--r--   0        0        0     2412 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/inline_mode/inline_query_result.py
+-rw-r--r--   0        0        0     6059 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/inline_mode/inline_query_result_animation.py
+-rw-r--r--   0        0        0     3413 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/inline_mode/inline_query_result_article.py
+-rw-r--r--   0        0        0     5193 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/inline_mode/inline_query_result_audio.py
+-rw-r--r--   0        0        0     4374 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/inline_mode/inline_query_result_cached_animation.py
+-rw-r--r--   0        0        0     4158 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/inline_mode/inline_query_result_cached_audio.py
+-rw-r--r--   0        0        0     4517 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/inline_mode/inline_query_result_cached_document.py
+-rw-r--r--   0        0        0     4441 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/inline_mode/inline_query_result_cached_photo.py
+-rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/inline_mode/inline_query_result_cached_sticker.py
+-rw-r--r--   0        0        0     4523 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/inline_mode/inline_query_result_cached_video.py
+-rw-r--r--   0        0        0     4331 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/inline_mode/inline_query_result_cached_voice.py
+-rw-r--r--   0        0        0     4287 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/inline_mode/inline_query_result_contact.py
+-rw-r--r--   0        0        0     5398 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/inline_mode/inline_query_result_document.py
+-rw-r--r--   0        0        0     4694 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/inline_mode/inline_query_result_location.py
+-rw-r--r--   0        0        0     5323 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/inline_mode/inline_query_result_photo.py
+-rw-r--r--   0        0        0     4941 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/inline_mode/inline_query_result_venue.py
+-rw-r--r--   0        0        0     5615 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/inline_mode/inline_query_result_video.py
+-rw-r--r--   0        0        0     4452 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/inline_mode/inline_query_result_voice.py
+-rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/input_media/__init__.py
+-rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/input_media/input_media.py
+-rw-r--r--   0        0        0     3429 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/input_media/input_media_animation.py
+-rw-r--r--   0        0        0     1329 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/input_media/input_media_area.py
+-rw-r--r--   0        0        0     1973 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/input_media/input_media_area_channel_post.py
+-rw-r--r--   0        0        0     3283 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/input_media/input_media_audio.py
+-rw-r--r--   0        0        0     2772 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/input_media/input_media_document.py
+-rw-r--r--   0        0        0     2686 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/input_media/input_media_photo.py
+-rw-r--r--   0        0        0     3652 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/input_media/input_media_video.py
+-rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/input_media/input_phone_contact.py
+-rw-r--r--   0        0        0     1316 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/input_message_content/__init__.py
+-rw-r--r--   0        0        0     1413 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/input_message_content/input_message_content.py
+-rw-r--r--   0        0        0     3248 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/input_message_content/input_reply_to_message.py
+-rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/input_message_content/input_reply_to_story.py
+-rw-r--r--   0        0        0     2670 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/input_message_content/input_text_message_content.py
+-rw-r--r--   0        0        0     3598 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/messages_and_media/__init__.py
+-rw-r--r--   0        0        0     4032 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/messages_and_media/animation.py
+-rw-r--r--   0        0        0     4057 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/messages_and_media/audio.py
+-rw-r--r--   0        0        0     3320 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/messages_and_media/checked_gift_code.py
+-rw-r--r--   0        0        0     2223 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/messages_and_media/contact.py
+-rw-r--r--   0        0        0     1541 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/messages_and_media/dice.py
+-rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/messages_and_media/document.py
+-rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/messages_and_media/exported_story_link.py
+-rw-r--r--   0        0        0     3042 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/messages_and_media/game.py
+-rw-r--r--   0        0        0     2465 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/messages_and_media/gift_code.py
+-rw-r--r--   0        0        0     3842 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/messages_and_media/giveaway.py
+-rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/messages_and_media/giveaway_launched.py
+-rw-r--r--   0        0        0     4895 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/messages_and_media/giveaway_result.py
+-rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/messages_and_media/location.py
+-rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/messages_and_media/media_area.py
+-rw-r--r--   0        0        0     2354 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/messages_and_media/media_area_channel_post.py
+-rw-r--r--   0        0        0     2614 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/messages_and_media/media_area_coordinates.py
+-rw-r--r--   0        0        0   202766 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/messages_and_media/message.py
+-rw-r--r--   0        0        0     4364 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/messages_and_media/message_entity.py
+-rw-r--r--   0        0        0     2928 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/messages_and_media/message_reaction_count_updated.py
+-rw-r--r--   0        0        0     4255 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/messages_and_media/message_reaction_updated.py
+-rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/messages_and_media/message_reactions.py
+-rw-r--r--   0        0        0     2889 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/messages_and_media/message_story.py
+-rw-r--r--   0        0        0     4233 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/messages_and_media/photo.py
+-rw-r--r--   0        0        0     8233 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/messages_and_media/poll.py
+-rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/messages_and_media/poll_option.py
+-rw-r--r--   0        0        0     2641 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/messages_and_media/reaction.py
+-rw-r--r--   0        0        0     1937 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/messages_and_media/reaction_count.py
+-rw-r--r--   0        0        0     2400 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/messages_and_media/reaction_type.py
+-rw-r--r--   0        0        0     7010 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/messages_and_media/sticker.py
+-rw-r--r--   0        0        0     2879 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/messages_and_media/stickerset.py
+-rw-r--r--   0        0        0     1927 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/messages_and_media/stories_privacy_rules.py
+-rw-r--r--   0        0        0    76095 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/messages_and_media/story.py
+-rw-r--r--   0        0        0     2520 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/messages_and_media/story_deleted.py
+-rw-r--r--   0        0        0     3044 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/messages_and_media/story_forward_header.py
+-rw-r--r--   0        0        0     3291 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/messages_and_media/story_skipped.py
+-rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/messages_and_media/story_views.py
+-rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/messages_and_media/stripped_thumbnail.py
+-rw-r--r--   0        0        0     3773 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/messages_and_media/thumbnail.py
+-rw-r--r--   0        0        0     2293 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/messages_and_media/venue.py
+-rw-r--r--   0        0        0     4377 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/messages_and_media/video.py
+-rw-r--r--   0        0        0     3829 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/messages_and_media/video_note.py
+-rw-r--r--   0        0        0     3462 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/messages_and_media/voice.py
+-rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/messages_and_media/web_app_data.py
+-rw-r--r--   0        0        0     6424 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/messages_and_media/web_page.py
+-rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/messages_and_media/web_page_empty.py
+-rw-r--r--   0        0        0     2665 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/messages_and_media/web_page_preview.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/pyromod/__init__.py
+-rw-r--r--   0        0        0     3385 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/pyromod/identifier.py
+-rw-r--r--   0        0        0     2911 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/pyromod/listener.py
+-rw-r--r--   0        0        0     3678 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/user_and_chats/__init__.py
+-rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/user_and_chats/birthday.py
+-rw-r--r--   0        0        0     3066 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/user_and_chats/business_info.py
+-rw-r--r--   0        0        0     4565 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/user_and_chats/business_message.py
+-rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/user_and_chats/business_recipients.py
+-rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/user_and_chats/business_weekly_open.py
+-rw-r--r--   0        0        0     2044 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/user_and_chats/business_working_hours.py
+-rw-r--r--   0        0        0    43160 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/user_and_chats/chat.py
+-rw-r--r--   0        0        0     2247 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/user_and_chats/chat_admin_with_invite_links.py
+-rw-r--r--   0        0        0     2402 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/user_and_chats/chat_color.py
+-rw-r--r--   0        0        0    22799 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/user_and_chats/chat_event.py
+-rw-r--r--   0        0        0     5524 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/user_and_chats/chat_event_filter.py
+-rw-r--r--   0        0        0     4590 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/user_and_chats/chat_invite_link.py
+-rw-r--r--   0        0        0     4120 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/user_and_chats/chat_join_request.py
+-rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/user_and_chats/chat_joined_by_request.py
+-rw-r--r--   0        0        0     2565 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/user_and_chats/chat_joiner.py
+-rw-r--r--   0        0        0     9490 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/user_and_chats/chat_member.py
+-rw-r--r--   0        0        0     3758 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/user_and_chats/chat_member_updated.py
+-rw-r--r--   0        0        0    10248 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/user_and_chats/chat_permissions.py
+-rw-r--r--   0        0        0     3986 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/user_and_chats/chat_photo.py
+-rw-r--r--   0        0        0     2662 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/user_and_chats/chat_preview.py
+-rw-r--r--   0        0        0     6413 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/user_and_chats/chat_privileges.py
+-rw-r--r--   0        0        0     2491 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/user_and_chats/chat_reactions.py
+-rw-r--r--   0        0        0     2684 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/user_and_chats/dialog.py
+-rw-r--r--   0        0        0     2357 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/user_and_chats/emoji_status.py
+-rw-r--r--   0        0        0     5071 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/user_and_chats/forum_topic.py
+-rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/user_and_chats/forum_topic_closed.py
+-rw-r--r--   0        0        0     2045 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/user_and_chats/forum_topic_created.py
+-rw-r--r--   0        0        0     1919 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/user_and_chats/forum_topic_edited.py
+-rw-r--r--   0        0        0     1126 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/user_and_chats/forum_topic_reopened.py
+-rw-r--r--   0        0        0     1126 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/user_and_chats/general_forum_topic_hidden.py
+-rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/user_and_chats/general_forum_topic_unhidden.py
+-rw-r--r--   0        0        0     1922 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/user_and_chats/invite_link_importer.py
+-rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/user_and_chats/peer_channel.py
+-rw-r--r--   0        0        0     1328 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/user_and_chats/peer_user.py
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/user_and_chats/restriction.py
+-rw-r--r--   0        0        0    17666 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/user_and_chats/user.py
+-rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/user_and_chats/username.py
+-rw-r--r--   0        0        0     1324 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/user_and_chats/video_chat_ended.py
+-rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/user_and_chats/video_chat_members_invited.py
+-rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/user_and_chats/video_chat_scheduled.py
+-rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyrogram/types/user_and_chats/video_chat_started.py
+-rw-r--r--   0        0        0     1580 2020-02-02 00:00:00.000000 pyroblack-2.3.60/.gitignore
+-rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 pyroblack-2.3.60/COPYING
+-rw-r--r--   0        0        0     7651 2020-02-02 00:00:00.000000 pyroblack-2.3.60/COPYING.lesser
+-rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 pyroblack-2.3.60/NOTICE
+-rw-r--r--   0        0        0     2206 2020-02-02 00:00:00.000000 pyroblack-2.3.60/README.md
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 pyroblack-2.3.60/hatch_build.py
+-rw-r--r--   0        0        0     2727 2020-02-02 00:00:00.000000 pyroblack-2.3.60/pyproject.toml
+-rw-r--r--   0        0        0     4857 2020-02-02 00:00:00.000000 pyroblack-2.3.60/PKG-INFO
```

### Comparing `pyroblack-2.3.52/Makefile` & `pyroblack-2.3.60/Makefile`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/build-docs.sh` & `pyroblack-2.3.60/build-docs.sh`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/compiler/__init__.py` & `pyroblack-2.3.60/compiler/__init__.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/compiler/api/__init__.py` & `pyroblack-2.3.60/compiler/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/compiler/api/compiler.py` & `pyroblack-2.3.60/compiler/api/compiler.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/compiler/api/source/auth_key.tl` & `pyroblack-2.3.60/compiler/api/source/auth_key.tl`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/compiler/api/source/main_api.tl` & `pyroblack-2.3.60/compiler/api/source/main_api.tl`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/compiler/api/source/sys_msgs.tl` & `pyroblack-2.3.60/compiler/api/source/sys_msgs.tl`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/compiler/api/template/combinator.txt` & `pyroblack-2.3.60/compiler/api/template/combinator.txt`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/compiler/api/template/type.txt` & `pyroblack-2.3.60/compiler/api/template/type.txt`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/compiler/errors/__init__.py` & `pyroblack-2.3.60/compiler/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/compiler/errors/compiler.py` & `pyroblack-2.3.60/compiler/errors/compiler.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/compiler/errors/sort.py` & `pyroblack-2.3.60/compiler/errors/sort.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/compiler/errors/source/400_BAD_REQUEST.tsv` & `pyroblack-2.3.60/compiler/errors/source/400_BAD_REQUEST.tsv`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/compiler/errors/source/401_UNAUTHORIZED.tsv` & `pyroblack-2.3.60/compiler/errors/source/401_UNAUTHORIZED.tsv`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/compiler/errors/source/403_FORBIDDEN.tsv` & `pyroblack-2.3.60/compiler/errors/source/403_FORBIDDEN.tsv`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/compiler/errors/source/406_NOT_ACCEPTABLE.tsv` & `pyroblack-2.3.60/compiler/errors/source/406_NOT_ACCEPTABLE.tsv`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/compiler/errors/source/420_FLOOD.tsv` & `pyroblack-2.3.60/compiler/errors/source/420_FLOOD.tsv`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/compiler/errors/source/500_INTERNAL_SERVER_ERROR.tsv` & `pyroblack-2.3.60/compiler/errors/source/500_INTERNAL_SERVER_ERROR.tsv`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/__init__.py` & `pyroblack-2.3.60/pyrogram/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with pyroblack.  If not, see <http://www.gnu.org/licenses/>.
 
 __fork_name__ = "pyroblack"
-__version__ = "2.3.52"
+__version__ = "2.3.60"
 __license__ = "GNU Lesser General Public License v3.0 (LGPL-3.0)"
 __copyright__ = "#  Copyright (C) 2024-present eyMarv <https://github.com/eyMarv>"
 
 from concurrent.futures.thread import ThreadPoolExecutor
 
 
 class StopTransmission(Exception):
```

### Comparing `pyroblack-2.3.52/pyrogram/client.py` & `pyroblack-2.3.60/pyrogram/client.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/dispatcher.py` & `pyroblack-2.3.60/pyrogram/dispatcher.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/emoji.py` & `pyroblack-2.3.60/pyrogram/emoji.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/file_id.py` & `pyroblack-2.3.60/pyrogram/file_id.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/filters.py` & `pyroblack-2.3.60/pyrogram/filters.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/mime_types.py` & `pyroblack-2.3.60/pyrogram/mime_types.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/sync.py` & `pyroblack-2.3.60/pyrogram/sync.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/utils.py` & `pyroblack-2.3.60/pyrogram/utils.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/connection/__init__.py` & `pyroblack-2.3.60/pyrogram/connection/__init__.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/connection/connection.py` & `pyroblack-2.3.60/pyrogram/connection/connection.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/connection/transport/__init__.py` & `pyroblack-2.3.60/pyrogram/connection/transport/__init__.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/connection/transport/tcp/__init__.py` & `pyroblack-2.3.60/pyrogram/connection/transport/tcp/__init__.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/connection/transport/tcp/tcp.py` & `pyroblack-2.3.60/pyrogram/connection/transport/tcp/tcp.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/connection/transport/tcp/tcp_abridged.py` & `pyroblack-2.3.60/pyrogram/connection/transport/tcp/tcp_abridged.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/connection/transport/tcp/tcp_abridged_o.py` & `pyroblack-2.3.60/pyrogram/connection/transport/tcp/tcp_abridged_o.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/connection/transport/tcp/tcp_full.py` & `pyroblack-2.3.60/pyrogram/connection/transport/tcp/tcp_full.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/connection/transport/tcp/tcp_intermediate.py` & `pyroblack-2.3.60/pyrogram/connection/transport/tcp/tcp_intermediate.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/connection/transport/tcp/tcp_intermediate_o.py` & `pyroblack-2.3.60/pyrogram/connection/transport/tcp/tcp_intermediate_o.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/crypto/__init__.py` & `pyroblack-2.3.60/pyrogram/crypto/__init__.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/crypto/aes.py` & `pyroblack-2.3.60/pyrogram/crypto/aes.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/crypto/mtproto.py` & `pyroblack-2.3.60/pyrogram/crypto/mtproto.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/crypto/prime.py` & `pyroblack-2.3.60/pyrogram/crypto/prime.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/crypto/rsa.py` & `pyroblack-2.3.60/pyrogram/crypto/rsa.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/enums/__init__.py` & `pyroblack-2.3.60/pyrogram/enums/__init__.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/enums/auto_name.py` & `pyroblack-2.3.60/pyrogram/enums/auto_name.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/enums/business_schedule.py` & `pyroblack-2.3.60/pyrogram/enums/business_schedule.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/enums/chat_action.py` & `pyroblack-2.3.60/pyrogram/enums/chat_action.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/enums/chat_event_action.py` & `pyroblack-2.3.60/pyrogram/enums/chat_event_action.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/enums/chat_member_status.py` & `pyroblack-2.3.60/pyrogram/enums/chat_member_status.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/enums/chat_members_filter.py` & `pyroblack-2.3.60/pyrogram/enums/chat_members_filter.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/enums/chat_type.py` & `pyroblack-2.3.60/pyrogram/enums/chat_type.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/enums/listerner_types.py` & `pyroblack-2.3.60/pyrogram/enums/listerner_types.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/enums/message_entity_type.py` & `pyroblack-2.3.60/pyrogram/enums/message_entity_type.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/enums/message_media_type.py` & `pyroblack-2.3.60/pyrogram/enums/message_media_type.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/enums/message_service_type.py` & `pyroblack-2.3.60/pyrogram/enums/message_service_type.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/enums/messages_filter.py` & `pyroblack-2.3.60/pyrogram/enums/messages_filter.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/enums/next_code_type.py` & `pyroblack-2.3.60/pyrogram/enums/next_code_type.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/enums/parse_mode.py` & `pyroblack-2.3.60/pyrogram/enums/parse_mode.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/enums/poll_type.py` & `pyroblack-2.3.60/pyrogram/enums/poll_type.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/enums/profile_color.py` & `pyroblack-2.3.60/pyrogram/enums/profile_color.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/enums/reaction_type.py` & `pyroblack-2.3.60/pyrogram/enums/reaction_type.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/enums/reply_color.py` & `pyroblack-2.3.60/pyrogram/enums/reply_color.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/enums/sent_code_type.py` & `pyroblack-2.3.60/pyrogram/enums/sent_code_type.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/enums/stories_privacy_rules.py` & `pyroblack-2.3.60/pyrogram/enums/stories_privacy_rules.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/enums/story_privacy.py` & `pyroblack-2.3.60/pyrogram/enums/story_privacy.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/enums/user_status.py` & `pyroblack-2.3.60/pyrogram/enums/user_status.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/errors/__init__.py` & `pyroblack-2.3.60/pyrogram/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/errors/rpc_error.py` & `pyroblack-2.3.60/pyrogram/errors/rpc_error.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/handlers/__init__.py` & `pyroblack-2.3.60/pyrogram/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/handlers/callback_query_handler.py` & `pyroblack-2.3.60/pyrogram/handlers/callback_query_handler.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/handlers/chat_join_request_handler.py` & `pyroblack-2.3.60/pyrogram/handlers/chat_join_request_handler.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/handlers/chat_member_updated_handler.py` & `pyroblack-2.3.60/pyrogram/handlers/chat_member_updated_handler.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/handlers/chosen_inline_result_handler.py` & `pyroblack-2.3.60/pyrogram/handlers/chosen_inline_result_handler.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/handlers/conversation_handler.py` & `pyroblack-2.3.60/pyrogram/handlers/conversation_handler.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/handlers/deleted_messages_handler.py` & `pyroblack-2.3.60/pyrogram/handlers/deleted_messages_handler.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/handlers/disconnect_handler.py` & `pyroblack-2.3.60/pyrogram/handlers/disconnect_handler.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/handlers/edited_message_handler.py` & `pyroblack-2.3.60/pyrogram/handlers/edited_message_handler.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/handlers/handler.py` & `pyroblack-2.3.60/pyrogram/handlers/handler.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/handlers/inline_query_handler.py` & `pyroblack-2.3.60/pyrogram/handlers/inline_query_handler.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/handlers/message_handler.py` & `pyroblack-2.3.60/pyrogram/handlers/message_handler.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/handlers/message_reaction_count_updated_handler.py` & `pyroblack-2.3.60/pyrogram/handlers/message_reaction_count_updated_handler.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/handlers/message_reaction_updated_handler.py` & `pyroblack-2.3.60/pyrogram/handlers/message_reaction_updated_handler.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/handlers/poll_handler.py` & `pyroblack-2.3.60/pyrogram/handlers/poll_handler.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/handlers/raw_update_handler.py` & `pyroblack-2.3.60/pyrogram/handlers/raw_update_handler.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/handlers/story_handler.py` & `pyroblack-2.3.60/pyrogram/handlers/story_handler.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/handlers/user_status_handler.py` & `pyroblack-2.3.60/pyrogram/handlers/user_status_handler.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/helpers/__init__.py` & `pyroblack-2.3.60/pyrogram/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/helpers/helpers.py` & `pyroblack-2.3.60/pyrogram/helpers/helpers.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/__init__.py` & `pyroblack-2.3.60/pyrogram/methods/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,26 +23,28 @@
 from .bots import Bots
 from .chats import Chats
 from .contacts import Contacts
 from .decorators import Decorators
 from .invite_links import InviteLinks
 from .messages import Messages
 from .password import Password
+from .payments import Payments
 from .pyromod import Pyromod
 from .stickers import Stickers
 from .users import Users
 from .utilities import Utilities
 
 
 class Methods(
     Advanced,
     Auth,
     Bots,
     Contacts,
     Password,
+    Payments,
     Pyromod,
     Chats,
     Stickers,
     Users,
     Messages,
     Decorators,
     Utilities,
```

### Comparing `pyroblack-2.3.52/pyrogram/methods/advanced/__init__.py` & `pyroblack-2.3.60/pyrogram/methods/advanced/__init__.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/advanced/invoke.py` & `pyroblack-2.3.60/pyrogram/methods/advanced/invoke.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/advanced/resolve_peer.py` & `pyroblack-2.3.60/pyrogram/methods/advanced/resolve_peer.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/advanced/save_file.py` & `pyroblack-2.3.60/pyrogram/methods/advanced/save_file.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/auth/__init__.py` & `pyroblack-2.3.60/pyrogram/methods/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/auth/accept_terms_of_service.py` & `pyroblack-2.3.60/pyrogram/methods/auth/accept_terms_of_service.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/auth/check_password.py` & `pyroblack-2.3.60/pyrogram/methods/auth/check_password.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/auth/connect.py` & `pyroblack-2.3.60/pyrogram/methods/auth/connect.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/auth/disconnect.py` & `pyroblack-2.3.60/pyrogram/methods/auth/disconnect.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/auth/get_password_hint.py` & `pyroblack-2.3.60/pyrogram/methods/auth/get_password_hint.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/auth/initialize.py` & `pyroblack-2.3.60/pyrogram/methods/auth/initialize.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/auth/log_out.py` & `pyroblack-2.3.60/pyrogram/methods/auth/log_out.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/auth/recover_password.py` & `pyroblack-2.3.60/pyrogram/methods/auth/recover_password.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/auth/resend_code.py` & `pyroblack-2.3.60/pyrogram/methods/auth/resend_code.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/auth/send_code.py` & `pyroblack-2.3.60/pyrogram/methods/auth/send_code.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/auth/send_recovery_code.py` & `pyroblack-2.3.60/pyrogram/methods/auth/send_recovery_code.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/auth/sign_in.py` & `pyroblack-2.3.60/pyrogram/methods/auth/sign_in.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/auth/sign_in_bot.py` & `pyroblack-2.3.60/pyrogram/methods/auth/sign_in_bot.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/auth/sign_up.py` & `pyroblack-2.3.60/pyrogram/methods/auth/sign_up.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/auth/terminate.py` & `pyroblack-2.3.60/pyrogram/methods/auth/terminate.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/bots/__init__.py` & `pyroblack-2.3.60/pyrogram/methods/bots/__init__.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/bots/answer_callback_query.py` & `pyroblack-2.3.60/pyrogram/methods/bots/answer_callback_query.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/bots/answer_inline_query.py` & `pyroblack-2.3.60/pyrogram/methods/bots/answer_inline_query.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/bots/answer_web_app_query.py` & `pyroblack-2.3.60/pyrogram/methods/bots/answer_web_app_query.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/bots/delete_bot_commands.py` & `pyroblack-2.3.60/pyrogram/methods/bots/delete_bot_commands.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/bots/get_bot_commands.py` & `pyroblack-2.3.60/pyrogram/methods/bots/get_bot_commands.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/bots/get_bot_default_privileges.py` & `pyroblack-2.3.60/pyrogram/methods/bots/get_bot_default_privileges.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/bots/get_bot_info.py` & `pyroblack-2.3.60/pyrogram/methods/bots/get_bot_info.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/bots/get_chat_menu_button.py` & `pyroblack-2.3.60/pyrogram/methods/bots/get_chat_menu_button.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/bots/get_game_high_scores.py` & `pyroblack-2.3.60/pyrogram/methods/bots/get_game_high_scores.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/bots/get_inline_bot_results.py` & `pyroblack-2.3.60/pyrogram/methods/bots/get_inline_bot_results.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/bots/request_callback_answer.py` & `pyroblack-2.3.60/pyrogram/methods/bots/request_callback_answer.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/bots/send_game.py` & `pyroblack-2.3.60/pyrogram/methods/bots/send_game.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/bots/send_inline_bot_result.py` & `pyroblack-2.3.60/pyrogram/methods/bots/send_inline_bot_result.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/bots/set_bot_commands.py` & `pyroblack-2.3.60/pyrogram/methods/bots/set_bot_commands.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/bots/set_bot_default_privileges.py` & `pyroblack-2.3.60/pyrogram/methods/bots/set_bot_default_privileges.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/bots/set_bot_info.py` & `pyroblack-2.3.60/pyrogram/methods/bots/set_bot_info.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/bots/set_chat_menu_button.py` & `pyroblack-2.3.60/pyrogram/methods/bots/set_chat_menu_button.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/bots/set_game_score.py` & `pyroblack-2.3.60/pyrogram/methods/bots/set_game_score.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/chats/__init__.py` & `pyroblack-2.3.60/pyrogram/methods/chats/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,17 @@
 from .get_dialogs_count import GetDialogsCount
 from .get_forum_topics import GetForumTopics
 from .get_forum_topics_by_id import GetForumTopicsByID
 from .get_nearby_chats import GetNearbyChats
 from .get_send_as_chats import GetSendAsChats
 from .hide_general_topic import HideGeneralTopic
 from .join_chat import JoinChat
+from .join_folder import JoinFolder
 from .leave_chat import LeaveChat
+from .leave_folder import LeaveFolder
 from .mark_chat_unread import MarkChatUnread
 from .pin_chat_message import PinChatMessage
 from .promote_chat_member import PromoteChatMember
 from .reopen_forum_topic import ReopenForumTopic
 from .reopen_general_topic import ReopenGeneralTopic
 from .restrict_chat_member import RestrictChatMember
 from .set_administrator_title import SetAdministratorTitle
@@ -74,15 +76,17 @@
 from .unpin_chat_message import UnpinChatMessage
 from .update_color import UpdateColor
 
 
 class Chats(
     GetChat,
     LeaveChat,
+    LeaveFolder,
     JoinChat,
+    JoinFolder,
     BanChatMember,
     UnbanChatMember,
     RestrictChatMember,
     PromoteChatMember,
     GetChatMembers,
     GetChatMember,
     SetChatPhoto,
```

### Comparing `pyroblack-2.3.52/pyrogram/methods/chats/add_chat_members.py` & `pyroblack-2.3.60/pyrogram/methods/chats/add_chat_members.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/chats/archive_chats.py` & `pyroblack-2.3.60/pyrogram/methods/chats/archive_chats.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/chats/ban_chat_member.py` & `pyroblack-2.3.60/pyrogram/methods/chats/ban_chat_member.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/chats/close_forum_topic.py` & `pyroblack-2.3.60/pyrogram/methods/chats/close_forum_topic.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/chats/close_general_topic.py` & `pyroblack-2.3.60/pyrogram/methods/chats/close_general_topic.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/chats/create_channel.py` & `pyroblack-2.3.60/pyrogram/methods/chats/create_channel.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/chats/create_forum_topic.py` & `pyroblack-2.3.60/pyrogram/methods/chats/create_forum_topic.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/chats/create_group.py` & `pyroblack-2.3.60/pyrogram/methods/chats/create_group.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/chats/create_supergroup.py` & `pyroblack-2.3.60/pyrogram/methods/chats/create_supergroup.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/chats/delete_channel.py` & `pyroblack-2.3.60/pyrogram/methods/chats/delete_channel.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/chats/delete_chat_photo.py` & `pyroblack-2.3.60/pyrogram/methods/chats/delete_chat_photo.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/chats/delete_forum_topic.py` & `pyroblack-2.3.60/pyrogram/methods/chats/delete_forum_topic.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/chats/delete_supergroup.py` & `pyroblack-2.3.60/pyrogram/methods/chats/delete_supergroup.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/chats/delete_user_history.py` & `pyroblack-2.3.60/pyrogram/methods/chats/delete_user_history.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/chats/edit_forum_topic.py` & `pyroblack-2.3.60/pyrogram/methods/chats/edit_forum_topic.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/chats/edit_general_topic.py` & `pyroblack-2.3.60/pyrogram/methods/chats/edit_general_topic.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/chats/get_chat.py` & `pyroblack-2.3.60/pyrogram/methods/chats/get_chat.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/chats/get_chat_event_log.py` & `pyroblack-2.3.60/pyrogram/methods/chats/get_chat_event_log.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/chats/get_chat_member.py` & `pyroblack-2.3.60/pyrogram/methods/chats/get_chat_member.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/chats/get_chat_members.py` & `pyroblack-2.3.60/pyrogram/methods/chats/get_chat_members.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/chats/get_chat_members_count.py` & `pyroblack-2.3.60/pyrogram/methods/chats/get_chat_members_count.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/chats/get_chat_online_count.py` & `pyroblack-2.3.60/pyrogram/methods/chats/get_chat_online_count.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/chats/get_dialogs.py` & `pyroblack-2.3.60/pyrogram/methods/chats/get_dialogs.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/chats/get_dialogs_count.py` & `pyroblack-2.3.60/pyrogram/methods/chats/get_dialogs_count.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/chats/get_forum_topics.py` & `pyroblack-2.3.60/pyrogram/methods/chats/get_forum_topics.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/chats/get_forum_topics_by_id.py` & `pyroblack-2.3.60/pyrogram/methods/chats/get_forum_topics_by_id.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/chats/get_nearby_chats.py` & `pyroblack-2.3.60/pyrogram/methods/chats/get_nearby_chats.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/chats/get_send_as_chats.py` & `pyroblack-2.3.60/pyrogram/methods/chats/get_send_as_chats.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/chats/hide_general_topic.py` & `pyroblack-2.3.60/pyrogram/methods/chats/hide_general_topic.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/chats/join_chat.py` & `pyroblack-2.3.60/pyrogram/methods/chats/join_chat.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/chats/leave_chat.py` & `pyroblack-2.3.60/pyrogram/methods/chats/leave_chat.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/chats/mark_chat_unread.py` & `pyroblack-2.3.60/pyrogram/methods/chats/mark_chat_unread.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/chats/pin_chat_message.py` & `pyroblack-2.3.60/pyrogram/methods/chats/pin_chat_message.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/chats/promote_chat_member.py` & `pyroblack-2.3.60/pyrogram/methods/chats/promote_chat_member.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/chats/reopen_forum_topic.py` & `pyroblack-2.3.60/pyrogram/methods/chats/reopen_forum_topic.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/chats/reopen_general_topic.py` & `pyroblack-2.3.60/pyrogram/methods/chats/reopen_general_topic.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/chats/restrict_chat_member.py` & `pyroblack-2.3.60/pyrogram/methods/chats/restrict_chat_member.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/chats/set_administrator_title.py` & `pyroblack-2.3.60/pyrogram/methods/chats/set_administrator_title.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/chats/set_chat_description.py` & `pyroblack-2.3.60/pyrogram/methods/chats/set_chat_description.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/chats/set_chat_permissions.py` & `pyroblack-2.3.60/pyrogram/methods/chats/set_chat_permissions.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/chats/set_chat_photo.py` & `pyroblack-2.3.60/pyrogram/methods/chats/set_chat_photo.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/chats/set_chat_protected_content.py` & `pyroblack-2.3.60/pyrogram/methods/chats/set_chat_protected_content.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/chats/set_chat_title.py` & `pyroblack-2.3.60/pyrogram/methods/chats/set_chat_title.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/chats/set_chat_username.py` & `pyroblack-2.3.60/pyrogram/methods/chats/set_chat_username.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/chats/set_send_as_chat.py` & `pyroblack-2.3.60/pyrogram/methods/chats/set_send_as_chat.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/chats/set_slow_mode.py` & `pyroblack-2.3.60/pyrogram/methods/chats/set_slow_mode.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/chats/toggle_folder_tags.py` & `pyroblack-2.3.60/pyrogram/methods/chats/toggle_folder_tags.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/chats/toggle_forum_topics.py` & `pyroblack-2.3.60/pyrogram/methods/chats/toggle_forum_topics.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/chats/toggle_join_to_send.py` & `pyroblack-2.3.60/pyrogram/methods/chats/toggle_join_to_send.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/chats/unarchive_chats.py` & `pyroblack-2.3.60/pyrogram/methods/chats/unarchive_chats.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/chats/unban_chat_member.py` & `pyroblack-2.3.60/pyrogram/methods/chats/unban_chat_member.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/chats/unhide_general_topic.py` & `pyroblack-2.3.60/pyrogram/methods/chats/unhide_general_topic.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/chats/unpin_all_chat_messages.py` & `pyroblack-2.3.60/pyrogram/methods/chats/unpin_all_chat_messages.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/chats/unpin_chat_message.py` & `pyroblack-2.3.60/pyrogram/methods/chats/unpin_chat_message.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/chats/update_color.py` & `pyroblack-2.3.60/pyrogram/methods/chats/update_color.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/contacts/__init__.py` & `pyroblack-2.3.60/pyrogram/methods/contacts/__init__.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/contacts/add_contact.py` & `pyroblack-2.3.60/pyrogram/methods/contacts/add_contact.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/contacts/delete_contacts.py` & `pyroblack-2.3.60/pyrogram/methods/contacts/delete_contacts.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/contacts/get_contacts.py` & `pyroblack-2.3.60/pyrogram/methods/contacts/get_contacts.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/contacts/get_contacts_count.py` & `pyroblack-2.3.60/pyrogram/methods/contacts/get_contacts_count.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/contacts/import_contacts.py` & `pyroblack-2.3.60/pyrogram/methods/contacts/import_contacts.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/decorators/__init__.py` & `pyroblack-2.3.60/pyrogram/methods/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/decorators/on_callback_query.py` & `pyroblack-2.3.60/pyrogram/methods/decorators/on_callback_query.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/decorators/on_chat_join_request.py` & `pyroblack-2.3.60/pyrogram/methods/decorators/on_chat_join_request.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/decorators/on_chat_member_updated.py` & `pyroblack-2.3.60/pyrogram/methods/decorators/on_chat_member_updated.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/decorators/on_chosen_inline_result.py` & `pyroblack-2.3.60/pyrogram/methods/decorators/on_chosen_inline_result.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/decorators/on_deleted_messages.py` & `pyroblack-2.3.60/pyrogram/methods/decorators/on_deleted_messages.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/decorators/on_disconnect.py` & `pyroblack-2.3.60/pyrogram/methods/decorators/on_disconnect.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/decorators/on_edited_message.py` & `pyroblack-2.3.60/pyrogram/methods/decorators/on_edited_message.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/decorators/on_inline_query.py` & `pyroblack-2.3.60/pyrogram/methods/decorators/on_inline_query.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/decorators/on_message.py` & `pyroblack-2.3.60/pyrogram/methods/decorators/on_message.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/decorators/on_message_reaction_count_updated.py` & `pyroblack-2.3.60/pyrogram/methods/decorators/on_message_reaction_count_updated.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/decorators/on_message_reaction_updated.py` & `pyroblack-2.3.60/pyrogram/methods/decorators/on_message_reaction_updated.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/decorators/on_poll.py` & `pyroblack-2.3.60/pyrogram/methods/decorators/on_poll.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/decorators/on_raw_update.py` & `pyroblack-2.3.60/pyrogram/methods/decorators/on_raw_update.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/decorators/on_story.py` & `pyroblack-2.3.60/pyrogram/methods/decorators/on_story.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/decorators/on_user_status.py` & `pyroblack-2.3.60/pyrogram/methods/decorators/on_user_status.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/invite_links/__init__.py` & `pyroblack-2.3.60/pyrogram/methods/invite_links/__init__.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/invite_links/approve_all_chat_join_requests.py` & `pyroblack-2.3.60/pyrogram/methods/invite_links/approve_all_chat_join_requests.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/invite_links/approve_chat_join_request.py` & `pyroblack-2.3.60/pyrogram/methods/invite_links/approve_chat_join_request.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/invite_links/create_chat_invite_link.py` & `pyroblack-2.3.60/pyrogram/methods/invite_links/create_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/invite_links/decline_all_chat_join_requests.py` & `pyroblack-2.3.60/pyrogram/methods/invite_links/decline_all_chat_join_requests.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/invite_links/decline_chat_join_request.py` & `pyroblack-2.3.60/pyrogram/methods/invite_links/decline_chat_join_request.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/invite_links/delete_chat_admin_invite_links.py` & `pyroblack-2.3.60/pyrogram/methods/invite_links/delete_chat_admin_invite_links.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/invite_links/delete_chat_invite_link.py` & `pyroblack-2.3.60/pyrogram/methods/invite_links/delete_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/invite_links/edit_chat_invite_link.py` & `pyroblack-2.3.60/pyrogram/methods/invite_links/edit_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/invite_links/export_chat_invite_link.py` & `pyroblack-2.3.60/pyrogram/methods/invite_links/export_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/invite_links/get_chat_admin_invite_links.py` & `pyroblack-2.3.60/pyrogram/methods/invite_links/get_chat_admin_invite_links.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/invite_links/get_chat_admin_invite_links_count.py` & `pyroblack-2.3.60/pyrogram/methods/invite_links/get_chat_admin_invite_links_count.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/invite_links/get_chat_admins_with_invite_links.py` & `pyroblack-2.3.60/pyrogram/methods/invite_links/get_chat_admins_with_invite_links.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/invite_links/get_chat_invite_link.py` & `pyroblack-2.3.60/pyrogram/methods/invite_links/get_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/invite_links/get_chat_invite_link_joiners.py` & `pyroblack-2.3.60/pyrogram/methods/invite_links/get_chat_invite_link_joiners.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/invite_links/get_chat_invite_link_joiners_count.py` & `pyroblack-2.3.60/pyrogram/methods/invite_links/get_chat_invite_link_joiners_count.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/invite_links/get_chat_join_requests.py` & `pyroblack-2.3.60/pyrogram/methods/invite_links/get_chat_join_requests.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/invite_links/revoke_chat_invite_link.py` & `pyroblack-2.3.60/pyrogram/methods/invite_links/revoke_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/messages/__init__.py` & `pyroblack-2.3.60/pyrogram/methods/messages/__init__.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/messages/copy_media_group.py` & `pyroblack-2.3.60/pyrogram/methods/messages/copy_media_group.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/messages/copy_message.py` & `pyroblack-2.3.60/pyrogram/methods/messages/copy_message.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/messages/delete_messages.py` & `pyroblack-2.3.60/pyrogram/methods/messages/delete_messages.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/messages/download_media.py` & `pyroblack-2.3.60/pyrogram/methods/messages/download_media.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,14 +100,17 @@
 
                 # Download from Message
                 await app.download_media(message)
 
                 # Download from file id
                 await app.download_media(message.photo.file_id)
 
+                # Download document of a message
+                await app.download_media(message.document)
+
                 # Keep track of the progress while downloading
                 async def progress(current, total):
                     print(f"{current * 100 / total:.1f}%")
 
                 await app.download_media(message, progress=progress)
 
             Download media in-memory
@@ -135,14 +138,16 @@
             for kind in available_media:
                 media = getattr(message, kind, None)
 
                 if media is not None:
                     break
             else:
                 raise ValueError("This message doesn't contain any downloadable media")
+        elif hasattr(message, "file_id"):
+            media = getattr(message, "file_id")
         else:
             media = message
 
         if isinstance(media, str):
             file_id_str = media
         else:
             file_id_str = media.file_id
```

### Comparing `pyroblack-2.3.52/pyrogram/methods/messages/edit_inline_caption.py` & `pyroblack-2.3.60/pyrogram/methods/messages/edit_inline_caption.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/messages/edit_inline_media.py` & `pyroblack-2.3.60/pyrogram/methods/messages/edit_inline_media.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/messages/edit_inline_reply_markup.py` & `pyroblack-2.3.60/pyrogram/methods/messages/edit_inline_reply_markup.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/messages/edit_inline_text.py` & `pyroblack-2.3.60/pyrogram/methods/messages/edit_inline_text.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/messages/edit_message_caption.py` & `pyroblack-2.3.60/pyrogram/methods/messages/edit_message_caption.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/messages/edit_message_media.py` & `pyroblack-2.3.60/pyrogram/methods/messages/edit_message_media.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/messages/edit_message_reply_markup.py` & `pyroblack-2.3.60/pyrogram/methods/messages/edit_message_reply_markup.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/messages/edit_message_text.py` & `pyroblack-2.3.60/pyrogram/methods/messages/edit_message_text.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/messages/forward_messages.py` & `pyroblack-2.3.60/pyrogram/methods/messages/forward_messages.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/messages/get_chat_history.py` & `pyroblack-2.3.60/pyrogram/methods/messages/get_chat_history.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/messages/get_chat_history_count.py` & `pyroblack-2.3.60/pyrogram/methods/messages/get_chat_history_count.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/messages/get_custom_emoji_stickers.py` & `pyroblack-2.3.60/pyrogram/methods/messages/get_custom_emoji_stickers.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/messages/get_discussion_message.py` & `pyroblack-2.3.60/pyrogram/methods/messages/get_discussion_message.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/messages/get_discussion_replies.py` & `pyroblack-2.3.60/pyrogram/methods/messages/get_discussion_replies.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/messages/get_discussion_replies_count.py` & `pyroblack-2.3.60/pyrogram/methods/messages/get_discussion_replies_count.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/messages/get_media_group.py` & `pyroblack-2.3.60/pyrogram/methods/messages/get_media_group.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/messages/get_messages.py` & `pyroblack-2.3.60/pyrogram/methods/messages/get_messages.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/messages/get_scheduled_messages.py` & `pyroblack-2.3.60/pyrogram/methods/messages/get_scheduled_messages.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,13 +50,11 @@
                 # Get scheduled messages
                 await app.get_scheduled_messages(chat_id)
 
         Raises:
             ValueError: In case of invalid arguments.
         """
         r = await self.invoke(
-            raw.functions.GetScheduledHistory(
-                peer=await self.resolve_peer(chat_id), hash=0
-            )
+            raw.functions.messages.GetScheduledHistory(peer=await self.resolve_peer(chat_id), hash=0)
         )
 
         return await utils.parse_messages(self, r, replies=0)
```

### Comparing `pyroblack-2.3.52/pyrogram/methods/messages/get_stickers.py` & `pyroblack-2.3.60/pyrogram/methods/messages/get_stickers.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/messages/inline_session.py` & `pyroblack-2.3.60/pyrogram/methods/messages/inline_session.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/messages/read_chat_history.py` & `pyroblack-2.3.60/pyrogram/methods/messages/read_chat_history.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/messages/retract_vote.py` & `pyroblack-2.3.60/pyrogram/methods/messages/retract_vote.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/messages/search_global.py` & `pyroblack-2.3.60/pyrogram/methods/messages/search_global.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/messages/search_global_count.py` & `pyroblack-2.3.60/pyrogram/methods/messages/search_global_count.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/messages/search_messages.py` & `pyroblack-2.3.60/pyrogram/methods/messages/search_messages.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/messages/search_messages_count.py` & `pyroblack-2.3.60/pyrogram/methods/messages/search_messages_count.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/messages/send_animation.py` & `pyroblack-2.3.60/pyrogram/methods/messages/send_animation.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/messages/send_audio.py` & `pyroblack-2.3.60/pyrogram/methods/messages/send_audio.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/messages/send_cached_media.py` & `pyroblack-2.3.60/pyrogram/methods/messages/send_cached_media.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/messages/send_chat_action.py` & `pyroblack-2.3.60/pyrogram/methods/messages/send_chat_action.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/messages/send_contact.py` & `pyroblack-2.3.60/pyrogram/methods/messages/send_contact.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/messages/send_dice.py` & `pyroblack-2.3.60/pyrogram/methods/messages/send_dice.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/messages/send_document.py` & `pyroblack-2.3.60/pyrogram/methods/messages/send_document.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/messages/send_location.py` & `pyroblack-2.3.60/pyrogram/methods/messages/send_location.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/messages/send_media_group.py` & `pyroblack-2.3.60/pyrogram/methods/messages/send_media_group.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/messages/send_message.py` & `pyroblack-2.3.60/pyrogram/methods/messages/send_message.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/messages/send_photo.py` & `pyroblack-2.3.60/pyrogram/methods/messages/send_photo.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/messages/send_poll.py` & `pyroblack-2.3.60/pyrogram/methods/messages/send_poll.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/messages/send_reaction.py` & `pyroblack-2.3.60/pyrogram/methods/messages/send_reaction.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/messages/send_sticker.py` & `pyroblack-2.3.60/pyrogram/methods/messages/send_sticker.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/messages/send_venue.py` & `pyroblack-2.3.60/pyrogram/methods/messages/send_venue.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/messages/send_video.py` & `pyroblack-2.3.60/pyrogram/methods/messages/send_video.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/messages/send_video_note.py` & `pyroblack-2.3.60/pyrogram/methods/messages/send_video_note.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/messages/send_voice.py` & `pyroblack-2.3.60/pyrogram/methods/messages/send_voice.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/messages/send_web_page.py` & `pyroblack-2.3.60/pyrogram/methods/messages/send_web_page.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/messages/stop_poll.py` & `pyroblack-2.3.60/pyrogram/methods/messages/stop_poll.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/messages/stream_media.py` & `pyroblack-2.3.60/pyrogram/methods/messages/stream_media.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/messages/vote_poll.py` & `pyroblack-2.3.60/pyrogram/methods/messages/vote_poll.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/password/__init__.py` & `pyroblack-2.3.60/pyrogram/methods/password/__init__.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/password/change_cloud_password.py` & `pyroblack-2.3.60/pyrogram/methods/password/change_cloud_password.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/password/enable_cloud_password.py` & `pyroblack-2.3.60/pyrogram/methods/password/enable_cloud_password.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/password/remove_cloud_password.py` & `pyroblack-2.3.60/pyrogram/methods/password/remove_cloud_password.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/pyromod/__init__.py` & `pyroblack-2.3.60/pyrogram/methods/pyromod/__init__.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/pyromod/ask.py` & `pyroblack-2.3.60/pyrogram/methods/pyromod/ask.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/pyromod/get_listener_matching_with_data.py` & `pyroblack-2.3.60/pyrogram/methods/pyromod/get_listener_matching_with_data.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/pyromod/get_listener_matching_with_identifier_pattern.py` & `pyroblack-2.3.60/pyrogram/methods/pyromod/get_listener_matching_with_identifier_pattern.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/pyromod/get_many_listeners_matching_with_data.py` & `pyroblack-2.3.60/pyrogram/methods/pyromod/get_many_listeners_matching_with_data.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/pyromod/get_many_listeners_matching_with_identifier_pattern.py` & `pyroblack-2.3.60/pyrogram/methods/pyromod/get_many_listeners_matching_with_identifier_pattern.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/pyromod/listen.py` & `pyroblack-2.3.60/pyrogram/methods/pyromod/listen.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/pyromod/register_next_step_handler.py` & `pyroblack-2.3.60/pyrogram/methods/pyromod/register_next_step_handler.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/pyromod/remove_listerner.py` & `pyroblack-2.3.60/pyrogram/methods/pyromod/remove_listerner.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/pyromod/stop_listener.py` & `pyroblack-2.3.60/pyrogram/methods/pyromod/stop_listener.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/pyromod/stop_listening.py` & `pyroblack-2.3.60/pyrogram/methods/pyromod/stop_listening.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/pyromod/wait_for_callback_query.py` & `pyroblack-2.3.60/pyrogram/methods/pyromod/wait_for_callback_query.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/pyromod/wait_for_message.py` & `pyroblack-2.3.60/pyrogram/methods/pyromod/wait_for_message.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/stickers/__init__.py` & `pyroblack-2.3.60/pyrogram/methods/stickers/__init__.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/stickers/add_sticker_to_set.py` & `pyroblack-2.3.60/pyrogram/methods/stickers/add_sticker_to_set.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/stickers/create_sticker_set.py` & `pyroblack-2.3.60/pyrogram/methods/stickers/create_sticker_set.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/stickers/get_sticker_set.py` & `pyroblack-2.3.60/pyrogram/methods/stickers/get_sticker_set.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/users/__init__.py` & `pyroblack-2.3.60/pyrogram/methods/users/__init__.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/users/block_user.py` & `pyroblack-2.3.60/pyrogram/methods/users/block_user.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/users/check_username.py` & `pyroblack-2.3.60/pyrogram/methods/users/check_username.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/users/delete_profile_photos.py` & `pyroblack-2.3.60/pyrogram/methods/users/delete_profile_photos.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/users/delete_stories.py` & `pyroblack-2.3.60/pyrogram/methods/users/delete_stories.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/users/edit_story.py` & `pyroblack-2.3.60/pyrogram/methods/users/edit_story.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/users/export_story_link.py` & `pyroblack-2.3.60/pyrogram/methods/users/export_story_link.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/users/forward_story.py` & `pyroblack-2.3.60/pyrogram/methods/users/forward_story.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/users/get_all_stories.py` & `pyroblack-2.3.60/pyrogram/methods/users/get_all_stories.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/users/get_chat_photos.py` & `pyroblack-2.3.60/pyrogram/methods/users/get_chat_photos.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/users/get_chat_photos_count.py` & `pyroblack-2.3.60/pyrogram/methods/users/get_chat_photos_count.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/users/get_common_chats.py` & `pyroblack-2.3.60/pyrogram/methods/users/get_common_chats.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/users/get_default_emoji_statuses.py` & `pyroblack-2.3.60/pyrogram/methods/users/get_default_emoji_statuses.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/users/get_me.py` & `pyroblack-2.3.60/pyrogram/methods/users/get_me.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/users/get_peer_stories.py` & `pyroblack-2.3.60/pyrogram/methods/users/get_peer_stories.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/users/get_stories.py` & `pyroblack-2.3.60/pyrogram/methods/users/get_stories.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/users/get_stories_history.py` & `pyroblack-2.3.60/pyrogram/methods/users/get_stories_history.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/users/get_users.py` & `pyroblack-2.3.60/pyrogram/methods/users/get_users.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/users/send_story.py` & `pyroblack-2.3.60/pyrogram/methods/users/send_story.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/users/set_emoji_status.py` & `pyroblack-2.3.60/pyrogram/methods/users/set_emoji_status.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/users/set_profile_photo.py` & `pyroblack-2.3.60/pyrogram/methods/users/set_profile_photo.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,26 +12,27 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
-from typing import Union, BinaryIO
+from typing import Union, BinaryIO, Optional
 
 import pyrogram
 from pyrogram import raw
 
 
 class SetProfilePhoto:
     async def set_profile_photo(
         self: "pyrogram.Client",
         *,
-        photo: Union[str, BinaryIO] = None,
-        video: Union[str, BinaryIO] = None,
+        photo: Optional[Union[str, BinaryIO]] = None,
+        video: Optional[Union[str, BinaryIO]] = None,
+        is_public: Optional[bool] = None
     ) -> bool:
         """Set a new profile photo or video (H.264/MPEG-4 AVC video, max 5 seconds).
 
         The ``photo`` and ``video`` arguments are mutually exclusive.
         Pass either one as named argument (see examples below).
 
         .. note::
@@ -48,27 +49,37 @@
                 pass a binary file-like object with its attribute ".name" set for in-memory uploads.
 
             video (``str`` | ``BinaryIO``, *optional*):
                 Profile video to set.
                 Pass a file path as string to upload a new video that exists on your local machine or
                 pass a binary file-like object with its attribute ".name" set for in-memory uploads.
 
+            is_public (``bool``, *optional*):
+                If set to True, the chosen profile photo will be shown to users that can't display
+                your main profile photo due to your privacy settings.
+                Defaults to None.
+
         Returns:
             ``bool``: True on success.
 
         Example:
             .. code-block:: python
 
                 # Set a new profile photo
                 await app.set_profile_photo(photo="new_photo.jpg")
 
                 # Set a new profile video
                 await app.set_profile_photo(video="new_video.mp4")
+
+                # Set/update your account's public profile photo
+                await app.set_profile_photo(photo="new_photo.jpg", is_public=True)
         """
 
         return bool(
             await self.invoke(
                 raw.functions.photos.UploadProfilePhoto(
-                    file=await self.save_file(photo), video=await self.save_file(video)
+                    fallback=is_public,
+                    file=await self.save_file(photo),
+                    video=await self.save_file(video)
                 )
             )
         )
```

### Comparing `pyroblack-2.3.52/pyrogram/methods/users/set_username.py` & `pyroblack-2.3.60/pyrogram/methods/users/set_username.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/users/unblock_user.py` & `pyroblack-2.3.60/pyrogram/methods/users/unblock_user.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/users/update_profile.py` & `pyroblack-2.3.60/pyrogram/methods/users/update_profile.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/utilities/__init__.py` & `pyroblack-2.3.60/pyrogram/methods/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/utilities/add_handler.py` & `pyroblack-2.3.60/pyrogram/methods/utilities/add_handler.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/utilities/compose.py` & `pyroblack-2.3.60/pyrogram/methods/utilities/compose.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/utilities/export_session_string.py` & `pyroblack-2.3.60/pyrogram/methods/utilities/export_session_string.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/utilities/idle.py` & `pyroblack-2.3.60/pyrogram/methods/utilities/idle.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/utilities/remove_handler.py` & `pyroblack-2.3.60/pyrogram/methods/utilities/remove_handler.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/utilities/restart.py` & `pyroblack-2.3.60/pyrogram/methods/utilities/restart.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/utilities/run.py` & `pyroblack-2.3.60/pyrogram/methods/utilities/run.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/utilities/run_sync.py` & `pyroblack-2.3.60/pyrogram/methods/utilities/run_sync.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/utilities/start.py` & `pyroblack-2.3.60/pyrogram/methods/utilities/start.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/utilities/stop.py` & `pyroblack-2.3.60/pyrogram/methods/utilities/stop.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/methods/utilities/stop_transmission.py` & `pyroblack-2.3.60/pyrogram/methods/utilities/stop_transmission.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/nav/__init__.py` & `pyroblack-2.3.60/pyrogram/nav/__init__.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/nav/pagination.py` & `pyroblack-2.3.60/pyrogram/nav/pagination.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/parser/__init__.py` & `pyroblack-2.3.60/pyrogram/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/parser/html.py` & `pyroblack-2.3.60/pyrogram/parser/html.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/parser/markdown.py` & `pyroblack-2.3.60/pyrogram/parser/markdown.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/parser/parser.py` & `pyroblack-2.3.60/pyrogram/parser/parser.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/parser/utils.py` & `pyroblack-2.3.60/pyrogram/parser/utils.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/raw/__init__.py` & `pyroblack-2.3.60/pyrogram/raw/__init__.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/raw/core/__init__.py` & `pyroblack-2.3.60/pyrogram/raw/core/__init__.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/raw/core/future_salt.py` & `pyroblack-2.3.60/pyrogram/raw/core/future_salt.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/raw/core/future_salts.py` & `pyroblack-2.3.60/pyrogram/raw/core/future_salts.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/raw/core/gzip_packed.py` & `pyroblack-2.3.60/pyrogram/raw/core/gzip_packed.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/raw/core/list.py` & `pyroblack-2.3.60/pyrogram/raw/core/list.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/raw/core/message.py` & `pyroblack-2.3.60/pyrogram/raw/core/message.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/raw/core/msg_container.py` & `pyroblack-2.3.60/pyrogram/raw/core/msg_container.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/raw/core/tl_object.py` & `pyroblack-2.3.60/pyrogram/raw/core/tl_object.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/raw/core/primitives/__init__.py` & `pyroblack-2.3.60/pyrogram/raw/core/primitives/__init__.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/raw/core/primitives/bool.py` & `pyroblack-2.3.60/pyrogram/raw/core/primitives/bool.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/raw/core/primitives/bytes.py` & `pyroblack-2.3.60/pyrogram/raw/core/primitives/bytes.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/raw/core/primitives/double.py` & `pyroblack-2.3.60/pyrogram/raw/core/primitives/double.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/raw/core/primitives/int.py` & `pyroblack-2.3.60/pyrogram/raw/core/primitives/int.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/raw/core/primitives/string.py` & `pyroblack-2.3.60/pyrogram/raw/core/primitives/string.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/raw/core/primitives/vector.py` & `pyroblack-2.3.60/pyrogram/raw/core/primitives/vector.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/session/__init__.py` & `pyroblack-2.3.60/pyrogram/session/__init__.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/session/auth.py` & `pyroblack-2.3.60/pyrogram/session/auth.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/session/session.py` & `pyroblack-2.3.60/pyrogram/session/session.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/session/internals/__init__.py` & `pyroblack-2.3.60/pyrogram/session/internals/__init__.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/session/internals/data_center.py` & `pyroblack-2.3.60/pyrogram/session/internals/data_center.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/session/internals/msg_factory.py` & `pyroblack-2.3.60/pyrogram/session/internals/msg_factory.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/session/internals/msg_id.py` & `pyroblack-2.3.60/pyrogram/session/internals/msg_id.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/session/internals/seq_no.py` & `pyroblack-2.3.60/pyrogram/session/internals/seq_no.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/storage/__init__.py` & `pyroblack-2.3.60/pyrogram/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/storage/dummy_client.py` & `pyroblack-2.3.60/pyrogram/storage/dummy_client.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/storage/file_storage.py` & `pyroblack-2.3.60/pyrogram/storage/file_storage.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/storage/memory_storage.py` & `pyroblack-2.3.60/pyrogram/storage/memory_storage.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/storage/mongo_storage.py` & `pyroblack-2.3.60/pyrogram/storage/mongo_storage.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/storage/sqlite_storage.py` & `pyroblack-2.3.60/pyrogram/storage/sqlite_storage.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/storage/storage.py` & `pyroblack-2.3.60/pyrogram/storage/storage.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/__init__.py` & `pyroblack-2.3.60/pyrogram/types/__init__.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/list.py` & `pyroblack-2.3.60/pyrogram/types/list.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/object.py` & `pyroblack-2.3.60/pyrogram/types/object.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/update.py` & `pyroblack-2.3.60/pyrogram/types/update.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/authorization/__init__.py` & `pyroblack-2.3.60/pyrogram/types/authorization/__init__.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/authorization/sent_code.py` & `pyroblack-2.3.60/pyrogram/types/authorization/sent_code.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/authorization/terms_of_service.py` & `pyroblack-2.3.60/pyrogram/types/authorization/terms_of_service.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/bots_and_keyboards/__init__.py` & `pyroblack-2.3.60/pyrogram/types/bots_and_keyboards/__init__.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/bots_and_keyboards/bot_command.py` & `pyroblack-2.3.60/pyrogram/types/bots_and_keyboards/bot_command.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/bots_and_keyboards/bot_command_scope.py` & `pyroblack-2.3.60/pyrogram/types/bots_and_keyboards/bot_command_scope.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/bots_and_keyboards/bot_command_scope_all_chat_administrators.py` & `pyroblack-2.3.60/pyrogram/types/bots_and_keyboards/bot_command_scope_all_chat_administrators.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/bots_and_keyboards/bot_command_scope_all_group_chats.py` & `pyroblack-2.3.60/pyrogram/types/bots_and_keyboards/bot_command_scope_all_group_chats.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/bots_and_keyboards/bot_command_scope_all_private_chats.py` & `pyroblack-2.3.60/pyrogram/types/bots_and_keyboards/bot_command_scope_all_private_chats.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/bots_and_keyboards/bot_command_scope_chat.py` & `pyroblack-2.3.60/pyrogram/types/bots_and_keyboards/bot_command_scope_chat.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_administrators.py` & `pyroblack-2.3.60/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_administrators.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_member.py` & `pyroblack-2.3.60/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_member.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/bots_and_keyboards/bot_command_scope_default.py` & `pyroblack-2.3.60/pyrogram/types/bots_and_keyboards/bot_command_scope_default.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/bots_and_keyboards/bot_info.py` & `pyroblack-2.3.60/pyrogram/types/bots_and_keyboards/bot_info.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/bots_and_keyboards/callback_game.py` & `pyroblack-2.3.60/pyrogram/types/bots_and_keyboards/callback_game.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/bots_and_keyboards/callback_query.py` & `pyroblack-2.3.60/pyrogram/types/bots_and_keyboards/callback_query.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/bots_and_keyboards/force_reply.py` & `pyroblack-2.3.60/pyrogram/types/bots_and_keyboards/force_reply.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/bots_and_keyboards/game_high_score.py` & `pyroblack-2.3.60/pyrogram/types/bots_and_keyboards/game_high_score.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/bots_and_keyboards/inline_keyboard_button.py` & `pyroblack-2.3.60/pyrogram/types/bots_and_keyboards/inline_keyboard_button.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/bots_and_keyboards/inline_keyboard_markup.py` & `pyroblack-2.3.60/pyrogram/types/bots_and_keyboards/inline_keyboard_markup.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/bots_and_keyboards/keyboard_button.py` & `pyroblack-2.3.60/pyrogram/types/bots_and_keyboards/keyboard_button.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/bots_and_keyboards/login_url.py` & `pyroblack-2.3.60/pyrogram/types/bots_and_keyboards/login_url.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/bots_and_keyboards/menu_button.py` & `pyroblack-2.3.60/pyrogram/types/bots_and_keyboards/menu_button.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/bots_and_keyboards/menu_button_commands.py` & `pyroblack-2.3.60/pyrogram/types/bots_and_keyboards/menu_button_commands.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/bots_and_keyboards/menu_button_default.py` & `pyroblack-2.3.60/pyrogram/types/bots_and_keyboards/menu_button_default.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/bots_and_keyboards/menu_button_web_app.py` & `pyroblack-2.3.60/pyrogram/types/bots_and_keyboards/menu_button_web_app.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/bots_and_keyboards/reply_keyboard_markup.py` & `pyroblack-2.3.60/pyrogram/types/bots_and_keyboards/reply_keyboard_markup.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/bots_and_keyboards/reply_keyboard_remove.py` & `pyroblack-2.3.60/pyrogram/types/bots_and_keyboards/reply_keyboard_remove.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/bots_and_keyboards/request_peer_type_channel.py` & `pyroblack-2.3.60/pyrogram/types/bots_and_keyboards/request_peer_type_channel.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/bots_and_keyboards/request_peer_type_chat.py` & `pyroblack-2.3.60/pyrogram/types/bots_and_keyboards/request_peer_type_chat.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/bots_and_keyboards/request_peer_type_user.py` & `pyroblack-2.3.60/pyrogram/types/bots_and_keyboards/request_peer_type_user.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/bots_and_keyboards/requested_chats.py` & `pyroblack-2.3.60/pyrogram/types/bots_and_keyboards/requested_chats.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/bots_and_keyboards/sent_web_app_message.py` & `pyroblack-2.3.60/pyrogram/types/bots_and_keyboards/sent_web_app_message.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/bots_and_keyboards/web_app_info.py` & `pyroblack-2.3.60/pyrogram/types/bots_and_keyboards/web_app_info.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/inline_mode/__init__.py` & `pyroblack-2.3.60/pyrogram/types/inline_mode/__init__.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/inline_mode/chosen_inline_result.py` & `pyroblack-2.3.60/pyrogram/types/inline_mode/chosen_inline_result.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/inline_mode/inline_query.py` & `pyroblack-2.3.60/pyrogram/types/inline_mode/inline_query.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/inline_mode/inline_query_result.py` & `pyroblack-2.3.60/pyrogram/types/inline_mode/inline_query_result.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/inline_mode/inline_query_result_animation.py` & `pyroblack-2.3.60/pyrogram/types/inline_mode/inline_query_result_animation.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/inline_mode/inline_query_result_article.py` & `pyroblack-2.3.60/pyrogram/types/inline_mode/inline_query_result_article.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/inline_mode/inline_query_result_audio.py` & `pyroblack-2.3.60/pyrogram/types/inline_mode/inline_query_result_audio.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/inline_mode/inline_query_result_cached_animation.py` & `pyroblack-2.3.60/pyrogram/types/inline_mode/inline_query_result_cached_animation.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/inline_mode/inline_query_result_cached_audio.py` & `pyroblack-2.3.60/pyrogram/types/inline_mode/inline_query_result_cached_audio.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/inline_mode/inline_query_result_cached_document.py` & `pyroblack-2.3.60/pyrogram/types/inline_mode/inline_query_result_cached_document.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/inline_mode/inline_query_result_cached_photo.py` & `pyroblack-2.3.60/pyrogram/types/inline_mode/inline_query_result_cached_photo.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/inline_mode/inline_query_result_cached_sticker.py` & `pyroblack-2.3.60/pyrogram/types/inline_mode/inline_query_result_cached_sticker.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/inline_mode/inline_query_result_cached_video.py` & `pyroblack-2.3.60/pyrogram/types/inline_mode/inline_query_result_cached_video.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/inline_mode/inline_query_result_cached_voice.py` & `pyroblack-2.3.60/pyrogram/types/inline_mode/inline_query_result_cached_voice.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/inline_mode/inline_query_result_contact.py` & `pyroblack-2.3.60/pyrogram/types/inline_mode/inline_query_result_contact.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/inline_mode/inline_query_result_document.py` & `pyroblack-2.3.60/pyrogram/types/inline_mode/inline_query_result_document.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/inline_mode/inline_query_result_location.py` & `pyroblack-2.3.60/pyrogram/types/inline_mode/inline_query_result_location.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/inline_mode/inline_query_result_photo.py` & `pyroblack-2.3.60/pyrogram/types/inline_mode/inline_query_result_photo.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/inline_mode/inline_query_result_venue.py` & `pyroblack-2.3.60/pyrogram/types/inline_mode/inline_query_result_venue.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/inline_mode/inline_query_result_video.py` & `pyroblack-2.3.60/pyrogram/types/inline_mode/inline_query_result_video.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/inline_mode/inline_query_result_voice.py` & `pyroblack-2.3.60/pyrogram/types/inline_mode/inline_query_result_voice.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/input_media/__init__.py` & `pyroblack-2.3.60/pyrogram/types/input_media/__init__.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/input_media/input_media.py` & `pyroblack-2.3.60/pyrogram/types/input_media/input_media.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/input_media/input_media_animation.py` & `pyroblack-2.3.60/pyrogram/types/input_media/input_media_animation.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/input_media/input_media_area.py` & `pyroblack-2.3.60/pyrogram/types/input_media/input_media_area.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/input_media/input_media_area_channel_post.py` & `pyroblack-2.3.60/pyrogram/types/input_media/input_media_area_channel_post.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/input_media/input_media_audio.py` & `pyroblack-2.3.60/pyrogram/types/input_media/input_media_audio.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/input_media/input_media_document.py` & `pyroblack-2.3.60/pyrogram/types/input_media/input_media_document.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/input_media/input_media_photo.py` & `pyroblack-2.3.60/pyrogram/types/input_media/input_media_photo.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/input_media/input_media_video.py` & `pyroblack-2.3.60/pyrogram/types/input_media/input_media_video.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/input_media/input_phone_contact.py` & `pyroblack-2.3.60/pyrogram/types/input_media/input_phone_contact.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/input_message_content/__init__.py` & `pyroblack-2.3.60/pyrogram/types/input_message_content/__init__.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/input_message_content/input_message_content.py` & `pyroblack-2.3.60/pyrogram/types/input_message_content/input_message_content.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/input_message_content/input_reply_to_message.py` & `pyroblack-2.3.60/pyrogram/types/input_message_content/input_reply_to_message.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/input_message_content/input_reply_to_story.py` & `pyroblack-2.3.60/pyrogram/types/input_message_content/input_reply_to_story.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/input_message_content/input_text_message_content.py` & `pyroblack-2.3.60/pyrogram/types/input_message_content/input_text_message_content.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/messages_and_media/__init__.py` & `pyroblack-2.3.60/pyrogram/types/messages_and_media/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with pyroblack.  If not, see <http://www.gnu.org/licenses/>.
 
 from .animation import Animation
 from .audio import Audio
+from .checked_gift_code import CheckedGiftCode
 from .contact import Contact
 from .dice import Dice
 from .document import Document
 from .exported_story_link import ExportedStoryLink
 from .game import Game
 from .giveaway import Giveaway
 from .giveaway_launched import GiveawayLaunched
@@ -63,14 +64,15 @@
 from .web_page import WebPage
 from .web_page_empty import WebPageEmpty
 from .web_page_preview import WebPagePreview
 
 __all__ = [
     "Animation",
     "Audio",
+    "CheckedGiftCode",
     "Contact",
     "Document",
     "Game",
     "Giveaway",
     "GiveawayLaunched",
     "GiveawayResult",
     "Location",
```

### Comparing `pyroblack-2.3.52/pyrogram/types/messages_and_media/animation.py` & `pyroblack-2.3.60/pyrogram/types/messages_and_media/animation.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/messages_and_media/audio.py` & `pyroblack-2.3.60/pyrogram/types/messages_and_media/audio.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/messages_and_media/contact.py` & `pyroblack-2.3.60/pyrogram/types/messages_and_media/contact.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/messages_and_media/dice.py` & `pyroblack-2.3.60/pyrogram/types/messages_and_media/dice.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/messages_and_media/document.py` & `pyroblack-2.3.60/pyrogram/types/messages_and_media/document.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/messages_and_media/exported_story_link.py` & `pyroblack-2.3.60/pyrogram/types/messages_and_media/exported_story_link.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/messages_and_media/game.py` & `pyroblack-2.3.60/pyrogram/types/messages_and_media/game.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/messages_and_media/gift_code.py` & `pyroblack-2.3.60/pyrogram/types/messages_and_media/gift_code.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,26 +24,29 @@
     """Contains gift code data.
 
     Parameters:
         via_giveaway (``bool``):
             True if the gift code is received via giveaway.
 
         unclaimed (``bool``):
-            True if the gift code is unclaimed.
+            True if the winner for the corresponding Telegram Premium subscription wasn't chosen.
 
         boost_peer (:obj:`~pyrogram.types.Chat`):
             The channel where the gift code was won.
 
         months (``int``):
             Number of months of subscription.
 
         slug (``str``):
             Identifier of gift code.
             You can combine it with `t.me/giftcode/{slug}`
             to get link for this gift.
+
+        link (``str``, *property*):
+            Generate a link to this gift code.
     """
 
     def __init__(
         self, *, via_giveaway: bool, unclaimed: bool, boost_peer, months: int, slug: str
     ):
         super().__init__()
 
@@ -51,15 +54,15 @@
         self.unclaimed = unclaimed
         self.boost_peer = boost_peer
         self.months = months
         self.slug = slug
 
     @staticmethod
     def _parse(client, giftcode: "raw.types.MessageActionGiftCode", chats):
-        peer = chats.get(utils.get_raw_peer_id(giftcode.boost_peer))
+        peer = chats.get(utils.get_raw_peer_id(getattr(giftcode, "boost_peer")))
 
         return GiftCode(
             via_giveaway=giftcode.via_giveaway,
             unclaimed=giftcode.unclaimed,
             boost_peer=types.Chat._parse_chat(client, peer) if peer else None,
             months=giftcode.months,
             slug=giftcode.slug,
```

### Comparing `pyroblack-2.3.52/pyrogram/types/messages_and_media/giveaway.py` & `pyroblack-2.3.60/pyrogram/types/messages_and_media/giveaway.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/messages_and_media/giveaway_launched.py` & `pyroblack-2.3.60/pyrogram/types/messages_and_media/giveaway_launched.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/messages_and_media/giveaway_result.py` & `pyroblack-2.3.60/pyrogram/types/messages_and_media/giveaway_result.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/messages_and_media/location.py` & `pyroblack-2.3.60/pyrogram/types/messages_and_media/location.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/messages_and_media/media_area.py` & `pyroblack-2.3.60/pyrogram/types/messages_and_media/media_area.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/messages_and_media/media_area_channel_post.py` & `pyroblack-2.3.60/pyrogram/types/messages_and_media/media_area_channel_post.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/messages_and_media/media_area_coordinates.py` & `pyroblack-2.3.60/pyrogram/types/messages_and_media/media_area_coordinates.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/messages_and_media/message.py` & `pyroblack-2.3.60/pyrogram/types/messages_and_media/message.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/messages_and_media/message_entity.py` & `pyroblack-2.3.60/pyrogram/types/messages_and_media/message_entity.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/messages_and_media/message_reaction_count_updated.py` & `pyroblack-2.3.60/pyrogram/types/messages_and_media/message_reaction_count_updated.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/messages_and_media/message_reaction_updated.py` & `pyroblack-2.3.60/pyrogram/types/messages_and_media/message_reaction_updated.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/messages_and_media/message_reactions.py` & `pyroblack-2.3.60/pyrogram/types/messages_and_media/message_reactions.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/messages_and_media/message_story.py` & `pyroblack-2.3.60/pyrogram/types/messages_and_media/message_story.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/messages_and_media/photo.py` & `pyroblack-2.3.60/pyrogram/types/messages_and_media/photo.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/messages_and_media/poll.py` & `pyroblack-2.3.60/pyrogram/types/messages_and_media/poll.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/messages_and_media/poll_option.py` & `pyroblack-2.3.60/pyrogram/types/messages_and_media/poll_option.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/messages_and_media/reaction.py` & `pyroblack-2.3.60/pyrogram/types/messages_and_media/reaction.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/messages_and_media/reaction_count.py` & `pyroblack-2.3.60/pyrogram/types/messages_and_media/reaction_count.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/messages_and_media/reaction_type.py` & `pyroblack-2.3.60/pyrogram/types/messages_and_media/reaction_type.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/messages_and_media/sticker.py` & `pyroblack-2.3.60/pyrogram/types/messages_and_media/sticker.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/messages_and_media/stickerset.py` & `pyroblack-2.3.60/pyrogram/types/messages_and_media/stickerset.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/messages_and_media/stories_privacy_rules.py` & `pyroblack-2.3.60/pyrogram/types/messages_and_media/stories_privacy_rules.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/messages_and_media/story.py` & `pyroblack-2.3.60/pyrogram/types/messages_and_media/story.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/messages_and_media/story_deleted.py` & `pyroblack-2.3.60/pyrogram/types/messages_and_media/story_deleted.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/messages_and_media/story_forward_header.py` & `pyroblack-2.3.60/pyrogram/types/messages_and_media/story_forward_header.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/messages_and_media/story_skipped.py` & `pyroblack-2.3.60/pyrogram/types/messages_and_media/story_skipped.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/messages_and_media/story_views.py` & `pyroblack-2.3.60/pyrogram/types/messages_and_media/story_views.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/messages_and_media/stripped_thumbnail.py` & `pyroblack-2.3.60/pyrogram/types/messages_and_media/stripped_thumbnail.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/messages_and_media/thumbnail.py` & `pyroblack-2.3.60/pyrogram/types/messages_and_media/thumbnail.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/messages_and_media/venue.py` & `pyroblack-2.3.60/pyrogram/types/messages_and_media/venue.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/messages_and_media/video.py` & `pyroblack-2.3.60/pyrogram/types/messages_and_media/video.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/messages_and_media/video_note.py` & `pyroblack-2.3.60/pyrogram/types/messages_and_media/video_note.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/messages_and_media/voice.py` & `pyroblack-2.3.60/pyrogram/types/messages_and_media/voice.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/messages_and_media/web_app_data.py` & `pyroblack-2.3.60/pyrogram/types/messages_and_media/web_app_data.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/messages_and_media/web_page.py` & `pyroblack-2.3.60/pyrogram/types/messages_and_media/web_page.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/messages_and_media/web_page_empty.py` & `pyroblack-2.3.60/pyrogram/types/messages_and_media/web_page_empty.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/messages_and_media/web_page_preview.py` & `pyroblack-2.3.60/pyrogram/types/messages_and_media/web_page_preview.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/pyromod/identifier.py` & `pyroblack-2.3.60/pyrogram/types/pyromod/identifier.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/pyromod/listener.py` & `pyroblack-2.3.60/pyrogram/types/pyromod/listener.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/user_and_chats/__init__.py` & `pyroblack-2.3.60/pyrogram/types/user_and_chats/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with pyroblack.  If not, see <http://www.gnu.org/licenses/>.
 
+from .birthday import Birthday
 from .business_info import BusinessInfo
 from .business_message import BusinessMessage
 from .business_recipients import BusinessRecipients
 from .business_weekly_open import BusinessWeeklyOpen
 from .business_working_hours import BusinessWorkingHours
 from .chat import Chat
 from .chat_admin_with_invite_links import ChatAdminWithInviteLinks
@@ -56,14 +57,15 @@
 from .username import Username
 from .video_chat_ended import VideoChatEnded
 from .video_chat_members_invited import VideoChatMembersInvited
 from .video_chat_scheduled import VideoChatScheduled
 from .video_chat_started import VideoChatStarted
 
 __all__ = [
+    "Birthday",
     "BusinessInfo",
     "BusinessMessage",
     "BusinessRecipients",
     "BusinessWeeklyOpen",
     "BusinessWorkingHours",
     "Chat",
     "ChatMember",
```

### Comparing `pyroblack-2.3.52/pyrogram/types/user_and_chats/business_info.py` & `pyroblack-2.3.60/pyrogram/types/user_and_chats/business_info.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/user_and_chats/business_message.py` & `pyroblack-2.3.60/pyrogram/types/user_and_chats/business_message.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/user_and_chats/business_recipients.py` & `pyroblack-2.3.60/pyrogram/types/user_and_chats/business_recipients.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/user_and_chats/business_weekly_open.py` & `pyroblack-2.3.60/pyrogram/types/user_and_chats/business_weekly_open.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/user_and_chats/business_working_hours.py` & `pyroblack-2.3.60/pyrogram/types/user_and_chats/business_working_hours.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/user_and_chats/chat.py` & `pyroblack-2.3.60/pyrogram/types/user_and_chats/chat.py`

 * *Files 1% similar despite different names*

```diff
@@ -181,14 +181,17 @@
             Chat reply color.
 
         profile_color (:obj:`~pyrogram.types.ChatColor`, *optional*):
             Chat profile color.
 
         business_info (:obj:`~pyrogram.types.BusinessInfo`, *optional*):
             Business information of a chat.
+
+        birthday (:obj:`~pyrogram.types.Birthday`, *optional*):
+            Information about user birthday.
     """
 
     def __init__(
         self,
         *,
         client: "pyrogram.Client" = None,
         id: int,
@@ -229,14 +232,15 @@
         linked_chat: "types.Chat" = None,
         send_as_chat: "types.Chat" = None,
         available_reactions: Optional["types.ChatReactions"] = None,
         usernames: List["types.Username"] = None,
         reply_color: "types.ChatColor" = None,
         profile_color: "types.ChatColor" = None,
         business_info: "types.BusinessInfo" = None,
+        birthday: "types.Birthday" = None
     ):
         super().__init__(client)
 
         self.id = id
         self.type = type
         self.is_verified = is_verified
         self.is_restricted = is_restricted
@@ -274,14 +278,15 @@
         self.linked_chat = linked_chat
         self.send_as_chat = send_as_chat
         self.available_reactions = available_reactions
         self.usernames = usernames
         self.reply_color = reply_color
         self.profile_color = profile_color
         self.business_info = business_info
+        self.birthday = birthday
 
     @property
     def full_name(self) -> str:
         return (
             " ".join(filter(None, [self.first_name, self.last_name]))
             or self.title
             or None
@@ -440,17 +445,16 @@
 
         if isinstance(chat_full, raw.types.users.UserFull):
             full_user = chat_full.full_user
 
             parsed_chat = Chat._parse_user_chat(client, users[full_user.id])
             parsed_chat.bio = full_user.about
             parsed_chat.folder_id = getattr(full_user, "folder_id", None)
-            parsed_chat.business_info = types.BusinessInfo._parse(
-                client, full_user, users
-            )
+            parsed_chat.business_info = types.BusinessInfo._parse(client, full_user, users)
+            parsed_chat.birthday = types.Birthday._parse(getattr(full_user, "birthday", None))
 
             if full_user.pinned_msg_id:
                 try:
                     parsed_chat.pinned_message = await client.get_messages(
                         chat_id=parsed_chat.id, message_ids=full_user.pinned_msg_id
                     )
                 except MessageIdsEmpty:
```

### Comparing `pyroblack-2.3.52/pyrogram/types/user_and_chats/chat_admin_with_invite_links.py` & `pyroblack-2.3.60/pyrogram/types/user_and_chats/chat_admin_with_invite_links.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/user_and_chats/chat_color.py` & `pyroblack-2.3.60/pyrogram/types/user_and_chats/chat_color.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/user_and_chats/chat_event.py` & `pyroblack-2.3.60/pyrogram/types/user_and_chats/chat_event.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/user_and_chats/chat_event_filter.py` & `pyroblack-2.3.60/pyrogram/types/user_and_chats/chat_event_filter.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/user_and_chats/chat_invite_link.py` & `pyroblack-2.3.60/pyrogram/types/user_and_chats/chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/user_and_chats/chat_join_request.py` & `pyroblack-2.3.60/pyrogram/types/user_and_chats/chat_join_request.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/user_and_chats/chat_joined_by_request.py` & `pyroblack-2.3.60/pyrogram/types/user_and_chats/chat_joined_by_request.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/user_and_chats/chat_joiner.py` & `pyroblack-2.3.60/pyrogram/types/user_and_chats/chat_joiner.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/user_and_chats/chat_member.py` & `pyroblack-2.3.60/pyrogram/types/user_and_chats/chat_member.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/user_and_chats/chat_member_updated.py` & `pyroblack-2.3.60/pyrogram/types/user_and_chats/chat_member_updated.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/user_and_chats/chat_permissions.py` & `pyroblack-2.3.60/pyrogram/types/user_and_chats/chat_permissions.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/user_and_chats/chat_photo.py` & `pyroblack-2.3.60/pyrogram/types/user_and_chats/chat_photo.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/user_and_chats/chat_preview.py` & `pyroblack-2.3.60/pyrogram/types/user_and_chats/chat_preview.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/user_and_chats/chat_privileges.py` & `pyroblack-2.3.60/pyrogram/types/user_and_chats/chat_privileges.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/user_and_chats/chat_reactions.py` & `pyroblack-2.3.60/pyrogram/types/user_and_chats/chat_reactions.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/user_and_chats/dialog.py` & `pyroblack-2.3.60/pyrogram/types/user_and_chats/dialog.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/user_and_chats/emoji_status.py` & `pyroblack-2.3.60/pyrogram/types/user_and_chats/emoji_status.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/user_and_chats/forum_topic.py` & `pyroblack-2.3.60/pyrogram/types/user_and_chats/forum_topic.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/user_and_chats/forum_topic_closed.py` & `pyroblack-2.3.60/pyrogram/types/user_and_chats/forum_topic_closed.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/user_and_chats/forum_topic_created.py` & `pyroblack-2.3.60/pyrogram/types/user_and_chats/forum_topic_created.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/user_and_chats/forum_topic_edited.py` & `pyroblack-2.3.60/pyrogram/types/user_and_chats/forum_topic_edited.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/user_and_chats/forum_topic_reopened.py` & `pyroblack-2.3.60/pyrogram/types/user_and_chats/forum_topic_reopened.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/user_and_chats/general_forum_topic_hidden.py` & `pyroblack-2.3.60/pyrogram/types/user_and_chats/general_forum_topic_hidden.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/user_and_chats/general_forum_topic_unhidden.py` & `pyroblack-2.3.60/pyrogram/types/user_and_chats/general_forum_topic_unhidden.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/user_and_chats/invite_link_importer.py` & `pyroblack-2.3.60/pyrogram/types/user_and_chats/invite_link_importer.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/user_and_chats/peer_channel.py` & `pyroblack-2.3.60/pyrogram/types/user_and_chats/peer_channel.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/user_and_chats/peer_user.py` & `pyroblack-2.3.60/pyrogram/types/user_and_chats/peer_user.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/user_and_chats/restriction.py` & `pyroblack-2.3.60/pyrogram/types/user_and_chats/restriction.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/user_and_chats/user.py` & `pyroblack-2.3.60/pyrogram/types/user_and_chats/user.py`

 * *Files 1% similar despite different names*

```diff
@@ -154,18 +154,18 @@
 
         mention (``str``, *property*):
             Generate a text mention for this user.
             You can use ``user.mention()`` to mention the user using their first name (styled using html), or
             ``user.mention("another name")`` for a custom name. To choose a different style
             ("html" or "md"/"markdown") use ``user.mention(style="md")``.
 
-        reply_color (:obj:`~pyrogram.types.ChatColor`, *optional*)
+        reply_color (:obj:`~pyrogram.types.ChatColor`, *optional*):
             Chat reply color.
 
-        profile_color (:obj:`~pyrogram.types.ChatColor`, *optional*)
+        profile_color (:obj:`~pyrogram.types.ChatColor`, *optional*):
             Chat profile color.
     """
 
     def __init__(
         self,
         *,
         client: "pyrogram.Client" = None,
```

### Comparing `pyroblack-2.3.52/pyrogram/types/user_and_chats/username.py` & `pyroblack-2.3.60/pyrogram/types/user_and_chats/username.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/user_and_chats/video_chat_ended.py` & `pyroblack-2.3.60/pyrogram/types/user_and_chats/video_chat_ended.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/user_and_chats/video_chat_members_invited.py` & `pyroblack-2.3.60/pyrogram/types/user_and_chats/video_chat_members_invited.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/user_and_chats/video_chat_scheduled.py` & `pyroblack-2.3.60/pyrogram/types/user_and_chats/video_chat_scheduled.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyrogram/types/user_and_chats/video_chat_started.py` & `pyroblack-2.3.60/pyrogram/types/user_and_chats/video_chat_started.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/.gitignore` & `pyroblack-2.3.60/.gitignore`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/COPYING` & `pyroblack-2.3.60/COPYING`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/COPYING.lesser` & `pyroblack-2.3.60/COPYING.lesser`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/NOTICE` & `pyroblack-2.3.60/NOTICE`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/README.md` & `pyroblack-2.3.60/README.md`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/hatch_build.py` & `pyroblack-2.3.60/hatch_build.py`

 * *Files identical despite different names*

### Comparing `pyroblack-2.3.52/pyproject.toml` & `pyroblack-2.3.60/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [project]
 name = "pyroblack"
 dynamic = ["version"]
 description = "Pyrogram, but black. Elegant, modern and asynchronous Telegram MTProto API framework in Python for users and bots"
 authors = [{ name = "eyMarv", email = "eyMarv07@gmail.com" }]
-dependencies = ["aiosqlite>=0.19.0", "pyaes==1.6.1", "pysocks==1.7.1", "pymediainfo-pyroblack>=6.0.1,<7.0.0"]
+dependencies = ["aiosqlite-black>=0.21.0", "pyaes==1.6.1", "pysocks==1.7.1", "pymediainfo-pyroblack>=6.1.1,<7.0.0"]
 readme = "README.md"
 license = "LGPL-3.0-or-later"
 requires-python = "~=3.8"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "Natural Language :: English",
@@ -26,15 +26,15 @@
     "Topic :: Internet",
     "Topic :: Communications",
     "Topic :: Communications :: Chat",
     "Topic :: Software Development :: Libraries",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: Software Development :: Libraries :: Application Frameworks",
 ]
-keywords = ["telegram chat messenger mtproto api client library python"]
+keywords = ["black bsxcs telegram chat messenger mtproto api client library python"]
 
 [tool.hatch.version]
 path = "pyrogram/__init__.py"
 
 # Used to call hatch_build.py
 [tool.hatch.build.hooks.custom]
 
@@ -62,15 +62,15 @@
     "sphinx-immaterial==0.11.11",
     "sphinx_copybutton",
     "sphinx-autobuild",
     "tornado>=6.3.3"
 ]
 
 speedup = [
-    "tgcrypto-pyroblack>=1.2.5",
+    "tgcrypto-pyroblack>=1.2.6",
     "uvloop>=0.19.0"
 ]
 
 [tool.hatch.metadata]
 allow-direct-references = true
 
 [tool.hatch.build.targets.sdist]
```

### Comparing `pyroblack-2.3.52/PKG-INFO` & `pyroblack-2.3.60/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.3
 Name: pyroblack
-Version: 2.3.52
+Version: 2.3.60
 Summary: Pyrogram, but black. Elegant, modern and asynchronous Telegram MTProto API framework in Python for users and bots
 Project-URL: Tracker, https://github.com/eyMarv/pyroblack/issues
 Project-URL: Community, https://t.me/OpenFileZ
 Project-URL: Source, https://github.com/eyMarv/pyroblack
 Project-URL: Documentation, https://eyMarv.github.io/pyroblack-docs
 Author-email: eyMarv <eyMarv07@gmail.com>
 License-Expression: LGPL-3.0-or-later
 License-File: COPYING
 License-File: COPYING.lesser
 License-File: NOTICE
-Keywords: telegram chat messenger mtproto api client library python
+Keywords: black bsxcs telegram chat messenger mtproto api client library python
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -30,32 +30,32 @@
 Classifier: Topic :: Communications
 Classifier: Topic :: Communications :: Chat
 Classifier: Topic :: Internet
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: ~=3.8
-Requires-Dist: aiosqlite>=0.19.0
+Requires-Dist: aiosqlite-black>=0.21.0
 Requires-Dist: pyaes==1.6.1
-Requires-Dist: pymediainfo-pyroblack<7.0.0,>=6.0.1
+Requires-Dist: pymediainfo-pyroblack<7.0.0,>=6.1.1
 Requires-Dist: pysocks==1.7.1
 Provides-Extra: dev
 Requires-Dist: hatch>=1.7.0; extra == 'dev'
 Requires-Dist: pytest-asyncio>=0.21.1; extra == 'dev'
 Requires-Dist: pytest-cov>=4.1.0; extra == 'dev'
 Requires-Dist: pytest>=7.4.3; extra == 'dev'
 Requires-Dist: twine>=4.0.2; extra == 'dev'
 Provides-Extra: docs
 Requires-Dist: sphinx; extra == 'docs'
 Requires-Dist: sphinx-autobuild; extra == 'docs'
 Requires-Dist: sphinx-copybutton; extra == 'docs'
 Requires-Dist: sphinx-immaterial==0.11.11; extra == 'docs'
 Requires-Dist: tornado>=6.3.3; extra == 'docs'
 Provides-Extra: speedup
-Requires-Dist: tgcrypto-pyroblack>=1.2.5; extra == 'speedup'
+Requires-Dist: tgcrypto-pyroblack>=1.2.6; extra == 'speedup'
 Requires-Dist: uvloop>=0.19.0; extra == 'speedup'
 Description-Content-Type: text/markdown
 
 <p align="center">
     <a href="https://github.com/eyMarv/pyroblack">
         <img src="https://eyMarv.github.io/pyroblack-docs/main/_static/pyroblack.png" alt="pyroblack" width="128">
     </a>
```

#### html2text {}

```diff
@@ -1,41 +1,41 @@
-Metadata-Version: 2.3 Name: pyroblack Version: 2.3.52 Summary: Pyrogram, but
+Metadata-Version: 2.3 Name: pyroblack Version: 2.3.60 Summary: Pyrogram, but
 black. Elegant, modern and asynchronous Telegram MTProto API framework in
 Python for users and bots Project-URL: Tracker, https://github.com/eyMarv/
 pyroblack/issues Project-URL: Community, https://t.me/OpenFileZ Project-URL:
 Source, https://github.com/eyMarv/pyroblack Project-URL: Documentation, https:/
 /eyMarv.github.io/pyroblack-docs Author-email: eyMarv
 gmail.com> License-Expression: LGPL-3.0-or-later License-File: COPYING License-
-File: COPYING.lesser License-File: NOTICE Keywords: telegram chat messenger
-mtproto api client library python Classifier: Development Status :: 5 -
-Production/Stable Classifier: Intended Audience :: Developers Classifier:
+File: COPYING.lesser License-File: NOTICE Keywords: black bsxcs telegram chat
+messenger mtproto api client library python Classifier: Development Status :: 5
+- Production/Stable Classifier: Intended Audience :: Developers Classifier:
 License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Natural Language :: English Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12 Classifier: Programming
 Language :: Python :: Implementation Classifier: Programming Language :: Python
 :: Implementation :: CPython Classifier: Programming Language :: Python ::
 Implementation :: PyPy Classifier: Topic :: Communications Classifier: Topic ::
 Communications :: Chat Classifier: Topic :: Internet Classifier: Topic ::
 Software Development :: Libraries Classifier: Topic :: Software Development ::
 Libraries :: Application Frameworks Classifier: Topic :: Software Development
-:: Libraries :: Python Modules Requires-Python: ~=3.8 Requires-Dist:
-aiosqlite>=0.19.0 Requires-Dist: pyaes==1.6.1 Requires-Dist: pymediainfo-
-pyroblack<7.0.0,>=6.0.1 Requires-Dist: pysocks==1.7.1 Provides-Extra: dev
+:: Libraries :: Python Modules Requires-Python: ~=3.8 Requires-Dist: aiosqlite-
+black>=0.21.0 Requires-Dist: pyaes==1.6.1 Requires-Dist: pymediainfo-
+pyroblack<7.0.0,>=6.1.1 Requires-Dist: pysocks==1.7.1 Provides-Extra: dev
 Requires-Dist: hatch>=1.7.0; extra == 'dev' Requires-Dist: pytest-
 asyncio>=0.21.1; extra == 'dev' Requires-Dist: pytest-cov>=4.1.0; extra ==
 'dev' Requires-Dist: pytest>=7.4.3; extra == 'dev' Requires-Dist: twine>=4.0.2;
 extra == 'dev' Provides-Extra: docs Requires-Dist: sphinx; extra == 'docs'
 Requires-Dist: sphinx-autobuild; extra == 'docs' Requires-Dist: sphinx-
 copybutton; extra == 'docs' Requires-Dist: sphinx-immaterial==0.11.11; extra ==
 'docs' Requires-Dist: tornado>=6.3.3; extra == 'docs' Provides-Extra: speedup
-Requires-Dist: tgcrypto-pyroblack>=1.2.5; extra == 'speedup' Requires-Dist:
+Requires-Dist: tgcrypto-pyroblack>=1.2.6; extra == 'speedup' Requires-Dist:
 uvloop>=0.19.0; extra == 'speedup' Description-Content-Type: text/markdown
                                   _[_p_y_r_o_b_l_a_c_k_]
                   TTeelleeggrraamm MMTTPPrroottoo AAPPII FFrraammeewwoorrkk ffoorr PPyytthhoonn
                      _D_o_c_u_m_e_n_t_a_t_i_o_n_ â¢ _I_s_s_u_e_s_ â¢ _S_u_p_p_o_r_t
 ## pyroblack > Elegant, modern and asynchronous Telegram MTProto API framework
 in Python for users and bots ``` python from pyrogram import Client, filters
 app = Client("my_account") @app.on_message(filters.private) async def hello
```

