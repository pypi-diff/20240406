# Comparing `tmp/solie-8.5.0.tar.gz` & `tmp/solie-8.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "solie-8.5.0.tar", max compression
+gzip compressed data, was "solie-8.5.1.tar", max compression
```

## Comparing `solie-8.5.0.tar` & `solie-8.5.1.tar`

### file list

```diff
@@ -1,79 +1,79 @@
--rw-r--r--   0        0        0      787 2024-04-06 13:51:29.779391 solie-8.5.0/pyproject.toml
--rw-r--r--   0        0        0     2478 2024-03-09 13:27:55.333963 solie-8.5.0/README.md
--rw-r--r--   0        0        0       65 2024-04-04 12:33:45.799336 solie-8.5.0/solie/__init__.py
--rw-r--r--   0        0        0       85 2024-04-04 12:41:05.189192 solie-8.5.0/solie/__main__.py
--rw-r--r--   0        0        0      363 2024-04-05 00:02:40.054806 solie-8.5.0/solie/common/__init__.py
--rw-r--r--   0        0        0      293 2024-04-04 11:56:27.778407 solie-8.5.0/solie/common/connect_event.py
--rw-r--r--   0        0        0      280 2024-04-05 00:02:06.898492 solie-8.5.0/solie/common/info.py
--rw-r--r--   0        0        0     1259 2024-04-04 12:51:28.608601 solie-8.5.0/solie/common/parallel.py
--rw-r--r--   0        0        0       65 2024-04-04 11:36:05.301867 solie-8.5.0/solie/entry/__init__.py
--rw-r--r--   0        0        0     4156 2024-04-05 11:40:24.240903 solie-8.5.0/solie/entry/lifetime.py
--rw-r--r--   0        0        0      202 2024-04-05 11:30:17.371547 solie-8.5.0/solie/entry/start.py
--rw-r--r--   0        0        0      668 2024-04-03 16:31:10.028573 solie-8.5.0/solie/overlay/__init__.py
--rw-r--r--   0        0        0     8585 2024-04-04 13:05:54.660856 solie-8.5.0/solie/overlay/coin_selection.py
--rw-r--r--   0        0        0     4493 2024-04-04 11:57:06.554716 solie-8.5.0/solie/overlay/datapath_input.py
--rw-r--r--   0        0        0     2203 2024-04-03 16:31:10.033574 solie-8.5.0/solie/overlay/donation_guide.py
--rw-r--r--   0        0        0     2716 2024-04-04 11:58:19.815741 solie-8.5.0/solie/overlay/download_fill_option.py
--rw-r--r--   0        0        0      646 2024-04-03 16:31:10.037100 solie-8.5.0/solie/overlay/long_text_view.py
--rw-r--r--   0        0        0     8055 2024-04-04 11:58:27.486831 solie-8.5.0/solie/overlay/strategy_basic_input.py
--rw-r--r--   0        0        0     6210 2024-04-05 11:56:28.614118 solie-8.5.0/solie/overlay/strategy_develop_input.py
--rw-r--r--   0        0        0     2441 2024-04-03 16:31:10.041098 solie-8.5.0/solie/overlay/strategy_info_view.py
--rw-r--r--   0        0        0     7816 2024-04-04 13:09:54.727633 solie-8.5.0/solie/overlay/token_selection.py
--rw-r--r--   0        0        0    10899 2024-03-09 13:27:55.378483 solie-8.5.0/solie/static/icon/blank_coin.png
--rw-r--r--   0        0        0    11242 2024-03-09 13:27:55.379480 solie-8.5.0/solie/static/icon/traffic_light_green.png
--rw-r--r--   0        0        0    11165 2024-03-09 13:27:55.379480 solie-8.5.0/solie/static/icon/traffic_light_red.png
--rw-r--r--   0        0        0    10810 2024-03-09 13:27:55.380992 solie-8.5.0/solie/static/icon/traffic_light_yellow.png
--rw-r--r--   0        0        0    78060 2024-03-09 13:27:55.382001 solie-8.5.0/solie/static/lexend_bold.ttf
--rw-r--r--   0        0        0   556216 2024-03-09 13:27:55.388006 solie-8.5.0/solie/static/notosans_regular.ttf
--rw-r--r--   0        0        0   228761 2024-03-09 13:27:55.391007 solie-8.5.0/solie/static/product_icon.ico
--rw-r--r--   0        0        0   165542 2024-03-09 13:27:55.393001 solie-8.5.0/solie/static/product_icon.png
--rw-r--r--   0        0        0     1678 2024-03-29 12:50:13.329402 solie-8.5.0/solie/static/sample_decision_script.txt
--rw-r--r--   0        0        0     1015 2024-03-29 12:49:25.127196 solie-8.5.0/solie/static/sample_indicators_script.txt
--rw-r--r--   0        0        0   120456 2024-03-09 13:27:55.396002 solie-8.5.0/solie/static/source_code_pro.ttf
--rw-r--r--   0        0        0     3064 2024-04-06 11:43:43.146126 solie-8.5.0/solie/utility/__init__.py
--rw-r--r--   0        0        0    30449 2024-04-04 11:33:50.635949 solie-8.5.0/solie/utility/analyze_market.py
--rw-r--r--   0        0        0     3599 2024-04-03 16:31:10.045095 solie-8.5.0/solie/utility/api_requester.py
--rw-r--r--   0        0        0     2261 2024-04-04 14:21:39.539090 solie-8.5.0/solie/utility/api_streamer.py
--rw-r--r--   0        0        0     3762 2024-04-03 16:31:10.047095 solie-8.5.0/solie/utility/backward_compatibility.py
--rw-r--r--   0        0        0      379 2024-04-01 16:30:30.467934 solie-8.5.0/solie/utility/ball.py
--rw-r--r--   0        0        0     2238 2024-04-04 12:25:21.345905 solie-8.5.0/solie/utility/check_internet.py
--rw-r--r--   0        0        0      475 2024-04-01 16:30:30.473475 solie-8.5.0/solie/utility/compare_versions.py
--rw-r--r--   0        0        0      624 2024-03-30 00:54:45.144782 solie-8.5.0/solie/utility/convert.py
--rw-r--r--   0        0        0     7329 2024-04-06 10:20:38.815616 solie-8.5.0/solie/utility/download_from_binance.py
--rw-r--r--   0        0        0     2368 2024-04-04 14:26:08.098735 solie-8.5.0/solie/utility/log_handler.py
--rw-r--r--   0        0        0      294 2024-04-03 16:31:10.051094 solie-8.5.0/solie/utility/pandas_related.py
--rw-r--r--   0        0        0     2272 2024-04-03 16:31:10.052097 solie-8.5.0/solie/utility/percent_axis_item.py
--rw-r--r--   0        0        0     8065 2024-04-03 23:15:40.155486 solie-8.5.0/solie/utility/rw_lock.py
--rw-r--r--   0        0        0      251 2024-04-03 16:31:10.055105 solie-8.5.0/solie/utility/simply_format.py
--rw-r--r--   0        0        0      229 2024-04-01 16:30:30.488484 solie-8.5.0/solie/utility/sort_pandas.py
--rw-r--r--   0        0        0     1647 2024-04-03 16:31:10.057101 solie-8.5.0/solie/utility/standardize.py
--rw-r--r--   0        0        0      484 2024-04-03 16:31:10.058095 solie-8.5.0/solie/utility/stop_flag.py
--rw-r--r--   0        0        0     1107 2024-04-03 16:31:10.059097 solie-8.5.0/solie/utility/structs.py
--rw-r--r--   0        0        0     2272 2024-04-03 16:31:10.060102 solie-8.5.0/solie/utility/syntax_highlighter.py
--rw-r--r--   0        0        0     4848 2024-04-04 12:09:23.272841 solie-8.5.0/solie/utility/time_axis_item.py
--rw-r--r--   0        0        0      926 2024-04-06 11:42:39.262331 solie-8.5.0/solie/utility/timing.py
--rw-r--r--   0        0        0     1624 2024-04-03 16:31:10.062097 solie-8.5.0/solie/utility/user_settings.py
--rw-r--r--   0        0        0      813 2024-04-03 17:07:30.543145 solie-8.5.0/solie/widget/__init__.py
--rw-r--r--   0        0        0     5292 2024-04-04 11:59:09.143773 solie-8.5.0/solie/widget/ask_popup.py
--rw-r--r--   0        0        0      312 2024-04-01 14:45:12.996498 solie-8.5.0/solie/widget/brand_label.py
--rw-r--r--   0        0        0      836 2024-04-01 14:45:14.358385 solie-8.5.0/solie/widget/gauge.py
--rw-r--r--   0        0        0      236 2024-04-01 14:45:14.989682 solie-8.5.0/solie/widget/horizontal_divider.py
--rw-r--r--   0        0        0     1922 2024-04-04 11:59:20.593678 solie-8.5.0/solie/widget/log_list.py
--rw-r--r--   0        0        0     4184 2024-04-04 23:30:33.899456 solie-8.5.0/solie/widget/overlay_popup.py
--rw-r--r--   0        0        0       83 2024-04-01 14:45:50.650424 solie-8.5.0/solie/widget/popup_box.py
--rw-r--r--   0        0        0     3202 2024-04-03 16:31:10.068616 solie-8.5.0/solie/widget/script_editor.py
--rw-r--r--   0        0        0     2576 2024-04-03 16:31:10.069616 solie-8.5.0/solie/widget/splash_screen.py
--rw-r--r--   0        0        0       84 2024-04-01 14:04:49.291376 solie-8.5.0/solie/widget/symbol_box.py
--rw-r--r--   0        0        0       98 2024-04-01 14:04:49.292379 solie-8.5.0/solie/widget/transparent_scroll_area.py
--rw-r--r--   0        0        0      233 2024-04-01 14:04:49.293376 solie-8.5.0/solie/widget/vertical_divider.py
--rw-r--r--   0        0        0       50 2024-04-03 16:31:10.070617 solie-8.5.0/solie/window/__init__.py
--rw-r--r--   0        0        0    61287 2024-04-06 01:35:32.018253 solie-8.5.0/solie/window/compiled.py
--rw-r--r--   0        0        0    35529 2024-04-04 14:37:31.636472 solie-8.5.0/solie/window/main.py
--rw-r--r--   0        0        0      319 2024-04-04 11:50:37.144088 solie-8.5.0/solie/worker/__init__.py
--rw-r--r--   0        0        0    32281 2024-04-06 12:49:54.725669 solie-8.5.0/solie/worker/collector.py
--rw-r--r--   0        0        0    12495 2024-04-06 10:12:12.050859 solie-8.5.0/solie/worker/manager.py
--rw-r--r--   0        0        0    59289 2024-04-06 11:46:25.564267 solie-8.5.0/solie/worker/simulator.py
--rw-r--r--   0        0        0    10598 2024-04-04 12:31:28.938266 solie-8.5.0/solie/worker/strategist.py
--rw-r--r--   0        0        0    93573 2024-04-06 13:35:04.602646 solie-8.5.0/solie/worker/transactor.py
--rw-r--r--   0        0        0      695 2024-04-04 11:45:07.528915 solie-8.5.0/solie/worker/united.py
--rw-r--r--   0        0        0     3699 1970-01-01 00:00:00.000000 solie-8.5.0/PKG-INFO
+-rw-r--r--   0        0        0      787 2024-04-06 14:04:14.127818 solie-8.5.1/pyproject.toml
+-rw-r--r--   0        0        0     2478 2024-03-09 13:27:55.333963 solie-8.5.1/README.md
+-rw-r--r--   0        0        0       65 2024-04-04 12:33:45.799336 solie-8.5.1/solie/__init__.py
+-rw-r--r--   0        0        0       85 2024-04-04 12:41:05.189192 solie-8.5.1/solie/__main__.py
+-rw-r--r--   0        0        0      363 2024-04-05 00:02:40.054806 solie-8.5.1/solie/common/__init__.py
+-rw-r--r--   0        0        0      293 2024-04-04 11:56:27.778407 solie-8.5.1/solie/common/connect_event.py
+-rw-r--r--   0        0        0      280 2024-04-05 00:02:06.898492 solie-8.5.1/solie/common/info.py
+-rw-r--r--   0        0        0     1259 2024-04-04 12:51:28.608601 solie-8.5.1/solie/common/parallel.py
+-rw-r--r--   0        0        0       65 2024-04-04 11:36:05.301867 solie-8.5.1/solie/entry/__init__.py
+-rw-r--r--   0        0        0     4156 2024-04-05 11:40:24.240903 solie-8.5.1/solie/entry/lifetime.py
+-rw-r--r--   0        0        0      202 2024-04-05 11:30:17.371547 solie-8.5.1/solie/entry/start.py
+-rw-r--r--   0        0        0      668 2024-04-03 16:31:10.028573 solie-8.5.1/solie/overlay/__init__.py
+-rw-r--r--   0        0        0     8585 2024-04-04 13:05:54.660856 solie-8.5.1/solie/overlay/coin_selection.py
+-rw-r--r--   0        0        0     4493 2024-04-04 11:57:06.554716 solie-8.5.1/solie/overlay/datapath_input.py
+-rw-r--r--   0        0        0     2203 2024-04-03 16:31:10.033574 solie-8.5.1/solie/overlay/donation_guide.py
+-rw-r--r--   0        0        0     2716 2024-04-04 11:58:19.815741 solie-8.5.1/solie/overlay/download_fill_option.py
+-rw-r--r--   0        0        0      646 2024-04-03 16:31:10.037100 solie-8.5.1/solie/overlay/long_text_view.py
+-rw-r--r--   0        0        0     8055 2024-04-04 11:58:27.486831 solie-8.5.1/solie/overlay/strategy_basic_input.py
+-rw-r--r--   0        0        0     6210 2024-04-05 11:56:28.614118 solie-8.5.1/solie/overlay/strategy_develop_input.py
+-rw-r--r--   0        0        0     2441 2024-04-03 16:31:10.041098 solie-8.5.1/solie/overlay/strategy_info_view.py
+-rw-r--r--   0        0        0     7816 2024-04-04 13:09:54.727633 solie-8.5.1/solie/overlay/token_selection.py
+-rw-r--r--   0        0        0    10899 2024-03-09 13:27:55.378483 solie-8.5.1/solie/static/icon/blank_coin.png
+-rw-r--r--   0        0        0    11242 2024-03-09 13:27:55.379480 solie-8.5.1/solie/static/icon/traffic_light_green.png
+-rw-r--r--   0        0        0    11165 2024-03-09 13:27:55.379480 solie-8.5.1/solie/static/icon/traffic_light_red.png
+-rw-r--r--   0        0        0    10810 2024-03-09 13:27:55.380992 solie-8.5.1/solie/static/icon/traffic_light_yellow.png
+-rw-r--r--   0        0        0    78060 2024-03-09 13:27:55.382001 solie-8.5.1/solie/static/lexend_bold.ttf
+-rw-r--r--   0        0        0   556216 2024-03-09 13:27:55.388006 solie-8.5.1/solie/static/notosans_regular.ttf
+-rw-r--r--   0        0        0   228761 2024-03-09 13:27:55.391007 solie-8.5.1/solie/static/product_icon.ico
+-rw-r--r--   0        0        0   165542 2024-03-09 13:27:55.393001 solie-8.5.1/solie/static/product_icon.png
+-rw-r--r--   0        0        0     1678 2024-03-29 12:50:13.329402 solie-8.5.1/solie/static/sample_decision_script.txt
+-rw-r--r--   0        0        0     1015 2024-03-29 12:49:25.127196 solie-8.5.1/solie/static/sample_indicators_script.txt
+-rw-r--r--   0        0        0   120456 2024-03-09 13:27:55.396002 solie-8.5.1/solie/static/source_code_pro.ttf
+-rw-r--r--   0        0        0     3064 2024-04-06 11:43:43.146126 solie-8.5.1/solie/utility/__init__.py
+-rw-r--r--   0        0        0    30449 2024-04-04 11:33:50.635949 solie-8.5.1/solie/utility/analyze_market.py
+-rw-r--r--   0        0        0     3599 2024-04-03 16:31:10.045095 solie-8.5.1/solie/utility/api_requester.py
+-rw-r--r--   0        0        0     2261 2024-04-04 14:21:39.539090 solie-8.5.1/solie/utility/api_streamer.py
+-rw-r--r--   0        0        0     3762 2024-04-03 16:31:10.047095 solie-8.5.1/solie/utility/backward_compatibility.py
+-rw-r--r--   0        0        0      379 2024-04-01 16:30:30.467934 solie-8.5.1/solie/utility/ball.py
+-rw-r--r--   0        0        0     2238 2024-04-04 12:25:21.345905 solie-8.5.1/solie/utility/check_internet.py
+-rw-r--r--   0        0        0      475 2024-04-01 16:30:30.473475 solie-8.5.1/solie/utility/compare_versions.py
+-rw-r--r--   0        0        0      624 2024-03-30 00:54:45.144782 solie-8.5.1/solie/utility/convert.py
+-rw-r--r--   0        0        0     7329 2024-04-06 10:20:38.815616 solie-8.5.1/solie/utility/download_from_binance.py
+-rw-r--r--   0        0        0     2368 2024-04-04 14:26:08.098735 solie-8.5.1/solie/utility/log_handler.py
+-rw-r--r--   0        0        0      294 2024-04-03 16:31:10.051094 solie-8.5.1/solie/utility/pandas_related.py
+-rw-r--r--   0        0        0     2272 2024-04-03 16:31:10.052097 solie-8.5.1/solie/utility/percent_axis_item.py
+-rw-r--r--   0        0        0     8065 2024-04-03 23:15:40.155486 solie-8.5.1/solie/utility/rw_lock.py
+-rw-r--r--   0        0        0      251 2024-04-03 16:31:10.055105 solie-8.5.1/solie/utility/simply_format.py
+-rw-r--r--   0        0        0      229 2024-04-01 16:30:30.488484 solie-8.5.1/solie/utility/sort_pandas.py
+-rw-r--r--   0        0        0     1647 2024-04-03 16:31:10.057101 solie-8.5.1/solie/utility/standardize.py
+-rw-r--r--   0        0        0      484 2024-04-03 16:31:10.058095 solie-8.5.1/solie/utility/stop_flag.py
+-rw-r--r--   0        0        0     1107 2024-04-03 16:31:10.059097 solie-8.5.1/solie/utility/structs.py
+-rw-r--r--   0        0        0     2272 2024-04-03 16:31:10.060102 solie-8.5.1/solie/utility/syntax_highlighter.py
+-rw-r--r--   0        0        0     4848 2024-04-04 12:09:23.272841 solie-8.5.1/solie/utility/time_axis_item.py
+-rw-r--r--   0        0        0      926 2024-04-06 11:42:39.262331 solie-8.5.1/solie/utility/timing.py
+-rw-r--r--   0        0        0     1624 2024-04-03 16:31:10.062097 solie-8.5.1/solie/utility/user_settings.py
+-rw-r--r--   0        0        0      813 2024-04-03 17:07:30.543145 solie-8.5.1/solie/widget/__init__.py
+-rw-r--r--   0        0        0     5292 2024-04-04 11:59:09.143773 solie-8.5.1/solie/widget/ask_popup.py
+-rw-r--r--   0        0        0      312 2024-04-01 14:45:12.996498 solie-8.5.1/solie/widget/brand_label.py
+-rw-r--r--   0        0        0      836 2024-04-01 14:45:14.358385 solie-8.5.1/solie/widget/gauge.py
+-rw-r--r--   0        0        0      236 2024-04-01 14:45:14.989682 solie-8.5.1/solie/widget/horizontal_divider.py
+-rw-r--r--   0        0        0     1922 2024-04-04 11:59:20.593678 solie-8.5.1/solie/widget/log_list.py
+-rw-r--r--   0        0        0     4184 2024-04-04 23:30:33.899456 solie-8.5.1/solie/widget/overlay_popup.py
+-rw-r--r--   0        0        0       83 2024-04-01 14:45:50.650424 solie-8.5.1/solie/widget/popup_box.py
+-rw-r--r--   0        0        0     3202 2024-04-03 16:31:10.068616 solie-8.5.1/solie/widget/script_editor.py
+-rw-r--r--   0        0        0     2576 2024-04-03 16:31:10.069616 solie-8.5.1/solie/widget/splash_screen.py
+-rw-r--r--   0        0        0       84 2024-04-01 14:04:49.291376 solie-8.5.1/solie/widget/symbol_box.py
+-rw-r--r--   0        0        0       98 2024-04-01 14:04:49.292379 solie-8.5.1/solie/widget/transparent_scroll_area.py
+-rw-r--r--   0        0        0      233 2024-04-01 14:04:49.293376 solie-8.5.1/solie/widget/vertical_divider.py
+-rw-r--r--   0        0        0       50 2024-04-03 16:31:10.070617 solie-8.5.1/solie/window/__init__.py
+-rw-r--r--   0        0        0    61287 2024-04-06 01:35:32.018253 solie-8.5.1/solie/window/compiled.py
+-rw-r--r--   0        0        0    35529 2024-04-04 14:37:31.636472 solie-8.5.1/solie/window/main.py
+-rw-r--r--   0        0        0      319 2024-04-04 11:50:37.144088 solie-8.5.1/solie/worker/__init__.py
+-rw-r--r--   0        0        0    32281 2024-04-06 12:49:54.725669 solie-8.5.1/solie/worker/collector.py
+-rw-r--r--   0        0        0    12495 2024-04-06 10:12:12.050859 solie-8.5.1/solie/worker/manager.py
+-rw-r--r--   0        0        0    59289 2024-04-06 11:46:25.564267 solie-8.5.1/solie/worker/simulator.py
+-rw-r--r--   0        0        0    10598 2024-04-04 12:31:28.938266 solie-8.5.1/solie/worker/strategist.py
+-rw-r--r--   0        0        0    93922 2024-04-06 14:03:38.138786 solie-8.5.1/solie/worker/transactor.py
+-rw-r--r--   0        0        0      695 2024-04-04 11:45:07.528915 solie-8.5.1/solie/worker/united.py
+-rw-r--r--   0        0        0     3699 1970-01-01 00:00:00.000000 solie-8.5.1/PKG-INFO
```

### Comparing `solie-8.5.0/pyproject.toml` & `solie-8.5.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "solie"
-version = "8.5.0"
+version = "8.5.1"
 description = "GUI trading bot designed for targeting the futures markets of Binance"
 authors = ["Cunarist"]
 readme = "README.md"
 repository = "https://github.com/cunarist/solie"
 
 [tool.poetry.dependencies]
 python = "^3.9,<3.13"
