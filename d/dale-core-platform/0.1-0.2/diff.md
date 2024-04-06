# Comparing `tmp/dale-core-platform-0.1.tar.gz` & `tmp/dale-core-platform-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dale-core-platform-0.1.tar", last modified: Sat Apr  6 01:32:44 2024, max compression
+gzip compressed data, was "dale-core-platform-0.2.tar", last modified: Sat Apr  6 04:05:31 2024, max compression
```

## Comparing `dale-core-platform-0.1.tar` & `dale-core-platform-0.2.tar`

### file list

```diff
@@ -1,128 +1,128 @@
-drwxr-xr-x   0 dale       (501) staff       (20)        0 2024-04-06 01:32:44.494183 dale-core-platform-0.1/
--rw-r--r--   0 dale       (501) staff       (20)     1066 2024-04-06 00:58:28.000000 dale-core-platform-0.1/LICENSE
--rw-r--r--   0 dale       (501) staff       (20)      981 2024-04-06 01:32:44.493895 dale-core-platform-0.1/PKG-INFO
--rw-r--r--   0 dale       (501) staff       (20)       67 2024-04-06 00:58:28.000000 dale-core-platform-0.1/README.md
-drwxr-xr-x   0 dale       (501) staff       (20)        0 2024-04-06 01:32:44.467463 dale-core-platform-0.1/cores/
--rw-r--r--   0 dale       (501) staff       (20)        0 2024-04-06 00:58:33.000000 dale-core-platform-0.1/cores/__init__.py
-drwxr-xr-x   0 dale       (501) staff       (20)        0 2024-04-06 01:32:44.467953 dale-core-platform-0.1/cores/const/
--rw-r--r--   0 dale       (501) staff       (20)      309 2024-04-06 00:58:33.000000 dale-core-platform-0.1/cores/const/__const.py
--rw-r--r--   0 dale       (501) staff       (20)        0 2024-04-06 00:58:33.000000 dale-core-platform-0.1/cores/const/__init__.py
-drwxr-xr-x   0 dale       (501) staff       (20)        0 2024-04-06 01:32:44.469487 dale-core-platform-0.1/cores/const/api/
--rw-r--r--   0 dale       (501) staff       (20)       94 2024-04-06 00:58:33.000000 dale-core-platform-0.1/cores/const/api/__init__.py
--rw-r--r--   0 dale       (501) staff       (20)      160 2024-04-06 00:58:33.000000 dale-core-platform-0.1/cores/const/api/api.py
--rw-r--r--   0 dale       (501) staff       (20)     1198 2024-04-06 00:58:33.000000 dale-core-platform-0.1/cores/const/api/request.py
--rw-r--r--   0 dale       (501) staff       (20)     1610 2024-04-06 00:58:33.000000 dale-core-platform-0.1/cores/const/api/swagger.py
-drwxr-xr-x   0 dale       (501) staff       (20)        0 2024-04-06 01:32:44.473472 dale-core-platform-0.1/cores/const/common/
--rw-r--r--   0 dale       (501) staff       (20)      368 2024-04-06 00:58:33.000000 dale-core-platform-0.1/cores/const/common/__init__.py
--rw-r--r--   0 dale       (501) staff       (20)   154078 2024-04-06 00:58:33.000000 dale-core-platform-0.1/cores/const/common/color_const.py
--rw-r--r--   0 dale       (501) staff       (20)      165 2024-04-06 00:58:33.000000 dale-core-platform-0.1/cores/const/common/common_const.py
--rw-r--r--   0 dale       (501) staff       (20)    26968 2024-04-06 00:58:33.000000 dale-core-platform-0.1/cores/const/common/emoji_const.py
--rw-r--r--   0 dale       (501) staff       (20)     2337 2024-04-06 00:58:33.000000 dale-core-platform-0.1/cores/const/common/environment_const.py
--rw-r--r--   0 dale       (501) staff       (20)     1103 2024-04-06 00:58:33.000000 dale-core-platform-0.1/cores/const/common/key_codes_const.py
--rw-r--r--   0 dale       (501) staff       (20)      586 2024-04-06 00:58:33.000000 dale-core-platform-0.1/cores/const/common/msg_const.py
--rw-r--r--   0 dale       (501) staff       (20)      166 2024-04-06 00:58:33.000000 dale-core-platform-0.1/cores/const/common/path_const.py
--rw-r--r--   0 dale       (501) staff       (20)       44 2024-04-06 00:58:33.000000 dale-core-platform-0.1/cores/const/common/store_const.py
--rw-r--r--   0 dale       (501) staff       (20)      216 2024-04-06 00:58:33.000000 dale-core-platform-0.1/cores/const/common/string_const.py
--rw-r--r--   0 dale       (501) staff       (20)     3420 2024-04-06 00:58:33.000000 dale-core-platform-0.1/cores/const/common/times_const.py
--rw-r--r--   0 dale       (501) staff       (20)      191 2024-04-06 00:58:33.000000 dale-core-platform-0.1/cores/const/common/types_const.py
-drwxr-xr-x   0 dale       (501) staff       (20)        0 2024-04-06 01:32:44.473876 dale-core-platform-0.1/cores/const/config/
--rw-r--r--   0 dale       (501) staff       (20)       51 2024-04-06 00:58:33.000000 dale-core-platform-0.1/cores/const/config/__init__.py
--rw-r--r--   0 dale       (501) staff       (20)      164 2024-04-06 00:58:33.000000 dale-core-platform-0.1/cores/const/config/testlink_const.py
-drwxr-xr-x   0 dale       (501) staff       (20)        0 2024-04-06 01:32:44.474292 dale-core-platform-0.1/cores/const/custom_exception/
--rw-r--r--   0 dale       (501) staff       (20)      100 2024-04-06 00:58:33.000000 dale-core-platform-0.1/cores/const/custom_exception/__init__.py
--rw-r--r--   0 dale       (501) staff       (20)      734 2024-04-06 00:58:33.000000 dale-core-platform-0.1/cores/const/custom_exception/custom_exception.py
-drwxr-xr-x   0 dale       (501) staff       (20)        0 2024-04-06 01:32:44.474717 dale-core-platform-0.1/cores/const/database/
--rw-r--r--   0 dale       (501) staff       (20)       36 2024-04-06 00:58:33.000000 dale-core-platform-0.1/cores/const/database/__init__.py
--rw-r--r--   0 dale       (501) staff       (20)      320 2024-04-06 00:58:33.000000 dale-core-platform-0.1/cores/const/database/db_const.py
-drwxr-xr-x   0 dale       (501) staff       (20)        0 2024-04-06 01:32:44.477041 dale-core-platform-0.1/cores/const/mobile/
--rw-r--r--   0 dale       (501) staff       (20)      228 2024-04-06 00:58:33.000000 dale-core-platform-0.1/cores/const/mobile/__init__.py
--rw-r--r--   0 dale       (501) staff       (20)      194 2024-04-06 00:58:33.000000 dale-core-platform-0.1/cores/const/mobile/appium_server_const.py
--rw-r--r--   0 dale       (501) staff       (20)      286 2024-04-06 00:58:33.000000 dale-core-platform-0.1/cores/const/mobile/capabilities_const.py
--rw-r--r--   0 dale       (501) staff       (20)     1836 2024-04-06 00:58:33.000000 dale-core-platform-0.1/cores/const/mobile/command_const.py
--rw-r--r--   0 dale       (501) staff       (20)      427 2024-04-06 00:58:33.000000 dale-core-platform-0.1/cores/const/mobile/device_const.py
--rw-r--r--   0 dale       (501) staff       (20)      369 2024-04-06 00:58:33.000000 dale-core-platform-0.1/cores/const/mobile/mobile_command_const.py
-drwxr-xr-x   0 dale       (501) staff       (20)        0 2024-04-06 01:32:44.477450 dale-core-platform-0.1/cores/const/web/
--rw-r--r--   0 dale       (501) staff       (20)       53 2024-04-06 00:58:33.000000 dale-core-platform-0.1/cores/const/web/__init__.py
--rw-r--r--   0 dale       (501) staff       (20)      156 2024-04-06 00:58:33.000000 dale-core-platform-0.1/cores/const/web/browsers_const.py
-drwxr-xr-x   0 dale       (501) staff       (20)        0 2024-04-06 01:32:44.478481 dale-core-platform-0.1/cores/decorators/
--rw-r--r--   0 dale       (501) staff       (20)      155 2024-04-06 00:58:33.000000 dale-core-platform-0.1/cores/decorators/__init__.py
--rw-r--r--   0 dale       (501) staff       (20)     2449 2024-04-06 00:58:33.000000 dale-core-platform-0.1/cores/decorators/handle_exception.py
--rw-r--r--   0 dale       (501) staff       (20)     2759 2024-04-06 00:58:33.000000 dale-core-platform-0.1/cores/decorators/parse_config.py
--rw-r--r--   0 dale       (501) staff       (20)     1551 2024-04-06 00:58:33.000000 dale-core-platform-0.1/cores/decorators/retry.py
-drwxr-xr-x   0 dale       (501) staff       (20)        0 2024-04-06 01:32:44.478707 dale-core-platform-0.1/cores/factory/
--rw-r--r--   0 dale       (501) staff       (20)       62 2024-04-06 00:58:33.000000 dale-core-platform-0.1/cores/factory/__init__.py
-drwxr-xr-x   0 dale       (501) staff       (20)        0 2024-04-06 01:32:44.480171 dale-core-platform-0.1/cores/factory/database_factory/
--rw-r--r--   0 dale       (501) staff       (20)       80 2024-04-06 00:58:33.000000 dale-core-platform-0.1/cores/factory/database_factory/__init__.py
--rw-r--r--   0 dale       (501) staff       (20)      741 2024-04-06 00:58:33.000000 dale-core-platform-0.1/cores/factory/database_factory/database_conn_generator.py
--rw-r--r--   0 dale       (501) staff       (20)     4902 2024-04-06 00:58:33.000000 dale-core-platform-0.1/cores/factory/database_factory/database_factory.py
-drwxr-xr-x   0 dale       (501) staff       (20)        0 2024-04-06 01:32:44.480538 dale-core-platform-0.1/cores/factory/driver_factory/
--rw-r--r--   0 dale       (501) staff       (20)      455 2024-04-06 00:58:33.000000 dale-core-platform-0.1/cores/factory/driver_factory/__init__.py
-drwxr-xr-x   0 dale       (501) staff       (20)        0 2024-04-06 01:32:44.481739 dale-core-platform-0.1/cores/factory/driver_factory/appium/
--rw-r--r--   0 dale       (501) staff       (20)        0 2024-04-06 00:58:33.000000 dale-core-platform-0.1/cores/factory/driver_factory/appium/__init__.py
--rw-r--r--   0 dale       (501) staff       (20)     3917 2024-04-06 00:58:33.000000 dale-core-platform-0.1/cores/factory/driver_factory/appium/appium_actions.py
--rw-r--r--   0 dale       (501) staff       (20)     1113 2024-04-06 00:58:33.000000 dale-core-platform-0.1/cores/factory/driver_factory/appium/appium_server.py
--rw-r--r--   0 dale       (501) staff       (20)     3197 2024-04-06 00:58:33.000000 dale-core-platform-0.1/cores/factory/driver_factory/appium/application_helper.py
--rw-r--r--   0 dale       (501) staff       (20)     3561 2024-04-06 00:58:33.000000 dale-core-platform-0.1/cores/factory/driver_factory/appium/mobile_driver.py
--rw-r--r--   0 dale       (501) staff       (20)    12268 2024-04-06 00:58:33.000000 dale-core-platform-0.1/cores/factory/driver_factory/appium/virtual_device.py
-drwxr-xr-x   0 dale       (501) staff       (20)        0 2024-04-06 01:32:44.483055 dale-core-platform-0.1/cores/factory/driver_factory/selenium/
--rw-r--r--   0 dale       (501) staff       (20)      134 2024-04-06 00:58:33.000000 dale-core-platform-0.1/cores/factory/driver_factory/selenium/__init__.py
--rw-r--r--   0 dale       (501) staff       (20)     1901 2024-04-06 00:58:33.000000 dale-core-platform-0.1/cores/factory/driver_factory/selenium/locator_modify_util.py
--rw-r--r--   0 dale       (501) staff       (20)    13617 2024-04-06 00:58:33.000000 dale-core-platform-0.1/cores/factory/driver_factory/selenium/selenium_actions.py
--rw-r--r--   0 dale       (501) staff       (20)      151 2024-04-06 00:58:33.000000 dale-core-platform-0.1/cores/factory/driver_factory/selenium/selenium_base.py
--rw-r--r--   0 dale       (501) staff       (20)     5025 2024-04-06 00:58:33.000000 dale-core-platform-0.1/cores/factory/driver_factory/selenium/selenium_driver.py
-drwxr-xr-x   0 dale       (501) staff       (20)        0 2024-04-06 01:32:44.483929 dale-core-platform-0.1/cores/factory/request_factory/
--rw-r--r--   0 dale       (501) staff       (20)      111 2024-04-06 00:58:33.000000 dale-core-platform-0.1/cores/factory/request_factory/__init__.py
--rw-r--r--   0 dale       (501) staff       (20)     5012 2024-04-06 00:58:33.000000 dale-core-platform-0.1/cores/factory/request_factory/base_factory.py
--rw-r--r--   0 dale       (501) staff       (20)     2833 2024-04-06 00:58:33.000000 dale-core-platform-0.1/cores/factory/request_factory/request_generator.py
-drwxr-xr-x   0 dale       (501) staff       (20)        0 2024-04-06 01:32:44.485111 dale-core-platform-0.1/cores/model/
--rw-r--r--   0 dale       (501) staff       (20)      125 2024-04-06 00:58:33.000000 dale-core-platform-0.1/cores/model/__init__.py
--rw-r--r--   0 dale       (501) staff       (20)      246 2024-04-06 00:58:33.000000 dale-core-platform-0.1/cores/model/db_conn.py
--rw-r--r--   0 dale       (501) staff       (20)      610 2024-04-06 00:58:33.000000 dale-core-platform-0.1/cores/model/environment.py
--rw-r--r--   0 dale       (501) staff       (20)      730 2024-04-06 00:58:33.000000 dale-core-platform-0.1/cores/model/request.py
--rw-r--r--   0 dale       (501) staff       (20)      348 2024-04-06 00:58:33.000000 dale-core-platform-0.1/cores/model/users.py
-drwxr-xr-x   0 dale       (501) staff       (20)        0 2024-04-06 01:32:44.485556 dale-core-platform-0.1/cores/utils/
--rw-r--r--   0 dale       (501) staff       (20)        0 2024-04-06 00:58:33.000000 dale-core-platform-0.1/cores/utils/__init__.py
-drwxr-xr-x   0 dale       (501) staff       (20)        0 2024-04-06 01:32:44.487015 dale-core-platform-0.1/cores/utils/backend/
--rw-r--r--   0 dale       (501) staff       (20)      203 2024-04-06 00:58:33.000000 dale-core-platform-0.1/cores/utils/backend/__init__.py
--rw-r--r--   0 dale       (501) staff       (20)      236 2024-04-06 00:58:33.000000 dale-core-platform-0.1/cores/utils/backend/data_setup_util.py
--rw-r--r--   0 dale       (501) staff       (20)     4045 2024-04-06 00:58:33.000000 dale-core-platform-0.1/cores/utils/backend/gitlab_util.py
--rw-r--r--   0 dale       (501) staff       (20)     8418 2024-04-06 00:58:33.000000 dale-core-platform-0.1/cores/utils/backend/request_util.py
--rw-r--r--   0 dale       (501) staff       (20)    13480 2024-04-06 00:58:33.000000 dale-core-platform-0.1/cores/utils/backend/swagger_parser_util.py
--rw-r--r--   0 dale       (501) staff       (20)      438 2024-04-06 00:58:33.000000 dale-core-platform-0.1/cores/utils/backend/verify_util.py
-drwxr-xr-x   0 dale       (501) staff       (20)        0 2024-04-06 01:32:44.490425 dale-core-platform-0.1/cores/utils/common/
--rw-r--r--   0 dale       (501) staff       (20)      483 2024-04-06 00:58:33.000000 dale-core-platform-0.1/cores/utils/common/__init__.py
--rw-r--r--   0 dale       (501) staff       (20)     4438 2024-04-06 00:58:33.000000 dale-core-platform-0.1/cores/utils/common/assertion_util.py
--rw-r--r--   0 dale       (501) staff       (20)     2094 2024-04-06 00:58:33.000000 dale-core-platform-0.1/cores/utils/common/color_util.py
--rw-r--r--   0 dale       (501) staff       (20)     3014 2024-04-06 00:58:33.000000 dale-core-platform-0.1/cores/utils/common/csv_util.py
--rw-r--r--   0 dale       (501) staff       (20)      596 2024-04-06 00:58:33.000000 dale-core-platform-0.1/cores/utils/common/execute_java_file.py
--rw-r--r--   0 dale       (501) staff       (20)      745 2024-04-06 00:58:33.000000 dale-core-platform-0.1/cores/utils/common/json_util.py
--rw-r--r--   0 dale       (501) staff       (20)      842 2024-04-06 00:58:33.000000 dale-core-platform-0.1/cores/utils/common/logger_util.py
--rw-r--r--   0 dale       (501) staff       (20)     1424 2024-04-06 00:58:33.000000 dale-core-platform-0.1/cores/utils/common/path_util.py
--rw-r--r--   0 dale       (501) staff       (20)     2980 2024-04-06 00:58:33.000000 dale-core-platform-0.1/cores/utils/common/prepare_fake_data.py
--rw-r--r--   0 dale       (501) staff       (20)      163 2024-04-06 00:58:33.000000 dale-core-platform-0.1/cores/utils/common/prepare_object.py
--rw-r--r--   0 dale       (501) staff       (20)     2415 2024-04-06 00:58:33.000000 dale-core-platform-0.1/cores/utils/common/store_util.py
--rw-r--r--   0 dale       (501) staff       (20)    10013 2024-04-06 00:58:33.000000 dale-core-platform-0.1/cores/utils/common/string_util.py
--rw-r--r--   0 dale       (501) staff       (20)     2250 2024-04-06 00:58:33.000000 dale-core-platform-0.1/cores/utils/common/time_util.py
-drwxr-xr-x   0 dale       (501) staff       (20)        0 2024-04-06 01:32:44.490631 dale-core-platform-0.1/cores/utils/perf/
--rw-r--r--   0 dale       (501) staff       (20)        0 2024-04-06 00:58:33.000000 dale-core-platform-0.1/cores/utils/perf/__init__.py
-drwxr-xr-x   0 dale       (501) staff       (20)        0 2024-04-06 01:32:44.491186 dale-core-platform-0.1/cores/utils/perf/selenium_headless_locust/
--rw-r--r--   0 dale       (501) staff       (20)      282 2024-04-06 00:58:33.000000 dale-core-platform-0.1/cores/utils/perf/selenium_headless_locust/__init__.py
--rw-r--r--   0 dale       (501) staff       (20)     2996 2024-04-06 00:58:33.000000 dale-core-platform-0.1/cores/utils/perf/selenium_headless_locust/core.py
--rw-r--r--   0 dale       (501) staff       (20)     3075 2024-04-06 00:58:33.000000 dale-core-platform-0.1/cores/utils/perf/selenium_headless_locust/locusts.py
-drwxr-xr-x   0 dale       (501) staff       (20)        0 2024-04-06 01:32:44.492370 dale-core-platform-0.1/cores/utils/testlink/
--rw-r--r--   0 dale       (501) staff       (20)      224 2024-04-06 00:58:33.000000 dale-core-platform-0.1/cores/utils/testlink/__init__.py
--rw-r--r--   0 dale       (501) staff       (20)     2546 2024-04-06 00:58:33.000000 dale-core-platform-0.1/cores/utils/testlink/add_remove_test_case.py
--rw-r--r--   0 dale       (501) staff       (20)      988 2024-04-06 00:58:33.000000 dale-core-platform-0.1/cores/utils/testlink/base_test_link.py
--rw-r--r--   0 dale       (501) staff       (20)      818 2024-04-06 00:58:33.000000 dale-core-platform-0.1/cores/utils/testlink/create_new_build.py
--rw-r--r--   0 dale       (501) staff       (20)     1296 2024-04-06 00:58:33.000000 dale-core-platform-0.1/cores/utils/testlink/set_test_case_result.py
--rw-r--r--   0 dale       (501) staff       (20)     1588 2024-04-06 00:58:33.000000 dale-core-platform-0.1/cores/utils/testlink/test_plan_management.py
-drwxr-xr-x   0 dale       (501) staff       (20)        0 2024-04-06 01:32:44.493215 dale-core-platform-0.1/dale_core_platform.egg-info/
--rw-r--r--   0 dale       (501) staff       (20)      981 2024-04-06 01:32:44.000000 dale-core-platform-0.1/dale_core_platform.egg-info/PKG-INFO
--rw-r--r--   0 dale       (501) staff       (20)     3681 2024-04-06 01:32:44.000000 dale-core-platform-0.1/dale_core_platform.egg-info/SOURCES.txt
--rw-r--r--   0 dale       (501) staff       (20)        1 2024-04-06 01:32:44.000000 dale-core-platform-0.1/dale_core_platform.egg-info/dependency_links.txt
--rw-r--r--   0 dale       (501) staff       (20)      372 2024-04-06 01:32:44.000000 dale-core-platform-0.1/dale_core_platform.egg-info/requires.txt
--rw-r--r--   0 dale       (501) staff       (20)       16 2024-04-06 01:32:44.000000 dale-core-platform-0.1/dale_core_platform.egg-info/top_level.txt
--rw-r--r--   0 dale       (501) staff       (20)       38 2024-04-06 01:32:44.494237 dale-core-platform-0.1/setup.cfg
--rw-r--r--   0 dale       (501) staff       (20)     1008 2024-04-06 01:32:35.000000 dale-core-platform-0.1/setup.py
-drwxr-xr-x   0 dale       (501) staff       (20)        0 2024-04-06 01:32:44.493387 dale-core-platform-0.1/unittests/
--rw-r--r--   0 dale       (501) staff       (20)      229 2024-04-06 00:58:28.000000 dale-core-platform-0.1/unittests/__init__.py
+drwxr-xr-x   0 dale       (501) staff       (20)        0 2024-04-06 04:05:31.654904 dale-core-platform-0.2/
+-rw-r--r--   0 dale       (501) staff       (20)     1066 2024-04-06 00:58:28.000000 dale-core-platform-0.2/LICENSE
+-rw-r--r--   0 dale       (501) staff       (20)      988 2024-04-06 04:05:31.654546 dale-core-platform-0.2/PKG-INFO
+-rw-r--r--   0 dale       (501) staff       (20)       67 2024-04-06 00:58:28.000000 dale-core-platform-0.2/README.md
+drwxr-xr-x   0 dale       (501) staff       (20)        0 2024-04-06 04:05:31.625424 dale-core-platform-0.2/cores/
+-rw-r--r--   0 dale       (501) staff       (20)        0 2024-04-06 00:58:33.000000 dale-core-platform-0.2/cores/__init__.py
+drwxr-xr-x   0 dale       (501) staff       (20)        0 2024-04-06 04:05:31.625923 dale-core-platform-0.2/cores/const/
+-rw-r--r--   0 dale       (501) staff       (20)      309 2024-04-06 00:58:33.000000 dale-core-platform-0.2/cores/const/__const.py
+-rw-r--r--   0 dale       (501) staff       (20)        0 2024-04-06 00:58:33.000000 dale-core-platform-0.2/cores/const/__init__.py
+drwxr-xr-x   0 dale       (501) staff       (20)        0 2024-04-06 04:05:31.627407 dale-core-platform-0.2/cores/const/api/
+-rw-r--r--   0 dale       (501) staff       (20)       94 2024-04-06 00:58:33.000000 dale-core-platform-0.2/cores/const/api/__init__.py
+-rw-r--r--   0 dale       (501) staff       (20)      160 2024-04-06 00:58:33.000000 dale-core-platform-0.2/cores/const/api/api.py
+-rw-r--r--   0 dale       (501) staff       (20)     1198 2024-04-06 00:58:33.000000 dale-core-platform-0.2/cores/const/api/request.py
+-rw-r--r--   0 dale       (501) staff       (20)     1610 2024-04-06 00:58:33.000000 dale-core-platform-0.2/cores/const/api/swagger.py
+drwxr-xr-x   0 dale       (501) staff       (20)        0 2024-04-06 04:05:31.632107 dale-core-platform-0.2/cores/const/common/
+-rw-r--r--   0 dale       (501) staff       (20)      368 2024-04-06 00:58:33.000000 dale-core-platform-0.2/cores/const/common/__init__.py
+-rw-r--r--   0 dale       (501) staff       (20)   154078 2024-04-06 00:58:33.000000 dale-core-platform-0.2/cores/const/common/color_const.py
+-rw-r--r--   0 dale       (501) staff       (20)      165 2024-04-06 00:58:33.000000 dale-core-platform-0.2/cores/const/common/common_const.py
+-rw-r--r--   0 dale       (501) staff       (20)    26968 2024-04-06 00:58:33.000000 dale-core-platform-0.2/cores/const/common/emoji_const.py
+-rw-r--r--   0 dale       (501) staff       (20)     2337 2024-04-06 00:58:33.000000 dale-core-platform-0.2/cores/const/common/environment_const.py
+-rw-r--r--   0 dale       (501) staff       (20)     1103 2024-04-06 00:58:33.000000 dale-core-platform-0.2/cores/const/common/key_codes_const.py
+-rw-r--r--   0 dale       (501) staff       (20)      586 2024-04-06 00:58:33.000000 dale-core-platform-0.2/cores/const/common/msg_const.py
+-rw-r--r--   0 dale       (501) staff       (20)      166 2024-04-06 00:58:33.000000 dale-core-platform-0.2/cores/const/common/path_const.py
+-rw-r--r--   0 dale       (501) staff       (20)       44 2024-04-06 00:58:33.000000 dale-core-platform-0.2/cores/const/common/store_const.py
+-rw-r--r--   0 dale       (501) staff       (20)      216 2024-04-06 00:58:33.000000 dale-core-platform-0.2/cores/const/common/string_const.py
+-rw-r--r--   0 dale       (501) staff       (20)     3420 2024-04-06 00:58:33.000000 dale-core-platform-0.2/cores/const/common/times_const.py
+-rw-r--r--   0 dale       (501) staff       (20)      191 2024-04-06 00:58:33.000000 dale-core-platform-0.2/cores/const/common/types_const.py
+drwxr-xr-x   0 dale       (501) staff       (20)        0 2024-04-06 04:05:31.632573 dale-core-platform-0.2/cores/const/config/
+-rw-r--r--   0 dale       (501) staff       (20)       51 2024-04-06 00:58:33.000000 dale-core-platform-0.2/cores/const/config/__init__.py
+-rw-r--r--   0 dale       (501) staff       (20)      164 2024-04-06 00:58:33.000000 dale-core-platform-0.2/cores/const/config/testlink_const.py
+drwxr-xr-x   0 dale       (501) staff       (20)        0 2024-04-06 04:05:31.633212 dale-core-platform-0.2/cores/const/custom_exception/
+-rw-r--r--   0 dale       (501) staff       (20)      100 2024-04-06 00:58:33.000000 dale-core-platform-0.2/cores/const/custom_exception/__init__.py
+-rw-r--r--   0 dale       (501) staff       (20)      734 2024-04-06 00:58:33.000000 dale-core-platform-0.2/cores/const/custom_exception/custom_exception.py
+drwxr-xr-x   0 dale       (501) staff       (20)        0 2024-04-06 04:05:31.633671 dale-core-platform-0.2/cores/const/database/
+-rw-r--r--   0 dale       (501) staff       (20)       36 2024-04-06 00:58:33.000000 dale-core-platform-0.2/cores/const/database/__init__.py
+-rw-r--r--   0 dale       (501) staff       (20)      320 2024-04-06 00:58:33.000000 dale-core-platform-0.2/cores/const/database/db_const.py
+drwxr-xr-x   0 dale       (501) staff       (20)        0 2024-04-06 04:05:31.635214 dale-core-platform-0.2/cores/const/mobile/
+-rw-r--r--   0 dale       (501) staff       (20)      228 2024-04-06 00:58:33.000000 dale-core-platform-0.2/cores/const/mobile/__init__.py
+-rw-r--r--   0 dale       (501) staff       (20)      194 2024-04-06 00:58:33.000000 dale-core-platform-0.2/cores/const/mobile/appium_server_const.py
+-rw-r--r--   0 dale       (501) staff       (20)      286 2024-04-06 00:58:33.000000 dale-core-platform-0.2/cores/const/mobile/capabilities_const.py
+-rw-r--r--   0 dale       (501) staff       (20)     1836 2024-04-06 00:58:33.000000 dale-core-platform-0.2/cores/const/mobile/command_const.py
+-rw-r--r--   0 dale       (501) staff       (20)      427 2024-04-06 00:58:33.000000 dale-core-platform-0.2/cores/const/mobile/device_const.py
+-rw-r--r--   0 dale       (501) staff       (20)      369 2024-04-06 00:58:33.000000 dale-core-platform-0.2/cores/const/mobile/mobile_command_const.py
+drwxr-xr-x   0 dale       (501) staff       (20)        0 2024-04-06 04:05:31.635890 dale-core-platform-0.2/cores/const/web/
+-rw-r--r--   0 dale       (501) staff       (20)       53 2024-04-06 00:58:33.000000 dale-core-platform-0.2/cores/const/web/__init__.py
+-rw-r--r--   0 dale       (501) staff       (20)      156 2024-04-06 00:58:33.000000 dale-core-platform-0.2/cores/const/web/browsers_const.py
+drwxr-xr-x   0 dale       (501) staff       (20)        0 2024-04-06 04:05:31.637624 dale-core-platform-0.2/cores/decorators/
+-rw-r--r--   0 dale       (501) staff       (20)      155 2024-04-06 00:58:33.000000 dale-core-platform-0.2/cores/decorators/__init__.py
+-rw-r--r--   0 dale       (501) staff       (20)     2449 2024-04-06 00:58:33.000000 dale-core-platform-0.2/cores/decorators/handle_exception.py
+-rw-r--r--   0 dale       (501) staff       (20)     2759 2024-04-06 00:58:33.000000 dale-core-platform-0.2/cores/decorators/parse_config.py
+-rw-r--r--   0 dale       (501) staff       (20)     1551 2024-04-06 00:58:33.000000 dale-core-platform-0.2/cores/decorators/retry.py
+drwxr-xr-x   0 dale       (501) staff       (20)        0 2024-04-06 04:05:31.637883 dale-core-platform-0.2/cores/factory/
+-rw-r--r--   0 dale       (501) staff       (20)       62 2024-04-06 00:58:33.000000 dale-core-platform-0.2/cores/factory/__init__.py
+drwxr-xr-x   0 dale       (501) staff       (20)        0 2024-04-06 04:05:31.639437 dale-core-platform-0.2/cores/factory/database_factory/
+-rw-r--r--   0 dale       (501) staff       (20)       80 2024-04-06 00:58:33.000000 dale-core-platform-0.2/cores/factory/database_factory/__init__.py
+-rw-r--r--   0 dale       (501) staff       (20)      741 2024-04-06 00:58:33.000000 dale-core-platform-0.2/cores/factory/database_factory/database_conn_generator.py
+-rw-r--r--   0 dale       (501) staff       (20)     4902 2024-04-06 00:58:33.000000 dale-core-platform-0.2/cores/factory/database_factory/database_factory.py
+drwxr-xr-x   0 dale       (501) staff       (20)        0 2024-04-06 04:05:31.639924 dale-core-platform-0.2/cores/factory/driver_factory/
+-rw-r--r--   0 dale       (501) staff       (20)      455 2024-04-06 00:58:33.000000 dale-core-platform-0.2/cores/factory/driver_factory/__init__.py
+drwxr-xr-x   0 dale       (501) staff       (20)        0 2024-04-06 04:05:31.641820 dale-core-platform-0.2/cores/factory/driver_factory/appium/
+-rw-r--r--   0 dale       (501) staff       (20)        0 2024-04-06 00:58:33.000000 dale-core-platform-0.2/cores/factory/driver_factory/appium/__init__.py
+-rw-r--r--   0 dale       (501) staff       (20)     3917 2024-04-06 00:58:33.000000 dale-core-platform-0.2/cores/factory/driver_factory/appium/appium_actions.py
+-rw-r--r--   0 dale       (501) staff       (20)     1113 2024-04-06 00:58:33.000000 dale-core-platform-0.2/cores/factory/driver_factory/appium/appium_server.py
+-rw-r--r--   0 dale       (501) staff       (20)     3197 2024-04-06 00:58:33.000000 dale-core-platform-0.2/cores/factory/driver_factory/appium/application_helper.py
+-rw-r--r--   0 dale       (501) staff       (20)     3561 2024-04-06 00:58:33.000000 dale-core-platform-0.2/cores/factory/driver_factory/appium/mobile_driver.py
+-rw-r--r--   0 dale       (501) staff       (20)    12268 2024-04-06 00:58:33.000000 dale-core-platform-0.2/cores/factory/driver_factory/appium/virtual_device.py
+drwxr-xr-x   0 dale       (501) staff       (20)        0 2024-04-06 04:05:31.643217 dale-core-platform-0.2/cores/factory/driver_factory/selenium/
+-rw-r--r--   0 dale       (501) staff       (20)      134 2024-04-06 00:58:33.000000 dale-core-platform-0.2/cores/factory/driver_factory/selenium/__init__.py
+-rw-r--r--   0 dale       (501) staff       (20)     1901 2024-04-06 00:58:33.000000 dale-core-platform-0.2/cores/factory/driver_factory/selenium/locator_modify_util.py
+-rw-r--r--   0 dale       (501) staff       (20)    13617 2024-04-06 00:58:33.000000 dale-core-platform-0.2/cores/factory/driver_factory/selenium/selenium_actions.py
+-rw-r--r--   0 dale       (501) staff       (20)      151 2024-04-06 00:58:33.000000 dale-core-platform-0.2/cores/factory/driver_factory/selenium/selenium_base.py
+-rw-r--r--   0 dale       (501) staff       (20)     5025 2024-04-06 00:58:33.000000 dale-core-platform-0.2/cores/factory/driver_factory/selenium/selenium_driver.py
+drwxr-xr-x   0 dale       (501) staff       (20)        0 2024-04-06 04:05:31.644269 dale-core-platform-0.2/cores/factory/request_factory/
+-rw-r--r--   0 dale       (501) staff       (20)      111 2024-04-06 00:58:33.000000 dale-core-platform-0.2/cores/factory/request_factory/__init__.py
+-rw-r--r--   0 dale       (501) staff       (20)     5012 2024-04-06 00:58:33.000000 dale-core-platform-0.2/cores/factory/request_factory/base_factory.py
+-rw-r--r--   0 dale       (501) staff       (20)     2833 2024-04-06 00:58:33.000000 dale-core-platform-0.2/cores/factory/request_factory/request_generator.py
+drwxr-xr-x   0 dale       (501) staff       (20)        0 2024-04-06 04:05:31.645476 dale-core-platform-0.2/cores/model/
+-rw-r--r--   0 dale       (501) staff       (20)      125 2024-04-06 00:58:33.000000 dale-core-platform-0.2/cores/model/__init__.py
+-rw-r--r--   0 dale       (501) staff       (20)      246 2024-04-06 00:58:33.000000 dale-core-platform-0.2/cores/model/db_conn.py
+-rw-r--r--   0 dale       (501) staff       (20)      610 2024-04-06 00:58:33.000000 dale-core-platform-0.2/cores/model/environment.py
+-rw-r--r--   0 dale       (501) staff       (20)      730 2024-04-06 00:58:33.000000 dale-core-platform-0.2/cores/model/request.py
+-rw-r--r--   0 dale       (501) staff       (20)      348 2024-04-06 00:58:33.000000 dale-core-platform-0.2/cores/model/users.py
+drwxr-xr-x   0 dale       (501) staff       (20)        0 2024-04-06 04:05:31.645894 dale-core-platform-0.2/cores/utils/
+-rw-r--r--   0 dale       (501) staff       (20)        0 2024-04-06 00:58:33.000000 dale-core-platform-0.2/cores/utils/__init__.py
+drwxr-xr-x   0 dale       (501) staff       (20)        0 2024-04-06 04:05:31.647510 dale-core-platform-0.2/cores/utils/backend/
+-rw-r--r--   0 dale       (501) staff       (20)      203 2024-04-06 00:58:33.000000 dale-core-platform-0.2/cores/utils/backend/__init__.py
+-rw-r--r--   0 dale       (501) staff       (20)      236 2024-04-06 00:58:33.000000 dale-core-platform-0.2/cores/utils/backend/data_setup_util.py
+-rw-r--r--   0 dale       (501) staff       (20)     4045 2024-04-06 00:58:33.000000 dale-core-platform-0.2/cores/utils/backend/gitlab_util.py
+-rw-r--r--   0 dale       (501) staff       (20)     8418 2024-04-06 00:58:33.000000 dale-core-platform-0.2/cores/utils/backend/request_util.py
+-rw-r--r--   0 dale       (501) staff       (20)    13480 2024-04-06 00:58:33.000000 dale-core-platform-0.2/cores/utils/backend/swagger_parser_util.py
+-rw-r--r--   0 dale       (501) staff       (20)      438 2024-04-06 00:58:33.000000 dale-core-platform-0.2/cores/utils/backend/verify_util.py
+drwxr-xr-x   0 dale       (501) staff       (20)        0 2024-04-06 04:05:31.650575 dale-core-platform-0.2/cores/utils/common/
+-rw-r--r--   0 dale       (501) staff       (20)      483 2024-04-06 00:58:33.000000 dale-core-platform-0.2/cores/utils/common/__init__.py
+-rw-r--r--   0 dale       (501) staff       (20)     4438 2024-04-06 00:58:33.000000 dale-core-platform-0.2/cores/utils/common/assertion_util.py
+-rw-r--r--   0 dale       (501) staff       (20)     2094 2024-04-06 00:58:33.000000 dale-core-platform-0.2/cores/utils/common/color_util.py
+-rw-r--r--   0 dale       (501) staff       (20)     3014 2024-04-06 00:58:33.000000 dale-core-platform-0.2/cores/utils/common/csv_util.py
+-rw-r--r--   0 dale       (501) staff       (20)      596 2024-04-06 00:58:33.000000 dale-core-platform-0.2/cores/utils/common/execute_java_file.py
+-rw-r--r--   0 dale       (501) staff       (20)      745 2024-04-06 00:58:33.000000 dale-core-platform-0.2/cores/utils/common/json_util.py
+-rw-r--r--   0 dale       (501) staff       (20)      842 2024-04-06 00:58:33.000000 dale-core-platform-0.2/cores/utils/common/logger_util.py
+-rw-r--r--   0 dale       (501) staff       (20)     1424 2024-04-06 00:58:33.000000 dale-core-platform-0.2/cores/utils/common/path_util.py
+-rw-r--r--   0 dale       (501) staff       (20)     2980 2024-04-06 00:58:33.000000 dale-core-platform-0.2/cores/utils/common/prepare_fake_data.py
+-rw-r--r--   0 dale       (501) staff       (20)      163 2024-04-06 00:58:33.000000 dale-core-platform-0.2/cores/utils/common/prepare_object.py
+-rw-r--r--   0 dale       (501) staff       (20)     2415 2024-04-06 00:58:33.000000 dale-core-platform-0.2/cores/utils/common/store_util.py
+-rw-r--r--   0 dale       (501) staff       (20)    10013 2024-04-06 00:58:33.000000 dale-core-platform-0.2/cores/utils/common/string_util.py
+-rw-r--r--   0 dale       (501) staff       (20)     2250 2024-04-06 00:58:33.000000 dale-core-platform-0.2/cores/utils/common/time_util.py
+drwxr-xr-x   0 dale       (501) staff       (20)        0 2024-04-06 04:05:31.650773 dale-core-platform-0.2/cores/utils/perf/
+-rw-r--r--   0 dale       (501) staff       (20)        0 2024-04-06 00:58:33.000000 dale-core-platform-0.2/cores/utils/perf/__init__.py
+drwxr-xr-x   0 dale       (501) staff       (20)        0 2024-04-06 04:05:31.651315 dale-core-platform-0.2/cores/utils/perf/selenium_headless_locust/
+-rw-r--r--   0 dale       (501) staff       (20)      282 2024-04-06 00:58:33.000000 dale-core-platform-0.2/cores/utils/perf/selenium_headless_locust/__init__.py
+-rw-r--r--   0 dale       (501) staff       (20)     2996 2024-04-06 00:58:33.000000 dale-core-platform-0.2/cores/utils/perf/selenium_headless_locust/core.py
+-rw-r--r--   0 dale       (501) staff       (20)     3075 2024-04-06 00:58:33.000000 dale-core-platform-0.2/cores/utils/perf/selenium_headless_locust/locusts.py
+drwxr-xr-x   0 dale       (501) staff       (20)        0 2024-04-06 04:05:31.652610 dale-core-platform-0.2/cores/utils/testlink/
+-rw-r--r--   0 dale       (501) staff       (20)      224 2024-04-06 00:58:33.000000 dale-core-platform-0.2/cores/utils/testlink/__init__.py
+-rw-r--r--   0 dale       (501) staff       (20)     2546 2024-04-06 00:58:33.000000 dale-core-platform-0.2/cores/utils/testlink/add_remove_test_case.py
+-rw-r--r--   0 dale       (501) staff       (20)      988 2024-04-06 00:58:33.000000 dale-core-platform-0.2/cores/utils/testlink/base_test_link.py
+-rw-r--r--   0 dale       (501) staff       (20)      818 2024-04-06 00:58:33.000000 dale-core-platform-0.2/cores/utils/testlink/create_new_build.py
+-rw-r--r--   0 dale       (501) staff       (20)     1296 2024-04-06 00:58:33.000000 dale-core-platform-0.2/cores/utils/testlink/set_test_case_result.py
+-rw-r--r--   0 dale       (501) staff       (20)     1588 2024-04-06 00:58:33.000000 dale-core-platform-0.2/cores/utils/testlink/test_plan_management.py
+drwxr-xr-x   0 dale       (501) staff       (20)        0 2024-04-06 04:05:31.653643 dale-core-platform-0.2/dale_core_platform.egg-info/
+-rw-r--r--   0 dale       (501) staff       (20)      988 2024-04-06 04:05:31.000000 dale-core-platform-0.2/dale_core_platform.egg-info/PKG-INFO
+-rw-r--r--   0 dale       (501) staff       (20)     3681 2024-04-06 04:05:31.000000 dale-core-platform-0.2/dale_core_platform.egg-info/SOURCES.txt
+-rw-r--r--   0 dale       (501) staff       (20)        1 2024-04-06 04:05:31.000000 dale-core-platform-0.2/dale_core_platform.egg-info/dependency_links.txt
+-rw-r--r--   0 dale       (501) staff       (20)      378 2024-04-06 04:05:31.000000 dale-core-platform-0.2/dale_core_platform.egg-info/requires.txt
+-rw-r--r--   0 dale       (501) staff       (20)       16 2024-04-06 04:05:31.000000 dale-core-platform-0.2/dale_core_platform.egg-info/top_level.txt
+-rw-r--r--   0 dale       (501) staff       (20)       38 2024-04-06 04:05:31.654962 dale-core-platform-0.2/setup.cfg
+-rw-r--r--   0 dale       (501) staff       (20)     1015 2024-04-06 04:05:10.000000 dale-core-platform-0.2/setup.py
+drwxr-xr-x   0 dale       (501) staff       (20)        0 2024-04-06 04:05:31.653819 dale-core-platform-0.2/unittests/
+-rw-r--r--   0 dale       (501) staff       (20)      229 2024-04-06 00:58:28.000000 dale-core-platform-0.2/unittests/__init__.py
```

### Comparing `dale-core-platform-0.1/LICENSE` & `dale-core-platform-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dale-core-platform-0.1/PKG-INFO` & `dale-core-platform-0.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: dale-core-platform
-Version: 0.1
-Summary: This package will include all the libs and helpers which built on Gauge framework. Support Selenim for web, Appium for Mobile, Requests for api and Locust for performance.
+Version: 0.2
+Summary: This package will include all the libs and helpers which built on Gauge framework. Support Selenium for web, Appium for Mobile, Requests for api and Locust for performance.
 Author: Dale Hoang
 Author-email: huy.quochoang2308@gmail.com
 License-File: LICENSE
