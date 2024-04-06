# Comparing `tmp/plugp100-5.0.0.dev4.tar.gz` & `tmp/plugp100-5.0.0.dev5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plugp100-5.0.0.dev4.tar", last modified: Sat Apr  6 08:02:09 2024, max compression
+gzip compressed data, was "plugp100-5.0.0.dev5.tar", last modified: Sat Apr  6 11:09:28 2024, max compression
```

## Comparing `plugp100-5.0.0.dev4.tar` & `plugp100-5.0.0.dev5.tar`

### file list

```diff
@@ -1,162 +1,162 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 08:02:09.220315 plugp100-5.0.0.dev4/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-06 08:01:42.000000 plugp100-5.0.0.dev4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-06 08:01:42.000000 plugp100-5.0.0.dev4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2833 2024-04-06 08:02:09.220315 plugp100-5.0.0.dev4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2131 2024-04-06 08:01:42.000000 plugp100-5.0.0.dev4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 08:02:09.196315 plugp100-5.0.0.dev4/plugp100/
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-06 08:02:08.000000 plugp100-5.0.0.dev4/plugp100/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 08:02:09.196315 plugp100-5.0.0.dev4/plugp100/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 08:01:42.000000 plugp100-5.0.0.dev4/plugp100/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19612 2024-04-06 08:01:42.000000 plugp100-5.0.0.dev4/plugp100/api/light_effect.py
--rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-04-06 08:01:42.000000 plugp100-5.0.0.dev4/plugp100/api/light_effect_preset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 08:02:09.196315 plugp100-5.0.0.dev4/plugp100/api/requests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 08:01:42.000000 plugp100-5.0.0.dev4/plugp100/api/requests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-06 08:01:42.000000 plugp100-5.0.0.dev4/plugp100/api/requests/handshake_params.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 08:02:09.196315 plugp100-5.0.0.dev4/plugp100/api/requests/internal/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 08:01:42.000000 plugp100-5.0.0.dev4/plugp100/api/requests/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-04-06 08:01:42.000000 plugp100-5.0.0.dev4/plugp100/api/requests/internal/snowflake_id.py
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-06 08:01:42.000000 plugp100-5.0.0.dev4/plugp100/api/requests/login_device.py
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-06 08:01:42.000000 plugp100-5.0.0.dev4/plugp100/api/requests/secure_passthrough_params.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 08:02:09.200315 plugp100-5.0.0.dev4/plugp100/api/requests/set_device_info/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 08:01:42.000000 plugp100-5.0.0.dev4/plugp100/api/requests/set_device_info/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-06 08:01:42.000000 plugp100-5.0.0.dev4/plugp100/api/requests/set_device_info/play_alarm_params.py
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-06 08:01:42.000000 plugp100-5.0.0.dev4/plugp100/api/requests/set_device_info/set_light_color_info_params.py
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-06 08:01:42.000000 plugp100-5.0.0.dev4/plugp100/api/requests/set_device_info/set_light_info_params.py
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-06 08:01:42.000000 plugp100-5.0.0.dev4/plugp100/api/requests/set_device_info/set_plug_info_params.py
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-06 08:01:42.000000 plugp100-5.0.0.dev4/plugp100/api/requests/set_device_info/set_trv_info_params.py
--rw-r--r--   0 runner    (1001) docker     (127)     4288 2024-04-06 08:01:42.000000 plugp100-5.0.0.dev4/plugp100/api/requests/tapo_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-06 08:01:42.000000 plugp100-5.0.0.dev4/plugp100/api/requests/trigger_logs_params.py
--rw-r--r--   0 runner    (1001) docker     (127)     8301 2024-04-06 08:01:42.000000 plugp100-5.0.0.dev4/plugp100/api/tapo_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 08:02:09.200315 plugp100-5.0.0.dev4/plugp100/common/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 08:01:42.000000 plugp100-5.0.0.dev4/plugp100/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-06 08:01:42.000000 plugp100-5.0.0.dev4/plugp100/common/credentials.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 08:02:09.200315 plugp100-5.0.0.dev4/plugp100/common/functional/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 08:01:42.000000 plugp100-5.0.0.dev4/plugp100/common/functional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5729 2024-04-06 08:01:42.000000 plugp100-5.0.0.dev4/plugp100/common/functional/tri.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 08:02:09.200315 plugp100-5.0.0.dev4/plugp100/common/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 08:01:42.000000 plugp100-5.0.0.dev4/plugp100/common/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-06 08:01:42.000000 plugp100-5.0.0.dev4/plugp100/common/utils/http_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-06 08:01:42.000000 plugp100-5.0.0.dev4/plugp100/common/utils/json_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 08:02:09.200315 plugp100-5.0.0.dev4/plugp100/discovery/
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-06 08:01:42.000000 plugp100-5.0.0.dev4/plugp100/discovery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4036 2024-04-06 08:01:42.000000 plugp100-5.0.0.dev4/plugp100/discovery/cloud_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3022 2024-04-06 08:01:42.000000 plugp100-5.0.0.dev4/plugp100/discovery/discovered_device.py
--rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-04-06 08:01:42.000000 plugp100-5.0.0.dev4/plugp100/discovery/rsa_session.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3616 2024-04-06 08:01:42.000000 plugp100-5.0.0.dev4/plugp100/discovery/tapo_discovery.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 08:02:09.200315 plugp100-5.0.0.dev4/plugp100/encryption/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 08:01:42.000000 plugp100-5.0.0.dev4/plugp100/encryption/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-04-06 08:01:42.000000 plugp100-5.0.0.dev4/plugp100/encryption/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-04-06 08:01:42.000000 plugp100-5.0.0.dev4/plugp100/encryption/key_pair.py
--rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-04-06 08:01:42.000000 plugp100-5.0.0.dev4/plugp100/encryption/tp_link_cipher.py
--rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-04-06 08:01:42.000000 plugp100-5.0.0.dev4/plugp100/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 08:02:09.204315 plugp100-5.0.0.dev4/plugp100/new/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 08:01:42.000000 plugp100-5.0.0.dev4/plugp100/new/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 08:02:09.204315 plugp100-5.0.0.dev4/plugp100/new/child/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 08:01:42.000000 plugp100-5.0.0.dev4/plugp100/new/child/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14264 2024-04-06 08:01:42.000000 plugp100-5.0.0.dev4/plugp100/new/child/tapohubchildren.py
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-04-06 08:01:42.000000 plugp100-5.0.0.dev4/plugp100/new/child/tapostripsocket.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 08:02:09.208315 plugp100-5.0.0.dev4/plugp100/new/components/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 08:01:42.000000 plugp100-5.0.0.dev4/plugp100/new/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-04-06 08:01:42.000000 plugp100-5.0.0.dev4/plugp100/new/components/alarm_component.py
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-04-06 08:01:42.000000 plugp100-5.0.0.dev4/plugp100/new/components/battery_component.py
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-06 08:01:42.000000 plugp100-5.0.0.dev4/plugp100/new/components/device_component.py
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-06 08:01:42.000000 plugp100-5.0.0.dev4/plugp100/new/components/energy_component.py
--rw-r--r--   0 runner    (1001) docker     (127)     3971 2024-04-06 08:01:42.000000 plugp100-5.0.0.dev4/plugp100/new/components/hub_children_component.py
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-06 08:01:42.000000 plugp100-5.0.0.dev4/plugp100/new/components/humidity_component.py
--rw-r--r--   0 runner    (1001) docker     (127)     2596 2024-04-06 08:01:42.000000 plugp100-5.0.0.dev4/plugp100/new/components/light_component.py
--rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-04-06 08:01:42.000000 plugp100-5.0.0.dev4/plugp100/new/components/light_effect_component.py
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-06 08:01:42.000000 plugp100-5.0.0.dev4/plugp100/new/components/motion_sensor_component.py
--rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-04-06 08:01:42.000000 plugp100-5.0.0.dev4/plugp100/new/components/on_off_component.py
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-06 08:01:42.000000 plugp100-5.0.0.dev4/plugp100/new/components/overheat_component.py
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-06 08:01:42.000000 plugp100-5.0.0.dev4/plugp100/new/components/report_mode_component.py
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-06 08:01:42.000000 plugp100-5.0.0.dev4/plugp100/new/components/smart_door_component.py
--rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-04-06 08:01:42.000000 plugp100-5.0.0.dev4/plugp100/new/components/socket_children_component.py
--rw-r--r--   0 runner    (1001) docker     (127)      850 2024-04-06 08:01:42.000000 plugp100-5.0.0.dev4/plugp100/new/components/temperature_component.py
--rw-r--r--   0 runner    (1001) docker     (127)      946 2024-04-06 08:01:42.000000 plugp100-5.0.0.dev4/plugp100/new/components/temperature_humidity_records.py
--rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-04-06 08:01:42.000000 plugp100-5.0.0.dev4/plugp100/new/components/trigger_log_component.py
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-06 08:01:42.000000 plugp100-5.0.0.dev4/plugp100/new/components/water_leak_component.py
--rw-r--r--   0 runner    (1001) docker     (127)     4080 2024-04-06 08:01:42.000000 plugp100-5.0.0.dev4/plugp100/new/device_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-06 08:01:42.000000 plugp100-5.0.0.dev4/plugp100/new/device_type.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 08:02:09.208315 plugp100-5.0.0.dev4/plugp100/new/errors/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 08:01:42.000000 plugp100-5.0.0.dev4/plugp100/new/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-06 08:01:42.000000 plugp100-5.0.0.dev4/plugp100/new/errors/invalid_authentication.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 08:02:09.208315 plugp100-5.0.0.dev4/plugp100/new/event_polling/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 08:01:42.000000 plugp100-5.0.0.dev4/plugp100/new/event_polling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-04-06 08:01:42.000000 plugp100-5.0.0.dev4/plugp100/new/event_polling/event_subscription.py
--rw-r--r--   0 runner    (1001) docker     (127)     3614 2024-04-06 08:01:42.000000 plugp100-5.0.0.dev4/plugp100/new/event_polling/poll_tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-04-06 08:01:42.000000 plugp100-5.0.0.dev4/plugp100/new/event_polling/state_tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-04-06 08:01:42.000000 plugp100-5.0.0.dev4/plugp100/new/hub_device_tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)     3833 2024-04-06 08:01:42.000000 plugp100-5.0.0.dev4/plugp100/new/tapobulb.py
--rw-r--r--   0 runner    (1001) docker     (127)     5295 2024-04-06 08:01:42.000000 plugp100-5.0.0.dev4/plugp100/new/tapodevice.py
--rw-r--r--   0 runner    (1001) docker     (127)     3405 2024-04-06 08:01:42.000000 plugp100-5.0.0.dev4/plugp100/new/tapohub.py
--rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-04-06 08:01:42.000000 plugp100-5.0.0.dev4/plugp100/new/tapoplug.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 08:02:09.208315 plugp100-5.0.0.dev4/plugp100/protocol/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 08:01:42.000000 plugp100-5.0.0.dev4/plugp100/protocol/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 08:02:09.208315 plugp100-5.0.0.dev4/plugp100/protocol/klap/
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-06 08:01:42.000000 plugp100-5.0.0.dev4/plugp100/protocol/klap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-04-06 08:01:42.000000 plugp100-5.0.0.dev4/plugp100/protocol/klap/klap_handshake_revision.py
--rw-r--r--   0 runner    (1001) docker     (127)    13480 2024-04-06 08:01:42.000000 plugp100-5.0.0.dev4/plugp100/protocol/klap/klap_protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)     4168 2024-04-06 08:01:42.000000 plugp100-5.0.0.dev4/plugp100/protocol/passthrough_protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)     5294 2024-04-06 08:01:42.000000 plugp100-5.0.0.dev4/plugp100/protocol/securepassthrough_transport.py
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-04-06 08:01:42.000000 plugp100-5.0.0.dev4/plugp100/protocol/tapo_protocol.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 08:02:09.212315 plugp100-5.0.0.dev4/plugp100/responses/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 08:01:42.000000 plugp100-5.0.0.dev4/plugp100/responses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-04-06 08:01:42.000000 plugp100-5.0.0.dev4/plugp100/responses/alarm_type_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     2676 2024-04-06 08:01:42.000000 plugp100-5.0.0.dev4/plugp100/responses/child_device_list.py
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-06 08:01:42.000000 plugp100-5.0.0.dev4/plugp100/responses/components.py
--rw-r--r--   0 runner    (1001) docker     (127)     5621 2024-04-06 08:01:42.000000 plugp100-5.0.0.dev4/plugp100/responses/device_state.py
--rw-r--r--   0 runner    (1001) docker     (127)      878 2024-04-06 08:01:42.000000 plugp100-5.0.0.dev4/plugp100/responses/device_usage_info.py
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-06 08:01:42.000000 plugp100-5.0.0.dev4/plugp100/responses/energy_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 08:02:09.212315 plugp100-5.0.0.dev4/plugp100/responses/hub_childs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 08:01:42.000000 plugp100-5.0.0.dev4/plugp100/responses/hub_childs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-04-06 08:01:42.000000 plugp100-5.0.0.dev4/plugp100/responses/hub_childs/hub_child_base_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-04-06 08:01:42.000000 plugp100-5.0.0.dev4/plugp100/responses/hub_childs/ke100_device_state.py
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-06 08:01:42.000000 plugp100-5.0.0.dev4/plugp100/responses/hub_childs/leak_device_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-04-06 08:01:42.000000 plugp100-5.0.0.dev4/plugp100/responses/hub_childs/s200b_device_state.py
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-04-06 08:01:42.000000 plugp100-5.0.0.dev4/plugp100/responses/hub_childs/switch_child_device_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-04-06 08:01:42.000000 plugp100-5.0.0.dev4/plugp100/responses/hub_childs/t100_device_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-06 08:01:42.000000 plugp100-5.0.0.dev4/plugp100/responses/hub_childs/t110_device_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     2380 2024-04-06 08:01:42.000000 plugp100-5.0.0.dev4/plugp100/responses/hub_childs/t31x_device_state.py
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-06 08:01:42.000000 plugp100-5.0.0.dev4/plugp100/responses/hub_childs/trigger_log_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-06 08:01:42.000000 plugp100-5.0.0.dev4/plugp100/responses/power_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2268 2024-04-06 08:01:42.000000 plugp100-5.0.0.dev4/plugp100/responses/tapo_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)      857 2024-04-06 08:01:42.000000 plugp100-5.0.0.dev4/plugp100/responses/tapo_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-06 08:01:42.000000 plugp100-5.0.0.dev4/plugp100/responses/temperature_unit.py
--rw-r--r--   0 runner    (1001) docker     (127)      825 2024-04-06 08:01:42.000000 plugp100-5.0.0.dev4/plugp100/responses/time_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 08:02:09.216315 plugp100-5.0.0.dev4/plugp100.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2833 2024-04-06 08:02:09.000000 plugp100-5.0.0.dev4/plugp100.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5085 2024-04-06 08:02:09.000000 plugp100-5.0.0.dev4/plugp100.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 08:02:09.000000 plugp100-5.0.0.dev4/plugp100.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-06 08:02:09.000000 plugp100-5.0.0.dev4/plugp100.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-06 08:02:09.000000 plugp100-5.0.0.dev4/plugp100.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-06 08:01:42.000000 plugp100-5.0.0.dev4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-06 08:01:42.000000 plugp100-5.0.0.dev4/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-06 08:01:42.000000 plugp100-5.0.0.dev4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-06 08:02:09.220315 plugp100-5.0.0.dev4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-04-06 08:01:42.000000 plugp100-5.0.0.dev4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 08:02:09.192315 plugp100-5.0.0.dev4/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 08:02:09.216315 plugp100-5.0.0.dev4/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 08:01:42.000000 plugp100-5.0.0.dev4/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-04-06 08:01:42.000000 plugp100-5.0.0.dev4/tests/integration/tapo_test_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     2718 2024-04-06 08:01:42.000000 plugp100-5.0.0.dev4/tests/integration/test_button_t310.py
--rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-04-06 08:01:42.000000 plugp100-5.0.0.dev4/tests/integration/test_hub.py
--rw-r--r--   0 runner    (1001) docker     (127)     3139 2024-04-06 08:01:42.000000 plugp100-5.0.0.dev4/tests/integration/test_ledstrip.py
--rw-r--r--   0 runner    (1001) docker     (127)     2160 2024-04-06 08:01:42.000000 plugp100-5.0.0.dev4/tests/integration/test_light.py
--rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-04-06 08:01:42.000000 plugp100-5.0.0.dev4/tests/integration/test_plug.py
--rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-04-06 08:01:42.000000 plugp100-5.0.0.dev4/tests/integration/test_power_strip.py
--rw-r--r--   0 runner    (1001) docker     (127)     2789 2024-04-06 08:01:42.000000 plugp100-5.0.0.dev4/tests/integration/test_sensor_s200b.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3735 2024-04-06 08:01:42.000000 plugp100-5.0.0.dev4/tests/integration/test_tapo_discovery.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 08:02:09.216315 plugp100-5.0.0.dev4/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 08:01:42.000000 plugp100-5.0.0.dev4/tests/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 08:02:09.216315 plugp100-5.0.0.dev4/tests/unit/hub_child/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 08:01:42.000000 plugp100-5.0.0.dev4/tests/unit/hub_child/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-04-06 08:01:42.000000 plugp100-5.0.0.dev4/tests/unit/hub_child/test_button.py
--rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-04-06 08:01:42.000000 plugp100-5.0.0.dev4/tests/unit/hub_child/test_temp_hum_sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2599 2024-04-06 08:01:42.000000 plugp100-5.0.0.dev4/tests/unit/hub_child/test_trv_ke100.py
--rw-r--r--   0 runner    (1001) docker     (127)     2815 2024-04-06 08:01:42.000000 plugp100-5.0.0.dev4/tests/unit/test_bulb.py
--rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-04-06 08:01:42.000000 plugp100-5.0.0.dev4/tests/unit/test_discovery.py
--rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-04-06 08:01:42.000000 plugp100-5.0.0.dev4/tests/unit/test_hub.py
--rw-r--r--   0 runner    (1001) docker     (127)     3637 2024-04-06 08:01:42.000000 plugp100-5.0.0.dev4/tests/unit/test_klap_protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-06 08:01:42.000000 plugp100-5.0.0.dev4/tests/unit/test_plug.py
--rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-04-06 08:01:42.000000 plugp100-5.0.0.dev4/tests/unit/test_plug_strip.py
--rw-r--r--   0 runner    (1001) docker     (127)      959 2024-04-06 08:01:42.000000 plugp100-5.0.0.dev4/tests/unit/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:09:28.678781 plugp100-5.0.0.dev5/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-06 11:09:01.000000 plugp100-5.0.0.dev5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-06 11:09:01.000000 plugp100-5.0.0.dev5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2833 2024-04-06 11:09:28.678781 plugp100-5.0.0.dev5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2131 2024-04-06 11:09:01.000000 plugp100-5.0.0.dev5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:09:28.654780 plugp100-5.0.0.dev5/plugp100/
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-06 11:09:28.000000 plugp100-5.0.0.dev5/plugp100/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:09:28.658781 plugp100-5.0.0.dev5/plugp100/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 11:09:01.000000 plugp100-5.0.0.dev5/plugp100/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19612 2024-04-06 11:09:01.000000 plugp100-5.0.0.dev5/plugp100/api/light_effect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-04-06 11:09:01.000000 plugp100-5.0.0.dev5/plugp100/api/light_effect_preset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:09:28.658781 plugp100-5.0.0.dev5/plugp100/api/requests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 11:09:01.000000 plugp100-5.0.0.dev5/plugp100/api/requests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-06 11:09:01.000000 plugp100-5.0.0.dev5/plugp100/api/requests/handshake_params.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:09:28.658781 plugp100-5.0.0.dev5/plugp100/api/requests/internal/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 11:09:01.000000 plugp100-5.0.0.dev5/plugp100/api/requests/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-04-06 11:09:01.000000 plugp100-5.0.0.dev5/plugp100/api/requests/internal/snowflake_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-06 11:09:01.000000 plugp100-5.0.0.dev5/plugp100/api/requests/login_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-06 11:09:01.000000 plugp100-5.0.0.dev5/plugp100/api/requests/secure_passthrough_params.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:09:28.658781 plugp100-5.0.0.dev5/plugp100/api/requests/set_device_info/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 11:09:01.000000 plugp100-5.0.0.dev5/plugp100/api/requests/set_device_info/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-06 11:09:01.000000 plugp100-5.0.0.dev5/plugp100/api/requests/set_device_info/play_alarm_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-06 11:09:01.000000 plugp100-5.0.0.dev5/plugp100/api/requests/set_device_info/set_light_color_info_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-06 11:09:01.000000 plugp100-5.0.0.dev5/plugp100/api/requests/set_device_info/set_light_info_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-06 11:09:01.000000 plugp100-5.0.0.dev5/plugp100/api/requests/set_device_info/set_plug_info_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-06 11:09:01.000000 plugp100-5.0.0.dev5/plugp100/api/requests/set_device_info/set_trv_info_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4288 2024-04-06 11:09:01.000000 plugp100-5.0.0.dev5/plugp100/api/requests/tapo_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-06 11:09:01.000000 plugp100-5.0.0.dev5/plugp100/api/requests/trigger_logs_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8301 2024-04-06 11:09:01.000000 plugp100-5.0.0.dev5/plugp100/api/tapo_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:09:28.658781 plugp100-5.0.0.dev5/plugp100/common/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 11:09:01.000000 plugp100-5.0.0.dev5/plugp100/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-06 11:09:01.000000 plugp100-5.0.0.dev5/plugp100/common/credentials.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:09:28.662781 plugp100-5.0.0.dev5/plugp100/common/functional/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 11:09:01.000000 plugp100-5.0.0.dev5/plugp100/common/functional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5729 2024-04-06 11:09:01.000000 plugp100-5.0.0.dev5/plugp100/common/functional/tri.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:09:28.662781 plugp100-5.0.0.dev5/plugp100/common/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 11:09:01.000000 plugp100-5.0.0.dev5/plugp100/common/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-06 11:09:01.000000 plugp100-5.0.0.dev5/plugp100/common/utils/http_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-06 11:09:01.000000 plugp100-5.0.0.dev5/plugp100/common/utils/json_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:09:28.662781 plugp100-5.0.0.dev5/plugp100/discovery/
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-06 11:09:01.000000 plugp100-5.0.0.dev5/plugp100/discovery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4036 2024-04-06 11:09:01.000000 plugp100-5.0.0.dev5/plugp100/discovery/cloud_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3657 2024-04-06 11:09:01.000000 plugp100-5.0.0.dev5/plugp100/discovery/discovered_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-04-06 11:09:01.000000 plugp100-5.0.0.dev5/plugp100/discovery/rsa_session.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3616 2024-04-06 11:09:01.000000 plugp100-5.0.0.dev5/plugp100/discovery/tapo_discovery.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:09:28.662781 plugp100-5.0.0.dev5/plugp100/encryption/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 11:09:01.000000 plugp100-5.0.0.dev5/plugp100/encryption/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-04-06 11:09:01.000000 plugp100-5.0.0.dev5/plugp100/encryption/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-04-06 11:09:01.000000 plugp100-5.0.0.dev5/plugp100/encryption/key_pair.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-04-06 11:09:01.000000 plugp100-5.0.0.dev5/plugp100/encryption/tp_link_cipher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-04-06 11:09:01.000000 plugp100-5.0.0.dev5/plugp100/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:09:28.662781 plugp100-5.0.0.dev5/plugp100/new/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 11:09:01.000000 plugp100-5.0.0.dev5/plugp100/new/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:09:28.666781 plugp100-5.0.0.dev5/plugp100/new/child/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 11:09:01.000000 plugp100-5.0.0.dev5/plugp100/new/child/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14264 2024-04-06 11:09:01.000000 plugp100-5.0.0.dev5/plugp100/new/child/tapohubchildren.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-04-06 11:09:01.000000 plugp100-5.0.0.dev5/plugp100/new/child/tapostripsocket.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:09:28.670781 plugp100-5.0.0.dev5/plugp100/new/components/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 11:09:01.000000 plugp100-5.0.0.dev5/plugp100/new/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-04-06 11:09:01.000000 plugp100-5.0.0.dev5/plugp100/new/components/alarm_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-04-06 11:09:01.000000 plugp100-5.0.0.dev5/plugp100/new/components/battery_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-06 11:09:01.000000 plugp100-5.0.0.dev5/plugp100/new/components/device_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-06 11:09:01.000000 plugp100-5.0.0.dev5/plugp100/new/components/energy_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3971 2024-04-06 11:09:01.000000 plugp100-5.0.0.dev5/plugp100/new/components/hub_children_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-06 11:09:01.000000 plugp100-5.0.0.dev5/plugp100/new/components/humidity_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2596 2024-04-06 11:09:01.000000 plugp100-5.0.0.dev5/plugp100/new/components/light_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-04-06 11:09:01.000000 plugp100-5.0.0.dev5/plugp100/new/components/light_effect_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-06 11:09:01.000000 plugp100-5.0.0.dev5/plugp100/new/components/motion_sensor_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-04-06 11:09:01.000000 plugp100-5.0.0.dev5/plugp100/new/components/on_off_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-06 11:09:01.000000 plugp100-5.0.0.dev5/plugp100/new/components/overheat_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-06 11:09:01.000000 plugp100-5.0.0.dev5/plugp100/new/components/report_mode_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-06 11:09:01.000000 plugp100-5.0.0.dev5/plugp100/new/components/smart_door_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-04-06 11:09:01.000000 plugp100-5.0.0.dev5/plugp100/new/components/socket_children_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-04-06 11:09:01.000000 plugp100-5.0.0.dev5/plugp100/new/components/temperature_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-04-06 11:09:01.000000 plugp100-5.0.0.dev5/plugp100/new/components/temperature_humidity_records.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-04-06 11:09:01.000000 plugp100-5.0.0.dev5/plugp100/new/components/trigger_log_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-06 11:09:01.000000 plugp100-5.0.0.dev5/plugp100/new/components/water_leak_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4080 2024-04-06 11:09:01.000000 plugp100-5.0.0.dev5/plugp100/new/device_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-06 11:09:01.000000 plugp100-5.0.0.dev5/plugp100/new/device_type.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:09:28.670781 plugp100-5.0.0.dev5/plugp100/new/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 11:09:01.000000 plugp100-5.0.0.dev5/plugp100/new/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-06 11:09:01.000000 plugp100-5.0.0.dev5/plugp100/new/errors/invalid_authentication.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:09:28.670781 plugp100-5.0.0.dev5/plugp100/new/event_polling/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 11:09:01.000000 plugp100-5.0.0.dev5/plugp100/new/event_polling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-04-06 11:09:01.000000 plugp100-5.0.0.dev5/plugp100/new/event_polling/event_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3614 2024-04-06 11:09:01.000000 plugp100-5.0.0.dev5/plugp100/new/event_polling/poll_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-04-06 11:09:01.000000 plugp100-5.0.0.dev5/plugp100/new/event_polling/state_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-04-06 11:09:01.000000 plugp100-5.0.0.dev5/plugp100/new/hub_device_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3833 2024-04-06 11:09:01.000000 plugp100-5.0.0.dev5/plugp100/new/tapobulb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5295 2024-04-06 11:09:01.000000 plugp100-5.0.0.dev5/plugp100/new/tapodevice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3405 2024-04-06 11:09:01.000000 plugp100-5.0.0.dev5/plugp100/new/tapohub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-04-06 11:09:01.000000 plugp100-5.0.0.dev5/plugp100/new/tapoplug.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:09:28.670781 plugp100-5.0.0.dev5/plugp100/protocol/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 11:09:01.000000 plugp100-5.0.0.dev5/plugp100/protocol/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:09:28.670781 plugp100-5.0.0.dev5/plugp100/protocol/klap/
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-06 11:09:01.000000 plugp100-5.0.0.dev5/plugp100/protocol/klap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-04-06 11:09:01.000000 plugp100-5.0.0.dev5/plugp100/protocol/klap/klap_handshake_revision.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13480 2024-04-06 11:09:01.000000 plugp100-5.0.0.dev5/plugp100/protocol/klap/klap_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4168 2024-04-06 11:09:01.000000 plugp100-5.0.0.dev5/plugp100/protocol/passthrough_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5294 2024-04-06 11:09:01.000000 plugp100-5.0.0.dev5/plugp100/protocol/securepassthrough_transport.py
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-04-06 11:09:01.000000 plugp100-5.0.0.dev5/plugp100/protocol/tapo_protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:09:28.674781 plugp100-5.0.0.dev5/plugp100/responses/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 11:09:01.000000 plugp100-5.0.0.dev5/plugp100/responses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-04-06 11:09:01.000000 plugp100-5.0.0.dev5/plugp100/responses/alarm_type_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2672 2024-04-06 11:09:01.000000 plugp100-5.0.0.dev5/plugp100/responses/child_device_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-06 11:09:01.000000 plugp100-5.0.0.dev5/plugp100/responses/components.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5621 2024-04-06 11:09:01.000000 plugp100-5.0.0.dev5/plugp100/responses/device_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-04-06 11:09:01.000000 plugp100-5.0.0.dev5/plugp100/responses/device_usage_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-06 11:09:01.000000 plugp100-5.0.0.dev5/plugp100/responses/energy_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:09:28.674781 plugp100-5.0.0.dev5/plugp100/responses/hub_childs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 11:09:01.000000 plugp100-5.0.0.dev5/plugp100/responses/hub_childs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-04-06 11:09:01.000000 plugp100-5.0.0.dev5/plugp100/responses/hub_childs/hub_child_base_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-04-06 11:09:01.000000 plugp100-5.0.0.dev5/plugp100/responses/hub_childs/ke100_device_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-06 11:09:01.000000 plugp100-5.0.0.dev5/plugp100/responses/hub_childs/leak_device_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-04-06 11:09:01.000000 plugp100-5.0.0.dev5/plugp100/responses/hub_childs/s200b_device_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-04-06 11:09:01.000000 plugp100-5.0.0.dev5/plugp100/responses/hub_childs/switch_child_device_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-04-06 11:09:01.000000 plugp100-5.0.0.dev5/plugp100/responses/hub_childs/t100_device_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-06 11:09:01.000000 plugp100-5.0.0.dev5/plugp100/responses/hub_childs/t110_device_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2380 2024-04-06 11:09:01.000000 plugp100-5.0.0.dev5/plugp100/responses/hub_childs/t31x_device_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-06 11:09:01.000000 plugp100-5.0.0.dev5/plugp100/responses/hub_childs/trigger_log_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-06 11:09:01.000000 plugp100-5.0.0.dev5/plugp100/responses/power_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2268 2024-04-06 11:09:01.000000 plugp100-5.0.0.dev5/plugp100/responses/tapo_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2024-04-06 11:09:01.000000 plugp100-5.0.0.dev5/plugp100/responses/tapo_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-06 11:09:01.000000 plugp100-5.0.0.dev5/plugp100/responses/temperature_unit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-04-06 11:09:01.000000 plugp100-5.0.0.dev5/plugp100/responses/time_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:09:28.678781 plugp100-5.0.0.dev5/plugp100.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2833 2024-04-06 11:09:28.000000 plugp100-5.0.0.dev5/plugp100.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5085 2024-04-06 11:09:28.000000 plugp100-5.0.0.dev5/plugp100.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 11:09:28.000000 plugp100-5.0.0.dev5/plugp100.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-06 11:09:28.000000 plugp100-5.0.0.dev5/plugp100.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-06 11:09:28.000000 plugp100-5.0.0.dev5/plugp100.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-06 11:09:01.000000 plugp100-5.0.0.dev5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-06 11:09:01.000000 plugp100-5.0.0.dev5/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-06 11:09:01.000000 plugp100-5.0.0.dev5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-06 11:09:28.678781 plugp100-5.0.0.dev5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-04-06 11:09:01.000000 plugp100-5.0.0.dev5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:09:28.654780 plugp100-5.0.0.dev5/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:09:28.678781 plugp100-5.0.0.dev5/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 11:09:01.000000 plugp100-5.0.0.dev5/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-04-06 11:09:01.000000 plugp100-5.0.0.dev5/tests/integration/tapo_test_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2718 2024-04-06 11:09:01.000000 plugp100-5.0.0.dev5/tests/integration/test_button_t310.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-04-06 11:09:01.000000 plugp100-5.0.0.dev5/tests/integration/test_hub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3139 2024-04-06 11:09:01.000000 plugp100-5.0.0.dev5/tests/integration/test_ledstrip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2160 2024-04-06 11:09:01.000000 plugp100-5.0.0.dev5/tests/integration/test_light.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-04-06 11:09:01.000000 plugp100-5.0.0.dev5/tests/integration/test_plug.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2165 2024-04-06 11:09:01.000000 plugp100-5.0.0.dev5/tests/integration/test_power_strip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2789 2024-04-06 11:09:01.000000 plugp100-5.0.0.dev5/tests/integration/test_sensor_s200b.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3735 2024-04-06 11:09:01.000000 plugp100-5.0.0.dev5/tests/integration/test_tapo_discovery.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:09:28.678781 plugp100-5.0.0.dev5/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 11:09:01.000000 plugp100-5.0.0.dev5/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:09:28.678781 plugp100-5.0.0.dev5/tests/unit/hub_child/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 11:09:01.000000 plugp100-5.0.0.dev5/tests/unit/hub_child/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-04-06 11:09:01.000000 plugp100-5.0.0.dev5/tests/unit/hub_child/test_button.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-04-06 11:09:01.000000 plugp100-5.0.0.dev5/tests/unit/hub_child/test_temp_hum_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2599 2024-04-06 11:09:01.000000 plugp100-5.0.0.dev5/tests/unit/hub_child/test_trv_ke100.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2815 2024-04-06 11:09:01.000000 plugp100-5.0.0.dev5/tests/unit/test_bulb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-04-06 11:09:01.000000 plugp100-5.0.0.dev5/tests/unit/test_discovery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-04-06 11:09:01.000000 plugp100-5.0.0.dev5/tests/unit/test_hub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3637 2024-04-06 11:09:01.000000 plugp100-5.0.0.dev5/tests/unit/test_klap_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-06 11:09:01.000000 plugp100-5.0.0.dev5/tests/unit/test_plug.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-04-06 11:09:01.000000 plugp100-5.0.0.dev5/tests/unit/test_plug_strip.py
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-04-06 11:09:01.000000 plugp100-5.0.0.dev5/tests/unit/test_utils.py
```

### Comparing `plugp100-5.0.0.dev4/LICENSE` & `plugp100-5.0.0.dev5/LICENSE`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev4/PKG-INFO` & `plugp100-5.0.0.dev5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plugp100
-Version: 5.0.0.dev4
+Version: 5.0.0.dev5
 Summary: Controller for TP-Link Tapo P100 and other devices
 Home-page: https://github.com/petretiandrea/plugp100
 Download-URL: https://github.com/petretiandrea/plugp100
 Author: @petretiandrea
 Author-email: petretiandrea@gmail.com
 License: GPL3
 Keywords: Tapo,P100
```

