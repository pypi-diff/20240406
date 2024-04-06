# Comparing `tmp/statesxt-0.5.7.tar.gz` & `tmp/statesxt-0.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "statesxt-0.5.7.tar", last modified: Wed Mar 20 13:45:47 2024, max compression
+gzip compressed data, was "statesxt-0.5.8.tar", last modified: Sat Apr  6 03:31:22 2024, max compression
```

## Comparing `statesxt-0.5.7.tar` & `statesxt-0.5.8.tar`

### file list

```diff
@@ -1,112 +1,112 @@
-drwxrwxrwx   0        0        0        0 2024-03-20 13:45:47.293215 statesxt-0.5.7/
--rw-rw-rw-   0        0        0       45 2024-02-29 16:14:01.000000 statesxt-0.5.7/.env.template
-drwxrwxrwx   0        0        0        0 2024-03-20 13:45:46.882669 statesxt-0.5.7/.github/
-drwxrwxrwx   0        0        0        0 2024-03-20 13:45:46.934549 statesxt-0.5.7/.github/workflows/
--rw-rw-rw-   0        0        0      595 2024-02-10 17:10:42.000000 statesxt-0.5.7/.github/workflows/test.yml
--rw-rw-rw-   0        0        0     4420 2024-03-11 09:38:40.000000 statesxt-0.5.7/.gitignore
--rw-rw-rw-   0        0        0      211 2024-01-11 08:44:43.000000 statesxt-0.5.7/.readthedocs.yaml
--rw-rw-rw-   0        0        0     1068 2024-01-06 09:36:25.000000 statesxt-0.5.7/LICENSE
--rw-rw-rw-   0        0        0     3296 2024-03-20 13:45:47.293215 statesxt-0.5.7/PKG-INFO
--rw-rw-rw-   0        0        0     2370 2024-03-12 03:02:11.000000 statesxt-0.5.7/README.md
--rwxrwxrwx   0        0        0     1042 2024-02-29 16:09:09.000000 statesxt-0.5.7/publish.bat
--rw-rw-rw-   0        0        0       42 2024-03-20 13:45:47.297249 statesxt-0.5.7/setup.cfg
--rw-rw-rw-   0        0        0     1354 2024-03-20 12:02:09.000000 statesxt-0.5.7/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-20 13:45:46.977105 statesxt-0.5.7/statesxt/
--rw-rw-rw-   0        0        0     2066 2024-02-13 03:17:19.000000 statesxt-0.5.7/statesxt/.env.template
-drwxrwxrwx   0        0        0        0 2024-03-20 13:45:46.882669 statesxt-0.5.7/statesxt/.github/
-drwxrwxrwx   0        0        0        0 2024-03-20 13:45:47.009404 statesxt-0.5.7/statesxt/.github/workflows/
--rw-rw-rw-   0        0        0      555 2024-03-11 08:09:16.000000 statesxt-0.5.7/statesxt/.github/workflows/test.yml
--rw-rw-rw-   0        0        0     3970 2024-02-13 03:16:33.000000 statesxt-0.5.7/statesxt/.gitignore
--rw-rw-rw-   0        0        0       37 2024-01-30 14:55:47.000000 statesxt-0.5.7/statesxt/README.md
--rw-rw-rw-   0        0        0        0 2024-01-10 13:51:23.000000 statesxt-0.5.7/statesxt/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-20 13:45:47.020060 statesxt-0.5.7/statesxt/base/
--rw-rw-rw-   0        0        0        0 2024-02-21 19:19:24.000000 statesxt-0.5.7/statesxt/base/__init__.py
--rw-rw-rw-   0        0        0     3582 2024-03-20 13:11:35.000000 statesxt-0.5.7/statesxt/base/base_driver.py
--rw-rw-rw-   0        0        0     3879 2024-03-11 08:18:05.000000 statesxt-0.5.7/statesxt/base/check.py
--rw-rw-rw-   0        0        0     7945 2024-03-16 03:36:14.000000 statesxt-0.5.7/statesxt/base/form.py
--rw-rw-rw-   0        0        0     5896 2024-03-20 12:28:09.000000 statesxt-0.5.7/statesxt/base/mouse_keys.py
--rw-rw-rw-   0        0        0     2993 2024-03-11 08:27:55.000000 statesxt-0.5.7/statesxt/base/table.py
--rw-rw-rw-   0        0        0     3519 2024-03-11 10:22:39.000000 statesxt-0.5.7/statesxt/base/wait.py
-drwxrwxrwx   0        0        0        0 2024-03-20 13:45:47.030194 statesxt-0.5.7/statesxt/database/
--rw-rw-rw-   0        0        0        0 2024-01-10 13:51:23.000000 statesxt-0.5.7/statesxt/database/__init__.py
--rw-rw-rw-   0        0        0     3595 2024-02-10 16:40:54.000000 statesxt-0.5.7/statesxt/database/database.py
-drwxrwxrwx   0        0        0        0 2024-03-20 13:45:47.043161 statesxt-0.5.7/statesxt/database/mocks/
--rw-rw-rw-   0        0        0      201 2024-03-11 05:34:22.000000 statesxt-0.5.7/statesxt/database/mocks/mock_login_invalid.json
--rw-rw-rw-   0        0        0      345 2024-03-11 05:34:22.000000 statesxt-0.5.7/statesxt/database/mocks/mock_login_valid.json
--rw-rw-rw-   0        0        0      273 2024-02-10 13:46:29.000000 statesxt-0.5.7/statesxt/database/queries.py
--rw-rw-rw-   0        0        0     1585 2024-02-10 13:46:29.000000 statesxt-0.5.7/statesxt/database/service.py
-drwxrwxrwx   0        0        0        0 2024-03-20 13:45:47.088067 statesxt-0.5.7/statesxt/docs/
--rw-rw-rw-   0        0        0      634 2024-01-10 13:51:23.000000 statesxt-0.5.7/statesxt/docs/Makefile
-drwxrwxrwx   0        0        0        0 2024-03-20 13:45:46.891762 statesxt-0.5.7/statesxt/docs/_static/
-drwxrwxrwx   0        0        0        0 2024-03-20 13:45:47.088067 statesxt-0.5.7/statesxt/docs/_static/css/
--rw-rw-rw-   0        0        0       47 2024-01-16 16:04:21.000000 statesxt-0.5.7/statesxt/docs/_static/css/custom.css
-drwxrwxrwx   0        0        0        0 2024-03-20 13:45:47.105229 statesxt-0.5.7/statesxt/docs/_static/images/
--rw-rw-rw-   0        0        0    15068 2024-01-30 01:18:07.000000 statesxt-0.5.7/statesxt/docs/_static/images/structure-en.png
--rw-rw-rw-   0        0        0    97392 2024-01-16 16:04:21.000000 statesxt-0.5.7/statesxt/docs/_static/images/uml-base.png
--rw-rw-rw-   0        0        0    31754 2024-01-30 01:45:13.000000 statesxt-0.5.7/statesxt/docs/_static/images/uml-framework-states.png
--rw-rw-rw-   0        0        0   479475 2024-01-16 16:04:21.000000 statesxt-0.5.7/statesxt/docs/_static/images/uml-framework.png
--rw-rw-rw-   0        0        0     1043 2024-01-16 16:04:21.000000 statesxt-0.5.7/statesxt/docs/conf.py
-drwxrwxrwx   0        0        0        0 2024-03-20 13:45:47.245823 statesxt-0.5.7/statesxt/docs/contents/
--rw-rw-rw-   0        0        0      589 2024-02-05 06:02:51.000000 statesxt-0.5.7/statesxt/docs/contents/README-md.rst
--rw-rw-rw-   0        0        0    34449 2024-02-05 05:47:40.000000 statesxt-0.5.7/statesxt/docs/contents/base.rst
--rw-rw-rw-   0        0        0      217 2024-02-05 05:47:53.000000 statesxt-0.5.7/statesxt/docs/contents/database.rst
--rw-rw-rw-   0        0        0     4854 2024-01-22 08:16:49.000000 statesxt-0.5.7/statesxt/docs/contents/env_template.rst
--rw-rw-rw-   0        0        0      619 2024-02-05 05:54:09.000000 statesxt-0.5.7/statesxt/docs/contents/gitignore.rst
--rw-rw-rw-   0        0        0     8018 2024-01-30 04:34:33.000000 statesxt-0.5.7/statesxt/docs/contents/introduction.rst
--rw-rw-rw-   0        0        0     2857 2024-01-22 08:18:41.000000 statesxt-0.5.7/statesxt/docs/contents/locators.rst
--rw-rw-rw-   0        0        0     3432 2024-01-22 08:18:24.000000 statesxt-0.5.7/statesxt/docs/contents/pages.rst
--rw-rw-rw-   0        0        0      750 2024-02-05 05:58:35.000000 statesxt-0.5.7/statesxt/docs/contents/poetry-lock.rst
--rw-rw-rw-   0        0        0      695 2024-02-05 05:59:49.000000 statesxt-0.5.7/statesxt/docs/contents/pyproject-toml.rst
--rw-rw-rw-   0        0        0     1886 2024-02-05 06:06:32.000000 statesxt-0.5.7/statesxt/docs/contents/pytest-ini.rst
--rw-rw-rw-   0        0        0     2051 2024-02-05 05:48:14.000000 statesxt-0.5.7/statesxt/docs/contents/quick_start.rst
--rw-rw-rw-   0        0        0    20029 2024-02-13 03:17:53.000000 statesxt-0.5.7/statesxt/docs/contents/testcases.rst
--rw-rw-rw-   0        0        0    26529 2024-02-15 09:55:59.000000 statesxt-0.5.7/statesxt/docs/contents/utils.rst
--rw-rw-rw-   0        0        0      714 2024-02-05 06:06:38.000000 statesxt-0.5.7/statesxt/docs/index.rst
--rwxrwxrwx   0        0        0      765 2024-01-10 13:51:23.000000 statesxt-0.5.7/statesxt/docs/make.bat
--rw-rw-rw-   0        0        0     1060 2024-01-11 08:44:43.000000 statesxt-0.5.7/statesxt/docs/requirements.txt
--rw-rw-rw-   0        0        0    14402 2024-03-20 12:02:16.000000 statesxt-0.5.7/statesxt/main.py
--rw-rw-rw-   0        0        0     9579 2024-03-11 09:05:54.000000 statesxt-0.5.7/statesxt/named_ranges.py
--rw-rw-rw-   0        0        0     1972 2024-02-21 19:19:18.000000 statesxt-0.5.7/statesxt/pyproject.toml
--rw-rw-rw-   0        0        0      117 2024-01-30 14:56:01.000000 statesxt-0.5.7/statesxt/pytest.ini
--rw-rw-rw-   0        0        0      748 2024-03-11 09:08:50.000000 statesxt-0.5.7/statesxt/restate.py
--rw-rw-rw-   0        0        0        0 2024-02-12 14:18:13.000000 statesxt-0.5.7/statesxt/results.json
-drwxrwxrwx   0        0        0        0 2024-03-20 13:45:47.254364 statesxt-0.5.7/statesxt/template/
--rw-rw-rw-   0        0        0        0 2024-02-12 12:50:29.000000 statesxt-0.5.7/statesxt/template/__init__.py
--rw-rw-rw-   0        0        0      374 2024-03-11 08:35:46.000000 statesxt-0.5.7/statesxt/template/interface.py
--rw-rw-rw-   0        0        0      418 2024-03-14 04:57:21.000000 statesxt-0.5.7/statesxt/template/locator.py
--rw-rw-rw-   0        0        0      876 2024-03-20 12:04:42.000000 statesxt-0.5.7/statesxt/template/page.py
-drwxrwxrwx   0        0        0        0 2024-03-20 13:45:47.254364 statesxt-0.5.7/statesxt/template/scenarios/
--rw-rw-rw-   0        0        0      310 2024-02-12 12:59:15.000000 statesxt-0.5.7/statesxt/template/scenarios/__init__.py
--rw-rw-rw-   0        0        0      543 2024-03-11 08:38:14.000000 statesxt-0.5.7/statesxt/template/scenarios/test_0_1.py
-drwxrwxrwx   0        0        0        0 2024-03-20 13:45:47.254364 statesxt-0.5.7/statesxt/template/states/
--rw-rw-rw-   0        0        0        0 2024-01-10 13:51:23.000000 statesxt-0.5.7/statesxt/template/states/__init__.py
--rw-rw-rw-   0        0        0      427 2024-03-14 04:57:09.000000 statesxt-0.5.7/statesxt/template/states/states_0_1.py
-drwxrwxrwx   0        0        0        0 2024-03-20 13:45:47.261544 statesxt-0.5.7/statesxt/testcases/
--rw-rw-rw-   0        0        0     1404 2024-03-12 02:06:36.000000 statesxt-0.5.7/statesxt/testcases/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-20 13:45:47.270182 statesxt-0.5.7/statesxt/testcases/_fixtures/
--rw-rw-rw-   0        0        0        0 2024-03-11 09:40:26.000000 statesxt-0.5.7/statesxt/testcases/_fixtures/__init__.py
--rw-rw-rw-   0        0        0      668 2024-03-12 04:17:10.000000 statesxt-0.5.7/statesxt/testcases/_fixtures/auth.py
--rw-rw-rw-   0        0        0     1333 2024-03-11 09:40:21.000000 statesxt-0.5.7/statesxt/testcases/_fixtures/composition.py
--rw-rw-rw-   0        0        0     1428 2024-03-11 09:40:20.000000 statesxt-0.5.7/statesxt/testcases/_fixtures/option.py
--rw-rw-rw-   0        0        0     1045 2024-03-12 04:27:48.000000 statesxt-0.5.7/statesxt/testcases/_fixtures/param.py
--rw-rw-rw-   0        0        0      691 2024-03-11 09:07:55.000000 statesxt-0.5.7/statesxt/testcases/conftest.py
--rw-rw-rw-   0        0        0      416 2024-02-12 14:10:26.000000 statesxt-0.5.7/statesxt/tox.ini
-drwxrwxrwx   0        0        0        0 2024-03-20 13:45:47.291680 statesxt-0.5.7/statesxt/utils/
--rw-rw-rw-   0        0        0        0 2024-02-21 19:19:40.000000 statesxt-0.5.7/statesxt/utils/__init__.py
--rw-rw-rw-   0        0        0      353 2024-03-11 08:57:51.000000 statesxt-0.5.7/statesxt/utils/crypter.py
--rw-rw-rw-   0        0        0     3586 2024-03-11 08:58:52.000000 statesxt-0.5.7/statesxt/utils/email.py
--rw-rw-rw-   0        0        0      453 2024-03-11 05:41:49.000000 statesxt-0.5.7/statesxt/utils/explicit_wait.py
--rw-rw-rw-   0        0        0      401 2024-03-11 08:59:43.000000 statesxt-0.5.7/statesxt/utils/faker.py
--rw-rw-rw-   0        0        0      331 2024-03-11 08:59:56.000000 statesxt-0.5.7/statesxt/utils/file_opener.py
--rw-rw-rw-   0        0        0     3103 2024-03-11 09:00:11.000000 statesxt-0.5.7/statesxt/utils/formatter.py
--rw-rw-rw-   0        0        0     1567 2024-03-11 09:02:41.000000 statesxt-0.5.7/statesxt/utils/logger.py
--rw-rw-rw-   0        0        0      771 2024-03-11 09:03:01.000000 statesxt-0.5.7/statesxt/utils/response_handler.py
--rw-rw-rw-   0        0        0     6079 2024-03-11 09:07:23.000000 statesxt-0.5.7/statesxt/utils/service_account.py
--rw-rw-rw-   0        0        0     1563 2024-03-11 07:27:19.000000 statesxt-0.5.7/statesxt/utils/store.py
--rw-rw-rw-   0        0        0     4705 2024-03-11 09:03:50.000000 statesxt-0.5.7/statesxt/utils/wrapper.py
-drwxrwxrwx   0        0        0        0 2024-03-20 13:45:47.293215 statesxt-0.5.7/statesxt.egg-info/
--rw-rw-rw-   0        0        0     3296 2024-03-20 13:45:46.000000 statesxt-0.5.7/statesxt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2656 2024-03-20 13:45:46.000000 statesxt-0.5.7/statesxt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-20 13:45:46.000000 statesxt-0.5.7/statesxt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2024-03-20 13:45:46.000000 statesxt-0.5.7/statesxt.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        9 2024-03-20 13:45:46.000000 statesxt-0.5.7/statesxt.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-06 03:31:22.911111 statesxt-0.5.8/
+-rw-rw-rw-   0        0        0       45 2024-02-29 16:14:01.000000 statesxt-0.5.8/.env.template
+drwxrwxrwx   0        0        0        0 2024-04-06 03:31:22.369843 statesxt-0.5.8/.github/
+drwxrwxrwx   0        0        0        0 2024-04-06 03:31:22.417051 statesxt-0.5.8/.github/workflows/
+-rw-rw-rw-   0        0        0      595 2024-02-10 17:10:42.000000 statesxt-0.5.8/.github/workflows/test.yml
+-rw-rw-rw-   0        0        0     4420 2024-03-11 09:38:40.000000 statesxt-0.5.8/.gitignore
+-rw-rw-rw-   0        0        0      211 2024-01-11 08:44:43.000000 statesxt-0.5.8/.readthedocs.yaml
+-rw-rw-rw-   0        0        0     1068 2024-01-06 09:36:25.000000 statesxt-0.5.8/LICENSE
+-rw-rw-rw-   0        0        0     3296 2024-04-06 03:31:22.908089 statesxt-0.5.8/PKG-INFO
+-rw-rw-rw-   0        0        0     2370 2024-03-12 03:02:11.000000 statesxt-0.5.8/README.md
+-rwxrwxrwx   0        0        0     1042 2024-02-29 16:09:09.000000 statesxt-0.5.8/publish.bat
+-rw-rw-rw-   0        0        0       42 2024-04-06 03:31:22.911111 statesxt-0.5.8/setup.cfg
+-rw-rw-rw-   0        0        0     1354 2024-03-21 16:41:04.000000 statesxt-0.5.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-06 03:31:22.457653 statesxt-0.5.8/statesxt/
+-rw-rw-rw-   0        0        0     2066 2024-02-13 03:17:19.000000 statesxt-0.5.8/statesxt/.env.template
+drwxrwxrwx   0        0        0        0 2024-04-06 03:31:22.371965 statesxt-0.5.8/statesxt/.github/
+drwxrwxrwx   0        0        0        0 2024-04-06 03:31:22.503630 statesxt-0.5.8/statesxt/.github/workflows/
+-rw-rw-rw-   0        0        0      555 2024-03-11 08:09:16.000000 statesxt-0.5.8/statesxt/.github/workflows/test.yml
+-rw-rw-rw-   0        0        0     3970 2024-02-13 03:16:33.000000 statesxt-0.5.8/statesxt/.gitignore
+-rw-rw-rw-   0        0        0       37 2024-01-30 14:55:47.000000 statesxt-0.5.8/statesxt/README.md
+-rw-rw-rw-   0        0        0        0 2024-01-10 13:51:23.000000 statesxt-0.5.8/statesxt/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-06 03:31:22.519218 statesxt-0.5.8/statesxt/base/
+-rw-rw-rw-   0        0        0        0 2024-03-21 16:17:37.000000 statesxt-0.5.8/statesxt/base/__init__.py
+-rw-rw-rw-   0        0        0     3582 2024-04-06 03:24:33.000000 statesxt-0.5.8/statesxt/base/base_driver.py
+-rw-rw-rw-   0        0        0     3872 2024-04-04 01:27:04.000000 statesxt-0.5.8/statesxt/base/check.py
+-rw-rw-rw-   0        0        0     8057 2024-04-06 02:38:40.000000 statesxt-0.5.8/statesxt/base/form.py
+-rw-rw-rw-   0        0        0     5945 2024-04-06 03:24:41.000000 statesxt-0.5.8/statesxt/base/mouse_keys.py
+-rw-rw-rw-   0        0        0     2993 2024-03-21 16:17:37.000000 statesxt-0.5.8/statesxt/base/table.py
+-rw-rw-rw-   0        0        0     4119 2024-04-06 03:24:53.000000 statesxt-0.5.8/statesxt/base/wait.py
+drwxrwxrwx   0        0        0        0 2024-04-06 03:31:22.527506 statesxt-0.5.8/statesxt/database/
+-rw-rw-rw-   0        0        0        0 2024-01-10 13:51:23.000000 statesxt-0.5.8/statesxt/database/__init__.py
+-rw-rw-rw-   0        0        0     3595 2024-02-10 16:40:54.000000 statesxt-0.5.8/statesxt/database/database.py
+drwxrwxrwx   0        0        0        0 2024-04-06 03:31:22.550413 statesxt-0.5.8/statesxt/database/mocks/
+-rw-rw-rw-   0        0        0      201 2024-03-11 05:34:22.000000 statesxt-0.5.8/statesxt/database/mocks/mock_login_invalid.json
+-rw-rw-rw-   0        0        0      345 2024-03-11 05:34:22.000000 statesxt-0.5.8/statesxt/database/mocks/mock_login_valid.json
+-rw-rw-rw-   0        0        0      273 2024-02-10 13:46:29.000000 statesxt-0.5.8/statesxt/database/queries.py
+-rw-rw-rw-   0        0        0     1585 2024-02-10 13:46:29.000000 statesxt-0.5.8/statesxt/database/service.py
+drwxrwxrwx   0        0        0        0 2024-04-06 03:31:22.608187 statesxt-0.5.8/statesxt/docs/
+-rw-rw-rw-   0        0        0      634 2024-01-10 13:51:23.000000 statesxt-0.5.8/statesxt/docs/Makefile
+drwxrwxrwx   0        0        0        0 2024-04-06 03:31:22.378072 statesxt-0.5.8/statesxt/docs/_static/
+drwxrwxrwx   0        0        0        0 2024-04-06 03:31:22.610148 statesxt-0.5.8/statesxt/docs/_static/css/
+-rw-rw-rw-   0        0        0       47 2024-01-16 16:04:21.000000 statesxt-0.5.8/statesxt/docs/_static/css/custom.css
+drwxrwxrwx   0        0        0        0 2024-04-06 03:31:22.641326 statesxt-0.5.8/statesxt/docs/_static/images/
+-rw-rw-rw-   0        0        0    15068 2024-01-30 01:18:07.000000 statesxt-0.5.8/statesxt/docs/_static/images/structure-en.png
+-rw-rw-rw-   0        0        0    97392 2024-01-16 16:04:21.000000 statesxt-0.5.8/statesxt/docs/_static/images/uml-base.png
+-rw-rw-rw-   0        0        0    31754 2024-01-30 01:45:13.000000 statesxt-0.5.8/statesxt/docs/_static/images/uml-framework-states.png
+-rw-rw-rw-   0        0        0   479475 2024-01-16 16:04:21.000000 statesxt-0.5.8/statesxt/docs/_static/images/uml-framework.png
+-rw-rw-rw-   0        0        0     1043 2024-01-16 16:04:21.000000 statesxt-0.5.8/statesxt/docs/conf.py
+drwxrwxrwx   0        0        0        0 2024-04-06 03:31:22.841607 statesxt-0.5.8/statesxt/docs/contents/
+-rw-rw-rw-   0        0        0      589 2024-02-05 06:02:51.000000 statesxt-0.5.8/statesxt/docs/contents/README-md.rst
+-rw-rw-rw-   0        0        0    34449 2024-02-05 05:47:40.000000 statesxt-0.5.8/statesxt/docs/contents/base.rst
+-rw-rw-rw-   0        0        0      217 2024-02-05 05:47:53.000000 statesxt-0.5.8/statesxt/docs/contents/database.rst
+-rw-rw-rw-   0        0        0     4854 2024-01-22 08:16:49.000000 statesxt-0.5.8/statesxt/docs/contents/env_template.rst
+-rw-rw-rw-   0        0        0      619 2024-02-05 05:54:09.000000 statesxt-0.5.8/statesxt/docs/contents/gitignore.rst
+-rw-rw-rw-   0        0        0     8018 2024-01-30 04:34:33.000000 statesxt-0.5.8/statesxt/docs/contents/introduction.rst
+-rw-rw-rw-   0        0        0     2857 2024-01-22 08:18:41.000000 statesxt-0.5.8/statesxt/docs/contents/locators.rst
+-rw-rw-rw-   0        0        0     3432 2024-01-22 08:18:24.000000 statesxt-0.5.8/statesxt/docs/contents/pages.rst
+-rw-rw-rw-   0        0        0      750 2024-02-05 05:58:35.000000 statesxt-0.5.8/statesxt/docs/contents/poetry-lock.rst
+-rw-rw-rw-   0        0        0      695 2024-02-05 05:59:49.000000 statesxt-0.5.8/statesxt/docs/contents/pyproject-toml.rst
+-rw-rw-rw-   0        0        0     1886 2024-02-05 06:06:32.000000 statesxt-0.5.8/statesxt/docs/contents/pytest-ini.rst
+-rw-rw-rw-   0        0        0     2051 2024-02-05 05:48:14.000000 statesxt-0.5.8/statesxt/docs/contents/quick_start.rst
+-rw-rw-rw-   0        0        0    20029 2024-02-13 03:17:53.000000 statesxt-0.5.8/statesxt/docs/contents/testcases.rst
+-rw-rw-rw-   0        0        0    26529 2024-02-15 09:55:59.000000 statesxt-0.5.8/statesxt/docs/contents/utils.rst
+-rw-rw-rw-   0        0        0      714 2024-02-05 06:06:38.000000 statesxt-0.5.8/statesxt/docs/index.rst
+-rwxrwxrwx   0        0        0      765 2024-01-10 13:51:23.000000 statesxt-0.5.8/statesxt/docs/make.bat
+-rw-rw-rw-   0        0        0     1060 2024-01-11 08:44:43.000000 statesxt-0.5.8/statesxt/docs/requirements.txt
+-rw-rw-rw-   0        0        0    14402 2024-03-21 16:41:12.000000 statesxt-0.5.8/statesxt/main.py
+-rw-rw-rw-   0        0        0     9579 2024-03-11 09:05:54.000000 statesxt-0.5.8/statesxt/named_ranges.py
+-rw-rw-rw-   0        0        0     1972 2024-02-21 19:19:18.000000 statesxt-0.5.8/statesxt/pyproject.toml
+-rw-rw-rw-   0        0        0      117 2024-01-30 14:56:01.000000 statesxt-0.5.8/statesxt/pytest.ini
+-rw-rw-rw-   0        0        0      748 2024-03-11 09:08:50.000000 statesxt-0.5.8/statesxt/restate.py
+-rw-rw-rw-   0        0        0        0 2024-02-12 14:18:13.000000 statesxt-0.5.8/statesxt/results.json
+drwxrwxrwx   0        0        0        0 2024-04-06 03:31:22.851308 statesxt-0.5.8/statesxt/template/
+-rw-rw-rw-   0        0        0        0 2024-02-12 12:50:29.000000 statesxt-0.5.8/statesxt/template/__init__.py
+-rw-rw-rw-   0        0        0      373 2024-04-05 05:07:19.000000 statesxt-0.5.8/statesxt/template/interface.py
+-rw-rw-rw-   0        0        0      414 2024-04-05 05:06:23.000000 statesxt-0.5.8/statesxt/template/locator.py
+-rw-rw-rw-   0        0        0     1084 2024-04-05 05:05:58.000000 statesxt-0.5.8/statesxt/template/page.py
+drwxrwxrwx   0        0        0        0 2024-04-06 03:31:22.854645 statesxt-0.5.8/statesxt/template/scenarios/
+-rw-rw-rw-   0        0        0      346 2024-04-05 05:02:10.000000 statesxt-0.5.8/statesxt/template/scenarios/__init__.py
+-rw-rw-rw-   0        0        0      642 2024-04-05 05:05:43.000000 statesxt-0.5.8/statesxt/template/scenarios/test_0_1.py
+drwxrwxrwx   0        0        0        0 2024-04-06 03:31:22.858419 statesxt-0.5.8/statesxt/template/states/
+-rw-rw-rw-   0        0        0       32 2024-04-05 04:54:55.000000 statesxt-0.5.8/statesxt/template/states/__init__.py
+-rw-rw-rw-   0        0        0      424 2024-04-05 05:07:15.000000 statesxt-0.5.8/statesxt/template/states/states_0_1.py
+drwxrwxrwx   0        0        0        0 2024-04-06 03:31:22.863306 statesxt-0.5.8/statesxt/testcases/
+-rw-rw-rw-   0        0        0     2058 2024-04-06 03:28:56.000000 statesxt-0.5.8/statesxt/testcases/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-06 03:31:22.877187 statesxt-0.5.8/statesxt/testcases/_fixtures/
+-rw-rw-rw-   0        0        0        0 2024-03-21 16:17:37.000000 statesxt-0.5.8/statesxt/testcases/_fixtures/__init__.py
+-rw-rw-rw-   0        0        0      668 2024-03-21 16:17:37.000000 statesxt-0.5.8/statesxt/testcases/_fixtures/auth.py
+-rw-rw-rw-   0        0        0     1333 2024-03-21 16:17:37.000000 statesxt-0.5.8/statesxt/testcases/_fixtures/composition.py
+-rw-rw-rw-   0        0        0     1428 2024-04-06 03:26:27.000000 statesxt-0.5.8/statesxt/testcases/_fixtures/option.py
+-rw-rw-rw-   0        0        0     1045 2024-04-03 03:18:39.000000 statesxt-0.5.8/statesxt/testcases/_fixtures/param.py
+-rw-rw-rw-   0        0        0      691 2024-04-06 03:26:46.000000 statesxt-0.5.8/statesxt/testcases/conftest.py
+-rw-rw-rw-   0        0        0      416 2024-02-12 14:10:26.000000 statesxt-0.5.8/statesxt/tox.ini
+drwxrwxrwx   0        0        0        0 2024-04-06 03:31:22.903564 statesxt-0.5.8/statesxt/utils/
+-rw-rw-rw-   0        0        0        0 2024-03-21 16:17:37.000000 statesxt-0.5.8/statesxt/utils/__init__.py
+-rw-rw-rw-   0        0        0      353 2024-03-21 16:17:37.000000 statesxt-0.5.8/statesxt/utils/crypter.py
+-rw-rw-rw-   0        0        0     3586 2024-03-21 16:17:37.000000 statesxt-0.5.8/statesxt/utils/email.py
+-rw-rw-rw-   0        0        0      624 2024-04-06 03:04:00.000000 statesxt-0.5.8/statesxt/utils/explicit_wait.py
+-rw-rw-rw-   0        0        0      401 2024-03-21 16:17:37.000000 statesxt-0.5.8/statesxt/utils/faker.py
+-rw-rw-rw-   0        0        0      331 2024-03-21 16:17:37.000000 statesxt-0.5.8/statesxt/utils/file_opener.py
+-rw-rw-rw-   0        0        0     3103 2024-03-21 16:17:37.000000 statesxt-0.5.8/statesxt/utils/formatter.py
+-rw-rw-rw-   0        0        0     1567 2024-03-21 16:17:37.000000 statesxt-0.5.8/statesxt/utils/logger.py
+-rw-rw-rw-   0        0        0      771 2024-03-21 16:17:37.000000 statesxt-0.5.8/statesxt/utils/response_handler.py
+-rw-rw-rw-   0        0        0     6079 2024-04-06 03:25:41.000000 statesxt-0.5.8/statesxt/utils/service_account.py
+-rw-rw-rw-   0        0        0     1563 2024-03-21 16:17:37.000000 statesxt-0.5.8/statesxt/utils/store.py
+-rw-rw-rw-   0        0        0     5198 2024-04-02 09:50:07.000000 statesxt-0.5.8/statesxt/utils/wrapper.py
+drwxrwxrwx   0        0        0        0 2024-04-06 03:31:22.905560 statesxt-0.5.8/statesxt.egg-info/
+-rw-rw-rw-   0        0        0     3296 2024-04-06 03:31:22.000000 statesxt-0.5.8/statesxt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2656 2024-04-06 03:31:22.000000 statesxt-0.5.8/statesxt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-06 03:31:22.000000 statesxt-0.5.8/statesxt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2024-04-06 03:31:22.000000 statesxt-0.5.8/statesxt.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        9 2024-04-06 03:31:22.000000 statesxt-0.5.8/statesxt.egg-info/top_level.txt
```

### Comparing `statesxt-0.5.7/.github/workflows/test.yml` & `statesxt-0.5.8/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `statesxt-0.5.7/.gitignore` & `statesxt-0.5.8/.gitignore`

 * *Files identical despite different names*

