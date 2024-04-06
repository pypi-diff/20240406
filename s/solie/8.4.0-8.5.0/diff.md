# Comparing `tmp/solie-8.4.0.tar.gz` & `tmp/solie-8.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "solie-8.4.0.tar", max compression
+gzip compressed data, was "solie-8.5.0.tar", max compression
```

## Comparing `solie-8.4.0.tar` & `solie-8.5.0.tar`

### file list

```diff
@@ -1,71 +1,79 @@
--rw-r--r--   0        0        0      852 2024-03-28 14:19:07.799437 solie-8.4.0/pyproject.toml
--rw-r--r--   0        0        0     2478 2024-03-09 13:27:55.333963 solie-8.4.0/README.md
--rw-r--r--   0        0        0    48500 2024-03-25 12:47:52.037390 solie-8.4.0/solie/__init__.py
--rw-r--r--   0        0        0       71 2024-03-09 15:48:49.775153 solie-8.4.0/solie/__main__.py
--rw-r--r--   0        0        0     3272 2024-03-26 15:22:37.188715 solie-8.4.0/solie/definition/api_requester.py
--rw-r--r--   0        0        0     1677 2024-03-09 17:08:46.075371 solie-8.4.0/solie/definition/api_streamer.py
--rw-r--r--   0        0        0      356 2024-03-26 12:30:42.549391 solie-8.4.0/solie/definition/errors.py
--rw-r--r--   0        0        0     2352 2024-03-16 03:43:10.697265 solie-8.4.0/solie/definition/log_handler.py
--rw-r--r--   0        0        0     1648 2024-03-09 16:59:10.375521 solie-8.4.0/solie/definition/percent_axis_item.py
--rw-r--r--   0        0        0     8028 2024-03-09 13:27:55.346958 solie-8.4.0/solie/definition/rw_lock.py
--rw-r--r--   0        0        0      226 2024-03-16 03:43:10.699264 solie-8.4.0/solie/definition/structs.py
--rw-r--r--   0        0        0     2272 2024-03-09 13:27:55.347957 solie-8.4.0/solie/definition/syntax_highlighter.py
--rw-r--r--   0        0        0     4848 2024-03-09 13:27:55.349466 solie-8.4.0/solie/definition/time_axis_item.py
--rw-r--r--   0        0        0     8940 2024-03-16 03:43:10.702273 solie-8.4.0/solie/overlay/coin_selection.py
--rw-r--r--   0        0        0     4663 2024-03-16 03:43:10.703844 solie-8.4.0/solie/overlay/datapath_input.py
--rw-r--r--   0        0        0     2223 2024-03-09 13:27:55.352477 solie-8.4.0/solie/overlay/donation_guide.py
--rw-r--r--   0        0        0     2774 2024-03-09 16:59:10.243988 solie-8.4.0/solie/overlay/download_fill_option.py
--rw-r--r--   0        0        0      794 2024-03-09 13:27:55.355477 solie-8.4.0/solie/overlay/long_text_view.py
--rw-r--r--   0        0        0     8337 2024-03-16 03:43:10.705803 solie-8.4.0/solie/overlay/strategy_basic_input.py
--rw-r--r--   0        0        0     5625 2024-03-16 03:43:10.707804 solie-8.4.0/solie/overlay/strategy_develop_input.py
--rw-r--r--   0        0        0     2544 2024-03-09 15:56:33.599704 solie-8.4.0/solie/overlay/strategy_info_view.py
--rw-r--r--   0        0        0     8074 2024-03-16 03:43:10.709812 solie-8.4.0/solie/overlay/token_selection.py
--rw-r--r--   0        0        0     1411 2024-03-27 13:56:26.405136 solie-8.4.0/solie/parallel.py
--rw-r--r--   0        0        0    10899 2024-03-09 13:27:55.378483 solie-8.4.0/solie/static/icon/blank_coin.png
--rw-r--r--   0        0        0    11242 2024-03-09 13:27:55.379480 solie-8.4.0/solie/static/icon/traffic_light_green.png
--rw-r--r--   0        0        0    11165 2024-03-09 13:27:55.379480 solie-8.4.0/solie/static/icon/traffic_light_red.png
--rw-r--r--   0        0        0    10810 2024-03-09 13:27:55.380992 solie-8.4.0/solie/static/icon/traffic_light_yellow.png
--rw-r--r--   0        0        0    78060 2024-03-09 13:27:55.382001 solie-8.4.0/solie/static/lexend_bold.ttf
--rw-r--r--   0        0        0   556216 2024-03-09 13:27:55.388006 solie-8.4.0/solie/static/notosans_regular.ttf
--rw-r--r--   0        0        0   228761 2024-03-09 13:27:55.391007 solie-8.4.0/solie/static/product_icon.ico
--rw-r--r--   0        0        0   165542 2024-03-09 13:27:55.393001 solie-8.4.0/solie/static/product_icon.png
--rw-r--r--   0        0        0     1611 2024-03-23 04:07:19.832487 solie-8.4.0/solie/static/sample_decision_script.txt
--rw-r--r--   0        0        0      948 2024-03-13 14:52:55.123101 solie-8.4.0/solie/static/sample_indicators_script.txt
--rw-r--r--   0        0        0   120456 2024-03-09 13:27:55.396002 solie-8.4.0/solie/static/source_code_pro.ttf
--rw-r--r--   0        0        0    60876 2024-03-10 00:18:36.209003 solie-8.4.0/solie/user_interface.py
--rw-r--r--   0        0        0      369 2024-03-26 12:58:53.518573 solie-8.4.0/solie/utility/ball.py
--rw-r--r--   0        0        0     2183 2024-03-09 17:08:46.077377 solie-8.4.0/solie/utility/check_internet.py
--rw-r--r--   0        0        0      269 2024-03-09 13:27:55.363476 solie-8.4.0/solie/utility/combine_candle_datas.py
--rw-r--r--   0        0        0      467 2024-03-09 13:27:55.364477 solie-8.4.0/solie/utility/compare_versions.py
--rw-r--r--   0        0        0      624 2024-03-26 13:20:53.854418 solie-8.4.0/solie/utility/convert.py
--rw-r--r--   0        0        0     1535 2024-03-09 13:27:55.365476 solie-8.4.0/solie/utility/decide.py
--rw-r--r--   0        0        0     4283 2024-03-09 16:50:06.741629 solie-8.4.0/solie/utility/download_aggtrade_data.py
--rw-r--r--   0        0        0     3002 2024-03-09 16:59:28.545315 solie-8.4.0/solie/utility/examine_data_files.py
--rw-r--r--   0        0        0     2707 2024-03-09 13:27:55.368484 solie-8.4.0/solie/utility/fill_holes_with_aggtrades.py
--rw-r--r--   0        0        0     2124 2024-03-28 13:22:26.539843 solie-8.4.0/solie/utility/make_indicators.py
--rw-r--r--   0        0        0      282 2024-03-09 13:27:55.370556 solie-8.4.0/solie/utility/outsource.py
--rw-r--r--   0        0        0      567 2024-03-28 14:09:36.434460 solie-8.4.0/solie/utility/remember_task_durations.py
--rw-r--r--   0        0        0      826 2024-03-09 13:27:55.372486 solie-8.4.0/solie/utility/simply_format.py
--rw-r--r--   0        0        0    26330 2024-03-28 13:27:58.689794 solie-8.4.0/solie/utility/simulate_chunk.py
--rw-r--r--   0        0        0      219 2024-03-09 13:27:55.373475 solie-8.4.0/solie/utility/sort_pandas.py
--rw-r--r--   0        0        0     2184 2024-03-09 16:59:09.702020 solie-8.4.0/solie/utility/standardize.py
--rw-r--r--   0        0        0      472 2024-03-09 13:27:55.376488 solie-8.4.0/solie/utility/stop_flag.py
--rw-r--r--   0        0        0     1937 2024-03-10 03:04:34.033231 solie-8.4.0/solie/utility/user_settings.py
--rw-r--r--   0        0        0     4673 2024-03-09 16:59:09.650652 solie-8.4.0/solie/widget/ask_popup.py
--rw-r--r--   0        0        0      312 2024-03-09 13:27:55.400002 solie-8.4.0/solie/widget/brand_label.py
--rw-r--r--   0        0        0      836 2024-03-09 13:27:55.400002 solie-8.4.0/solie/widget/gauge.py
--rw-r--r--   0        0        0      236 2024-03-09 13:27:55.401000 solie-8.4.0/solie/widget/horizontal_divider.py
--rw-r--r--   0        0        0     1319 2024-03-16 03:43:10.711802 solie-8.4.0/solie/widget/log_list.py
--rw-r--r--   0        0        0     3401 2024-03-16 03:43:10.712802 solie-8.4.0/solie/widget/overlay_panel.py
--rw-r--r--   0        0        0       83 2024-03-09 13:27:55.405002 solie-8.4.0/solie/widget/popup_box.py
--rw-r--r--   0        0        0     3224 2024-03-09 15:56:33.616112 solie-8.4.0/solie/widget/script_editor.py
--rw-r--r--   0        0        0     2532 2024-03-09 15:56:33.617111 solie-8.4.0/solie/widget/splash_screen.py
--rw-r--r--   0        0        0       84 2024-03-09 13:27:55.408000 solie-8.4.0/solie/widget/symbol_box.py
--rw-r--r--   0        0        0       98 2024-03-09 13:27:55.409004 solie-8.4.0/solie/widget/transparent_scroll_area.py
--rw-r--r--   0        0        0      233 2024-03-09 13:27:55.410001 solie-8.4.0/solie/widget/vertical_divider.py
--rw-r--r--   0        0        0    31834 2024-03-25 12:06:14.320274 solie-8.4.0/solie/worker/collector.py
--rw-r--r--   0        0        0    12213 2024-03-26 13:11:50.644854 solie-8.4.0/solie/worker/manager.py
--rw-r--r--   0        0        0    57959 2024-03-26 15:51:56.784460 solie-8.4.0/solie/worker/simulator.py
--rw-r--r--   0        0        0    10715 2024-03-23 02:57:33.959575 solie-8.4.0/solie/worker/strategist.py
--rw-r--r--   0        0        0    94446 2024-03-28 14:09:36.443490 solie-8.4.0/solie/worker/transactor.py
--rw-r--r--   0        0        0     3650 1970-01-01 00:00:00.000000 solie-8.4.0/PKG-INFO
+-rw-r--r--   0        0        0      787 2024-04-06 13:51:29.779391 solie-8.5.0/pyproject.toml
+-rw-r--r--   0        0        0     2478 2024-03-09 13:27:55.333963 solie-8.5.0/README.md
+-rw-r--r--   0        0        0       65 2024-04-04 12:33:45.799336 solie-8.5.0/solie/__init__.py
+-rw-r--r--   0        0        0       85 2024-04-04 12:41:05.189192 solie-8.5.0/solie/__main__.py
+-rw-r--r--   0        0        0      363 2024-04-05 00:02:40.054806 solie-8.5.0/solie/common/__init__.py
+-rw-r--r--   0        0        0      293 2024-04-04 11:56:27.778407 solie-8.5.0/solie/common/connect_event.py
+-rw-r--r--   0        0        0      280 2024-04-05 00:02:06.898492 solie-8.5.0/solie/common/info.py
+-rw-r--r--   0        0        0     1259 2024-04-04 12:51:28.608601 solie-8.5.0/solie/common/parallel.py
+-rw-r--r--   0        0        0       65 2024-04-04 11:36:05.301867 solie-8.5.0/solie/entry/__init__.py
+-rw-r--r--   0        0        0     4156 2024-04-05 11:40:24.240903 solie-8.5.0/solie/entry/lifetime.py
+-rw-r--r--   0        0        0      202 2024-04-05 11:30:17.371547 solie-8.5.0/solie/entry/start.py
+-rw-r--r--   0        0        0      668 2024-04-03 16:31:10.028573 solie-8.5.0/solie/overlay/__init__.py
+-rw-r--r--   0        0        0     8585 2024-04-04 13:05:54.660856 solie-8.5.0/solie/overlay/coin_selection.py
+-rw-r--r--   0        0        0     4493 2024-04-04 11:57:06.554716 solie-8.5.0/solie/overlay/datapath_input.py
+-rw-r--r--   0        0        0     2203 2024-04-03 16:31:10.033574 solie-8.5.0/solie/overlay/donation_guide.py
+-rw-r--r--   0        0        0     2716 2024-04-04 11:58:19.815741 solie-8.5.0/solie/overlay/download_fill_option.py
+-rw-r--r--   0        0        0      646 2024-04-03 16:31:10.037100 solie-8.5.0/solie/overlay/long_text_view.py
+-rw-r--r--   0        0        0     8055 2024-04-04 11:58:27.486831 solie-8.5.0/solie/overlay/strategy_basic_input.py
+-rw-r--r--   0        0        0     6210 2024-04-05 11:56:28.614118 solie-8.5.0/solie/overlay/strategy_develop_input.py
+-rw-r--r--   0        0        0     2441 2024-04-03 16:31:10.041098 solie-8.5.0/solie/overlay/strategy_info_view.py
+-rw-r--r--   0        0        0     7816 2024-04-04 13:09:54.727633 solie-8.5.0/solie/overlay/token_selection.py
+-rw-r--r--   0        0        0    10899 2024-03-09 13:27:55.378483 solie-8.5.0/solie/static/icon/blank_coin.png
+-rw-r--r--   0        0        0    11242 2024-03-09 13:27:55.379480 solie-8.5.0/solie/static/icon/traffic_light_green.png
+-rw-r--r--   0        0        0    11165 2024-03-09 13:27:55.379480 solie-8.5.0/solie/static/icon/traffic_light_red.png
+-rw-r--r--   0        0        0    10810 2024-03-09 13:27:55.380992 solie-8.5.0/solie/static/icon/traffic_light_yellow.png
+-rw-r--r--   0        0        0    78060 2024-03-09 13:27:55.382001 solie-8.5.0/solie/static/lexend_bold.ttf
+-rw-r--r--   0        0        0   556216 2024-03-09 13:27:55.388006 solie-8.5.0/solie/static/notosans_regular.ttf
+-rw-r--r--   0        0        0   228761 2024-03-09 13:27:55.391007 solie-8.5.0/solie/static/product_icon.ico
+-rw-r--r--   0        0        0   165542 2024-03-09 13:27:55.393001 solie-8.5.0/solie/static/product_icon.png
+-rw-r--r--   0        0        0     1678 2024-03-29 12:50:13.329402 solie-8.5.0/solie/static/sample_decision_script.txt
+-rw-r--r--   0        0        0     1015 2024-03-29 12:49:25.127196 solie-8.5.0/solie/static/sample_indicators_script.txt
+-rw-r--r--   0        0        0   120456 2024-03-09 13:27:55.396002 solie-8.5.0/solie/static/source_code_pro.ttf
+-rw-r--r--   0        0        0     3064 2024-04-06 11:43:43.146126 solie-8.5.0/solie/utility/__init__.py
+-rw-r--r--   0        0        0    30449 2024-04-04 11:33:50.635949 solie-8.5.0/solie/utility/analyze_market.py
+-rw-r--r--   0        0        0     3599 2024-04-03 16:31:10.045095 solie-8.5.0/solie/utility/api_requester.py
+-rw-r--r--   0        0        0     2261 2024-04-04 14:21:39.539090 solie-8.5.0/solie/utility/api_streamer.py
+-rw-r--r--   0        0        0     3762 2024-04-03 16:31:10.047095 solie-8.5.0/solie/utility/backward_compatibility.py
+-rw-r--r--   0        0        0      379 2024-04-01 16:30:30.467934 solie-8.5.0/solie/utility/ball.py
+-rw-r--r--   0        0        0     2238 2024-04-04 12:25:21.345905 solie-8.5.0/solie/utility/check_internet.py
+-rw-r--r--   0        0        0      475 2024-04-01 16:30:30.473475 solie-8.5.0/solie/utility/compare_versions.py
+-rw-r--r--   0        0        0      624 2024-03-30 00:54:45.144782 solie-8.5.0/solie/utility/convert.py
+-rw-r--r--   0        0        0     7329 2024-04-06 10:20:38.815616 solie-8.5.0/solie/utility/download_from_binance.py
+-rw-r--r--   0        0        0     2368 2024-04-04 14:26:08.098735 solie-8.5.0/solie/utility/log_handler.py
+-rw-r--r--   0        0        0      294 2024-04-03 16:31:10.051094 solie-8.5.0/solie/utility/pandas_related.py
+-rw-r--r--   0        0        0     2272 2024-04-03 16:31:10.052097 solie-8.5.0/solie/utility/percent_axis_item.py
+-rw-r--r--   0        0        0     8065 2024-04-03 23:15:40.155486 solie-8.5.0/solie/utility/rw_lock.py
+-rw-r--r--   0        0        0      251 2024-04-03 16:31:10.055105 solie-8.5.0/solie/utility/simply_format.py
+-rw-r--r--   0        0        0      229 2024-04-01 16:30:30.488484 solie-8.5.0/solie/utility/sort_pandas.py
+-rw-r--r--   0        0        0     1647 2024-04-03 16:31:10.057101 solie-8.5.0/solie/utility/standardize.py
+-rw-r--r--   0        0        0      484 2024-04-03 16:31:10.058095 solie-8.5.0/solie/utility/stop_flag.py
+-rw-r--r--   0        0        0     1107 2024-04-03 16:31:10.059097 solie-8.5.0/solie/utility/structs.py
+-rw-r--r--   0        0        0     2272 2024-04-03 16:31:10.060102 solie-8.5.0/solie/utility/syntax_highlighter.py
+-rw-r--r--   0        0        0     4848 2024-04-04 12:09:23.272841 solie-8.5.0/solie/utility/time_axis_item.py
+-rw-r--r--   0        0        0      926 2024-04-06 11:42:39.262331 solie-8.5.0/solie/utility/timing.py
+-rw-r--r--   0        0        0     1624 2024-04-03 16:31:10.062097 solie-8.5.0/solie/utility/user_settings.py
+-rw-r--r--   0        0        0      813 2024-04-03 17:07:30.543145 solie-8.5.0/solie/widget/__init__.py
+-rw-r--r--   0        0        0     5292 2024-04-04 11:59:09.143773 solie-8.5.0/solie/widget/ask_popup.py
+-rw-r--r--   0        0        0      312 2024-04-01 14:45:12.996498 solie-8.5.0/solie/widget/brand_label.py
+-rw-r--r--   0        0        0      836 2024-04-01 14:45:14.358385 solie-8.5.0/solie/widget/gauge.py
+-rw-r--r--   0        0        0      236 2024-04-01 14:45:14.989682 solie-8.5.0/solie/widget/horizontal_divider.py
+-rw-r--r--   0        0        0     1922 2024-04-04 11:59:20.593678 solie-8.5.0/solie/widget/log_list.py
+-rw-r--r--   0        0        0     4184 2024-04-04 23:30:33.899456 solie-8.5.0/solie/widget/overlay_popup.py
+-rw-r--r--   0        0        0       83 2024-04-01 14:45:50.650424 solie-8.5.0/solie/widget/popup_box.py
+-rw-r--r--   0        0        0     3202 2024-04-03 16:31:10.068616 solie-8.5.0/solie/widget/script_editor.py
+-rw-r--r--   0        0        0     2576 2024-04-03 16:31:10.069616 solie-8.5.0/solie/widget/splash_screen.py
+-rw-r--r--   0        0        0       84 2024-04-01 14:04:49.291376 solie-8.5.0/solie/widget/symbol_box.py
+-rw-r--r--   0        0        0       98 2024-04-01 14:04:49.292379 solie-8.5.0/solie/widget/transparent_scroll_area.py
+-rw-r--r--   0        0        0      233 2024-04-01 14:04:49.293376 solie-8.5.0/solie/widget/vertical_divider.py
+-rw-r--r--   0        0        0       50 2024-04-03 16:31:10.070617 solie-8.5.0/solie/window/__init__.py
+-rw-r--r--   0        0        0    61287 2024-04-06 01:35:32.018253 solie-8.5.0/solie/window/compiled.py
+-rw-r--r--   0        0        0    35529 2024-04-04 14:37:31.636472 solie-8.5.0/solie/window/main.py
+-rw-r--r--   0        0        0      319 2024-04-04 11:50:37.144088 solie-8.5.0/solie/worker/__init__.py
+-rw-r--r--   0        0        0    32281 2024-04-06 12:49:54.725669 solie-8.5.0/solie/worker/collector.py
+-rw-r--r--   0        0        0    12495 2024-04-06 10:12:12.050859 solie-8.5.0/solie/worker/manager.py
+-rw-r--r--   0        0        0    59289 2024-04-06 11:46:25.564267 solie-8.5.0/solie/worker/simulator.py
+-rw-r--r--   0        0        0    10598 2024-04-04 12:31:28.938266 solie-8.5.0/solie/worker/strategist.py
+-rw-r--r--   0        0        0    93573 2024-04-06 13:35:04.602646 solie-8.5.0/solie/worker/transactor.py
+-rw-r--r--   0        0        0      695 2024-04-04 11:45:07.528915 solie-8.5.0/solie/worker/united.py
+-rw-r--r--   0        0        0     3699 1970-01-01 00:00:00.000000 solie-8.5.0/PKG-INFO
```

### Comparing `solie-8.4.0/pyproject.toml` & `solie-8.5.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "solie"
-version = "8.4.0"
+version = "8.5.0"
 description = "GUI trading bot designed for targeting the futures markets of Binance"
 authors = ["Cunarist"]
 readme = "README.md"
 repository = "https://github.com/cunarist/solie"
 
 [tool.poetry.dependencies]
 python = "^3.9,<3.13"
@@ -20,15 +20,12 @@
 apscheduler = "^3.10.4"
 pygments = "^2.17.1"
 yapf = "^0.32.0"
 getmac = "^0.8.3"
 pandas-ta = { version = "^0.3.14b", allow-prereleases = true }
 time-machine = "^2.13.0"
 xdialog = "^1.1.1"
+dataclasses-json = "^0.6.4"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
-
-[tool.ruff.lint]
-extend-select = ["N", "I", "T20"]
-exclude = ["solie/user_interface.py"]
```

### Comparing `solie-8.4.0/README.md` & `solie-8.5.0/README.md`

 * *Files identical despite different names*

### Comparing `solie-8.4.0/solie/definition/api_requester.py` & `solie-8.5.0/solie/utility/api_requester.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,42 +1,49 @@
 import hashlib
 import hmac
+import json
 from datetime import datetime, timezone
 from urllib.parse import urlencode
 
 import aiohttp
 
-from solie.definition.errors import ApiRequestError
+
+class ApiRequestError(Exception):
+    def __init__(self, info_text: str, payload: dict | None):
+        error_message = info_text
+        if payload:
+            error_message += "\n"
+            error_message += json.dumps(payload, indent=2)
+        super().__init__(error_message)
 
 
 class ApiRequester:
     used_rates = {}
 
     def __init__(self):
-        self.keys = {
-            "binance_api": "",
-            "binance_secret": "",
-        }
+        self.binance_api_key = ""
+        self.binance_api_secret = ""
 
-    def update_keys(self, keys):
-        self.keys.update(keys)
+    def update_keys(self, binance_api_key: str, binance_api_secret: str):
+        self.binance_api_key = binance_api_key
+        self.binance_api_secret = binance_api_secret
 
     async def binance(
         self, http_method: str, path: str, payload: dict = {}, server="futures"
     ):
         query_string = urlencode(payload)
         # replace single quote to double quote
         query_string = query_string.replace("%27", "%22")
 
         signature = hmac.new(
-            self.keys["binance_secret"].encode("utf-8"),
+            self.binance_api_secret.encode("utf-8"),
             query_string.encode("utf-8"),
             hashlib.sha256,
         ).hexdigest()
-        headers = {"X-MBX-APIKEY": self.keys["binance_api"]}
+        headers = {"X-MBX-APIKEY": self.binance_api_key}
 
         if server == "spot":
             url = "https://api.binance.com"
         elif server == "futures":
             url = "https://fapi.binance.com"
         else:
             raise ValueError("This Binance server is not supported")
```

### Comparing `solie-8.4.0/solie/definition/api_streamer.py` & `solie-8.5.0/solie/utility/api_streamer.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,44 +1,63 @@
 import asyncio
+import json
+import logging
 from typing import Callable, Coroutine
 
 import aiohttp
 
-import solie
+logger = logging.getLogger(__name__)
+
+
+class ApiStreamError(Exception):
+    def __init__(self, received: dict | list):
+        formatted = json.dumps(received, indent=2)
+        super().__init__(formatted)
 
 
 class ApiStreamer:
-    def __init__(self, url: str, when_received: Callable[..., Coroutine]):
+    def __init__(
+        self,
+        url: str,
+        handler: Callable[[dict], Coroutine] | Callable[[list], Coroutine],
+    ):
         self._url = url
-        self._when_received = when_received
+        self._handler = handler
         self.session = aiohttp.ClientSession()
 
         if url != "":
             asyncio.create_task(self._run_websocket())
 
     def __del__(self):
         asyncio.create_task(self._close_self())
 
     async def _run_websocket(self):
         while True:
             try:
                 async with self.session.ws_connect(self._url) as websocket:
-                    solie.logger.info(f"Websocket connected: {self._url}")
+                    logger.info(f"Websocket connected: {self._url}")
                     async for received_raw in websocket:
                         if received_raw.type in (
                             aiohttp.WSMsgType.CLOSED,
                             aiohttp.WSMsgType.ERROR,
                         ):
-                            solie.logger.info(f"Websocket closed: {self._url}")
+                            logger.info(f"Websocket closed: {self._url}")
                             break
                         else:
                             received = received_raw.json()
-                            asyncio.create_task(self._when_received(received=received))
-                    solie.logger.info(f"Websocket stopped: {self._url}")
+
+                            def done_callback(task: asyncio.Task, received=received):
+                                error = task.exception()
+                                if error:
+                                    raise ApiStreamError(received) from error
+
+                            task = asyncio.create_task(self._handler(received))
+                            task.add_done_callback(done_callback)
+                    logger.info(f"Websocket stopped: {self._url}")
             except Exception as error:
                 # Handle errors that might occur due to network issues
-                solie.logger.exception(f"Websocket error: {error}")
+                logger.exception(f"Websocket error: {error}")
                 # Wait for a few seconds before attempting to reconnect
                 await asyncio.sleep(5)
 
     async def _close_self(self):
         await self.session.close()
```

### Comparing `solie-8.4.0/solie/definition/log_handler.py` & `solie-8.5.0/solie/utility/log_handler.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 import asyncio
 import logging
-import os
 import time
 from datetime import datetime, timezone
+from pathlib import Path
+from typing import Callable
 
 import aiofiles
-
-import solie
+import aiofiles.os
 
 
 class LogHandler(logging.Handler):
-    def __init__(self, log_path: str):
+    file_lock = asyncio.Lock()
+
+    def __init__(self, log_path: Path, callback: Callable[[str, str], None]):
         super().__init__()
 
-        os.makedirs(log_path, exist_ok=True)
         self.log_path = log_path
+        self.callback = callback
 
         log_format = "%(asctime)s.%(msecs)03d %(levelname)s"
         date_format = "%Y-%m-%d %H:%M:%S"
         log_formatter = logging.Formatter(log_format, datefmt=date_format)
         log_formatter.converter = time.gmtime
         self.setFormatter(log_formatter)
 
@@ -36,37 +38,30 @@
             # when this is from an exception
             lines = formatted.split("\n")
             summarization = lines[0]
             log_content = "\n".join(lines[1:])
             exception = log_record.exc_info[0]
             if exception is None:
                 return
-            exc_type = exception.__name__
-            summarization += f" - {exc_type}"
+            summarization += f" - {exception.__name__}"
         else:
             # when this is a normal log
             summarization = formatted
             log_content = log_record.getMessage()
             first_line_content = log_content.split("\n")[0].strip()
             summarization += f" - {first_line_content}"
             summarization = summarization[:80]
 
-        asyncio.create_task(
-            self.add_log_output(
-                summarization,
-                log_content,
-            )
-        )
+        log_content = f"{formatted}\n{log_content}"
 
-    async def add_log_output(self, *args, **kwargs):
-        # get the data
-        summarization = args[0]
-        log_content = args[1]
+        asyncio.create_task(self.add_log_output(summarization, log_content))
 
+    async def add_log_output(self, summarization: str, log_content: str):
         # add to log list
-        solie.window.listWidget.addItem(summarization, log_content)
+        self.callback(summarization, log_content)
 
         # save to file
-        filepath = f"{self.log_path}/{self.filename}"
-        async with aiofiles.open(filepath, "a", encoding="utf8") as file:
-            await file.write(f"{summarization}\n")
-            await file.write(f"{log_content}\n\n")
+        filepath = self.log_path / self.filename
+        async with self.file_lock:
+            async with aiofiles.open(filepath, "a", encoding="utf8") as file:
+                line_divider = "-" * 80
+                await file.write(f"{log_content}\n\n{line_divider}\n\n")
```

### Comparing `solie-8.4.0/solie/definition/percent_axis_item.py` & `solie-8.5.0/solie/utility/percent_axis_item.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 import math
 
 from pyqtgraph import AxisItem
 
-from solie.utility import simply_format
-
 
 class PercentAxisItem(AxisItem):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
     def tickValues(self, min_value, max_value, size):  # noqa:N802
         min_value = max(0.001 * max_value, min_value)
@@ -37,13 +35,37 @@
         strings = []
 
         if len(tick_values) > 0:
             next_condition = tick_values[0]
             for tick_value in tick_values:
                 if tick_value >= next_condition:
                     next_condition = tick_value + distance
-                    string = simply_format.fixed_float(tick_value, 6)
+                    string = self.format_fixed_float(tick_value, 6)
                     strings.append(string)
                 else:
                     strings.append("")
 
         return strings
+
+    def format_fixed_float(
+        self, number: int | float, width=4, positive_sign=False
+    ) -> str:
+        if width < 4:
+            width = 4
+
+        if number < 0 or (positive_sign and number >= 0):
+            # when sign should be included
+            absolute_limit = 10 ** (width - 1)
+        else:
+            absolute_limit = 10**width
+
+        if abs(number) >= absolute_limit:
+            number = absolute_limit - 1 if number > 0 else -absolute_limit + 1
+
+        string = f"{number:12.12f}"
+
+        if positive_sign and number >= 0:
+            string = "+" + string
+
+        string = string[:width]
+
+        return string
```

### Comparing `solie-8.4.0/solie/definition/rw_lock.py` & `solie-8.5.0/solie/utility/rw_lock.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 import asyncio
+from asyncio import AbstractEventLoop, Future, Task
 from collections import deque
-from typing import Any, Deque, Generic, List, Optional, Tuple, TypeVar
-
-Loop = asyncio.AbstractEventLoop
-OptLoop = Optional[Loop]
-
-# silence LGTM service alerts
-Future = asyncio.Future
-Task = asyncio.Task
+from typing import Any, Generic, TypeVar
 
 
 # The internal lock object managing the RWLock state.
 class _RWLockCore:
     _RL = 1
     _WL = 2
 
-    def __init__(self, fast: bool, loop: Loop):
+    def __init__(self, fast: bool, loop: AbstractEventLoop):
         self._do_yield = not fast
-        self._loop: Loop = loop
-        self._read_waiters: Deque[Future[None]] = deque()
-        self._write_waiters: Deque[Future[None]] = deque()
+        self._loop = loop
+        self._read_waiters: deque[Future[None]] = deque()
+        self._write_waiters: deque[Future[None]] = deque()
         self._r_state: int = 0
         self._w_state: int = 0
         # tasks will be few, so a list is not inefficient
-        self._owning: List[Tuple[Task[Any], int]] = []
+        self._owning: list[tuple[Task[Any], int]] = []
+
+    @property
+    def r_state(self) -> int:
+        return self._r_state
+
+    @property
+    def w_state(self) -> int:
+        return self._w_state
 
     @property
     def read_locked(self) -> bool:
         return self._r_state > 0
 
     @property
     def write_locked(self) -> bool:
@@ -163,15 +165,15 @@
 
     async def __aenter__(self):
         await self.acquire()
         # We have no use for the "as ..."  clause in the with
         # statement for locks.
         return None
 
-    async def __aexit__(self, *args: List[Any]):
+    async def __aexit__(self, *args: list[Any]):
         self.release()
 
     async def acquire(self):
         raise NotImplementedError  # pragma: no cover
 
     def release(self):
         raise NotImplementedError  # pragma: no cover
@@ -199,15 +201,15 @@
         await self._lock.acquire_read()
         return self._wrapper
 
     async def __aexit__(self, exc_type, exc, tb):
         self._lock.release_read()
 
     def __repr__(self) -> str:
-        status = "locked" if self._lock._r_state > 0 else "unlocked"
+        status = "locked" if self._lock.r_state > 0 else "unlocked"
         return "<ReaderLock: [{}]>".format(status)
 
 
 class WriteLock(_ContextManagerMixin, Generic[T]):
     def __init__(self, lock: _RWLockCore, wrapper: Cell[T]):
         self._wrapper = wrapper
         self._lock = lock
@@ -220,15 +222,15 @@
         await self._lock.acquire_write()
         return self._wrapper
 
     async def __aexit__(self, exc_type, exc, tb):
         self._lock.release_write()
 
     def __repr__(self) -> str:
-        status = "locked" if self._lock._w_state > 0 else "unlocked"
+        status = "locked" if self._lock.w_state > 0 else "unlocked"
         return "<WriterLock: [{}]>".format(status)
 
 
 class RWLock(Generic[T]):
     """A RWLock maintains a pair of associated locks, one for read-only
     operations and one for writing. The read lock may be held simultaneously
     by multiple reader tasks, so long as there are no writers. The write
@@ -236,15 +238,15 @@
     """
 
     core = _RWLockCore
 
     def __init__(self, cell_data: T, fast: bool = True):
         loop = asyncio.get_running_loop()
         self._wrapper = Cell(cell_data)
-        self._loop: Loop = loop
+        self._loop = loop
         core = self.core(fast, self._loop)
         self.read_lock = ReadLock(core, self._wrapper)
         self.write_lock = WriteLock(core, self._wrapper)
 
     def __repr__(self) -> str:
         rl = self.read_lock.__repr__()
         wl = self.write_lock.__repr__()
```

### Comparing `solie-8.4.0/solie/definition/syntax_highlighter.py` & `solie-8.5.0/solie/utility/syntax_highlighter.py`

 * *Files identical despite different names*

### Comparing `solie-8.4.0/solie/definition/time_axis_item.py` & `solie-8.5.0/solie/utility/time_axis_item.py`

 * *Files identical despite different names*

### Comparing `solie-8.4.0/solie/overlay/coin_selection.py` & `solie-8.5.0/solie/overlay/coin_selection.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 import asyncio
 
 from PySide6 import QtCore, QtGui, QtWidgets
 
-import solie
-from solie.definition.api_requester import ApiRequester
-from solie.utility import outsource, user_settings
-from solie.widget.horizontal_divider import HorizontalDivider
+from solie.common import PACKAGE_PATH, outsource
+from solie.utility import ApiRequester
+from solie.widget import BaseOverlay, HorizontalDivider, ask
 
 
-class CoinSelection(QtWidgets.QWidget):
-    def __init__(self, done_event: asyncio.Event, payload):
+class CoinSelection(BaseOverlay):
+    def __init__(self, asset_token: str):
         super().__init__()
         self.is_closed = False
 
-        asyncio.create_task(self.fill(done_event))
+        self.asset_token = asset_token
 
-    async def fill(self, done_event):
+        asyncio.create_task(self.fill())
+
+    async def fill(self):
         # ■■■■■ for remembering ■■■■■
 
         api_requester = ApiRequester()
-        symbol_checkboxes = {}
+        symbol_checkboxes: dict[str, QtWidgets.QCheckBox] = {}
 
         # ■■■■■ get previous things ■■■■■
 
-        asset_token = user_settings.get_data_settings()["asset_token"]
+        asset_token = self.asset_token
 
         # ■■■■■ get available symbols ■■■■■
 
         available_symbols = []
 
         response = await api_requester.binance(
             http_method="GET",
@@ -97,15 +98,15 @@
         card_layout = QtWidgets.QVBoxLayout(card)
         card_layout.setContentsMargins(80, 40, 80, 40)
         cards_layout.addWidget(card)
 
         # explanation
         detail_text = QtWidgets.QLabel()
         detail_text.setText(
-            "These are all available coins on Binance."
+            "These are all the available coins from the token you chose."
             "\nYou can select a minimum of 1 and a maximum of 12."
         )
         detail_text.setAlignment(QtCore.Qt.AlignmentFlag.AlignCenter)
         detail_text.setWordWrap(True)
         card_layout.addWidget(detail_text)
 
         # spacing
@@ -126,15 +127,15 @@
         spacing_text.setFont(spacing_text_font)
         card_layout.addWidget(spacing_text)
 
         # input
         symbol_icon_labels = {}
         input_layout = QtWidgets.QGridLayout()
         blank_coin_pixmap = QtGui.QPixmap()
-        blank_coin_pixmap.load(f"{solie.PATH}/static/icon/blank_coin.png")
+        blank_coin_pixmap.load(str(PACKAGE_PATH / "static" / "icon" / "blank_coin.png"))
         for turn, symbol in enumerate(available_symbols):
             coin_symbol = symbol.removesuffix(asset_token)
             coin_name = coin_names.get(coin_symbol, "")
             coin_rank = coin_ranks.get(coin_symbol, 0)
             this_layout = QtWidgets.QHBoxLayout()
             row = turn // 2
             column = turn % 2
@@ -162,58 +163,52 @@
                 QtWidgets.QSizePolicy.Policy.Minimum,
             )
             this_layout.addItem(spacer)
         card_layout.addItem(input_layout)
 
         # ■■■■■ a card ■■■■■
 
+        self.result: list[str]
+
         # confirm function
-        async def job_cf(*args):
-            data_settings = {}
-            selected_symbols = []
+        async def job_cf():
+            selected_symbols: list[str] = []
             for symbol, checkbox in symbol_checkboxes.items():
                 is_checked = checkbox.isChecked()
                 if is_checked:
                     selected_symbols.append(symbol)
-            if 1 <= len(selected_symbols) <= 12:
-                is_symbol_count_ok = True
-                data_settings["target_symbols"] = selected_symbols
-            else:
-                is_symbol_count_ok = False
-                question = [
+            if not 1 <= len(selected_symbols) <= 12:
+                await ask(
                     "Select a proper number of coins",
                     "You can select a minimum of 1 and a maximum of 12.",
                     ["Okay"],
-                ]
-                await solie.window.ask(question)
-            if is_symbol_count_ok:
-                question = [
+                )
+            else:
+                answer = await ask(
                     "Okay to proceed?",
                     "You cannot change your selections unless you make a new data"
                     " folder.",
                     ["No", "Yes"],
-                ]
-                answer = await solie.window.ask(question)
+                )
                 if answer in (0, 1):
                     return
-                await user_settings.apply_data_settings(data_settings)
-                await user_settings.load()
                 self.is_closed = True
-                done_event.set()
+                self.result = selected_symbols
+                self.done_event.set()
 
         # card structure
         card = QtWidgets.QGroupBox()
         card.setFixedWidth(720)
         card_layout = QtWidgets.QHBoxLayout(card)
         card_layout.setContentsMargins(80, 40, 80, 40)
         cards_layout.addWidget(card)
 
         # confirm button
         confirm_button = QtWidgets.QPushButton("Okay", card)
-        outsource.do(confirm_button.clicked, job_cf)
+        outsource(confirm_button.clicked, job_cf)
         confirm_button.setSizePolicy(
             QtWidgets.QSizePolicy.Policy.Fixed,
             QtWidgets.QSizePolicy.Policy.Fixed,
         )
         card_layout.addWidget(confirm_button)
 
         # ■■■■■ spacing ■■■■■
```

### Comparing `solie-8.4.0/solie/overlay/datapath_input.py` & `solie-8.5.0/solie/overlay/datapath_input.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,18 @@
-import asyncio
+from pathlib import Path
 
 import xdialog
 from PySide6 import QtCore, QtGui, QtWidgets
 
-import solie
-from solie.parallel import go
-from solie.utility import outsource, user_settings
-from solie.widget.horizontal_divider import HorizontalDivider
+from solie.common import go, outsource
+from solie.widget import BaseOverlay, HorizontalDivider, ask
 
 
-class DatapathInput(QtWidgets.QWidget):
-    def __init__(self, done_event: asyncio.Event, payload):
+class DatapathInput(BaseOverlay):
+    def __init__(self):
         # ■■■■■ the basic ■■■■■
 
         super().__init__()
 
         # ■■■■■ full layout ■■■■■
 
         full_layout = QtWidgets.QHBoxLayout(self)
@@ -75,57 +73,57 @@
         # spacing
         spacing_text = QtWidgets.QLabel("")
         spacing_text_font = QtGui.QFont()
         spacing_text_font.setPointSize(3)
         spacing_text.setFont(spacing_text_font)
         card_layout.addWidget(spacing_text)
 
-        datapath = ""
+        datapath: Path | None = None
 
         async def job_dp():
             nonlocal datapath
-            datapath = await go(xdialog.directory, title="Data folder")
-            folder_label.setText(datapath)
+            datapath = Path(await go(xdialog.directory, title="Data folder"))
+            folder_label.setText(str(datapath))
 
         # choose button
         this_layout = QtWidgets.QHBoxLayout()
         card_layout.addLayout(this_layout)
         choose_button = QtWidgets.QPushButton("Choose folder", card)
-        outsource.do(choose_button.clicked, job_dp)
+        outsource(choose_button.clicked, job_dp)
         choose_button.setSizePolicy(
             QtWidgets.QSizePolicy.Policy.Fixed,
             QtWidgets.QSizePolicy.Policy.Fixed,
         )
         this_layout.addWidget(choose_button)
 
         # ■■■■■ a card ■■■■■
 
+        self.result: Path
+
         async def job_ac():
-            if datapath == "":
-                question = [
+            if datapath is None:
+                await ask(
                     "Data folder is not chosen",
                     "Choose your data folder first.",
                     ["Okay"],
-                ]
-                await solie.window.ask(question)
+                )
             else:
-                await user_settings.apply_app_settings({"datapath": datapath})
-                await user_settings.load()
-                done_event.set()
+                self.result = datapath
+                self.done_event.set()
 
         # card structure
         card = QtWidgets.QGroupBox()
         card.setFixedWidth(720)
         card_layout = QtWidgets.QHBoxLayout(card)
         card_layout.setContentsMargins(80, 40, 80, 40)
         cards_layout.addWidget(card)
 
         # confirm button
         confirm_button = QtWidgets.QPushButton("Okay", card)
-        outsource.do(confirm_button.clicked, job_ac)
+        outsource(confirm_button.clicked, job_ac)
         confirm_button.setSizePolicy(
             QtWidgets.QSizePolicy.Policy.Fixed,
             QtWidgets.QSizePolicy.Policy.Fixed,
         )
         card_layout.addWidget(confirm_button)
 
         # ■■■■■ spacing ■■■■■
```

### Comparing `solie-8.4.0/solie/overlay/donation_guide.py` & `solie-8.5.0/solie/overlay/donation_guide.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-import asyncio
-
 from PySide6 import QtCore, QtWidgets
 
+from solie.widget import BaseOverlay
+
 
-class DonationGuide(QtWidgets.QWidget):
-    def __init__(self, done_event: asyncio.Event, payload):
+class DonationGuide(BaseOverlay):
+    def __init__(self):
         # ■■■■■ the basic ■■■■■
 
         super().__init__()
 
         # ■■■■■ full layout ■■■■■
 
         full_layout = QtWidgets.QHBoxLayout(self)
```

### Comparing `solie-8.4.0/solie/overlay/download_fill_option.py` & `solie-8.5.0/solie/overlay/download_fill_option.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,21 @@
-import asyncio
-
 from PySide6 import QtWidgets
 
-from solie.utility import outsource
+from solie.common import outsource
+from solie.widget import BaseOverlay
 
 
-class DownloadFillOption(QtWidgets.QWidget):
-    def __init__(self, done_event: asyncio.Event, payload):
+class DownloadFillOption(BaseOverlay):
+    def __init__(self):
         # ■■■■■ the basic ■■■■■
 
         super().__init__()
 
         # ■■■■■ prepare variables ■■■■■
 
-        answer_container = payload[0]
         fill_options = (
             "From 2020 to last year",
             "From first month of this year to last month",
             "This month",
             "Yesterday and the day before yesterday",
         )
 
@@ -61,22 +59,23 @@
         card = QtWidgets.QGroupBox()
         card.setFixedWidth(720)
         card_layout = QtWidgets.QVBoxLayout(card)
         card_layout.setContentsMargins(80, 40, 80, 40)
         cards_layout.addWidget(card)
 
         # option buttons
+        self.result: int | None = None
         for turn, text in enumerate(fill_options):
 
-            async def job(turn=turn, *args, **kwargs):
-                answer_container["filling_type"] = turn
-                done_event.set()
+            async def job(turn=turn):
+                self.result = turn
+                self.done_event.set()
 
             option_button = QtWidgets.QPushButton(text, card)
-            outsource.do(option_button.clicked, job)
+            outsource(option_button.clicked, job)
             card_layout.addWidget(option_button)
 
         # ■■■■■ spacing ■■■■■
 
         spacer = QtWidgets.QSpacerItem(
             0,
             0,
```

### Comparing `solie-8.4.0/solie/overlay/long_text_view.py` & `solie-8.5.0/solie/overlay/long_text_view.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,22 @@
-import asyncio
+from PySide6 import QtCore, QtWidgets
 
-from PySide6 import QtCore, QtGui, QtWidgets
+from solie.widget import BaseOverlay
 
 
-class LongTextView(QtWidgets.QWidget):
-    def __init__(self, done_event: asyncio.Event, payload):
+class LongTextView(BaseOverlay):
+    def __init__(self, long_text: str):
         # ■■■■■ the basic ■■■■■
 
         super().__init__()
 
-        long_text = payload[0]
-
         # ■■■■■ full layout ■■■■■
 
         full_layout = QtWidgets.QVBoxLayout(self)
         cards_layout = QtWidgets.QVBoxLayout()
         full_layout.addLayout(cards_layout)
 
         label = QtWidgets.QLabel(long_text)
-        fixed_width_font = QtGui.QFont("Source Code Pro", 9)
-        label.setFont(fixed_width_font)
         label.setTextInteractionFlags(
             QtCore.Qt.TextInteractionFlag.TextSelectableByMouse
         )
         cards_layout.addWidget(label)
```

### Comparing `solie-8.4.0/solie/overlay/strategy_basic_input.py` & `solie-8.5.0/solie/overlay/strategy_basic_input.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,22 @@
-import asyncio
 import re
 
 from PySide6 import QtCore, QtGui, QtWidgets
 
-import solie
-from solie.utility import compare_versions, outsource
-from solie.widget.horizontal_divider import HorizontalDivider
+from solie.common import PACKAGE_PATH, outsource
+from solie.utility import Strategy, is_left_version_higher
+from solie.widget import BaseOverlay, HorizontalDivider, ask
 
 
-class StrategyBasicInput(QtWidgets.QWidget):
-    def __init__(self, done_event: asyncio.Event, payload):
+class StrategyBasicInput(BaseOverlay):
+    def __init__(self, strategy: Strategy):
         # ■■■■■ the basic ■■■■■
 
         super().__init__()
 
-        # ■■■■■ prepare things ■■■■■
-
-        strategy = payload
-
         # ■■■■■ full layout ■■■■■
 
         full_layout = QtWidgets.QHBoxLayout(self)
         cards_layout = QtWidgets.QVBoxLayout()
         full_layout.addLayout(cards_layout)
 
         # ■■■■■ spacing ■■■■■
@@ -69,36 +64,37 @@
         spacing_text.setFont(spacing_text_font)
         card_layout.addWidget(spacing_text)
 
         # input
         this_layout = QtWidgets.QFormLayout()
         card_layout.addLayout(this_layout)
         code_name_input = QtWidgets.QLineEdit()
-        code_name_input.setText(strategy["code_name"])
+        code_name_input.setText(strategy.code_name)
         this_layout.addRow("Code name", code_name_input)
         readable_name_input = QtWidgets.QLineEdit()
-        readable_name_input.setText(strategy["readable_name"])
+        readable_name_input.setText(strategy.readable_name)
         this_layout.addRow("Readable name", readable_name_input)
         version_input = QtWidgets.QLineEdit()
-        version_input.setText(strategy["version"])
+        version_input.setText(strategy.version)
         this_layout.addRow("Version", version_input)
         description_input = QtWidgets.QTextEdit()
-        description_input.setPlainText(strategy["description"])
+        description_input.setPlainText(strategy.description)
         this_layout.addRow("Description", description_input)
         risk_level_input = QtWidgets.QComboBox()
+        iconpath = PACKAGE_PATH / "static" / "icon"
         red_pixmap = QtGui.QPixmap()
-        red_pixmap.load(f"{solie.PATH}/static/icon/traffic_light_red.png")
+        red_pixmap.load(str(iconpath / "traffic_light_red.png"))
         yellow_pixmap = QtGui.QPixmap()
-        yellow_pixmap.load(f"{solie.PATH}/static/icon/traffic_light_yellow.png")
+        yellow_pixmap.load(str(iconpath / "traffic_light_yellow.png"))
         green_pixmap = QtGui.QPixmap()
-        green_pixmap.load(f"{solie.PATH}/static/icon/traffic_light_green.png")
-        risk_level_input.addItem(red_pixmap, "High")
-        risk_level_input.addItem(yellow_pixmap, "Middle")
+        green_pixmap.load(str(iconpath / "traffic_light_green.png"))
         risk_level_input.addItem(green_pixmap, "Low")
-        risk_level_input.setCurrentIndex(strategy["risk_level"])
+        risk_level_input.addItem(yellow_pixmap, "Middle")
+        risk_level_input.addItem(red_pixmap, "High")
+        risk_level_input.setCurrentIndex(strategy.risk_level)
         this_layout.addRow("Risk level", risk_level_input)
 
         # ■■■■■ a card ■■■■■
 
         # card structure
         card = QtWidgets.QGroupBox()
         card.setFixedWidth(720)
@@ -131,80 +127,77 @@
         spacing_text.setFont(spacing_text_font)
         card_layout.addWidget(spacing_text)
 
         # input
         this_layout = QtWidgets.QFormLayout()
         card_layout.addLayout(this_layout)
         parallelized_input = QtWidgets.QCheckBox()
-        parallelized_input.setChecked(strategy["parallelized_simulation"])
+        parallelized_input.setChecked(strategy.parallelized_simulation)
         this_layout.addRow("Parallelized", parallelized_input)
         chunk_division_input = QtWidgets.QSpinBox()
         chunk_division_input.setSuffix(" days")
         chunk_division_input.setMinimum(7)
         chunk_division_input.setMaximum(90)
         chunk_division_input.setButtonSymbols(
             QtWidgets.QSpinBox.ButtonSymbols.NoButtons
         )
-        chunk_division_input.setValue(strategy["chunk_division"])
+        chunk_division_input.setValue(strategy.chunk_division)
         this_layout.addRow("Chunk division", chunk_division_input)
 
         # ■■■■■ a card ■■■■■
 
         # card structure
         card = QtWidgets.QGroupBox()
         card.setFixedWidth(720)
         card_layout = QtWidgets.QHBoxLayout(card)
         card_layout.setContentsMargins(80, 40, 80, 40)
         cards_layout.addWidget(card)
 
         # function
-        async def job(*args):
+        async def job():
             code_name = code_name_input.text()
             if re.fullmatch(r"[A-Z]{6}", code_name):
-                strategy["code_name"] = code_name
+                strategy.code_name = code_name
             else:
-                question = [
+                await ask(
                     "Code name format is wrong.",
                     "You should make the code name with 6 capital letters.",
                     ["Okay"],
-                ]
-                await solie.window.ask(question)
+                )
                 return
-            strategy["readable_name"] = readable_name_input.text()
+            strategy.readable_name = readable_name_input.text()
             version = version_input.text()
             if re.fullmatch(r"[0-9]+\.[0-9]+", version):
-                if not compare_versions.is_left_higher(strategy["version"], version):
-                    strategy["version"] = version
+                if not is_left_version_higher(strategy.version, version):
+                    strategy.version = version
                 else:
-                    question = [
+                    await ask(
                         "Version is lower.",
                         "You can't lower the version of your strategy. It should only"
                         " go up higher.",
                         ["Okay"],
-                    ]
-                    await solie.window.ask(question)
+                    )
                     return
             else:
-                question = [
+                await ask(
                     "Version format is wrong.",
                     "You should write the version in two numeric fields, divided by a"
                     " single dot.",
                     ["Okay"],
-                ]
-                await solie.window.ask(question)
+                )
                 return
-            strategy["description"] = description_input.toPlainText()
-            strategy["risk_level"] = risk_level_input.currentIndex()
-            strategy["parallelized_simulation"] = parallelized_input.isChecked()
-            strategy["chunk_division"] = chunk_division_input.value()
-            done_event.set()
+            strategy.description = description_input.toPlainText()
+            strategy.risk_level = risk_level_input.currentIndex()
+            strategy.parallelized_simulation = parallelized_input.isChecked()
+            strategy.chunk_division = chunk_division_input.value()
+            self.done_event.set()
 
         # confirm button
         confirm_button = QtWidgets.QPushButton("Save and close", card)
-        outsource.do(confirm_button.clicked, job)
+        outsource(confirm_button.clicked, job)
         confirm_button.setSizePolicy(
             QtWidgets.QSizePolicy.Policy.Fixed,
             QtWidgets.QSizePolicy.Policy.Fixed,
         )
         card_layout.addWidget(confirm_button)
 
         # ■■■■■ spacing ■■■■■
```

### Comparing `solie-8.4.0/solie/overlay/strategy_develop_input.py` & `solie-8.5.0/solie/overlay/strategy_develop_input.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,29 +1,23 @@
-import asyncio
 import webbrowser
 
 import aiofiles
 from PySide6 import QtCore, QtWidgets
 
-import solie
-from solie.parallel import go
-from solie.utility import outsource
-from solie.widget.script_editor import ScriptEditor
-from solie.widget.vertical_divider import VerticalDivider
+from solie.common import PACKAGE_PATH, go, outsource
+from solie.utility import Strategy
+from solie.widget import BaseOverlay, ScriptEditor, VerticalDivider, ask
 
 
-class StrategyDevelopInput(QtWidgets.QWidget):
-    def __init__(self, done_event: asyncio.Event, payload):
+class StrategyDevelopInput(BaseOverlay):
+    def __init__(self, strategy: Strategy):
         # ■■■■■ the basic ■■■■■
 
         super().__init__()
-
-        # ■■■■■ prepare things ■■■■■
-
-        strategy = payload
+        self.strategy = strategy
 
         # ■■■■■ full layout ■■■■■
 
         full_layout = QtWidgets.QVBoxLayout(self)
 
         # ■■■■■ script editors ■■■■■
 
@@ -38,31 +32,33 @@
         detail_text = QtWidgets.QLabel()
         detail_text.setText("Indicators script")
         detail_text.setAlignment(QtCore.Qt.AlignmentFlag.AlignCenter)
         column_layout.addWidget(detail_text)
 
         # input
         indicators_script_input = ScriptEditor(self)
-        indicators_script_input.setPlainText(strategy["indicators_script"])
+        indicators_script_input.setPlainText(strategy.indicators_script)
         column_layout.addWidget(indicators_script_input)
+        self.indicators_script_input = indicators_script_input
 
         # column layout
         column_layout = QtWidgets.QVBoxLayout()
         this_layout.addLayout(column_layout)
 
         # title
         detail_text = QtWidgets.QLabel()
         detail_text.setText("Decision script")
         detail_text.setAlignment(QtCore.Qt.AlignmentFlag.AlignCenter)
         column_layout.addWidget(detail_text)
 
         # input
         decision_script_input = ScriptEditor(self)
-        decision_script_input.setPlainText(strategy["decision_script"])
+        decision_script_input.setPlainText(strategy.decision_script)
         column_layout.addWidget(decision_script_input)
+        self.decision_script_input = decision_script_input
 
         # ■■■■■ a card ■■■■■
 
         # card structure
         card = QtWidgets.QGroupBox()
         card_layout = QtWidgets.QHBoxLayout(card)
         full_layout.addWidget(card)
@@ -72,53 +68,22 @@
             0,
             0,
             QtWidgets.QSizePolicy.Policy.Expanding,
             QtWidgets.QSizePolicy.Policy.Minimum,
         )
         card_layout.addItem(spacer)
 
-        # sample script button
-        async def job_as(*args):
-            # indicators script
-            filepath = f"{solie.PATH}/static/sample_indicators_script.txt"
-            async with aiofiles.open(filepath, "r", encoding="utf8") as file:
-                script = await file.read()
-
-            indicators_script_input.setPlainText(script)
-
-            # decision script
-            filepath = f"{solie.PATH}/static/sample_decision_script.txt"
-            async with aiofiles.open(filepath, "r", encoding="utf8") as file:
-                script = await file.read()
-
-            decision_script_input.setPlainText(script)
-
-            question = [
-                "Sample scripts applied",
-                "It is not yet saved. Modify the code as you want.",
-                ["Okay"],
-            ]
-            await solie.window.ask(question)
-
-        button = QtWidgets.QPushButton("Fill with sample", card)
-        outsource.do(button.clicked, job_as)
-        button.setSizePolicy(
-            QtWidgets.QSizePolicy.Policy.Fixed,
-            QtWidgets.QSizePolicy.Policy.Fixed,
-        )
-        card_layout.addWidget(button)
-
         # confirm button
-        async def job_ss(*args):
-            strategy["indicators_script"] = indicators_script_input.toPlainText()
-            strategy["decision_script"] = decision_script_input.toPlainText()
-            done_event.set()
+        async def job_ss():
+            strategy.indicators_script = indicators_script_input.toPlainText()
+            strategy.decision_script = decision_script_input.toPlainText()
+            self.done_event.set()
 
         button = QtWidgets.QPushButton("Save and close", card)
-        outsource.do(button.clicked, job_ss)
+        outsource(button.clicked, job_ss)
         button.setSizePolicy(
             QtWidgets.QSizePolicy.Policy.Fixed,
             QtWidgets.QSizePolicy.Policy.Fixed,
         )
         card_layout.addWidget(button)
 
         # Vertical divider
@@ -128,39 +93,86 @@
         # action menu
         action_menu = QtWidgets.QMenu(self)
         action_button = QtWidgets.QPushButton()
         action_button.setText("☰")
         action_button.setMenu(action_menu)
         card_layout.addWidget(action_button)
 
+        # sample script button
+        async def job_as():
+            # indicators script
+            filepath = PACKAGE_PATH / "static" / "sample_indicators_script.txt"
+            async with aiofiles.open(filepath, "r", encoding="utf8") as file:
+                script = await file.read()
+
+            indicators_script_input.setPlainText(script)
+
+            # decision script
+            filepath = PACKAGE_PATH / "static" / "sample_decision_script.txt"
+            async with aiofiles.open(filepath, "r", encoding="utf8") as file:
+                script = await file.read()
+
+            decision_script_input.setPlainText(script)
+
+            await ask(
+                "Sample scripts applied",
+                "It hasn't been saved yet,"
+                " feel free to customize the code to your liking.",
+                ["Okay"],
+            )
+
+        new_action = action_menu.addAction("Apply sample scripts")
+        outsource(new_action.triggered, job_as)
+
         # API docs button
-        async def job_ad(*args):
+        async def job_ad():
             url = "https://solie-docs.cunarist.com/making-strategy/"
             await go(webbrowser.open, url)
 
         new_action = action_menu.addAction("Show Solie API docs")
-        outsource.do(new_action.triggered, job_ad)
+        outsource(new_action.triggered, job_ad)
 
         # Pandas docs button
-        async def job_pd(*args):
+        async def job_pd():
             url = "https://pandas.pydata.org/docs/reference/index.html"
             await go(webbrowser.open, url)
 
         new_action = action_menu.addAction("Show Pandas API docs")
-        outsource.do(new_action.triggered, job_pd)
+        outsource(new_action.triggered, job_pd)
 
         # TA docs button
-        async def job_td(*args):
+        async def job_td():
             url = "https://github.com/twopirllc/pandas-ta#indicators-by-category"
             await go(webbrowser.open, url)
 
         new_action = action_menu.addAction("Show TA API docs")
-        outsource.do(new_action.triggered, job_td)
+        outsource(new_action.triggered, job_td)
 
         # spacing
         spacer = QtWidgets.QSpacerItem(
             0,
             0,
             QtWidgets.QSizePolicy.Policy.Expanding,
             QtWidgets.QSizePolicy.Policy.Minimum,
         )
         card_layout.addItem(spacer)
+
+    async def confirm_closing(self) -> bool:
+        strategy = self.strategy
+
+        written_decision = self.decision_script_input.toPlainText()
+        is_decision_script_saved = written_decision == strategy.decision_script
+        written_indicators = self.indicators_script_input.toPlainText()
+        is_indicators_script_saved = written_indicators == strategy.indicators_script
+        if is_decision_script_saved and is_indicators_script_saved:
+            return True
+
+        should_close = False
+        answer = await ask(
+            "Scripts are not saved yet",
+            "Are you sure you want to exit the editor without saving?",
+            ["Cancel", "Exit"],
+        )
+        if answer == 2:
+            should_close = True
+
+        return should_close
```

### Comparing `solie-8.4.0/solie/overlay/strategy_info_view.py` & `solie-8.5.0/solie/overlay/strategy_info_view.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,19 @@
-import asyncio
-
 from PySide6 import QtCore, QtGui, QtWidgets
 
-from solie.widget.horizontal_divider import HorizontalDivider
+from solie.utility import Strategy
+from solie.widget import BaseOverlay, HorizontalDivider
 
 
-class StrategyInfoView(QtWidgets.QWidget):
-    def __init__(self, done_event: asyncio.Event, payload):
+class StrategyInfoView(BaseOverlay):
+    def __init__(self, strategy: Strategy):
         # ■■■■■ the basic ■■■■■
 
         super().__init__()
 
-        # ■■■■■ prepare things ■■■■■
-
-        strategy = payload
-
         # ■■■■■ full layout ■■■■■
 
         full_layout = QtWidgets.QHBoxLayout(self)
         cards_layout = QtWidgets.QVBoxLayout()
         full_layout.addLayout(cards_layout)
 
         # ■■■■■ spacing ■■■■■
@@ -63,15 +58,15 @@
         spacing_text = QtWidgets.QLabel("")
         spacing_text_font = QtGui.QFont()
         spacing_text_font.setPointSize(3)
         spacing_text.setFont(spacing_text_font)
         card_layout.addWidget(spacing_text)
 
         # explanation
-        detail_text = QtWidgets.QLabel(strategy["description"])
+        detail_text = QtWidgets.QLabel(strategy.description)
         detail_text.setWordWrap(True)
         card_layout.addWidget(detail_text)
 
         # ■■■■■ spacing ■■■■■
 
         # spacing
         spacer = QtWidgets.QSpacerItem(
```

### Comparing `solie-8.4.0/solie/overlay/token_selection.py` & `solie-8.5.0/solie/overlay/token_selection.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,46 +1,48 @@
 import asyncio
 
 from PySide6 import QtCore, QtGui, QtWidgets
 
-import solie
-from solie.definition.api_requester import ApiRequester
-from solie.utility import outsource, user_settings
-from solie.widget.horizontal_divider import HorizontalDivider
+from solie.common import PACKAGE_PATH, outsource
+from solie.utility import ApiRequester
+from solie.widget import BaseOverlay, HorizontalDivider, ask
 
 
-class TokenSelection(QtWidgets.QWidget):
-    def __init__(self, done_event: asyncio.Event, payload):
+class TokenSelection(BaseOverlay):
+    def __init__(self):
         super().__init__()
         self.is_closed = False
 
-        asyncio.create_task(self.fill(done_event))
+        asyncio.create_task(self.fill(self.done_event))
 
     async def fill(self, done_event):
         # ■■■■■ for remembering ■■■■■
 
-        token_radioboxes = {}
+        token_radioboxes: dict[str, QtWidgets.QRadioButton] = {}
 
         # ■■■■■ prepare the api requester ■■■■■
 
         api_requester = ApiRequester()
 
         # ■■■■■ get all symbols ■■■■■
 
-        available_symbols = []
+        available_tokens: set[str] = set()
+        available_symbols: set[str] = set()
 
         response = await api_requester.binance(
             http_method="GET",
             path="/fapi/v1/exchangeInfo",
             payload={},
         )
         about_symbols = response["symbols"]
         for about_symbol in about_symbols:
+            token = about_symbol["marginAsset"]
+            available_tokens.add(token)
             symbol = about_symbol["symbol"]
-            available_symbols.append(symbol)
+            available_symbols.add(symbol)
 
         # ■■■■■ get coin informations ■■■■■
 
         response = await api_requester.coingecko(
             "GET",
             "/api/v3/coins/markets",
             {
@@ -56,15 +58,14 @@
             coin_symbol = about_coin["symbol"].upper()
             coin_names[coin_symbol] = about_coin["name"]
             coin_icon_urls[coin_symbol] = about_coin["image"]
             coin_ranks[coin_symbol] = about_coin["market_cap_rank"]
 
         # ■■■■■ set things ■■■■■
 
-        available_tokens = ["USDT", "BUSD"]
         number_of_markets = {token: 0 for token in available_tokens}
 
         for symbol in available_symbols:
             for token in available_tokens:
                 if symbol.endswith(token):
                     number_of_markets[token] += 1
 
@@ -91,15 +92,15 @@
         card.setFixedWidth(720)
         card_layout = QtWidgets.QVBoxLayout(card)
         card_layout.setContentsMargins(80, 40, 80, 40)
         cards_layout.addWidget(card)
 
         # explanation
         detail_text = QtWidgets.QLabel()
-        detail_text.setText("These are all available tokens on Binance.")
+        detail_text.setText("These are all the available tokens on Binance.")
         detail_text.setAlignment(QtCore.Qt.AlignmentFlag.AlignCenter)
         detail_text.setWordWrap(True)
         card_layout.addWidget(detail_text)
 
         # spacing
         spacing_text = QtWidgets.QLabel("")
         spacing_text_font = QtGui.QFont()
@@ -118,16 +119,16 @@
         spacing_text.setFont(spacing_text_font)
         card_layout.addWidget(spacing_text)
 
         # input
         token_icon_labels = {}
         input_layout = QtWidgets.QGridLayout()
         blank_coin_pixmap = QtGui.QPixmap()
-        blank_coin_pixmap.load(f"{solie.PATH}/static/icon/blank_coin.png")
-        for turn, token in enumerate(available_tokens):
+        blank_coin_pixmap.load(str(PACKAGE_PATH / "static" / "icon/blank_coin.png"))
+        for turn, token in enumerate(sorted(available_tokens)):
             this_layout = QtWidgets.QHBoxLayout()
             row = turn // 2
             column = turn % 2
             input_layout.addLayout(this_layout, row, column)
             radiobutton = QtWidgets.QRadioButton(card)
             token_radioboxes[token] = radiobutton
             this_layout.addWidget(radiobutton)
@@ -148,57 +149,51 @@
                 QtWidgets.QSizePolicy.Policy.Minimum,
             )
             this_layout.addItem(spacer)
         card_layout.addItem(input_layout)
 
         # ■■■■■ a card ■■■■■
 
+        self.result: str
+
         # confirm function
-        async def job_cf(*args):
-            data_settings = {}
+        async def job_cf():
             selected_tokens = []
             for symbol, radiobox in token_radioboxes.items():
                 is_selected = radiobox.isChecked()
                 if is_selected:
                     selected_tokens.append(symbol)
-            if len(selected_tokens) == 1:
-                is_symbol_count_ok = True
-                data_settings["asset_token"] = selected_tokens[0]
-            else:
-                is_symbol_count_ok = False
-                question = [
+            if len(selected_tokens) == 0:
+                await ask(
                     "Nothing selected",
                     "Choose one of the tokens.",
                     ["Okay"],
-                ]
-                await solie.window.ask(question)
-            if is_symbol_count_ok:
-                question = [
+                )
+            if len(selected_tokens) == 1:
+                answer = await ask(
                     "Okay to proceed?",
                     "Solie will treat this token as your asset.",
                     ["No", "Yes"],
-                ]
-                answer = await solie.window.ask(question)
+                )
                 if answer in (0, 1):
                     return
-                await user_settings.apply_data_settings(data_settings)
-                await user_settings.load()
                 self.is_closed = True
-                done_event.set()
+                self.result = selected_tokens[0]
+                self.done_event.set()
 
         # card structure
         card = QtWidgets.QGroupBox()
         card.setFixedWidth(720)
         card_layout = QtWidgets.QHBoxLayout(card)
         card_layout.setContentsMargins(80, 40, 80, 40)
         cards_layout.addWidget(card)
 
         # confirm button
         confirm_button = QtWidgets.QPushButton("Okay", card)
-        outsource.do(confirm_button.clicked, job_cf)
+        outsource(confirm_button.clicked, job_cf)
         confirm_button.setSizePolicy(
             QtWidgets.QSizePolicy.Policy.Fixed,
             QtWidgets.QSizePolicy.Policy.Fixed,
         )
         card_layout.addWidget(confirm_button)
 
         # ■■■■■ spacing ■■■■■
```

### Comparing `solie-8.4.0/solie/parallel.py` & `solie-8.5.0/solie/common/parallel.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,25 +2,21 @@
 import functools
 import multiprocessing
 from concurrent.futures import ProcessPoolExecutor
 from typing import Callable, TypeVar
 
 T = TypeVar("T")
 
+PROCESS_COUNT = multiprocessing.cpu_count()
+sync_manager = multiprocessing.Manager()
 
-def prepare():
-    global process_count
-    global process_pool
-    global communicator
 
-    # Use only half of the cores
-    # as stuffing all the cores with tasks leads to a system slowdown.
-    process_count = multiprocessing.cpu_count()
-    process_pool = ProcessPoolExecutor(process_count)
-    communicator = multiprocessing.Manager()
+def prepare_process_pool():
+    global process_pool
+    process_pool = ProcessPoolExecutor(PROCESS_COUNT)
 
 
 async def go(callable: Callable[..., T], *args, **kwargs) -> T:
     """
     Executes the given callable in a separate process pool
     using `asyncio`'s `run_in_executor`.
     This function is intended for executing blocking or CPU-bound operations
```

### Comparing `solie-8.4.0/solie/static/icon/blank_coin.png` & `solie-8.5.0/solie/static/icon/blank_coin.png`

 * *Files identical despite different names*

### Comparing `solie-8.4.0/solie/static/icon/traffic_light_green.png` & `solie-8.5.0/solie/static/icon/traffic_light_green.png`

 * *Files identical despite different names*

### Comparing `solie-8.4.0/solie/static/icon/traffic_light_red.png` & `solie-8.5.0/solie/static/icon/traffic_light_red.png`

 * *Files identical despite different names*

### Comparing `solie-8.4.0/solie/static/icon/traffic_light_yellow.png` & `solie-8.5.0/solie/static/icon/traffic_light_yellow.png`

 * *Files identical despite different names*

### Comparing `solie-8.4.0/solie/static/lexend_bold.ttf` & `solie-8.5.0/solie/static/lexend_bold.ttf`

 * *Files identical despite different names*

### Comparing `solie-8.4.0/solie/static/notosans_regular.ttf` & `solie-8.5.0/solie/static/notosans_regular.ttf`

 * *Files identical despite different names*

### Comparing `solie-8.4.0/solie/static/product_icon.ico` & `solie-8.5.0/solie/static/product_icon.ico`

 * *Files identical despite different names*

### Comparing `solie-8.4.0/solie/static/product_icon.png` & `solie-8.5.0/solie/static/product_icon.png`

 * *Files identical despite different names*

### Comparing `solie-8.4.0/solie/static/sample_decision_script.txt` & `solie-8.5.0/solie/static/sample_decision_script.txt`

 * *Files 21% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+import math
+from datetime import datetime, timedelta, timezone
+
 acquire_ratio = 0.8 / len(target_symbols)  # Split asset by symbol count
 wallet_balance = account_state["wallet_balance"]
 
 for symbol in target_symbols:
 
     current_price = current_candle_data[str((symbol, "Close"))]
```

### Comparing `solie-8.4.0/solie/static/sample_indicators_script.txt` & `solie-8.5.0/solie/static/sample_indicators_script.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+import numpy as np
+import pandas as pd
+import pandas_ta as ta
+
 short_period = 180
 long_period = 720
 
 for symbol in target_symbols:
 
     # Get candle data
     close_sr = candle_data[(symbol, "Close")]
```

### Comparing `solie-8.4.0/solie/static/source_code_pro.ttf` & `solie-8.5.0/solie/static/source_code_pro.ttf`

 * *Files identical despite different names*

### Comparing `solie-8.4.0/solie/user_interface.py` & `solie-8.5.0/solie/window/compiled.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
 ################################################################################
-## Form generated from reading UI file 'user_interface.ui'
+## Form generated from reading UI file 'window.ui'
 ##
-## Created by: Qt User Interface Compiler version 6.6.0
+## Created by: Qt User Interface Compiler version 6.6.2
 ##
 ## WARNING! All changes made in this file will be lost when recompiling UI file!
 ################################################################################
 
 from PySide6.QtCore import (QCoreApplication, QDate, QDateTime, QLocale,
     QMetaObject, QObject, QPoint, QRect,
     QSize, QTime, QUrl, Qt)
@@ -83,15 +83,15 @@
 "    max-height: 10em;\n"
 "    background: rgba(255,255,255,0.05);\n"
 "	border: 1px solid rgba(255,255,255,0.1);\n"
 " "
                         "   border-radius: 5em;\n"
 "}\n"
 "\n"
-"AskPopup, OverlayPanel {\n"
+"AskPopup, OverlayPopup {\n"
 "    background: rgba(0, 0, 0, 191);\n"
 "}\n"
 "\n"
 "PopupBox {\n"
 "    border: 1px solid rgba(255,255,255,0.1);\n"
 "    border-radius: 0.4em;\n"
 "    background: #2B2B2B;\n"
@@ -117,15 +117,15 @@
         self.board = QTabWidget(self.centralwidget)
         self.board.setObjectName(u"board")
         self.board.setTabPosition(QTabWidget.North)
         self.tab_5 = QWidget()
         self.tab_5.setObjectName(u"tab_5")
         self.verticalLayout_4 = QVBoxLayout(self.tab_5)
         self.verticalLayout_4.setObjectName(u"verticalLayout_4")
-        self.verticalSpacer_3 = QSpacerItem(20, 40, QSizePolicy.Minimum, QSizePolicy.Expanding)
+        self.verticalSpacer_3 = QSpacerItem(20, 40, QSizePolicy.Policy.Minimum, QSizePolicy.Policy.Expanding)
 
         self.verticalLayout_4.addItem(self.verticalSpacer_3)
 
         self.verticalLayout_14 = QVBoxLayout()
         self.verticalLayout_14.setObjectName(u"verticalLayout_14")
 
         self.verticalLayout_4.addLayout(self.verticalLayout_14)
@@ -136,32 +136,32 @@
         self.verticalLayout_4.addLayout(self.horizontalLayout_20)
 
         self.horizontalLayout_17 = QHBoxLayout()
         self.horizontalLayout_17.setObjectName(u"horizontalLayout_17")
 
         self.verticalLayout_4.addLayout(self.horizontalLayout_17)
 
-        self.verticalSpacer_4 = QSpacerItem(20, 40, QSizePolicy.Minimum, QSizePolicy.Expanding)
+        self.verticalSpacer_4 = QSpacerItem(20, 40, QSizePolicy.Policy.Minimum, QSizePolicy.Policy.Expanding)
 
         self.verticalLayout_4.addItem(self.verticalSpacer_4)
 
         self.horizontalLayout_21 = QHBoxLayout()
         self.horizontalLayout_21.setObjectName(u"horizontalLayout_21")
-        self.horizontalSpacer_17 = QSpacerItem(40, 20, QSizePolicy.Expanding, QSizePolicy.Minimum)
+        self.horizontalSpacer_17 = QSpacerItem(40, 20, QSizePolicy.Policy.Expanding, QSizePolicy.Policy.Minimum)
 
         self.horizontalLayout_21.addItem(self.horizontalSpacer_17)
 
         self.pushButton_9 = QPushButton(self.tab_5)
         self.pushButton_9.setObjectName(u"pushButton_9")
         self.pushButton_9.setStyleSheet(u"color:rgba(255,255,255,0.5)")
         self.pushButton_9.setFlat(True)
 
         self.horizontalLayout_21.addWidget(self.pushButton_9)
 
-        self.horizontalSpacer_18 = QSpacerItem(40, 20, QSizePolicy.Expanding, QSizePolicy.Minimum)
+        self.horizontalSpacer_18 = QSpacerItem(40, 20, QSizePolicy.Policy.Expanding, QSizePolicy.Policy.Minimum)
 
         self.horizontalLayout_21.addItem(self.horizontalSpacer_18)
 
 
         self.verticalLayout_4.addLayout(self.horizontalLayout_21)
 
         self.groupBox_10 = QGroupBox(self.tab_5)
@@ -179,15 +179,15 @@
 
         self.groupBox_6 = QGroupBox(self.tab_5)
         self.groupBox_6.setObjectName(u"groupBox_6")
         self.verticalLayout_17 = QVBoxLayout(self.groupBox_6)
         self.verticalLayout_17.setObjectName(u"verticalLayout_17")
         self.horizontalLayout_24 = QHBoxLayout()
         self.horizontalLayout_24.setObjectName(u"horizontalLayout_24")
-        self.horizontalSpacer_8 = QSpacerItem(40, 20, QSizePolicy.Expanding, QSizePolicy.Minimum)
+        self.horizontalSpacer_8 = QSpacerItem(40, 20, QSizePolicy.Policy.Expanding, QSizePolicy.Policy.Minimum)
 
         self.horizontalLayout_24.addItem(self.horizontalSpacer_8)
 
         self.pushButton_2 = QPushButton(self.groupBox_6)
         self.pushButton_2.setObjectName(u"pushButton_2")
 
         self.horizontalLayout_24.addWidget(self.pushButton_2)
@@ -196,23 +196,23 @@
         self.frame.setObjectName(u"frame")
         self.frame.setFrameShape(QFrame.VLine)
 
         self.horizontalLayout_24.addWidget(self.frame)
 
         self.pushButton_13 = QPushButton(self.groupBox_6)
         self.pushButton_13.setObjectName(u"pushButton_13")
-        sizePolicy = QSizePolicy(QSizePolicy.Fixed, QSizePolicy.Fixed)
+        sizePolicy = QSizePolicy(QSizePolicy.Policy.Fixed, QSizePolicy.Policy.Fixed)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(self.pushButton_13.sizePolicy().hasHeightForWidth())
         self.pushButton_13.setSizePolicy(sizePolicy)
 
         self.horizontalLayout_24.addWidget(self.pushButton_13)
 
-        self.horizontalSpacer_9 = QSpacerItem(40, 20, QSizePolicy.Expanding, QSizePolicy.Minimum)
+        self.horizontalSpacer_9 = QSpacerItem(40, 20, QSizePolicy.Policy.Expanding, QSizePolicy.Policy.Minimum)
 
         self.horizontalLayout_24.addItem(self.horizontalSpacer_9)
 
 
         self.verticalLayout_17.addLayout(self.horizontalLayout_24)
 
         self.horizontalLayout_12 = QHBoxLayout()
@@ -283,15 +283,15 @@
 
         self.groupBox = QGroupBox(self.tab)
         self.groupBox.setObjectName(u"groupBox")
         self.horizontalLayout_3 = QHBoxLayout(self.groupBox)
         self.horizontalLayout_3.setObjectName(u"horizontalLayout_3")
         self.label_16 = QLabel(self.groupBox)
         self.label_16.setObjectName(u"label_16")
-        sizePolicy1 = QSizePolicy(QSizePolicy.Preferred, QSizePolicy.Fixed)
+        sizePolicy1 = QSizePolicy(QSizePolicy.Policy.Preferred, QSizePolicy.Policy.Fixed)
         sizePolicy1.setHorizontalStretch(0)
         sizePolicy1.setVerticalStretch(0)
         sizePolicy1.setHeightForWidth(self.label_16.sizePolicy().hasHeightForWidth())
         self.label_16.setSizePolicy(sizePolicy1)
         font1 = QFont()
         self.label_16.setFont(font1)
         self.label_16.setAlignment(Qt.AlignCenter)
@@ -303,15 +303,15 @@
 
         self.groupBox_9 = QGroupBox(self.tab)
         self.groupBox_9.setObjectName(u"groupBox_9")
         self.verticalLayout_5 = QVBoxLayout(self.groupBox_9)
         self.verticalLayout_5.setObjectName(u"verticalLayout_5")
         self.horizontalLayout_15 = QHBoxLayout()
         self.horizontalLayout_15.setObjectName(u"horizontalLayout_15")
-        self.horizontalSpacer = QSpacerItem(0, 0, QSizePolicy.Expanding, QSizePolicy.Minimum)
+        self.horizontalSpacer = QSpacerItem(0, 0, QSizePolicy.Policy.Expanding, QSizePolicy.Policy.Minimum)
 
         self.horizontalLayout_15.addItem(self.horizontalSpacer)
 
         self.checkBox_2 = QCheckBox(self.groupBox_9)
         self.checkBox_2.setObjectName(u"checkBox_2")
         self.checkBox_2.setChecked(True)
 
@@ -354,24 +354,24 @@
 
         self.checkBox = QCheckBox(self.groupBox_9)
         self.checkBox.setObjectName(u"checkBox")
         self.checkBox.setMaximumSize(QSize(16777215, 16777215))
 
         self.horizontalLayout_15.addWidget(self.checkBox)
 
-        self.horizontalSpacer_3 = QSpacerItem(0, 0, QSizePolicy.Expanding, QSizePolicy.Minimum)
+        self.horizontalSpacer_3 = QSpacerItem(0, 0, QSizePolicy.Policy.Expanding, QSizePolicy.Policy.Minimum)
 
         self.horizontalLayout_15.addItem(self.horizontalSpacer_3)
 
 
         self.verticalLayout_5.addLayout(self.horizontalLayout_15)
 
         self.horizontalLayout_5 = QHBoxLayout()
         self.horizontalLayout_5.setObjectName(u"horizontalLayout_5")
-        self.horizontalSpacer_2 = QSpacerItem(40, 20, QSizePolicy.Expanding, QSizePolicy.Minimum)
+        self.horizontalSpacer_2 = QSpacerItem(40, 20, QSizePolicy.Policy.Expanding, QSizePolicy.Policy.Minimum)
 
         self.horizontalLayout_5.addItem(self.horizontalSpacer_2)
 
         self.label = QLabel(self.groupBox_9)
         self.label.setObjectName(u"label")
 
         self.horizontalLayout_5.addWidget(self.label)
@@ -435,15 +435,15 @@
         self.pushButton_12 = QPushButton(self.groupBox_9)
         self.pushButton_12.setObjectName(u"pushButton_12")
         sizePolicy.setHeightForWidth(self.pushButton_12.sizePolicy().hasHeightForWidth())
         self.pushButton_12.setSizePolicy(sizePolicy)
 
         self.horizontalLayout_5.addWidget(self.pushButton_12)
 
-        self.horizontalSpacer_4 = QSpacerItem(40, 20, QSizePolicy.Expanding, QSizePolicy.Minimum)
+        self.horizontalSpacer_4 = QSpacerItem(40, 20, QSizePolicy.Policy.Expanding, QSizePolicy.Policy.Minimum)
 
         self.horizontalLayout_5.addItem(self.horizontalSpacer_4)
 
 
         self.verticalLayout_5.addLayout(self.horizontalLayout_5)
 
         self.horizontalLayout_27 = QHBoxLayout()
@@ -526,15 +526,15 @@
         self.groupBox_3 = QGroupBox(self.tab_13)
         self.groupBox_3.setObjectName(u"groupBox_3")
         self.groupBox_3.setEnabled(True)
         self.verticalLayout_6 = QVBoxLayout(self.groupBox_3)
         self.verticalLayout_6.setObjectName(u"verticalLayout_6")
         self.horizontalLayout_23 = QHBoxLayout()
         self.horizontalLayout_23.setObjectName(u"horizontalLayout_23")
-        self.horizontalSpacer_21 = QSpacerItem(40, 20, QSizePolicy.Expanding, QSizePolicy.Minimum)
+        self.horizontalSpacer_21 = QSpacerItem(40, 20, QSizePolicy.Policy.Expanding, QSizePolicy.Policy.Minimum)
 
         self.horizontalLayout_23.addItem(self.horizontalSpacer_21)
 
         self.checkBox_3 = QCheckBox(self.groupBox_3)
         self.checkBox_3.setObjectName(u"checkBox_3")
 
         self.horizontalLayout_23.addWidget(self.checkBox_3)
@@ -613,24 +613,24 @@
         self.spinBox_2.setButtonSymbols(QAbstractSpinBox.NoButtons)
         self.spinBox_2.setCorrectionMode(QAbstractSpinBox.CorrectToNearestValue)
         self.spinBox_2.setMinimum(1)
         self.spinBox_2.setMaximum(100)
 
         self.horizontalLayout_23.addWidget(self.spinBox_2)
 
-        self.horizontalSpacer_22 = QSpacerItem(40, 20, QSizePolicy.Expanding, QSizePolicy.Minimum)
+        self.horizontalSpacer_22 = QSpacerItem(40, 20, QSizePolicy.Policy.Expanding, QSizePolicy.Policy.Minimum)
 
         self.horizontalLayout_23.addItem(self.horizontalSpacer_22)
 
 
         self.verticalLayout_6.addLayout(self.horizontalLayout_23)
 
         self.horizontalLayout_9 = QHBoxLayout()
         self.horizontalLayout_9.setObjectName(u"horizontalLayout_9")
-        self.horizontalSpacer_13 = QSpacerItem(40, 20, QSizePolicy.Expanding, QSizePolicy.Minimum)
+        self.horizontalSpacer_13 = QSpacerItem(40, 20, QSizePolicy.Policy.Expanding, QSizePolicy.Policy.Minimum)
 
         self.horizontalLayout_9.addItem(self.horizontalSpacer_13)
 
         self.label_23 = QLabel(self.groupBox_3)
         self.label_23.setObjectName(u"label_23")
 
         self.horizontalLayout_9.addWidget(self.label_23)
@@ -687,15 +687,15 @@
         self.pushButton_11 = QPushButton(self.groupBox_3)
         self.pushButton_11.setObjectName(u"pushButton_11")
         sizePolicy.setHeightForWidth(self.pushButton_11.sizePolicy().hasHeightForWidth())
         self.pushButton_11.setSizePolicy(sizePolicy)
 
         self.horizontalLayout_9.addWidget(self.pushButton_11)
 
-        self.horizontalSpacer_14 = QSpacerItem(40, 20, QSizePolicy.Expanding, QSizePolicy.Minimum)
+        self.horizontalSpacer_14 = QSpacerItem(40, 20, QSizePolicy.Policy.Expanding, QSizePolicy.Policy.Minimum)
 
         self.horizontalLayout_9.addItem(self.horizontalSpacer_14)
 
 
         self.verticalLayout_6.addLayout(self.horizontalLayout_9)
 
         self.horizontalLayout_8 = QHBoxLayout()
@@ -734,15 +734,15 @@
         self.horizontalLayout_25 = QHBoxLayout(self.groupBox_17)
         self.horizontalLayout_25.setObjectName(u"horizontalLayout_25")
         self.scrollArea_8 = QScrollArea(self.groupBox_17)
         self.scrollArea_8.setObjectName(u"scrollArea_8")
         self.scrollArea_8.setWidgetResizable(True)
         self.scrollAreaWidgetContents_8 = QWidget()
         self.scrollAreaWidgetContents_8.setObjectName(u"scrollAreaWidgetContents_8")
-        self.scrollAreaWidgetContents_8.setGeometry(QRect(0, 0, 1216, 611))
+        self.scrollAreaWidgetContents_8.setGeometry(QRect(0, 0, 280, 65))
         self.verticalLayout_19 = QVBoxLayout(self.scrollAreaWidgetContents_8)
         self.verticalLayout_19.setObjectName(u"verticalLayout_19")
         self.verticalLayout_16 = QVBoxLayout()
         self.verticalLayout_16.setObjectName(u"verticalLayout_16")
 
         self.verticalLayout_19.addLayout(self.verticalLayout_16)
 
@@ -754,15 +754,15 @@
         self.pushButton_5.setMaximumSize(QSize(260, 16777215))
 
         self.horizontalLayout_26.addWidget(self.pushButton_5)
 
 
         self.verticalLayout_19.addLayout(self.horizontalLayout_26)
 
-        self.verticalSpacer_5 = QSpacerItem(20, 40, QSizePolicy.Minimum, QSizePolicy.Expanding)
+        self.verticalSpacer_5 = QSpacerItem(20, 40, QSizePolicy.Policy.Minimum, QSizePolicy.Policy.Expanding)
 
         self.verticalLayout_19.addItem(self.verticalSpacer_5)
 
         self.scrollArea_8.setWidget(self.scrollAreaWidgetContents_8)
 
         self.horizontalLayout_25.addWidget(self.scrollArea_8)
 
@@ -778,21 +778,21 @@
         self.tabWidget.setObjectName(u"tabWidget")
         self.tab_9 = QWidget()
         self.tab_9.setObjectName(u"tab_9")
         self.verticalLayout_20 = QVBoxLayout(self.tab_9)
         self.verticalLayout_20.setObjectName(u"verticalLayout_20")
         self.horizontalLayout_34 = QHBoxLayout()
         self.horizontalLayout_34.setObjectName(u"horizontalLayout_34")
-        self.horizontalSpacer_15 = QSpacerItem(323, 20, QSizePolicy.Expanding, QSizePolicy.Minimum)
+        self.horizontalSpacer_15 = QSpacerItem(323, 20, QSizePolicy.Policy.Expanding, QSizePolicy.Policy.Minimum)
 
         self.horizontalLayout_34.addItem(self.horizontalSpacer_15)
 
         self.verticalLayout_18 = QVBoxLayout()
         self.verticalLayout_18.setObjectName(u"verticalLayout_18")
-        self.verticalSpacer_6 = QSpacerItem(20, 40, QSizePolicy.Minimum, QSizePolicy.Expanding)
+        self.verticalSpacer_6 = QSpacerItem(20, 40, QSizePolicy.Policy.Minimum, QSizePolicy.Policy.Expanding)
 
         self.verticalLayout_18.addItem(self.verticalSpacer_6)
 
         self.horizontalLayout_13 = QHBoxLayout()
         self.horizontalLayout_13.setObjectName(u"horizontalLayout_13")
 
         self.verticalLayout_18.addLayout(self.horizontalLayout_13)
@@ -825,22 +825,22 @@
         self.pushButton_7.setSizePolicy(sizePolicy)
 
         self.horizontalLayout_36.addWidget(self.pushButton_7)
 
 
         self.verticalLayout_18.addLayout(self.horizontalLayout_36)
 
-        self.verticalSpacer_7 = QSpacerItem(20, 40, QSizePolicy.Minimum, QSizePolicy.Expanding)
+        self.verticalSpacer_7 = QSpacerItem(20, 40, QSizePolicy.Policy.Minimum, QSizePolicy.Policy.Expanding)
 
         self.verticalLayout_18.addItem(self.verticalSpacer_7)
 
 
         self.horizontalLayout_34.addLayout(self.verticalLayout_18)
 
-        self.horizontalSpacer_16 = QSpacerItem(324, 20, QSizePolicy.Expanding, QSizePolicy.Minimum)
+        self.horizontalSpacer_16 = QSpacerItem(324, 20, QSizePolicy.Policy.Expanding, QSizePolicy.Policy.Minimum)
 
         self.horizontalLayout_34.addItem(self.horizontalSpacer_16)
 
 
         self.verticalLayout_20.addLayout(self.horizontalLayout_34)
 
         self.tabWidget.addTab(self.tab_9, "")
@@ -849,24 +849,24 @@
         self.verticalLayout_9 = QVBoxLayout(self.tab_4)
         self.verticalLayout_9.setObjectName(u"verticalLayout_9")
         self.scrollArea_9 = QScrollArea(self.tab_4)
         self.scrollArea_9.setObjectName(u"scrollArea_9")
         self.scrollArea_9.setWidgetResizable(True)
         self.scrollAreaWidgetContents_9 = QWidget()
         self.scrollAreaWidgetContents_9.setObjectName(u"scrollAreaWidgetContents_9")
-        self.scrollAreaWidgetContents_9.setGeometry(QRect(0, 0, 1212, 584))
+        self.scrollAreaWidgetContents_9.setGeometry(QRect(0, 0, 752, 466))
         self.horizontalLayout_6 = QHBoxLayout(self.scrollAreaWidgetContents_9)
         self.horizontalLayout_6.setObjectName(u"horizontalLayout_6")
-        self.horizontalSpacer_10 = QSpacerItem(40, 20, QSizePolicy.Expanding, QSizePolicy.Minimum)
+        self.horizontalSpacer_10 = QSpacerItem(40, 20, QSizePolicy.Policy.Expanding, QSizePolicy.Policy.Minimum)
 
         self.horizontalLayout_6.addItem(self.horizontalSpacer_10)
 
         self.verticalLayout_13 = QVBoxLayout()
         self.verticalLayout_13.setObjectName(u"verticalLayout_13")
-        self.verticalSpacer_2 = QSpacerItem(20, 40, QSizePolicy.Minimum, QSizePolicy.Expanding)
+        self.verticalSpacer_2 = QSpacerItem(20, 40, QSizePolicy.Policy.Minimum, QSizePolicy.Policy.Expanding)
 
         self.verticalLayout_13.addItem(self.verticalSpacer_2)
 
         self.groupBox_7 = QGroupBox(self.scrollAreaWidgetContents_9)
         self.groupBox_7.setObjectName(u"groupBox_7")
         self.groupBox_7.setMinimumSize(QSize(720, 0))
         self.groupBox_7.setMaximumSize(QSize(720, 16777215))
@@ -895,15 +895,15 @@
         self.label_43.setObjectName(u"label_43")
         self.label_43.setFont(font3)
 
         self.verticalLayout_22.addWidget(self.label_43)
 
         self.horizontalLayout_18 = QHBoxLayout()
         self.horizontalLayout_18.setObjectName(u"horizontalLayout_18")
-        self.horizontalSpacer_11 = QSpacerItem(40, 20, QSizePolicy.Expanding, QSizePolicy.Minimum)
+        self.horizontalSpacer_11 = QSpacerItem(40, 20, QSizePolicy.Policy.Expanding, QSizePolicy.Policy.Minimum)
 
         self.horizontalLayout_18.addItem(self.horizontalSpacer_11)
 
         self.formLayout = QFormLayout()
         self.formLayout.setObjectName(u"formLayout")
         self.label_5 = QLabel(self.groupBox_7)
         self.label_5.setObjectName(u"label_5")
@@ -937,15 +937,15 @@
         self.pushButton_22.setMaximumSize(QSize(360, 16777215))
 
         self.formLayout.setWidget(2, QFormLayout.FieldRole, self.pushButton_22)
 
 
         self.horizontalLayout_18.addLayout(self.formLayout)
 
-        self.horizontalSpacer_12 = QSpacerItem(40, 20, QSizePolicy.Expanding, QSizePolicy.Minimum)
+        self.horizontalSpacer_12 = QSpacerItem(40, 20, QSizePolicy.Policy.Expanding, QSizePolicy.Policy.Minimum)
 
         self.horizontalLayout_18.addItem(self.horizontalSpacer_12)
 
 
         self.verticalLayout_22.addLayout(self.horizontalLayout_18)
 
 
@@ -980,15 +980,15 @@
         self.label_49.setObjectName(u"label_49")
         self.label_49.setFont(font3)
 
         self.verticalLayout_30.addWidget(self.label_49)
 
         self.horizontalLayout_37 = QHBoxLayout()
         self.horizontalLayout_37.setObjectName(u"horizontalLayout_37")
-        self.horizontalSpacer_25 = QSpacerItem(40, 20, QSizePolicy.Expanding, QSizePolicy.Minimum)
+        self.horizontalSpacer_25 = QSpacerItem(40, 20, QSizePolicy.Policy.Expanding, QSizePolicy.Policy.Minimum)
 
         self.horizontalLayout_37.addItem(self.horizontalSpacer_25)
 
         self.formLayout_5 = QFormLayout()
         self.formLayout_5.setObjectName(u"formLayout_5")
         self.label_51 = QLabel(self.groupBox_11)
         self.label_51.setObjectName(u"label_51")
@@ -1009,32 +1009,32 @@
         self.comboBox_3.setMaximumSize(QSize(360, 16777215))
 
         self.formLayout_5.setWidget(0, QFormLayout.FieldRole, self.comboBox_3)
 
 
         self.horizontalLayout_37.addLayout(self.formLayout_5)
 
-        self.horizontalSpacer_26 = QSpacerItem(40, 20, QSizePolicy.Expanding, QSizePolicy.Minimum)
+        self.horizontalSpacer_26 = QSpacerItem(40, 20, QSizePolicy.Policy.Expanding, QSizePolicy.Policy.Minimum)
 
         self.horizontalLayout_37.addItem(self.horizontalSpacer_26)
 
 
         self.verticalLayout_30.addLayout(self.horizontalLayout_37)
 
 
         self.verticalLayout_13.addWidget(self.groupBox_11)
 
-        self.verticalSpacer = QSpacerItem(20, 40, QSizePolicy.Minimum, QSizePolicy.Expanding)
+        self.verticalSpacer = QSpacerItem(20, 40, QSizePolicy.Policy.Minimum, QSizePolicy.Policy.Expanding)
 
         self.verticalLayout_13.addItem(self.verticalSpacer)
 
 
         self.horizontalLayout_6.addLayout(self.verticalLayout_13)
 
-        self.horizontalSpacer_5 = QSpacerItem(40, 20, QSizePolicy.Expanding, QSizePolicy.Minimum)
+        self.horizontalSpacer_5 = QSpacerItem(40, 20, QSizePolicy.Policy.Expanding, QSizePolicy.Policy.Minimum)
 
         self.horizontalLayout_6.addItem(self.horizontalSpacer_5)
 
         self.scrollArea_9.setWidget(self.scrollAreaWidgetContents_9)
 
         self.verticalLayout_9.addWidget(self.scrollArea_9)
 
@@ -1085,29 +1085,29 @@
 
         self.groupBox_18 = QGroupBox(self.tab_6)
         self.groupBox_18.setObjectName(u"groupBox_18")
         self.verticalLayout_24 = QVBoxLayout(self.groupBox_18)
         self.verticalLayout_24.setObjectName(u"verticalLayout_24")
         self.horizontalLayout_2 = QHBoxLayout()
         self.horizontalLayout_2.setObjectName(u"horizontalLayout_2")
-        self.horizontalSpacer_6 = QSpacerItem(40, 20, QSizePolicy.Expanding, QSizePolicy.Minimum)
+        self.horizontalSpacer_6 = QSpacerItem(40, 20, QSizePolicy.Policy.Expanding, QSizePolicy.Policy.Minimum)
 
         self.horizontalLayout_2.addItem(self.horizontalSpacer_6)
 
         self.pushButton = QPushButton(self.groupBox_18)
         self.pushButton.setObjectName(u"pushButton")
 
         self.horizontalLayout_2.addWidget(self.pushButton)
 
         self.pushButton_6 = QPushButton(self.groupBox_18)
         self.pushButton_6.setObjectName(u"pushButton_6")
 
         self.horizontalLayout_2.addWidget(self.pushButton_6)
 
-        self.horizontalSpacer_7 = QSpacerItem(40, 20, QSizePolicy.Expanding, QSizePolicy.Minimum)
+        self.horizontalSpacer_7 = QSpacerItem(40, 20, QSizePolicy.Policy.Expanding, QSizePolicy.Policy.Minimum)
 
         self.horizontalLayout_2.addItem(self.horizontalSpacer_7)
 
 
         self.verticalLayout_24.addLayout(self.horizontalLayout_2)
 
 
@@ -1121,15 +1121,15 @@
         self.gridLayout = QGridLayout()
         self.gridLayout.setObjectName(u"gridLayout")
         self.scrollArea_6 = QScrollArea(self.tab_7)
         self.scrollArea_6.setObjectName(u"scrollArea_6")
         self.scrollArea_6.setWidgetResizable(True)
         self.scrollAreaWidgetContents_6 = QWidget()
         self.scrollAreaWidgetContents_6.setObjectName(u"scrollAreaWidgetContents_6")
-        self.scrollAreaWidgetContents_6.setGeometry(QRect(0, 0, 398, 265))
+        self.scrollAreaWidgetContents_6.setGeometry(QRect(0, 0, 81, 34))
         self.gridLayout_6 = QGridLayout(self.scrollAreaWidgetContents_6)
         self.gridLayout_6.setObjectName(u"gridLayout_6")
         self.label_33 = QLabel(self.scrollAreaWidgetContents_6)
         self.label_33.setObjectName(u"label_33")
         self.label_33.setAlignment(Qt.AlignCenter)
 
         self.gridLayout_6.addWidget(self.label_33, 0, 0, 1, 1)
@@ -1139,15 +1139,15 @@
         self.gridLayout.addWidget(self.scrollArea_6, 1, 2, 1, 1)
 
         self.scrollArea_4 = QScrollArea(self.tab_7)
         self.scrollArea_4.setObjectName(u"scrollArea_4")
         self.scrollArea_4.setWidgetResizable(True)
         self.scrollAreaWidgetContents_4 = QWidget()
         self.scrollAreaWidgetContents_4.setObjectName(u"scrollAreaWidgetContents_4")
-        self.scrollAreaWidgetContents_4.setGeometry(QRect(0, 0, 398, 265))
+        self.scrollAreaWidgetContents_4.setGeometry(QRect(0, 0, 81, 34))
         self.gridLayout_7 = QGridLayout(self.scrollAreaWidgetContents_4)
         self.gridLayout_7.setObjectName(u"gridLayout_7")
         self.label_35 = QLabel(self.scrollAreaWidgetContents_4)
         self.label_35.setObjectName(u"label_35")
         self.label_35.setAlignment(Qt.AlignCenter)
 
         self.gridLayout_7.addWidget(self.label_35, 0, 0, 1, 1)
@@ -1157,15 +1157,15 @@
         self.gridLayout.addWidget(self.scrollArea_4, 3, 1, 1, 1)
 
         self.scrollArea = QScrollArea(self.tab_7)
         self.scrollArea.setObjectName(u"scrollArea")
         self.scrollArea.setWidgetResizable(True)
         self.scrollAreaWidgetContents = QWidget()
         self.scrollAreaWidgetContents.setObjectName(u"scrollAreaWidgetContents")
-        self.scrollAreaWidgetContents.setGeometry(QRect(0, 0, 398, 265))
+        self.scrollAreaWidgetContents.setGeometry(QRect(0, 0, 81, 34))
         self.gridLayout_4 = QGridLayout(self.scrollAreaWidgetContents)
         self.gridLayout_4.setObjectName(u"gridLayout_4")
         self.label_12 = QLabel(self.scrollAreaWidgetContents)
         self.label_12.setObjectName(u"label_12")
         self.label_12.setAlignment(Qt.AlignCenter)
 
         self.gridLayout_4.addWidget(self.label_12, 0, 0, 1, 1)
@@ -1175,15 +1175,15 @@
         self.gridLayout.addWidget(self.scrollArea, 1, 0, 1, 1)
 
         self.scrollArea_5 = QScrollArea(self.tab_7)
         self.scrollArea_5.setObjectName(u"scrollArea_5")
         self.scrollArea_5.setWidgetResizable(True)
         self.scrollAreaWidgetContents_5 = QWidget()
         self.scrollAreaWidgetContents_5.setObjectName(u"scrollAreaWidgetContents_5")
-        self.scrollAreaWidgetContents_5.setGeometry(QRect(0, 0, 398, 265))
+        self.scrollAreaWidgetContents_5.setGeometry(QRect(0, 0, 81, 34))
         self.gridLayout_8 = QGridLayout(self.scrollAreaWidgetContents_5)
         self.gridLayout_8.setObjectName(u"gridLayout_8")
         self.label_36 = QLabel(self.scrollAreaWidgetContents_5)
         self.label_36.setObjectName(u"label_36")
         self.label_36.setAlignment(Qt.AlignCenter)
 
         self.gridLayout_8.addWidget(self.label_36, 0, 0, 1, 1)
@@ -1193,15 +1193,15 @@
         self.gridLayout.addWidget(self.scrollArea_5, 3, 0, 1, 1)
 
         self.scrollArea_3 = QScrollArea(self.tab_7)
         self.scrollArea_3.setObjectName(u"scrollArea_3")
         self.scrollArea_3.setWidgetResizable(True)
         self.scrollAreaWidgetContents_3 = QWidget()
         self.scrollAreaWidgetContents_3.setObjectName(u"scrollAreaWidgetContents_3")
-        self.scrollAreaWidgetContents_3.setGeometry(QRect(0, 0, 398, 265))
+        self.scrollAreaWidgetContents_3.setGeometry(QRect(0, 0, 81, 34))
         self.gridLayout_5 = QGridLayout(self.scrollAreaWidgetContents_3)
         self.gridLayout_5.setObjectName(u"gridLayout_5")
         self.label_32 = QLabel(self.scrollAreaWidgetContents_3)
         self.label_32.setObjectName(u"label_32")
         self.label_32.setAlignment(Qt.AlignCenter)
 
         self.gridLayout_5.addWidget(self.label_32, 0, 0, 1, 1)
@@ -1211,15 +1211,15 @@
         self.gridLayout.addWidget(self.scrollArea_3, 1, 1, 1, 1)
 
         self.scrollArea_7 = QScrollArea(self.tab_7)
         self.scrollArea_7.setObjectName(u"scrollArea_7")
         self.scrollArea_7.setWidgetResizable(True)
         self.scrollAreaWidgetContents_7 = QWidget()
         self.scrollAreaWidgetContents_7.setObjectName(u"scrollAreaWidgetContents_7")
-        self.scrollAreaWidgetContents_7.setGeometry(QRect(0, 0, 398, 265))
+        self.scrollAreaWidgetContents_7.setGeometry(QRect(0, 0, 81, 34))
         self.gridLayout_9 = QGridLayout(self.scrollAreaWidgetContents_7)
         self.gridLayout_9.setObjectName(u"gridLayout_9")
         self.label_34 = QLabel(self.scrollAreaWidgetContents_7)
         self.label_34.setObjectName(u"label_34")
         self.label_34.setAlignment(Qt.AlignCenter)
 
         self.gridLayout_9.addWidget(self.label_34, 0, 0, 1, 1)
@@ -1286,15 +1286,15 @@
 
         self.gridLayout_3.addWidget(self.gauge, 5, 0, 1, 1)
 
         MainWindow.setCentralWidget(self.centralwidget)
 
         self.retranslateUi(MainWindow)
 
-        self.board.setCurrentIndex(0)
+        self.board.setCurrentIndex(1)
         self.comboBox.setCurrentIndex(-1)
         self.tabWidget.setCurrentIndex(0)
 
 
         QMetaObject.connectSlotsByName(MainWindow)
     # setupUi
```

### Comparing `solie-8.4.0/solie/utility/check_internet.py` & `solie-8.5.0/solie/utility/check_internet.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 import asyncio
+import logging
 from typing import Callable, Coroutine
 
 import aiohttp
 
-import solie
+logger = logging.getLogger(__name__)
 
-is_checked = asyncio.Event()
-_was_connected = False
-_connected_functions: list[Callable[..., Coroutine]] = []
-_disconnected_functions: list[Callable[..., Coroutine]] = []
+is_internet_checked = asyncio.Event()
+was_connected = False
+connected_functions: list[Callable[[], Coroutine]] = []
+disconnected_functions: list[Callable[[], Coroutine]] = []
 
 
-def connected():
-    if is_checked.is_set():
-        return _was_connected
+def internet_connected():
+    if is_internet_checked.is_set():
+        return was_connected
     else:
         raise RuntimeError("Internet connection is not being monitored")
 
 
-async def monitor():
-    global _was_connected
+async def monitor_internet():
+    global was_connected
     while True:
         # try to connect to DNS servers
         attempt_ips = [
             "1.0.0.1",  # Cloudflare
             "1.1.1.1",  # Cloudflare
             "8.8.4.4",  # Google
             "8.8.8.8",  # Google
@@ -40,32 +41,32 @@
                         if response.status == 200:
                             is_connected = True
                             break
                 except Exception:
                     pass
 
         # detect changes
-        if _was_connected and not is_connected:
-            for job in _disconnected_functions:
+        if was_connected and not is_connected:
+            for job in disconnected_functions:
                 asyncio.create_task(job())
-            solie.logger.warning("Internet disconnected")
-        elif not _was_connected and is_connected:
-            for job in _connected_functions:
+            logger.warning("Internet disconnected")
+        elif not was_connected and is_connected:
+            for job in connected_functions:
                 asyncio.create_task(job())
-            solie.logger.info("Internet connected")
+            logger.info("Internet connected")
 
         # remember connection state
-        _was_connected = is_connected
-        is_checked.set()
+        was_connected = is_connected
+        is_internet_checked.set()
 
         # wait for a while
         await asyncio.sleep(1)
 
 
-def add_connected_functions(job: Callable[..., Coroutine]):
-    global _connected_functions
-    _connected_functions.append(job)
+def add_connected_functions(job: Callable[[], Coroutine]):
+    global connected_functions
+    connected_functions.append(job)
 
 
-def add_disconnected_functions(job: Callable[..., Coroutine]):
-    global _disconnected_functions
-    _disconnected_functions.append(job)
+def add_disconnected_functions(job: Callable[[], Coroutine]):
+    global disconnected_functions
+    disconnected_functions.append(job)
```

### Comparing `solie-8.4.0/solie/utility/convert.py` & `solie-8.5.0/solie/utility/convert.py`

 * *Files identical despite different names*

### Comparing `solie-8.4.0/solie/utility/examine_data_files.py` & `solie-8.5.0/solie/utility/backward_compatibility.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,76 +1,91 @@
 import json
-import os
+from pathlib import Path
 
 import aiofiles
+import aiofiles.os
 import pandas as pd
 
-from solie.parallel import go
-from solie.utility import user_settings
+from solie.common import go
 
 
-async def do():
-    datapath = user_settings.get_app_settings()["datapath"]
-
-    # 5.0: data settings
+async def examine_data_files(datapath: Path):
+    # 5.0: Data settings
     try:
-        filepath = f"{datapath}/basics.json"
+        filepath = datapath / "basics.json"
         async with aiofiles.open(filepath, "r", encoding="utf8") as file:
             content = await file.read()
             data_settings = json.loads(content)
-        os.remove(filepath)
-        filepath = f"{datapath}/data_settings.json"
+        await aiofiles.os.remove(filepath)
+        filepath = datapath / "data_settings.json"
         async with aiofiles.open(filepath, "w", encoding="utf8") as file:
-            content = json.dumps(data_settings, indent=4)
+            content = json.dumps(data_settings, indent=2)
             await file.write(content)
     except Exception:
         pass
 
-    # 5.0: symbol column was added to auto order record
+    # 5.0: Symbol column was added to auto order record
     try:
-        filepath = f"{datapath}/transactor/auto_order_record.pickle"
+        filepath = datapath / "transactor" / "auto_order_record.pickle"
         auto_order_record: pd.DataFrame = await go(pd.read_pickle, filepath)
         if "Symbol" not in auto_order_record.columns:
             auto_order_record["Symbol"] = ""
             await go(auto_order_record.to_pickle, filepath)
     except Exception:
         pass
 
-    # 5.0: solie default strategy now has strategy code SLSLDS
+    # 5.0: Solie default strategy now has strategy code SLSLDS
     try:
-        filepath = f"{datapath}/transactor/automation_settings.json"
+        filepath = datapath / "transactor" / "automation_settings.json"
         async with aiofiles.open(filepath, "r", encoding="utf8") as file:
             content = await file.read()
             automation_settings = json.loads(content)
         if automation_settings.get("strategy", None) == 2:
             automation_settings.pop("strategy")
             automation_settings["strategy_code"] = "SLSLDS"
         async with aiofiles.open(filepath, "w", encoding="utf8") as file:
-            content = json.dumps(automation_settings, indent=4)
+            content = json.dumps(automation_settings, indent=2)
             await file.write(content)
     except Exception:
         pass
 
-    # 6.0: use strategy index instead of strategy code
+    # 6.0: Use strategy index instead of strategy code
     try:
-        filepath = f"{datapath}/transactor/automation_settings.json"
+        filepath = datapath / "transactor" / "automation_settings.json"
         async with aiofiles.open(filepath, "r", encoding="utf8") as file:
             content = await file.read()
             automation_settings = json.loads(content)
         if "strategy_code" in automation_settings.keys():
             automation_settings.pop("strategy_code")
         if "strategy_index" not in automation_settings.keys():
             automation_settings["strategy_index"] = 0
         async with aiofiles.open(filepath, "w", encoding="utf8") as file:
-            content = json.dumps(automation_settings, indent=4)
+            content = json.dumps(automation_settings, indent=2)
             await file.write(content)
     except Exception:
         pass
 
-    # 6.3: auto_trade and manual_trade
+    # 6.3: Auto_trade and manual_trade
     try:
-        filepath = f"{datapath}/transactor/asset_record.pickle"
+        filepath = datapath / "transactor" / "asset_record.pickle"
         asset_record: pd.DataFrame = await go(pd.read_pickle, filepath)
         asset_record["Cause"] = asset_record["Cause"].replace("trade", "auto_trade")
         await go(asset_record.to_pickle, filepath)
     except Exception:
         pass
+
+    # 8.5: Now strategist has `Strategies` object instead of `list[dict]`
+    try:
+        filepath = datapath / "strategist" / "strategies.json"
+        async with aiofiles.open(filepath, "r", encoding="utf8") as file:
+            content = await file.read()
+            strategies = json.loads(content)
+        if not isinstance(strategies, list):
+            raise ValueError("Already good")
+        for strategy in strategies:
+            strategy["risk_level"] = 2 - strategy["risk_level"]  # Reversed
+        new_strategies = {"all": strategies}
+        async with aiofiles.open(filepath, "w", encoding="utf8") as file:
+            content = json.dumps(new_strategies, indent=2)
+            await file.write(content)
+    except Exception:
+        pass
```

### Comparing `solie-8.4.0/solie/utility/simulate_chunk.py` & `solie-8.5.0/solie/utility/analyze_market.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,53 +1,195 @@
+import itertools
 import math
 import random
+from dataclasses import dataclass
 from datetime import datetime, timedelta, timezone
+from multiprocessing.managers import ListProxy
+from types import CodeType
+from typing import Tuple
 
 import numpy as np
 import pandas as pd
+import pandas_ta as ta
 
-from solie.definition.errors import SimulationError
-from solie.utility import decide
 
+def make_indicators(
+    target_symbols: list[str],
+    candle_data: pd.DataFrame,
+    indicators_script: str | CodeType,
+    only_last_index: bool = False,
+) -> pd.DataFrame:
+    # ■■■■■ interpolate nans ■■■■■
 
-def do(dataset):
+    candle_data = candle_data.interpolate()
+
+    # ■■■■■ make dummy row to avoid ta error with all nan series ■■■■■
+
+    if len(candle_data) > 0:
+        dummy_index = candle_data.index[-1] + timedelta(seconds=1)
+    else:
+        dummy_index = datetime.fromtimestamp(0, tz=timezone.utc)
+
+    candle_data.loc[dummy_index, :] = 0.0
+
+    # ■■■■■ basic values ■■■■■
+
+    blank_columns = itertools.product(
+        target_symbols,
+        ("Price", "Volume", "Abstract"),
+        ("Blank",),
+    )
+    new_indicators: dict[tuple, pd.Series] = {}
+    base_index = candle_data.index
+    for blank_column in blank_columns:
+        new_indicators[blank_column] = pd.Series(
+            np.nan,
+            index=base_index,
+            dtype=np.float32,
+        )
+
+    # ■■■■■ make individual indicators ■■■■■
+
+    namespace = {
+        "ta": ta,
+        "pd": pd,
+        "np": np,
+        "target_symbols": target_symbols,
+        "candle_data": candle_data,
+        "new_indicators": new_indicators,
+    }
+    exec(indicators_script, namespace)
+    new_indicators = {k: v for k, v in new_indicators.items() if v is not None}
+
+    # ■■■■■ concatenate individual indicators into one ■■■■■
+
+    for column_name, new_indicator in new_indicators.items():
+        new_indicator.name = column_name
+
+    indicators = pd.concat(new_indicators.values(), axis="columns")
+    indicators = indicators.astype(np.float32)
+
+    # ■■■■■ remove dummy row ■■■■■
+
+    indicators = indicators.iloc[:-1]
+
+    if only_last_index:
+        return indicators.tail(1)
+    else:
+        return indicators
+
+
+def decide(
+    target_symbols: list[str],
+    current_moment: datetime,
+    current_candle_data: np.record,
+    current_indicators: np.record,
+    account_state: dict,
+    scribbles: dict,
+    decision_script: str | CodeType,
+) -> Tuple[dict, dict]:
+    # ■■■■■ decision template ■■■■■
+
+    decision = {}
+    for symbol in target_symbols:
+        decision[symbol] = {}
+
+    # ■■■■■ write decisions ■■■■■
+
+    namespace = {
+        "datetime": datetime,
+        "timezone": timezone,
+        "timedelta": timedelta,
+        "math": math,
+        "target_symbols": target_symbols,
+        "current_moment": current_moment,
+        "current_candle_data": current_candle_data,
+        "current_indicators": current_indicators,
+        "account_state": account_state,
+        "scribbles": scribbles,
+        "decision": decision,
+    }
+
+    exec(decision_script, namespace)
+
+    # ■■■■■ return decision ■■■■■
+
+    blank_symbols = []
+    for symbol, symbol_decision in decision.items():
+        if len(symbol_decision) == 0:
+            blank_symbols.append(symbol)
+    for blank_symbol in blank_symbols:
+        decision.pop(blank_symbol)
+
+    return decision, scribbles
+
+
+class SimulationError(Exception):
+    pass
+
+
+@dataclass
+class CalculationInput:
+    progress_list: ListProxy
+    target_progress: int
+    target_symbols: list[str]
+    calculation_index: pd.DatetimeIndex
+    chunk_candle_data: pd.DataFrame
+    chunk_indicators: pd.DataFrame
+    chunk_asset_record: pd.DataFrame
+    chunk_unrealized_changes: pd.Series
+    chunk_scribbles: dict
+    chunk_account_state: dict
+    chunk_virtual_state: dict
+    decision_script: str
+
+
+@dataclass
+class CalculationOutput:
+    chunk_asset_record: pd.DataFrame
+    chunk_unrealized_changes: pd.Series
+    chunk_scribbles: dict
+    chunk_account_state: dict
+    chunk_virtual_state: dict
+
+
+def simulate_chunk(calculation_input: CalculationInput) -> CalculationOutput:
     # leverage is treated as 1
     # because those are going to be applied at the presentation phase
 
     # ■■■■■ get data ■■■■■
 
-    progress_list = dataset["progress_list"]
-    target_progress = dataset["target_progress"]
-    target_symbols = dataset["target_symbols"]
-    calculation_index: pd.DatetimeIndex = dataset["calculation_index"]
-    chunk_candle_data: pd.DataFrame = dataset["chunk_candle_data"]
-    chunk_indicators: pd.DataFrame = dataset["chunk_indicators"]
-    chunk_asset_record: pd.DataFrame = dataset["chunk_asset_record"]
-    chunk_unrealized_changes: pd.Series = dataset["chunk_unrealized_changes"]
-    chunk_scribbles: dict = dataset["chunk_scribbles"]
-    chunk_account_state: dict = dataset["chunk_account_state"]
-    chunk_virtual_state: dict = dataset["chunk_virtual_state"]
-    decision_script: str = dataset["decision_script"]
+    progress_list = calculation_input.progress_list
+    target_progress = calculation_input.target_progress
+    target_symbols = calculation_input.target_symbols
+    calculation_index = calculation_input.calculation_index
+    chunk_candle_data = calculation_input.chunk_candle_data
+    chunk_indicators = calculation_input.chunk_indicators
+    chunk_asset_record = calculation_input.chunk_asset_record
+    chunk_unrealized_changes = calculation_input.chunk_unrealized_changes
+    chunk_scribbles = calculation_input.chunk_scribbles
+    chunk_account_state = calculation_input.chunk_account_state
+    chunk_virtual_state = calculation_input.chunk_virtual_state
+    decision_script = calculation_input.decision_script
 
     # ■■■■■ basic values ■■■■■
 
     decision_lag = 3000  # milliseconds
 
     # ■■■■■ return blank data if there's nothing to calculate ■■■■■
 
     if len(calculation_index) == 0:
-        dataset = {
-            "chunk_asset_record": chunk_asset_record,
-            "chunk_unrealized_changes": chunk_unrealized_changes,
-            "chunk_scribbles": chunk_scribbles,
-            "chunk_account_state": chunk_account_state,
-            "chunk_virtual_state": chunk_virtual_state,
-        }
-
-        return dataset
+        calculation_output = CalculationOutput(
+            chunk_asset_record=chunk_asset_record,
+            chunk_unrealized_changes=chunk_unrealized_changes,
+            chunk_scribbles=chunk_scribbles,
+            chunk_account_state=chunk_account_state,
+            chunk_virtual_state=chunk_virtual_state,
+        )
+        return calculation_output
 
     # ■■■■■ convert to numpy objects for fast calculation ■■■■■
 
     calculation_index_ar = calculation_index.to_numpy()  # inside are datetime objects
     candle_data_ar = chunk_candle_data.to_records()
     indicators_ar = chunk_indicators.to_records()
     asset_record_ar = chunk_asset_record.to_records()
@@ -482,15 +624,15 @@
         chunk_unrealized_changes_ar[-1]["index"] = before_moment
         chunk_unrealized_changes_ar[-1]["0"] = unrealized_change
 
         # ■■■■■ make decision and place order ■■■■■
 
         current_candle_data: np.record = candle_data_ar[cycle]
         current_indicators: np.record = indicators_ar[cycle]
-        decision, chunk_scribbles = decide.choose(
+        decision, chunk_scribbles = decide(
             target_symbols=target_symbols,
             current_moment=current_moment,
             current_candle_data=current_candle_data,
             current_indicators=current_indicators,
             account_state=chunk_account_state.copy(),
             scribbles=chunk_scribbles,
             decision_script=decision_script_compiled,
@@ -522,16 +664,15 @@
     chunk_unrealized_changes_df.index = pd.to_datetime(
         chunk_unrealized_changes_df.index, utc=True
     )
     chunk_unrealized_changes = chunk_unrealized_changes_df["0"]
 
     # ■■■■■ return calculated data ■■■■■
 
-    dataset = {
-        "chunk_asset_record": chunk_asset_record,
-        "chunk_unrealized_changes": chunk_unrealized_changes,
-        "chunk_scribbles": chunk_scribbles,
-        "chunk_account_state": chunk_account_state,
-        "chunk_virtual_state": chunk_virtual_state,
-    }
-
-    return dataset
+    calculation_output = CalculationOutput(
+        chunk_asset_record=chunk_asset_record,
+        chunk_unrealized_changes=chunk_unrealized_changes,
+        chunk_scribbles=chunk_scribbles,
+        chunk_account_state=chunk_account_state,
+        chunk_virtual_state=chunk_virtual_state,
+    )
+    return calculation_output
```

### Comparing `solie-8.4.0/solie/widget/ask_popup.py` & `solie-8.5.0/solie/widget/ask_popup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,40 +1,62 @@
 import asyncio
 
 from PySide6 import QtCore, QtGui, QtWidgets
 
-from solie.utility import outsource
-from solie.widget.popup_box import PopupBox
+from solie.common import outsource
+
+from .popup_box import PopupBox
 
 # https://stackoverflow.com/questions/67029993/pyqt-creating-a-popup-in-the-window
 
 
+# show an ask popup and blocks the stack
+async def ask(main_text: str, detail_text: str, options: list[str]) -> int:
+    ask_popup = AskPopup(main_text, detail_text, options)
+    ask_popup.show()
+
+    await ask_popup.done_event.wait()
+    ask_popup.setParent(None)
+
+    return ask_popup.answer
+
+
 class AskPopup(QtWidgets.QWidget):
     done_event = asyncio.Event()
+    installed_window: QtWidgets.QMainWindow
 
     def showEvent(self, event):  # noqa:N802
         # needed for filling the window when resized
         parent: QtWidgets.QMainWindow = self.parent()  # type:ignore
         self.setGeometry(parent.rect())
 
     def eventFilter(self, source, event):  # noqa:N802
         # needed for filling the window when resized
         if event.type() == event.Type.Resize:
             self.setGeometry(source.rect())
         return super().eventFilter(source, event)
 
-    def __init__(self, parent, question):
+    @classmethod
+    def install_window(cls, window: QtWidgets.QMainWindow):
+        cls.installed_window = window
+
+    def __init__(
+        self,
+        main_text: str,
+        detail_text: str,
+        options: list[str],
+    ):
         # ■■■■■ the basic ■■■■■
 
-        super().__init__(parent)
+        super().__init__(self.installed_window)
 
         # ■■■■■ set properties ■■■■■
 
         # needed for filling the window when resized
-        parent.installEventFilter(self)
+        self.installed_window.installEventFilter(self)
 
         # ■■■■■ in case other ask popup exists ■■■■■
 
         self.done_event.set()
         self.done_event.clear()
 
         # ■■■■■ prepare answer ■■■■■
@@ -73,67 +95,67 @@
         close_button_font = QtGui.QFont()
         close_button_font.setPointSize(11)
         close_button.setFont(close_button_font)
 
         async def job_de():
             self.done_event.set()
 
-        outsource.do(close_button.clicked, job_de)
+        outsource(close_button.clicked, job_de)
         this_layout.addWidget(close_button)
         content_box_layout.addLayout(this_layout)
 
         # spacing
         widget = QtWidgets.QSpacerItem(
             0,
             0,
             QtWidgets.QSizePolicy.Policy.Minimum,
             QtWidgets.QSizePolicy.Policy.Expanding,
         )
         content_box_layout.addItem(widget)
 
         # title
-        main_text = QtWidgets.QLabel()
-        main_text.setText(question[0])
-        main_text.setAlignment(QtCore.Qt.AlignmentFlag.AlignCenter)
+        main_text_widget = QtWidgets.QLabel()
+        main_text_widget.setText(main_text)
+        main_text_widget.setAlignment(QtCore.Qt.AlignmentFlag.AlignCenter)
         main_text_font = QtGui.QFont()
         main_text_font.setPointSize(12)
-        main_text.setFont(main_text_font)
-        main_text.setWordWrap(True)
-        content_box_layout.addWidget(main_text)
+        main_text_widget.setFont(main_text_font)
+        main_text_widget.setWordWrap(True)
+        content_box_layout.addWidget(main_text_widget)
 
         # spacing
         spacing_text = QtWidgets.QLabel("")
         spacing_text_font = QtGui.QFont()
         spacing_text_font.setPointSize(3)
         spacing_text.setFont(spacing_text_font)
         content_box_layout.addWidget(spacing_text)
 
         # explanation
-        detail_text = QtWidgets.QLabel()
-        detail_text.setText(question[1])
-        detail_text.setAlignment(QtCore.Qt.AlignmentFlag.AlignCenter)
-        detail_text.setWordWrap(True)
-        content_box_layout.addWidget(detail_text)
+        detail_text_widget = QtWidgets.QLabel()
+        detail_text_widget.setText(detail_text)
+        detail_text_widget.setAlignment(QtCore.Qt.AlignmentFlag.AlignCenter)
+        detail_text_widget.setWordWrap(True)
+        content_box_layout.addWidget(detail_text_widget)
 
         # spacing
         widget = QtWidgets.QSpacerItem(
             0,
             0,
             QtWidgets.QSizePolicy.Policy.Minimum,
             QtWidgets.QSizePolicy.Policy.Expanding,
         )
         content_box_layout.addItem(widget)
 
         # line including selection buttons
         this_layout = QtWidgets.QHBoxLayout()
-        for turn, option in enumerate(question[2]):
+        for turn, option in enumerate(options):
             option_button = QtWidgets.QPushButton(option, content_box)
 
-            async def job(answer=turn + 1, *args, **kwargs):
+            async def job(answer=turn + 1):
                 self.answer = answer
                 self.done_event.set()
 
-            outsource.do(option_button.clicked, job)
+            outsource(option_button.clicked, job)
             option_button.setMaximumWidth(240)
             this_layout.addWidget(option_button)
 
         content_box_layout.addLayout(this_layout)
```

### Comparing `solie-8.4.0/solie/widget/gauge.py` & `solie-8.5.0/solie/widget/gauge.py`

 * *Files identical despite different names*

### Comparing `solie-8.4.0/solie/widget/log_list.py` & `solie-8.5.0/solie/widget/log_list.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,43 @@
 from PySide6 import QtCore, QtGui, QtWidgets
 
-import solie
-from solie.overlay.long_text_view import LongTextView
-from solie.utility import outsource
+from solie.common import outsource
+
+from .overlay_popup import BaseOverlay, overlay
+
+
+class LogOverlay(BaseOverlay):
+    def __init__(self, log_content: str):
+        # ■■■■■ the basic ■■■■■
+
+        super().__init__()
+
+        # ■■■■■ full layout ■■■■■
+
+        full_layout = QtWidgets.QVBoxLayout(self)
+        cards_layout = QtWidgets.QVBoxLayout()
+        full_layout.addLayout(cards_layout)
+
+        label = QtWidgets.QLabel(log_content)
+        fixed_width_font = QtGui.QFont("Source Code Pro", 9)
+        label.setFont(fixed_width_font)
+        label.setTextInteractionFlags(
+            QtCore.Qt.TextInteractionFlag.TextSelectableByMouse
+        )
+        cards_layout.addWidget(label)
 
 
 class LogList(QtWidgets.QListWidget):
     def __init__(self, parent):
         super().__init__(parent)
         self.fixed_width_font = QtGui.QFont("Source Code Pro", 9)
         self.setFont(self.fixed_width_font)
-        outsource.do(self.itemClicked, self.show_fulltext)
+        outsource(self.itemClicked, self.show_fulltext)
 
-    def addItem(self, summarization: str, log_content: str):  # noqa:N802
+    def add_item(self, summarization: str, log_content: str):
         maximum_item_limit = 1024
 
         new_item = QtWidgets.QListWidgetItem(self)
         new_item.setText(summarization)
         new_item.setData(QtCore.Qt.ItemDataRole.UserRole, log_content)
 
         super().addItem(new_item)
@@ -24,15 +45,17 @@
         index_count = self.count()
 
         if index_count > maximum_item_limit:
             remove_count = index_count - maximum_item_limit
             for _ in range(remove_count):
                 self.takeItem(0)
 
-    async def show_fulltext(self, *args, **kwargs):
+    async def show_fulltext(self):
         selected_index = self.currentRow()
 
         selected_item = self.item(selected_index)
         text = selected_item.data(QtCore.Qt.ItemDataRole.UserRole)
 
-        formation = ["This is the full log", LongTextView, True, [text]]
-        await solie.window.overlay(formation)
+        await overlay(
+            "This is the full log",
+            LogOverlay(text),
+        )
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `solie-8.4.0/solie/widget/overlay_panel.py` & `solie-8.5.0/solie/widget/overlay_popup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,46 +1,77 @@
+# https://stackoverflow.com/questions/67029993/pyqt-creating-a-popup-in-the-window
 import asyncio
+from typing import TypeVar
 
 from PySide6 import QtCore, QtGui, QtWidgets
 
-from solie.utility import outsource
-from solie.widget.popup_box import PopupBox
-from solie.widget.transparent_scroll_area import TransparentScrollArea
+from solie.common import outsource
 
-# https://stackoverflow.com/questions/67029993/pyqt-creating-a-popup-in-the-window
+from .popup_box import PopupBox
+from .transparent_scroll_area import TransparentScrollArea
 
 
-class OverlayPanel(QtWidgets.QWidget):
+class BaseOverlay(QtWidgets.QWidget):
     done_event = asyncio.Event()
 
+    async def confirm_closing(self) -> bool:
+        return True
+
+
+W = TypeVar("W", bound=BaseOverlay)
+
+
+# show an mainpulatable overlap popup
+async def overlay(title: str, widget: W, close_button=True) -> W:
+    overlay_panel = OverlayPopup(title, widget, close_button)
+    overlay_panel.show()
+
+    await widget.done_event.wait()
+    overlay_panel.setParent(None)
+
+    return widget
+
+
+class OverlayPopup(QtWidgets.QWidget):
+    installed_window: QtWidgets.QMainWindow
+
     def showEvent(self, event):  # noqa:N802
         # needed for filling the window when resized
         parent: QtWidgets.QMainWindow = self.parent()  # type:ignore
         self.setGeometry(parent.rect())
 
     def eventFilter(self, source, event):  # noqa:N802
         # needed for filling the window when resized
         if event.type() == event.Type.Resize:
             self.setGeometry(source.rect())
         return super().eventFilter(source, event)
 
-    def __init__(self, parent, formation):
+    @classmethod
+    def install_window(cls, window: QtWidgets.QMainWindow):
+        cls.installed_window = window
+
+    def __init__(
+        self,
+        title: str,
+        widget: BaseOverlay,
+        close_button: bool,
+    ):
         # ■■■■■ the basic ■■■■■
 
-        super().__init__(parent)
+        super().__init__(self.installed_window)
 
         # ■■■■■ set properties ■■■■■
 
         # needed for filling the window when resized
-        parent.installEventFilter(self)
+        self.installed_window.installEventFilter(self)
 
-        # ■■■■■ in case other ask popup exists ■■■■■
+        # ■■■■■ in case other overlay popup exists ■■■■■
 
-        self.done_event.set()
-        self.done_event.clear()
+        widget.done_event.set()
+        widget.done_event.clear()
 
         # ■■■■■ prepare answer ■■■■■
 
         self.answer = 0
 
         # ■■■■■ full structure ■■■■■
 
@@ -59,41 +90,42 @@
         content_box.setAutoFillBackground(True)
         content_box.setMaximumSize(1600, 1200)
         content_box_layout = QtWidgets.QVBoxLayout(content_box)
         full_layout.addWidget(content_box)
 
         # line containing the title and close button
         this_layout = QtWidgets.QHBoxLayout()
-        title_label = QtWidgets.QLabel(formation[0])
+        title_label = QtWidgets.QLabel(title)
         title_label_font = QtGui.QFont()
         title_label_font.setPointSize(12)
         title_label.setFont(title_label_font)
         title_label.setWordWrap(False)
         this_layout.addWidget(title_label)
-        widget = QtWidgets.QSpacerItem(
+        top_widget = QtWidgets.QSpacerItem(
             0,
             0,
             QtWidgets.QSizePolicy.Policy.Expanding,
             QtWidgets.QSizePolicy.Policy.Minimum,
         )
-        this_layout.addItem(widget)
-        if formation[2]:
-            close_button = QtWidgets.QPushButton("✕", content_box)
+        this_layout.addItem(top_widget)
+        if close_button:
+            close_button_widget = QtWidgets.QPushButton("✕", content_box)
             close_button_font = QtGui.QFont()
             close_button_font.setPointSize(11)
-            close_button.setFont(close_button_font)
+            close_button_widget.setFont(close_button_font)
 
             async def job():
-                self.done_event.set()
+                should_close = await widget.confirm_closing()
+                if should_close:
+                    widget.done_event.set()
 
-            outsource.do(close_button.clicked, job)
-            this_layout.addWidget(close_button)
+            outsource(close_button_widget.clicked, job)
+            this_layout.addWidget(close_button_widget)
         content_box_layout.addLayout(this_layout)
 
         # scroll area
         scroll_area = TransparentScrollArea()
-        scroll_widget = formation[1](self.done_event, formation[3])
 
-        scroll_area.setWidget(scroll_widget)
+        scroll_area.setWidget(widget)
         scroll_area.setWidgetResizable(True)
 
         content_box_layout.addWidget(scroll_area)
```

### Comparing `solie-8.4.0/solie/widget/script_editor.py` & `solie-8.5.0/solie/widget/script_editor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from PySide6 import QtCore, QtGui, QtWidgets
 from yapf.yapflib.errors import YapfError
 from yapf.yapflib.yapf_api import FormatCode
 
-from solie.definition.syntax_highlighter import SyntaxHighlighter
+from solie.utility import SyntaxHighlighter
 
 
 class ScriptEditor(QtWidgets.QPlainTextEdit):
     def __init__(self, parent):
         super().__init__(parent)
         self.fixed_width_font = QtGui.QFont("Source Code Pro", 9)
         self.setFont(self.fixed_width_font)
```

### Comparing `solie-8.4.0/solie/widget/splash_screen.py` & `solie-8.5.0/solie/widget/splash_screen.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import asyncio
 
 import aiofiles
 from PySide6 import QtGui, QtWidgets
 
-import solie
-from solie.widget.brand_label import BrandLabel
+from solie.common import PACKAGE_PATH, PACKAGE_VERSION
+
+from .brand_label import BrandLabel
 
 
 class SplashScreen(QtWidgets.QFrame):
     def __init__(self):
         super().__init__()
 
         self.full_layout = QtWidgets.QHBoxLayout()
@@ -37,32 +38,31 @@
             QtWidgets.QSizePolicy.Policy.Expanding,
         )
         central_layout.addItem(spacer)
 
         this_layout = QtWidgets.QHBoxLayout()
         central_layout.addLayout(this_layout)
         product_icon_pixmap = QtGui.QPixmap()
-        async with aiofiles.open(
-            f"{solie.PATH}/static/product_icon.png", mode="rb"
-        ) as file:
+        filepath = PACKAGE_PATH / "static" / "product_icon.png"
+        async with aiofiles.open(filepath, mode="rb") as file:
             product_icon_data = await file.read()
         product_icon_pixmap.loadFromData(product_icon_data)
         product_icon_label = QtWidgets.QLabel("", self)
         product_icon_label.setPixmap(product_icon_pixmap)
         product_icon_label.setScaledContents(True)
         product_icon_label.setFixedSize(80, 80)
         this_layout.addWidget(product_icon_label)
         spacing_text = QtWidgets.QLabel("")
         spacing_text_font = QtGui.QFont()
         spacing_text_font.setPointSize(8)
         spacing_text.setFont(spacing_text_font)
         this_layout.addWidget(spacing_text)
         title_label = BrandLabel(self, "SOLIE", 48)
         this_layout.addWidget(title_label)
-        text = solie.VERSION
+        text = PACKAGE_VERSION
         label = BrandLabel(self, text, 24)
         this_layout.addWidget(label)
 
         spacer = QtWidgets.QSpacerItem(
             0,
             0,
             QtWidgets.QSizePolicy.Policy.Minimum,
```

### Comparing `solie-8.4.0/solie/worker/collector.py` & `solie-8.5.0/solie/worker/collector.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,169 +1,199 @@
 import asyncio
 import itertools
+import logging
 import math
-import os
 import random
 import webbrowser
 from collections import deque
 from datetime import datetime, timedelta, timezone
-from typing import Dict, List, Set
 
+import aiofiles.os
 import numpy as np
 import pandas as pd
+from apscheduler.schedulers.asyncio import AsyncIOScheduler
+from PySide6 import QtWidgets
 
-import solie
-from solie.definition.api_requester import ApiRequester
-from solie.definition.api_streamer import ApiStreamer
-from solie.definition.rw_lock import RWLock
-from solie.definition.structs import DownloadPreset
-from solie.overlay.donation_guide import DonationGuide
-from solie.overlay.download_fill_option import DownloadFillOption
-from solie.parallel import go
+from solie.common import go, outsource
+from solie.overlay import DonationGuide, DownloadFillOption
 from solie.utility import (
-    check_internet,
-    combine_candle_datas,
+    ApiRequester,
+    ApiStreamer,
+    DownloadPreset,
+    RWLock,
+    add_disconnected_functions,
+    add_task_duration,
+    combine_candle_data,
     download_aggtrade_data,
     fill_holes_with_aggtrades,
-    remember_task_durations,
-    sort_pandas,
-    standardize,
-    stop_flag,
-    user_settings,
+    find_stop_flag,
+    format_numeric,
+    get_current_moment,
+    internet_connected,
+    make_stop_flag,
+    sort_data_frame,
+    standardize_candle_data,
 )
+from solie.widget import overlay
+from solie.window import Window
+
+from .united import team
+
+logger = logging.getLogger(__name__)
 
 
 class Collector:
-    def __init__(self):
+    def __init__(self, window: Window, scheduler: AsyncIOScheduler):
         # ■■■■■ for data management ■■■■■
 
-        self.workerpath = user_settings.get_app_settings()["datapath"] + "/collector"
-        os.makedirs(self.workerpath, exist_ok=True)
+        self.window = window
+        self.scheduler = scheduler
+        self.workerpath = window.datapath / "collector"
 
-        # ■■■■■ worker secret memory ■■■■■
+        # ■■■■■ internal memory ■■■■■
 
-        self.secret_memory = {
-            "price_precisions": {},
-            "markets_gone": [],
-        }
+        self.price_precisions: dict[str, int] = {}  # Symbol and decimal places
+        self.markets_gone: list[str] = []  # Symbols
 
         # ■■■■■ remember and display ■■■■■
 
         self.api_requester = ApiRequester()
 
         self.aggtrade_candle_sizes = {}
-        for symbol in user_settings.get_data_settings()["target_symbols"]:
+        for symbol in window.data_settings.target_symbols:
             self.aggtrade_candle_sizes[symbol] = 0
 
         # Candle data.
         # It's expected to have only the data of current year,
         # while data of previous years are stored in the disk.
-        self.candle_data = RWLock(standardize.candle_data())
+        self.candle_data = RWLock(
+            standardize_candle_data(window.data_settings.target_symbols)
+        )
 
         # Realtime data chunks
         field_names = itertools.product(
-            user_settings.get_data_settings()["target_symbols"],
+            window.data_settings.target_symbols,
             ("Best Bid Price", "Best Ask Price", "Mark Price"),
         )
         field_names = [str(field_name) for field_name in field_names]
         dtype = [(field_name, np.float32) for field_name in field_names]
         dtpye = [("index", "datetime64[ns]")] + dtype
         self.realtime_data_chunks = RWLock(
             deque([np.recarray(shape=(0,), dtype=dtpye) for _ in range(2)], maxlen=64)
         )
 
         # Aggregate trades
         field_names = itertools.product(
-            user_settings.get_data_settings()["target_symbols"],
+            window.data_settings.target_symbols,
             ("Price", "Volume"),
         )
         field_names = [str(field_name) for field_name in field_names]
         dtype = [(field_name, np.float32) for field_name in field_names]
         dtpye = [("index", "datetime64[ns]")] + dtype
         self.aggregate_trades = RWLock(np.recarray(shape=(0,), dtype=dtpye))
 
         # ■■■■■ repetitive schedules ■■■■■
 
-        solie.window.scheduler.add_job(
+        self.scheduler.add_job(
             self.display_status_information,
             trigger="cron",
             second="*",
         )
-        solie.window.scheduler.add_job(
+        self.scheduler.add_job(
             self.fill_candle_data_holes,
             trigger="cron",
             second="*/10",
         )
-        solie.window.scheduler.add_job(
+        self.scheduler.add_job(
             self.add_candle_data,
             trigger="cron",
             second="*/10",
         )
-        solie.window.scheduler.add_job(
+        self.scheduler.add_job(
             self.organize_data,
             trigger="cron",
             minute="*",
         )
-        solie.window.scheduler.add_job(
+        self.scheduler.add_job(
             self.get_exchange_information,
             trigger="cron",
             minute="*",
         )
-        solie.window.scheduler.add_job(
+        self.scheduler.add_job(
             self.save_candle_data,
             trigger="cron",
             hour="*",
         )
 
         # ■■■■■ websocket streamings ■■■■■
 
         self.api_streamers = {
             "MARK_PRICE": ApiStreamer(
                 "wss://fstream.binance.com/ws/!markPrice@arr@1s",
                 self.add_mark_price,
             ),
         }
-        for symbol in user_settings.get_data_settings()["target_symbols"]:
+        for symbol in self.window.data_settings.target_symbols:
             api_streamer = ApiStreamer(
                 f"wss://fstream.binance.com/ws/{symbol.lower()}@bookTicker",
                 self.add_book_tickers,
             )
             self.api_streamers[f"BOOK_TICKER_{symbol}"] = api_streamer
             api_streamer = ApiStreamer(
                 f"wss://fstream.binance.com/ws/{symbol.lower()}@aggTrade",
                 self.add_aggregate_trades,
             )
             self.api_streamers[f"AGG_TRADE_{symbol}"] = api_streamer
 
-        # ■■■■■ invoked by the internet connection status change  ■■■■■
+        # ■■■■■ invoked by the internet connection status change ■■■■■
+
+        add_disconnected_functions(self.clear_aggregate_trades)
 
-        check_internet.add_disconnected_functions(self.clear_aggregate_trades)
+        # ■■■■■ connect UI events ■■■■■
+
+        job = self.guide_donation
+        outsource(window.pushButton_9.clicked, job)
+        job = self.download_fill_candle_data
+        outsource(window.pushButton_2.clicked, job)
+
+        action_menu = QtWidgets.QMenu(self.window)
+        self.window.pushButton_13.setMenu(action_menu)
+
+        text = "Open historical data webpage of Binance"
+        job = self.open_binance_data_page
+        new_action = action_menu.addAction(text)
+        outsource(new_action.triggered, job)
+        text = "Stop filling candle data"
+        job = self.stop_filling_candle_data
+        new_action = action_menu.addAction(text)
+        outsource(new_action.triggered, job)
+
+    async def load(self):
+        await aiofiles.os.makedirs(self.workerpath, exist_ok=True)
 
-    async def load(self, *args, **kwargs):
         # candle data
         current_year = datetime.now(timezone.utc).year
         async with self.candle_data.write_lock as cell:
-            filepath = f"{self.workerpath}/candle_data_{current_year}.pickle"
-            if os.path.isfile(filepath):
+            filepath = self.workerpath / f"candle_data_{current_year}.pickle"
+            if await aiofiles.os.path.isfile(filepath):
                 df: pd.DataFrame = await go(pd.read_pickle, filepath)
                 if not df.index.is_monotonic_increasing:
-                    df = await go(sort_pandas.data_frame, df)
+                    df = await go(sort_data_frame, df)
                 cell.data = df
-        await asyncio.sleep(0)
 
-    async def organize_data(self, *args, **kwargs):
+    async def organize_data(self):
         start_time = datetime.now(timezone.utc)
 
         async with self.candle_data.write_lock as cell:
             original_index = cell.data.index
             if not cell.data.index.is_unique:
                 unique_index = original_index.drop_duplicates()
                 cell.data = cell.data.reindex(unique_index)
             if not cell.data.index.is_monotonic_increasing:
-                cell.data = await go(sort_pandas.data_frame, cell.data)
+                cell.data = await go(sort_data_frame, cell.data)
 
         async with self.realtime_data_chunks.write_lock as cell:
             cell.data[-1].sort(order="index")
             if len(cell.data[-1]) > 2**16:
                 new_chunk = cell.data[-1][0:0].copy()
                 cell.data.append(new_chunk)
                 del new_chunk
@@ -172,52 +202,43 @@
             cell.data.sort(order="index")
             last_index = cell.data[-1]["index"]
             slice_from = last_index - np.timedelta64(60, "s")
             mask = cell.data["index"] > slice_from
             cell.data = cell.data[mask].copy()
 
         duration = (datetime.now(timezone.utc) - start_time).total_seconds()
-        remember_task_durations.add("collector_organize_data", duration)
+        add_task_duration("collector_organize_data", duration)
 
-    async def save_candle_data(self, *args, **kwargs):
+    async def save_candle_data(self):
         # ■■■■■ default values ■■■■■
 
         current_year = datetime.now(timezone.utc).year
-        filepath = f"{self.workerpath}/candle_data_{current_year}.pickle"
+        filepath = self.workerpath / f"candle_data_{current_year}.pickle"
+        filepath_new = self.workerpath / f"candle_data_{current_year}.pickle.new"
+        filepath_backup = self.workerpath / f"candle_data_{current_year}.pickle.backup"
 
         async with self.candle_data.read_lock as cell:
             mask = cell.data.index.year == current_year  # type:ignore
             year_df: pd.DataFrame = cell.data[mask].copy()
 
         # ■■■■■ make a new file ■■■■■
 
-        await go(
-            year_df.to_pickle,
-            filepath + ".new",
-        )
+        await go(year_df.to_pickle, filepath_new)
 
         # ■■■■■ safely replace the existing file ■■■■■
 
-        try:
-            os.remove(filepath + ".backup")
-        except FileNotFoundError:
-            pass
-
-        try:
-            os.rename(filepath, filepath + ".backup")
-        except FileNotFoundError:
-            pass
-
-        try:
-            os.rename(filepath + ".new", filepath)
-        except FileNotFoundError:
-            pass
+        if await aiofiles.os.path.isfile(filepath_backup):
+            await aiofiles.os.remove(filepath_backup)
+        if await aiofiles.os.path.isfile(filepath):
+            await aiofiles.os.rename(filepath, filepath_backup)
+        if await aiofiles.os.path.isfile(filepath_new):
+            await aiofiles.os.rename(filepath_new, filepath)
 
-    async def get_exchange_information(self, *args, **kwargs):
-        if not check_internet.connected():
+    async def get_exchange_information(self):
+        if not internet_connected():
             return
 
         payload = {}
         response = await self.api_requester.binance(
             http_method="GET",
             path="/fapi/v1/exchangeInfo",
             payload=payload,
@@ -231,52 +252,51 @@
             for filter in about_symbol["filters"]:
                 if filter["filterType"] == "PRICE_FILTER":
                     about_filter = filter
                     break
 
             ticksize = float(about_filter["tickSize"])
             price_precision = int(math.log10(1 / ticksize))
-            self.secret_memory["price_precisions"][symbol] = price_precision
+            self.price_precisions[symbol] = price_precision
 
-    async def fill_candle_data_holes(self, *args, **kwargs):
+    async def fill_candle_data_holes(self):
         # ■■■■■ check internet connection ■■■■■
 
-        if not check_internet.connected():
+        if not internet_connected():
             return
 
         # ■■■■■ moments ■■■■■
 
-        current_moment = datetime.now(timezone.utc).replace(microsecond=0)
-        current_moment = current_moment - timedelta(seconds=current_moment.second % 10)
+        current_moment = get_current_moment()
         split_moment = current_moment - timedelta(days=2)
 
         # ■■■■■ fill holes ■■■■■
 
         markets_gone = []
         full_symbols = []
         request_count = 0
 
         # only the recent part
         async with self.candle_data.read_lock as cell:
             recent_candle_data = cell.data[cell.data.index >= split_moment].copy()
 
         did_fill = False
 
-        target_symbols = user_settings.get_data_settings()["target_symbols"]
+        target_symbols = self.window.data_settings.target_symbols
         while len(full_symbols) < len(target_symbols) and request_count < 10:
             for symbol in target_symbols:
                 if symbol in full_symbols:
                     continue
 
                 from_moment = current_moment - timedelta(hours=24)
                 until_moment = current_moment - timedelta(minutes=1)
 
                 inspect_df: pd.DataFrame = recent_candle_data[symbol][
                     from_moment:until_moment
-                ]
+                ]  # type:ignore
                 base_index = inspect_df.dropna().index
                 temp_sr = pd.Series(0, index=base_index)
                 written_moments = len(temp_sr)
 
                 if written_moments == (86400 - 60) / 10 + 1:
                     # case when there are no holes
                     full_symbols.append(symbol)
@@ -316,72 +336,72 @@
                         aggtrades[aggtrade_id] = aggtrade
                     last_fetched_id = max(aggtrades.keys())
                     last_fetched_time = datetime.fromtimestamp(
                         aggtrades[last_fetched_id]["T"] / 1000, tz=timezone.utc
                     )
 
                 recent_candle_data = await go(
-                    fill_holes_with_aggtrades.do,
+                    fill_holes_with_aggtrades,
                     symbol,
                     recent_candle_data,
                     aggtrades,
                     moment_to_fill_from,
                     last_fetched_time,
                 )
                 did_fill = True
 
-        self.secret_memory["markets_gone"] = markets_gone
+        self.markets_gone = markets_gone
 
         if not did_fill:
             return
 
         # combine
         async with self.candle_data.write_lock as cell:
             original_candle_data = cell.data[cell.data.index < split_moment]
             # in case the other data is added during the task
             # read the data again
             temp_df = cell.data[cell.data.index >= split_moment]
             recent_candle_data = recent_candle_data.combine_first(temp_df)
             if not recent_candle_data.index.is_monotonic_increasing:
                 recent_candle_data = await go(
-                    sort_pandas.data_frame,
+                    sort_data_frame,
                     recent_candle_data,
                 )
             candle_data = pd.concat([original_candle_data, recent_candle_data])
             cell.data = candle_data
 
-    async def display_status_information(self, *args, **kwargs):
+    async def display_status_information(self):
         async with self.candle_data.read_lock as cell:
             if len(cell.data) == 0:
                 # when the app is executed for the first time
                 return
 
-        if len(self.secret_memory["price_precisions"]) == 0:
+        if len(self.price_precisions) == 0:
             # right after the app execution
             return
 
         # price
         async with self.aggregate_trades.read_lock as cell:
             ar = cell.data.copy()
-        price_precisions = self.secret_memory["price_precisions"]
+        price_precisions = self.price_precisions
 
-        for symbol in user_settings.get_data_settings()["target_symbols"]:
+        for symbol in self.window.data_settings.target_symbols:
             temp_ar = ar[str((symbol, "Price"))]
             temp_ar = temp_ar[temp_ar != 0]
             if len(temp_ar) > 0:
                 price_precision = price_precisions[symbol]
                 latest_price = temp_ar[-1]
                 text = f"＄{latest_price:.{price_precision}f}"
             else:
                 text = "Unavailable"
-            solie.window.price_labels[symbol].setText(text)
+            self.window.price_labels[symbol].setText(text)
 
         # bottom information
-        if len(self.secret_memory["markets_gone"]) == 0:
-            cumulation_rate = await self.get_candle_data_cumulation_rate()
+        if len(self.markets_gone) == 0:
+            cumulation_rate = await self.check_candle_data_cumulation_rate()
             async with self.realtime_data_chunks.read_lock as cell:
                 chunk_count = len(cell.data)
             first_written_time = None
             last_written_time = None
             for turn in range(chunk_count):
                 async with self.realtime_data_chunks.read_lock as cell:
                     if len(cell.data[turn]) > 0:
@@ -404,59 +424,58 @@
             written_length_text = f"{range_days}d {range_hours}h {range_minutes}m"
 
             text = ""
             text += f"24h candle data accumulation rate {cumulation_rate * 100:.2f}%"
             text += "  ⦁  "
             text += f"Realtime data length {written_length_text}"
         else:
-            markets_gone = self.secret_memory["markets_gone"]
+            markets_gone = self.markets_gone
             if len(markets_gone) == 1:
-                text = f"It seems that {markets_gone[0]} market is removed by Binance. You should make a new data folder."
+                text = (
+                    f"It seems that {markets_gone[0]} market is removed by Binance."
+                    + " You should make a new data folder."
+                )
             else:
-                text = f"It seems that {', '.join(markets_gone)} markets are removed by Binance. You should make a new data folder."
+                text = (
+                    f"It seems that {', '.join(markets_gone)} markets are removed by Binance."
+                    + " You should make a new data folder."
+                )
 
-        solie.window.label_6.setText(text)
+        self.window.label_6.setText(text)
 
-    async def get_candle_data_cumulation_rate(self, *args, **kwargs):
-        current_moment = datetime.now(timezone.utc).replace(microsecond=0)
-        current_moment = current_moment - timedelta(seconds=current_moment.second % 10)
+    async def check_candle_data_cumulation_rate(self) -> float:
+        current_moment = get_current_moment()
         count_start_moment = current_moment - timedelta(hours=24)
         async with self.candle_data.read_lock as cell:
             cumulated_moments = len(cell.data[count_start_moment:].dropna())
         needed_moments = 24 * 60 * 60 / 10
-        cumulation_rate = min(float(1), (cumulated_moments + 1) / needed_moments)
+        cumulation_rate = min(1.0, (cumulated_moments + 2) / needed_moments)
         return cumulation_rate
 
-    async def open_binance_data_page(self, *args, **kwargs):
+    async def open_binance_data_page(self):
         await go(webbrowser.open, "https://www.binance.com/en/landing/data")
 
-    async def download_fill_candle_data(self, *args, **kwargs):
+    async def download_fill_candle_data(self):
         # ■■■■■ ask filling type ■■■■■
 
-        answer_container = {"filling_type": None}
-
-        formation = [
+        overlay_widget = await overlay(
             "Choose the range to fill",
-            DownloadFillOption,
-            True,
-            [answer_container],
-        ]
-
-        await solie.window.overlay(formation)
+            DownloadFillOption(),
+        )
+        filling_type = overlay_widget.result
 
-        filling_type = answer_container["filling_type"]
         if filling_type is None:
             return
 
         # ■■■■■ prepare target tuples for downloading ■■■■■
 
-        task_id = stop_flag.make("download_fill_candle_data")
+        task_id = make_stop_flag("download_fill_candle_data")
 
-        download_presets: List[DownloadPreset] = []
-        target_symbols = user_settings.get_data_settings()["target_symbols"]
+        download_presets: list[DownloadPreset] = []
+        target_symbols = self.window.data_settings.target_symbols
         if filling_type == 0:
             current_year = datetime.now(timezone.utc).year
             for year in range(2020, current_year):
                 for month in range(1, 12 + 1):
                     for symbol in target_symbols:
                         download_presets.append(
                             DownloadPreset(
@@ -523,126 +542,124 @@
         total_steps = len(download_presets)
         done_steps = 0
 
         # ■■■■■ play the progress bar ■■■■■
 
         async def play_progress_bar():
             while True:
-                if stop_flag.find("download_fill_candle_data", task_id):
-                    solie.window.progressBar_3.setValue(0)
+                if find_stop_flag("download_fill_candle_data", task_id):
+                    self.window.progressBar_3.setValue(0)
                     return
                 else:
                     if done_steps == total_steps:
-                        progressbar_value = solie.window.progressBar_3.value()
+                        progressbar_value = self.window.progressBar_3.value()
                         if progressbar_value == 1000:
                             await asyncio.sleep(0.1)
-                            solie.window.progressBar_3.setValue(0)
+                            self.window.progressBar_3.setValue(0)
                             return
-                    before_value = solie.window.progressBar_3.value()
+                    before_value = self.window.progressBar_3.value()
                     if before_value < 1000:
                         remaining = (
                             math.ceil(1000 / total_steps * done_steps) - before_value
                         )
                         new_value = before_value + math.ceil(remaining * 0.2)
-                        solie.window.progressBar_3.setValue(new_value)
+                        self.window.progressBar_3.setValue(new_value)
                     await asyncio.sleep(0.01)
 
         asyncio.create_task(play_progress_bar())
 
         # ■■■■■ calculate in parellel ■■■■■
 
         # Gather information about years.
         current_year = datetime.now(timezone.utc).year
-        all_years: Set[int] = {t.year for t in download_presets}
+        all_years: set[int] = {t.year for t in download_presets}
 
         # Download and save historical data by year for lower memory usage.
         # Key is the year, value is the list of download presets.
-        classified_download_presets: Dict[int, List[DownloadPreset]] = {
+        classified_download_presets: dict[int, list[DownloadPreset]] = {
             y: [] for y in all_years
         }
         for download_preset in download_presets:
             classified_download_presets[download_preset.year].append(download_preset)
 
         for preset_year, download_presets in classified_download_presets.items():
             # Make an empty dataframe, but of same types with that of candle data.
             async with self.candle_data.read_lock as cell:
                 combined_df = RWLock(cell.data.iloc[0:0].copy())
 
-            async def download_fill(download_preset):
+            async def download_fill(download_preset: DownloadPreset) -> None:
                 nonlocal done_steps
                 nonlocal combined_df
 
-                if stop_flag.find("download_fill_candle_data", task_id):
+                if find_stop_flag("download_fill_candle_data", task_id):
                     return
 
-                returned = await go(download_aggtrade_data.do, download_preset)
+                returned = await go(download_aggtrade_data, download_preset)
                 if returned is not None:
                     new_df = returned
                     async with combined_df.write_lock as cell:
-                        new = await go(combine_candle_datas.do, new_df, cell.data)
+                        new = await go(combine_candle_data, new_df, cell.data)
                         cell.data = new
 
                 done_steps += 1
 
             tasks = [asyncio.create_task(download_fill(p)) for p in download_presets]
             await asyncio.wait(tasks)
 
             if preset_year < current_year:
                 # For data of previous years,
                 # save them in the disk.
                 async with combined_df.read_lock as cell:
                     await go(
                         cell.data.to_pickle,
-                        f"{self.workerpath}/candle_data_{preset_year}.pickle",
+                        self.workerpath / f"candle_data_{preset_year}.pickle",
                     )
             else:
                 # For data of current year, pass it to this collector worker
                 # and store them in the memory.
                 async with combined_df.read_lock as cell:
                     async with self.candle_data.write_lock as cell_worker:
                         cell_worker.data = await go(
-                            combine_candle_datas.do,
+                            combine_candle_data,
                             cell.data,
                             cell_worker.data,
                         )
                 await self.save_candle_data()
 
         # ■■■■■ add to log ■■■■■
 
         text = "Filled the candle data with the history data downloaded from Binance"
-        solie.logger.info(text)
+        logger.info(text)
 
         # ■■■■■ display to graphs ■■■■■
 
-        asyncio.create_task(solie.window.transactor.display_lines())
-        asyncio.create_task(solie.window.simulator.display_lines())
-        asyncio.create_task(solie.window.simulator.display_available_years())
+        asyncio.create_task(team.transactor.display_lines())
+        asyncio.create_task(team.simulator.display_lines())
+        asyncio.create_task(team.simulator.display_available_years())
 
-    async def add_book_tickers(self, *args, **kwargs):
-        received: dict = kwargs.get("received")  # type:ignore
+    async def add_book_tickers(self, received: dict):
         start_time = datetime.now(timezone.utc)
         symbol = received["s"]
         best_bid = received["b"]
         best_ask = received["a"]
         event_time = np.datetime64(received["E"] * 10**6, "ns")
         async with self.realtime_data_chunks.write_lock as cell:
             original_size = cell.data[-1].shape[0]
             cell.data[-1].resize(original_size + 1, refcheck=False)
             cell.data[-1][-1]["index"] = event_time
             find_key = str((symbol, "Best Bid Price"))
             cell.data[-1][-1][find_key] = best_bid
             find_key = str((symbol, "Best Ask Price"))
             cell.data[-1][-1][find_key] = best_ask
         duration = (datetime.now(timezone.utc) - start_time).total_seconds()
-        remember_task_durations.add("add_book_tickers", duration)
+        add_task_duration("add_book_tickers", duration)
 
-    async def add_mark_price(self, *args, **kwargs):
-        received: dict = kwargs.get("received")  # type:ignore
+    async def add_mark_price(self, received: list):
         start_time = datetime.now(timezone.utc)
-        target_symbols = user_settings.get_data_settings()["target_symbols"]
+        target_symbols = self.window.data_settings.target_symbols
         event_time = np.datetime64(received[0]["E"] * 10**6, "ns")
         filtered_data = {}
         for about_mark_price in received:
             symbol = about_mark_price["s"]
             if symbol in target_symbols:
                 mark_price = float(about_mark_price["p"])
                 filtered_data[symbol] = mark_price
@@ -650,39 +667,37 @@
             original_size = cell.data[-1].shape[0]
             cell.data[-1].resize(original_size + 1, refcheck=False)
             cell.data[-1][-1]["index"] = event_time
             for symbol, mark_price in filtered_data.items():
                 find_key = str((symbol, "Mark Price"))
                 cell.data[-1][-1][find_key] = mark_price
         duration = (datetime.now(timezone.utc) - start_time).total_seconds()
-        remember_task_durations.add("add_mark_price", duration)
+        add_task_duration("add_mark_price", duration)
 
-    async def add_aggregate_trades(self, *args, **kwargs):
-        received: dict = kwargs.get("received")  # type:ignore
+    async def add_aggregate_trades(self, received: dict):
         start_time = datetime.now(timezone.utc)
         symbol = received["s"]
         price = float(received["p"])
         volume = float(received["q"])
         trade_time = np.datetime64(received["T"] * 10**6, "ns")
         async with self.aggregate_trades.write_lock as cell:
             original_size = cell.data.shape[0]
             cell.data.resize(original_size + 1, refcheck=False)
             cell.data[-1]["index"] = trade_time
             cell.data[-1][str((symbol, "Price"))] = price
             cell.data[-1][str((symbol, "Volume"))] = volume
         duration = (datetime.now(timezone.utc) - start_time).total_seconds()
-        remember_task_durations.add("add_aggregate_trades", duration)
+        add_task_duration("add_aggregate_trades", duration)
 
-    async def clear_aggregate_trades(self, *args, **kwargs):
+    async def clear_aggregate_trades(self):
         async with self.aggregate_trades.write_lock as cell:
             cell.data = cell.data[0:0].copy()
 
-    async def add_candle_data(self, *args, **kwargs):
-        current_moment = datetime.now(timezone.utc).replace(microsecond=0)
-        current_moment = current_moment - timedelta(seconds=current_moment.second % 10)
+    async def add_candle_data(self):
+        current_moment = get_current_moment()
         before_moment = current_moment - timedelta(seconds=10)
 
         async with self.aggregate_trades.read_lock as cell:
             data_length = len(cell.data)
         if data_length == 0:
             return
 
@@ -698,15 +713,15 @@
 
         first_received_index = aggregate_trades[0]["index"]
         if first_received_index >= np.datetime64(before_moment):
             return
 
         new_datas = {}
 
-        for symbol in user_settings.get_data_settings()["target_symbols"]:
+        for symbol in self.window.data_settings.target_symbols:
             block_start_timestamp = before_moment.timestamp()
             block_end_timestamp = current_moment.timestamp()
 
             index_ar = aggregate_trades["index"].astype(np.int64) / 10**9
             after_start_mask = block_start_timestamp <= index_ar
             before_end_mask = index_ar < block_end_timestamp
             block_ar = aggregate_trades[after_start_mask & before_end_mask]
@@ -738,23 +753,33 @@
             new_datas[(symbol, "Close")] = close_price
             new_datas[(symbol, "Volume")] = sum_volume
 
         async with self.candle_data.write_lock as cell:
             for column_name, new_data_value in new_datas.items():
                 cell.data.loc[before_moment, column_name] = new_data_value
             if not cell.data.index.is_monotonic_increasing:
-                cell.data = await go(sort_pandas.data_frame, cell.data)
+                cell.data = await go(sort_data_frame, cell.data)
 
         duration = (datetime.now(timezone.utc) - current_moment).total_seconds()
-        remember_task_durations.add("add_candle_data", duration)
+        add_task_duration("add_candle_data", duration)
 
-    async def stop_filling_candle_data(self, *args, **kwargs):
-        stop_flag.make("download_fill_candle_data")
+    async def stop_filling_candle_data(self):
+        make_stop_flag("download_fill_candle_data")
 
-    async def guide_donation(self, *args, **kwargs):
-        formation = [
+    async def guide_donation(self):
+        await overlay(
             "Support Solie",
-            DonationGuide,
-            True,
-            None,
+            DonationGuide(),
+        )
+
+    async def check_saved_years(self) -> list[int]:
+        years = [
+            int(format_numeric(filename))
+            for filename in await aiofiles.os.listdir(self.workerpath)
+            if filename.startswith("candle_data_") and filename.endswith(".pickle")
         ]
-        await solie.window.overlay(formation)
+        return years
+
+    async def read_saved_candle_data(self, year: int) -> pd.DataFrame:
+        filepath = self.workerpath / f"candle_data_{year}.pickle"
+        candle_data: pd.DataFrame = await go(pd.read_pickle, filepath)
+        return candle_data
```

### Comparing `solie-8.4.0/solie/worker/manager.py` & `solie-8.5.0/solie/worker/manager.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,48 +1,54 @@
 import asyncio
 import json
+import logging
 import os
 import statistics
 import webbrowser
 from collections import deque
 from datetime import datetime, timedelta, timezone
 
 import aiofiles
+import aiofiles.os
 import time_machine
+from apscheduler.schedulers.asyncio import AsyncIOScheduler
 
-import solie
-from solie.definition.api_requester import ApiRequester
-from solie.parallel import go
+from solie.common import PROCESS_COUNT, go, outsource
 from solie.utility import (
-    check_internet,
-    convert,
-    remember_task_durations,
-    simply_format,
-    user_settings,
+    ApiRequester,
+    get_task_duration,
+    internet_connected,
+    save_datapath,
+    value_to_indexes,
 )
+from solie.widget import ask
+from solie.window import Window
+
+from .united import team
 
 WINDOW_LOCK_OPTIONS = (
     "NEVER",
     "10_SECOND",
     "1_MINUTE",
     "10_MINUTE",
     "1_HOUR",
 )
 
+logger = logging.getLogger(__name__)
+
 
 class Manager:
-    def __init__(self):
+    def __init__(self, window: Window, scheduler: AsyncIOScheduler):
         # ■■■■■ for data management ■■■■■
 
-        self.workerpath = user_settings.get_app_settings()["datapath"] + "/manager"
-        os.makedirs(self.workerpath, exist_ok=True)
+        self.window = window
+        self.scheduler = scheduler
+        self.workerpath = window.datapath / "manager"
 
-        # ■■■■■ worker secret memory ■■■■■
-
-        self.secret_memory = {}
+        # ■■■■■ internal memory ■■■■■
 
         # ■■■■■ remember and display ■■■■■
 
         self.api_requester = ApiRequester()
 
         self.online_status = {
             "ping": 0,
@@ -56,103 +62,116 @@
 
         time_traveller = time_machine.travel(datetime.now(timezone.utc))
         time_traveller.start()
         self.time_traveller = time_traveller
 
         # ■■■■■ repetitive schedules ■■■■■
 
-        solie.window.scheduler.add_job(
+        self.scheduler.add_job(
             self.lock_board,
             trigger="cron",
             second="*",
         )
-        solie.window.scheduler.add_job(
+        self.scheduler.add_job(
             self.display_system_status,
             trigger="cron",
             second="*",
         )
-        solie.window.scheduler.add_job(
+        self.scheduler.add_job(
             self.check_online_status,
             trigger="cron",
             second="*",
         )
-        solie.window.scheduler.add_job(
+        self.scheduler.add_job(
             self.correct_time,
             trigger="cron",
             minute="*",
         )
-        solie.window.scheduler.add_job(
+        self.scheduler.add_job(
             self.check_binance_limits,
             trigger="cron",
             hour="*",
         )
 
         # ■■■■■ websocket streamings ■■■■■
 
         self.api_streamers = {}
 
-        # ■■■■■ invoked by the internet connection status change  ■■■■■
+        # ■■■■■ invoked by the internet connection status change ■■■■■
+
+        # ■■■■■ connect UI events ■■■■■
+
+        job = self.run_script
+        outsource(window.pushButton.clicked, job)
+        job = self.open_datapath
+        outsource(window.pushButton_8.clicked, job)
+        job = self.deselect_log_output
+        outsource(window.pushButton_6.clicked, job)
+        job = self.reset_datapath
+        outsource(window.pushButton_22.clicked, job)
+        job = self.open_documentation
+        outsource(window.pushButton_7.clicked, job)
+        job = self.change_settings
+        outsource(window.comboBox_3.currentIndexChanged, job)
+
+    async def load(self):
+        await aiofiles.os.makedirs(self.workerpath, exist_ok=True)
 
-    async def load(self, *args, **kwargs):
         # settings
-        filepath = self.workerpath + "/settings.json"
-        if os.path.isfile(filepath):
+        filepath = self.workerpath / "settings.json"
+        if await aiofiles.os.path.isfile(filepath):
             async with aiofiles.open(filepath, "r", encoding="utf8") as file:
                 content = await file.read()
                 self.settings = json.loads(content)
-        solie.window.comboBox_3.setCurrentIndex(
-            convert.value_to_indexes(WINDOW_LOCK_OPTIONS, self.settings["lock_board"])[
-                0
-            ]
+        self.window.comboBox_3.setCurrentIndex(
+            value_to_indexes(WINDOW_LOCK_OPTIONS, self.settings["lock_board"])[0]
         )
 
         # python script
-        filepath = self.workerpath + "/python_script.txt"
-        if os.path.isfile(filepath):
+        filepath = self.workerpath / "python_script.txt"
+        if await aiofiles.os.path.isfile(filepath):
             async with aiofiles.open(filepath, "r", encoding="utf8") as file:
                 script = await file.read()
         else:
-            script = "logger.info(window)"
-        solie.window.plainTextEdit.setPlainText(script)
+            script = "from solie.worker import team\n\nlogger.info(team)"
+        self.window.plainTextEdit.setPlainText(script)
 
-    async def change_settings(self, *args, **kwargs):
-        current_index = solie.window.comboBox_3.currentIndex()
+    async def change_settings(self):
+        current_index = self.window.comboBox_3.currentIndex()
         self.settings["lock_board"] = WINDOW_LOCK_OPTIONS[current_index]
 
-        filepath = self.workerpath + "/settings.json"
+        filepath = self.workerpath / "settings.json"
         async with aiofiles.open(filepath, "w", encoding="utf8") as file:
-            content = json.dumps(self.settings, indent=4)
+            content = json.dumps(self.settings, indent=2)
             await file.write(content)
 
-    async def open_datapath(self, *args, **kwargs):
-        await go(os.startfile, user_settings.get_app_settings()["datapath"])
+    async def open_datapath(self):
+        await go(os.startfile, self.window.datapath)
 
-    async def deselect_log_output(self, *args, **kwargs):
-        solie.window.listWidget.clearSelection()
+    async def deselect_log_output(self):
+        self.window.listWidget.clearSelection()
 
-    async def display_internal_status(self, *args, **kwargs):
+    async def display_internal_status(self):
         while True:
             texts = []
             all_tasks = asyncio.all_tasks()
             tasks_not_done = 0
             for task in all_tasks:
                 if not task.done():
                     tasks_not_done += 1
                     text = task.get_name()
                     texts.append(text)
             max_tasks_shown = 8
             if len(texts) <= max_tasks_shown:
                 list_text = "\n".join(texts)
             else:
                 list_text = "\n".join(texts[:max_tasks_shown]) + "\n..."
-            solie.window.label_12.setText(f"{tasks_not_done} total\n\n{list_text}")
+            self.window.label_12.setText(f"{tasks_not_done} total\n\n{list_text}")
 
-            solie.window.label_32.setText(
-                f"Process count: {solie.parallel.process_count}"
-            )
+            self.window.label_32.setText(f"Process count: {PROCESS_COUNT}")
 
             texts = []
             texts.append("Limits")
             for limit_type, limit_value in self.binance_limits.items():
                 text = f"{limit_type}: {limit_value}"
                 texts.append(text)
             used_rates = self.api_requester.used_rates
@@ -160,52 +179,52 @@
                 texts.append("")
                 texts.append("Usage")
                 for used_type, used_tuple in used_rates.items():
                     time_string = used_tuple[1].strftime("%m-%d %H:%M:%S")
                     text = f"{used_type}: {used_tuple[0]}({time_string})"
                     texts.append(text)
             text = "\n".join(texts)
-            solie.window.label_35.setText(text)
+            self.window.label_35.setText(text)
 
             texts = []
-            task_durations = remember_task_durations.get()
+            task_durations = get_task_duration()
             for data_name, deque_data in task_durations.items():
                 if len(deque_data) > 0:
                     text = data_name
                     text += "\n"
                     data_value = sum(deque_data) / len(deque_data)
-                    text += f"Mean {simply_format.fixed_float(data_value,6)}s "
+                    text += f"Mean {data_value:.6f}s "
                     data_value = statistics.median(deque_data)
-                    text += f"Median {simply_format.fixed_float(data_value,6)}s "
+                    text += f"Median {data_value:.6f}s "
                     text += "\n"
                     data_value = min(deque_data)
-                    text += f"Minimum {simply_format.fixed_float(data_value,6)}s "
+                    text += f"Minimum {data_value:.6f}s "
                     data_value = max(deque_data)
-                    text += f"Maximum {simply_format.fixed_float(data_value,6)}s "
+                    text += f"Maximum {data_value:.6f}s "
                     texts.append(text)
             text = "\n\n".join(texts)
-            solie.window.label_33.setText(text)
+            self.window.label_33.setText(text)
 
-            block_sizes = solie.window.collector.aggtrade_candle_sizes
+            block_sizes = team.collector.aggtrade_candle_sizes
             lines = (f"{symbol} {count}" for (symbol, count) in block_sizes.items())
             text = "\n".join(lines)
-            solie.window.label_36.setText(text)
+            self.window.label_36.setText(text)
 
             await asyncio.sleep(0.1)
 
-    async def run_script(self, *args, **kwargs):
-        script_text = solie.window.plainTextEdit.toPlainText()
-        filepath = self.workerpath + "/python_script.txt"
+    async def run_script(self):
+        script_text = self.window.plainTextEdit.toPlainText()
+        filepath = self.workerpath / "python_script.txt"
         async with aiofiles.open(filepath, "w", encoding="utf8") as file:
             await file.write(script_text)
-        namespace = {"window": solie.window, "logger": solie.logger}
+        namespace = {"logger": logger}
         exec(script_text, namespace)
 
-    async def check_online_status(self, *args, **kwargs):
-        if not check_internet.connected():
+    async def check_online_status(self):
+        if not internet_connected():
             return
 
         async def job():
             request_time = datetime.now(timezone.utc)
             payload = {}
             response = await self.api_requester.binance(
                 http_method="GET",
@@ -220,56 +239,56 @@
             server_time = datetime.fromtimestamp(server_timestamp, tz=timezone.utc)
             local_time = datetime.now(timezone.utc)
             time_difference = (server_time - local_time).total_seconds() - ping / 2
             self.online_status["server_time_differences"].append(time_difference)
 
         asyncio.create_task(job())
 
-    async def display_system_status(self, *args, **kwargs):
+    async def display_system_status(self):
         time = datetime.now(timezone.utc)
         time_text = time.strftime("%Y-%m-%d %H:%M:%S")
-        internet_connected = check_internet.connected()
+        is_internet_connected = internet_connected()
         ping = self.online_status["ping"]
-        board_enabled = solie.window.board.isEnabled()
+        board_enabled = self.window.board.isEnabled()
 
         deque_data = self.online_status["server_time_differences"]
         if len(deque_data) > 0:
             mean_difference = sum(deque_data) / len(deque_data)
         else:
             mean_difference = 0.0
 
         text = ""
         text += f"Current time UTC {time_text}"
         text += "  ⦁  "
-        if internet_connected:
+        if is_internet_connected:
             text += "Connected to the internet"
         else:
             text += "Not connected to the internet"
         text += "  ⦁  "
         text += f"Ping {ping:.3f}s"
         text += "  ⦁  "
         text += f"Server time difference {mean_difference:+.3f}s"
         text += "  ⦁  "
         text += f"Board {('unlocked' if board_enabled else 'locked')}"
-        solie.window.gauge.setText(text)
+        self.window.gauge.setText(text)
 
-    async def correct_time(self, *args, **kwargs):
+    async def correct_time(self):
         server_time_differences = self.online_status["server_time_differences"]
         if len(server_time_differences) < 30:
             return
         mean_difference = sum(server_time_differences) / len(server_time_differences)
         new_time = datetime.now(timezone.utc) + timedelta(seconds=mean_difference)
 
         self.time_traveller.stop()
         time_traveller = time_machine.travel(new_time)
         time_traveller.start()
         self.time_traveller = time_traveller
 
-    async def check_binance_limits(self, *args, **kwargs):
-        if not check_internet.connected():
+    async def check_binance_limits(self):
+        if not internet_connected():
             return
 
         payload = {}
         response = await self.api_requester.binance(
             http_method="GET",
             path="/fapi/v1/exchangeInfo",
             payload=payload,
@@ -278,35 +297,34 @@
             limit_type = about_rate_limit["rateLimitType"]
             limit_value = about_rate_limit["limit"]
             interval_unit = about_rate_limit["interval"]
             interval_value = about_rate_limit["intervalNum"]
             limit_name = f"{limit_type}({interval_value}{interval_unit})"
             self.binance_limits[limit_name] = limit_value
 
-    async def reset_datapath(self, *args, **kwargs):
-        question = [
+    async def reset_datapath(self):
+        answer = await ask(
             "Are you sure you want to change the data folder?",
             "Solie will shut down shortly. You will get to choose the new data folder"
             " when you start Solie again. Previous data folder does not get deleted.",
             ["No", "Yes"],
-        ]
-        answer = await solie.window.ask(question)
+        )
 
         if answer in (0, 1):
             return
 
-        await user_settings.apply_app_settings({"datapath": None})
+        await save_datapath(None)
 
-        solie.window.should_confirm_closing = False
-        solie.window.close()
+        self.window.should_confirm_closing = False
+        self.window.close()
 
-    async def open_documentation(self, *args, **kwargs):
+    async def open_documentation(self):
         await go(webbrowser.open, "https://solie-docs.cunarist.com")
 
-    async def lock_board(self, *args, **kwargs):
+    async def lock_board(self):
         lock_window_setting = self.settings["lock_board"]
 
         if lock_window_setting == "NEVER":
             return
         elif lock_window_setting == "10_SECOND":
             wait_time = timedelta(seconds=10)
         elif lock_window_setting == "1_MINUTE":
@@ -314,14 +332,14 @@
         elif lock_window_setting == "10_MINUTE":
             wait_time = timedelta(minutes=10)
         elif lock_window_setting == "1_HOUR":
             wait_time = timedelta(hours=1)
         else:
             raise ValueError("Invalid duration value for locking the window")
 
-        last_interaction_time = solie.window.last_interaction
+        last_interaction_time = self.window.last_interaction
         if datetime.now(timezone.utc) < last_interaction_time + wait_time:
             return
 
-        is_enabled = solie.window.board.isEnabled()
+        is_enabled = self.window.board.isEnabled()
         if is_enabled:
-            solie.window.board.setEnabled(False)
+            self.window.board.setEnabled(False)
```

### Comparing `solie-8.4.0/solie/worker/simulator.py` & `solie-8.5.0/solie/worker/simulator.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,212 +1,263 @@
 import asyncio
 import math
-import os
 import pickle
 import re
 from datetime import datetime, timedelta, timezone
-from typing import List
 
 import aiofiles
+import aiofiles.os
 import numpy as np
 import pandas as pd
+from apscheduler.schedulers.asyncio import AsyncIOScheduler
+from PySide6 import QtWidgets
 from scipy.signal import find_peaks
 
-import solie
-from solie.definition.rw_lock import RWLock
-from solie.parallel import go
+from solie.common import go, outsource, sync_manager
 from solie.utility import (
+    CalculationInput,
+    RWLock,
+    SimulationSettings,
+    SimulationSummary,
+    find_stop_flag,
+    get_current_moment,
     make_indicators,
-    simply_format,
+    make_stop_flag,
     simulate_chunk,
-    sort_pandas,
-    standardize,
-    stop_flag,
-    user_settings,
+    sort_data_frame,
+    sort_series,
+    standardize_account_state,
+    standardize_asset_record,
+    standardize_unrealized_changes,
 )
+from solie.widget import ask
+from solie.window import Window
+
+from .united import team
 
 
 class Simulator:
-    def __init__(self):
+    def __init__(self, window: Window, scheduler: AsyncIOScheduler):
         # ■■■■■ for data management ■■■■■
 
-        self.workerpath = user_settings.get_app_settings()["datapath"] + "/simulator"
-        os.makedirs(self.workerpath, exist_ok=True)
-
-        # ■■■■■ worker secret memory ■■■■■
+        self.window = window
+        self.scheduler = scheduler
+        self.workerpath = window.datapath / "simulator"
 
-        self.secret_memory = {}
+        # ■■■■■ internal memory ■■■■■
 
         # ■■■■■ remember and display ■■■■■
 
-        self.viewing_symbol = user_settings.get_data_settings()["target_symbols"][0]
+        self.viewing_symbol = window.data_settings.target_symbols[0]
         self.should_draw_all_years = False
 
-        self.about_viewing = None
-
-        self.calculation_settings = {
-            "year": datetime.now(timezone.utc).year,
-            "strategy_index": 0,
-        }
-        self.presentation_settings = {
-            "maker_fee": 0.02,
-            "taker_fee": 0.04,
-            "leverage": 1,
-        }
+        self.simulation_settings = SimulationSettings(
+            year=datetime.now(timezone.utc).year,
+        )
+        self.simulation_summary: SimulationSummary | None = None
 
-        self.raw_account_state = standardize.account_state()
+        self.raw_account_state = standardize_account_state(
+            self.window.data_settings.target_symbols
+        )
         self.raw_scribbles = {}
-        self.raw_asset_record = RWLock(standardize.asset_record())
-        self.raw_unrealized_changes = RWLock(standardize.unrealized_changes())
+        self.raw_asset_record = RWLock(standardize_asset_record())
+        self.raw_unrealized_changes = RWLock(standardize_unrealized_changes())
 
-        self.account_state = standardize.account_state()
+        self.account_state = standardize_account_state(
+            self.window.data_settings.target_symbols
+        )
         self.scribbles = {}
-        self.asset_record = RWLock(standardize.asset_record())
-        self.unrealized_changes = RWLock(standardize.unrealized_changes())
+        self.asset_record = RWLock(standardize_asset_record())
+        self.unrealized_changes = RWLock(standardize_unrealized_changes())
 
         # ■■■■■ repetitive schedules ■■■■■
 
-        solie.window.scheduler.add_job(
+        self.scheduler.add_job(
             self.display_available_years,
             trigger="cron",
             hour="*",
         )
-        solie.window.scheduler.add_job(
+        self.scheduler.add_job(
             self.display_lines,
             trigger="cron",
             hour="*",
             kwargs={"periodic": True},
         )
 
         # ■■■■■ websocket streamings ■■■■■
 
         self.api_streamers = {}
 
-        # ■■■■■ invoked by the internet connection status change  ■■■■■
+        # ■■■■■ invoked by the internet connection status change ■■■■■
+
+        # ■■■■■ connect UI events ■■■■■
+
+        job = self.display_range_information
+        outsource(window.plot_widget_2.sigRangeChanged, job)
+        job = self.set_minimum_view_range
+        outsource(window.plot_widget_2.sigRangeChanged, job)
+        job = self.update_calculation_settings
+        outsource(window.comboBox.currentIndexChanged, job)
+        job = self.calculate
+        outsource(window.pushButton_3.clicked, job)
+        job = self.update_presentation_settings
+        outsource(window.spinBox_2.editingFinished, job)
+        job = self.update_presentation_settings
+        outsource(window.doubleSpinBox.editingFinished, job)
+        job = self.update_presentation_settings
+        outsource(window.doubleSpinBox_2.editingFinished, job)
+        job = self.erase
+        outsource(window.pushButton_4.clicked, job)
+        job = self.update_calculation_settings
+        outsource(window.comboBox_5.currentIndexChanged, job)
+        job = self.toggle_combined_draw
+        outsource(window.checkBox_3.toggled, job)
+        job = self.display_year_range
+        outsource(window.pushButton_15.clicked, job)
+        job = self.delete_calculation_data
+        outsource(window.pushButton_16.clicked, job)
+        job = self.draw
+        outsource(window.pushButton_17.clicked, job)
+        job = self.update_viewing_symbol
+        outsource(window.comboBox_6.currentIndexChanged, job)
+
+        action_menu = QtWidgets.QMenu(self.window)
+        self.window.pushButton_11.setMenu(action_menu)
+
+        text = "Calculate temporarily only on visible range"
+        job = self.simulate_only_visible
+        new_action = action_menu.addAction(text)
+        outsource(new_action.triggered, job)
+        text = "Stop calculation"
+        job = self.stop_calculation
+        new_action = action_menu.addAction(text)
+        outsource(new_action.triggered, job)
+        text = "Find spots with lowest unrealized profit"
+        job = self.analyze_unrealized_peaks
+        new_action = action_menu.addAction(text)
+        outsource(new_action.triggered, job)
+        text = "Display same range as transaction graph"
+        job = self.match_graph_range
+        new_action = action_menu.addAction(text)
+        outsource(new_action.triggered, job)
+
+    async def load(self):
+        await aiofiles.os.makedirs(self.workerpath, exist_ok=True)
 
-    async def load(self, *args, **kwargs):
         text = "Nothing drawn"
-        solie.window.label_19.setText(text)
+        self.window.label_19.setText(text)
 
-    async def update_viewing_symbol(self, *args, **kwargs):
-        alias = solie.window.comboBox_6.currentText()
-        symbol = solie.window.alias_to_symbol[alias]
+    async def update_viewing_symbol(self):
+        alias = self.window.comboBox_6.currentText()
+        symbol = self.window.alias_to_symbol[alias]
         self.viewing_symbol = symbol
 
         await self.display_lines()
 
-    async def update_calculation_settings(self, *args, **kwargs):
-        text = solie.window.comboBox_5.currentText()
+    async def update_calculation_settings(self):
+        text = self.window.comboBox_5.currentText()
         if text == "":
             return
-        from_year = self.calculation_settings["year"]
+        from_year = self.simulation_settings.year
         to_year = int(text)
-        self.calculation_settings["year"] = to_year
+        self.simulation_settings.year = to_year
         if from_year != to_year:
             asyncio.create_task(self.display_year_range())
 
-        index = solie.window.comboBox.currentIndex()
-        self.calculation_settings["strategy_index"] = index
+        index = self.window.comboBox.currentIndex()
+        self.simulation_settings.strategy_index = index
 
         await self.display_lines()
 
-    async def update_presentation_settings(self, *args, **kwargs):
-        input_value = solie.window.spinBox_2.value()
-        self.presentation_settings["leverage"] = input_value
-        input_value = solie.window.doubleSpinBox.value()
-        self.presentation_settings["taker_fee"] = input_value
-        input_value = solie.window.doubleSpinBox_2.value()
-        self.presentation_settings["maker_fee"] = input_value
+    async def update_presentation_settings(self):
+        input_value = self.window.spinBox_2.value()
+        self.simulation_settings.leverage = input_value
+        input_value = self.window.doubleSpinBox.value()
+        self.simulation_settings.taker_fee = input_value
+        input_value = self.window.doubleSpinBox_2.value()
+        self.simulation_settings.maker_fee = input_value
         await self.present()
 
-    async def display_lines(self, *args, **kwargs):
+    async def display_lines(self, periodic=False, frequent=False):
         # ■■■■■ start the task ■■■■■
 
-        periodic = kwargs.get("periodic", False)
-        frequent = kwargs.get("frequent", False)
-        only_light_lines = kwargs.get("only_light_lines", False)
-
-        if only_light_lines:
-            task_name = "display_light_simulation_lines"
-        else:
-            task_name = "display_all_simulation_lines"
+        task_name = "display_simulation_lines"
 
-        task_id = stop_flag.make(task_name)
+        task_id = make_stop_flag(task_name)
 
         # ■■■■■ check drawing mode ■■■■■
 
         should_draw_all_years = self.should_draw_all_years
 
         if frequent:
             pass
 
         # ■■■■■ check if the data exists ■■■■■
 
-        async with solie.window.collector.candle_data.read_lock as cell:
+        async with team.collector.candle_data.read_lock as cell:
             if len(cell.data) == 0:
                 return
 
         # ■■■■■ wait for the latest data to be added ■■■■■
 
-        current_moment = datetime.now(timezone.utc).replace(microsecond=0)
-        current_moment = current_moment - timedelta(seconds=current_moment.second % 10)
+        current_moment = get_current_moment()
         before_moment = current_moment - timedelta(seconds=10)
 
         if periodic:
             for _ in range(50):
-                if stop_flag.find(task_name, task_id):
+                if find_stop_flag(task_name, task_id):
                     return
-                async with solie.window.collector.candle_data.read_lock as cell:
+                async with team.collector.candle_data.read_lock as cell:
                     last_index = cell.data.index[-1]
                     if last_index == before_moment:
                         break
                 await asyncio.sleep(0.1)
 
         # ■■■■■ get ready for task duration measurement ■■■■■
 
         pass
 
         # ■■■■■ check things ■■■■■
 
         symbol = self.viewing_symbol
-        strategy_index = self.calculation_settings["strategy_index"]
-        strategy = solie.window.strategist.strategies[strategy_index]
+        strategy_index = self.simulation_settings.strategy_index
+        strategy = team.strategist.strategies.all[strategy_index]
 
         # ■■■■■ get light data ■■■■■
 
-        async with solie.window.collector.realtime_data_chunks.read_lock as cell:
+        async with team.collector.realtime_data_chunks.read_lock as cell:
             before_chunk = cell.data[-2].copy()
             current_chunk = cell.data[-1].copy()
         realtime_data = np.concatenate((before_chunk, current_chunk))
-        async with solie.window.collector.aggregate_trades.read_lock as cell:
+        async with team.collector.aggregate_trades.read_lock as cell:
             aggregate_trades = cell.data.copy()
 
         # ■■■■■ draw light lines ■■■■■
 
         # mark price
         data_x = realtime_data["index"].astype(np.int64) / 10**9
         data_y = realtime_data[str((symbol, "Mark Price"))]
         mask = data_y != 0
         data_y = data_y[mask]
         data_x = data_x[mask]
-        widget = solie.window.simulation_lines["mark_price"][0]
+        widget = self.window.simulation_lines["mark_price"][0]
         widget.setData(data_x, data_y)
-        if stop_flag.find(task_name, task_id):
+        if find_stop_flag(task_name, task_id):
             return
         await asyncio.sleep(0)
 
         # last price
         data_x = aggregate_trades["index"].astype(np.int64) / 10**9
         data_y = aggregate_trades[str((symbol, "Price"))]
         mask = data_y != 0
         data_y = data_y[mask]
         data_x = data_x[mask]
-        widget = solie.window.simulation_lines["last_price"][0]
+        widget = self.window.simulation_lines["last_price"][0]
         widget.setData(data_x, data_y)
-        if stop_flag.find(task_name, task_id):
+        if find_stop_flag(task_name, task_id):
             return
         await asyncio.sleep(0)
 
         # last trade volume
         index_ar = aggregate_trades["index"].astype(np.int64) / 10**9
         value_ar = aggregate_trades[str((symbol, "Volume"))]
         mask = value_ar != 0
@@ -214,40 +265,40 @@
         value_ar = value_ar[mask]
         length = len(index_ar)
         zero_ar = np.zeros(length)
         nan_ar = np.empty(length)
         nan_ar[:] = np.nan
         data_x = np.repeat(index_ar, 3)
         data_y = np.stack([nan_ar, zero_ar, value_ar], axis=1).reshape(-1)
-        widget = solie.window.simulation_lines["last_volume"][0]
+        widget = self.window.simulation_lines["last_volume"][0]
         widget.setData(data_x, data_y)
-        if stop_flag.find(task_name, task_id):
+        if find_stop_flag(task_name, task_id):
             return
         await asyncio.sleep(0)
 
         # book tickers
         data_x = realtime_data["index"].astype(np.int64) / 10**9
         data_y = realtime_data[str((symbol, "Best Bid Price"))]
         mask = data_y != 0
         data_y = data_y[mask]
         data_x = data_x[mask]
-        widget = solie.window.simulation_lines["book_tickers"][0]
+        widget = self.window.simulation_lines["book_tickers"][0]
         widget.setData(data_x, data_y)
-        if stop_flag.find(task_name, task_id):
+        if find_stop_flag(task_name, task_id):
             return
         await asyncio.sleep(0)
 
         data_x = realtime_data["index"].astype(np.int64) / 10**9
         data_y = realtime_data[str((symbol, "Best Ask Price"))]
         mask = data_y != 0
         data_y = data_y[mask]
         data_x = data_x[mask]
-        widget = solie.window.simulation_lines["book_tickers"][1]
+        widget = self.window.simulation_lines["book_tickers"][1]
         widget.setData(data_x, data_y)
-        if stop_flag.find(task_name, task_id):
+        if find_stop_flag(task_name, task_id):
             return
         await asyncio.sleep(0)
 
         # entry price
         entry_price = self.account_state["positions"][symbol]["entry_price"]
         first_moment = self.account_state["observed_until"] - timedelta(hours=12)
         last_moment = self.account_state["observed_until"] + timedelta(hours=12)
@@ -255,63 +306,51 @@
             data_x = np.linspace(
                 first_moment.timestamp(), last_moment.timestamp(), num=1000
             )
             data_y = np.linspace(entry_price, entry_price, num=1000)
         else:
             data_x = []
             data_y = []
-        widget = solie.window.simulation_lines["entry_price"][0]
+        widget = self.window.simulation_lines["entry_price"][0]
         widget.setData(data_x, data_y)
-        if stop_flag.find(task_name, task_id):
+        if find_stop_flag(task_name, task_id):
             return
         await asyncio.sleep(0)
 
         # ■■■■■ record task duration ■■■■■
 
         pass
 
-        # ■■■■■ stop if the target is only light lines ■■■■■
-
-        if only_light_lines:
-            return
-
         # ■■■■■ set range of heavy data ■■■■■
 
         if should_draw_all_years:
-            years = [
-                int(simply_format.numeric(filename))
-                for filename in os.listdir(solie.window.collector.workerpath)
-                if filename.startswith("candle_data_") and filename.endswith(".pickle")
-            ]
+            years = await team.collector.check_saved_years()
             slice_from = datetime.fromtimestamp(0, tz=timezone.utc)
             slice_until = datetime.now(timezone.utc)
             slice_until = slice_until.replace(minute=0, second=0, microsecond=0)
         else:
-            year = self.calculation_settings["year"]
+            year = self.simulation_settings.year
             years = [year]
             slice_from = datetime(year, 1, 1, tzinfo=timezone.utc)
             if year == datetime.now(timezone.utc).year:
                 slice_until = datetime.now(timezone.utc)
                 slice_until = slice_until.replace(minute=0, second=0, microsecond=0)
             else:
                 slice_until = datetime(year + 1, 1, 1, tzinfo=timezone.utc)
         slice_until -= timedelta(seconds=1)
 
         # ■■■■■ get heavy data ■■■■■
 
-        divided_datas: List[pd.DataFrame] = []
+        divided_datas: list[pd.DataFrame] = []
         for year in years:
-            filepath = f"{solie.window.collector.workerpath}/candle_data_{year}.pickle"
-            more_df = await go(pd.read_pickle, filepath)
+            more_df = await team.collector.read_saved_candle_data(year)
             divided_datas.append(more_df)
         candle_data_original: pd.DataFrame = await go(pd.concat, divided_datas)
         if not candle_data_original.index.is_monotonic_increasing:
-            candle_data_original = await go(
-                sort_pandas.data_frame, candle_data_original
-            )
+            candle_data_original = await go(sort_data_frame, candle_data_original)
         async with self.unrealized_changes.read_lock as cell:
             unrealized_changes = cell.data.copy()
         async with self.asset_record.read_lock as cell:
             if len(cell.data) > 0:
                 last_asset = cell.data.iloc[-1]["Result Asset"]
             else:
                 last_asset = None
@@ -337,23 +376,23 @@
         if last_asset is not None:
             observed_until = self.account_state["observed_until"]
             if len(asset_record) == 0 or asset_record.index[-1] < observed_until:
                 if slice_from < observed_until:
                     asset_record.loc[observed_until, "Cause"] = "other"
                     asset_record.loc[observed_until, "Result Asset"] = last_asset
                     if not asset_record.index.is_monotonic_increasing:
-                        asset_record = await go(sort_pandas.data_frame, asset_record)
+                        asset_record = await go(sort_data_frame, asset_record)
 
         # add the left end
 
         if before_asset is not None:
             asset_record.loc[slice_from, "Cause"] = "other"
             asset_record.loc[slice_from, "Result Asset"] = before_asset
             if not asset_record.index.is_monotonic_increasing:
-                asset_record = await go(sort_pandas.data_frame, asset_record)
+                asset_record = await go(sort_data_frame, asset_record)
 
         # ■■■■■ draw heavy lines ■■■■■
 
         # price movement
         index_ar = candle_data.index.to_numpy(dtype=np.int64) / 10**9
         open_ar = candle_data[(symbol, "Open")].to_numpy()
         close_ar = candle_data[(symbol, "Close")].to_numpy()
@@ -390,17 +429,17 @@
                 nan_ar[rise_ar],
                 high_ar[rise_ar],
                 low_ar[rise_ar],
                 nan_ar[rise_ar],
             ],
             axis=1,
         ).reshape(-1)
-        widget = solie.window.simulation_lines["price_rise"][0]
+        widget = self.window.simulation_lines["price_rise"][0]
         widget.setData(data_x, data_y)
-        if stop_flag.find(task_name, task_id):
+        if find_stop_flag(task_name, task_id):
             return
         await asyncio.sleep(0)
 
         data_x = np.stack(
             [
                 index_ar[fall_ar] + 2,
                 index_ar[fall_ar] + 5,
@@ -424,17 +463,17 @@
                 nan_ar[fall_ar],
                 high_ar[fall_ar],
                 low_ar[fall_ar],
                 nan_ar[fall_ar],
             ],
             axis=1,
         ).reshape(-1)
-        widget = solie.window.simulation_lines["price_fall"][0]
+        widget = self.window.simulation_lines["price_fall"][0]
         widget.setData(data_x, data_y)
-        if stop_flag.find(task_name, task_id):
+        if find_stop_flag(task_name, task_id):
             return
         await asyncio.sleep(0)
 
         data_x = np.stack(
             [
                 index_ar[stay_ar] + 2,
                 index_ar[stay_ar] + 5,
@@ -458,253 +497,251 @@
                 nan_ar[stay_ar],
                 high_ar[stay_ar],
                 low_ar[stay_ar],
                 nan_ar[stay_ar],
             ],
             axis=1,
         ).reshape(-1)
-        widget = solie.window.simulation_lines["price_stay"][0]
+        widget = self.window.simulation_lines["price_stay"][0]
         widget.setData(data_x, data_y)
-        if stop_flag.find(task_name, task_id):
+        if find_stop_flag(task_name, task_id):
             return
         await asyncio.sleep(0)
 
         # wobbles
         sr = candle_data[(symbol, "High")]
         data_x = sr.index.to_numpy(dtype=np.int64) / 10**9
         data_y = sr.to_numpy(dtype=np.float32)
-        widget = solie.window.simulation_lines["wobbles"][0]
+        widget = self.window.simulation_lines["wobbles"][0]
         widget.setData(data_x, data_y)
-        if stop_flag.find(task_name, task_id):
+        if find_stop_flag(task_name, task_id):
             return
         await asyncio.sleep(0)
 
         sr = candle_data[(symbol, "Low")]
         data_x = sr.index.to_numpy(dtype=np.int64) / 10**9
         data_y = sr.to_numpy(dtype=np.float32)
-        widget = solie.window.simulation_lines["wobbles"][1]
+        widget = self.window.simulation_lines["wobbles"][1]
         widget.setData(data_x, data_y)
-        if stop_flag.find(task_name, task_id):
+        if find_stop_flag(task_name, task_id):
             return
         await asyncio.sleep(0)
 
         # trade volume
         sr = candle_data[(symbol, "Volume")]
         sr = sr.fillna(value=0)
         data_x = sr.index.to_numpy(dtype=np.int64) / 10**9
         data_y = sr.to_numpy(dtype=np.float32)
-        widget = solie.window.simulation_lines["volume"][0]
+        widget = self.window.simulation_lines["volume"][0]
         widget.setData(data_x, data_y)
-        if stop_flag.find(task_name, task_id):
+        if find_stop_flag(task_name, task_id):
             return
         await asyncio.sleep(0)
 
         # asset
         data_x = asset_record["Result Asset"].index.to_numpy(dtype=np.int64) / 10**9
         data_y = asset_record["Result Asset"].to_numpy(dtype=np.float32)
-        widget = solie.window.simulation_lines["asset"][0]
+        widget = self.window.simulation_lines["asset"][0]
         widget.setData(data_x, data_y)
-        if stop_flag.find(task_name, task_id):
+        if find_stop_flag(task_name, task_id):
             return
         await asyncio.sleep(0)
 
         # asset with unrealized profit
         sr = asset_record["Result Asset"]
         if len(sr) >= 2:
             sr = sr.resample("10S").ffill()
         unrealized_changes_sr = unrealized_changes.reindex(sr.index)
         sr = sr * (1 + unrealized_changes_sr)
         data_x = sr.index.to_numpy(dtype=np.int64) / 10**9 + 5
         data_y = sr.to_numpy(dtype=np.float32)
-        widget = solie.window.simulation_lines["asset_with_unrealized_profit"][0]
+        widget = self.window.simulation_lines["asset_with_unrealized_profit"][0]
         widget.setData(data_x, data_y)
-        if stop_flag.find(task_name, task_id):
+        if find_stop_flag(task_name, task_id):
             return
         await asyncio.sleep(0)
 
         # buy and sell
         df = asset_record.loc[asset_record["Symbol"] == symbol]
         df = df[df["Side"] == "sell"]
         sr = df["Fill Price"]
         data_x = sr.index.to_numpy(dtype=np.int64) / 10**9
         data_y = sr.to_numpy(dtype=np.float32)
-        widget = solie.window.simulation_lines["sell"][0]
+        widget = self.window.simulation_lines["sell"][0]
         widget.setData(data_x, data_y)
-        if stop_flag.find(task_name, task_id):
+        if find_stop_flag(task_name, task_id):
             return
         await asyncio.sleep(0)
 
         df = asset_record.loc[asset_record["Symbol"] == symbol]
         df = df[df["Side"] == "buy"]
         sr = df["Fill Price"]
         data_x = sr.index.to_numpy(dtype=np.int64) / 10**9
         data_y = sr.to_numpy(dtype=np.float32)
-        widget = solie.window.simulation_lines["buy"][0]
+        widget = self.window.simulation_lines["buy"][0]
         widget.setData(data_x, data_y)
-        if stop_flag.find(task_name, task_id):
+        if find_stop_flag(task_name, task_id):
             return
         await asyncio.sleep(0)
 
         # ■■■■■ record task duration ■■■■■
 
         pass
 
         # ■■■■■ make indicators ■■■■■
 
-        indicators_script = strategy["indicators_script"]
+        indicators_script = strategy.indicators_script
 
         indicators = await go(
-            make_indicators.do,
+            make_indicators,
             target_symbols=[self.viewing_symbol],
             candle_data=candle_data_original,
             indicators_script=indicators_script,
         )
 
         indicators = indicators[slice_from:slice_until]
 
         # ■■■■■ draw strategy lines ■■■■■
 
         # price indicators
         df = indicators[symbol]["Price"]
         data_x = df.index.to_numpy(dtype=np.int64) / 10**9
         data_x += 5
-        line_list = solie.window.simulation_lines["price_indicators"]
+        line_list = self.window.simulation_lines["price_indicators"]
         for turn, widget in enumerate(line_list):
             if turn < len(df.columns):
                 column_name = df.columns[turn]
                 sr = df[column_name]
                 data_y = sr.to_numpy(dtype=np.float32)
                 inside_strings = re.findall(r"\(([^)]+)", column_name)
                 if len(inside_strings) == 0:
                     color = "#AAAAAA"
                 else:
                     color = inside_strings[0]
                 widget.setPen(color)
                 widget.setData(data_x, data_y)
-                if stop_flag.find(task_name, task_id):
+                if find_stop_flag(task_name, task_id):
                     return
                 await asyncio.sleep(0)
             else:
-                if stop_flag.find(task_name, task_id):
+                if find_stop_flag(task_name, task_id):
                     return
                 widget.clear()
 
         # trade volume indicators
         df = indicators[symbol]["Volume"]
         data_x = df.index.to_numpy(dtype=np.int64) / 10**9
         data_x += 5
-        line_list = solie.window.simulation_lines["volume_indicators"]
+        line_list = self.window.simulation_lines["volume_indicators"]
         for turn, widget in enumerate(line_list):
             if turn < len(df.columns):
                 column_name = df.columns[turn]
                 sr = df[column_name]
                 data_y = sr.to_numpy(dtype=np.float32)
                 inside_strings = re.findall(r"\(([^)]+)", column_name)
                 if len(inside_strings) == 0:
                     color = "#AAAAAA"
                 else:
                     color = inside_strings[0]
                 widget.setPen(color)
                 widget.setData(data_x, data_y)
-                if stop_flag.find(task_name, task_id):
+                if find_stop_flag(task_name, task_id):
                     return
                 await asyncio.sleep(0)
             else:
-                if stop_flag.find(task_name, task_id):
+                if find_stop_flag(task_name, task_id):
                     return
                 widget.clear()
 
         # abstract indicators
         df = indicators[symbol]["Abstract"]
         data_x = df.index.to_numpy(dtype=np.int64) / 10**9
         data_x += 5
-        line_list = solie.window.simulation_lines["abstract_indicators"]
+        line_list = self.window.simulation_lines["abstract_indicators"]
         for turn, widget in enumerate(line_list):
             if turn < len(df.columns):
                 column_name = df.columns[turn]
                 sr = df[column_name]
                 data_y = sr.to_numpy(dtype=np.float32)
                 inside_strings = re.findall(r"\(([^)]+)", column_name)
                 if len(inside_strings) == 0:
                     color = "#AAAAAA"
                 else:
                     color = inside_strings[0]
                 widget.setPen(color)
                 widget.setData(data_x, data_y)
-                if stop_flag.find(task_name, task_id):
+                if find_stop_flag(task_name, task_id):
                     return
                 await asyncio.sleep(0)
             else:
-                if stop_flag.find(task_name, task_id):
+                if find_stop_flag(task_name, task_id):
                     return
                 widget.clear()
 
         # ■■■■■ set minimum view range ■■■■■
 
         await self.set_minimum_view_range()
 
-    async def erase(self, *args, **kwargs):
-        self.raw_account_state = standardize.account_state()
+    async def erase(self):
+        self.raw_account_state = standardize_account_state(
+            self.window.data_settings.target_symbols
+        )
         self.raw_scribbles = {}
-        self.raw_asset_record = RWLock(standardize.asset_record())
-        self.raw_unrealized_changes = RWLock(standardize.unrealized_changes())
-        self.about_viewing = None
+        self.raw_asset_record = RWLock(standardize_asset_record())
+        self.raw_unrealized_changes = RWLock(standardize_unrealized_changes())
+        self.simulation_summary = None
 
         await self.present()
 
-    async def display_available_years(self, *args, **kwargs):
-        years = [
-            int(simply_format.numeric(filename))
-            for filename in os.listdir(solie.window.collector.workerpath)
-            if filename.startswith("candle_data_") and filename.endswith(".pickle")
-        ]
+    async def display_available_years(self):
+        years = await team.collector.check_saved_years()
         years.sort(reverse=True)
 
-        widget = solie.window.comboBox_5
+        widget = self.window.comboBox_5
         choices = [int(widget.itemText(i)) for i in range(widget.count())]
         choices.sort(reverse=True)
 
         if years != choices:
             # if it's changed
-            solie.window.comboBox_5.clear()
-            solie.window.comboBox_5.addItems([str(y) for y in years])
+            self.window.comboBox_5.clear()
+            self.window.comboBox_5.addItems([str(y) for y in years])
 
-    async def simulate_only_visible(self, *args, **kwargs):
+    async def simulate_only_visible(self):
         await self.calculate(only_visible=True)
 
-    async def display_range_information(self, *args, **kwargs):
-        task_id = stop_flag.make("display_simulation_range_information")
+    async def display_range_information(self):
+        task_id = make_stop_flag("display_simulation_range_information")
 
         symbol = self.viewing_symbol
 
-        range_start_timestamp = solie.window.plot_widget_2.getAxis("bottom").range[0]
+        range_start_timestamp = self.window.plot_widget_2.getAxis("bottom").range[0]
         range_start_timestamp = max(range_start_timestamp, 0.0)
         range_start = datetime.fromtimestamp(range_start_timestamp, tz=timezone.utc)
 
-        if stop_flag.find("display_simulation_range_information", task_id):
+        if find_stop_flag("display_simulation_range_information", task_id):
             return
 
-        range_end_timestamp = solie.window.plot_widget_2.getAxis("bottom").range[1]
+        range_end_timestamp = self.window.plot_widget_2.getAxis("bottom").range[1]
         if range_end_timestamp < 0:
             # case when pyqtgraph passed negative value because it's too big
             range_end_timestamp = 9223339636
         else:
             # maximum value available in pandas
             range_end_timestamp = min(range_end_timestamp, 9223339636.0)
         range_end = datetime.fromtimestamp(range_end_timestamp, tz=timezone.utc)
 
-        if stop_flag.find("display_simulation_range_information", task_id):
+        if find_stop_flag("display_simulation_range_information", task_id):
             return
 
         range_length = range_end - range_start
         range_days = range_length.days
         range_hours, remains = divmod(range_length.seconds, 3600)
         range_minutes, remains = divmod(remains, 60)
 
-        if stop_flag.find("display_simulation_range_information", task_id):
+        if find_stop_flag("display_simulation_range_information", task_id):
             return
 
         async with self.unrealized_changes.read_lock as cell:
             unrealized_changes = cell.data[range_start:range_end].copy()
         async with self.asset_record.read_lock as cell:
             asset_record = cell.data[range_start:range_end].copy()
 
@@ -739,18 +776,18 @@
             symbol_yield = 0
         # least unrealized changes
         if len(unrealized_changes) > 0:
             min_unrealized_change = unrealized_changes.min()
         else:
             min_unrealized_change = 0
 
-        if stop_flag.find("display_simulation_range_information", task_id):
+        if find_stop_flag("display_simulation_range_information", task_id):
             return
 
-        view_range = solie.window.plot_widget_2.getAxis("left").range
+        view_range = self.window.plot_widget_2.getAxis("left").range
         range_down = view_range[0]
         range_up = view_range[1]
         price_range_height = (1 - range_down / range_up) * 100
 
         text = ""
         text += f"Visible time range {range_days}d {range_hours}h {range_minutes}s"
         text += "  ⦁  "
@@ -762,89 +799,88 @@
         text += "Transaction amount"
         text += f" ×{symbol_margin_ratio:.4f}({total_margin_ratio:.4f})"
         text += "  ⦁  "
         text += f"Total realized profit {symbol_yield:+.4f}({total_yield:+.4f})%"
         text += "  ⦁  "
         text += "Lowest unrealized profit"
         text += f" {min_unrealized_change*100:+.4f}%"
-        solie.window.label_13.setText(text)
+        self.window.label_13.setText(text)
 
-    async def set_minimum_view_range(self, *args, **kwargs):
-        widget = solie.window.plot_widget_2
+    async def set_minimum_view_range(self):
+        widget = self.window.plot_widget_2
         range_down = widget.getAxis("left").range[0]
         widget.plotItem.vb.setLimits(minYRange=range_down * 0.005)  # type:ignore
-        widget = solie.window.plot_widget_3
+        widget = self.window.plot_widget_3
         range_down = widget.getAxis("left").range[0]
         widget.plotItem.vb.setLimits(minYRange=range_down * 0.005)  # type:ignore
 
-    async def calculate(self, *args, **kwargs):
-        task_id = stop_flag.make("calculate_simulation")
-
-        only_visible = kwargs.get("only_visible", False)
+    async def calculate(self, only_visible=True):
+        task_id = make_stop_flag("calculate_simulation")
 
         prepare_step = 0
         calculate_step = 0
 
         async def play_progress_bar():
             while True:
-                if stop_flag.find("calculate_simulation", task_id):
-                    solie.window.progressBar_4.setValue(0)
-                    solie.window.progressBar.setValue(0)
+                if find_stop_flag("calculate_simulation", task_id):
+                    self.window.progressBar_4.setValue(0)
+                    self.window.progressBar.setValue(0)
                     return
                 else:
                     if prepare_step == 6 and calculate_step == 1000:
                         is_progressbar_filled = True
-                        progressbar_value = solie.window.progressBar_4.value()
+                        progressbar_value = self.window.progressBar_4.value()
                         if progressbar_value < 1000:
                             is_progressbar_filled = False
-                        progressbar_value = solie.window.progressBar.value()
+                        progressbar_value = self.window.progressBar.value()
                         if progressbar_value < 1000:
                             is_progressbar_filled = False
                         if is_progressbar_filled:
                             await asyncio.sleep(0.1)
-                            solie.window.progressBar_4.setValue(0)
-                            solie.window.progressBar.setValue(0)
+                            self.window.progressBar_4.setValue(0)
+                            self.window.progressBar.setValue(0)
                             return
-                    widget = solie.window.progressBar_4
+                    widget = self.window.progressBar_4
                     before_value = widget.value()
                     if before_value < 1000:
                         remaining = math.ceil(1000 / 6 * prepare_step) - before_value
                         new_value = before_value + math.ceil(remaining * 0.2)
                         widget.setValue(new_value)
-                    widget = solie.window.progressBar
+                    widget = self.window.progressBar
                     before_value = widget.value()
                     if before_value < 1000:
                         remaining = calculate_step - before_value
                         new_value = before_value + math.ceil(remaining * 0.2)
                         widget.setValue(new_value)
                     await asyncio.sleep(0.01)
 
         asyncio.create_task(play_progress_bar())
 
         prepare_step = 1
 
         # ■■■■■ default values and the strategy ■■■■■
 
-        year = self.calculation_settings["year"]
-        strategy_index = self.calculation_settings["strategy_index"]
+        year = self.simulation_settings.year
+        strategy_index = self.simulation_settings.strategy_index
 
-        strategy = solie.window.strategist.strategies[strategy_index]
-        strategy_code_name = strategy["code_name"]
-        strategy_version = strategy["version"]
-        should_parallelize = strategy["parallelized_simulation"]
-        chunk_length = strategy["chunk_division"]
-
-        path_start = f"{self.workerpath}/{strategy_code_name}_{strategy_version}_{year}"
-        asset_record_path = path_start + "_asset_record.pickle"
-        unrealized_changes_path = path_start + "_unrealized_changes.pickle"
-        scribbles_path = path_start + "_scribbles.pickle"
-        account_state_path = path_start + "_account_state.pickle"
-        virtual_state_path = path_start + "_virtual_state.pickle"
+        strategy = team.strategist.strategies.all[strategy_index]
+        strategy_code_name = strategy.code_name
+        strategy_version = strategy.version
+        should_parallelize = strategy.parallelized_simulation
+        chunk_length = strategy.chunk_division
+
+        workerpath = self.workerpath
+        prefix = f"{strategy_code_name}_{strategy_version}_{year}"
+        asset_record_path = workerpath / f"{prefix}_asset_record.pickle"
+        unrealized_changes_path = workerpath / f"{prefix}_unrealized_changes.pickle"
+        scribbles_path = workerpath / f"{prefix}_scribbles.pickle"
+        account_state_path = workerpath / f"{prefix}_account_state.pickle"
+        virtual_state_path = workerpath / f"{prefix}_virtual_state.pickle"
 
-        target_symbols = user_settings.get_data_settings()["target_symbols"]
+        target_symbols = self.window.data_settings.target_symbols
 
         prepare_step = 2
 
         # ■■■■■ Get data ■■■■■
 
         # Set ranges
         slice_from = datetime(year, 1, 1, tzinfo=timezone.utc)
@@ -853,28 +889,29 @@
             slice_until = datetime.now(timezone.utc)
             slice_until = slice_until.replace(minute=0, second=0, microsecond=0)
         else:
             slice_until = datetime(year + 1, 1, 1, tzinfo=timezone.utc)
         slice_until -= timedelta(seconds=1)
 
         # Get the candle data of this year.
-        filepath = f"{solie.window.collector.workerpath}/candle_data_{year}.pickle"
-        year_candle_data: pd.DataFrame = await go(pd.read_pickle, filepath)
+        year_candle_data = await team.collector.read_saved_candle_data(year)
 
         # Interpolate so that there's no inappropriate holes.
         year_candle_data = year_candle_data.interpolate()
 
         prepare_step = 3
 
         # ■■■■■ prepare data and calculation range ■■■■■
 
-        blank_asset_record = standardize.asset_record()
-        blank_unrealized_changes = standardize.unrealized_changes()
+        blank_asset_record = standardize_asset_record()
+        blank_unrealized_changes = standardize_unrealized_changes()
         blank_scribbles = {}
-        blank_account_state = standardize.account_state()
+        blank_account_state = standardize_account_state(
+            self.window.data_settings.target_symbols
+        )
         blank_virtual_state = {
             "available_balance": 1,
             "locations": {},
             "placements": {},
         }
         for symbol in target_symbols:
             blank_virtual_state["locations"][symbol] = {
@@ -890,32 +927,36 @@
 
             previous_asset_record = blank_asset_record.copy()
             previous_unrealized_changes = blank_unrealized_changes.copy()
             previous_scribbles = blank_scribbles.copy()
             previous_account_state = blank_account_state.copy()
             previous_virtual_state = blank_virtual_state.copy()
 
-            view_range = solie.window.plot_widget_2.getAxis("bottom").range
+            view_range = self.window.plot_widget_2.getAxis("bottom").range
             view_start = datetime.fromtimestamp(view_range[0], tz=timezone.utc)
             view_end = datetime.fromtimestamp(view_range[1], tz=timezone.utc)
 
             if self.should_draw_all_years:
                 calculate_from = view_start
                 calculate_until = view_end
             else:
                 calculate_from = max(view_start, slice_from)
                 calculate_until = min(view_end, slice_until)
 
         else:
             # when calculating properly
             try:
-                filepath = asset_record_path
-                previous_asset_record = await go(pd.read_pickle, filepath)
-                filepath = unrealized_changes_path
-                previous_unrealized_changes = await go(pd.read_pickle, filepath)
+                previous_asset_record: pd.DataFrame = await go(
+                    pd.read_pickle,
+                    asset_record_path,
+                )
+                previous_unrealized_changes: pd.Series = await go(
+                    pd.read_pickle,
+                    unrealized_changes_path,
+                )
                 async with aiofiles.open(scribbles_path, "rb") as file:
                     content = await file.read()
                     previous_scribbles = pickle.loads(content)
                 async with aiofiles.open(account_state_path, "rb") as file:
                     content = await file.read()
                     previous_account_state = pickle.loads(content)
                 async with aiofiles.open(virtual_state_path, "rb") as file:
@@ -939,46 +980,46 @@
             previous_asset_record.loc[calculate_from, "Cause"] = "other"
             previous_asset_record.loc[calculate_from, "Result Asset"] = float(1)
 
         prepare_step = 5
 
         # ■■■■■ prepare per chunk data ■■■■■
 
-        calculation_input_data = []
-        progress_list = solie.parallel.communicator.list([0])
+        calculation_inputs: list[CalculationInput] = []
+        progress_list = sync_manager.list([0])
 
         if should_calculate:
-            decision_script = strategy["decision_script"]
-            indicators_script = strategy["indicators_script"]
+            decision_script = strategy.decision_script
+            indicators_script = strategy.indicators_script
 
             # a little more data for generation
             provide_from = calculate_from - timedelta(days=7)
             year_indicators = await go(
-                make_indicators.do,
+                make_indicators,
                 target_symbols=target_symbols,
                 candle_data=year_candle_data[provide_from:calculate_until],
                 indicators_script=indicators_script,
             )
 
             # range cut
             needed_candle_data = year_candle_data[calculate_from:calculate_until]
-            needed_index = needed_candle_data.index
+            needed_index: pd.DatetimeIndex = needed_candle_data.index  # type: ignore
             needed_indicators = year_indicators.reindex(needed_index)
 
             if should_parallelize:
                 division = timedelta(days=chunk_length)
                 chunk_candle_data_list = [
                     chunk_candle_data
                     for _, chunk_candle_data in needed_candle_data.groupby(
                         pd.Grouper(freq=division, origin="epoch")  # type:ignore
                     )
                 ]
 
                 chunk_count = len(chunk_candle_data_list)
-                progress_list = solie.parallel.communicator.list([0] * chunk_count)
+                progress_list = sync_manager.list([0] * chunk_count)
 
                 for turn, chunk_candle_data in enumerate(chunk_candle_data_list):
                     chunk_index = chunk_candle_data.index
                     chunk_indicators = needed_indicators.reindex(chunk_index)
                     chunk_asset_record = previous_asset_record.iloc[0:0]
                     chunk_unrealized_changes = previous_unrealized_changes.iloc[0:0]
                     first_timestamp = chunk_index[0].timestamp()
@@ -990,66 +1031,65 @@
                         chunk_account_state = previous_account_state
                         chunk_virtual_state = previous_virtual_state
                     else:
                         chunk_scribbles = blank_scribbles
                         chunk_account_state = blank_account_state
                         chunk_virtual_state = blank_virtual_state
 
-                    dataset = {
-                        "progress_list": progress_list,
-                        "target_progress": turn,
-                        "target_symbols": target_symbols,
-                        "calculation_index": chunk_index,
-                        "chunk_candle_data": chunk_candle_data,
-                        "chunk_indicators": chunk_indicators,
-                        "chunk_asset_record": chunk_asset_record,
-                        "chunk_unrealized_changes": chunk_unrealized_changes,
-                        "chunk_scribbles": chunk_scribbles,
-                        "chunk_account_state": chunk_account_state,
-                        "chunk_virtual_state": chunk_virtual_state,
-                        "decision_script": decision_script,
-                    }
-                    calculation_input_data.append(dataset)
+                    calculation_input = CalculationInput(
+                        progress_list=progress_list,
+                        target_progress=turn,
+                        target_symbols=target_symbols,
+                        calculation_index=chunk_index,
+                        chunk_candle_data=chunk_candle_data,
+                        chunk_indicators=chunk_indicators,
+                        chunk_asset_record=chunk_asset_record,
+                        chunk_unrealized_changes=chunk_unrealized_changes,
+                        chunk_scribbles=chunk_scribbles,
+                        chunk_account_state=chunk_account_state,
+                        chunk_virtual_state=chunk_virtual_state,
+                        decision_script=decision_script,
+                    )
+                    calculation_inputs.append(calculation_input)
 
             else:
-                dataset = {
-                    "progress_list": progress_list,
-                    "target_progress": 0,
-                    "target_symbols": target_symbols,
-                    "calculation_index": needed_index,
-                    "chunk_candle_data": needed_candle_data,
-                    "chunk_indicators": needed_indicators,
-                    "chunk_asset_record": previous_asset_record,
-                    "chunk_unrealized_changes": previous_unrealized_changes,
-                    "chunk_scribbles": previous_scribbles,
-                    "chunk_account_state": previous_account_state,
-                    "chunk_virtual_state": previous_virtual_state,
-                    "decision_script": decision_script,
-                }
-                calculation_input_data.append(dataset)
+                calculation_input = CalculationInput(
+                    progress_list=progress_list,
+                    target_progress=0,
+                    target_symbols=target_symbols,
+                    calculation_index=needed_index,
+                    chunk_candle_data=needed_candle_data,
+                    chunk_indicators=needed_indicators,
+                    chunk_asset_record=previous_asset_record,
+                    chunk_unrealized_changes=previous_unrealized_changes,
+                    chunk_scribbles=previous_scribbles,
+                    chunk_account_state=previous_account_state,
+                    chunk_virtual_state=previous_virtual_state,
+                    decision_script=decision_script,
+                )
+                calculation_inputs.append(calculation_input)
 
         prepare_step = 6
 
         # ■■■■■ calculate ■■■■■
 
         calculation_output_data = []
 
         if should_calculate:
             coroutines = [
-                go(simulate_chunk.do, input_data)
-                for input_data in calculation_input_data
+                go(simulate_chunk, input_data) for input_data in calculation_inputs
             ]
             gathered = asyncio.gather(*coroutines)
 
             total_seconds = (calculate_until - calculate_from).total_seconds()
 
             async def update_calculation_step():
                 nonlocal calculate_step
                 while True:
-                    if stop_flag.find("calculate_simulation", task_id):
+                    if find_stop_flag("calculate_simulation", task_id):
                         return
                     if gathered.done():
                         return
                     total_progress = sum(progress_list)
                     calculate_step = math.ceil(total_progress * 1000 / total_seconds)
                     await asyncio.sleep(0.01)
 
@@ -1060,54 +1100,54 @@
         calculate_step = 1000
 
         # ■■■■■ get calculation result ■■■■■
 
         if should_calculate:
             asset_record = previous_asset_record
             for chunk_ouput_data in calculation_output_data:
-                chunk_asset_record = chunk_ouput_data["chunk_asset_record"]
+                chunk_asset_record = chunk_ouput_data.chunk_asset_record
                 concat_data = [asset_record, chunk_asset_record]
-                asset_record = pd.concat(concat_data)
+                asset_record: pd.DataFrame = pd.concat(concat_data)  # type:ignore
             mask = ~asset_record.index.duplicated()
             asset_record = asset_record[mask]
             if not asset_record.index.is_monotonic_increasing:
-                asset_record = await go(sort_pandas.data_frame, asset_record)
+                asset_record = await go(sort_data_frame, asset_record)
 
             unrealized_changes = previous_unrealized_changes
             for chunk_ouput_data in calculation_output_data:
-                chunk_unrealized_changes = chunk_ouput_data["chunk_unrealized_changes"]
+                chunk_unrealized_changes = chunk_ouput_data.chunk_unrealized_changes
                 concat_data = [unrealized_changes, chunk_unrealized_changes]
-                unrealized_changes: pd.Series = pd.concat(concat_data)
+                unrealized_changes: pd.Series = pd.concat(concat_data)  # type:ignore
             mask = ~unrealized_changes.index.duplicated()
             unrealized_changes = unrealized_changes[mask]
             if not unrealized_changes.index.is_monotonic_increasing:
-                unrealized_changes = await go(sort_pandas.series, unrealized_changes)
+                unrealized_changes = await go(sort_series, unrealized_changes)
 
-            scribbles = calculation_output_data[-1]["chunk_scribbles"]
-            account_state = calculation_output_data[-1]["chunk_account_state"]
-            virtual_state = calculation_output_data[-1]["chunk_virtual_state"]
+            scribbles = calculation_output_data[-1].chunk_scribbles
+            account_state = calculation_output_data[-1].chunk_account_state
+            virtual_state = calculation_output_data[-1].chunk_virtual_state
 
         else:
             asset_record = previous_asset_record
             unrealized_changes = previous_unrealized_changes
             scribbles = previous_scribbles
             account_state = previous_account_state
             virtual_state = previous_virtual_state
 
         # ■■■■■ remember and present ■■■■■
 
         self.raw_asset_record = RWLock(asset_record)
         self.raw_unrealized_changes = RWLock(unrealized_changes)
         self.raw_scribbles = scribbles
         self.raw_account_state = account_state
-        self.about_viewing = {
-            "year": year,
-            "strategy_code_name": strategy_code_name,
-            "strategy_version": strategy_version,
-        }
+        self.simulation_summary = SimulationSummary(
+            year=year,
+            strategy_code_name=strategy_code_name,
+            strategy_version=strategy_version,
+        )
         await self.present()
 
         # ■■■■■ save if properly calculated ■■■■■
 
         if not only_visible and should_calculate:
             await go(asset_record.to_pickle, asset_record_path)
             await go(unrealized_changes.to_pickle, unrealized_changes_path)
@@ -1117,53 +1157,53 @@
             async with aiofiles.open(account_state_path, "wb") as file:
                 content = pickle.dumps(account_state)
                 await file.write(content)
             async with aiofiles.open(virtual_state_path, "wb") as file:
                 content = pickle.dumps(virtual_state)
                 await file.write(content)
 
-    async def present(self, *args, **kwargs):
-        maker_fee = self.presentation_settings["maker_fee"]
-        taker_fee = self.presentation_settings["taker_fee"]
-        leverage = self.presentation_settings["leverage"]
+    async def present(self):
+        maker_fee = self.simulation_settings.maker_fee
+        taker_fee = self.simulation_settings.taker_fee
+        leverage = self.simulation_settings.leverage
 
         async with self.raw_asset_record.read_lock as cell:
             asset_record = cell.data.copy()
 
         async with self.raw_unrealized_changes.read_lock as cell:
             unrealized_changes = cell.data.copy()
 
         scribbles = self.raw_scribbles.copy()
         account_state = self.raw_account_state.copy()
 
         # ■■■■■ get strategy details ■■■■
 
-        if self.about_viewing is None:
+        if self.simulation_summary is None:
             should_parallelize = False
             chunk_length = 0
         else:
-            strategy_index = self.calculation_settings["strategy_index"]
-            strategy = solie.window.strategist.strategies[strategy_index]
-            should_parallelize = strategy["parallelized_simulation"]
-            chunk_length = strategy["chunk_division"]
+            strategy_index = self.simulation_settings.strategy_index
+            strategy = team.strategist.strategies.all[strategy_index]
+            should_parallelize = strategy.parallelized_simulation
+            chunk_length = strategy.chunk_division
 
         # ■■■■■ apply other factors to the asset trace ■■■■
 
         if should_parallelize:
             division = timedelta(days=chunk_length)
             grouper = pd.Grouper(freq=division, origin="epoch")  # type:ignore
             grouped = asset_record.groupby(grouper)
             chunk_asset_record_list = [r.dropna() for _, r in grouped]
             chunk_count = len(chunk_asset_record_list)
 
         else:
             chunk_asset_record_list = [asset_record]
             chunk_count = 1
 
-        chunk_asset_changes_list = []
+        chunk_asset_changes_list: list[pd.Series] = []
         for turn in range(chunk_count):
             chunk_asset_record = chunk_asset_record_list[turn]
             # leverage
             chunk_result_asset_sr = chunk_asset_record["Result Asset"]
             chunk_asset_shifts = chunk_result_asset_sr.diff()
             if len(chunk_asset_shifts) > 0:
                 chunk_asset_shifts.iloc[0] = 0
@@ -1187,21 +1227,21 @@
                 chunk_asset_changes_by_leverage * chunk_asset_changes_by_fee
             )
             chunk_asset_changes_list.append(chunk_asset_changes)
 
         unrealized_changes = unrealized_changes * leverage
         year_asset_changes: pd.Series = pd.concat(chunk_asset_changes_list)
         if not year_asset_changes.index.is_monotonic_increasing:
-            year_asset_changes = await go(sort_pandas.series, year_asset_changes)
+            year_asset_changes = await go(sort_series, year_asset_changes)
 
         if len(asset_record) > 0:
             start_point = asset_record.index[0]
             year_asset_changes[start_point] = float(1)
             if not year_asset_changes.index.is_monotonic_increasing:
-                year_asset_changes = await go(sort_pandas.series, year_asset_changes)
+                year_asset_changes = await go(sort_series, year_asset_changes)
         asset_record = asset_record.reindex(year_asset_changes.index)
         asset_record["Result Asset"] = year_asset_changes.cumprod()
 
         presentation_asset_record = asset_record.copy()
         presentation_unrealized_changes = unrealized_changes.copy()
         presentation_scribbles = scribbles.copy()
         presentation_account_state = account_state.copy()
@@ -1216,197 +1256,184 @@
             cell.data = presentation_asset_record
 
         # ■■■■■ display ■■■■■
 
         asyncio.create_task(self.display_lines())
         asyncio.create_task(self.display_range_information())
 
-        if self.about_viewing is None:
+        if self.simulation_summary is None:
             text = "Nothing drawn"
-            solie.window.label_19.setText(text)
+            self.window.label_19.setText(text)
         else:
-            year = self.about_viewing["year"]
-            strategy_code_name = self.about_viewing["strategy_code_name"]
-            strategy_version = self.about_viewing["strategy_version"]
+            year = self.simulation_summary.year
+            strategy_code_name = self.simulation_summary.strategy_code_name
+            strategy_version = self.simulation_summary.strategy_version
             text = ""
             text += f"Target year {year}"
             text += "  ⦁  "
             text += f"Strategy code name {strategy_code_name}"
             text += "  ⦁  "
             text += f"Strategy version {strategy_version}"
-            solie.window.label_19.setText(text)
+            self.window.label_19.setText(text)
 
-    async def display_year_range(self, *args, **kwargs):
+    async def display_year_range(self):
         range_start = datetime(
-            year=self.calculation_settings["year"],
+            year=self.simulation_settings.year,
             month=1,
             day=1,
             tzinfo=timezone.utc,
         )
         range_start = range_start.timestamp()
         range_end = datetime(
-            year=self.calculation_settings["year"] + 1,
+            year=self.simulation_settings.year + 1,
             month=1,
             day=1,
             tzinfo=timezone.utc,
         )
         range_end = range_end.timestamp()
-        widget = solie.window.plot_widget_2
+        widget = self.window.plot_widget_2
         widget.setXRange(range_start, range_end)
 
-    async def delete_calculation_data(self, *args, **kwargs):
-        year = self.calculation_settings["year"]
-        strategy_index = self.calculation_settings["strategy_index"]
-
-        strategy = solie.window.strategist.strategies[strategy_index]
-        strategy_code_name = strategy["code_name"]
-        strategy_version = strategy["version"]
-
-        path_start = f"{self.workerpath}/{strategy_code_name}_{strategy_version}_{year}"
-        asset_record_path = path_start + "_asset_record.pickle"
-        unrealized_changes_path = path_start + "_unrealized_changes.pickle"
-        scribbles_path = path_start + "_scribbles.pickle"
-        account_state_path = path_start + "_account_state.pickle"
-        virtual_state_path = path_start + "_virtual_state.pickle"
+    async def delete_calculation_data(self):
+        year = self.simulation_settings.year
+        strategy_index = self.simulation_settings.strategy_index
+
+        strategy = team.strategist.strategies.all[strategy_index]
+        strategy_code_name = strategy.code_name
+        strategy_version = strategy.version
+
+        workerpath = self.workerpath
+        prefix = f"{strategy_code_name}_{strategy_version}_{year}"
+        asset_record_path = workerpath / f"{prefix}_asset_record.pickle"
+        unrealized_changes_path = workerpath / f"{prefix}_unrealized_changes.pickle"
+        scribbles_path = workerpath / f"{prefix}_scribbles.pickle"
+        account_state_path = workerpath / f"{prefix}_account_state.pickle"
+        virtual_state_path = workerpath / f"{prefix}_virtual_state.pickle"
 
         does_file_exist = False
 
-        if os.path.exists(asset_record_path):
+        if await aiofiles.os.path.isfile(asset_record_path):
             does_file_exist = True
-        if os.path.exists(unrealized_changes_path):
+        if await aiofiles.os.path.isfile(unrealized_changes_path):
             does_file_exist = True
-        if os.path.exists(scribbles_path):
+        if await aiofiles.os.path.isfile(scribbles_path):
             does_file_exist = True
-        if os.path.exists(account_state_path):
+        if await aiofiles.os.path.isfile(account_state_path):
             does_file_exist = True
-        if os.path.exists(virtual_state_path):
+        if await aiofiles.os.path.isfile(virtual_state_path):
             does_file_exist = True
 
         if not does_file_exist:
-            question = [
+            await ask(
                 "No calculation data on this combination",
                 f"You should calculate first on year {year} with strategy code name"
                 f" {strategy_code_name} version {strategy_version}.",
                 ["Okay"],
-            ]
-            await solie.window.ask(question)
+            )
             return
         else:
-            question = [
+            answer = await ask(
                 "Are you sure you want to delete calculation data on this combination?",
                 "If you do, you should perform the calculation again to see the"
                 f" prediction on year {year} with strategy code name"
                 f" {strategy_code_name} version {strategy_version}. Calculation data of"
                 " other combinations does not get affected.",
                 ["Cancel", "Delete"],
-            ]
-            answer = await solie.window.ask(question)
+            )
             if answer in (0, 1):
                 return
 
-        try:
-            os.remove(asset_record_path)
-        except FileNotFoundError:
-            pass
-        try:
-            os.remove(unrealized_changes_path)
-        except FileNotFoundError:
-            pass
-        try:
-            os.remove(scribbles_path)
-        except FileNotFoundError:
-            pass
-        try:
-            os.remove(account_state_path)
-        except FileNotFoundError:
-            pass
-        try:
-            os.remove(virtual_state_path)
-        except FileNotFoundError:
-            pass
+        if await aiofiles.os.path.isfile(asset_record_path):
+            await aiofiles.os.remove(asset_record_path)
+        if await aiofiles.os.path.isfile(unrealized_changes_path):
+            await aiofiles.os.remove(unrealized_changes_path)
+        if await aiofiles.os.path.isfile(scribbles_path):
+            await aiofiles.os.remove(scribbles_path)
+        if await aiofiles.os.path.isfile(account_state_path):
+            await aiofiles.os.remove(account_state_path)
+        if await aiofiles.os.path.isfile(virtual_state_path):
+            await aiofiles.os.remove(virtual_state_path)
 
         await self.erase()
 
-    async def draw(self, *args, **kwargs):
-        year = self.calculation_settings["year"]
-        strategy_index = self.calculation_settings["strategy_index"]
-
-        strategy = solie.window.strategist.strategies[strategy_index]
-        strategy_code_name = strategy["code_name"]
-        strategy_version = strategy["version"]
-
-        path_start = f"{self.workerpath}/{strategy_code_name}_{strategy_version}_{year}"
-        asset_record_path = path_start + "_asset_record.pickle"
-        unrealized_changes_path = path_start + "_unrealized_changes.pickle"
-        scribbles_path = path_start + "_scribbles.pickle"
-        account_state_path = path_start + "_account_state.pickle"
+    async def draw(self):
+        year = self.simulation_settings.year
+        strategy_index = self.simulation_settings.strategy_index
+
+        strategy = team.strategist.strategies.all[strategy_index]
+        strategy_code_name = strategy.code_name
+        strategy_version = strategy.version
+
+        workerpath = self.workerpath
+        prefix = f"{strategy_code_name}_{strategy_version}_{year}"
+        asset_record_path = workerpath / f"{prefix}_asset_record.pickle"
+        unrealized_changes_path = workerpath / f"{prefix}_unrealized_changes.pickle"
+        scribbles_path = workerpath / f"{prefix}_scribbles.pickle"
+        account_state_path = workerpath / f"{prefix}_account_state.pickle"
 
         try:
             async with self.raw_asset_record.write_lock as cell:
                 new = await go(pd.read_pickle, asset_record_path)
                 cell.data = new
             async with self.raw_unrealized_changes.write_lock as cell:
                 new = await go(pd.read_pickle, unrealized_changes_path)
                 cell.data = new
             async with aiofiles.open(scribbles_path, "rb") as file:
                 content = await file.read()
                 self.raw_scribbles = pickle.loads(content)
             async with aiofiles.open(account_state_path, "rb") as file:
                 content = await file.read()
                 self.raw_account_state = pickle.loads(content)
-            self.about_viewing = {
-                "year": year,
-                "strategy_code_name": strategy_code_name,
-                "strategy_version": strategy_version,
-            }
+            self.simulation_summary = SimulationSummary(
+                year=year,
+                strategy_code_name=strategy_code_name,
+                strategy_version=strategy_version,
+            )
             await self.present()
         except FileNotFoundError:
-            question = [
+            await ask(
                 "No calculation data on this combination",
                 f"You should calculate first on year {year} with strategy code name"
                 f" {strategy_code_name} version {strategy_version}.",
                 ["Okay"],
-            ]
-            await solie.window.ask(question)
+            )
             return
 
-    async def match_graph_range(self, *args, **kwargs):
-        range_start = solie.window.plot_widget.getAxis("bottom").range[0]
-        range_end = solie.window.plot_widget.getAxis("bottom").range[1]
-        widget = solie.window.plot_widget_2
+    async def match_graph_range(self):
+        range_start = self.window.plot_widget.getAxis("bottom").range[0]
+        range_end = self.window.plot_widget.getAxis("bottom").range[1]
+        widget = self.window.plot_widget_2
         widget.setXRange(range_start, range_end, padding=0)  # type:ignore
 
-    async def stop_calculation(self, *args, **kwargs):
-        stop_flag.make("calculate_simulation")
+    async def stop_calculation(self):
+        make_stop_flag("calculate_simulation")
 
-    async def analyze_unrealized_peaks(self, *args, **kwargs):
+    async def analyze_unrealized_peaks(self):
         async with self.unrealized_changes.read_lock as cell:
             peak_indexes, _ = find_peaks(-cell.data, distance=3600 / 10)  # type:ignore
             peak_sr = cell.data.iloc[peak_indexes]
         peak_sr = peak_sr.sort_values().iloc[:12]
         if len(peak_sr) < 12:
-            question = [
+            await ask(
                 "Calculation data is either missing or too short",
                 "Cannot get the list of meaningful spots with lowest unrealized"
                 " profit.",
                 ["Okay"],
-            ]
-            await solie.window.ask(question)
+            )
         else:
             text_lines = [
                 f"{index} {peak_value:+.2f}%"
                 for index, peak_value in peak_sr.iteritems()
             ]
-            question = [
+            await ask(
                 "Spots with lowest unrealized profit",
                 "\n".join(text_lines),
                 ["Okay"],
-            ]
-            await solie.window.ask(question)
+            )
 
-    async def toggle_combined_draw(self, *args, **kwargs):
-        is_checked = args[0]
+    async def toggle_combined_draw(self):
+        is_checked = self.window.checkBox_3.isChecked()
         if is_checked:
             self.should_draw_all_years = True
         else:
             self.should_draw_all_years = False
         await self.display_lines()
```

### Comparing `solie-8.4.0/solie/worker/strategist.py` & `solie-8.5.0/solie/worker/strategist.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,111 +1,114 @@
 import asyncio
-import json
-import os
+from dataclasses import replace
 
 import aiofiles
+import aiofiles.os
+from apscheduler.schedulers.asyncio import AsyncIOScheduler
 from PySide6 import QtGui, QtWidgets
 
-import solie
-from solie.overlay.strategy_basic_input import StrategyBasicInput
-from solie.overlay.strategy_develop_input import StrategyDevelopInput
-from solie.utility import outsource, standardize, user_settings
+from solie.common import PACKAGE_PATH, outsource
+from solie.overlay import StrategyBasicInput, StrategyDevelopInput
+from solie.utility import Strategies, Strategy, create_strategy_code_name
+from solie.widget import ask, overlay
+from solie.window import Window
 
 
 class Strategiest:
-    def __init__(self):
+    def __init__(self, window: Window, scheduler: AsyncIOScheduler):
         # ■■■■■ for data management ■■■■■
 
-        self.workerpath = user_settings.get_app_settings()["datapath"] + "/strategist"
-        os.makedirs(self.workerpath, exist_ok=True)
+        self.window = window
+        self.scheduler = scheduler
+        self.workerpath = window.datapath / "strategist"
 
-        # ■■■■■ worker secret memory ■■■■■
-
-        self.secret_memory = {}
+        # ■■■■■ internal memory ■■■■■
 
         # ■■■■■ remember and display ■■■■■
 
-        self.strategies = []
+        self.strategies: Strategies
         self.strategy_cards: list[QtWidgets.QGroupBox] = []
 
         self.before_selections = {}
 
+        iconpath = PACKAGE_PATH / "static" / "icon"
         self.red_pixmap = QtGui.QPixmap()
-        self.red_pixmap.load(f"{solie.PATH}/static/icon/traffic_light_red.png")
+        self.red_pixmap.load(str(iconpath / "traffic_light_red.png"))
         self.yellow_pixmap = QtGui.QPixmap()
-        self.yellow_pixmap.load(f"{solie.PATH}/static/icon/traffic_light_yellow.png")
+        self.yellow_pixmap.load(str(iconpath / "traffic_light_yellow.png"))
         self.green_pixmap = QtGui.QPixmap()
-        self.green_pixmap.load(f"{solie.PATH}/static/icon/traffic_light_green.png")
+        self.green_pixmap.load(str(iconpath / "traffic_light_green.png"))
 
         # ■■■■■ repetitive schedules ■■■■■
 
         # ■■■■■ websocket streamings ■■■■■
 
         self.api_streamers = {}
 
-        # ■■■■■ invoked by the internet connection status change  ■■■■■
+        # ■■■■■ invoked by the internet connection status change ■■■■■
+
+        # ■■■■■ connect UI events ■■■■■
+
+        job = self.add_blank_strategy
+        outsource(window.pushButton_5.clicked, job)
+
+    async def load(self):
+        await aiofiles.os.makedirs(self.workerpath, exist_ok=True)
 
-    async def load(self, *args, **kwargs):
-        # custom strategies
-        try:
-            filepath = self.workerpath + "/strategies.json"
+        filepath = self.workerpath / "strategies.json"
+        if await aiofiles.os.path.isfile(filepath):
             async with aiofiles.open(filepath, "r", encoding="utf8") as file:
-                content = await file.read()
-                self.strategies = json.loads(content)
-        except FileNotFoundError:
-            first_strategy = standardize.strategy()
-            first_strategy["code_name"] = "SLIESS"
-            first_strategy["readable_name"] = "Sample Strategy"
-            first_strategy["description"] = (
-                "Not for real investment."
-                + " This strategy is only for demonstration purposes."
+                self.strategies = Strategies.from_json(await file.read())
+        else:
+            first_strategy = Strategy(
+                code_name="SLIESS",
+                readable_name="Sample Strategy",
+                description="Not for real investment."
+                + " This strategy is only for demonstration purposes.",
             )
-            first_strategy["risk_level"] = 2
-            filepath = f"{solie.PATH}/static/sample_indicators_script.txt"
+            filepath = PACKAGE_PATH / "static" / "sample_indicators_script.txt"
             async with aiofiles.open(filepath, "r", encoding="utf8") as file:
                 read_data = await file.read()
-                first_strategy["indicators_script"] = read_data
-            filepath = f"{solie.PATH}/static/sample_decision_script.txt"
+                first_strategy.indicators_script = read_data
+            filepath = PACKAGE_PATH / "static" / "sample_decision_script.txt"
             async with aiofiles.open(filepath, "r", encoding="utf8") as file:
                 read_data = await file.read()
-                first_strategy["decision_script"] = read_data
-            self.strategies = [first_strategy]
+                first_strategy.decision_script = read_data
+            self.strategies = Strategies(all=[first_strategy])
 
-    async def save_strategies(self, *args, **kwargs):
-        filepath = self.workerpath + "/strategies.json"
+    async def save_strategies(self):
+        filepath = self.workerpath / "strategies.json"
         async with aiofiles.open(filepath, "w", encoding="utf8") as file:
-            content = json.dumps(self.strategies, indent=4)
-            await file.write(content)
+            await file.write(self.strategies.to_json(indent=2))
 
-    async def display_strategies(self, *args, **kwargs):
-        solie.window.comboBox_2.clear()
-        solie.window.comboBox.clear()
+    async def display_strategies(self):
+        self.window.comboBox_2.clear()
+        self.window.comboBox.clear()
         for strategy_card in self.strategy_cards:
             strategy_card.setParent(None)
         self.strategy_cards = []
 
-        for strategy in self.strategies:
-            if strategy["risk_level"] == 0:
+        for strategy in self.strategies.all:
+            if strategy.risk_level == 2:
                 icon_pixmap = self.red_pixmap
-            elif strategy["risk_level"] == 1:
+            elif strategy.risk_level == 1:
                 icon_pixmap = self.yellow_pixmap
-            elif strategy["risk_level"] == 2:
+            elif strategy.risk_level == 0:
                 icon_pixmap = self.green_pixmap
             else:
                 raise ValueError("Invalid risk level for drawing an icon")
-            text = f"{strategy['code_name']} {strategy['version']}"
-            text += f" - {strategy['readable_name']}"
+            text = f"{strategy.code_name} {strategy.version} - {strategy.readable_name}"
             traffic_light_icon = QtGui.QIcon()
             traffic_light_icon.addPixmap(icon_pixmap)
 
-            solie.window.comboBox_2.addItem(traffic_light_icon, text)
-            solie.window.comboBox.addItem(traffic_light_icon, text)
+            self.window.comboBox_2.addItem(traffic_light_icon, text)
+            self.window.comboBox.addItem(traffic_light_icon, text)
 
             strategy_card = QtWidgets.QGroupBox()
-            solie.window.verticalLayout_16.addWidget(strategy_card)
+            self.window.verticalLayout_16.addWidget(strategy_card)
             self.strategy_cards.append(strategy_card)
             card_layout = QtWidgets.QHBoxLayout(strategy_card)
 
             icon_label = QtWidgets.QLabel("")
             card_layout.addWidget(icon_label)
             icon_label.setPixmap(icon_pixmap)
             icon_label.setScaledContents(True)
@@ -120,123 +123,118 @@
                 QtWidgets.QSizePolicy.Policy.Expanding,
                 QtWidgets.QSizePolicy.Policy.Minimum,
             )
             card_layout.addItem(spacer)
 
             async def job_bs(strategy=strategy):
                 await self.remember_strategy_selections()
-                formation = [
+                await overlay(
                     "Develop your strategy",
-                    StrategyDevelopInput,
-                    True,
-                    strategy,
-                ]
-                await solie.window.overlay(formation)
+                    StrategyDevelopInput(strategy),
+                )
                 asyncio.create_task(self.display_strategies())
                 asyncio.create_task(self.save_strategies())
                 asyncio.create_task(self.restore_strategy_selections())
 
             edit_button = QtWidgets.QPushButton("Develop")
             card_layout.addWidget(edit_button)
-            outsource.do(edit_button.clicked, job_bs)
+            outsource(edit_button.clicked, job_bs)
 
             async def job_eb(strategy=strategy):
                 await self.remember_strategy_selections()
-                formation = [
+                await overlay(
                     "Edit your strategy's basic information",
-                    StrategyBasicInput,
-                    True,
-                    strategy,
-                ]
-                await solie.window.overlay(formation)
+                    StrategyBasicInput(strategy),
+                )
                 asyncio.create_task(self.display_strategies())
                 asyncio.create_task(self.save_strategies())
                 asyncio.create_task(self.restore_strategy_selections())
 
             edit_button = QtWidgets.QPushButton("Edit basic info")
             card_layout.addWidget(edit_button)
-            outsource.do(edit_button.clicked, job_eb)
+            outsource(edit_button.clicked, job_eb)
 
-            action_menu = QtWidgets.QMenu(solie.window)
+            action_menu = QtWidgets.QMenu(self.window)
             action_button = QtWidgets.QPushButton()
             action_button.setText("☰")
             action_button.setMenu(action_menu)
             card_layout.addWidget(action_button)
 
             async def job_rs(strategy=strategy):
-                question = [
+                answer = await ask(
                     "Remove this strategy?",
                     "Once you remove this, it cannot be recovered.",
                     ["Remove"],
-                ]
-                answer = await solie.window.ask(question)
+                )
                 if answer == 0:
                     return
                 await self.remember_strategy_selections()
-                self.strategies.remove(strategy)
+                self.strategies.all.remove(strategy)
                 asyncio.create_task(self.display_strategies())
                 asyncio.create_task(self.save_strategies())
                 asyncio.create_task(self.restore_strategy_selections())
 
             new_action = action_menu.addAction("Remove")
-            outsource.do(new_action.triggered, job_rs)
+            outsource(new_action.triggered, job_rs)
 
             async def job_dp(strategy=strategy):
                 await self.remember_strategy_selections()
-                duplicated = strategy.copy()
-                duplicated["code_name"] = standardize.create_strategy_code_name()
-                self.strategies.append(duplicated)
+                duplicated = replace(
+                    strategy,
+                    code_name=create_strategy_code_name(),
+                )
+                self.strategies.all.append(duplicated)
                 asyncio.create_task(self.display_strategies())
                 asyncio.create_task(self.save_strategies())
                 asyncio.create_task(self.restore_strategy_selections())
 
             new_action = action_menu.addAction("Duplicate")
-            outsource.do(new_action.triggered, job_dp)
+            outsource(new_action.triggered, job_dp)
 
             async def job_ss(strategy=strategy):
                 await self.remember_strategy_selections()
-                original_index = self.strategies.index(strategy)
+                original_index = self.strategies.all.index(strategy)
                 after_index = original_index + 1
-                self.strategies.pop(original_index)
-                self.strategies.insert(after_index, strategy)
+                self.strategies.all.pop(original_index)
+                self.strategies.all.insert(after_index, strategy)
                 asyncio.create_task(self.display_strategies())
                 asyncio.create_task(self.save_strategies())
                 asyncio.create_task(self.restore_strategy_selections())
 
             edit_button = QtWidgets.QPushButton("▼")
             card_layout.addWidget(edit_button)
-            outsource.do(edit_button.clicked, job_ss)
+            outsource(edit_button.clicked, job_ss)
 
             async def job_us(strategy=strategy):
                 await self.remember_strategy_selections()
-                original_index = self.strategies.index(strategy)
+                original_index = self.strategies.all.index(strategy)
                 after_index = original_index - 1
-                self.strategies.pop(original_index)
-                self.strategies.insert(after_index, strategy)
+                self.strategies.all.pop(original_index)
+                self.strategies.all.insert(after_index, strategy)
                 asyncio.create_task(self.display_strategies())
                 asyncio.create_task(self.save_strategies())
                 asyncio.create_task(self.restore_strategy_selections())
 
             edit_button = QtWidgets.QPushButton("▲")
             card_layout.addWidget(edit_button)
-            outsource.do(edit_button.clicked, job_us)
+            outsource(edit_button.clicked, job_us)
 
-    async def add_blank_strategy(self, *args, **kwargs):
+    async def add_blank_strategy(self):
         await self.remember_strategy_selections()
-        new_strategy = standardize.strategy()
-        self.strategies.append(new_strategy)
+        new_strategy = Strategy(code_name=create_strategy_code_name())
+        self.strategies.all.append(new_strategy)
         await self.display_strategies()
         await self.restore_strategy_selections()
 
-    async def remember_strategy_selections(self, *args, **kwargs):
-        before_index = solie.window.comboBox_2.currentIndex()
-        self.before_selections["transactor"] = self.strategies[before_index]
-        before_index = solie.window.comboBox.currentIndex()
-        self.before_selections["simulator"] = self.strategies[before_index]
-
-    async def restore_strategy_selections(self, *args, **kwargs):
-        if self.before_selections["transactor"] in self.strategies:
-            new_index = self.strategies.index(self.before_selections["transactor"])
-            solie.window.comboBox_2.setCurrentIndex(new_index)
-        if self.before_selections["simulator"] in self.strategies:
-            new_index = self.strategies.index(self.before_selections["simulator"])
-            solie.window.comboBox.setCurrentIndex(new_index)
+    async def remember_strategy_selections(self):
+        before_index = self.window.comboBox_2.currentIndex()
+        self.before_selections["transactor"] = self.strategies.all[before_index]
+        before_index = self.window.comboBox.currentIndex()
+        self.before_selections["simulator"] = self.strategies.all[before_index]
+
+    async def restore_strategy_selections(self):
+        if self.before_selections["transactor"] in self.strategies.all:
+            new_index = self.strategies.all.index(self.before_selections["transactor"])
+            self.window.comboBox_2.setCurrentIndex(new_index)
+        if self.before_selections["simulator"] in self.strategies.all:
+            new_index = self.strategies.all.index(self.before_selections["simulator"])
+            self.window.comboBox.setCurrentIndex(new_index)
```

### Comparing `solie-8.4.0/solie/worker/transactor.py` & `solie-8.5.0/solie/worker/transactor.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,294 +1,317 @@
 import asyncio
 import json
+import logging
 import math
-import os
 import pickle
 import re
 import webbrowser
 from datetime import datetime, timedelta, timezone
 
 import aiofiles
+import aiofiles.os
 import numpy as np
 import pandas as pd
+from apscheduler.schedulers.asyncio import AsyncIOScheduler
+from PySide6 import QtWidgets
 
-import solie
-from solie.definition.api_requester import ApiRequester
-from solie.definition.api_streamer import ApiStreamer
-from solie.definition.errors import ApiRequestError
-from solie.definition.rw_lock import RWLock
-from solie.overlay.long_text_view import LongTextView
-from solie.parallel import go
+from solie.common import go, outsource
+from solie.overlay import LongTextView
 from solie.utility import (
-    ball,
-    check_internet,
-    convert,
+    ApiRequester,
+    ApiRequestError,
+    ApiStreamer,
+    RWLock,
+    TransactionSettings,
+    add_connected_functions,
+    add_task_duration,
+    ball_ceil,
     decide,
+    find_stop_flag,
+    get_current_moment,
+    internet_connected,
+    list_to_dict,
     make_indicators,
-    remember_task_durations,
-    sort_pandas,
-    standardize,
-    stop_flag,
-    user_settings,
+    make_stop_flag,
+    sort_data_frame,
+    sort_series,
+    standardize_account_state,
+    standardize_asset_record,
+    standardize_unrealized_changes,
 )
+from solie.widget import ask, overlay
+from solie.window import Window
 
+from .united import team
 
-class Transactor:
-    def __init__(self):
-        # ■■■■■ for data management ■■■■■
+logger = logging.getLogger(__name__)
 
-        self.workerpath = user_settings.get_app_settings()["datapath"] + "/transactor"
-        os.makedirs(self.workerpath, exist_ok=True)
 
-        # ■■■■■ worker secret memory ■■■■■
+class Transactor:
+    def __init__(self, window: Window, scheduler: AsyncIOScheduler):
+        # ■■■■■ for data management ■■■■■
 
-        self.secret_memory = {
-            "maximum_quantities": {},
-            "minimum_notionals": {},
-            "price_precisions": {},
-            "quantity_precisions": {},
-            "maximum_leverages": {},
-            "leverages": {},
-            "is_key_restrictions_satisfied": True,
-        }
+        self.window = window
+        self.scheduler = scheduler
+        self.workerpath = window.datapath / "transactor"
+
+        # ■■■■■ internal memory ■■■■■
+
+        self.maximum_quantities: dict[str, float] = {}  # Symbol and value
+        self.minimum_notionals: dict[str, float] = {}  # Symbol and value
+        self.price_precisions: dict[str, int] = {}  # Symbol and decimal places
+        self.quantity_precisions: dict[str, int] = {}  # Symbol and decimal places
+        self.maximum_leverages: dict[str, int] = {}  # Symbol and value
+        self.leverages: dict[str, int] = {}  # Symbol and value
+        self.is_key_restrictions_satisfied = True
 
         # ■■■■■ remember and display ■■■■■
 
         self.api_requester = ApiRequester()
 
-        self.viewing_symbol = user_settings.get_data_settings()["target_symbols"][0]
+        self.viewing_symbol = window.data_settings.target_symbols[0]
         self.should_draw_frequently = True
 
-        self.account_state = standardize.account_state()
+        self.account_state = standardize_account_state(
+            window.data_settings.target_symbols
+        )
 
         self.scribbles = {}
-        self.automation_settings = {
-            "strategy_index": 0,
-            "should_transact": False,
-        }
-        self.mode_settings = {
-            "desired_leverage": 1,
-        }
-        self.keys = {
-            "binance_api": "",
-            "binance_secret": "",
-        }
-        self.unrealized_changes = RWLock(standardize.unrealized_changes())
-        self.asset_record = RWLock(standardize.asset_record())
+        self.transaction_settings = TransactionSettings()
+        self.unrealized_changes = RWLock(standardize_unrealized_changes())
+        self.asset_record = RWLock(standardize_asset_record())
         self.auto_order_record = RWLock(
             pd.DataFrame(
                 columns=[
                     "Symbol",
                     "Order ID",
                 ],
                 index=pd.DatetimeIndex([], tz="UTC"),
             )
         )
 
         # ■■■■■ repetitive schedules ■■■■■
 
-        solie.window.scheduler.add_job(
+        self.scheduler.add_job(
             self.display_status_information,
             trigger="cron",
             second="*",
         )
-        solie.window.scheduler.add_job(
+        self.scheduler.add_job(
             self.display_range_information,
             trigger="cron",
             second="*",
         )
-        solie.window.scheduler.add_job(
+        self.scheduler.add_job(
             self.cancel_conflicting_orders,
             trigger="cron",
             second="*",
         )
-        solie.window.scheduler.add_job(
+        self.scheduler.add_job(
             self.display_lines,
             trigger="cron",
             second="*/10",
             kwargs={"periodic": True, "frequent": True},
         )
-        solie.window.scheduler.add_job(
+        self.scheduler.add_job(
             self.pan_view_range,
             trigger="cron",
             second="*/10",
         )
-        solie.window.scheduler.add_job(
+        self.scheduler.add_job(
             self.perform_transaction,
             trigger="cron",
             second="*/10",
         )
-        solie.window.scheduler.add_job(
+        self.scheduler.add_job(
             self.save_scribbles,
             trigger="cron",
             second="*/10",
         )
-        solie.window.scheduler.add_job(
+        self.scheduler.add_job(
             self.watch_binance,
             trigger="cron",
             second="*/10",
         )
-        solie.window.scheduler.add_job(
+        self.scheduler.add_job(
             self.organize_data,
             trigger="cron",
             minute="*",
         )
-        solie.window.scheduler.add_job(
+        self.scheduler.add_job(
             self.save_large_data,
             trigger="cron",
             hour="*",
         )
 
         # ■■■■■ websocket streamings ■■■■■
 
         self.api_streamers = {
             "ACCOUNT": ApiStreamer(
                 "",
                 self.listen_to_account,
             )
         }
 
-        # ■■■■■ invoked by the internet connection status change  ■■■■■
+        # ■■■■■ invoked by the internet connection status change ■■■■■
 
-        check_internet.add_connected_functions(self.watch_binance)
+        add_connected_functions(self.watch_binance)
+
+        # ■■■■■ connect UI events ■■■■■
+
+        # Special widgets
+        job = self.display_range_information
+        outsource(window.plot_widget.sigRangeChanged, job)
+        job = self.set_minimum_view_range
+        outsource(window.plot_widget.sigRangeChanged, job)
+        job = self.update_automation_settings
+        outsource(window.comboBox_2.currentIndexChanged, job)
+        job = self.update_automation_settings
+        outsource(window.checkBox.toggled, job)
+        job = self.update_keys
+        outsource(window.lineEdit_4.editingFinished, job)
+        job = self.update_keys
+        outsource(window.lineEdit_6.editingFinished, job)
+        job = self.toggle_frequent_draw
+        outsource(window.checkBox_2.toggled, job)
+        job = self.display_day_range
+        outsource(window.pushButton_14.clicked, job)
+        job = self.update_mode_settings
+        outsource(window.spinBox.editingFinished, job)
+        job = self.update_viewing_symbol
+        outsource(window.comboBox_4.currentIndexChanged, job)
+
+        action_menu = QtWidgets.QMenu(self.window)
+        self.window.pushButton_12.setMenu(action_menu)
+
+        text = "Open Binance exchange"
+        job = self.open_exchange
+        new_action = action_menu.addAction(text)
+        outsource(new_action.triggered, job)
+        text = "Open Binance futures wallet"
+        job = self.open_futures_wallet_page
+        new_action = action_menu.addAction(text)
+        outsource(new_action.triggered, job)
+        text = "Open Binance API management webpage"
+        job = self.open_api_management_page
+        new_action = action_menu.addAction(text)
+        outsource(new_action.triggered, job)
+        text = "Clear all positions and open orders"
+        job = self.clear_positions_and_open_orders
+        new_action = action_menu.addAction(text)
+        outsource(new_action.triggered, job)
+        text = "Display same range as simulation graph"
+        job = self.match_graph_range
+        new_action = action_menu.addAction(text)
+        outsource(new_action.triggered, job)
+        text = "Show Raw Account State Object"
+        job = self.show_raw_account_state_object
+        new_action = action_menu.addAction(text)
+        outsource(new_action.triggered, job)
+
+    async def load(self):
+        await aiofiles.os.makedirs(self.workerpath, exist_ok=True)
 
-    async def load(self, *args, **kwargs):
         # scribbles
-        try:
-            filepath = self.workerpath + "/scribbles.pickle"
+        filepath = self.workerpath / "scribbles.pickle"
+        if await aiofiles.os.path.isfile(filepath):
             async with aiofiles.open(filepath, "rb") as file:
                 content = await file.read()
                 self.scribbles = pickle.loads(content)
-        except FileNotFoundError:
-            pass
-        await asyncio.sleep(0)
 
-        # automation settings
-        try:
-            filepath = self.workerpath + "/automation_settings.json"
+        # transaction settings
+        filepath = self.workerpath / "transaction_settings.json"
+        if await aiofiles.os.path.isfile(filepath):
             async with aiofiles.open(filepath, "r", encoding="utf8") as file:
-                content = await file.read()
-                read_data = json.loads(content)
-            self.automation_settings = read_data
-            state = read_data["should_transact"]
-            solie.window.checkBox.setChecked(state)
-            strategy_index = read_data["strategy_index"]
-            solie.window.comboBox_2.setCurrentIndex(strategy_index)
-        except FileNotFoundError:
-            pass
-        await asyncio.sleep(0)
-
-        # mode settings
-        try:
-            filepath = self.workerpath + "/mode_settings.json"
-            async with aiofiles.open(filepath, "r", encoding="utf8") as file:
-                content = await file.read()
-                read_data = json.loads(content)
-            self.mode_settings = read_data
-            new_value = read_data["desired_leverage"]
-            solie.window.spinBox.setValue(new_value)
-        except FileNotFoundError:
-            pass
-        await asyncio.sleep(0)
-
-        # keys
-        try:
-            filepath = self.workerpath + "/keys.json"
-            async with aiofiles.open(filepath, "r", encoding="utf8") as file:
-                content = await file.read()
-                keys = json.loads(content)
-            text = keys["binance_api"]
-            solie.window.lineEdit_4.setText(text)
-            text = keys["binance_secret"]
-            solie.window.lineEdit_6.setText(text)
-            self.keys = keys
-            self.api_requester.update_keys(keys)
-        except FileNotFoundError:
-            pass
-        await asyncio.sleep(0)
+                read_data = TransactionSettings.from_json(await file.read())
+            self.transaction_settings = read_data
+            state = read_data.should_transact
+            self.window.checkBox.setChecked(state)
+            strategy_index = read_data.strategy_index
+            self.window.comboBox_2.setCurrentIndex(strategy_index)
+            new_value = read_data.desired_leverage
+            self.window.spinBox.setValue(new_value)
+            text = read_data.binance_api_key
+            self.window.lineEdit_4.setText(text)
+            text = read_data.binance_api_secret
+            self.window.lineEdit_6.setText(text)
+            self.api_requester.update_keys(
+                read_data.binance_api_key, read_data.binance_api_secret
+            )
 
         # unrealized changes
-        try:
-            filepath = self.workerpath + "/unrealized_changes.pickle"
+        filepath = self.workerpath / "unrealized_changes.pickle"
+        if await aiofiles.os.path.isfile(filepath):
             self.unrealized_changes = RWLock(await go(pd.read_pickle, filepath))
-        except FileNotFoundError:
-            pass
-        await asyncio.sleep(0)
 
         # asset record
-        try:
-            filepath = self.workerpath + "/asset_record.pickle"
+        filepath = self.workerpath / "asset_record.pickle"
+        if await aiofiles.os.path.isfile(filepath):
             self.asset_record = RWLock(await go(pd.read_pickle, filepath))
-        except FileNotFoundError:
-            pass
-        await asyncio.sleep(0)
 
         # auto order record
-        try:
-            filepath = self.workerpath + "/auto_order_record.pickle"
+        filepath = self.workerpath / "auto_order_record.pickle"
+        if await aiofiles.os.path.isfile(filepath):
             self.auto_order_record = RWLock(await go(pd.read_pickle, filepath))
-        except FileNotFoundError:
-            pass
-        await asyncio.sleep(0)
 
-    async def organize_data(self, *args, **kwargs):
+    async def organize_data(self):
         async with self.unrealized_changes.write_lock as cell:
             if not cell.data.index.is_unique:
                 unique_index = cell.data.index.drop_duplicates()
                 cell.data = cell.data.reindex(unique_index)
             if not cell.data.index.is_monotonic_increasing:
-                cell.data = await go(sort_pandas.series, cell.data)
+                cell.data = await go(sort_series, cell.data)
 
         async with self.auto_order_record.write_lock as cell:
             if not cell.data.index.is_unique:
                 unique_index = cell.data.index.drop_duplicates()
                 cell.data = cell.data.reindex(unique_index)
             if not cell.data.index.is_monotonic_increasing:
-                cell.data = await go(sort_pandas.data_frame, cell.data)
+                cell.data = await go(sort_data_frame, cell.data)
             max_length = 2**16
             if len(cell.data) > max_length:
                 cell.data = cell.data.iloc[-max_length:].copy()
 
         async with self.asset_record.write_lock as cell:
             if not cell.data.index.is_unique:
                 unique_index = cell.data.index.drop_duplicates()
                 cell.data = cell.data.reindex(unique_index)
             if not cell.data.index.is_monotonic_increasing:
-                cell.data = await go(sort_pandas.data_frame, cell.data)
+                cell.data = await go(sort_data_frame, cell.data)
 
-    async def save_large_data(self, *args, **kwargs):
+    async def save_large_data(self):
         async with self.unrealized_changes.read_lock as cell:
             unrealized_changes = cell.data.copy()
         await go(
             unrealized_changes.to_pickle,
-            self.workerpath + "/unrealized_changes.pickle",
+            self.workerpath / "unrealized_changes.pickle",
         )
 
         async with self.auto_order_record.read_lock as cell:
             auto_order_record = cell.data.copy()
         await go(
             auto_order_record.to_pickle,
-            self.workerpath + "/auto_order_record.pickle",
+            self.workerpath / "auto_order_record.pickle",
         )
 
         async with self.asset_record.read_lock as cell:
             asset_record = cell.data.copy()
         await go(
             asset_record.to_pickle,
-            self.workerpath + "/asset_record.pickle",
+            self.workerpath / "asset_record.pickle",
         )
 
-    async def save_scribbles(self, *args, **kwargs):
-        filepath = self.workerpath + "/scribbles.pickle"
+    async def save_scribbles(self):
+        filepath = self.workerpath / "scribbles.pickle"
         async with aiofiles.open(filepath, "wb") as file:
             content = pickle.dumps(self.scribbles)
             await file.write(content)
 
-    async def update_user_data_stream(self, *args, **kwargs):
-        if not check_internet.connected():
+    async def update_user_data_stream(self):
+        if not internet_connected():
             return
 
         try:
             payload = {}
             response = await self.api_requester.binance(
                 http_method="POST",
                 path="/fapi/v1/listenKey",
@@ -300,58 +323,56 @@
         listen_key = response["listenKey"]
 
         self.api_streamers["ACCOUNT"] = ApiStreamer(
             "wss://fstream.binance.com/ws/" + listen_key,
             self.listen_to_account,
         )
 
-    async def listen_to_account(self, *args, **kwargs):
-        received = kwargs["received"]
-
+    async def listen_to_account(self, received: dict):
         # ■■■■■ default values ■■■■■
 
         event_type = received["e"]
         event_timestamp = received["E"] / 1000
         event_time = datetime.fromtimestamp(event_timestamp, tz=timezone.utc)
 
         self.account_state["observed_until"] = event_time
 
         # ■■■■■ do the task according to event type ■■■■■
 
         if event_type == "listenKeyExpired":
             text = "Binance user data stream listen key got expired"
-            solie.logger.warning(text)
+            logger.warning(text)
             await self.update_user_data_stream()
 
         if event_type == "ACCOUNT_UPDATE":
             about_update = received["a"]
             about_assets = about_update["B"]
             about_positions = about_update["P"]
 
-            asset_token = user_settings.get_data_settings()["asset_token"]
+            asset_token = self.window.data_settings.asset_token
 
-            about_assets_keyed = convert.list_to_dict(about_assets, "a")
+            about_assets_keyed = list_to_dict(about_assets, "a")
             if asset_token in about_assets_keyed:
                 about_asset = about_assets_keyed[asset_token]
                 wallet_balance = float(about_asset["wb"])
                 self.wallet_balance_state = wallet_balance
 
-            about_positions_keyed = convert.list_to_dict(about_positions, "ps")
+            about_positions_keyed = list_to_dict(about_positions, "ps")
             if "BOTH" in about_positions_keyed:
                 about_position = about_positions_keyed["BOTH"]
 
-                target_symbols = user_settings.get_data_settings()["target_symbols"]
+                target_symbols = self.window.data_settings.target_symbols
                 if about_position["s"] not in target_symbols:
                     return
 
                 symbol = about_position["s"]
                 amount = float(about_position["pa"])
                 entry_price = float(about_position["ep"])
 
-                leverage = self.secret_memory["leverages"][symbol]
+                leverage = self.leverages[symbol]
                 margin = abs(amount) * entry_price / leverage
                 if amount < 0:
                     direction = "short"
                 elif amount > 0:
                     direction = "long"
                 else:
                     direction = "none"
@@ -360,15 +381,15 @@
                 self.account_state["positions"][symbol]["direction"] = direction
                 self.account_state["positions"][symbol]["entry_price"] = entry_price
                 self.account_state["positions"][symbol]["update_time"] = event_time
 
         if event_type == "ORDER_TRADE_UPDATE":
             about_update = received["o"]
 
-            target_symbols = user_settings.get_data_settings()["target_symbols"]
+            target_symbols = self.window.data_settings.target_symbols
             if about_update["s"] not in target_symbols:
                 return
 
             # from received
             symbol = about_update.get("s")
             order_id = about_update.get("i")
             order_type = about_update.get("o")
@@ -385,15 +406,15 @@
             last_filled_price = float(about_update.get("L", 0))
             price = float(about_update.get("p", 0))
             stop_price = float(about_update.get("sp", 0))
             commission = float(about_update.get("n", 0))
             realized_profit = float(about_update.get("rp", 0))
 
             # from remembered
-            leverage = self.secret_memory["leverages"][symbol]
+            leverage = self.leverages[symbol]
             wallet_balance = self.account_state["wallet_balance"]
 
             # when the order is removed
             if order_status not in ("NEW", "PARTIALLY_FILLED"):
                 if order_id in self.account_state["open_orders"][symbol].keys():
                     self.account_state["open_orders"][symbol].pop(order_id)
 
@@ -519,118 +540,106 @@
                         new_value = last_asset + added_revenue
                         cell.data.loc[record_time, "Result Asset"] = new_value
                         if order_id in unique_order_ids:
                             cell.data.loc[record_time, "Cause"] = "auto_trade"
                         else:
                             cell.data.loc[record_time, "Cause"] = "manual_trade"
                     if not cell.data.index.is_monotonic_increasing:
-                        cell.data = await go(sort_pandas.data_frame, cell.data)
+                        cell.data = await go(sort_data_frame, cell.data)
 
         # ■■■■■ cancel conflicting orders ■■■■■
 
         await self.cancel_conflicting_orders()
 
-    async def open_exchange(self, *args, **kwargs):
+    async def open_exchange(self):
         symbol = self.viewing_symbol
         await go(
             webbrowser.open,
             f"https://www.binance.com/en/futures/{symbol}",
         )
 
-    async def open_futures_wallet_page(self, *args, **kwargs):
+    async def open_futures_wallet_page(self):
         await go(
             webbrowser.open,
             "https://www.binance.com/en/my/wallet/account/futures",
         )
 
-    async def open_api_management_page(self, *args, **kwargs):
+    async def open_api_management_page(self):
         await go(
             webbrowser.open,
             "https://www.binance.com/en/my/settings/api-management",
         )
 
-    async def update_keys(self, *args, **kwargs):
-        server = kwargs.get("server", "real")
-
-        binance_api = solie.window.lineEdit_4.text()
-        binance_secret = solie.window.lineEdit_6.text()
-
-        new_keys = {}
-        new_keys["binance_api"] = binance_api
-        new_keys["binance_secret"] = binance_secret
-
-        self.keys = new_keys
-
-        filepath = self.workerpath + "/keys.json"
+    async def save_transaction_settings(self):
+        filepath = self.workerpath / "transaction_settings.json"
         async with aiofiles.open(filepath, "w", encoding="utf8") as file:
-            content = json.dumps(new_keys, indent=4)
-            await file.write(content)
+            await file.write(self.transaction_settings.to_json(indent=2))
 
-        new_keys = {}
-        new_keys["server"] = server
-        new_keys["binance_api"] = binance_api
-        new_keys["binance_secret"] = binance_secret
+    async def update_keys(self):
+        binance_api_key = self.window.lineEdit_4.text()
+        binance_api_secret = self.window.lineEdit_6.text()
 
-        self.api_requester.update_keys(new_keys)
+        self.transaction_settings.binance_api_key = binance_api_key
+        self.transaction_settings.binance_api_secret = binance_api_secret
+
+        await self.save_transaction_settings()
+        self.api_requester.update_keys(binance_api_key, binance_api_secret)
         await self.update_user_data_stream()
 
-    async def update_automation_settings(self, *args, **kwargs):
+    async def update_automation_settings(self):
         # ■■■■■ get information about strategy ■■■■■
 
-        strategy_index = solie.window.comboBox_2.currentIndex()
-        self.automation_settings["strategy_index"] = strategy_index
+        strategy_index = self.window.comboBox_2.currentIndex()
+        self.transaction_settings.strategy_index = strategy_index
 
         asyncio.create_task(self.display_lines())
 
         # ■■■■■ is automation turned on ■■■■■
 
-        is_checked = solie.window.checkBox.isChecked()
+        is_checked = self.window.checkBox.isChecked()
 
         if is_checked:
-            self.automation_settings["should_transact"] = True
+            self.transaction_settings.should_transact = True
         else:
-            self.automation_settings["should_transact"] = False
+            self.transaction_settings.should_transact = False
 
         # ■■■■■ save ■■■■■
 
-        filepath = self.workerpath + "/automation_settings.json"
-        async with aiofiles.open(filepath, "w", encoding="utf8") as file:
-            content = json.dumps(self.automation_settings, indent=4)
-            await file.write(content)
+        await self.save_transaction_settings()
 
-    async def display_range_information(self, *args, **kwargs):
-        task_id = stop_flag.make("display_transaction_range_information")
+    async def display_range_information(self):
+        task_id = make_stop_flag("display_transaction_range_information")
 
         symbol = self.viewing_symbol
 
-        range_start_timestamp = solie.window.plot_widget.getAxis("bottom").range[0]
+        range_start_timestamp = self.window.plot_widget.getAxis("bottom").range[0]
         range_start_timestamp = max(range_start_timestamp, 0.0)
         range_start = datetime.fromtimestamp(range_start_timestamp, tz=timezone.utc)
 
-        if stop_flag.find("display_transaction_range_information", task_id):
+        if find_stop_flag("display_transaction_range_information", task_id):
             return
 
-        range_end_timestamp = solie.window.plot_widget.getAxis("bottom").range[1]
+        range_end_timestamp = self.window.plot_widget.getAxis("bottom").range[1]
         if range_end_timestamp < 0.0:
             # case when pyqtgraph passed negative value because it's too big
             range_end_timestamp = 9223339636.0
         else:
             # maximum value available in pandas
             range_end_timestamp = min(range_end_timestamp, 9223339636.0)
         range_end = datetime.fromtimestamp(range_end_timestamp, tz=timezone.utc)
 
-        if stop_flag.find("display_transaction_range_information", task_id):
+        if find_stop_flag("display_transaction_range_information", task_id):
             return
 
         range_length = range_end - range_start
         range_days = range_length.days
         range_hours, remains = divmod(range_length.seconds, 3600)
         range_minutes, remains = divmod(remains, 60)
 
-        if stop_flag.find("display_transaction_range_information", task_id):
+        if find_stop_flag("display_transaction_range_information", task_id):
             return
 
         async with self.unrealized_changes.read_lock as cell:
             unrealized_changes = cell.data[range_start:range_end].copy()
         async with self.asset_record.read_lock as cell:
             asset_record = cell.data[range_start:range_end].copy()
 
@@ -665,18 +674,18 @@
             symbol_yield = 0
         # least unrealized changes
         if len(unrealized_changes) > 0:
             min_unrealized_change = unrealized_changes.min()
         else:
             min_unrealized_change = 0
 
-        if stop_flag.find("display_transaction_range_information", task_id):
+        if find_stop_flag("display_transaction_range_information", task_id):
             return
 
-        view_range = solie.window.plot_widget.getAxis("left").range
+        view_range = self.window.plot_widget.getAxis("left").range
         range_down = view_range[0]
         range_up = view_range[1]
         price_range_height = (1 - range_down / range_up) * 100
 
         text = ""
         text += f"Visible time range {range_days}d {range_hours}h {range_minutes}s"
         text += "  ⦁  "
@@ -688,110 +697,106 @@
         text += "Transaction amount"
         text += f" ×{symbol_margin_ratio:.4f}({total_margin_ratio:.4f})"
         text += "  ⦁  "
         text += f"Total realized profit {symbol_yield:+.4f}({total_yield:+.4f})%"
         text += "  ⦁  "
         text += "Lowest unrealized profit"
         text += f" {min_unrealized_change*100:+.4f}%"
-        solie.window.label_8.setText(text)
+        self.window.label_8.setText(text)
 
-    async def set_minimum_view_range(self, *args, **kwargs):
-        widget = solie.window.plot_widget
+    async def set_minimum_view_range(self):
+        widget = self.window.plot_widget
         range_down = widget.getAxis("left").range[0]
         widget.plotItem.vb.setLimits(minYRange=range_down * 0.005)  # type:ignore
-        widget = solie.window.plot_widget_1
+        widget = self.window.plot_widget_1
         range_down = widget.getAxis("left").range[0]
         widget.plotItem.vb.setLimits(minYRange=range_down * 0.005)  # type:ignore
 
-    async def display_strategy_index(self, *args, **kwargs):
-        strategy_index = self.automation_settings["strategy_index"]
-        solie.window.comboBox_2.setCurrentIndex(strategy_index)
+    async def display_strategy_index(self):
+        strategy_index = self.transaction_settings.strategy_index
+        self.window.comboBox_2.setCurrentIndex(strategy_index)
 
-    async def display_lines(self, *args, **kwargs):
+    async def display_lines(self, periodic=False, frequent=False):
         # ■■■■■ start the task ■■■■■
 
-        periodic = kwargs.get("periodic", False)
-        frequent = kwargs.get("frequent", False)
-
         task_name = "display_transaction_lines"
 
-        task_id = stop_flag.make(task_name)
+        task_id = make_stop_flag(task_name)
 
         # ■■■■■ check drawing mode ■■■■■
 
         should_draw_frequently = self.should_draw_frequently
 
         if frequent:
             if not should_draw_frequently:
                 return
 
         # ■■■■■ check if the data exists ■■■■■
 
-        async with solie.window.collector.candle_data.read_lock as cell:
+        async with team.collector.candle_data.read_lock as cell:
             if len(cell.data) == 0:
                 return
 
         # ■■■■■ wait for the latest data to be added ■■■■■
 
-        current_moment = datetime.now(timezone.utc).replace(microsecond=0)
-        current_moment = current_moment - timedelta(seconds=current_moment.second % 10)
+        current_moment = get_current_moment()
         before_moment = current_moment - timedelta(seconds=10)
 
         if periodic:
             for _ in range(50):
-                if stop_flag.find(task_name, task_id):
+                if find_stop_flag(task_name, task_id):
                     return
-                async with solie.window.collector.candle_data.read_lock as cell:
+                async with team.collector.candle_data.read_lock as cell:
                     last_index = cell.data.index[-1]
                     if last_index == before_moment:
                         break
                 await asyncio.sleep(0.1)
 
         # ■■■■■ get ready for task duration measurement ■■■■■
 
         task_start_time = datetime.now(timezone.utc)
 
         # ■■■■■ check things ■■■■■
 
         symbol = self.viewing_symbol
-        strategy_index = self.automation_settings["strategy_index"]
-        strategy = solie.window.strategist.strategies[strategy_index]
+        strategy_index = self.transaction_settings.strategy_index
+        strategy = team.strategist.strategies.all[strategy_index]
 
         # ■■■■■ get light data ■■■■■
 
-        async with solie.window.collector.realtime_data_chunks.read_lock as cell:
+        async with team.collector.realtime_data_chunks.read_lock as cell:
             before_chunk = cell.data[-2].copy()
             current_chunk = cell.data[-1].copy()
         realtime_data = np.concatenate((before_chunk, current_chunk))
-        async with solie.window.collector.aggregate_trades.read_lock as cell:
+        async with team.collector.aggregate_trades.read_lock as cell:
             aggregate_trades = cell.data.copy()
 
         # ■■■■■ draw light lines ■■■■■
 
         # mark price
         data_x = realtime_data["index"].astype(np.int64) / 10**9
         data_y = realtime_data[str((symbol, "Mark Price"))]
         mask = data_y != 0
         data_y = data_y[mask]
         data_x = data_x[mask]
-        widget = solie.window.transaction_lines["mark_price"][0]
+        widget = self.window.transaction_lines["mark_price"][0]
         widget.setData(data_x, data_y)
-        if stop_flag.find(task_name, task_id):
+        if find_stop_flag(task_name, task_id):
             return
         await asyncio.sleep(0)
 
         # last price
         data_x = aggregate_trades["index"].astype(np.int64) / 10**9
         data_y = aggregate_trades[str((symbol, "Price"))]
         mask = data_y != 0
         data_y = data_y[mask]
         data_x = data_x[mask]
-        widget = solie.window.transaction_lines["last_price"][0]
+        widget = self.window.transaction_lines["last_price"][0]
         widget.setData(data_x, data_y)
-        if stop_flag.find(task_name, task_id):
+        if find_stop_flag(task_name, task_id):
             return
         await asyncio.sleep(0)
 
         # last trade volume
         index_ar = aggregate_trades["index"].astype(np.int64) / 10**9
         value_ar = aggregate_trades[str((symbol, "Volume"))]
         mask = value_ar != 0
@@ -799,40 +804,40 @@
         value_ar = value_ar[mask]
         length = len(index_ar)
         zero_ar = np.zeros(length)
         nan_ar = np.empty(length)
         nan_ar[:] = np.nan
         data_x = np.repeat(index_ar, 3)
         data_y = np.stack([nan_ar, zero_ar, value_ar], axis=1).reshape(-1)
-        widget = solie.window.transaction_lines["last_volume"][0]
+        widget = self.window.transaction_lines["last_volume"][0]
         widget.setData(data_x, data_y)
-        if stop_flag.find(task_name, task_id):
+        if find_stop_flag(task_name, task_id):
             return
         await asyncio.sleep(0)
 
         # book tickers
         data_x = realtime_data["index"].astype(np.int64) / 10**9
         data_y = realtime_data[str((symbol, "Best Bid Price"))]
         mask = data_y != 0
         data_y = data_y[mask]
         data_x = data_x[mask]
-        widget = solie.window.transaction_lines["book_tickers"][0]
+        widget = self.window.transaction_lines["book_tickers"][0]
         widget.setData(data_x, data_y)
-        if stop_flag.find(task_name, task_id):
+        if find_stop_flag(task_name, task_id):
             return
         await asyncio.sleep(0)
 
         data_x = realtime_data["index"].astype(np.int64) / 10**9
         data_y = realtime_data[str((symbol, "Best Ask Price"))]
         mask = data_y != 0
         data_y = data_y[mask]
         data_x = data_x[mask]
-        widget = solie.window.transaction_lines["book_tickers"][1]
+        widget = self.window.transaction_lines["book_tickers"][1]
         widget.setData(data_x, data_y)
-        if stop_flag.find(task_name, task_id):
+        if find_stop_flag(task_name, task_id):
             return
         await asyncio.sleep(0)
 
         # entry price
         entry_price = self.account_state["positions"][symbol]["entry_price"]
         first_moment = self.account_state["observed_until"] - timedelta(hours=12)
         last_moment = self.account_state["observed_until"] + timedelta(hours=12)
@@ -840,17 +845,17 @@
             data_x = np.linspace(
                 first_moment.timestamp(), last_moment.timestamp(), num=1000
             )
             data_y = np.linspace(entry_price, entry_price, num=1000)
         else:
             data_x = []
             data_y = []
-        widget = solie.window.transaction_lines["entry_price"][0]
+        widget = self.window.transaction_lines["entry_price"][0]
         widget.setData(data_x, data_y)
-        if stop_flag.find(task_name, task_id):
+        if find_stop_flag(task_name, task_id):
             return
         await asyncio.sleep(0)
 
         # ■■■■■ set range of heavy data ■■■■■
 
         if should_draw_frequently:
             get_from = datetime.now(timezone.utc) - timedelta(days=28)
@@ -861,15 +866,15 @@
             get_from = datetime(current_year, 1, 1, tzinfo=timezone.utc)
             slice_from = datetime(current_year, 1, 1, tzinfo=timezone.utc)
             slice_until = datetime.now(timezone.utc)
         slice_until -= timedelta(seconds=1)
 
         # ■■■■■ get heavy data ■■■■■
 
-        async with solie.window.collector.candle_data.read_lock as cell:
+        async with team.collector.candle_data.read_lock as cell:
             candle_data_original = cell.data[get_from:slice_until][[symbol]].copy()
         async with self.unrealized_changes.read_lock as cell:
             unrealized_changes = cell.data.copy()
         async with self.asset_record.read_lock as cell:
             if len(cell.data) > 0:
                 last_asset = cell.data.iloc[-1]["Result Asset"]
             else:
@@ -896,23 +901,23 @@
         if last_asset is not None:
             observed_until = self.account_state["observed_until"]
             if len(asset_record) == 0 or asset_record.index[-1] < observed_until:
                 if slice_from < observed_until:
                     asset_record.loc[observed_until, "Cause"] = "other"
                     asset_record.loc[observed_until, "Result Asset"] = last_asset
                     if not asset_record.index.is_monotonic_increasing:
-                        asset_record = await go(sort_pandas.data_frame, asset_record)
+                        asset_record = await go(sort_data_frame, asset_record)
 
         # add the left end
 
         if before_asset is not None:
             asset_record.loc[slice_from, "Cause"] = "other"
             asset_record.loc[slice_from, "Result Asset"] = before_asset
             if not asset_record.index.is_monotonic_increasing:
-                asset_record = await go(sort_pandas.data_frame, asset_record)
+                asset_record = await go(sort_data_frame, asset_record)
 
         # ■■■■■ draw heavy lines ■■■■■
 
         # price movement
         index_ar = candle_data.index.to_numpy(dtype=np.int64) / 10**9
         open_ar = candle_data[(symbol, "Open")].to_numpy()
         close_ar = candle_data[(symbol, "Close")].to_numpy()
@@ -949,17 +954,17 @@
                 nan_ar[rise_ar],
                 high_ar[rise_ar],
                 low_ar[rise_ar],
                 nan_ar[rise_ar],
             ],
             axis=1,
         ).reshape(-1)
-        widget = solie.window.transaction_lines["price_rise"][0]
+        widget = self.window.transaction_lines["price_rise"][0]
         widget.setData(data_x, data_y)
-        if stop_flag.find(task_name, task_id):
+        if find_stop_flag(task_name, task_id):
             return
         await asyncio.sleep(0)
 
         data_x = np.stack(
             [
                 index_ar[fall_ar] + 2,
                 index_ar[fall_ar] + 5,
@@ -983,17 +988,17 @@
                 nan_ar[fall_ar],
                 high_ar[fall_ar],
                 low_ar[fall_ar],
                 nan_ar[fall_ar],
             ],
             axis=1,
         ).reshape(-1)
-        widget = solie.window.transaction_lines["price_fall"][0]
+        widget = self.window.transaction_lines["price_fall"][0]
         widget.setData(data_x, data_y)
-        if stop_flag.find(task_name, task_id):
+        if find_stop_flag(task_name, task_id):
             return
         await asyncio.sleep(0)
 
         data_x = np.stack(
             [
                 index_ar[stay_ar] + 2,
                 index_ar[stay_ar] + 5,
@@ -1017,240 +1022,240 @@
                 nan_ar[stay_ar],
                 high_ar[stay_ar],
                 low_ar[stay_ar],
                 nan_ar[stay_ar],
             ],
             axis=1,
         ).reshape(-1)
-        widget = solie.window.transaction_lines["price_stay"][0]
+        widget = self.window.transaction_lines["price_stay"][0]
         widget.setData(data_x, data_y)
-        if stop_flag.find(task_name, task_id):
+        if find_stop_flag(task_name, task_id):
             return
         await asyncio.sleep(0)
 
         # wobbles
         sr = candle_data[(symbol, "High")]
         data_x = sr.index.to_numpy(dtype=np.int64) / 10**9
         data_y = sr.to_numpy(dtype=np.float32)
-        widget = solie.window.transaction_lines["wobbles"][0]
+        widget = self.window.transaction_lines["wobbles"][0]
         widget.setData(data_x, data_y)
-        if stop_flag.find(task_name, task_id):
+        if find_stop_flag(task_name, task_id):
             return
         await asyncio.sleep(0)
 
         sr = candle_data[(symbol, "Low")]
         data_x = sr.index.to_numpy(dtype=np.int64) / 10**9
         data_y = sr.to_numpy(dtype=np.float32)
-        widget = solie.window.transaction_lines["wobbles"][1]
+        widget = self.window.transaction_lines["wobbles"][1]
         widget.setData(data_x, data_y)
-        if stop_flag.find(task_name, task_id):
+        if find_stop_flag(task_name, task_id):
             return
         await asyncio.sleep(0)
 
         # trade volume
         sr = candle_data[(symbol, "Volume")]
         sr = sr.fillna(value=0)
         data_x = sr.index.to_numpy(dtype=np.int64) / 10**9
         data_y = sr.to_numpy(dtype=np.float32)
-        widget = solie.window.transaction_lines["volume"][0]
+        widget = self.window.transaction_lines["volume"][0]
         widget.setData(data_x, data_y)
-        if stop_flag.find(task_name, task_id):
+        if find_stop_flag(task_name, task_id):
             return
         await asyncio.sleep(0)
 
         # asset
         data_x = asset_record["Result Asset"].index.to_numpy(dtype=np.int64) / 10**9
         data_y = asset_record["Result Asset"].to_numpy(dtype=np.float32)
-        widget = solie.window.transaction_lines["asset"][0]
+        widget = self.window.transaction_lines["asset"][0]
         widget.setData(data_x, data_y)
-        if stop_flag.find(task_name, task_id):
+        if find_stop_flag(task_name, task_id):
             return
         await asyncio.sleep(0)
 
         # asset with unrealized profit
         sr = asset_record["Result Asset"]
         if len(sr) >= 2:
             sr = sr.resample("10S").ffill()
         unrealized_changes_sr = unrealized_changes.reindex(sr.index)
         sr = sr * (1 + unrealized_changes_sr)
         data_x = sr.index.to_numpy(dtype=np.int64) / 10**9 + 5
         data_y = sr.to_numpy(dtype=np.float32)
-        widget = solie.window.transaction_lines["asset_with_unrealized_profit"][0]
+        widget = self.window.transaction_lines["asset_with_unrealized_profit"][0]
         widget.setData(data_x, data_y)
-        if stop_flag.find(task_name, task_id):
+        if find_stop_flag(task_name, task_id):
             return
         await asyncio.sleep(0)
 
         # buy and sell
         df = asset_record.loc[asset_record["Symbol"] == symbol]
         df = df[df["Side"] == "sell"]
         sr = df["Fill Price"]
         data_x = sr.index.to_numpy(dtype=np.int64) / 10**9
         data_y = sr.to_numpy(dtype=np.float32)
-        widget = solie.window.transaction_lines["sell"][0]
+        widget = self.window.transaction_lines["sell"][0]
         widget.setData(data_x, data_y)
-        if stop_flag.find(task_name, task_id):
+        if find_stop_flag(task_name, task_id):
             return
         await asyncio.sleep(0)
 
         df = asset_record.loc[asset_record["Symbol"] == symbol]
         df = df[df["Side"] == "buy"]
         sr = df["Fill Price"]
         data_x = sr.index.to_numpy(dtype=np.int64) / 10**9
         data_y = sr.to_numpy(dtype=np.float32)
-        widget = solie.window.transaction_lines["buy"][0]
+        widget = self.window.transaction_lines["buy"][0]
         widget.setData(data_x, data_y)
-        if stop_flag.find(task_name, task_id):
+        if find_stop_flag(task_name, task_id):
             return
         await asyncio.sleep(0)
 
         # ■■■■■ record task duration ■■■■■
 
         duration = (datetime.now(timezone.utc) - task_start_time).total_seconds()
-        remember_task_durations.add(task_name, duration)
+        add_task_duration(task_name, duration)
 
         # ■■■■■ make indicators ■■■■■
 
-        indicators_script = strategy["indicators_script"]
+        indicators_script = strategy.indicators_script
 
         indicators = await go(
-            make_indicators.do,
+            make_indicators,
             target_symbols=[self.viewing_symbol],
             candle_data=candle_data_original,
             indicators_script=indicators_script,
         )
 
         indicators = indicators[slice_from:slice_until]
 
         # ■■■■■ draw strategy lines ■■■■■
 
         # price indicators
         df = indicators[symbol]["Price"]
         data_x = df.index.to_numpy(dtype=np.int64) / 10**9
         data_x += 5
-        line_list = solie.window.transaction_lines["price_indicators"]
+        line_list = self.window.transaction_lines["price_indicators"]
         for turn, widget in enumerate(line_list):
             if turn < len(df.columns):
                 column_name = df.columns[turn]
                 sr = df[column_name]
                 data_y = sr.to_numpy(dtype=np.float32)
                 inside_strings = re.findall(r"\(([^)]+)", column_name)
                 if len(inside_strings) == 0:
                     color = "#AAAAAA"
                 else:
                     color = inside_strings[0]
                 widget.setPen(color)
                 widget.setData(data_x, data_y)
-                if stop_flag.find(task_name, task_id):
+                if find_stop_flag(task_name, task_id):
                     return
                 await asyncio.sleep(0)
             else:
-                if stop_flag.find(task_name, task_id):
+                if find_stop_flag(task_name, task_id):
                     return
                 widget.clear()
 
         # trade volume indicators
         df = indicators[symbol]["Volume"]
         data_x = df.index.to_numpy(dtype=np.int64) / 10**9
         data_x += 5
-        line_list = solie.window.transaction_lines["volume_indicators"]
+        line_list = self.window.transaction_lines["volume_indicators"]
         for turn, widget in enumerate(line_list):
             if turn < len(df.columns):
                 column_name = df.columns[turn]
                 sr = df[column_name]
                 data_y = sr.to_numpy(dtype=np.float32)
                 inside_strings = re.findall(r"\(([^)]+)", column_name)
                 if len(inside_strings) == 0:
                     color = "#AAAAAA"
                 else:
                     color = inside_strings[0]
                 widget.setPen(color)
                 widget.setData(data_x, data_y)
-                if stop_flag.find(task_name, task_id):
+                if find_stop_flag(task_name, task_id):
                     return
                 await asyncio.sleep(0)
             else:
-                if stop_flag.find(task_name, task_id):
+                if find_stop_flag(task_name, task_id):
                     return
                 widget.clear()
 
         # abstract indicators
         df = indicators[symbol]["Abstract"]
         data_x = df.index.to_numpy(dtype=np.int64) / 10**9
         data_x += 5
-        line_list = solie.window.transaction_lines["abstract_indicators"]
+        line_list = self.window.transaction_lines["abstract_indicators"]
         for turn, widget in enumerate(line_list):
             if turn < len(df.columns):
                 column_name = df.columns[turn]
                 sr = df[column_name]
                 data_y = sr.to_numpy(dtype=np.float32)
                 inside_strings = re.findall(r"\(([^)]+)", column_name)
                 if len(inside_strings) == 0:
                     color = "#AAAAAA"
                 else:
                     color = inside_strings[0]
                 widget.setPen(color)
                 widget.setData(data_x, data_y)
-                if stop_flag.find(task_name, task_id):
+                if find_stop_flag(task_name, task_id):
                     return
                 await asyncio.sleep(0)
             else:
-                if stop_flag.find(task_name, task_id):
+                if find_stop_flag(task_name, task_id):
                     return
                 widget.clear()
 
         # ■■■■■ set minimum view range ■■■■■
 
         await self.set_minimum_view_range()
 
-    async def toggle_frequent_draw(self, *args, **kwargs):
-        is_checked = args[0]
+    async def toggle_frequent_draw(self):
+        is_checked = self.window.checkBox_2.isChecked()
         if is_checked:
             self.should_draw_frequently = True
         else:
             self.should_draw_frequently = False
         await self.display_lines()
 
-    async def update_viewing_symbol(self, *args, **kwargs):
-        alias = solie.window.comboBox_4.currentText()
-        symbol = solie.window.alias_to_symbol[alias]
+    async def update_viewing_symbol(self):
+        alias = self.window.comboBox_4.currentText()
+        symbol = self.window.alias_to_symbol[alias]
         self.viewing_symbol = symbol
 
         asyncio.create_task(self.display_lines())
         asyncio.create_task(self.display_status_information())
         asyncio.create_task(self.display_range_information())
 
-    async def display_status_information(self, *args, **kwargs):
+    async def display_status_information(self):
         # ■■■■■ Display important things first ■■■■■
 
         time_passed = datetime.now(timezone.utc) - self.account_state["observed_until"]
         if time_passed > timedelta(seconds=30):
             text = (
                 "Couldn't get the latest info on your Binance account due to a problem"
                 " with your key or connection to the Binance server."
             )
-            solie.window.label_16.setText(text)
+            self.window.label_16.setText(text)
             return
 
-        if not self.secret_memory["is_key_restrictions_satisfied"]:
+        if not self.is_key_restrictions_satisfied:
             text = (
                 "API key's restrictions are not satisfied. Auto transaction is"
                 " disabled. Go to your Binance API managements webpage to change"
                 " the restrictions."
             )
-            solie.window.label_16.setText(text)
+            self.window.label_16.setText(text)
             return
 
-        cumulation_rate = await solie.window.collector.get_candle_data_cumulation_rate()
+        cumulation_rate = await team.collector.check_candle_data_cumulation_rate()
         if cumulation_rate < 1:
             text = (
                 "For auto transaction to work, the past 24 hour accumulation rate of"
                 " candle data must be 100%. Auto transaction is disabled."
             )
-            solie.window.label_16.setText(text)
+            self.window.label_16.setText(text)
             return
 
         # ■■■■■ display assets and positions information ■■■■■
 
         position = self.account_state["positions"][self.viewing_symbol]
         if position["direction"] == "long":
             direction_text = "long"
@@ -1280,201 +1285,197 @@
         text += "Entry price"
         text += f" ＄{position['entry_price']:.4f}"
         text += "  ⦁  "
         text += "Open orders"
         text += f" {open_orders_count}"
         text += f"({all_open_orders_count})"
 
-        solie.window.label_16.setText(text)
+        self.window.label_16.setText(text)
 
-    async def perform_transaction(self, *args, **kwargs):
+    async def perform_transaction(self):
         # ■■■■■ Clear the progress bar ■■■■
 
-        solie.window.progressBar_2.setValue(0)
+        self.window.progressBar_2.setValue(0)
 
         # ■■■■■ Stop if conditions are not met ■■■■
 
-        if not check_internet.connected():
+        if not internet_connected():
             return
 
-        if not self.automation_settings["should_transact"]:
+        if not self.transaction_settings.should_transact:
             return
 
-        if not self.secret_memory["is_key_restrictions_satisfied"]:
+        if not self.is_key_restrictions_satisfied:
             return
 
-        cumulation_rate = await solie.window.collector.get_candle_data_cumulation_rate()
+        cumulation_rate = await team.collector.check_candle_data_cumulation_rate()
         if cumulation_rate < 1:
             return
 
         # ■■■■■ Moment ■■■■■
 
-        current_moment = datetime.now(timezone.utc).replace(microsecond=0)
-        current_moment = current_moment - timedelta(seconds=current_moment.second % 10)
+        current_moment = get_current_moment()
         before_moment = current_moment - timedelta(seconds=10)
 
         # ■■■■■ Play the progress bar ■■■■■
 
         is_cycle_done = False
 
         async def play_progress_bar():
             passed_time = timedelta(seconds=0)
             while passed_time < timedelta(seconds=10):
                 passed_time = datetime.now(timezone.utc) - current_moment
                 if not is_cycle_done:
                     new_value = int(passed_time / timedelta(seconds=10) * 1000)
                 else:
-                    before_value = solie.window.progressBar_2.value()
+                    before_value = self.window.progressBar_2.value()
                     remaining = 1000 - before_value
                     new_value = before_value + math.ceil(remaining * 0.2)
-                solie.window.progressBar_2.setValue(new_value)
+                self.window.progressBar_2.setValue(new_value)
                 await asyncio.sleep(0.01)
 
         asyncio.create_task(play_progress_bar())
 
         # ■■■■■ Check if the data exists ■■■■■
 
-        async with solie.window.collector.candle_data.read_lock as cell:
+        async with team.collector.candle_data.read_lock as cell:
             if len(cell.data) == 0:
                 # case when the app is executed for the first time
                 return
 
         # ■■■■■ Wait for the latest data to be added ■■■■■
 
         for _ in range(50):
-            async with solie.window.collector.candle_data.read_lock as cell:
+            async with team.collector.candle_data.read_lock as cell:
                 last_index = cell.data.index[-1]
                 if last_index == before_moment:
                     break
             await asyncio.sleep(0.1)
 
         # ■■■■■ Get the candle data ■■■■■
 
         slice_from = datetime.now(timezone.utc) - timedelta(days=28)
-        async with solie.window.collector.candle_data.read_lock as cell:
+        async with team.collector.candle_data.read_lock as cell:
             candle_data = cell.data[slice_from:].copy()
 
         # ■■■■■ Make decision ■■■■■
 
-        target_symbols = user_settings.get_data_settings()["target_symbols"]
+        target_symbols = self.window.data_settings.target_symbols
 
-        strategy_index = self.automation_settings["strategy_index"]
-        strategy = solie.window.strategist.strategies[strategy_index]
+        strategy_index = self.transaction_settings.strategy_index
+        strategy = team.strategist.strategies.all[strategy_index]
 
-        indicators_script = strategy["indicators_script"]
+        indicators_script = strategy.indicators_script
 
-        # Split the candle data by symbol before sending to reduct UI lags
-        indicators_per_symbol: dict[str, pd.DataFrame] = {}
+        # Split the candle data by symbol before calculation to reduct UI lags
+        coroutines = []
         for symbol in target_symbols:
-            symbol_indicators = await go(
-                make_indicators.do,
-                target_symbols=[symbol],
-                candle_data=candle_data[[symbol]],
-                indicators_script=indicators_script,
-                only_last_index=True,
+            coroutines.append(
+                go(
+                    make_indicators,
+                    target_symbols=[symbol],
+                    candle_data=candle_data[[symbol]],
+                    indicators_script=indicators_script,
+                    only_last_index=True,
+                )
             )
-            indicators_per_symbol[symbol] = symbol_indicators
-        indicators = pd.concat(indicators_per_symbol.values(), axis=1)
+            await asyncio.sleep(0)
+        symbol_indicators = await asyncio.gather(*coroutines)
+        indicators = pd.concat(symbol_indicators, axis="columns")
 
         current_candle_data: np.record = candle_data.tail(1).to_records()[-1]
         current_indicators: np.record = indicators.to_records()[-1]
-        decision_script = strategy["decision_script"]
+        decision_script = strategy.decision_script
 
         decision, scribbles = await go(
-            decide.choose,
+            decide,
             target_symbols=target_symbols,
             current_moment=current_moment,
             current_candle_data=current_candle_data,
             current_indicators=current_indicators,
             account_state=self.account_state,
             scribbles=self.scribbles,
             decision_script=decision_script,
         )
         self.scribbles = scribbles
 
         # ■■■■■ Record task duration ■■■■■
 
         is_cycle_done = True
         duration = (datetime.now(timezone.utc) - current_moment).total_seconds()
-        remember_task_durations.add("perform_transaction", duration)
+        add_task_duration("perform_transaction", duration)
 
         # ■■■■■ Place order ■■■■■
 
         await self.place_orders(decision)
 
-    async def display_day_range(self, *args, **kwargs):
+    async def display_day_range(self):
         range_start = (datetime.now(timezone.utc) - timedelta(hours=24)).timestamp()
         range_end = datetime.now(timezone.utc).timestamp()
-        widget = solie.window.plot_widget
+        widget = self.window.plot_widget
         widget.setXRange(range_start, range_end)
 
-    async def match_graph_range(self, *args, **kwargs):
-        range_start = solie.window.plot_widget_2.getAxis("bottom").range[0]
-        range_end = solie.window.plot_widget_2.getAxis("bottom").range[1]
-        widget = solie.window.plot_widget
+    async def match_graph_range(self):
+        range_start = self.window.plot_widget_2.getAxis("bottom").range[0]
+        range_end = self.window.plot_widget_2.getAxis("bottom").range[1]
+        widget = self.window.plot_widget
         widget.setXRange(range_start, range_end, padding=0)  # type:ignore
 
-    async def update_mode_settings(self, *args, **kwargs):
-        desired_leverage = solie.window.spinBox.value()
-        self.mode_settings["desired_leverage"] = desired_leverage
+    async def update_mode_settings(self):
+        desired_leverage = self.window.spinBox.value()
+        self.transaction_settings.desired_leverage = desired_leverage
 
         # ■■■■■ tell if some symbol's leverage cannot be set as desired ■■■■■
 
-        target_symbols = user_settings.get_data_settings()["target_symbols"]
+        target_symbols = self.window.data_settings.target_symbols
         target_max_leverages = {}
         for symbol in target_symbols:
-            max_leverage = self.secret_memory["maximum_leverages"].get(symbol, 125)
+            max_leverage = self.maximum_leverages.get(symbol, 125)
             target_max_leverages[symbol] = max_leverage
         lowest_max_leverage = min(target_max_leverages.values())
 
         if lowest_max_leverage < desired_leverage:
-            question = [
+            answer = await ask(
                 "Leverage on some symbols cannot be set as desired",
                 "Binance has its own leverage limit per market. For some symbols,"
                 " leverage will be set as high as it can be, but not as same as the"
                 " value entered. Generally, situation gets safer in terms of lowest"
                 " unrealized changes and profit turns out to be a bit lower than"
                 " simulation prediction with the same leverage.",
                 ["Show details", "Okay"],
-            ]
-            answer = await solie.window.ask(question)
+            )
             if answer == 1:
                 texts = []
                 for symbol, max_leverage in target_max_leverages.items():
                     texts.append(f"{symbol} {max_leverage}")
                 text = "\n".join(texts)
-                question = [
+                await ask(
                     "These are highest available leverages",
                     text,
                     ["Okay"],
-                ]
-                await solie.window.ask(question)
+                )
 
         # ■■■■■ save ■■■■■
 
-        filepath = self.workerpath + "/mode_settings.json"
-        async with aiofiles.open(filepath, "w", encoding="utf8") as file:
-            content = json.dumps(self.mode_settings, indent=4)
-            await file.write(content)
+        await self.save_transaction_settings()
 
-    async def watch_binance(self, *args, **kwargs):
+    async def watch_binance(self):
         # ■■■■■ Basic data ■■■■■
 
-        target_symbols = user_settings.get_data_settings()["target_symbols"]
-        asset_token = user_settings.get_data_settings()["asset_token"]
+        target_symbols = self.window.data_settings.target_symbols
+        asset_token = self.window.data_settings.asset_token
 
         # ■■■■■ Check internet connection ■■■■■
 
-        if not check_internet.connected():
+        if not internet_connected():
             return
 
         # ■■■■■ Moment ■■■■■
 
-        current_moment = datetime.now(timezone.utc).replace(microsecond=0)
-        current_moment = current_moment - timedelta(seconds=current_moment.second % 10)
+        current_moment = get_current_moment()
         before_moment = current_moment - timedelta(seconds=10)
 
         # ■■■■■ Request exchange information ■■■■■
 
         payload = {}
         response = await self.api_requester.binance(
             http_method="GET",
@@ -1483,32 +1484,32 @@
         )
         about_exchange = response
 
         for about_symbol in about_exchange["symbols"]:
             symbol = about_symbol["symbol"]
 
             about_filters = about_symbol["filters"]
-            about_filters_keyed = convert.list_to_dict(about_filters, "filterType")
+            about_filters_keyed = list_to_dict(about_filters, "filterType")
 
             minimum_notional = float(about_filters_keyed["MIN_NOTIONAL"]["notional"])
-            self.secret_memory["minimum_notionals"][symbol] = minimum_notional
+            self.minimum_notionals[symbol] = minimum_notional
 
             maximum_quantity = min(
                 float(about_filters_keyed["LOT_SIZE"]["maxQty"]),
                 float(about_filters_keyed["MARKET_LOT_SIZE"]["maxQty"]),
             )
-            self.secret_memory["maximum_quantities"][symbol] = maximum_quantity
+            self.maximum_quantities[symbol] = maximum_quantity
 
             ticksize = float(about_filters_keyed["PRICE_FILTER"]["tickSize"])
             price_precision = int(math.log10(1 / ticksize))
-            self.secret_memory["price_precisions"][symbol] = price_precision
+            self.price_precisions[symbol] = price_precision
 
             stepsize = float(about_filters_keyed["LOT_SIZE"]["stepSize"])
             quantity_precision = int(math.log10(1 / stepsize))
-            self.secret_memory["quantity_precisions"][symbol] = quantity_precision
+            self.quantity_precisions[symbol] = quantity_precision
 
         # ■■■■■ Request leverage bracket information ■■■■■
 
         try:
             payload = {
                 "timestamp": int(datetime.now(timezone.utc).timestamp() * 1000),
             }
@@ -1518,15 +1519,15 @@
                 payload=payload,
             )
             about_brackets = response
 
             for about_bracket in about_brackets:
                 symbol = about_bracket["symbol"]
                 max_leverage = about_bracket["brackets"][0]["initialLeverage"]
-                self.secret_memory["maximum_leverages"][symbol] = max_leverage
+                self.maximum_leverages[symbol] = max_leverage
         except ApiRequestError:
             # when the key is not ready
             return
 
         # ■■■■■ Request account information ■■■■■
 
         try:
@@ -1563,21 +1564,21 @@
         # ■■■■■ Update account state ■■■■■
 
         # observed until
         self.account_state["observed_until"] = current_moment
 
         # wallet_balance
         about_assets = about_account["assets"]
-        about_assets_keyed = convert.list_to_dict(about_assets, "asset")
+        about_assets_keyed = list_to_dict(about_assets, "asset")
         about_asset = about_assets_keyed[asset_token]
         wallet_balance = float(about_asset["walletBalance"])
         self.account_state["wallet_balance"] = wallet_balance
 
         about_positions = about_account["positions"]
-        about_positions_keyed = convert.list_to_dict(about_positions, "symbol")
+        about_positions_keyed = list_to_dict(about_positions, "symbol")
 
         # positions
         for symbol in target_symbols:
             about_position = about_positions_keyed[symbol]
 
             if float(about_position["notional"]) > 0:
                 direction = "long"
@@ -1695,30 +1696,30 @@
         self.account_state["open_orders"] = open_orders
 
         # ■■■■■ Update hidden state ■■■■■
 
         for symbol in target_symbols:
             about_position = about_positions_keyed[symbol]
             leverage = int(about_position["leverage"])
-            self.secret_memory["leverages"][symbol] = leverage
+            self.leverages[symbol] = leverage
 
         # ■■■■■ Record unrealized change ■■■■■
 
         # unrealized profit is not included in walletBalance
         wallet_balance = float(about_asset["walletBalance"])
         if wallet_balance != 0:
             unrealized_profit = float(about_asset["unrealizedProfit"])
             unrealized_change = unrealized_profit / wallet_balance
         else:
             unrealized_change = 0
 
         async with self.unrealized_changes.write_lock as cell:
             cell.data[before_moment] = unrealized_change
             if not cell.data.index.is_monotonic_increasing:
-                cell.data = await go(sort_pandas.series, cell.data)
+                cell.data = await go(sort_series, cell.data)
 
         # ■■■■■ Make an asset trace if it's blank ■■■■■
 
         async with self.asset_record.write_lock as cell:
             if len(cell.data) == 0:
                 wallet_balance = float(about_asset["walletBalance"])
                 current_time = datetime.now(timezone.utc)
@@ -1739,31 +1740,31 @@
             # when the difference is bigger than a billionth
             # referal fee, funding fee, wallet transfer, etc..
             async with self.asset_record.write_lock as cell:
                 current_time = datetime.now(timezone.utc)
                 cell.data.loc[current_time, "Cause"] = "other"
                 cell.data.loc[current_time, "Result Asset"] = wallet_balance
                 if not cell.data.index.is_monotonic_increasing:
-                    cell.data = await go(sort_pandas.data_frame, cell.data)
+                    cell.data = await go(sort_data_frame, cell.data)
         else:
             # when the difference is small enough to consider as an numeric error
             async with self.asset_record.write_lock as cell:
                 last_index = cell.data.index[-1]
                 cell.data.loc[last_index, "Result Asset"] = wallet_balance
 
         # ■■■■■ Correct mode of the account market if automation is turned on ■■■■■
 
-        if self.automation_settings["should_transact"]:
+        if self.transaction_settings.should_transact:
 
             async def job_1(symbol):
                 about_position = about_positions_keyed[symbol]
                 current_leverage = int(about_position["leverage"])
 
-                desired_leverage = self.mode_settings["desired_leverage"]
-                maximum_leverages = self.secret_memory["maximum_leverages"]
+                desired_leverage = self.transaction_settings.desired_leverage
+                maximum_leverages = self.maximum_leverages
                 max_leverage = maximum_leverages.get(symbol, 125)
                 goal_leverage = min(desired_leverage, max_leverage)
 
                 if current_leverage != goal_leverage:
                     timestamp = int(datetime.now(timezone.utc).timestamp() * 1000)
                     payload = {
                         "symbol": symbol,
@@ -1856,23 +1857,22 @@
         enable_required_restrictions = [
             "enableFutures",
         ]
         for restriction_name in enable_required_restrictions:
             is_enabled = api_restrictions[restriction_name]
             if not is_enabled:
                 is_satisfied = False
-        self.secret_memory["is_key_restrictions_satisfied"] = is_satisfied
+        self.is_key_restrictions_satisfied = is_satisfied
 
-    async def place_orders(self, *args, **kwargs):
-        decision = args[0]
-        target_symbols = user_settings.get_data_settings()["target_symbols"]
+    async def place_orders(self, decision: dict):
+        target_symbols = self.window.data_settings.target_symbols
 
         current_prices: dict[str, float] = {}
         for symbol in target_symbols:
-            async with solie.window.collector.aggregate_trades.read_lock as cell:
+            async with team.collector.aggregate_trades.read_lock as cell:
                 ar = cell.data[-10000:].copy()
             temp_ar = ar[str((symbol, "Price"))]
             temp_ar = temp_ar[temp_ar != 0]
             current_prices[symbol] = float(temp_ar[-1])
 
         # cancel_all
         # now_close
@@ -1908,15 +1908,15 @@
             update_time = datetime.fromtimestamp(timestamp, tz=timezone.utc)
             async with self.auto_order_record.write_lock as cell:
                 while update_time in cell.data.index:
                     update_time += timedelta(milliseconds=1)
                 cell.data.loc[update_time, "Symbol"] = order_symbol
                 cell.data.loc[update_time, "Order ID"] = order_id
                 if not cell.data.index.is_monotonic_increasing:
-                    cell.data = await go(sort_pandas.data_frame, cell.data)
+                    cell.data = await go(sort_data_frame, cell.data)
 
         # ■■■■■ Do cancel orders ■■■■■
 
         # These orders must be executed one after another.
         # For example, some `later_orders` expect a position made from `now_orders`
         cancel_orders = []
 
@@ -1940,105 +1940,95 @@
         now_orders = []
 
         for symbol in target_symbols:
             if symbol not in decision:
                 continue
 
             current_price = current_prices[symbol]
-            leverage = self.secret_memory["leverages"][symbol]
-            maximum_quantity = self.secret_memory["maximum_quantities"][symbol]
-            minimum_notional = self.secret_memory["minimum_notionals"][symbol]
-            price_precision = self.secret_memory["price_precisions"][symbol]
-            quantity_precision = self.secret_memory["quantity_precisions"][symbol]
+            leverage = self.leverages[symbol]
+            maximum_quantity = self.maximum_quantities[symbol]
+            minimum_notional = self.minimum_notionals[symbol]
+            quantity_precision = self.quantity_precisions[symbol]
+            current_direction = self.account_state["positions"][symbol]["direction"]
 
             if "now_close" in decision[symbol]:
-                is_possible = True
                 command = decision[symbol]["now_close"]
                 quantity = maximum_quantity
-                if self.account_state["positions"][symbol]["direction"] == "long":
-                    side = "SELL"
-                elif self.account_state["positions"][symbol]["direction"] == "short":
-                    side = "BUY"
-                else:
-                    side = "NONE"  # Dummy
-                    is_possible = False
-                if is_possible:
+                if current_direction in ("long", "short"):
+                    order_side = "SELL" if current_direction == "long" else "BUY"
                     new_order = {
                         "timestamp": int(datetime.now(timezone.utc).timestamp() * 1000),
                         "symbol": symbol,
                         "type": "MARKET",
-                        "side": side,
+                        "side": order_side,
                         "quantity": quantity,
                         "reduceOnly": True,
                         "newOrderRespType": "RESULT",
                     }
                     now_orders.append(new_order)
+                else:
+                    logger.warn("Cannot close position when there isn't any")
 
             if "now_buy" in decision[symbol]:
                 command = decision[symbol]["now_buy"]
                 notional = max(minimum_notional, float(command["margin"]) * leverage)
                 quantity = min(maximum_quantity, notional / current_price)
                 new_order = {
                     "timestamp": int(datetime.now(timezone.utc).timestamp() * 1000),
                     "symbol": symbol,
                     "type": "MARKET",
                     "side": "BUY",
-                    "quantity": ball.ceil(quantity, quantity_precision),
+                    "quantity": ball_ceil(quantity, quantity_precision),
                     "newOrderRespType": "RESULT",
                 }
                 now_orders.append(new_order)
 
             if "now_sell" in decision[symbol]:
                 command = decision[symbol]["now_sell"]
                 notional = max(minimum_notional, float(command["margin"]) * leverage)
                 quantity = min(maximum_quantity, notional / current_price)
                 new_order = {
                     "timestamp": int(datetime.now(timezone.utc).timestamp() * 1000),
                     "symbol": symbol,
                     "type": "MARKET",
                     "side": "SELL",
-                    "quantity": ball.ceil(quantity, quantity_precision),
+                    "quantity": ball_ceil(quantity, quantity_precision),
                     "newOrderRespType": "RESULT",
                 }
                 now_orders.append(new_order)
 
         if now_orders:
             tasks = [asyncio.create_task(job_new_order(o)) for o in now_orders]
             await asyncio.wait(tasks)
 
-        # ■■■■■ Wait for the positions to be affected by now orders ■■■■■
-
-        await asyncio.sleep(2.0)
-
         # ■■■■■ Do book orders ■■■■■
 
         book_orders = []
 
         for symbol in target_symbols:
             if symbol not in decision:
                 continue
 
-            current_price = current_prices[symbol]
-            leverage = self.secret_memory["leverages"][symbol]
-            maximum_quantity = self.secret_memory["maximum_quantities"][symbol]
-            minimum_notional = self.secret_memory["minimum_notionals"][symbol]
-            price_precision = self.secret_memory["price_precisions"][symbol]
-            quantity_precision = self.secret_memory["quantity_precisions"][symbol]
+            leverage = self.leverages[symbol]
+            maximum_quantity = self.maximum_quantities[symbol]
+            minimum_notional = self.minimum_notionals[symbol]
+            price_precision = self.price_precisions[symbol]
+            quantity_precision = self.quantity_precisions[symbol]
 
             if "book_buy" in decision[symbol]:
                 command = decision[symbol]["book_buy"]
                 notional = max(minimum_notional, float(command["margin"]) * leverage)
                 boundary = float(command["boundary"])
                 quantity = min(maximum_quantity, notional / boundary)
                 new_order = {
                     "timestamp": int(datetime.now(timezone.utc).timestamp() * 1000),
                     "symbol": symbol,
                     "type": "LIMIT",
                     "side": "BUY",
-                    "quantity": ball.ceil(quantity, quantity_precision),
+                    "quantity": ball_ceil(quantity, quantity_precision),
                     "price": round(boundary, price_precision),
                     "timeInForce": "GTC",
                 }
                 book_orders.append(new_order)
 
             if "book_sell" in decision[symbol]:
                 command = decision[symbol]["book_sell"]
@@ -2046,15 +2036,15 @@
                 boundary = float(command["boundary"])
                 quantity = min(maximum_quantity, notional / boundary)
                 new_order = {
                     "timestamp": int(datetime.now(timezone.utc).timestamp() * 1000),
                     "symbol": symbol,
                     "type": "LIMIT",
                     "side": "SELL",
-                    "quantity": ball.ceil(quantity, quantity_precision),
+                    "quantity": ball_ceil(quantity, quantity_precision),
                     "price": round(boundary, price_precision),
                     "timeInForce": "GTC",
                 }
                 book_orders.append(new_order)
 
         if book_orders:
             tasks = [asyncio.create_task(job_new_order(o)) for o in book_orders]
@@ -2064,150 +2054,154 @@
 
         later_orders = []
 
         for symbol in target_symbols:
             if symbol not in decision:
                 continue
 
-            current_price = current_prices[symbol]
-            leverage = self.secret_memory["leverages"][symbol]
-            maximum_quantity = self.secret_memory["maximum_quantities"][symbol]
-            minimum_notional = self.secret_memory["minimum_notionals"][symbol]
-            price_precision = self.secret_memory["price_precisions"][symbol]
-            quantity_precision = self.secret_memory["quantity_precisions"][symbol]
+            leverage = self.leverages[symbol]
+            maximum_quantity = self.maximum_quantities[symbol]
+            minimum_notional = self.minimum_notionals[symbol]
+            price_precision = self.price_precisions[symbol]
+            quantity_precision = self.quantity_precisions[symbol]
+            current_direction = self.account_state["positions"][symbol]["direction"]
+
+            # Even if there's no open position analyzed yet
+            # due to user data stream from Binance being slow,
+            # it's possible to assume that a position would have already been created
+            # if there was a `now_buy` or `now_sell` order.
+            if current_direction == "none":
+                if "now_buy" in decision[symbol]:
+                    current_direction = "long"
+                elif "now_sell" in decision[symbol]:
+                    current_direction = "short"
 
             if "later_up_close" in decision[symbol]:
-                is_possible = True
                 command = decision[symbol]["later_up_close"]
-                if self.account_state["positions"][symbol]["direction"] == "long":
-                    new_order_side = "SELL"
-                    new_order_type = "TAKE_PROFIT_MARKET"
-                elif self.account_state["positions"][symbol]["direction"] == "short":
-                    new_order_side = "BUY"
-                    new_order_type = "STOP_MARKET"
-                else:
-                    new_order_side = "NONE"  # Dummy
-                    new_order_type = "NONE"  # Dummy
-                    is_possible = False
-                if is_possible:
+                if current_direction in ("long", "short"):
+                    if current_direction == "long":
+                        order_side = "SELL"
+                        order_type = "TAKE_PROFIT_MARKET"
+                    else:
+                        order_side = "BUY"
+                        order_type = "STOP_MARKET"
                     new_order = {
                         "timestamp": int(datetime.now(timezone.utc).timestamp() * 1000),
                         "symbol": symbol,
-                        "type": new_order_type,
-                        "side": new_order_side,
+                        "type": order_type,
+                        "side": order_side,
                         "stopPrice": round(float(command["boundary"]), price_precision),
                         "closePosition": True,
                     }
                     later_orders.append(new_order)
+                else:
+                    logger.warn("Cannot place `later_up_close` with no open position")
 
             if "later_down_close" in decision[symbol]:
-                is_possible = True
                 command = decision[symbol]["later_down_close"]
-                if self.account_state["positions"][symbol]["direction"] == "long":
-                    new_order_side = "SELL"
-                    new_order_type = "STOP_MARKET"
-                elif self.account_state["positions"][symbol]["direction"] == "short":
-                    new_order_side = "BUY"
-                    new_order_type = "TAKE_PROFIT_MARKET"
-                else:
-                    new_order_side = "NONE"  # Dummy
-                    new_order_type = "NONE"  # Dummy
-                    is_possible = False
-                if is_possible:
+                if current_direction in ("long", "short"):
+                    if current_direction == "long":
+                        order_side = "SELL"
+                        order_type = "STOP_MARKET"
+                    else:
+                        order_side = "BUY"
+                        order_type = "TAKE_PROFIT_MARKET"
                     new_order = {
                         "timestamp": int(datetime.now(timezone.utc).timestamp() * 1000),
                         "symbol": symbol,
-                        "type": new_order_type,
-                        "side": new_order_side,
+                        "type": order_type,
+                        "side": order_side,
                         "stopPrice": round(float(command["boundary"]), price_precision),
                         "closePosition": True,
                     }
                     later_orders.append(new_order)
+                else:
+                    logger.warn("Cannot place `later_down_close` with no open position")
 
             if "later_up_buy" in decision[symbol]:
                 command = decision[symbol]["later_up_buy"]
                 notional = max(minimum_notional, float(command["margin"]) * leverage)
                 boundary = float(command["boundary"])
                 quantity = min(maximum_quantity, notional / boundary)
                 new_order = {
                     "timestamp": int(datetime.now(timezone.utc).timestamp() * 1000),
                     "symbol": symbol,
                     "type": "STOP_MARKET",
                     "side": "BUY",
-                    "quantity": ball.ceil(quantity, quantity_precision),
+                    "quantity": ball_ceil(quantity, quantity_precision),
                     "stopPrice": round(boundary, price_precision),
                 }
                 later_orders.append(new_order)
 
             if "later_down_buy" in decision[symbol]:
                 command = decision[symbol]["later_down_buy"]
                 notional = max(minimum_notional, float(command["margin"]) * leverage)
                 boundary = float(command["boundary"])
                 quantity = min(maximum_quantity, notional / boundary)
                 new_order = {
                     "timestamp": int(datetime.now(timezone.utc).timestamp() * 1000),
                     "symbol": symbol,
                     "type": "TAKE_PROFIT_MARKET",
                     "side": "BUY",
-                    "quantity": ball.ceil(quantity, quantity_precision),
+                    "quantity": ball_ceil(quantity, quantity_precision),
                     "stopPrice": round(boundary, price_precision),
                 }
                 later_orders.append(new_order)
 
             if "later_up_sell" in decision[symbol]:
                 command = decision[symbol]["later_up_sell"]
                 notional = max(minimum_notional, float(command["margin"]) * leverage)
                 boundary = float(command["boundary"])
                 quantity = min(maximum_quantity, notional / boundary)
                 new_order = {
                     "timestamp": int(datetime.now(timezone.utc).timestamp() * 1000),
                     "symbol": symbol,
                     "type": "TAKE_PROFIT_MARKET",
                     "side": "SELL",
-                    "quantity": ball.ceil(quantity, quantity_precision),
+                    "quantity": ball_ceil(quantity, quantity_precision),
                     "stopPrice": round(boundary, price_precision),
                 }
                 later_orders.append(new_order)
 
             if "later_down_sell" in decision[symbol]:
                 command = decision[symbol]["later_down_sell"]
                 notional = max(minimum_notional, float(command["margin"]) * leverage)
                 boundary = float(command["boundary"])
                 quantity = min(maximum_quantity, notional / boundary)
                 new_order = {
                     "timestamp": int(datetime.now(timezone.utc).timestamp() * 1000),
                     "symbol": symbol,
                     "type": "STOP_MARKET",
                     "side": "SELL",
-                    "quantity": ball.ceil(quantity, quantity_precision),
+                    "quantity": ball_ceil(quantity, quantity_precision),
                     "stopPrice": round(boundary, price_precision),
                 }
                 later_orders.append(new_order)
 
         if later_orders:
             tasks = [asyncio.create_task(job_new_order(o)) for o in later_orders]
             await asyncio.wait(tasks)
 
-    async def clear_positions_and_open_orders(self, *args, **kwargs):
+    async def clear_positions_and_open_orders(self):
         decision = {}
-        for symbol in user_settings.get_data_settings()["target_symbols"]:
+        for symbol in self.window.data_settings.target_symbols:
             decision[symbol] = {
                 "cancel_all": {},
                 "now_close": {},
             }
         await self.place_orders(decision)
 
-    async def cancel_conflicting_orders(self, *args, **kwargs):
-        if not self.automation_settings["should_transact"]:
+    async def cancel_conflicting_orders(self):
+        if not self.transaction_settings.should_transact:
             return
 
         conflicting_order_tuples = []
-        for symbol in user_settings.get_data_settings()["target_symbols"]:
+        for symbol in self.window.data_settings.target_symbols:
             symbol_open_orders = self.account_state["open_orders"][symbol]
-            groups_by_command = {}
+            groups_by_command: dict[str, list[int]] = {}
             for order_id, open_order_state in symbol_open_orders.items():
                 command_name = open_order_state["command_name"]
                 if command_name not in groups_by_command.keys():
                     groups_by_command[command_name] = [order_id]
                 else:
                     groups_by_command[command_name].append(order_id)
             for command_name, group in groups_by_command.items():
@@ -2235,38 +2229,35 @@
             except ApiRequestError:
                 pass
 
         if conflicting_order_tuples:
             tasks = [asyncio.create_task(job(c)) for c in conflicting_order_tuples]
             await asyncio.wait(tasks)
 
-    async def pan_view_range(self, *args, **kwargs):
+    async def pan_view_range(self):
         if not self.should_draw_frequently:
             return
 
-        widget = solie.window.plot_widget
+        widget = self.window.plot_widget
         before_range = widget.getAxis("bottom").range
         range_start = before_range[0]
         range_end = before_range[1]
 
         if range_end - range_start < 6 * 60 * 60:  # six hours
             return
 
         widget.setXRange(range_start + 10, range_end + 10, padding=0)  # type:ignore
 
-    async def show_raw_account_state_object(self, *args, **kwargs):
+    async def show_raw_account_state_object(self):
         text = ""
 
         time = datetime.now(timezone.utc)
         time_text = time.strftime("%Y-%m-%d %H:%M:%S")
         text += f"At UTC {time_text}"
 
         text += "\n\n"
-        text += json.dumps(self.account_state, indent=4, default=str)
+        text += json.dumps(self.account_state, indent=2, default=str)
 
-        formation = [
+        await overlay(
             "This is the raw account state object",
-            LongTextView,
-            True,
-            [text],
-        ]
-        await solie.window.overlay(formation)
+            LongTextView(text),
+        )
```

### Comparing `solie-8.4.0/PKG-INFO` & `solie-8.5.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: solie
-Version: 8.4.0
+Version: 8.5.0
 Summary: GUI trading bot designed for targeting the futures markets of Binance
 Home-page: https://github.com/cunarist/solie
 Author: Cunarist
 Requires-Python: >=3.9,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: aiodns (>=3.1.1,<4.0.0)
 Requires-Dist: aiofiles (>=23.2.1,<24.0.0)
 Requires-Dist: aiohttp (>=3.8.6,<4.0.0)
 Requires-Dist: apscheduler (>=3.10.4,<4.0.0)
+Requires-Dist: dataclasses-json (>=0.6.4,<0.7.0)
 Requires-Dist: faust-cchardet (>=2.1.19,<3.0.0)
 Requires-Dist: getmac (>=0.8.3,<0.9.0)
 Requires-Dist: numpy (>=1.26.2,<2.0.0)
 Requires-Dist: pandas (>=1.5.3,<2.0.0)
 Requires-Dist: pandas-ta (>=0.3.14b,<0.4.0)
 Requires-Dist: pygments (>=2.17.1,<3.0.0)
 Requires-Dist: pyqtgraph (>=0.13.4,<0.14.0)
```