### Comparing `plugp100-5.0.0.dev4/README.md` & `plugp100-5.0.0.dev5/README.md`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev4/plugp100/__init__.py` & `plugp100-5.0.0.dev5/plugp100/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,8 +12,8 @@
         sys.path.append(os.path.join(vendor_dir, vendor_path))
 
 from plugp100.responses import *
 from plugp100.api.requests import *
 from plugp100.api import *
 from plugp100.common import *
 
-__version__ = "5.0.0-dev.4"
+__version__ = "5.0.0-dev.5"
```

### Comparing `plugp100-5.0.0.dev4/plugp100/api/light_effect.py` & `plugp100-5.0.0.dev5/plugp100/api/light_effect.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev4/plugp100/api/light_effect_preset.py` & `plugp100-5.0.0.dev5/plugp100/api/light_effect_preset.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev4/plugp100/api/requests/internal/snowflake_id.py` & `plugp100-5.0.0.dev5/plugp100/api/requests/internal/snowflake_id.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev4/plugp100/api/requests/login_device.py` & `plugp100-5.0.0.dev5/plugp100/api/requests/login_device.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev4/plugp100/api/requests/tapo_request.py` & `plugp100-5.0.0.dev5/plugp100/api/requests/tapo_request.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev4/plugp100/api/tapo_client.py` & `plugp100-5.0.0.dev5/plugp100/api/tapo_client.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev4/plugp100/common/functional/tri.py` & `plugp100-5.0.0.dev5/plugp100/common/functional/tri.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev4/plugp100/common/utils/http_client.py` & `plugp100-5.0.0.dev5/plugp100/common/utils/http_client.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev4/plugp100/discovery/cloud_client.py` & `plugp100-5.0.0.dev5/plugp100/discovery/cloud_client.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev4/plugp100/discovery/discovered_device.py` & `plugp100-5.0.0.dev5/plugp100/discovery/discovered_device.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import dataclasses
+import logging
 from typing import Optional, Any
 
 import aiohttp
 
 from plugp100.common.credentials import AuthCredential
 from plugp100.new.device_factory import DeviceConnectConfiguration, connect
 from plugp100.new.tapodevice import TapoDevice
