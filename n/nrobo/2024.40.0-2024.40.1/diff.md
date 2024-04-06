# Comparing `tmp/nrobo-2024.40.0.tar.gz` & `tmp/nrobo-2024.40.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nrobo-2024.40.0.tar", last modified: Fri Apr  5 07:34:28 2024, max compression
+gzip compressed data, was "nrobo-2024.40.1.tar", last modified: Sat Apr  6 10:58:01 2024, max compression
```

## Comparing `nrobo-2024.40.0.tar` & `nrobo-2024.40.1.tar`

### file list

```diff
@@ -1,124 +1,127 @@
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-05 07:34:28.644186 nrobo-2024.40.0/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     1079 2024-02-02 05:31:36.000000 nrobo-2024.40.0/LICENSE
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)    18169 2024-04-05 07:34:28.643248 nrobo-2024.40.0/PKG-INFO
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)    16531 2024-04-05 07:20:34.000000 nrobo-2024.40.0/README.rst
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-05 07:34:28.595636 nrobo-2024.40.0/nrobo/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     8668 2024-04-05 07:34:02.000000 nrobo-2024.40.0/nrobo/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-05 07:34:28.601045 nrobo-2024.40.0/nrobo/appium/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      716 2024-03-11 11:20:45.000000 nrobo-2024.40.0/nrobo/appium/__init__.py
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)       72 2024-03-11 14:41:50.000000 nrobo-2024.40.0/nrobo/appium/android_capability.yaml
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)       73 2024-03-11 12:05:03.000000 nrobo-2024.40.0/nrobo/appium/ios_capability.yaml
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-05 07:34:28.603938 nrobo-2024.40.0/nrobo/browserConfigs/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      452 2024-02-29 19:11:43.000000 nrobo-2024.40.0/nrobo/browserConfigs/__init__.py
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)       35 2024-02-29 19:12:02.000000 nrobo-2024.40.0/nrobo/browserConfigs/capability.yaml
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)       17 2024-02-19 15:42:30.000000 nrobo-2024.40.0/nrobo/browserConfigs/chrome_config.txt
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)       39 2024-02-29 19:12:02.000000 nrobo-2024.40.0/nrobo/browserConfigs/chrome_prefs.yaml
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)       63 2024-02-29 19:12:02.000000 nrobo-2024.40.0/nrobo/browserConfigs/markers.yaml
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-05 07:34:28.604520 nrobo-2024.40.0/nrobo/browsers/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      459 2024-02-15 02:56:21.000000 nrobo-2024.40.0/nrobo/browsers/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-05 07:34:28.605116 nrobo-2024.40.0/nrobo/browsers/chrome/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     2168 2024-02-15 02:56:21.000000 nrobo-2024.40.0/nrobo/browsers/chrome/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-05 07:34:28.605705 nrobo-2024.40.0/nrobo/browsers/edge/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      468 2024-02-15 02:56:21.000000 nrobo-2024.40.0/nrobo/browsers/edge/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-05 07:34:28.606292 nrobo-2024.40.0/nrobo/browsers/firefox/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      472 2024-02-29 19:11:43.000000 nrobo-2024.40.0/nrobo/browsers/firefox/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-05 07:34:28.606873 nrobo-2024.40.0/nrobo/browsers/safari/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      477 2024-02-29 19:11:43.000000 nrobo-2024.40.0/nrobo/browsers/safari/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-05 07:34:28.610605 nrobo-2024.40.0/nrobo/cli/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     2654 2024-03-23 16:37:25.000000 nrobo-2024.40.0/nrobo/cli/__init__.py
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     2895 2024-03-11 13:01:11.000000 nrobo-2024.40.0/nrobo/cli/cli_constants.py
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)       17 2024-02-15 02:56:21.000000 nrobo-2024.40.0/nrobo/cli/cli_version.yaml
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-05 07:34:28.611228 nrobo-2024.40.0/nrobo/cli/detection/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     2585 2024-02-29 19:12:02.000000 nrobo-2024.40.0/nrobo/cli/detection/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-05 07:34:28.611833 nrobo-2024.40.0/nrobo/cli/formatting/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     1226 2024-02-29 19:11:43.000000 nrobo-2024.40.0/nrobo/cli/formatting/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-05 07:34:28.613376 nrobo-2024.40.0/nrobo/cli/install/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)    12266 2024-03-24 02:00:53.000000 nrobo-2024.40.0/nrobo/cli/install/__init__.py
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      987 2024-04-02 19:56:57.000000 nrobo-2024.40.0/nrobo/cli/install/requirements.txt
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)    15058 2024-03-07 11:01:00.000000 nrobo-2024.40.0/nrobo/cli/launcher.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-05 07:34:28.613983 nrobo-2024.40.0/nrobo/cli/ncodes/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      594 2024-02-29 19:12:02.000000 nrobo-2024.40.0/nrobo/cli/ncodes/__init__.py
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     1806 2024-03-01 03:35:55.000000 nrobo-2024.40.0/nrobo/cli/nglobals.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-05 07:34:28.614588 nrobo-2024.40.0/nrobo/cli/nrobo_args/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)    25971 2024-03-11 13:04:58.000000 nrobo-2024.40.0/nrobo/cli/nrobo_args/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-05 07:34:28.615264 nrobo-2024.40.0/nrobo/cli/tools/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      813 2024-02-29 19:11:43.000000 nrobo-2024.40.0/nrobo/cli/tools/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-05 07:34:28.616132 nrobo-2024.40.0/nrobo/cli/upgrade/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     6308 2024-03-06 04:27:25.000000 nrobo-2024.40.0/nrobo/cli/upgrade/__init__.py
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)    32195 2024-04-05 07:34:02.000000 nrobo-2024.40.0/nrobo/conftest.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-05 07:34:28.616956 nrobo-2024.40.0/nrobo/exceptions/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     1937 2024-02-29 19:12:02.000000 nrobo-2024.40.0/nrobo/exceptions/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-05 07:34:28.620355 nrobo-2024.40.0/nrobo/framework/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)        0 2024-02-05 04:31:26.000000 nrobo-2024.40.0/nrobo/framework/__init__.py
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      540 2024-02-16 15:47:33.000000 nrobo-2024.40.0/nrobo/framework/conftest-host.py
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      779 2024-03-07 13:19:52.000000 nrobo-2024.40.0/nrobo/framework/nrobo-config.yaml
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-05 07:34:28.622321 nrobo-2024.40.0/nrobo/framework/pages/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     1506 2024-02-29 19:12:02.000000 nrobo-2024.40.0/nrobo/framework/pages/PagePyPiHome.py
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      485 2024-02-29 19:12:02.000000 nrobo-2024.40.0/nrobo/framework/pages/PageSearch.py
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     2540 2024-02-29 19:12:02.000000 nrobo-2024.40.0/nrobo/framework/pages/__init__.py
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)       26 2024-03-23 15:17:33.000000 nrobo-2024.40.0/nrobo/framework/requirements.txt
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)        0 2024-03-30 08:56:49.000000 nrobo-2024.40.0/nrobo/framework/secrets.yaml
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-05 07:34:28.622953 nrobo-2024.40.0/nrobo/framework/tests/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)        2 2024-02-07 04:51:13.000000 nrobo-2024.40.0/nrobo/framework/tests/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-05 07:34:28.586385 nrobo-2024.40.0/nrobo/framework/tests/mobile/
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-05 07:34:28.623573 nrobo-2024.40.0/nrobo/framework/tests/mobile/appium/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      383 2024-03-07 08:23:34.000000 nrobo-2024.40.0/nrobo/framework/tests/mobile/appium/test_appium.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-05 07:34:28.624185 nrobo-2024.40.0/nrobo/framework/tests/web/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     1904 2024-02-29 19:12:02.000000 nrobo-2024.40.0/nrobo/framework/tests/web/PyPi_home_page_test.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-05 07:34:28.624787 nrobo-2024.40.0/nrobo/framework/tests/web/examples/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     6470 2024-02-29 19:12:02.000000 nrobo-2024.40.0/nrobo/framework/tests/web/examples/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-05 07:34:28.626014 nrobo-2024.40.0/nrobo/framework/tests/web/gui/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      723 2024-03-03 02:33:11.000000 nrobo-2024.40.0/nrobo/framework/tests/web/gui/PyPi_home_page_test.py
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)        0 2024-02-06 09:49:32.000000 nrobo-2024.40.0/nrobo/framework/tests/web/gui/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-05 07:34:28.626498 nrobo-2024.40.0/nrobo/framework/tests/web/no_gui/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)        0 2024-02-06 09:49:18.000000 nrobo-2024.40.0/nrobo/framework/tests/web/no_gui/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-05 07:34:28.630725 nrobo-2024.40.0/nrobo/framework/tests/web/selenium_wrapper_nrobo_methods/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)        0 2024-02-29 19:12:02.000000 nrobo-2024.40.0/nrobo/framework/tests/web/selenium_wrapper_nrobo_methods/__init__.py
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      820 2024-02-29 19:12:02.000000 nrobo-2024.40.0/nrobo/framework/tests/web/selenium_wrapper_nrobo_methods/test_action_chain_methods.py
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     2427 2024-02-29 19:12:02.000000 nrobo-2024.40.0/nrobo/framework/tests/web/selenium_wrapper_nrobo_methods/test_alert_methods.py
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     7583 2024-02-29 19:12:02.000000 nrobo-2024.40.0/nrobo/framework/tests/web/selenium_wrapper_nrobo_methods/test_element_wrapper_methods.py
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)    19118 2024-02-29 19:12:02.000000 nrobo-2024.40.0/nrobo/framework/tests/web/selenium_wrapper_nrobo_methods/test_nrobo_methods.py
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     1418 2024-02-29 19:12:02.000000 nrobo-2024.40.0/nrobo/framework/tests/web/selenium_wrapper_nrobo_methods/test_nrobo_wait_methods.py
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     6860 2024-02-29 19:12:02.000000 nrobo-2024.40.0/nrobo/framework/tests/web/selenium_wrapper_nrobo_methods/test_select.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-05 07:34:28.631368 nrobo-2024.40.0/nrobo/selenese/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)    46611 2024-04-01 12:06:54.000000 nrobo-2024.40.0/nrobo/selenese/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-05 07:34:28.632102 nrobo-2024.40.0/nrobo/util/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      431 2024-02-15 02:56:21.000000 nrobo-2024.40.0/nrobo/util/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-05 07:34:28.632700 nrobo-2024.40.0/nrobo/util/commands/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      431 2024-02-15 02:56:21.000000 nrobo-2024.40.0/nrobo/util/commands/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-05 07:34:28.633288 nrobo-2024.40.0/nrobo/util/commands/ncommands/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     2105 2024-03-06 18:41:46.000000 nrobo-2024.40.0/nrobo/util/commands/ncommands/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-05 07:34:28.633863 nrobo-2024.40.0/nrobo/util/commands/posix/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      533 2024-02-29 19:11:43.000000 nrobo-2024.40.0/nrobo/util/commands/posix/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-05 07:34:28.634444 nrobo-2024.40.0/nrobo/util/commands/windows/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      535 2024-02-29 19:11:43.000000 nrobo-2024.40.0/nrobo/util/commands/windows/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-05 07:34:28.635034 nrobo-2024.40.0/nrobo/util/common/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     7376 2024-03-18 10:49:47.000000 nrobo-2024.40.0/nrobo/util/common/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-05 07:34:28.635614 nrobo-2024.40.0/nrobo/util/constants/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     1686 2024-02-29 19:11:43.000000 nrobo-2024.40.0/nrobo/util/constants/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-05 07:34:28.636645 nrobo-2024.40.0/nrobo/util/database/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)        0 2024-03-30 08:55:53.000000 nrobo-2024.40.0/nrobo/util/database/__init__.py
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     1992 2024-03-30 08:55:53.000000 nrobo-2024.40.0/nrobo/util/database/connectors.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-05 07:34:28.637218 nrobo-2024.40.0/nrobo/util/filesystem/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     6919 2024-02-29 19:12:02.000000 nrobo-2024.40.0/nrobo/util/filesystem/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-05 07:34:28.637781 nrobo-2024.40.0/nrobo/util/network/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      844 2024-02-29 19:12:02.000000 nrobo-2024.40.0/nrobo/util/network/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-05 07:34:28.638371 nrobo-2024.40.0/nrobo/util/platform/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      742 2024-02-29 19:11:43.000000 nrobo-2024.40.0/nrobo/util/platform/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-05 07:34:28.638953 nrobo-2024.40.0/nrobo/util/process/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     3322 2024-02-29 19:12:02.000000 nrobo-2024.40.0/nrobo/util/process/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-05 07:34:28.639524 nrobo-2024.40.0/nrobo/util/python/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     2101 2024-02-29 19:11:43.000000 nrobo-2024.40.0/nrobo/util/python/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-05 07:34:28.640090 nrobo-2024.40.0/nrobo/util/regex/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      976 2024-02-29 19:11:43.000000 nrobo-2024.40.0/nrobo/util/regex/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-05 07:34:28.640707 nrobo-2024.40.0/nrobo/util/version/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     8316 2024-02-29 19:12:02.000000 nrobo-2024.40.0/nrobo/util/version/__init__.py
-drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-05 07:34:28.641914 nrobo-2024.40.0/nrobo.egg-info/
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)    18169 2024-04-05 07:34:28.000000 nrobo-2024.40.0/nrobo.egg-info/PKG-INFO
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     2776 2024-04-05 07:34:28.000000 nrobo-2024.40.0/nrobo.egg-info/SOURCES.txt
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)        1 2024-04-05 07:34:28.000000 nrobo-2024.40.0/nrobo.egg-info/dependency_links.txt
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)       41 2024-04-05 07:34:28.000000 nrobo-2024.40.0/nrobo.egg-info/entry_points.txt
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)       43 2024-04-05 07:34:28.000000 nrobo-2024.40.0/nrobo.egg-info/requires.txt
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)        6 2024-04-05 07:34:28.000000 nrobo-2024.40.0/nrobo.egg-info/top_level.txt
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     2545 2024-04-05 07:34:02.000000 nrobo-2024.40.0/pyproject.toml
--rw-r--r--   0 einsteinpanchdev   (501) staff       (20)       38 2024-04-05 07:34:28.644357 nrobo-2024.40.0/setup.cfg
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-06 10:58:01.397645 nrobo-2024.40.1/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     1079 2024-02-02 05:31:36.000000 nrobo-2024.40.1/LICENSE
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)    18169 2024-04-06 10:58:01.396987 nrobo-2024.40.1/PKG-INFO
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)    16531 2024-04-06 10:57:44.000000 nrobo-2024.40.1/README.rst
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-06 10:58:01.366448 nrobo-2024.40.1/nrobo/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     8702 2024-04-06 10:57:34.000000 nrobo-2024.40.1/nrobo/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-06 10:58:01.369850 nrobo-2024.40.1/nrobo/appium/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      716 2024-03-11 11:20:45.000000 nrobo-2024.40.1/nrobo/appium/__init__.py
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)       72 2024-03-11 14:41:50.000000 nrobo-2024.40.1/nrobo/appium/android_capability.yaml
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)       73 2024-03-11 12:05:03.000000 nrobo-2024.40.1/nrobo/appium/ios_capability.yaml
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-06 10:58:01.371721 nrobo-2024.40.1/nrobo/browserConfigs/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      452 2024-02-29 19:11:43.000000 nrobo-2024.40.1/nrobo/browserConfigs/__init__.py
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)       35 2024-02-29 19:12:02.000000 nrobo-2024.40.1/nrobo/browserConfigs/capability.yaml
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)       17 2024-02-19 15:42:30.000000 nrobo-2024.40.1/nrobo/browserConfigs/chrome_config.txt
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)       39 2024-02-29 19:12:02.000000 nrobo-2024.40.1/nrobo/browserConfigs/chrome_prefs.yaml
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)       63 2024-02-29 19:12:02.000000 nrobo-2024.40.1/nrobo/browserConfigs/markers.yaml
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-06 10:58:01.372090 nrobo-2024.40.1/nrobo/browsers/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      459 2024-02-15 02:56:21.000000 nrobo-2024.40.1/nrobo/browsers/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-06 10:58:01.372458 nrobo-2024.40.1/nrobo/browsers/chrome/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     2168 2024-02-15 02:56:21.000000 nrobo-2024.40.1/nrobo/browsers/chrome/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-06 10:58:01.372825 nrobo-2024.40.1/nrobo/browsers/edge/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      468 2024-02-15 02:56:21.000000 nrobo-2024.40.1/nrobo/browsers/edge/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-06 10:58:01.373196 nrobo-2024.40.1/nrobo/browsers/firefox/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      472 2024-02-29 19:11:43.000000 nrobo-2024.40.1/nrobo/browsers/firefox/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-06 10:58:01.373566 nrobo-2024.40.1/nrobo/browsers/safari/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      477 2024-02-29 19:11:43.000000 nrobo-2024.40.1/nrobo/browsers/safari/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-06 10:58:01.375547 nrobo-2024.40.1/nrobo/cli/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     2654 2024-03-23 16:37:25.000000 nrobo-2024.40.1/nrobo/cli/__init__.py
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     2895 2024-03-11 13:01:11.000000 nrobo-2024.40.1/nrobo/cli/cli_constants.py
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)       17 2024-02-15 02:56:21.000000 nrobo-2024.40.1/nrobo/cli/cli_version.yaml
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-06 10:58:01.375919 nrobo-2024.40.1/nrobo/cli/detection/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     2585 2024-02-29 19:12:02.000000 nrobo-2024.40.1/nrobo/cli/detection/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-06 10:58:01.376381 nrobo-2024.40.1/nrobo/cli/formatting/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     1226 2024-02-29 19:11:43.000000 nrobo-2024.40.1/nrobo/cli/formatting/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-06 10:58:01.377288 nrobo-2024.40.1/nrobo/cli/install/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)    12266 2024-03-24 02:00:53.000000 nrobo-2024.40.1/nrobo/cli/install/__init__.py
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      987 2024-04-02 19:56:57.000000 nrobo-2024.40.1/nrobo/cli/install/requirements.txt
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)    15058 2024-03-07 11:01:00.000000 nrobo-2024.40.1/nrobo/cli/launcher.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-06 10:58:01.377678 nrobo-2024.40.1/nrobo/cli/ncodes/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      594 2024-02-29 19:12:02.000000 nrobo-2024.40.1/nrobo/cli/ncodes/__init__.py
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     1806 2024-03-01 03:35:55.000000 nrobo-2024.40.1/nrobo/cli/nglobals.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-06 10:58:01.378068 nrobo-2024.40.1/nrobo/cli/nrobo_args/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)    25971 2024-03-11 13:04:58.000000 nrobo-2024.40.1/nrobo/cli/nrobo_args/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-06 10:58:01.378527 nrobo-2024.40.1/nrobo/cli/tools/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      813 2024-02-29 19:11:43.000000 nrobo-2024.40.1/nrobo/cli/tools/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-06 10:58:01.378911 nrobo-2024.40.1/nrobo/cli/upgrade/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     6308 2024-03-06 04:27:25.000000 nrobo-2024.40.1/nrobo/cli/upgrade/__init__.py
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)    32195 2024-04-06 10:57:34.000000 nrobo-2024.40.1/nrobo/conftest.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-06 10:58:01.379289 nrobo-2024.40.1/nrobo/exceptions/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     1937 2024-02-29 19:12:02.000000 nrobo-2024.40.1/nrobo/exceptions/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-06 10:58:01.381089 nrobo-2024.40.1/nrobo/framework/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)        0 2024-02-05 04:31:26.000000 nrobo-2024.40.1/nrobo/framework/__init__.py
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      540 2024-02-16 15:47:33.000000 nrobo-2024.40.1/nrobo/framework/conftest-host.py
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      779 2024-03-07 13:19:52.000000 nrobo-2024.40.1/nrobo/framework/nrobo-config.yaml
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-06 10:58:01.382144 nrobo-2024.40.1/nrobo/framework/pages/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     1506 2024-02-29 19:12:02.000000 nrobo-2024.40.1/nrobo/framework/pages/PagePyPiHome.py
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      485 2024-02-29 19:12:02.000000 nrobo-2024.40.1/nrobo/framework/pages/PageSearch.py
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     2540 2024-02-29 19:12:02.000000 nrobo-2024.40.1/nrobo/framework/pages/__init__.py
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)       26 2024-03-23 15:17:33.000000 nrobo-2024.40.1/nrobo/framework/requirements.txt
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)        0 2024-03-30 08:56:49.000000 nrobo-2024.40.1/nrobo/framework/secrets.yaml
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-06 10:58:01.382804 nrobo-2024.40.1/nrobo/framework/test-data/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-05 19:41:06.000000 nrobo-2024.40.1/nrobo/framework/test-data/__init__.py
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     6402 2024-02-13 06:51:47.000000 nrobo-2024.40.1/nrobo/framework/test-data/nRoBo-Logo.png
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-06 10:58:01.383198 nrobo-2024.40.1/nrobo/framework/tests/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)        2 2024-02-07 04:51:13.000000 nrobo-2024.40.1/nrobo/framework/tests/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-06 10:58:01.359964 nrobo-2024.40.1/nrobo/framework/tests/mobile/
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-06 10:58:01.383591 nrobo-2024.40.1/nrobo/framework/tests/mobile/appium/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      383 2024-03-07 08:23:34.000000 nrobo-2024.40.1/nrobo/framework/tests/mobile/appium/test_appium.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-06 10:58:01.384234 nrobo-2024.40.1/nrobo/framework/tests/web/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     1904 2024-02-29 19:12:02.000000 nrobo-2024.40.1/nrobo/framework/tests/web/PyPi_home_page_test.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-06 10:58:01.384732 nrobo-2024.40.1/nrobo/framework/tests/web/examples/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     6470 2024-02-29 19:12:02.000000 nrobo-2024.40.1/nrobo/framework/tests/web/examples/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-06 10:58:01.385835 nrobo-2024.40.1/nrobo/framework/tests/web/gui/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      723 2024-03-03 02:33:11.000000 nrobo-2024.40.1/nrobo/framework/tests/web/gui/PyPi_home_page_test.py
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)        0 2024-02-06 09:49:32.000000 nrobo-2024.40.1/nrobo/framework/tests/web/gui/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-06 10:58:01.386150 nrobo-2024.40.1/nrobo/framework/tests/web/no_gui/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)        0 2024-02-06 09:49:18.000000 nrobo-2024.40.1/nrobo/framework/tests/web/no_gui/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-06 10:58:01.389069 nrobo-2024.40.1/nrobo/framework/tests/web/selenium_wrapper_nrobo_methods/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)        0 2024-02-29 19:12:02.000000 nrobo-2024.40.1/nrobo/framework/tests/web/selenium_wrapper_nrobo_methods/__init__.py
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      820 2024-02-29 19:12:02.000000 nrobo-2024.40.1/nrobo/framework/tests/web/selenium_wrapper_nrobo_methods/test_action_chain_methods.py
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     2427 2024-02-29 19:12:02.000000 nrobo-2024.40.1/nrobo/framework/tests/web/selenium_wrapper_nrobo_methods/test_alert_methods.py
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     8284 2024-04-05 20:33:08.000000 nrobo-2024.40.1/nrobo/framework/tests/web/selenium_wrapper_nrobo_methods/test_element_wrapper_methods.py
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)    19118 2024-02-29 19:12:02.000000 nrobo-2024.40.1/nrobo/framework/tests/web/selenium_wrapper_nrobo_methods/test_nrobo_methods.py
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     1418 2024-02-29 19:12:02.000000 nrobo-2024.40.1/nrobo/framework/tests/web/selenium_wrapper_nrobo_methods/test_nrobo_wait_methods.py
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     6860 2024-02-29 19:12:02.000000 nrobo-2024.40.1/nrobo/framework/tests/web/selenium_wrapper_nrobo_methods/test_select.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-06 10:58:01.389458 nrobo-2024.40.1/nrobo/selenese/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)    49008 2024-04-06 08:38:03.000000 nrobo-2024.40.1/nrobo/selenese/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-06 10:58:01.389927 nrobo-2024.40.1/nrobo/util/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      431 2024-02-15 02:56:21.000000 nrobo-2024.40.1/nrobo/util/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-06 10:58:01.390316 nrobo-2024.40.1/nrobo/util/commands/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      431 2024-02-15 02:56:21.000000 nrobo-2024.40.1/nrobo/util/commands/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-06 10:58:01.390704 nrobo-2024.40.1/nrobo/util/commands/ncommands/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     2105 2024-03-06 18:41:46.000000 nrobo-2024.40.1/nrobo/util/commands/ncommands/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-06 10:58:01.391089 nrobo-2024.40.1/nrobo/util/commands/posix/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      533 2024-02-29 19:11:43.000000 nrobo-2024.40.1/nrobo/util/commands/posix/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-06 10:58:01.391472 nrobo-2024.40.1/nrobo/util/commands/windows/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      535 2024-02-29 19:11:43.000000 nrobo-2024.40.1/nrobo/util/commands/windows/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-06 10:58:01.391846 nrobo-2024.40.1/nrobo/util/common/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     7376 2024-03-18 10:49:47.000000 nrobo-2024.40.1/nrobo/util/common/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-06 10:58:01.392227 nrobo-2024.40.1/nrobo/util/constants/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     1686 2024-02-29 19:11:43.000000 nrobo-2024.40.1/nrobo/util/constants/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-06 10:58:01.392917 nrobo-2024.40.1/nrobo/util/database/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)        0 2024-03-30 08:55:53.000000 nrobo-2024.40.1/nrobo/util/database/__init__.py
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     1992 2024-03-30 08:55:53.000000 nrobo-2024.40.1/nrobo/util/database/connectors.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-06 10:58:01.393303 nrobo-2024.40.1/nrobo/util/filesystem/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     6919 2024-02-29 19:12:02.000000 nrobo-2024.40.1/nrobo/util/filesystem/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-06 10:58:01.393682 nrobo-2024.40.1/nrobo/util/network/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      844 2024-02-29 19:12:02.000000 nrobo-2024.40.1/nrobo/util/network/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-06 10:58:01.394058 nrobo-2024.40.1/nrobo/util/platform/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      742 2024-02-29 19:11:43.000000 nrobo-2024.40.1/nrobo/util/platform/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-06 10:58:01.394450 nrobo-2024.40.1/nrobo/util/process/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     3322 2024-02-29 19:12:02.000000 nrobo-2024.40.1/nrobo/util/process/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-06 10:58:01.394847 nrobo-2024.40.1/nrobo/util/python/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     2101 2024-02-29 19:11:43.000000 nrobo-2024.40.1/nrobo/util/python/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-06 10:58:01.395223 nrobo-2024.40.1/nrobo/util/regex/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)      976 2024-02-29 19:11:43.000000 nrobo-2024.40.1/nrobo/util/regex/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-06 10:58:01.395600 nrobo-2024.40.1/nrobo/util/version/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     8316 2024-02-29 19:12:02.000000 nrobo-2024.40.1/nrobo/util/version/__init__.py
+drwxr-xr-x   0 einsteinpanchdev   (501) staff       (20)        0 2024-04-06 10:58:01.396099 nrobo-2024.40.1/nrobo.egg-info/
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)    18169 2024-04-06 10:58:01.000000 nrobo-2024.40.1/nrobo.egg-info/PKG-INFO
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     2855 2024-04-06 10:58:01.000000 nrobo-2024.40.1/nrobo.egg-info/SOURCES.txt
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)        1 2024-04-06 10:58:01.000000 nrobo-2024.40.1/nrobo.egg-info/dependency_links.txt
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)       41 2024-04-06 10:58:01.000000 nrobo-2024.40.1/nrobo.egg-info/entry_points.txt
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)       43 2024-04-06 10:58:01.000000 nrobo-2024.40.1/nrobo.egg-info/requires.txt
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)        6 2024-04-06 10:58:01.000000 nrobo-2024.40.1/nrobo.egg-info/top_level.txt
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)     2545 2024-04-06 10:57:34.000000 nrobo-2024.40.1/pyproject.toml
+-rw-r--r--   0 einsteinpanchdev   (501) staff       (20)       38 2024-04-06 10:58:01.397760 nrobo-2024.40.1/setup.cfg
```

### Comparing `nrobo-2024.40.0/LICENSE` & `nrobo-2024.40.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nrobo-2024.40.0/PKG-INFO` & `nrobo-2024.40.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nrobo
-Version: 2024.40.0
+Version: 2024.40.1
 Summary: Powerful! Yet, Easy to USE! Automated Testing Framework
 Author-email: Panchdev Singh Chauhan <erpanchdev@gmail.com>
 Maintainer-email: Panchdev Singh Chauhan <erpanchdev@gmail.com>
 Project-URL: Homepage, https://pypi.org/project/nrobo/
 Project-URL: GitHub Repo, https://github.com/pancht/ngrobo
 Project-URL: Bug Tracker, https://github.com/pancht/ngrobo/issues
 Project-URL: changelog, https://github.com/pancht/ngrobo/blob/master/CHANGELOG.md