```

### Comparing `solie-8.5.0/README.md` & `solie-8.5.1/README.md`

 * *Files identical despite different names*

### Comparing `solie-8.5.0/solie/common/parallel.py` & `solie-8.5.1/solie/common/parallel.py`

 * *Files identical despite different names*

### Comparing `solie-8.5.0/solie/entry/lifetime.py` & `solie-8.5.1/solie/entry/lifetime.py`

 * *Files identical despite different names*

### Comparing `solie-8.5.0/solie/overlay/__init__.py` & `solie-8.5.1/solie/overlay/__init__.py`

 * *Files identical despite different names*

### Comparing `solie-8.5.0/solie/overlay/coin_selection.py` & `solie-8.5.1/solie/overlay/coin_selection.py`

 * *Files identical despite different names*

### Comparing `solie-8.5.0/solie/overlay/datapath_input.py` & `solie-8.5.1/solie/overlay/datapath_input.py`

 * *Files identical despite different names*

### Comparing `solie-8.5.0/solie/overlay/donation_guide.py` & `solie-8.5.1/solie/overlay/donation_guide.py`

 * *Files identical despite different names*

### Comparing `solie-8.5.0/solie/overlay/download_fill_option.py` & `solie-8.5.1/solie/overlay/download_fill_option.py`

 * *Files identical despite different names*

### Comparing `solie-8.5.0/solie/overlay/long_text_view.py` & `solie-8.5.1/solie/overlay/long_text_view.py`

 * *Files identical despite different names*

### Comparing `solie-8.5.0/solie/overlay/strategy_basic_input.py` & `solie-8.5.1/solie/overlay/strategy_basic_input.py`

 * *Files identical despite different names*

### Comparing `solie-8.5.0/solie/overlay/strategy_develop_input.py` & `solie-8.5.1/solie/overlay/strategy_develop_input.py`

 * *Files identical despite different names*

### Comparing `solie-8.5.0/solie/overlay/strategy_info_view.py` & `solie-8.5.1/solie/overlay/strategy_info_view.py`

 * *Files identical despite different names*

### Comparing `solie-8.5.0/solie/overlay/token_selection.py` & `solie-8.5.1/solie/overlay/token_selection.py`

 * *Files identical despite different names*

### Comparing `solie-8.5.0/solie/static/icon/blank_coin.png` & `solie-8.5.1/solie/static/icon/blank_coin.png`

 * *Files identical despite different names*

### Comparing `solie-8.5.0/solie/static/icon/traffic_light_green.png` & `solie-8.5.1/solie/static/icon/traffic_light_green.png`

 * *Files identical despite different names*

### Comparing `solie-8.5.0/solie/static/icon/traffic_light_red.png` & `solie-8.5.1/solie/static/icon/traffic_light_red.png`

 * *Files identical despite different names*

### Comparing `solie-8.5.0/solie/static/icon/traffic_light_yellow.png` & `solie-8.5.1/solie/static/icon/traffic_light_yellow.png`

 * *Files identical despite different names*

### Comparing `solie-8.5.0/solie/static/lexend_bold.ttf` & `solie-8.5.1/solie/static/lexend_bold.ttf`

 * *Files identical despite different names*

### Comparing `solie-8.5.0/solie/static/notosans_regular.ttf` & `solie-8.5.1/solie/static/notosans_regular.ttf`

 * *Files identical despite different names*

### Comparing `solie-8.5.0/solie/static/product_icon.ico` & `solie-8.5.1/solie/static/product_icon.ico`

 * *Files identical despite different names*

### Comparing `solie-8.5.0/solie/static/product_icon.png` & `solie-8.5.1/solie/static/product_icon.png`

 * *Files identical despite different names*

### Comparing `solie-8.5.0/solie/static/sample_decision_script.txt` & `solie-8.5.1/solie/static/sample_decision_script.txt`

 * *Files identical despite different names*

### Comparing `solie-8.5.0/solie/static/sample_indicators_script.txt` & `solie-8.5.1/solie/static/sample_indicators_script.txt`

 * *Files identical despite different names*

### Comparing `solie-8.5.0/solie/static/source_code_pro.ttf` & `solie-8.5.1/solie/static/source_code_pro.ttf`

 * *Files identical despite different names*

### Comparing `solie-8.5.0/solie/utility/__init__.py` & `solie-8.5.1/solie/utility/__init__.py`

 * *Files identical despite different names*

### Comparing `solie-8.5.0/solie/utility/analyze_market.py` & `solie-8.5.1/solie/utility/analyze_market.py`

 * *Files identical despite different names*

### Comparing `solie-8.5.0/solie/utility/api_requester.py` & `solie-8.5.1/solie/utility/api_requester.py`

 * *Files identical despite different names*

### Comparing `solie-8.5.0/solie/utility/api_streamer.py` & `solie-8.5.1/solie/utility/api_streamer.py`

 * *Files identical despite different names*

### Comparing `solie-8.5.0/solie/utility/backward_compatibility.py` & `solie-8.5.1/solie/utility/backward_compatibility.py`

 * *Files identical despite different names*

### Comparing `solie-8.5.0/solie/utility/check_internet.py` & `solie-8.5.1/solie/utility/check_internet.py`

 * *Files identical despite different names*

### Comparing `solie-8.5.0/solie/utility/convert.py` & `solie-8.5.1/solie/utility/convert.py`

 * *Files identical despite different names*

### Comparing `solie-8.5.0/solie/utility/download_from_binance.py` & `solie-8.5.1/solie/utility/download_from_binance.py`

 * *Files identical despite different names*

### Comparing `solie-8.5.0/solie/utility/log_handler.py` & `solie-8.5.1/solie/utility/log_handler.py`

 * *Files identical despite different names*

### Comparing `solie-8.5.0/solie/utility/percent_axis_item.py` & `solie-8.5.1/solie/utility/percent_axis_item.py`

 * *Files identical despite different names*

### Comparing `solie-8.5.0/solie/utility/rw_lock.py` & `solie-8.5.1/solie/utility/rw_lock.py`

 * *Files identical despite different names*

### Comparing `solie-8.5.0/solie/utility/standardize.py` & `solie-8.5.1/solie/utility/standardize.py`

 * *Files identical despite different names*

### Comparing `solie-8.5.0/solie/utility/structs.py` & `solie-8.5.1/solie/utility/structs.py`

 * *Files identical despite different names*

### Comparing `solie-8.5.0/solie/utility/syntax_highlighter.py` & `solie-8.5.1/solie/utility/syntax_highlighter.py`

 * *Files identical despite different names*

### Comparing `solie-8.5.0/solie/utility/time_axis_item.py` & `solie-8.5.1/solie/utility/time_axis_item.py`

 * *Files identical despite different names*

### Comparing `solie-8.5.0/solie/utility/timing.py` & `solie-8.5.1/solie/utility/timing.py`

 * *Files identical despite different names*

### Comparing `solie-8.5.0/solie/utility/user_settings.py` & `solie-8.5.1/solie/utility/user_settings.py`

 * *Files identical despite different names*

### Comparing `solie-8.5.0/solie/widget/__init__.py` & `solie-8.5.1/solie/widget/__init__.py`

 * *Files identical despite different names*

### Comparing `solie-8.5.0/solie/widget/ask_popup.py` & `solie-8.5.1/solie/widget/ask_popup.py`

 * *Files identical despite different names*

### Comparing `solie-8.5.0/solie/widget/gauge.py` & `solie-8.5.1/solie/widget/gauge.py`

 * *Files identical despite different names*

### Comparing `solie-8.5.0/solie/widget/log_list.py` & `solie-8.5.1/solie/widget/log_list.py`

 * *Files identical despite different names*

### Comparing `solie-8.5.0/solie/widget/overlay_popup.py` & `solie-8.5.1/solie/widget/overlay_popup.py`

 * *Files identical despite different names*

### Comparing `solie-8.5.0/solie/widget/script_editor.py` & `solie-8.5.1/solie/widget/script_editor.py`

 * *Files identical despite different names*

### Comparing `solie-8.5.0/solie/widget/splash_screen.py` & `solie-8.5.1/solie/widget/splash_screen.py`

 * *Files identical despite different names*

### Comparing `solie-8.5.0/solie/window/compiled.py` & `solie-8.5.1/solie/window/compiled.py`

 * *Files identical despite different names*

### Comparing `solie-8.5.0/solie/window/main.py` & `solie-8.5.1/solie/window/main.py`

 * *Files identical despite different names*

### Comparing `solie-8.5.0/solie/worker/collector.py` & `solie-8.5.1/solie/worker/collector.py`

 * *Files identical despite different names*

### Comparing `solie-8.5.0/solie/worker/manager.py` & `solie-8.5.1/solie/worker/manager.py`

 * *Files identical despite different names*

### Comparing `solie-8.5.0/solie/worker/simulator.py` & `solie-8.5.1/solie/worker/simulator.py`

 * *Files identical despite different names*

### Comparing `solie-8.5.0/solie/worker/strategist.py` & `solie-8.5.1/solie/worker/strategist.py`

 * *Files identical despite different names*

### Comparing `solie-8.5.0/solie/worker/transactor.py` & `solie-8.5.1/solie/worker/transactor.py`

 * *Files 1% similar despite different names*

```diff
@@ -2071,14 +2071,21 @@
             # if there was a `now_buy` or `now_sell` order.
             if current_direction == "none":
                 if "now_buy" in decision[symbol]:
                     current_direction = "long"
                 elif "now_sell" in decision[symbol]:
                     current_direction = "short"
 
+            # Even if there's open position analyzed,
+            # it's possible to assume that a position would have already been closed
+            # if there was a `now_close` order.
+            if current_direction in ("long", "short"):
+                if "now_close" in decision[symbol]:
+                    current_direction = "none"
+
             if "later_up_close" in decision[symbol]:
                 command = decision[symbol]["later_up_close"]
                 if current_direction in ("long", "short"):
                     if current_direction == "long":
                         order_side = "SELL"
                         order_type = "TAKE_PROFIT_MARKET"
                     else:
```

### Comparing `solie-8.5.0/solie/worker/united.py` & `solie-8.5.1/solie/worker/united.py`

 * *Files identical despite different names*

### Comparing `solie-8.5.0/PKG-INFO` & `solie-8.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solie
-Version: 8.5.0
+Version: 8.5.1
 Summary: GUI trading bot designed for targeting the futures markets of Binance
 Home-page: https://github.com/cunarist/solie
 Author: Cunarist
 Requires-Python: >=3.9,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