@@ -10,37 +11,41 @@
 
 @dataclasses.dataclass
 class DiscoveredDevice:
     device_type: str
     device_model: str
     ip: str
     mac: str
-    mgt_encrypt_schm: "EncryptionScheme"
+    mgt_encrypt_schm: Optional["EncryptionSchema"]
 
     device_id: Optional[str] = None
     owner: Optional[str] = None
     hw_ver: Optional[str] = None
     is_support_iot_cloud: Optional[bool] = None
     obd_src: Optional[str] = None
     factory_default: Optional[bool] = None
 
     @staticmethod
     def from_dict(values: dict[str, Any]) -> "DiscoveredDevice":
+        if enc_schema_info := values.get("mgt_encrypt_schm", None):
+            encryption_schema = EncryptionSchema(**enc_schema_info)
+        else:
+            encryption_schema = None
         return DiscoveredDevice(
             device_type=values.get("device_type", values.get("device_type_text")),
             device_model=values.get("device_model", values.get("model")),
             ip=values.get("ip", values.get("alias")),
             mac=values.get("mac"),
             device_id=values.get("device_id", values.get("device_id_hash", None)),
             owner=values.get("owner", values.get("device_owner_hash", None)),
             hw_ver=values.get("hw_ver", None),
             is_support_iot_cloud=values.get("is_support_iot_cloud", None),
             obd_src=values.get("obd_src", None),
             factory_default=values.get("factory_default", None),
-            mgt_encrypt_schm=EncryptionScheme(**values.get("mgt_encrypt_schm")),
+            mgt_encrypt_schm=encryption_schema,
         )
 
     @property
     def as_dict(self) -> dict[str, Any]:
         return {
             "device_type": self.device_type,
             "device_model": self.device_model,
@@ -52,32 +57,44 @@
             "is_support_iot_cloud": self.is_support_iot_cloud,
             "factory_default": self.factory_default,
             "mgt_encrypt_schm": {
                 "is_support_https": self.mgt_encrypt_schm.is_support_https,
                 "encrypt_type": self.mgt_encrypt_schm.encrypt_type,
                 "http_port": self.mgt_encrypt_schm.http_port,
                 "lv": self.mgt_encrypt_schm.lv,
-            },
+            }
+            if self.mgt_encrypt_schm is not None
+            else None,
         }
 
     async def get_tapo_device(
         self, credentials: AuthCredential, session: Optional[aiohttp.ClientSession] = None
     ) -> TapoDevice:
-        config = DeviceConnectConfiguration(
-            host=self.ip,
-            port=self.mgt_encrypt_schm.http_port,
-            credentials=credentials,
-            device_type=self.device_type,
-            encryption_type=self.mgt_encrypt_schm.encrypt_type,
-            encryption_version=self.mgt_encrypt_schm.lv,
-        )
+        if encrypt_schema := self.mgt_encrypt_schm:
+            config = DeviceConnectConfiguration(
+                host=self.ip,
+                port=encrypt_schema.http_port,
+                credentials=credentials,
+                device_type=self.device_type,
+                encryption_type=encrypt_schema.encrypt_type,
+                encryption_version=encrypt_schema.lv,
+            )
+        else:
+            logging.warning(
+                "No encryption schema found for discovered device {}, {}",
+                self.ip,
+                self.device_type,
+            )
+            config = DeviceConnectConfiguration(
+                host=self.ip, port=80, device_type=self.device_type
+            )
         return await connect(config, session)
 
 
 @dataclasses.dataclass
-class EncryptionScheme:
+class EncryptionSchema:
     """Base model for encryption scheme of discovery result."""
 
     is_support_https: Optional[bool] = None
     encrypt_type: Optional[str] = None
     http_port: Optional[int] = None
     lv: Optional[int] = 1