@@ -384,107 +384,107 @@
    :align: center
    :header-rows: 1
 
    * - Country
      - Percent
      - Download Count
    * - US
-     - 38.96%
-     - 23,088
+     - 38.91%
+     - 23,363
    * - CN
-     - 13.06%
-     - 7,741
+     - 12.98%
+     - 7,792
    * - DE
-     - 6.48%
-     - 3,838
+     - 6.76%
+     - 4,057
    * - SG
-     - 5.58%
-     - 3,308
+     - 5.55%
+     - 3,332
    * - RU
-     - 5.17%
-     - 3,064
+     - 5.12%
+     - 3,075
    * - HK
-     - 4.13%
-     - 2,449
+     - 4.10%
+     - 2,462
    * - JP
-     - 3.10%
-     - 1,834
+     - 3.07%
+     - 1,842
    * - FR
-     - 2.83%
-     - 1,677
+     - 2.81%
+     - 1,685
    * - KR
-     - 2.72%
+     - 2.68%
      - 1,611
    * - CA
-     - 2.67%
-     - 1,583
+     - 2.65%
+     - 1,591
    * - NO
-     - 2.00%
-     - 1,183
+     - 2.18%
+     - 1,307
    * - GB
-     - 1.84%
-     - 1,091
+     - 1.83%
+     - 1,096
    * - AU
      - 1.75%