-Requires-Dist: requests>=2.31
-Requires-Dist: colorlog>=6.7
-Requires-Dist: pydantic>=2.4.2
-Requires-Dist: behave>=1.2.6
-Requires-Dist: behavex>=3.0.0
-Requires-Dist: requests-to-curl>=1.1
-Requires-Dist: mysql-connector-python>=8.0.30
-Requires-Dist: pymongo>=4.2.0
-Requires-Dist: redis>=4.3.4
-Requires-Dist: psycopg2-binary>=2.9.7
-Requires-Dist: locust>=2.16.1
-Requires-Dist: python-gitlab>=3.15.0
-Requires-Dist: webdriver_manager>=4.0.1
-Requires-Dist: selenium==4.4.3
-Requires-Dist: Appium-Python-Client==2.9.0
-Requires-Dist: dataclasses-json>=0.6.2
-Requires-Dist: Faker==19.6.2
-Requires-Dist: TestLink-API-Python-client>=0.8.1
-Requires-Dist: getgauge>=0.4.0
+Requires-Dist: requests==2.31
+Requires-Dist: colorlog==6.7
+Requires-Dist: pydantic==2.4.2
+Requires-Dist: behave==1.2.6
+Requires-Dist: behavex==3.0.0
+Requires-Dist: requests-to-curl==1.1
+Requires-Dist: mysql-connector-python==8.0.30
+Requires-Dist: pymongo==4.2.0
+Requires-Dist: redis==4.3.4
+Requires-Dist: psycopg2-binary==2.9.7
+Requires-Dist: locust==2.16.1
+Requires-Dist: python-gitlab==3.15.0
+Requires-Dist: webdriver_manager==4.0.1
+Requires-Dist: selenium====4.4.3
+Requires-Dist: Appium-Python-Client====2.9.0
+Requires-Dist: dataclasses-json==0.6.2
+Requires-Dist: Faker====19.6.2
+Requires-Dist: TestLink-API-Python-client==0.8.1
+Requires-Dist: getgauge==0.4.0
```

### Comparing `dale-core-platform-0.1/cores/const/api/request.py` & `dale-core-platform-0.2/cores/const/api/request.py`

 * *Files identical despite different names*

### Comparing `dale-core-platform-0.1/cores/const/api/swagger.py` & `dale-core-platform-0.2/cores/const/api/swagger.py`

 * *Files identical despite different names*

### Comparing `dale-core-platform-0.1/cores/const/common/color_const.py` & `dale-core-platform-0.2/cores/const/common/color_const.py`

 * *Files identical despite different names*

### Comparing `dale-core-platform-0.1/cores/const/common/emoji_const.py` & `dale-core-platform-0.2/cores/const/common/emoji_const.py`

 * *Files identical despite different names*

### Comparing `dale-core-platform-0.1/cores/const/common/environment_const.py` & `dale-core-platform-0.2/cores/const/common/environment_const.py`

 * *Files identical despite different names*

### Comparing `dale-core-platform-0.1/cores/const/common/key_codes_const.py` & `dale-core-platform-0.2/cores/const/common/key_codes_const.py`

 * *Files identical despite different names*

### Comparing `dale-core-platform-0.1/cores/const/common/msg_const.py` & `dale-core-platform-0.2/cores/const/common/msg_const.py`

 * *Files identical despite different names*

### Comparing `dale-core-platform-0.1/cores/const/common/times_const.py` & `dale-core-platform-0.2/cores/const/common/times_const.py`

 * *Files identical despite different names*

### Comparing `dale-core-platform-0.1/cores/const/custom_exception/custom_exception.py` & `dale-core-platform-0.2/cores/const/custom_exception/custom_exception.py`

 * *Files identical despite different names*

### Comparing `dale-core-platform-0.1/cores/const/mobile/command_const.py` & `dale-core-platform-0.2/cores/const/mobile/command_const.py`

 * *Files identical despite different names*

### Comparing `dale-core-platform-0.1/cores/decorators/handle_exception.py` & `dale-core-platform-0.2/cores/decorators/handle_exception.py`

 * *Files identical despite different names*

### Comparing `dale-core-platform-0.1/cores/decorators/parse_config.py` & `dale-core-platform-0.2/cores/decorators/parse_config.py`

 * *Files identical despite different names*

### Comparing `dale-core-platform-0.1/cores/decorators/retry.py` & `dale-core-platform-0.2/cores/decorators/retry.py`

 * *Files identical despite different names*

### Comparing `dale-core-platform-0.1/cores/factory/database_factory/database_conn_generator.py` & `dale-core-platform-0.2/cores/factory/database_factory/database_conn_generator.py`

 * *Files identical despite different names*

### Comparing `dale-core-platform-0.1/cores/factory/database_factory/database_factory.py` & `dale-core-platform-0.2/cores/factory/database_factory/database_factory.py`

 * *Files identical despite different names*

### Comparing `dale-core-platform-0.1/cores/factory/driver_factory/appium/appium_actions.py` & `dale-core-platform-0.2/cores/factory/driver_factory/appium/appium_actions.py`

 * *Files identical despite different names*

### Comparing `dale-core-platform-0.1/cores/factory/driver_factory/appium/appium_server.py` & `dale-core-platform-0.2/cores/factory/driver_factory/appium/appium_server.py`

 * *Files identical despite different names*

### Comparing `dale-core-platform-0.1/cores/factory/driver_factory/appium/application_helper.py` & `dale-core-platform-0.2/cores/factory/driver_factory/appium/application_helper.py`

 * *Files identical despite different names*

### Comparing `dale-core-platform-0.1/cores/factory/driver_factory/appium/mobile_driver.py` & `dale-core-platform-0.2/cores/factory/driver_factory/appium/mobile_driver.py`

 * *Files identical despite different names*

### Comparing `dale-core-platform-0.1/cores/factory/driver_factory/appium/virtual_device.py` & `dale-core-platform-0.2/cores/factory/driver_factory/appium/virtual_device.py`

 * *Files identical despite different names*

### Comparing `dale-core-platform-0.1/cores/factory/driver_factory/selenium/locator_modify_util.py` & `dale-core-platform-0.2/cores/factory/driver_factory/selenium/locator_modify_util.py`

 * *Files identical despite different names*

### Comparing `dale-core-platform-0.1/cores/factory/driver_factory/selenium/selenium_actions.py` & `dale-core-platform-0.2/cores/factory/driver_factory/selenium/selenium_actions.py`

 * *Files identical despite different names*

### Comparing `dale-core-platform-0.1/cores/factory/driver_factory/selenium/selenium_driver.py` & `dale-core-platform-0.2/cores/factory/driver_factory/selenium/selenium_driver.py`

 * *Files identical despite different names*

### Comparing `dale-core-platform-0.1/cores/factory/request_factory/base_factory.py` & `dale-core-platform-0.2/cores/factory/request_factory/base_factory.py`

 * *Files identical despite different names*

### Comparing `dale-core-platform-0.1/cores/factory/request_factory/request_generator.py` & `dale-core-platform-0.2/cores/factory/request_factory/request_generator.py`

 * *Files identical despite different names*

### Comparing `dale-core-platform-0.1/cores/model/environment.py` & `dale-core-platform-0.2/cores/model/environment.py`

 * *Files identical despite different names*

### Comparing `dale-core-platform-0.1/cores/model/request.py` & `dale-core-platform-0.2/cores/model/request.py`

 * *Files identical despite different names*

### Comparing `dale-core-platform-0.1/cores/utils/backend/gitlab_util.py` & `dale-core-platform-0.2/cores/utils/backend/gitlab_util.py`

 * *Files identical despite different names*

### Comparing `dale-core-platform-0.1/cores/utils/backend/request_util.py` & `dale-core-platform-0.2/cores/utils/backend/request_util.py`

 * *Files identical despite different names*

### Comparing `dale-core-platform-0.1/cores/utils/backend/swagger_parser_util.py` & `dale-core-platform-0.2/cores/utils/backend/swagger_parser_util.py`

 * *Files identical despite different names*

### Comparing `dale-core-platform-0.1/cores/utils/common/assertion_util.py` & `dale-core-platform-0.2/cores/utils/common/assertion_util.py`

 * *Files identical despite different names*

### Comparing `dale-core-platform-0.1/cores/utils/common/color_util.py` & `dale-core-platform-0.2/cores/utils/common/color_util.py`

 * *Files identical despite different names*

### Comparing `dale-core-platform-0.1/cores/utils/common/csv_util.py` & `dale-core-platform-0.2/cores/utils/common/csv_util.py`

 * *Files identical despite different names*

### Comparing `dale-core-platform-0.1/cores/utils/common/execute_java_file.py` & `dale-core-platform-0.2/cores/utils/common/execute_java_file.py`

 * *Files identical despite different names*

### Comparing `dale-core-platform-0.1/cores/utils/common/json_util.py` & `dale-core-platform-0.2/cores/utils/common/json_util.py`

 * *Files identical despite different names*

### Comparing `dale-core-platform-0.1/cores/utils/common/logger_util.py` & `dale-core-platform-0.2/cores/utils/common/logger_util.py`

 * *Files identical despite different names*

### Comparing `dale-core-platform-0.1/cores/utils/common/path_util.py` & `dale-core-platform-0.2/cores/utils/common/path_util.py`

 * *Files identical despite different names*

### Comparing `dale-core-platform-0.1/cores/utils/common/prepare_fake_data.py` & `dale-core-platform-0.2/cores/utils/common/prepare_fake_data.py`

 * *Files identical despite different names*

### Comparing `dale-core-platform-0.1/cores/utils/common/store_util.py` & `dale-core-platform-0.2/cores/utils/common/store_util.py`

 * *Files identical despite different names*

### Comparing `dale-core-platform-0.1/cores/utils/common/string_util.py` & `dale-core-platform-0.2/cores/utils/common/string_util.py`

 * *Files identical despite different names*

### Comparing `dale-core-platform-0.1/cores/utils/common/time_util.py` & `dale-core-platform-0.2/cores/utils/common/time_util.py`

 * *Files identical despite different names*

### Comparing `dale-core-platform-0.1/cores/utils/perf/selenium_headless_locust/core.py` & `dale-core-platform-0.2/cores/utils/perf/selenium_headless_locust/core.py`

 * *Files identical despite different names*

### Comparing `dale-core-platform-0.1/cores/utils/perf/selenium_headless_locust/locusts.py` & `dale-core-platform-0.2/cores/utils/perf/selenium_headless_locust/locusts.py`

 * *Files identical despite different names*

### Comparing `dale-core-platform-0.1/cores/utils/testlink/add_remove_test_case.py` & `dale-core-platform-0.2/cores/utils/testlink/add_remove_test_case.py`

 * *Files identical despite different names*

### Comparing `dale-core-platform-0.1/cores/utils/testlink/base_test_link.py` & `dale-core-platform-0.2/cores/utils/testlink/base_test_link.py`

 * *Files identical despite different names*

### Comparing `dale-core-platform-0.1/cores/utils/testlink/create_new_build.py` & `dale-core-platform-0.2/cores/utils/testlink/create_new_build.py`

 * *Files identical despite different names*

### Comparing `dale-core-platform-0.1/cores/utils/testlink/set_test_case_result.py` & `dale-core-platform-0.2/cores/utils/testlink/set_test_case_result.py`

 * *Files identical despite different names*

### Comparing `dale-core-platform-0.1/cores/utils/testlink/test_plan_management.py` & `dale-core-platform-0.2/cores/utils/testlink/test_plan_management.py`

 * *Files identical despite different names*

### Comparing `dale-core-platform-0.1/dale_core_platform.egg-info/PKG-INFO` & `dale-core-platform-0.2/dale_core_platform.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: dale-core-platform
-Version: 0.1
-Summary: This package will include all the libs and helpers which built on Gauge framework. Support Selenim for web, Appium for Mobile, Requests for api and Locust for performance.
+Version: 0.2
+Summary: This package will include all the libs and helpers which built on Gauge framework. Support Selenium for web, Appium for Mobile, Requests for api and Locust for performance.
 Author: Dale Hoang
 Author-email: huy.quochoang2308@gmail.com
 License-File: LICENSE