```

### Comparing `plugp100-5.0.0.dev4/plugp100/discovery/rsa_session.py` & `plugp100-5.0.0.dev5/plugp100/discovery/rsa_session.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev4/plugp100/discovery/tapo_discovery.py` & `plugp100-5.0.0.dev5/plugp100/discovery/tapo_discovery.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev4/plugp100/encryption/helpers.py` & `plugp100-5.0.0.dev5/plugp100/encryption/helpers.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev4/plugp100/encryption/key_pair.py` & `plugp100-5.0.0.dev5/plugp100/encryption/key_pair.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev4/plugp100/encryption/tp_link_cipher.py` & `plugp100-5.0.0.dev5/plugp100/encryption/tp_link_cipher.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev4/plugp100/example.py` & `plugp100-5.0.0.dev5/plugp100/example.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev4/plugp100/new/child/tapohubchildren.py` & `plugp100-5.0.0.dev5/plugp100/new/child/tapohubchildren.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev4/plugp100/new/child/tapostripsocket.py` & `plugp100-5.0.0.dev5/plugp100/new/child/tapostripsocket.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev4/plugp100/new/components/alarm_component.py` & `plugp100-5.0.0.dev5/plugp100/new/components/alarm_component.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev4/plugp100/new/components/battery_component.py` & `plugp100-5.0.0.dev5/plugp100/new/components/battery_component.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev4/plugp100/new/components/energy_component.py` & `plugp100-5.0.0.dev5/plugp100/new/components/energy_component.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev4/plugp100/new/components/hub_children_component.py` & `plugp100-5.0.0.dev5/plugp100/new/components/hub_children_component.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev4/plugp100/new/components/light_component.py` & `plugp100-5.0.0.dev5/plugp100/new/components/light_component.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev4/plugp100/new/components/light_effect_component.py` & `plugp100-5.0.0.dev5/plugp100/new/components/light_effect_component.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev4/plugp100/new/components/on_off_component.py` & `plugp100-5.0.0.dev5/plugp100/new/components/on_off_component.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev4/plugp100/new/components/overheat_component.py` & `plugp100-5.0.0.dev5/plugp100/new/components/overheat_component.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev4/plugp100/new/components/report_mode_component.py` & `plugp100-5.0.0.dev5/plugp100/new/components/report_mode_component.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev4/plugp100/new/components/socket_children_component.py` & `plugp100-5.0.0.dev5/plugp100/new/components/socket_children_component.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev4/plugp100/new/components/temperature_component.py` & `plugp100-5.0.0.dev5/plugp100/new/components/temperature_component.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev4/plugp100/new/components/temperature_humidity_records.py` & `plugp100-5.0.0.dev5/plugp100/new/components/temperature_humidity_records.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev4/plugp100/new/components/trigger_log_component.py` & `plugp100-5.0.0.dev5/plugp100/new/components/trigger_log_component.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev4/plugp100/new/components/water_leak_component.py` & `plugp100-5.0.0.dev5/plugp100/new/components/water_leak_component.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev4/plugp100/new/device_factory.py` & `plugp100-5.0.0.dev5/plugp100/new/device_factory.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev4/plugp100/new/event_polling/event_subscription.py` & `plugp100-5.0.0.dev5/plugp100/new/event_polling/event_subscription.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev4/plugp100/new/event_polling/poll_tracker.py` & `plugp100-5.0.0.dev5/plugp100/new/event_polling/poll_tracker.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev4/plugp100/new/event_polling/state_tracker.py` & `plugp100-5.0.0.dev5/plugp100/new/event_polling/state_tracker.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev4/plugp100/new/hub_device_tracker.py` & `plugp100-5.0.0.dev5/plugp100/new/hub_device_tracker.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev4/plugp100/new/tapobulb.py` & `plugp100-5.0.0.dev5/plugp100/new/tapobulb.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev4/plugp100/new/tapodevice.py` & `plugp100-5.0.0.dev5/plugp100/new/tapodevice.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev4/plugp100/new/tapohub.py` & `plugp100-5.0.0.dev5/plugp100/new/tapohub.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev4/plugp100/new/tapoplug.py` & `plugp100-5.0.0.dev5/plugp100/new/tapoplug.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev4/plugp100/protocol/klap/klap_handshake_revision.py` & `plugp100-5.0.0.dev5/plugp100/protocol/klap/klap_handshake_revision.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev4/plugp100/protocol/klap/klap_protocol.py` & `plugp100-5.0.0.dev5/plugp100/protocol/klap/klap_protocol.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev4/plugp100/protocol/passthrough_protocol.py` & `plugp100-5.0.0.dev5/plugp100/protocol/passthrough_protocol.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev4/plugp100/protocol/securepassthrough_transport.py` & `plugp100-5.0.0.dev5/plugp100/protocol/securepassthrough_transport.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev4/plugp100/protocol/tapo_protocol.py` & `plugp100-5.0.0.dev5/plugp100/protocol/tapo_protocol.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev4/plugp100/responses/child_device_list.py` & `plugp100-5.0.0.dev5/plugp100/responses/child_device_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
                 self.get_children(
                     lambda x: HubChildBaseInfo.from_json(x).get_or_else(None)
                 ),
             )
         )
 
     def get_next_index(self) -> int:
-        return self.start_index + len(self.child_device_list) + 1
+        return self.start_index + len(self.child_device_list)
 
     def has_next(self) -> bool:
         return self.get_next_index() < self.sum
 
     def merge(self, other: "ChildDeviceList") -> "ChildDeviceList":
         for other_child in other.child_device_list:
             self.child_device_list.append(other_child)
```

### Comparing `plugp100-5.0.0.dev4/plugp100/responses/components.py` & `plugp100-5.0.0.dev5/plugp100/responses/components.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev4/plugp100/responses/device_state.py` & `plugp100-5.0.0.dev5/plugp100/responses/device_state.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev4/plugp100/responses/device_usage_info.py` & `plugp100-5.0.0.dev5/plugp100/responses/device_usage_info.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev4/plugp100/responses/energy_info.py` & `plugp100-5.0.0.dev5/plugp100/responses/energy_info.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev4/plugp100/responses/hub_childs/hub_child_base_info.py` & `plugp100-5.0.0.dev5/plugp100/responses/hub_childs/hub_child_base_info.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev4/plugp100/responses/hub_childs/ke100_device_state.py` & `plugp100-5.0.0.dev5/plugp100/responses/hub_childs/ke100_device_state.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev4/plugp100/responses/hub_childs/leak_device_state.py` & `plugp100-5.0.0.dev5/plugp100/responses/hub_childs/leak_device_state.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev4/plugp100/responses/hub_childs/s200b_device_state.py` & `plugp100-5.0.0.dev5/plugp100/responses/hub_childs/s200b_device_state.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev4/plugp100/responses/hub_childs/switch_child_device_state.py` & `plugp100-5.0.0.dev5/plugp100/responses/hub_childs/switch_child_device_state.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev4/plugp100/responses/hub_childs/t100_device_state.py` & `plugp100-5.0.0.dev5/plugp100/responses/hub_childs/t100_device_state.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev4/plugp100/responses/hub_childs/t110_device_state.py` & `plugp100-5.0.0.dev5/plugp100/responses/hub_childs/t110_device_state.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev4/plugp100/responses/hub_childs/t31x_device_state.py` & `plugp100-5.0.0.dev5/plugp100/responses/hub_childs/t31x_device_state.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev4/plugp100/responses/hub_childs/trigger_log_response.py` & `plugp100-5.0.0.dev5/plugp100/responses/hub_childs/trigger_log_response.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev4/plugp100/responses/tapo_exception.py` & `plugp100-5.0.0.dev5/plugp100/responses/tapo_exception.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev4/plugp100/responses/tapo_response.py` & `plugp100-5.0.0.dev5/plugp100/responses/tapo_response.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev4/plugp100/responses/time_info.py` & `plugp100-5.0.0.dev5/plugp100/responses/time_info.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev4/plugp100.egg-info/PKG-INFO` & `plugp100-5.0.0.dev5/plugp100.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plugp100
-Version: 5.0.0.dev4
+Version: 5.0.0.dev5
 Summary: Controller for TP-Link Tapo P100 and other devices
 Home-page: https://github.com/petretiandrea/plugp100
 Download-URL: https://github.com/petretiandrea/plugp100
 Author: @petretiandrea
 Author-email: petretiandrea@gmail.com
 License: GPL3
 Keywords: Tapo,P100