-     - 1,039
+     - 1,048
    * - IN
      - 1.52%
-     - 901
+     - 911
    * - SE
-     - 1.21%
-     - 716
+     - 1.20%
+     - 718
    * - TH
-     - 0.79%
-     - 466
+     - 0.78%
+     - 469
    * - HR
      - 0.78%
-     - 462
-   * - DK
-     - 0.67%
-     - 395
+     - 466
    * - IE
      - 0.66%
-     - 389
+     - 395
+   * - DK
+     - 0.66%
+     - 395
    * - TW
-     - 0.61%
+     - 0.60%
      - 363
    * - IL
-     - 0.58%
+     - 0.57%
      - 341
    * - NL
-     - 0.50%
+     - 0.49%
      - 297
    * - ES
      - 0.44%
      - 262
    * - CH
      - 0.42%
-     - 251
+     - 254
    * - AE
-     - 0.35%
+     - 0.34%
      - 207
    * - CZ
      - 0.24%
      - 144
    * - FI
      - 0.16%
-     - 93
+     - 97
    * - ZA
      - 0.15%
      - 89
    * - BR
      - 0.13%
      - 77
    * - PL
      - 0.10%
      - 61
-   * - TR
+   * - CW
      - 0.07%
      - 44
-   * - CW
+   * - TR
      - 0.07%
      - 44
    * - OM
      - 0.07%
      - 42
    * - IS
      - 0.07%