-Requires-Dist: requests>=2.31
-Requires-Dist: colorlog>=6.7
-Requires-Dist: pydantic>=2.4.2
-Requires-Dist: behave>=1.2.6
-Requires-Dist: behavex>=3.0.0
-Requires-Dist: requests-to-curl>=1.1
-Requires-Dist: mysql-connector-python>=8.0.30
-Requires-Dist: pymongo>=4.2.0
-Requires-Dist: redis>=4.3.4
-Requires-Dist: psycopg2-binary>=2.9.7
-Requires-Dist: locust>=2.16.1
-Requires-Dist: python-gitlab>=3.15.0
-Requires-Dist: webdriver_manager>=4.0.1
-Requires-Dist: selenium==4.4.3
-Requires-Dist: Appium-Python-Client==2.9.0
-Requires-Dist: dataclasses-json>=0.6.2
-Requires-Dist: Faker==19.6.2
-Requires-Dist: TestLink-API-Python-client>=0.8.1
-Requires-Dist: getgauge>=0.4.0
+Requires-Dist: requests==2.31
+Requires-Dist: colorlog==6.7
+Requires-Dist: pydantic==2.4.2
+Requires-Dist: behave==1.2.6
+Requires-Dist: behavex==3.0.0
+Requires-Dist: requests-to-curl==1.1
+Requires-Dist: mysql-connector-python==8.0.30
+Requires-Dist: pymongo==4.2.0
+Requires-Dist: redis==4.3.4
+Requires-Dist: psycopg2-binary==2.9.7
+Requires-Dist: locust==2.16.1
+Requires-Dist: python-gitlab==3.15.0
+Requires-Dist: webdriver_manager==4.0.1
+Requires-Dist: selenium====4.4.3
+Requires-Dist: Appium-Python-Client====2.9.0
+Requires-Dist: dataclasses-json==0.6.2
+Requires-Dist: Faker====19.6.2
+Requires-Dist: TestLink-API-Python-client==0.8.1
+Requires-Dist: getgauge==0.4.0
```

### Comparing `dale-core-platform-0.1/dale_core_platform.egg-info/SOURCES.txt` & `dale-core-platform-0.2/dale_core_platform.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dale-core-platform-0.1/setup.py` & `dale-core-platform-0.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 from setuptools import setup, find_packages
 
 setup(
     name='dale-core-platform',
-    version='0.1',
+    version='0.2',
     packages=find_packages(),
-    description="This package will include all the libs and helpers which built on Gauge framework. Support Selenim for web, Appium for Mobile, Requests for api and Locust for performance.",
+    description="This package will include all the libs and helpers which built on Gauge framework. Support Selenium for web, Appium for Mobile, Requests for api and Locust for performance.",
     author='Dale Hoang',
     author_email='huy.quochoang2308@gmail.com',
     install_requires=[
-        'requests>=2.31',
-        'colorlog>=6.7',
-        'pydantic>=2.4.2',
-        'behave>=1.2.6',
-        'behavex>=3.0.0',
-        'requests-to-curl>=1.1',
-        'mysql-connector-python>=8.0.30',
-        'pymongo>=4.2.0',
-        'redis>=4.3.4',
-        'psycopg2-binary>=2.9.7',
-        'locust>=2.16.1',
-        'python-gitlab>=3.15.0',
-        'webdriver_manager>=4.0.1',
-        'selenium==4.4.3',
-        'Appium-Python-Client==2.9.0',
-        'dataclasses-json>=0.6.2',
-        'Faker==19.6.2',
-        'TestLink-API-Python-client>=0.8.1',
-        'getgauge>=0.4.0'
+        'requests==2.31',
+        'colorlog==6.7',
+        'pydantic==2.4.2',
+        'behave==1.2.6',
+        'behavex==3.0.0',
+        'requests-to-curl==1.1',
+        'mysql-connector-python==8.0.30',
+        'pymongo==4.2.0',
+        'redis==4.3.4',
+        'psycopg2-binary==2.9.7',
+        'locust==2.16.1',
+        'python-gitlab==3.15.0',
+        'webdriver_manager==4.0.1',
+        'selenium====4.4.3',
+        'Appium-Python-Client====2.9.0',
+        'dataclasses-json==0.6.2',
+        'Faker====19.6.2',
+        'TestLink-API-Python-client==0.8.1',
+        'getgauge==0.4.0'
     ],
 )
```