```

### Comparing `plugp100-5.0.0.dev4/plugp100.egg-info/SOURCES.txt` & `plugp100-5.0.0.dev5/plugp100.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev4/setup.py` & `plugp100-5.0.0.dev5/setup.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev4/tests/integration/tapo_test_helper.py` & `plugp100-5.0.0.dev5/tests/integration/tapo_test_helper.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev4/tests/integration/test_button_t310.py` & `plugp100-5.0.0.dev5/tests/integration/test_button_t310.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev4/tests/integration/test_hub.py` & `plugp100-5.0.0.dev5/tests/integration/test_hub.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev4/tests/integration/test_ledstrip.py` & `plugp100-5.0.0.dev5/tests/integration/test_ledstrip.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev4/tests/integration/test_light.py` & `plugp100-5.0.0.dev5/tests/integration/test_light.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev4/tests/integration/test_plug.py` & `plugp100-5.0.0.dev5/tests/integration/test_plug.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev4/tests/integration/test_power_strip.py` & `plugp100-5.0.0.dev5/tests/integration/test_power_strip.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import unittest
 
 from plugp100.new.device_factory import connect
-from plugp100.new.tapoplugstrip import TapoPlugStrip
+from plugp100.new.tapoplug import TapoPlug
 from tests.integration.tapo_test_helper import (
     _test_expose_device_info,
     get_test_config,
 )
 
 
 class PowerStripTest(unittest.IsolatedAsyncioTestCase):
     _device = None
     _api = None
 
     async def asyncSetUp(self) -> None:
         connect_config = await get_test_config(device_type="power_strip")