@@ -501,28 +501,28 @@
    * - CY
      - 0.01%
      - 6
    * - DZ
      - 0.01%
      - 4
    * - EE
-     - 0.01%
+     - 0.00%
      - 3
    * - AR
-     - 0.01%
+     - 0.00%
      - 3
    * - SK
      - 0.00%
      - 2
-   * - RS
+   * - MX
      - 0.00%
      - 1
    * - PT
      - 0.00%
      - 1
-   * - MX
+   * - RS
      - 0.00%
      - 1
    * - **Total**
      - **100.00%**
-     - **59,255**
+     - **60,042**
```

### Comparing `nrobo-2024.40.0/README.rst` & `nrobo-2024.40.1/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -348,107 +348,107 @@
    :align: center
    :header-rows: 1
 
    * - Country
      - Percent
      - Download Count
    * - US
-     - 38.96%
-     - 23,088
+     - 38.91%
+     - 23,363
    * - CN
-     - 13.06%
-     - 7,741
+     - 12.98%
+     - 7,792
    * - DE
-     - 6.48%
-     - 3,838
+     - 6.76%
+     - 4,057
    * - SG
-     - 5.58%
-     - 3,308
+     - 5.55%
+     - 3,332
    * - RU
-     - 5.17%
-     - 3,064
+     - 5.12%
+     - 3,075
    * - HK