### Comparing `statesxt-0.5.7/LICENSE` & `statesxt-0.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `statesxt-0.5.7/PKG-INFO` & `statesxt-0.5.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: statesxt
-Version: 0.5.7
+Version: 0.5.8
 Summary: A project template for testing your website application.
 Home-page: https://test.pypi.org/project/statesxt/
 Author: Jason Caleb
 Author-email: cjsonnnnn@gmail.com
 License: MIT License
 Project-URL: Source, https://github.com/jsonnnnn/statesxt
 Project-URL: Documentation, https://statesxt.readthedocs.io/en/latest/
```

### Comparing `statesxt-0.5.7/README.md` & `statesxt-0.5.8/README.md`

 * *Files identical despite different names*

### Comparing `statesxt-0.5.7/publish.bat` & `statesxt-0.5.8/publish.bat`

 * *Files identical despite different names*

### Comparing `statesxt-0.5.7/setup.py` & `statesxt-0.5.8/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", encoding="utf8") as file:
     LONG_DESC = file.read()
 
 setuptools.setup(
     name="statesxt",
-    version="0.5.7",
+    version="0.5.8",
     description="A project template for testing your website application.",
     long_description=LONG_DESC,
     long_description_content_type="text/markdown",
     url="https://test.pypi.org/project/statesxt/",
     author="Jason Caleb",
     author_email="cjsonnnnn@gmail.com",
     license="MIT License",
```

### Comparing `statesxt-0.5.7/statesxt/.env.template` & `statesxt-0.5.8/statesxt/.env.template`

 * *Files identical despite different names*

### Comparing `statesxt-0.5.7/statesxt/.github/workflows/test.yml` & `statesxt-0.5.8/statesxt/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `statesxt-0.5.7/statesxt/.gitignore` & `statesxt-0.5.8/statesxt/.gitignore`

 * *Files identical despite different names*

### Comparing `statesxt-0.5.7/statesxt/base/base_driver.py` & `statesxt-0.5.8/statesxt/base/base_driver.py`

 * *Files identical despite different names*

### Comparing `statesxt-0.5.7/statesxt/base/check.py` & `statesxt-0.5.8/statesxt/base/check.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,25 +25,25 @@
             cust_message (str): is a custom message, which other than both 'success' and 'fail'
 
         Returns:
             bool: True means that the element is found, and vice versa
         """
 
         if isVisible:
-            eAlert = self.wd.an_element(By.CLASS_NAME, "toast-body")
+            alert = self.wd.an_element(By.CLASS_NAME, "toast-body")
             if isSuccess:
-                if eAlert.text == "success" or eAlert.text == cust_message:
+                if alert.text == "success" or alert.text == cust_message:
                     return True
             else:
-                if eAlert.text == "fail" or eAlert.text == cust_message:
+                if alert.text == "fail" or alert.text == cust_message:
                     return True
             return False
         else:
-            eAlert = self.wd.invisible(By.CLASS_NAME, "toast-body")
-            return True if eAlert else False
+            alert = self.wd.invisible(By.CLASS_NAME, "toast-body")
+            return True if alert else False
 
     def check_indicator_row(
         self,
         available_rows: list[WebElement],
         target_row: list,
     ) -> bool:
         """
```

### Comparing `statesxt-0.5.7/statesxt/base/form.py` & `statesxt-0.5.8/statesxt/base/form.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,14 +44,15 @@
     def insert_to_textbox(
         self,
         element: Union[WebElement, Callable[[], WebElement]],
         input: str,
         byEnter: bool = False,
         onFocus: bool = True,
         sleep: float = None,
+        isInserted: bool = True,
     ) -> None:
         """
         Inserts string into a textbox element
 
         Args:
             element (WebElement): is the input element
             input (str): is the string to be inputted
@@ -59,32 +60,33 @@
             sleep: duration between action
             onFocus: to scroll before inserting
 
         Returns:
             None
         """
 
-        if input or (input == ""):
-            if isinstance(element, Callable):
-                element = element()
-            if onFocus or sleep:
-                self.mkd.scrolling(element, sleep)
-
-            self.ac.click(element).send_keys(Keys.END).key_down(Keys.SHIFT).send_keys(Keys.HOME).key_up(Keys.SHIFT).send_keys(Keys.BACKSPACE).send_keys(input).perform()
-
-            if byEnter:
-                self.ac.send_keys(Keys.ENTER).perform()
-
-            self.ac.reset_actions()
-
-            # for faster approach
-            # textbox_element.click()
-            # textbox_element.clear()
-            # textbox_element.send_keys(input)
-            # textbox_element.send_keys(Keys.ENTER)
+        if isInserted:
+            if input or (input == ""):
+                if isinstance(element, Callable):
+                    element = element()
+                if onFocus or sleep:
+                    self.mkd.scrolling(element, sleep)
+
+                self.ac.click(element).send_keys(Keys.END).key_down(Keys.SHIFT).send_keys(Keys.HOME).key_up(Keys.SHIFT).send_keys(Keys.BACKSPACE).send_keys(input).perform()
+
+                if byEnter:
+                    self.ac.send_keys(Keys.ENTER).perform()
+
+                self.ac.reset_actions()
+
+                # for faster approach
+                # textbox_element.click()
+                # textbox_element.clear()
+                # textbox_element.send_keys(input)
+                # textbox_element.send_keys(Keys.ENTER)
 
     def select_opt_in_dropdown(
         self,
         element: Union[WebElement, Callable[[], WebElement]],
         option,
         method="visible_text",
         onFocus: bool = False,
```

### Comparing `statesxt-0.5.7/statesxt/base/mouse_keys.py` & `statesxt-0.5.8/statesxt/base/mouse_keys.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from selenium.webdriver.common.action_chains import ActionChains
 from selenium.webdriver.remote.webelement import WebElement
 from selenium.webdriver.firefox.webdriver import WebDriver
 from selenium.webdriver.chrome.webdriver import WebDriver
 from selenium.webdriver.edge.webdriver import WebDriver
+from selenium.webdriver.common.keys import Keys
 from typing import Callable
 from typing import Union
 import time as t
 
 
 class MouseKeysDriver:
     """
@@ -16,32 +17,31 @@
     def __init__(self, driver: WebDriver) -> None:
         self.ac = ActionChains(driver)
         self.__driver = driver
 
     def clicking(
         self,
         element: Union[WebElement, Callable[[], WebElement]],
-        isClick: bool = True,
-        useJS: bool = True,
+        isClicked: bool = True,
         onFocus: bool = True,
         sleep: float = None,
         steps: int = None,
         block: str = "center",
+        useJS: bool = False,
     ) -> None:
-        if isClick:
+        if isClicked:
             if isinstance(element, Callable):
                 element = element()
             if onFocus or sleep:
                 self.scrolling(
                     element=element,
                     sleep=sleep,
                     steps=steps,
                     block=block,
                 )
-            # click the element
             (
                 self.__driver.execute_script(
                     "arguments[0].click();",
                     element,
                 )
                 if useJS
                 else element.click()
@@ -124,26 +124,26 @@
                     click_page_number(title="previous page", pns=pns, titles=titles) if (direction == "backward") else click_page_number(title="next page", pns=pns, titles=titles)
                 )
         return False if tobeFound else True
 
     def scrolling(
         self,
         element: Union[WebElement, Callable[[], WebElement]] = None,
-        sleep: float = 0.75,
+        sleep: float = 0.5,
         steps: int = None,
         block: str = "center",
     ) -> None:
         """
         'block', defines vertical alignment.
         - 'start'
         - 'center' (default)
         - 'end'
         - 'nearest'
         """
-        sleep = sleep if sleep else 0.75
+        sleep = sleep if sleep else 0.5
 
         if element:
             if isinstance(element, Callable):
                 element = element()
             if steps:
                 self.ac.scroll_by_amount(0, steps).pause(sleep).perform()
                 self.__driver.execute_script(
@@ -153,16 +153,17 @@
             else:
                 self.__driver.execute_script(
                     "arguments[0].scrollIntoView({block: '" + block + "'});",
                     element,
                 )
                 t.sleep(sleep)
         else:
-            self.ac.scroll_by_amount(0, steps).pause(sleep).perform()
-            self.ac.reset_actions()
+            if steps:
+                self.ac.scroll_by_amount(0, steps).pause(sleep).perform()
+                self.ac.reset_actions()
 
     def zooming(self, zoom_percentage: float, sleep: int = 1) -> None:
         """
         Zooms in and out the screen.
 
         Args:
             - zoom_percentage (float), is the percentage of the screen wanted to be
```

### Comparing `statesxt-0.5.7/statesxt/base/table.py` & `statesxt-0.5.8/statesxt/base/table.py`

 * *Files identical despite different names*

### Comparing `statesxt-0.5.7/statesxt/base/wait.py` & `statesxt-0.5.8/statesxt/base/wait.py`

 * *Files 23% similar despite different names*

```diff
@@ -31,76 +31,86 @@
     Provides explicit wait, i.e. will wait until either the element has found or exceed time limit.
     """
 
     def __init__(self, driver, duration: int) -> None:
         self.init_duration = duration
         self.wdw = WebDriverWait(driver, duration)
 
-    @Wrapper.exception_handling_returns_None
-    def all_elements(self, by: MyBy, locator, cusdur: float = 0, cusfreq: float = 0.5) -> list[WebElement]:
+    def all_elements(self, by: MyBy, locator, staleness_element=None, cusdur: float = 0, cusfreq: float = 0.5) -> list[WebElement]:
         # config
         if cusdur > 0:
             self.wdw._timeout = cusdur
         if cusfreq != 0.5:
             self.wdw._poll = cusfreq
+        # wait for staleness of another element
+        if staleness_element:
+            self.wdw.until(EC.staleness_of(staleness_element))
         # get
         res = self.wdw.until(EC.presence_of_all_elements_located((by, locator)))
         # reset
         self.wdw._timeout = self.init_duration
         self.wdw._poll = 0.5
         return res
 
-    @Wrapper.exception_handling_returns_None
-    def an_element(self, by: MyBy, locator, cusdur: float = 0, cusfreq: float = 0.5) -> WebElement:
+    def an_element(self, by: MyBy, locator, staleness_element=None, cusdur: float = 0, cusfreq: float = 0.5) -> WebElement:
         # config
         if cusdur > 0:
             self.wdw._timeout = cusdur
         if cusfreq != 0.5:
             self.wdw._poll = cusfreq
+        # wait for staleness of another element
+        if staleness_element:
+            self.wdw.until(EC.staleness_of(staleness_element))
         # get
         res = self.wdw.until(EC.presence_of_element_located((by, locator)))
         # reset
         self.wdw._timeout = self.init_duration
         self.wdw._poll = 0.5
         return res
 
-    @Wrapper.exception_handling_returns_None
-    def clickable(self, by: MyBy, locator, cusdur: float = 0, cusfreq: float = 0.5) -> WebElement:
+    def clickable(self, by: MyBy, locator, staleness_element=None, cusdur: float = 0, cusfreq: float = 0.5) -> WebElement:
         # config
         if cusdur > 0:
             self.wdw._timeout = cusdur
         if cusfreq != 0.5:
             self.wdw._poll = cusfreq
+        # wait for staleness of another element
+        if staleness_element:
+            self.wdw.until(EC.staleness_of(staleness_element))
         # get
         res = self.wdw.until(EC.element_to_be_clickable((by, locator)))
         # reset
         self.wdw._timeout = self.init_duration
         self.wdw._poll = 0.5
         return res
 
-    @Wrapper.exception_handling_returns_None
-    def invisible(self, by: MyBy, locator, cusdur: float = 0, cusfreq: float = 0.5) -> bool:
+    def invisible(self, by: MyBy, locator, staleness_element=None, cusdur: float = 0, cusfreq: float = 0.5) -> bool:
         # config
         if cusdur > 0:
             self.wdw._timeout = cusdur
         if cusfreq != 0.5:
             self.wdw._poll = cusfreq
+        # wait for staleness of another element
+        if staleness_element:
+            self.wdw.until(EC.staleness_of(staleness_element))
         # get
         res = self.wdw.until(EC.invisibility_of_element_located((by, locator)))
         # reset
         self.wdw._timeout = self.init_duration
         self.wdw._poll = 0.5
         return res
 
-    @Wrapper.exception_handling_returns_None
-    def visible(self, by: MyBy, locator, cusdur: float = 0, cusfreq: float = 0.5) -> WebElement:
+    def visible(self, by: MyBy, locator, staleness_element=None, cusdur: float = 0, cusfreq: float = 0.5) -> WebElement:
         # config
         if cusdur > 0:
             self.wdw._timeout = cusdur
         if cusfreq != 0.5:
             self.wdw._poll = cusfreq
+        # wait for staleness of another element
+        if staleness_element:
+            self.wdw.until(EC.staleness_of(staleness_element))
         # get
         res = self.wdw.until(EC.visibility_of_element_located((by, locator)))
         # reset
         self.wdw._timeout = self.init_duration
         self.wdw._poll = 0.5
         return res
```

### Comparing `statesxt-0.5.7/statesxt/database/database.py` & `statesxt-0.5.8/statesxt/database/database.py`

 * *Files identical despite different names*

### Comparing `statesxt-0.5.7/statesxt/database/service.py` & `statesxt-0.5.8/statesxt/database/service.py`

 * *Files identical despite different names*

### Comparing `statesxt-0.5.7/statesxt/docs/Makefile` & `statesxt-0.5.8/statesxt/docs/Makefile`

 * *Files identical despite different names*

### Comparing `statesxt-0.5.7/statesxt/docs/_static/images/structure-en.png` & `statesxt-0.5.8/statesxt/docs/_static/images/structure-en.png`

 * *Files identical despite different names*

### Comparing `statesxt-0.5.7/statesxt/docs/_static/images/uml-base.png` & `statesxt-0.5.8/statesxt/docs/_static/images/uml-base.png`

 * *Files identical despite different names*

### Comparing `statesxt-0.5.7/statesxt/docs/_static/images/uml-framework-states.png` & `statesxt-0.5.8/statesxt/docs/_static/images/uml-framework-states.png`

 * *Files identical despite different names*

### Comparing `statesxt-0.5.7/statesxt/docs/_static/images/uml-framework.png` & `statesxt-0.5.8/statesxt/docs/_static/images/uml-framework.png`

 * *Files identical despite different names*

### Comparing `statesxt-0.5.7/statesxt/docs/conf.py` & `statesxt-0.5.8/statesxt/docs/conf.py`

 * *Files identical despite different names*

### Comparing `statesxt-0.5.7/statesxt/docs/contents/README-md.rst` & `statesxt-0.5.8/statesxt/docs/contents/README-md.rst`

 * *Files identical despite different names*

### Comparing `statesxt-0.5.7/statesxt/docs/contents/base.rst` & `statesxt-0.5.8/statesxt/docs/contents/base.rst`

 * *Files identical despite different names*

### Comparing `statesxt-0.5.7/statesxt/docs/contents/env_template.rst` & `statesxt-0.5.8/statesxt/docs/contents/env_template.rst`

 * *Files identical despite different names*

### Comparing `statesxt-0.5.7/statesxt/docs/contents/gitignore.rst` & `statesxt-0.5.8/statesxt/docs/contents/gitignore.rst`

 * *Files identical despite different names*

### Comparing `statesxt-0.5.7/statesxt/docs/contents/introduction.rst` & `statesxt-0.5.8/statesxt/docs/contents/introduction.rst`

 * *Files identical despite different names*

### Comparing `statesxt-0.5.7/statesxt/docs/contents/locators.rst` & `statesxt-0.5.8/statesxt/docs/contents/locators.rst`

 * *Files identical despite different names*

### Comparing `statesxt-0.5.7/statesxt/docs/contents/pages.rst` & `statesxt-0.5.8/statesxt/docs/contents/pages.rst`

 * *Files identical despite different names*

### Comparing `statesxt-0.5.7/statesxt/docs/contents/poetry-lock.rst` & `statesxt-0.5.8/statesxt/docs/contents/poetry-lock.rst`

 * *Files identical despite different names*

### Comparing `statesxt-0.5.7/statesxt/docs/contents/pyproject-toml.rst` & `statesxt-0.5.8/statesxt/docs/contents/pyproject-toml.rst`

 * *Files identical despite different names*

### Comparing `statesxt-0.5.7/statesxt/docs/contents/pytest-ini.rst` & `statesxt-0.5.8/statesxt/docs/contents/pytest-ini.rst`

 * *Files identical despite different names*

### Comparing `statesxt-0.5.7/statesxt/docs/contents/quick_start.rst` & `statesxt-0.5.8/statesxt/docs/contents/quick_start.rst`

 * *Files identical despite different names*

### Comparing `statesxt-0.5.7/statesxt/docs/contents/testcases.rst` & `statesxt-0.5.8/statesxt/docs/contents/testcases.rst`

 * *Files identical despite different names*

### Comparing `statesxt-0.5.7/statesxt/docs/contents/utils.rst` & `statesxt-0.5.8/statesxt/docs/contents/utils.rst`

 * *Files identical despite different names*

### Comparing `statesxt-0.5.7/statesxt/docs/index.rst` & `statesxt-0.5.8/statesxt/docs/index.rst`

 * *Files identical despite different names*

### Comparing `statesxt-0.5.7/statesxt/docs/make.bat` & `statesxt-0.5.8/statesxt/docs/make.bat`

 * *Files identical despite different names*

### Comparing `statesxt-0.5.7/statesxt/docs/requirements.txt` & `statesxt-0.5.8/statesxt/docs/requirements.txt`

 * *Files identical despite different names*

### Comparing `statesxt-0.5.7/statesxt/main.py` & `statesxt-0.5.8/statesxt/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -265,15 +265,15 @@
                 print(f"{self.ansi['error']}A page folder with name {self.obj(page_name_path)} already exists{self.ansi['reset']}")
         else:
             print(f"{self.ansi['error']}{self.name} could not find folder {self.obj(parent_folder)} in {self.obj(self.destdir)}{self.ansi['reset']}")
 
     def cli(self):
         parser = argparse.ArgumentParser(description="Generate Directories")
         parser.add_argument("opt", help="Action to perform: 'generate', 'remove', 'update', and 'create-page'", choices=["generate", "remove", "update", "create-page"])
-        parser.add_argument("-v", "--version", action="version", version="StateSXT 0.5.7")
+        parser.add_argument("-v", "--version", action="version", version="StateSXT 0.5.8")
         args = parser.parse_args()
 
         if str(args.opt).lower() == "generate":
             self.generate()
         elif str(args.opt).lower() == "remove":
             self.remove()
         elif str(args.opt).lower() == "update":
```

### Comparing `statesxt-0.5.7/statesxt/named_ranges.py` & `statesxt-0.5.8/statesxt/named_ranges.py`

 * *Files identical despite different names*

### Comparing `statesxt-0.5.7/statesxt/pyproject.toml` & `statesxt-0.5.8/statesxt/pyproject.toml`

 * *Files identical despite different names*

### Comparing `statesxt-0.5.7/statesxt/restate.py` & `statesxt-0.5.8/statesxt/restate.py`

 * *Files identical despite different names*

### Comparing `statesxt-0.5.7/statesxt/testcases/_fixtures/auth.py` & `statesxt-0.5.8/statesxt/testcases/_fixtures/auth.py`

 * *Files identical despite different names*

### Comparing `statesxt-0.5.7/statesxt/testcases/_fixtures/composition.py` & `statesxt-0.5.8/statesxt/testcases/_fixtures/composition.py`

 * *Files identical despite different names*

### Comparing `statesxt-0.5.7/statesxt/testcases/_fixtures/option.py` & `statesxt-0.5.8/statesxt/testcases/_fixtures/option.py`

 * *Files identical despite different names*

### Comparing `statesxt-0.5.7/statesxt/testcases/_fixtures/param.py` & `statesxt-0.5.8/statesxt/testcases/_fixtures/param.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 
 @pytest.fixture(scope="class")
 def usecase3(request):
     request.cls.usecase = 3
 
 
 @pytest.fixture(scope="class")
-def usecase5(request):
+def usecase4(request):
     request.cls.usecase = 4
 
 
 @pytest.fixture(scope="class")
 def usecase5(request):
     request.cls.usecase = 5
```

### Comparing `statesxt-0.5.7/statesxt/testcases/conftest.py` & `statesxt-0.5.8/statesxt/testcases/conftest.py`

 * *Files identical despite different names*

### Comparing `statesxt-0.5.7/statesxt/utils/email.py` & `statesxt-0.5.8/statesxt/utils/email.py`

 * *Files identical despite different names*

### Comparing `statesxt-0.5.7/statesxt/utils/formatter.py` & `statesxt-0.5.8/statesxt/utils/formatter.py`

 * *Files identical despite different names*

### Comparing `statesxt-0.5.7/statesxt/utils/logger.py` & `statesxt-0.5.8/statesxt/utils/logger.py`

 * *Files identical despite different names*

### Comparing `statesxt-0.5.7/statesxt/utils/response_handler.py` & `statesxt-0.5.8/statesxt/utils/response_handler.py`

 * *Files identical despite different names*

### Comparing `statesxt-0.5.7/statesxt/utils/service_account.py` & `statesxt-0.5.8/statesxt/utils/service_account.py`

 * *Files identical despite different names*

### Comparing `statesxt-0.5.7/statesxt/utils/store.py` & `statesxt-0.5.8/statesxt/utils/store.py`

 * *Files identical despite different names*

### Comparing `statesxt-0.5.7/statesxt/utils/wrapper.py` & `statesxt-0.5.8/statesxt/utils/wrapper.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from functools import wraps
 import logging
 import sys
-
+from selenium.common.exceptions import StaleElementReferenceException
 from .faker import FakerGenerator
+import time as t
 
 
 class Wrapper:
     """Making use functools\wraps"""
 
     @classmethod
     def exception_handling_returns_None(cls, func):
@@ -41,14 +42,30 @@
             except Exception as e:
                 logging.getLogger(f"root.{__name__}.{decoratorClassName}.{decoratorMethodName}").error(f"error:\n{str(e)}")
                 raise Exception(str(e))
 
         return wrapper
 
     @classmethod
+    def stale_handler(func):
+        """
+        forced a function to retry find a missing staled element
+        """
+
+        @wraps(func)
+        def wrapper(*args, **kwargs):
+            try:
+                return func(*args, **kwargs)
+            except StaleElementReferenceException:
+                t.sleep(1.8)
+                return func(*args, **kwargs)
+
+        return wrapper
+
+    @classmethod
     def result_receiving(cls, func):
         """
         to track the result of test cases, so instead of directly raising error, it lets to write down the error first, e.g. email, report, and summary
         """
         decoratorClassName = cls.__name__
         decoratorMethodName = sys._getframe().f_code.co_name
```

### Comparing `statesxt-0.5.7/statesxt.egg-info/PKG-INFO` & `statesxt-0.5.8/statesxt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: statesxt
-Version: 0.5.7
+Version: 0.5.8
 Summary: A project template for testing your website application.
 Home-page: https://test.pypi.org/project/statesxt/
 Author: Jason Caleb
 Author-email: cjsonnnnn@gmail.com
 License: MIT License
 Project-URL: Source, https://github.com/jsonnnnn/statesxt
 Project-URL: Documentation, https://statesxt.readthedocs.io/en/latest/
```

### Comparing `statesxt-0.5.7/statesxt.egg-info/SOURCES.txt` & `statesxt-0.5.8/statesxt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