-        self._device: TapoPlugStrip = await connect(connect_config)
+        self._device: TapoPlug = await connect(connect_config)
         await self._device.update()
 
     async def asyncTearDown(self):
         await self._device.client.close()
 
     async def test_expose_device_info(self):
         await _test_expose_device_info(self._device, self)
```

### Comparing `plugp100-5.0.0.dev4/tests/integration/test_sensor_s200b.py` & `plugp100-5.0.0.dev5/tests/integration/test_sensor_s200b.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev4/tests/integration/test_tapo_discovery.py` & `plugp100-5.0.0.dev5/tests/integration/test_tapo_discovery.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import socket
 import threading
 import unittest
 
 from cryptography.hazmat.primitives import serialization, hashes
 from cryptography.hazmat.primitives.asymmetric import padding
 
-from plugp100.discovery.discovered_device import DiscoveredDevice, EncryptionScheme
+from plugp100.discovery.discovered_device import DiscoveredDevice, EncryptionSchema
 from plugp100.discovery.tapo_discovery import (
     TapoDiscovery,
     _build_packet_for_payload_json,
     PKT_ONBOARD_RESPONSE,
 )
 
 
@@ -84,15 +84,15 @@
             devices,
             [
                 DiscoveredDevice(
                     device_type="SMART.TAPOPLUG",
                     device_model="P105(IT)",
                     ip="192.168.1.3",
                     mac="9C-53-22-A7-C8-35",
-                    mgt_encrypt_schm=EncryptionScheme(
+                    mgt_encrypt_schm=EncryptionSchema(
                         is_support_https=False, encrypt_type="KLAP", http_port=80, lv=2
                     ),
                     device_id="26d9887af76f0d5facf8febeb20f6ec9",
                     owner="006EE6989D4F3A0F47715B4F1585CC27",
                     hw_ver=None,
                     is_support_iot_cloud=True,
                     obd_src="tplink",
```

### Comparing `plugp100-5.0.0.dev4/tests/unit/hub_child/test_button.py` & `plugp100-5.0.0.dev5/tests/unit/hub_child/test_button.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev4/tests/unit/hub_child/test_temp_hum_sensor.py` & `plugp100-5.0.0.dev5/tests/unit/hub_child/test_temp_hum_sensor.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev4/tests/unit/hub_child/test_trv_ke100.py` & `plugp100-5.0.0.dev5/tests/unit/hub_child/test_trv_ke100.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev4/tests/unit/test_bulb.py` & `plugp100-5.0.0.dev5/tests/unit/test_bulb.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev4/tests/unit/test_discovery.py` & `plugp100-5.0.0.dev5/tests/unit/test_discovery.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev4/tests/unit/test_hub.py` & `plugp100-5.0.0.dev5/tests/unit/test_hub.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from plugp100.new.device_type import DeviceType
 from plugp100.new.tapohub import TapoHub
-from tests.conftest import hub
+from tests.conftest import hub, hub_lot_devices
 
 
 @hub
 async def test_must_expose_device_info(device: TapoHub):
     assert device.device_type == DeviceType.Hub
 
     assert device.device_id is not None
@@ -36,7 +36,12 @@
 
 
 @hub
 async def test_get_alarm_tones(device: TapoHub):
     if device.has_alarm:
         tones = (await device.get_supported_alarm_tones()).get_or_raise()
         assert len(tones.tones) > 0
+
+
+@hub_lot_devices
+async def test_should_get_all_children(device: TapoHub):
+    assert len(device.children) == 17
```

### Comparing `plugp100-5.0.0.dev4/tests/unit/test_klap_protocol.py` & `plugp100-5.0.0.dev5/tests/unit/test_klap_protocol.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev4/tests/unit/test_plug.py` & `plugp100-5.0.0.dev5/tests/unit/test_plug.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev4/tests/unit/test_plug_strip.py` & `plugp100-5.0.0.dev5/tests/unit/test_plug_strip.py`

 * *Files identical despite different names*

### Comparing `plugp100-5.0.0.dev4/tests/unit/test_utils.py` & `plugp100-5.0.0.dev5/tests/unit/test_utils.py`

 * *Files identical despite different names*