-     - 4.13%
-     - 2,449
+     - 4.10%
+     - 2,462
    * - JP
-     - 3.10%
-     - 1,834
+     - 3.07%
+     - 1,842
    * - FR
-     - 2.83%
-     - 1,677
+     - 2.81%
+     - 1,685
    * - KR
-     - 2.72%
+     - 2.68%
      - 1,611
    * - CA
-     - 2.67%
-     - 1,583
+     - 2.65%
+     - 1,591
    * - NO
-     - 2.00%
-     - 1,183
+     - 2.18%
+     - 1,307
    * - GB
-     - 1.84%
-     - 1,091
+     - 1.83%
+     - 1,096
    * - AU
      - 1.75%
-     - 1,039
+     - 1,048
    * - IN
      - 1.52%
-     - 901
+     - 911
    * - SE
-     - 1.21%
-     - 716
+     - 1.20%
+     - 718
    * - TH
-     - 0.79%
-     - 466
+     - 0.78%
+     - 469
    * - HR
      - 0.78%
-     - 462
-   * - DK
-     - 0.67%
-     - 395
+     - 466
    * - IE
      - 0.66%
-     - 389
+     - 395
+   * - DK
+     - 0.66%
+     - 395
    * - TW
-     - 0.61%
+     - 0.60%
      - 363
    * - IL
-     - 0.58%
+     - 0.57%
      - 341
    * - NL
-     - 0.50%
+     - 0.49%
      - 297
    * - ES
      - 0.44%
      - 262
    * - CH
      - 0.42%
-     - 251
+     - 254
    * - AE
-     - 0.35%
+     - 0.34%
      - 207
    * - CZ
      - 0.24%
      - 144
    * - FI
      - 0.16%
-     - 93
+     - 97
    * - ZA
      - 0.15%
      - 89
    * - BR
      - 0.13%
      - 77
    * - PL
      - 0.10%
      - 61
-   * - TR
+   * - CW
      - 0.07%
      - 44
-   * - CW
+   * - TR
      - 0.07%
      - 44
    * - OM
      - 0.07%
      - 42
    * - IS
      - 0.07%
@@ -465,28 +465,28 @@
    * - CY
      - 0.01%
      - 6
    * - DZ
      - 0.01%
      - 4
    * - EE
-     - 0.01%
+     - 0.00%
      - 3
    * - AR
-     - 0.01%
+     - 0.00%
      - 3
    * - SK
      - 0.00%
      - 2
-   * - RS
+   * - MX
      - 0.00%
      - 1
    * - PT
      - 0.00%
      - 1
-   * - MX
+   * - RS
      - 0.00%
      - 1
    * - **Total**
      - **100.00%**
-     - **59,255**
+     - **60,042**
```

### Comparing `nrobo-2024.40.0/nrobo/__init__.py` & `nrobo-2024.40.1/nrobo/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 nrobo module loads nRoBo globals.
 
 
 @author: Panchdev Singh Chauhan
 @email: erpanchdev@gmail.com
 """
 
-__version__ = '2024.40.0'
+__version__ = '2024.40.1'
 
 # install rich library
 import os
 from pathlib import Path
 
 
 class DB_CONNECTOR_TYPE:
@@ -143,14 +143,15 @@
     NGLOBALS_PY_FILE = CLI / Path("nglobals.py")
 
     EXCEPTIONS = Path("exceptions")
 
     # framework packages
     FRAMEWORK = Path("framework")
     PAGES = Path("pages")
+    TEST_DATA = Path('test-data')
     FRAMEWORK_PAGES = FRAMEWORK / PAGES
     FRAMEWORK_PAGE_PYPI_HOME_PY_FILE = FRAMEWORK_PAGES / Path("PagePyPiHome.py")
     TESTS = Path("tests")
     MOBILE = Path("mobile")
     WEB = Path("web")
     FRAMEWORK_TESTS = FRAMEWORK / TESTS
     GUI = FRAMEWORK_TESTS / WEB / Path("gui")
```

### Comparing `nrobo-2024.40.0/nrobo/appium/__init__.py` & `nrobo-2024.40.1/nrobo/appium/__init__.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.40.0/nrobo/browsers/chrome/__init__.py` & `nrobo-2024.40.1/nrobo/browsers/chrome/__init__.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.40.0/nrobo/cli/__init__.py` & `nrobo-2024.40.1/nrobo/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.40.0/nrobo/cli/cli_constants.py` & `nrobo-2024.40.1/nrobo/cli/cli_constants.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.40.0/nrobo/cli/detection/__init__.py` & `nrobo-2024.40.1/nrobo/cli/detection/__init__.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.40.0/nrobo/cli/formatting/__init__.py` & `nrobo-2024.40.1/nrobo/cli/formatting/__init__.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.40.0/nrobo/cli/install/__init__.py` & `nrobo-2024.40.1/nrobo/cli/install/__init__.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.40.0/nrobo/cli/install/requirements.txt` & `nrobo-2024.40.1/nrobo/cli/install/requirements.txt`

 * *Files identical despite different names*

### Comparing `nrobo-2024.40.0/nrobo/cli/launcher.py` & `nrobo-2024.40.1/nrobo/cli/launcher.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.40.0/nrobo/cli/ncodes/__init__.py` & `nrobo-2024.40.1/nrobo/cli/ncodes/__init__.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.40.0/nrobo/cli/nglobals.py` & `nrobo-2024.40.1/nrobo/cli/nglobals.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.40.0/nrobo/cli/nrobo_args/__init__.py` & `nrobo-2024.40.1/nrobo/cli/nrobo_args/__init__.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.40.0/nrobo/cli/tools/__init__.py` & `nrobo-2024.40.1/nrobo/cli/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.40.0/nrobo/cli/upgrade/__init__.py` & `nrobo-2024.40.1/nrobo/cli/upgrade/__init__.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.40.0/nrobo/conftest.py` & `nrobo-2024.40.1/nrobo/conftest.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.40.0/nrobo/exceptions/__init__.py` & `nrobo-2024.40.1/nrobo/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.40.0/nrobo/framework/conftest-host.py` & `nrobo-2024.40.1/nrobo/framework/conftest-host.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.40.0/nrobo/framework/nrobo-config.yaml` & `nrobo-2024.40.1/nrobo/framework/nrobo-config.yaml`

 * *Files identical despite different names*

### Comparing `nrobo-2024.40.0/nrobo/framework/pages/PagePyPiHome.py` & `nrobo-2024.40.1/nrobo/framework/pages/PagePyPiHome.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.40.0/nrobo/framework/pages/__init__.py` & `nrobo-2024.40.1/nrobo/framework/pages/__init__.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.40.0/nrobo/framework/tests/web/PyPi_home_page_test.py` & `nrobo-2024.40.1/nrobo/framework/tests/web/PyPi_home_page_test.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.40.0/nrobo/framework/tests/web/examples/__init__.py` & `nrobo-2024.40.1/nrobo/framework/tests/web/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.40.0/nrobo/framework/tests/web/gui/PyPi_home_page_test.py` & `nrobo-2024.40.1/nrobo/framework/tests/web/gui/PyPi_home_page_test.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.40.0/nrobo/framework/tests/web/selenium_wrapper_nrobo_methods/test_action_chain_methods.py` & `nrobo-2024.40.1/nrobo/framework/tests/web/selenium_wrapper_nrobo_methods/test_action_chain_methods.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.40.0/nrobo/framework/tests/web/selenium_wrapper_nrobo_methods/test_alert_methods.py` & `nrobo-2024.40.1/nrobo/framework/tests/web/selenium_wrapper_nrobo_methods/test_alert_methods.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.40.0/nrobo/framework/tests/web/selenium_wrapper_nrobo_methods/test_element_wrapper_methods.py` & `nrobo-2024.40.1/nrobo/framework/tests/web/selenium_wrapper_nrobo_methods/test_element_wrapper_methods.py`

 * *Files 4% similar despite different names*

```diff
@@ -200,10 +200,32 @@
 
         page = Page(driver, logger)
         page.get("https://the-internet.herokuapp.com/")
 
         lnkLogin = (By.CSS_SELECTOR, "[href='/login']")
         page.screenshot('element_screenshot_as_file.png', *lnkLogin)
 
+    @pytest.mark.skip
+    def test_uploads(self, driver, logger):
+        """Example of file upload"""
+
+        page = Page(driver, logger)
+        page.maximize_window()
+        page.get("https://the-internet.herokuapp.com/upload")
+
+        from pathlib import Path
+        from nrobo import NROBO_PATHS
+        upload_file = NROBO_PATHS.TEST_DATA / 'nRoBo-Logo.png'
+
+        file_input = (By.CSS_SELECTOR, "input[type='file']")
+        btn_upload = (By.ID, "file-submit")
+
+        page.file_upload(*file_input, upload_file, *btn_upload)
+
+        file_name_element = page.find_element(By.ID, "uploaded-files")
+        file_name = file_name_element.text
+
+        assert file_name == "nRoBo-Logo.png"
+
```

### Comparing `nrobo-2024.40.0/nrobo/framework/tests/web/selenium_wrapper_nrobo_methods/test_nrobo_methods.py` & `nrobo-2024.40.1/nrobo/framework/tests/web/selenium_wrapper_nrobo_methods/test_nrobo_methods.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.40.0/nrobo/framework/tests/web/selenium_wrapper_nrobo_methods/test_nrobo_wait_methods.py` & `nrobo-2024.40.1/nrobo/framework/tests/web/selenium_wrapper_nrobo_methods/test_nrobo_wait_methods.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.40.0/nrobo/framework/tests/web/selenium_wrapper_nrobo_methods/test_select.py` & `nrobo-2024.40.1/nrobo/framework/tests/web/selenium_wrapper_nrobo_methods/test_select.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.40.0/nrobo/selenese/__init__.py` & `nrobo-2024.40.1/nrobo/selenese/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -141,20 +141,43 @@
         :Usage:
             ::
 
                 name = <obj>.name"""
 
         return self.driver.name
 
+    def _wait_page_load(self):
+        def wait_for_page_to_be_loaded(self):
+            """Waits for give timeout time for page to completely load.
+            timeout time is configurable in nrobo-config.yaml"""
+
+            if int(os.environ[EnvKeys.APPIUM]):
+                return
+
+            # nprint("Wait for page load...", style=STYLE.HLOrange)
+            try:
+                # Webdriver implementation of page load timeout
+                self.set_page_load_timeout(self.nconfig[WAITS.TIMEOUT])
+
+                # Custom page load timeout
+                WebDriverWait(self.driver, self.nconfig[WAITS.TIMEOUT]).until(
+                    lambda driver: driver.execute_script('return document.readyState') == 'complete')
+            except TimeoutException as te:
+                nprint(f"Exception: {te}", STYLE.HLRed)
+            except AttributeError as ae:
+                nprint(f"Exception: {ae}", STYLE.HLRed)
+            # nprint("End of Wait for page load...", style=STYLE.PURPLE4)
+
     def get(self, url: str):
         """selenium webdriver wrapper method: get"""
 
         url = str(url).replace('\\', "\\\\")  # perform replacements
         nprint(f"Go to url <{url}>", logger=self.logger)
         self.driver.get(url)
+        self._wait_page_load()
 
         self.update_windows(self.window_handles)
 
     def execute(self, driver_command: str, params: dict = None) -> dict:
         """selenium webdriver wrapper method: execute"""
 
         nprint(f"Executing script...")
@@ -1121,27 +1144,27 @@
     def wait_for_page_to_be_loaded(self):
         """Waits for give timeout time for page to completely load.
         timeout time is configurable in nrobo-config.yaml"""
 
         if int(os.environ[EnvKeys.APPIUM]):
             return
 
-        nprint("Wait for page load...", style=STYLE.HLOrange)
+        # nprint("Wait for page load...", style=STYLE.HLOrange)
         try:
             # Webdriver implementation of page load timeout
             self.set_page_load_timeout(self.nconfig[WAITS.TIMEOUT])
 
             # Custom page load timeout
             WebDriverWait(self.driver, self.nconfig[WAITS.TIMEOUT]).until(
                 lambda driver: driver.execute_script('return document.readyState') == 'complete')
         except TimeoutException as te:
             nprint(f"Exception: {te}", STYLE.HLRed)
         except AttributeError as ae:
             nprint(f"Exception: {ae}", STYLE.HLRed)
-        nprint("End of Wait for page load...", style=STYLE.PURPLE4)
+        # nprint("End of Wait for page load...", style=STYLE.PURPLE4)
 
     @staticmethod
     def wait(time_in_sec=None):
         """
                Pause for <time_in_sec>
 
                :param time_in_sec:
@@ -1365,15 +1388,50 @@
 
     def __init__(self, driver: AnyDriver, logger: logging.Logger, duration: int = 250,
                  devices: list[AnyDevice] | None = None):
         """constructor"""
         super().__init__(driver, logger, duration=duration, devices=devices)
 
 
-class NRobo(AppiumNrobo):
+class NRoBoCustomMethods(AppiumNrobo):
+    """NRobo Advanced and custom methods"""
+
+    def __init__(self, driver: AnyDriver, logger: logging.Logger, duration: int = 250,
+                 devices: list[AnyDevice] | None = None):
+        """constructor"""
+        super().__init__(driver, logger, duration=duration, devices=devices)
+
+    def file_upload(self, file_input_by: By,
+                    file_input_value: str,
+                    file_path: Path | str,
+                    upload_ele_by: By,
+                    upload_ele_value: str):
+        """
+        Upload given file
+
+        :param file_input_by: By type of file input element
+        :param file_input_value: By value of file input element
+        :param file_path: absolute path of file to be uploaded
+        :param upload_ele_by: By type of upload action element
+        :param upload_ele_value: By value of upload action element
+        :return:
+        """
+        if isinstance(file_path, Path):
+            file_path = str(file_path.absolute())
+
+        self.find_element(file_input_by, file_input_value).send_keys(file_path)
+
+        self.click(upload_ele_by, upload_ele_value)
+
+    def type_into(self, by: AnyBy, value: Optional[str] = None, *text) -> None:
+        """Type given text into given element located by (by, value)"""
+        self.send_keys(by, value, text)
+
+
+class NRobo(NRoBoCustomMethods):
     """Base NRobo class for each of the Page Classes in nRoBo framework.
 
        Each Page class must inherit NRobo class in order to leverage the nRoBo framework.
 
        This class takes care of handling browsers, user sessions, actions, logs and many more
 
        pertaining to browser interactions.
```

### Comparing `nrobo-2024.40.0/nrobo/util/commands/ncommands/__init__.py` & `nrobo-2024.40.1/nrobo/util/commands/ncommands/__init__.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.40.0/nrobo/util/commands/posix/__init__.py` & `nrobo-2024.40.1/nrobo/util/commands/posix/__init__.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.40.0/nrobo/util/commands/windows/__init__.py` & `nrobo-2024.40.1/nrobo/util/commands/windows/__init__.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.40.0/nrobo/util/common/__init__.py` & `nrobo-2024.40.1/nrobo/util/common/__init__.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.40.0/nrobo/util/constants/__init__.py` & `nrobo-2024.40.1/nrobo/util/constants/__init__.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.40.0/nrobo/util/database/connectors.py` & `nrobo-2024.40.1/nrobo/util/database/connectors.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.40.0/nrobo/util/filesystem/__init__.py` & `nrobo-2024.40.1/nrobo/util/filesystem/__init__.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.40.0/nrobo/util/network/__init__.py` & `nrobo-2024.40.1/nrobo/util/network/__init__.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.40.0/nrobo/util/platform/__init__.py` & `nrobo-2024.40.1/nrobo/util/platform/__init__.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.40.0/nrobo/util/process/__init__.py` & `nrobo-2024.40.1/nrobo/util/process/__init__.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.40.0/nrobo/util/python/__init__.py` & `nrobo-2024.40.1/nrobo/util/python/__init__.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.40.0/nrobo/util/regex/__init__.py` & `nrobo-2024.40.1/nrobo/util/regex/__init__.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.40.0/nrobo/util/version/__init__.py` & `nrobo-2024.40.1/nrobo/util/version/__init__.py`

 * *Files identical despite different names*

### Comparing `nrobo-2024.40.0/nrobo.egg-info/PKG-INFO` & `nrobo-2024.40.1/nrobo.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nrobo
-Version: 2024.40.0
+Version: 2024.40.1
 Summary: Powerful! Yet, Easy to USE! Automated Testing Framework
 Author-email: Panchdev Singh Chauhan <erpanchdev@gmail.com>
 Maintainer-email: Panchdev Singh Chauhan <erpanchdev@gmail.com>
 Project-URL: Homepage, https://pypi.org/project/nrobo/
 Project-URL: GitHub Repo, https://github.com/pancht/ngrobo
 Project-URL: Bug Tracker, https://github.com/pancht/ngrobo/issues
 Project-URL: changelog, https://github.com/pancht/ngrobo/blob/master/CHANGELOG.md
@@ -384,107 +384,107 @@
    :align: center
    :header-rows: 1
 
    * - Country
      - Percent
      - Download Count
    * - US
-     - 38.96%
-     - 23,088
+     - 38.91%
+     - 23,363
    * - CN
-     - 13.06%
-     - 7,741
+     - 12.98%
+     - 7,792
    * - DE
-     - 6.48%
-     - 3,838
+     - 6.76%
+     - 4,057
    * - SG
-     - 5.58%
-     - 3,308
+     - 5.55%
+     - 3,332
    * - RU
-     - 5.17%
-     - 3,064
+     - 5.12%
+     - 3,075
    * - HK
-     - 4.13%
-     - 2,449
+     - 4.10%
+     - 2,462
    * - JP
-     - 3.10%
-     - 1,834
+     - 3.07%
+     - 1,842
    * - FR
-     - 2.83%
-     - 1,677
+     - 2.81%
+     - 1,685
    * - KR
-     - 2.72%
+     - 2.68%
      - 1,611
    * - CA
-     - 2.67%
-     - 1,583
+     - 2.65%
+     - 1,591
    * - NO
-     - 2.00%
-     - 1,183
+     - 2.18%
+     - 1,307
    * - GB
-     - 1.84%
-     - 1,091
+     - 1.83%
+     - 1,096
    * - AU
      - 1.75%
-     - 1,039
+     - 1,048
    * - IN
      - 1.52%
-     - 901
+     - 911
    * - SE
-     - 1.21%
-     - 716
+     - 1.20%
+     - 718
    * - TH
-     - 0.79%
-     - 466
+     - 0.78%
+     - 469
    * - HR
      - 0.78%
-     - 462
-   * - DK
-     - 0.67%
-     - 395
+     - 466
    * - IE
      - 0.66%
-     - 389
+     - 395
+   * - DK
+     - 0.66%
+     - 395
    * - TW
-     - 0.61%
+     - 0.60%
      - 363
    * - IL
-     - 0.58%
+     - 0.57%
      - 341
    * - NL
-     - 0.50%
+     - 0.49%
      - 297
    * - ES
      - 0.44%
      - 262
    * - CH
      - 0.42%
-     - 251
+     - 254
    * - AE
-     - 0.35%
+     - 0.34%
      - 207
    * - CZ
      - 0.24%
      - 144
    * - FI
      - 0.16%
-     - 93
+     - 97
    * - ZA
      - 0.15%
      - 89
    * - BR
      - 0.13%
      - 77
    * - PL
      - 0.10%
      - 61
-   * - TR
+   * - CW
      - 0.07%
      - 44
-   * - CW
+   * - TR
      - 0.07%
      - 44
    * - OM
      - 0.07%
      - 42
    * - IS
      - 0.07%
@@ -501,28 +501,28 @@
    * - CY
      - 0.01%
      - 6
    * - DZ
      - 0.01%
      - 4
    * - EE
-     - 0.01%
+     - 0.00%
      - 3
    * - AR
-     - 0.01%
+     - 0.00%
      - 3
    * - SK
      - 0.00%
      - 2
-   * - RS
+   * - MX
      - 0.00%
      - 1
    * - PT
      - 0.00%
      - 1
-   * - MX
+   * - RS
      - 0.00%
      - 1
    * - **Total**
      - **100.00%**
-     - **59,255**
+     - **60,042**
```

### Comparing `nrobo-2024.40.0/nrobo.egg-info/SOURCES.txt` & `nrobo-2024.40.1/nrobo.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -40,14 +40,16 @@
 nrobo/framework/conftest-host.py
 nrobo/framework/nrobo-config.yaml
 nrobo/framework/requirements.txt
 nrobo/framework/secrets.yaml
 nrobo/framework/pages/PagePyPiHome.py
 nrobo/framework/pages/PageSearch.py
 nrobo/framework/pages/__init__.py
+nrobo/framework/test-data/__init__.py
+nrobo/framework/test-data/nRoBo-Logo.png
 nrobo/framework/tests/__init__.py
 nrobo/framework/tests/mobile/appium/test_appium.py
 nrobo/framework/tests/web/PyPi_home_page_test.py
 nrobo/framework/tests/web/examples/__init__.py
 nrobo/framework/tests/web/gui/PyPi_home_page_test.py
 nrobo/framework/tests/web/gui/__init__.py
 nrobo/framework/tests/web/no_gui/__init__.py
```

### Comparing `nrobo-2024.40.0/pyproject.toml` & `nrobo-2024.40.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [build-system]
 requires = ["setuptools >= 40.7.0",]
 build-backend = "setuptools.build_meta"
 
 # Project details
 [project]
 name = "nrobo"
-version = "2024.40.0"
+version = "2024.40.1"
 authors = [{name="Panchdev Singh Chauhan", email="erpanchdev@gmail.com"}]
 maintainers = [{name="Panchdev Singh Chauhan", email="erpanchdev@gmail.com"}]
 description = "Powerful! Yet, Easy to USE! Automated Testing Framework"
 readme = "README.rst"
 keywords = ["test automation", "test automation framework", "automated testing", "automation testing", "testing", "qa", "acceptance test", "automation"]
 classifiers = [
     "Programming Language :: Python :: 3 :: Only",
```

